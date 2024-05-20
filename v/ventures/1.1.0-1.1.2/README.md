# Comparing `tmp/ventures-1.1.0.tar.gz` & `tmp/ventures-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.1.0.tar", max compression
+gzip compressed data, was "ventures-1.1.2.tar", max compression
```

## Comparing `ventures-1.1.0.tar` & `ventures-1.1.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rwxr-xr-x   0        0        0      540 2024-05-20 03:36:16.958377 ventures-1.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      311 2024-04-23 18:58:19.584376 ventures-1.1.0/readme.md
--rwxr-xr-x   0        0        0     1120 2024-05-18 18:56:41.459616 ventures-1.1.0/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.1.0/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.1.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.1.0/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.1.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.1.0/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.1.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   195780 2024-05-20 03:39:15.480047 ventures-1.1.0/venues/stages/ventures/_status/DB/records.json
--rw-r--r--   0        0        0     1217 2024-05-20 03:37:43.477222 ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1133 2024-05-20 03:37:22.901492 ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0      110 2024-05-20 03:39:13.452072 ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rwxr-xr-x   0        0        0     1283 2024-05-19 23:18:17.298859 ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1428 2024-05-18 02:01:33.088701 ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-20 03:39:14.488059 ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rw-r--r--   0        0        0      964 2024-05-20 01:26:25.762311 ventures-1.1.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      767 2024-05-20 01:26:19.954331 ventures-1.1.0/venues/stages/ventures/_status/monitors/3_task/status_1.py
--rwxr-xr-x   0        0        0       61 2024-05-20 03:39:13.776068 ventures-1.1.0/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
--rw-r--r--   0        0        0     1274 2024-05-20 03:38:46.552411 ventures-1.1.0/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1654 2024-05-20 03:38:38.620512 ventures-1.1.0/venues/stages/ventures/_status/monitors/4_detached/status_1.py
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.1.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.1.0/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
--rw-r--r--   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
--rw-r--r--   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
--rw-r--r--   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
--rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
--rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
--rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/adventure.py
--rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/clique.py
--rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
--rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
--rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
--rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
--rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
--rwxr-xr-x   0        0        0      463 2024-05-18 01:29:56.857560 ventures-1.1.0/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.1.0/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.1.0/venues/stages/ventures/mixer.S.HTML
--rwxr-xr-x   0        0        0     1133 2024-05-18 18:53:30.969670 ventures-1.1.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rw-r--r--   0        0        0     1755 2024-05-20 00:56:07.601346 ventures-1.1.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rw-r--r--   0        0        0     1716 2024-05-20 00:59:57.187843 ventures-1.1.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1200 2024-05-18 18:45:09.731099 ventures-1.1.0/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0     2439 2024-05-20 00:56:04.745365 ventures-1.1.0/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0     2835 2024-05-20 00:59:51.107883 ventures-1.1.0/venues/stages/ventures/plays/turn_on.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.1.0/venues/stages/ventures/plays_venture/is_on.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:56.689210 ventures-1.1.0/venues/stages/ventures/plays_venture/turn_off.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:52.973247 ventures-1.1.0/venues/stages/ventures/plays_venture/turn_on.py
--rwxr-xr-x   0        0        0     1246 2024-05-18 01:05:35.842084 ventures-1.1.0/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.1.0/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0     2190 2024-05-20 03:35:10.195306 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive/__init__.py
--rw-r--r--   0        0        0     1709 2024-05-20 03:35:20.863155 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
--rw-r--r--   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
--rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
--rw-r--r--   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
--rw-r--r--   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.1.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0      486 2024-05-17 22:53:36.062918 ventures-1.1.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.1.0/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      230 2024-05-17 22:53:33.130949 ventures-1.1.0/venues/stages/ventures/utilities/map/scan.py
--rw-r--r--   0        0        0      919 2024-05-20 00:48:43.604121 ventures-1.1.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      676 2024-05-20 00:48:36.716162 ventures-1.1.0/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.1.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rwxr-xr-x   0        0        0      381 2024-05-18 03:46:35.268323 ventures-1.1.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      181 2024-05-18 03:46:08.652619 ventures-1.1.0/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.1.0/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 ventures-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      540 2024-05-20 03:45:07.891902 ventures-1.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0      311 2024-04-23 18:58:19.584376 ventures-1.1.2/readme.md
+-rwxr-xr-x   0        0        0     1120 2024-05-18 18:56:41.459616 ventures-1.1.2/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.1.2/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.1.2/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.1.2/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.1.2/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.1.2/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.1.2/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   197026 2024-05-20 03:44:27.204359 ventures-1.1.2/venues/stages/ventures/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1217 2024-05-20 03:37:43.477222 ventures-1.1.2/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1133 2024-05-20 03:37:22.901492 ventures-1.1.2/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-20 03:44:24.108394 ventures-1.1.2/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1283 2024-05-19 23:18:17.298859 ventures-1.1.2/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1428 2024-05-18 02:01:33.088701 ventures-1.1.2/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-20 03:44:26.144371 ventures-1.1.2/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rwxr-xr-x   0        0        0      964 2024-05-20 01:26:25.762311 ventures-1.1.2/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      767 2024-05-20 01:26:19.954331 ventures-1.1.2/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-20 03:44:24.408390 ventures-1.1.2/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rw-r--r--   0        0        0      409 2024-05-20 03:44:21.936418 ventures-1.1.2/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      288 2024-05-20 03:42:15.521870 ventures-1.1.2/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.1.2/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.1.2/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      463 2024-05-18 01:29:56.857560 ventures-1.1.2/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.1.2/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.1.2/venues/stages/ventures/mixer.S.HTML
+-rwxr-xr-x   0        0        0     1133 2024-05-18 18:53:30.969670 ventures-1.1.2/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1755 2024-05-20 00:56:07.601346 ventures-1.1.2/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1716 2024-05-20 00:59:57.187843 ventures-1.1.2/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1200 2024-05-18 18:45:09.731099 ventures-1.1.2/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0     2439 2024-05-20 00:56:04.745365 ventures-1.1.2/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0     2835 2024-05-20 00:59:51.107883 ventures-1.1.2/venues/stages/ventures/plays/turn_on.py
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.1.2/venues/stages/ventures/plays_venture/is_on.py
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:56.689210 ventures-1.1.2/venues/stages/ventures/plays_venture/turn_off.py
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:52.973247 ventures-1.1.2/venues/stages/ventures/plays_venture/turn_on.py
+-rwxr-xr-x   0        0        0     1377 2024-05-20 03:44:44.816161 ventures-1.1.2/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.1.2/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2190 2024-05-20 03:35:10.195306 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rwxr-xr-x   0        0        0     1709 2024-05-20 03:35:20.863155 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rwxr-xr-x   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.1.2/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      486 2024-05-17 22:53:36.062918 ventures-1.1.2/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.1.2/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      230 2024-05-17 22:53:33.130949 ventures-1.1.2/venues/stages/ventures/utilities/map/scan.py
+-rwxr-xr-x   0        0        0      919 2024-05-20 00:48:43.604121 ventures-1.1.2/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      676 2024-05-20 00:48:36.716162 ventures-1.1.2/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.1.2/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rwxr-xr-x   0        0        0      381 2024-05-18 03:46:35.268323 ventures-1.1.2/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      181 2024-05-18 03:46:08.652619 ventures-1.1.2/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.1.2/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 ventures-1.1.2/PKG-INFO
```

### Comparing `ventures-1.1.0/pyproject.toml` & `ventures-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ventures"
-version = "1.1.0"
+version = "1.1.2"
 description = ""
 authors = []
 readme = "readme.md"
 packages = [
     { include = "ventures", from = "venues/stages" },
 ]
 license = "licensed"
```

### Comparing `ventures-1.1.0/venues/stages/ventures/__init__.py` & `ventures-1.1.2/venues/stages/ventures/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.1.2/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/DB/records.json` & `ventures-1.1.2/venues/stages/ventures/_status/DB/records.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9893617021276595%*

 * *Differences: {"'_default'": "{'47': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [4.899993655271828e-07, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'status_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), OrderedDict([('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('elapsed', [9.329960448667407e-07, "*

 * *               "'seconds']), […]*

```diff
@@ -5595,14 +5595,129 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "47": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.899993655271828e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                9.329960448667407e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_detached/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.14738973799831,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.237549413999659,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.087940819998039,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 0,
+                    "passes": 5
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
         "5": {
             "alarms": [],
             "paths": [],
             "stats": {
                 "checks": {
                     "alarms": 0,
                     "passes": 0
```

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.1.2/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.1.2/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/monitors/3_task/status_1.py` & `ventures-1.1.2/venues/stages/ventures/_status/monitors/3_task/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status.proc.py` & `ventures-1.1.2/venues/stages/ventures/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/clique.py` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py` & `ventures-1.1.2/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/plays/is_on.py` & `ventures-1.1.2/venues/stages/ventures/plays/is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/plays/turn_off.py` & `ventures-1.1.2/venues/stages/ventures/plays/turn_off.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/plays/turn_on.py` & `ventures-1.1.2/venues/stages/ventures/plays/turn_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/readme.md` & `ventures-1.1.2/venues/stages/ventures/readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -40,14 +40,23 @@
 the_map = str (
 	normpath (join (
 		os.getcwd (), 
 		"ventures_map.JSON"
 	))
 )
 
+def turn_on_sanique ():
+	return;
+	
+def turn_off_sanique ():
+	return;
+	
+def check_sanique_is_on ():
+	return;
+
 from ventures import ventures_map
 ventures = ventures_map ({
 	"map": the_map,
 	"ventures": [
 		{
 			"name": "adventure_1",
 			"turn on": {
@@ -60,31 +69,29 @@
 				
 				"Popen": {},
 				
 				"kind": "process_identity"
 			}
 		},
 		{
-			"name": "adventure_2",
+			"name": "adventure_1_sanique",
+			"kind": "task",
 			"turn on": {
-				"adventure": [ 
-					"python3",
-					"-m",
-					"http.server",
-					"8081"
-				],
-				
-				"Popen": {},
-				
-				"kind": "process_identity"
-			}
+				"adventure": turn_on_sanique,
+			},
+			"turn off": turn_off_sanique,
+			"is on": check_sanique_is_on
 		}
 	]
 })
 
 ventures ["turn on"] ()
 
 time.sleep (10)
 
+ventures ["is on"] ()
+
+time.sleep (5)
+
 ventures ["turn off"] ()
 
 ```
```

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive/__init__.py` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py` & `ventures-1.1.2/venues/stages/ventures/utilities/hike_passive_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc` & `ventures-1.1.2/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/process/check_is_on.py` & `ventures-1.1.2/venues/stages/ventures/utilities/process/check_is_on.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.1.2/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.1.2/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.1.0/PKG-INFO` & `ventures-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ventures
-Version: 1.1.0
+Version: 1.1.2
 Summary: 
 License: licensed
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

