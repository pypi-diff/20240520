# Comparing `tmp/ventures-1.0.0.tar.gz` & `tmp/ventures-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventures-1.0.0.tar", max compression
+gzip compressed data, was "ventures-1.1.0.tar", max compression
```

## Comparing `ventures-1.0.0.tar` & `ventures-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,93 @@
--rwxr-xr-x   0        0        0      540 2024-05-18 18:10:18.533173 ventures-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0      311 2024-04-23 18:58:19.584376 ventures-1.0.0/readme.md
--rwxr-xr-x   0        0        0     1123 2024-05-18 03:45:00.445378 ventures-1.0.0/venues/stages/ventures/__init__.py
--rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.0.0/venues/stages/ventures/__itinerary/later.S.HTML
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.0.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.0.0/venues/stages/ventures/_ops/_clique/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.0.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.0.0/venues/stages/ventures/_ops/_clique/group/__init__.py
--rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.0.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   106931 2024-05-18 00:21:57.981594 ventures-1.0.0/venues/stages/ventures/_status/DB/records.json
--rwxr-xr-x   0        0        0     1204 2024-05-17 23:47:23.323002 ventures-1.0.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1073 2024-05-18 02:01:08.136974 ventures-1.0.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
--rwxr-xr-x   0        0        0       97 2024-05-18 00:21:55.845617 ventures-1.0.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
--rwxr-xr-x   0        0        0     1283 2024-05-17 23:45:15.820415 ventures-1.0.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1428 2024-05-18 02:01:33.088701 ventures-1.0.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
--rwxr-xr-x   0        0        0      287 2024-05-18 00:21:55.861617 ventures-1.0.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
--rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.0.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1487 2024-05-17 22:33:48.503784 ventures-1.0.0/venues/stages/ventures/_status/status.proc.py
--rwxr-xr-x   0        0        0      463 2024-05-18 01:29:56.857560 ventures-1.0.0/venues/stages/ventures/clique.py
--rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.0.0/venues/stages/ventures/license.S.HTML
--rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.0.0/venues/stages/ventures/mixer.S.HTML
--rwxr-xr-x   0        0        0     1120 2024-05-18 16:36:38.457346 ventures-1.0.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1595 2024-05-18 17:49:33.851292 ventures-1.0.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1656 2024-05-18 17:49:46.015144 ventures-1.0.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1346 2024-05-18 16:36:36.849371 ventures-1.0.0/venues/stages/ventures/plays/is_on.py
--rwxr-xr-x   0        0        0     2145 2024-05-18 17:49:31.571320 ventures-1.0.0/venues/stages/ventures/plays/turn_off.py
--rwxr-xr-x   0        0        0     2699 2024-05-18 17:49:43.755172 ventures-1.0.0/venues/stages/ventures/plays/turn_on.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.0.0/venues/stages/ventures/plays_venture/is_on.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:56.689210 ventures-1.0.0/venues/stages/ventures/plays_venture/turn_off.py
--rwxr-xr-x   0        0        0        0 2024-05-18 03:03:52.973247 ventures-1.0.0/venues/stages/ventures/plays_venture/turn_on.py
--rwxr-xr-x   0        0        0     1246 2024-05-18 01:05:35.842084 ventures-1.0.0/venues/stages/ventures/readme.md
--rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.0.0/venues/stages/ventures/status_1.py
--rwxr-xr-x   0        0        0      732 2024-05-17 22:33:48.503784 ventures-1.0.0/venues/stages/ventures/utilities/hike_passive/__init__.py
--rwxr-xr-x   0        0        0     1123 2024-05-17 22:47:00.319152 ventures-1.0.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.0.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
--rwxr-xr-x   0        0        0      486 2024-05-17 22:53:36.062918 ventures-1.0.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.0.0/venues/stages/ventures/utilities/map/etch.py
--rwxr-xr-x   0        0        0      230 2024-05-17 22:53:33.130949 ventures-1.0.0/venues/stages/ventures/utilities/map/scan.py
--rwxr-xr-x   0        0        0     2166 2024-04-20 04:40:12.981620 ventures-1.0.0/venues/stages/ventures/utilities/p_expect/__init__.py
--rwxr-xr-x   0        0        0     1997 2024-04-20 04:44:34.600566 ventures-1.0.0/venues/stages/ventures/utilities/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.0.0/venues/stages/ventures/utilities/p_expect/__pycache__/background.cpython-310.pyc
--rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.0.0/venues/stages/ventures/utilities/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.0.0/venues/stages/ventures/utilities/p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.0.0/venues/stages/ventures/utilities/p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.0.0/venues/stages/ventures/utilities/p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.0.0/venues/stages/ventures/utilities/p_expect/parse_records.py
--rwxr-xr-x   0        0        0      604 2024-05-17 23:06:21.818637 ventures-1.0.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
--rwxr-xr-x   0        0        0      374 2024-05-17 23:06:20.270653 ventures-1.0.0/venues/stages/ventures/utilities/process/check_is_on.py
--rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.0.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
--rwxr-xr-x   0        0        0      381 2024-05-18 03:46:35.268323 ventures-1.0.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
--rwxr-xr-x   0        0        0      181 2024-05-18 03:46:08.652619 ventures-1.0.0/venues/stages/ventures/utilities/ventures/find_venture.py
--rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.0.0/venues/stages/ventures/ventures_map.S.HTML
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 ventures-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0      540 2024-05-20 03:36:16.958377 ventures-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0      311 2024-04-23 18:58:19.584376 ventures-1.1.0/readme.md
+-rwxr-xr-x   0        0        0     1120 2024-05-18 18:56:41.459616 ventures-1.1.0/venues/stages/ventures/__init__.py
+-rwxr-xr-x   0        0        0       77 2024-03-23 20:03:57.719484 ventures-1.1.0/venues/stages/ventures/__itinerary/later.S.HTML
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ventures-1.1.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ventures-1.1.0/venues/stages/ventures/_ops/_clique/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.907926 ventures-1.1.0/venues/stages/ventures/_ops/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ventures-1.1.0/venues/stages/ventures/_ops/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0        5 2024-03-23 19:57:06.923925 ventures-1.1.0/venues/stages/ventures/_ops/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0   195780 2024-05-20 03:39:15.480047 ventures-1.1.0/venues/stages/ventures/_status/DB/records.json
+-rw-r--r--   0        0        0     1217 2024-05-20 03:37:43.477222 ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1133 2024-05-20 03:37:22.901492 ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py
+-rwxr-xr-x   0        0        0      110 2024-05-20 03:39:13.452072 ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/ventures_map.JSON
+-rwxr-xr-x   0        0        0     1283 2024-05-19 23:18:17.298859 ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1428 2024-05-18 02:01:33.088701 ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py
+-rwxr-xr-x   0        0        0      287 2024-05-20 03:39:14.488059 ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/ventures_map.JSON
+-rw-r--r--   0        0        0      964 2024-05-20 01:26:25.762311 ventures-1.1.0/venues/stages/ventures/_status/monitors/3_task/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      767 2024-05-20 01:26:19.954331 ventures-1.1.0/venues/stages/ventures/_status/monitors/3_task/status_1.py
+-rwxr-xr-x   0        0        0       61 2024-05-20 03:39:13.776068 ventures-1.1.0/venues/stages/ventures/_status/monitors/3_task/ventures_map.JSON
+-rw-r--r--   0        0        0     1274 2024-05-20 03:38:46.552411 ventures-1.1.0/venues/stages/ventures/_status/monitors/4_detached/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1654 2024-05-20 03:38:38.620512 ventures-1.1.0/venues/stages/ventures/_status/monitors/4_detached/status_1.py
+-rwxr-xr-x   0        0        0     1059 2024-05-17 23:24:21.178569 ventures-1.1.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1552 2024-05-18 18:54:48.340835 ventures-1.1.0/venues/stages/ventures/_status/status.proc.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      696 2024-05-20 01:13:11.931840 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/__pycache__/adventure.cpython-310.pyc
+-rw-r--r--   0        0        0      855 2024-05-20 01:13:12.079840 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/is_on.cpython-310.pyc
+-rw-r--r--   0        0        0     1084 2024-05-20 01:15:40.911816 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/off.cpython-310.pyc
+-rw-r--r--   0        0        0     1485 2024-05-20 01:26:11.102361 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1375 2024-05-17 02:22:56.802361 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1337 2024-05-17 02:19:51.828256 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      726 2024-05-20 01:13:04.363836 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0      971 2024-05-20 01:15:36.191819 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     1599 2024-05-20 01:26:06.062378 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0      465 2024-05-20 01:12:36.835817 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/adventure.py
+-rwxr-xr-x   0        0        0      811 2024-05-17 02:18:12.637274 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/clique.py
+-rwxr-xr-x   0        0        0     1541 2024-05-18 01:56:48.979818 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__init__.py
+-rwxr-xr-x   0        0        0     1306 2024-05-18 01:56:51.707788 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      426 2024-05-17 02:18:12.849271 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__init__.py
+-rwxr-xr-x   0        0        0      728 2024-05-17 02:53:34.348860 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/harbor/sockets_guest/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0     1200 2024-05-09 23:05:53.524538 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/generate_inventory_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      533 2024-05-13 01:14:35.297029 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/__pycache__/retrieve_sanique_URL.cpython-310.pyc
+-rwxr-xr-x   0        0        0      541 2024-05-17 02:18:12.953270 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0      786 2024-05-13 01:08:31.259266 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/check_key/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      298 2024-05-17 02:18:12.969270 ventures-1.1.0/venues/stages/ventures/_status/status_venues/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      463 2024-05-18 01:29:56.857560 ventures-1.1.0/venues/stages/ventures/clique.py
+-rwxr-xr-x   0        0        0      227 2024-03-23 19:57:06.947925 ventures-1.1.0/venues/stages/ventures/license.S.HTML
+-rwxr-xr-x   0        0        0      154 2024-03-23 19:57:06.959925 ventures-1.1.0/venues/stages/ventures/mixer.S.HTML
+-rwxr-xr-x   0        0        0     1133 2024-05-18 18:53:30.969670 ventures-1.1.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc
+-rw-r--r--   0        0        0     1755 2024-05-20 00:56:07.601346 ventures-1.1.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc
+-rw-r--r--   0        0        0     1716 2024-05-20 00:59:57.187843 ventures-1.1.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1200 2024-05-18 18:45:09.731099 ventures-1.1.0/venues/stages/ventures/plays/is_on.py
+-rwxr-xr-x   0        0        0     2439 2024-05-20 00:56:04.745365 ventures-1.1.0/venues/stages/ventures/plays/turn_off.py
+-rwxr-xr-x   0        0        0     2835 2024-05-20 00:59:51.107883 ventures-1.1.0/venues/stages/ventures/plays/turn_on.py
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:48.545292 ventures-1.1.0/venues/stages/ventures/plays_venture/is_on.py
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:56.689210 ventures-1.1.0/venues/stages/ventures/plays_venture/turn_off.py
+-rwxr-xr-x   0        0        0        0 2024-05-18 03:03:52.973247 ventures-1.1.0/venues/stages/ventures/plays_venture/turn_on.py
+-rwxr-xr-x   0        0        0     1246 2024-05-18 01:05:35.842084 ventures-1.1.0/venues/stages/ventures/readme.md
+-rwxr-xr-x   0        0        0       62 2024-05-17 20:48:10.862930 ventures-1.1.0/venues/stages/ventures/status_1.py
+-rwxr-xr-x   0        0        0     2190 2024-05-20 03:35:10.195306 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-20 03:35:20.863155 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2276 2024-05-20 00:26:05.006522 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__init__.py
+-rw-r--r--   0        0        0     1657 2024-05-20 00:26:42.330194 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2184 2024-04-20 04:44:34.604566 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py
+-rwxr-xr-x   0        0        0     2329 2024-05-20 00:04:41.018507 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py
+-rw-r--r--   0        0        0     1857 2024-05-20 00:31:14.064156 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     2200 2024-05-20 00:31:14.064156 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:44:36.648534 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1986 2024-05-20 00:29:35.140705 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/parse_records.py
+-rw-r--r--   0        0        0     1422 2024-05-20 01:32:24.940994 ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_v1/__init__.py
+-rwxr-xr-x   0        0        0      589 2024-05-17 23:32:23.401039 ventures-1.1.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      486 2024-05-17 22:53:36.062918 ventures-1.1.0/venues/stages/ventures/utilities/map/__pycache__/scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      324 2024-05-17 23:32:19.661081 ventures-1.1.0/venues/stages/ventures/utilities/map/etch.py
+-rwxr-xr-x   0        0        0      230 2024-05-17 22:53:33.130949 ventures-1.1.0/venues/stages/ventures/utilities/map/scan.py
+-rw-r--r--   0        0        0      919 2024-05-20 00:48:43.604121 ventures-1.1.0/venues/stages/ventures/utilities/process/__pycache__/check_is_on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      676 2024-05-20 00:48:36.716162 ventures-1.1.0/venues/stages/ventures/utilities/process/check_is_on.py
+-rwxr-xr-x   0        0        0      582 2024-05-18 16:13:45.692580 ventures-1.1.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py
+-rwxr-xr-x   0        0        0      381 2024-05-18 03:46:35.268323 ventures-1.1.0/venues/stages/ventures/utilities/ventures/__pycache__/find_venture.cpython-310.pyc
+-rwxr-xr-x   0        0        0      181 2024-05-18 03:46:08.652619 ventures-1.1.0/venues/stages/ventures/utilities/ventures/find_venture.py
+-rwxr-xr-x   0        0        0      922 2024-05-17 22:33:48.503784 ventures-1.1.0/venues/stages/ventures/ventures_map.S.HTML
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 ventures-1.1.0/PKG-INFO
```

### Comparing `ventures-1.0.0/pyproject.toml` & `ventures-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ventures"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = []
 readme = "readme.md"
 packages = [
     { include = "ventures", from = "venues/stages" },
 ]
 license = "licensed"
```

### Comparing `ventures-1.0.0/venues/stages/ventures/__init__.py` & `ventures-1.1.0/venues/stages/ventures/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 		ventures_map_bracket = turn_on ({
 			"ventures": ventures,
 			"map": the_map
 		})
 		
 		#rich.print_json (data = ventures_map_bracket);
 		
-		
 		status = is_on ({
 			"ventures": ventures,
 			"the_map": the_map
 		});
 
 	def is_on_move ():
 		status = is_on ({
```

### Comparing `ventures-1.0.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html` & `ventures-1.1.0/venues/stages/ventures/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/_status/DB/records.json` & `ventures-1.1.0/venues/stages/ventures/_status/DB/records.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8152173913043479%*

 * *Differences: {"'_default'": "{'30': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [4.579997039400041e-07, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'status_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))]), OrderedDict([('checks', "*

 * *               '[OrderedDict([(\'check\', \'check 1\'), (\'exception\', "Exception(\'After 10 '*

 * *               'loops, […]*

```diff
@@ -2586,28 +2586,3023 @@
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "30": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 86, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9080): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x781a6d8e2230>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x781a6d8e2230>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9080): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x781a6d8e2230>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 56, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 519, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9080): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x781a6d8e2230>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task_and_process/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 52, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.579997039400041e-07,
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
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 86, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(MaxRetryError(\"HTTPConnectionPool(host='0.0.0.0', port=9080): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x781a6d8e2230>: Failed to establish a new connection: [Errno 111] Connection refused'))\"))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 198, in _new_conn",
+                                "    sock = connection.create_connection(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 85, in create_connection",
+                                "    raise err",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/connection.py\", line 73, in create_connection",
+                                "    sock.connect(sa)",
+                                "ConnectionRefusedError: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 496, in _make_request",
+                                "    conn.request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 400, in request",
+                                "    self.endheaders()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1278, in endheaders",
+                                "    self._send_output(message_body, encode_chunked=encode_chunked)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1038, in _send_output",
+                                "    self.send(msg)",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 976, in send",
+                                "    self.connect()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 238, in connect",
+                                "    self.sock = self._new_conn()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 213, in _new_conn",
+                                "    raise NewConnectionError(",
+                                "urllib3.exceptions.NewConnectionError: <urllib3.connection.HTTPConnection object at 0x781a6d8e2230>: Failed to establish a new connection: [Errno 111] Connection refused",
+                                "",
+                                "The above exception was the direct cause of the following exception:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 515, in increment",
+                                "    raise MaxRetryError(_pool, url, reason) from reason  # type: ignore[arg-type]",
+                                "urllib3.exceptions.MaxRetryError: HTTPConnectionPool(host='0.0.0.0', port=9080): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x781a6d8e2230>: Failed to establish a new connection: [Errno 111] Connection refused'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 56, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 519, in send",
+                                "    raise ConnectionError(e, request=request)",
+                                "requests.exceptions.ConnectionError: HTTPConnectionPool(host='0.0.0.0', port=9080): Max retries exceeded with url: / (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x781a6d8e2230>: Failed to establish a new connection: [Errno 111] Connection refused'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task_and_process/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 52, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 3,
+                    "passes": 1
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "31": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 86, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 60, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task_and_process/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 52, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.180001269560307e-07,
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
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 86, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 60, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task_and_process/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 52, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 3,
+                    "passes": 1
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "32": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 86, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, python_http did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 60, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, python_http did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task_and_process/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, 1_1_venture_python3_http did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 52, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, 1_1_venture_python3_http did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                9.81999619398266e-07,
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
+                            "exception": "Exception('After 10 loops, adventure_1 did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 86, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1 did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, python_http did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 60, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, python_http did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task_and_process/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, 1_1_venture_python3_http did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 52, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 72, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, 1_1_venture_python3_http did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 3,
+                    "passes": 1
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "33": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "KeyError('process_identity')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 60, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 53, in turn_off",
+                                "    \"is on\": check_is_on (adventure [\"process_identity\"])",
+                                "KeyError: 'process_identity'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task_and_process/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.550006557721645e-07,
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
+                                2.1278499360014393,
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
+                            "exception": "KeyError('process_identity')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 60, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 53, in turn_off",
+                                "    \"is on\": check_is_on (adventure [\"process_identity\"])",
+                                "KeyError: 'process_identity'"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task_and_process/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.1034752080013277,
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
+                    "alarms": 1,
+                    "passes": 3
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "34": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "Exception('After 10 loops, adventure_1_sanique did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 60, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 114, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1_sanique did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/3_task_and_process/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.070011633913964e-07,
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
+                                1.14185902600002,
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
+                            "exception": "Exception('After 10 loops, adventure_1_sanique did not turn off.')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/3_task_and_process/status_1.py\", line 60, in check_1",
+                                "    ventures [\"turn off\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 67, in turn_off_move",
+                                "    turn_off ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_off.py\", line 114, in turn_off",
+                                "    raise Exception (",
+                                "Exception: After 10 loops, adventure_1_sanique did not turn off."
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_task_and_process/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.0902313900005538,
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
+                    "alarms": 1,
+                    "passes": 3
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "35": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.230017556343228e-07,
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
+                                4.1669214550020115,
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
+                                2.2787210659989796,
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
+                                1.1117348879997735,
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
+                    "passes": 4
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "36": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'sys' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 46, in turn_on_move",
+                                "    ventures_map_bracket = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 76, in turn_on",
+                                "    process = hike_passive ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 98, in hike_passive",
+                                "    detached_process_pid = start_detached_process ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 86, in start_detached_process",
+                                "    daemonize()",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 51, in daemonize",
+                                "    sys.exit(0)",
+                                "NameError: name 'sys' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'sys' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 46, in turn_on_move",
+                                "    ventures_map_bracket = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 76, in turn_on",
+                                "    process = hike_passive ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 98, in hike_passive",
+                                "    detached_process_pid = start_detached_process ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 86, in start_detached_process",
+                                "    daemonize()",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 60, in daemonize",
+                                "    sys.exit(0)",
+                                "NameError: name 'sys' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.100009730085731e-07,
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
+                                0.0003806060012720991,
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
+                            "exception": "NameError(\"name 'sys' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 46, in turn_on_move",
+                                "    ventures_map_bracket = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 76, in turn_on",
+                                "    process = hike_passive ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 98, in hike_passive",
+                                "    detached_process_pid = start_detached_process ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 86, in start_detached_process",
+                                "    daemonize()",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 51, in daemonize",
+                                "    sys.exit(0)",
+                                "NameError: name 'sys' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.230814417001966,
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
+                            "exception": "NameError(\"name 'sys' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 46, in turn_on_move",
+                                "    ventures_map_bracket = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 76, in turn_on",
+                                "    process = hike_passive ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 98, in hike_passive",
+                                "    detached_process_pid = start_detached_process ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 86, in start_detached_process",
+                                "    daemonize()",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 60, in daemonize",
+                                "    sys.exit(0)",
+                                "NameError: name 'sys' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 2,
+                    "passes": 3
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "37": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'the_process' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 46, in turn_on_move",
+                                "    ventures_map_bracket = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 76, in turn_on",
+                                "    process = hike_passive ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 106, in hike_passive",
+                                "    \"process_identity\": the_process.pid",
+                                "NameError: name 'the_process' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "NameError(\"name 'the_process' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 46, in turn_on_move",
+                                "    ventures_map_bracket = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 76, in turn_on",
+                                "    process = hike_passive ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 106, in hike_passive",
+                                "    \"process_identity\": the_process.pid",
+                                "NameError: name 'the_process' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.85999873187393e-07,
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
+                                0.00031344700255431235,
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
+                            "exception": "NameError(\"name 'the_process' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 73, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 46, in turn_on_move",
+                                "    ventures_map_bracket = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 76, in turn_on",
+                                "    process = hike_passive ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 106, in hike_passive",
+                                "    \"process_identity\": the_process.pid",
+                                "NameError: name 'the_process' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.2390268060007656,
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
+                            "exception": "NameError(\"name 'the_process' is not defined\")",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 46, in check_1",
+                                "    ventures [\"turn on\"] ()",
+                                "  File \"/habitat/venues/stages/ventures/__init__.py\", line 46, in turn_on_move",
+                                "    ventures_map_bracket = turn_on ({",
+                                "  File \"/habitat/venues/stages/ventures/plays/turn_on.py\", line 76, in turn_on",
+                                "    process = hike_passive ({",
+                                "  File \"/habitat/venues/stages/ventures/utilities/hike_passive/__init__.py\", line 106, in hike_passive",
+                                "    \"process_identity\": the_process.pid",
+                                "NameError: name 'the_process' is not defined"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 2,
+                    "passes": 3
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "38": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.410009518731385e-07,
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
+                                0.00041790799878071994,
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
+                                1.1756437819967687,
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
+                                2.255928471997322,
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
+                                1.1097982049977873,
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
+        "39": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response')))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "http.client.RemoteDisconnected: Remote end closed connection without response",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 470, in increment",
+                                "    raise reraise(type(error), error, _stacktrace)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/util.py\", line 38, in reraise",
+                                "    raise value.with_traceback(tb)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 77, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 501, in send",
+                                "    raise ConnectionError(err, request=request)",
+                                "requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response')))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "http.client.RemoteDisconnected: Remote end closed connection without response",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 470, in increment",
+                                "    raise reraise(type(error), error, _stacktrace)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/util.py\", line 38, in reraise",
+                                "    raise value.with_traceback(tb)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 49, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:8080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 501, in send",
+                                "    raise ConnectionError(err, request=request)",
+                                "requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.660040187649429e-07,
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
+                                0.0004980699959560297,
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
+                            "exception": "ConnectionError(ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response')))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "http.client.RemoteDisconnected: Remote end closed connection without response",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 470, in increment",
+                                "    raise reraise(type(error), error, _stacktrace)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/util.py\", line 38, in reraise",
+                                "    raise value.with_traceback(tb)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 77, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 501, in send",
+                                "    raise ConnectionError(err, request=request)",
+                                "requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.2652692300034687,
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
+                            "exception": "ConnectionError(ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response')))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "http.client.RemoteDisconnected: Remote end closed connection without response",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 470, in increment",
+                                "    raise reraise(type(error), error, _stacktrace)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/util.py\", line 38, in reraise",
+                                "    raise value.with_traceback(tb)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 49, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:8080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 501, in send",
+                                "    raise ConnectionError(err, request=request)",
+                                "requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 2,
+                    "passes": 3
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
         "4": {
             "alarms": [],
             "paths": [],
             "stats": {
                 "checks": {
                     "alarms": 0,
                     "passes": 0
                 },
                 "paths": {
                     "alarms": 0,
                     "empty": 0
                 }
             }
         },
+        "40": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.72000930737704e-07,
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
+                                0.0005374879983719438,
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
+                                1.1551003220010898,
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
+                                2.2731085710038315,
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
+                                1.1234774829936214,
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
+        "41": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response')))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "http.client.RemoteDisconnected: Remote end closed connection without response",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 470, in increment",
+                                "    raise reraise(type(error), error, _stacktrace)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/util.py\", line 38, in reraise",
+                                "    raise value.with_traceback(tb)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 77, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 501, in send",
+                                "    raise ConnectionError(err, request=request)",
+                                "requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/2_3_ventures/status_1.py"
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "ConnectionError(ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response')))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "http.client.RemoteDisconnected: Remote end closed connection without response",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 470, in increment",
+                                "    raise reraise(type(error), error, _stacktrace)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/util.py\", line 38, in reraise",
+                                "    raise value.with_traceback(tb)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 49, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:8080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 501, in send",
+                                "    raise ConnectionError(err, request=request)",
+                                "requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.0320000001229346e-06,
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
+                                0.0005513560026884079,
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
+                            "exception": "ConnectionError(ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response')))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "http.client.RemoteDisconnected: Remote end closed connection without response",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 470, in increment",
+                                "    raise reraise(type(error), error, _stacktrace)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/util.py\", line 38, in reraise",
+                                "    raise value.with_traceback(tb)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py\", line 77, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:9080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 501, in send",
+                                "    raise ConnectionError(err, request=request)",
+                                "requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2_3_ventures/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.280709737999132,
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
+                            "exception": "ConnectionError(ProtocolError('Connection aborted.', RemoteDisconnected('Remote end closed connection without response')))",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "http.client.RemoteDisconnected: Remote end closed connection without response",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 486, in send",
+                                "    resp = conn.urlopen(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 847, in urlopen",
+                                "    retries = retries.increment(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/retry.py\", line 470, in increment",
+                                "    raise reraise(type(error), error, _stacktrace)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/util/util.py\", line 38, in reraise",
+                                "    raise value.with_traceback(tb)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 793, in urlopen",
+                                "    response = self._make_request(",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py\", line 537, in _make_request",
+                                "    response = conn.getresponse()",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/urllib3/connection.py\", line 466, in getresponse",
+                                "    httplib_response = super().getresponse()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 1375, in getresponse",
+                                "    response.begin()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 318, in begin",
+                                "    version, status, reason = self._read_status()",
+                                "  File \"/usr/lib/python3.10/http/client.py\", line 287, in _read_status",
+                                "    raise RemoteDisconnected(\"Remote end closed connection without\"",
+                                "urllib3.exceptions.ProtocolError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))",
+                                "",
+                                "During handling of the above exception, another exception occurred:",
+                                "",
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 49, in check_1",
+                                "    response = requests.get(\"http://0.0.0.0:8080\")",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 73, in get",
+                                "    return request(\"get\", url, params=params, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/api.py\", line 59, in request",
+                                "    return session.request(method=method, url=url, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 589, in request",
+                                "    resp = self.send(prep, **send_kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/sessions.py\", line 703, in send",
+                                "    r = adapter.send(request, **kwargs)",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/requests/adapters.py\", line 501, in send",
+                                "    raise ConnectionError(err, request=request)",
+                                "requests.exceptions.ConnectionError: ('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 2,
+                    "passes": 3
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "42": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 61, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.459966582246125e-07,
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
+                                0.00041078000504057854,
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
+                                4.153507388997241,
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
+                                2.3337952450019657,
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
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 61, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 1,
+                    "passes": 4
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "43": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/1_1_venture/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.199996616691351e-07,
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
+                                0.0004921479994663969,
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
+                                4.141855159999977,
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
+                                2.2755246689994237,
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
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/habitat/.venv/lib/python3.10/site-packages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py\", line 56, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/habitat/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py\", line 76, in check_1",
+                                "    assert (connection_exception == \"yes\")",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1_1_venture/status_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "checks": {
+                    "alarms": 1,
+                    "passes": 4
+                },
+                "paths": {
+                    "alarms": 0,
+                    "empty": 0
+                }
+            }
+        },
+        "44": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.0060030035674572e-06,
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
+                                0.00034812199737643823,
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
+                                3.122727276997466,
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
+                                2.247845573001541,
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
+                                2.1136106600024505,
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
+        "45": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                5.949987098574638e-07,
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
+                                0.000709092004399281,
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
+                                4.132691959006479,
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
+                                2.256639263003308,
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
+                                2.108515059000638,
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
+        "46": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                7.609996828250587e-07,
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
+                                0.0004954350006300956,
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
+                                3.1405070390028413,
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
+                                2.267292552998697,
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
+                                3.08708655800001,
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

### Comparing `ventures-1.0.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 17 23:47:17 2024 UTC, .py size: 1073 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 85ec 4766 3104 0000  o.........Gf1...
+00000000: 6f0d 0d0a 0000 0000 72c5 4a66 6d04 0000  o.......r.Jfm...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6403 6c0a  m.Z.m.Z...d.d.l.
 00000070: 5a0a 6401 6403 6c0b 5a0b 6405 6406 8400  Z.d.d.l.Z.d.d...
@@ -13,64 +13,65 @@
 000000c0: 0000 2901 da0c 7665 6e74 7572 6573 5f6d  ..)...ventures_m
 000000d0: 6170 4e29 03da 0764 6972 6e61 6d65 da04  apN)...dirname..
 000000e0: 6a6f 696e da08 6e6f 726d 7061 7468 6300  join..normpathc.
 000000f0: 0000 0000 0000 0000 0000 0005 0000 0008  ................
 00000100: 0000 0043 0000 0073 cc00 0000 7400 a001  ...C...s....t...
 00000110: 7402 a101 6a03 a004 a100 7d00 7405 7406  t...j.....}.t.t.
 00000120: 7407 7c00 6401 8302 8301 8301 7d01 7408  t.|.d.......}.t.
-00000130: 6402 7c01 8302 0100 7409 7c01 6403 6700  d.|.....t.|.d.g.
-00000140: 6404 a201 6900 6405 6406 9c03 6407 9c02  d...i.d.d...d...
+00000130: 6402 7c01 8302 0100 7409 7c01 6403 6404  d.|.....t.|.d.d.
+00000140: 6700 6405 a201 6900 6406 9c02 6407 9c03  g.d...i.d...d...
 00000150: 6701 6408 9c02 8301 7d02 7c02 6409 1900  g.d.....}.|.d...
 00000160: 8300 0100 740a a00b 640a a101 0100 740c  ....t...d.....t.
 00000170: a00d 640b a101 7d03 7c03 6a0e 640c 6b02  ..d...}.|.j.d.k.
 00000180: 733d 4a00 8201 7c02 640d 1900 8300 0100  s=J...|.d.......
 00000190: 740a a00b 640a a101 0100 640e 7d04 7a07  t...d.....d.}.z.
 000001a0: 740c a00d 640b a101 7d03 5700 6e0d 0400  t...d...}.W.n...
 000001b0: 740c 6a0f 6a10 795d 0100 0100 0100 640f  t.j.j.y]......d.
 000001c0: 7d04 5900 6e01 7700 7c04 640f 6b02 7364  }.Y.n.w.|.d.k.sd
 000001d0: 4a00 8201 6400 5300 2910 4e7a 1176 656e  J...d.S.).Nz.ven
 000001e0: 7475 7265 735f 6d61 702e 4a53 4f4e 7a08  tures_map.JSONz.
-000001f0: 7468 655f 6d61 703a da0b 6164 7665 6e74  the_map:..advent
-00000200: 7572 655f 3129 04da 0770 7974 686f 6e33  ure_1)...python3
-00000210: 7a02 2d6d 7a0b 6874 7470 2e73 6572 7665  z.-mz.http.serve
-00000220: 72da 0438 3038 30da 1070 726f 6365 7373  r..8080..process
-00000230: 5f69 6465 6e74 6974 7929 03da 0961 6476  _identity)...adv
-00000240: 656e 7475 7265 da05 506f 7065 6eda 046b  enture..Popen..k
-00000250: 696e 6429 02da 046e 616d 65fa 0774 7572  ind)...name..tur
-00000260: 6e20 6f6e 2902 da03 6d61 70da 0876 656e  n on)...map..ven
-00000270: 7475 7265 7372 0e00 0000 e901 0000 007a  turesr.........z
-00000280: 1368 7474 703a 2f2f 302e 302e 302e 303a  .http://0.0.0.0:
-00000290: 3830 3830 e9c8 0000 007a 0874 7572 6e20  8080.....z.turn 
-000002a0: 6f66 66da 026e 6fda 0379 6573 2911 da07  off..no..yes)...
-000002b0: 7061 7468 6c69 62da 0450 6174 68da 085f  pathlib..Path.._
-000002c0: 5f66 696c 655f 5fda 0670 6172 656e 74da  _file__..parent.
-000002d0: 0772 6573 6f6c 7665 da03 7374 7272 0500  .resolve..strr..
-000002e0: 0000 7204 0000 00da 0570 7269 6e74 7202  ..r......printr.
-000002f0: 0000 00da 0474 696d 65da 0573 6c65 6570  .....time..sleep
-00000300: da08 7265 7175 6573 7473 da03 6765 74da  ..requests..get.
-00000310: 0b73 7461 7475 735f 636f 6465 da0a 6578  .status_code..ex
-00000320: 6365 7074 696f 6e73 da0f 436f 6e6e 6563  ceptions..Connec
-00000330: 7469 6f6e 4572 726f 7229 05da 0b74 6869  tionError)...thi
-00000340: 735f 666f 6c64 6572 da07 7468 655f 6d61  s_folder..the_ma
-00000350: 7072 1000 0000 da08 7265 7370 6f6e 7365  pr......response
-00000360: da14 636f 6e6e 6563 7469 6f6e 5f65 7863  ..connection_exc
-00000370: 6570 7469 6f6e a900 7227 0000 00fa 482f  eption..r'....H/
-00000380: 6861 6269 7461 742f 7665 6e75 6573 2f73  habitat/venues/s
-00000390: 7461 6765 732f 7665 6e74 7572 6573 2f5f  tages/ventures/_
-000003a0: 7374 6174 7573 2f6d 6f6e 6974 6f72 732f  status/monitors/
-000003b0: 315f 315f 7665 6e74 7572 652f 7374 6174  1_1_venture/stat
-000003c0: 7573 5f31 2e70 79da 0763 6865 636b 5f31  us_1.py..check_1
-000003d0: 1000 0000 733e 0000 0010 0102 0104 0102  ....s>..........
-000003e0: 0102 0104 fe04 ff0a 0702 0202 0102 0306  ................
-000003f0: 0202 0602 0104 f804 fe02 ff08 fe0a 130a  ................
-00000400: 020a 010e 010a 020a 0204 0102 010e 0110  ................
-00000410: 0108 0102 ff10 0372 2900 0000 7a07 6368  .......r)...z.ch
-00000420: 6563 6b20 3129 0eda 075f 5f64 6f63 5f5f  eck 1)...__doc__
-00000430: 7210 0000 0072 0200 0000 721e 0000 00da  r....r....r.....
-00000440: 026f 7372 1500 0000 da07 6f73 2e70 6174  .osr......os.pat
-00000450: 6872 0300 0000 7204 0000 0072 0500 0000  hr....r....r....
-00000460: da03 7379 7372 1c00 0000 7229 0000 00da  ..sysr....r)....
-00000470: 0663 6865 636b 7372 2700 0000 7227 0000  .checksr'...r'..
-00000480: 0072 2700 0000 7228 0000 00da 083c 6d6f  .r'...r(.....<mo
-00000490: 6475 6c65 3e01 0000 0073 1600 0000 0401  dule>....s......
-000004a0: 0c04 0802 0802 0801 1401 0801 0801 0802  ................
-000004b0: 0430 08ff                                .0..
+000001f0: 7468 655f 6d61 703a da18 315f 315f 7665  the_map:..1_1_ve
+00000200: 6e74 7572 655f 7079 7468 6f6e 335f 6874  nture_python3_ht
+00000210: 7470 da10 7072 6f63 6573 735f 6964 656e  tp..process_iden
+00000220: 7469 7479 2904 da07 7079 7468 6f6e 337a  tity)...python3z
+00000230: 022d 6d7a 0b68 7474 702e 7365 7276 6572  .-mz.http.server
+00000240: da04 3830 3830 2902 da09 6164 7665 6e74  ..8080)...advent
+00000250: 7572 65da 0550 6f70 656e 2903 da04 6e61  ure..Popen)...na
+00000260: 6d65 da04 6b69 6e64 fa07 7475 726e 206f  me..kind..turn o
+00000270: 6e29 02da 036d 6170 da08 7665 6e74 7572  n)...map..ventur
+00000280: 6573 720e 0000 00e9 0100 0000 7a13 6874  esr.........z.ht
+00000290: 7470 3a2f 2f30 2e30 2e30 2e30 3a38 3038  tp://0.0.0.0:808
+000002a0: 30e9 c800 0000 7a08 7475 726e 206f 6666  0.....z.turn off
+000002b0: da02 6e6f da03 7965 7329 11da 0770 6174  ..no..yes)...pat
+000002c0: 686c 6962 da04 5061 7468 da08 5f5f 6669  hlib..Path..__fi
+000002d0: 6c65 5f5f da06 7061 7265 6e74 da07 7265  le__..parent..re
+000002e0: 736f 6c76 65da 0373 7472 7205 0000 0072  solve..strr....r
+000002f0: 0400 0000 da05 7072 696e 7472 0200 0000  ......printr....
+00000300: da04 7469 6d65 da05 736c 6565 70da 0872  ..time..sleep..r
+00000310: 6571 7565 7374 73da 0367 6574 da0b 7374  equests..get..st
+00000320: 6174 7573 5f63 6f64 65da 0a65 7863 6570  atus_code..excep
+00000330: 7469 6f6e 73da 0f43 6f6e 6e65 6374 696f  tions..Connectio
+00000340: 6e45 7272 6f72 2905 da0b 7468 6973 5f66  nError)...this_f
+00000350: 6f6c 6465 72da 0774 6865 5f6d 6170 7210  older..the_mapr.
+00000360: 0000 00da 0872 6573 706f 6e73 65da 1463  .....response..c
+00000370: 6f6e 6e65 6374 696f 6e5f 6578 6365 7074  onnection_except
+00000380: 696f 6ea9 0072 2700 0000 fa48 2f68 6162  ion..r'....H/hab
+00000390: 6974 6174 2f76 656e 7565 732f 7374 6167  itat/venues/stag
+000003a0: 6573 2f76 656e 7475 7265 732f 5f73 7461  es/ventures/_sta
+000003b0: 7475 732f 6d6f 6e69 746f 7273 2f31 5f31  tus/monitors/1_1
+000003c0: 5f76 656e 7475 7265 2f73 7461 7475 735f  _venture/status_
+000003d0: 312e 7079 da07 6368 6563 6b5f 3110 0000  1.py..check_1...
+000003e0: 0073 3e00 0000 1001 0201 0401 0201 0201  .s>.............
+000003f0: 04fe 04ff 0a07 0202 0201 0203 0201 0602  ................
+00000400: 0206 04f9 04fd 02ff 08fe 0a13 0a07 0a01  ................
+00000410: 0e01 0a07 0a07 0401 0201 0e01 1001 0801  ................
+00000420: 02ff 1003 7229 0000 007a 0763 6865 636b  ....r)...z.check
+00000430: 2031 290e da07 5f5f 646f 635f 5f72 1000   1)...__doc__r..
+00000440: 0000 7202 0000 0072 1e00 0000 da02 6f73  ..r....r......os
+00000450: 7215 0000 00da 076f 732e 7061 7468 7203  r......os.pathr.
+00000460: 0000 0072 0400 0000 7205 0000 00da 0373  ...r....r......s
+00000470: 7973 721c 0000 0072 2900 0000 da06 6368  ysr....r).....ch
+00000480: 6563 6b73 7227 0000 0072 2700 0000 7227  ecksr'...r'...r'
+00000490: 0000 0072 2800 0000 da08 3c6d 6f64 756c  ...r(.....<modul
+000004a0: 653e 0100 0000 7316 0000 0004 010c 0408  e>....s.........
+000004b0: 0208 0208 0114 0108 0108 0108 0204 4108  ..............A.
+000004c0: ff                                       .
```

### Comparing `ventures-1.0.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py` & `ventures-1.1.0/venues/stages/ventures/_status/monitors/1_1_venture/status_1.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,42 +24,59 @@
 	
 	print ("the_map:", the_map)
 	
 	ventures = ventures_map ({
 		"map": the_map,
 		"ventures": [
 			{
-				"name": "adventure_1",
+				"name": "1_1_venture_python3_http",
 				"kind": "process_identity",
 				"turn on": {
 					"adventure": [ 
 						"python3",
 						"-m",
 						"http.server",
 						"8080"
 					],
 					"Popen": {},
 				}
-			}
+			},
 		]
 	})
 	
 	ventures ["turn on"] ()
 	
+	#
+	#
+	#
+	#
+	
 	time.sleep (1)
-	response = requests.get("http://0.0.0.0:8080")
+	response = requests.get ("http://0.0.0.0:8080")
 	assert (response.status_code == 200)
 
+	#
+	#
+	#
+	#
+
 	ventures ["turn off"] ()
 	
+	#
+	#
+	#
+	#
+	
 	time.sleep (1)
 	connection_exception = "no"
 	try:
 		response = requests.get ("http://0.0.0.0:8080")
 	except requests.exceptions.ConnectionError:
 		connection_exception = "yes"
 		
 	assert (connection_exception == "yes")
 	
+	
+	
 checks = {
 	'check 1': check_1
 }
```

### Comparing `ventures-1.0.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/__pycache__/status_1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 17 23:35:15 2024 UTC, .py size: 1423 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b3e9 4766 8f05 0000  o.........Gf....
+00000000: 6f0d 0d0a 0000 0000 fd0b 4866 9405 0000  o.........Hf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6403 6c0a  m.Z.m.Z...d.d.l.
 00000070: 5a0a 6401 6403 6c0b 5a0b 6405 6406 8400  Z.d.d.l.Z.d.d...
@@ -13,38 +13,38 @@
 000000c0: 6573 5f6d 6170 4e29 03da 0764 6972 6e61  es_mapN)...dirna
 000000d0: 6d65 da04 6a6f 696e da08 6e6f 726d 7061  me..join..normpa
 000000e0: 7468 6300 0000 0000 0000 0000 0000 0004  thc.............
 000000f0: 0000 0009 0000 0043 0000 0073 e000 0000  .......C...s....
 00000100: 7400 a001 7402 a101 6a03 a004 a100 7d00  t...t...j.....}.
 00000110: 7405 7406 7407 7c00 6401 8302 8301 8301  t.t.t.|.d.......
 00000120: 7d01 7408 6402 7c01 8302 0100 7409 7c01  }.t.d.|.....t.|.
-00000130: 6403 6700 6404 a201 6900 6405 6406 9c03  d.g.d...i.d.d...
-00000140: 6407 9c02 6408 6700 6409 a201 6900 6405  d...d.g.d...i.d.
-00000150: 6406 9c03 6407 9c02 640a 6700 640b a201  d...d...d.g.d...
-00000160: 6900 6405 6406 9c03 6407 9c02 6703 640c  i.d.d...d...g.d.
+00000130: 6403 6404 6700 6405 a201 6900 6406 9c02  d.d.g.d...i.d...
+00000140: 6407 9c03 6408 6404 6700 6409 a201 6900  d...d.d.g.d...i.
+00000150: 6406 9c02 6407 9c03 640a 6404 6700 640b  d...d...d.d.g.d.
+00000160: a201 6900 6406 9c02 6407 9c03 6703 640c  ..i.d...d...g.d.
 00000170: 9c02 8301 7d02 7c02 640d 1900 8300 0100  ....}.|.d.......
 00000180: 740a a00b 640e a101 0100 740c a00d 640f  t...d.....t...d.
 00000190: a101 7d03 7c03 6a0e 6410 6b02 7351 4a00  ..}.|.j.d.k.sQJ.
 000001a0: 8201 740c a00d 6411 a101 7d03 7c03 6a0e  ..t...d...}.|.j.
 000001b0: 6410 6b02 735d 4a00 8201 740c a00d 6412  d.k.s]J...t...d.
 000001c0: a101 7d03 7c03 6a0e 6410 6b02 7369 4a00  ..}.|.j.d.k.siJ.
 000001d0: 8201 7c02 6413 1900 8300 0100 6400 5300  ..|.d.......d.S.
 000001e0: 2914 4e7a 1176 656e 7475 7265 735f 6d61  ).Nz.ventures_ma
 000001f0: 702e 4a53 4f4e 7a08 7468 655f 6d61 703a  p.JSONz.the_map:
-00000200: da0b 6164 7665 6e74 7572 655f 3129 04da  ..adventure_1)..
-00000210: 0770 7974 686f 6e33 fa02 2d6d fa0b 6874  .python3..-m..ht
-00000220: 7470 2e73 6572 7665 72da 0439 3038 30da  tp.server..9080.
-00000230: 1070 726f 6365 7373 5f69 6465 6e74 6974  .process_identit
-00000240: 7929 03da 0961 6476 656e 7475 7265 da05  y)...adventure..
-00000250: 506f 7065 6eda 046b 696e 6429 02da 046e  Popen..kind)...n
-00000260: 616d 65fa 0774 7572 6e20 6f6e da0b 6164  ame..turn on..ad
-00000270: 7665 6e74 7572 655f 3229 0472 0700 0000  venture_2).r....
-00000280: 7208 0000 0072 0900 0000 da04 3930 3831  r....r......9081
+00000200: da0b 6164 7665 6e74 7572 655f 31da 1070  ..adventure_1..p
+00000210: 726f 6365 7373 5f69 6465 6e74 6974 7929  rocess_identity)
+00000220: 04da 0770 7974 686f 6e33 fa02 2d6d fa0b  ...python3..-m..
+00000230: 6874 7470 2e73 6572 7665 72da 0439 3038  http.server..908
+00000240: 3029 02da 0961 6476 656e 7475 7265 da05  0)...adventure..
+00000250: 506f 7065 6e29 03da 046e 616d 65da 046b  Popen)...name..k
+00000260: 696e 64fa 0774 7572 6e20 6f6e da0b 6164  ind..turn on..ad
+00000270: 7665 6e74 7572 655f 3229 0472 0800 0000  venture_2).r....
+00000280: 7209 0000 0072 0a00 0000 da04 3930 3831  r....r......9081
 00000290: da0b 6164 7665 6e74 7572 655f 3329 0472  ..adventure_3).r
-000002a0: 0700 0000 7208 0000 0072 0900 0000 da04  ....r....r......
+000002a0: 0800 0000 7209 0000 0072 0a00 0000 da04  ....r....r......
 000002b0: 3930 3832 2902 da03 6d61 70da 0876 656e  9082)...map..ven
 000002c0: 7475 7265 7372 1000 0000 e901 0000 007a  turesr.........z
 000002d0: 1368 7474 703a 2f2f 302e 302e 302e 303a  .http://0.0.0.0:
 000002e0: 3930 3830 e9c8 0000 007a 1368 7474 703a  9080.....z.http:
 000002f0: 2f2f 302e 302e 302e 303a 3930 3831 7a13  //0.0.0.0:9081z.
 00000300: 6874 7470 3a2f 2f30 2e30 2e30 2e30 3a39  http://0.0.0.0:9
 00000310: 3038 327a 0874 7572 6e20 6f66 6629 0fda  082z.turn off)..
@@ -60,22 +60,22 @@
 000003b0: 6f6e 7365 a900 7228 0000 00fa 492f 6861  onse..r(....I/ha
 000003c0: 6269 7461 742f 7665 6e75 6573 2f73 7461  bitat/venues/sta
 000003d0: 6765 732f 7665 6e74 7572 6573 2f5f 7374  ges/ventures/_st
 000003e0: 6174 7573 2f6d 6f6e 6974 6f72 732f 325f  atus/monitors/2_
 000003f0: 335f 7665 6e74 7572 6573 2f73 7461 7475  3_ventures/statu
 00000400: 735f 312e 7079 da07 6368 6563 6b5f 3110  s_1.py..check_1.
 00000410: 0000 0073 4e00 0000 1001 0201 0401 0201  ...sN...........
-00000420: 0201 04fe 04ff 0a07 0202 0201 0203 0602  ................
-00000430: 0206 0201 04f8 04fe 020e 0602 0206 0201  ................
-00000440: 04f8 04fe 020e 0602 0206 0201 04f8 04fe  ................
-00000450: 02e5 08fe 0a2d 0a02 0a02 0e01 0a02 0e01  .....-..........
+00000420: 0201 04fe 04ff 0a07 0202 0201 0203 0201  ................
+00000430: 0602 0206 04f9 04fd 020e 0201 0602 0206  ................
+00000440: 04f9 04fd 020f 0201 0602 0206 04f9 04fd  ................
+00000450: 02e4 08fe 0a2e 0a02 0a02 0e01 0a02 0e01  ................
 00000460: 0a02 0e01 0e02 722a 0000 007a 0763 6865  ......r*...z.che
 00000470: 636b 2031 290e da07 5f5f 646f 635f 5f72  ck 1)...__doc__r
 00000480: 1600 0000 7202 0000 0072 2200 0000 da02  ....r....r".....
 00000490: 6f73 7219 0000 00da 076f 732e 7061 7468  osr......os.path
 000004a0: 7203 0000 0072 0400 0000 7205 0000 00da  r....r....r.....
 000004b0: 0373 7973 7220 0000 0072 2a00 0000 da06  .sysr ...r*.....
 000004c0: 6368 6563 6b73 7228 0000 0072 2800 0000  checksr(...r(...
 000004d0: 7228 0000 0072 2900 0000 da08 3c6d 6f64  r(...r).....<mod
 000004e0: 756c 653e 0100 0000 7316 0000 0004 010c  ule>....s.......
 000004f0: 0408 0208 0208 0114 0108 0108 0108 0204  ................
-00000500: 4908 ff                                  I..
+00000500: 4a08 ff                                  J..
```

### Comparing `ventures-1.0.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py` & `ventures-1.1.0/venues/stages/ventures/_status/monitors/2_3_ventures/status_1.py`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/_status/monitors/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/_status/status.proc.py` & `ventures-1.1.0/venues/stages/ventures/_status/status.proc.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 	
 	"simultaneous": True,
 	"simultaneous_capacity": 50,
 
 	"time_limit": 60,
 
 	"module_paths": [
-		normpath (join (venues, "stages"))
+		str (normpath (join (this_directory, "status_venues"))),
+		str (normpath (join (venues, "stages")))
 	],
 
 	"relative_path": this_stage,
 	
 	"db_directory": db_directory,
 	
 	"aggregation_format": 2
```

### Comparing `ventures-1.0.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/plays/__pycache__/is_on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 18 16:36:36 2024 UTC, .py size: 1346 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 14d9 4866 4205 0000  o.........HfB...
+00000000: 6f0d 0d0a 0000 0000 35f7 4866 b004 0000  o.......5.Hf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 8400 5a07 6406 6407 8400 5a08 6402  d...Z.d.d...Z.d.
 00000070: 5300 2908 7a05 270a 090a 22e9 0000 0000  S.).z.'...".....
@@ -20,51 +20,52 @@
 00000130: 0072 0700 0000 fa2e 2f68 6162 6974 6174  .r....../habitat
 00000140: 2f76 656e 7565 732f 7374 6167 6573 2f76  /venues/stages/v
 00000150: 656e 7475 7265 732f 706c 6179 732f 6973  entures/plays/is
 00000160: 5f6f 6e2e 7079 da0c 6669 6e64 5f76 656e  _on.py..find_ven
 00000170: 7475 7265 1400 0000 730a 0000 0008 010c  ture....s.......
 00000180: 0108 0102 ff10 0372 0900 0000 6301 0000  .......r....c...
 00000190: 0000 0000 0000 0000 000c 0000 0008 0000  ................
-000001a0: 0043 0000 0073 d200 0000 7c00 6401 1900  .C...s....|.d...
+000001a0: 0043 0000 0073 d600 0000 7c00 6401 1900  .C...s....|.d...
 000001b0: 7d01 7c00 6402 1900 7d02 7400 7c01 6403  }.|.d...}.t.|.d.
 000001c0: 8302 8f0d 7d03 7401 a002 7c03 a101 7d04  ....}.t...|...}.
 000001d0: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
 000001e0: 731d 7701 0100 0100 0100 5900 0100 6900  s.w.......Y...i.
 000001f0: 7d05 7c04 4400 5d3a 7d06 7c04 7c06 1900  }.|.D.]:}.|.|...
 00000200: 7d07 7c07 6404 1900 7d08 7c08 6405 6b02  }.|.d...}.|.d.k.
 00000210: 7244 7c07 6405 1900 7d09 7403 7c09 8301  rD|.d...}.t.|...
 00000220: 7d0a 7c09 7c0a 6406 9c02 7c05 7c06 3c00  }.|.|.d...|.|.<.
 00000230: 7126 7c08 6407 6b02 7259 7404 7c02 7c06  q&|.d.k.rYt.|.|.
 00000240: 8302 7d0b 7c0b 6408 1900 8300 7d0a 6409  ..}.|.d.....}.d.
 00000250: 7c0a 6901 7c05 7c06 3c00 7126 7405 640a  |.i.|.|.<.q&t.d.
 00000260: 7c08 9b00 640b 9d03 8301 8201 7406 6a07  |...d.......t.j.
-00000270: 7c05 640c 8d01 0100 6400 5300 290d 4eda  |.d.....d.S.).N.
-00000280: 0774 6865 5f6d 6170 7205 0000 00da 0172  .the_mapr......r
-00000290: da04 6b69 6e64 da10 7072 6f63 6573 735f  ..kind..process_
-000002a0: 6964 656e 7469 7479 2902 720d 0000 00da  identity).r.....
-000002b0: 0673 7461 7475 73da 0474 6173 6b7a 0569  .status..taskz.i
-000002c0: 7320 6f6e 720e 0000 007a 064b 696e 6420  s onr....z.Kind 
-000002d0: 227a 0c22 206e 6f74 2066 6f75 6e64 2e29  "z." not found.)
-000002e0: 01da 0464 6174 6129 08da 046f 7065 6eda  ...data)...open.
-000002f0: 046a 736f 6eda 046c 6f61 6472 0200 0000  .json..loadr....
-00000300: 7209 0000 0072 0400 0000 da04 7269 6368  r....r......rich
-00000310: da0a 7072 696e 745f 6a73 6f6e 290c da06  ..print_json)...
-00000320: 7061 636b 6574 720a 0000 0072 0500 0000  packetr....r....
-00000330: da02 4650 da07 6272 6163 6b65 74da 0873  ..FP..bracket..s
-00000340: 7461 7475 7365 73da 0961 6476 656e 7475  tatuses..adventu
-00000350: 7265 da11 6164 7665 6e74 7572 655f 6465  re..adventure_de
-00000360: 7461 696c 7372 0c00 0000 720d 0000 0072  tailsr....r....r
-00000370: 0e00 0000 7206 0000 0072 0700 0000 7207  ....r....r....r.
-00000380: 0000 0072 0800 0000 da05 6973 5f6f 6e1c  ...r......is_on.
-00000390: 0000 0073 3200 0000 0801 0801 0c02 0c01  ...s2...........
-000003a0: 1cff 0404 0801 0801 0801 0803 0801 0801  ................
-000003b0: 0204 0201 0afe 0205 0802 0a01 0a03 0405  ................
-000003c0: 08ff 0204 1002 0c02 0402 721c 0000 0029  ..........r....)
-000003d0: 09da 075f 5f64 6f63 5f5f da06 7073 7574  ...__doc__..psut
-000003e0: 696c da04 7469 6d65 7212 0000 0072 1400  il..timer....r..
-000003f0: 0000 da26 7665 6e74 7572 6573 2e75 7469  ...&ventures.uti
-00000400: 6c69 7469 6573 2e70 726f 6365 7373 2e63  lities.process.c
-00000410: 6865 636b 5f69 735f 6f6e 7202 0000 0072  heck_is_onr....r
-00000420: 0900 0000 721c 0000 0072 0700 0000 7207  ....r....r....r.
-00000430: 0000 0072 0700 0000 7208 0000 00da 083c  ...r....r......<
-00000440: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
-00000450: 0401 0806 0801 0801 0803 0c03 0804 0c08  ................
+00000270: 640c 7c05 6901 640d 8d01 0100 6400 5300  d.|.i.d.....d.S.
+00000280: 290e 4eda 0774 6865 5f6d 6170 7205 0000  ).N..the_mapr...
+00000290: 00da 0172 da04 6b69 6e64 da10 7072 6f63  ...r..kind..proc
+000002a0: 6573 735f 6964 656e 7469 7479 2902 720d  ess_identity).r.
+000002b0: 0000 00da 0673 7461 7475 73da 0474 6173  .....status..tas
+000002c0: 6b7a 0569 7320 6f6e 720e 0000 007a 064b  kz.is onr....z.K
+000002d0: 696e 6420 227a 0c22 206e 6f74 2066 6f75  ind "z." not fou
+000002e0: 6e64 2eda 0873 7461 7475 7365 7329 01da  nd...statuses)..
+000002f0: 0464 6174 6129 08da 046f 7065 6eda 046a  .data)...open..j
+00000300: 736f 6eda 046c 6f61 6472 0200 0000 7209  son..loadr....r.
+00000310: 0000 0072 0400 0000 da04 7269 6368 da0a  ...r......rich..
+00000320: 7072 696e 745f 6a73 6f6e 290c da06 7061  print_json)...pa
+00000330: 636b 6574 720a 0000 0072 0500 0000 da02  cketr....r......
+00000340: 4650 da07 6272 6163 6b65 7472 1000 0000  FP..bracketr....
+00000350: da09 6164 7665 6e74 7572 65da 1161 6476  ..adventure..adv
+00000360: 656e 7475 7265 5f64 6574 6169 6c73 720c  enture_detailsr.
+00000370: 0000 0072 0d00 0000 720e 0000 0072 0600  ...r....r....r..
+00000380: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00000390: 00da 0569 735f 6f6e 1c00 0000 7336 0000  ...is_on....s6..
+000003a0: 0008 0108 010c 020c 011c ff04 0408 0108  ................
+000003b0: 0108 0108 0308 0108 0102 0302 010a fe02  ................
+000003c0: 0508 020a 010a 0104 0308 ff02 0410 0204  ................
+000003d0: 0204 0108 ff04 0472 1c00 0000 2909 da07  .......r....)...
+000003e0: 5f5f 646f 635f 5fda 0670 7375 7469 6cda  __doc__..psutil.
+000003f0: 0474 696d 6572 1300 0000 7215 0000 00da  .timer....r.....
+00000400: 2676 656e 7475 7265 732e 7574 696c 6974  &ventures.utilit
+00000410: 6965 732e 7072 6f63 6573 732e 6368 6563  ies.process.chec
+00000420: 6b5f 6973 5f6f 6e72 0200 0000 7209 0000  k_is_onr....r...
+00000430: 0072 1c00 0000 7207 0000 0072 0700 0000  .r....r....r....
+00000440: 7207 0000 0072 0800 0000 da08 3c6d 6f64  r....r......<mod
+00000450: 756c 653e 0100 0000 7310 0000 0004 0108  ule>....s.......
+00000460: 0608 0108 0108 030c 0308 040c 08         .............
```

### Comparing `ventures-1.0.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/plays/__pycache__/turn_off.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 18 17:49:31 2024 UTC, .py size: 2145 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bea 4866 6108 0000  o.......+.Hfa...
+00000000: 6f0d 0d0a 0000 0000 a49f 4a66 8709 0000  o.........Jf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6406 6407 6c09 5a09 6406 6407 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0a 6406 6407 6c0b 5a0b 6406 6407 6c0c  Z.d.d.l.Z.d.d.l.
@@ -10,91 +10,101 @@
 00000090: 5a0e 6407 5300 290a 7a19 270a 0974 7572  Z.d.S.).z.'..tur
 000000a0: 6e5f 6f66 6620 287b 0a09 090a 097d 290a  n_off ({.....}).
 000000b0: 090a 22e9 0200 0000 2901 da08 6574 6368  ..".....)...etch
 000000c0: 5f6d 6170 2901 da08 7363 616e 5f6d 6170  _map)...scan_map
 000000d0: 2901 da0c 6669 6e64 5f76 656e 7475 7265  )...find_venture
 000000e0: 2901 da0b 6368 6563 6b5f 6973 5f6f 6ee9  )...check_is_on.
 000000f0: 0000 0000 4e63 0100 0000 0000 0000 0000  ....Nc..........
-00000100: 0000 0d00 0000 0800 0000 4300 0000 73ba  ..........C...s.
+00000100: 0000 0d00 0000 0800 0000 4300 0000 73de  ..........C...s.
 00000110: 0100 007c 0064 0119 007d 017c 0064 0219  ...|.d...}.|.d..
 00000120: 007d 0274 007c 0164 0383 028f 0d7d 0374  .}.t.|.d.....}.t
 00000130: 01a0 027c 03a1 017d 0457 0064 0004 0004  ...|...}.W.d....
 00000140: 0083 0301 006e 0831 0073 1d77 0101 0001  .....n.1.s.w....
 00000150: 0001 0059 0001 0074 0364 047c 0483 0201  ...Y...t.d.|....
-00000160: 0067 007d 057c 0444 005d a87d 067c 047c  .g.}.|.D.].}.|.|
-00000170: 0619 007d 077c 0764 0519 007d 0874 0364  ...}.|.d...}.t.d
-00000180: 067c 0883 0201 007c 0864 076b 0272 8b7c  .|.....|.d.k.r.|
-00000190: 0764 0719 0064 086b 0372 8b7c 0764 0719  .d...d.k.r.|.d..
-000001a0: 007d 0974 047c 0983 0164 096b 0372 8b74  .}.t.|...d.k.r.t
-000001b0: 05a0 067c 0974 076a 08a1 0201 0064 087c  ...|.t.j.....d.|
-000001c0: 047c 0619 0064 073c 0064 0a7d 0a09 0074  .|...d.<.d.}...t
-000001d0: 047c 0983 017d 0b74 096a 0a64 0c7c 067c  .|...}.t.j.d.|.|
-000001e0: 0b64 0d9c 0269 0164 0e8d 0101 007c 0b64  .d...i.d.....|.d
-000001f0: 096b 0272 726e 1974 0ba0 0c64 0fa1 0101  .k.rrn.t...d....
-00000200: 007c 0a64 0f37 007d 0a7c 0a64 106b 0272  .|.d.7.}.|.d.k.r
-00000210: 8a74 0d64 117c 0a9b 0064 127c 069b 0064  .t.d.|...d.|...d
-00000220: 139d 0583 0182 0171 5e7c 0864 146b 0272  .......q^|.d.k.r
-00000230: d374 0e7c 027c 0683 027d 0c7c 0c64 1519  .t.|.|...}.|.d..
-00000240: 0083 0064 096b 0372 d37c 0c64 1619 0083  ...d.k.r.|.d....
-00000250: 0001 0064 0a7d 0a09 007c 0c64 1519 0083  ...d.}...|.d....
-00000260: 007d 0b74 096a 0a64 0c7c 0c64 1719 007c  .}.t.j.d.|.d...|
-00000270: 0b64 0d9c 0269 0164 0e8d 0101 007c 0b64  .d...i.d.....|.d
-00000280: 096b 0272 ba6e 1974 0ba0 0c64 0fa1 0101  .k.r.n.t...d....
-00000290: 007c 0a64 0f37 007d 0a7c 0a64 106b 0272  .|.d.7.}.|.d.k.r
-000002a0: d274 0d64 117c 0a9b 0064 127c 069b 0064  .t.d.|...d.|...d
-000002b0: 139d 0583 0182 0171 a371 2b74 0f7c 017c  .......q.q+t.|.|
-000002c0: 0464 189c 0283 0101 0064 0053 0029 194e  .d.......d.S.).N
-000002d0: da07 7468 655f 6d61 70da 0876 656e 7475  ..the_map..ventu
-000002e0: 7265 73da 0172 7a15 7665 6e74 7572 6573  res..rz.ventures
-000002f0: 5f6d 6170 5f62 7261 636b 6574 3ada 046b  _map_bracket:..k
-00000300: 696e 647a 056b 696e 643a da10 7072 6f63  indz.kind:..proc
-00000310: 6573 735f 6964 656e 7469 7479 da00 da03  ess_identity....
-00000320: 6f66 6672 0600 0000 547a 0c73 7461 7475  offr....Tz.statu
-00000330: 7320 6368 6563 6b29 02da 046e 616d 65da  s check)...name.
-00000340: 0673 7461 7475 7329 01da 0464 6174 61e9  .status)...data.
-00000350: 0100 0000 e90a 0000 007a 0641 6674 6572  .........z.After
-00000360: 207a 0820 6c6f 6f70 732c 207a 1220 6469   z. loops, z. di
-00000370: 6420 6e6f 7420 7475 726e 206f 6666 2eda  d not turn off..
-00000380: 0474 6173 6b7a 0569 7320 6f6e 7a08 7475  .taskz.is onz.tu
-00000390: 726e 206f 6666 720e 0000 0029 02da 0470  rn offr....)...p
-000003a0: 6174 68da 0762 7261 636b 6574 2910 da04  ath..bracket)...
-000003b0: 6f70 656e da04 6a73 6f6e da04 6c6f 6164  open..json..load
-000003c0: da05 7072 696e 7472 0500 0000 da02 6f73  ..printr......os
-000003d0: da04 6b69 6c6c da06 7369 676e 616c da07  ..kill..signal..
-000003e0: 5349 4754 4552 4dda 0472 6963 68da 0a70  SIGTERM..rich..p
-000003f0: 7269 6e74 5f6a 736f 6eda 0474 696d 65da  rint_json..time.
-00000400: 0573 6c65 6570 da09 4578 6365 7074 696f  .sleep..Exceptio
-00000410: 6e72 0400 0000 7202 0000 0029 0dda 0670  nr....r....)...p
-00000420: 6163 6b65 74da 0c74 6865 5f6d 6170 5f70  acket..the_map_p
-00000430: 6174 6872 0800 0000 da02 4650 da14 7665  athr......FP..ve
-00000440: 6e74 7572 6573 5f6d 6170 5f62 7261 636b  ntures_map_brack
-00000450: 6574 da09 746f 5f64 656c 6574 6572 0e00  et..to_deleter..
-00000460: 0000 da09 6164 7665 6e74 7572 6572 0a00  ....adventurer..
-00000470: 0000 720b 0000 00da 046c 6f6f 7072 0f00  ..r......loopr..
-00000480: 0000 da07 7665 6e74 7572 65a9 0072 2b00  ....venture..r+.
-00000490: 0000 fa31 2f68 6162 6974 6174 2f76 656e  ...1/habitat/ven
-000004a0: 7565 732f 7374 6167 6573 2f76 656e 7475  ues/stages/ventu
-000004b0: 7265 732f 706c 6179 732f 7475 726e 5f6f  res/plays/turn_o
-000004c0: 6666 2e70 79da 0874 7572 6e5f 6f66 661e  ff.py..turn_off.
-000004d0: 0000 0073 7c00 0000 0801 0801 0c02 0c01  ...s|...........
-000004e0: 1cff 0a03 0402 0801 0801 0801 0a02 0802  ................
-000004f0: 0c01 0801 0c02 0e01 0c01 0403 0201 0801  ................
-00000500: 0401 0201 0201 0201 04fe 08ff 0807 0201  ................
-00000510: 0a02 0802 0801 0201 1001 04ff 02f0 0815  ................
-00000520: 0a01 0e02 0a01 0402 0201 0a01 0401 0201  ................
-00000530: 0601 0201 04fe 08ff 0807 0201 0a02 0802  ................
-00000540: 0801 0201 1001 04ff 02f0 0280 0218 0201  ................
-00000550: 0201 0cfe 722d 0000 0029 0fda 075f 5f64  ....r-...)...__d
-00000560: 6f63 5f5f da12 7574 696c 6974 6965 732e  oc__..utilities.
-00000570: 6d61 702e 6574 6368 7202 0000 00da 1275  map.etchr......u
-00000580: 7469 6c69 7469 6573 2e6d 6170 2e73 6361  tilities.map.sca
-00000590: 6e72 0300 0000 da1f 7574 696c 6974 6965  nr......utilitie
-000005a0: 732e 7665 6e74 7572 6573 2e66 696e 645f  s.ventures.find_
-000005b0: 7665 6e74 7572 6572 0400 0000 da1d 7574  venturer......ut
-000005c0: 696c 6974 6965 732e 7072 6f63 6573 732e  ilities.process.
-000005d0: 6368 6563 6b5f 6973 5f6f 6e72 0500 0000  check_is_onr....
-000005e0: 721e 0000 0072 1700 0000 721c 0000 0072  r....r....r....r
-000005f0: 1a00 0000 7220 0000 0072 2d00 0000 722b  ....r ...r-...r+
-00000600: 0000 0072 2b00 0000 722b 0000 0072 2c00  ...r+...r+...r,.
-00000610: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000620: 7316 0000 0004 020c 0a0c 010c 010c 0108  s...............
-00000630: 0308 0308 0108 0108 010c 05              ...........
+00000160: 0067 007d 057c 0444 005d ba7d 067c 047c  .g.}.|.D.].}.|.|
+00000170: 0619 007d 077c 0764 0519 007d 0874 046a  ...}.|.d...}.t.j
+00000180: 0564 067c 0764 079c 0264 088d 0101 007c  .d.|.d...d.....|
+00000190: 0864 096b 0272 9b7c 0764 0919 0064 0a6b  .d.k.r.|.d...d.k
+000001a0: 0372 9b7c 0764 0919 007d 0974 046a 0564  .r.|.d...}.t.j.d
+000001b0: 0674 067c 0983 0164 0b9c 0264 088d 0101  .t.|...d...d....
+000001c0: 0074 067c 0983 0164 0c6b 0372 9b74 07a0  .t.|...d.k.r.t..
+000001d0: 087c 0974 096a 0aa1 0201 0064 0a7c 047c  .|.t.j.....d.|.|
+000001e0: 0619 0064 093c 0064 0d7d 0a09 0074 067c  ...d.<.d.}...t.|
+000001f0: 0983 017d 0b74 046a 0564 067c 067c 0b64  ...}.t.j.d.|.|.d
+00000200: 0f9c 0264 109c 0264 088d 0101 007c 0b64  ...d...d.....|.d
+00000210: 0c6b 0272 826e 1974 0ba0 0c64 11a1 0101  .k.r.n.t...d....
+00000220: 007c 0a64 1137 007d 0a7c 0a64 126b 0272  .|.d.7.}.|.d.k.r
+00000230: 9a74 0d64 137c 0a9b 0064 147c 069b 0064  .t.d.|...d.|...d
+00000240: 159d 0583 0182 0171 6d7c 0864 166b 0272  .......qm|.d.k.r
+00000250: e574 0e7c 027c 0683 027d 0c7c 0c64 1719  .t.|.|...}.|.d..
+00000260: 0083 0064 0c6b 0372 e57c 0c64 0619 0083  ...d.k.r.|.d....
+00000270: 0001 0064 0d7d 0a09 007c 0c64 1719 0083  ...d.}...|.d....
+00000280: 007d 0b74 046a 0564 1864 197c 0a7c 0c64  .}.t.j.d.d.|.|.d
+00000290: 1a19 007c 0b64 1b9c 0469 0164 088d 0101  ...|.d...i.d....
+000002a0: 007c 0b64 0c6b 0272 cc6e 1974 0ba0 0c64  .|.d.k.r.n.t...d
+000002b0: 11a1 0101 007c 0a64 1137 007d 0a7c 0a64  .....|.d.7.}.|.d
+000002c0: 126b 0272 e474 0d64 137c 0a9b 0064 147c  .k.r.t.d.|...d.|
+000002d0: 069b 0064 159d 0583 0182 0171 b371 2b74  ...d.......q.q+t
+000002e0: 0f7c 017c 0464 1c9c 0283 0101 0064 0053  .|.|.d.......d.S
+000002f0: 0029 1d4e da07 7468 655f 6d61 70da 0876  .).N..the_map..v
+00000300: 656e 7475 7265 73da 0172 7a15 7665 6e74  entures..rz.vent
+00000310: 7572 6573 5f6d 6170 5f62 7261 636b 6574  ures_map_bracket
+00000320: 3ada 046b 696e 647a 0874 7572 6e20 6f66  :..kindz.turn of
+00000330: 6629 02da 0470 6c61 79da 0961 6476 656e  f)...play..adven
+00000340: 7475 7265 2901 da04 6461 7461 da10 7072  ture)...data..pr
+00000350: 6f63 6573 735f 6964 656e 7469 7479 da00  ocess_identity..
+00000360: 2902 720b 0000 0072 0e00 0000 da03 6f66  ).r....r......of
+00000370: 6672 0600 0000 5429 02da 046e 616d 65da  fr....T)...name.
+00000380: 0673 7461 7475 7329 0272 0b00 0000 7a12  .status).r....z.
+00000390: 7374 6174 7573 2063 6865 636b 2063 7963  status check cyc
+000003a0: 6c65 e901 0000 00e9 0a00 0000 7a06 4166  le..........z.Af
+000003b0: 7465 7220 7a08 206c 6f6f 7073 2c20 7a12  ter z. loops, z.
+000003c0: 2064 6964 206e 6f74 2074 7572 6e20 6f66   did not turn of
+000003d0: 662e da04 7461 736b 7a05 6973 206f 6e7a  f...taskz.is onz
+000003e0: 1976 656e 7475 7265 2073 7461 7475 7320  .venture status 
+000003f0: 6368 6563 6b20 6c6f 6f70 7a17 6166 7465  check loopz.afte
+00000400: 7220 7475 726e 206f 6666 2077 6173 2073  r turn off was s
+00000410: 656e 7472 1100 0000 2904 da04 7768 656e  entr....)...when
+00000420: da04 6c6f 6f70 7211 0000 0072 1200 0000  ..loopr....r....
+00000430: 2902 da04 7061 7468 da07 6272 6163 6b65  )...path..bracke
+00000440: 7429 10da 046f 7065 6eda 046a 736f 6eda  t)...open..json.
+00000450: 046c 6f61 64da 0570 7269 6e74 da04 7269  .load..print..ri
+00000460: 6368 da0a 7072 696e 745f 6a73 6f6e 7205  ch..print_jsonr.
+00000470: 0000 00da 026f 73da 046b 696c 6cda 0673  .....os..kill..s
+00000480: 6967 6e61 6cda 0753 4947 5445 524d da04  ignal..SIGTERM..
+00000490: 7469 6d65 da05 736c 6565 70da 0945 7863  time..sleep..Exc
+000004a0: 6570 7469 6f6e 7204 0000 0072 0200 0000  eptionr....r....
+000004b0: 290d da06 7061 636b 6574 da0c 7468 655f  )...packet..the_
+000004c0: 6d61 705f 7061 7468 7208 0000 00da 0246  map_pathr......F
+000004d0: 50da 1476 656e 7475 7265 735f 6d61 705f  P..ventures_map_
+000004e0: 6272 6163 6b65 74da 0974 6f5f 6465 6c65  bracket..to_dele
+000004f0: 7465 7211 0000 0072 0c00 0000 720a 0000  ter....r....r...
+00000500: 0072 0e00 0000 7217 0000 0072 1200 0000  .r....r....r....
+00000510: da07 7665 6e74 7572 65a9 0072 2d00 0000  ..venture..r-...
+00000520: fa31 2f68 6162 6974 6174 2f76 656e 7565  .1/habitat/venue
+00000530: 732f 7374 6167 6573 2f76 656e 7475 7265  s/stages/venture
+00000540: 732f 706c 6179 732f 7475 726e 5f6f 6666  s/plays/turn_off
+00000550: 2e70 79da 0874 7572 6e5f 6f66 661e 0000  .py..turn_off...
+00000560: 0073 8e00 0000 0801 0801 0c02 0c01 1cff  .s..............
+00000570: 0a03 0402 0801 0801 0801 0403 0201 0201  ................
+00000580: 0afe 0806 0c01 0801 0402 0201 0601 0afe  ................
+00000590: 0c05 0e01 0c01 0403 0201 0801 0401 0201  ................
+000005a0: 0202 0201 04fe 0afe 0808 0201 0a02 0802  ................
+000005b0: 0801 0201 1001 04ff 02ef 0816 0a01 0e02  ................
+000005c0: 0a01 0402 0201 0a01 0402 0201 0201 0201  ................
+000005d0: 0601 0201 04fc 08ff 0809 0201 0a02 0802  ................
+000005e0: 0801 0201 1001 04ff 02ed 0280 021b 0201  ................
+000005f0: 0201 0cfe 722f 0000 0029 0fda 075f 5f64  ....r/...)...__d
+00000600: 6f63 5f5f da12 7574 696c 6974 6965 732e  oc__..utilities.
+00000610: 6d61 702e 6574 6368 7202 0000 00da 1275  map.etchr......u
+00000620: 7469 6c69 7469 6573 2e6d 6170 2e73 6361  tilities.map.sca
+00000630: 6e72 0300 0000 da1f 7574 696c 6974 6965  nr......utilitie
+00000640: 732e 7665 6e74 7572 6573 2e66 696e 645f  s.ventures.find_
+00000650: 7665 6e74 7572 6572 0400 0000 da1d 7574  venturer......ut
+00000660: 696c 6974 6965 732e 7072 6f63 6573 732e  ilities.process.
+00000670: 6368 6563 6b5f 6973 5f6f 6e72 0500 0000  check_is_onr....
+00000680: 721e 0000 0072 1b00 0000 7222 0000 0072  r....r....r"...r
+00000690: 2000 0000 7224 0000 0072 2f00 0000 722d   ...r$...r/...r-
+000006a0: 0000 0072 2d00 0000 722d 0000 0072 2e00  ...r-...r-...r..
+000006b0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000006c0: 7316 0000 0004 020c 0a0c 010c 010c 0108  s...............
+000006d0: 0308 0308 0108 0108 010c 05              ...........
```

### Comparing `ventures-1.0.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/plays/__pycache__/turn_on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 18 17:49:43 2024 UTC, .py size: 2699 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,108 @@
-00000000: 6f0d 0d0a 0000 0000 37ea 4866 8b0a 0000  o.......7.Hf....
+00000000: 6f0d 0d0a 0000 0000 87a0 4a66 130b 0000  o.........Jf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6405 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 5a0a 6405 6407 6c0b 5a0b 6405 6407 6c0c  Z.d.d.l.Z.d.d.l.
 00000080: 5a0c 0900 6408 6409 8400 5a0d 6407 5300  Z...d.d...Z.d.S.
 00000090: 290a e902 0000 0029 01da 0c68 696b 655f  )......)...hike_
 000000a0: 7061 7373 6976 6529 01da 0865 7463 685f  passive)...etch_
 000000b0: 6d61 7029 01da 0873 6361 6e5f 6d61 7029  map)...scan_map)
 000000c0: 01da 0c66 696e 645f 7665 6e74 7572 65e9  ...find_venture.
 000000d0: 0000 0000 2901 da0b 6368 6563 6b5f 6973  ....)...check_is
 000000e0: 5f6f 6e4e 6301 0000 0000 0000 0000 0000  _onNc...........
-000000f0: 000c 0000 0007 0000 0043 0000 0073 e001  .........C...s..
+000000f0: 000c 0000 0008 0000 0043 0000 0073 e401  .........C...s..
 00000100: 0000 7c00 6401 1900 7d01 7c00 6402 1900  ..|.d...}.|.d...
 00000110: 7d02 6900 7d03 7400 6a01 a002 7c02 a101  }.i.}.t.j...|...
 00000120: 7216 7403 6403 7c02 6901 8301 7d03 7c01  r.t.d.|.i...}.|.
-00000130: 4400 5dce 7d04 7c04 6404 1900 6405 1900  D.].}.|.d...d...
+00000130: 4400 5dd0 7d04 7c04 6404 1900 6405 1900  D.].}.|.d...d...
 00000140: 7d05 7c04 6406 1900 7d06 7c04 6407 1900  }.|.d...}.|.d...
 00000150: 7d07 7c07 7c03 7600 7258 7c06 6408 6b02  }.|.|.v.rX|.d.k.
 00000160: 7245 7c03 7c07 1900 6408 1900 6409 6b03  rE|.|...d...d.k.
 00000170: 7245 7404 7c03 7c07 1900 6408 1900 8301  rEt.|.|...d.....
 00000180: 7d08 7c08 640a 6b02 7245 7118 7c06 640b  }.|.d.k.rEq.|.d.
 00000190: 6b02 7258 7405 7c01 7c07 8302 7d09 7c09  k.rXt.|.|...}.|.
 000001a0: 640c 1900 8300 7d08 7c08 640a 6b02 7258  d.....}.|.d.k.rX
-000001b0: 7118 7c06 6408 6b02 729e 7406 640d 7c05  q.|.d.k.r.t.d.|.
+000001b0: 7118 7c06 6408 6b02 72a0 7406 640d 7c05  q.|.d.k.r.t.d.|.
 000001c0: 6901 8301 7d0a 640e 7d0b 0900 7404 7c0a  i...}.d.}...t.|.
-000001d0: 6408 1900 8301 7d08 7407 6a08 6410 7c07  d.....}.t.j.d.|.
-000001e0: 7c08 6411 9c02 6901 6412 8d01 0100 7c08  |.d...i.d.....|.
-000001f0: 640a 6b02 727b 6e19 7409 a00a 6413 a101  d.k.r{n.t...d...
-00000200: 0100 7c0b 6413 3700 7d0b 7c0b 6414 6b02  ..|.d.7.}.|.d.k.
-00000210: 7293 740b 6415 7c0b 9b00 6416 7c07 9b00  r.t.d.|...d.|...
-00000220: 6417 9d05 8301 8201 7165 7c06 7c0a 6408  d.......qe|.|.d.
-00000230: 1900 6418 9c02 7c03 7c07 3c00 7118 7c06  ..d...|.|.<.q.|.
-00000240: 640b 6b02 72df 7c05 8300 0100 640e 7d0b  d.k.r.|.....d.}.
-00000250: 0900 7c09 640c 1900 8300 7d08 7407 6a08  ..|.d.....}.t.j.
-00000260: 6410 7c09 6407 1900 7c08 6411 9c02 6901  d.|.d...|.d...i.
-00000270: 6412 8d01 0100 7c08 640a 6b02 72bf 6e19  d.....|.d.k.r.n.
-00000280: 7409 a00a 6413 a101 0100 7c0b 6413 3700  t...d.....|.d.7.
-00000290: 7d0b 7c0b 6414 6b02 72d7 740b 6415 7c0b  }.|.d.k.r.t.d.|.
-000002a0: 9b00 6416 7c07 9b00 6417 9d05 8301 8201  ..d.|...d.......
-000002b0: 71a8 6406 7c06 6901 7c03 7c07 3c00 7118  q.d.|.i.|.|.<.q.
-000002c0: 740b 6419 7c06 9b00 641a 9d03 8301 8201  t.d.|...d.......
-000002d0: 740c 7c02 7c03 641b 9c02 8301 0100 7c03  t.|.|.d.......|.
-000002e0: 5300 291c 4eda 0876 656e 7475 7265 73da  S.).N..ventures.
-000002f0: 036d 6170 da04 7061 7468 7a07 7475 726e  .map..pathz.turn
-00000300: 206f 6eda 0961 6476 656e 7475 7265 da04   on..adventure..
-00000310: 6b69 6e64 da04 6e61 6d65 da10 7072 6f63  kind..name..proc
-00000320: 6573 735f 6964 656e 7469 7479 da00 da02  ess_identity....
-00000330: 6f6e da04 7461 736b 7a05 6973 206f 6eda  on..taskz.is on.
-00000340: 0673 6372 6970 7472 0600 0000 547a 0c73  .scriptr....Tz.s
-00000350: 7461 7475 7320 6368 6563 6b29 0272 0d00  tatus check).r..
-00000360: 0000 da06 7374 6174 7573 2901 da04 6461  ....status)...da
-00000370: 7461 e901 0000 00e9 0a00 0000 7a06 4166  ta..........z.Af
-00000380: 7465 7220 7a08 206c 6f6f 7073 2c20 7a11  ter z. loops, z.
-00000390: 2064 6964 206e 6f74 2074 7572 6e20 6f6e   did not turn on
-000003a0: 2e29 0272 0c00 0000 720e 0000 007a 064b  .).r....r....z.K
-000003b0: 696e 6420 227a 0f20 7761 7320 6e6f 7420  ind "z. was not 
-000003c0: 666f 756e 642e 2902 720a 0000 00da 0762  found.).r......b
-000003d0: 7261 636b 6574 290d da02 6f73 720a 0000  racket)...osr...
-000003e0: 00da 0665 7869 7374 7372 0400 0000 7207  ...existsr....r.
-000003f0: 0000 0072 0500 0000 7202 0000 00da 0472  ...r....r......r
-00000400: 6963 68da 0a70 7269 6e74 5f6a 736f 6eda  ich..print_json.
-00000410: 0474 696d 65da 0573 6c65 6570 da09 4578  .time..sleep..Ex
-00000420: 6365 7074 696f 6e72 0300 0000 290c da06  ceptionr....)...
-00000430: 7061 636b 6574 7208 0000 00da 0c74 6865  packetr......the
-00000440: 5f6d 6170 5f70 6174 68da 1476 656e 7475  _map_path..ventu
-00000450: 7265 735f 6d61 705f 6272 6163 6b65 7472  res_map_bracketr
-00000460: 0b00 0000 da10 6164 7665 6e74 7572 655f  ......adventure_
-00000470: 7363 7269 7074 720c 0000 0072 0d00 0000  scriptr....r....
-00000480: 7213 0000 00da 0776 656e 7475 7265 da07  r......venture..
-00000490: 7072 6f63 6573 73da 046c 6f6f 70a9 0072  process..loop..r
-000004a0: 2600 0000 fa30 2f68 6162 6974 6174 2f76  &....0/habitat/v
-000004b0: 656e 7565 732f 7374 6167 6573 2f76 656e  enues/stages/ven
-000004c0: 7475 7265 732f 706c 6179 732f 7475 726e  tures/plays/turn
-000004d0: 5f6f 6e2e 7079 da07 7475 726e 5f6f 6e27  _on.py..turn_on'
-000004e0: 0000 0073 9800 0000 0801 0801 0402 0c01  ...s............
-000004f0: 0201 0401 06ff 0804 0c01 0801 0801 0807  ................
-00000500: 0801 1001 1001 0801 0202 0802 0a01 0a01  ................
-00000510: 0801 0201 0804 0201 0401 06ff 0404 0201  ................
-00000520: 0c01 0401 0201 0201 0201 04fe 08ff 0807  ................
-00000530: 0201 0a02 0802 0801 0201 1001 04ff 02f0  ................
-00000540: 0215 0601 0afe 0205 0802 0601 0402 0201  ................
-00000550: 0a01 0401 0201 0601 0201 04fe 08ff 0807  ................
-00000560: 0201 0a02 0802 0801 0201 1001 04ff 02f0  ................
-00000570: 0415 0aff 1006 0203 0201 0201 08fe 0405  ................
-00000580: 7228 0000 0029 0eda 1675 7469 6c69 7469  r(...)...utiliti
-00000590: 6573 2e68 696b 655f 7061 7373 6976 6572  es.hike_passiver
-000005a0: 0200 0000 da12 7574 696c 6974 6965 732e  ......utilities.
-000005b0: 6d61 702e 6574 6368 7203 0000 00da 1275  map.etchr......u
-000005c0: 7469 6c69 7469 6573 2e6d 6170 2e73 6361  tilities.map.sca
-000005d0: 6e72 0400 0000 da1f 7574 696c 6974 6965  nr......utilitie
-000005e0: 732e 7665 6e74 7572 6573 2e66 696e 645f  s.ventures.find_
-000005f0: 7665 6e74 7572 6572 0500 0000 da26 7665  venturer.....&ve
-00000600: 6e74 7572 6573 2e75 7469 6c69 7469 6573  ntures.utilities
-00000610: 2e70 726f 6365 7373 2e63 6865 636b 5f69  .process.check_i
-00000620: 735f 6f6e 7207 0000 0072 1a00 0000 7218  s_onr....r....r.
-00000630: 0000 0072 1c00 0000 7228 0000 0072 2600  ...r....r(...r&.
-00000640: 0000 7226 0000 0072 2600 0000 7227 0000  ..r&...r&...r'..
-00000650: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000660: 1400 0000 0c03 0c01 0c01 0c01 0c02 0803  ................
-00000670: 0803 0801 0204 0c13                      ........
+000001d0: 6408 1900 8301 7d08 7407 6a08 6410 6411  d.....}.t.j.d.d.
+000001e0: 7c0b 7c07 7c08 6412 9c04 6901 6413 8d01  |.|.|.d...i.d...
+000001f0: 0100 7c08 640a 6b02 727d 6e19 7409 a00a  ..|.d.k.r}n.t...
+00000200: 6414 a101 0100 7c0b 6414 3700 7d0b 7c0b  d.....|.d.7.}.|.
+00000210: 6415 6b02 7295 740b 6416 7c0b 9b00 6417  d.k.r.t.d.|...d.
+00000220: 7c07 9b00 6418 9d05 8301 8201 7165 7c06  |...d.......qe|.
+00000230: 7c0a 6408 1900 6419 9c02 7c03 7c07 3c00  |.d...d...|.|.<.
+00000240: 7118 7c06 640b 6b02 72e1 7c05 8300 0100  q.|.d.k.r.|.....
+00000250: 640e 7d0b 0900 7c04 640c 1900 8300 7d08  d.}...|.d.....}.
+00000260: 7407 6a08 6410 6411 7c0b 7c07 7c08 6412  t.j.d.d.|.|.|.d.
+00000270: 9c04 6901 6413 8d01 0100 7c08 640a 6b02  ..i.d.....|.d.k.
+00000280: 72c1 6e19 7409 a00a 6414 a101 0100 7c0b  r.n.t...d.....|.
+00000290: 6414 3700 7d0b 7c0b 6415 6b02 72d9 740b  d.7.}.|.d.k.r.t.
+000002a0: 6416 7c0b 9b00 6417 7c07 9b00 6418 9d05  d.|...d.|...d...
+000002b0: 8301 8201 71aa 6406 7c06 6901 7c03 7c07  ....q.d.|.i.|.|.
+000002c0: 3c00 7118 740b 641a 7c06 9b00 641b 9d03  <.q.t.d.|...d...
+000002d0: 8301 8201 740c 7c02 7c03 641c 9c02 8301  ....t.|.|.d.....
+000002e0: 0100 7c03 5300 291d 4eda 0876 656e 7475  ..|.S.).N..ventu
+000002f0: 7265 73da 036d 6170 da04 7061 7468 7a07  res..map..pathz.
+00000300: 7475 726e 206f 6eda 0961 6476 656e 7475  turn on..adventu
+00000310: 7265 da04 6b69 6e64 da04 6e61 6d65 da10  re..kind..name..
+00000320: 7072 6f63 6573 735f 6964 656e 7469 7479  process_identity
+00000330: da00 da02 6f6e da04 7461 736b 7a05 6973  ....on..taskz.is
+00000340: 206f 6eda 0673 6372 6970 7472 0600 0000   on..scriptr....
+00000350: 547a 1976 656e 7475 7265 2073 7461 7475  Tz.venture statu
+00000360: 7320 6368 6563 6b20 6c6f 6f70 7a16 6166  s check loopz.af
+00000370: 7465 7220 7475 726e 206f 6e20 7761 7320  ter turn on was 
+00000380: 7365 6e74 2904 da04 7768 656e da04 6c6f  sent)...when..lo
+00000390: 6f70 720d 0000 00da 0673 7461 7475 7329  opr......status)
+000003a0: 01da 0464 6174 61e9 0100 0000 e90a 0000  ...data.........
+000003b0: 007a 0641 6674 6572 207a 0820 6c6f 6f70  .z.After z. loop
+000003c0: 732c 207a 1120 6469 6420 6e6f 7420 7475  s, z. did not tu
+000003d0: 726e 206f 6e2e 2902 720c 0000 0072 0e00  rn on.).r....r..
+000003e0: 0000 7a06 4b69 6e64 2022 7a0f 2077 6173  ..z.Kind "z. was
+000003f0: 206e 6f74 2066 6f75 6e64 2e29 0272 0a00   not found.).r..
+00000400: 0000 da07 6272 6163 6b65 7429 0dda 026f  ....bracket)...o
+00000410: 7372 0a00 0000 da06 6578 6973 7473 7204  sr......existsr.
+00000420: 0000 0072 0700 0000 7205 0000 0072 0200  ...r....r....r..
+00000430: 0000 da04 7269 6368 da0a 7072 696e 745f  ....rich..print_
+00000440: 6a73 6f6e da04 7469 6d65 da05 736c 6565  json..time..slee
+00000450: 70da 0945 7863 6570 7469 6f6e 7203 0000  p..Exceptionr...
+00000460: 0029 0cda 0670 6163 6b65 7472 0800 0000  .)...packetr....
+00000470: da0c 7468 655f 6d61 705f 7061 7468 da14  ..the_map_path..
+00000480: 7665 6e74 7572 6573 5f6d 6170 5f62 7261  ventures_map_bra
+00000490: 636b 6574 720b 0000 00da 1061 6476 656e  cketr......adven
+000004a0: 7475 7265 5f73 6372 6970 7472 0c00 0000  ture_scriptr....
+000004b0: 720d 0000 0072 1500 0000 da07 7665 6e74  r....r......vent
+000004c0: 7572 65da 0770 726f 6365 7373 7214 0000  ure..processr...
+000004d0: 00a9 0072 2700 0000 fa30 2f68 6162 6974  ...r'....0/habit
+000004e0: 6174 2f76 656e 7565 732f 7374 6167 6573  at/venues/stages
+000004f0: 2f76 656e 7475 7265 732f 706c 6179 732f  /ventures/plays/
+00000500: 7475 726e 5f6f 6e2e 7079 da07 7475 726e  turn_on.py..turn
+00000510: 5f6f 6e27 0000 0073 a000 0000 0801 0801  _on'...s........
+00000520: 0402 0c01 0201 0401 06ff 0804 0c01 0801  ................
+00000530: 0801 0807 0801 1001 1001 0801 0202 0802  ................
+00000540: 0a01 0a01 0801 0201 0804 0201 0401 06ff  ................
+00000550: 0404 0201 0c01 0401 0201 0201 0201 0201  ................
+00000560: 0201 04fc 08ff 0809 0201 0a02 0802 0801  ................
+00000570: 0201 1001 04ff 02ee 0217 0601 0afe 0205  ................
+00000580: 0802 0601 0402 0201 0a01 0401 0201 0201  ................
+00000590: 0201 0201 0201 04fc 08ff 0809 0201 0a02  ................
+000005a0: 0802 0801 0201 1001 04ff 02ee 0417 0aff  ................
+000005b0: 1006 0203 0201 0201 08fe 0405 7229 0000  ............r)..
+000005c0: 0029 0eda 1675 7469 6c69 7469 6573 2e68  .)...utilities.h
+000005d0: 696b 655f 7061 7373 6976 6572 0200 0000  ike_passiver....
+000005e0: da12 7574 696c 6974 6965 732e 6d61 702e  ..utilities.map.
+000005f0: 6574 6368 7203 0000 00da 1275 7469 6c69  etchr......utili
+00000600: 7469 6573 2e6d 6170 2e73 6361 6e72 0400  ties.map.scanr..
+00000610: 0000 da1f 7574 696c 6974 6965 732e 7665  ....utilities.ve
+00000620: 6e74 7572 6573 2e66 696e 645f 7665 6e74  ntures.find_vent
+00000630: 7572 6572 0500 0000 da26 7665 6e74 7572  urer.....&ventur
+00000640: 6573 2e75 7469 6c69 7469 6573 2e70 726f  es.utilities.pro
+00000650: 6365 7373 2e63 6865 636b 5f69 735f 6f6e  cess.check_is_on
+00000660: 7207 0000 0072 1c00 0000 721a 0000 0072  r....r....r....r
+00000670: 1e00 0000 7229 0000 0072 2700 0000 7227  ....r)...r'...r'
+00000680: 0000 0072 2700 0000 7228 0000 00da 083c  ...r'...r(.....<
+00000690: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
+000006a0: 0c03 0c01 0c01 0c01 0c02 0803 0803 0801  ................
+000006b0: 0204 0c13                                ....
```

### Comparing `ventures-1.0.0/venues/stages/ventures/plays/is_on.py` & `ventures-1.1.0/venues/stages/ventures/plays/is_on.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,36 +38,33 @@
 		adventure_details = bracket [ adventure ]
 		kind = adventure_details ["kind"]
 		#print (ventures)
 		
 		if (kind == "process_identity"):
 			process_identity = adventure_details ["process_identity"]
 			status = check_is_on (process_identity)
-			#print (f'    [{ status }] :: "{ adventure }" "{ process_identity }"')
 			
 			statuses [ adventure ] = {
 				"process_identity": process_identity,
 				"status": status
 			}
 			
 			continue;
 			
 		if (kind == "task"):	
 			venture = find_venture (ventures, adventure)
-			#print ("venture:", venture)
-			
 			status = venture ["is on"] ()
-			
-			#print (f'    [{ status }] :: "{ adventure }"')
 				
 			statuses [ adventure ] = {
 				"status": status
 			}	
 				
 			continue;
 			
 		raise Exception (f'Kind "{ kind }" not found.')
 				
-	rich.print_json (data = statuses)
+	rich.print_json (data = {
+		"statuses": statuses
+	})
 
 	return;
```

### Comparing `ventures-1.0.0/venues/stages/ventures/plays/turn_off.py` & `ventures-1.1.0/venues/stages/ventures/plays/turn_off.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,30 +37,41 @@
 	print ("ventures_map_bracket:", ventures_map_bracket)
 	
 	to_delete = []
 	for name in ventures_map_bracket:
 		adventure = ventures_map_bracket [ name ]
 		kind = adventure ["kind"]
 		
-		print ("kind:", kind)
 		
+		rich.print_json (data = {
+			"play": "turn off",
+			"adventure": adventure
+		})
+
+
 		if (kind == "process_identity"):
 			if (adventure ["process_identity"] != ""):
 				process_identity = adventure ["process_identity"]
 			
+				rich.print_json (data = {
+					"play": "turn off",
+					"process_identity": check_is_on (process_identity)
+				})
+					
 				if (check_is_on (process_identity) != "off"):
 					os.kill (process_identity, signal.SIGTERM)
 					ventures_map_bracket [ name ] ["process_identity"] = ""
 					
 					#to_delete.append (name)
 					loop = 0
 					while True:
 						status = check_is_on (process_identity)	
 						rich.print_json (data = {
-							"status check": {
+							"play": "turn off",
+							"status check cycle": {
 								"name": name,
 								"status": status
 							}
 						})
 						
 						if (status == "off"):
 							break;
@@ -79,16 +90,19 @@
 			
 			if (venture ["is on"] () != "off"):			
 				venture ["turn off"] ()
 				
 				loop = 0
 				while True:
 					status = venture ["is on"] ()		
+
 					rich.print_json (data = {
-						"status check": {
+						"venture status check loop": {
+							"when": "after turn off was sent",
+							"loop": loop,
 							"name": venture ["name"],
 							"status": status
 						}
 					})
 					
 					if (status == "off"):
 						break;
```

### Comparing `ventures-1.0.0/venues/stages/ventures/plays/turn_on.py` & `ventures-1.1.0/venues/stages/ventures/plays/turn_on.py`

 * *Files 13% similar despite different names*

```diff
@@ -77,15 +77,17 @@
 				"script": adventure_script
 			})
 			
 			loop = 0
 			while True:
 				status = check_is_on (process ["process_identity"])	
 				rich.print_json (data = {
-					"status check": {
+					"venture status check loop": {
+						"when": "after turn on was sent",
+						"loop": loop,
 						"name": name,
 						"status": status
 					}
 				})
 				
 				if (status == "on"):
 					break;
@@ -106,18 +108,20 @@
 			continue;
 			
 		if (kind == "task"):
 			adventure_script ()
 			
 			loop = 0
 			while True:
-				status = venture ["is on"] ()		
+				status = adventure ["is on"] ()		
 				rich.print_json (data = {
-					"status check": {
-						"name": venture ["name"],
+					"venture status check loop": {
+						"when": "after turn on was sent",
+						"loop": loop,
+						"name": name,
 						"status": status
 					}
 				})
 				
 				if (status == "on"):
 					break;
```

### Comparing `ventures-1.0.0/venues/stages/ventures/readme.md` & `ventures-1.1.0/venues/stages/ventures/readme.md`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 17 22:33:48 2024 UTC, .py size: 732 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,107 @@
-00000000: 6f0d 0d0a 0000 0000 4cdb 4766 dc02 0000  o.......L.Gf....
+00000000: 6f0d 0d0a 0000 0000 eec4 4a66 8e08 0000  o.........Jf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
-00000050: 6402 6c05 5a05 6401 6402 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
-00000060: 6402 6c07 5a07 6401 6402 6c08 5a08 6404  d.l.Z.d.d.l.Z.d.
-00000070: 6405 8400 5a09 6406 6407 8400 5a0a 6408  d...Z.d.d...Z.d.
-00000080: 6409 8400 5a0b 6402 5300 290a 7a6b 0a09  d...Z.d.S.).zk..
-00000090: 6672 6f6d 2076 6163 6369 6e65 732e 6d69  from vaccines.mi
-000000a0: 7865 732e 7665 6e74 7572 6573 5f6d 6170  xes.ventures_map
-000000b0: 2e68 696b 655f 7061 7373 6976 6520 696d  .hike_passive im
-000000c0: 706f 7274 2068 696b 655f 7061 7373 6976  port hike_passiv
-000000d0: 650a 0968 696b 655f 7061 7373 6976 6520  e..hike_passive 
-000000e0: 280a 0909 7363 7269 7074 203d 205b 0a09  (...script = [..
-000000f0: 090a 0909 5d0a 0929 0ae9 0000 0000 4e29  ....]..)......N)
-00000100: 01da 0846 7261 6374 696f 6e63 0100 0000  ...Fractionc....
-00000110: 0000 0000 0000 0000 0100 0000 0500 0000  ................
-00000120: 0300 0000 732a 0000 0074 00a0 017c 00a1  ....s*...t...|..
-00000130: 0189 0074 02a0 0387 0066 0164 0164 0284  ...t.....f.d.d..
-00000140: 08a1 0101 0074 04a0 0564 03a1 0101 0088  .....t...d......
-00000150: 0053 0029 044e 6300 0000 0000 0000 0000  .S.).Nc.........
-00000160: 0000 0000 0000 0002 0000 0013 0000 0073  ...............s
-00000170: 0800 0000 8800 a000 a100 5300 a901 4e29  ..........S...N)
-00000180: 01da 0974 6572 6d69 6e61 7465 a900 a901  ...terminate....
-00000190: da0b 7468 655f 7072 6f63 6573 7372 0500  ..the_processr..
-000001a0: 0000 fa42 2f68 6162 6974 6174 2f76 656e  ...B/habitat/ven
-000001b0: 7565 732f 7374 6167 6573 2f76 656e 7475  ues/stages/ventu
-000001c0: 7265 732f 7574 696c 6974 6965 732f 6869  res/utilities/hi
-000001d0: 6b65 5f70 6173 7369 7665 2f5f 5f69 6e69  ke_passive/__ini
-000001e0: 745f 5f2e 7079 da08 3c6c 616d 6264 613e  t__.py..<lambda>
-000001f0: 2200 0000 7302 0000 0008 007a 1a65 7870  "...s......z.exp
-00000200: 6c69 6369 742e 3c6c 6f63 616c 733e 2e3c  licit.<locals>.<
-00000210: 6c61 6d62 6461 3ee9 0500 0000 2906 da0a  lambda>.....)...
-00000220: 7375 6270 726f 6365 7373 da05 506f 7065  subprocess..Pope
-00000230: 6eda 0661 7465 7869 74da 0872 6567 6973  n..atexit..regis
-00000240: 7465 72da 0474 696d 65da 0573 6c65 6570  ter..time..sleep
-00000250: 2901 da06 7363 7269 7074 7205 0000 0072  )...scriptr....r
-00000260: 0600 0000 7208 0000 00da 0865 7870 6c69  ....r......expli
-00000270: 6369 7420 0000 0073 0800 0000 0a01 1201  cit ...s........
-00000280: 0a01 0402 7212 0000 0063 0100 0000 0000  ....r....c......
-00000290: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-000002a0: 0000 730e 0000 0074 00a0 017c 00a1 017d  ..s....t...|...}
-000002b0: 017c 0153 0072 0300 0000 2902 720b 0000  .|.S.r....).r...
-000002c0: 0072 0c00 0000 2902 7211 0000 0072 0700  .r....).r....r..
-000002d0: 0000 7205 0000 0072 0500 0000 7208 0000  ..r....r....r...
-000002e0: 00da 0869 6d70 6c69 6369 742b 0000 0073  ...implicit+...s
-000002f0: 0800 0000 0401 0201 04ff 0403 7213 0000  ............r...
-00000300: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
-00000310: 0000 0300 0000 4300 0000 7326 0000 007c  ......C...s&...|
-00000320: 0064 0119 007d 0174 00a0 017c 01a1 017d  .d...}.t...|...}
-00000330: 0274 0264 027c 0283 0201 0064 037c 026a  .t.d.|.....d.|.j
-00000340: 0369 0153 0029 044e 7211 0000 007a 0c74  .i.S.).Nr....z.t
-00000350: 6865 5f70 726f 6365 7373 3ada 1070 726f  he_process:..pro
-00000360: 6365 7373 5f69 6465 6e74 6974 7929 0472  cess_identity).r
-00000370: 0b00 0000 720c 0000 00da 0570 7269 6e74  ....r......print
-00000380: da03 7069 6429 03da 0670 6163 6b65 7472  ..pid)...packetr
-00000390: 1100 0000 7207 0000 0072 0500 0000 7205  ....r....r....r.
-000003a0: 0000 0072 0800 0000 da0c 6869 6b65 5f70  ...r......hike_p
-000003b0: 6173 7369 7665 3100 0000 730e 0000 0008  assive1...s.....
-000003c0: 0104 0202 0104 ff0a 0406 0304 ff72 1800  .............r..
-000003d0: 0000 290c da07 5f5f 646f 635f 5fda 0472  ..)...__doc__..r
-000003e0: 6963 68da 0966 7261 6374 696f 6e73 7202  ich..fractionsr.
-000003f0: 0000 00da 0f6d 756c 7469 7072 6f63 6573  .....multiproces
-00000400: 7369 6e67 720b 0000 0072 0f00 0000 da02  singr....r......
-00000410: 6f73 720d 0000 0072 1200 0000 7213 0000  osr....r....r...
-00000420: 0072 1800 0000 7205 0000 0072 0500 0000  .r....r....r....
-00000430: 7205 0000 0072 0800 0000 da08 3c6d 6f64  r....r......<mod
-00000440: 756c 653e 0100 0000 7316 0000 0004 0a08  ule>....s.......
-00000450: 090c 0208 0108 0108 0108 0108 0108 0508  ................
-00000460: 0b0c 06                                  ...
+00000020: 0002 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
+00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
+00000040: 6401 6403 6c03 6d04 5a04 0100 6401 6404  d.d.l.m.Z...d.d.
+00000050: 6c05 5a05 6401 6405 6c06 6d07 5a07 0100  l.Z.d.d.l.m.Z...
+00000060: 6401 6404 6c08 5a08 6401 6404 6c09 5a09  d.d.l.Z.d.d.l.Z.
+00000070: 6401 6404 6c0a 5a0a 6401 6404 6c0b 5a0b  d.d.l.Z.d.d.l.Z.
+00000080: 6401 6404 6c0c 5a0c 6401 6404 6c0b 5a0b  d.d.l.Z.d.d.l.Z.
+00000090: 6401 6404 6c0d 5a0d 6401 6404 6c09 5a09  d.d.l.Z.d.d.l.Z.
+000000a0: 6406 6407 8400 5a0e 6404 5300 2908 7a6e  d.d...Z.d.S.).zn
+000000b0: 0a09 6672 6f6d 2076 6163 6369 6e65 732e  ..from vaccines.
+000000c0: 6d69 7865 732e 7665 6e74 7572 6573 5f6d  mixes.ventures_m
+000000d0: 6170 2e68 696b 655f 7061 7373 6976 6520  ap.hike_passive 
+000000e0: 696d 706f 7274 2068 696b 655f 7061 7373  import hike_pass
+000000f0: 6976 650a 0968 696b 655f 7061 7373 6976  ive..hike_passiv
+00000100: 6520 287b 0a09 0922 7363 7269 7074 223a  e ({..."script":
+00000110: 205b 0a09 090a 0909 5d0a 097d 290a e900   [......]..})...
+00000120: 0000 0029 01da 1568 696b 655f 7061 7373  ...)...hike_pass
+00000130: 6976 655f 705f 6578 7065 6374 2901 da13  ive_p_expect)...
+00000140: 7072 6f63 6573 735f 6f6e 5f69 6d70 6c69  process_on_impli
+00000150: 6369 744e 2901 da08 4672 6163 7469 6f6e  citN)...Fraction
+00000160: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
+00000170: 0004 0000 0003 0000 0073 3400 0000 7c00  .........s4...|.
+00000180: 6401 1900 7d01 6402 6403 8400 8900 8700  d...}.d.d.......
+00000190: 6601 6404 6405 8408 7d02 7400 6a01 7c01  f.d.d...}.t.j.|.
+000001a0: 6406 6407 8d02 7d03 6408 7c03 6a02 6901  d.d...}.d.|.j.i.
+000001b0: 5300 2909 4eda 0673 6372 6970 7463 0000  S.).N..scriptc..
+000001c0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000001d0: 0000 5300 0000 739c 0000 0074 00a0 01a1  ..S...s....t....
+000001e0: 007d 007c 0064 016b 0472 0d74 02a0 0364  .}.|.d.k.r.t...d
+000001f0: 01a1 0101 0074 00a0 04a1 0001 0074 00a0  .....t.......t..
+00000200: 01a1 007d 007c 0064 016b 0472 1e74 02a0  ...}.|.d.k.r.t..
+00000210: 0364 01a1 0101 0074 00a0 0564 02a1 0101  .d.....t...d....
+00000220: 0074 00a0 0664 01a1 0101 0074 026a 07a0  .t...d.....t.j..
+00000230: 08a1 0001 0074 026a 09a0 08a1 0001 0074  .....t.j.......t
+00000240: 026a 0aa0 08a1 0001 0074 0b74 006a 0c64  .j.......t.t.j.d
+00000250: 0383 0274 025f 0774 0b74 006a 0c64 0483  ...t._.t.t.j.d..
+00000260: 0274 025f 0974 0b74 006a 0c64 0483 0274  .t._.t.t.j.d...t
+00000270: 025f 0a64 0053 0029 054e 7201 0000 00fa  ._.d.S.).Nr.....
+00000280: 012f da01 72da 0177 290d da02 6f73 da04  ./..r..w)...os..
+00000290: 666f 726b da03 7379 73da 0465 7869 74da  fork..sys..exit.
+000002a0: 0673 6574 7369 64da 0563 6864 6972 da05  .setsid..chdir..
+000002b0: 756d 6173 6bda 0573 7464 696e da05 636c  umask..stdin..cl
+000002c0: 6f73 65da 0673 7464 6f75 74da 0673 7464  ose..stdout..std
+000002d0: 6572 72da 046f 7065 6eda 0764 6576 6e75  err..open..devnu
+000002e0: 6c6c 2901 da03 7069 64a9 0072 1700 0000  ll)...pid..r....
+000002f0: fa42 2f68 6162 6974 6174 2f76 656e 7565  .B/habitat/venue
+00000300: 732f 7374 6167 6573 2f76 656e 7475 7265  s/stages/venture
+00000310: 732f 7574 696c 6974 6965 732f 6869 6b65  s/utilities/hike
+00000320: 5f70 6173 7369 7665 2f5f 5f69 6e69 745f  _passive/__init_
+00000330: 5f2e 7079 da09 6461 656d 6f6e 697a 6531  _.py..daemonize1
+00000340: 0000 0073 1e00 0000 0802 0801 0a02 0803  ...s............
+00000350: 0803 0801 0a02 0a03 0a03 0a03 0a01 0a01  ................
+00000360: 0e03 0e01 1201 7a1f 6869 6b65 5f70 6173  ......z.hike_pas
+00000370: 7369 7665 2e3c 6c6f 6361 6c73 3e2e 6461  sive.<locals>.da
+00000380: 656d 6f6e 697a 6563 0100 0000 0000 0000  emonizec........
+00000390: 0000 0000 0400 0000 0400 0000 1300 0000  ................
+000003a0: 734a 0000 007c 0064 0119 007d 0174 00a0  sJ...|.d...}.t..
+000003b0: 01a1 007d 027c 0264 026b 0272 2388 0083  ...}.|.d.k.r#...
+000003c0: 0001 0074 026a 037c 0164 0364 048d 027d  ...t.j.|.d.d...}
+000003d0: 0374 0464 057c 036a 0583 0201 0074 00a0  .t.d.|.j.....t..
+000003e0: 0664 02a1 0101 0064 0053 007c 0253 0029  .d.....d.S.|.S.)
+000003f0: 064e 7205 0000 0072 0100 0000 5429 01da  .Nr....r....T)..
+00000400: 0573 6865 6c6c 7a33 0a09 0909 0a09 0909  .shellz3........
+00000410: 0a09 0909 0963 6869 6c64 2070 726f 6365  .....child proce
+00000420: 7373 2070 6964 3a0a 0909 0909 0a09 0909  ss pid:.........
+00000430: 090a 0909 0909 0a09 0909 0929 0772 0900  ...........).r..
+00000440: 0000 720a 0000 00da 0a73 7562 7072 6f63  ..r......subproc
+00000450: 6573 73da 0550 6f70 656e da05 7072 696e  ess..Popen..prin
+00000460: 7472 1600 0000 da05 5f65 7869 7429 04da  tr......_exit)..
+00000470: 0763 6f6d 6d61 6e64 7205 0000 0072 1600  .commandr....r..
+00000480: 0000 da0b 7468 655f 7072 6f63 6573 73a9  ....the_process.
+00000490: 0172 1900 0000 7217 0000 0072 1800 0000  .r....r....r....
+000004a0: da16 7374 6172 745f 6465 7461 6368 6564  ..start_detached
+000004b0: 5f70 726f 6365 7373 5100 0000 7314 0000  _processQ...s...
+000004c0: 0008 0108 0308 0206 030e 0204 0204 0704  ................
+000004d0: f90e 0a04 047a 2c68 696b 655f 7061 7373  .....z,hike_pass
+000004e0: 6976 652e 3c6c 6f63 616c 733e 2e73 7461  ive.<locals>.sta
+000004f0: 7274 5f64 6574 6163 6865 645f 7072 6f63  rt_detached_proc
+00000500: 6573 7354 2901 da09 636c 6f73 655f 6664  essT)...close_fd
+00000510: 73da 1070 726f 6365 7373 5f69 6465 6e74  s..process_ident
+00000520: 6974 7929 0572 1b00 0000 721c 0000 0072  ity).r....r....r
+00000530: 1600 0000 da04 6a6f 696e 721d 0000 0029  ......joinr....)
+00000540: 05da 0670 6163 6b65 7472 0500 0000 7222  ...packetr....r"
+00000550: 0000 0072 2000 0000 da14 6465 7461 6368  ...r .....detach
+00000560: 6564 5f70 726f 6365 7373 5f70 6964 7217  ed_process_pidr.
+00000570: 0000 0072 2100 0000 7218 0000 00da 0c68  ...r!...r......h
+00000580: 696b 655f 7061 7373 6976 652e 0000 0073  ike_passive....s
+00000590: 1200 0000 0801 0802 0c20 041f 0201 0201  ......... ......
+000005a0: 06fe 0606 04ff 7228 0000 0029 0fda 075f  ......r(...)..._
+000005b0: 5f64 6f63 5f5f da28 7665 6e74 7572 6573  _doc__.(ventures
+000005c0: 2e75 7469 6c69 7469 6573 2e68 696b 655f  .utilities.hike_
+000005d0: 7061 7373 6976 655f 705f 6578 7065 6374  passive_p_expect
+000005e0: 7202 0000 00da 3376 656e 7475 7265 732e  r.....3ventures.
+000005f0: 7574 696c 6974 6965 732e 6869 6b65 5f70  utilities.hike_p
+00000600: 6173 7369 7665 5f70 5f65 7870 6563 745f  assive_p_expect_
+00000610: 322e 696d 706c 6963 6974 7203 0000 00da  2.implicitr.....
+00000620: 0472 6963 68da 0966 7261 6374 696f 6e73  .rich..fractions
+00000630: 7204 0000 00da 0f6d 756c 7469 7072 6f63  r......multiproc
+00000640: 6573 7369 6e67 721b 0000 00da 0474 696d  essingr......tim
+00000650: 6572 0900 0000 da06 6174 6578 6974 720b  er......atexitr.
+00000660: 0000 0072 2800 0000 7217 0000 0072 1700  ...r(...r....r..
+00000670: 0000 7217 0000 0072 1800 0000 da08 3c6d  ..r....r......<m
+00000680: 6f64 756c 653e 0100 0000 731e 0000 0004  odule>....s.....
+00000690: 0a02 090c 060c 0108 030c 0308 0108 0108  ................
+000006a0: 0108 0108 0108 0108 0108 010c 05         .............
```

### Comparing `ventures-1.0.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/utilities/map/__pycache__/etch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/utilities/p_expect/__init__.py` & `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect_2/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 
 '''
+	from vaccines.mixes.ventures_map.hike_passive_p_expect import hike_passive_p_expect
+	hike_passive_p_expect ({
+		"script": [
+		
+		]
+	})
+'''
+
+'''
 	from biotech.topics.process_on.p_expect import process_on
 
 	env = os.environ.copy ()
 	env ["PYTHONPATH"] = ":".join (sys.path)
 	the_venture = process_on (
 		env = env
 	)
 	
 	the_records = venture ["records"] ()
 	for obj in the_queue:
 		print ("UTF8:", obj ["UTF8"] ["line"], end = '')
 '''
 
+#++++
+#
 import pexpect
 import rich
-
+#
+#
 import atexit
 import os
-
 from multiprocessing import Process, Queue
+#
+#++++
 
 def off (venture):
 	try:
 		print ("""
 		
 			attemping to stop the tethered venture
```

### Comparing `ventures-1.0.0/venues/stages/ventures/utilities/p_expect/__pycache__/background.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/utilities/p_expect/__pycache__/implicit.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/utilities/p_expect/__pycache__/parse_records.cpython-310.pyc` & `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/utilities/p_expect/implicit.py` & `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/utilities/p_expect/parse_records.py` & `ventures-1.1.0/venues/stages/ventures/utilities/hike_passive_p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py` & `ventures-1.1.0/venues/stages/ventures/utilities/process/check_is_on_cycle.py`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/venues/stages/ventures/ventures_map.S.HTML` & `ventures-1.1.0/venues/stages/ventures/ventures_map.S.HTML`

 * *Files identical despite different names*

### Comparing `ventures-1.0.0/PKG-INFO` & `ventures-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ventures
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 License: licensed
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

