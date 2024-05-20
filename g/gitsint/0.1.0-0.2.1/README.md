# Comparing `tmp/gitsint-0.1.0.tar.gz` & `tmp/gitsint-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitsint-0.1.0.tar", max compression
+gzip compressed data, was "gitsint-0.2.1.tar", max compression
```

## Comparing `gitsint-0.1.0.tar` & `gitsint-0.2.1.tar`

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
+-rw-r--r--   0        0        0     1066 2024-05-20 15:53:16.177005 gitsint-0.2.1/LICENSE
+-rw-r--r--   0        0        0    35149 2024-05-19 09:46:11.286809 gitsint-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     4653 2024-05-20 20:12:14.549993 gitsint-0.2.1/README.md
+-rw-r--r--   0        0        0     4749 2024-05-20 21:02:05.111266 gitsint-0.2.1/gitsint/README.md
+-rw-r--r--   0        0        0    12460 2024-05-20 19:55:49.748563 gitsint-0.2.1/gitsint/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-19 09:46:11.286809 gitsint-0.2.1/gitsint/instruments.py
+-rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.2.1/gitsint/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.2.1/gitsint/modules/profile/__init__.py
+-rw-r--r--   0        0        0     2453 2024-05-20 19:54:10.549360 gitsint-0.2.1/gitsint/modules/profile/friends.py
+-rw-r--r--   0        0        0      385 2024-05-20 19:47:09.923659 gitsint-0.2.1/gitsint/modules/profile/profile.py
+-rw-r--r--   0        0        0        0 2024-05-19 09:46:11.296809 gitsint-0.2.1/gitsint/modules/repos/__init__.py
+-rw-r--r--   0        0        0     8601 2024-05-20 15:47:29.310895 gitsint-0.2.1/gitsint/modules/repos/repository.py
+-rw-r--r--   0        0        0      822 2024-05-20 21:02:31.791733 gitsint-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 gitsint-0.2.1/PKG-INFO
```

### Comparing `gitsint-0.1.0/LICENSE` & `gitsint-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.0/LICENSE.md` & `gitsint-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.0/gitsint/__init__.py` & `gitsint-0.2.1/gitsint/__init__.py`

 * *Files 1% similar despite different names*

```diff
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
```

### Comparing `gitsint-0.1.0/gitsint/modules/profile/friends.py` & `gitsint-0.2.1/gitsint/modules/profile/friends.py`

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

### Comparing `gitsint-0.1.0/gitsint/modules/repos/repository.py` & `gitsint-0.2.1/gitsint/modules/repos/repository.py`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.0/pyproject.toml` & `gitsint-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitsint"
-version = "0.1.0"
+version = "0.2.1"
 description = "gitsint allows you to check everything from a github user."
 authors = ["Zerostats"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -28,12 +28,12 @@
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

