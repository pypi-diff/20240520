# Comparing `tmp/gitsint-0.1.0.tar.gz` & `tmp/gitsint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitsint-0.1.0.tar", max compression
+gzip compressed data, was "gitsint-0.1.1.tar", max compression
```

## Comparing `gitsint-0.1.0.tar` & `gitsint-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1066 2024-05-20 15:53:16.177005 gitsint-0.1.0/LICENSE
--rw-r--r--   0        0        0    35149 2024-05-19 09:46:11.286809 gitsint-0.1.0/LICENSE.md
--rw-r--r--   0        0        0        0 2024-05-20 17:04:34.870616 gitsint-0.1.0/README.md
--rw-r--r--   0        0        0    12459 2024-05-20 15:53:16.177005 gitsint-0.1.0/gitsint/__init__.py
--rw-r--r--   0        0        0      266 2024-05-19 09:46:11.286809 gitsint-0.1.0/gitsint/instruments.py
--rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.1.0/gitsint/modules/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.1.0/gitsint/modules/profile/__init__.py
--rw-r--r--   0        0        0     2526 2024-05-20 11:05:48.441921 gitsint-0.1.0/gitsint/modules/profile/friends.py
--rw-r--r--   0        0        0      385 2024-05-20 11:05:57.412526 gitsint-0.1.0/gitsint/modules/profile/profile.py
--rw-r--r--   0        0        0        0 2024-05-19 09:46:11.296809 gitsint-0.1.0/gitsint/modules/repos/__init__.py
--rw-r--r--   0        0        0     8601 2024-05-20 15:47:29.310895 gitsint-0.1.0/gitsint/modules/repos/repository.py
--rw-r--r--   0        0        0      770 2024-05-20 17:04:03.473780 gitsint-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 gitsint-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-20 15:53:16.177005 gitsint-0.1.1/LICENSE
+-rw-r--r--   0        0        0    35149 2024-05-19 09:46:11.286809 gitsint-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     4685 2024-05-20 21:27:19.000210 gitsint-0.1.1/README.md
+-rw-r--r--   0        0        0     4685 2024-05-20 21:34:44.671467 gitsint-0.1.1/gitsint/README.md
+-rw-r--r--   0        0        0    12459 2024-05-20 21:33:45.161504 gitsint-0.1.1/gitsint/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-19 09:46:11.286809 gitsint-0.1.1/gitsint/instruments.py
+-rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.1.1/gitsint/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.1.1/gitsint/modules/profile/__init__.py
+-rw-r--r--   0        0        0     2453 2024-05-20 19:54:10.549360 gitsint-0.1.1/gitsint/modules/profile/friends.py
+-rw-r--r--   0        0        0      385 2024-05-20 19:47:09.923659 gitsint-0.1.1/gitsint/modules/profile/profile.py
+-rw-r--r--   0        0        0        0 2024-05-19 09:46:11.296809 gitsint-0.1.1/gitsint/modules/repos/__init__.py
+-rw-r--r--   0        0        0     8601 2024-05-20 15:47:29.310895 gitsint-0.1.1/gitsint/modules/repos/repository.py
+-rw-r--r--   0        0        0      858 2024-05-20 21:35:09.651617 gitsint-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5616 1970-01-01 00:00:00.000000 gitsint-0.1.1/PKG-INFO
```

### Comparing `gitsint-0.1.0/LICENSE` & `gitsint-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.0/LICENSE.md` & `gitsint-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.0/gitsint/__init__.py` & `gitsint-0.1.1/gitsint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 
 DEBUG        = True
 OUTPUT_PATH  = os.path.abspath(os.path.join(os.path.dirname(__file__), "../output"))
 json_data = []
 username_FORMAT = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b'
 
-__version__ = "1.0"
+__version__ = "0.1.0"
 
 
 def import_submodules(package, recursive=True):
     """Get all the Gitint submodules"""
     if isinstance(package, str):
         package = importlib.import_module(package)
     results = {}
@@ -78,15 +78,15 @@
     #TODO
     if(args.cli):
         return
     def print_fancy_credits():
         print('===============================')
         print('        Gitsint Credits        ')
         print('===============================')
-        print('\033[94mGithub: https://github.com/Zerostats/Gitint\033[0m')
+        print('\033[94mGithub: https://github.com/zerostats/gitsint\033[0m')
         print('\033[94mThis tool is made for educational purposes only.\033[0m')
         print('\033[94mDo not use it for illegal purposes.\033[0m')
         print('===============================')
 
     print_fancy_credits()
     
 def fetch_user(username: str,args) -> str:
@@ -301,21 +301,19 @@
                     help="Create a JSON with the results")
     parser.add_argument("-T","--timeout", type=int , default=10, required=False,dest="timeout",
                     help="Set max timeout value (default 10)")
     parser.add_argument("--cli", default=False, required=False,action="store_true",dest="cli",
                     help="Print the response in JSON format")
     parser.add_argument("--clean", default=False, required=False,action="store_true",dest="cli",
                     help="Print the response in JSON format")
-    #check_update()
+    check_update()
     args = parser.parse_args()
     
-
     credit(args)
     username=args.username[0]
-
     user = fetch_user(username,args)
     if "Error" in user:
         print(colored(user, 'red'))
         exit()
 
 
     # Import Modules
```

### Comparing `gitsint-0.1.0/gitsint/modules/profile/friends.py` & `gitsint-0.1.1/gitsint/modules/profile/friends.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,54 +34,53 @@
         if len(extracted_usernames) == 0:
             break
         usernames.extend(extracted_usernames)
         page_num += 1
     return usernames
 
 
-async def track(user,client,out,args):
+async def track(user,client,out):
     followers_url = f"https://github.com/{user}?tab=followers"
     following_url = f"https://github.com/{user}?tab=following"
 
-    if args.cli == False:
-        print(f"Tracking {user}'s followers and following...")
     followers_usernames = await extract_all_usernames(followers_url,client,out)
     following_usernames = await extract_all_usernames(following_url,client,out)
 
     
     common_usernames =  [user for user in followers_usernames if user in following_usernames]
     
     
 
     return json.dumps(common_usernames)
 
-async def friends(user, client, out,args):
+async def friends(user, client, out, args):
     
     name = "friends"
     domain = "friends"
     method="bs4"
     frequent_rate_limit=True
-    username = user["login"]
-
+    
+    username = user['login']
 
     try:
 
         # TODO if repo > 100
-        usernames = await track(username,client,out,args,)
+        usernames = await track(username,client,out)
         #print(users)
              
         out.append({"name": name,"domain":domain,"method":method,"frequent_rate_limit":frequent_rate_limit,
                     "rateLimit": False,
                     "exists": True,
                     "data": usernames,
                     "others": None,
 
                     })
 
-    except Exception:
+    except Exception as e:
+        print(e)
         
         out.append({"name": name,"domain":domain,"method":method,"frequent_rate_limit":frequent_rate_limit,
                     "rateLimit": False,
                     "exists": False,
                     "data": None,
                     "others": None,
```

### Comparing `gitsint-0.1.0/gitsint/modules/repos/repository.py` & `gitsint-0.1.1/gitsint/modules/repos/repository.py`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.0/pyproject.toml` & `gitsint-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "gitsint"
-version = "0.1.0"
-description = "gitsint allows you to check everything from a github user."
+version = "0.1.1"
+description = "Gitsint allows you to check everything from a github user. It's a powerfull github osint tool"
 authors = ["Zerostats"]
 license = "MIT"
 readme = "README.md"
 
+
 [tool.poetry.dependencies]
 python = "^3.10"
 termcolor = "^2.4.0"
 httpx = "^0.27.0"
 trio = "^0.25.1"
 tqdm = "^4.66.4"
 colorama = "^0.4.6"
@@ -28,12 +29,12 @@
 poethepoet = "^0.26.1"
 
 [tool.poetry.scripts]
 gitsint = "gitsint:main"
 
 
 [tool.poe.tasks]
-docker = "docker build -t gitsint-docker ."
-
+docker = "docker build . -t my-gitsint-image"
+docker-run = "docker run my-gitsint-image gitsint"
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

