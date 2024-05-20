# Comparing `tmp/fast_multi_regex-0.7.tar.gz` & `tmp/fast_multi_regex-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_multi_regex-0.7.tar", last modified: Sun May 19 16:08:00 2024, max compression
+gzip compressed data, was "fast_multi_regex-0.8.tar", last modified: Sun May 19 16:43:07 2024, max compression
```

## Comparing `fast_multi_regex-0.7.tar` & `fast_multi_regex-0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 16:08:00.758302 fast_multi_regex-0.7/
--rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.7/LICENSE
--rwxrwxrwx   0     1024 users      (100)     2314 2024-05-19 16:08:00.757302 fast_multi_regex-0.7/PKG-INFO
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 16:08:00.739302 fast_multi_regex-0.7/fast_multi_regex/
--rwxrwxrwx   0     1024 users      (100)      541 2024-05-19 11:29:13.000000 fast_multi_regex-0.7/fast_multi_regex/__init__.py
--rwxrwxrwx   0     1024 users      (100)     6199 2024-05-19 11:41:53.000000 fast_multi_regex-0.7/fast_multi_regex/api.py
--rwxrwxrwx   0     1024 users      (100)     3166 2024-05-19 11:43:21.000000 fast_multi_regex-0.7/fast_multi_regex/api_types.py
--rwxrwxrwx   0     1024 users      (100)    38984 2024-05-19 16:04:10.000000 fast_multi_regex-0.7/fast_multi_regex/matcher.py
--rwxrwxrwx   0     1024 users      (100)     3194 2024-05-19 11:28:53.000000 fast_multi_regex-0.7/fast_multi_regex/server.py
--rwxrwxrwx   0     1024 users      (100)    11603 2024-05-19 14:35:20.000000 fast_multi_regex-0.7/fast_multi_regex/utils.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 16:08:00.754302 fast_multi_regex-0.7/fast_multi_regex.egg-info/
--rwxrwxrwx   0     1024 users      (100)     2314 2024-05-19 16:08:00.000000 fast_multi_regex-0.7/fast_multi_regex.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      422 2024-05-19 16:08:00.000000 fast_multi_regex-0.7/fast_multi_regex.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2024-05-19 16:08:00.000000 fast_multi_regex-0.7/fast_multi_regex.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)       79 2024-05-19 16:08:00.000000 fast_multi_regex-0.7/fast_multi_regex.egg-info/entry_points.txt
--rwxrwxrwx   0     1024 users      (100)       76 2024-05-19 16:08:00.000000 fast_multi_regex-0.7/fast_multi_regex.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)       17 2024-05-19 16:08:00.000000 fast_multi_regex-0.7/fast_multi_regex.egg-info/top_level.txt
--rwxrwxrwx   0     1024 users      (100)       38 2024-05-19 16:08:00.758302 fast_multi_regex-0.7/setup.cfg
--rwxrwxrwx   0     1024 users      (100)     1300 2024-05-19 16:07:57.000000 fast_multi_regex-0.7/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 16:43:07.562597 fast_multi_regex-0.8/
+-rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.8/LICENSE
+-rwxrwxrwx   0     1024 users      (100)     2320 2024-05-19 16:43:07.561597 fast_multi_regex-0.8/PKG-INFO
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 16:43:07.542597 fast_multi_regex-0.8/fast_multi_regex/
+-rwxrwxrwx   0     1024 users      (100)      541 2024-05-19 11:29:13.000000 fast_multi_regex-0.8/fast_multi_regex/__init__.py
+-rwxrwxrwx   0     1024 users      (100)     6358 2024-05-19 16:41:29.000000 fast_multi_regex-0.8/fast_multi_regex/api.py
+-rwxrwxrwx   0     1024 users      (100)     3166 2024-05-19 11:43:21.000000 fast_multi_regex-0.8/fast_multi_regex/api_types.py
+-rwxrwxrwx   0     1024 users      (100)    39019 2024-05-19 16:27:18.000000 fast_multi_regex-0.8/fast_multi_regex/matcher.py
+-rwxrwxrwx   0     1024 users      (100)     3194 2024-05-19 11:28:53.000000 fast_multi_regex-0.8/fast_multi_regex/server.py
+-rwxrwxrwx   0     1024 users      (100)    11603 2024-05-19 14:35:20.000000 fast_multi_regex-0.8/fast_multi_regex/utils.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 16:43:07.558597 fast_multi_regex-0.8/fast_multi_regex.egg-info/
+-rwxrwxrwx   0     1024 users      (100)     2320 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      422 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)       79 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/entry_points.txt
+-rwxrwxrwx   0     1024 users      (100)       76 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)       17 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/top_level.txt
+-rwxrwxrwx   0     1024 users      (100)       38 2024-05-19 16:43:07.563597 fast_multi_regex-0.8/setup.cfg
+-rwxrwxrwx   0     1024 users      (100)     1300 2024-05-19 16:42:33.000000 fast_multi_regex-0.8/setup.py
```

### Comparing `fast_multi_regex-0.7/LICENSE` & `fast_multi_regex-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.7/PKG-INFO` & `fast_multi_regex-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_multi_regex
-Version: 0.7
+Version: 0.8
 Summary: Fast multi-regex, multi-pattern, boolean expression matching
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 介绍
 
 - 快速多正则多模匹配，10万个正则表达式编译2分钟，匹配1千次耗时最低0.003s以内，支持多正则之间的布尔运算匹配，基于 hyperscan / pyeda
-- 提供封装的 HTTP 服务，编译和匹配过程不同进程，支持热更新正则库
+- 提供封装的 HTTP 服务，编译和匹配过程使用不同进程，支持热更新正则库
 
 ## 使用
 ```shell
 pip install fast-multi-regex
 fast_multi_regex_server --help
 fast_multi_regex_server
 ```
```

### Comparing `fast_multi_regex-0.7/fast_multi_regex/__init__.py` & `fast_multi_regex-0.8/fast_multi_regex/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.7/fast_multi_regex/api.py` & `fast_multi_regex-0.8/fast_multi_regex/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,19 @@
         context={
             'matchers_folder': matchers_folder,
             'matchers': global_matchers,
         },
     )
 
 
-app = FastAPI()
+app = FastAPI(
+    title='fast-multi-regex',
+    summary='A fast multi regex matcher',
+    description='快速多正则和布尔表达式匹配，支持热更新正则库',
+)
 app.add_event_handler("startup", startup)
 security = HTTPBearer()
 
 
 def verify_token(credentials: HTTPAuthorizationCredentials = Depends(security)):
     if credentials:
         token = credentials.credentials
```

### Comparing `fast_multi_regex-0.7/fast_multi_regex/api_types.py` & `fast_multi_regex-0.8/fast_multi_regex/api_types.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.7/fast_multi_regex/matcher.py` & `fast_multi_regex-0.8/fast_multi_regex/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     hyperscan_size: int = Field(0, description='hyperscan 数据库大小, 单位字节')
     hyperscan_info: str = Field("", description='hyperscan 数据库信息')
     literal: bool = Field(False, description='是否只有字面量正则，把所有 expression 都当作普通字符匹配，flag/ext 全部失效')
 
 
 class OneFindRegex(BaseModel):
     regex_id: int = Field(..., description='正则在数据库中的 ID')
-    regex: OneRegex = Field(..., description='第一个正则, expression/flag 唯一，其他属性供参考')
+    regex: OneRegex = Field(..., description='第一个正则, expression/flag 唯一(以及literal=False下的flag_ext)，其他属性供参考')
     mark_count: int = Field(None, description='包含的 mark 数量')
     first_mark: str = Field(None, description='包含的第一个 mark，compile 的 targes 顺序')
     first_mark_no: int = Field(None, description='first_mark 中在 regexs 中的索引号')
 
 
 class MultiRegexMatcher:
     def __init__(self, cache_size: int = 128) -> None:
```

### Comparing `fast_multi_regex-0.7/fast_multi_regex/server.py` & `fast_multi_regex-0.8/fast_multi_regex/server.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.7/fast_multi_regex/utils.py` & `fast_multi_regex-0.8/fast_multi_regex/utils.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.7/fast_multi_regex.egg-info/PKG-INFO` & `fast_multi_regex-0.8/fast_multi_regex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-multi-regex
-Version: 0.7
+Version: 0.8
 Summary: Fast multi-regex, multi-pattern, boolean expression matching
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 介绍
 
 - 快速多正则多模匹配，10万个正则表达式编译2分钟，匹配1千次耗时最低0.003s以内，支持多正则之间的布尔运算匹配，基于 hyperscan / pyeda
-- 提供封装的 HTTP 服务，编译和匹配过程不同进程，支持热更新正则库
+- 提供封装的 HTTP 服务，编译和匹配过程使用不同进程，支持热更新正则库
 
 ## 使用
 ```shell
 pip install fast-multi-regex
 fast_multi_regex_server --help
 fast_multi_regex_server
 ```
```

### Comparing `fast_multi_regex-0.7/setup.py` & `fast_multi_regex-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = 'https://github.com/aitsc/fast_multi_regex'
 
 setup(
     name='fast_multi_regex',
-    version='0.7',
+    version='0.8',
     description="Fast multi-regex, multi-pattern, boolean expression matching",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tanshicheng',
     license='GPLv3',
     url='https://github.com/aitsc/fast_multi_regex',
     keywords='tools',
```

