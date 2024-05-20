# Comparing `tmp/storybuilder-0.0.34-py3-none-any.whl.zip` & `tmp/storybuilder-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 15221 bytes, number of entries: 12
--rw-rw-r--  2.0 unx      112 b- defN 24-May-13 12:34 storybuilder/__init__.py
--rw-rw-r--  2.0 unx     4732 b- defN 24-May-13 12:34 storybuilder/characterpostures.py
--rw-rw-r--  2.0 unx     2012 b- defN 24-May-16 10:05 storybuilder/cosuploader.py
--rw-rw-r--  2.0 unx     5305 b- defN 24-May-13 12:34 storybuilder/speechsynthesizer.py
--rw-rw-r--  2.0 unx    41353 b- defN 24-May-16 12:27 storybuilder/storybuilder.py
--rw-rw-r--  2.0 unx     4599 b- defN 24-May-16 05:44 storybuilder/storyprofiles.py
--rw-rw-r--  2.0 unx     2652 b- defN 24-May-14 09:53 storybuilder/storyvoicebuilder.py
--rw-r--r--  2.0 unx     1062 b- defN 24-May-16 12:27 storybuilder-0.0.34.dist-info/LICENSE
--rw-rw-r--  2.0 unx      869 b- defN 24-May-16 12:27 storybuilder-0.0.34.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-16 12:27 storybuilder-0.0.34.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 24-May-16 12:27 storybuilder-0.0.34.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1021 b- defN 24-May-16 12:27 storybuilder-0.0.34.dist-info/RECORD
-12 files, 63822 bytes uncompressed, 13495 bytes compressed:  78.9%
+Zip file size: 13537 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      112 b- defN 24-May-13 03:49 storybuilder/__init__.py
+-rw-r--r--  2.0 unx     1601 b- defN 24-May-13 03:38 storybuilder/cosuploader.py
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-13 04:00 storybuilder/speechsynthesizer.py
+-rw-r--r--  2.0 unx    31502 b- defN 24-May-13 05:58 storybuilder/storybuilder.py
+-rw-r--r--  2.0 unx     4715 b- defN 24-May-12 15:23 storybuilder/storyprofiles.py
+-rw-r--r--  2.0 unx     2631 b- defN 24-May-13 04:01 storybuilder/storyvoicebuilder.py
+-rw-r--r--  2.0 unx     1062 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      699 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      926 b- defN 24-May-13 05:59 storybuilder-0.0.9.dist-info/RECORD
+11 files, 48658 bytes uncompressed, 11963 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,13 +1,10 @@
 Filename: storybuilder/__init__.py
 Comment: 
 
-Filename: storybuilder/characterpostures.py
-Comment: 
-
 Filename: storybuilder/cosuploader.py
 Comment: 
 
 Filename: storybuilder/speechsynthesizer.py
 Comment: 
 
 Filename: storybuilder/storybuilder.py
@@ -15,23 +12,23 @@
 
 Filename: storybuilder/storyprofiles.py
 Comment: 
 
 Filename: storybuilder/storyvoicebuilder.py
 Comment: 
 
-Filename: storybuilder-0.0.34.dist-info/LICENSE
+Filename: storybuilder-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: storybuilder-0.0.34.dist-info/METADATA
+Filename: storybuilder-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: storybuilder-0.0.34.dist-info/WHEEL
+Filename: storybuilder-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: storybuilder-0.0.34.dist-info/top_level.txt
+Filename: storybuilder-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: storybuilder-0.0.34.dist-info/RECORD
+Filename: storybuilder-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## storybuilder/cosuploader.py

```diff
@@ -1,64 +1,39 @@
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
-from qcloud_cos import CosServiceError
-from qcloud_cos import CosClientError
 
 import os
 import hashlib
 
-
 class CosUploader:
-    def __init__(
-        self,
-        service_root,
-        cos_region,
-        cos_secret_id,
-        cos_secret_key,
-        cos_bucket,
-        cos_token=None,
-        cos_scheme="https",
-    ):
+    def __init__(self, service_root, cos_region, cos_secret_id, cos_secret_key, cos_bucket, cos_token=None, cos_scheme="https"):
         self.service_root = service_root
-        self._config = CosConfig(
-            Region=cos_region,
-            SecretId=cos_secret_id,
-            SecretKey=cos_secret_key,
-            Token=cos_token,
-            Scheme=cos_scheme,
-        )
+        self._config = CosConfig(Region=cos_region, SecretId=cos_secret_id, SecretKey=cos_secret_key, Token=cos_token, Scheme=cos_scheme)
         self._client = CosS3Client(self._config)
         self._bucket = cos_bucket
 
     def calculate_file_hash(self, file_path):
         hash_md5 = hashlib.md5()
         with open(file_path, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_md5.update(chunk)
         return hash_md5.hexdigest()
 
     def get_file_name(self, file_path):
         filename, file_extension = os.path.splitext(os.path.basename(file_path))
         return filename + "_" + self.calculate_file_hash(file_path) + file_extension
-
-    def local2cos(self, local_path, storyId, target_relative_path="test"):
-        if target_relative_path is None:
-            target_relative_path = ""
-        elif len(target_relative_path) > 0:
-            target_relative_path = (
-                target_relative_path
-                if target_relative_path[0] != "/"
-                else target_relative_path[1:]
-            )
+        
+    def local2cos(self, local_path, storyId, target_relative_path='test'):
         try:
-            filename = os.path.join(
-                target_relative_path,
-                storyId,
-                # self.get_file_name(local_path),
-                os.path.basename(local_path),
-            )
+            filename = os.path.join(self.site_root, 
+                                    target_relative_path if target_relative_path[0] !='/' else target_relative_path[1:], 
+                                    storyId, 
+                                    self.get_file_name(local_path))
         except:
-            print("file not found:", local_path)
+            print("file not found =========", local_path)
+
         response = self._client.upload_file(
-            Bucket=self._bucket, LocalFilePath=local_path, Key=filename
+            Bucket=self._bucket,
+            LocalFilePath=local_path,
+            Key=filename
         )
-        return "/"+filename
+        return filename
```

## storybuilder/storybuilder.py

```diff
@@ -4,176 +4,146 @@
 import uuid
 import copy
 import re
 import xml.etree.ElementTree as ET
 from PIL import Image
 
 from .storyprofiles import CHARACTER_FIGURE_ACCESSORY_KEYS, STORY_SCENARIO_STYLES
-from .characterpostures import CHARACTER_FIGURES
-
-DEFAULT_LANGUAGE="zh-CN"
-LANGUAGE_ENG="en-US"
-DEFAULT_NARRATOR="M"
 
 class Story:
-
-    @staticmethod
-    def test(page):
-        #path = os.path.join(page.storyId, "test.json")
-        #directory = os.path.dirname(path)
-        #if not os.path.exists(directory):
-        #    os.makedirs(directory)
-        with open("test.json", "w") as file:
-            json.dump(
-                page.export(), file, ensure_ascii=False, indent=4, sort_keys=False
-            )
-
-    @staticmethod
-    def removeEmojis(text):
-        emojiPattern = re.compile(pattern = "["
-            u"\U0001F600-\U0001F64F"  # emoticons
-            u"\U0001F300-\U0001F5FF"  # symbols & pictographs
-            u"\U0001F680-\U0001F6FF"  # transport & map symbols
-            u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
-            u"\U0001F926-\U0001F991"
-                            "]+", flags = re.UNICODE)
-        return re.sub(emojiPattern, '', text)
-
+    
     @staticmethod
     def retrieveSvgSize(image_path):
         # Load the SVG file
-        tree = ET.parse(image_path)
+        tree = ET.parse(image_path) 
         root = tree.getroot()
-
+        
         # Extract attributes from the <svg> tag
-        width = root.get("width", 0)  # Get the width attribute
-        height = root.get("height", 0)  # Get the height attribute
-        viewBox = root.get("viewBox", "0, 0, 0, 0")  # Get the viewBox attribute
-
-        split_pattern = r"[ ,]+"
-
-        return [int(width), int(height)], [
-            int(float(num)) for num in re.split(split_pattern, viewBox)
-        ]
-
+        width = root.get('width', 0)  # Get the width attribute
+        height = root.get('height', 0)  # Get the height attribute
+        viewBox = root.get('viewBox', '0, 0, 0, 0')  # Get the viewBox attribute
+    
+        split_pattern = r'[ ,]+'
+        
+        return [int(width), int(height)], [int(num) for num in re.split(split_pattern, viewBox)]
+    
     @staticmethod
     def retrievePixelSize(image_path):
         # Open the image using the Python Imaging Library (PIL)
         image = Image.open(image_path)
-
+    
         # Get the width and height of the image in pixels
         width, height = image.size
-
+    
         # Return the width and height as a tuple
         return width, height
-
+    
     @staticmethod
     def getImageSize(file_path):
         width = height = 0
         try:
-            if ".svg" in file_path[-4:]:
+            if '.svg' in file_path[-4:]:
                 dim2, dim4 = Story.retrieveSvgSize(file_path)
-                if dim2 == [0, 0]:
+                if dim2 == [0,0]:
                     width = dim4[2]
                     height = dim4[3]
                 else:
                     width = dim2[0]
                     height = dim2[1]
-            elif (
-                ".jpg" in file_path[-4:]
-                or ".jpeg" in file_path[-5:]
-                or ".png" in file_path[-4:]
-                or ".gif" in file_path[-4:]
-            ):
+            elif '.jpg' in file_path[-4:] or '.jpeg' in file_path[-5:] or '.png' in file_path[-4:] or '.gif' in file_path[-4:]:
                 width, height = Story.retrievePixelSize(file_path)
         except:
-            print("retrieve image file size error:", file_path)
+                print('retrieve image file size error =========', file_path)
         return width, height
 
-    def __init__(self, title, storyId=None, style="shinkai_makoto", mode="test", **kwargs):
+    def _loadStoryDataDefaults(self, filename, key='defaultCharacters'):
+        with open(filename) as f:
+            data = f.read()
+    
+        pattern = r'export const (\w+) = (.*?)(;)'
+        flags = re.DOTALL | re.MULTILINE
+    
+        matches = re.finditer(pattern, data, flags=flags)
+    
+        # Replace export const with key:
+        matched = {key:None}
+        for one_match in matches:
+            if one_match.group(1) == key:
+                cleaned_string = one_match.group(2).strip().replace('\n', '').replace(',]', ']')
+                matched[key] = json.loads(cleaned_string)
+        
+        return matched
+
+    
+    def __init__(self, title, storyId=None, style="shinkai_makoto", **kwargs):
         self.title = title
-        self.storyId = storyId if storyId != None else uuid.uuid4()
+        self.storyId = storyId if storyId!=None else uuid.uuid4()
         self.styles = STORY_SCENARIO_STYLES[style]
-        self.locale = kwargs["locale"] if "locale" in kwargs else DEFAULT_LANGUAGE
-        self.narrator = kwargs["narrator"] if "narrator" in kwargs else DEFAULT_NARRATOR
+        self.locale = kwargs["locale"] if "locale" in kwargs else "cn"
+        self.narrator = kwargs["narrator"] if "narrator" in kwargs else "M"
         self.pages = []
-        assert mode.lower() in ("test", "production")
-        self.mode=mode.lower()
-        if self.mode == "production":
-            self.posterPath = 'story/posters/'
-            self.audioPath = 'story/audios/'
-        else:
-            self.posterPath = 'test/posters/'
-            self.audioPath = 'test/audios/'
 
         self._cosUploader = kwargs["uploader"] if "uploader" in kwargs else None
         self._synthesizer = kwargs["synthesizer"] if "synthesizer" in kwargs else None
+        
+        self._defaultCharacters = None
+        # 需要提供defaultdata.tsx源文件所在项目根路径
+        figureSource = kwargs["figureSource"] if "figureSource" in kwargs else None
+        if figureSource != None:
+            print("Load default character figure info at", figureSource)
 
-        self._defaultCharacters = CHARACTER_FIGURES
-
-        print(f"New story Title: {title}, Id:", self.storyId)
+            self._defaultCharacters = self._loadStoryDataDefaults(figureSource, key='defaultCharacters')['defaultCharacters']
+        else:
+            print("No source file for default character figure loaded, please input number for posture variable.")
 
-    def getAudioPath(self, fileName):
-        return os.path.join("/", self.audioPath, self.storyId, fileName)
+        print("New story Id", self.storyId)
 
-    def getUserPostureId(
-        self, actor, postures, keyScenario="stand", excludeAccessories=True
-    ):
+    def getUserPostureId(self, actor, postures, keyScenario = 'stand', excludeAccessories=True):
         if type(postures) is int:
             return postures
         if type(postures) is list and type(postures[0]) is int:
             return postures[0]
         if self._defaultCharacters == None:
             return 0
 
-        currentActorFigures = self._defaultCharacters[actor]
+        currentActorFigures = self._defaultCharacters[actor]['figure']
         availableFigures = []
         for j, figure in enumerate(currentActorFigures):
+            fullFigure = figure['source'].split('/')[-1]
             skip = False
             if excludeAccessories:
                 for accessory in CHARACTER_FIGURE_ACCESSORY_KEYS:
-                    if accessory in figure:
+                    if accessory in fullFigure:
                         skip = True
             if skip:
                 continue
-            if keyScenario in figure and all(keyWord in figure for keyWord in postures):
-                availableFigures.append({"index": j, "figure": figure})
+            if keyScenario in fullFigure and all(keyWord in fullFigure for keyWord in postures):
+                availableFigures.append({'index':j, 'figure':fullFigure.split('.')[0]})
         if len(availableFigures) > 0:
-            return random.choice(availableFigures)["index"]
+            return random.choice(availableFigures)['index']
         else:
             return 0
 
     def appendPage(self, page):
         self.pages.append(page)
 
     def insertPage(self, pos, page):
         self.pages.insert(pos, page)
 
     def createPage(self, sceneType, **kwargs):
-        if sceneType.lower() not in (
-            "exam",
-            "notes",
-            "cover",
-            "blackboard",
-            "concentrak",
-            "classroom",
-        ):
-            raise Exception(
-                f"Invalid scenario type {sceneType}, must be one of ('exam', 'notes', 'cover', 'blackboard', 'concentrak', 'classroom')"
-            )
-
+        if sceneType.lower() not in ("exam", "notes", "cover", "blackboard", "concentrak", "classroom"):
+            raise Exception(f"Invalid scenario type {sceneType}, must be one of ('exam', 'notes', 'cover', 'blackboard', 'concentrak', 'classroom')")
+        
         newPage = None
 
         if sceneType.lower() == "classroom":
             if "actor" not in kwargs:
                 raise Exception(f'argument "actor" is required')
             if "postures" in kwargs:
-                newPage = ClassroomPage(
-                    self, kwargs["actor"], postures=kwargs["postures"]
-                )
+                newPage = ClassroomPage(self, kwargs["actor"], postures=kwargs["postures"])
             else:
                 newPage = ClassroomPage(self, kwargs["actor"])
         elif sceneType.lower() == "blackboard":
             if "source" not in kwargs:
                 raise Exception(f'argument "source" is required')
             if "rect" in kwargs:
                 newPage = BlackboardPage(self, kwargs["source"], rect=kwargs["rect"])
@@ -211,52 +181,40 @@
         return newPage
 
     def export(self):
         voices = [{"sound": "/story/audios/OurMusicBox - 24 Hour Coverage - intro.mp3"}]
         events = []
         for page in self.pages:
             pageObject = page.export(voiceOffset=len(voices), pageId=float(len(events)))
-            voices = voices + [
-                {"sound": entry["sound"]} for entry in pageObject["voices"]
-            ]
+            voices = voices + [{"sound": entry["sound"]} for entry in pageObject["voices"]]
             events = events + pageObject["events"]
 
         return {"voices": voices, "events": events}
 
     def exportScripts(self):
         voices = []
-        for i, page in enumerate(self.pages):
+        for page in self.pages:
             pageObject = page.export(voiceOffset=len(voices))
-            voices = voices + [{"page": i, "voices": pageObject["voices"]}]
+            voices = voices + pageObject["voices"]
 
         return voices
-
-    def exportAudios(self, localOutputPath, uploadToCos=False):
+    
+    def exportAudios(self, outputPath):
         if self._synthesizer:
             voices = self.exportScripts()
-            for page in voices:
-                for i, voice in enumerate(page["voices"]):
-                    fileName = os.path.basename(voice["sound"])
-                    character = voice["narrator"]
-                    for language in voice["subscript"]:
-                        subscript = (
-                            voice["alternative"][language]
-                            if ("alternative" in voice) and (language in voice["alternative"]) and (voice["alternative"][language] != None)
-                            else voice["subscript"][language]
-                        )
-                        print(f'page/script id: {page["page"]}/{i}')
-                        self._synthesizer.synthesizeFile(
-                            character, self.removeEmojis(subscript), language, localOutputPath, fileName
-                        )
-                        localOutputFileName = os.path.join(localOutputPath, fileName)
-
-                        if  self._cosUploader != None and uploadToCos:
-                            _ = self._cosUploader.local2cos(localOutputFileName, self.storyId, self.audioPath)    
-                        
-
+            for voice in voices:
+                fileName = voice["sound"]
+                character = voice["narrator"]
+                for language in voice["subscript"]:
+                    subscript = voice["alternative"][language] if "alternative" in voice else voice["subscript"][language]
+                    self._synthesizer.synthesizeFile(character, 
+                                                     subscript, 
+                                                     language, 
+                                                     outputPath, 
+                                                     fileName)
 
 class Page:
     def __init__(self, type, storyInstance):
         self.story = storyInstance
         self.narrator = storyInstance.narrator
         self.locale = storyInstance.locale
         self.type = type
@@ -267,779 +225,536 @@
         self.subscripts = []
         self.narrations = []
         self.actor = ""
 
     def _getUserId(self, actor):
         userId = -1
         for i, object in enumerate(self.objects):
-            if object["name"].lower() == actor.lower():
+            if object["name"].upper() == actor.upper():
                 userId = i
-
+    
         if userId == -1:
-            self.objects.append({"name": actor})
+            self.objects.append({"name":actor})
             userId = len(self.objects) - 1
         return userId
 
-    def updateScript(
-        self, scriptId: int, text=None, actor=None, alternativeText=None, locale=None
-    ):
+    def updateScript(self, scriptId: int, text=None, actor=None, alternativeText=None, locale=None):
         locale = self.locale if locale == None else locale
         if len(self.subscripts) > 0 and scriptId < len(self.subscripts):
             if text != None:
-                self.subscripts[scriptId]["subscript"][locale] = text
+                self.subscripts[scriptId]['subscript'][locale] = text 
             if actor != None:
-                self.subscripts[scriptId]["narrator"] = actor
+                self.subscripts[scriptId]['narrator'] = actor
             if alternativeText != None:
-                if "alternative" not in self.subscripts[scriptId]:
-                    self.subscripts[scriptId]["alternative"] = {locale: alternativeText}
-                else:
-                    self.subscripts[scriptId]["alternative"][locale] = alternativeText
+                self.subscripts[scriptId]['alternative'][locale] = alternativeText 
         else:
             scriptId = scriptId - len(self.subscript)
             if len(self.narrations) > 0 and scriptId < len(self.narrations):
                 if text != None:
-                    self.narrations[scriptId]["subscript"][locale] = text
+                    self.narrations[scriptId]['subscript'][locale] = text 
                 if actor != None:
-                    self.narrations[scriptId]["narrator"] = actor
+                    self.narrations[scriptId]['narrator'] = actor
                 if alternativeText != None:
-                    self.narrations[scriptId]["alternative"][locale] = alternativeText
+                    self.narrations[scriptId]['alternative'][locale] = alternativeText             
 
     def export(self, voiceOffset=0, pageId=0.0):
         raise NotImplementedError("Subclasses must implement export()")
 
-
 ##### 问答页面 #####
 class ExamPage(Page):
     def __init__(self, storyInstance, actor, postures=["smilesay"]):
         super().__init__("exam", storyInstance)
         self.scene = self.story.styles["scenarios"]["exam"]
         self.actor = actor
-        self.defaultObject = "exam"
-        self.soundFile = self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3")
 
-        posture_list = (
-            [postures]
-            if (isinstance(postures, str) or isinstance(postures, int))
-            else postures
-        )
-        self.interactions.append(
-            {
-                "start": "",
-                "duration": "",
-                "position": self.story.styles["positions"]["right-bottom"],
-                "transform": "scale(1.5, 1.5)",
-                "figure": self.story.getUserPostureId(
-                    actor, posture_list, keyScenario="half"
-                ),
-                "type": "motion",
-                "actor": self._getUserId(self.actor),
-            }
-        )
+        posture_list = [postures] if (isinstance(postures, str) or isinstance(postures, int)) else postures      
+        self.interactions.append({
+          "start": "",
+          "duration": "",
+          "position": self.story.styles["positions"]["right-bottom"],
+          "transform": "scale(1.5, 1.5)",
+          "figure": self.story.getUserPostureId(actor, posture_list, keyScenario='half'),
+          "type": "motion",
+          "actor": self._getUserId(self.actor)
+        })
         self.questionInteractions = []
         self.questionSubscripts = []
 
     def setQuestion(self, question, options, answers=[], **kwargs):
         assert isinstance(options, list)
         answer_list = list(answers) if not isinstance(answers, list) else answers
-
+        
         self.board = {
-            "content": {
-                "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else 20,
-                "fontColor": "white",
-                "question": {self.locale: question},
-                "options": {self.locale: options},
-                "answer": {self.locale: answer_list},
-                "colsPerRow": kwargs["colsPerRow"] if "colsPerRow" in kwargs else 1,
-            },
-            "type": "exam",
-            "rect": kwargs["rect"] if "rect" in kwargs else [0, 0, 1, 1],
+          "content": {
+          "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else 20,
+          "fontColor": "white",
+          "question": {self.locale: question},
+          "options": {self.locale: options},
+          "answer": {self.locale: answer_list},
+          "colsPerRow": kwargs["colsPerRow"] if "colsPerRow" in kwargs else 1
+        },
+        "type": "exam",
+        "rect": kwargs["rect"] if "rect" in kwargs else [0, 0, 1, 1]
         }
 
         self.correctAnswerId = 0
         for i, option in enumerate(options):
             for entry in answer_list:
                 if entry == option:
                     self.correctAnswerId += 2**i
 
         self.questionInteractions = []
         self.questionSubscripts = []
+        # 错误答案提示行为 onResult: -1
+        self.questionInteractions.append({
+          "start": "",
+          "duration": "",
+          "onResult": -1,
+          "content": {
+            "popup": 4,
+            "voice": -1,
+            "text": {self.locale: kwargs["alwaysTruePrompt"]} if "alwaysTruePrompt" in kwargs else {"cn":"再想想", "en": "Try again"}
+          },
+          "actor": self._getUserId("exam"),
+          "type": "talk"
+        })
 
         # 添加初始化问题语音
-        self.questionSubscripts = [{
-                "sound": self.soundFile,
-                "subscript": {self.locale: question},
-                "narrator": self.actor,
-            }]
-
+        self.questionSubscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", "subscript":question, "narrator": self.actor})
         # 初始化页面行为 onResult: -2
-        self.questionInteractions.append(
-            {
-                "start": "",
-                "duration": "",
-                "onResult": -2,
-                "content": {
-                    "popup": 4,
-                    "voice": len(self.questionSubscripts) - 1,
-                    "text": "",
-                },
-                "actor": self._getUserId(self.defaultObject),
-                "type": "talk",
-            }
-        )
-
-        # 错误答案提示行为 onResult: -1
-        self.questionInteractions.append(
-            {
-                "start": "",
-                "duration": "",
-                "onResult": -1,
-                "content": {
-                    "popup": 4,
-                    "voice": -1,
-                    "text": (
-                        {self.locale: kwargs["alwaysTruePrompt"]}
-                        if "alwaysTruePrompt" in kwargs
-                        else {DEFAULT_LANGUAGE: "再想想", LANGUAGE_ENG: "Try again"}
-                    ),
-                },
-                "actor": self._getUserId(self.defaultObject),
-                "type": "talk",
-            }
-        )
+        self.questionInteractions.append({
+          "start": "",
+          "duration": "auto",
+          "onResult": -2,
+          "content": {
+            "popup": 4,
+            "voice": len(self.questionSubscripts)-1,
+            "text": ""
+          },
+          "actor": self._getUserId("exam"),
+          "type": "talk"
+        })
 
         # 正确答案行为 onResult: 由所有正确答案id计算所得
-        if self.correctAnswerId > 0:
-            self.questionInteractions.append(
-                {
-                    "start": "",
-                    "duration": "",
-                    "onResult": self.correctAnswerId,
-                    "content": {"popup": 2, "text": ""},
-                    "actor": self._getUserId(self.defaultObject),
-                    "type": "talk",
-                }
-            )
-
+        if self.answerId > 0:
+            self.questionInteractions.append({
+              "start": "",
+              "duration": "",
+              "onResult": self.correctAnswerId,
+              "content": {
+                "popup": 2,
+                "text": ""
+              },
+              "actor": self._getUserId("exam"),
+              "type": "talk"
+            })            
+    
     def setFontSize(self, size):
         self.board["fontSize"] = size
-
+    
     def setColsPerRow(self, colsPerRow):
         self.board["colsPerRow"] = colsPerRow
 
     def setRect(self, rect):
         self.board["rect"] = rect
 
     def setFontColor(self, color):
         self.board["fontColor"] = color
 
-    def addImage(self, source, rect=[0, 0, 1, 1], uploadToCos=True, caption=None):
-        assert len(rect) >= 4 and type(rect) is list
+    def addImage(self, source, rect=[0,0,1,1], **kwargs):
+        assert len(rect)>=4 and type(rect) is list
         if "contentList" not in self.board:
-            self.board["contentList"] = []
-
-        if  self.story._cosUploader != None and uploadToCos:
-            source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)    
-
-        self.board["contentList"].append(
-            {
-                "rect": rect,
-                "image": {self.locale: source},
-            }
-        )
-        if caption != None and len(caption) > 0:
-            self.board["contentList"][-1]["caption"] = {self.locale: caption}
-
-    def updateImage(self, pos, source, rect=[0, 0, 1, 1], uploadToCos=True, caption=None):
-        if pos < len(self.board["contentList"]) and pos >= 0:
-            assert len(rect) >= 4 and type(rect) is list
-
-            if  self.story._cosUploader != None and uploadToCos:
-                source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)    
-
-            self.board["contentList"][pos] = {
-                    "rect": rect,
-                    "image": {self.locale: source},
-                }
+            self.board["contentList"] = []    
             
-            if caption != None and len(caption) > 0:
-                self.board["contentList"][pos]["caption"] = {self.locale: caption}
-
-    def removeImage(self, pos):
-        if pos < len(self.board["contentList"]) and pos >= 0:
-            self.board["contentList"].pop(pos)
+        if  self.story._cosUploader != None:
+            target_path = kwargs["targetPath"] if "targetPath" in kwargs else None
+            source = self.story._cosUploader.local2cos(source, self.story.storyId, target_path)    
+        
+        self.board["contentList"].append({
+            "caption": {self.locale: kwargs["caption"]} if "caption" in kwargs else "",
+            "rect": rect,
+            "image": {"cn" : source}
+          })
 
     def export(self, voiceOffset=0, pageId=0.0):
         outSubscripts = self.subscripts + self.questionSubscripts
         outInteractions = self.interactions + self.questionInteractions
 
+        interactionOffset = len(self.interactions)
         for i, interaction in enumerate(outInteractions):
-            if (
-                "content" in interaction
-                and interaction["content"].get("voice", -1) >= 0
-            ):
-                outInteractions[i]["content"]["voice"] += voiceOffset
-
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
+                outInteractions[i]["content"]["voice"] += voiceOffset + (0 if i < interactionOffset else interactionOffset)
+        
         return {
             "voices": outSubscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene,
-                    "board": self.board,
-                    "objects": self.objects,
-                    "interactions": outInteractions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            ],
+            ]
         }
 
-
 ##### 总结页面 #####
 class NotesPage(Page):
     RESERVED_VOICE = -999
-
-    def __init__(self, storyInstance, actor, postures=["smilesay"], endingEffect=True):
+    def __init__(self, storyInstance, actor, postures=["smilesay"]):
         super().__init__("notes", storyInstance)
         self.scene = self.story.styles["scenarios"]["notes"]["scene"]
         self.board = self.story.styles["scenarios"]["notes"]["board"]
         self.bullets = []
-        self.actor = actor
-        self.defaultObject = "ending"
-        self.soundFile = self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3")
-
-        if endingEffect:
-            self.interactions.append(
-                {
-                    "start": "",
-                    "duration": "",
-                    "content": {"text": "", "voice": self.RESERVED_VOICE},
-                    "type": "talk",
-                    "actor": self._getUserId(self.defaultObject),
-                }
-            )
-
-        posture_list = (
-            [postures]
-            if (isinstance(postures, str) or isinstance(postures, int))
-            else postures
-        )
-        self.interactions.insert(
-            0,
-            {
-                "start": "",
-                "duration": "",
-                "position": self.story.styles["positions"]["right-bottom"],
-                "transform": "scale(1.5, 1.5)",
-                "figure": self.story.getUserPostureId(
-                    actor, posture_list, keyScenario="half"
-                ),
-                "type": "motion",
-                "actor": self._getUserId(actor),
+        self.interactions.append({
+            "start": "",
+            "duration": "",
+            "content": {
+                "text": "",
+                "voice": self.RESERVED_VOICE
             },
-        )
+            "type": "talk",
+            "actor": self._getUserId("ending")
+        })
+
+        posture_list = [postures] if (isinstance(postures, str) or isinstance(postures, int)) else postures
+        self.interactions.insert(0, {
+            "start": "",
+            "duration": "",
+            "position": self.story.styles["positions"]["right-bottom"],
+            "transform": "scale(1.5, 1.5)",
+            "figure": self.story.getUserPostureId(actor, posture_list, keyScenario='half'),
+            "type": "motion",
+            "actor": self._getUserId(actor)
+        })
+        self.actor = actor
 
     def addBullet(self, text):
         self.bullets.append(text)
 
-    def updateBullet(self, pos, text):
-        if pos < len(self.bulltes) and pos >= 0:
-            self.bullets[pos] = text
-
-    def removeBullet(self, pos):
-        if pos < len(self.bulltes) and pos >= 0:
-            self.bullets.pop(pos)
-
     def export(self, voiceOffset=0, pageId=0.0):
         bullets_string = subscript = ""
         for bullet in self.bullets:
             bullets_string += f"<li>{bullet}</li>"
-        subscript = "<break time=\"1500ms\"/>".join(self.bullets)
+            subscript += f"{bullet}..."
 
         outBoard = copy.deepcopy(self.board)
-        outBoard["content"]["html"] = {
-            self.locale: outBoard["content"]["html"].format(bullets_string)
-        }
+        outBoard["content"]["html"] = {self.locale: outBoard["content"]["html"].format(bullets_string)}
 
         outSubscripts = copy.deepcopy(self.subscripts)
-        outSubscripts.append(
-            {
-                "sound": self.soundFile,
-                "subscript": {self.locale: subscript},
-                "narrator": self.actor,
-            }
-        )
+        outSubscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", "subscript":{self.locale:subscript}, "narrator": self.actor})
 
         outInteractions = copy.deepcopy(self.interactions)
-        outInteractions.insert(
-            len(outInteractions) - 1,
-            {
-                "start": "",
-                "duration": "",
-                "content": {"popup": 4, "voice": len(outSubscripts) - 1, "text": ""},
-                "type": "talk",
-                "actor": self._getUserId(self.defaultObject),
-            },
-        )
+        outInteractions.insert(len(outInteractions)-1, {
+            "start": "",
+            "duration": "",
+            "content": {"popup": 4, "voice": len(outSubscripts)-1, "text": ""},
+            "type": "talk",
+            "actor": self._getUserId(self.actor)
+        })
         for i, interaction in enumerate(outInteractions):
             if "content" in interaction:
                 if interaction["content"].get("voice", -1) >= 0:
                     outInteractions[i]["content"]["voice"] += voiceOffset
                 elif interaction["content"].get("voice", -1) == self.RESERVED_VOICE:
                     outInteractions[i]["content"]["voice"] = 0
 
         return {
             "voices": outSubscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene,
-                    "board": outBoard,
-                    "objects": self.objects,
-                    "interactions": outInteractions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": outBoard,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            ],
+            ]
         }
 
-
 ##### 黑板页面 #####
 class BlackboardPage(Page):
-    def __init__(self, storyInstance, source, rect=[0, 0, 1, 1], uploadToCos=True):
-        assert len(rect) >= 4 and type(rect) is list
+    def __init__(self, storyInstance, source, rect=[0,0,1,1]):
+        assert len(rect)>=4 and type(rect) is list
         super().__init__("blackboard", storyInstance)
         self.scene = self.story.styles["scenarios"]["blackboard"]
-
-        if  self.story._cosUploader != None and uploadToCos:
-            source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)
-
-        self.board = {"content": {"image": {self.locale: source}}, "rect": rect}
+        self.board = {
+            "content": {"image": source},
+            "rect": rect
+        }
 
     def addNarration(self, text, narrator=None, alternativeText=None):
-        if alternativeText != None:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3"),
-                    "subscript": {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                }
-            )
+        if alternativeText != None:          
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator
+                                })
         else:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3"),
-                    "subscript": {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                    "alternative": {self.locale: alternativeText},
-                }
-            )
-        self.interactions.append(
-            {
-                "start": "",
-                "duration": "auto",
-                "content": {
-                    "popup": 4,
-                    "voice": len(self.subscripts) - 1,
-                    "text": {self.locale: text},
-                },
-                "actor": self._getUserId(
-                    narrator if narrator != None else self.narrator
-                ),
-                "type": "talk",
-            }
-        )
-
-    def updateNarration(self, pos, text, narrator=None, alternativeText=None):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts[pos]["subscript"][self.locale] = text
-            self.interactions[pos]["content"]["text"][self.locale] = text
-            if narrator != None:
-                self.subscripts[pos]["narrator"] = narrator
-                self.interactions[pos]["actor"] = self._getUserId(narrator)
-            if alternativeText != None:
-                self.subscripts[pos]["alternative"][self.locale] = alternativeText
-
-    def removeNarration(self, pos):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts.pop(pos)
-            self.interactions.pop(pos)
-            if pos < len(self.interactions):
-                for i, interaction in enumerate(self.interactions[pos:]):
-                    self.interactions[i]["content"]["voice"] = interaction["content"]["voice"] - 1
-
-    def updateImage(self, source=None, rect=None, locale=None, uploadToCos=True):
-        if source != None:
-            if  self.story._cosUploader != None and uploadToCos:
-                source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)
-                
-            self.board["content"]["image"][
-                locale if locale != None else self.locale
-            ] = source
-        if rect != None:
-            self.board["content"]["rect"] = rect
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator,
+                                "alternative": {self.locale: alternativeText}})
+        self.interactions.append({
+            "start": "",
+            "duration": "",
+            "content": {
+                "popup": 4,
+                "voice": len(self.subscripts)-1,
+                "text": {self.locale: text}
+            },
+            "actor": self._getUserId(narrator if narrator!=None else self.narrator),
+            "type": "talk"
+        })
 
     def export(self, voiceOffset=0, pageId=0.0):
         outInteractions = copy.deepcopy(self.interactions)
         for i, interaction in enumerate(outInteractions):
-            if (
-                "content" in interaction
-                and interaction["content"].get("voice", -1) >= 0
-            ):
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
                 outInteractions[i]["content"]["voice"] += voiceOffset
         return {
             "voices": self.subscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene,
-                    "board": self.board,
-                    "objects": self.objects,
-                    "interactions": outInteractions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            ],
+            ]
         }
 
-
 ##### 概念页面 #####
 class ConcentrakPage(Page):
     def __init__(self, storyInstance, text):
         super().__init__("concentrak", storyInstance)
         self.scene = self.story.styles["scenarios"]["concentrak"]
-        self.defaultObject = "concentrak"
-        self.interactions.append(
-            {
-                "start": "",
-                "duration": "",
-                "actor": self._getUserId(self.defaultObject),
-                "content": {"popup": 6, "text": {self.locale: text}},
+        self.narrator = ""
+        self.interactions.append({
+            "start": "",
+            "duration": "",
+            "actor": self._getUserId("concentrak"),
+            "content": {
+                "popup": 6,
+                "voice": -1,
+                "text": {self.locale: text}
             }
-        )
-
-    def addNarration(self, text, narrator=None, alternativeText=None):
+        })
+    
+    def addNarration(self, text, narrator=None, alternativeText=None):            
         if alternativeText != None:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3"),
-                    "subscript": {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                }
-            )
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                    "subscript":{self.locale: text}, 
+                                    "narrator": narrator if narrator!=None else self.narrator})
         else:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3"),
-                    "subscript": {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                    "alternative": {self.locale: alternativeText},
-                }
-            )
-        self.interactions.append(
-            {
-                "start": "",
-                "duration": "auto",
-                "content": {
-                    "popup": 4,
-                    "voice": len(self.subscripts) - 1,
-                    "text": {self.locale: text},
-                },
-                "actor": self._getUserId(
-                    narrator if narrator != None else self.narrator
-                ),
-                "type": "talk",
-            }
-        )
-
-    def updateNarration(self, pos, text, narrator=None, alternativeText=None):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts[pos]["subscript"][self.locale] = text
-            self.interactions[pos]["content"]["text"][self.locale] = text
-            if narrator != None:
-                self.subscripts[pos]["narrator"] = narrator
-                self.interactions[pos]["actor"] = self._getUserId(narrator)
-            if alternativeText != None:
-                self.subscripts[pos]["alternative"][self.locale] = alternativeText
-
-    def removeNarration(self, pos):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts.pop(pos)
-            self.interactions.pop(pos)
-            if pos < len(self.interactions):
-                for i, interaction in enumerate(self.interactions[pos:]):
-                    self.interactions[i]["content"]["voice"] = interaction["content"]["voice"] - 1
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator,
+                                "alternative": {self.locale: alternativeText}})
+        self.interactions.append({
+            "start": "",
+            "duration": "",
+            "content": {
+                "popup": 4,
+                "voice": len(self.subscripts)-1,
+                "text": {self.locale: text}
+            },
+            "actor": self._getUserId(narrator if narrator!=None else self.narrator),
+            "type": "talk"
+        })
 
     def export(self, voiceOffset=0, pageId=0.0):
         outInteractions = copy.deepcopy(self.interactions)
         for i, interaction in enumerate(outInteractions):
-            if (
-                "content" in interaction
-                and interaction["content"].get("voice", -1) >= 0
-            ):
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
                 outInteractions[i]["content"]["voice"] += voiceOffset
         return {
             "voices": self.subscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene,
-                    "board": self.board,
-                    "objects": self.objects,
-                    "interactions": outInteractions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            ],
+            ]
         }
 
-
 ##### 首页页面 #####
 class CoverPage(Page):
-    def __init__(self, storyInstance, source, rect=[0, 0, 1, 1], uploadToCos=True):
-        assert len(rect) >= 4 and type(rect) is list
+    def __init__(self, storyInstance, source, rect=[0,0,1,1]):
+        assert len(rect)>=4 and type(rect) is list
         super().__init__("cover", storyInstance)
         self.scene = self.story.styles["scenarios"]["cover"]
-
-        if self.story._cosUploader != None and uploadToCos:
-            source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)
-
-        self.board = {"content": {"image": {self.locale: source}}, "rect": rect}
-
-    def addNarration(self, text, narrator=None, alternativeText=None):
+        self.board = {
+            "content": {"image": source},
+            "rect": rect
+        }
+    
+    def addNarration(self, text, narrator=None, alternativeText=None):            
         if alternativeText != None:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3"),
-                    "subscript": {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                }
-            )
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                    "subscript":{self.locale: text}, 
+                                    "narrator": narrator if narrator!=None else self.narrator})
         else:
-            self.subscripts.append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3"),
-                    "subscript": {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                    "alternative": {self.locale: alternativeText},
-                }
-            )
-        self.interactions.append(
-            {
-                "start": "",
-                "duration": "",
-                "content": {
-                    "popup": 4,
-                    "voice": len(self.subscripts) - 1,
-                    "text": {self.locale: text},
-                },
-                "actor": self._getUserId(
-                    narrator if narrator != None else self.narrator
-                ),
-                "type": "talk",
-            }
-        )
-
-    def updateNarration(self, pos, text, narrator=None, alternativeText=None):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts[pos]["subscript"][self.locale] = text
-            self.interactions[pos]["content"]["text"][self.locale] = text
-            if narrator != None:
-                self.subscripts[pos]["narrator"] = narrator
-                self.interactions[pos]["actor"] = self._getUserId(narrator)
-            if alternativeText != None:
-                self.subscripts[pos]["alternative"][self.locale] = alternativeText
-
-    def removeNarration(self, pos):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.subscripts.pop(pos)
-            self.interactions.pop(pos)
-            if pos < len(self.interactions):
-                for i, interaction in enumerate(self.interactions[pos:]):
-                    self.interactions[i]["content"]["voice"] = interaction["content"]["voice"] - 1
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator,
+                                "alternative": {self.locale: alternativeText}})
+        self.interactions.append({
+            "start": "",
+            "duration": "",
+            "content": {
+                "popup": 4,
+                "voice": len(self.subscripts)-1,
+                "text": {self.locale: text}
+            },
+            "actor": self._getUserId(narrator if narrator!=None else self.narrator),
+            "type": "talk"
+        })
 
     def export(self, voiceOffset=0, pageId=0.0):
         outInteractions = copy.deepcopy(self.interactions)
         for i, interaction in enumerate(outInteractions):
-            if (
-                "content" in interaction
-                and interaction["content"].get("voice", -1) >= 0
-            ):
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
                 outInteractions[i]["content"]["voice"] += voiceOffset
         return {
             "voices": self.subscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene,
-                    "board": self.board,
-                    "objects": self.objects,
-                    "interactions": self.interactions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": self.interactions
                 }
-            ],
+            ]
         }
 
-
 ##### 教室页面 #####
 class ClassroomPage(Page):
     def __init__(self, storyInstance, actor, postures=["smilesay"]):
         super().__init__("classroom", storyInstance)
         self.scene = self.story.styles["scenarios"]["classroom"]
-        self.narrations = {"subscripts": [], "interactions": []}
+        self.narrations = {"subscripts":[], "interactions":[]}
 
-        posture_list = (
-            [postures]
-            if (isinstance(postures, str) or isinstance(postures, int))
-            else postures
-        )
-        self.subscripts.insert(
-            0,
-            {
-                "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3"),
-                "subscript": {self.locale: ""},
-                "narrator": actor,
-            },
-        )
-        self.interactions.insert(
-            0,
-            {
-                "start": "",
-                "duration": "",
-                "content": {
-                    "popup": self.story.styles["popup"],
-                    "voice": 0,
-                    "text": {self.locale: ""},
-                },
-                "figure": self.story.getUserPostureId(
-                    actor, posture_list, keyScenario="-stand-"
-                ),
-                "position": self.story.styles["positions"][
-                    "left" if actor == "boy" else "right"
-                ],
-                "transform": f'scale({self.story.styles["scale"]}, {self.story.styles["scale"]})',
-                "type": "talk",
-                "actor": self._getUserId(actor),
+        posture_list = [postures] if (isinstance(postures, str) or isinstance(postures, int)) else postures
+        self.subscripts.insert(0, {
+            "sound": f"voice-{uuid.uuid4()}.mp3", 
+            "subscript":{self.locale: ""}, 
+            "narrator": actor
+        })
+        self.interactions.insert(0, {
+            "start": "",
+            "duration": "",
+            "content": {
+                "popup": self.story.styles["popup"],
+                "voice": 0,
+                "text": {self.locale: ""}
             },
-        )
+            "figure": self.story.getUserPostureId(actor, posture_list, keyScenario='-stand-'),
+            "position": self.story.styles["positions"]["left" if actor == "boy" else "right"],
+            "transform": f'scale({self.story.styles["scale"]}, {self.story.styles["scale"]})',
+            "type": "talk",
+            "actor": self._getUserId(actor)
+        })
         self.actor = actor
         self.hasImage = False
 
     def setVoice(self, text, alternativeText=None):
         self.subscripts[0]["subscript"][self.locale] = text
         if alternativeText != None:
             self.subscripts[0]["alternativeText"][self.locale] = alternativeText
         self.interactions[0]["content"]["text"][self.locale] = text
 
-    def setImage(self, source, rect=[0.2, 0.2, 400, 400], autoFit=True, uploadToCos=True, **kwargs):
-        assert len(rect) >= 4 and type(rect) is list
+    def setImage(self, source, autoFit=True, rect=[0.2,0.2,400,400], **kwargs):
+        assert len(rect)>=4 and type(rect) is list
         width, height = Story.getImageSize(source)
         assert width > 0 and height > 0
         assert rect[2] > 0 and rect[3] > 0
 
         if autoFit:
-            # image is wider in ratio
-            if width / height > rect[2] / rect[3]:
-                height = round(rect[2] * height / width, 3)
+            #image is wider in ratio
+            if width/height > rect[2]/rect[3]:
+                height = rect[2]*height/width
                 width = rect[2]
             # vice versa, rect is wider in ratio
             else:
-                width = round(rect[3] * width / height, 3)
+                width = rect[3]*width/height
                 height = rect[3]
-            rect[2] = width
-            rect[3] = height
-
-        if autoFit and self.actor == "boy":
-            if rect[2] > 1.0:
-                rect[0] = round(0.9 - rect[2]/960.0, 3)
-            elif rect[2] < 1.0:
-                rect[0] = 0.9 - rect[2]
 
-        if self.story._cosUploader != None and uploadToCos:
-            source = self.story._cosUploader.local2cos(source, self.story.storyId, self.story.posterPath)
+        if autoFit and self.actor == "girl":
+            if rect[3] > 1.0:
+                rect[0] = 960 * 0.9 - rect[3]
+            elif rect[3] < 1.0:
+                rect[0] = 0.9 - rect[3]
+
+        if self.story._cosUploader != None:
+            target_path = kwargs["targetPath"] if "targetPath" in kwargs else None
+            source = self.story._cosUploader.local2cos(source, self.story.storyId, target_path)
 
         self.board = {
             "content": {
                 "caption": kwargs["caption"] if "caption" in kwargs else "",
                 "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else "24px",
                 "fontColor": kwargs["fontColor"] if "fontColor" in kwargs else "white",
-                "image": {self.locale: source},
+                "image": {"cn" : source},
                 "magnify": True,
-                "border": self.story.styles["frame"],
+                "border": self.story.styles["frame"]
             },
-            "rect": rect,
+            "rect": rect
         }
         self.hasImage = True
 
-    def setVideo(self, source, autoFit=True, rect=[0.1, 0.1, 640, 360], **kwargs):
-        assert len(rect) >= 4 and type(rect) is list
-
-        if autoFit and self.actor == "boy":
-            if rect[2] > 1.0:
-                rect[0] = round(0.9 - rect[2]/0.9, 3)
-            elif rect[2] < 1.0:
-                rect[0] = 0.9 - rect[2]
+    def setVideo(self, source, autoFit=True, rect=[0.1,0.1,640,360], **kwargs):
+        assert len(rect)>=4 and type(rect) is list
 
+        if autoFit and self.actor == "girl":
+            if rect[3] > 1.0:
+                rect[0] = 960 * 0.9 - rect[3]
+            elif rect[3] < 1.0:
+                rect[0] = 0.9 - rect[3]
+            
         self.board = {
             "content": {
                 "caption": kwargs["caption"] if "caption" in kwargs else "",
                 "fontSize": kwargs["fontSize"] if "fontSize" in kwargs else "24px",
                 "fontColor": kwargs["fontColor"] if "fontColor" in kwargs else "white",
-                "src": {self.locale: source},
-                "border": self.story.styles["frame"],
+                "src": source,
+                "border": self.story.styles["frame"]
             },
-            "rect": rect,
+            "rect": rect
         }
         if "videoType" in kwargs:
             self.board["content"]["videoType"] = kwargs["videoType"].lower()
         self.hasImage = True
 
     def addNarration(self, text, narrator=None, alternativeText=None):
         if alternativeText != None:
-            self.narrations["subscripts"].append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3"),
-                    "subscript": {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                }
-            )
+            self.narrations["subscripts"].append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                                  "subscript":{self.locale: text}, 
+                                                  "narrator": narrator if narrator!=None else self.narrator})
         else:
-            self.narrations["subscripts"].append(
-                {
-                    "sound": self.story.getAudioPath(f"voice-{uuid.uuid4()}.mp3"),
-                    "subscript": {self.locale: text},
-                    "narrator": narrator if narrator != None else self.narrator,
-                    "alternative": {self.locale: alternativeText},
-                }
-            )
-        self.narrations["interactions"].append(
-            {
-                "start": "",
-                "duration": "auto",
-                "content": {
-                    "popup": 4,
-                    "voice": len(self.narrations["subscripts"]) - 1,
-                    "text": {self.locale: text},
-                },
-                "onPoster": 1,
-                "actor": self._getUserId(
-                    narrator if narrator != None else self.narrator
-                ),
-                "type": "talk",
-            }
-        )
-
-    def updateNarration(self, pos, text, narrator=None, alternativeText=None):
-        if pos < len(self.subscripts) and pos >= 0:
-            self.narrations["subscripts"][pos]["subscript"][self.locale] = text
-            self.narrations["interactions"][pos]["content"]["text"][self.locale] = text
-            if narrator != None:
-                self.narrations["subscripts"][pos]["narrator"] = narrator
-                self.narrations["interactions"][pos]["actor"] = self._getUserId(narrator)
-            if alternativeText != None:
-                self.narrations["subscripts"][pos]["alternative"][self.locale] = alternativeText
-
-    def removeNarration(self, pos):
-        if pos < len(self.narrations["subscripts"]) and pos >= 0:
-            self.narrations["subscripts"].pop(pos)
-            self.narrations["interactions"].pop(pos)
-            if pos < len(self.narrations["interactions"]):
-                for i, interaction in enumerate(self.narrations["interactions"][pos:]):
-                    self.narrations["interactions"][i]["content"]["voice"] = interaction["content"]["voice"] - 1
+            self.subscripts.append({"sound": f"voice-{uuid.uuid4()}.mp3", 
+                                "subscript":{self.locale: text}, 
+                                "narrator": narrator if narrator!=None else self.narrator,
+                                "alternative": {self.locale: alternativeText}})
+        self.narrations["interactions"].append({
+            "start": "",
+            "duration": "auto",
+            "content": {
+                "popup": 4,
+                "voice": len(self.narrations["subscripts"])-1,
+                "text": {self.locale: text}
+            },
+            "onPoster": 1,
+            "actor": self._getUserId(narrator if narrator!=None else self.narrator),
+            "type": "talk"
+        })
 
     def export(self, voiceOffset=0, pageId=0.0):
         outSubscripts = copy.deepcopy(self.subscripts)
         outInteractions = copy.deepcopy(self.interactions)
         outNarrations = copy.deepcopy(self.narrations)
 
         if self.hasImage:
@@ -1051,24 +766,21 @@
         outSubscripts = outSubscripts + outNarrations["subscripts"]
         narrationOffset = len(outSubscripts)
         for i, interaction in enumerate(outNarrations["interactions"]):
             outNarrations["interactions"][i]["content"]["voice"] += narrationOffset
             outInteractions.append(outNarrations["interactions"][i])
 
         for j, interaction in enumerate(outInteractions):
-            if (
-                "content" in interaction
-                and interaction["content"].get("voice", -1) >= 0
-            ):
+            if "content" in interaction and interaction["content"].get("voice", -1) >= 0:
                 outInteractions[j]["content"]["voice"] += voiceOffset
         return {
             "voices": outSubscripts,
             "events": [
                 {
-                    "id": pageId,
-                    "scene": self.scene,
-                    "board": self.board,
-                    "objects": self.objects,
-                    "interactions": outInteractions,
+                "id": pageId,
+                "scene": self.scene,
+                "board": self.board,
+                "objects": self.objects,
+                "interactions": outInteractions
                 }
-            ],
-        }
+            ]
+        }
```

## storybuilder/storyprofiles.py

```diff
@@ -90,28 +90,34 @@
         '数数': '暑shù',
         '∠': '角',
         '°': '度',
         '<ul>': '',
         '</ul>': '',
         '<li>': '',
         '</li>': '。',
+        '😳': '',
+        '😄': '',
+        '💡': '',
         '·': '-',
         '>': '大于',
         '<': '小于',
         '>=': '大于等于',
         '<=': '小于等于',
         'WHO': 'WH欧',
         'elif': 'L-If',
         'for': 'four',
     },
     "en-US": {
         '<ul>': '',
         '</ul>': '',
         '<li>': '',
         '</li>': '。',
+        '😳': '',
+        '😄': '',
+        '💡': '',
     }
 }
 
 CHARACTER_FIGURE_ACCESSORY_KEYS = ['mask', 'cap']
 
 STORY_SCENARIO_STYLES = {
     "shinkai_makoto": {
@@ -120,52 +126,52 @@
             "classroom": "475dc094-e147-478e-a1cf-770df5efa081",
             "notes": {
                 "scene":"ce3ae229-7e6b-4e10-9d0a-e5e53d923d61",
                 "board":{
                     "content":{
                         "rect": [0.2, 0.2, 0.6, 0.8], 
                         "type": "notes", 
-                        "html":"<h2 style=\'color:white\'><br/><ul>{}</ul></h2>"
+                        "html":"<h2 style='color:white'><br/><ul>{}</ul></h2>"
                     }
                 }
             },
             "exam": "a65ed1dc-9e27-4c3d-a5f7-090fc2af4917",
             "blackboard": {"bgColor": "#98A698"},
             "concentrak": {"index": "0bd6c33e-31eb-4083-8dd8-ee07837bc975", "bgColor": "#C1D0BA"},
         },
         "frame": "10px solid #843C0C",
         "positions": {
             "left": [0.2, 0.05],
             "right": [0.8, 0.05],
-            "right-bottom": [0.85, -0.05],
+            "right_bottom": [0.85, -0.05],
         },
         "popup": 11,
         "scale": 1
     },
     "close_up": {
         "scenarios": {
             "cover": "5cdab8ba-c028-45ea-87cc-b0d75dd81e10",
             "classroom": "b99b0dc2-0387-4a4f-9c61-308b362cb8f6",
             "notes": {
                 "scene": "6c5c45c3-070f-439a-a6f7-a366a04c357c",
                 "board":{
                     "content":{
                         "rect": [0.1, 0.28, 0.7, 0.5], 
                         "type": "notes", 
-                        "html":"<p><ul style=\'color: white\' size='5'>{}</ul></p>"
+                        "html":"<p><ul style='color: white' size='5'>{}</ul></p>"
                     }
                 }
             },
             "exam": "ea874992-c7a9-44c4-8bef-13cad8cee917",
             "blackboard": "e183c517-cbb7-4831-bcf6-efd310ee8790",
             "concentrak": {"index": "0bd6c33e-31eb-4083-8dd8-ee07837bc975", "bgColor": "#9BB9BF"},
         },
         "frame": "10px solid #843C0C",
         "positions": {
             "left": [0.2, -0.25],
             "right": [0.8, -0.25],
-            "right-bottom": [0.8, 0.05],
+            "right_bottom": [0.8, 0.05],
         },
         "popup": 10,
         "scale": 2
     }
 }
```

## storybuilder/storyvoicebuilder.py

```diff
@@ -38,15 +38,15 @@
 
         character = character if character != '' else 'M'
         synthesizer.set_voice(
             language,
             CHARACTER_VOICE_PROFILES[character][language]['voiceName'],
             **CHARACTER_VOICE_PROFILES[character][language]['kwargs'])
 
-        if fileName == None or len(fileName) < 1:
+        if fileName == None:
             fileName = self._newAudioFileName(language)
             print(f'No input file_name, generate new file name as: {fileName}')
         elif language.lower() not in ('cn', 'zh-cn'):
             fileName = self._fixAudioFileName(fileName, language)
             print(f'Adjust file_name with language code as: {fileName}')
 
         print('Original:', text)
```

## Comparing `storybuilder-0.0.34.dist-info/LICENSE` & `storybuilder-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `storybuilder-0.0.34.dist-info/METADATA` & `storybuilder-0.0.9.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 Metadata-Version: 2.1
 Name: storybuilder
-Version: 0.0.34
+Version: 0.0.9
 Summary: A Python toolkit to build story meta.
 Author-email: Kelvin Xu <xxk59@hotmail.com>
 Project-URL: Homepage, https://github.com/xxk59/StoryBuilder
 Project-URL: Issues, https://github.com/xxk59/StoryBuilder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow
-Requires-Dist: azure-cognitiveservices-speech
-Requires-Dist: cos-python-sdk-v5
-Requires-Dist: pydub
-Requires-Dist: pyperclip
-Requires-Dist: ffmpeg
 
 # StoryBuilder
 
 Toolkit to build a story meta
 
 # Pre-requisites
```

