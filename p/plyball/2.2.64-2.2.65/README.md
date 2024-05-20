# Comparing `tmp/plyball-2.2.64.tar.gz` & `tmp/plyball-2.2.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyball-2.2.64.tar", last modified: Fri Mar 15 20:51:07 2024, max compression
+gzip compressed data, was "plyball-2.2.65.tar", last modified: Mon May 20 01:17:02 2024, max compression
```

## Comparing `plyball-2.2.64.tar` & `plyball-2.2.65.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-15 20:50:59.000000 plyball-2.2.64/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-15 20:50:59.000000 plyball-2.2.64/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-15 20:51:07.268429 plyball-2.2.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-15 20:50:59.000000 plyball-2.2.64/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.264429 plyball-2.2.64/plyball/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/plyball/baseballreference/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/baseballreference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/baseballreference/baseballreference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/plyball/fangraphs/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/fangraphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15582 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/fangraphs/fangraphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/plyball/lahman/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/lahman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/lahman/lahman.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/plyball/mlb/
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/mlb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/plyball/ottoneu/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/ottoneu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/ottoneu/ottoneu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/plyball/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/pipeline/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/player_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/player_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/plyball/retrosheet/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/retrosheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/retrosheet/retrosheet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/plyball/statcast/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/statcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/statcast/statcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-03-15 20:50:59.000000 plyball-2.2.64/plyball/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/plyball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-15 20:51:07.000000 plyball-2.2.64/plyball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-15 20:51:07.000000 plyball-2.2.64/plyball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 20:51:07.000000 plyball-2.2.64/plyball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-15 20:51:07.000000 plyball-2.2.64/plyball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-15 20:51:07.000000 plyball-2.2.64/plyball.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 20:51:07.268429 plyball-2.2.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-03-15 20:50:59.000000 plyball-2.2.64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 20:51:07.268429 plyball-2.2.64/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-15 20:50:59.000000 plyball-2.2.64/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-20 01:16:54.000000 plyball-2.2.65/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 01:16:54.000000 plyball-2.2.65/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-20 01:17:02.451050 plyball-2.2.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 01:16:54.000000 plyball-2.2.65/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/baseballreference/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/baseballreference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/baseballreference/baseballreference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/fangraphs/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/fangraphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/fangraphs/fangraphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/lahman/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/lahman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/lahman/lahman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/mlb/
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/mlb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/ottoneu/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/ottoneu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/ottoneu/ottoneu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.447050 plyball-2.2.65/plyball/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/pipeline/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/player_id_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/player_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/plyball/retrosheet/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/retrosheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/retrosheet/retrosheet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/plyball/statcast/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/statcast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/statcast/statcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-20 01:16:54.000000 plyball-2.2.65/plyball/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/plyball.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 01:17:02.000000 plyball-2.2.65/plyball.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:17:02.451050 plyball-2.2.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-20 01:16:54.000000 plyball-2.2.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:17:02.451050 plyball-2.2.65/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-20 01:16:54.000000 plyball-2.2.65/tests/__init__.py
```

### Comparing `plyball-2.2.64/LICENSE.txt` & `plyball-2.2.65/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/PKG-INFO` & `plyball-2.2.65/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plyball
-Version: 2.2.64
+Version: 2.2.65
 Summary: A simple package for scraping baseball data from the most popular sites.
 Home-page: https://github.com/waaronmorris/plyball
 Author: W. Aaron Morris
 Author-email: w.aaron.morris@gmail.com
 License: MIT
 Keywords: baseball sabermetrics data statistics statcast web scraping
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `plyball-2.2.64/README.md` & `plyball-2.2.65/README.md`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/plyball/baseballreference/baseballreference.py` & `plyball-2.2.65/plyball/baseballreference/baseballreference.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/plyball/fangraphs/fangraphs.py` & `plyball-2.2.65/plyball/fangraphs/fangraphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         json = requests.get(
             url=self._urls['projections'].format(
                 '&'.join(['{}={}'.format(k, v) for k, v in parameters.items()]))).json()
         df = pd.DataFrame(json)
 
         return df
 
-    def get_daily_mlb_game_log(
+    def get_daily_game_log(
             self,
             player_id: int,
             position: str,
             season: int = None,
             start_date: str = None,
             end_date: str = None,
             **kwargs):
```

### Comparing `plyball-2.2.64/plyball/lahman/lahman.py` & `plyball-2.2.65/plyball/lahman/lahman.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/plyball/mlb/__init__.py` & `plyball-2.2.65/plyball/mlb/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,34 @@
+import datetime as dt
 import logging
+from typing import List, Dict
 
 import requests
 
 base_url = 'https://statsapi.mlb.com/api/v1/'
 
 urls = {
-        'schedule_by_day': base_url + "schedule/games/?sportId=1&date={run_date}",
-        'line_ups':        base_url + 'schedule?gamePk={game_pk}&language=en&hydrate=lineups,probablePitcher(note)'
+    'schedule_by_day': base_url + "schedule/games/?sportId=1&date={run_date}",
+    'line_ups': base_url + 'schedule?gamePk={game_pk}&language=en&hydrate=lineups,probablePitcher(note)',
+    'game': base_url + "game/{game_pk}/boxscore?timecode={run_date}",
+    'schedule': base_url + "schedule/?eventTypes=primary,secondary&sportId=1&startDate={start_date}&endDate={end_date}"
 }
 
 headers = {
         "Content-Type": "application/json"
 }
 
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
 
 
 class MLBStats(object):
+    """
+    Class for MLBStats
+
+    """
     def __init__(self):
         self.logger = logging.getLogger(__name__)
         self.logger.info('MLBStats Initialized')
 
     def get_game_lineups(self, game_pk):
         """
         Get Lineups for Today's Games
@@ -80,29 +87,86 @@
         Process game data
 
         :param game_data:
         :return:
         """
         pass
 
-    def get_lineups_by_day(self, run_date):
+    def get_lineups_by_day(self, run_date: dt.datetime):
         """
         Get Schedule by Day
 
         :param run_date:
         :return:
         """
         self.logger.info('Getting Lineups|{}'.format(urls['schedule_by_day'].format(run_date=run_date)))
         games = []
 
         # Send a GET request to the API endpoint
-        response = requests.get(urls['schedule_by_day'].format(run_date=run_date), headers=headers)
+        response = requests.get(urls['schedule_by_day'].format(run_date=run_date.strftime("%Y-%m-%d")), headers=headers)
 
         # Check if the request was successful
         if response.status_code == 200:
             # Get the JSON response
             data = response.json()
 
             # Check if the game data is available
             for date in data["dates"]:
                 for game in date["games"]:
                     return self.get_game_lineups(game["gamePk"])
+
+    def get_game_boxscore(self, game_pk) -> List[Dict]:
+        """
+        Get Game Logs
+
+        :param game_pk:
+        :return:
+        """
+        self.logger.info('Getting Game Logs|{}'.format(urls['game'].format(run_date=game_pk)))
+
+        # Send a GET request to the API endpoint
+        response = requests.get(urls['game'].format(run_date=game_pk), headers=headers)
+
+        # Check if the request was successful
+        if response.status_code == 200:
+            # Get the JSON response
+            data = response.json()
+
+            # Check if the game data is available
+            if "dates" in data and len(data["dates"]) > 0 and "games" in data["dates"][0] and len(
+                    data["dates"][0]["games"]) > 0:
+                game = data["dates"][0]["games"][0]
+
+                return game
+            else:
+                raise Exception(f"Error retrieving the game data for Game ID: {game_pk}")
+        else:
+            raise Exception(f"Error retrieving the game data for Game ID: {game_pk}")
+
+    def get_schedule(self, start_date: dt.datetime, end_date: dt.datetime) -> List[Dict]:
+        """
+        Get Schedule
+
+        :return:
+        """
+        self.logger.info('Getting Schedule|{}'.format(urls['schedule']))
+        games = []
+
+        # Send a GET request to the API endpoint
+        response = requests.get(urls['schedule'].format(
+            start_date=start_date.strftime("%Y-%m-%d"),
+            end_date=end_date.strftime("%Y-%m-%d"),
+            headers=headers))
+
+        # Check if the request was successful
+        if response.status_code == 200:
+            # Get the JSON response
+            data = response.json()
+
+            # Check if the game data is available
+            for date in data["dates"]:
+                for game in date["games"]:
+                    games.append(game)
+
+            return games
+        else:
+            raise Exception(f"Error retrieving the schedule")
```

### Comparing `plyball-2.2.64/plyball/ottoneu/ottoneu.py` & `plyball-2.2.65/plyball/ottoneu/ottoneu.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/plyball/pipeline/evaluation.py` & `plyball-2.2.65/plyball/pipeline/evaluation.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/plyball/player_id_lookup.py` & `plyball-2.2.65/plyball/player_id_lookup.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/plyball/retrosheet/retrosheet.py` & `plyball-2.2.65/plyball/retrosheet/retrosheet.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/plyball/statcast/statcast.py` & `plyball-2.2.65/plyball/statcast/statcast.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/plyball/utils.py` & `plyball-2.2.65/plyball/utils.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/plyball.egg-info/PKG-INFO` & `plyball-2.2.65/plyball.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plyball
-Version: 2.2.64
+Version: 2.2.65
 Summary: A simple package for scraping baseball data from the most popular sites.
 Home-page: https://github.com/waaronmorris/plyball
 Author: W. Aaron Morris
 Author-email: w.aaron.morris@gmail.com
 License: MIT
 Keywords: baseball sabermetrics data statistics statcast web scraping
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `plyball-2.2.64/plyball.egg-info/SOURCES.txt` & `plyball-2.2.65/plyball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/setup.py` & `plyball-2.2.65/setup.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.64/tests/__init__.py` & `plyball-2.2.65/tests/__init__.py`

 * *Files identical despite different names*

