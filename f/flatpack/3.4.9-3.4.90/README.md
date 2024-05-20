# Comparing `tmp/flatpack-3.4.9.tar.gz` & `tmp/flatpack-3.4.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.4.9.tar", last modified: Thu May  2 22:54:15 2024, max compression
+gzip compressed data, was "flatpack-3.4.90.tar", last modified: Mon May 20 15:17:09 2024, max compression
```

## Comparing `flatpack-3.4.9.tar` & `flatpack-3.4.90.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.770763 flatpack-3.4.9/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.9/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 22:54:15.770566 flatpack-3.4.9/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-01 14:25:58.000000 flatpack-3.4.9/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.768324 flatpack-3.4.9/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.9/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.9/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.769398 flatpack-3.4.9/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.9/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      796 2024-05-02 08:44:24.000000 flatpack-3.4.9/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.9/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-02 14:38:54.000000 flatpack-3.4.9/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    27166 2024-05-02 17:28:01.000000 flatpack-3.4.9/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.770036 flatpack-3.4.9/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6876 2024-04-27 20:15:24.000000 flatpack-3.4.9/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.9/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.9/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6413 2024-04-27 15:03:11.000000 flatpack-3.4.9/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-02 22:54:15.770307 flatpack-3.4.9/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     6252 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-02 22:54:15.000000 flatpack-3.4.9/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-02 22:54:15.770809 flatpack-3.4.9/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1089 2024-05-02 15:56:21.000000 flatpack-3.4.9/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:17:09.410331 flatpack-3.4.90/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.4.90/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6253 2024-05-20 15:17:09.410045 flatpack-3.4.90/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5422 2024-05-18 05:22:15.000000 flatpack-3.4.90/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:17:09.407365 flatpack-3.4.90/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.4.90/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.4.90/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.4.90/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.4.90/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:17:09.408627 flatpack-3.4.90/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.4.90/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1475 2024-05-20 10:20:46.000000 flatpack-3.4.90/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.4.90/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       52 2024-05-18 04:12:26.000000 flatpack-3.4.90/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.4.90/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    34886 2024-05-20 14:53:14.000000 flatpack-3.4.90/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:17:09.409352 flatpack-3.4.90/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.4.90/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.4.90/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.4.90/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.4.90/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.4.90/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.4.90/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     8543 2024-05-20 15:16:59.000000 flatpack-3.4.90/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-20 15:17:09.409672 flatpack-3.4.90/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6253 2024-05-20 15:17:09.000000 flatpack-3.4.90/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-20 15:17:09.000000 flatpack-3.4.90/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-20 15:17:09.000000 flatpack-3.4.90/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-20 15:17:09.000000 flatpack-3.4.90/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      313 2024-05-20 15:17:09.000000 flatpack-3.4.90/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-20 15:17:09.000000 flatpack-3.4.90/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-20 15:17:09.410391 flatpack-3.4.90/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1090 2024-05-20 15:17:05.000000 flatpack-3.4.90/setup.py
```

### Comparing `flatpack-3.4.9/LICENSE` & `flatpack-3.4.90/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.9/PKG-INFO` & `flatpack-3.4.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.9
+Version: 3.4.90
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
-Requires-Dist: cryptography==42.0.5
+Requires-Dist: cryptography==42.0.6
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: fastapi==0.110.2
 Requires-Dist: hnswlib==0.8.0
 Requires-Dist: httpx==0.27.0
-Requires-Dist: huggingface-hub==0.22.2
-Requires-Dist: llama-cpp-python==0.2.65
+Requires-Dist: huggingface-hub==0.23.0
+Requires-Dist: llama-cpp-python==0.2.75
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: olefile==0.47
 Requires-Dist: psutil==5.9.5
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
```

### Comparing `flatpack-3.4.9/README.md` & `flatpack-3.4.90/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.9/flatpack/agent_manager.py` & `flatpack-3.4.90/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.9/flatpack/datasets.py` & `flatpack-3.4.90/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.9/flatpack/instructions.py` & `flatpack-3.4.90/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.9/flatpack/main.py` & `flatpack-3.4.90/flatpack/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,33 +5,37 @@
 import ngrok
 import os
 import re
 import requests
 import select
 import shlex
 import signal
+import subprocess
 import sys
 import toml
 import uvicorn
+import venv
 
 from .agent_manager import AgentManager
 from cryptography.fernet import Fernet
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
-from fastapi.responses import JSONResponse
+from fastapi.staticfiles import StaticFiles
+from huggingface_hub import snapshot_download
 from importlib.metadata import version
 from .parsers import parse_toml_to_venv_script
 from pathlib import Path
 from sentence_transformers import SentenceTransformer
 from .session_manager import SessionManager
 from typing import List, Optional
 from .vector_manager import VectorManager
 
-CONFIG_FILE_PATH = os.path.join(os.path.expanduser("~"), ".fpk_config.toml")
-KEY_FILE_PATH = os.path.join(os.path.expanduser("~"), ".fpk_encryption_key")
+HOME_DIR = Path.home()
+CONFIG_FILE_PATH = HOME_DIR / ".fpk_config.toml"
+KEY_FILE_PATH = HOME_DIR / ".fpk_encryption_key"
 GITHUB_REPO_URL = "https://api.github.com/repos/romlingroup/flatpack"
 BASE_URL = "https://raw.githubusercontent.com/romlingroup/flatpack/main/warehouse"
 VERSION = version("flatpack")
 
 config = {
     "api_key": None
 }
@@ -40,50 +44,45 @@
 class FPKEncryptionKeyError(Exception):
     """Custom exception for missing encryption key."""
     pass
 
 
 def fpk_build(directory: str):
     """Build a model using a building script from the last unboxed flatpack."""
-    cache_file_path = Path('last_flatpack.cache')
+    cache_file_path = HOME_DIR / ".fpk_unbox.cache"
     print(f"Looking for cached flatpack in {cache_file_path}.")
 
     if directory and fpk_valid_directory_name(directory):
         print(f"Using provided directory: {directory}")
         last_unboxed_flatpack = directory
+        building_script_path = Path(last_unboxed_flatpack) / 'build' / 'build.sh'
     elif cache_file_path.exists():
         print(f"Found cached flatpack in {cache_file_path}.")
         last_unboxed_flatpack = cache_file_path.read_text().strip()
-        if not fpk_valid_directory_name(last_unboxed_flatpack):
-            print(f"❌ Invalid directory name from cache: '{last_unboxed_flatpack}'.")
-            return
+        building_script_path = Path(last_unboxed_flatpack) / 'build' / 'build.sh'
     else:
         print("❌ No cached flatpack found, and no valid directory provided.")
         return
 
-    building_script_path = Path(last_unboxed_flatpack) / 'build' / 'build.sh'
     if not building_script_path.exists():
         print(f"❌ Building script not found in {last_unboxed_flatpack}.")
         return
 
     safe_script_path = shlex.quote(str(building_script_path))
 
     result = os.system(f"bash -u {safe_script_path}")
     if result != 0:
         print("❌ An error occurred while executing the build script.")
     else:
         print("✅ Build script executed successfully.")
 
 
-def fpk_cache_last_flatpack(directory_name: str):
+def fpk_cache_unbox(directory_name: str):
     """Cache the last unboxed flatpack's directory name to a file within the corresponding build directory."""
-    flatpack_dir = Path.cwd()
-    flatpack_dir.mkdir(parents=True, exist_ok=True)
-
-    cache_file_path = flatpack_dir / 'last_flatpack.cache'
+    cache_file_path = HOME_DIR / ".fpk_unbox.cache"
     with open(cache_file_path, 'w') as f:
         f.write(directory_name)
 
 
 def fpk_check_ngrok_auth():
     """Check if the NGROK_AUTHTOKEN environment variable is set."""
     ngrok_auth_token = os.environ.get('NGROK_AUTHTOKEN')
@@ -121,15 +120,15 @@
 
 def fpk_decrypt_data(encrypted_data: str, key: bytes) -> str:
     """Decrypt data using the provided key."""
     fernet = Fernet(key)
     return fernet.decrypt(encrypted_data.encode()).decode()
 
 
-def fpk_display_disclaimer(directory_name: str):
+def fpk_display_disclaimer(directory_name: str, local: bool):
     """Display a disclaimer message with details about a specific flatpack.
 
     Args:
         directory_name (str): Name of the flatpack directory.
     """
     disclaimer_template = """
 -----------------------------------------------------
@@ -151,64 +150,73 @@
 See the License for the specific language governing
 permissions and limitations under the License.
 {please_note}
 To accept, type 'YES'. To decline, type 'NO'.
 -----------------------------------------------------
     """
 
-    please_note_content = """
+    if not local:
+        please_note_content = """
 PLEASE NOTE: The flatpack you are about to unbox is
 governed by its own licenses and terms, separate from
 this software. You may find further details at:
 
 https://fpk.ai/w/{}
-    """.format(directory_name)
+            """.format(directory_name)
+        please_note_colored = fpk_colorize(please_note_content, "yellow")
+    else:
+        please_note_colored = ""
 
-    please_note_colored = fpk_colorize(please_note_content, "yellow")
     print(disclaimer_template.format(please_note=please_note_colored))
 
 
 def fpk_encrypt_data(data: str, key: bytes) -> str:
     """Encrypt data using the provided key."""
     fernet = Fernet(key)
     return fernet.encrypt(data.encode()).decode()
 
 
 def fpk_fetch_flatpack_toml_from_dir(directory_name: str, session: httpx.Client) -> Optional[str]:
     """Fetch the flatpack TOML configuration from a specific directory.
-
     Args:
         directory_name (str): Name of the flatpack directory.
         session (httpx.Client): HTTP client session for making requests.
-
     Returns:
         Optional[str]: The TOML content if found, otherwise None.
     """
     toml_url = f"{BASE_URL}/{directory_name}/flatpack.toml"
-    response = session.get(toml_url)
-    if response.status_code != 200:
+    try:
+        response = session.get(toml_url)
+        if response.status_code != 200:
+            return None
+        return response.text
+    except httpx.HTTPError as e:
+        print(f"❌ Network error occurred: {e}")
         return None
-    return response.text
 
 
 def fpk_fetch_github_dirs(session: httpx.Client) -> List[str]:
     """Fetch a list of directory names from the GitHub repository.
-
     Args:
         session (httpx.Client): HTTP client session for making requests.
-
     Returns:
         List[str]: List of directory names.
     """
-    response = session.get(GITHUB_REPO_URL + "/contents/warehouse")
-    if response.status_code != 200:
-        return ["❌ Error fetching data from GitHub"]
-    directories = [item['name'] for item in response.json() if
-                   item['type'] == 'dir' and item['name'].lower() != 'legacy' and item['name'].lower() != 'template']
-    return sorted(directories)
+    try:
+        response = session.get(GITHUB_REPO_URL + "/contents/warehouse")
+        if response.status_code == 200:
+            directories = [item['name'] for item in response.json() if
+                           item['type'] == 'dir' and item['name'].lower() != 'legacy' and item[
+                               'name'].lower() != 'template']
+            return sorted(directories)
+        else:
+            return ["❌ Error fetching data from GitHub: HTTP Status Code: " + str(response.status_code)]
+    except httpx.HTTPError as e:
+        print(f"❌ Unable to connect to GitHub")
+        sys.exit(1)
 
 
 def fpk_find_models(directory_path: str = None) -> List[str]:
     """Find model files in a specified directory or the current directory.
 
     Args:
         directory_path (Optional[str]): Path to the directory to search in. Defaults to the current directory.
@@ -246,16 +254,15 @@
         print(f"Error decrypting API key: {e}")
 
     return None
 
 
 def fpk_get_last_flatpack(directory_name: str) -> Optional[str]:
     """Retrieve the last unboxed flatpack's directory name from the cache file within the correct build directory."""
-    flatpack_dir = Path.cwd()
-    cache_file_path = flatpack_dir / 'last_flatpack.cache'
+    cache_file_path = HOME_DIR / ".fpk_unbox.cache"
     if cache_file_path.exists():
         return cache_file_path.read_text().strip()
     return None
 
 
 def fpk_get_or_create_encryption_key() -> bytes:
     """Retrieve or generate and save an encryption key."""
@@ -337,57 +344,57 @@
 
 
 def fpk_set_secure_file_permissions(file_path):
     """Set secure file permissions for the specified file."""
     os.chmod(file_path, stat.S_IRUSR | stat.S_IWUSR)
 
 
-def fpk_unbox(directory_name: str, session, verbose: bool = False, local: bool = False):
+def fpk_unbox(directory_name: str, session, local: bool = False):
     """Unbox a flatpack from GitHub or a local directory."""
     flatpack_dir = Path.cwd() / directory_name
-    flatpack_dir.mkdir(parents=True, exist_ok=True)
     build_dir = flatpack_dir / "build"
+
+    if build_dir.exists():
+        print(f"❌ Error: Build directory already exists.")
+        sys.exit(1)
+
+    flatpack_dir.mkdir(parents=True, exist_ok=True)
     build_dir.mkdir(parents=True, exist_ok=True)
 
     temp_toml_path = build_dir / 'temp_flatpack.toml'
-
     if local:
         local_directory_path = flatpack_dir
         toml_path = local_directory_path / 'flatpack.toml'
         if not toml_path.exists():
             print(f"❌ flatpack.toml not found in the specified directory: '{directory_name}'.")
             return
         toml_content = toml_path.read_text()
     else:
         if not fpk_valid_directory_name(directory_name):
             print(f"❌ Invalid directory name: '{directory_name}'.")
             return
-
         toml_content = fpk_fetch_flatpack_toml_from_dir(directory_name, session)
         if not toml_content:
             print(f"❌ Error: Failed to fetch TOML content for '{directory_name}'.")
             return
 
     temp_toml_path.write_text(toml_content)
-
     bash_script_content = parse_toml_to_venv_script(str(temp_toml_path), '3.11.8', directory_name)
     bash_script_path = build_dir / 'flatpack.sh'
     bash_script_path.write_text(bash_script_content)
-
     temp_toml_path.unlink()
 
     print(f"📦 Unboxing {directory_name}...")
     command = f"bash {bash_script_path}"
     result = os.system(command)
-
     if result != 0:
         print("❌ Error: Failed to execute the bash script.")
     else:
-        fpk_cache_last_flatpack(directory_name)
-        print(f"🎉 All done!")
+        fpk_cache_unbox(str(flatpack_dir))
+        print("🎉 All done!")
 
 
 def fpk_valid_directory_name(name: str) -> bool:
     """
     Validate that the directory name contains only alphanumeric characters, dashes, and underscores.
 
     Args:
@@ -408,22 +415,20 @@
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 
-@app.get("/")
-async def landing_page():
-    return JSONResponse(content={"message": "flatpack"})
-
-
-@app.get("/test")
-async def test_endpoint():
-    return JSONResponse(content={"message": "Hello, World!"})
+def setup_static_directory(app, directory: str):
+    if os.path.exists(directory) and os.path.isdir(directory):
+        app.mount("/", StaticFiles(directory=f"{directory}/build", html=True), name="static")
+        print(f"Static files will be served from: {directory}")
+    else:
+        print(f"The directory '{directory}' does not exist or is not a directory.")
 
 
 def setup_arg_parser():
     # Create the top-level parser
     parser = argparse.ArgumentParser(description='Flatpack command line interface')
     subparsers = parser.add_subparsers(dest='command', help='Available commands')
 
@@ -453,66 +458,64 @@
     parser_get_api = api_key_subparsers.add_parser('get', help='Get the current API key')
     parser_get_api.set_defaults(func=lambda args, session: fpk_cli_handle_get_api_key(args, session))
 
     # Unbox commands
     parser_unbox = subparsers.add_parser('unbox', help='Unbox a flatpack from GitHub or a local directory.')
     parser_unbox.add_argument('input', nargs='?', default=None, help='The name of the flatpack to unbox.')
     parser_unbox.add_argument('--local', action='store_true', help='Unbox from a local directory instead of GitHub.')
-    parser_unbox.add_argument('--verbose', action='store_true', help='Display detailed outputs for debugging.')
     parser_unbox.set_defaults(func=lambda args, session: fpk_cli_handle_unbox(args, session))
 
     # Build commands
     parser_build = subparsers.add_parser('build',
                                          help='Build a model using the building script from the last unboxed flatpack.')
     parser_build.add_argument('directory', nargs='?', default=None, help='The directory of the flatpack to build.')
-    parser_build.add_argument('--verbose', action='store_true', help='Display detailed outputs for debugging.')
     parser_build.set_defaults(func=lambda args, session: fpk_cli_handle_build(args, session))
 
     # Run server
     parser_run = subparsers.add_parser('run', help='Run the FastAPI server.')
     parser_run.add_argument('input', nargs='?', default=None, help='The name of the flatpack to run.')
-    parser_run.add_argument('--verbose', action='store_true', help='Display detailed outputs for debugging.')
     parser_run.set_defaults(func=lambda args, session: fpk_cli_handle_run(args, session))
 
     # Vector database management
     parser_vector = subparsers.add_parser('vector', help='Vector database management')
     vector_subparsers = parser_vector.add_subparsers(dest='vector_command')
 
     parser_add_text = vector_subparsers.add_parser('add-texts',
                                                    help='Add new texts to generate embeddings and store them.')
     parser_add_text.add_argument('texts', nargs='+', help='Texts to add.')
     parser_add_text.add_argument('--data-dir', type=str, default='.',
                                  help='Directory path for storing the vector database and metadata files.')
-    parser_add_text.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
+    parser_add_text.set_defaults(func=lambda args, session, vm: fpk_cli_handle_vector_commands(args, session, vm))
 
     parser_search_text = vector_subparsers.add_parser('search-text',
                                                       help='Search for texts similar to the given query.')
     parser_search_text.add_argument('query', help='Text query to search for.')
     parser_search_text.add_argument('--data-dir', type=str, default='.',
                                     help='Directory path for storing the vector database and metadata files.')
-    parser_search_text.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
+    parser_search_text.set_defaults(func=lambda args, session, vm: fpk_cli_handle_vector_commands(args, session, vm))
 
     parser_add_pdf = vector_subparsers.add_parser('add-pdf', help='Add text from a PDF file to the vector database.')
     parser_add_pdf.add_argument('pdf_path', help='Path to the PDF file to add.')
     parser_add_pdf.add_argument('--data-dir', type=str, default='.',
                                 help='Directory path for storing the vector database and metadata files.')
-    parser_add_pdf.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
+    parser_add_pdf.set_defaults(func=lambda args, session, vm: fpk_cli_handle_vector_commands(args, session, vm))
 
     parser_add_url = vector_subparsers.add_parser('add-url', help='Add text from a URL to the vector database.')
     parser_add_url.add_argument('url', help='URL to add.')
     parser_add_url.add_argument('--data-dir', type=str, default='.',
                                 help='Directory path for storing the vector database and metadata files.')
-    parser_add_url.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
+    parser_add_url.set_defaults(func=lambda args, session, vm: fpk_cli_handle_vector_commands(args, session, vm))
 
     parser_add_wikipedia_page = vector_subparsers.add_parser('add-wikipedia',
                                                              help='Add text from a Wikipedia page to the vector database.')
     parser_add_wikipedia_page.add_argument('page_title', help='The title of the Wikipedia page to add.')
     parser_add_wikipedia_page.add_argument('--data-dir', type=str, default='.',
                                            help='Directory path for storing the vector database and metadata files.')
-    parser_add_wikipedia_page.set_defaults(func=lambda args, session: fpk_cli_handle_vector_commands(args, session))
+    parser_add_wikipedia_page.set_defaults(
+        func=lambda args, session, vm: fpk_cli_handle_vector_commands(args, session, vm))
 
     # Add commands for agents
     parser_agents = subparsers.add_parser('agents', help='Manage agents')
     agent_subparsers = parser_agents.add_subparsers(dest='agent_command', help='Available agent commands')
 
     # Add command to spawn an agent
     parser_spawn = agent_subparsers.add_parser('spawn', help='Spawn a new agent with a script')
@@ -524,14 +527,21 @@
     parser_list.set_defaults(func=fpk_cli_handle_list_agents)
 
     # Add command to terminate an agent
     parser_terminate = agent_subparsers.add_parser('terminate', help='Terminate an active agent')
     parser_terminate.add_argument('pid', type=int, help='Process ID of the agent to terminate')
     parser_terminate.set_defaults(func=fpk_cli_handle_terminate_agent)
 
+    # Model compression
+    parser_compress = subparsers.add_parser('compress', help='Compress a model for deployment.')
+    parser_compress.add_argument('model_id', type=str,
+                                 help='The name of the Hugging Face repository (format: username/repo_name).')
+    parser_compress.add_argument('--token', type=str, help='Hugging Face token for private repositories.', default=None)
+    parser_compress.set_defaults(func=lambda args, session: fpk_cli_handle_compress(args, session))
+
     return parser
 
 
 def fpk_cli_handle_add_pdf(pdf_path, vm):
     if not os.path.exists(pdf_path):
         print(f"❌ PDF file does not exist: '{pdf_path}'.")
         return
@@ -552,14 +562,154 @@
 
 
 def fpk_cli_handle_build(args, session):
     directory_name = args.directory
     fpk_build(directory_name)
 
 
+def create_venv(venv_dir):
+    subprocess.run(["python3", "-m", "venv", venv_dir])
+
+
+def fpk_cli_handle_compress(args, session):
+    model_id = args.model_id
+    token = args.token
+
+    if not re.match(r'^[\w-]+/[\w.-]+$', model_id):
+        print("❌ Please specify a valid Hugging Face repository in the format 'username/repo_name'.")
+        return
+
+    repo_name = model_id.split('/')[-1]
+    local_dir = repo_name
+
+    if os.path.exists(local_dir):
+        print(f"📂 The model '{model_id}' is already downloaded in the directory '{local_dir}'.")
+    else:
+        try:
+            if token:
+                print(f"📥 Downloading private model '{model_id}' with provided token...")
+                snapshot_download(repo_id=model_id, local_dir=local_dir, revision="main", token=token)
+            else:
+                print(f"📥 Downloading public model '{model_id}'...")
+                snapshot_download(repo_id=model_id, local_dir=local_dir, revision="main")
+            print(f"🤗 Finished downloading {model_id} into the directory '{local_dir}'")
+        except Exception as e:
+            print(f"❌ Failed to download the model. Please check your internet connection and try again. Error: {e}")
+            return
+
+    llama_cpp_dir = "llama.cpp"
+    ready_file = os.path.join(llama_cpp_dir, "ready")
+    venv_dir = os.path.join(llama_cpp_dir, "venv")
+    venv_activate = os.path.join(venv_dir, "bin", "activate")
+    requirements_file = os.path.join(llama_cpp_dir, "requirements.txt")
+
+    if not os.path.exists(llama_cpp_dir):
+        try:
+            print(f"📥 Cloning llama.cpp repository...")
+            clone_result = subprocess.run(["git", "clone", "https://github.com/ggerganov/llama.cpp", llama_cpp_dir])
+            if clone_result.returncode != 0:
+                print(
+                    "❌ Failed to clone the llama.cpp repository. Please check your internet connection and try again.")
+                return
+            print(f"📥 Finished cloning llama.cpp repository into '{llama_cpp_dir}'")
+        except Exception as e:
+            print(f"❌ Failed to clone the llama.cpp repository. Error: {e}")
+            return
+
+    if not os.path.exists(ready_file):
+        try:
+            print(f"🔨 Running 'make' in the llama.cpp directory...")
+            make_result = subprocess.run(["make"], cwd=llama_cpp_dir)
+            if make_result.returncode != 0:
+                print(f"❌ Failed to run 'make' in the llama.cpp directory. Please check the logs for more details.")
+                return
+            print(f"🔨 Finished running 'make' in the llama.cpp directory")
+
+            if not os.path.exists(venv_dir):
+                print(f"🐍 Creating virtual environment in '{venv_dir}'...")
+                create_venv(venv_dir)
+                print(f"🐍 Virtual environment created.")
+            else:
+                print(f"📂 Virtual environment already exists in '{venv_dir}'")
+
+            print(f"📦 Installing llama.cpp dependencies in virtual environment...")
+            pip_result = subprocess.run([f"source {venv_activate} && pip install -r {requirements_file}"], shell=True,
+                                        executable="/bin/bash")
+            if pip_result.returncode != 0:
+                print(f"❌ Failed to install dependencies. Please check the logs for more details.")
+                return
+            print(f"📦 Finished installing llama.cpp dependencies")
+
+            with open(ready_file, 'w') as f:
+                f.write("Ready")
+        except Exception as e:
+            print(f"❌ An error occurred during the setup of llama.cpp. Error: {e}")
+            return
+
+    output_file = f"{local_dir}/{repo_name}-fp16.bin"
+    quantized_output_file = f"{local_dir}/{repo_name}-Q4_K_M.gguf"
+    outtype = "f16"
+
+    if not os.path.exists(output_file):
+        try:
+            print(f"🛠 Converting the model using llama.cpp...")
+            convert_result = subprocess.run(
+                [
+                    f"source {venv_activate} && python {os.path.join(llama_cpp_dir, 'convert-hf-to-gguf.py')} {local_dir} --outfile {output_file} --outtype {outtype}"
+                ],
+                shell=True, executable="/bin/bash"
+            )
+
+            if convert_result.returncode == 0:
+                print(f"✅ Conversion complete. The model has been compressed and saved as '{output_file}'.")
+            else:
+                print(f"❌ Conversion failed. Please check the logs for more details.")
+                return
+        except Exception as e:
+            print(f"❌ An error occurred during the model conversion. Error: {e}")
+            return
+    else:
+        print(f"📂 The model has already been converted and saved as '{output_file}'.")
+
+    if os.path.exists(output_file):
+        try:
+            print(f"🛠 Quantizing the model...")
+            quantize_command = f"./{llama_cpp_dir}/quantize {output_file} {quantized_output_file} Q4_K_M"
+            quantize_result = subprocess.run(quantize_command, shell=True, executable="/bin/bash")
+
+            if quantize_result.returncode == 0:
+                print(f"✅ Quantization complete. The quantized model has been saved as '{quantized_output_file}'.")
+                print(f"🗑 Deleting the original .bin file '{output_file}'...")
+                os.remove(output_file)
+                print(f"🗑 Deleted the original .bin file '{output_file}'.")
+            else:
+                print(f"❌ Quantization failed. Please check the logs for more details.")
+        except Exception as e:
+            print(f"❌ An error occurred during the quantization process. Error: {e}")
+    else:
+        print(f"❌ The original model file '{output_file}' does not exist.")
+
+    if os.path.exists(quantized_output_file):
+        try:
+            print(f"🧪 Testing the quantized model with inference...")
+
+            test_command = f"./{llama_cpp_dir}/main -m {quantized_output_file} -p 'Write a two-line poem about rain.'"
+            test_result = subprocess.run([f"source {venv_activate} && {test_command}"], shell=True,
+                                         executable="/bin/bash", capture_output=True, text=True)
+
+            if test_result.returncode == 0:
+                print(f"✅ Inference test passed. The quantized model is working correctly.")
+                print(test_result.stdout)
+            else:
+                print(f"❌ Inference test failed. Please check the logs for more details.")
+                print(test_result.stderr)
+        except Exception as e:
+            print(f"❌ An error occurred during the inference test. Error: {e}")
+
+
 def fpk_cli_handle_find(args, session):
     print(fpk_find_models())
 
 
 def fpk_cli_handle_get_api_key(args, session):
     print("Retrieving API key...")
     print(fpk_get_api_key())
@@ -581,22 +731,26 @@
 
 
 def fpk_cli_handle_run(args, session):
     if not args.input:
         print("❌ Please specify a flatpack for the run command.")
         return
 
-    directory_name = args.input
-    existing_dirs = fpk_fetch_github_dirs(session)
+    directory = args.input
 
-    if directory_name not in existing_dirs:
-        print(f"❌ The flatpack '{directory_name}' does not exist.")
+    if os.path.exists(directory) and os.path.isdir(directory):
+        print(f"Using provided flatpack: {directory}")
+    else:
+        print(f"❌ The flatpack '{directory}' does not exist.")
         return
 
     fpk_check_ngrok_auth()
+
+    setup_static_directory(app, directory)
+
     try:
         port = 8000
         listener = ngrok.forward(port, authtoken_from_env=True)
         print(f"Ingress established at {listener.url()}")
         uvicorn.run(app, host="0.0.0.0", port=port)
     except KeyboardInterrupt:
         print("❌ FastAPI server has been stopped.")
@@ -648,19 +802,22 @@
     if not args.input:
         print("❌ Please specify a flatpack for the unbox command.")
         return
 
     directory_name = args.input
     existing_dirs = fpk_fetch_github_dirs(session)
 
-    if directory_name not in existing_dirs:
+    if directory_name not in existing_dirs and not args.local:
         print(f"❌ The flatpack '{directory_name}' does not exist.")
         return
 
-    fpk_display_disclaimer(directory_name)
+    if args.local:
+        fpk_display_disclaimer(directory_name, local=True)
+    else:
+        fpk_display_disclaimer(directory_name, local=False)
 
     while True:
         user_response = input().strip().upper()
         if user_response == "YES":
             break
         elif user_response == "NO":
             print("❌ Installation aborted by user.")
@@ -674,27 +831,29 @@
             print(f"❌ Local directory does not exist: '{directory_name}'.")
             return
         toml_path = local_directory_path / 'flatpack.toml'
         if not toml_path.exists():
             print(f"❌ flatpack.toml not found in the specified directory: '{directory_name}'.")
             return
 
-    print("Verbose mode:", args.verbose)
     print(f"✅ Directory name resolved to: '{directory_name}'")
-    fpk_unbox(directory_name, session, verbose=args.verbose, local=args.local)
+    fpk_unbox(directory_name, session, local=args.local)
 
 
 def fpk_cli_handle_version(args, session):
     print(VERSION)
 
 
-def fpk_cli_handle_vector_commands(args, session):
-    print("Handling vector commands...")
+def fpk_initialize_vector_manager(args):
+    # Initialize VectorManager once
+    return VectorManager(model_id='all-MiniLM-L6-v2', directory=getattr(args, 'data_dir', '.'))
+
 
-    vm = VectorManager(model_name='all-MiniLM-L6-v2', directory=getattr(args, 'data_dir', '.'))
+def fpk_cli_handle_vector_commands(args, session, vm):
+    print("Handling vector commands...")
 
     if args.vector_command == 'add-texts':
         vm.add_texts(args.texts, "manual")
         print(f"Added {len(args.texts)} texts to the database.")
     elif args.vector_command == 'search-text':
         results = vm.search_vectors(args.query)
         if results:
@@ -715,16 +874,19 @@
 def main():
     """Main entry point for the flatpack command line interface."""
     try:
         with SessionManager() as session:
             parser = setup_arg_parser()
             args = parser.parse_args()
 
+            # Initialize VectorManager once
+            vm = fpk_initialize_vector_manager(args)
+
             if hasattr(args, 'func'):
-                args.func(args, session)
+                args.func(args, session, vm)
             else:
                 parser.print_help()
 
     except Exception as e:
         print(f"❌ An unexpected error occurred: {e}")
         sys.exit(1)
```

### Comparing `flatpack-3.4.9/flatpack/modules/lstm.py` & `flatpack-3.4.90/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.9/flatpack/modules/rnn.py` & `flatpack-3.4.90/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.9/flatpack/parsers.py` & `flatpack-3.4.90/flatpack/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,47 +87,55 @@
 handle_error() {{
     echo "😟 Oops! Something went wrong."
     exit 1
 }}
 
 if [[ $IS_COLAB -ne 0 ]]; then
     apt install python3.10-venv
-fi  
-    
+fi
+
 echo "🐍 Checking for Python"
-PYTHON_CMD=python
+if [[ -x "$(command -v python3.11)" ]]; then
+    PYTHON_CMD=python3.11
+elif [[ -x "$(command -v python3.10)" ]]; then
+    PYTHON_CMD=python3.10
+elif [[ -x "$(command -v python3)" ]]; then
+    PYTHON_CMD=python3
+else
+    PYTHON_CMD=python
+fi
 
 echo "Python command to be used: $PYTHON_CMD"
 
 echo "🦄 Creating the virtual environment at {env_name}/{build_prefix}"
-    
+
 if ! $PYTHON_CMD -m venv "{env_name}/{build_prefix}"; then
     echo "❌ Failed to create the virtual environment using $PYTHON_CMD"
     handle_error
 else
     echo "✅ Successfully created the virtual environment"
 fi
-    
+
 # Ensuring the VENV_PYTHON path does not begin with a dot and is correctly formed
 export VENV_PYTHON="{env_name}/{build_prefix}/bin/python"
 if [[ -f "$VENV_PYTHON" ]]; then
     echo "✅ VENV_PYTHON is set correctly to $VENV_PYTHON"
     echo "🐍 Checking Python version in the virtual environment..."
     $VENV_PYTHON --version
 else
     echo "❌ VENV_PYTHON is set to $VENV_PYTHON, but this file does not exist"
     handle_error
 fi
-    
+
 # Ensure pip is installed within the virtual environment
 if [ ! -x "$VENV_PYTHON -m pip" ]; then
     echo "Installing pip within the virtual environment..."
     $VENV_PYTHON -m ensurepip
 fi
-    
+
 # Set VENV_PIP variable to the path of pip within the virtual environment
 export VENV_PIP="$VENV_PYTHON -m pip"
     """
     script.append(venv_setup)
 
     # Create other directories within the build directory as per the TOML configuration
     directories_map = config.get("directories")
@@ -146,15 +154,15 @@
     if package_list:
         script.append(f"$VENV_PIP install {' '.join(package_list)}")
 
     # Clone required git repositories
     for git in config.get("git", []):
         from_source, to_destination, branch = git.get("from_source"), git.get("to_destination"), git.get("branch")
         if from_source and to_destination and branch:
-            repo_path = f"{model_name}/{build_prefix}/{to_destination.replace('/home/content/', '')}"
+            repo_path = f"{model_name}/{build_prefix}/{to_destination}"
             git_clone = f"""
 echo "Cloning repository from: {from_source}"
 git clone -b {branch} {from_source} {repo_path}
 if [ $? -eq 0 ]; then
     echo "Git clone was successful."
 else
     echo "Git clone failed."
@@ -169,24 +177,26 @@
             """.strip()
             script.append(git_clone)
 
     # Download datasets or files
     for item_type in ["dataset", "file"]:
         for item in config.get(item_type, []):
             from_source, to_destination = item.get("from_source"), item.get("to_destination")
+
             if from_source and to_destination:
+
                 if is_url(from_source):
-                    download_command = f"curl -L {from_source} -o ./{model_name}/{build_prefix}/{to_destination.replace('/home/content/', '')}"
+                    download_command = f"curl -s -L {from_source} -o ./{model_name}/{build_prefix}/{to_destination}"
                     script.append(download_command)
                 else:
-                    download_command = f"cp -r .{from_source} ./{model_name}/{build_prefix}/{to_destination.replace('/home/content/', '')}"
+                    download_command = f"cp -r ./{model_name}/{from_source} ./{model_name}/{build_prefix}/{to_destination}"
                     script.append(download_command)
 
     # Execute specified run commands
     run_vec = config.get("run", [])
     for run in run_vec:
-        command, args = run.get("command"), run.get("args")
-        if command and args:
-            replaced_args = args.replace("/home/content/", f"./{model_name}/{build_prefix}/")
-            script.append(f"{command} {replaced_args}")
+        command, file = run.get("command"), run.get("file")
+        if command and file:
+            prepended_file = f"./{model_name}/{build_prefix}/" + file
+            script.append(f"{command} {prepended_file}")
 
     return "\n".join(script)
```

### Comparing `flatpack-3.4.9/flatpack.egg-info/PKG-INFO` & `flatpack-3.4.90/flatpack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.4.9
+Version: 3.4.90
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
-Requires-Dist: cryptography==42.0.5
+Requires-Dist: cryptography==42.0.6
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: fastapi==0.110.2
 Requires-Dist: hnswlib==0.8.0
 Requires-Dist: httpx==0.27.0
-Requires-Dist: huggingface-hub==0.22.2
-Requires-Dist: llama-cpp-python==0.2.65
+Requires-Dist: huggingface-hub==0.23.0
+Requires-Dist: llama-cpp-python==0.2.75
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: olefile==0.47
 Requires-Dist: psutil==5.9.5
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
```

### Comparing `flatpack-3.4.9/flatpack.egg-info/SOURCES.txt` & `flatpack-3.4.90/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.4.9/setup.py` & `flatpack-3.4.90/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.4.9",
+    version="3.4.90",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
-        "cryptography==42.0.5",
+        "cryptography==42.0.6",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.2",
         "hnswlib==0.8.0",
         "httpx==0.27.0",
-        "huggingface-hub==0.22.2",
-        "llama-cpp-python==0.2.65",
+        "huggingface-hub==0.23.0",
+        "llama-cpp-python==0.2.75",
         "ngrok==1.2.0",
         "nltk==3.8.1",
         "olefile==0.47",
         "psutil==5.9.5",
         "pydantic==2.7.1",
         "pypdf==4.2.0",
         "requests==2.31.0",
```

