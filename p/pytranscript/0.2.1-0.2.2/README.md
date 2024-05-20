# Comparing `tmp/pytranscript-0.2.1.tar.gz` & `tmp/pytranscript-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytranscript-0.2.1.tar", last modified: Sun May 19 22:47:00 2024, max compression
+gzip compressed data, was "pytranscript-0.2.2.tar", last modified: Mon May 20 01:58:58 2024, max compression
```

## Comparing `pytranscript-0.2.1.tar` & `pytranscript-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:47:00.136238 pytranscript-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-19 22:46:54.000000 pytranscript-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-19 22:47:00.136238 pytranscript-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-19 22:46:54.000000 pytranscript-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-19 22:46:54.000000 pytranscript-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:47:00.136238 pytranscript-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:47:00.132238 pytranscript-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:47:00.132238 pytranscript-0.2.1/src/pytranscript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-19 22:47:00.000000 pytranscript-0.2.1/src/pytranscript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-19 22:47:00.000000 pytranscript-0.2.1/src/pytranscript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:47:00.000000 pytranscript-0.2.1/src/pytranscript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 22:47:00.000000 pytranscript-0.2.1/src/pytranscript.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-19 22:47:00.000000 pytranscript-0.2.1/src/pytranscript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 22:47:00.000000 pytranscript-0.2.1/src/pytranscript.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16600 2024-05-19 22:46:54.000000 pytranscript-0.2.1/src/pytranscript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:58:58.007921 pytranscript-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 01:58:53.000000 pytranscript-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-20 01:58:58.007921 pytranscript-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-20 01:58:53.000000 pytranscript-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-20 01:58:53.000000 pytranscript-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:58:58.007921 pytranscript-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:58:58.007921 pytranscript-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:58:58.007921 pytranscript-0.2.2/src/pytranscript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-20 01:58:57.000000 pytranscript-0.2.2/src/pytranscript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-20 01:58:58.000000 pytranscript-0.2.2/src/pytranscript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:58:57.000000 pytranscript-0.2.2/src/pytranscript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 01:58:57.000000 pytranscript-0.2.2/src/pytranscript.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 01:58:57.000000 pytranscript-0.2.2/src/pytranscript.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 01:58:57.000000 pytranscript-0.2.2/src/pytranscript.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18389 2024-05-20 01:58:53.000000 pytranscript-0.2.2/src/pytranscript.py
```

### Comparing `pytranscript-0.2.1/LICENSE` & `pytranscript-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytranscript-0.2.1/PKG-INFO` & `pytranscript-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytranscript
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI to transcript and translate audio and video files
 Author-email: arnaud-ma <arnaudma.code@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [arnaud-ma]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,45 +66,45 @@
 pytranscript INPUT_FILE [OPTIONS]
 ```
 
 ### Options
 
 - `-m, --model` - Path to the Vosk model directory. Always required.
 - `-o, --output` - Output file where the text will be saved. Default: input file name with `.txt` extension.
+- `-f, --format` - Format of the transcript. Must be one of 'csv', 'json', 'srt', 'txt', 'vtt' or 'all'. Default: input file extension.
 - `-li, --lang_input` - Language of the input / the model. Default: auto.
 - `-lo --lang_input` - Language to translate the text to. Default: no translation.
 - `-s, --start` - Start time of the audio to transcribe in seconds.
 - `-e, --end` - End time of the audio to transcribe in seconds.
 - `--max_size` - Will stop the transcription if the output file reaches the specified size in bytes. Takes precedence over the `--end` option.
 - `--keep-wav` - Keep the converted audio wav file after the process is done.
 - `-v, -verbosity` - Verbosity level. 0: no output, 1: only errors, 2: errors, info and progressbar, 3: debug. Default: 2.
 
 ## Example
 
 The most basic usage is:
 
 ```bash
-pytranscript video.mp4 -m vosk-model-en-us-aspire-0.2 -lo fr
+pytranscript video.mp4 -m vosk-model-en-us-aspire-0.2 -lo fr -f srt
 ```
 
-Where `vosk-model-en-us-aspire-0.2` is the Vosk model directory. The text will be translated from English to French, and the output will be saved in a file named `video.txt`.
+Where `vosk-model-en-us-aspire-0.2` is the Vosk model directory. The text will be translated from English to French, and the output will be saved in `video.srt`.
 
 Using the `keep-wav` option can be useful if you want to do many transcriptions within the same file, allowing you to use the same `.wav` file for each transcription, thus saving conversion time.
  ⚠️ The `.wav` file is cropped according to the start and end time options.
 
 ### API
 
-The API provides a Transcript object containing the time and text. The `translate` method can be used to get another Transcript object with the translated text. The output saved in a file in the cli is just the string
-`str(transcript)`.
+The API provides a Transcript object containing the time and text. The `translate` method can be used to get another Transcript object with the translated text. The output saved in a file in the cli is just a method
+`to_{format}` of the Transcript object.
 
 A reproduction of the previous example using the API:
 
 ```python
 import pytranscript as pt
 
-wav_file = pt.to_valid_wav('video.mp4', "video.wav", start=0, end=None)
-transcript = pt.transcribe(wav_file, model='vosk-model-en-us-aspire-0.2', max_size=None)
-transcript_fr = transcript.translate('fr')
+wav_file = pt.to_valid_wav("video.mp4", "video.wav", start=0, end=None)
+transcript = pt.transcribe(wav_file, model="vosk-model-en-us-aspire-0.2", max_size=None)
+transcript_fr, errors = transcript.translate("fr")
 
-with open('video.txt', 'w', encoding="utf8") as f:
-    f.write(str(transcript_fr))
+transcript_fr.write("video.srt")
 ```
```

### Comparing `pytranscript-0.2.1/README.md` & `pytranscript-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,45 +23,45 @@
 pytranscript INPUT_FILE [OPTIONS]
 ```
 
 ### Options
 
 - `-m, --model` - Path to the Vosk model directory. Always required.
 - `-o, --output` - Output file where the text will be saved. Default: input file name with `.txt` extension.
+- `-f, --format` - Format of the transcript. Must be one of 'csv', 'json', 'srt', 'txt', 'vtt' or 'all'. Default: input file extension.
 - `-li, --lang_input` - Language of the input / the model. Default: auto.
 - `-lo --lang_input` - Language to translate the text to. Default: no translation.
 - `-s, --start` - Start time of the audio to transcribe in seconds.
 - `-e, --end` - End time of the audio to transcribe in seconds.
 - `--max_size` - Will stop the transcription if the output file reaches the specified size in bytes. Takes precedence over the `--end` option.
 - `--keep-wav` - Keep the converted audio wav file after the process is done.
 - `-v, -verbosity` - Verbosity level. 0: no output, 1: only errors, 2: errors, info and progressbar, 3: debug. Default: 2.
 
 ## Example
 
 The most basic usage is:
 
 ```bash
-pytranscript video.mp4 -m vosk-model-en-us-aspire-0.2 -lo fr
+pytranscript video.mp4 -m vosk-model-en-us-aspire-0.2 -lo fr -f srt
 ```
 
-Where `vosk-model-en-us-aspire-0.2` is the Vosk model directory. The text will be translated from English to French, and the output will be saved in a file named `video.txt`.
+Where `vosk-model-en-us-aspire-0.2` is the Vosk model directory. The text will be translated from English to French, and the output will be saved in `video.srt`.
 
 Using the `keep-wav` option can be useful if you want to do many transcriptions within the same file, allowing you to use the same `.wav` file for each transcription, thus saving conversion time.
  ⚠️ The `.wav` file is cropped according to the start and end time options.
 
 ### API
 
-The API provides a Transcript object containing the time and text. The `translate` method can be used to get another Transcript object with the translated text. The output saved in a file in the cli is just the string
-`str(transcript)`.
+The API provides a Transcript object containing the time and text. The `translate` method can be used to get another Transcript object with the translated text. The output saved in a file in the cli is just a method
+`to_{format}` of the Transcript object.
 
 A reproduction of the previous example using the API:
 
 ```python
 import pytranscript as pt
 
-wav_file = pt.to_valid_wav('video.mp4', "video.wav", start=0, end=None)
-transcript = pt.transcribe(wav_file, model='vosk-model-en-us-aspire-0.2', max_size=None)
-transcript_fr = transcript.translate('fr')
+wav_file = pt.to_valid_wav("video.mp4", "video.wav", start=0, end=None)
+transcript = pt.transcribe(wav_file, model="vosk-model-en-us-aspire-0.2", max_size=None)
+transcript_fr, errors = transcript.translate("fr")
 
-with open('video.txt', 'w', encoding="utf8") as f:
-    f.write(str(transcript_fr))
+transcript_fr.write("video.srt")
 ```
```

### Comparing `pytranscript-0.2.1/pyproject.toml` & `pytranscript-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#writing-pyproject-toml
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytranscript"
-version = "0.2.1"
+version = "0.2.2"
 description = "CLI to transcript and translate audio and video files"
 readme = "README.md"
 requires-python = ">=3.12"
 license = {file = "LICENSE"}
 keywords = ["transcript", "translation", "audio", "video", "subtitles"]
 authors = [{ name = "arnaud-ma", email = "arnaudma.code@gmail.com" }]
 classifiers = [ # https://pypi.org/classifiers/
```

### Comparing `pytranscript-0.2.1/src/pytranscript.egg-info/PKG-INFO` & `pytranscript-0.2.2/src/pytranscript.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytranscript
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI to transcript and translate audio and video files
 Author-email: arnaud-ma <arnaudma.code@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [arnaud-ma]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,45 +66,45 @@
 pytranscript INPUT_FILE [OPTIONS]
 ```
 
 ### Options
 
 - `-m, --model` - Path to the Vosk model directory. Always required.
 - `-o, --output` - Output file where the text will be saved. Default: input file name with `.txt` extension.
+- `-f, --format` - Format of the transcript. Must be one of 'csv', 'json', 'srt', 'txt', 'vtt' or 'all'. Default: input file extension.
 - `-li, --lang_input` - Language of the input / the model. Default: auto.
 - `-lo --lang_input` - Language to translate the text to. Default: no translation.
 - `-s, --start` - Start time of the audio to transcribe in seconds.
 - `-e, --end` - End time of the audio to transcribe in seconds.
 - `--max_size` - Will stop the transcription if the output file reaches the specified size in bytes. Takes precedence over the `--end` option.
 - `--keep-wav` - Keep the converted audio wav file after the process is done.
 - `-v, -verbosity` - Verbosity level. 0: no output, 1: only errors, 2: errors, info and progressbar, 3: debug. Default: 2.
 
 ## Example
 
 The most basic usage is:
 
 ```bash
-pytranscript video.mp4 -m vosk-model-en-us-aspire-0.2 -lo fr
+pytranscript video.mp4 -m vosk-model-en-us-aspire-0.2 -lo fr -f srt
 ```
 
-Where `vosk-model-en-us-aspire-0.2` is the Vosk model directory. The text will be translated from English to French, and the output will be saved in a file named `video.txt`.
+Where `vosk-model-en-us-aspire-0.2` is the Vosk model directory. The text will be translated from English to French, and the output will be saved in `video.srt`.
 
 Using the `keep-wav` option can be useful if you want to do many transcriptions within the same file, allowing you to use the same `.wav` file for each transcription, thus saving conversion time.
  ⚠️ The `.wav` file is cropped according to the start and end time options.
 
 ### API
 
-The API provides a Transcript object containing the time and text. The `translate` method can be used to get another Transcript object with the translated text. The output saved in a file in the cli is just the string
-`str(transcript)`.
+The API provides a Transcript object containing the time and text. The `translate` method can be used to get another Transcript object with the translated text. The output saved in a file in the cli is just a method
+`to_{format}` of the Transcript object.
 
 A reproduction of the previous example using the API:
 
 ```python
 import pytranscript as pt
 
-wav_file = pt.to_valid_wav('video.mp4', "video.wav", start=0, end=None)
-transcript = pt.transcribe(wav_file, model='vosk-model-en-us-aspire-0.2', max_size=None)
-transcript_fr = transcript.translate('fr')
+wav_file = pt.to_valid_wav("video.mp4", "video.wav", start=0, end=None)
+transcript = pt.transcribe(wav_file, model="vosk-model-en-us-aspire-0.2", max_size=None)
+transcript_fr, errors = transcript.translate("fr")
 
-with open('video.txt', 'w', encoding="utf8") as f:
-    f.write(str(transcript_fr))
+transcript_fr.write("video.srt")
 ```
```

### Comparing `pytranscript-0.2.1/src/pytranscript.py` & `pytranscript-0.2.2/src/pytranscript.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,26 @@
 
     Args:
         time (list[float]): a list of the time of each line in the transcript.
         text (list[str]): a list of the text of each line in the transcript.
         language (str): the language of the transcript. Default: "auto"
         time_end (float): the time of the last line in the transcript. If not specified,
         it will be the time of the last line + 5 seconds.
+
+    Methods:
+        append(time: float, text: str) -> None: append a new line to the transcript
+        translate(target: str) -> tuple[Transcript, list[LineError]]: translate the
+            transcript to the target language
+        {srt or vtt or csv or txt}_generator() -> generator: generate t
+            the transcript as a string in SRT, VTT, CSV, JSON or TXT format,
+            line by line
+        to_{srt or vtt or csv or txt or json}() -> str: return the transcript
+            as a string in SRT, VTT, CSV, JSON or TXT format
+        write(output: StrPath) -> None: write the transcript to a file, the format
+            will be inferred from the file extension
     """
 
     time: list[float] = field(default_factory=list)
     text: list[str] = field(default_factory=list)
     language: str = "auto"
     time_end: float | None = None
 
@@ -101,20 +113,14 @@
             return self.time_end
         return self.time[-1] + 5
 
     def append(self, time: float, text: str) -> None:
         self.time.append(time)
         self.text.append(text)
 
-    def __str__(self):
-        return "\n".join(
-            f"{seconds_to_time(time)} : {line}"
-            for time, line in zip(self.time, self.text, strict=True)
-        )
-
     def __len__(self):
         return len(self.time)
 
     def __getitem__(self, key):
         return self.time[key], self.text[key]
 
     def translate(self, target: str) -> tuple[Transcript, list[LineError]]:
@@ -177,43 +183,55 @@
 
     def csv_generator(self):
         """Generate the transcript as a string in CSV format, line by line."""
         yield "time,text\n"
         for time, line in zip(self.time, self.text, strict=True):
             yield f"{time},{line}\n"
 
+    def txt_generator(self):
+        """Generate the transcript as a string in TXT format, line by line."""
+        for time, line in zip(self.time, self.text, strict=True):
+            yield f"{seconds_to_time(time)} : {line}\n"
+
     def to_srt(self) -> str:
         """Return the transcript as a string in SRT format."""
         return "".join(self.srt_generator())
 
     def to_vtt(self) -> str:
         """Return the transcript as a string in VTT format."""
         return "".join(self.vtt_generator())
 
     def to_json(self) -> str:
         """Return the transcript as a string in JSON format."""
         return json.dumps({"text": self.text, "time": self.time})
 
     def to_txt(self) -> str:
         """Return the transcript as a string in TXT format."""
-        return str(self)
+        return "".join(self.txt_generator())
 
     def to_csv(self) -> str:
         """Return the transcript as a string in CSV format."""
         return "".join(self.csv_generator())
 
-    def write(self, output: StrPath, format: TranscriptFormat) -> None:  # noqa: A002
+    def write(self, output: StrPath) -> None:
         """Write the transcript to a file.
 
         Args:
-            output (Path): the path to the output file.
-            format (TranscriptFormat): the format of the transcript.
+            output (Path): the path to the output file. The format will be inferred
+            from the file extension.
+            It must be one of 'csv', 'json', 'srt', 'txt' or 'vtt'.
         """
-        method = getattr(self, f"to_{format}")
-        Path(output).write_text(method())
+        output = Path(output)
+        fmt = output.suffix[1:]  # type: ignore
+        if fmt not in TRANSCRIPT_FORMATS:
+            msg = f"Unknown format for {output.name}: {fmt}"
+            raise ValueError(msg)
+
+        method = getattr(self, f"to_{fmt}")
+        output.write_text(method())
 
 
 def to_valid_wav(
     source: StrPath,
     output: StrPath | None = None,
     start: float = 0,
     end: float | None = None,
@@ -280,48 +298,48 @@
     except (IndexError, KeyError):
         warnings.warn("No time found in the result", stacklevel=2)
         return None
     return time, result_dict.get("text", "")
 
 
 def transcribe(
-    input_file: StrPath, model_path: StrPath, max_size: int | None = None
+    input_file: StrPath, model: StrPath, max_size: int | None = None
 ) -> Transcript:
     """Transcribe a  mono PCM 16-bit WAV file using a vosk model
     (https://alphacephei.com/vosk/models).
 
     Args:
         input_file (str): the transcript file, must be a mono PCM 16-bit WAV file.
-        model_path (str): the vosk model path
+        model (str): the vosk model path
         max_size (bool, optional): Transcribe only the first max_size bytes of the file.
         If not specified, the whole file will be transcribed.
 
     Raises:
         FileNotFoundError: A file is not found at the given path
         TypeError: The input file is not a wav file
 
     Returns:
         Transcript: the transcript of the file
     """
     input_file = Path(input_file)
-    model_path = Path(model_path)
+    model = Path(model)
 
     if not input_file.is_file():
         msg = f"{input_file} not found"
         raise FileNotFoundError(msg)
 
-    if not model_path.exists():
-        msg = f"{model_path} not found"
+    if not model.exists():
+        msg = f"{model} not found"
         raise FileNotFoundError(msg)
 
     if not _is_valid_wav_file(input_file):
         msg = f"{input_file} is not a valid WAV file"
         raise TypeError(msg)
-    model = vosk.Model(str(model_path))
-    rec = _initialize_recognizer(model, input_file)
+    vosk_model = vosk.Model(str(model))
+    rec = _initialize_recognizer(vosk_model, input_file)
 
     return transcribe_with_vosk(input_file, rec, max_size)
 
 
 def _is_valid_wav_file(input_file: Path) -> bool:
     """Validate if the input file is a valid WAV file."""
     try:
@@ -393,18 +411,18 @@
 
     output: Path | None = None
     """
     the path to the output file. Default: same as the input file with only the extension
     changed
     """
 
-    format: str = "all"
+    format: str | None = None
     """
-    the format of the transcript. Must be one of 'csv', 'json', 'srt', 'txt', 'vtt'
-    or 'all'. Default: 'all'
+    the format of the transcript. Must be one of 'csv', 'json', 'srt', 'txt', 'vtt',
+    'all' or 'auto'. Default: the format will be inferred from the output file extension
     """
 
     model: Path = Path("model")
     "the path to the vosk model"
 
     lan_output: str | None = None  # the language of the transcript
     "the language of the output transcript. Default: no translation"
@@ -424,19 +442,40 @@
     keep_wav: bool = False
     "keep the wav file after the transcript"
 
     verbosity: int = 2
     """Verbosity level. 0: no output, 1: only errors, 2: errors, info and progressbar,
     3: debug. Default: 2."""
 
-    def process_args(self):
-        if self.format not in typing.get_args(AllTranscriptFormats):
+    def _init_format(self):
+        if not (
+            self.format in typing.get_args(AllTranscriptFormats) or self.format is None
+        ):
             msg = f"bad transcript format: {self.format}"
             raise ValueError(msg)
 
+        match (self.output, self.format):
+            case (None, None):
+                self.format = "all"
+                self.output = self.input.with_suffix("")
+
+            case (None, _):
+                self.output = self.input.with_suffix(f".{self.format}")
+
+            case (_, None):
+                if self.output.is_dir():
+                    self.output = self.output / self.input.stem
+                    self.format = "all"
+                else:
+                    self.format = self.output.suffix[1:]
+
+            case _:
+                pass
+
+    def _init_verbose(self):
         vosk.SetLogLevel(-1)  # disable vosk logs
         match self.verbosity:
             case 0:
                 logging.disable()
             case 1:
                 logging.basicConfig(level=logging.ERROR)
             case 2:
@@ -444,31 +483,36 @@
             case 3:
                 logging.basicConfig(level=logging.DEBUG)
                 vosk.SetLogLevel(0)
             case _:
                 msg = "verbosity must be 0, 1, 2 or 3"
                 raise ValueError(msg)
 
+    def process_args(self):
+        self._init_format()
+        self._init_verbose()
+
     def configure(self):
         self.add_argument("input")
         self.add_argument("-o", "--output")
         self.add_argument("-f", "--format")
         self.add_argument("-m", "--model")
         self.add_argument("-li", "--lan_input")
         self.add_argument("-lo", "--lan_output")
         self.add_argument("-s", "--start")
         self.add_argument("-e", "--end")
         self.add_argument("-v", "--verbosity")
 
     def get_output(self, fmt: TranscriptFormat) -> Path:
-        if self.output is None:
-            if self.format == "all":
-                return self.input.with_suffix(f".{fmt}")
+        if self.output is not None:
+            return self.output
+
+        if self.format == "all":
             return self.input.with_suffix(f".{fmt}")
-        return self.output
+        return self.input.with_suffix(f".{fmt}")
 
     def translate(self, transcript: Transcript):
         if self.lan_output is None:
             return transcript
 
         new_transcript, errors = transcript.translate(self.lan_output)
         if errors:
@@ -478,25 +522,26 @@
 
 
 # ruff: noqa: G004
 def main():
     logging.basicConfig(level=logging.INFO)
     parser = ArgumentParser()
     args = parser.parse_args()
+
     logging.info(f"Convert {args.input} to WAV format")
     wav_file = to_valid_wav(args.input, start=args.start, end=args.end)
 
     logging.info(f"Transcribe {wav_file}...")
     transcript = transcribe(wav_file, args.model, args.max_size)
 
     if not args.keep_wav:
+        # we can remove the file if we don't need it anymore
         wav_file.unlink()
 
     transcript.language = args.lan_input
-
     new_transcript = args.translate(transcript)
 
     if args.format == "all":
         for fmt in TRANSCRIPT_FORMATS:
-            new_transcript.write(args.get_output(fmt), fmt)
+            new_transcript.write(args.get_output(fmt))
     else:
-        new_transcript.write(args.get_output(args.format), args.format)
+        new_transcript.write(args.get_output(args.format))
```

