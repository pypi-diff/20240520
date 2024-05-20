# Comparing `tmp/dragon-city-utils-2.0.3.tar.gz` & `tmp/dragon_city_utils-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragon-city-utils-2.0.3.tar", last modified: Tue Feb  6 15:18:43 2024, max compression
+gzip compressed data, was "dragon_city_utils-2.1.0.tar", max compression
```

## Comparing `dragon-city-utils-2.0.3.tar` & `dragon_city_utils-2.1.0.tar`

### file list

```diff
@@ -1,65 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.539192 dragon-city-utils-2.0.3/
--rw-rw-rw-   0        0        0     8997 2024-02-06 15:18:43.530198 dragon-city-utils-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8627 2024-02-06 14:36:42.000000 dragon-city-utils-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.127148 dragon-city-utils-2.0.3/dcutils/
--rw-rw-rw-   0        0        0       59 2024-02-06 14:23:38.000000 dragon-city-utils-2.0.3/dcutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.132148 dragon-city-utils-2.0.3/dcutils/_utils/
--rw-rw-rw-   0        0        0        0 2024-02-06 14:56:22.000000 dragon-city-utils-2.0.3/dcutils/_utils/__init__.py
--rw-rw-rw-   0        0        0     1852 2024-02-06 13:49:09.000000 dragon-city-utils-2.0.3/dcutils/_utils/file.py
--rw-rw-rw-   0        0        0      405 2024-02-02 13:20:33.000000 dragon-city-utils-2.0.3/dcutils/dc_config.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.142156 dragon-city-utils-2.0.3/dcutils/static/
--rw-rw-rw-   0        0        0        0 2024-02-06 14:56:12.000000 dragon-city-utils-2.0.3/dcutils/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.145149 dragon-city-utils-2.0.3/dcutils/static/animations/
--rw-rw-rw-   0        0        0      169 2023-03-13 19:58:04.000000 dragon-city-utils-2.0.3/dcutils/static/animations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.377149 dragon-city-utils-2.0.3/dcutils/static/animations/flash/
--rw-rw-rw-   0        0        0      858 2024-02-06 14:21:18.000000 dragon-city-utils-2.0.3/dcutils/static/animations/flash/dragon.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.416150 dragon-city-utils-2.0.3/dcutils/static/animations/spine/
--rw-rw-rw-   0        0        0     1297 2024-02-06 14:23:08.000000 dragon-city-utils-2.0.3/dcutils/static/animations/spine/dragon.py
--rw-rw-rw-   0        0        0      258 2023-10-23 02:01:47.000000 dragon-city-utils-2.0.3/dcutils/static/base.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.160148 dragon-city-utils-2.0.3/dcutils/static/islands/
--rw-rw-rw-   0        0        0       67 2023-03-15 00:51:18.000000 dragon-city-utils-2.0.3/dcutils/static/islands/__init__.py
--rw-rw-rw-   0        0        0      506 2023-06-03 11:58:29.000000 dragon-city-utils-2.0.3/dcutils/static/islands/package.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.162150 dragon-city-utils-2.0.3/dcutils/static/localization/
--rw-rw-rw-   0        0        0     8032 2024-02-06 15:16:31.000000 dragon-city-utils-2.0.3/dcutils/static/localization/__init__.py
--rw-rw-rw-   0        0        0      139 2024-02-06 14:14:05.000000 dragon-city-utils-2.0.3/dcutils/static/platform_prefixes.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.170150 dragon-city-utils-2.0.3/dcutils/static/sounds/
--rw-rw-rw-   0        0        0       64 2023-03-13 22:09:33.000000 dragon-city-utils-2.0.3/dcutils/static/sounds/__init__.py
--rw-rw-rw-   0        0        0     7579 2023-10-23 02:01:41.000000 dragon-city-utils-2.0.3/dcutils/static/sounds/config.py
--rw-rw-rw-   0        0        0      818 2024-02-06 14:28:38.000000 dragon-city-utils-2.0.3/dcutils/static/sounds/musics.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.182149 dragon-city-utils-2.0.3/dcutils/static/sprites/
--rw-rw-rw-   0        0        0      256 2024-02-06 14:20:04.000000 dragon-city-utils-2.0.3/dcutils/static/sprites/__init__.py
--rw-rw-rw-   0        0        0      839 2024-02-06 14:20:04.000000 dragon-city-utils-2.0.3/dcutils/static/sprites/chest.py
--rw-rw-rw-   0        0        0     1178 2024-02-06 14:20:04.000000 dragon-city-utils-2.0.3/dcutils/static/sprites/dragon.py
--rw-rw-rw-   0        0        0      867 2024-02-06 14:20:04.000000 dragon-city-utils-2.0.3/dcutils/static/sprites/dragon_thumb.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.184150 dragon-city-utils-2.0.3/dcutils/tools/
--rw-rw-rw-   0        0        0        0 2023-05-01 12:40:11.000000 dragon-city-utils-2.0.3/dcutils/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.188150 dragon-city-utils-2.0.3/dcutils/tools/calculators/
--rw-rw-rw-   0        0        0        0 2023-03-07 21:06:47.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/__init__.py
--rw-rw-rw-   0        0        0     9468 2023-10-23 02:01:41.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/battle_simulator.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.194148 dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/
--rw-rw-rw-   0        0        0      162 2023-03-15 00:52:07.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.215152 dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/attack_damage/
--rw-rw-rw-   0        0        0     1251 2023-10-23 02:01:41.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/attack_damage/__init__.py
--rw-rw-rw-   0        0        0      429 2023-03-13 00:11:04.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/attack_damage/config.py
--rw-rw-rw-   0        0        0      131 2024-02-06 14:38:25.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/dragon_rarities.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.236151 dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/status/
--rw-rw-rw-   0        0        0     3722 2023-10-23 02:01:41.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/status/__init__.py
--rw-rw-rw-   0        0        0    63433 2023-03-12 23:55:40.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/status/config.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.248152 dragon-city-utils-2.0.3/dcutils/tools/calculators/elements/
--rw-rw-rw-   0        0        0      801 2023-10-23 02:01:41.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/elements/__init__.py
--rw-rw-rw-   0        0        0     2146 2023-05-04 21:25:49.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/elements/config.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.254151 dragon-city-utils-2.0.3/dcutils/tools/calculators/food/
--rw-rw-rw-   0        0        0      166 2023-10-23 02:01:41.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/food/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.337148 dragon-city-utils-2.0.3/dcutils/tools/calculators/orb_recall/
--rw-rw-rw-   0        0        0     1050 2023-10-23 02:01:41.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/orb_recall/__init__.py
--rw-rw-rw-   0        0        0      368 2023-03-12 22:38:45.000000 dragon-city-utils-2.0.3/dcutils/tools/calculators/orb_recall/config.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.361150 dragon-city-utils-2.0.3/dcutils/tools/url_parser/
--rw-rw-rw-   0        0        0        0 2023-04-21 21:30:31.000000 dragon-city-utils-2.0.3/dcutils/tools/url_parser/__init__.py
--rw-rw-rw-   0        0        0     3172 2023-10-23 02:01:41.000000 dragon-city-utils-2.0.3/dcutils/tools/url_parser/dragon.py
-drwxrwxrwx   0        0        0        0 2024-02-06 15:18:43.527205 dragon-city-utils-2.0.3/dragon_city_utils.egg-info/
--rw-rw-rw-   0        0        0     8997 2024-02-06 15:18:42.000000 dragon-city-utils-2.0.3/dragon_city_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2803 2024-02-06 15:18:42.000000 dragon-city-utils-2.0.3/dragon_city_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 15:18:42.000000 dragon-city-utils-2.0.3/dragon_city_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-02-06 15:18:42.000000 dragon-city-utils-2.0.3/dragon_city_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-06 15:18:43.539192 dragon-city-utils-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-02-06 15:18:41.000000 dragon-city-utils-2.0.3/setup.py
+-rw-r--r--   0        0        0        0 2024-05-20 00:15:42.691629 dragon_city_utils-2.1.0/dcutils/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-06 14:56:22.001825 dragon_city_utils-2.1.0/dcutils/_utils/__init__.py
+-rw-r--r--   0        0        0     1852 2024-02-06 13:49:09.756193 dragon_city_utils-2.1.0/dcutils/_utils/file_manager.py
+-rw-r--r--   0        0        0      364 2024-05-20 00:03:57.325731 dragon_city_utils-2.1.0/dcutils/dc_config.py
+-rw-r--r--   0        0        0        0 2024-02-06 14:56:12.192421 dragon_city_utils-2.1.0/dcutils/static/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-20 00:04:08.782600 dragon_city_utils-2.1.0/dcutils/static/animations/__init__.py
+-rw-r--r--   0        0        0      818 2024-05-20 00:04:12.694584 dragon_city_utils-2.1.0/dcutils/static/animations/flash/dragon.py
+-rw-r--r--   0        0        0     1257 2024-05-20 00:04:15.826468 dragon_city_utils-2.1.0/dcutils/static/animations/spine/dragon.py
+-rw-r--r--   0        0        0      218 2024-05-20 00:04:02.227368 dragon_city_utils-2.1.0/dcutils/static/base.py
+-rw-r--r--   0        0        0       34 2024-05-20 00:04:18.682061 dragon_city_utils-2.1.0/dcutils/static/islands/__init__.py
+-rw-r--r--   0        0        0      473 2024-05-20 00:04:22.004711 dragon_city_utils-2.1.0/dcutils/static/islands/package.py
+-rw-r--r--   0        0        0     7872 2024-05-20 00:26:05.212770 dragon_city_utils-2.1.0/dcutils/static/localization/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-20 00:04:05.944453 dragon_city_utils-2.1.0/dcutils/static/platform_prefixes.py
+-rw-r--r--   0        0        0       32 2024-05-20 00:04:27.863424 dragon_city_utils-2.1.0/dcutils/static/sounds/__init__.py
+-rw-r--r--   0        0        0     7569 2024-05-20 00:26:47.532975 dragon_city_utils-2.1.0/dcutils/static/sounds/config.py
+-rw-r--r--   0        0        0      786 2024-05-20 00:04:33.466317 dragon_city_utils-2.1.0/dcutils/static/sounds/musics.py
+-rw-r--r--   0        0        0      153 2024-05-20 00:04:36.496325 dragon_city_utils-2.1.0/dcutils/static/sprites/__init__.py
+-rw-r--r--   0        0        0      808 2024-05-20 00:04:38.935062 dragon_city_utils-2.1.0/dcutils/static/sprites/chest.py
+-rw-r--r--   0        0        0     1146 2024-05-20 00:04:44.136141 dragon_city_utils-2.1.0/dcutils/static/sprites/dragon.py
+-rw-r--r--   0        0        0      836 2024-05-20 00:04:41.736329 dragon_city_utils-2.1.0/dcutils/static/sprites/dragon_thumb.py
+-rw-r--r--   0        0        0        0 2023-05-01 12:40:11.011972 dragon_city_utils-2.1.0/dcutils/tools/__init__.py
+-rw-r--r--   0        0        0     3628 2024-05-20 12:25:58.937731 dragon_city_utils-2.1.0/dcutils/tools/ai/base.py
+-rw-r--r--   0        0        0     1564 2024-05-20 00:06:50.707849 dragon_city_utils-2.1.0/dcutils/tools/ai/elements_detector.py
+-rw-r--r--   0        0        0     1384 2024-05-20 00:05:28.724872 dragon_city_utils-2.1.0/dcutils/tools/ai/phase_detector.py
+-rw-r--r--   0        0        0        0 2023-03-07 21:06:47.706681 dragon_city_utils-2.1.0/dcutils/tools/calculators/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-20 00:05:31.955562 dragon_city_utils-2.1.0/dcutils/tools/calculators/dragon/__init__.py
+-rw-r--r--   0        0        0     1208 2024-05-20 00:05:34.447947 dragon_city_utils-2.1.0/dcutils/tools/calculators/dragon/attack_damage/__init__.py
+-rw-r--r--   0        0        0      428 2024-05-20 00:10:22.139051 dragon_city_utils-2.1.0/dcutils/tools/calculators/dragon/attack_damage/config.py
+-rw-r--r--   0        0        0      131 2024-02-06 14:38:25.723211 dragon_city_utils-2.1.0/dcutils/tools/calculators/dragon/dragon_rarities.py
+-rw-r--r--   0        0        0     3686 2024-05-20 00:05:46.082198 dragon_city_utils-2.1.0/dcutils/tools/calculators/dragon/status/__init__.py
+-rw-r--r--   0        0        0    63433 2023-03-12 23:55:40.514136 dragon_city_utils-2.1.0/dcutils/tools/calculators/dragon/status/config.py
+-rw-r--r--   0        0        0      729 2024-05-20 00:05:54.417926 dragon_city_utils-2.1.0/dcutils/tools/calculators/elements/__init__.py
+-rw-r--r--   0        0        0     2111 2024-05-20 00:05:57.330731 dragon_city_utils-2.1.0/dcutils/tools/calculators/elements/config.py
+-rw-r--r--   0        0        0      286 2024-02-29 04:52:58.872590 dragon_city_utils-2.1.0/dcutils/tools/calculators/food/__init__.py
+-rw-r--r--   0        0        0     4453 2024-02-29 04:50:27.913313 dragon_city_utils-2.1.0/dcutils/tools/calculators/food/config.py
+-rw-r--r--   0        0        0     9468 2023-10-23 02:01:41.959853 dragon_city_utils-2.1.0/dcutils/tools/calculators/old_battle_simulator.py
+-rw-r--r--   0        0        0     1009 2024-05-20 00:06:00.438032 dragon_city_utils-2.1.0/dcutils/tools/calculators/orb_recall/__init__.py
+-rw-r--r--   0        0        0      275 2024-05-20 00:06:03.804607 dragon_city_utils-2.1.0/dcutils/tools/calculators/orb_recall/config.py
+-rw-r--r--   0        0        0        0 2023-04-21 21:30:31.175986 dragon_city_utils-2.1.0/dcutils/tools/url_parser/__init__.py
+-rw-r--r--   0        0        0     3137 2024-05-20 00:03:54.465403 dragon_city_utils-2.1.0/dcutils/tools/url_parser/dragon.py
+-rw-r--r--   0        0        0      639 2024-05-20 12:28:16.638265 dragon_city_utils-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8627 2024-02-06 14:36:42.870242 dragon_city_utils-2.1.0/README.md
+-rw-r--r--   0        0        0     9052 1970-01-01 00:00:00.000000 dragon_city_utils-2.1.0/PKG-INFO
```

### Comparing `dragon-city-utils-2.0.3/PKG-INFO` & `dragon_city_utils-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: dragon-city-utils
-Version: 2.0.3
-Summary: Dragon City Utils, a collection of tools and utilities for managing static assets and performing calculations related to the Dragon City game.
-Author: Marcuth
-Author-email: example@gmail.com
-License: MIT License
-Keywords: dragoncity dcutils tools
-Description-Content-Type: text/markdown
-
 # dragon-city-utils
 
 Welcome to the documentation of Dragon City Utils, a collection of tools and utilities for managing static assets and performing calculations related to the game Dragon City. Below, you'll find detailed explanations and code snippets for various functionalities.
 
 ## Static Files
 
 ### Sprites
@@ -380,8 +370,8 @@
 
 Get the localization data as a dictionary.
 
 ```python
 loc_dict = loc.dict
 ```
 
-Feel free to explore these functionalities and integrate them into your projects!
+Feel free to explore these functionalities and integrate them into your projects!
```

### Comparing `dragon-city-utils-2.0.3/README.md` & `dragon_city_utils-2.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,377 +1,397 @@
-# dragon-city-utils
-
-Welcome to the documentation of Dragon City Utils, a collection of tools and utilities for managing static assets and performing calculations related to the game Dragon City. Below, you'll find detailed explanations and code snippets for various functionalities.
-
-## Static Files
-
-### Sprites
-
-#### Dragon Sprite
-
-You can download a dragon sprite using the following code:
-
-```python
-from dcutils.static.sprites import DragonSprite
-
-dragon_sprite = DragonSprite(
-    image_name = "1000_dragon_nature",
-    phase = 3,
-    skin = "skin1",
-    image_quality = 2
-)
-
-dragon_sprite.download(output="dragon_nature_sprite.png")
-```
-#### Dragon Thumb
-
-To download a dragon thumb:
-
-```python
-from dcutils.static.sprites import DragonThumb
-
-dragon_thumb = DragonThumb(
-    image_name = "1000_dragon_nature",
-    phase = 3,
-    skin = "skin1"
-)
-
-dragon_thumb.download(output="dragon_nature_thumb.png")
-```
-
-### Animations
-
-#### Dragon Animation (Flash Animation)
-
-To download a dragon flash animation:
-
-```python
-from dcutils.static.animations import DragonFlashAnimation
-
-dragon_flash_animation = DragonFlashAnimation(
-    image_name = "1000_dragon_nature",
-    phase = 3,
-    skin = "skin1"
-)
-
-dragon_flash_animation.download(output="dragon_nature_flash_animation.swf")
-```
-
-#### Dragon Animation (Spine Animation)
-
-To download a dragon spine animation:
-
-```python
-from dcutils.static.animations import DragonSpineAnimation
-
-dragon_spine_animation = DragonSpineAnimation(
-    image_name = "1000_dragon_nature",
-    phase = 3,
-    skin = 1
-)
-
-dragon_spine_animation.download(output="dragon_spine_animation.zip")
-```
-
-### Island Packages
-
-To download an island package:
-
-```python
-from dcutils.static.islands import IslandPackage
-
-island_package = IslandPackage(uri = "/mobile/ui/heroicraces_islands/hr_71_heroicorigins.zip")
-
-island_package.download(output = "island_package.zip")
-```
-
-### Sounds
-
-#### Music
-
-To download music:
-
-```python
-from dcutils.static.sounds import GeneralMusic
-
-music = GeneralMusic(music_name = "531_dc_party_planning_island")
-
-music.download(output = "531_dc_party_planning_island.mp3")
-```
-
-## Tools
-
-### Calculators
-
-#### Calculate Element Strengths
-
-```python
-from dcutils.tools.calculators import calculate_strongs
-
-strongs = calculate_strongs(elements = ["terra", "flame"])
-```
-**Output:**
-```
-['electric', 'flame', 'nature', 'ice']
-```
-
-#### Calculate Element Weaknesses
-
-```python
-from dcutils.tools.calculators import calculate_weaknesses
-
-weaknesses = calculate_weaknesses(first_element="terra")
-```
-**Output:**
-```
-['metal', 'war']
-```
-
-#### Calculate Orb Recall Gain
-
-```python
-from dcutils.tools.calculators import calculate_orb_recall_gain
-
-orb_recall_gain = calculate_orb_recall_gain(dragon_level = 15, dragon_stars = 2)
-```
-**Output:**
-```
-389
-```
-
-### Calculate Attack Damage
-
-You can calculate attack damage using the `calculate_attack_damage` function.
-
-```python
-from dcutils.tools.calculators.dragon import calculate_attack_damage
-
-damage_info = calculate_attack_damage(
-    category = 1,
-    level = 50,
-    attack_power=  1000,
-    rank_class = 3,
-    stars = 2
-)
-```
-
-### Calculate
-
-You can calculate dragon status using the `calculate_status` function.
-
-```python
-from dcutils.tools.calculators.dragon import calculate_status
-
-status_info = calculate_status(
-    category = 1,
-    rarity = "R",
-    level = 50,
-    rank_class = 3,
-    stars = 2,
-    hp_runes = 5,
-    damage_runes = 3,
-    with_tower_bonus = True,
-    extra_hp_multiplier=  0.1,
-    extra_damage_multiplier = 0.05
-)
-```
-
-### AI (Artificial Intelligence)
-
-#### Elements Detector
-
-```python
-from dcutils.tools.ai.elements_detector import ElementsDetectorAI
-
-elements_detector = ElementsDetectorAI()
-
-elements_result = elements_detector.detect(image_path = "ui_3110_dragon_hoardereternal_1@2x.png", limit = 4)
-```
-**Output:**
-```
-[{'element': 'ice', 'confidence_score': 0.4871271550655365}, {'element': 'nature', 'confidence_score': 0.296091228723526}, {'element': 'flame', 'confidence_score': 0.16774502396583557}, {'element': 'sea', 'confidence_score': 0.03868602588772774}]
-```
-
-#### Phase Detector
-
-```python 
-from dcutils.tools.ai.phase_detector import PhaseDetectorAI
-
-phase_detector = PhaseDetectorAI()
-
-phase_result = phase_detector.detect(image_path="ui_3110_dragon_hoardereternal_1@2x.png")
-```
-**Output:**
-```
-{'phase': 'baby', 'confidence_score': 0.9999938011169434}
-```
-
-### URL Parser
-
-#### Dragon URL Parser
-
-You can parse various information from Dragon URLs:
-
-```python
-from dcutils.tools.url_parser.dragon import DragonUrlParser
-
-# Example URLs
-url_flash_animation = "https://dci-static-s1.socialpointgames.com/static/dragoncity/assets/sprites/1000_dragon_nature_skin1_3.swf"
-url_spine_animation = "https://dci-static-s1.socialpointgames.com/static/dragoncity/mobile/engine/version_1_1/dragons/1000_dragon_nature_3/1000_dragon_nature_skin1_3_HD_tweened_dxt5.zip"
-url_sprite = "https://dci-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/dragons/ui_1000_dragon_nature_skin1_3@2x.png"
-url_thumb = "https://dci-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/dragons/HD/thumb_1000_dragon_nature_skin1_3.png"
-
-# Parse from URLs
-result_flash_animation = DragonUrlParser.from_flash_animation(url_flash_animation)
-result_spine_animation = DragonUrlParser.from_spine_animation(url_spine_animation)
-result_sprite = DragonUrlParser.from_sprite(url_sprite)
-result_thumb = DragonUrlParser.from_thumb(url_thumb)
-
-# Get specific information
-dragon_id = DragonUrlParser.get_id(url_thumb)
-image_name = DragonUrlParser.get_image_name(url_thumb)
-image_quality = DragonUrlParser.get_image_quality(url_sprite)
-phase = DragonUrlParser.get_phase(url_sprite)
-skin = DragonUrlParser.get_skin(url_sprite)
-```
-
-Each function returns relevant information parsed from the given Dragon URL.
-
-Feel free to explore these functionalities and integrate them into your projects!
-
-## Localization
-
-The `Localization` class allows you to handle localization data efficiently. You can load localization from files, fetch it from an endpoint, and perform various operations on the data.
-
-```python
-from dcutils.static.localization import Localization
-
-# Example usage
-loc = Localization(language = "en")
-print(loc)
-```
-
-### Methods
-
-#### load_file
-
-Load localization data from a file.
-
-```python
-loc = Localization.load_file(file_path = "localization.json")
-```
-
-#### load_compressed_file
-
-Load compressed localization data from a file.
-
-```python
-loc = Localization.load_compressed_file(file_path = "localization.gz")
-```
-
-#### fetch
-
-Fetch localization data from an endpoint.
-
-```python
-loc_data = Localization.fetch(language = "en")
-```
-
-#### get_value_from_key
-
-Get the value from a key in the localization data.
-
-```python
-value = loc.get_value_from_key("key_name")
-```
-
-#### get_key_from_value
-
-Get the key from a value in the localization data.
-
-```python
-key = loc.get_key_from_value("value_name")
-```
-
-#### get_dragon_name
-
-Get the name of a dragon based on its ID.
-
-```python
-name = loc.get_dragon_name(id = 1000)
-```
-
-#### get_dragon_description
-
-Get the description of a dragon based on its ID.
-
-```python
-description = loc.get_dragon_description(id = 1000)
-```
-
-#### get_attack_name
-
-Get the name of an attack based on its ID.
-
-```python
-name = loc.get_attack_name(id = 1)
-```
-
-#### get_skill_name
-
-Get the name of a skill based on its ID.
-
-```python
-name = loc.get_skill_name(id = 1)
-```
-
-#### get_skill_description
-
-Get the description of a skill based on its ID.
-
-```python
-description = loc.get_skill_description(id = 1)
-```
-
-#### search_keys
-
-Search for keys containing a specific query.
-
-```python
-keys = loc.search_keys(query = "search_query")
-```
-
-#### search_values
-
-Search for values containing a specific query.
-
-```python
-values = loc.search_values(query = "search_query")
-```
-
-#### compare
-
-Compare the current localization data with old localization data.
-
-```python
-comparison = loc.compare(old_localization = old_loc)
-```
-
-### Properties
-
-#### list
-
-Get the localization data as a list.
-
-```python
-loc_list = loc.list
-```
-
-#### dict
-
-Get the localization data as a dictionary.
-
-```python
-loc_dict = loc.dict
-```
-
-Feel free to explore these functionalities and integrate them into your projects!
+Metadata-Version: 2.1
+Name: dragon-city-utils
+Version: 2.1.0
+Summary: Dragon City Utils, a collection of tools and utilities for managing static assets and performing calculations related to the Dragon City game.
+License: MIT
+Author: Marcuth
+Author-email: example@gmail.com
+Requires-Python: >=3.12,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: keras (>=3.0.5,<4.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
+Requires-Dist: pydantic (>=2.6.3,<3.0.0)
+Requires-Dist: python-filter (>=2.0.6,<3.0.0)
+Requires-Dist: python-pathutil (>=0.0.0.0.2,<0.0.1.0.0)
+Requires-Dist: tensorflow (>=2.16.1,<3.0.0)
+Description-Content-Type: text/markdown
+
+# dragon-city-utils
+
+Welcome to the documentation of Dragon City Utils, a collection of tools and utilities for managing static assets and performing calculations related to the game Dragon City. Below, you'll find detailed explanations and code snippets for various functionalities.
+
+## Static Files
+
+### Sprites
+
+#### Dragon Sprite
+
+You can download a dragon sprite using the following code:
+
+```python
+from dcutils.static.sprites import DragonSprite
+
+dragon_sprite = DragonSprite(
+    image_name = "1000_dragon_nature",
+    phase = 3,
+    skin = "skin1",
+    image_quality = 2
+)
+
+dragon_sprite.download(output="dragon_nature_sprite.png")
+```
+#### Dragon Thumb
+
+To download a dragon thumb:
+
+```python
+from dcutils.static.sprites import DragonThumb
+
+dragon_thumb = DragonThumb(
+    image_name = "1000_dragon_nature",
+    phase = 3,
+    skin = "skin1"
+)
+
+dragon_thumb.download(output="dragon_nature_thumb.png")
+```
+
+### Animations
+
+#### Dragon Animation (Flash Animation)
+
+To download a dragon flash animation:
+
+```python
+from dcutils.static.animations import DragonFlashAnimation
+
+dragon_flash_animation = DragonFlashAnimation(
+    image_name = "1000_dragon_nature",
+    phase = 3,
+    skin = "skin1"
+)
+
+dragon_flash_animation.download(output="dragon_nature_flash_animation.swf")
+```
+
+#### Dragon Animation (Spine Animation)
+
+To download a dragon spine animation:
+
+```python
+from dcutils.static.animations import DragonSpineAnimation
+
+dragon_spine_animation = DragonSpineAnimation(
+    image_name = "1000_dragon_nature",
+    phase = 3,
+    skin = 1
+)
+
+dragon_spine_animation.download(output="dragon_spine_animation.zip")
+```
+
+### Island Packages
+
+To download an island package:
+
+```python
+from dcutils.static.islands import IslandPackage
+
+island_package = IslandPackage(uri = "/mobile/ui/heroicraces_islands/hr_71_heroicorigins.zip")
+
+island_package.download(output = "island_package.zip")
+```
+
+### Sounds
+
+#### Music
+
+To download music:
+
+```python
+from dcutils.static.sounds import GeneralMusic
+
+music = GeneralMusic(music_name = "531_dc_party_planning_island")
+
+music.download(output = "531_dc_party_planning_island.mp3")
+```
+
+## Tools
+
+### Calculators
+
+#### Calculate Element Strengths
+
+```python
+from dcutils.tools.calculators import calculate_strongs
+
+strongs = calculate_strongs(elements = ["terra", "flame"])
+```
+**Output:**
+```
+['electric', 'flame', 'nature', 'ice']
+```
+
+#### Calculate Element Weaknesses
+
+```python
+from dcutils.tools.calculators import calculate_weaknesses
+
+weaknesses = calculate_weaknesses(first_element="terra")
+```
+**Output:**
+```
+['metal', 'war']
+```
+
+#### Calculate Orb Recall Gain
+
+```python
+from dcutils.tools.calculators import calculate_orb_recall_gain
+
+orb_recall_gain = calculate_orb_recall_gain(dragon_level = 15, dragon_stars = 2)
+```
+**Output:**
+```
+389
+```
+
+### Calculate Attack Damage
+
+You can calculate attack damage using the `calculate_attack_damage` function.
+
+```python
+from dcutils.tools.calculators.dragon import calculate_attack_damage
+
+damage_info = calculate_attack_damage(
+    category = 1,
+    level = 50,
+    attack_power=  1000,
+    rank_class = 3,
+    stars = 2
+)
+```
+
+### Calculate
+
+You can calculate dragon status using the `calculate_status` function.
+
+```python
+from dcutils.tools.calculators.dragon import calculate_status
+
+status_info = calculate_status(
+    category = 1,
+    rarity = "R",
+    level = 50,
+    rank_class = 3,
+    stars = 2,
+    hp_runes = 5,
+    damage_runes = 3,
+    with_tower_bonus = True,
+    extra_hp_multiplier=  0.1,
+    extra_damage_multiplier = 0.05
+)
+```
+
+### AI (Artificial Intelligence)
+
+#### Elements Detector
+
+```python
+from dcutils.tools.ai.elements_detector import ElementsDetectorAI
+
+elements_detector = ElementsDetectorAI()
+
+elements_result = elements_detector.detect(image_path = "ui_3110_dragon_hoardereternal_1@2x.png", limit = 4)
+```
+**Output:**
+```
+[{'element': 'ice', 'confidence_score': 0.4871271550655365}, {'element': 'nature', 'confidence_score': 0.296091228723526}, {'element': 'flame', 'confidence_score': 0.16774502396583557}, {'element': 'sea', 'confidence_score': 0.03868602588772774}]
+```
+
+#### Phase Detector
+
+```python 
+from dcutils.tools.ai.phase_detector import PhaseDetectorAI
+
+phase_detector = PhaseDetectorAI()
+
+phase_result = phase_detector.detect(image_path="ui_3110_dragon_hoardereternal_1@2x.png")
+```
+**Output:**
+```
+{'phase': 'baby', 'confidence_score': 0.9999938011169434}
+```
+
+### URL Parser
+
+#### Dragon URL Parser
+
+You can parse various information from Dragon URLs:
+
+```python
+from dcutils.tools.url_parser.dragon import DragonUrlParser
+
+# Example URLs
+url_flash_animation = "https://dci-static-s1.socialpointgames.com/static/dragoncity/assets/sprites/1000_dragon_nature_skin1_3.swf"
+url_spine_animation = "https://dci-static-s1.socialpointgames.com/static/dragoncity/mobile/engine/version_1_1/dragons/1000_dragon_nature_3/1000_dragon_nature_skin1_3_HD_tweened_dxt5.zip"
+url_sprite = "https://dci-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/dragons/ui_1000_dragon_nature_skin1_3@2x.png"
+url_thumb = "https://dci-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/dragons/HD/thumb_1000_dragon_nature_skin1_3.png"
+
+# Parse from URLs
+result_flash_animation = DragonUrlParser.from_flash_animation(url_flash_animation)
+result_spine_animation = DragonUrlParser.from_spine_animation(url_spine_animation)
+result_sprite = DragonUrlParser.from_sprite(url_sprite)
+result_thumb = DragonUrlParser.from_thumb(url_thumb)
+
+# Get specific information
+dragon_id = DragonUrlParser.get_id(url_thumb)
+image_name = DragonUrlParser.get_image_name(url_thumb)
+image_quality = DragonUrlParser.get_image_quality(url_sprite)
+phase = DragonUrlParser.get_phase(url_sprite)
+skin = DragonUrlParser.get_skin(url_sprite)
+```
+
+Each function returns relevant information parsed from the given Dragon URL.
+
+Feel free to explore these functionalities and integrate them into your projects!
+
+## Localization
+
+The `Localization` class allows you to handle localization data efficiently. You can load localization from files, fetch it from an endpoint, and perform various operations on the data.
+
+```python
+from dcutils.static.localization import Localization
+
+# Example usage
+loc = Localization(language = "en")
+print(loc)
+```
+
+### Methods
+
+#### load_file
+
+Load localization data from a file.
+
+```python
+loc = Localization.load_file(file_path = "localization.json")
+```
+
+#### load_compressed_file
+
+Load compressed localization data from a file.
+
+```python
+loc = Localization.load_compressed_file(file_path = "localization.gz")
+```
+
+#### fetch
+
+Fetch localization data from an endpoint.
+
+```python
+loc_data = Localization.fetch(language = "en")
+```
+
+#### get_value_from_key
+
+Get the value from a key in the localization data.
+
+```python
+value = loc.get_value_from_key("key_name")
+```
+
+#### get_key_from_value
+
+Get the key from a value in the localization data.
+
+```python
+key = loc.get_key_from_value("value_name")
+```
+
+#### get_dragon_name
+
+Get the name of a dragon based on its ID.
+
+```python
+name = loc.get_dragon_name(id = 1000)
+```
+
+#### get_dragon_description
+
+Get the description of a dragon based on its ID.
+
+```python
+description = loc.get_dragon_description(id = 1000)
+```
+
+#### get_attack_name
+
+Get the name of an attack based on its ID.
+
+```python
+name = loc.get_attack_name(id = 1)
+```
+
+#### get_skill_name
+
+Get the name of a skill based on its ID.
+
+```python
+name = loc.get_skill_name(id = 1)
+```
+
+#### get_skill_description
+
+Get the description of a skill based on its ID.
+
+```python
+description = loc.get_skill_description(id = 1)
+```
+
+#### search_keys
+
+Search for keys containing a specific query.
+
+```python
+keys = loc.search_keys(query = "search_query")
+```
+
+#### search_values
+
+Search for values containing a specific query.
+
+```python
+values = loc.search_values(query = "search_query")
+```
+
+#### compare
+
+Compare the current localization data with old localization data.
+
+```python
+comparison = loc.compare(old_localization = old_loc)
+```
+
+### Properties
+
+#### list
+
+Get the localization data as a list.
+
+```python
+loc_list = loc.list
+```
+
+#### dict
+
+Get the localization data as a dictionary.
+
+```python
+loc_dict = loc.dict
+```
+
+Feel free to explore these functionalities and integrate them into your projects!
```

### Comparing `dragon-city-utils-2.0.3/dcutils/_utils/file.py` & `dragon_city_utils-2.1.0/dcutils/_utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-2.0.3/dcutils/static/animations/flash/dragon.py` & `dragon_city_utils-2.1.0/dcutils/static/animations/flash/dragon.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,10 +18,8 @@
 
         if skin:
             skin = f"_{skin}"
             
         else:
             skin = ""
 
-        self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/assets/sprites/{image_name}{skin}_{phase}.swf"
-
-__all__ = [ "DragonFlashAnimation" ]
+        self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/assets/sprites/{image_name}{skin}_{phase}.swf"
```

### Comparing `dragon-city-utils-2.0.3/dcutils/static/animations/spine/dragon.py` & `dragon_city_utils-2.1.0/dcutils/static/animations/spine/dragon.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,10 +26,8 @@
         else:
             skin = ""
 
         if use_new_url:
             self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/mobile/engine/version_1_1/dragons/{image_name}_{phase}/{image_name}{skin}_{phase}_HD_tweened_{platform}.zip"
             
         else:
-            self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/mobile/engine/version_1_1/dragons/{image_name}_{phase}/basic_{image_name}{skin}_{phase}_HD_spine-3-8-59_{platform}.zip"
-
-__all__ = [ "DragonSpineAnimation" ]
+            self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/mobile/engine/version_1_1/dragons/{image_name}_{phase}/basic_{image_name}{skin}_{phase}_HD_spine-3-8-59_{platform}.zip"
```

### Comparing `dragon-city-utils-2.0.3/dcutils/static/localization/__init__.py` & `dragon_city_utils-2.1.0/dcutils/static/localization/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 from typing import Optional, Union, Any, Self
 from pydantic import validate_call
 from pyfilter import DictListFilter
 import httpx
 import json
 
-from ..._utils.file import (
+from ..._utils.file_manager import (
     write_json_file,
     read_json_file,
     write_compressed_json_file,
     read_compressed_json_file
 )
 
 LocalizationDict = dict[str, str]
 LocalizationList = list[LocalizationDict]
 
 class Localization:
-    __list: list
-    __dict: dict
+    _list: list
+    _dict: dict
 
     @validate_call
     def __init__(
         self,
         language: Optional[str] = None,
-        loc: Optional[
-            Union[list[dict], dict]
-        ] = None
+        loc: Union[list[dict], dict, None] = None
     ) -> None:
         if language:
-            self.__list: LocalizationList = self.fetch(language)
-            self.__dict: LocalizationDict = DictListFilter(self.__list).merge_dicts()
+            self._list: LocalizationList = self.fetch(language)
+            self._dict: LocalizationDict = DictListFilter(self._list).merge_dicts()
 
         elif loc:
-            self.__load(loc)
+            self._load(loc)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({json.dumps(self.dict, indent=4)[:300]}" + "...})"
 
     def __str__(self) -> str:
         return self.__repr__()
 
@@ -68,41 +66,41 @@
     @classmethod
     @validate_call
     def load(cls, loc: Union[list, dict]) -> Self:
         loc_obj = cls()
         object_type = type(loc)
 
         if object_type == list:
-            loc_obj._Localization__list = loc
-            loc_obj._Localization__dict = DictListFilter(loc).merge_dicts()
+            loc_obj._list = loc
+            loc_obj._dict = DictListFilter(loc).merge_dicts()
 
         elif object_type == dict:
-            loc_obj._Localization__dict = loc
-            loc_obj._Localization__list = []
+            loc_obj._dict = loc
+            loc_obj._list = []
 
             for key, value in loc.items():
                 dict_ = { key: value }
-                loc_obj._Localization__localization.append(dict_)
+                loc_obj._list.append(dict_)
 
         else:
             raise ValueError(f"'{object_type}' is an invalid type to load a localization!")
 
         return loc_obj
 
     @validate_call
     def save_file(
         self,
         file_path: str,
         from_: str = "dict"
     ) -> None:
         if from_ == "dict":
-            data = self.__dict
+            data = self._dict
 
         elif from_ == "list":
-            data = self.__list
+            data = self._list
 
         else:
             ValueError()
 
         write_json_file(file_path, data)
 
     @validate_call
@@ -129,48 +127,48 @@
         endpoint_url = f"https://sp-translations.socialpointgames.com/deploy/dc/android/prod/dc_android_{language}_prod_wetd46pWuR8J5CmS.json"
 
         response = httpx.get(endpoint_url)
         data = response.json()
         return data
 
     @validate_call
-    def __load(self, loc: Union[list, dict]):
+    def _load(self, loc: Union[list, dict]):
         type_ = type(loc)
 
         if type_ == list:
-            self.__load_list(loc)
+            self._load_list(loc)
 
         elif type_ == dict:
-            self.__load_dict(loc)
+            self._load_dict(loc)
 
         else:
             raise ValueError(f"{type_} is an invalid type to load a localization")
 
     @validate_call
-    def __load_list(self, loc: list[dict]):
-        self.__list = loc
-        self.__dict = DictListFilter(loc).merge_dicts()
+    def _load_list(self, loc: list[dict]):
+        self._list = loc
+        self._dict = DictListFilter(loc).merge_dicts()
 
     @validate_call
-    def __load_dict(self, loc: dict):
-        self.__dict = loc
-        self.__list = []
+    def _load_dict(self, loc: dict):
+        self._dict = loc
+        self._list = []
 
         for key, value in loc.items():
             dict_ = { key: value }
-            self.__list.append(dict_)
+            self._list.append(dict_)
 
     @validate_call
     def get_value_from_key(self, key: str) -> Optional[str]:
-        if key in self.__dict.keys():
-            return self.__dict[key]
+        if key in self._dict.keys():
+            return self._dict[key]
 
     @validate_call
     def get_key_from_value(self, value: str) -> Optional[str]:
-        for dict_key, dict_value in self.__dict.items():
+        for dict_key, dict_value in self._dict.items():
             if dict_value == value:
                 return dict_key
 
     @validate_call
     def get_dragon_name(self, id: int) -> Optional[str]:
         key = f"tid_unit_{id}_name"
         return self.get_value_from_key(key)
@@ -199,15 +197,15 @@
     def search_keys(self, query: str) -> list[str]:
         query = (query
             .lower()
             .strip())
 
         results = []
 
-        for key in self.__dict.keys():
+        for key in self._dict.keys():
             parsed_key = (key
                 .lower()
                 .strip())
 
             if query in parsed_key:
                 results.append(key)
 
@@ -217,15 +215,15 @@
     def search_values(self, query: str) -> list[str] | list:
         query = (query
             .lower()
             .strip())
 
         results = []
 
-        for value in self.__dict.values():
+        for value in self._dict.values():
             parsed_value = (value
                 .lower()
                 .strip())
 
             if query in parsed_value:
                 results.append(value)
 
@@ -244,45 +242,43 @@
 
         new_fields = []
         edited_fields = []
         deleted_fields = []
 
         old_localization_keys = old_localization.keys()
 
-        for key in self.__dict.keys():
+        for key in self._dict.keys():
             if key not in old_localization_keys:
                 new_fields.append({
                     "key": key,
-                    "value": self.__dict[key]
+                    "value": self._dict[key]
                 })
 
         for key in old_localization_keys:
-            if key not in self.__dict:
+            if key not in self._dict:
                 deleted_fields.append({
                     "key": key,
                     "value": old_localization[key]
                 })
 
-            elif old_localization[key] != self.__dict[key]:
+            elif old_localization[key] != self._dict[key]:
                 edited_fields.append({
                     "key": key,
                     "values": {
                         "new": old_localization[key],
-                        "old": self.__dict[key]
+                        "old": self._dict[key]
                     }
                 })
 
         return dict(
             new_fields = new_fields,
             edited_fields = edited_fields,
             deleted_fields = deleted_fields
         )
 
     @property
     def list(self) -> LocalizationList:
-        return self.__list or []
+        return self._list or []
 
     @property
     def dict(self) -> LocalizationDict:
-        return self.__dict or {}
-
-__all__ = [ "Localization" ]
+        return self._dict or {}
```

### Comparing `dragon-city-utils-2.0.3/dcutils/static/sounds/config.py` & `dragon_city_utils-2.1.0/dcutils/static/sounds/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from pydantic import validate_call
+from typing import Optional
 
 music_names = ["107_audio_nw_maintheme", "150_dc_music_labyrinth_island_2015", "151_dc_music_labyrinth_battle_2015", "152_dc_christmas_music_2015", "166_dc_sun_island_music", "168_dc_moon_island_music", "196_dc_ninja_island_main", "197_dc_ninja_island_battle", "200_anniversary_island_music", "201_pirates_island_music", "202_pirates_island_battle_music", "203_journey_island_battle_music", "205_journey_island_part_02", "206_journey_island_part_03", "207_earth_travel_island_music", "207_heroic_race_music", "208_earth_travel_battle_music", "209_dc_jungle_island_music", "212_dc_music_atlantis_island", "213_dc_music_atlantis_battle", "214_dc_music_crazylab_island", "215_dc_music_crazylab_battle", "216_dc_summer_island_music", "217_dc_music_olympic_island", "218_dc_music_olympic_battle", "222_dc_amusument_park_island_music", "223_dc_amusument_park_battle_music", "224_dc_frankenstein_island", "225_dc_frankenstein_battle", "226_dc_dc_music_forest_battle", "227_dc_dc_music_forest_white", "232_dc_heroic_races_ocean_music", "233_dc_vampiric_island_music", "234_dc_vampiric_island_battle_music", "235_dc_heroic_races_winter_music", "236_dc_winter_tower_island_music", "247_dc_heroic_races_dark_realm_music", "248_dc_fairytale_island_music", "249_dc_fairytale_battle_music", "250_dc_heroic_races_elders_forest", "251_dc_stvalentine_island_music", "252_dc_stvalentine_battle_music", "257_dc_apocaypse_island_music", "264_dc_beautybeast_island_music", "265_dc_beautybeast_battle_music", "266_dc_boneyard_music", "267_dc_dc2056_island_music", "268_dc_dc2056_battle_music", "269_dc_heroic_races_spring", "270_dc_happyinferno_island_music", "271_dc_happyinferno_battle_music", "275_dc_music_got_island", "276_dc_music_got_island_battle", "281_dc_heroic_races_demonic_dojo", "283_dc_videogame_island_music", "284_dc_videogame_battle_music", "285_dc_summer_island_music", "286_dc_heroic_races_summer", "288_dc_music_dungeon_island", "289_dc_music_dungeon_battle", "291_dc_music_ragnarok_island", "292_dc_heroic_races_oni_forest", "293_dc_pvp_battle_theme_01", "296_dc_heroic_races_crystal", "297_dc_music_comic_island", "298_dc_music_comic_island_battle", "299_dc_heroic_races_factory", "300_dc_music_shadow_island", "301_dc_music_shadow_island_battle", "302_dc_heroic_races_galactic", "303_dc_heroic_races_frozen_lake", "304_dc_music_dragon_justice_island", "311_dc_music_illusion_island", "312_dc_music_illusion_island_battle", "363_dc_farm_island_music", "364_dc_farm_battle_music", "365_dc_burglar_island_music", "391_dc_music_blizzard_island", "392_dc_heroic_races_vortex", "393_dc_fire_and_ice_island_music_b", "394_dc_fire_and_ice_battle_music_b", "402_dc_music_snow_island", "403_dc_heroic_races_heaven", "406_dc_turbo_island_music", "407_dc_turbo_battle_music", "412_dc_music_oni_island", "413_dc_music_oni_island_battle", "414_dc_heroic_races_black_magic", "416_dc_watchtower_island_music", "418_dc_magic_castle_island_music", "419_dc_magic_castle_island_battle_music", "420_dc_neo_tokyo_island_music", "421_dc_heroic_races_pixel_art", "438_dc_dragon_wars_island", "439_dc_dragon_wars_island_battle", "440_dc_heroic_races_metagame", "443_dc_music_pyramid_island", "444_dc_pyramid_battle_music", "449_dc_team_races_atlas", "450_dc_music_ruined_tower_island", "451_dc_fae_island_music", "452_dc_fae_castle_music", "456_dc_team_races_yggdrassil", "457_dc_music_moon_elevator_tower_island", "459_dc_heroic_races_luxury_cruise", "460_dc_wasteland_rescue_island", "461_dc_wasteland_rescue_battle", "462_dc_funfair_island_music", "463_dc_music_funfair_battle_music", "476_dc_puzzle_island_music", "478_dc_chocolate_tower_island_music", "482_dc_heroic_races_dreamfields", "484_dc_hallomuertos_island_music", "485_dc_hallomuertos_battle_music", "486_dc_lost_temple_alliance_race_music", "487_dc_catacombs_island_music", "490_dc_divination_island_music", "491_dc_divination_battle_music", "492_dc_seasons_island_music", "493_dc_seasons_island_battle_music", "494_dc_weather_machine_island_music", "495_dc_heroic_races_christmas_party", "496_dc_color_splash_island_music", "497_dc_color_splash_battle_music", "498_dc_battleground_menu_music", "499_dc_battleground_battle_music_1", "501_dc_heroic_races_superheroes", "502_dc_galactic_mini_island_music", "503_dc_galactic_mini_battle_music", "504_dc_chinese_new_year_island_music", "505_dc_chinese_new_year_battle_music", "506_dc_valentine_puzzle_island_music", "507_dc_liberty_island_music", "508_dc_abyssal_island_music", "509_dc_abyssal_island_battle_music", "510_dc_carnaval_island_music", "514_dc_heroic_races_true_superheroes", "515_dc_sushi_puzzle_island_music", "517_dc_castle_town_island_music", "518_dc_castle_town_battle_music", "519_dc_heroic_races_eternity", "520_dc_chibi_puzzle_island_music", "521_dc_easter_fog_island_music", "522_dc_fast_food_island_music", "523_dc_fast_food_battle_music", "524_dc_cosmic_puzzle", "525_dc_heroic_races_the_fallen_music", "527_dc_tank_blitz_island_music", "528_dc_tank_blitz_battle_music", "529_dc_pet_island_music", "530_dc_pet_island_battle_music", "531_dc_party_planning_island", "532_dc_party_planning_island_battle", "533_dc_heroic_races_positivity", "536_dc_runner_island_menu_music", "537_dc_runner_island_level_music_01", "540_dc_search_puzzle_island_music", "541_dc_toy_tower_island_music", "549_dc_martial_arts_island_music", "557_dc_music_festival_island_music", "558_dc_music_festival_island_battle_music", "561_dc_heroic_races_pirates", "562_dc_fantasy_island_music", "563_dc_fantasy_island_battle_music", "564_dc_safari_puzzle_island_music", "566_dc_heroic_races_community", "567_dc_wild_animals_island_music", "568_dc_wild_animals_island_battle_music", "569_dc_mafia_island_music", "570_dc_heroic_races_halloween", "571_dc_seven_wonders_island_music", "572_dc_seven_wonders_island_battle_music", "577_dc_puzzle_knights_island_music", "578_dc_knights_paladins_island_music", "579_dc_knights_paladins_island_battle_music", "580_dc_heroic_races_cybernetic", "581_dc_aquatic_runner_island_menu_music", "582_dc_aquatic_runner_island_level_music", "583_dc_winter_runner_island_menu_music", "584_dc_winter_runner_island_level_music", "586_dc_xmas_19_island_music", "587_dc_xmas_19_island_battle_music", "588_dc_winter_island_music", "589_dc_winter_island_battle_music", "590_dc_heroic_races_frozen_cave", "591_dc_abyssal_fog_island_music", "600_dc_heroic_races_virago", "608_dc_music_maze_easter_map_loop", "609_dc_music_maze_easter_battle_loop", "610_dc_music_maze_gods_island_loop", "611_dc_music_puzzle_gods_island_loop", "612_dc_music_battle_gods_island_loop", "613_dc_music_maze_5_de_mayo_loop", "614_dc_music_battle_5_de_mayo_loop", "617_dc_music_battle_pass_mysterious_loop", "MAIN1.MP3", "MAIN2.MP3", "MAIN3.MP3", "New Text Document.txt", "dc_music_celestial_island_2015", "dc_music_garden_battle", "dc_music_garden_island", "dc_music_got_island_2015", "dc_music_halloween_battle_2015", "dc_music_halloween_island_2015", "dc_music_hollywood_island_battle", "dc_music_idol_island", "dc_music_ufo_island_2015", "dungeon_gridisland_background_music", "dungeon_gridisland_battle_music", "songcolisseum_b_2", "songcolisseum_c_1"]
 
 @validate_call
-def get_music_name_from_tag(tag: str) -> str | None:
+def get_music_name_from_tag(tag: str) -> Optinal[str]:
     tag_in_lower_case = tag.lower()
     music_name_key_1 = f"dc_{tag_in_lower_case}_island"
     music_name_key_2 = f"_{tag_in_lower_case}"
 
     for music_name in music_names:
         if music_name_key_1 in music_name or music_name.endswith(music_name_key_2):
-            return music_name
-
-__all__ = [ get_music_name_from_tag ]
+            return music_name
```

### Comparing `dragon-city-utils-2.0.3/dcutils/static/sounds/musics.py` & `dragon_city_utils-2.1.0/dcutils/static/sounds/musics.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,10 +14,8 @@
 
         if tag:
             music_name = get_music_name_from_tag(tag)
 
         if not music_name:
             raise ValueError("Please enter a valid song name! If you have entered a tag please check it as it was not possible to get a song name from it.")
 
-        self.url = f"http://dci-static-s1.socialpointgames.com/static/dragoncity/mobile/sounds/music/{music_name}.mp3"
-
-__all__ = [ "GeneralMusic" ]
+        self.url = f"http://dci-static-s1.socialpointgames.com/static/dragoncity/mobile/sounds/music/{music_name}.mp3"
```

### Comparing `dragon-city-utils-2.0.3/dcutils/static/sprites/chest.py` & `dragon_city_utils-2.1.0/dcutils/static/sprites/chest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,10 +16,8 @@
 
         elif image_quality == 2:
             image_quality_str = "@2x"
 
         else:
             raise ValueError(f"{image_quality} Not a valid number for image quality of a chest. Choose a number between 1 and 2")
         
-        self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/chests/ui_{image_name}{image_quality_str}.png"
-
-__all__ = [ "ChestSprite" ]
+        self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/chests/ui_{image_name}{image_quality_str}.png"
```

### Comparing `dragon-city-utils-2.0.3/dcutils/static/sprites/dragon.py` & `dragon_city_utils-2.1.0/dcutils/static/sprites/dragon.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,10 +27,8 @@
 
         elif image_quality == 2:
             image_quality_str = "@2x"
 
         else:
             raise ValueError(f"{image_quality} Not a valid number for image quality of a dragon. Choose a number between 1 and 2")
 
-        self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/dragons/ui_{image_name}{skin}_{phase}{image_quality_str}.png"
-
-__all__ = [ "DragonSprite" ]
+        self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/dragons/ui_{image_name}{skin}_{phase}{image_quality_str}.png"
```

### Comparing `dragon-city-utils-2.0.3/dcutils/static/sprites/dragon_thumb.py` & `dragon_city_utils-2.1.0/dcutils/static/sprites/dragon_thumb.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,10 +18,8 @@
 
         if skin:
             skin = f"_{skin}"
         
         else:
             skin = ""
         
-        self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/dragons/HD/thumb_{image_name}{skin}_{phase}.png"
-
-__all__ = [ "DragonThumb" ]
+        self.url = f"https://{platform_prefix}-static-s1.socialpointgames.com/static/dragoncity/mobile/ui/dragons/HD/thumb_{image_name}{skin}_{phase}.png"
```

### Comparing `dragon-city-utils-2.0.3/dcutils/tools/calculators/battle_simulator.py` & `dragon_city_utils-2.1.0/dcutils/tools/calculators/old_battle_simulator.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/attack_damage/__init__.py` & `dragon_city_utils-2.1.0/dcutils/tools/calculators/dragon/attack_damage/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,10 +43,8 @@
     )
 
     return dict(
         minimum = minimum,
         maximum = maximum,
         average = average,
         random = random_damage
-    )
-
-__all__ = [ "calculate_attack_damage" ]
+    )
```

### Comparing `dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/status/__init__.py` & `dragon_city_utils-2.1.0/dcutils/tools/calculators/dragon/status/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,10 +104,8 @@
                 damage = round(tower_damage_bonus)
             ),
             extra = dict(
                 hp = round(extra_hp_bonus),
                 damage = round(extra_damage_bonus)
             )
         )
-    )
-
-__all__ = [ "calculate_status" ]
+    )
```

### Comparing `dragon-city-utils-2.0.3/dcutils/tools/calculators/dragon/status/config.py` & `dragon_city_utils-2.1.0/dcutils/tools/calculators/dragon/status/config.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-2.0.3/dcutils/tools/calculators/elements/__init__.py` & `dragon_city_utils-2.1.0/dcutils/tools/calculators/elements/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,13 +21,8 @@
 
     for element in ELEMENTS_CONFIG.keys():
         element_strongs = ELEMENTS_CONFIG[element]["strongs"]
 
         if first_element in element_strongs:
             weaknesses.append(element)
 
-    return weaknesses
-
-__all__ = [
-    "calculate_strongs",
-    "calculate_weaknesses"
-]
+    return weaknesses
```

### Comparing `dragon-city-utils-2.0.3/dcutils/tools/calculators/elements/config.py` & `dragon_city_utils-2.1.0/dcutils/tools/calculators/elements/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,10 +83,8 @@
         "strongs": ["happy", "chaos"],
         "weaknesses": []
     },
     "physical": {
         "strongs": [],
         "weaknesses": ["legend"]
     }
-}
-
-__all__ = [ "ELEMENTS_CONFIG" ]
+}
```

### Comparing `dragon-city-utils-2.0.3/dcutils/tools/calculators/orb_recall/__init__.py` & `dragon_city_utils-2.1.0/dcutils/tools/calculators/orb_recall/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,10 +20,8 @@
 
     for i in range(dragon_level if dragon_level <= 30 else 30):
         orbs_gain += ORB_RECALL_CONFIG["per_levels"][i]
 
     for i in range(dragon_stars):
         orbs_gain += ORB_RECALL_CONFIG["per_stars"][i]
 
-    return orbs_gain
-
-__all__ = [ "calculate_recall_gain" ]
+    return orbs_gain
```

### Comparing `dragon-city-utils-2.0.3/dcutils/tools/url_parser/dragon.py` & `dragon_city_utils-2.1.0/dcutils/tools/url_parser/dragon.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,10 +105,8 @@
     @validate_call
     def from_spine_animation(cls, url: str) -> dict:
         return dict(
             id = cls.get_id(url),
             image_name = cls.get_image_name(url),
             phase = cls.get_phase(url),
             skin = cls.get_skin(url)
-        )
-
-__all__ = [ "DragonUrlParser" ]
+        )
```

