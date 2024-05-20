# Comparing `tmp/xspace-dl-0.2.22.tar.gz` & `tmp/xspace-dl-0.2.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspace-dl-0.2.22.tar", last modified: Mon May 20 14:42:03 2024, max compression
+gzip compressed data, was "xspace-dl-0.2.23.tar", last modified: Mon May 20 15:03:46 2024, max compression
```

## Comparing `xspace-dl-0.2.22.tar` & `xspace-dl-0.2.23.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:42:03.059161 xspace-dl-0.2.22/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/LICENSE
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 14:42:03.058979 xspace-dl-0.2.22/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/README.md
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/pyproject.toml
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 14:42:03.059211 xspace-dl-0.2.22/setup.cfg
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 14:41:29.000000 xspace-dl-0.2.22/setup.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:42:03.057649 xspace-dl-0.2.22/xspace/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:37:36.000000 xspace-dl-0.2.22/xspace/__init__.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)    16837 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/xspace/api.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.22/xspace/cookies.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7359 2024-05-20 14:37:45.000000 xspace-dl-0.2.22/xspace/main.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6083 2024-05-20 14:39:00.000000 xspace-dl-0.2.22/xspace/xspace.py
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     7074 2024-05-20 14:38:05.000000 xspace-dl-0.2.22/xspace/xspace_dl.py
-drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 14:42:03.058755 xspace-dl-0.2.22/xspace_dl.egg-info/
--rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/PKG-INFO
--rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 14:42:03.000000 xspace-dl-0.2.22/xspace_dl.egg-info/SOURCES.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/dependency_links.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/entry_points.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/requires.txt
--rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 14:42:02.000000 xspace-dl-0.2.22/xspace_dl.egg-info/top_level.txt
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:03:46.019061 xspace-dl-0.2.23/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    18092 2024-05-20 14:08:08.000000 xspace-dl-0.2.23/LICENSE
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:03:46.018890 xspace-dl-0.2.23/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6218 2024-05-20 14:08:08.000000 xspace-dl-0.2.23/README.md
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1085 2024-05-20 14:08:08.000000 xspace-dl-0.2.23/pyproject.toml
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       38 2024-05-20 15:03:46.019108 xspace-dl-0.2.23/setup.cfg
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      856 2024-05-20 15:02:48.000000 xspace-dl-0.2.23/setup.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:03:46.017385 xspace-dl-0.2.23/xspace/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      171 2024-05-20 14:37:36.000000 xspace-dl-0.2.23/xspace/__init__.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)    16579 2024-05-20 15:01:12.000000 xspace-dl-0.2.23/xspace/api.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     1978 2024-05-20 14:08:08.000000 xspace-dl-0.2.23/xspace/cookies.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7335 2024-05-20 15:01:42.000000 xspace-dl-0.2.23/xspace/main.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6059 2024-05-20 15:02:04.000000 xspace-dl-0.2.23/xspace/xspace.py
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     7062 2024-05-20 15:01:55.000000 xspace-dl-0.2.23/xspace/xspace_dl.py
+drwxr-xr-x   0 eggswhysaid   (502) staff       (20)        0 2024-05-20 15:03:46.018623 xspace-dl-0.2.23/xspace_dl.egg-info/
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)     6693 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/PKG-INFO
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)      344 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        1 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       47 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/entry_points.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)       17 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/requires.txt
+-rw-r--r--   0 eggswhysaid   (502) staff       (20)        7 2024-05-20 15:03:45.000000 xspace-dl-0.2.23/xspace_dl.egg-info/top_level.txt
```

### Comparing `xspace-dl-0.2.22/LICENSE` & `xspace-dl-0.2.23/LICENSE`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.22/PKG-INFO` & `xspace-dl-0.2.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.22
+Version: 0.2.23
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
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.22 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.23 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```

### Comparing `xspace-dl-0.2.22/README.md` & `xspace-dl-0.2.23/README.md`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.22/pyproject.toml` & `xspace-dl-0.2.23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.22/setup.py` & `xspace-dl-0.2.23/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xspace-dl',
-    version='0.2.22',
+    version='0.2.23',
     author='Your Name',
     author_email='your.email@example.com',
     description='A python module to download Twitter spaces',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rosebabaganoush/xspace-dl',
     packages=find_packages(),
```

### Comparing `xspace-dl-0.2.22/xspace/api.py` & `xspace-dl-0.2.23/xspace/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 from requests.adapters import HTTPAdapter, Retry
 from requests.exceptions import (ConnectionError, HTTPError, JSONDecodeError,
                                  RetryError)
 
 from .cookies import validate_cookies
 
-"""Twitter unofficial API authorization header."""
+"""X unofficial API authorization header."""
 TWITTER_AUTHORIZATION = "Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA"
 
 """Retry parameters for making all requests."""
 RETRY = Retry(
     total=5,
     connect=3,
     read=2,
@@ -84,15 +84,15 @@
             raise RuntimeError("API request failed with HTTP error") from e
 
 
 class APIClient:
     """Base API client."""
 
     """Base URL of the API."""
-    _API_URL = "https://twitter.com/i/api"
+    _API_URL = "https://x.com/i/api"
 
     def __init__(self, client: HTTPClient, path: str, cookies: dict[str, str]) -> None:
         """Initialize the API client.
 
         - client: The `HTTPClient` instance to send requests.
         - path: The path to add to the base URL of the API.
         - cookies: The cookies used for making all requests to the API.
@@ -136,18 +136,18 @@
                 f"Cannot decode response from URL: {response.url}, status code: {response.status_code}"
             )
             logging.debug(f"Response text: {response.text!r}")
             raise RuntimeError("API response cannot be decoded as JSON")
 
 
 class GraphQLAPI(APIClient):
-    """Twitter GraphQL API client."""
+    """X GraphQL API client."""
 
     def __init__(self, client: HTTPClient, path: str, cookies: dict[str, str]) -> None:
-        """Initialize the Twitter GraphQL API client.
+        """Initialize the X GraphQL API client.
 
         - client: The `HTTPClient` instance to send requests.
         - path: The path to add to the base URL of the API.
         - cookies: The cookies used for making all requests to the API.
         """
         super().__init__(client, path, cookies)
 
@@ -167,81 +167,81 @@
     def get(
         self,
         query_id: str,
         operation_name: str,
         variables: dict[str, str] | str,
         features: dict[str, str] | str | None = None,
     ) -> Any:
-        """Send HTTP GET requests to the Twitter GraphQL API.
+        """Send HTTP GET requests to the X GraphQL API.
 
         - query_id: The query ID of the GraphQL API endpoint.
         - operation_name: The name of the operation to be executed.
         - variables: Query variables of the GraphQL query.
         - features: Feature switches of the GraphQL query.
 
         - return: The returned object of the query.
         """
         params = {"variables": self._dump_json(variables)}
         if features:
             params["features"] = self._dump_json(features)
         return super().get(self.join_url(query_id, operation_name), params)
 
     def audio_space_by_id(self, space_id: str) -> dict:
-        """Query Twitter Space details by its ID.
+        """Query X Space details by its ID.
 
-        - space_id: The ID of the Twitter Space.
+        - space_id: The ID of the X Space.
 
-        - return: The details of the queried Twitter Space.
+        - return: The details of the queried X Space.
         """
         query_id = "xVEzTKg_mLTHubK5ayL0HA"
         operation_name = "AudioSpaceById"
         variables = {
             "id": space_id,
             "isMetatagsQuery": True,
             "withReplays": True,
             "withListeners": True,
         }
         # "features" is copied as-is from real requests
-        features = '{"spaces_2022_h2_clipping":true,"spaces_2022_h2_spaces_communities":true,"responsive_web_graphql_exclude_directive_enabled":true,"verified_phone_label_enabled":false,"creator_subscriptions_tweet_preview_api_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"responsive_web_twitter_article_tweet_consumption_enabled":false,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":true,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":true,"responsive_web_graphql_timeline_navigation_enabled":true,"longform_notetweets_rich_text_read_enabled":true,"longform_notetweets_inline_media_enabled":true,"responsive_web_media_download_video_enabled":false,"responsive_web_enhance_cards_enabled":false}'
+        features = '{"spaces_2022_h2_clipping":true,"spaces_2022_h2_spaces_communities":true,"responsive_web_graphql_exclude_directive_enabled":true,"verified_phone_label_enabled":false,"creator_subscriptions_tweet_preview_api_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"responsive_web_x_article_tweet_consumption_enabled":false,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":true,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":true,"responsive_web_graphql_timeline_navigation_enabled":true,"longform_notetweets_rich_text_read_enabled":true,"longform_notetweets_inline_media_enabled":true,"responsive_web_media_download_video_enabled":false,"responsive_web_enhance_cards_enabled":false}'
         return self.get(query_id, operation_name, variables, features)
 
     def user_by_screen_name(self, screen_name: str) -> dict:
-        """Query Twitter user details by their screen name (@ handle).
+        """Query X user details by their screen name (@ handle).
 
-        - screen_name: The screen name (@ handle) of the Twitter user.
+        - screen_name: The screen name (@ handle) of the X user.
 
-        - return: The details of the queried Twitter user.
+        - return: The details of the queried X user.
         """
         query_id = "oUZZZ8Oddwxs8Cd3iW3UEA"
         operation_name = "UserByScreenName"
         variables = {"screen_name": screen_name, "withSafetyModeUserFields": True}
         # "features" is copied as-is from real requests
         features = '{"hidden_profile_likes_enabled":false,"responsive_web_graphql_exclude_directive_enabled":true,"verified_phone_label_enabled":false,"subscriptions_verification_info_verified_since_enabled":true,"highlights_tweets_tab_ui_enabled":true,"creator_subscriptions_tweet_preview_api_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true}'
         return self.get(query_id, operation_name, variables, features)
 
     def profile_spotlights_query(self, screen_name: str) -> dict:
-        """Backup API endpoint to query Twitter user details by their screen name (@ handle).
+        """Backup API endpoint to query X user details by their screen name (@ handle).
 
         The response data from this API contains less information of the user than the `user_by_screen_name`
         API, but still has the essential `rest_id` field. Therefore, it is used as a backup of the other API
         endpoint if the other one was rate limited.
 
-        - screen_name: The screen name (@ handle) of the Twitter user.
+        - screen_name: The screen name (@ handle) of the X user.
 
-        - return: The details of the queried Twitter user.
+        - return: The details of the queried X user.
         """
         query_id = "ZQEuHPrIYlvh1NAyIQHP_w"
         operation_name = "ProfileSpotlightsQuery"
         variables = {"screen_name": screen_name}
         return self.get(query_id, operation_name, variables)
 
     def user_id(self, screen_name: str) -> str:
         """Retrieve the numeric user ID (`rest_id`) of the user with the specified screen name (@ handle).
 
-        - screen_name: The screen name (@ handle) of the Twitter user.
+        - screen_name: The screen name (@ handle) of the X user.
 
         - return: The numeric user ID (`rest_id`) of the specified user.
         """
         try:
             data = self.user_by_screen_name(screen_name)
             return data["data"]["user"]["result"]["rest_id"]
         except HTTPError:
@@ -249,90 +249,90 @@
             data = self.profile_spotlights_query(screen_name)
             return data["data"]["user_result_by_screen_name"]["result"]["rest_id"]
 
     def user_id_from_url(self, user_url: str) -> str:
         """Retrieve the numeric user ID (`rest_id`) of the user that the specified profile URL linked to.
 
         Supported URL formats:
-        - https://twitter.com/<screen_name>
-        - http://twitter.com/<screen_name>
-        - twitter.com/<screen_name>
+        - https://x.com/<screen_name>
+        - http://x.com/<screen_name>
+        - x.com/<screen_name>
         and with any number of trailing slashes (`/`).
 
-        - user_url: The URL pointing to the profile of the Twitter user.
+        - user_url: The URL pointing to the profile of the X user.
 
         - return: The numeric user ID (`rest_id`) of the specified user.
 
-        - raise RuntimeError: If the specified URL is not a valid Twitter user profile URL.
+        - raise RuntimeError: If the specified URL is not a valid X user profile URL.
         """
         if match := re.match(
-            r"^(?:https?:\/\/|)twitter\.com\/(?P<screen_name>\w+)$", user_url.strip("/")
+            r"^(?:https?:\/\/|)x\.com\/(?P<screen_name>\w+)$", user_url.strip("/")
         ):
             return self.user_id(match.group("screen_name"))
-        raise RuntimeError(f"Invalid Twitter user URL: {user_url}")
+        raise RuntimeError(f"Invalid X user URL: {user_url}")
 
 
 class FleetsAPI(APIClient):
-    """Twitter Fleets API client."""
+    """X Fleets API client."""
 
     def __init__(self, client: HTTPClient, path: str, cookies: dict[str, str]) -> None:
-        """Initialize the Twitter Fleets API client.
+        """Initialize the X Fleets API client.
 
         - client: The `HTTPClient` instance to send requests.
         - path: The path to add to the base URL of the API.
         - cookies: The cookies used for making all requests to the API.
         """
         super().__init__(client, path, cookies)
 
     def get(self, version: str, endpoint: str, params: dict[str, str]) -> Any:
-        """Send HTTP GET requests to the Twitter Fleets API.
+        """Send HTTP GET requests to the X Fleets API.
 
         - version: The version of the API.
         - endpoint: The endpoint of the API.
         - params: Query parameters of the request.
 
         - return: The object returned in the response of the API.
         """
         return super().get(self.join_url(version, endpoint), params)
 
     def avatar_content(self, *user_ids: str) -> dict:
-        """Retrieve Twitter Space details of the specified user IDs.
+        """Retrieve X Space details of the specified user IDs.
 
         This endpoint limits to a maximum of 100 user IDs per request.
 
         - user_ids: Numeric user IDs (`rest_id`) of users.
 
-        - return: Twitter Space details of the specified user IDs. Only ongoing Twitter Spaces will be returned.
+        - return: X Space details of the specified user IDs. Only ongoing X Spaces will be returned.
         """
         if len(user_ids) > 100:
             raise RuntimeError(
                 "Number of user IDs exceeded the limit of 100 per request"
             )
         version = "v1"
         endpoint = "avatar_content"
         params = {"user_ids": ",".join(user_ids), "only_spaces": "true"}
         return self.get(version, endpoint, params)
 
 
 class LiveVideoStreamAPI(APIClient):
-    """Twitter Live Video Stream API client."""
+    """X Live Video Stream API client."""
 
     def __init__(self, client: HTTPClient, path: str, cookies: dict[str, str]) -> None:
-        """Initialize the Twitter Live Video Stream API client.
+        """Initialize the X Live Video Stream API client.
 
         - client: The `HTTPClient` instance to send requests.
         - path: The path to add to the base URL of the API.
         - cookies: The cookies used for making all requests to the API.
         """
         super().__init__(client, path, cookies)
 
     def status(self, media_key: str) -> dict:
-        """Retrieve Twitter Space media playlist details by the specified media key.
+        """Retrieve X Space media playlist details by the specified media key.
 
-        - media_key: The media key of the Twitter Space.
+        - media_key: The media key of the X Space.
 
         - return: The media playlist details of the specified media key.
         """
         return super().get(self.join_url("status", media_key))
 
 
 class DummyAPI:
@@ -352,53 +352,53 @@
         """Always evaluate instances of the class to `False`.
 
         This is just for the convenience of testing the instance directly in `if` statements:
         >>> api = DummyAPI()
         ... if api:  # non-dummy API instances would evaluate to `True`
         ...     # do something if the API was initialized
         ...     pass
-        See also: `TwitterAPI.__bool__()`
+        See also: `XAPI.__bool__()`
 
         - return: `False`.
         """
         return False
 
 
-class TwitterAPI:
-    """The collection of all Twitter APIs."""
+class XAPI:
+    """The collection of all X APIs."""
 
     def __init__(self) -> None:
-        """Initialize the instance of the Twitter API collection.
+        """Initialize the instance of the X API collection.
 
         Note that this will not initialize APIs in this collection. They will initially only be an
         instance of the `DummyAPI` class.
         They need to be initialized by calling the `init_apis()` method with cookies of the user.
         """
         self.client = HTTPClient()
-        self.graphql_api = DummyAPI("Twitter GraphQL API")
-        self.fleets_api = DummyAPI("Twitter Fleets API")
-        self.live_video_stream_api = DummyAPI("Twitter Live Video Stream API")
+        self.graphql_api = DummyAPI("X GraphQL API")
+        self.fleets_api = DummyAPI("X Fleets API")
+        self.live_video_stream_api = DummyAPI("X Live Video Stream API")
 
     def init_apis(self, cookies: dict[str, str]) -> None:
         """Initialize all APIs in this collection with the specified cookies."""
         self.graphql_api = GraphQLAPI(self.client, "graphql", cookies)
         self.fleets_api = FleetsAPI(self.client, "fleets", cookies)
         self.live_video_stream_api = LiveVideoStreamAPI(
             self.client, "1.1/live_video_stream", cookies
         )
 
     def __bool__(self) -> bool:
         """Determine if all APIs are initialized.
 
         This is just for the convenience of testing the instance directly in `if` statements:
-        >>> api = TwitterAPI()
+        >>> api = XAPI()
         ... if api:
         ...     print("API initialized")  # would run if all APIs in the `api` instance are initialized
         See also: `DummyAPI.__bool__()`
 
         - return: `True` if and only if all APIs are initialized, `False` otherwise.
         """
         return bool(self.graphql_api and self.fleets_api and self.live_video_stream_api)
 
 
-"""The global instance of the collection of Twitter APIs."""
-API = TwitterAPI()
+"""The global instance of the collection of X APIs."""
+API = XAPI()
```

### Comparing `xspace-dl-0.2.22/xspace/cookies.py` & `xspace-dl-0.2.23/xspace/cookies.py`

 * *Files identical despite different names*

### Comparing `xspace-dl-0.2.22/xspace/main.py` & `xspace-dl-0.2.23/xspace/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     _t: TracebackType = None,
 ) -> None:
     """Make Exceptions more legible for the end users"""
     # Exception type and value
     print(f"\033[31;1;4mError\033[0m: {exc_value}\nRetry with -v to see more details")
 
 def space(args: argparse.Namespace) -> int:
-    """Manage the twitter space related function"""
+    """Manage the x space related function"""
     has_input = (
         args.user_url
         or args.input_url
         or args.input_metadata
         or args.from_dynamic_url
         or args.from_master_url
     )
@@ -110,15 +110,15 @@
             if not args.keep_files:
                 xspace_dl.cleanup()
     return EXIT_CODE_SUCCESS
 
 def main() -> int:
     """Main function, creates the argument parser"""
     parser = argparse.ArgumentParser(
-        description="Script designed to help download twitter spaces"
+        description="Script designed to help download x spaces"
     )
 
     input_group = parser.add_argument_group("input")
     input_method = input_group.add_mutually_exclusive_group()
     output_group = parser.add_argument_group("output")
 
     parser.add_argument("-v", "--verbose", action="store_true")
@@ -129,16 +129,16 @@
         "-c",
         "--input-cookie-file",
         type=str,
         metavar="COOKIE_FILE",
         help=(
             "cookies file in the Netscape format. The specs of the Netscape cookies format "
             "can be found here: https://curl.se/docs/http-cookies.html. The cookies file is "
-            "now required due to the Twitter API change that prohibited guest user access to "
-            "Twitter API endpoints on 2023-07-01."
+            "now required due to the X API change that prohibited guest user access to "
+            "X API endpoints on 2023-07-01."
         ),
         required=True,
     )
 
     input_method.add_argument("-i", "--input-url", type=str, metavar="SPACE_URL")
     input_method.add_argument("-U", "--user-url", type=str, metavar="USER_URL")
     input_group.add_argument(
```

### Comparing `xspace-dl-0.2.22/xspace/xspace.py` & `xspace-dl-0.2.23/xspace/xspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 from collections import defaultdict
 from datetime import datetime
 
 from .api import API
 
 class Xspace(dict):  # Ensure the class name is Xspace
-    """Downloader class for twitter spaces"""
+    """Downloader class for x spaces"""
 
     def __init__(self, metadata: dict) -> None:
         dict.__init__(
             self,
             {
                 "id": "",
                 "url": "",
@@ -38,15 +38,15 @@
                 self["creator_id"] = API.graphql_api.user_id(
                     creator_info["screen_name"]
                 )
 
             self.source = metadata
             self.root = root
             self["id"] = root["rest_id"]
-            self["url"] = "https://twitter.com/i/spaces/" + self["id"]
+            self["url"] = "https://x.com/i/spaces/" + self["id"]
             self["title"] = root["title"]
             try:
                 self["start_date"] = datetime.fromtimestamp(
                     int(root["started_at"]) / 1000
                 ).strftime("%Y-%m-%d")
             except ValueError as err:
                 sched_start = datetime.fromtimestamp(
@@ -142,22 +142,22 @@
         """Create a Xspace instance from a space url"""
         try:
             space_id = re.findall(r"(?<=spaces/)\w*", url)[0]
         except IndexError as err:
             raise ValueError(
                 (
                     "Input URL is not valid.\n"
-                    "The URL format should 'https://twitter.com/i/spaces/<space_id>'"
+                    "The URL format should 'https://x.com/i/spaces/<space_id>'"
                 )
             ) from err
         return cls(cls._metadata(space_id))
 
     @classmethod
     def from_user_avatar(cls, user_url: str):
-        """Create a Xspace instance from a twitter user's ongoing space"""
+        """Create a Xspace instance from a x user's ongoing space"""
         user_id = API.graphql_api.user_id_from_url(user_url)
         avatar_content = API.fleets_api.avatar_content(user_id)
         try:
             broadcast_id = avatar_content["users"][user_id]["spaces"]["live_content"][
                 "audiospace"
             ]["broadcast_id"]
         except KeyError as err:
```

### Comparing `xspace-dl-0.2.22/xspace/xspace_dl.py` & `xspace-dl-0.2.23/xspace/xspace_dl.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .api import API
 from .xspace import Xspace  # Updated import
 
 DEFAULT_FNAME_FORMAT = "(%(creator_name)s)%(title)s-%(id)s"
 MP4_COVER_FORMAT_MAP = {"jpg": MP4Cover.FORMAT_JPEG, "png": MP4Cover.FORMAT_PNG}
 
 class XspaceDL:
-    """Downloader class for twitter spaces"""
+    """Downloader class for x spaces"""
 
     def __init__(self, space: Xspace, format_str: str) -> None:
         self.space = space
         self.format_str = format_str or DEFAULT_FNAME_FORMAT
         self._tempdir = ""
 
     @cached_property
@@ -79,15 +79,15 @@
         filename = os.path.basename(self.filename) + ".m3u8"
         path = os.path.join(save_dir, filename)
         with open(path, "w", encoding="utf-8") as stream_io:
             stream_io.write(self.playlist_text)
         logging.debug("%(path)s written to disk", dict(path=path))
 
     def download(self) -> None:
-        """Download a twitter space"""
+        """Download a x space"""
         if not shutil.which("ffmpeg"):
             raise FileNotFoundError("ffmpeg not installed")
         space = self.space
         self._tempdir = tempfile.mkdtemp(dir=".")
         self.write_playlist(save_dir=self._tempdir)
         state = space["state"]
```

### Comparing `xspace-dl-0.2.22/xspace_dl.egg-info/PKG-INFO` & `xspace-dl-0.2.23/xspace_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xspace-dl
-Version: 0.2.22
+Version: 0.2.23
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
-Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.22 Summary: A python module
+Metadata-Version: 2.1 Name: xspace-dl Version: 0.2.23 Summary: A python module
 to download Twitter spaces Home-page: https://github.com/rosebabaganoush/
 xspace-dl Author: Your Name Author-email: your.email@example.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v2 (GPLv2) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
                            ************ TTwwssppaaccee--ddll ************
```

