# Comparing `tmp/sharepoint_crud-1.1-py3-none-any.whl.zip` & `tmp/sharepoint_crud-1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4187 bytes, number of entries: 7
+Zip file size: 4615 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       38 b- defN 24-Apr-15 17:29 sharepoint_crud/__init__.py
--rw-r--r--  2.0 unx     1465 b- defN 24-Apr-15 17:29 sharepoint_crud/sharepoint.py
--rw-r--r--  2.0 unx     1072 b- defN 24-Apr-15 17:31 sharepoint_crud-1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3480 b- defN 24-Apr-15 17:31 sharepoint_crud-1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 17:31 sharepoint_crud-1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-15 17:31 sharepoint_crud-1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      584 b- defN 24-Apr-15 17:31 sharepoint_crud-1.1.dist-info/RECORD
-7 files, 6747 bytes uncompressed, 3143 bytes compressed:  53.4%
+-rw-r--r--  2.0 unx     3200 b- defN 24-May-20 19:12 sharepoint_crud/sharepoint.py
+-rw-r--r--  2.0 unx     1072 b- defN 24-May-20 19:14 sharepoint_crud-1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3509 b- defN 24-May-20 19:14 sharepoint_crud-1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 19:14 sharepoint_crud-1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-20 19:14 sharepoint_crud-1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      584 b- defN 24-May-20 19:14 sharepoint_crud-1.5.dist-info/RECORD
+7 files, 8511 bytes uncompressed, 3571 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sharepoint_crud/__init__.py
 Comment: 
 
 Filename: sharepoint_crud/sharepoint.py
 Comment: 
 
-Filename: sharepoint_crud-1.1.dist-info/LICENSE
+Filename: sharepoint_crud-1.5.dist-info/LICENSE
 Comment: 
 
-Filename: sharepoint_crud-1.1.dist-info/METADATA
+Filename: sharepoint_crud-1.5.dist-info/METADATA
 Comment: 
 
-Filename: sharepoint_crud-1.1.dist-info/WHEEL
+Filename: sharepoint_crud-1.5.dist-info/WHEEL
 Comment: 
 
-Filename: sharepoint_crud-1.1.dist-info/top_level.txt
+Filename: sharepoint_crud-1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: sharepoint_crud-1.1.dist-info/RECORD
+Filename: sharepoint_crud-1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sharepoint_crud/sharepoint.py

```diff
@@ -1,12 +1,16 @@
 from office365.sharepoint.client_context import ClientContext
 from office365.runtime.auth.user_credential import UserCredential
 from office365.sharepoint.files.file import File
+from office365.sharepoint.files.file_creation_information import FileCreationInformation
+import os
 
 class SharePointCrud():
+    """Class for interacting with SharePoint.
+    """
     def __init__(self, site, username, password):
         self._site = site
         self._username = username
         self._password = password
 
 
     @property
@@ -35,25 +39,70 @@
 
 
     @password.setter
     def password(self, password):
         self._password = password
 
 
-    def _auth(self):
+    def _auth(self) -> ClientContext:
+        """Method for authenticating the user.
+
+        Returns:
+            ClientContext: context for the user.
+        """
         conn = ClientContext(self._site).with_credentials(UserCredential(self._username, self._password))
         return conn
 
 
-    def get_files_list(self, folder_name):
+    def get_files_list(self, folder_name:str) -> list:
+        """Method for getting the list of files in a folder.
+
+        Args:
+            folder_name (str): The name of the folder.
+
+        Returns:
+            list: List of files in the folder.
+        """
         conn = self._auth()
         target_folder_url = f"{folder_name}"
         root_folder = conn.web.get_folder_by_server_relative_url(target_folder_url)
         root_folder.expand(['Files', 'Folders']).get().execute_query()
         return root_folder.files
 
 
-    def get_file(self, folder_name, file_name):
+    def get_file(self, folder_name:str, file_name:str) -> bytes:
+        """Method for getting the content of a file.
+
+        Args:
+            folder_name (str): the name of the folder.
+            file_name (str): the name of the file.
+
+        Returns:
+            bytes: the content of the file.
+        """
         conn = self._auth()
         file_url = f'/sites/{folder_name}/{file_name}'
         file = File.open_binary(conn, file_url)
         return file.content
+
+
+    def upload_file(self, file:str, folder_name:str, overwrite:bool=False) -> any:
+        """Method for uploading a file to a folder.
+
+        Args:
+            file (str): the filename from the file to be uploaded.
+            folder_name (str): the name of the folder on SharePoint.
+            overwrite (bool, optional): whether to overwrite the file if it already exists. Defaults to False.
+
+        Returns:
+            any: the response from the server.
+        """
+        conn = self._auth()
+        target_folder_url = f'/sites/{folder_name}'
+        input(target_folder_url)
+        file_info = FileCreationInformation()
+        file_info.content = open(file, 'rb').read()
+        file_info.url = os.path.basename(file)
+        file_info.overwrite = overwrite
+        target_folder = conn.web.get_folder_by_server_relative_url(target_folder_url)
+        response = target_folder.files.add(file_info).execute_query()
+        return response
```

## Comparing `sharepoint_crud-1.1.dist-info/LICENSE` & `sharepoint_crud-1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sharepoint_crud-1.1.dist-info/METADATA` & `sharepoint_crud-1.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharepoint-crud
-Version: 1.1
+Version: 1.5
 Summary: Library for interacting with SharePoint
 Home-page: https://github.com/almemanuel/sharepoint-crud
 Author: Emanuel Almeida
 Author-email: emanuel.almeida1998@outlook.com
 Keywords: sharepoint office365
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,41 +26,41 @@
 
 ### Improvement
 
 This project is under development, so if you have any suggestions, please let me know:
 
 - [x] Get file content
 - [ ] Search for a file
-- [ ] Upload file
+- [x] Upload file
 - [ ] Edit file
 - [ ] Delete a file
 
 ## 💻 Requeriments
 Before you begin, ensure you have met the following requirements:
 - you have installed a `python 3.8` or higher
 
-## 🚀 Install pypoint
+## 🚀 Install sharepoint-crud
 - run the command: `pip install sharepoint-crud` to activate the virtual environment
 - voilà!
 
 ## ☕ Run
-To run pypoint, you need a sharepoint account. You can instanciate an object with the following parameters:
+To run sharepoint-crud, you need a sharepoint account. You can instanciate an object with the following parameters:
 
 ```python
 from sharepoint-crud import SharePointCrud
 
 sharepoint = SharePointCrud(
   'https://your-site.sharepoint.com/sites/your-library',
   'your-email@your-domain.com',
   'your-password'
 )
 
 ```
 
-Actually, is possible download a file from sharepoint:
+Actually, is possible download and upload file. An example:
 
 ```python
 file_content = sharepoint.get_file('your/folder/to/your/file', 'your-file.file_format')
 
 ```
 An example:
 I have a file `example.csv` in the folder `my_library/Shared Files/my_folder` on SharePoint:
@@ -72,15 +72,15 @@
   'your-email@your-domain.com',
   'your-password'
 ).get_file('my_library/Shared Files/my_folder', 'example.csv')
 ```
 
 ## 📫 Contributing
 
-To contribute to pypoint, follow these steps:
+To contribute to sharepoint-crud, follow these steps:
 1. Fork this repository.
 2. Create a branch: `git checkout -b <branch_name>`.
 3. Make your changes and confirm them: `git commit -m '<commit_message>'`
 4. Send to the original branch: `git push origin <project_name> <location>`
 5. Create the pull request.
 
 Alternatively, consult the GitHub documentation on [creating a pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sharepoint-crud Version: 1.1 Summary: Library for
+Metadata-Version: 2.1 Name: sharepoint-crud Version: 1.5 Summary: Library for
 interacting with SharePoint Home-page: https://github.com/almemanuel/
 sharepoint-crud Author: Emanuel Almeida Author-email:
 emanuel.almeida1998@outlook.com Keywords: sharepoint office365 Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: office365-rest-python-
 client (==2.2.0) # sharepoint-crud ![GitHub repo size](https://img.shields.io/
@@ -11,33 +11,34 @@
 sharepoint-crud?style=for-the-badge) ![GitHub forks](https://img.shields.io/
 github/forks/almemanuel/sharepoint-crud?style=for-the-badge) ![Bitbucket open
 issues](https://img.shields.io/bitbucket/issues/almemanuel/sharepoint-
 crud?style=for-the-badge) ![Bitbucket open pull requests](https://
 img.shields.io/bitbucket/pr-raw/almemanuel/sharepoint-crud?style=for-the-badge)
 > Solution to integrate SharePoint with your Python script ### Improvement This
 project is under development, so if you have any suggestions, please let me
-know: - [x] Get file content - [ ] Search for a file - [ ] Upload file - [ ]
+know: - [x] Get file content - [ ] Search for a file - [x] Upload file - [ ]
 Edit file - [ ] Delete a file ## ð» Requeriments Before you begin, ensure you
 have met the following requirements: - you have installed a `python 3.8` or
-higher ## ð Install pypoint - run the command: `pip install sharepoint-crud`
-to activate the virtual environment - voilÃ ! ## â Run To run pypoint, you
-need a sharepoint account. You can instanciate an object with the following
-parameters: ```python from sharepoint-crud import SharePointCrud sharepoint =
-SharePointCrud( 'https://your-site.sharepoint.com/sites/your-library', 'your-
-email@your-domain.com', 'your-password' ) ``` Actually, is possible download a
-file from sharepoint: ```python file_content = sharepoint.get_file('your/
-folder/to/your/file', 'your-file.file_format') ``` An example: I have a file
-`example.csv` in the folder `my_library/Shared Files/my_folder` on SharePoint:
-```python from sharepoint-crud import SharePointCrud file_content =
-SharePointCrud( 'https://your-site.sharepoint.com/sites/your-library', 'your-
-email@your-domain.com', 'your-password' ).get_file('my_library/Shared Files/
-my_folder', 'example.csv') ``` ## ð« Contributing To contribute to pypoint,
-follow these steps: 1. Fork this repository. 2. Create a branch: `git checkout
--b `. 3. Make your changes and confirm them: `git commit -m ''` 4. Send to the
-original branch: `git push origin ` 5. Create the pull request. Alternatively,
-consult the GitHub documentation on [creating a pull request](https://
-help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-
-a-pull-request). ## ð¤ Colaborators
+higher ## ð Install sharepoint-crud - run the command: `pip install
+sharepoint-crud` to activate the virtual environment - voilÃ ! ## â Run To
+run sharepoint-crud, you need a sharepoint account. You can instanciate an
+object with the following parameters: ```python from sharepoint-crud import
+SharePointCrud sharepoint = SharePointCrud( 'https://your-site.sharepoint.com/
+sites/your-library', 'your-email@your-domain.com', 'your-password' ) ```
+Actually, is possible download and upload file. An example: ```python
+file_content = sharepoint.get_file('your/folder/to/your/file', 'your-
+file.file_format') ``` An example: I have a file `example.csv` in the folder
+`my_library/Shared Files/my_folder` on SharePoint: ```python from sharepoint-
+crud import SharePointCrud file_content = SharePointCrud( 'https://your-
+site.sharepoint.com/sites/your-library', 'your-email@your-domain.com', 'your-
+password' ).get_file('my_library/Shared Files/my_folder', 'example.csv') ``` ##
+ð« Contributing To contribute to sharepoint-crud, follow these steps: 1. Fork
+this repository. 2. Create a branch: `git checkout -b `. 3. Make your changes
+and confirm them: `git commit -m ''` 4. Send to the original branch: `git push
+origin ` 5. Create the pull request. Alternatively, consult the GitHub
+documentation on [creating a pull request](https://help.github.com/en/github/
+collaborating-with-issues-and-pull-requests/creating-a-pull-request). ## ð¤
+Colaborators
 _[_E_m_a_n_u_e_l_'_s_ _p_r_o_f_i_l_e_ _p_h_o_t_o_]
      _EE_mm_aa_nn_uu_ee_ll_ _AA_ll_mm_ee_ii_dd_aa
 ## ð LicenÃ§a This project is under license. See the file [LICENÃA]
 (LICENSE.md) for more details. [â¬ Turn to top](#sharepoint-crud)
```

## Comparing `sharepoint_crud-1.1.dist-info/RECORD` & `sharepoint_crud-1.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sharepoint_crud/__init__.py,sha256=wbWfUY7BX-usnxTvOKCjeHxubHcHAzQ4NBw-VtBqz64,38
-sharepoint_crud/sharepoint.py,sha256=voiJa4BJ1G4A5N0a9ooT5YUIxj7Buj1FoC-_x-IcKwE,1465
-sharepoint_crud-1.1.dist-info/LICENSE,sha256=bHWyNN01z5OOvkkp8RiYvHxmVQfO5hrwlIKwyKbcQNM,1072
-sharepoint_crud-1.1.dist-info/METADATA,sha256=Km-Gv9mXlVB-fgdgk-RZrvIshNqWetZbz3-MS8aZ_RM,3480
-sharepoint_crud-1.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-sharepoint_crud-1.1.dist-info/top_level.txt,sha256=cQjZT_co8HPUiERUai5BU3rwVm8tQDFkqUAleN-JgXU,16
-sharepoint_crud-1.1.dist-info/RECORD,,
+sharepoint_crud/sharepoint.py,sha256=mhhGjdKN_8SBbdecd-ubKJmcT57rGaMOgovZ1noOY6U,3200
+sharepoint_crud-1.5.dist-info/LICENSE,sha256=bHWyNN01z5OOvkkp8RiYvHxmVQfO5hrwlIKwyKbcQNM,1072
+sharepoint_crud-1.5.dist-info/METADATA,sha256=bmCyE0fJ-GGm0sCDAOpeGtNsPehZB8Hf1josAwWoSd4,3509
+sharepoint_crud-1.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+sharepoint_crud-1.5.dist-info/top_level.txt,sha256=cQjZT_co8HPUiERUai5BU3rwVm8tQDFkqUAleN-JgXU,16
+sharepoint_crud-1.5.dist-info/RECORD,,
```

