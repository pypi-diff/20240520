# Comparing `tmp/noveler-0.1.2.tar.gz` & `tmp/noveler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noveler-0.1.2.tar", max compression
+gzip compressed data, was "noveler-0.1.3.tar", max compression
```

## Comparing `noveler-0.1.2.tar` & `noveler-0.1.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2024-04-05 16:46:40.584169 noveler-0.1.2/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-05 23:46:41.029817 noveler-0.1.2/README.md
--rw-r--r--   0        0        0       72 2024-03-27 02:28:45.063002 noveler-0.1.2/noveler/__init__.py
--rw-r--r--   0        0        0     7397 2024-05-16 16:29:47.881622 noveler-0.1.2/noveler/application.py
--rw-r--r--   0        0        0     5138 2024-04-26 23:37:57.167329 noveler-0.1.2/noveler/controllers/ActivityController.py
--rw-r--r--   0        0        0    26678 2024-04-26 23:26:37.587556 noveler-0.1.2/noveler/controllers/AssistantController.py
--rw-r--r--   0        0        0    11098 2024-04-26 23:42:46.902640 noveler-0.1.2/noveler/controllers/AuthorController.py
--rw-r--r--   0        0        0      984 2024-04-29 20:02:53.981822 noveler-0.1.2/noveler/controllers/BaseController.py
--rw-r--r--   0        0        0    13579 2024-04-29 20:07:01.963452 noveler-0.1.2/noveler/controllers/BibliographyController.py
--rw-r--r--   0        0        0    25404 2024-04-29 23:40:17.360757 noveler-0.1.2/noveler/controllers/ChapterController.py
--rw-r--r--   0        0        0    75357 2024-04-30 18:57:39.408452 noveler-0.1.2/noveler/controllers/CharacterController.py
--rw-r--r--   0        0        0    17439 2024-05-17 18:13:22.445990 noveler-0.1.2/noveler/controllers/EventController.py
--rw-r--r--   0        0        0    16728 2024-04-30 18:44:07.987106 noveler-0.1.2/noveler/controllers/ExportController.py
--rw-r--r--   0        0        0    10472 2024-04-29 22:15:45.985866 noveler-0.1.2/noveler/controllers/ImageController.py
--rw-r--r--   0        0        0     7221 2024-04-29 23:00:47.199253 noveler-0.1.2/noveler/controllers/LinkController.py
--rw-r--r--   0        0        0    23864 2024-04-29 23:07:38.798422 noveler-0.1.2/noveler/controllers/LocationController.py
--rw-r--r--   0        0        0     6655 2024-04-29 23:14:13.518805 noveler-0.1.2/noveler/controllers/NoteController.py
--rw-r--r--   0        0        0     2865 2024-04-29 23:14:38.879658 noveler-0.1.2/noveler/controllers/OllamaModelController.py
--rw-r--r--   0        0        0    21926 2024-04-29 23:22:47.753481 noveler-0.1.2/noveler/controllers/SceneController.py
--rw-r--r--   0        0        0    23049 2024-04-29 23:29:10.431386 noveler-0.1.2/noveler/controllers/StoryController.py
--rw-r--r--   0        0        0     9149 2024-04-29 23:31:13.876182 noveler-0.1.2/noveler/controllers/SubmissionController.py
--rw-r--r--   0        0        0    17444 2024-04-29 23:31:13.774179 noveler-0.1.2/noveler/controllers/UserController.py
--rw-r--r--   0        0        0     1221 2024-03-30 00:37:25.669229 noveler-0.1.2/noveler/controllers/__init__.py
--rw-r--r--   0        0        0     3374 2024-04-18 17:39:28.714791 noveler-0.1.2/noveler/models/Activity.py
--rw-r--r--   0        0        0     6358 2024-05-03 01:08:29.388098 noveler-0.1.2/noveler/models/Assistance.py
--rw-r--r--   0        0        0     4790 2024-03-26 17:54:58.737034 noveler-0.1.2/noveler/models/Author.py
--rw-r--r--   0        0        0     3316 2024-05-05 19:32:49.704937 noveler-0.1.2/noveler/models/AuthorStory.py
--rw-r--r--   0        0        0       70 2024-03-24 02:35:40.239112 noveler-0.1.2/noveler/models/Base.py
--rw-r--r--   0        0        0     7430 2024-05-05 18:44:03.133809 noveler-0.1.2/noveler/models/Bibliography.py
--rw-r--r--   0        0        0     4817 2024-05-05 19:15:35.689588 noveler-0.1.2/noveler/models/BibliographyAuthor.py
--rw-r--r--   0        0        0     6709 2024-03-30 20:19:56.562647 noveler-0.1.2/noveler/models/Chapter.py
--rw-r--r--   0        0        0     3799 2024-03-30 15:06:41.382174 noveler-0.1.2/noveler/models/ChapterLink.py
--rw-r--r--   0        0        0     3798 2024-03-30 15:06:11.516345 noveler-0.1.2/noveler/models/ChapterNote.py
--rw-r--r--   0        0        0    27269 2024-05-15 04:11:34.202461 noveler-0.1.2/noveler/models/Character.py
--rw-r--r--   0        0        0     3594 2024-04-03 17:49:52.714571 noveler-0.1.2/noveler/models/CharacterEvent.py
--rw-r--r--   0        0        0     4529 2024-04-03 04:05:10.789780 noveler-0.1.2/noveler/models/CharacterImage.py
--rw-r--r--   0        0        0     3483 2024-04-03 04:06:41.377737 noveler-0.1.2/noveler/models/CharacterLink.py
--rw-r--r--   0        0        0     3609 2024-04-03 04:05:52.527628 noveler-0.1.2/noveler/models/CharacterNote.py
--rw-r--r--   0        0        0     7615 2024-04-03 16:14:05.483259 noveler-0.1.2/noveler/models/CharacterRelationship.py
--rw-r--r--   0        0        0      649 2024-03-23 23:08:42.545496 noveler-0.1.2/noveler/models/CharacterRelationshipTypes.py
--rw-r--r--   0        0        0     3589 2024-04-03 17:54:57.531181 noveler-0.1.2/noveler/models/CharacterStory.py
--rw-r--r--   0        0        0     5186 2024-03-26 17:58:57.654914 noveler-0.1.2/noveler/models/CharacterTrait.py
--rw-r--r--   0        0        0     5923 2024-05-17 18:15:18.785448 noveler-0.1.2/noveler/models/Event.py
--rw-r--r--   0        0        0     3366 2024-03-26 17:59:36.066040 noveler-0.1.2/noveler/models/EventLink.py
--rw-r--r--   0        0        0     3353 2024-03-26 18:00:15.887213 noveler-0.1.2/noveler/models/EventNote.py
--rw-r--r--   0        0        0     7577 2024-05-15 17:34:54.008689 noveler-0.1.2/noveler/models/Image.py
--rw-r--r--   0        0        0     4309 2024-03-26 18:00:46.640121 noveler-0.1.2/noveler/models/ImageLocation.py
--rw-r--r--   0        0        0      403 2024-03-24 00:00:16.388632 noveler-0.1.2/noveler/models/ImageMimeTypes.py
--rw-r--r--   0        0        0     6190 2024-05-15 17:41:06.577136 noveler-0.1.2/noveler/models/Link.py
--rw-r--r--   0        0        0     3414 2024-03-24 02:51:56.610270 noveler-0.1.2/noveler/models/LinkLocation.py
--rw-r--r--   0        0        0     3366 2024-03-30 14:28:11.555374 noveler-0.1.2/noveler/models/LinkScene.py
--rw-r--r--   0        0        0     3397 2024-03-30 15:15:20.441603 noveler-0.1.2/noveler/models/LinkStory.py
--rw-r--r--   0        0        0    10829 2024-05-17 18:15:41.119110 noveler-0.1.2/noveler/models/Location.py
--rw-r--r--   0        0        0     3311 2024-03-24 02:53:02.016031 noveler-0.1.2/noveler/models/LocationNote.py
--rw-r--r--   0        0        0     6026 2024-05-15 18:39:18.266390 noveler-0.1.2/noveler/models/Note.py
--rw-r--r--   0        0        0     3366 2024-03-30 14:29:01.876861 noveler-0.1.2/noveler/models/NoteScene.py
--rw-r--r--   0        0        0     3397 2024-03-30 15:16:00.109707 noveler-0.1.2/noveler/models/NoteStory.py
--rw-r--r--   0        0        0     5644 2024-05-15 18:41:45.146555 noveler-0.1.2/noveler/models/OllamaModel.py
--rw-r--r--   0        0        0     7206 2024-05-15 18:42:51.323681 noveler-0.1.2/noveler/models/Scene.py
--rw-r--r--   0        0        0     7248 2024-05-15 18:44:18.920291 noveler-0.1.2/noveler/models/Story.py
--rw-r--r--   0        0        0     9722 2024-05-15 18:45:30.881700 noveler-0.1.2/noveler/models/Submission.py
--rw-r--r--   0        0        0      768 2024-05-15 18:46:35.155017 noveler-0.1.2/noveler/models/SubmissionResultType.py
--rw-r--r--   0        0        0     9026 2024-05-15 18:47:38.667364 noveler-0.1.2/noveler/models/User.py
--rw-r--r--   0        0        0     2004 2024-05-17 18:14:04.813251 noveler-0.1.2/noveler/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 19:38:44.012362 noveler-0.1.2/noveler/tmp/empty
--rw-r--r--   0        0        0      781 2024-05-17 18:17:19.063008 noveler-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 noveler-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-05 16:46:40.584169 noveler-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-05 23:46:41.029817 noveler-0.1.3/README.md
+-rw-r--r--   0        0        0       72 2024-03-27 02:28:45.063002 noveler-0.1.3/noveler/__init__.py
+-rw-r--r--   0        0        0     7397 2024-05-16 16:29:47.881622 noveler-0.1.3/noveler/application.py
+-rw-r--r--   0        0        0     5138 2024-04-26 23:37:57.167329 noveler-0.1.3/noveler/controllers/ActivityController.py
+-rw-r--r--   0        0        0    26678 2024-04-26 23:26:37.587556 noveler-0.1.3/noveler/controllers/AssistantController.py
+-rw-r--r--   0        0        0    11098 2024-04-26 23:42:46.902640 noveler-0.1.3/noveler/controllers/AuthorController.py
+-rw-r--r--   0        0        0      984 2024-04-29 20:02:53.981822 noveler-0.1.3/noveler/controllers/BaseController.py
+-rw-r--r--   0        0        0    13579 2024-04-29 20:07:01.963452 noveler-0.1.3/noveler/controllers/BibliographyController.py
+-rw-r--r--   0        0        0    25404 2024-04-29 23:40:17.360757 noveler-0.1.3/noveler/controllers/ChapterController.py
+-rw-r--r--   0        0        0    75357 2024-04-30 18:57:39.408452 noveler-0.1.3/noveler/controllers/CharacterController.py
+-rw-r--r--   0        0        0    17439 2024-05-17 18:13:22.445990 noveler-0.1.3/noveler/controllers/EventController.py
+-rw-r--r--   0        0        0    16728 2024-04-30 18:44:07.987106 noveler-0.1.3/noveler/controllers/ExportController.py
+-rw-r--r--   0        0        0    10472 2024-04-29 22:15:45.985866 noveler-0.1.3/noveler/controllers/ImageController.py
+-rw-r--r--   0        0        0     7221 2024-04-29 23:00:47.199253 noveler-0.1.3/noveler/controllers/LinkController.py
+-rw-r--r--   0        0        0    23864 2024-04-29 23:07:38.798422 noveler-0.1.3/noveler/controllers/LocationController.py
+-rw-r--r--   0        0        0     6655 2024-04-29 23:14:13.518805 noveler-0.1.3/noveler/controllers/NoteController.py
+-rw-r--r--   0        0        0     2865 2024-04-29 23:14:38.879658 noveler-0.1.3/noveler/controllers/OllamaModelController.py
+-rw-r--r--   0        0        0    21926 2024-04-29 23:22:47.753481 noveler-0.1.3/noveler/controllers/SceneController.py
+-rw-r--r--   0        0        0    23049 2024-04-29 23:29:10.431386 noveler-0.1.3/noveler/controllers/StoryController.py
+-rw-r--r--   0        0        0     9149 2024-04-29 23:31:13.876182 noveler-0.1.3/noveler/controllers/SubmissionController.py
+-rw-r--r--   0        0        0    17444 2024-04-29 23:31:13.774179 noveler-0.1.3/noveler/controllers/UserController.py
+-rw-r--r--   0        0        0     1221 2024-03-30 00:37:25.669229 noveler-0.1.3/noveler/controllers/__init__.py
+-rw-r--r--   0        0        0     3374 2024-04-18 17:39:28.714791 noveler-0.1.3/noveler/models/Activity.py
+-rw-r--r--   0        0        0     6358 2024-05-03 01:08:29.388098 noveler-0.1.3/noveler/models/Assistance.py
+-rw-r--r--   0        0        0     4790 2024-03-26 17:54:58.737034 noveler-0.1.3/noveler/models/Author.py
+-rw-r--r--   0        0        0     3316 2024-05-05 19:32:49.704937 noveler-0.1.3/noveler/models/AuthorStory.py
+-rw-r--r--   0        0        0       70 2024-03-24 02:35:40.239112 noveler-0.1.3/noveler/models/Base.py
+-rw-r--r--   0        0        0     7430 2024-05-05 18:44:03.133809 noveler-0.1.3/noveler/models/Bibliography.py
+-rw-r--r--   0        0        0     4817 2024-05-05 19:15:35.689588 noveler-0.1.3/noveler/models/BibliographyAuthor.py
+-rw-r--r--   0        0        0     6709 2024-03-30 20:19:56.562647 noveler-0.1.3/noveler/models/Chapter.py
+-rw-r--r--   0        0        0     3799 2024-03-30 15:06:41.382174 noveler-0.1.3/noveler/models/ChapterLink.py
+-rw-r--r--   0        0        0     3798 2024-03-30 15:06:11.516345 noveler-0.1.3/noveler/models/ChapterNote.py
+-rw-r--r--   0        0        0    27253 2024-05-20 20:51:47.613321 noveler-0.1.3/noveler/models/Character.py
+-rw-r--r--   0        0        0     3594 2024-04-03 17:49:52.714571 noveler-0.1.3/noveler/models/CharacterEvent.py
+-rw-r--r--   0        0        0     4529 2024-04-03 04:05:10.789780 noveler-0.1.3/noveler/models/CharacterImage.py
+-rw-r--r--   0        0        0     3483 2024-04-03 04:06:41.377737 noveler-0.1.3/noveler/models/CharacterLink.py
+-rw-r--r--   0        0        0     3609 2024-04-03 04:05:52.527628 noveler-0.1.3/noveler/models/CharacterNote.py
+-rw-r--r--   0        0        0     7615 2024-04-03 16:14:05.483259 noveler-0.1.3/noveler/models/CharacterRelationship.py
+-rw-r--r--   0        0        0      649 2024-03-23 23:08:42.545496 noveler-0.1.3/noveler/models/CharacterRelationshipTypes.py
+-rw-r--r--   0        0        0     3589 2024-04-03 17:54:57.531181 noveler-0.1.3/noveler/models/CharacterStory.py
+-rw-r--r--   0        0        0     5186 2024-03-26 17:58:57.654914 noveler-0.1.3/noveler/models/CharacterTrait.py
+-rw-r--r--   0        0        0     5923 2024-05-17 18:15:18.785448 noveler-0.1.3/noveler/models/Event.py
+-rw-r--r--   0        0        0     3366 2024-03-26 17:59:36.066040 noveler-0.1.3/noveler/models/EventLink.py
+-rw-r--r--   0        0        0     3353 2024-03-26 18:00:15.887213 noveler-0.1.3/noveler/models/EventNote.py
+-rw-r--r--   0        0        0     7577 2024-05-15 17:34:54.008689 noveler-0.1.3/noveler/models/Image.py
+-rw-r--r--   0        0        0     4309 2024-03-26 18:00:46.640121 noveler-0.1.3/noveler/models/ImageLocation.py
+-rw-r--r--   0        0        0      403 2024-03-24 00:00:16.388632 noveler-0.1.3/noveler/models/ImageMimeTypes.py
+-rw-r--r--   0        0        0     6190 2024-05-15 17:41:06.577136 noveler-0.1.3/noveler/models/Link.py
+-rw-r--r--   0        0        0     3414 2024-03-24 02:51:56.610270 noveler-0.1.3/noveler/models/LinkLocation.py
+-rw-r--r--   0        0        0     3366 2024-03-30 14:28:11.555374 noveler-0.1.3/noveler/models/LinkScene.py
+-rw-r--r--   0        0        0     3397 2024-03-30 15:15:20.441603 noveler-0.1.3/noveler/models/LinkStory.py
+-rw-r--r--   0        0        0    10829 2024-05-17 18:15:41.119110 noveler-0.1.3/noveler/models/Location.py
+-rw-r--r--   0        0        0     3311 2024-03-24 02:53:02.016031 noveler-0.1.3/noveler/models/LocationNote.py
+-rw-r--r--   0        0        0     6026 2024-05-15 18:39:18.266390 noveler-0.1.3/noveler/models/Note.py
+-rw-r--r--   0        0        0     3366 2024-03-30 14:29:01.876861 noveler-0.1.3/noveler/models/NoteScene.py
+-rw-r--r--   0        0        0     3397 2024-03-30 15:16:00.109707 noveler-0.1.3/noveler/models/NoteStory.py
+-rw-r--r--   0        0        0     5644 2024-05-15 18:41:45.146555 noveler-0.1.3/noveler/models/OllamaModel.py
+-rw-r--r--   0        0        0     7206 2024-05-15 18:42:51.323681 noveler-0.1.3/noveler/models/Scene.py
+-rw-r--r--   0        0        0     7248 2024-05-15 18:44:18.920291 noveler-0.1.3/noveler/models/Story.py
+-rw-r--r--   0        0        0     9722 2024-05-15 18:45:30.881700 noveler-0.1.3/noveler/models/Submission.py
+-rw-r--r--   0        0        0      768 2024-05-15 18:46:35.155017 noveler-0.1.3/noveler/models/SubmissionResultType.py
+-rw-r--r--   0        0        0     9026 2024-05-15 18:47:38.667364 noveler-0.1.3/noveler/models/User.py
+-rw-r--r--   0        0        0     2004 2024-05-17 18:14:04.813251 noveler-0.1.3/noveler/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:38:44.012362 noveler-0.1.3/noveler/tmp/empty
+-rw-r--r--   0        0        0      781 2024-05-20 20:59:03.005103 noveler-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 noveler-0.1.3/PKG-INFO
```

### Comparing `noveler-0.1.2/LICENSE` & `noveler-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/README.md` & `noveler-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/application.py` & `noveler-0.1.3/noveler/application.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/ActivityController.py` & `noveler-0.1.3/noveler/controllers/ActivityController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/AssistantController.py` & `noveler-0.1.3/noveler/controllers/AssistantController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/AuthorController.py` & `noveler-0.1.3/noveler/controllers/AuthorController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/BaseController.py` & `noveler-0.1.3/noveler/controllers/BaseController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/BibliographyController.py` & `noveler-0.1.3/noveler/controllers/BibliographyController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/ChapterController.py` & `noveler-0.1.3/noveler/controllers/ChapterController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/CharacterController.py` & `noveler-0.1.3/noveler/controllers/CharacterController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/EventController.py` & `noveler-0.1.3/noveler/controllers/EventController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/ExportController.py` & `noveler-0.1.3/noveler/controllers/ExportController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/ImageController.py` & `noveler-0.1.3/noveler/controllers/ImageController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/LinkController.py` & `noveler-0.1.3/noveler/controllers/LinkController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/LocationController.py` & `noveler-0.1.3/noveler/controllers/LocationController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/NoteController.py` & `noveler-0.1.3/noveler/controllers/NoteController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/OllamaModelController.py` & `noveler-0.1.3/noveler/controllers/OllamaModelController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/SceneController.py` & `noveler-0.1.3/noveler/controllers/SceneController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/StoryController.py` & `noveler-0.1.3/noveler/controllers/StoryController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/SubmissionController.py` & `noveler-0.1.3/noveler/controllers/SubmissionController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/UserController.py` & `noveler-0.1.3/noveler/controllers/UserController.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/controllers/__init__.py` & `noveler-0.1.3/noveler/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Activity.py` & `noveler-0.1.3/noveler/models/Activity.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Assistance.py` & `noveler-0.1.3/noveler/models/Assistance.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Author.py` & `noveler-0.1.3/noveler/models/Author.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/AuthorStory.py` & `noveler-0.1.3/noveler/models/AuthorStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Bibliography.py` & `noveler-0.1.3/noveler/models/Bibliography.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/BibliographyAuthor.py` & `noveler-0.1.3/noveler/models/BibliographyAuthor.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Chapter.py` & `noveler-0.1.3/noveler/models/Chapter.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/ChapterLink.py` & `noveler-0.1.3/noveler/models/ChapterLink.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/ChapterNote.py` & `noveler-0.1.3/noveler/models/ChapterNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Character.py` & `noveler-0.1.3/noveler/models/Character.py`

 * *Files 1% similar despite different names*

```diff
@@ -683,15 +683,15 @@
         -------
         str
             The validated date of birth
         """
 
         config = ConfigParser()
         config.read("config.cfg")
-        date_format = config.get("datetime", "date_format")
+        date_format = config.get("formats", "date")
 
         if date_of_birth and bool(datetime.strptime(date_of_birth, date_format)) is False:
             raise ValueError("The date of birth must be in the format 'YYYY-MM-DD'.")
 
         if date_of_birth:
             return datetime.strptime(date_of_birth, date_format)
 
@@ -711,15 +711,15 @@
         -------
         str
             The validated date of death
         """
 
         config = ConfigParser()
         config.read("config.cfg")
-        date_format = config.get("datetime", "date_format")
+        date_format = config.get("formats", "date")
 
         if date_of_death and bool(datetime.strptime(date_of_death, date_format)) is False:
             raise ValueError("The date of death must be in the format 'YYYY-MM-DD'.")
 
         if date_of_death:
             return datetime.strptime(date_of_death, date_format)
```

### Comparing `noveler-0.1.2/noveler/models/CharacterEvent.py` & `noveler-0.1.3/noveler/models/CharacterEvent.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/CharacterImage.py` & `noveler-0.1.3/noveler/models/CharacterImage.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/CharacterLink.py` & `noveler-0.1.3/noveler/models/CharacterLink.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/CharacterNote.py` & `noveler-0.1.3/noveler/models/CharacterNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/CharacterRelationship.py` & `noveler-0.1.3/noveler/models/CharacterRelationship.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/CharacterRelationshipTypes.py` & `noveler-0.1.3/noveler/models/CharacterRelationshipTypes.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/CharacterStory.py` & `noveler-0.1.3/noveler/models/CharacterStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/CharacterTrait.py` & `noveler-0.1.3/noveler/models/CharacterTrait.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Event.py` & `noveler-0.1.3/noveler/models/Event.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/EventLink.py` & `noveler-0.1.3/noveler/models/EventLink.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/EventNote.py` & `noveler-0.1.3/noveler/models/EventNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Image.py` & `noveler-0.1.3/noveler/models/Image.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/ImageLocation.py` & `noveler-0.1.3/noveler/models/ImageLocation.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Link.py` & `noveler-0.1.3/noveler/models/Link.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/LinkLocation.py` & `noveler-0.1.3/noveler/models/LinkLocation.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/LinkScene.py` & `noveler-0.1.3/noveler/models/LinkScene.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/LinkStory.py` & `noveler-0.1.3/noveler/models/LinkStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Location.py` & `noveler-0.1.3/noveler/models/Location.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/LocationNote.py` & `noveler-0.1.3/noveler/models/LocationNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Note.py` & `noveler-0.1.3/noveler/models/Note.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/NoteScene.py` & `noveler-0.1.3/noveler/models/NoteScene.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/NoteStory.py` & `noveler-0.1.3/noveler/models/NoteStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/OllamaModel.py` & `noveler-0.1.3/noveler/models/OllamaModel.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Scene.py` & `noveler-0.1.3/noveler/models/Scene.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Story.py` & `noveler-0.1.3/noveler/models/Story.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/Submission.py` & `noveler-0.1.3/noveler/models/Submission.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/SubmissionResultType.py` & `noveler-0.1.3/noveler/models/SubmissionResultType.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/User.py` & `noveler-0.1.3/noveler/models/User.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/noveler/models/__init__.py` & `noveler-0.1.3/noveler/models/__init__.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.2/pyproject.toml` & `noveler-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "noveler"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Richard Lucas <webmaster@applebiter.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "noveler"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Richard Lucas", email="webmaster@applebiter.com" },
 ]
 description = "Novel, short story, and serial authoring software"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `noveler-0.1.2/PKG-INFO` & `noveler-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noveler
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Richard Lucas
 Author-email: webmaster@applebiter.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

