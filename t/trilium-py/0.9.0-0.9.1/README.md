# Comparing `tmp/trilium_py-0.9.0-py3-none-any.whl.zip` & `tmp/trilium_py-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 34432 bytes, number of entries: 14
+Zip file size: 35664 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      141 b- defN 24-Apr-22 06:33 trilium_py/__init__.py
--rw-r--r--  2.0 unx    45427 b- defN 24-May-20 07:05 trilium_py/client.py
+-rw-r--r--  2.0 unx    47014 b- defN 24-May-20 08:30 trilium_py/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 07:17 trilium_py/utils/__init__.py
 -rw-r--r--  2.0 unx     2290 b- defN 24-Apr-22 06:32 trilium_py/utils/html_util.py
+-rw-r--r--  2.0 unx     1083 b- defN 24-May-20 08:28 trilium_py/utils/image_util.py
 -rw-r--r--  2.0 unx     9328 b- defN 24-Apr-22 06:33 trilium_py/utils/markdown_math.py
 -rw-r--r--  2.0 unx     3909 b- defN 24-Apr-22 06:33 trilium_py/utils/note_util.py
 -rw-r--r--  2.0 unx      681 b- defN 24-Apr-22 06:33 trilium_py/utils/param_util.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-22 06:33 trilium_py/utils/time_util.py
 -rw-r--r--  2.0 unx      486 b- defN 24-Apr-22 06:33 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    15968 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1162 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/RECORD
-14 files, 114887 bytes uncompressed, 32494 bytes compressed:  71.7%
+-rwxrwx---  2.0 unx    35184 b- defN 24-May-20 08:38 trilium_py-0.9.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    16604 b- defN 24-May-20 08:38 trilium_py-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 08:38 trilium_py-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-20 08:38 trilium_py-0.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1249 b- defN 24-May-20 08:38 trilium_py-0.9.1.dist-info/RECORD
+15 files, 118280 bytes uncompressed, 33590 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: trilium_py/utils/__init__.py
 Comment: 
 
 Filename: trilium_py/utils/html_util.py
 Comment: 
 
+Filename: trilium_py/utils/image_util.py
+Comment: 
+
 Filename: trilium_py/utils/markdown_math.py
 Comment: 
 
 Filename: trilium_py/utils/note_util.py
 Comment: 
 
 Filename: trilium_py/utils/param_util.py
@@ -21,23 +24,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.9.0.dist-info/LICENSE.txt
+Filename: trilium_py-0.9.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.9.0.dist-info/METADATA
+Filename: trilium_py-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.9.0.dist-info/WHEEL
+Filename: trilium_py-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.9.0.dist-info/top_level.txt
+Filename: trilium_py-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.9.0.dist-info/RECORD
+Filename: trilium_py-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -13,14 +13,15 @@
 from loguru import logger
 from natsort import natsort
 
 from .utils.markdown_math import reconstructMath, sanitizeInput
 from .utils.note_util import beautify_content, sort_note_by_headings
 from .utils.param_util import clean_param, format_query_string
 from .utils.time_util import get_today, get_yesterday
+from .utils.image_util import compress_image_bytes, get_extension_from_image_mime
 
 
 class ETAPI:
     def __init__(self, server_url: str, token: Optional[str] = None):
         if sys.version_info < (3, 9):
             print(
                 (
@@ -1130,15 +1131,15 @@
         :return:
         """
         url = f"{self.server_url}/etapi/sync/now"
         res = requests.post(url, headers=self.get_header())
         if res.status_code == 200:
             logger.info("sync successfully")
 
-    def get_attachmants(self, noteId: str):
+    def get_attachments(self, noteId: str):
         """
         get attachment list of a note
         :param noteId:
         :return:
         """
         url = f'{self.server_url}/etapi/notes/{noteId}/attachments'
 
@@ -1247,18 +1248,23 @@
         return res.json()
 
     def get_attachment_content(self, attachmentId: str) -> bytes:
         url = f'{self.server_url}/etapi/attachments/{attachmentId}/content'
         res = requests.get(url, headers=self.get_header())
         return res.content
 
-    def update_attachment_content(self, attachmentId: str, file_path: str) -> bool:
+    def update_attachment_content(
+        self, attachmentId: str, data_source: str, is_file: bool = True
+    ) -> bool:
         # upload file, set content
         url = f'{self.server_url}/etapi/attachments/{attachmentId}/content'
-        file_data = open(file_path, 'rb').read()
+        if is_file:
+            file_data = open(data_source, 'rb').read()
+        else:
+            file_data = data_source
         res = requests.put(
             url,
             data=file_data,
             headers={
                 'content-type': 'application/octet-stream',
                 'Content-Transfer-Encoding': 'binary',
                 'Authorization': self.token,
@@ -1271,14 +1277,47 @@
     def delete_attachment(self, attachmentId: str) -> bool:
         url = f'{self.server_url}/etapi/attachments/{attachmentId}'
         res = requests.delete(url, headers=self.get_header())
         if res.status_code == 204:
             return True
         return False
 
+    def optimize_image_attachments(self, noteId: str):
+        """
+        comporess image attachments
+        :param noteId:
+        :return:
+        """
+
+        attachments = self.get_attachments(noteId)
+        for attachment in attachments:
+            try:
+                logger.info(attachment)
+                if not attachment['role'] == 'image' and attachment['contentLength'] > 0:
+                    continue
+                image_data = self.get_attachment_content(attachment['attachmentId'])
+                extension = get_extension_from_image_mime(attachment['mime'])
+                if extension == 'jpg':
+                    # jpg can not be processed yet
+                    continue
+                compressed_data = compress_image_bytes(image_data, extension)
+                size_before = len(image_data)
+                size_after = len(compressed_data)
+                logger.info(f"Size before compression: {size_before} bytes")
+                logger.info(f"Size after compression: {size_after} bytes")
+                if size_after < size_before:
+                    logger.info('replace image')
+                    self.update_attachment_content(
+                        attachment['attachmentId'], compressed_data, is_file=False
+                    )
+                else:
+                    logger.info('skip image')
+            except:
+                pass
+
     def sort_note_content(self, noteId: str, locale_str: str = 'zh_CN.UTF-8'):
         """
         Sort note content by headings
         You can set locale to sort with respect to your local language.
 
         :param noteId:
         :param locale_str:  should be something like 'zh_CN.UTF-8'
```

## Comparing `trilium_py-0.9.0.dist-info/LICENSE.txt` & `trilium_py-0.9.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.9.0.dist-info/METADATA` & `trilium_py-0.9.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
@@ -14,24 +14,26 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: BeautifulSoup4
 Requires-Dist: requests
 Requires-Dist: markdown2[all]
 Requires-Dist: natsort
 Requires-Dist: loguru
 Requires-Dist: minify-html
+Requires-Dist: pillow
 Requires-Dist: python-magic-bin ; platform_system == "Windows"
 Requires-Dist: python-magic ; sys_platform == "darwin"
 Requires-Dist: python-magic ; sys_platform == "linux"
 
 # 🐍 trilium-py
 
 <p align="center">
@@ -59,16 +61,19 @@
       * [🏭 Create Note](#-create-note)
          * [🖼️ Create Image note](#️-create-image-note)
       * [👀 Get note](#-get-note)
       * [🔄 Update note](#-update-note)
       * [🗑️ Delete note](#️-delete-note)
       * [📅 Day note](#-day-note)
       * [📤 Export note](#-export-note)
+      * [📥 import note](#-import-note)
+      * [💾 Save revision](#-save-revision)
       * [💾 Create data backup](#-create-data-backup)
       * [🏷 Create attribute](#-create-attribute)
+      * [Get attachment list](#get-attachment-list)
       * [Get attachment info](#get-attachment-info)
       * [Update attachment info](#update-attachment-info)
       * [Get attachment content](#get-attachment-content)
       * [Update attachment content](#update-attachment-content)
       * [Create attachment](#create-attachment)
    * [(Advanced Usage) ✅ TODO List](#advanced-usage--todo-list)
       * [Add TODO item](#add-todo-item)
@@ -87,14 +92,15 @@
          * [Import from Turtl](#import-from-turtl)
          * [Import from other markdown software](#import-from-other-markdown-software)
    * [(Advanced Usage) 🎨 Beautify notes](#advanced-usage--beautify-notes)
       * [Beautify a note](#beautify-a-note)
       * [Beautify a note and its child notes](#beautify-a-note-and-its-child-notes)
    * [(Advanced Usage) 🧹 Sort note content](#advanced-usage--sort-note-content)
    * [(Advanced Usage) 🧹 Delete empty new note](#advanced-usage--delete-empty-new-note)
+   * [(Advanced Usage) 🗜️ Optimize image size](#advanced-usage-️-optimize-image-size)
    * [🛠️ Develop](#️-develop)
    * [🔗 Original OpenAPI Documentation](#-original-openapi-documentation)
 <!--te-->
 
 ## 🔧 Installation
 
 ```bash
@@ -323,15 +329,15 @@
 ```
 
 ### Get attachment list
 
 Get all attachments of a single note.
 
 ```
-res = ea.get_attachmants('uMJt0Ajr1CuC')
+res = ea.get_attachments('uMJt0Ajr1CuC')
 ```
 
 ### Get attachment info
 
 Get image title and etc.
 
 ```python
@@ -578,14 +584,23 @@
 workspace, scattered across various locations. I made this bulk deletion of these empty "new notes." Additionally, it
 generates warning messages for "new notes" that contain content, maybe we should change the title for those notes.
 
 ```python
 ea.delete_empty_note()
 ```
 
+## (Advanced Usage) 🗜️ Optimize image size
+
+Try to reduce image size by using PIL's optimize feature. If the image in your note is not compressed, you can try this.
+I've successfully convert a note of 44MB to 9.9MB after this process. Backup your data before try this.
+
+```
+ea.optimize_image_attachments('uMJt0Ajr1CuC')
+```
+
 ## 🛠️ Develop
 
 Install with pip egg link to make package change without reinstall.
 
 ```python
 python -m pip install --user -e .
 ```
```

### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.9.0 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.9.1 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
 OSI Approved :: GNU Affero General Public License v3 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
-Only Requires-Python: >=3.9, <4 Description-Content-Type: text/markdown
-License-File: LICENSE.txt Requires-Dist: BeautifulSoup4 Requires-Dist: requests
-Requires-Dist: markdown2[all] Requires-Dist: natsort Requires-Dist: loguru
-Requires-Dist: minify-html Requires-Dist: python-magic-bin ; platform_system ==
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only Requires-Python: >=3.9,
+<4 Description-Content-Type: text/markdown License-File: LICENSE.txt Requires-
+Dist: BeautifulSoup4 Requires-Dist: requests Requires-Dist: markdown2[all]
+Requires-Dist: natsort Requires-Dist: loguru Requires-Dist: minify-html
+Requires-Dist: pillow Requires-Dist: python-magic-bin ; platform_system ==
 "Windows" Requires-Dist: python-magic ; sys_platform == "darwin" Requires-Dist:
 python-magic ; sys_platform == "linux" # ð trilium-py
                             English | _ç_®__ä_½__ä_¸_­_æ__
 Python client for ETAPI of Trilium Note. [![Downloads](https://
 static.pepy.tech/badge/trilium-py)](https://pepy.tech/project/trilium-py) [!
 [Supported Versions](https://img.shields.io/pypi/pyversions/trilium-py.svg)]
 (https://pypi.org/project/trilium-py) [![Supported Versions](https://
@@ -30,53 +31,56 @@
 trilium-py](#-trilium-py) * [ð¦® Table of Contents](#-table-of-contents) *
 [ð§ Installation](#-installation) * [ð (Basic) Usage](#-basic-usage) *
 [ð Initialization](#-initialization) * [ð Application Information](#-
 application-information) * [ð Search note](#-search-note) * [ð­ Create
 Note](#-create-note) * [ð¼ï¸ Create Image note](#ï¸-create-image-note) *
 [ð Get note](#-get-note) * [ð Update note](#-update-note) * [ðï¸
 Delete note](#ï¸-delete-note) * [ð Day note](#-day-note) * [ð¤ Export
-note](#-export-note) * [ð¾ Create data backup](#-create-data-backup) * [ð·
-Create attribute](#-create-attribute) * [Get attachment info](#get-attachment-
-info) * [Update attachment info](#update-attachment-info) * [Get attachment
-content](#get-attachment-content) * [Update attachment content](#update-
-attachment-content) * [Create attachment](#create-attachment) * [(Advanced
-Usage) â TODO List](#advanced-usage--todo-list) * [Add TODO item](#add-todo-
-item) * [Check/Uncheck a TODO item](#checkuncheck-a-todo-item) * [Update a TODO
-item](#update-a-todo-item) * [Delete a TODO item](#delete-a-todo-item) * [Move
-yesterday's unfinished todo to today](#move-yesterdays-unfinished-todo-to-
-today) * [(Advanced Usage) ð Upload Markdown files](#advanced-usage--upload-
-markdown-files) * [Upload single Markdown file with images](#upload-single-
-markdown-file-with-images) * [Bulk upload Markdown files in a folder](#bulk-
-upload-markdown-files-in-a-folder) * [Import from VNote](#import-from-vnote) *
-[Import from Joplin](#import-from-joplin) * [Import from Logseq](#import-from-
-logseq) * [Import from Obsidian](#import-from-obsidian) * [Import from Youdao
-Note/æéäºç¬è®°](#import-from-youdao-noteæéäºç¬è®°) * [Import from
-Turtl](#import-from-turtl) * [Import from other markdown software](#import-
-from-other-markdown-software) * [(Advanced Usage) ð¨ Beautify notes]
-(#advanced-usage--beautify-notes) * [Beautify a note](#beautify-a-note) *
-[Beautify a note and its child notes](#beautify-a-note-and-its-child-notes) * [
-(Advanced Usage) ð§¹ Sort note content](#advanced-usage--sort-note-content) *
-[(Advanced Usage) ð§¹ Delete empty new note](#advanced-usage--delete-empty-
-new-note) * [ð ï¸ Develop](#ï¸-develop) * [ð Original OpenAPI
-Documentation](#-original-openapi-documentation) ## ð§ Installation ```bash
-python3 -m pip install trilium-py --user ``` ## ð (Basic) Usage These are
-basic function that Trilium's ETAPI provides. Down below are some simple
-example code to use this package. ### ð Initialization If you have a ETAPI
-token, change the `server_url` and `token` to yours. ```python from
-trilium_py.client import ETAPI server_url = 'http://localhost:8080' token =
-'YOUR_TOKEN' ea = ETAPI(server_url, token) ``` If you haven't created ETAPI
-token, you can create one with your password. Please note, you can only see
-this token once, please save it if you want to reuse the token. ```python from
-trilium_py.client import ETAPI server_url = 'http://localhost:8080' password =
-'1234' ea = ETAPI(server_url) token = ea.login(password) print(token) ``` After
-initialization, you can use Trilium ETAPI with python now. The following are
-some examples. ### ð Application Information To start with, you can get the
-application information like this. ```python print(ea.app_info()) ``` It should
-give you the version of your server application and some extra information. ###
-ð Search note Search note with keyword. ```python res = ea.search_note
+note](#-export-note) * [ð¥ import note](#-import-note) * [ð¾ Save revision]
+(#-save-revision) * [ð¾ Create data backup](#-create-data-backup) * [ð·
+Create attribute](#-create-attribute) * [Get attachment list](#get-attachment-
+list) * [Get attachment info](#get-attachment-info) * [Update attachment info]
+(#update-attachment-info) * [Get attachment content](#get-attachment-content) *
+[Update attachment content](#update-attachment-content) * [Create attachment]
+(#create-attachment) * [(Advanced Usage) â TODO List](#advanced-usage--todo-
+list) * [Add TODO item](#add-todo-item) * [Check/Uncheck a TODO item]
+(#checkuncheck-a-todo-item) * [Update a TODO item](#update-a-todo-item) *
+[Delete a TODO item](#delete-a-todo-item) * [Move yesterday's unfinished todo
+to today](#move-yesterdays-unfinished-todo-to-today) * [(Advanced Usage) ð
+Upload Markdown files](#advanced-usage--upload-markdown-files) * [Upload single
+Markdown file with images](#upload-single-markdown-file-with-images) * [Bulk
+upload Markdown files in a folder](#bulk-upload-markdown-files-in-a-folder) *
+[Import from VNote](#import-from-vnote) * [Import from Joplin](#import-from-
+joplin) * [Import from Logseq](#import-from-logseq) * [Import from Obsidian]
+(#import-from-obsidian) * [Import from Youdao Note/æéäºç¬è®°](#import-
+from-youdao-noteæéäºç¬è®°) * [Import from Turtl](#import-from-turtl) *
+[Import from other markdown software](#import-from-other-markdown-software) * [
+(Advanced Usage) ð¨ Beautify notes](#advanced-usage--beautify-notes) *
+[Beautify a note](#beautify-a-note) * [Beautify a note and its child notes]
+(#beautify-a-note-and-its-child-notes) * [(Advanced Usage) ð§¹ Sort note
+content](#advanced-usage--sort-note-content) * [(Advanced Usage) ð§¹ Delete
+empty new note](#advanced-usage--delete-empty-new-note) * [(Advanced Usage)
+ðï¸ Optimize image size](#advanced-usage-ï¸-optimize-image-size) *
+[ð ï¸ Develop](#ï¸-develop) * [ð Original OpenAPI Documentation](#-
+original-openapi-documentation) ## ð§ Installation ```bash python3 -m pip
+install trilium-py --user ``` ## ð (Basic) Usage These are basic function
+that Trilium's ETAPI provides. Down below are some simple example code to use
+this package. ### ð Initialization If you have a ETAPI token, change the
+`server_url` and `token` to yours. ```python from trilium_py.client import
+ETAPI server_url = 'http://localhost:8080' token = 'YOUR_TOKEN' ea = ETAPI
+(server_url, token) ``` If you haven't created ETAPI token, you can create one
+with your password. Please note, you can only see this token once, please save
+it if you want to reuse the token. ```python from trilium_py.client import
+ETAPI server_url = 'http://localhost:8080' password = '1234' ea = ETAPI
+(server_url) token = ea.login(password) print(token) ``` After initialization,
+you can use Trilium ETAPI with python now. The following are some examples. ###
+ð Application Information To start with, you can get the application
+information like this. ```python print(ea.app_info()) ``` It should give you
+the version of your server application and some extra information. ### ð
+Search note Search note with keyword. ```python res = ea.search_note
 ( search="python", ) for x in res['results']: print(x['noteId'], x['title'])
 ``` Search with regular expression. For example, search and get all child notes
 under certain note: ```python res = ea.search_note( # regular expression search
 for note title search="note.title %= '.*'", ancestorNoteId="Parent Note ID",
 fastSearch=False, limit=1000, ) ``` ### ð­ Create Note You can create a
 simple note like this. ```python res = ea.create_note( parentNoteId="root",
 title="Simple note 1", type="text", content="Simple note example",
@@ -111,15 +115,15 @@
 ```bash 0 3 * * * python /path/to/backup-script.py ``` ### ð· Create
 attribute You can create a tag for a note ```python res = ea.create_attribute
 ( noteId='noteid', type='label', name='name_of_the_tag',
 value='value_of_the_tag', isInheritable=True ) ``` The `noteId` is not
 mandatory, if not provided, Trilium will generate a random one. You can
 retrieve it in the return. ```python noteId = res['note']['noteId'] ``` ### Get
 attachment list Get all attachments of a single note. ``` res =
-ea.get_attachmants('uMJt0Ajr1CuC') ``` ### Get attachment info Get image title
+ea.get_attachments('uMJt0Ajr1CuC') ``` ### Get attachment info Get image title
 and etc. ```python res = ea.get_attachment('Y5V6pYq6nwXo') ``` ### Update
 attachment info Change image title and etc. ```python res =
 ea.update_attachment( attachmentId='2b7pPzqocS1s', title='hello etapi',
 role='image', mime='image/png' ) ``` ### Get attachment content Get the real
 image file ```python res = ea.get_attachment_content('icpDE4orQxlI') with open
 ('1.png', 'wb') as f: f.write(res) ``` ### Update attachment content Replace
 the image with new one ```python res = ea.update_attachment_content
@@ -192,13 +196,17 @@
 preferences. ```python res = ea.sort_note_content('lPxtkknjR2bJ') res =
 ea.sort_note_content('y6hROhWjNmHQ', 'zh_CN.UTF-8') ``` ## (Advanced Usage)
 ð§¹ Delete empty `new note` Sometimes I inadvertently create numerous "new
 notes" which remain undeleted within my note tree. These "new notes" clutter my
 workspace, scattered across various locations. I made this bulk deletion of
 these empty "new notes." Additionally, it generates warning messages for "new
 notes" that contain content, maybe we should change the title for those notes.
-```python ea.delete_empty_note() ``` ## ð ï¸ Develop Install with pip egg
-link to make package change without reinstall. ```python python -m pip install
---user -e . ``` ## ð Original OpenAPI Documentation The original OpenAPI
-document is [here](https://github.com/zadam/trilium/blob/master/src/etapi/
-etapi.openapi.yaml). You can open it with [swagger editor](https://
-editor.swagger.io/).
+```python ea.delete_empty_note() ``` ## (Advanced Usage) ðï¸ Optimize image
+size Try to reduce image size by using PIL's optimize feature. If the image in
+your note is not compressed, you can try this. I've successfully convert a note
+of 44MB to 9.9MB after this process. Backup your data before try this. ```
+ea.optimize_image_attachments('uMJt0Ajr1CuC') ``` ## ð ï¸ Develop Install
+with pip egg link to make package change without reinstall. ```python python -
+m pip install --user -e . ``` ## ð Original OpenAPI Documentation The
+original OpenAPI document is [here](https://github.com/zadam/trilium/blob/
+master/src/etapi/etapi.openapi.yaml). You can open it with [swagger editor]
+(https://editor.swagger.io/).
```

## Comparing `trilium_py-0.9.0.dist-info/RECORD` & `trilium_py-0.9.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 trilium_py/__init__.py,sha256=uSMH49RW2MFU_LVKKKm6lt3xOBsDWo0cb8--nMcNlgY,141
-trilium_py/client.py,sha256=otd_sAgzOlLvwlWPh-_bh6mSCE29mkz_FRXTmfLrVjA,45427
+trilium_py/client.py,sha256=Y3ENSBOqwWLmeNZ9VRGxWciOdy0OHGc4oSoanDN5LYM,47014
 trilium_py/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 trilium_py/utils/html_util.py,sha256=OuFEt5bHiiNYtBDX_ABPXudDoHpid97GmicFQwuidNE,2290
+trilium_py/utils/image_util.py,sha256=zEPaS3vSbUWDXMMzzlz30DWuVTQS1YW1nJoxCAEeGiE,1083
 trilium_py/utils/markdown_math.py,sha256=sAiR_5YaCE_EOeQ4vZBjoc5t0Z1n_5EQ4JmJ1TAweCY,9328
 trilium_py/utils/note_util.py,sha256=jSavmxnV8Fn-DKoFeNLFVxtkrn176wQF_pbiPJCdEu8,3909
 trilium_py/utils/param_util.py,sha256=jlnKrCKBtaN1wfQgxDTvGmuMM0p7vk809vpaLgK0dXg,681
 trilium_py/utils/time_util.py,sha256=DIFQmCKZ_wL5lCdeTMJZAtFolZw_dic6NKZ8CCJTa1A,208
 trilium_py/utils/url_util.py,sha256=1eHmHlti4CwsN-hjqfennxiohkrUX0jtuX3UleTD120,486
-trilium_py-0.9.0.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-trilium_py-0.9.0.dist-info/METADATA,sha256=Jq_Yg-N8XlY48cRVCbZiC-kQSbf7vSiXAMB1vHsKO9U,15968
-trilium_py-0.9.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-trilium_py-0.9.0.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
-trilium_py-0.9.0.dist-info/RECORD,,
+trilium_py-0.9.1.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+trilium_py-0.9.1.dist-info/METADATA,sha256=YlJeM5LHbnnW7FFfsw2YYoTgwFbPnZVZjV9Cs53Q34Y,16604
+trilium_py-0.9.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+trilium_py-0.9.1.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
+trilium_py-0.9.1.dist-info/RECORD,,
```

