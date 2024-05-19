# Comparing `tmp/transcribe_me-0.2.2.tar.gz` & `tmp/transcribe_me-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe_me-0.2.2.tar", last modified: Sun May 19 22:56:42 2024, max compression
+gzip compressed data, was "transcribe_me-0.2.3.tar", last modified: Sun May 19 23:13:15 2024, max compression
```

## Comparing `transcribe_me-0.2.2.tar` & `transcribe_me-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 22:56:42.297164 transcribe_me-0.2.2/
--rw-r--r--   0 johnny     (501) staff       (20)     1069 2024-04-04 11:41:30.000000 transcribe_me-0.2.2/LICENSE
--rw-r--r--   0 johnny     (501) staff       (20)    12265 2024-05-19 22:56:42.296614 transcribe_me-0.2.2/PKG-INFO
--rw-r--r--   0 johnny     (501) staff       (20)    11516 2024-05-19 21:18:12.000000 transcribe_me-0.2.2/README.md
--rw-r--r--   0 johnny     (501) staff       (20)     1034 2024-05-19 22:50:22.000000 transcribe_me-0.2.2/pyproject.toml
--rw-r--r--   0 johnny     (501) staff       (20)       38 2024-05-19 22:56:42.297229 transcribe_me-0.2.2/setup.cfg
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 22:56:42.292935 transcribe_me-0.2.2/transcribe_me/
--rw-r--r--   0 johnny     (501) staff       (20)      183 2024-04-21 03:16:17.000000 transcribe_me-0.2.2/transcribe_me/__init__.py
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 22:56:42.294401 transcribe_me-0.2.2/transcribe_me/audio/
--rw-r--r--   0 johnny     (501) staff       (20)        0 2024-04-20 19:31:16.000000 transcribe_me-0.2.2/transcribe_me/audio/__init__.py
--rw-r--r--   0 johnny     (501) staff       (20)     1152 2024-04-20 19:32:38.000000 transcribe_me-0.2.2/transcribe_me/audio/splitting.py
--rw-r--r--   0 johnny     (501) staff       (20)     3280 2024-04-20 19:32:38.000000 transcribe_me-0.2.2/transcribe_me/audio/transcription.py
--rw-r--r--   0 johnny     (501) staff       (20)     1520 2024-05-19 22:36:48.000000 transcribe_me-0.2.2/transcribe_me/cli.py
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 22:56:42.295138 transcribe_me-0.2.2/transcribe_me/config/
--rw-r--r--   0 johnny     (501) staff       (20)       71 2024-04-20 19:32:38.000000 transcribe_me-0.2.2/transcribe_me/config/__init__.py
--rw-r--r--   0 johnny     (501) staff       (20)     7346 2024-05-19 22:49:47.000000 transcribe_me-0.2.2/transcribe_me/config/config_manager.py
--rw-r--r--   0 johnny     (501) staff       (20)      246 2024-04-20 18:34:10.000000 transcribe_me-0.2.2/transcribe_me/config/schema.yaml
--rw-r--r--   0 johnny     (501) staff       (20)       99 2024-04-20 19:32:38.000000 transcribe_me-0.2.2/transcribe_me/main.py
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 22:56:42.295823 transcribe_me-0.2.2/transcribe_me/summarization/
--rw-r--r--   0 johnny     (501) staff       (20)        0 2024-04-20 19:31:16.000000 transcribe_me-0.2.2/transcribe_me/summarization/__init__.py
--rw-r--r--   0 johnny     (501) staff       (20)     5012 2024-05-19 22:27:58.000000 transcribe_me-0.2.2/transcribe_me/summarization/summarizer.py
-drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 22:56:42.296364 transcribe_me-0.2.2/transcribe_me.egg-info/
--rw-r--r--   0 johnny     (501) staff       (20)    12265 2024-05-19 22:56:42.000000 transcribe_me-0.2.2/transcribe_me.egg-info/PKG-INFO
--rw-r--r--   0 johnny     (501) staff       (20)      614 2024-05-19 22:56:42.000000 transcribe_me-0.2.2/transcribe_me.egg-info/SOURCES.txt
--rw-r--r--   0 johnny     (501) staff       (20)        1 2024-05-19 22:56:42.000000 transcribe_me-0.2.2/transcribe_me.egg-info/dependency_links.txt
--rw-r--r--   0 johnny     (501) staff       (20)       58 2024-05-19 22:56:42.000000 transcribe_me-0.2.2/transcribe_me.egg-info/entry_points.txt
--rw-r--r--   0 johnny     (501) staff       (20)       65 2024-05-19 22:56:42.000000 transcribe_me-0.2.2/transcribe_me.egg-info/requires.txt
--rw-r--r--   0 johnny     (501) staff       (20)       14 2024-05-19 22:56:42.000000 transcribe_me-0.2.2/transcribe_me.egg-info/top_level.txt
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 23:13:15.276309 transcribe_me-0.2.3/
+-rw-r--r--   0 johnny     (501) staff       (20)     1069 2024-04-04 11:41:30.000000 transcribe_me-0.2.3/LICENSE
+-rw-r--r--   0 johnny     (501) staff       (20)    12265 2024-05-19 23:13:15.275942 transcribe_me-0.2.3/PKG-INFO
+-rw-r--r--   0 johnny     (501) staff       (20)    11516 2024-05-19 21:18:12.000000 transcribe_me-0.2.3/README.md
+-rw-r--r--   0 johnny     (501) staff       (20)     1034 2024-05-19 22:50:22.000000 transcribe_me-0.2.3/pyproject.toml
+-rw-r--r--   0 johnny     (501) staff       (20)       38 2024-05-19 23:13:15.276354 transcribe_me-0.2.3/setup.cfg
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 23:13:15.272069 transcribe_me-0.2.3/transcribe_me/
+-rw-r--r--   0 johnny     (501) staff       (20)      183 2024-04-21 03:16:17.000000 transcribe_me-0.2.3/transcribe_me/__init__.py
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 23:13:15.273588 transcribe_me-0.2.3/transcribe_me/audio/
+-rw-r--r--   0 johnny     (501) staff       (20)        0 2024-04-20 19:31:16.000000 transcribe_me-0.2.3/transcribe_me/audio/__init__.py
+-rw-r--r--   0 johnny     (501) staff       (20)     1152 2024-04-20 19:32:38.000000 transcribe_me-0.2.3/transcribe_me/audio/splitting.py
+-rw-r--r--   0 johnny     (501) staff       (20)     3280 2024-04-20 19:32:38.000000 transcribe_me-0.2.3/transcribe_me/audio/transcription.py
+-rw-r--r--   0 johnny     (501) staff       (20)     1520 2024-05-19 22:59:38.000000 transcribe_me-0.2.3/transcribe_me/cli.py
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 23:13:15.274493 transcribe_me-0.2.3/transcribe_me/config/
+-rw-r--r--   0 johnny     (501) staff       (20)       71 2024-04-20 19:32:38.000000 transcribe_me-0.2.3/transcribe_me/config/__init__.py
+-rw-r--r--   0 johnny     (501) staff       (20)     7346 2024-05-19 22:49:47.000000 transcribe_me-0.2.3/transcribe_me/config/config_manager.py
+-rw-r--r--   0 johnny     (501) staff       (20)      246 2024-04-20 18:34:10.000000 transcribe_me-0.2.3/transcribe_me/config/schema.yaml
+-rw-r--r--   0 johnny     (501) staff       (20)       99 2024-04-20 19:32:38.000000 transcribe_me-0.2.3/transcribe_me/main.py
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 23:13:15.275009 transcribe_me-0.2.3/transcribe_me/summarization/
+-rw-r--r--   0 johnny     (501) staff       (20)        0 2024-04-20 19:31:16.000000 transcribe_me-0.2.3/transcribe_me/summarization/__init__.py
+-rw-r--r--   0 johnny     (501) staff       (20)     5012 2024-05-19 22:27:58.000000 transcribe_me-0.2.3/transcribe_me/summarization/summarizer.py
+drwxr-xr-x   0 johnny     (501) staff       (20)        0 2024-05-19 23:13:15.275602 transcribe_me-0.2.3/transcribe_me.egg-info/
+-rw-r--r--   0 johnny     (501) staff       (20)    12265 2024-05-19 23:13:15.000000 transcribe_me-0.2.3/transcribe_me.egg-info/PKG-INFO
+-rw-r--r--   0 johnny     (501) staff       (20)      614 2024-05-19 23:13:15.000000 transcribe_me-0.2.3/transcribe_me.egg-info/SOURCES.txt
+-rw-r--r--   0 johnny     (501) staff       (20)        1 2024-05-19 23:13:15.000000 transcribe_me-0.2.3/transcribe_me.egg-info/dependency_links.txt
+-rw-r--r--   0 johnny     (501) staff       (20)       58 2024-05-19 23:13:15.000000 transcribe_me-0.2.3/transcribe_me.egg-info/entry_points.txt
+-rw-r--r--   0 johnny     (501) staff       (20)       65 2024-05-19 23:13:15.000000 transcribe_me-0.2.3/transcribe_me.egg-info/requires.txt
+-rw-r--r--   0 johnny     (501) staff       (20)       14 2024-05-19 23:13:15.000000 transcribe_me-0.2.3/transcribe_me.egg-info/top_level.txt
```

### Comparing `transcribe_me-0.2.2/LICENSE` & `transcribe_me-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.2.2/PKG-INFO` & `transcribe_me-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-me
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI tool to transcribe audio files using OpenAI API
 Author-email: echoHello <bash@echohello.dev>
 Project-URL: Homepage, https://github.com/echohello-dev/transcribe-me
 Project-URL: Bug Tracker, https://github.com/echohello-dev/transcribe-me/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `transcribe_me-0.2.2/README.md` & `transcribe_me-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.2.2/pyproject.toml` & `transcribe_me-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.2.2/transcribe_me/audio/splitting.py` & `transcribe_me-0.2.3/transcribe_me/audio/splitting.py`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.2.2/transcribe_me/audio/transcription.py` & `transcribe_me-0.2.3/transcribe_me/audio/transcription.py`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.2.2/transcribe_me/cli.py` & `transcribe_me-0.2.3/transcribe_me/cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,22 +36,22 @@
         config_manager.install_config()
         return
 
     if args.command == "archive":
         config_manager.archive_files(args.input, args.output)
         return
 
-    if args.command == "only":
-        transcription.process_audio_files(input_folder, output_folder, config)
-        return
-
     config = config_manager.load_config()
 
     input_folder = args.input
     output_folder = args.output
 
+    if args.command == "only":
+        transcription.process_audio_files(input_folder, output_folder, config)
+        return
+
     transcription.process_audio_files(input_folder, output_folder, config)
     summarizer.generate_summaries(input_folder, output_folder, config)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `transcribe_me-0.2.2/transcribe_me/config/config_manager.py` & `transcribe_me-0.2.3/transcribe_me/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.2.2/transcribe_me/summarization/summarizer.py` & `transcribe_me-0.2.3/transcribe_me/summarization/summarizer.py`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.2.2/transcribe_me.egg-info/PKG-INFO` & `transcribe_me-0.2.3/transcribe_me.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-me
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI tool to transcribe audio files using OpenAI API
 Author-email: echoHello <bash@echohello.dev>
 Project-URL: Homepage, https://github.com/echohello-dev/transcribe-me
 Project-URL: Bug Tracker, https://github.com/echohello-dev/transcribe-me/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `transcribe_me-0.2.2/transcribe_me.egg-info/SOURCES.txt` & `transcribe_me-0.2.3/transcribe_me.egg-info/SOURCES.txt`

 * *Files identical despite different names*

