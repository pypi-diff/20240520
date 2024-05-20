# Comparing `tmp/jzai-59.83.46.tar.gz` & `tmp/jzai-59.83.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzai-59.83.46.tar", last modified: Mon May 20 08:29:09 2024, max compression
+gzip compressed data, was "jzai-59.83.47.tar", last modified: Mon May 20 08:33:54 2024, max compression
```

## Comparing `jzai-59.83.46.tar` & `jzai-59.83.47.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 08:29:09.255979 jzai-59.83.46/
--rw-rw-rw-   0        0        0      275 2024-05-20 08:29:09.254660 jzai-59.83.46/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.46/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 08:29:09.231903 jzai-59.83.46/jzai/
--rw-rw-rw-   0        0        0       24 2024-05-20 08:27:39.000000 jzai-59.83.46/jzai/__init__.py
--rw-rw-rw-   0        0        0     9366 2024-05-20 08:20:05.000000 jzai-59.83.46/jzai/bot.py
--rw-rw-rw-   0        0        0      266 2024-05-20 08:28:47.000000 jzai-59.83.46/jzai/cli.py
--rw-rw-rw-   0        0        0      885 2024-05-17 02:19:53.000000 jzai-59.83.46/jzai/db.py
--rw-rw-rw-   0        0        0      258 2024-05-17 02:22:13.000000 jzai-59.83.46/jzai/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:29:09.253199 jzai-59.83.46/jzai.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 08:29:09.000000 jzai-59.83.46/jzai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 08:29:09.255979 jzai-59.83.46/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-20 08:29:05.000000 jzai-59.83.46/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:33:54.211055 jzai-59.83.47/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:33:54.210002 jzai-59.83.47/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 02:18:49.000000 jzai-59.83.47/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 08:33:54.191077 jzai-59.83.47/jzai/
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:31:07.000000 jzai-59.83.47/jzai/__init__.py
+-rw-rw-rw-   0        0        0     9373 2024-05-20 08:33:38.000000 jzai-59.83.47/jzai/bot.py
+-rw-rw-rw-   0        0        0      256 2024-05-20 08:31:28.000000 jzai-59.83.47/jzai/cli.py
+-rw-rw-rw-   0        0        0      875 2024-05-20 08:31:32.000000 jzai-59.83.47/jzai/db.py
+-rw-rw-rw-   0        0        0      248 2024-05-20 08:31:36.000000 jzai-59.83.47/jzai/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:33:54.208988 jzai-59.83.47/jzai.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-20 08:33:54.000000 jzai-59.83.47/jzai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-20 08:33:54.000000 jzai-59.83.47/jzai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:33:54.000000 jzai-59.83.47/jzai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-20 08:33:54.000000 jzai-59.83.47/jzai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-20 08:33:54.000000 jzai-59.83.47/jzai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-20 08:33:54.000000 jzai-59.83.47/jzai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:33:54.212461 jzai-59.83.47/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-20 08:33:49.000000 jzai-59.83.47/setup.py
```

### Comparing `jzai-59.83.46/jzai/bot.py` & `jzai-59.83.47/jzai/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#bot.py
 import os
 import json
 import re
 import hashlib
 import pyttsx3
 import speech_recognition as sr
 from nltk.tokenize import word_tokenize
@@ -193,15 +194,15 @@
             print(f"{self.current_user if self.current_user else 'You'}: {user_input}")
             self.process_input(user_input)
         except sr.UnknownValueError:
             print(f"{self.name}: Sorry, I could not understand your speech.")
         except sr.RequestError as e:
             print(f"{self.name}: Speech recognition request failed:", e)
 
-def main():
+def run():
     bot = Bot(name="JZ")
     asyncio.run(bot.load_users())
 
     try:
         while True:
             if not bot.current_user:
                 user_choice = input("Do you want to (login) or (signup)? ")
@@ -222,8 +223,8 @@
     except KeyboardInterrupt:
         print("\nExiting...")
     finally:
         bot.engine.stop()
 
 if __name__ == "__main__":
     import cProfile
-    cProfile.run('main()')
+    cProfile.run('run()')
```

### Comparing `jzai-59.83.46/jzai/db.py` & `jzai-59.83.47/jzai/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# my_bot_package/db.py
+# jzai/db.py
 
 import json
 import os
 
 USER_DATA_FILE = 'users.json'
 CHAT_LOGS_DIR = 'chat_logs'
```

