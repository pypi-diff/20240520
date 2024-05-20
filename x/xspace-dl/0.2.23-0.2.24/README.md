# Comparing `tmp/xspace-dl-0.2.23.tar.gz` & `tmp/xspace-dl-0.2.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.2.23.tar", last modified: Mon May 20 15:03:46 2024, max compression
+gzip compressed data, was "xspace-dl-0.2.24.tar", last modified: Mon May 20 15:13:47 2024, max compression
```

## Comparing `xspace-dl-0.2.23.tar` & `xspace-dl-0.2.24.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:03:46.019061 xspace-dl-0.2.23/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.23/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:03:46.018890 xspace-dl-0.2.23/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.23/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.23/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 15:03:46.019108 xspace-dl-0.2.23/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 15:02:48.000000 xspace-dl-0.2.23/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:03:46.017385 xspace-dl-0.2.23/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:37:36.000000 xspace-dl-0.2.23/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16579 2024-05-20 15:01:12.000000 xspace-dl-0.2.23/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.23/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7335 2024-05-20 15:01:42.000000 xspace-dl-0.2.23/xspace/main.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6059 2024-05-20 15:02:04.000000 xspace-dl-0.2.23/xspace/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7062 2024-05-20 15:01:55.000000 xspace-dl-0.2.23/xspace/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:03:46.018623 xspace-dl-0.2.23/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:13:47.288847 xspace-dl-0.2.24/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.24/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:13:47.288673 xspace-dl-0.2.24/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.24/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.24/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 15:13:47.288896 xspace-dl-0.2.24/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 15:13:37.000000 xspace-dl-0.2.24/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:13:47.287287 xspace-dl-0.2.24/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:37:36.000000 xspace-dl-0.2.24/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16585 2024-05-20 15:13:19.000000 xspace-dl-0.2.24/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.24/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7335 2024-05-20 15:01:42.000000 xspace-dl-0.2.24/xspace/main.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6059 2024-05-20 15:02:04.000000 xspace-dl-0.2.24/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7062 2024-05-20 15:01:55.000000 xspace-dl-0.2.24/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:13:47.288447 xspace-dl-0.2.24/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 15:13:47.000000 xspace-dl-0.2.24/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.2.23/LICENSE` & `xspace-dl-0.2.24/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.23/PKG-INFO` & `xspace-dl-0.2.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.23
+Version: 0.2.24
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/rosebabaganoush/xspace-dl
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.23 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.24 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```

### Comparing `xspace-dl-0.2.23/README.md` & `xspace-dl-0.2.24/README.md`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.23/pyproject.toml` & `xspace-dl-0.2.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.23/setup.py` & `xspace-dl-0.2.24/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',
-    version='0.2.23',
+    version='0.2.24',
     author='Your Name',
     author_email='your.email@example.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rosebabaganoush/xspace-dl',
     packages=find_packages(),
```

### Comparing `xspace-dl-0.2.23/xspace/api.py` & `xspace-dl-0.2.24/xspace/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         variables = {
             "id": space_id,
             "isMetatagsQuery": True,
             "withReplays": True,
             "withListeners": True,
         }
         # "features" is copied as-is from real requests
-        features = '{"spaces_2022_h2_clipping":true,"spaces_2022_h2_spaces_communities":true,"responsive_web_graphql_exclude_directive_enabled":true,"verified_phone_label_enabled":false,"creator_subscriptions_tweet_preview_api_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"responsive_web_x_article_tweet_consumption_enabled":false,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":true,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":true,"responsive_web_graphql_timeline_navigation_enabled":true,"longform_notetweets_rich_text_read_enabled":true,"longform_notetweets_inline_media_enabled":true,"responsive_web_media_download_video_enabled":false,"responsive_web_enhance_cards_enabled":false}'
+        features = '{"spaces_2022_h2_clipping":true,"spaces_2022_h2_spaces_communities":true,"responsive_web_graphql_exclude_directive_enabled":true,"verified_phone_label_enabled":false,"creator_subscriptions_tweet_preview_api_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"responsive_web_twitter_article_tweet_consumption_enabled":false,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":true,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":true,"responsive_web_graphql_timeline_navigation_enabled":true,"longform_notetweets_rich_text_read_enabled":true,"longform_notetweets_inline_media_enabled":true,"responsive_web_media_download_video_enabled":false,"responsive_web_enhance_cards_enabled":false}'
         return self.get(query_id, operation_name, variables, features)
 
     def user_by_screen_name(self, screen_name: str) -> dict:
         """Query X user details by their screen name (@ handle).
 
         - screen_name: The screen name (@ handle) of the X user.
```

### Comparing `xspace-dl-0.2.23/xspace/cookies.py` & `xspace-dl-0.2.24/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.23/xspace/main.py` & `xspace-dl-0.2.24/xspace/main.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.23/xspace/xspace.py` & `xspace-dl-0.2.24/xspace/xspace.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.23/xspace/xspace_dl.py` & `xspace-dl-0.2.24/xspace/xspace_dl.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.23/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.2.24/xspace_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.23
+Version: 0.2.24
 Summary: A python module to download Twitter spaces
 Home-page: https://github.com/rosebabaganoush/xspace-dl
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.23 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.24 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```

