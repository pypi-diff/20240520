# Comparing `tmp/transcribe_me-0.2.0.tar.gz` & `tmp/transcribe_me-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe_me-0.2.0.tar", last modified: Sun Apr 21 03:18:01 2024, max compression
+gzip compressed data, was "transcribe_me-0.2.1.tar", last modified: Sun May 19 22:30:54 2024, max compression
```

## Comparing `transcribe_me-0.2.0.tar` & `transcribe_me-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:18:01.552845 transcribe_me-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 03:15:31.000000 transcribe_me-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-04-21 03:18:01.552845 transcribe_me-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-21 03:15:31.000000 transcribe_me-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-21 03:15:31.000000 transcribe_me-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 03:18:01.552845 transcribe_me-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:18:01.552845 transcribe_me-0.2.0/transcribe_me/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-21 03:15:31.000000 transcribe_me-0.2.0/transcribe_me/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-21 03:15:31.000000 transcribe_me-0.2.0/transcribe_me/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-21 03:15:31.000000 transcribe_me-0.2.0/transcribe_me/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:18:01.552845 transcribe_me-0.2.0/transcribe_me.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-04-21 03:18:01.000000 transcribe_me-0.2.0/transcribe_me.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-21 03:18:01.000000 transcribe_me-0.2.0/transcribe_me.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:18:01.000000 transcribe_me-0.2.0/transcribe_me.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 03:18:01.000000 transcribe_me-0.2.0/transcribe_me.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-21 03:18:01.000000 transcribe_me-0.2.0/transcribe_me.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 03:18:01.000000 transcribe_me-0.2.0/transcribe_me.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:30:54.253239 transcribe_me-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-19 22:28:43.000000 transcribe_me-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-19 22:30:54.253239 transcribe_me-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-05-19 22:28:43.000000 transcribe_me-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-19 22:28:43.000000 transcribe_me-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:30:54.253239 transcribe_me-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:30:54.249239 transcribe_me-0.2.1/transcribe_me/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 22:28:43.000000 transcribe_me-0.2.1/transcribe_me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-19 22:28:43.000000 transcribe_me-0.2.1/transcribe_me/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-19 22:28:43.000000 transcribe_me-0.2.1/transcribe_me/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:30:54.249239 transcribe_me-0.2.1/transcribe_me.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-19 22:30:54.000000 transcribe_me-0.2.1/transcribe_me.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-19 22:30:54.000000 transcribe_me-0.2.1/transcribe_me.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:30:54.000000 transcribe_me-0.2.1/transcribe_me.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-19 22:30:54.000000 transcribe_me-0.2.1/transcribe_me.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-19 22:30:54.000000 transcribe_me-0.2.1/transcribe_me.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 22:30:54.000000 transcribe_me-0.2.1/transcribe_me.egg-info/top_level.txt
```

### Comparing `transcribe_me-0.2.0/LICENSE` & `transcribe_me-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.2.0/PKG-INFO` & `transcribe_me-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-me
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI tool to transcribe audio files using OpenAI API
 Author-email: echoHello <bash@echohello.dev>
 Project-URL: Homepage, https://github.com/echohello-dev/transcribe-me
 Project-URL: Bug Tracker, https://github.com/echohello-dev/transcribe-me/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -106,14 +106,20 @@
 
 4. (Optional) You can archive the input directory to keep track of the processed audio files:
 
    ```bash
    transcribe-me archive
    ```
 
+5. (Optional) You can also transcribe only the audio files that have not been transcribed yet:
+
+    ```bash
+    transcribe-me only
+    ```
+
 ### Docker
 
 You can also run the application using Docker:
 
 1. Install Docker on your machine by following the instructions on the [Docker website](https://docs.docker.com/get-docker/).
 
 2. Create a `.transcribe.yaml` configuration file:
```

### Comparing `transcribe_me-0.2.0/README.md` & `transcribe_me-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,20 @@
 
 4. (Optional) You can archive the input directory to keep track of the processed audio files:
 
    ```bash
    transcribe-me archive
    ```
 
+5. (Optional) You can also transcribe only the audio files that have not been transcribed yet:
+
+    ```bash
+    transcribe-me only
+    ```
+
 ### Docker
 
 You can also run the application using Docker:
 
 1. Install Docker on your machine by following the instructions on the [Docker website](https://docs.docker.com/get-docker/).
 
 2. Create a `.transcribe.yaml` configuration file:
```

### Comparing `transcribe_me-0.2.0/pyproject.toml` & `transcribe_me-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `transcribe_me-0.2.0/transcribe_me/cli.py` & `transcribe_me-0.2.1/transcribe_me/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def parse_arguments():
     parser = argparse.ArgumentParser(
         description="Transcribe audio files and generate summaries."
     )
     parser.add_argument(
         "command",
         nargs="?",
-        choices=["install", "archive"],
+        choices=["install", "archive", "only"],
         help="Install the configuration file or archive files.",
     )
     parser.add_argument(
         "--input",
         type=str,
         default="input",
         help="Path to the input folder containing audio files.",
@@ -36,14 +36,18 @@
         config_manager.install_config()
         return
 
     if args.command == "archive":
         config_manager.archive_files(args.input, args.output)
         return
 
+    if args.command == "only":
+        transcription.process_audio_files(input_folder, output_folder, config)
+        return
+
     config = config_manager.load_config()
 
     input_folder = args.input
     output_folder = args.output
 
     transcription.process_audio_files(input_folder, output_folder, config)
     summarizer.generate_summaries(input_folder, output_folder, config)
```

### Comparing `transcribe_me-0.2.0/transcribe_me.egg-info/PKG-INFO` & `transcribe_me-0.2.1/transcribe_me.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-me
-Version: 0.2.0
+Version: 0.2.1
 Summary: A CLI tool to transcribe audio files using OpenAI API
 Author-email: echoHello <bash@echohello.dev>
 Project-URL: Homepage, https://github.com/echohello-dev/transcribe-me
 Project-URL: Bug Tracker, https://github.com/echohello-dev/transcribe-me/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -106,14 +106,20 @@
 
 4. (Optional) You can archive the input directory to keep track of the processed audio files:
 
    ```bash
    transcribe-me archive
    ```
 
+5. (Optional) You can also transcribe only the audio files that have not been transcribed yet:
+
+    ```bash
+    transcribe-me only
+    ```
+
 ### Docker
 
 You can also run the application using Docker:
 
 1. Install Docker on your machine by following the instructions on the [Docker website](https://docs.docker.com/get-docker/).
 
 2. Create a `.transcribe.yaml` configuration file:
```

