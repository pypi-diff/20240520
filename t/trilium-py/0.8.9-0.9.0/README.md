# Comparing `tmp/trilium_py-0.8.9-py3-none-any.whl.zip` & `tmp/trilium_py-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 34238 bytes, number of entries: 14
+Zip file size: 34432 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      141 b- defN 24-Apr-22 06:33 trilium_py/__init__.py
--rw-r--r--  2.0 unx    44149 b- defN 24-Apr-22 06:50 trilium_py/client.py
+-rw-r--r--  2.0 unx    45427 b- defN 24-May-20 07:05 trilium_py/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 07:17 trilium_py/utils/__init__.py
 -rw-r--r--  2.0 unx     2290 b- defN 24-Apr-22 06:32 trilium_py/utils/html_util.py
 -rw-r--r--  2.0 unx     9328 b- defN 24-Apr-22 06:33 trilium_py/utils/markdown_math.py
 -rw-r--r--  2.0 unx     3909 b- defN 24-Apr-22 06:33 trilium_py/utils/note_util.py
 -rw-r--r--  2.0 unx      681 b- defN 24-Apr-22 06:33 trilium_py/utils/param_util.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-22 06:33 trilium_py/utils/time_util.py
 -rw-r--r--  2.0 unx      486 b- defN 24-Apr-22 06:33 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    15640 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/RECORD
-14 files, 113281 bytes uncompressed, 32300 bytes compressed:  71.5%
+-rwxrwx---  2.0 unx    35184 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    15968 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1162 b- defN 24-May-20 07:12 trilium_py-0.9.0.dist-info/RECORD
+14 files, 114887 bytes uncompressed, 32494 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.8.9.dist-info/LICENSE.txt
+Filename: trilium_py-0.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.8.9.dist-info/METADATA
+Filename: trilium_py-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.8.9.dist-info/WHEEL
+Filename: trilium_py-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.8.9.dist-info/top_level.txt
+Filename: trilium_py-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.8.9.dist-info/RECORD
+Filename: trilium_py-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -496,39 +496,73 @@
         return res.json()
 
     def get_calendar_years(self, year: str) -> dict:
         url = f'{self.server_url}/etapi/calendar/years/{year}'
         res = requests.get(url, headers=self.get_header())
         return res.json()
 
-    def export_note(self, noteId: str, format: str, savePath: str, chunk_size=128):
+    def export_note(self, noteId: str, format: str, save_path: str, chunk_size=128):
         """
         Export note by id. Please note that protected notes are not allowed to be exported by ETAPI.
 
         :param noteId: note id
         :param format: format should be "html" or "markdown" or "md" for short
-        :savePath: path for exported file
+        :save_path: path for exported file
         :chunk_size: download chunk size, default to 128
         :return:
         """
         url = f'{self.server_url}/etapi/notes/{noteId}/export'
         if format in ['md', 'markdown']:
             format = 'markdown'
         else:
             format = 'html'
         params = {
             "format": format,
         }
         r = requests.get(url, params=clean_param(params), headers=self.get_header())
         logger.info(r.status_code)
-        with open(savePath, 'wb') as fd:
+        with open(save_path, 'wb') as fd:
             for chunk in r.iter_content(chunk_size=chunk_size):
                 fd.write(chunk)
         return True
 
+    def import_note(self, noteId: str, file_path: str):
+        """
+        import zip format note
+        """
+        url = f'{self.server_url}/etapi/notes/{noteId}/import'
+        file_data = open(file_path, 'rb').read()
+        res = requests.post(
+            url,
+            data=file_data,
+            headers={
+                'content-type': 'application/octet-stream',
+                'Content-Transfer-Encoding': 'binary',
+                'Authorization': self.token,
+            },
+        )
+        logger.info(res)
+        if res.status_code == 201:
+            return True
+        else:
+            return False
+
+    def save_revision(self, noteId: str):
+        """
+        force save note revision
+        :param noteId:
+        :return:
+        """
+
+        url = f'{self.server_url}/etapi/notes/{noteId}/revision'
+        res = requests.post(url, headers=self.get_header())
+        if res.status_code == 204:
+            return True
+        return False
+
     def get_today_note_content(self):
         date = get_today()
         return self.get_day_note(date)
 
     def set_today_note_content(self, content):
         date = get_today()
         return self.set_day_note(date, content)
@@ -1096,14 +1130,25 @@
         :return:
         """
         url = f"{self.server_url}/etapi/sync/now"
         res = requests.post(url, headers=self.get_header())
         if res.status_code == 200:
             logger.info("sync successfully")
 
+    def get_attachmants(self, noteId: str):
+        """
+        get attachment list of a note
+        :param noteId:
+        :return:
+        """
+        url = f'{self.server_url}/etapi/notes/{noteId}/attachments'
+
+        res = requests.get(url, headers=self.get_header())
+        return res.json()
+
     def get_attachment(self, attachmentId: str) -> dict:
         """
         get attachment by id
 
         :param attachmentId:
         :return:
         """
```

## Comparing `trilium_py-0.8.9.dist-info/LICENSE.txt` & `trilium_py-0.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.8.9.dist-info/METADATA` & `trilium_py-0.9.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
@@ -42,64 +42,61 @@
 
 [![Downloads](https://static.pepy.tech/badge/trilium-py)](https://pepy.tech/project/trilium-py)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/trilium-py.svg)](https://pypi.org/project/trilium-py)
 [![Supported Versions](https://img.shields.io/pypi/v/trilium-py?color=%2334D058&label=pypi%20package)](https://pypi.org/project/trilium-py)
 [![PyPI license](https://img.shields.io/pypi/l/trilium-py.svg)](https://pypi.python.org/pypi/trilium-py/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 
-<a href="https://github.com/Nriver"><img align="center" src="https://moe-counter--nriver1.repl.co/get/@Nriver_trilium-py"></a><br>
-
 ## 🦮 Table of Contents
 
 <!--ts-->
-
-- [🐍 trilium-py](#-trilium-py)
-    - [🦮 Table of Contents](#-table-of-contents)
-    - [🔧 Installation](#-installation)
-    - [📖 (Basic) Usage](#-basic-usage)
-        - [🚀 Initialization](#-initialization)
-        - [📊 Application Information](#-application-information)
-        - [🔍 Search note](#-search-note)
-        - [🏭 Create Note](#-create-note)
-            - [🖼️ Create Image note](#️-create-image-note)
-        - [👀 Get note](#-get-note)
-        - [🔄 Update note](#-update-note)
-        - [🗑️ Delete note](#️-delete-note)
-        - [📅 Day note](#-day-note)
-        - [📤 Export note](#-export-note)
-        - [💾 Create data backup](#-create-data-backup)
-        - [🏷 Create Attribute](#-create-attribute)
-        - [Get attachment info](#get-attachment-info)
-        - [Update attachment info](#update-attachment-info)
-        - [Get attachment content](#get-attachment-content)
-        - [Update attachment content](#update-attachment-content)
-        - [Create attachment](#create-attachment)
-    - [(Advanced Usage) ✅ TODO List](#advanced-usage--todo-list)
-        - [Add TODO item](#add-todo-item)
-        - [Check/Uncheck a TODO item](#checkuncheck-a-todo-item)
-        - [Update a TODO item](#update-a-todo-item)
-        - [Delete a TODO item](#delete-a-todo-item)
-        - [Move yesterday's unfinished todo to today](#move-yesterdays-unfinished-todo-to-today)
-    - [(Advanced Usage) 🚚 Upload Markdown files](#advanced-usage--upload-markdown-files)
-        - [Upload single Markdown file with images](#upload-single-markdown-file-with-images)
-        - [Bulk upload Markdown files in a folder](#bulk-upload-markdown-files-in-a-folder)
-            - [Import from VNote](#import-from-vnote)
-            - [Import from Joplin](#import-from-joplin)
-            - [Import from Logseq](#import-from-logseq)
-            - [Import from Obsidian](#import-from-obsidian)
-            - [Import from Youdao Note/有道云笔记](#import-from-youdao-note有道云笔记)
-            - [Import from Turtl](#import-from-turtl)
-            - [Import from other markdown software](#import-from-other-markdown-software)
-    - [(Advanced Usage) 🎨 Beautify notes](#advanced-usage--beautify-notes)
-        - [Beautify a note](#beautify-a-note)
-        - [Beautify a note and its child notes](#beautify-a-note-and-its-child-notes)
-    - [(Advanced Usage) Sort note content](#advanced-usage--sort-note-content)
-    - [🛠️ Develop](#️-develop)
-    - [🔗 Original OpenAPI Documentation](#-original-openapi-documentation)
-
+* [🐍 trilium-py](#-trilium-py)
+   * [🦮 Table of Contents](#-table-of-contents)
+   * [🔧 Installation](#-installation)
+   * [📖 (Basic) Usage](#-basic-usage)
+      * [🚀 Initialization](#-initialization)
+      * [📊 Application Information](#-application-information)
+      * [🔍 Search note](#-search-note)
+      * [🏭 Create Note](#-create-note)
+         * [🖼️ Create Image note](#️-create-image-note)
+      * [👀 Get note](#-get-note)
+      * [🔄 Update note](#-update-note)
+      * [🗑️ Delete note](#️-delete-note)
+      * [📅 Day note](#-day-note)
+      * [📤 Export note](#-export-note)
+      * [💾 Create data backup](#-create-data-backup)
+      * [🏷 Create attribute](#-create-attribute)
+      * [Get attachment info](#get-attachment-info)
+      * [Update attachment info](#update-attachment-info)
+      * [Get attachment content](#get-attachment-content)
+      * [Update attachment content](#update-attachment-content)
+      * [Create attachment](#create-attachment)
+   * [(Advanced Usage) ✅ TODO List](#advanced-usage--todo-list)
+      * [Add TODO item](#add-todo-item)
+      * [Check/Uncheck a TODO item](#checkuncheck-a-todo-item)
+      * [Update a TODO item](#update-a-todo-item)
+      * [Delete a TODO item](#delete-a-todo-item)
+      * [Move yesterday's unfinished todo to today](#move-yesterdays-unfinished-todo-to-today)
+   * [(Advanced Usage) 🚚 Upload Markdown files](#advanced-usage--upload-markdown-files)
+      * [Upload single Markdown file with images](#upload-single-markdown-file-with-images)
+      * [Bulk upload Markdown files in a folder](#bulk-upload-markdown-files-in-a-folder)
+         * [Import from VNote](#import-from-vnote)
+         * [Import from Joplin](#import-from-joplin)
+         * [Import from Logseq](#import-from-logseq)
+         * [Import from Obsidian](#import-from-obsidian)
+         * [Import from Youdao Note/有道云笔记](#import-from-youdao-note有道云笔记)
+         * [Import from Turtl](#import-from-turtl)
+         * [Import from other markdown software](#import-from-other-markdown-software)
+   * [(Advanced Usage) 🎨 Beautify notes](#advanced-usage--beautify-notes)
+      * [Beautify a note](#beautify-a-note)
+      * [Beautify a note and its child notes](#beautify-a-note-and-its-child-notes)
+   * [(Advanced Usage) 🧹 Sort note content](#advanced-usage--sort-note-content)
+   * [(Advanced Usage) 🧹 Delete empty new note](#advanced-usage--delete-empty-new-note)
+   * [🛠️ Develop](#️-develop)
+   * [🔗 Original OpenAPI Documentation](#-original-openapi-documentation)
 <!--te-->
 
 ## 🔧 Installation
 
 ```bash
 python3 -m pip install trilium-py --user
 ```
@@ -261,15 +258,36 @@
 
 Export note comes in two formats `html` or `markdown`/`md`.
 
 ```python
 res = ea.export_note(
     noteId='sK5fn4T6yZRI',
     format='md',
-    savePath='/home/nate/data/1/test.zip',
+    save_path='/home/nate/data/1/test.zip',
+)
+```
+
+### 📥 import note
+
+This is the built-in feature in trilium. The input file should be a zip file.
+
+```python
+res = ea.export_note(
+    noteId='sK5fn4T6yZRI',
+    file_path='/home/nate/data/1/test.zip',
+)
+```
+
+### 💾 Save revision
+
+Save note revision manually.
+
+```
+res = ea.save_revision(
+    noteId='MJzyFRXAVaC9',
 )
 ```
 
 ### 💾 Create data backup
 
 This example will create a database backup file like this `trilium-data/backup/backup-test.db`.
 
@@ -300,14 +318,22 @@
 
 The `noteId` is not mandatory, if not provided, Trilium will generate a random one. You can retrieve it in the return.
 
 ```python
 noteId = res['note']['noteId']
 ```
 
+### Get attachment list
+
+Get all attachments of a single note.
+
+```
+res = ea.get_attachmants('uMJt0Ajr1CuC')
+```
+
 ### Get attachment info
 
 Get image title and etc.
 
 ```python
 res = ea.get_attachment('Y5V6pYq6nwXo')
 ```
@@ -542,17 +568,17 @@
 sorting process and tailors it to your linguistic preferences.
 
 ```python
 res = ea.sort_note_content('lPxtkknjR2bJ')
 res = ea.sort_note_content('y6hROhWjNmHQ', 'zh_CN.UTF-8')
 ```
 
-## ## (Advanced Usage) 🧹 Delete empty `new note`
+## (Advanced Usage) 🧹 Delete empty `new note`
 
-I inadvertently create numerous "new notes" which remain undeleted within my note tree. These "new notes" clutter my
+Sometimes I inadvertently create numerous "new notes" which remain undeleted within my note tree. These "new notes" clutter my
 workspace, scattered across various locations. I made this bulk deletion of these empty "new notes." Additionally, it
 generates warning messages for "new notes" that contain content, maybe we should change the title for those notes.
 
 ```python
 ea.delete_empty_note()
 ```
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.8.9 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.9.0 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
@@ -22,50 +22,50 @@
 static.pepy.tech/badge/trilium-py)](https://pepy.tech/project/trilium-py) [!
 [Supported Versions](https://img.shields.io/pypi/pyversions/trilium-py.svg)]
 (https://pypi.org/project/trilium-py) [![Supported Versions](https://
 img.shields.io/pypi/v/trilium-py?color=%2334D058&label=pypi%20package)](https:/
 /pypi.org/project/trilium-py) [![PyPI license](https://img.shields.io/pypi/l/
 trilium-py.svg)](https://pypi.python.org/pypi/trilium-py/) [![Maintenance]
 (https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/
-Naereen/StrapDown.js/graphs/commit-activity) _[_h_t_t_p_s_:_/_/_m_o_e_-_c_o_u_n_t_e_r_-_-
-_n_r_i_v_e_r_1_._r_e_p_l_._c_o_/_g_e_t_/_@_N_r_i_v_e_r___t_r_i_l_i_u_m_-_p_y_]
-## ð¦® Table of Contents - [ð trilium-py](#-trilium-py) - [ð¦® Table of
-Contents](#-table-of-contents) - [ð§ Installation](#-installation) - [ð
-(Basic) Usage](#-basic-usage) - [ð Initialization](#-initialization) - [ð
-Application Information](#-application-information) - [ð Search note](#-
-search-note) - [ð­ Create Note](#-create-note) - [ð¼ï¸ Create Image note]
-(#ï¸-create-image-note) - [ð Get note](#-get-note) - [ð Update note](#-
-update-note) - [ðï¸ Delete note](#ï¸-delete-note) - [ð Day note](#-day-
-note) - [ð¤ Export note](#-export-note) - [ð¾ Create data backup](#-create-
-data-backup) - [ð· Create Attribute](#-create-attribute) - [Get attachment
-info](#get-attachment-info) - [Update attachment info](#update-attachment-info)
-- [Get attachment content](#get-attachment-content) - [Update attachment
-content](#update-attachment-content) - [Create attachment](#create-attachment)
-- [(Advanced Usage) â TODO List](#advanced-usage--todo-list) - [Add TODO
-item](#add-todo-item) - [Check/Uncheck a TODO item](#checkuncheck-a-todo-item)
-- [Update a TODO item](#update-a-todo-item) - [Delete a TODO item](#delete-a-
-todo-item) - [Move yesterday's unfinished todo to today](#move-yesterdays-
-unfinished-todo-to-today) - [(Advanced Usage) ð Upload Markdown files]
-(#advanced-usage--upload-markdown-files) - [Upload single Markdown file with
-images](#upload-single-markdown-file-with-images) - [Bulk upload Markdown files
-in a folder](#bulk-upload-markdown-files-in-a-folder) - [Import from VNote]
-(#import-from-vnote) - [Import from Joplin](#import-from-joplin) - [Import from
-Logseq](#import-from-logseq) - [Import from Obsidian](#import-from-obsidian) -
-[Import from Youdao Note/æéäºç¬è®°](#import-from-youdao-
-noteæéäºç¬è®°) - [Import from Turtl](#import-from-turtl) - [Import from
-other markdown software](#import-from-other-markdown-software) - [(Advanced
-Usage) ð¨ Beautify notes](#advanced-usage--beautify-notes) - [Beautify a
-note](#beautify-a-note) - [Beautify a note and its child notes](#beautify-a-
-note-and-its-child-notes) - [(Advanced Usage) Sort note content](#advanced-
-usage--sort-note-content) - [ð ï¸ Develop](#ï¸-develop) - [ð Original
-OpenAPI Documentation](#-original-openapi-documentation) ## ð§ Installation
-```bash python3 -m pip install trilium-py --user ``` ## ð (Basic) Usage
-These are basic function that Trilium's ETAPI provides. Down below are some
-simple example code to use this package. ### ð Initialization If you have a
-ETAPI token, change the `server_url` and `token` to yours. ```python from
+Naereen/StrapDown.js/graphs/commit-activity) ## ð¦® Table of Contents * [ð
+trilium-py](#-trilium-py) * [ð¦® Table of Contents](#-table-of-contents) *
+[ð§ Installation](#-installation) * [ð (Basic) Usage](#-basic-usage) *
+[ð Initialization](#-initialization) * [ð Application Information](#-
+application-information) * [ð Search note](#-search-note) * [ð­ Create
+Note](#-create-note) * [ð¼ï¸ Create Image note](#ï¸-create-image-note) *
+[ð Get note](#-get-note) * [ð Update note](#-update-note) * [ðï¸
+Delete note](#ï¸-delete-note) * [ð Day note](#-day-note) * [ð¤ Export
+note](#-export-note) * [ð¾ Create data backup](#-create-data-backup) * [ð·
+Create attribute](#-create-attribute) * [Get attachment info](#get-attachment-
+info) * [Update attachment info](#update-attachment-info) * [Get attachment
+content](#get-attachment-content) * [Update attachment content](#update-
+attachment-content) * [Create attachment](#create-attachment) * [(Advanced
+Usage) â TODO List](#advanced-usage--todo-list) * [Add TODO item](#add-todo-
+item) * [Check/Uncheck a TODO item](#checkuncheck-a-todo-item) * [Update a TODO
+item](#update-a-todo-item) * [Delete a TODO item](#delete-a-todo-item) * [Move
+yesterday's unfinished todo to today](#move-yesterdays-unfinished-todo-to-
+today) * [(Advanced Usage) ð Upload Markdown files](#advanced-usage--upload-
+markdown-files) * [Upload single Markdown file with images](#upload-single-
+markdown-file-with-images) * [Bulk upload Markdown files in a folder](#bulk-
+upload-markdown-files-in-a-folder) * [Import from VNote](#import-from-vnote) *
+[Import from Joplin](#import-from-joplin) * [Import from Logseq](#import-from-
+logseq) * [Import from Obsidian](#import-from-obsidian) * [Import from Youdao
+Note/æéäºç¬è®°](#import-from-youdao-noteæéäºç¬è®°) * [Import from
+Turtl](#import-from-turtl) * [Import from other markdown software](#import-
+from-other-markdown-software) * [(Advanced Usage) ð¨ Beautify notes]
+(#advanced-usage--beautify-notes) * [Beautify a note](#beautify-a-note) *
+[Beautify a note and its child notes](#beautify-a-note-and-its-child-notes) * [
+(Advanced Usage) ð§¹ Sort note content](#advanced-usage--sort-note-content) *
+[(Advanced Usage) ð§¹ Delete empty new note](#advanced-usage--delete-empty-
+new-note) * [ð ï¸ Develop](#ï¸-develop) * [ð Original OpenAPI
+Documentation](#-original-openapi-documentation) ## ð§ Installation ```bash
+python3 -m pip install trilium-py --user ``` ## ð (Basic) Usage These are
+basic function that Trilium's ETAPI provides. Down below are some simple
+example code to use this package. ### ð Initialization If you have a ETAPI
+token, change the `server_url` and `token` to yours. ```python from
 trilium_py.client import ETAPI server_url = 'http://localhost:8080' token =
 'YOUR_TOKEN' ea = ETAPI(server_url, token) ``` If you haven't created ETAPI
 token, you can create one with your password. Please note, you can only see
 this token once, please save it if you want to reuse the token. ```python from
 trilium_py.client import ETAPI server_url = 'http://localhost:8080' password =
 '1234' ea = ETAPI(server_url) token = ea.login(password) print(token) ``` After
 initialization, you can use Trilium ETAPI with python now. The following are
@@ -94,71 +94,77 @@
 title="Python client moded", ) ``` ### ðï¸ Delete note Simply delete a note
 by id. ```python ea.delete_note("noteid") ``` ### ð Day note You can get the
 content of a certain date with `get_day_note`. The date string should be in
 format of "%Y-%m-%d", e.g. " 2022-02-25". ```python ea.get_day_note("2022-02-
 25") ``` Then set/update a day note with `set_day_note`. The content should be
 a (html) string. ```python ea.set_day_note(date, new_content) ``` ### ð¤
 Export note Export note comes in two formats `html` or `markdown`/`md`.
-```python res = ea.export_note( noteId='sK5fn4T6yZRI', format='md', savePath='/
-home/nate/data/1/test.zip', ) ``` ### ð¾ Create data backup This example will
-create a database backup file like this `trilium-data/backup/backup-test.db`.
-```python res = ea.backup("test") ``` You can use the cron utility in Linux to
-schedule regular automatic backups. For example, to set up a daily backup at 3:
-00 AM, you would use the following cron expression: ```bash 0 3 * * * python /
-path/to/backup-script.py ``` ### ð· Create attribute You can create a tag for
-a note ```python res = ea.create_attribute( noteId='noteid', type='label',
-name='name_of_the_tag', value='value_of_the_tag', isInheritable=True ) ``` The
-`noteId` is not mandatory, if not provided, Trilium will generate a random one.
-You can retrieve it in the return. ```python noteId = res['note']['noteId'] ```
-### Get attachment info Get image title and etc. ```python res =
-ea.get_attachment('Y5V6pYq6nwXo') ``` ### Update attachment info Change image
-title and etc. ```python res = ea.update_attachment
-( attachmentId='2b7pPzqocS1s', title='hello etapi', role='image', mime='image/
-png' ) ``` ### Get attachment content Get the real image file ```python res =
-ea.get_attachment_content('icpDE4orQxlI') with open('1.png', 'wb') as f:
-f.write(res) ``` ### Update attachment content Replace the image with new one
-```python res = ea.update_attachment_content('icWqV6zFtE0V', '/home/nate/data/
-1.png') ``` ### Create attachment Upload a image file as attachment of a note.
-```python res = ea.create_attachment( ownerId='8m8luXym5LxT', file_path='/home/
-nate/data/ksnip_20230630-103509.png', ) ``` ## (Advanced Usage) â TODO List
-With the power of Python, I have expanded the basic usage of ETAPI. You can do
-something with todo list now. ### Add TODO item You can use `add_todo` to add a
-TODO item, param is the TODO description ```python ea.add_todo("ä¹°æå®å®")
-``` ### Check/Uncheck a TODO item param is the index of the TODO item ```python
-ea.todo_check(0) ea.todo_uncheck(1) ``` ### Update a TODO item Use
-`update_todo` to update a TODO item description at certain index. ```python
-ea.update_todo(0, "å»ç å¤´æ´ç¹è¯æ¡") ``` ### Delete a TODO item Remove a
-TODO item by its index. ```python ea.delete_todo(1) ``` ### Move yesterday's
-unfinished todo to today As the title suggests, you can move yesterday's
-unfinished things to today. Unfinished todo's will be deleted from yesterday's
-note. ```python ea.move_yesterday_unfinished_todo_to_today() ``` ## (Advanced
-Usage) ð Upload Markdown files ### Upload single Markdown file with images
-You can import Markdown file with images into Trilium now! Trilium-py will help
-you to upload the images and fix the links for you! ```python res =
-ea.upload_md_file( parentNoteId="root", file="./md-demo/manjaro ä¿®æ¹caps
-lock.md", ) ``` ### Bulk upload Markdown files in a folder You can upload a
-folder with lots of Markdown files to Trilium and preserve the folder
-structure! #### Import from VNote Say, upload all the notes from [VNote](https:
-//github.com/vnotex/vnote), simply do this: ```python res = ea.upload_md_folder
-( parentNoteId="root", mdFolder="~/data/vnotebook/", ignoreFolder=
-['vx_notebook', 'vx_recycle_bin', 'vx_images', '_v_images'], ) ``` #### Import
-from Joplin Joplin can be imported effortlessly. ```python res =
-ea.upload_md_folder( parentNoteId="root", mdFolder="/home/nate/data/
-joplin_data/", ignoreFolder=['_resources', ], ) ``` #### Import from Logseq
-```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="/home/nate/
-data/logseq_data/", ignoreFolder=['assets', 'logseq'], ) ``` #### Import from
-Obsidian Obsidian has a very unique linking system for files. You should use
-[obsidian-export ](https://github.com/zoni/obsidian-export) to convert a
-Obsidian vault to regular Markdown files. Then you should be able to import the
-note into Trilium with trilium-py. Convert it first. ```bash obsidian-export /
-path/to/your/vault /out ``` Then import just like a normal markdown, trilium-py
-will handle the images for you. ```python res = ea.upload_md_folder
-( parentNoteId="root", mdFolder="E:/data/out", ) ``` #### Import from Youdao
-Note/æéäºç¬è®° Youdao does not provide an export feature anymore.
-Luckily, you can use
+```python res = ea.export_note( noteId='sK5fn4T6yZRI', format='md',
+save_path='/home/nate/data/1/test.zip', ) ``` ### ð¥ import note This is the
+built-in feature in trilium. The input file should be a zip file. ```python res
+= ea.export_note( noteId='sK5fn4T6yZRI', file_path='/home/nate/data/1/
+test.zip', ) ``` ### ð¾ Save revision Save note revision manually. ``` res =
+ea.save_revision( noteId='MJzyFRXAVaC9', ) ``` ### ð¾ Create data backup This
+example will create a database backup file like this `trilium-data/backup/
+backup-test.db`. ```python res = ea.backup("test") ``` You can use the cron
+utility in Linux to schedule regular automatic backups. For example, to set up
+a daily backup at 3: 00 AM, you would use the following cron expression:
+```bash 0 3 * * * python /path/to/backup-script.py ``` ### ð· Create
+attribute You can create a tag for a note ```python res = ea.create_attribute
+( noteId='noteid', type='label', name='name_of_the_tag',
+value='value_of_the_tag', isInheritable=True ) ``` The `noteId` is not
+mandatory, if not provided, Trilium will generate a random one. You can
+retrieve it in the return. ```python noteId = res['note']['noteId'] ``` ### Get
+attachment list Get all attachments of a single note. ``` res =
+ea.get_attachmants('uMJt0Ajr1CuC') ``` ### Get attachment info Get image title
+and etc. ```python res = ea.get_attachment('Y5V6pYq6nwXo') ``` ### Update
+attachment info Change image title and etc. ```python res =
+ea.update_attachment( attachmentId='2b7pPzqocS1s', title='hello etapi',
+role='image', mime='image/png' ) ``` ### Get attachment content Get the real
+image file ```python res = ea.get_attachment_content('icpDE4orQxlI') with open
+('1.png', 'wb') as f: f.write(res) ``` ### Update attachment content Replace
+the image with new one ```python res = ea.update_attachment_content
+('icWqV6zFtE0V', '/home/nate/data/1.png') ``` ### Create attachment Upload a
+image file as attachment of a note. ```python res = ea.create_attachment
+( ownerId='8m8luXym5LxT', file_path='/home/nate/data/ksnip_20230630-
+103509.png', ) ``` ## (Advanced Usage) â TODO List With the power of Python,
+I have expanded the basic usage of ETAPI. You can do something with todo list
+now. ### Add TODO item You can use `add_todo` to add a TODO item, param is the
+TODO description ```python ea.add_todo("ä¹°æå®å®") ``` ### Check/Uncheck a
+TODO item param is the index of the TODO item ```python ea.todo_check(0)
+ea.todo_uncheck(1) ``` ### Update a TODO item Use `update_todo` to update a
+TODO item description at certain index. ```python ea.update_todo(0,
+"å»ç å¤´æ´ç¹è¯æ¡") ``` ### Delete a TODO item Remove a TODO item by its
+index. ```python ea.delete_todo(1) ``` ### Move yesterday's unfinished todo to
+today As the title suggests, you can move yesterday's unfinished things to
+today. Unfinished todo's will be deleted from yesterday's note. ```python
+ea.move_yesterday_unfinished_todo_to_today() ``` ## (Advanced Usage) ð
+Upload Markdown files ### Upload single Markdown file with images You can
+import Markdown file with images into Trilium now! Trilium-py will help you to
+upload the images and fix the links for you! ```python res = ea.upload_md_file
+( parentNoteId="root", file="./md-demo/manjaro ä¿®æ¹caps lock.md", ) ``` ###
+Bulk upload Markdown files in a folder You can upload a folder with lots of
+Markdown files to Trilium and preserve the folder structure! #### Import from
+VNote Say, upload all the notes from [VNote](https://github.com/vnotex/vnote),
+simply do this: ```python res = ea.upload_md_folder( parentNoteId="root",
+mdFolder="~/data/vnotebook/", ignoreFolder=['vx_notebook', 'vx_recycle_bin',
+'vx_images', '_v_images'], ) ``` #### Import from Joplin Joplin can be imported
+effortlessly. ```python res = ea.upload_md_folder( parentNoteId="root",
+mdFolder="/home/nate/data/joplin_data/", ignoreFolder=['_resources', ], ) ```
+#### Import from Logseq ```python res = ea.upload_md_folder
+( parentNoteId="root", mdFolder="/home/nate/data/logseq_data/", ignoreFolder=
+['assets', 'logseq'], ) ``` #### Import from Obsidian Obsidian has a very
+unique linking system for files. You should use [obsidian-export ](https://
+github.com/zoni/obsidian-export) to convert a Obsidian vault to regular
+Markdown files. Then you should be able to import the note into Trilium with
+trilium-py. Convert it first. ```bash obsidian-export /path/to/your/vault /out
+``` Then import just like a normal markdown, trilium-py will handle the images
+for you. ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="E:
+/data/out", ) ``` #### Import from Youdao Note/æéäºç¬è®° Youdao does not
+provide an export feature anymore. Luckily, you can use
 github.com/DeppWang/youdaonote-pull> to download your notes and convert them
 into markdown files. After that, trilium-py should be able to help you import
 them. ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="/
 home/nate/gitRepo/youdaonote-pull/out/", ) ``` #### Import from Turtl You need
 to convert Turtl from json to markdown first. See [turtl-to-markdown](https://
 github.com/Nriver/trilium-py/tree/main/examples/turtl-to-markdown) for details.
 Then you can import with trilium-py like this: ```python res =
@@ -180,19 +186,19 @@
 ('tlPuzU2szLJh') ``` ## (Advanced Usage) ð§¹ Sort note content Sort a note by
 the heading names. This feature could prove invaluable for notes containing
 extensive lists, such as book titles sorted into various genres. It's equally
 useful for managing browser bookmarks or collecting links. Additionally, you
 have the option to specify a language code for sorting based on your local
 language. This enhances the sorting process and tailors it to your linguistic
 preferences. ```python res = ea.sort_note_content('lPxtkknjR2bJ') res =
-ea.sort_note_content('y6hROhWjNmHQ', 'zh_CN.UTF-8') ``` ## ## (Advanced Usage)
-ð§¹ Delete empty `new note` I inadvertently create numerous "new notes" which
-remain undeleted within my note tree. These "new notes" clutter my workspace,
-scattered across various locations. I made this bulk deletion of these empty
-"new notes." Additionally, it generates warning messages for "new notes" that
-contain content, maybe we should change the title for those notes. ```python
-ea.delete_empty_note() ``` ## ð ï¸ Develop Install with pip egg link to make
-package change without reinstall. ```python python -m pip install --user -e .
-``` ## ð Original OpenAPI Documentation The original OpenAPI document is
-[here](https://github.com/zadam/trilium/blob/master/src/etapi/
+ea.sort_note_content('y6hROhWjNmHQ', 'zh_CN.UTF-8') ``` ## (Advanced Usage)
+ð§¹ Delete empty `new note` Sometimes I inadvertently create numerous "new
+notes" which remain undeleted within my note tree. These "new notes" clutter my
+workspace, scattered across various locations. I made this bulk deletion of
+these empty "new notes." Additionally, it generates warning messages for "new
+notes" that contain content, maybe we should change the title for those notes.
+```python ea.delete_empty_note() ``` ## ð ï¸ Develop Install with pip egg
+link to make package change without reinstall. ```python python -m pip install
+--user -e . ``` ## ð Original OpenAPI Documentation The original OpenAPI
+document is [here](https://github.com/zadam/trilium/blob/master/src/etapi/
 etapi.openapi.yaml). You can open it with [swagger editor](https://
 editor.swagger.io/).
```

## Comparing `trilium_py-0.8.9.dist-info/RECORD` & `trilium_py-0.9.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 trilium_py/__init__.py,sha256=uSMH49RW2MFU_LVKKKm6lt3xOBsDWo0cb8--nMcNlgY,141
-trilium_py/client.py,sha256=HJm8qnanq5mlDHtXCZLWHdmAOSfeWdVchsWZV8dlt1M,44149
+trilium_py/client.py,sha256=otd_sAgzOlLvwlWPh-_bh6mSCE29mkz_FRXTmfLrVjA,45427
 trilium_py/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 trilium_py/utils/html_util.py,sha256=OuFEt5bHiiNYtBDX_ABPXudDoHpid97GmicFQwuidNE,2290
 trilium_py/utils/markdown_math.py,sha256=sAiR_5YaCE_EOeQ4vZBjoc5t0Z1n_5EQ4JmJ1TAweCY,9328
 trilium_py/utils/note_util.py,sha256=jSavmxnV8Fn-DKoFeNLFVxtkrn176wQF_pbiPJCdEu8,3909
 trilium_py/utils/param_util.py,sha256=jlnKrCKBtaN1wfQgxDTvGmuMM0p7vk809vpaLgK0dXg,681
 trilium_py/utils/time_util.py,sha256=DIFQmCKZ_wL5lCdeTMJZAtFolZw_dic6NKZ8CCJTa1A,208
 trilium_py/utils/url_util.py,sha256=1eHmHlti4CwsN-hjqfennxiohkrUX0jtuX3UleTD120,486
-trilium_py-0.8.9.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-trilium_py-0.8.9.dist-info/METADATA,sha256=7jqrk3Y-rythyxZSj5o_kuB9znwO14IP5ym5TA0ifcE,15640
-trilium_py-0.8.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-trilium_py-0.8.9.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
-trilium_py-0.8.9.dist-info/RECORD,,
+trilium_py-0.9.0.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+trilium_py-0.9.0.dist-info/METADATA,sha256=Jq_Yg-N8XlY48cRVCbZiC-kQSbf7vSiXAMB1vHsKO9U,15968
+trilium_py-0.9.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+trilium_py-0.9.0.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
+trilium_py-0.9.0.dist-info/RECORD,,
```

