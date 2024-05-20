# Comparing `tmp/mediumroast_py-0.6.1.tar.gz` & `tmp/mediumroast_py-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediumroast_py-0.6.1.tar", max compression
+gzip compressed data, was "mediumroast_py-0.6.2.tar", max compression
```

## Comparing `mediumroast_py-0.6.1.tar` & `mediumroast_py-0.6.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    11357 2022-07-26 03:31:36.080868 mediumroast_py-0.6.1/LICENSE
--rw-r--r--   0        0        0     2458 2024-05-05 21:42:42.608247 mediumroast_py-0.6.1/README.md
--rwxr-xr-x   0        0        0        0 2022-07-26 03:31:36.083900 mediumroast_py-0.6.1/mediumroast_py/__init__.py
--rwxr-xr-x   0        0        0        0 2022-07-26 03:31:36.083981 mediumroast_py-0.6.1/mediumroast_py/api/__init__.py
--rw-r--r--   0        0        0     6987 2024-05-05 17:08:08.184732 mediumroast_py-0.6.1/mediumroast_py/api/authorize.py
--rw-r--r--   0        0        0    28700 2024-05-06 00:17:34.882274 mediumroast_py-0.6.1/mediumroast_py/api/github.py
--rw-r--r--   0        0        0    22641 2024-05-05 23:26:51.007155 mediumroast_py-0.6.1/mediumroast_py/api/github_server.py
--rw-r--r--   0        0        0      956 2024-05-06 00:21:30.162814 mediumroast_py-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 mediumroast_py-0.6.1/setup.py
--rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 mediumroast_py-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-26 03:31:36.080868 mediumroast_py-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2458 2024-05-05 21:42:42.608247 mediumroast_py-0.6.2/README.md
+-rwxr-xr-x   0        0        0        0 2022-07-26 03:31:36.083900 mediumroast_py-0.6.2/mediumroast_py/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-07-26 03:31:36.083981 mediumroast_py-0.6.2/mediumroast_py/api/__init__.py
+-rw-r--r--   0        0        0     8285 2024-05-16 03:48:03.303403 mediumroast_py-0.6.2/mediumroast_py/api/authorize.py
+-rw-r--r--   0        0        0    39540 2024-05-19 23:40:38.833396 mediumroast_py-0.6.2/mediumroast_py/api/github.py
+-rw-r--r--   0        0        0    22452 2024-05-20 00:28:01.330278 mediumroast_py-0.6.2/mediumroast_py/api/github_server.py
+-rw-r--r--   0        0        0      270 2024-05-19 23:48:07.744829 mediumroast_py-0.6.2/mediumroast_py/api/messages.json
+-rw-r--r--   0        0        0      956 2024-05-15 01:22:04.558727 mediumroast_py-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 mediumroast_py-0.6.2/setup.py
+-rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 mediumroast_py-0.6.2/PKG-INFO
```

### Comparing `mediumroast_py-0.6.1/LICENSE` & `mediumroast_py-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mediumroast_py-0.6.1/README.md` & `mediumroast_py-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mediumroast_py-0.6.1/mediumroast_py/api/authorize.py` & `mediumroast_py-0.6.2/mediumroast_py/api/authorize.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,17 @@
             A dictionary containing environment variables.
         client_type : str, optional
             The type of the client ('github-app' by default).
         """
         self.env = env
         self.client_type = client_type
         self.client_id = env['clientId']
+        self.app_id = env['appId']
+        self.installation_id = env['installationId']
+        self.secret_file = env['secretFile']
         self.device_code = None
 
     def get_access_token_device_flow(self):
         """
         Gets an access token using the device flow.
 
         The method sends a POST request to 'https://github.com/login/device/code' to get the device and user codes.
@@ -59,16 +62,15 @@
         Returns
         -------
         dict
             A dictionary containing the access token and its expiration time.
         """
         # Request device and user codes
         response = requests.post('https://github.com/login/device/code', data={
-            'client_id': self.client_id,
-            # 'scope': 'repo'
+            'client_id': self.client_id
         })
         response.raise_for_status()
         data = parse_qs(response.content.decode())
 
         # Open the verification URL in the user's browser
         print(f"Opening browser with: {data['verification_uri'][0]}")
         webbrowser.open(data['verification_uri'][0])
@@ -117,63 +119,99 @@
         with open(pat_file_path, 'r') as file:
             pat = file.read().strip()
         # Set the expiration time to a far future date
         expires_at = float('inf')
 
         return {'token': pat, 'expires_at': expires_at, 'auth_type': 'pat'}
 
-    def get_access_token_pem(self, pem_file_path, app_id, installation_id):
+    def get_access_token_pem(self):
         """
         Get an installation access token using a PEM file.
 
-        Parameters
-        ----------
-        pem_file_path : str
-            The path to the PEM file.
-        app_id : str
-            The App ID.
-        installation_id : str
-            The installation ID.
-
         Returns
         -------
         str
             The installation access token.
         """
         # Load the private key
-        private_key = Path(pem_file_path).read_text()
+        private_key = Path(self.secret_file).read_text()
 
         # Generate the JWT
         payload = {
             # issued at time
             'iat': int(time.time()),
             # JWT expiration time (10 minute maximum)
             'exp': int(time.time()) + (10 * 60),
             # GitHub App's identifier
-            'iss': app_id
+            'iss': self.app_id
         }
         jwt_token = jwt.encode(payload, private_key, algorithm='RS256')
 
         # Create the headers to include in the request
         headers = {
             'Authorization': f'Bearer {jwt_token}',
             'Accept': 'application/vnd.github.v3+json'
         }
 
         # Make the request to generate the installation access token
         response = requests.post(
-            f'https://api.github.com/app/installations/{installation_id}/access_tokens', headers=headers)
+            f'https://api.github.com/app/installations/{self.installation_id}/access_tokens', headers=headers)
         response.raise_for_status()
 
         # Extract the token and its expiration time from the response
         token_data = response.json()
         token = token_data['token']
         expires_at = token_data['expires_at']
 
         return {'token': token, 'expires_at': expires_at, 'auth_type': 'pem'}
+    
+
+    def get_access_token_client_secret(self, client_id, client_secret):
+        """
+        Get an access token using a client secret.
+
+        Parameters
+        ----------
+        client_secret : str
+            The client secret.
+        client_id : str
+            The client ID.
+
+        Returns
+        -------
+        dict
+            A dictionary containing the access token and its expiration time.
+        """
+        return [False, f'initial implementation completed but unconfirmed, untested and unsupported', None]
+        # The URL of the token endpoint
+        url = "https://github.com/login/oauth/access_token"
+
+        # The data to send in the POST request
+        data = {
+            "client_id": client_id,
+            "client_secret": client_secret,
+            "code": "authorization_code",  # Replace with your actual authorization code
+        }
+
+        # Make the POST request
+        response = requests.post(url, data=data)
+
+        # Check the response
+        if response.status_code == 200:
+            # Parse the response as JSON
+            token_info = response.json()
+
+            # Return the access token and its expiration time
+            return {
+                "access_token": token_info["access_token"],
+                "expires_in": token_info["expires_in"],
+            }
+        else:
+            # If the request failed, raise an exception
+            response.raise_for_status()
 
     def check_and_refresh_token(self, token_info):
         """
         Check the expiration of the access token and regenerate it if necessary.
 
         Parameters
         ----------
```

### Comparing `mediumroast_py-0.6.1/mediumroast_py/api/github.py` & `mediumroast_py-0.6.2/mediumroast_py/api/github.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from github import Github
 import base64
 import json
 import time
 import requests
+import urllib.parse
 from requests.auth import HTTPBasicAuth
+from datetime import datetime
+from pprint import pprint
 
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright (C) 2024 Mediumroast, Inc."
 __author__ = "Michael Hay"
 __email__ = "hello@mediumroast.io"
 __status__ = "Production"
 
@@ -160,35 +163,56 @@
             if response.status_code == 200:
                 return [True, 'SUCCESS: able to capture actions billings info', response.json()]
             else:
                 return [False, f'ERROR: unable to capture actions billings info due to [{response.status_code}]', None]
         except Exception as e:
             return [False, f'ERROR: unable to capture actions billings info due to [{str(e)}]', str(e)]
 
+    # def get_storage_billings(self):
+    #     """
+    #     Get the storage billings information for the organization.
+
+    #     Returns
+    #     -------
+    #     list
+    #         A list containing a boolean indicating success or failure, a status message, and the storage billings information as a dictionary (or the error message in case of failure).
+        # """
+        # return [False, f'initial port completed but implementation unconfirmed, untested and unsupported', None]
+        # try:
+        #     url = f"https://api.github.com/orgs/{self.org_name}/settings/billing/shared-storage"
+        #     response = requests.get(url, auth=HTTPBasicAuth(self.username, self.token))
+
+        #     if response.status_code == 200:
+        #         return [True, 'SUCCESS: able to capture storage billings info', response.json()]
+        #     else:
+        #         return [False, f'ERROR: unable to capture storage billings info due to [{response.status_code}]', None]
+        # except Exception as e:
+        #     return [False, f'ERROR: unable to capture storage billings info due to [{str(e)}]', str(e)]
+        # Create a python function that talks directly to the GitHub API to get the storage billings information
     def get_storage_billings(self):
         """
         Get the storage billings information for the organization.
 
         Returns
         -------
         list
             A list containing a boolean indicating success or failure, a status message, and the storage billings information as a dictionary (or the error message in case of failure).
         """
-        return [False, f'initial port completed but implementation unconfirmed, untested and unsupported', None]
         try:
             url = f"https://api.github.com/orgs/{self.org_name}/settings/billing/shared-storage"
             response = requests.get(url, auth=HTTPBasicAuth(self.username, self.token))
 
             if response.status_code == 200:
                 return [True, 'SUCCESS: able to capture storage billings info', response.json()]
             else:
                 return [False, f'ERROR: unable to capture storage billings info due to [{response.status_code}]', None]
         except Exception as e:
             return [False, f'ERROR: unable to capture storage billings info due to [{str(e)}]', str(e)]
     
+    
     def get_github_org(self):
         """
         Get the organization's information.
 
         Returns
         -------
         list
@@ -237,22 +261,40 @@
         Returns
         -------
         list
             A list containing a boolean indicating success or failure, a status message, and the pull request's raw data (or the error message in case of failure).
         """
         try:
             repo = self.github_instance.get_repo(f"{self.org_name}/{self.repo_name}")
-            pull = repo.create_pull(title=commit_description, body=commit_description, head=branch_name, base=self.main_branch_name)
+            branch = repo.get_branch(branch_name)
+            pull = repo.create_pull(
+                title=commit_description, 
+                body=commit_description, 
+                head=branch.name,
+                base=self.main_branch_name
+            )
+            pull = repo.get_pull(pull.number)
             if pull.mergeable:
-                pull.merge(commit_message=commit_description)
-                return [True, 'SUCCESS: Pull request created and merged successfully', pull.raw_data]
+                my_merge = pull.merge(commit_message=commit_description)
+                return [
+                    True, 
+                    {'status_code': 200, 'status_msg': f'Operation successful merged branch [{branch.name}] into [{self.main_branch_name}]'}, my_merge.merged
+                ]
             else:
-                return [False, 'FAILED: Pull request not created or merged successfully due to merge conflict', None]
-        except Exception as e:
-            return [False, f"FAILED: Pull request not created or merged successfully due to [{str(e)}]", None]
+                return [
+                    False, 
+                    {'status_code': 420, 'status_msg': 'Pull request cannot be merged into branch [{self.main_branch_name}] current pull state: [{pull.state}].'}, 
+                    pull
+                ]
+        except Exception as e:
+            return [
+                False, 
+                {'status_code': 421, 'status_msg': f"Pull request or branch merge failed due to [{str(e)}]"}, 
+                None
+            ]
         
     def check_for_lock(self, container_name):
         """
         Check if a container is locked.
 
         Parameters
         ----------
@@ -270,14 +312,15 @@
             lock_exists = any(content.path == f"{container_name}/{self.lock_file_name}" for content in contents)
             if lock_exists:
                 return [True, f"container [{container_name}] is locked with lock file [{self.lock_file_name}]", lock_exists]
             else:
                 return [False, f"container [{container_name}] is not locked with lock file [{self.lock_file_name}]", lock_exists]
         except Exception as e:
             return [False, str(e), None]
+        
 
     def lock_container(self, container_name):
         """
         Lock a container by creating a lock file in it.
 
         Parameters
         ----------
@@ -291,18 +334,18 @@
         list
             A list containing a boolean indicating success or failure, a status message, and the lock file's raw data (or the error message in case of failure).
         """
         lock_file = f"{container_name}/{self.lock_file_name}"
         try:
             repo = self.github_instance.get_repo(f"{self.org_name}/{self.repo_name}")
             latest_commit = repo.get_commits()[0]
-            lock_response = repo.create_file(lock_file, f"Locking container [{container_name}]", "", branch=self.main_branch_name)
-            return [True, f"SUCCESS: Locked the container [{container_name}]", lock_response.raw_data]
+            lock_response = repo.create_file(lock_file, f"Locking container [{container_name}] with [{lock_file}].", "", branch=self.main_branch_name)
+            return [True, {"status_code": 200,"status_msg": f"Locked the container [{container_name}]"}, lock_response]
         except Exception as e:
-            return [False, f"FAILED: Unable to lock the container [{container_name}]", str(e)]
+            return [False, {"status_code": 504, "status_msg": f"FAILED: Unable to lock the container [{container_name}]"}, str(e)]
 
     def unlock_container(self, container_name, commit_sha, branch_name=None):
         """
         Unlock a container by deleting the lock file in it.
 
         Parameters
         ----------
@@ -320,19 +363,19 @@
         branch_name = branch_name if branch_name else self.main_branch_name
         lock_exists = self.check_for_lock(container_name)
         if lock_exists[0]:
             try:
                 repo = self.github_instance.get_repo(f"{self.org_name}/{self.repo_name}")
                 file_contents = repo.get_contents(lock_file, ref=branch_name)
                 unlock_response = repo.delete_file(lock_file, f"Unlocking container [{container_name}]", file_contents.sha, branch=branch_name)
-                return [True, f"SUCCESS: Unlocked the container [{container_name}]", unlock_response.raw_data]
+                return [True, {"status_code": 200, "status_msg": f"Unlocked the container [{container_name}]"}, unlock_response]
             except Exception as e:
-                return [False, f"FAILED: Unable to unlock the container [{container_name}]", str(e)]
+                return [False, {"status_code": 504, "status_msg": f"Unable to unlock the container [{container_name}]"}, str(e)]
         else:
-            return [False, f"FAILED: Unable to unlock the container [{container_name}]", None]
+            return [False, {"status_code": 503, "status_msg": f"Unable to unlock the container [{container_name}]"}, None]
         
     def delete_blob(self, container_name, file_name, branch_name, sha):
         """
         Delete a blob (file) in a container (directory) in a specific branch.
 
         Parameters
         ----------
@@ -356,42 +399,57 @@
             file_path = f"{container_name}/{file_name}"
             file_contents = repo.get_contents(file_path, ref=branch_name)
             delete_response = repo.delete_file(file_path, f"Delete object [{file_name}]", file_contents.sha, branch=branch_name)
             return [True, { 'status_code': 200, 'status_msg': f'deleted object [{file_name}] from container [{container_name}]' }, delete_response.raw_data]
         except Exception as e:
             return [False, { 'status_code': 503, 'status_msg': f'unable to delete object [{file_name}] from container [{container_name}]' }, str(e)]
 
-    def read_blob(self, file_name, branch_name='main', sha=None):
+    def read_blob(self, file_name):
         """
         Read a blob (file) from a container (directory) in a specific branch.
 
         Parameters
         ----------
-        container_name : str
-            The name of the container from which to read the blob.
         file_name : str
-            The name of the blob to read.
-        branch_name : str
-            The name of the branch where the blob is located.
-        sha : str, optional
-            The SHA of the blob to read.
+            The name of the blob to read with a complete path to the file (e.g. dirname/filename.ext).
 
         Returns
         -------
         list
             A list containing a boolean indicating success or failure, a status message, and the blob's raw data (or the error message in case of failure).
         """
-        try:
-            repo = self.github_instance.get_repo(f"{self.org_name}/{self.repo_name}")
-            file_path = f"{file_name}"
-            file_contents = repo.get_contents(file_path, ref=branch_name)
-            decoded_content = base64.b64decode(file_contents.content)
-            return [True, f"SUCCESS: read object [{file_name}] from container [{file_name}]", decoded_content]
-        except Exception as e:
-            return [False, f"ERROR: unable to read object [{file_name}].", str(e)] 
+
+        encoded_file_name = urllib.parse.quote(file_name)
+        object_url = f"https://api.github.com/repos/{self.org_name}/{self.repo_name}/contents/{encoded_file_name}"
+        headers = {'Authorization': 'token ' + self.token}
+        try:
+            result = requests.get(object_url, headers=headers)
+            result_json = result.json()
+            download_url = result_json['download_url']
+            download_result = requests.get(download_url)
+            bin_file = download_result.content
+            return [
+                True, 
+                {"status_code": 200, "status_msg": f"read object [{file_name}] from container [{file_name}]"}, 
+                bin_file
+            ]
+        except Exception as e:
+            return [
+                False, 
+                {"status_code": 503, "status_msg": f"unable to read object [{file_name}] due to [{e}]."}, 
+                e
+            ]
+        # NOTE: The code below is the original implementation that doesn't work for larger files
+        # try:
+        #     repo = self.github_instance.get_repo(f"{self.org_name}/{self.repo_name}")
+        #     file_contents = repo.get_contents(file_name, ref=branch_name)
+        #     decoded_content = base64.b64decode(file_contents.content)
+        #     return [True, f"SUCCESS: read object [{file_name}] from container [{file_name}]", decoded_content]
+        # except Exception as e:
+        #     return [False, f"ERROR: unable to read object [{file_name}].", str(e)] 
     
     def write_blob(self, container_name, file_name, blob, branch_name, sha=None):
         """
         Write a blob (file) to a container (directory) in a specific branch.
 
         Parameters
         ----------
@@ -421,15 +479,15 @@
                 write_response = repo.update_file(file_path, f"Update object [{file_name}]", blob, file_contents.sha, branch=branch_name)
             else:
                 write_response = repo.create_file(file_path, f"Create object [{file_name}]", blob, branch=branch_name)
             return [True, f"SUCCESS: wrote object [{file_name}] to container [{container_name}]", write_response.raw_data]
         except Exception as e:
             return [False, f"ERROR: unable to write object [{file_name}] to container [{container_name}]", str(e)]
 
-    def write_object(self, container_name, obj, ref, my_sha):
+    def write_object(self, container_name, obj, ref, sha):
         """
         Write an object to a container in a specific branch.
 
         Parameters
         ----------
         container_name : str
             The name of the container where the object will be written.
@@ -439,23 +497,51 @@
             The name of the branch where the object will be written.
 
         Returns
         -------
         list
             A list containing a boolean indicating success or failure, a status message, and the write response's raw data (or the error message in case of failure).
         """
+        content_to_transmit = json.dumps(obj)
         try:
             repo = self.github_instance.get_repo(f"{self.org_name}/{self.repo_name}")
             file_path = f"{container_name}/{self.object_files[container_name]}"
-            content = base64.b64encode(json.dumps(obj).encode()).decode()
-            file_contents = repo.get_contents(file_path, ref=ref)
-            write_response = repo.update_file(file_path, f"Update object [{self.object_files[container_name]}]", content, file_contents.sha, branch=ref)
-            return [True, f"SUCCESS: wrote object [{self.object_files[container_name]}] to container [{container_name}]", write_response.raw_data]
-        except Exception as e:
-            return [False, f"ERROR: unable to write object [{self.object_files[container_name]}] to container [{container_name}]", str(e)]
+            # file_contents = repo.get_contents(file_path, ref=ref, sha=sha)
+            write_response = repo.update_file(
+                file_path, 
+                f"Update object [{self.object_files[container_name]}]", 
+                content=content_to_transmit,
+                sha=sha, 
+                branch=ref
+            )
+            # NOTICE: github.Repository.Repository.update_file() has a formatting bug in the library the below is the fix
+            # for the bug.  The bug is that the content is not being encoded to bytes before being base64 encoded. If this is
+            # not done the content will be base64 encoded as a string and the file will be corrupted. The version of library needs
+            # to be manually patched to fix this issue.
+            # if not isinstance(content, bytes):
+            #   content = content.encode("utf-8")
+            #   content = b64encode(content).decode("utf-8")
+            return [
+                True, 
+                {
+                    "status_msg": f"wrote object [{self.object_files[container_name]}] to container [{container_name}]",
+                    "status_code": 200 
+                },
+                write_response
+            ]
+        except Exception as e:
+            print(e)
+            return [
+                False, 
+                {
+                    "status_code":f"unable to write object [{self.object_files[container_name]}] to container [{container_name}] due to [{str(e)}]",
+                    "status_msg": 503
+                }, 
+                str(e)
+            ]
         
     def read_objects(self, container_name, branch_name=None):
         """
         Read all objects from a container in a specific branch.
 
         Parameters
         ----------
@@ -471,45 +557,161 @@
         """
         try:
             repo = self.github_instance.get_repo(f"{self.org_name}/{self.repo_name}")
             branch_name = branch_name if branch_name else self.main_branch_name
             file_path = f"{container_name}/{self.object_files[container_name]}"
             file_contents = repo.get_contents(file_path, ref=branch_name)
             decoded_content = base64.b64decode(file_contents.content).decode()
-            return [True, f"SUCCESS: read objects from container [{container_name}]", json.loads(decoded_content)]
+            return [True, f"SUCCESS: read objects from container [{container_name}]", {"mr_json": json.loads(decoded_content), "sha": file_contents.sha}]
         except Exception as e:
             return [False, f"ERROR: unable to read objects from container [{container_name}]", str(e)]
     
-    def update_object(self, container_name, obj, ref):
+
+    def update_object(self, container_name, updates=None, dont_write=False, system=False, white_list=[]):
         """
-        Update an object in a container in a specific branch.
+        Updates an object in a specified container.
 
         Parameters
         ----------
         container_name : str
             The name of the container where the object is located.
-        obj : dict
-            The object to update.
-        branch_name : str
-            The name of the branch where the object is located.
+        obj_name : str
+            The name of the object to update.
+        key : str, optional
+            The key in the object to update. This parameter is ignored if `updates` is provided.
+        value : str, optional
+            The new value to set for the key. This parameter is ignored if `updates` is provided.
+        updates : dict, optional
+            A dictionary of key-value pairs to update in the object. If provided, `key` and `value` are ignored.
+        dont_write : bool, optional
+            If True, the object will not be written back to the container. Default is False.
+        system : bool, optional
+            If True, the function is being called by the system, and will bypass certain checks. Default is False.
+        white_list : list, optional
+            A list of keys that are allowed to be updated. If empty, all keys can be updated. Default is an empty list.
 
         Returns
         -------
         list
-            A list containing a boolean indicating success or failure, a status message, and the update response's raw data (or the error message in case of failure).
+            A list containing a boolean indicating success or failure, and a status message.
         """
-        try:
-            repo = self.github_instance.get_repo(f"{self.org_name}/{self.repo_name}")
-            file_path = f"{container_name}/{self.object_files[container_name]}"
-            content = base64.b64encode(json.dumps(obj).encode()).decode()
-            file_contents = repo.get_contents(file_path, ref=ref)
-            write_response = repo.update_file(file_path, f"Update object [{self.object_files[container_name]}]", content, file_contents.sha, branch=ref)
-            return [True, f"SUCCESS: updated object [{self.object_files[container_name]}] in container [{container_name}]", write_response.raw_data]
-        except Exception as e:
-            return [False, f"ERROR: unable to update object [{self.object_files[container_name]}] in container [{container_name}]", str(e)]
+        
+        # Check to see if this is a system call or not
+        if not system:
+            # Since this is not a system call check to see if the key is in the white list
+            for my_obj in updates.keys():
+                for key in updates[my_obj].keys():
+                    if key not in white_list:
+                        return [
+                            False, 
+                            {
+                                'status_code': 403, 
+                                'status_msg': 'Updating the key [{}] is not supported.'.format(key)
+                            },
+                            None
+                        ]
+        
+        # Read in all objects from the main branch of the container
+        read_response = self.read_objects(container_name)
+        # Check to see if the read was successful
+        if not read_response[0]:
+            return [
+                False,
+                {
+                    'status_code': read_response[1]['status_code'],
+                    'status_msg': 'Failed to read objects from container [{}].'.format(container_name)
+                },
+                None
+            ]
+        
+        # Catch the container for modification
+        repo_metadata = {
+            "containers": {}, 
+            "branch": {}
+        }
+
+        caught = dict()
+        if not dont_write:
+            repo_metadata["containers"][container_name] = {}
+            caught = self.catch_container(repo_metadata)
+            if not caught[0]:
+                return [
+                    False,
+                    {
+                        'status_code': 503,
+                        'status_msg': caught[1]['status_msg']
+                    },
+                    caught
+                ]
+        
+        # Get the object from the read response
+        current_objects = read_response[2]['mr_json']
+        # Loop through the updates, find the object(s) to update, and then perform the updates
+        for my_obj in updates.keys():
+            obj_name = my_obj
+            obj = None
+            # Remove the object from the list of objects so we can add it back later
+            for item in current_objects:
+                if item.get('name') == obj_name:  # assuming 'name' is the relevant key in the dictionaries
+                    obj = item
+                    # Remove object from the list
+                    current_objects.remove(item)
+                    break
+            # Check to see if the object exists
+            if obj is None:
+                return [
+                    False,
+                    {
+                        'status_code': 404,
+                        'status_msg': 'Object [{}] does not exist in container [{}].'.format(obj_name, container_name)
+                    },
+                    None
+                ]
+            # Check to see if we should update the object using the updates dictionary
+            for key, value in updates[my_obj].items():
+                # Update the object
+                obj[key] = value
+                now = datetime.now()
+                obj['modification_date'] = now.isoformat()
+
+            # Append the updated object to the list of objects
+            current_objects.append(obj)
+
+        # Check to see if we should write the updated object back to the container
+        if not dont_write:
+            write_response = self.write_object(
+                container_name, 
+                current_objects,
+                caught[2]['branch']['name'],
+                caught[2]['containers'][container_name]['object_sha']
+            )
+            if not write_response[0]:
+                return [
+                    False,
+                    {
+                        'status_code': write_response[1]['status_code'],
+                        'status_msg': 'Failed to write updated object [{}] to container [{}].'.format(obj_name, container_name)
+                    },
+                    None
+                ]
+        
+        # Release the container
+        released = self.release_container(caught[2], f"Updated [{len(current_objects)}] [{container_name}] objects.")
+        if not released[0]:
+            return [
+                False,
+                {
+                    'status_code': 503,
+                    'status_msg': 'Cannot release the container please check [{}] in GitHub.'.format(container_name)
+                },
+                released
+            ]
+
+        # Return the updated object
+        return [True, {'status_code': 200, 'status_msg': 'Object updated successfully.'}, obj]
 
     def delete_object(self, container_name, file_name, branch_name, sha):
         """
         Delete an object from a container in a specific branch.
 
         Parameters
         ----------
@@ -558,59 +760,99 @@
                 file_path = f"{container_name}/{container_name}.json"
                 response = repo.create_file(file_path, f"Create container [{container_name}]", empty_json)
                 responses.append(response)
             except Exception as e:
                 responses.append(str(e))
         return [all(isinstance(res, Github.GitCommit.GitCommit) for res in responses), responses]
     
-    def catch_container(self, containers=['Studies', 'Companies', 'Interactions']):
+    def catch_container(self, repo_metadata):
         """
         Catch (lock) multiple containers (directories) in the repository.
 
         Parameters
         ----------
-        containers : list, optional
-            The names of the containers to catch, by default ['Studies', 'Companies', 'Interactions'].
+        repo_metadata : dict
+            The metadata of the repository, including the branch name, branch SHA, and container information.
 
         Returns
         -------
         list
-            A list containing a boolean indicating success or failure, and a list of responses for each container catch (or the error message in case of failure).
+            A list containing a boolean indicating success or failure, a dictionary with status code and message, and a list of responses for each container catch (or the error message in case of failure).
         """
-        responses = []
-        for container_name in containers:
-            try:
-                repo = self.github_instance.get_repo(f"{self.org_name}/{self.repo_name}")
-                file_path = f"{container_name}/{container_name}.json"
-                file_contents = repo.get_contents(file_path)
-                decoded_content = base64.b64decode(file_contents.content).decode()
-                responses.append([True, json.loads(decoded_content)])
-            except Exception as e:
-                responses.append([False, str(e)])
-        return responses
+        # Check to see if the containers are locked
+        for container in repo_metadata['containers']:
+            # Call the method above to check for a lock
+            lock_exists = self.check_for_lock(container)
+            # If the lock exists return an error
+            if lock_exists[0]:
+                return [False, {'status_code': 503, 'status_msg': f'the container [{container}] is locked unable and cannot perform creates, updates or deletes on objects.'}, lock_exists]
+
+        # Lock the containers
+        for container in repo_metadata['containers']:
+            # Call the method above to lock the container
+            locked = self.lock_container(container)
+            # Check to see if the container was locked and return the error if not
+            if not locked[0]:
+                return [False, {'status_code': 503, 'status_msg': f'unable to lock [{container}] and cannot perform creates, updates or deletes on objects.'}, locked]
+            # Save the lock sha into containers as a separate object
+            repo_metadata['containers'][container]['lockSha'] = locked[2]['commit'].sha
+
+        # Call the method above create_branch_from_main to create a new branch
+        branch_created = self.create_branch_from_main()
+        # Check to see if the branch was created
+        if not branch_created[0]:
+            return [False, {'status_code': 503, 'status_msg': 'unable to create new branch'}, branch_created]
+        # Save the branch sha into containers as a separate object
+        repo_metadata['branch'] = {
+            'name': branch_created[2]['ref'],
+            'sha': branch_created[2]['object']['sha']
+        }
+
+        # Read the objects from the containers
+        for container in repo_metadata['containers']:
+            # Call the method above to read the objects
+            read_response = self.read_objects(container)
+            # Check to see if the read was successful
+            if not read_response[0]:
+                return [False, {'status_code': 503, 'status_msg': f'Unable to read the source objects [{container}/{self.object_files[container]}].'}, read_response]
+            # Save the object sha into containers as a separate object
+            # repo_metadata['containers'][container]['objectSha'] = read_response[2]['data']['sha']
+            repo_metadata['containers'][container]['object_sha'] = read_response[2]['sha']
+            # Save the objects into containers as a separate object
+            repo_metadata['containers'][container]['objects'] = read_response[2]['mr_json']
+
+        return [True, {'status_code': 200, 'status_msg': f"{len(repo_metadata['containers'])} containers are ready for use."}, repo_metadata]
     
-    def release_container(self, repo_metadata):
+    def release_container(self, repo_metadata, commit_description=None):
         """
         Release (unlock) multiple containers (directories) in the repository.
 
         Parameters
         ----------
-        containers : list, optional
-            The names of the containers to release, by default ['Studies', 'Companies', 'Interactions'].
+        repo_metadata : dict
+            The metadata of the repository, including the branch name, branch SHA, and container information.
 
         Returns
         -------
         list
-            A list containing a boolean indicating success or failure, and a list of responses for each container release (or the error message in case of failure).
+            A list containing a boolean indicating success or failure, a dictionary with status code and message, and a list of responses for each container release (or the error message in case of failure).
         """
+        # Merge the branch to main
+        merge_response = self.merge_branch_to_main(repo_metadata['branch']['name'], commit_description)
+        # Check to see if the merge was successful and return the error if not
+        if not merge_response[0]:
+            return [False, {'status_code': 503, 'status_msg': 'Unable to merge the branch to main.'}, merge_response]
+
+        # Unlock the containers by looping through them
         for container in repo_metadata['containers']:
             # Unlock branch
             branch_unlocked = self.unlock_container(container, repo_metadata['containers'][container]['lockSha'], repo_metadata['branch']['name'])
             if not branch_unlocked[0]:
                 return [False, {'status_code': 503, 'status_msg': f"Unable to unlock the container, objects may have been written please check [{container}] for objects and the lock file."}, branch_unlocked]
             # Unlock main
             main_unlocked = self.unlock_container(container, repo_metadata['containers'][container]['lockSha'])
             if not main_unlocked[0]:
                 return [False, {'status_code': 503, 'status_msg': f"Unable to unlock the container, objects may have been written please check [{container}] for objects and the lock file."}, main_unlocked]
+
         # Return success with number of objects written
         return [True, {'status_code': 200, 'status_msg': f"Released [{len(repo_metadata['containers'])}] containers."}, None]
```

### Comparing `mediumroast_py-0.6.1/mediumroast_py/api/github_server.py` & `mediumroast_py-0.6.2/mediumroast_py/api/github_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,26 +81,24 @@
             A list of all objects to search through. If None, all objects will be retrieved from the GitHub repository.
 
         Returns
         -------
         dict
             The object with the specified attribute value, or None if no such object exists.
         """
-        # if attribute == 'name':
-        #     value = value.lower()
         my_objects = []
         if all_objects is None:
             all_objects_resp = self.server_ctl.read_objects(self.obj_type)
             all_objects = all_objects_resp[2]
         if len(all_objects) == 0:
-            return [False, f"No {self.obj_type} objects found"]
-        for obj in all_objects:
-            if obj.get(attribute) == value:
+            return [False, f"No {self.obj_type} objects found", None]
+        for obj in all_objects['mr_json']:
+            if obj[attribute] == value:
                 my_objects.append(obj)
-        return [True, my_objects]
+        return [True, {'status_code': 200, 'status_msg': 'found objects matching {attribute} = {value}'}, my_objects]
 
     def create_obj(self, objs):
         """
         Create new objects in the GitHub repository.
 
         Parameters
         ----------
@@ -118,15 +116,15 @@
         for obj in objs:
             caught[2]['mrJson'].append(obj)
         released = self.server_ctl.release_container(caught[2])
         if not released[0]:
             return released
         return [True, {'status_code': 200, 'status_msg': f"created [{len(objs)}] {self.obj_type}"}, None]
 
-    def update_obj(self, obj_name, key, value, dont_write=False, system=False, white_list=None):
+    def update_obj(self, updates=None, dont_write=False, system=False, white_list=None):
         """
         Update an object in the GitHub repository.
 
         Parameters
         ----------
         obj_name : str
             The name of the object to update.
@@ -142,15 +140,21 @@
             A list of attributes that are allowed to be updated. If None, all attributes can be updated.
 
         Returns
         -------
         list
             A list containing a boolean indicating success or failure, and a status message.
         """
-        return self.server_ctl.update_object(self.obj_type, obj_name, key, value, dont_write, system, white_list)
+        return self.server_ctl.update_object(
+            self.obj_type, 
+            updates=updates,
+            dont_write=dont_write, 
+            system=system, 
+            white_list=white_list
+        )
 
     def delete_obj(self, obj_name, source, repo_metadata=None, catch_it=True):
         """
         Delete an object from the GitHub repository.
 
         Parameters
         ----------
@@ -561,15 +565,15 @@
         org : str
             The name of the organization on GitHub.
         process_name : str
             The name of the process.
         """
         super().__init__(token, org, process_name, 'Interactions')
 
-    def update_obj(self, obj_to_update, dont_write=False, system=False):
+    def update_obj(self, updates, dont_write=False, system=False):
         """
         Update an interaction object in the GitHub repository.
 
         This method uses the server_ctl attribute to call the update_obj method.
 
         Parameters
         ----------
@@ -581,27 +585,27 @@
             If True, the object will be treated as a system object.
 
         Returns
         -------
         dict
             The updated interaction object.
         """
-        # Destructure obj_to_update
-        name = obj_to_update['name']
-        key = obj_to_update['key']
-        value = obj_to_update['value']
-
         # Define the attributes that can be updated by the user
         white_list = [
             'status', 'content_type', 'file_size', 'reading_time', 'word_count', 'page_count', 'description', 'abstract',
             'region', 'country', 'city', 'state_province', 'zip_postal', 'street_address', 'latitude', 'longitude',
-            'public', 'groups', 'topics', 'tags'
+            'public', 'groups', 'contact_name', 'topics', 'tags'
         ]
 
-        return super().update_obj(name, key, value, dont_write, system, white_list)
+        return super().update_obj(
+            updates=updates,
+            dont_write=dont_write, 
+            system=system, 
+            white_list=white_list
+        )
 
     def delete_obj(self, obj_name):
         """
         Delete an interaction object from the GitHub repository.
 
         This method uses the server_ctl attribute to call the delete_obj method.
 
@@ -636,15 +640,16 @@
         Returns
         -------
         dict
             The interaction object with the specified file hash, or None if no such object exists.
         """
         return self.find_by_x('file_hash', hash)
     
-    def download_interaction_content(self, interaction_name):
+    def download_interaction_content(self, interaction_path):
+        
         """
         Download the file associated with an interaction object.
 
         This method uses the server_ctl attribute to call the download_interaction_file method.
 
         Parameters
         ----------
@@ -652,15 +657,9 @@
             The name of the interaction object.
 
         Returns
         -------
         dict
             The file associated with the interaction object.
         """
-        interaction_response = self.find_by_name(interaction_name)
-        if not interaction_response[0]:
-            return interaction_response
-        else:
-            interaction = interaction_response[1][0]
-            file_url = interaction['url']
-            file_contents = self.server_ctl.read_blob(file_url, 'main')
-            return file_contents
+        file_contents = self.server_ctl.read_blob(interaction_path)
+        return file_contents
```

### Comparing `mediumroast_py-0.6.1/pyproject.toml` & `mediumroast_py-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mediumroast_py"
-version = "0.6.1"
+version = "0.6.2"
 description = "This Python package provides a Software Development Kit (SDK) for interacting with Mediumroast for GitHub. It is used internally by Mediumroast, Inc. and meant for developers to make use of."
 authors = ["Michael Hay <michael.hay@mediumroast.io>"]
 license = "Apache-2.0"
 repository = "https://github.com/mediumroast/mediumroast_py"
 readme = "README.md"
 keywords = ["Product Management", "Competitive Insights", "Customer Insights", "Partner Insights", "Empowered Teams"]
```

### Comparing `mediumroast_py-0.6.1/setup.py` & `mediumroast_py-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'requests>=2.28.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['test = run_tests:main']}
 
 setup_kwargs = {
     'name': 'mediumroast-py',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'This Python package provides a Software Development Kit (SDK) for interacting with Mediumroast for GitHub. It is used internally by Mediumroast, Inc. and meant for developers to make use of.',
     'long_description': "# mediumroast_py\n\n## Introduction\n\nThis Python package provides a Software Development Kit (SDK) for interacting with Mediumroast for GitHub. It is used internally by Mediumroast, Inc. and meant for developers to make use of.\n\n### Notice\nThe SDK is in active development and is subject to change. The SDK is not yet stable and should not be used in production environments. \n\n## Installation\n\nTo install the package, you can use pip:\n\n```bash\npip install mediumroast_py\n```\n\n## Usage\nTo use the package, you will need to import the `mediumroast_py` modules and classes. The package provides three main classes for interacting with objects: `Companies`, `Interactions`, and `Users`.\n\n### Authentication\nTo use the package, you will need to authenticate with the Mediumroast API using the `GitHubAuth` class. Here is an example of how to authenticate with the Mediumroast API using a GitHub App installation and a private key file. You will need to set the `MR_CLIENT_ID`, `MR_APP_ID`, and `YOUR_INSTALLATION_ID` environment variables to the appropriate values for your GitHub App installation. You will also need to set the `YOUR_PEM_FILE` environment variable to the path of your private key file. Here is an example of how to authenticate with the Mediumroast API using a GitHub App installation and a private key file.\n\n```python\nfrom mediumroast_py.api import Companies, Interactions, Users\nfrom mediumroast_py.api.authorize import GitHubAuth\n\nauth = GitHubAuth(env={'clientId': os.getenv('MR_CLIENT_ID')})\ntoken = auth.get_access_token_pem(\n      os.getenv('YOUR_PEM_FILE'), \n      os.getenv('MR_APP_ID'), \n      os.getenv('YOUR_INSTALLATION_ID')\n)\n```\n\n### Companies\nThe `Companies` class provides methods for interacting with companies in Mediumroast. You can use the `get_all` method to get information about all companies.\n\n```python\ncompany_ctl = Companies(token_info['token'], os.getenv('YOUR_ORG') , process_name)\ncompanies = company_ctl.get_all()\n```\n\n### Interactions\nThe `Interactions` class provides methods for interacting with interactions in Mediumroast. You can use the `get_all` method to get information about all interactions.\n\n```python\ninteraction_ctl = Interactions(token_info['token'], os.getenv('YOUR_ORG') , process_name)\ninteractions = interaction_ctl.get_all()\n```\n\n## Issues\nIf you encounter any issues with the SDK, please report them on the [mediumroast_py issues](https://github.com/mediumroast/mediumroast_py/issues) page.\n",
     'author': 'Michael Hay',
     'author_email': 'michael.hay@mediumroast.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mediumroast/mediumroast_py',
```

### Comparing `mediumroast_py-0.6.1/PKG-INFO` & `mediumroast_py-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediumroast-py
-Version: 0.6.1
+Version: 0.6.2
 Summary: This Python package provides a Software Development Kit (SDK) for interacting with Mediumroast for GitHub. It is used internally by Mediumroast, Inc. and meant for developers to make use of.
 Home-page: https://github.com/mediumroast/mediumroast_py
 License: Apache-2.0
 Keywords: Product Management,Competitive Insights,Customer Insights,Partner Insights,Empowered Teams
 Author: Michael Hay
 Author-email: michael.hay@mediumroast.io
 Requires-Python: >=3.8,<4.0
```

