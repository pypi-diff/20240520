# Comparing `tmp/nonebot-plugin-hx-yinying-1.3.0.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.3.0.tar", last modified: Thu May 16 01:03:48 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.3.1.tar", last modified: Mon May 20 07:01:17 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.3.0.tar` & `nonebot-plugin-hx-yinying-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 01:03:48.936639 nonebot-plugin-hx-yinying-1.3.0/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     6502 2024-05-16 01:03:48.937715 nonebot-plugin-hx-yinying-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6062 2024-04-28 16:24:12.000000 nonebot-plugin-hx-yinying-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 01:03:48.760971 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    56210 2024-05-15 15:18:50.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    75314 2024-05-16 01:01:05.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0     1532 2024-05-16 01:03:03.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0     2549 2024-05-11 16:56:48.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/image_check.py
--rw-rw-rw-   0        0        0     5372 2024-05-15 12:55:21.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/report.py
--rw-rw-rw-   0        0        0     5032 2024-05-12 17:16:42.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/smms.py
-drwxrwxrwx   0        0        0        0 2024-05-16 01:03:48.924240 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     6502 2024-05-16 01:03:48.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-16 01:03:48.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 01:03:48.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2024-05-16 01:03:48.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-16 01:03:48.000000 nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-16 01:03:48.945463 nonebot-plugin-hx-yinying-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1002 2024-05-16 01:02:53.000000 nonebot-plugin-hx-yinying-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:01:17.769565 nonebot-plugin-hx-yinying-1.3.1/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6502 2024-05-20 07:01:17.770568 nonebot-plugin-hx-yinying-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6062 2024-04-28 16:24:12.000000 nonebot-plugin-hx-yinying-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 07:01:16.919557 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    56210 2024-05-15 15:18:50.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    75749 2024-05-20 06:58:45.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0     1533 2024-05-20 06:59:25.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     2549 2024-05-11 16:56:48.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/image_check.py
+-rw-rw-rw-   0        0        0     5372 2024-05-15 12:55:21.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/report.py
+-rw-rw-rw-   0        0        0     5032 2024-05-12 17:16:42.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/smms.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:01:17.762548 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     6502 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-20 07:01:15.000000 nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-20 07:01:17.777568 nonebot-plugin-hx-yinying-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-20 07:00:39.000000 nonebot-plugin-hx-yinying-1.3.1/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.3.0/LICENSE` & `nonebot-plugin-hx-yinying-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.0/PKG-INFO` & `nonebot-plugin-hx-yinying-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.3.0
+Version: 1.3.1
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.1 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.3.0/README.md` & `nonebot-plugin-hx-yinying-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -869,17 +869,20 @@
         at_reply = json_get(config, "at_reply", default=False)
         private = json_get(config, "private", default=True)
         def check_user_group_rules(to_me):
             is_admin = id in admin_list or id == admin_pro or id in superuser
             is_white = group_id in white_group or id in white_user
             is_black = group_id not in black_group or id not in black_user
             is_private = private if isinstance(eve, GroupMessageEvent) else True
+            is_bot = id is not eve.self_id
             if to_me and isinstance(eve, GroupMessageEvent):
-                return at_reply
-            return is_admin or is_white or (is_private and is_black)
+                return is_admin or is_white or (at_reply and is_bot and is_black)
+            if isinstance(eve, GroupMessageEvent):
+                return is_admin or is_white or (is_bot and is_black)
+            return is_admin or is_white or (is_private and is_black and is_bot)
         if isinstance(eve, GroupMessageEvent):
             to_me = event.to_me
             if rule_mode == "white":
                 return check_user_group_rules(to_me) or group_id in white_group
             else:
                 return check_user_group_rules(to_me)
         elif not isinstance(eve, GroupMessageEvent) and not private:
@@ -1333,14 +1336,16 @@
     nick = json_get(id_config,"nick")
     text = f"{nick}已经有{time_later}秒没有找你聊天了，{nick}就是我，快去看看{nick}在干什么吧,以第一人称生成一段面对{nick}时想找{nick}聊天的话"
     headers = {
         'Content-type': 'application/json',
         'Authorization': f'Bearer {hx_config.yinying_token}'
     }
     osu = await data_in(None,id,text,nick,False)
+    if not id:
+        return None
     if not osu:
         raise RuntimeError("[Hx]:初始化data失败，终止api调用进程！")
     async with httpx.AsyncClient(timeout=httpx.Timeout(connect=10, read=60, write=20, pool=30)) as client:
             back = await client.post("https://api-yinying-ng.wingmark.cn/v1/chatWithCyberFurry", headers=headers, json=osu)
     try:
             back = back.json()
     except json.decoder.JSONDecodeError as e:
@@ -1356,14 +1361,17 @@
 #主要构建
 async def yinying(groupid,id,text,nick,in_img):
     headers = {
         'Content-type': 'application/json',
         'Authorization': f'Bearer {hx_config.yinying_token}'
     }
     osu = await data_in(groupid,id,nick,text,in_img)
+    logger.debug(osu)
+    if not osu.get("chatId",None):
+        raise RuntimeError("[Hx]:未找到chatid，无效对话！")
     if not osu:
         raise RuntimeError("[Hx]:初始化data失败，终止api调用进程！")
     async with httpx.AsyncClient(timeout=httpx.Timeout(connect=10, read=60, write=20, pool=30)) as client:
             back_1 = await client.post("https://api-yinying-ng.wingmark.cn/v1/chatWithCyberFurry", headers=headers, json=osu)
     try:
             back = back_1.json()
     except json.decoder.JSONDecodeError as e:
@@ -1385,18 +1393,19 @@
     text = unescape(await gen_chat_text(event, bot))
     groupid = get_groupid(event)
     id = get_id(event)
     nick = await get_nick(bot,event)
     img = await get_img_urls(event)
     if  (text == "" or text == None or text == "！d" or text == "/！d") and img == []:
         if text == "！d" or text == "/！d":
-            return
+            return 0
         else:
             msg = "诶唔，你叫我是有什么事嘛？"
             await send_msg(matcher,event,msg)
+            return 0
     if img != []:
         in_img = await image_check(img[0])
         if text == "" or text == None:
             back_msg = str(await yinying(groupid,id,"看看这个图片",nick,in_img))
         else:
             back_msg = str(await yinying(groupid,id,text,nick,in_img))
         msg = back_msg.replace("/n","\n")
@@ -1412,14 +1421,15 @@
     img = await get_img_urls(event)
     groupid = get_groupid(event)
     id = get_id(event)
     nick = await get_nick(bot,event)
     if  (text == "" or text == None) and img == []:
         msg = "诶唔，你叫我是有什么事嘛？"
         await send_msg(matcher,event,msg)
+        return 0
     if img != []:
         in_img = await image_check(img[0])
         if text == "" or text == None:
             back_msg = str(await yinying(groupid,id,"看看这个图片",nick,in_img))
         else:
             back_msg = str(await yinying(groupid,id,text,nick,in_img))
         msg = back_msg.replace("/n","\n")
```

### Comparing `nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Optional, Union
 import nonebot
 from pydantic import BaseModel,AnyHttpUrl,Field
 
 
 class Config(BaseModel):
     # 插件版本号勿动！！！！
-    hx_version: Optional[str] = "1.3.0"
+    hx_version: Optional[str] = "1.3.01"
     # 秩乱v你的appid
     yinying_appid: Optional[str] = None
     # 秩乱给你的token
     yinying_token: Optional[str] = None
     # 插件数据文件存储路径，可不填。
     hx_path: Optional[str] = None
     # 图像检查api，爱来自阿里云
```

### Comparing `nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/image_check.py` & `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/image_check.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/report.py` & `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/report.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying/smms.py` & `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying/smms.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.3.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.3.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.3.0
+Version: 1.3.1
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.3.1 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.3.0/setup.py` & `nonebot-plugin-hx-yinying-1.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.3.0",
+    version="1.3.01",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

