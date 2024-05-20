# Comparing `tmp/halchat-0.0.1.tar.gz` & `tmp/halchat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halchat-0.0.1.tar", last modified: Sun May 12 14:05:59 2024, max compression
+gzip compressed data, was "halchat-0.0.2.tar", last modified: Mon May 20 17:53:07 2024, max compression
```

## Comparing `halchat-0.0.1.tar` & `halchat-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 14:05:59.323113 halchat-0.0.1/
--rw-rw-rw-   0        0        0     1090 2024-05-12 13:55:45.000000 halchat-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      480 2024-05-12 14:05:59.322115 halchat-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       49 2024-05-12 13:59:25.000000 halchat-0.0.1/README.md
--rw-rw-rw-   0        0        0      423 2024-05-12 14:05:13.000000 halchat-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 14:05:59.323113 halchat-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-12 14:05:59.306594 halchat-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-12 14:05:59.321109 halchat-0.0.1/src/HalChat.egg-info/
--rw-rw-rw-   0        0        0      480 2024-05-12 14:05:59.000000 halchat-0.0.1/src/HalChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-12 14:05:59.000000 halchat-0.0.1/src/HalChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 14:05:59.000000 halchat-0.0.1/src/HalChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 14:05:59.000000 halchat-0.0.1/src/HalChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7342 2024-05-12 13:47:32.000000 halchat-0.0.1/src/HalChatAPI.py
--rw-rw-rw-   0        0        0     1702 2024-02-12 15:42:01.000000 halchat-0.0.1/src/HalEncryption.py
--rw-rw-rw-   0        0        0     2724 2024-02-12 16:04:02.000000 halchat-0.0.1/src/HalHash.py
--rw-rw-rw-   0        0        0        0 2024-05-12 13:57:45.000000 halchat-0.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 17:53:07.148060 halchat-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-12 13:55:45.000000 halchat-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      480 2024-05-20 17:53:07.147060 halchat-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2024-05-12 13:59:25.000000 halchat-0.0.2/README.md
+-rw-rw-rw-   0        0        0      423 2024-05-19 12:45:04.000000 halchat-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 17:53:07.148060 halchat-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 17:53:07.135555 halchat-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 17:53:07.146061 halchat-0.0.2/src/HalChat.egg-info/
+-rw-rw-rw-   0        0        0      480 2024-05-20 17:53:07.000000 halchat-0.0.2/src/HalChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-20 17:53:07.000000 halchat-0.0.2/src/HalChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 17:53:07.000000 halchat-0.0.2/src/HalChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 17:53:07.000000 halchat-0.0.2/src/HalChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8037 2024-05-19 13:07:56.000000 halchat-0.0.2/src/HalChatAPI.py
+-rw-rw-rw-   0        0        0     1702 2024-02-12 15:42:01.000000 halchat-0.0.2/src/HalEncryption.py
+-rw-rw-rw-   0        0        0     2724 2024-02-12 16:04:02.000000 halchat-0.0.2/src/HalHash.py
+-rw-rw-rw-   0        0        0        0 2024-05-12 13:57:45.000000 halchat-0.0.2/src/__init__.py
```

### Comparing `halchat-0.0.1/LICENSE` & `halchat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `halchat-0.0.1/src/HalChatAPI.py` & `halchat-0.0.2/src/HalChatAPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from HalEncryption import HalEncryption
 from Cryptodome.Cipher import PKCS1_OAEP
 from Cryptodome.PublicKey import RSA
 from Cryptodome.Hash import SHA256
 import base64
 
 class HalChatAPI:
-    def __init__(self,code,sleepTime=1,save_file_passwords='HalChatPasswords.json',auto_join_chats=True):
+    def __init__(self,code,sleepTime=1,save_file_passwords='HalChatPasswords.json',auto_join_chats=True,check_bots_messages=False):
         self.code=code
         self.url='https://halchat.halwarsing.net/api'
-        self.events={'onNewMessage':[],'onNewChat':[],'onReceivePassword':[],'onStart':[],'onClickButton':[]}
+        self.events={'onNewMessage':[],'onNewChat':[],'onReceivePassword':[],'onStart':[],'onClickButton':[],'onBotMessage':[]}
         self.isRun=False
         self.sleepTime=sleepTime
         self.chats={}
         self.chatsPasswords={}
         self.bot=requests.post('https://halwarsing.net/api/api?req=getInfoUser',data={'code':self.code}).json()
         self.botId=self.bot['id']
         self.he=HalEncryption()
         self.requested_passwords={}
         self.save_file_passwords=save_file_passwords
         self.auto_join_chats=auto_join_chats
+        self.check_bots_messages=check_bots_messages
         self.loadPasswords()
 
     def apiReq(self,req:str,getData:str='',postData:dict={}):
         postData['code']=self.code
         out=requests.post(self.url+'?req='+req+getData,data=postData)
         if out.status_code:
             try:
@@ -80,15 +81,19 @@
                             self.addChatPassword(v['fromChat'],passw)
                             self.savePasswords()
                             v['data']=passw
                             del self.requested_passwords[v['fromChat']]
                         self.run_event('onReceivePassword',[v['fromChat'],v['data']])
                     elif v['type']==6:
                         self.run_event('onClickButton',[v['fromChat'],v['fromId'],v['fromMsg'],v['data']])
-                    
+            if self.check_bots_messages:
+                data=self.getBotsMessages()
+                if not data is None and data['errorCode']==0:
+                    for msg in data['messages']:
+                        self.run_event('onBotMessage',[msg['fromId'],msg['time'],msg['data']])
             time.sleep(self.sleepTime)
 
     def close(self):
         self.isRun=False
 
     def addChatPassword(self,chatId:int,password:str):
         self.chatsPasswords[str(chatId)]=password
@@ -150,8 +155,15 @@
         return self.apiReq('editMessage',getData="&chatId="+str(chatId)+"&msgId="+str(msgId),
                            postData={'message':message,'attachments':json.dumps(attachments),'encryptId':encryptId})
 
     def setMenu(self,chatId:int,menu:list):
         return self.apiReq('setMenu',getData="&chatId="+str(chatId),postData={'menu':json.dumps(menu)})
     
     def execHDB(self,chatId:int,query:str):
-        return self.apiReq('execHDB','&chatId='+chatId,{'query':json.dumps({'exec':exec})})
+        return self.apiReq('execHDB','&chatId='+chatId,{'query':json.dumps({'exec':exec})})
+    
+    def getBotsMessages(self,fromId:int=-1):
+        return self.apiReq('getBotsMessages','&fromId='+('' if fromId<=0 else str(fromId)))
+    
+    #protocol messages between app and bot
+    def sendBotMessage(self,toId:int,data:str):
+        return self.apiReq('sendBotMessage','&toId='+str(toId),{'data':data})
```

### Comparing `halchat-0.0.1/src/HalEncryption.py` & `halchat-0.0.2/src/HalEncryption.py`

 * *Files identical despite different names*

### Comparing `halchat-0.0.1/src/HalHash.py` & `halchat-0.0.2/src/HalHash.py`

 * *Files identical despite different names*

