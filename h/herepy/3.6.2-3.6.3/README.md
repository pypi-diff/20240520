# Comparing `tmp/herepy-3.6.2.tar.gz` & `tmp/herepy-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herepy-3.6.2.tar", last modified: Sat Apr  6 19:03:19 2024, max compression
+gzip compressed data, was "herepy-3.6.3.tar", last modified: Mon May 20 07:29:28 2024, max compression
```

## Comparing `herepy-3.6.2.tar` & `herepy-3.6.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.662596 herepy-3.6.2/
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1071 2023-09-13 13:06:01.000000 herepy-3.6.2/COPYING
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1071 2023-09-13 13:06:01.000000 herepy-3.6.2/LICENSE
--rw-r--r--   0 abdullahselek   (501) staff       (20)      118 2023-09-13 13:06:01.000000 herepy-3.6.2/MANIFEST.in
--rw-r--r--   0 abdullahselek   (501) staff       (20)       91 2023-09-13 13:06:01.000000 herepy-3.6.2/NOTICE
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6756 2024-04-06 19:03:19.662527 herepy-3.6.2/PKG-INFO
--rw-r--r--   0 abdullahselek   (501) staff       (20)     5574 2023-09-13 13:06:01.000000 herepy-3.6.2/README.rst
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.658762 herepy-3.6.2/herepy/
--rw-r--r--   0 abdullahselek   (501) staff       (20)     3420 2024-04-06 19:00:51.000000 herepy-3.6.2/herepy/__init__.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     5846 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/destination_weather_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      754 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/error.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    10908 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/ev_charging_stations_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     8642 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/fleet_telematics_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4792 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/geocoder_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2905 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/geocoder_autocomplete_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2537 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/geocoder_reverse_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      730 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/here_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    12999 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/here_enum.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    13901 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/isoline_routing_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     8695 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/map_image_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4861 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/map_tile_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      734 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/mercator_projection.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    10149 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/models.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     3816 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/objects.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4273 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/places_api.py
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.659555 herepy-3.6.2/herepy/platform/
--rw-r--r--   0 abdullahselek   (501) staff       (20)       47 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/platform/__init__.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      544 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/platform/tour_planning_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     5819 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/polling.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    15370 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/public_transit_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)        0 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/py.typed
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2531 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/rme_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    40099 2024-04-06 18:43:16.000000 herepy-3.6.2/herepy/routing_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    12825 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/traffic_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2047 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/utils.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4021 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/vector_tile_api.py
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.662303 herepy-3.6.2/herepy.egg-info/
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6756 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/PKG-INFO
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1447 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/SOURCES.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)        1 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/dependency_links.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)       20 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/requires.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)        7 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/top_level.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)       20 2024-03-31 17:22:24.000000 herepy-3.6.2/requirements.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)      235 2024-04-06 19:03:19.662836 herepy-3.6.2/setup.cfg
--rwxr-xr-x   0 abdullahselek   (501) staff       (20)     2072 2024-03-31 17:36:07.000000 herepy-3.6.2/setup.py
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.662121 herepy-3.6.2/tests/
--rw-r--r--   0 abdullahselek   (501) staff       (20)     7759 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_destination_weather_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    29190 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_enum.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6286 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_ev_charging_stations_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     7156 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_fleet_telematics_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4614 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_geocoder_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2690 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_geocoder_autocomplete_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1556 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_geocoder_reverse_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    14367 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_isoline_routing_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6013 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_map_image_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    14479 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_map_tile_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      366 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_mercator_projection.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6811 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_models.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     3559 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_places_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    14931 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_publictransit_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1616 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_rme_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    45084 2024-04-06 18:44:02.000000 herepy-3.6.2/tests/test_routing_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    16597 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_traffic_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      957 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_utils.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2718 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_vector_tile_api.py
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-05-20 07:29:28.766458 herepy-3.6.3/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1071 2023-09-13 13:06:01.000000 herepy-3.6.3/COPYING
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1071 2023-09-13 13:06:01.000000 herepy-3.6.3/LICENSE
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      118 2023-09-13 13:06:01.000000 herepy-3.6.3/MANIFEST.in
+-rw-r--r--   0 abdullahselek   (501) staff       (20)       91 2023-09-13 13:06:01.000000 herepy-3.6.3/NOTICE
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6756 2024-05-20 07:29:28.766388 herepy-3.6.3/PKG-INFO
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     5574 2023-09-13 13:06:01.000000 herepy-3.6.3/README.rst
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-05-20 07:29:28.761399 herepy-3.6.3/herepy/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     3420 2024-05-20 07:07:48.000000 herepy-3.6.3/herepy/__init__.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     5846 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/destination_weather_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      754 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/error.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    10908 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/ev_charging_stations_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     8642 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/fleet_telematics_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     4916 2024-05-20 07:07:10.000000 herepy-3.6.3/herepy/geocoder_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2905 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/geocoder_autocomplete_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2537 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/geocoder_reverse_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      730 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/here_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    12999 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/here_enum.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    13901 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/isoline_routing_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     8695 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/map_image_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     4861 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/map_tile_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      734 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/mercator_projection.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    10149 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/models.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     3816 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/objects.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     4273 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/places_api.py
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-05-20 07:29:28.762257 herepy-3.6.3/herepy/platform/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)       47 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/platform/__init__.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      544 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/platform/tour_planning_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     5819 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/polling.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    15370 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/public_transit_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)        0 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/py.typed
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2531 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/rme_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    40829 2024-05-20 07:07:10.000000 herepy-3.6.3/herepy/routing_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    12825 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/traffic_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2047 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/utils.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     4021 2023-09-13 13:06:01.000000 herepy-3.6.3/herepy/vector_tile_api.py
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-05-20 07:29:28.766144 herepy-3.6.3/herepy.egg-info/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6756 2024-05-20 07:29:28.000000 herepy-3.6.3/herepy.egg-info/PKG-INFO
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1447 2024-05-20 07:29:28.000000 herepy-3.6.3/herepy.egg-info/SOURCES.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)        1 2024-05-20 07:29:28.000000 herepy-3.6.3/herepy.egg-info/dependency_links.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)       20 2024-05-20 07:29:28.000000 herepy-3.6.3/herepy.egg-info/requires.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)        7 2024-05-20 07:29:28.000000 herepy-3.6.3/herepy.egg-info/top_level.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)       20 2024-03-31 17:22:24.000000 herepy-3.6.3/requirements.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      235 2024-05-20 07:29:28.766714 herepy-3.6.3/setup.cfg
+-rwxr-xr-x   0 abdullahselek   (501) staff       (20)     2072 2024-03-31 17:36:07.000000 herepy-3.6.3/setup.py
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-05-20 07:29:28.765950 herepy-3.6.3/tests/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     7759 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_destination_weather_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    29190 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_enum.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6286 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_ev_charging_stations_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     7156 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_fleet_telematics_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     5991 2024-05-20 07:07:10.000000 herepy-3.6.3/tests/test_geocoder_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2690 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_geocoder_autocomplete_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1556 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_geocoder_reverse_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    14367 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_isoline_routing_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6013 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_map_image_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    14479 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_map_tile_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      366 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_mercator_projection.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6811 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_models.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     3559 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_places_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    14931 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_publictransit_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1616 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_rme_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    45692 2024-05-20 07:07:10.000000 herepy-3.6.3/tests/test_routing_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    16597 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_traffic_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      957 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_utils.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2718 2023-09-13 13:06:01.000000 herepy-3.6.3/tests/test_vector_tile_api.py
```

### Comparing `herepy-3.6.2/COPYING` & `herepy-3.6.3/COPYING`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/LICENSE` & `herepy-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/PKG-INFO` & `herepy-3.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herepy
-Version: 3.6.2
+Version: 3.6.3
 Summary: A library that provides a Python interface to the HERE APIs
 Home-page: https://github.com/abdullahselek/HerePy
 Download-URL: https://pypi.org/pypi/herepy
 Author: Abdullah Selek
 Author-email: abdullahselek.os@gmail.com
 Maintainer: Abdullah Selek
 Maintainer-email: abdullahselek.os@gmail.com
```

### Comparing `herepy-3.6.2/README.rst` & `herepy-3.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/__init__.py` & `herepy-3.6.3/herepy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """A library that provides a Python interface to the HERE APIs"""
 
 __author__ = "Abdullah Selek"
 __email__ = "abdullahselek.os@gmail.com"
 __copyright__ = "Copyright (c) 2017 Abdullah Selek"
 __license__ = "MIT License"
-__version__ = "3.6.2"
+__version__ = "3.6.3"
 __url__ = "https://github.com/abdullahselek/HerePy"
 __download_url__ = "https://pypi.org/pypi/herepy"
 __description__ = "A library that provides a Python interface to the HERE APIs"
 
 
 import json
```

### Comparing `herepy-3.6.2/herepy/destination_weather_api.py` & `herepy-3.6.3/herepy/destination_weather_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/error.py` & `herepy-3.6.3/herepy/error.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/ev_charging_stations_api.py` & `herepy-3.6.3/herepy/ev_charging_stations_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/fleet_telematics_api.py` & `herepy-3.6.3/herepy/fleet_telematics_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/geocoder_api.py` & `herepy-3.6.3/herepy/geocoder_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,19 +102,19 @@
             "apiKey": self._api_key,
             "lang": lang,
         }
         return self.__get(data)
 
     def address_with_details(
         self,
-        house_number: int,
-        street: str,
         city: str,
         country: str,
         lang: str = "en-US",
+        house_number: Optional[int] = None,
+        street: Optional[str] = None,
     ) -> Optional[GeocoderResponse]:
         """Geocodes with given address details
         Args:
           house_number (int):
             house number.
           street (str):
             street name.
@@ -125,19 +125,24 @@
           lang (str):
             BCP47 compliant Language Code.
         Returns:
           GeocoderResponse
         Raises:
           HEREError"""
 
+        qq_query = ""
+        if house_number is not None:
+            qq_query += f"houseNumber={house_number};"
+        if street is not None:
+            qq_query += f"street={street};"
+        qq_query += f"city={city};"
+        qq_query += f"country={country}"
+
         data = {
-            "qq": str.format("houseNumber={0};", house_number)
-            + str.format("street={0};", street)
-            + str.format("city={0};", city)
-            + str.format("country={0}", country),
+            "qq": qq_query,
             "apiKey": self._api_key,
             "lang": lang,
         }
         return self.__get(data)
 
     def street_intersection(
         self, street: str, city: str, lang: str = "en-US"
```

### Comparing `herepy-3.6.2/herepy/geocoder_autocomplete_api.py` & `herepy-3.6.3/herepy/geocoder_autocomplete_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/geocoder_reverse_api.py` & `herepy-3.6.3/herepy/geocoder_reverse_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/here_api.py` & `herepy-3.6.3/herepy/here_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/here_enum.py` & `herepy-3.6.3/herepy/here_enum.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/isoline_routing_api.py` & `herepy-3.6.3/herepy/isoline_routing_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/map_image_api.py` & `herepy-3.6.3/herepy/map_image_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/map_tile_api.py` & `herepy-3.6.3/herepy/map_tile_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/mercator_projection.py` & `herepy-3.6.3/herepy/mercator_projection.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/models.py` & `herepy-3.6.3/herepy/models.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/objects.py` & `herepy-3.6.3/herepy/objects.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/places_api.py` & `herepy-3.6.3/herepy/places_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/platform/tour_planning_api.py` & `herepy-3.6.3/herepy/platform/tour_planning_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/polling.py` & `herepy-3.6.3/herepy/polling.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/public_transit_api.py` & `herepy-3.6.3/herepy/public_transit_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/rme_api.py` & `herepy-3.6.3/herepy/rme_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/routing_api.py` & `herepy-3.6.3/herepy/routing_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -978,38 +978,70 @@
     RouteId. In every case a mitigation is to re-run CalculateRoute request to
     acquire a new proper RouteId.
     """
 
 
 # pylint: disable=R0911
 def error_from_routing_service_error(json_data):
-    """Return the correct subclass for routing errors"""
+    """Return the correct error class for routing errors."""
 
-    # V8 error handling
-    if "error" in json_data and json_data["error"] == "Unauthorized":
-        return InvalidCredentialsError(json_data["error_description"])
+    if "error" in json_data:
+        return _auth_error(json_data)
     elif "status" in json_data:
-        error_msg = str.format(
-            "Cause: {0}; Action: {1}", json_data["cause"], json_data["action"]
-        )
-        if json_data["status"] == 400:
-            return InvalidRequestError(error_msg)
-        elif json_data["status"] == 403:
-            return AccessDeniedError(error_msg)
-
-    # V7 error handling
-    if "subtype" in json_data:
-        subtype = json_data["subtype"]
-        details = json_data["details"]
-
-        if subtype == "InvalidInputData":
-            return InvalidInputDataError(details)
-        if subtype == "WaypointNotFound":
-            return WaypointNotFoundError(details)
-        if subtype == "NoRouteFound":
-            return NoRouteFoundError(details)
-        if subtype == "LinkIdNotFound":
-            return LinkIdNotFoundError(details)
-        if subtype == "RouteNotReconstructed":
-            return RouteNotReconstructedError(details)
-    # pylint: disable=W0212
-    return HEREError("Error occurred on " + sys._getframe(1).f_code.co_name)
+        return _status_error(json_data)
+    elif "subtype" in json_data:
+        return _request_error(json_data)
+    else:
+        return _default_error(json_data)
+      
+
+def _auth_error(json_data):
+    """ 'error' in response data, return appropriate error."""
+
+    error_type = json_data["error"]
+    
+    if error_type in ["Unauthorized", "Forbidden"]:
+        return InvalidCredentialsError(json_data["error_description"])
+    else:
+        return _default_error(json_data)
+
+
+def _status_error(json_data):
+    """ 'status' in response data, return appropriate error."""
+
+    error_msg = f"Cause: {json_data['cause']}; Action: {json_data['action']}"
+    status_code = json_data["status"]
+    if status_code == 400:
+        return InvalidRequestError(error_msg)
+    elif status_code == 403:
+        return AccessDeniedError(error_msg)
+    else:
+        return _default_error(json_data)
+
+
+
+def _request_error(json_data):
+    """ 'subtype' in error response, return appropriate response"""
+
+    subtype = json_data["subtype"]
+    details = json_data["details"]
+
+    if subtype == "InvalidInputData":
+        return InvalidInputDataError(details)
+    elif subtype == "WaypointNotFound":
+        return WaypointNotFoundError(details)
+    elif subtype == "NoRouteFound":
+        return NoRouteFoundError(details)
+    elif subtype == "LinkIdNotFound":
+        return LinkIdNotFoundError(details)
+    elif subtype == "RouteNotReconstructed":
+        return RouteNotReconstructedError(details)
+    else:
+        return _default_error(json_data)
+
+
+def _default_error(json_data):
+  """ default response message when error type is unknown."""
+
+  function_name = sys._getframe(1).f_code.co_name
+  default_error_message = f"Error occurred on {function_name} - API Response: {json_data}" 
+  return HEREError(default_error_message)
```

### Comparing `herepy-3.6.2/herepy/traffic_api.py` & `herepy-3.6.3/herepy/traffic_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/utils.py` & `herepy-3.6.3/herepy/utils.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy/vector_tile_api.py` & `herepy-3.6.3/herepy/vector_tile_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/herepy.egg-info/PKG-INFO` & `herepy-3.6.3/herepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herepy
-Version: 3.6.2
+Version: 3.6.3
 Summary: A library that provides a Python interface to the HERE APIs
 Home-page: https://github.com/abdullahselek/HerePy
 Download-URL: https://pypi.org/pypi/herepy
 Author: Abdullah Selek
 Author-email: abdullahselek.os@gmail.com
 Maintainer: Abdullah Selek
 Maintainer-email: abdullahselek.os@gmail.com
```

### Comparing `herepy-3.6.2/herepy.egg-info/SOURCES.txt` & `herepy-3.6.3/herepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/setup.py` & `herepy-3.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_destination_weather_api.py` & `herepy-3.6.3/tests/test_destination_weather_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_enum.py` & `herepy-3.6.3/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_ev_charging_stations_api.py` & `herepy-3.6.3/tests/test_ev_charging_stations_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_fleet_telematics_api.py` & `herepy-3.6.3/tests/test_fleet_telematics_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_geocoder_api.py` & `herepy-3.6.3/tests/test_geocoder_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -86,19 +86,62 @@
             expectedResponse = f.read()
         responses.add(
             responses.GET,
             "https://geocode.search.hereapi.com/v1/geocode",
             expectedResponse,
             status=200,
         )
-        response = self._api.address_with_details(34, "Barbaros", "Istanbul", "Turkey")
+        response = self._api.address_with_details(
+            street="Barbaros",
+            city="Istanbul",
+            country="Turkey",
+            house_number=34
+        )
+        self.assertTrue(response)
+        self.assertIsInstance(response, herepy.GeocoderResponse)
+
+    @responses.activate
+    def test_address_with_detail_without_street(self):
+        with open("testdata/models/geocoder.json", "r") as f:
+            expected_response = f.read()
+        responses.add(
+            responses.GET,
+            "https://geocode.search.hereapi.com/v1/geocode",
+            expected_response,
+            status=200,
+        )
+        response = self._api.address_with_details(
+            city="Istanbul",
+            country="Turkey",
+            house_number=34,
+            street= None
+        )
         self.assertTrue(response)
         self.assertIsInstance(response, herepy.GeocoderResponse)
 
     @responses.activate
+    def test_address_with_detail_without_house_number(self):
+        with open("testdata/models/geocoder.json", "r") as f:
+            expected_response = f.read()
+        responses.add(
+            responses.GET,
+            "https://geocode.search.hereapi.com/v1/geocode",
+            expected_response,
+            status=200,
+        )
+        response = self._api.address_with_details(
+            street="Barbaros",
+            city="Istanbul",
+            country="Turkey",
+            house_number= None
+        )
+        self.assertTrue(response)
+        self.assertIsInstance(response, herepy.GeocoderResponse)
+        
+    @responses.activate
     def test_addresswithdetails_whenerroroccurred(self):
         with open("testdata/models/geocoder_error.json", "r") as f:
             expectedResponse = f.read()
         responses.add(
             responses.GET,
             "https://geocode.search.hereapi.com/v1/geocode",
             expectedResponse,
```

### Comparing `herepy-3.6.2/tests/test_geocoder_autocomplete_api.py` & `herepy-3.6.3/tests/test_geocoder_autocomplete_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_geocoder_reverse_api.py` & `herepy-3.6.3/tests/test_geocoder_reverse_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_isoline_routing_api.py` & `herepy-3.6.3/tests/test_isoline_routing_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_map_image_api.py` & `herepy-3.6.3/tests/test_map_image_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_map_tile_api.py` & `herepy-3.6.3/tests/test_map_tile_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_models.py` & `herepy-3.6.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_places_api.py` & `herepy-3.6.3/tests/test_places_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_publictransit_api.py` & `herepy-3.6.3/tests/test_publictransit_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_rme_api.py` & `herepy-3.6.3/tests/test_rme_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_routing_api.py` & `herepy-3.6.3/tests/test_routing_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,28 @@
             status=401,
         )
         api = herepy.RoutingApi("wrong_api_key", "wrong_app_code")
         with self.assertRaises(herepy.InvalidCredentialsError):
             api.car_route([11.0, 12.0], [22.0, 23.0])
 
     @responses.activate
+    def test_carroute_when_error_forbidden_credentials_occurred(self):
+        with open("testdata/models/routing_error_forbidden_credentials.json", "r") as f:
+            expectedResponse = f.read()
+        responses.add(
+            responses.GET,
+            "https://route.ls.hereapi.com/routing/7.2/calculateroute.json",
+            expectedResponse,
+            status=401,
+        )
+        api = herepy.RoutingApi("forbidden_api_key", "forbidden_app_code")
+        with self.assertRaises(herepy.InvalidCredentialsError):
+            api.car_route([11.0, 12.0], [22.0, 23.0])
+
+    @responses.activate
     def test_carroute_when_error_no_route_found_occurred(self):
         with open("testdata/models/routing_error_no_route_found.json", "r") as f:
             expectedResponse = f.read()
         responses.add(
             responses.GET,
             "https://route.ls.hereapi.com/routing/7.2/calculateroute.json",
             expectedResponse,
```

### Comparing `herepy-3.6.2/tests/test_traffic_api.py` & `herepy-3.6.3/tests/test_traffic_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_utils.py` & `herepy-3.6.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.2/tests/test_vector_tile_api.py` & `herepy-3.6.3/tests/test_vector_tile_api.py`

 * *Files identical despite different names*

