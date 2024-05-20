# Comparing `tmp/nonebot2-2.3.0.tar.gz` & `tmp/nonebot2-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot2-2.3.0.tar", max compression
+gzip compressed data, was "nonebot2-2.3.1.tar", max compression
```

## Comparing `nonebot2-2.3.0.tar` & `nonebot2-2.3.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1078 2024-05-01 09:02:00.544923 nonebot2-2.3.0/LICENSE
--rw-r--r--   0        0        0    20697 2024-05-01 09:02:00.544923 nonebot2-2.3.0/README.md
--rw-r--r--   0        0        0    12601 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/__init__.py
--rw-r--r--   0        0        0      913 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/adapters/__init__.py
--rw-r--r--   0        0        0    12802 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/compat.py
--rw-r--r--   0        0        0    16345 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/config.py
--rw-r--r--   0        0        0     1863 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/consts.py
--rw-r--r--   0        0        0     6295 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/dependencies/__init__.py
--rw-r--r--   0        0        0     1693 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/dependencies/utils.py
--rw-r--r--   0        0        0     1845 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/__init__.py
--rw-r--r--   0        0        0     8202 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/aiohttp.py
--rw-r--r--   0        0        0     9770 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/fastapi.py
--rw-r--r--   0        0        0     4186 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/httpx.py
--rw-r--r--   0        0        0     4113 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/none.py
--rw-r--r--   0        0        0     8535 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/quart.py
--rw-r--r--   0        0        0     3773 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/drivers/websockets.py
--rw-r--r--   0        0        0     6462 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/exception.py
--rw-r--r--   0        0        0        0 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/__init__.py
--rw-r--r--   0        0        0      253 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/__init__.py
--rw-r--r--   0        0        0     3968 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/adapter.py
--rw-r--r--   0        0        0     5191 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/bot.py
--rw-r--r--   0        0        0     2926 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/event.py
--rw-r--r--   0        0        0    12912 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/message.py
--rw-r--r--   0        0        0     7495 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/adapter/template.py
--rw-r--r--   0        0        0     1450 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/__init__.py
--rw-r--r--   0        0        0     1799 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/_lifespan.py
--rw-r--r--   0        0        0    10962 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/abstract.py
--rw-r--r--   0        0        0     1160 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/combine.py
--rw-r--r--   0        0        0    11376 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/driver/model.py
--rw-r--r--   0        0        0      516 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/matcher/__init__.py
--rw-r--r--   0        0        0     2823 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/matcher/manager.py
--rw-r--r--   0        0        0    29452 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/matcher/matcher.py
--rw-r--r--   0        0        0      746 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/matcher/provider.py
--rw-r--r--   0        0        0    17537 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/params.py
--rw-r--r--   0        0        0     5707 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/permission.py
--rw-r--r--   0        0        0     3219 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/internal/rule.py
--rw-r--r--   0        0        0     2636 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/log.py
--rw-r--r--   0        0        0     1057 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/matcher.py
--rw-r--r--   0        0        0    15429 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/message.py
--rw-r--r--   0        0        0     6487 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/params.py
--rw-r--r--   0        0        0     3063 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/permission.py
--rw-r--r--   0        0        0     7673 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/__init__.py
--rw-r--r--   0        0        0     6905 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/load.py
--rw-r--r--   0        0        0     9076 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/manager.py
--rw-r--r--   0        0        0     2669 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/model.py
--rw-r--r--   0        0        0    30978 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/on.py
--rw-r--r--   0        0        0    14583 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugin/on.pyi
--rw-r--r--   0        0        0      669 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugins/echo.py
--rw-r--r--   0        0        0     1262 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/plugins/single_session.py
--rw-r--r--   0        0        0        0 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/py.typed
--rw-r--r--   0        0        0    23027 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/rule.py
--rw-r--r--   0        0        0     6964 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/typing.py
--rw-r--r--   0        0        0     9444 2024-05-01 09:02:00.548923 nonebot2-2.3.0/nonebot/utils.py
--rw-r--r--   0        0        0     3663 2024-05-01 09:02:00.552923 nonebot2-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    22766 1970-01-01 00:00:00.000000 nonebot2-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-20 14:20:22.551958 nonebot2-2.3.1/LICENSE
+-rw-r--r--   0        0        0    21144 2024-05-20 14:20:22.551958 nonebot2-2.3.1/README.md
+-rw-r--r--   0        0        0    12601 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/__init__.py
+-rw-r--r--   0        0        0      913 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/adapters/__init__.py
+-rw-r--r--   0        0        0    12802 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/compat.py
+-rw-r--r--   0        0        0    16345 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/config.py
+-rw-r--r--   0        0        0     1863 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/consts.py
+-rw-r--r--   0        0        0     6295 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/dependencies/__init__.py
+-rw-r--r--   0        0        0     1693 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/dependencies/utils.py
+-rw-r--r--   0        0        0     1845 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/drivers/__init__.py
+-rw-r--r--   0        0        0     8202 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/drivers/aiohttp.py
+-rw-r--r--   0        0        0     9770 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/drivers/fastapi.py
+-rw-r--r--   0        0        0     4186 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/drivers/httpx.py
+-rw-r--r--   0        0        0     4113 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/drivers/none.py
+-rw-r--r--   0        0        0     8535 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/drivers/quart.py
+-rw-r--r--   0        0        0     3773 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/drivers/websockets.py
+-rw-r--r--   0        0        0     6462 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/exception.py
+-rw-r--r--   0        0        0        0 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/internal/__init__.py
+-rw-r--r--   0        0        0      253 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/internal/adapter/__init__.py
+-rw-r--r--   0        0        0     3968 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/internal/adapter/adapter.py
+-rw-r--r--   0        0        0     5191 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/internal/adapter/bot.py
+-rw-r--r--   0        0        0     2926 2024-05-20 14:20:22.555958 nonebot2-2.3.1/nonebot/internal/adapter/event.py
+-rw-r--r--   0        0        0    12912 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/adapter/message.py
+-rw-r--r--   0        0        0     7495 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/adapter/template.py
+-rw-r--r--   0        0        0     1450 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/driver/__init__.py
+-rw-r--r--   0        0        0     1799 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/driver/_lifespan.py
+-rw-r--r--   0        0        0    10962 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/driver/abstract.py
+-rw-r--r--   0        0        0     1160 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/driver/combine.py
+-rw-r--r--   0        0        0    11376 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/driver/model.py
+-rw-r--r--   0        0        0      516 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/matcher/__init__.py
+-rw-r--r--   0        0        0     2823 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/matcher/manager.py
+-rw-r--r--   0        0        0    29452 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/matcher/matcher.py
+-rw-r--r--   0        0        0      746 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/matcher/provider.py
+-rw-r--r--   0        0        0    17686 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/params.py
+-rw-r--r--   0        0        0     5707 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/permission.py
+-rw-r--r--   0        0        0     3219 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/internal/rule.py
+-rw-r--r--   0        0        0     2636 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/log.py
+-rw-r--r--   0        0        0     1057 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/matcher.py
+-rw-r--r--   0        0        0    15429 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/message.py
+-rw-r--r--   0        0        0     6487 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/params.py
+-rw-r--r--   0        0        0     3063 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/permission.py
+-rw-r--r--   0        0        0     7673 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/plugin/__init__.py
+-rw-r--r--   0        0        0     6905 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/plugin/load.py
+-rw-r--r--   0        0        0     9076 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/plugin/manager.py
+-rw-r--r--   0        0        0     2669 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/plugin/model.py
+-rw-r--r--   0        0        0    30978 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/plugin/on.py
+-rw-r--r--   0        0        0    14583 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/plugin/on.pyi
+-rw-r--r--   0        0        0      669 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/plugins/echo.py
+-rw-r--r--   0        0        0     1262 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/plugins/single_session.py
+-rw-r--r--   0        0        0        0 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/py.typed
+-rw-r--r--   0        0        0    23027 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/rule.py
+-rw-r--r--   0        0        0     7172 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/typing.py
+-rw-r--r--   0        0        0     9444 2024-05-20 14:20:22.559959 nonebot2-2.3.1/nonebot/utils.py
+-rw-r--r--   0        0        0     3663 2024-05-20 14:20:22.559959 nonebot2-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0    23213 1970-01-01 00:00:00.000000 nonebot2-2.3.1/PKG-INFO
```

### Comparing `nonebot2-2.3.0/LICENSE` & `nonebot2-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/README.md` & `nonebot2-2.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,23 +119,25 @@
   |                QQ（[仓库](https://github.com/nonebot/adapter-qq)，[协议](https://bot.q.qq.com/wiki/)）                |  ✅  |                            QQ 官方接口调整较多                            |
   |                             Console（[仓库](https://github.com/nonebot/adapter-console)）                             |  ✅  |                                控制台交互                                 |
   |     Red（[仓库](https://github.com/nonebot/adapter-red)，[协议](https://chrononeko.github.io/QQNTRedProtocol/)）      |  ✅  |                                  QQ 协议                                  |
   |           Satori（[仓库](https://github.com/nonebot/adapter-satori)，[协议](https://satori.js.org/zh-CN)）            |  ✅  |               支持 Onebot、TG、飞书、微信公众号、Koishi 等                |
   |   Discord（[仓库](https://github.com/nonebot/adapter-discord)，[协议](https://discord.com/developers/docs/intro)）    |  ✅  |                             Discord Bot 协议                              |
   |               DoDo（[仓库](https://github.com/nonebot/adapter-dodo)，[协议](https://open.imdodo.com/)）               |  ✅  |                               DoDo Bot 协议                               |
   |        Kritor（[仓库](https://github.com/nonebot/adapter-kritor)，[协议](https://github.com/KarinJS/kritor)）         |  ✅  |                 Kritor (OnebotX) 协议，QQ 机器人接口标准                  |
+  |    Mirai（[仓库](https://github.com/nonebot/adapter-mirai)，[协议](https://docs.mirai.mamoe.net/mirai-api-http/)）    |  ✅  |                                  QQ 协议                                  |
   |         钉钉（[仓库](https://github.com/nonebot/adapter-ding)，[协议](https://open.dingtalk.com/document/)）          |  🤗  |                        寻找 Maintainer（暂不可用）                        |
   |     开黑啦（[仓库](https://github.com/Tian-que/nonebot-adapter-kaiheila)，[协议](https://developer.kookapp.cn/)）     |  ↗️  |                                由社区贡献                                 |
   | Mirai（[仓库](https://github.com/ieew/nonebot_adapter_mirai2)，[协议](https://docs.mirai.mamoe.net/mirai-api-http/)） |  ↗️  |                            QQ 协议，由社区贡献                            |
   |                          Ntchat（[仓库](https://github.com/JustUndertaker/adapter-ntchat)）                           |  ↗️  |                           微信协议，由社区贡献                            |
   |                      MineCraft（[仓库](https://github.com/17TheWord/nonebot-adapter-minecraft)）                      |  ↗️  |                                由社区贡献                                 |
   |                          BiliBili Live（[仓库](https://github.com/wwweww/adapter-bilibili)）                          |  ↗️  |                                由社区贡献                                 |
   |                       Walle-Q（[仓库](https://github.com/onebot-walle/nonebot_adapter_walleq)）                       |  ↗️  |                            QQ 协议，由社区贡献                            |
   |                       Villa（[仓库](https://github.com/CMHopeSunshine/nonebot-adapter-villa)）                        |  ❌  |                     米游社大别野 Bot 协议，官方已下线                     |
   | Rocket.Chat（[仓库](https://github.com/IUnlimit/nonebot-adapter-rocketchat)，[协议](https://developer.rocket.chat/)） |  ↗️  |                     Rocket.Chat Bot 协议，由社区贡献                      |
+  |     Tailchat（[仓库](https://github.com/eya46/nonebot-adapter-tailchat)，[协议](https://tailchat.msgbyte.com/)）      |  ↗️  |                  Tailchat 开放平台 Bot 协议，由社区贡献                   |
 
 - 坚实后盾：支持多种 web 框架，可自定义替换、组合
 
   |                              驱动框架                               |  类型  |
   | :-----------------------------------------------------------------: | :----: |
   |              [FastAPI](https://fastapi.tiangolo.com/)               | 服务端 |
   | [Quart](https://quart.palletsprojects.com/en/latest/)（异步 Flask） | 服务端 |
```

#### html2text {}

```diff
@@ -41,40 +41,44 @@
 satori.js.org/zh-CN)ï¼ | â | æ¯æ
 OnebotãTGãé£ä¹¦ãå¾®ä¿¡å¬ä¼å·ãKoishi ç­ | | Discordï¼[ä»åº]
 (https://github.com/nonebot/adapter-discord)ï¼[åè®®](https://discord.com/
 developers/docs/intro)ï¼ | â | Discord Bot åè®® | | DoDoï¼[ä»åº](https:
 //github.com/nonebot/adapter-dodo)ï¼[åè®®](https://open.imdodo.com/)ï¼ |
 â | DoDo Bot åè®® | | Kritorï¼[ä»åº](https://github.com/nonebot/adapter-
 kritor)ï¼[åè®®](https://github.com/KarinJS/kritor)ï¼ | â | Kritor
-(OnebotX) åè®®ï¼QQ æºå¨äººæ¥å£æ å | | ééï¼[ä»åº](https://
-github.com/nonebot/adapter-ding)ï¼[åè®®](https://open.dingtalk.com/document/
-)ï¼ | ð¤ | å¯»æ¾ Maintainerï¼æä¸å¯ç¨ï¼ | | å¼é»å¦ï¼[ä»åº]
-(https://github.com/Tian-que/nonebot-adapter-kaiheila)ï¼[åè®®](https://
+(OnebotX) åè®®ï¼QQ æºå¨äººæ¥å£æ å | | Miraiï¼[ä»åº](https://
+github.com/nonebot/adapter-mirai)ï¼[åè®®](https://docs.mirai.mamoe.net/
+mirai-api-http/)ï¼ | â | QQ åè®® | | ééï¼[ä»åº](https://github.com/
+nonebot/adapter-ding)ï¼[åè®®](https://open.dingtalk.com/document/)ï¼ | ð¤
+| å¯»æ¾ Maintainerï¼æä¸å¯ç¨ï¼ | | å¼é»å¦ï¼[ä»åº](https://
+github.com/Tian-que/nonebot-adapter-kaiheila)ï¼[åè®®](https://
 developer.kookapp.cn/)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® | | Miraiï¼[ä»åº]
 (https://github.com/ieew/nonebot_adapter_mirai2)ï¼[åè®®](https://
 docs.mirai.mamoe.net/mirai-api-http/)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç®
 | | Ntchatï¼[ä»åº](https://github.com/JustUndertaker/adapter-ntchat)ï¼ |
 âï¸ | å¾®ä¿¡åè®®ï¼ç±ç¤¾åºè´¡ç® | | MineCraftï¼[ä»åº](https://
 github.com/17TheWord/nonebot-adapter-minecraft)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® |
 | BiliBili Liveï¼[ä»åº](https://github.com/wwweww/adapter-bilibili)ï¼ |
 âï¸ | ç±ç¤¾åºè´¡ç® | | Walle-Qï¼[ä»åº](https://github.com/onebot-
 walle/nonebot_adapter_walleq)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç® | |
 Villaï¼[ä»åº](https://github.com/CMHopeSunshine/nonebot-adapter-villa)ï¼ |
 â | ç±³æ¸¸ç¤¾å¤§å«é Bot åè®®ï¼å®æ¹å·²ä¸çº¿ | | Rocket.Chatï¼
 [ä»åº](https://github.com/IUnlimit/nonebot-adapter-rocketchat)ï¼[åè®®]
 (https://developer.rocket.chat/)ï¼ | âï¸ | Rocket.Chat Bot
-åè®®ï¼ç±ç¤¾åºè´¡ç® | - åå®åç¾ï¼æ¯æå¤ç§ web
-æ¡æ¶ï¼å¯èªå®ä¹æ¿æ¢ãç»å | é©±å¨æ¡æ¶ | ç±»å | | :-------------
-----------------------------------------------------: | :----: | | [FastAPI]
-(https://fastapi.tiangolo.com/) | æå¡ç«¯ | | [Quart](https://
-quart.palletsprojects.com/en/latest/)ï¼å¼æ­¥ Flaskï¼ | æå¡ç«¯ | |
-[aiohttp](https://docs.aiohttp.org/en/stable/) | å®¢æ·ç«¯ | | [httpx](https://
-www.python-httpx.org/) | å®¢æ·ç«¯ | | [websockets](https://
-websockets.readthedocs.io/en/stable/) | å®¢æ·ç«¯ | æ´å¤ï¼[æ¦è§](https://
-nonebot.dev/docs/) ## ä»ä¹ä¸æ¯ NoneBot2 NoneBot2
+åè®®ï¼ç±ç¤¾åºè´¡ç® | | Tailchatï¼[ä»åº](https://github.com/eya46/
+nonebot-adapter-tailchat)ï¼[åè®®](https://tailchat.msgbyte.com/)ï¼ | âï¸
+| Tailchat å¼æ¾å¹³å° Bot åè®®ï¼ç±ç¤¾åºè´¡ç® | -
+åå®åç¾ï¼æ¯æå¤ç§ web æ¡æ¶ï¼å¯èªå®ä¹æ¿æ¢ãç»å |
+é©±å¨æ¡æ¶ | ç±»å | | :----------------------------------------------------
+-------------: | :----: | | [FastAPI](https://fastapi.tiangolo.com/) |
+æå¡ç«¯ | | [Quart](https://quart.palletsprojects.com/en/latest/)ï¼å¼æ­¥
+Flaskï¼ | æå¡ç«¯ | | [aiohttp](https://docs.aiohttp.org/en/stable/) |
+å®¢æ·ç«¯ | | [httpx](https://www.python-httpx.org/) | å®¢æ·ç«¯ | |
+[websockets](https://websockets.readthedocs.io/en/stable/) | å®¢æ·ç«¯ |
+æ´å¤ï¼[æ¦è§](https://nonebot.dev/docs/) ## ä»ä¹ä¸æ¯ NoneBot2 NoneBot2
 ä¸æ¯æä¸ªå¹³å°æèåè®®çå·ä½å®ç°ï¼å®åªè´è´£åå·²æåè®®ééå¨éä¿¡ï¼å¹¶å¤çæ¥æ¶å°çäºä»¶ãæä»¥ï¼âNoneBot
 æ blabla å¹³å°ç blabla åè½åï¼âè¿ç§é®é¢æ¯ä¸ NoneBot2
 æ å³çãè¯·å¨ç¸åºå¹³å°çåè½ææ¡£ä¸­ç¡®è®¤ï¼æä¸ç¸åºå¹³å°çåè®®ééå¼åèèç³»ã
 NoneBot2 ä¸æ¯ NoneBot1
 çæ¿ä»£åãäºå®ä¸ï¼å®ä»¬é½å¨è¢«ç§¯æçç»´æ¤çãä½æ¯ï¼å¦æä½ æ³å°è¯ä¸äºæ°åè½ï¼æèæ³è¦æ¯ææ´å¤çå¹³å°ï¼å¯ä»¥èèä½¿ç¨
 NoneBot2ã > ~~NoneBot2 å NoneBot1 çåºå«ï¼å°±åæ¯ VisualStudio Code
 å VisualStudio ä¸æ ·~~ ## å³å»å¼å§ ~~å®æ´~~ææ¡£å¯ä»¥å¨ [è¿é]
```

### Comparing `nonebot2-2.3.0/nonebot/__init__.py` & `nonebot2-2.3.1/nonebot/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/adapters/__init__.py` & `nonebot2-2.3.1/nonebot/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/compat.py` & `nonebot2-2.3.1/nonebot/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/config.py` & `nonebot2-2.3.1/nonebot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/consts.py` & `nonebot2-2.3.1/nonebot/consts.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/dependencies/__init__.py` & `nonebot2-2.3.1/nonebot/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/dependencies/utils.py` & `nonebot2-2.3.1/nonebot/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/drivers/__init__.py` & `nonebot2-2.3.1/nonebot/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/drivers/aiohttp.py` & `nonebot2-2.3.1/nonebot/drivers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/drivers/fastapi.py` & `nonebot2-2.3.1/nonebot/drivers/fastapi.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/drivers/httpx.py` & `nonebot2-2.3.1/nonebot/drivers/httpx.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/drivers/none.py` & `nonebot2-2.3.1/nonebot/drivers/none.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/drivers/quart.py` & `nonebot2-2.3.1/nonebot/drivers/quart.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/drivers/websockets.py` & `nonebot2-2.3.1/nonebot/drivers/websockets.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/exception.py` & `nonebot2-2.3.1/nonebot/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/adapter/adapter.py` & `nonebot2-2.3.1/nonebot/internal/adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/adapter/bot.py` & `nonebot2-2.3.1/nonebot/internal/adapter/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/adapter/event.py` & `nonebot2-2.3.1/nonebot/internal/adapter/event.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/adapter/message.py` & `nonebot2-2.3.1/nonebot/internal/adapter/message.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/adapter/template.py` & `nonebot2-2.3.1/nonebot/internal/adapter/template.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/driver/__init__.py` & `nonebot2-2.3.1/nonebot/internal/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/driver/_lifespan.py` & `nonebot2-2.3.1/nonebot/internal/driver/_lifespan.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/driver/abstract.py` & `nonebot2-2.3.1/nonebot/internal/driver/abstract.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/driver/combine.py` & `nonebot2-2.3.1/nonebot/internal/driver/combine.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/driver/model.py` & `nonebot2-2.3.1/nonebot/internal/driver/model.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/matcher/__init__.py` & `nonebot2-2.3.1/nonebot/internal/matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/matcher/manager.py` & `nonebot2-2.3.1/nonebot/internal/matcher/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/matcher/matcher.py` & `nonebot2-2.3.1/nonebot/internal/matcher/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/matcher/provider.py` & `nonebot2-2.3.1/nonebot/internal/matcher/provider.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/params.py` & `nonebot2-2.3.1/nonebot/internal/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,22 @@
     cast,
 )
 
 from pydantic.fields import FieldInfo as PydanticFieldInfo
 
 from nonebot.dependencies import Param, Dependent
 from nonebot.dependencies.utils import check_field_type
-from nonebot.typing import T_State, T_Handler, T_DependencyCache
 from nonebot.compat import FieldInfo, ModelField, PydanticUndefined, extract_field_info
+from nonebot.typing import (
+    _STATE_FLAG,
+    T_State,
+    T_Handler,
+    T_DependencyCache,
+    origin_is_annotated,
+)
 from nonebot.utils import (
     get_name,
     run_sync,
     is_gen_callable,
     run_sync_ctx_manager,
     is_async_gen_callable,
     is_coroutine_callable,
@@ -345,15 +351,17 @@
 
     @classmethod
     @override
     def _check_param(
         cls, param: inspect.Parameter, allow_types: tuple[type[Param], ...]
     ) -> Optional[Self]:
         # param type is T_State
-        if param.annotation is T_State:
+        if origin_is_annotated(
+            get_origin(param.annotation)
+        ) and _STATE_FLAG in get_args(param.annotation):
             return cls()
         # legacy: param is named "state" and has no type annotation
         elif param.annotation == param.empty and param.name == "state":
             return cls()
 
     @override
     async def _solve(  # pyright: ignore[reportIncompatibleMethodOverride]
```

### Comparing `nonebot2-2.3.0/nonebot/internal/permission.py` & `nonebot2-2.3.1/nonebot/internal/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/internal/rule.py` & `nonebot2-2.3.1/nonebot/internal/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/log.py` & `nonebot2-2.3.1/nonebot/log.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/matcher.py` & `nonebot2-2.3.1/nonebot/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/message.py` & `nonebot2-2.3.1/nonebot/message.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/params.py` & `nonebot2-2.3.1/nonebot/params.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/permission.py` & `nonebot2-2.3.1/nonebot/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/plugin/__init__.py` & `nonebot2-2.3.1/nonebot/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/plugin/load.py` & `nonebot2-2.3.1/nonebot/plugin/load.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/plugin/manager.py` & `nonebot2-2.3.1/nonebot/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/plugin/model.py` & `nonebot2-2.3.1/nonebot/plugin/model.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/plugin/on.py` & `nonebot2-2.3.1/nonebot/plugin/on.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/plugin/on.pyi` & `nonebot2-2.3.1/nonebot/plugin/on.pyi`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/plugins/echo.py` & `nonebot2-2.3.1/nonebot/plugins/echo.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/plugins/single_session.py` & `nonebot2-2.3.1/nonebot/plugins/single_session.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/rule.py` & `nonebot2-2.3.1/nonebot/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/nonebot/typing.py` & `nonebot2-2.3.1/nonebot/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,15 +104,23 @@
 def evaluate_forwardref(
     ref: t.ForwardRef, globalns: dict[str, t.Any], localns: dict[str, t.Any]
 ) -> t.Any:
     return ref._evaluate(globalns, localns, frozenset())
 
 
 # state
-T_State: TypeAlias = dict[t.Any, t.Any]
+# use annotated flag to avoid ForwardRef recreate generic type (py >= 3.11)
+class StateFlag:
+    def __repr__(self) -> str:
+        return "StateFlag()"
+
+
+_STATE_FLAG = StateFlag()
+
+T_State: TypeAlias = t.Annotated[dict[t.Any, t.Any], _STATE_FLAG]
 """事件处理状态 State 类型"""
 
 _DependentCallable: TypeAlias = t.Union[
     t.Callable[..., T], t.Callable[..., t.Awaitable[T]]
 ]
 
 # driver hooks
```

### Comparing `nonebot2-2.3.0/nonebot/utils.py` & `nonebot2-2.3.1/nonebot/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.3.0/pyproject.toml` & `nonebot2-2.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot2"
-version = "2.3.0"
+version = "2.3.1"
 description = "An asynchronous python bot framework."
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://nonebot.dev/"
 repository = "https://github.com/nonebot/nonebot2"
 documentation = "https://nonebot.dev/"
```

### Comparing `nonebot2-2.3.0/PKG-INFO` & `nonebot2-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot2
-Version: 2.3.0
+Version: 2.3.1
 Summary: An asynchronous python bot framework.
 Home-page: https://nonebot.dev/
 License: MIT
 Keywords: bot,qq,qqbot,mirai,coolq
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.9,<4.0
@@ -165,23 +165,25 @@
   |                QQ（[仓库](https://github.com/nonebot/adapter-qq)，[协议](https://bot.q.qq.com/wiki/)）                |  ✅  |                            QQ 官方接口调整较多                            |
   |                             Console（[仓库](https://github.com/nonebot/adapter-console)）                             |  ✅  |                                控制台交互                                 |
   |     Red（[仓库](https://github.com/nonebot/adapter-red)，[协议](https://chrononeko.github.io/QQNTRedProtocol/)）      |  ✅  |                                  QQ 协议                                  |
   |           Satori（[仓库](https://github.com/nonebot/adapter-satori)，[协议](https://satori.js.org/zh-CN)）            |  ✅  |               支持 Onebot、TG、飞书、微信公众号、Koishi 等                |
   |   Discord（[仓库](https://github.com/nonebot/adapter-discord)，[协议](https://discord.com/developers/docs/intro)）    |  ✅  |                             Discord Bot 协议                              |
   |               DoDo（[仓库](https://github.com/nonebot/adapter-dodo)，[协议](https://open.imdodo.com/)）               |  ✅  |                               DoDo Bot 协议                               |
   |        Kritor（[仓库](https://github.com/nonebot/adapter-kritor)，[协议](https://github.com/KarinJS/kritor)）         |  ✅  |                 Kritor (OnebotX) 协议，QQ 机器人接口标准                  |
+  |    Mirai（[仓库](https://github.com/nonebot/adapter-mirai)，[协议](https://docs.mirai.mamoe.net/mirai-api-http/)）    |  ✅  |                                  QQ 协议                                  |
   |         钉钉（[仓库](https://github.com/nonebot/adapter-ding)，[协议](https://open.dingtalk.com/document/)）          |  🤗  |                        寻找 Maintainer（暂不可用）                        |
   |     开黑啦（[仓库](https://github.com/Tian-que/nonebot-adapter-kaiheila)，[协议](https://developer.kookapp.cn/)）     |  ↗️  |                                由社区贡献                                 |
   | Mirai（[仓库](https://github.com/ieew/nonebot_adapter_mirai2)，[协议](https://docs.mirai.mamoe.net/mirai-api-http/)） |  ↗️  |                            QQ 协议，由社区贡献                            |
   |                          Ntchat（[仓库](https://github.com/JustUndertaker/adapter-ntchat)）                           |  ↗️  |                           微信协议，由社区贡献                            |
   |                      MineCraft（[仓库](https://github.com/17TheWord/nonebot-adapter-minecraft)）                      |  ↗️  |                                由社区贡献                                 |
   |                          BiliBili Live（[仓库](https://github.com/wwweww/adapter-bilibili)）                          |  ↗️  |                                由社区贡献                                 |
   |                       Walle-Q（[仓库](https://github.com/onebot-walle/nonebot_adapter_walleq)）                       |  ↗️  |                            QQ 协议，由社区贡献                            |
   |                       Villa（[仓库](https://github.com/CMHopeSunshine/nonebot-adapter-villa)）                        |  ❌  |                     米游社大别野 Bot 协议，官方已下线                     |
   | Rocket.Chat（[仓库](https://github.com/IUnlimit/nonebot-adapter-rocketchat)，[协议](https://developer.rocket.chat/)） |  ↗️  |                     Rocket.Chat Bot 协议，由社区贡献                      |
+  |     Tailchat（[仓库](https://github.com/eya46/nonebot-adapter-tailchat)，[协议](https://tailchat.msgbyte.com/)）      |  ↗️  |                  Tailchat 开放平台 Bot 协议，由社区贡献                   |
 
 - 坚实后盾：支持多种 web 框架，可自定义替换、组合
 
   |                              驱动框架                               |  类型  |
   | :-----------------------------------------------------------------: | :----: |
   |              [FastAPI](https://fastapi.tiangolo.com/)               | 服务端 |
   | [Quart](https://quart.palletsprojects.com/en/latest/)（异步 Flask） | 服务端 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot2 Version: 2.3.0 Summary: An asynchronous
+Metadata-Version: 2.1 Name: nonebot2 Version: 2.3.1 Summary: An asynchronous
 python bot framework. Home-page: https://nonebot.dev/ License: MIT Keywords:
 bot,qq,qqbot,mirai,coolq Author: yanyongyu Author-email: yyy@nonebot.dev
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
 Framework :: Library Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -69,40 +69,44 @@
 satori.js.org/zh-CN)ï¼ | â | æ¯æ
 OnebotãTGãé£ä¹¦ãå¾®ä¿¡å¬ä¼å·ãKoishi ç­ | | Discordï¼[ä»åº]
 (https://github.com/nonebot/adapter-discord)ï¼[åè®®](https://discord.com/
 developers/docs/intro)ï¼ | â | Discord Bot åè®® | | DoDoï¼[ä»åº](https:
 //github.com/nonebot/adapter-dodo)ï¼[åè®®](https://open.imdodo.com/)ï¼ |
 â | DoDo Bot åè®® | | Kritorï¼[ä»åº](https://github.com/nonebot/adapter-
 kritor)ï¼[åè®®](https://github.com/KarinJS/kritor)ï¼ | â | Kritor
-(OnebotX) åè®®ï¼QQ æºå¨äººæ¥å£æ å | | ééï¼[ä»åº](https://
-github.com/nonebot/adapter-ding)ï¼[åè®®](https://open.dingtalk.com/document/
-)ï¼ | ð¤ | å¯»æ¾ Maintainerï¼æä¸å¯ç¨ï¼ | | å¼é»å¦ï¼[ä»åº]
-(https://github.com/Tian-que/nonebot-adapter-kaiheila)ï¼[åè®®](https://
+(OnebotX) åè®®ï¼QQ æºå¨äººæ¥å£æ å | | Miraiï¼[ä»åº](https://
+github.com/nonebot/adapter-mirai)ï¼[åè®®](https://docs.mirai.mamoe.net/
+mirai-api-http/)ï¼ | â | QQ åè®® | | ééï¼[ä»åº](https://github.com/
+nonebot/adapter-ding)ï¼[åè®®](https://open.dingtalk.com/document/)ï¼ | ð¤
+| å¯»æ¾ Maintainerï¼æä¸å¯ç¨ï¼ | | å¼é»å¦ï¼[ä»åº](https://
+github.com/Tian-que/nonebot-adapter-kaiheila)ï¼[åè®®](https://
 developer.kookapp.cn/)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® | | Miraiï¼[ä»åº]
 (https://github.com/ieew/nonebot_adapter_mirai2)ï¼[åè®®](https://
 docs.mirai.mamoe.net/mirai-api-http/)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç®
 | | Ntchatï¼[ä»åº](https://github.com/JustUndertaker/adapter-ntchat)ï¼ |
 âï¸ | å¾®ä¿¡åè®®ï¼ç±ç¤¾åºè´¡ç® | | MineCraftï¼[ä»åº](https://
 github.com/17TheWord/nonebot-adapter-minecraft)ï¼ | âï¸ | ç±ç¤¾åºè´¡ç® |
 | BiliBili Liveï¼[ä»åº](https://github.com/wwweww/adapter-bilibili)ï¼ |
 âï¸ | ç±ç¤¾åºè´¡ç® | | Walle-Qï¼[ä»åº](https://github.com/onebot-
 walle/nonebot_adapter_walleq)ï¼ | âï¸ | QQ åè®®ï¼ç±ç¤¾åºè´¡ç® | |
 Villaï¼[ä»åº](https://github.com/CMHopeSunshine/nonebot-adapter-villa)ï¼ |
 â | ç±³æ¸¸ç¤¾å¤§å«é Bot åè®®ï¼å®æ¹å·²ä¸çº¿ | | Rocket.Chatï¼
 [ä»åº](https://github.com/IUnlimit/nonebot-adapter-rocketchat)ï¼[åè®®]
 (https://developer.rocket.chat/)ï¼ | âï¸ | Rocket.Chat Bot
-åè®®ï¼ç±ç¤¾åºè´¡ç® | - åå®åç¾ï¼æ¯æå¤ç§ web
-æ¡æ¶ï¼å¯èªå®ä¹æ¿æ¢ãç»å | é©±å¨æ¡æ¶ | ç±»å | | :-------------
-----------------------------------------------------: | :----: | | [FastAPI]
-(https://fastapi.tiangolo.com/) | æå¡ç«¯ | | [Quart](https://
-quart.palletsprojects.com/en/latest/)ï¼å¼æ­¥ Flaskï¼ | æå¡ç«¯ | |
-[aiohttp](https://docs.aiohttp.org/en/stable/) | å®¢æ·ç«¯ | | [httpx](https://
-www.python-httpx.org/) | å®¢æ·ç«¯ | | [websockets](https://
-websockets.readthedocs.io/en/stable/) | å®¢æ·ç«¯ | æ´å¤ï¼[æ¦è§](https://
-nonebot.dev/docs/) ## ä»ä¹ä¸æ¯ NoneBot2 NoneBot2
+åè®®ï¼ç±ç¤¾åºè´¡ç® | | Tailchatï¼[ä»åº](https://github.com/eya46/
+nonebot-adapter-tailchat)ï¼[åè®®](https://tailchat.msgbyte.com/)ï¼ | âï¸
+| Tailchat å¼æ¾å¹³å° Bot åè®®ï¼ç±ç¤¾åºè´¡ç® | -
+åå®åç¾ï¼æ¯æå¤ç§ web æ¡æ¶ï¼å¯èªå®ä¹æ¿æ¢ãç»å |
+é©±å¨æ¡æ¶ | ç±»å | | :----------------------------------------------------
+-------------: | :----: | | [FastAPI](https://fastapi.tiangolo.com/) |
+æå¡ç«¯ | | [Quart](https://quart.palletsprojects.com/en/latest/)ï¼å¼æ­¥
+Flaskï¼ | æå¡ç«¯ | | [aiohttp](https://docs.aiohttp.org/en/stable/) |
+å®¢æ·ç«¯ | | [httpx](https://www.python-httpx.org/) | å®¢æ·ç«¯ | |
+[websockets](https://websockets.readthedocs.io/en/stable/) | å®¢æ·ç«¯ |
+æ´å¤ï¼[æ¦è§](https://nonebot.dev/docs/) ## ä»ä¹ä¸æ¯ NoneBot2 NoneBot2
 ä¸æ¯æä¸ªå¹³å°æèåè®®çå·ä½å®ç°ï¼å®åªè´è´£åå·²æåè®®ééå¨éä¿¡ï¼å¹¶å¤çæ¥æ¶å°çäºä»¶ãæä»¥ï¼âNoneBot
 æ blabla å¹³å°ç blabla åè½åï¼âè¿ç§é®é¢æ¯ä¸ NoneBot2
 æ å³çãè¯·å¨ç¸åºå¹³å°çåè½ææ¡£ä¸­ç¡®è®¤ï¼æä¸ç¸åºå¹³å°çåè®®ééå¼åèèç³»ã
 NoneBot2 ä¸æ¯ NoneBot1
 çæ¿ä»£åãäºå®ä¸ï¼å®ä»¬é½å¨è¢«ç§¯æçç»´æ¤çãä½æ¯ï¼å¦æä½ æ³å°è¯ä¸äºæ°åè½ï¼æèæ³è¦æ¯ææ´å¤çå¹³å°ï¼å¯ä»¥èèä½¿ç¨
 NoneBot2ã > ~~NoneBot2 å NoneBot1 çåºå«ï¼å°±åæ¯ VisualStudio Code
 å VisualStudio ä¸æ ·~~ ## å³å»å¼å§ ~~å®æ´~~ææ¡£å¯ä»¥å¨ [è¿é]
```

