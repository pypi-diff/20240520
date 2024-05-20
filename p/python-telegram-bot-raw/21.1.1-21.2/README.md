# Comparing `tmp/python-telegram-bot-raw-21.1.1.tar.gz` & `tmp/python-telegram-bot-raw-21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-telegram-bot-raw-21.1.1.tar", last modified: Mon Apr 15 15:01:10 2024, max compression
+gzip compressed data, was "python-telegram-bot-raw-21.2.tar", last modified: Mon May 20 15:25:44 2024, max compression
```

## Comparing `python-telegram-bot-raw-21.1.1.tar` & `python-telegram-bot-raw-21.2.tar`

### file list

```diff
@@ -1,177 +1,180 @@
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    32422 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/LICENSE
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    40192 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/LICENSE.dual
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7651 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/LICENSE.lesser
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/MANIFEST.in
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12541 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12714 2024-04-15 14:54:41.000000 python-telegram-bot-raw-21.1.1/README.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10852 2024-04-15 14:54:41.000000 python-telegram-bot-raw-21.1.1/README_RAW.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3686 2024-04-15 14:50:11.000000 python-telegram-bot-raw-21.1.1/pyproject.toml
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.058611 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12541 2024-04-15 15:01:09.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5123 2024-04-15 15:01:10.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/SOURCES.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2024-04-15 15:01:09.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/dependency_links.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      203 2024-04-15 15:01:09.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/requires.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2024-04-15 15:01:09.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/top_level.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.1.1/requirements-opts.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      484 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.1.1/requirements.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      235 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/setup.cfg
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5073 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/setup.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.066611 python-telegram-bot-raw-21.1.1/telegram/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15285 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1820 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/__main__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2861 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_birthdate.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   379065 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_bot.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3273 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_botcommand.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10380 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_botcommandscope.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2511 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_botdescription.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1805 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_botname.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15745 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_business.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    33026 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_callbackquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   147253 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11366 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatadministratorrights.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15478 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatboost.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6764 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatinvitelink.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8746 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatjoinrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3296 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26788 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatmember.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7991 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatmemberupdated.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10917 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatpermissions.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4274 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_choseninlineresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6956 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_dice.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.070611 python-telegram-bot-raw-21.1.1/telegram/_files/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3536 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/_basemedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3836 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/_basethumbedmedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4272 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/animation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4497 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/audio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7096 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/chatphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2720 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/contact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3552 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/document.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14644 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/file.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4191 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/inputfile.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26864 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/inputmedia.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5621 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/inputsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4762 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/location.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2826 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/photosize.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17443 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/sticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4466 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/venue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4114 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/video.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3516 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/videonote.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3031 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/voice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4383 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_forcereply.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6965 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_forumtopic.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.070611 python-telegram-bot-raw-21.1.1/telegram/_games/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_games/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1309 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_games/callbackgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8114 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_games/game.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2518 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_games/gamehighscore.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14854 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_giveaway.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.074610 python-telegram-bot-raw-21.1.1/telegram/_inline/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15174 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinekeyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5601 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinekeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9211 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2838 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5274 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultarticle.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5695 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5138 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5666 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcacheddocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5423 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5514 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5679 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3659 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5586 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5351 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5530 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcontact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7143 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultdocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2735 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7814 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9328 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7919 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7128 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5353 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultsbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7172 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvenue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8610 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5587 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2746 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputcontactmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12830 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputinvoicemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6586 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputlocationmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1567 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4804 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputtextmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4561 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputvenuemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9168 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_keyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2547 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_keyboardbuttonpolltype.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12851 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_keyboardbuttonrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4498 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_linkpreviewoptions.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5134 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_loginurl.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6856 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_menubutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   202907 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_message.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2015 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messageautodeletetimerchanged.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8934 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messageentity.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1704 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messageid.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10097 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messageorigin.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7958 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messagereactionupdated.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.074610 python-telegram-bot-raw-21.1.1/telegram/_passport/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22754 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/credentials.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6373 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/data.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12726 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/encryptedpassportelement.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5171 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/passportdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    18799 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/passportelementerrors.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7157 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/passportfile.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.074610 python-telegram-bot-raw-21.1.1/telegram/_payment/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5012 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/invoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2703 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/labeledprice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3118 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/orderinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5904 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/precheckoutquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2977 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/shippingaddress.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2502 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/shippingoption.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4475 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/shippingquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4939 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/successfulpayment.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17858 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_poll.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2864 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_proximityalerttriggered.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6543 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_reaction.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20722 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_reply.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16464 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_replykeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3251 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_replykeyboardremove.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2199 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_sentwebappmessage.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    13120 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_shared.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2551 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_story.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4136 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_switchinlinequerychosenchat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    27782 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_telegramobject.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    34486 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_update.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    80314 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_user.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2907 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_userprofilephotos.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/telegram/_utils/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2310 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/argumentparsing.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8924 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/datetime.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4305 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/defaultvalue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2641 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/enum.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5747 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/files.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1970 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/logging.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/markup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1833 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/repr.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1441 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/strings.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3641 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/types.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1989 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/warnings.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3863 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/warnings_transition.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2234 2024-04-15 14:56:01.000000 python-telegram-bot-raw-21.1.1/telegram/_version.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6022 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_videochat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2444 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_webappdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2124 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_webappinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7720 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_webhookinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3585 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_writeaccessallowed.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   106661 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/constants.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7574 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/error.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7252 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/helpers.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/telegram/py.typed
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/telegram/request/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20478 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/_baserequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12968 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/_httpxrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5204 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/_requestdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7408 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/_requestparameter.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1899 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/warnings.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.087887 python-telegram-bot-raw-21.2/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    32422 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.2/LICENSE
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    40192 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.2/LICENSE.dual
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7651 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.2/LICENSE.lesser
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.2/MANIFEST.in
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12538 2024-05-20 15:25:44.087887 python-telegram-bot-raw-21.2/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12713 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/README.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10851 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/README_RAW.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3802 2024-05-20 14:14:05.000000 python-telegram-bot-raw-21.2/pyproject.toml
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.067887 python-telegram-bot-raw-21.2/python_telegram_bot_raw.egg-info/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12538 2024-05-20 15:25:43.000000 python-telegram-bot-raw-21.2/python_telegram_bot_raw.egg-info/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5205 2024-05-20 15:25:44.000000 python-telegram-bot-raw-21.2/python_telegram_bot_raw.egg-info/SOURCES.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2024-05-20 15:25:43.000000 python-telegram-bot-raw-21.2/python_telegram_bot_raw.egg-info/dependency_links.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      203 2024-05-20 15:25:43.000000 python-telegram-bot-raw-21.2/python_telegram_bot_raw.egg-info/requires.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2024-05-20 15:25:43.000000 python-telegram-bot-raw-21.2/python_telegram_bot_raw.egg-info/top_level.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.2/requirements-opts.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      484 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.2/requirements.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      235 2024-05-20 15:25:44.091888 python-telegram-bot-raw-21.2/setup.cfg
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5073 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/setup.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.075887 python-telegram-bot-raw-21.2/telegram/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15954 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1820 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/__main__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3014 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_birthdate.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   381003 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_bot.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3273 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_botcommand.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10380 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_botcommandscope.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2511 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_botdescription.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1805 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_botname.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15798 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_business.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    33147 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_callbackquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   160879 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11560 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatadministratorrights.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    19594 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatbackground.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15478 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatboost.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7024 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatfullinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6764 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatinvitelink.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8746 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatjoinrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3296 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26982 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatmember.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8643 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatmemberupdated.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10917 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_chatpermissions.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4274 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_choseninlineresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6956 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_dice.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.079887 python-telegram-bot-raw-21.2/telegram/_files/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3536 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/_basemedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3836 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/_basethumbedmedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4272 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/animation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4497 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/audio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7096 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/chatphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2720 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/contact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3552 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/document.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14644 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/file.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4191 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/inputfile.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26864 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/inputmedia.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5621 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/inputsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4762 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/location.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2826 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/photosize.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15852 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/sticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4466 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/venue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4114 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/video.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3516 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/videonote.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3031 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_files/voice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4535 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_forcereply.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6965 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_forumtopic.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.079887 python-telegram-bot-raw-21.2/telegram/_games/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_games/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1309 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_games/callbackgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8114 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_games/game.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2518 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_games/gamehighscore.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14854 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_giveaway.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.083887 python-telegram-bot-raw-21.2/telegram/_inline/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15262 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinekeyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5601 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinekeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9211 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2838 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5274 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultarticle.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5695 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5138 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5666 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcacheddocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5423 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5514 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5679 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3659 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5586 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5351 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5530 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcontact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7143 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultdocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2735 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7814 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9471 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7919 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7128 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5353 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultsbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7172 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultvenue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8610 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5587 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2746 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inputcontactmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12830 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inputinvoicemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6729 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inputlocationmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1567 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inputmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4804 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inputtextmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4561 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_inline/inputvenuemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9168 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_keyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2547 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_keyboardbuttonpolltype.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12851 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_keyboardbuttonrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4498 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_linkpreviewoptions.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5134 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_loginurl.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6856 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_menubutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   203540 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_message.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2015 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_messageautodeletetimerchanged.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8934 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_messageentity.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1704 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_messageid.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10097 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_messageorigin.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7958 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_messagereactionupdated.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.083887 python-telegram-bot-raw-21.2/telegram/_passport/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_passport/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22754 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_passport/credentials.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6373 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_passport/data.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12829 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_passport/encryptedpassportelement.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5171 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_passport/passportdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    18897 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_passport/passportelementerrors.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7204 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_passport/passportfile.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.087887 python-telegram-bot-raw-21.2/telegram/_payment/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_payment/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5012 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_payment/invoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2703 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_payment/labeledprice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3118 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_payment/orderinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5904 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_payment/precheckoutquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2977 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_payment/shippingaddress.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2502 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_payment/shippingoption.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4475 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_payment/shippingquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4939 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_payment/successfulpayment.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26833 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_poll.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2864 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_proximityalerttriggered.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6543 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_reaction.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20876 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_reply.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16558 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_replykeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3345 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_replykeyboardremove.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2199 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_sentwebappmessage.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10584 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_shared.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2551 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_story.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4136 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_switchinlinequerychosenchat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    27782 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_telegramobject.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    34462 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_update.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    80597 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_user.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2907 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_userprofilephotos.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.087887 python-telegram-bot-raw-21.2/telegram/_utils/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2310 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/argumentparsing.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8924 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/datetime.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4305 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/defaultvalue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2951 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/entities.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2674 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/enum.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5747 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/files.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1970 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/logging.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/markup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1833 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/repr.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1441 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/strings.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3641 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/types.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2176 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/warnings.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4086 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_utils/warnings_transition.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2234 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_version.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6022 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_videochat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2444 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_webappdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2124 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_webappinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7720 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_webhookinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3585 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/_writeaccessallowed.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   110327 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/constants.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7574 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/error.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7252 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/helpers.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.2/telegram/py.typed
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-05-20 15:25:44.087887 python-telegram-bot-raw-21.2/telegram/request/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/request/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20537 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/request/_baserequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12960 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/request/_httpxrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5204 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/request/_requestdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7408 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/request/_requestparameter.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2749 2024-05-20 15:15:04.000000 python-telegram-bot-raw-21.2/telegram/warnings.py
```

### Comparing `python-telegram-bot-raw-21.1.1/LICENSE` & `python-telegram-bot-raw-21.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/LICENSE.dual` & `python-telegram-bot-raw-21.2/LICENSE.dual`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/LICENSE.lesser` & `python-telegram-bot-raw-21.2/LICENSE.lesser`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/PKG-INFO` & `python-telegram-bot-raw-21.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 21.1.1
+Version: 21.2
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
@@ -49,17 +49,17 @@
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot-raw.svg
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-7.2-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-7.3-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
-   :alt: Supported Bot API versions
+   :alt: Supported Bot API version
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot-raw
    :target: https://pypistats.org/packages/python-telegram-bot-raw
    :alt: PyPi Package Monthly Download
 
 .. image:: https://readthedocs.org/projects/python-telegram-bot/badge/?version=stable
    :target: https://docs.python-telegram-bot.org/
@@ -120,15 +120,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **7.2** are supported.
+All types and methods of the Telegram Bot API **7.3** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-21.1.1/README.rst` & `python-telegram-bot-raw-21.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
    :target: https://pypi.org/project/python-telegram-bot/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot.svg
    :target: https://pypi.org/project/python-telegram-bot/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-7.2-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-7.3-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
-   :alt: Supported Bot API versions
+   :alt: Supported Bot API version
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot
    :target: https://pypistats.org/packages/python-telegram-bot
    :alt: PyPi Package Monthly Download
 
 .. image:: https://readthedocs.org/projects/python-telegram-bot/badge/?version=stable
    :target: https://docs.python-telegram-bot.org/en/stable/
@@ -85,15 +85,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **7.2** are supported.
+All types and methods of the Telegram Bot API **7.3** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-21.1.1/README_RAW.rst` & `python-telegram-bot-raw-21.2/README_RAW.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot-raw.svg
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-7.2-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-7.3-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
-   :alt: Supported Bot API versions
+   :alt: Supported Bot API version
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot-raw
    :target: https://pypistats.org/packages/python-telegram-bot-raw
    :alt: PyPi Package Monthly Download
 
 .. image:: https://readthedocs.org/projects/python-telegram-bot/badge/?version=stable
    :target: https://docs.python-telegram-bot.org/
@@ -81,15 +81,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **7.2** are supported.
+All types and methods of the Telegram Bot API **7.3** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-21.1.1/pyproject.toml` & `python-telegram-bot-raw-21.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 
 [tool.ruff.lint]
 preview = true
 explicit-preview-rules = true
 ignore = ["PLR2004", "PLR0911", "PLR0912", "PLR0913", "PLR0915", "PERF203"]
 select = ["E", "F", "I", "PL", "UP", "RUF", "PTH", "C4", "B", "PIE", "SIM", "RET", "RSE",
           "G", "ISC", "PT", "ASYNC", "TCH", "SLOT", "PERF", "PYI", "FLY", "AIR", "RUF022",
-          "RUF023", "Q", "INP", "W"]
+          "RUF023", "Q", "INP", "W", "YTT", "DTZ", "ARG"]
 # Add "FURB" after it's out of preview
+# Add "A (flake8-builtins)" after we drop pylint
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*.py" = ["B018"]
-"tests/**.py" = ["RUF012", "ASYNC101"]
-"docs/**.py" = ["INP001"]
+"tests/**.py" = ["RUF012", "ASYNC101", "DTZ", "ARG"]
+"docs/**.py" = ["INP001", "ARG"]
+"examples/**.py" = ["ARG"]
 
 # PYLINT:
 [tool.pylint."messages control"]
 enable = ["useless-suppression"]
 disable = ["duplicate-code", "too-many-arguments", "too-many-public-methods",
         "too-few-public-methods", "broad-exception-caught", "too-many-instance-attributes",
         "fixme", "missing-function-docstring", "missing-class-docstring", "too-many-locals",
@@ -44,15 +46,15 @@
 
 [tool.pylint.classes]
 exclude-protected = ["_unfrozen"]
 
 # PYTEST:
 [tool.pytest.ini_options]
 testpaths = ["tests"]
-addopts = "--no-success-flaky-report -rsxX"
+addopts = "--no-success-flaky-report -rX"
 filterwarnings = [
     "error",
     "ignore::DeprecationWarning",
     'ignore:Tasks created via `Application\.create_task` while the application is not running',
     "ignore::ResourceWarning",
     # TODO: Write so good code that we don't need to ignore ResourceWarnings anymore
     # Unfortunately due to https://github.com/pytest-dev/pytest/issues/8343 we can't have this here
```

### Comparing `python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/PKG-INFO` & `python-telegram-bot-raw-21.2/python_telegram_bot_raw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 21.1.1
+Version: 21.2
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
@@ -49,17 +49,17 @@
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot-raw.svg
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-7.2-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-7.3-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
-   :alt: Supported Bot API versions
+   :alt: Supported Bot API version
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot-raw
    :target: https://pypistats.org/packages/python-telegram-bot-raw
    :alt: PyPi Package Monthly Download
 
 .. image:: https://readthedocs.org/projects/python-telegram-bot/badge/?version=stable
    :target: https://docs.python-telegram-bot.org/
@@ -120,15 +120,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **7.2** are supported.
+All types and methods of the Telegram Bot API **7.3** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/SOURCES.txt` & `python-telegram-bot-raw-21.2/python_telegram_bot_raw.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 telegram/_botcommandscope.py
 telegram/_botdescription.py
 telegram/_botname.py
 telegram/_business.py
 telegram/_callbackquery.py
 telegram/_chat.py
 telegram/_chatadministratorrights.py
+telegram/_chatbackground.py
 telegram/_chatboost.py
+telegram/_chatfullinfo.py
 telegram/_chatinvitelink.py
 telegram/_chatjoinrequest.py
 telegram/_chatlocation.py
 telegram/_chatmember.py
 telegram/_chatmemberupdated.py
 telegram/_chatpermissions.py
 telegram/_choseninlineresult.py
@@ -146,14 +148,15 @@
 telegram/_payment/shippingoption.py
 telegram/_payment/shippingquery.py
 telegram/_payment/successfulpayment.py
 telegram/_utils/__init__.py
 telegram/_utils/argumentparsing.py
 telegram/_utils/datetime.py
 telegram/_utils/defaultvalue.py
+telegram/_utils/entities.py
 telegram/_utils/enum.py
 telegram/_utils/files.py
 telegram/_utils/logging.py
 telegram/_utils/markup.py
 telegram/_utils/repr.py
 telegram/_utils/strings.py
 telegram/_utils/types.py
```

### Comparing `python-telegram-bot-raw-21.1.1/requirements-opts.txt` & `python-telegram-bot-raw-21.2/requirements-opts.txt`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/setup.py` & `python-telegram-bot-raw-21.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/__init__.py` & `python-telegram-bot-raw-21.2/telegram/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,23 @@
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """A library that provides a Python interface to the Telegram Bot API"""
 
 __author__ = "devs@python-telegram-bot.org"
 __all__ = (
     "Animation",
     "Audio",
+    "BackgroundFill",
+    "BackgroundFillFreeformGradient",
+    "BackgroundFillGradient",
+    "BackgroundFillSolid",
+    "BackgroundType",
+    "BackgroundTypeChatTheme",
+    "BackgroundTypeFill",
+    "BackgroundTypePattern",
+    "BackgroundTypeWallpaper",
     "Birthdate",
     "Bot",
     "BotCommand",
     "BotCommandScope",
     "BotCommandScopeAllChatAdministrators",
     "BotCommandScopeAllGroupChats",
     "BotCommandScopeAllPrivateChats",
@@ -42,22 +51,24 @@
     "BusinessMessagesDeleted",
     "BusinessOpeningHours",
     "BusinessOpeningHoursInterval",
     "CallbackGame",
     "CallbackQuery",
     "Chat",
     "ChatAdministratorRights",
+    "ChatBackground",
     "ChatBoost",
     "ChatBoostAdded",
     "ChatBoostRemoved",
     "ChatBoostSource",
     "ChatBoostSourceGiftCode",
     "ChatBoostSourceGiveaway",
     "ChatBoostSourcePremium",
     "ChatBoostUpdated",
+    "ChatFullInfo",
     "ChatInviteLink",
     "ChatJoinRequest",
     "ChatLocation",
     "ChatMember",
     "ChatMemberAdministrator",
     "ChatMemberBanned",
     "ChatMemberLeft",
@@ -127,14 +138,15 @@
     "InputMedia",
     "InputMediaAnimation",
     "InputMediaAudio",
     "InputMediaDocument",
     "InputMediaPhoto",
     "InputMediaVideo",
     "InputMessageContent",
+    "InputPollOption",
     "InputSticker",
     "InputTextMessageContent",
     "InputVenueMessageContent",
     "Invoice",
     "KeyboardButton",
     "KeyboardButtonPollType",
     "KeyboardButtonRequestChat",
@@ -254,25 +266,38 @@
     BusinessMessagesDeleted,
     BusinessOpeningHours,
     BusinessOpeningHoursInterval,
 )
 from ._callbackquery import CallbackQuery
 from ._chat import Chat
 from ._chatadministratorrights import ChatAdministratorRights
+from ._chatbackground import (
+    BackgroundFill,
+    BackgroundFillFreeformGradient,
+    BackgroundFillGradient,
+    BackgroundFillSolid,
+    BackgroundType,
+    BackgroundTypeChatTheme,
+    BackgroundTypeFill,
+    BackgroundTypePattern,
+    BackgroundTypeWallpaper,
+    ChatBackground,
+)
 from ._chatboost import (
     ChatBoost,
     ChatBoostAdded,
     ChatBoostRemoved,
     ChatBoostSource,
     ChatBoostSourceGiftCode,
     ChatBoostSourceGiveaway,
     ChatBoostSourcePremium,
     ChatBoostUpdated,
     UserChatBoosts,
 )
+from ._chatfullinfo import ChatFullInfo
 from ._chatinvitelink import ChatInviteLink
 from ._chatjoinrequest import ChatJoinRequest
 from ._chatlocation import ChatLocation
 from ._chatmember import (
     ChatMember,
     ChatMemberAdministrator,
     ChatMemberBanned,
@@ -399,15 +424,15 @@
 from ._payment.labeledprice import LabeledPrice
 from ._payment.orderinfo import OrderInfo
 from ._payment.precheckoutquery import PreCheckoutQuery
 from ._payment.shippingaddress import ShippingAddress
 from ._payment.shippingoption import ShippingOption
 from ._payment.shippingquery import ShippingQuery
 from ._payment.successfulpayment import SuccessfulPayment
-from ._poll import Poll, PollAnswer, PollOption
+from ._poll import InputPollOption, Poll, PollAnswer, PollOption
 from ._proximityalerttriggered import ProximityAlertTriggered
 from ._reaction import ReactionCount, ReactionType, ReactionTypeCustomEmoji, ReactionTypeEmoji
 from ._reply import ExternalReplyInfo, ReplyParameters, TextQuote
 from ._replykeyboardmarkup import ReplyKeyboardMarkup
 from ._replykeyboardremove import ReplyKeyboardRemove
 from ._sentwebappmessage import SentWebAppMessage
 from ._shared import ChatShared, SharedUser, UsersShared
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/__main__.py` & `python-telegram-bot-raw-21.2/telegram/__main__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_birthdate.py` & `python-telegram-bot-raw-21.2/telegram/_birthdate.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Birthday."""
-from datetime import datetime
+from datetime import date
 from typing import Optional
 
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class Birthdate(TelegramObject):
     """
-    This object represents a user's birthday.
+    This object describes the birthdate of a user.
 
     Objects of this class are comparable in terms of equality. Two objects of this class are
     considered equal, if their :attr:`day`, and :attr:`month` are equal.
 
     .. versionadded:: 21.1
 
     Args:
@@ -66,23 +66,27 @@
         self._id_attrs = (
             self.day,
             self.month,
         )
 
         self._freeze()
 
-    def to_date(self, year: Optional[int] = None) -> datetime:
-        """Return the birthdate as a datetime object.
+    def to_date(self, year: Optional[int] = None) -> date:
+        """Return the birthdate as a date object.
+
+        .. versionchanged:: 21.2
+           Now returns a :obj:`datetime.date` object instead of a :obj:`datetime.datetime` object,
+           as was originally intended.
 
         Args:
             year (:obj:`int`, optional): The year to use. Required, if the :attr:`year` was not
                 present.
 
         Returns:
-            :obj:`datetime.datetime`: The birthdate as a datetime object.
+            :obj:`datetime.date`: The birthdate as a date object.
         """
         if self.year is None and year is None:
             raise ValueError(
                 "The `year` argument is required if the `year` attribute was not present."
             )
 
-        return datetime(year or self.year, self.month, self.day)  # type: ignore[arg-type]
+        return date(year or self.year, self.month, self.day)  # type: ignore[arg-type]
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_bot.py` & `python-telegram-bot-raw-21.2/telegram/_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     CRYPTO_INSTALLED = False
 
 from telegram._botcommand import BotCommand
 from telegram._botcommandscope import BotCommandScope
 from telegram._botdescription import BotDescription, BotShortDescription
 from telegram._botname import BotName
 from telegram._business import BusinessConnection
-from telegram._chat import Chat
 from telegram._chatadministratorrights import ChatAdministratorRights
 from telegram._chatboost import UserChatBoosts
+from telegram._chatfullinfo import ChatFullInfo
 from telegram._chatinvitelink import ChatInviteLink
 from telegram._chatmember import ChatMember
 from telegram._chatpermissions import ChatPermissions
 from telegram._files.animation import Animation
 from telegram._files.audio import Audio
 from telegram._files.chatphoto import ChatPhoto
 from telegram._files.contact import Contact
@@ -80,15 +80,15 @@
 from telegram._files.voice import Voice
 from telegram._forumtopic import ForumTopic
 from telegram._games.gamehighscore import GameHighScore
 from telegram._inline.inlinequeryresultsbutton import InlineQueryResultsButton
 from telegram._menubutton import MenuButton
 from telegram._message import Message
 from telegram._messageid import MessageId
-from telegram._poll import Poll
+from telegram._poll import InputPollOption, Poll
 from telegram._reaction import ReactionType, ReactionTypeCustomEmoji, ReactionTypeEmoji
 from telegram._reply import ReplyParameters
 from telegram._sentwebappmessage import SentWebAppMessage
 from telegram._telegramobject import TelegramObject
 from telegram._update import Update
 from telegram._user import User
 from telegram._userprofilephotos import UserProfilePhotos
@@ -520,15 +520,18 @@
     @property
     def name(self) -> str:
         """:obj:`str`: Bot's @username. Shortcut for the corresponding attribute of :attr:`bot`."""
         return f"@{self.username}"
 
     @classmethod
     def _warn(
-        cls, message: str, category: Type[Warning] = PTBUserWarning, stacklevel: int = 0
+        cls,
+        message: Union[str, PTBUserWarning],
+        category: Type[Warning] = PTBUserWarning,
+        stacklevel: int = 0,
     ) -> None:
         """Convenience method to issue a warning. This method is here mostly to make it easier
         for ExtBot to add 1 level to all warning calls.
         """
         warn(message=message, category=category, stacklevel=stacklevel + 1)
 
     def _parse_file_input(
@@ -833,15 +836,14 @@
         """
         if hasattr(self, endpoint):
             self._warn(
                 (
                     f"Please use 'Bot.{endpoint}' instead of "
                     f"'Bot.do_api_request(\"{endpoint}\", ...)'"
                 ),
-                PTBDeprecationWarning,
                 stacklevel=2,
             )
 
         camel_case_endpoint = to_camel_case(endpoint)
         try:
             result = await self._post(
                 camel_case_endpoint,
@@ -2283,17 +2285,18 @@
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         Use this method to send audio files, if you want Telegram clients to display the file
         as a playable voice message. For this to work, your audio must be in an ``.ogg`` file
-        encoded with OPUS (other formats may be sent as Audio or Document). Bots can currently
-        send voice messages of up to :tg-const:`telegram.constants.FileSizeLimit.FILESIZE_UPLOAD`
-        in size, this limit may be changed in the future.
+        encoded with OPUS , or in .MP3 format, or in .M4A format (other formats may be sent as
+        :class:`~telegram.Audio` or :class:`~telegram.Document`). Bots can currently send voice
+        messages of up to :tg-const:`telegram.constants.FileSizeLimit.FILESIZE_UPLOAD` in size,
+        this limit may be changed in the future.
 
         Note:
             To use this method, the file must have the type :mimetype:`audio/ogg` and be no more
             than :tg-const:`telegram.constants.FileSizeLimit.VOICE_NOTE_FILE_SIZE` in size.
             :tg-const:`telegram.constants.FileSizeLimit.VOICE_NOTE_FILE_SIZE`-
             :tg-const:`telegram.constants.FileSizeLimit.FILESIZE_DOWNLOAD` voice notes will be
             sent as files.
@@ -2606,15 +2609,17 @@
             longitude (:obj:`float`, optional): Longitude of location.
             horizontal_accuracy (:obj:`int`, optional): The radius of uncertainty for the location,
                 measured in meters;
                 0-:tg-const:`telegram.constants.LocationLimit.HORIZONTAL_ACCURACY`.
             live_period (:obj:`int`, optional): Period in seconds for which the location will be
                 updated, should be between
                 :tg-const:`telegram.constants.LocationLimit.MIN_LIVE_PERIOD` and
-                :tg-const:`telegram.constants.LocationLimit.MAX_LIVE_PERIOD`.
+                :tg-const:`telegram.constants.LocationLimit.MAX_LIVE_PERIOD`, or
+                :tg-const:`telegram.constants.LocationLimit.LIVE_PERIOD_FOREVER` for live
+                locations that can be edited indefinitely.
             heading (:obj:`int`, optional): For live locations, a direction in which the user is
                 moving, in degrees. Must be between
                 :tg-const:`telegram.constants.LocationLimit.MIN_HEADING` and
                 :tg-const:`telegram.constants.LocationLimit.MAX_HEADING` if specified.
             proximity_alert_radius (:obj:`int`, optional): For live locations, a maximum distance
                 for proximity alerts about approaching another chat member, in meters. Must be
                 between :tg-const:`telegram.constants.LocationLimit.MIN_PROXIMITY_ALERT_RADIUS`
@@ -2716,14 +2721,15 @@
         inline_message_id: Optional[str] = None,
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         horizontal_accuracy: Optional[float] = None,
         heading: Optional[int] = None,
         proximity_alert_radius: Optional[int] = None,
+        live_period: Optional[int] = None,
         *,
         location: Optional[Location] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
@@ -2754,14 +2760,23 @@
             proximity_alert_radius (:obj:`int`, optional): Maximum distance for proximity alerts
                 about approaching another chat member, in meters. Must be between
                 :tg-const:`telegram.constants.LocationLimit.MIN_PROXIMITY_ALERT_RADIUS`
                 and :tg-const:`telegram.constants.LocationLimit.MAX_PROXIMITY_ALERT_RADIUS`
                 if specified.
             reply_markup (:class:`telegram.InlineKeyboardMarkup`, optional): An object for a new
                 inline keyboard.
+            live_period (:obj:`int`, optional): New period in seconds during which the location
+                can be updated, starting from the message send date. If
+                :tg-const:`telegram.constants.LocationLimit.LIVE_PERIOD_FOREVER` is specified,
+                then the location can be updated forever. Otherwise, the new value must not exceed
+                the current ``live_period`` by more than a day, and the live location expiration
+                date must remain within the next 90 days. If not specified, then ``live_period``
+                remains unchanged
+
+                .. versionadded:: 21.2.
 
         Keyword Args:
             location (:class:`telegram.Location`, optional): The location to send.
 
         Returns:
             :class:`telegram.Message`: On success, if edited message is not an inline message, the
             edited message is returned, otherwise :obj:`True` is returned.
@@ -2786,14 +2801,15 @@
             "longitude": longitude,
             "chat_id": chat_id,
             "message_id": message_id,
             "inline_message_id": inline_message_id,
             "horizontal_accuracy": horizontal_accuracy,
             "heading": heading,
             "proximity_alert_radius": proximity_alert_radius,
+            "live_period": live_period,
         }
 
         return await self._send_message(
             "editMessageLiveLocation",
             data,
             reply_markup=reply_markup,
             read_timeout=read_timeout,
@@ -4191,18 +4207,20 @@
             arg_read_timeout: float = read_timeout or 0
         else:
             try:
                 arg_read_timeout = self._request[0].read_timeout or 0
             except NotImplementedError:
                 arg_read_timeout = 2
                 self._warn(
-                    f"The class {self._request[0].__class__.__name__} does not override "
-                    "the property `read_timeout`. Overriding this property will be mandatory in "
-                    "future versions. Using 2 seconds as fallback.",
-                    PTBDeprecationWarning,
+                    PTBDeprecationWarning(
+                        "20.7",
+                        f"The class {self._request[0].__class__.__name__} does not override "
+                        "the property `read_timeout`. Overriding this property will be mandatory "
+                        "in future versions. Using 2 seconds as fallback.",
+                    ),
                     stacklevel=2,
                 )
 
         # Ideally we'd use an aggressive read timeout for the polling. However,
         # * Short polling should return within 2 seconds.
         # * Long polling poses a different problem: the connection might have been dropped while
         #   waiting for the server to return and there's no way of knowing the connection had been
@@ -4430,24 +4448,27 @@
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
-    ) -> Chat:
+    ) -> ChatFullInfo:
         """
         Use this method to get up to date information about the chat (current name of the user for
         one-on-one conversations, current username of a user, group or channel, etc.).
 
+        .. versionchanged:: 21.2
+            In accordance to Bot API 7.3, this method now returns a :class:`telegram.ChatFullInfo`.
+
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
 
         Returns:
-            :class:`telegram.Chat`
+            :class:`telegram.ChatFullInfo`
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id}
 
@@ -4457,15 +4478,15 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return Chat.de_json(result, self)  # type: ignore[return-value]
+        return ChatFullInfo.de_json(result, self)  # type: ignore[return-value]
 
     async def get_chat_administrators(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5307,15 +5328,16 @@
 
                 .. versionadded:: 20.0
             can_post_stories (:obj:`bool`, optional): Pass :obj:`True`, if the administrator can
                 post stories to the chat.
 
                 .. versionadded:: 20.6
             can_edit_stories (:obj:`bool`, optional): Pass :obj:`True`, if the administrator can
-                edit stories posted by other users.
+                edit stories posted by other users, post stories to the chat page, pin chat
+                stories, and access the chat's story archive
 
                 .. versionadded:: 20.6
             can_delete_stories (:obj:`bool`, optional): Pass :obj:`True`, if the administrator can
                 delete stories posted by other users.
 
                 .. versionadded:: 20.6
 
@@ -6308,15 +6330,14 @@
 
     async def create_new_sticker_set(
         self,
         user_id: int,
         name: str,
         title: str,
         stickers: Sequence["InputSticker"],
-        sticker_format: Optional[str] = None,
         sticker_type: Optional[str] = None,
         needs_repainting: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6335,14 +6356,17 @@
             replace the parameters ``png_sticker``, ``tgs_sticker``,``webm_sticker``, ``emojis``,
             and ``mask_position``.
 
         .. versionchanged:: 20.5
             Removed the deprecated parameters mentioned above and adjusted the order of the
             parameters.
 
+        .. versionremoved:: 21.2
+           Removed the deprecated parameter ``sticker_format``.
+
         Args:
             user_id (:obj:`int`): User identifier of created sticker set owner.
             name (:obj:`str`): Short name of sticker set, to be used in t.me/addstickers/ URLs
                 (e.g., animals). Can contain only english letters, digits and underscores.
                 Must begin with a letter, can't contain consecutive underscores and
                 must end in "_by_<bot username>". <bot_username> is case insensitive.
                 :tg-const:`telegram.constants.StickerLimit.MIN_NAME_AND_TITLE`-
@@ -6354,24 +6378,14 @@
             stickers (Sequence[:class:`telegram.InputSticker`]): A sequence of
                 :tg-const:`telegram.constants.StickerSetLimit.MIN_INITIAL_STICKERS`-
                 :tg-const:`telegram.constants.StickerSetLimit.MAX_INITIAL_STICKERS` initial
                 stickers to be added to the sticker set.
 
                 .. versionadded:: 20.2
 
-            sticker_format (:obj:`str`): Format of stickers in the set, must be one of
-                :attr:`~telegram.constants.StickerFormat.STATIC`,
-                :attr:`~telegram.constants.StickerFormat.ANIMATED` or
-                :attr:`~telegram.constants.StickerFormat.VIDEO`.
-
-                .. versionadded:: 20.2
-
-                .. deprecated:: 21.1
-                    Use :paramref:`telegram.InputSticker.format` instead.
-
             sticker_type (:obj:`str`, optional): Type of stickers in the set, pass
                 :attr:`telegram.Sticker.REGULAR` or :attr:`telegram.Sticker.MASK`, or
                 :attr:`telegram.Sticker.CUSTOM_EMOJI`. By default, a regular sticker set is created
 
                 .. versionadded:: 20.0
 
             needs_repainting (:obj:`bool`, optional): Pass :obj:`True` if stickers in the sticker
@@ -6383,28 +6397,19 @@
 
         Returns:
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
         """
-        if sticker_format is not None:
-            warn(
-                "The parameter `sticker_format` is deprecated. Use the parameter"
-                " `InputSticker.format` in the parameter `stickers` instead.",
-                stacklevel=2,
-                category=PTBDeprecationWarning,
-            )
-
         data: JSONDict = {
             "user_id": user_id,
             "name": name,
             "title": title,
             "stickers": stickers,
-            "sticker_format": sticker_format,
             "sticker_type": sticker_type,
             "needs_repainting": needs_repainting,
         }
 
         return await self._post(
             "createNewStickerSet",
             data,
@@ -6811,15 +6816,15 @@
             api_kwargs=api_kwargs,
         )
 
     async def send_poll(
         self,
         chat_id: Union[int, str],
         question: str,
-        options: Sequence[str],
+        options: Sequence[Union[str, "InputPollOption"]],
         is_anonymous: Optional[bool] = None,
         type: Optional[str] = None,  # pylint: disable=redefined-builtin
         allows_multiple_answers: Optional[bool] = None,
         correct_option_id: Optional[CorrectOptionID] = None,
         is_closed: Optional[bool] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
@@ -6828,14 +6833,16 @@
         open_period: Optional[int] = None,
         close_date: Optional[Union[int, datetime]] = None,
         explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         business_connection_id: Optional[str] = None,
+        question_parse_mode: ODVInput[str] = DEFAULT_NONE,
+        question_entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         reply_to_message_id: Optional[int] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6844,22 +6851,28 @@
         """
         Use this method to send a native poll.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             question (:obj:`str`): Poll question, :tg-const:`telegram.Poll.MIN_QUESTION_LENGTH`-
                 :tg-const:`telegram.Poll.MAX_QUESTION_LENGTH` characters.
-            options (Sequence[:obj:`str`]): Sequence of answer options,
+            options (Sequence[:obj:`str` | :class:`telegram.InputPollOption`]): Sequence of
                 :tg-const:`telegram.Poll.MIN_OPTION_NUMBER`-
-                :tg-const:`telegram.Poll.MAX_OPTION_NUMBER` strings
+                :tg-const:`telegram.Poll.MAX_OPTION_NUMBER` answer options. Each option may either
+                be a string with
                 :tg-const:`telegram.Poll.MIN_OPTION_LENGTH`-
-                :tg-const:`telegram.Poll.MAX_OPTION_LENGTH` characters each.
+                :tg-const:`telegram.Poll.MAX_OPTION_LENGTH` characters or an
+                :class:`~telegram.InputPollOption` object. Strings are converted to
+                :class:`~telegram.InputPollOption` objects automatically.
 
                 .. versionchanged:: 20.0
                     |sequenceargs|
+
+                .. versionchanged:: 21.2
+                   Bot API 7.3 adds support for :class:`~telegram.InputPollOption` objects.
             is_anonymous (:obj:`bool`, optional): :obj:`True`, if the poll needs to be anonymous,
                 defaults to :obj:`True`.
             type (:obj:`str`, optional): Poll type, :tg-const:`telegram.Poll.QUIZ` or
                 :tg-const:`telegram.Poll.REGULAR`, defaults to :tg-const:`telegram.Poll.REGULAR`.
             allows_multiple_answers (:obj:`bool`, optional): :obj:`True`, if the poll allows
                 multiple answers, ignored for polls in quiz mode, defaults to :obj:`False`.
             correct_option_id (:obj:`int`, optional): 0-based identifier of the correct answer
@@ -6906,14 +6919,24 @@
                 keyboard, instructions to remove reply keyboard or to force a reply from the user.
             reply_parameters (:class:`telegram.ReplyParameters`, optional): |reply_parameters|
 
                 .. versionadded:: 20.8
             business_connection_id (:obj:`str`, optional): |business_id_str|
 
                 .. versionadded:: 21.1
+            question_parse_mode (:obj:`str`, optional): Mode for parsing entities in the question.
+                See the constants in :class:`telegram.constants.ParseMode` for the available modes.
+                Currently, only custom emoji entities are allowed.
+
+                .. versionadded:: 21.2
+            question_entities (Sequence[:class:`telegram.Message`], optional): Special entities
+                that appear in the poll :paramref:`question`. It can be specified instead of
+                :paramref:`question_parse_mode`.
+
+                .. versionadded:: 21.2
 
         Keyword Args:
             allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply|
                 Mutually exclusive with :paramref:`reply_parameters`, which this is a convenience
                 parameter for
 
                 .. versionchanged:: 20.8
@@ -6937,25 +6960,30 @@
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {
             "chat_id": chat_id,
             "question": question,
-            "options": options,
+            "options": [
+                InputPollOption(option) if isinstance(option, str) else option
+                for option in options
+            ],
             "explanation_parse_mode": explanation_parse_mode,
             "is_anonymous": is_anonymous,
             "type": type,
             "allows_multiple_answers": allows_multiple_answers,
             "correct_option_id": correct_option_id,
             "is_closed": is_closed,
             "explanation": explanation,
             "explanation_entities": explanation_entities,
             "open_period": open_period,
             "close_date": close_date,
+            "question_parse_mode": question_parse_mode,
+            "question_entities": question_entities,
         }
 
         return await self._send_message(
             "sendPoll",
             data,
             reply_to_message_id=reply_to_message_id,
             disable_notification=disable_notification,
@@ -8863,15 +8891,15 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    def to_dict(self, recursive: bool = True) -> JSONDict:
+    def to_dict(self, recursive: bool = True) -> JSONDict:  # noqa: ARG002
         """See :meth:`telegram.TelegramObject.to_dict`."""
         data: JSONDict = {"id": self.id, "username": self.username, "first_name": self.first_name}
 
         if self.last_name:
             data["last_name"] = self.last_name
 
         return data
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_botcommand.py` & `python-telegram-bot-raw-21.2/telegram/_botcommand.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_botcommandscope.py` & `python-telegram-bot-raw-21.2/telegram/_botcommandscope.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_botdescription.py` & `python-telegram-bot-raw-21.2/telegram/_botdescription.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_botname.py` & `python-telegram-bot-raw-21.2/telegram/_botname.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_business.py` & `python-telegram-bot-raw-21.2/telegram/_business.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         data["chat"] = Chat.de_json(data.get("chat"), bot)
 
         return super().de_json(data=data, bot=bot)
 
 
 class BusinessIntro(TelegramObject):
     """
-    This object represents the intro of a business account.
+    This object contains information about the start page settings of a Telegram Business account.
 
     Objects of this class are comparable in terms of equality.
     Two objects of this class are considered equal, if their
     :attr:`title`, :attr:`message` and :attr:`sticker` are equal.
 
     .. versionadded:: 21.1
 
@@ -242,15 +242,15 @@
         data["sticker"] = Sticker.de_json(data.get("sticker"), bot)
 
         return super().de_json(data=data, bot=bot)
 
 
 class BusinessLocation(TelegramObject):
     """
-    This object represents the location of a business account.
+    This object contains information about the location of a Telegram Business account.
 
     Objects of this class are comparable in terms of equality.
     Two objects of this class are considered equal, if their
     :attr:`address` is equal.
 
     .. versionadded:: 21.1
 
@@ -294,15 +294,15 @@
         data["location"] = Location.de_json(data.get("location"), bot)
 
         return super().de_json(data=data, bot=bot)
 
 
 class BusinessOpeningHoursInterval(TelegramObject):
     """
-    This object represents the time intervals describing business opening hours.
+    This object describes an interval of time during which a business is open.
 
     Objects of this class are comparable in terms of equality.
     Two objects of this class are considered equal, if their
     :attr:`opening_minute` and :attr:`closing_minute` are equal.
 
     .. versionadded:: 21.1
 
@@ -386,15 +386,15 @@
         if self._closing_time is None:
             self._closing_time = self._parse_minute(self.closing_minute)
         return self._closing_time
 
 
 class BusinessOpeningHours(TelegramObject):
     """
-    This object represents the opening hours of a business account.
+    This object describes the opening hours of a business.
 
     Objects of this class are comparable in terms of equality.
     Two objects of this class are considered equal, if their
     :attr:`time_zone_name` and :attr:`opening_hours` are equal.
 
     .. versionadded:: 21.1
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_callbackquery.py` & `python-telegram-bot-raw-21.2/telegram/_callbackquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,14 +457,15 @@
         self,
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         horizontal_accuracy: Optional[float] = None,
         heading: Optional[int] = None,
         proximity_alert_radius: Optional[int] = None,
+        live_period: Optional[int] = None,
         *,
         location: Optional[Location] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
@@ -505,14 +506,15 @@
                 write_timeout=write_timeout,
                 connect_timeout=connect_timeout,
                 pool_timeout=pool_timeout,
                 api_kwargs=api_kwargs,
                 horizontal_accuracy=horizontal_accuracy,
                 heading=heading,
                 proximity_alert_radius=proximity_alert_radius,
+                live_period=live_period,
                 chat_id=None,
                 message_id=None,
             )
         return await self._get_message().edit_live_location(
             latitude=latitude,
             longitude=longitude,
             location=location,
@@ -521,14 +523,15 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             horizontal_accuracy=horizontal_accuracy,
             heading=heading,
             proximity_alert_radius=proximity_alert_radius,
+            live_period=live_period,
         )
 
     async def stop_message_live_location(
         self,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_chat.py` & `python-telegram-bot-raw-21.2/telegram/_chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Chat."""
 from datetime import datetime
 from html import escape
-from typing import TYPE_CHECKING, Final, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Any, Final, Optional, Sequence, Tuple, Union
 
 from telegram import constants
 from telegram._birthdate import Birthdate
 from telegram._chatlocation import ChatLocation
 from telegram._chatpermissions import ChatPermissions
 from telegram._files.chatphoto import ChatPhoto
 from telegram._forumtopic import ForumTopic
@@ -32,17 +32,19 @@
 from telegram._reaction import ReactionType
 from telegram._telegramobject import TelegramObject
 from telegram._utils import enum
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import CorrectOptionID, FileInput, JSONDict, ODVInput, ReplyMarkup
+from telegram._utils.warnings import warn
 from telegram.helpers import escape_markdown
 from telegram.helpers import mention_html as helpers_mention_html
 from telegram.helpers import mention_markdown as helpers_mention_markdown
+from telegram.warnings import PTBDeprecationWarning
 
 if TYPE_CHECKING:
     from telegram import (
         Animation,
         Audio,
         Bot,
         BusinessIntro,
@@ -53,14 +55,15 @@
         Contact,
         Document,
         InlineKeyboardMarkup,
         InputMediaAudio,
         InputMediaDocument,
         InputMediaPhoto,
         InputMediaVideo,
+        InputPollOption,
         LabeledPrice,
         LinkPreviewOptions,
         Location,
         Message,
         MessageEntity,
         MessageId,
         PhotoSize,
@@ -70,14 +73,53 @@
         Venue,
         Video,
         VideoNote,
         Voice,
     )
 
 
+_deprecated_attrs = (
+    "accent_color_id",
+    "active_usernames",
+    "available_reactions",
+    "background_custom_emoji_id",
+    "bio",
+    "birthdate",
+    "business_intro",
+    "business_location",
+    "business_opening_hours",
+    "can_set_sticker_set",
+    "custom_emoji_sticker_set_name",
+    "description",
+    "emoji_status_custom_emoji_id",
+    "emoji_status_expiration_date",
+    "has_aggressive_anti_spam_enabled",
+    "has_hidden_members",
+    "has_private_forwards",
+    "has_protected_content",
+    "has_restricted_voice_and_video_messages",
+    "has_visible_history",
+    "invite_link",
+    "join_by_request",
+    "join_to_send_messages",
+    "linked_chat_id",
+    "location",
+    "message_auto_delete_time",
+    "permissions",
+    "personal_chat",
+    "photo",
+    "pinned_message",
+    "profile_accent_color_id",
+    "profile_background_custom_emoji_id",
+    "slow_mode_delay",
+    "sticker_set_name",
+    "unrestrict_boost_count",
+)
+
+
 class Chat(TelegramObject):
     """This object represents a chat.
 
     Objects of this class are comparable in terms of equality. Two objects of this class are
     considered equal, if their :attr:`id` is equal.
 
     .. versionchanged:: 20.0
@@ -103,330 +145,610 @@
         title (:obj:`str`, optional): Title, for supergroups, channels and group chats.
         username (:obj:`str`, optional): Username, for private chats, supergroups and channels if
             available.
         first_name (:obj:`str`, optional): First name of the other party in a private chat.
         last_name (:obj:`str`, optional): Last name of the other party in a private chat.
         photo (:class:`telegram.ChatPhoto`, optional): Chat photo.
             Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         bio (:obj:`str`, optional): Bio of the other party in a private chat. Returned only in
             :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_private_forwards (:obj:`bool`, optional): :obj:`True`, if privacy settings of the other
             party in the private chat allows to use ``tg://user?id=<user_id>`` links only in chats
             with the user. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 13.9
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         description (:obj:`str`, optional): Description, for groups, supergroups and channel chats.
             Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         invite_link (:obj:`str`, optional): Primary invite link, for groups, supergroups and
             channel. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         pinned_message (:class:`telegram.Message`, optional): The most recent pinned message
             (by sending date). Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         permissions (:class:`telegram.ChatPermissions`): Optional. Default chat member permissions,
             for groups and supergroups. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         slow_mode_delay (:obj:`int`, optional): For supergroups, the minimum allowed delay between
             consecutive messages sent by each unprivileged user.
             Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         message_auto_delete_time (:obj:`int`, optional): The time after which all messages sent to
             the chat will be automatically deleted; in seconds. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 13.4
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_protected_content (:obj:`bool`, optional): :obj:`True`, if messages from the chat can't
             be forwarded to other chats. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 13.9
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_visible_history (:obj:`bool`, optional): :obj:`True`, if new chat members will have
             access to old messages; available only to chat administrators. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         sticker_set_name (:obj:`str`, optional): For supergroups, name of group sticker set.
             Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         can_set_sticker_set (:obj:`bool`, optional): :obj:`True`, if the bot can change group the
             sticker set. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         linked_chat_id (:obj:`int`, optional): Unique identifier for the linked chat, i.e. the
             discussion group identifier for a channel and vice versa; for supergroups and channel
             chats. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         location (:class:`telegram.ChatLocation`, optional): For supergroups, the location to which
             the supergroup is connected. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         join_to_send_messages (:obj:`bool`, optional): :obj:`True`, if users need to join the
             supergroup before they can send messages. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         join_by_request (:obj:`bool`, optional): :obj:`True`, if all users directly joining the
-            supergroup need to be approved by supergroup administrators. Returned only in
-            :meth:`telegram.Bot.get_chat`.
+            supergroup without using an invite link need to be approved by supergroup
+            administrators. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_restricted_voice_and_video_messages (:obj:`bool`, optional): :obj:`True`, if the
             privacy settings of the other party restrict sending voice and video note messages
             in the private chat. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         is_forum (:obj:`bool`, optional): :obj:`True`, if the supergroup chat is a forum
             (has topics_ enabled).
 
             .. versionadded:: 20.0
         active_usernames (Sequence[:obj:`str`], optional):  If set, the list of all `active chat
             usernames <https://telegram.org/blog/topics-in-groups-collectible-usernames\
             #collectible-usernames>`_; for private chats, supergroups and channels. Returned
             only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         business_intro (:class:`telegram.BusinessIntro`, optional): For private chats with
             business accounts, the intro of the business. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         business_location (:class:`telegram.BusinessLocation`, optional): For private chats with
             business accounts, the location of the business. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         business_opening_hours (:class:`telegram.BusinessOpeningHours`, optional): For private
             chats with business accounts, the opening hours of the business. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         available_reactions (Sequence[:class:`telegram.ReactionType`], optional): List of available
             reactions allowed in the chat. If omitted, then all of
             :const:`telegram.constants.ReactionEmoji` are allowed. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         accent_color_id (:obj:`int`, optional): Identifier of the
             :class:`accent color <telegram.constants.AccentColor>` for the chat name and
             backgrounds of the chat photo, reply header, and link preview. See `accent colors`_
             for more details. Returned only in :meth:`telegram.Bot.get_chat`. Always returned in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         background_custom_emoji_id (:obj:`str`, optional): Custom emoji identifier of emoji chosen
             by the chat for the reply header and link preview background. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         profile_accent_color_id (:obj:`int`, optional): Identifier of the
             :class:`accent color <telegram.constants.ProfileAccentColor>` for the chat's profile
             background. See profile `accent colors`_ for more details. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         profile_background_custom_emoji_id (:obj:`str`, optional): Custom emoji identifier of
             the emoji chosen by the chat for its profile background. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         emoji_status_custom_emoji_id (:obj:`str`, optional): Custom emoji identifier of emoji
             status of the chat or the other party in a private chat. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         emoji_status_expiration_date (:class:`datetime.datetime`, optional): Expiration date of
             emoji status of the chat or the other party in a private chat, in seconds. Returned
             only in :meth:`telegram.Bot.get_chat`.
             |datetime_localization|
 
             .. versionadded:: 20.5
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_aggressive_anti_spam_enabled (:obj:`bool`, optional): :obj:`True`, if aggressive
             anti-spam checks are enabled in the supergroup. The field is only available to chat
             administrators. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_hidden_members (:obj:`bool`, optional): :obj:`True`, if non-administrators can only
             get the list of bots and administrators in the chat. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         unrestrict_boost_count (:obj:`int`, optional): For supergroups, the minimum number of
             boosts that a non-administrator user needs to add in order to ignore slow mode and chat
             permissions. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         custom_emoji_sticker_set_name (:obj:`str`, optional): For supergroups, the name of the
             group's custom emoji sticker set. Custom emoji from this set can be used by all users
             and bots in the group. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         birthdate (:obj:`telegram.Birthdate`, optional): For private chats,
             the date of birth of the user. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         personal_chat (:obj:`telegram.Chat`, optional): For private chats, the personal channel of
             the user. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
 
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
+
     Attributes:
         id (:obj:`int`): Unique identifier for this chat. This number may be greater than 32 bits
             and some programming languages may have difficulty/silent defects in interpreting it.
             But it is smaller than 52 bits, so a signed 64-bit integer or double-precision float
             type are safe for storing this identifier.
         type (:obj:`str`): Type of chat, can be either :attr:`PRIVATE`, :attr:`GROUP`,
             :attr:`SUPERGROUP` or :attr:`CHANNEL`.
         title (:obj:`str`): Optional. Title, for supergroups, channels and group chats.
         username (:obj:`str`): Optional. Username, for private chats, supergroups and channels if
             available.
         first_name (:obj:`str`): Optional. First name of the other party in a private chat.
         last_name (:obj:`str`): Optional. Last name of the other party in a private chat.
         photo (:class:`telegram.ChatPhoto`): Optional. Chat photo.
             Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         bio (:obj:`str`): Optional. Bio of the other party in a private chat. Returned only in
             :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_private_forwards (:obj:`bool`): Optional. :obj:`True`, if privacy settings of the other
             party in the private chat allows to use ``tg://user?id=<user_id>`` links only in chats
             with the user. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 13.9
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         description (:obj:`str`): Optional. Description, for groups, supergroups and channel chats.
             Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         invite_link (:obj:`str`): Optional. Primary invite link, for groups, supergroups and
             channel. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         pinned_message (:class:`telegram.Message`): Optional. The most recent pinned message
             (by sending date). Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         permissions (:class:`telegram.ChatPermissions`): Optional. Default chat member permissions,
             for groups and supergroups. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         slow_mode_delay (:obj:`int`): Optional. For supergroups, the minimum allowed delay between
             consecutive messages sent by each unprivileged user. Returned only in
             :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         message_auto_delete_time (:obj:`int`): Optional. The time after which all messages sent to
             the chat will be automatically deleted; in seconds. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 13.4
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_protected_content (:obj:`bool`): Optional. :obj:`True`, if messages from the chat can't
             be forwarded to other chats. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 13.9
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_visible_history (:obj:`bool`): Optional. :obj:`True`, if new chat members will have
             access to old messages; available only to chat administrators. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         sticker_set_name (:obj:`str`): Optional. For supergroups, name of Group sticker set.
             Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         can_set_sticker_set (:obj:`bool`): Optional. :obj:`True`, if the bot can change group the
             sticker set. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         linked_chat_id (:obj:`int`): Optional. Unique identifier for the linked chat, i.e. the
             discussion group identifier for a channel and vice versa; for supergroups and channel
             chats. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         location (:class:`telegram.ChatLocation`): Optional. For supergroups, the location to which
             the supergroup is connected. Returned only in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         join_to_send_messages (:obj:`bool`): Optional. :obj:`True`, if users need to join
             the supergroup before they can send messages. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
-        join_by_request (:obj:`bool`): Optional. :obj:`True`, if all users directly
-            joining the supergroup need to be approved by supergroup administrators. Returned only
-            in :meth:`telegram.Bot.get_chat`.
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
+        join_by_request (:obj:`bool`): Optional. :obj:`True`, if all users directly joining the
+            supergroup without using an invite link need to be approved by supergroup
+            administrators. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_restricted_voice_and_video_messages (:obj:`bool`): Optional. :obj:`True`, if the
             privacy settings of the other party restrict sending voice and video note messages
             in the private chat. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         is_forum (:obj:`bool`): Optional. :obj:`True`, if the supergroup chat is a forum
             (has topics_ enabled).
 
             .. versionadded:: 20.0
         active_usernames (Tuple[:obj:`str`]): Optional. If set, the list of all `active chat
             usernames <https://telegram.org/blog/topics-in-groups-collectible-usernames\
             #collectible-usernames>`_; for private chats, supergroups and channels. Returned
             only in :meth:`telegram.Bot.get_chat`.
             This list is empty if the chat has no active usernames or this chat instance was not
             obtained via :meth:`~telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         business_intro (:class:`telegram.BusinessIntro`): Optional. For private chats with
             business accounts, the intro of the business. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         business_location (:class:`telegram.BusinessLocation`): Optional. For private chats with
             business accounts, the location of the business. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         business_opening_hours (:class:`telegram.BusinessOpeningHours`): Optional. For private
             chats with business accounts, the opening hours of the business. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         available_reactions (Tuple[:class:`telegram.ReactionType`]): Optional. List of available
             reactions allowed in the chat. If omitted, then all of
             :const:`telegram.constants.ReactionEmoji` are allowed. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         accent_color_id (:obj:`int`): Optional. Identifier of the
             :class:`accent color <telegram.constants.AccentColor>` for the chat name and
             backgrounds of the chat photo, reply header, and link preview. See `accent colors`_
             for more details. Returned only in :meth:`telegram.Bot.get_chat`. Always returned in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         background_custom_emoji_id (:obj:`str`): Optional. Custom emoji identifier of emoji chosen
             by the chat for the reply header and link preview background. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         profile_accent_color_id (:obj:`int`): Optional. Identifier of the
             :class:`accent color <telegram.constants.ProfileAccentColor>` for the chat's profile
             background. See profile `accent colors`_ for more details. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         profile_background_custom_emoji_id (:obj:`str`): Optional. Custom emoji identifier of
             the emoji chosen by the chat for its profile background. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.8
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         emoji_status_custom_emoji_id (:obj:`str`): Optional. Custom emoji identifier of emoji
             status of the chat or the other party in a private chat. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         emoji_status_expiration_date (:class:`datetime.datetime`): Optional. Expiration date of
             emoji status of the chat or the other party in a private chat, in seconds. Returned
             only in :meth:`telegram.Bot.get_chat`.
             |datetime_localization|
 
             .. versionadded:: 20.5
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_aggressive_anti_spam_enabled (:obj:`bool`): Optional. :obj:`True`, if aggressive
             anti-spam checks are enabled in the supergroup. The field is only available to chat
             administrators. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         has_hidden_members (:obj:`bool`): Optional. :obj:`True`, if non-administrators can only
             get the list of bots and administrators in the chat. Returned only in
             :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 20.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         unrestrict_boost_count (:obj:`int`): Optional. For supergroups, the minimum number of
             boosts that a non-administrator user needs to add in order to ignore slow mode and chat
             permissions. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         custom_emoji_sticker_set_name (:obj:`str`): Optional. For supergroups, the name of the
             group's custom emoji sticker set. Custom emoji from this set can be used by all users
             and bots in the group. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.0
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         birthdate (:obj:`telegram.Birthdate`): Optional. For private chats,
             the date of birth of the user. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
+
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
         personal_chat (:obj:`telegram.Chat`): Optional. For private chats, the personal channel of
             the user. Returned only in :meth:`telegram.Bot.get_chat`.
 
             .. versionadded:: 21.1
 
+            .. deprecated:: 21.2
+                In accordance to Bot API 7.3, this attribute will be moved to
+                :class:`telegram.ChatFullInfo`.
+
     .. _topics: https://telegram.org/blog/topics-in-groups-collectible-usernames#topics-in-groups
     .. _accent colors: https://core.telegram.org/bots/api#accent-colors
     """
 
     __slots__ = (
         "accent_color_id",
         "active_usernames",
@@ -467,15 +789,14 @@
         "slow_mode_delay",
         "sticker_set_name",
         "title",
         "type",
         "unrestrict_boost_count",
         "username",
     )
-
     SENDER: Final[str] = constants.ChatType.SENDER
     """:const:`telegram.constants.ChatType.SENDER`
 
     .. versionadded:: 13.5
     """
     PRIVATE: Final[str] = constants.ChatType.PRIVATE
     """:const:`telegram.constants.ChatType.PRIVATE`"""
@@ -514,15 +835,15 @@
         is_forum: Optional[bool] = None,
         active_usernames: Optional[Sequence[str]] = None,
         emoji_status_custom_emoji_id: Optional[str] = None,
         emoji_status_expiration_date: Optional[datetime] = None,
         has_aggressive_anti_spam_enabled: Optional[bool] = None,
         has_hidden_members: Optional[bool] = None,
         available_reactions: Optional[Sequence[ReactionType]] = None,
-        accent_color_id: Optional[int] = None,
+        accent_color_id: Optional[int] = None,  # required in API 7.3 - Optional for back compat
         background_custom_emoji_id: Optional[str] = None,
         profile_accent_color_id: Optional[int] = None,
         profile_background_custom_emoji_id: Optional[str] = None,
         has_visible_history: Optional[bool] = None,
         unrestrict_boost_count: Optional[int] = None,
         custom_emoji_sticker_set_name: Optional[str] = None,
         birthdate: Optional[Birthdate] = None,
@@ -581,18 +902,42 @@
         self.custom_emoji_sticker_set_name: Optional[str] = custom_emoji_sticker_set_name
         self.birthdate: Optional[Birthdate] = birthdate
         self.personal_chat: Optional["Chat"] = personal_chat
         self.business_intro: Optional["BusinessIntro"] = business_intro
         self.business_location: Optional["BusinessLocation"] = business_location
         self.business_opening_hours: Optional["BusinessOpeningHours"] = business_opening_hours
 
+        if self.__class__ is Chat:
+            for arg in _deprecated_attrs:
+                if (val := object.__getattribute__(self, arg)) is not None and val != ():
+                    warn(
+                        PTBDeprecationWarning(
+                            "21.2",
+                            f"The argument `{arg}` is deprecated and will only be available via "
+                            "`ChatFullInfo` in the future.",
+                        ),
+                        stacklevel=2,
+                    )
+
         self._id_attrs = (self.id,)
 
         self._freeze()
 
+    def __getattribute__(self, name: str) -> Any:
+        if name in _deprecated_attrs and self.__class__ is Chat:
+            warn(
+                PTBDeprecationWarning(
+                    "21.2",
+                    f"The attribute `{name}` is deprecated and will only be accessible via "
+                    "`ChatFullInfo` in the future.",
+                ),
+                stacklevel=2,
+            )
+        return super().__getattribute__(name)
+
     @property
     def effective_name(self) -> Optional[str]:
         """
         :obj:`str`: Convenience property. Gives :attr:`title` if not :obj:`None`,
         else :attr:`full_name` if not :obj:`None`.
 
         .. versionadded:: 20.1
@@ -654,15 +999,15 @@
         )
 
         data["pinned_message"] = Message.de_json(data.get("pinned_message"), bot)
         data["permissions"] = ChatPermissions.de_json(data.get("permissions"), bot)
         data["location"] = ChatLocation.de_json(data.get("location"), bot)
         data["available_reactions"] = ReactionType.de_list(data.get("available_reactions"), bot)
         data["birthdate"] = Birthdate.de_json(data.get("birthdate"), bot)
-        data["personal_chat"] = cls.de_json(data.get("personal_chat"), bot)
+        data["personal_chat"] = Chat.de_json(data.get("personal_chat"), bot)
         data["business_intro"] = BusinessIntro.de_json(data.get("business_intro"), bot)
         data["business_location"] = BusinessLocation.de_json(data.get("business_location"), bot)
         data["business_opening_hours"] = BusinessOpeningHours.de_json(
             data.get("business_opening_hours"), bot
         )
 
         api_kwargs = {}
@@ -2541,15 +2886,15 @@
             message_thread_id=message_thread_id,
             business_connection_id=business_connection_id,
         )
 
     async def send_poll(
         self,
         question: str,
-        options: Sequence[str],
+        options: Sequence[Union[str, "InputPollOption"]],
         is_anonymous: Optional[bool] = None,
         type: Optional[str] = None,
         allows_multiple_answers: Optional[bool] = None,
         correct_option_id: Optional[CorrectOptionID] = None,
         is_closed: Optional[bool] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
@@ -2558,14 +2903,16 @@
         open_period: Optional[int] = None,
         close_date: Optional[Union[int, datetime]] = None,
         explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         business_connection_id: Optional[str] = None,
+        question_parse_mode: ODVInput[str] = DEFAULT_NONE,
+        question_entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2604,14 +2951,16 @@
             close_date=close_date,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             explanation_entities=explanation_entities,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             business_connection_id=business_connection_id,
+            question_parse_mode=question_parse_mode,
+            question_entities=question_entities,
         )
 
     async def send_copy(
         self,
         from_chat_id: Union[str, int],
         message_id: int,
         caption: Optional[str] = None,
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_chatadministratorrights.py` & `python-telegram-bot-raw-21.2/telegram/_chatadministratorrights.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,17 @@
             messages; for groups and supergroups only.
         can_post_stories (:obj:`bool`): :obj:`True`, if the administrator can post
             stories to the chat.
 
             .. versionadded:: 20.6
             .. versionchanged:: 21.0
                 |non_optional_story_argument|
-        can_edit_stories (:obj:`bool`): :obj:`True`, if the administrator can edit
-            stories posted by other users.
+        can_edit_stories (:obj:`bool`): :obj:`True`, if the administrator can edit stories posted
+            by other users, post stories to the chat page, pin chat stories, and access the chat's
+            story archive
 
             .. versionadded:: 20.6
             .. versionchanged:: 21.0
                 |non_optional_story_argument|
         can_delete_stories (:obj:`bool`): :obj:`True`, if the administrator can delete
             stories posted by other users.
 
@@ -124,16 +125,17 @@
             messages; for groups and supergroups only.
         can_post_stories (:obj:`bool`): :obj:`True`, if the administrator can post
             stories to the chat.
 
             .. versionadded:: 20.6
             .. versionchanged:: 21.0
                 |non_optional_story_argument|
-        can_edit_stories (:obj:`bool`): :obj:`True`, if the administrator can edit
-            stories posted by other users.
+        can_edit_stories (:obj:`bool`): :obj:`True`, if the administrator can edit stories posted
+            by other users, post stories to the chat page, pin chat stories, and access the chat's
+            story archive
 
             .. versionadded:: 20.6
             .. versionchanged:: 21.0
                 |non_optional_story_argument|
         can_delete_stories (:obj:`bool`): :obj:`True`, if the administrator can delete
             stories posted by other users.
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_chatboost.py` & `python-telegram-bot-raw-21.2/telegram/_chatboost.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_chatinvitelink.py` & `python-telegram-bot-raw-21.2/telegram/_chatinvitelink.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_chatjoinrequest.py` & `python-telegram-bot-raw-21.2/telegram/_chatjoinrequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_chatlocation.py` & `python-telegram-bot-raw-21.2/telegram/_chatlocation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_chatmember.py` & `python-telegram-bot-raw-21.2/telegram/_chatmember.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,16 +231,17 @@
             to pin messages; for groups and supergroups only.
         can_post_stories (:obj:`bool`): :obj:`True`, if the administrator can post
             stories to the chat.
 
             .. versionadded:: 20.6
             .. versionchanged:: 21.0
                 |non_optional_story_argument|
-        can_edit_stories (:obj:`bool`): :obj:`True`, if the administrator can edit
-            stories posted by other users.
+        can_edit_stories (:obj:`bool`): :obj:`True`, if the administrator can edit stories posted
+            by other users, post stories to the chat page, pin chat stories, and access the chat's
+            story archive
 
             .. versionadded:: 20.6
             .. versionchanged:: 21.0
                 |non_optional_story_argument|
         can_delete_stories (:obj:`bool`): :obj:`True`, if the administrator can delete
             stories posted by other users.
 
@@ -290,16 +291,17 @@
             to pin messages; for groups and supergroups only.
         can_post_stories (:obj:`bool`): :obj:`True`, if the administrator can post
             stories to the chat.
 
             .. versionadded:: 20.6
             .. versionchanged:: 21.0
                 |non_optional_story_argument|
-        can_edit_stories (:obj:`bool`): :obj:`True`, if the administrator can edit
-            stories posted by other users.
+        can_edit_stories (:obj:`bool`): :obj:`True`, if the administrator can edit stories posted
+            by other users, post stories to the chat page, pin chat stories, and access the chat's
+            story archive
 
             .. versionadded:: 20.6
             .. versionchanged:: 21.0
                 |non_optional_story_argument|
         can_delete_stories (:obj:`bool`): :obj:`True`, if the administrator can delete
             stories posted by other users.
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_chatmemberupdated.py` & `python-telegram-bot-raw-21.2/telegram/_chatmemberupdated.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,19 @@
         new_chat_member (:class:`telegram.ChatMember`): New information about the chat member.
         invite_link (:class:`telegram.ChatInviteLink`, optional): Chat invite link, which was used
             by the user to join the chat. For joining by invite link events only.
         via_chat_folder_invite_link (:obj:`bool`, optional): :obj:`True`, if the user joined the
             chat via a chat folder invite link
 
             .. versionadded:: 20.3
+        via_join_request (:obj:`bool`, optional): :obj:`True`, if the user joined the chat after
+            sending a direct join request without using an invite link and being approved by
+            an administrator
+
+            .. versionadded:: 21.2
 
     Attributes:
         chat (:class:`telegram.Chat`): Chat the user belongs to.
         from_user (:class:`telegram.User`): Performer of the action, which resulted in the change.
         date (:class:`datetime.datetime`): Date the change was done in Unix time. Converted to
             :class:`datetime.datetime`.
 
@@ -76,50 +81,58 @@
         new_chat_member (:class:`telegram.ChatMember`): New information about the chat member.
         invite_link (:class:`telegram.ChatInviteLink`): Optional. Chat invite link, which was used
             by the user to join the chat. For joining by invite link events only.
         via_chat_folder_invite_link (:obj:`bool`): Optional. :obj:`True`, if the user joined the
             chat via a chat folder invite link
 
             .. versionadded:: 20.3
+        via_join_request (:obj:`bool`): Optional. :obj:`True`, if the user joined the chat after
+            sending a direct join request without using an invite link and being approved
+            by an administrator
+
+            .. versionadded:: 21.2
 
     """
 
     __slots__ = (
         "chat",
         "date",
         "from_user",
         "invite_link",
         "new_chat_member",
         "old_chat_member",
         "via_chat_folder_invite_link",
+        "via_join_request",
     )
 
     def __init__(
         self,
         chat: Chat,
         from_user: User,
         date: datetime.datetime,
         old_chat_member: ChatMember,
         new_chat_member: ChatMember,
         invite_link: Optional[ChatInviteLink] = None,
         via_chat_folder_invite_link: Optional[bool] = None,
+        via_join_request: Optional[bool] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.chat: Chat = chat
         self.from_user: User = from_user
         self.date: datetime.datetime = date
         self.old_chat_member: ChatMember = old_chat_member
         self.new_chat_member: ChatMember = new_chat_member
         self.via_chat_folder_invite_link: Optional[bool] = via_chat_folder_invite_link
 
         # Optionals
         self.invite_link: Optional[ChatInviteLink] = invite_link
+        self.via_join_request: Optional[bool] = via_join_request
 
         self._id_attrs = (
             self.chat,
             self.from_user,
             self.date,
             self.old_chat_member,
             self.new_chat_member,
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_chatpermissions.py` & `python-telegram-bot-raw-21.2/telegram/_chatpermissions.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_choseninlineresult.py` & `python-telegram-bot-raw-21.2/telegram/_choseninlineresult.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_dice.py` & `python-telegram-bot-raw-21.2/telegram/_dice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/_basemedium.py` & `python-telegram-bot-raw-21.2/telegram/_files/_basemedium.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/_basethumbedmedium.py` & `python-telegram-bot-raw-21.2/telegram/_files/_basethumbedmedium.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/animation.py` & `python-telegram-bot-raw-21.2/telegram/_files/animation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/audio.py` & `python-telegram-bot-raw-21.2/telegram/_files/audio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/chatphoto.py` & `python-telegram-bot-raw-21.2/telegram/_files/chatphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/contact.py` & `python-telegram-bot-raw-21.2/telegram/_files/contact.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/document.py` & `python-telegram-bot-raw-21.2/telegram/_files/document.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/file.py` & `python-telegram-bot-raw-21.2/telegram/_files/file.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/inputfile.py` & `python-telegram-bot-raw-21.2/telegram/_files/inputfile.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/inputmedia.py` & `python-telegram-bot-raw-21.2/telegram/_files/inputmedia.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/inputsticker.py` & `python-telegram-bot-raw-21.2/telegram/_files/inputsticker.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/location.py` & `python-telegram-bot-raw-21.2/telegram/_files/location.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/photosize.py` & `python-telegram-bot-raw-21.2/telegram/_files/photosize.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/sticker.py` & `python-telegram-bot-raw-21.2/telegram/_files/sticker.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 from telegram._files._basethumbedmedium import _BaseThumbedMedium
 from telegram._files.file import File
 from telegram._files.photosize import PhotoSize
 from telegram._telegramobject import TelegramObject
 from telegram._utils import enum
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.types import JSONDict
-from telegram._utils.warnings import warn
-from telegram.warnings import PTBDeprecationWarning
 
 if TYPE_CHECKING:
     from telegram import Bot
 
 
 class Sticker(_BaseThumbedMedium):
     """This object represents a sticker.
@@ -233,28 +231,20 @@
     .. versionchanged:: 21.1
         The parameters ``is_video`` and ``is_animated`` are deprecated and now made optional. Thus,
         the order of the arguments had to be changed.
 
     .. versionchanged:: 20.5
        |removed_thumb_note|
 
+    .. versionremoved:: 21.2
+       Removed the deprecated arguments and attributes ``is_animated`` and ``is_video``.
+
     Args:
         name (:obj:`str`): Sticker set name.
         title (:obj:`str`): Sticker set title.
-        is_animated (:obj:`bool`): :obj:`True`, if the sticker set contains animated stickers.
-
-            .. deprecated:: 21.1
-                Bot API 7.2 deprecated this field. This parameter will be removed in a future
-                version of the library.
-        is_video (:obj:`bool`): :obj:`True`, if the sticker set contains video stickers.
-            .. versionadded:: 13.11
-
-            .. deprecated:: 21.1
-                Bot API 7.2 deprecated this field. This parameter will be removed in a future
-                version of the library.
         stickers (Sequence[:class:`telegram.Sticker`]): List of all set stickers.
 
             .. versionchanged:: 20.0
                 |sequenceclassargs|
 
         sticker_type (:obj:`str`): Type of stickers in the set, currently one of
             :attr:`telegram.Sticker.REGULAR`, :attr:`telegram.Sticker.MASK`,
@@ -265,25 +255,14 @@
             ``.TGS``, or ``.WEBM`` format.
 
             .. versionadded:: 20.2
 
     Attributes:
         name (:obj:`str`): Sticker set name.
         title (:obj:`str`): Sticker set title.
-        is_animated (:obj:`bool`): :obj:`True`, if the sticker set contains animated stickers.
-
-            .. deprecated:: 21.1
-                Bot API 7.2 deprecated this field. This parameter will be removed in a future
-                version of the library.
-        is_video (:obj:`bool`): :obj:`True`, if the sticker set contains video stickers.
-            .. versionadded:: 13.11
-
-            .. deprecated:: 21.1
-                Bot API 7.2 deprecated this field. This parameter will be removed in a future
-                version of the library.
         stickers (Tuple[:class:`telegram.Sticker`]): List of all set stickers.
 
             .. versionchanged:: 20.0
                 |tupleclassattrs|
 
         sticker_type (:obj:`str`): Type of stickers in the set, currently one of
             :attr:`telegram.Sticker.REGULAR`, :attr:`telegram.Sticker.MASK`,
@@ -293,51 +272,38 @@
         thumbnail (:class:`telegram.PhotoSize`): Optional. Sticker set thumbnail in the ``.WEBP``,
             ``.TGS``, or ``.WEBM`` format.
 
             .. versionadded:: 20.2
     """
 
     __slots__ = (
-        "is_animated",
-        "is_video",
         "name",
         "sticker_type",
         "stickers",
         "thumbnail",
         "title",
     )
 
     def __init__(
         self,
         name: str,
         title: str,
         stickers: Sequence[Sticker],
         sticker_type: str,
-        is_animated: Optional[bool] = None,
-        is_video: Optional[bool] = None,
         thumbnail: Optional[PhotoSize] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.name: str = name
         self.title: str = title
         self.stickers: Tuple[Sticker, ...] = parse_sequence_arg(stickers)
         self.sticker_type: str = sticker_type
         # Optional
         self.thumbnail: Optional[PhotoSize] = thumbnail
-        if is_animated is not None or is_video is not None:
-            warn(
-                "The parameters `is_animated` and `is_video` are deprecated and will be removed "
-                "in a future version.",
-                PTBDeprecationWarning,
-                stacklevel=2,
-            )
-        self.is_animated: Optional[bool] = is_animated
-        self.is_video: Optional[bool] = is_video
         self._id_attrs = (self.name,)
 
         self._freeze()
 
     @classmethod
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["StickerSet"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
@@ -346,15 +312,15 @@
 
         data["thumbnail"] = PhotoSize.de_json(data.get("thumbnail"), bot)
         data["stickers"] = Sticker.de_list(data.get("stickers"), bot)
 
         api_kwargs = {}
         # These are deprecated fields that TG still returns for backwards compatibility
         # Let's filter them out to speed up the de-json process
-        for deprecated_field in ("contains_masks", "thumb"):
+        for deprecated_field in ("contains_masks", "thumb", "is_animated", "is_video"):
             if deprecated_field in data:
                 api_kwargs[deprecated_field] = data.pop(deprecated_field)
 
         return super()._de_json(data=data, bot=bot, api_kwargs=api_kwargs)
 
 
 class MaskPosition(TelegramObject):
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/venue.py` & `python-telegram-bot-raw-21.2/telegram/_files/venue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/video.py` & `python-telegram-bot-raw-21.2/telegram/_files/video.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/videonote.py` & `python-telegram-bot-raw-21.2/telegram/_files/videonote.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_files/voice.py` & `python-telegram-bot-raw-21.2/telegram/_files/voice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_forcereply.py` & `python-telegram-bot-raw-21.2/telegram/_forcereply.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 
 class ForceReply(TelegramObject):
     """
     Upon receiving a message with this object, Telegram clients will display a reply interface to
     the user (act as if the user has selected the bot's message and tapped 'Reply'). This can be
     extremely useful if you want to create user-friendly step-by-step interfaces without having
-    to sacrifice privacy mode.
+    to sacrifice `privacy mode <https://core.telegram.org/bots/features#privacy-mode>`_. Not
+    supported in channels and for messages sent on behalf of a Telegram Business account.
 
     Objects of this class are comparable in terms of equality. Two objects of this class are
     considered equal, if their :attr:`selective` is equal.
 
     .. versionchanged:: 20.0
         The (undocumented) argument ``force_reply`` was removed and instead :attr:`force_reply`
         is now always set to :obj:`True` as expected by the Bot API.
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_forumtopic.py` & `python-telegram-bot-raw-21.2/telegram/_forumtopic.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_games/callbackgame.py` & `python-telegram-bot-raw-21.2/telegram/_games/callbackgame.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_games/game.py` & `python-telegram-bot-raw-21.2/telegram/_games/game.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_games/gamehighscore.py` & `python-telegram-bot-raw-21.2/telegram/_games/gamehighscore.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_giveaway.py` & `python-telegram-bot-raw-21.2/telegram/_giveaway.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinekeyboardbutton.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinekeyboardbutton.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,54 +87,56 @@
 
             Caution:
                 Only ``HTTPS`` links are allowed after Bot API 6.1.
         callback_data (:obj:`str` | :obj:`object`, optional): Data to be sent in a callback query
             to the bot when button is pressed, UTF-8
             :tg-const:`telegram.InlineKeyboardButton.MIN_CALLBACK_DATA`-
             :tg-const:`telegram.InlineKeyboardButton.MAX_CALLBACK_DATA` bytes.
+            Not supported for messages sent on behalf of a Telegram Business account.
             If the bot instance allows arbitrary callback data, anything can be passed.
 
             Tip:
                 The value entered here will be available in :attr:`telegram.CallbackQuery.data`.
 
             .. seealso:: :wiki:`Arbitrary callback_data <Arbitrary-callback_data>`
 
         web_app (:obj:`telegram.WebAppInfo`, optional): Description of the `Web App
             <https://core.telegram.org/bots/webapps>`_  that will be launched when the user presses
             the button. The Web App will be able to send an arbitrary message on behalf of the user
             using the method :meth:`~telegram.Bot.answer_web_app_query`. Available only in
-            private chats between a user and the bot.
+            private chats between a user and the bot. Not supported for messages sent on behalf of
+            a Telegram Business account.
 
             .. versionadded:: 20.0
-        switch_inline_query (:obj:`str`, optional): If set, pressing the button will prompt the
-            user to select one of their chats, open that chat and insert the bot's username and the
-            specified inline query in the input field. Can be empty, in which case just the bot's
-            username will be inserted. This offers an easy way for users to start using your bot
-            in inline mode when they are currently in a private chat with it. Especially useful
-            when combined with ``switch_pm*`` actions - in this case the user will be automatically
-            returned to the chat they switched from, skipping the chat selection screen.
+        switch_inline_query (:obj:`str`, optional): If set, pressing the button will insert the
+            bot's username and the specified inline query in the current chat's input field. May be
+            empty, in which case only the bot's username will be inserted.
+
+            This offers a quick way for the user to open your bot in inline mode in the same chat -
+            good for selecting something from multiple options. Not supported in channels and for
+            messages sent on behalf of a Telegram Business account.
 
             Tip:
                 This is similar to the new parameter :paramref:`switch_inline_query_chosen_chat`,
                 but gives no control over which chats can be selected.
         switch_inline_query_current_chat (:obj:`str`, optional): If set, pressing the button will
-            insert the bot's username and the specified inline query in the current chat's input
-            field. Can be empty, in which case only the bot's username will be inserted. This
-            offers a quick way for the user to open your bot in inline mode in the same chat - good
-            for selecting something from multiple options.
+            prompt the user to select one of their chats of the specified type, open that chat and
+            insert the bot's username and the specified inline query in the input field. Not
+            supported for messages sent on behalf of a Telegram Business account.
         callback_game (:class:`telegram.CallbackGame`, optional): Description of the game that will
             be launched when the user presses the button. This type of button **must** always be
             the **first** button in the first row.
         pay (:obj:`bool`, optional): Specify :obj:`True`, to send a Pay button. This type of button
             **must** always be the **first** button in the first row and can only be used in
             invoice messages.
         switch_inline_query_chosen_chat (:obj:`telegram.SwitchInlineQueryChosenChat`, optional):
             If set, pressing the button will prompt the user to select one of their chats of the
             specified type, open that chat and insert the bot's username and the specified inline
-            query in the input field.
+            query in the input field. Not supported for messages sent on behalf of a Telegram
+            Business account.
 
             .. versionadded:: 20.3
 
             Tip:
                 This is similar to :paramref:`switch_inline_query`, but gives more control on
                 which chats can be selected.
 
@@ -155,47 +157,49 @@
 
             Caution:
                 Only ``HTTPS`` links are allowed after Bot API 6.1.
         callback_data (:obj:`str` | :obj:`object`): Optional. Data to be sent in a callback query
             to the bot when button is pressed, UTF-8
             :tg-const:`telegram.InlineKeyboardButton.MIN_CALLBACK_DATA`-
             :tg-const:`telegram.InlineKeyboardButton.MAX_CALLBACK_DATA` bytes.
+            Not supported for messages sent on behalf of a Telegram Business account.
         web_app (:obj:`telegram.WebAppInfo`): Optional. Description of the `Web App
             <https://core.telegram.org/bots/webapps>`_  that will be launched when the user presses
             the button. The Web App will be able to send an arbitrary message on behalf of the user
             using the method :meth:`~telegram.Bot.answer_web_app_query`. Available only in
-            private chats between a user and the bot.
+            private chats between a user and the bot. Not supported for messages sent on behalf of
+            a Telegram Business account.
 
             .. versionadded:: 20.0
-        switch_inline_query (:obj:`str`): Optional. If set, pressing the button will prompt the
-            user to select one of their chats, open that chat and insert the bot's username and the
-            specified inline query in the input field. Can be empty, in which case just the bot's
-            username will be inserted. This offers an easy way for users to start using your bot
-            in inline mode when they are currently in a private chat with it. Especially useful
-            when combined with ``switch_pm*`` actions - in this case the user will be automatically
-            returned to the chat they switched from, skipping the chat selection screen.
+        switch_inline_query (:obj:`str`): Optional. If set, pressing the button will insert the
+            bot's username and the specified inline query in the current chat's input field. May be
+            empty, in which case only the bot's username will be inserted.
+
+            This offers a quick way for the user to open your bot in inline mode in the same chat -
+            good for selecting something from multiple options. Not supported in channels and for
+            messages sent on behalf of a Telegram Business account.
 
             Tip:
                 This is similar to the new parameter :paramref:`switch_inline_query_chosen_chat`,
                 but gives no control over which chats can be selected.
         switch_inline_query_current_chat (:obj:`str`): Optional. If set, pressing the button will
-            insert the bot's username and the specified inline query in the current chat's input
-            field. Can be empty, in which case only the bot's username will be inserted. This
-            offers a quick way for the user to open your bot in inline mode in the same chat - good
-            for selecting something from multiple options.
+            prompt the user to select one of their chats of the specified type, open that chat and
+            insert the bot's username and the specified inline query in the input field. Not
+            supported for messages sent on behalf of a Telegram Business account.
         callback_game (:class:`telegram.CallbackGame`): Optional. Description of the game that will
             be launched when the user presses the button. This type of button **must** always be
             the **first** button in the first row.
         pay (:obj:`bool`): Optional. Specify :obj:`True`, to send a Pay button. This type of button
             **must** always be the **first** button in the first row and can only be used in
             invoice messages.
         switch_inline_query_chosen_chat (:obj:`telegram.SwitchInlineQueryChosenChat`): Optional.
             If set, pressing the button will prompt the user to select one of their chats of the
             specified type, open that chat and insert the bot's username and the specified inline
-            query in the input field.
+            query in the input field. Not supported for messages sent on behalf of a Telegram
+            Business account.
 
             .. versionadded:: 20.3
 
             Tip:
                 This is similar to :attr:`switch_inline_query`, but gives more control on
                 which chats can be selected.
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinekeyboardmarkup.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinekeyboardmarkup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequery.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresult.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresult.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultarticle.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultarticle.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultaudio.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultaudio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedaudio.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedaudio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcacheddocument.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcacheddocument.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedgif.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedgif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedmpeg4gif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedphoto.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedsticker.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedsticker.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedvideo.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedvideo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedvoice.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcachedvoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcontact.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultcontact.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultdocument.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultdocument.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultgame.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultgame.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultgif.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultgif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultlocation.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultlocation.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,17 @@
         title (:obj:`str`): Location title.
         horizontal_accuracy (:obj:`float`): Optional. The radius of uncertainty for the location,
             measured in meters; 0-
             :tg-const:`telegram.InlineQueryResultLocation.HORIZONTAL_ACCURACY`.
         live_period (:obj:`int`): Optional. Period in seconds for which the location will be
             updated, should be between
             :tg-const:`telegram.InlineQueryResultLocation.MIN_LIVE_PERIOD` and
-            :tg-const:`telegram.InlineQueryResultLocation.MAX_LIVE_PERIOD`.
+            :tg-const:`telegram.InlineQueryResultLocation.MAX_LIVE_PERIOD` or
+            :tg-const:`telegram.constants.LocationLimit.LIVE_PERIOD_FOREVER` for live
+            locations that can be edited indefinitely.
         heading (:obj:`int`): Optional. For live locations, a direction in which the user is
             moving, in degrees. Must be between
             :tg-const:`telegram.InlineQueryResultLocation.MIN_HEADING` and
             :tg-const:`telegram.InlineQueryResultLocation.MAX_HEADING` if specified.
         proximity_alert_radius (:obj:`int`): Optional. For live locations, a maximum distance
             for proximity alerts about approaching another chat member, in meters. Must be
             between :tg-const:`telegram.InlineQueryResultLocation.MIN_PROXIMITY_ALERT_RADIUS`
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultmpeg4gif.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultmpeg4gif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultphoto.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultsbutton.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultsbutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvenue.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultvenue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvideo.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultvideo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvoice.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inlinequeryresultvoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inputcontactmessagecontent.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inputcontactmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inputinvoicemessagecontent.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inputinvoicemessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inputlocationmessagecontent.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inputlocationmessagecontent.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,17 @@
         longitude (:obj:`float`): Longitude of the location in degrees.
         horizontal_accuracy (:obj:`float`, optional): The radius of uncertainty for the location,
             measured in meters; 0-
             :tg-const:`telegram.InputLocationMessageContent.HORIZONTAL_ACCURACY`.
         live_period (:obj:`int`, optional): Period in seconds for which the location will be
             updated, should be between
             :tg-const:`telegram.InputLocationMessageContent.MIN_LIVE_PERIOD` and
-            :tg-const:`telegram.InputLocationMessageContent.MAX_LIVE_PERIOD`.
+            :tg-const:`telegram.InputLocationMessageContent.MAX_LIVE_PERIOD` or
+            :tg-const:`telegram.constants.LocationLimit.LIVE_PERIOD_FOREVER` for live
+            locations that can be edited indefinitely.
         heading (:obj:`int`, optional): For live locations, a direction in which the user is
             moving, in degrees. Must be between
             :tg-const:`telegram.InputLocationMessageContent.MIN_HEADING` and
             :tg-const:`telegram.InputLocationMessageContent.MAX_HEADING` if specified.
         proximity_alert_radius (:obj:`int`, optional): For live locations, a maximum distance
             for proximity alerts about approaching another chat member, in meters. Must be
             between :tg-const:`telegram.InputLocationMessageContent.MIN_PROXIMITY_ALERT_RADIUS`
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inputmessagecontent.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inputmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inputtextmessagecontent.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inputtextmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_inline/inputvenuemessagecontent.py` & `python-telegram-bot-raw-21.2/telegram/_inline/inputvenuemessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_keyboardbutton.py` & `python-telegram-bot-raw-21.2/telegram/_keyboardbutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_keyboardbuttonpolltype.py` & `python-telegram-bot-raw-21.2/telegram/_keyboardbuttonpolltype.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_keyboardbuttonrequest.py` & `python-telegram-bot-raw-21.2/telegram/_keyboardbuttonrequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_linkpreviewoptions.py` & `python-telegram-bot-raw-21.2/telegram/_linkpreviewoptions.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_loginurl.py` & `python-telegram-bot-raw-21.2/telegram/_loginurl.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_menubutton.py` & `python-telegram-bot-raw-21.2/telegram/_menubutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_message.py` & `python-telegram-bot-raw-21.2/telegram/_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import datetime
 import re
 from html import escape
 from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Tuple, TypedDict, Union
 
 from telegram._chat import Chat
+from telegram._chatbackground import ChatBackground
 from telegram._chatboost import ChatBoostAdded
 from telegram._dice import Dice
 from telegram._files.animation import Animation
 from telegram._files.audio import Audio
 from telegram._files.contact import Contact
 from telegram._files.document import Document
 from telegram._files.location import Location
@@ -60,14 +61,15 @@
 from telegram._shared import ChatShared, UsersShared
 from telegram._story import Story
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.defaultvalue import DEFAULT_NONE, DefaultValue
+from telegram._utils.entities import parse_message_entities, parse_message_entity
 from telegram._utils.types import (
     CorrectOptionID,
     FileInput,
     JSONDict,
     MarkdownVersion,
     ODVInput,
     ReplyMarkup,
@@ -95,14 +97,15 @@
         GiveawayCreated,
         GiveawayWinners,
         InputMedia,
         InputMediaAudio,
         InputMediaDocument,
         InputMediaPhoto,
         InputMediaVideo,
+        InputPollOption,
         LabeledPrice,
         MessageId,
         MessageOrigin,
         ReactionType,
         TextQuote,
     )
 
@@ -194,15 +197,15 @@
         # this is to include the Literal from InaccessibleMessage
         if data["date"] == 0:
             data["date"] = ZERO_DATE
         else:
             data["date"] = from_timestamp(data["date"], tzinfo=loc_tzinfo)
 
         data["chat"] = Chat.de_json(data.get("chat"), bot)
-        return super()._de_json(data=data, bot=bot)
+        return super()._de_json(data=data, bot=bot, api_kwargs=api_kwargs)
 
 
 class InaccessibleMessage(MaybeInaccessibleMessage):
     """This object represents an inaccessible message.
 
     These are messages that are e.g. deleted.
 
@@ -549,14 +552,19 @@
 
         sender_business_bot (:obj:`telegram.User`, optional): The bot that actually sent the
             message on behalf of the business account. Available only for outgoing messages sent
             on behalf of the connected business account.
 
             .. versionadded:: 21.1
 
+        chat_background_set  (:obj:`telegram.ChatBackground`, optional): Service message: chat
+            background set.
+
+            .. versionadded:: 21.2
+
     Attributes:
         message_id (:obj:`int`): Unique message identifier inside this chat.
         from_user (:class:`telegram.User`): Optional. Sender of the message; empty for messages
             sent to channels. For backward compatibility, this will contain a fake sender user in
             non-channel chats, if the message was sent on behalf of a chat.
         sender_chat (:class:`telegram.Chat`): Optional. Sender of the message, sent on behalf of a
             chat. For example, the channel itself for channel posts, the supergroup itself for
@@ -849,14 +857,19 @@
 
         sender_business_bot (:obj:`telegram.User`): Optional. The bot that actually sent the
             message on behalf of the business account. Available only for outgoing messages sent
             on behalf of the connected business account.
 
             .. versionadded:: 21.1
 
+        chat_background_set (:obj:`telegram.ChatBackground`): Optional. Service message: chat
+            background set
+
+            .. versionadded:: 21.2
+
     .. |custom_emoji_no_md1_support| replace:: Since custom emoji entities are not supported by
        :attr:`~telegram.constants.ParseMode.MARKDOWN`, this method now raises a
        :exc:`ValueError` when encountering a custom emoji.
 
     .. |blockquote_no_md1_support| replace:: Since block quotation entities are not supported
        by :attr:`~telegram.constants.ParseMode.MARKDOWN`, this method now raises a
        :exc:`ValueError` when encountering a block quotation.
@@ -872,14 +885,15 @@
         "audio",
         "author_signature",
         "boost_added",
         "business_connection_id",
         "caption",
         "caption_entities",
         "channel_chat_created",
+        "chat_background_set",
         "chat_shared",
         "connected_website",
         "contact",
         "delete_chat_photo",
         "dice",
         "document",
         "edit_date",
@@ -1025,14 +1039,15 @@
         forward_origin: Optional["MessageOrigin"] = None,
         reply_to_story: Optional[Story] = None,
         boost_added: Optional[ChatBoostAdded] = None,
         sender_boost_count: Optional[int] = None,
         business_connection_id: Optional[str] = None,
         sender_business_bot: Optional[User] = None,
         is_from_offline: Optional[bool] = None,
+        chat_background_set: Optional[ChatBackground] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(chat=chat, message_id=message_id, date=date, api_kwargs=api_kwargs)
 
         with self._unfrozen():
             # Required
@@ -1123,14 +1138,15 @@
             self.forward_origin: Optional[MessageOrigin] = forward_origin
             self.reply_to_story: Optional[Story] = reply_to_story
             self.boost_added: Optional[ChatBoostAdded] = boost_added
             self.sender_boost_count: Optional[int] = sender_boost_count
             self.business_connection_id: Optional[str] = business_connection_id
             self.sender_business_bot: Optional[User] = sender_business_bot
             self.is_from_offline: Optional[bool] = is_from_offline
+            self.chat_background_set: Optional[ChatBackground] = chat_background_set
 
             self._effective_attachment = DEFAULT_NONE
 
             self._id_attrs = (self.message_id, self.chat)
 
     @property
     def chat_id(self) -> int:
@@ -1237,14 +1253,15 @@
             data.get("general_forum_topic_unhidden"), bot
         )
         data["write_access_allowed"] = WriteAccessAllowed.de_json(
             data.get("write_access_allowed"), bot
         )
         data["users_shared"] = UsersShared.de_json(data.get("users_shared"), bot)
         data["chat_shared"] = ChatShared.de_json(data.get("chat_shared"), bot)
+        data["chat_background_set"] = ChatBackground.de_json(data.get("chat_background_set"), bot)
 
         # Unfortunately, this needs to be here due to cyclic imports
         from telegram._giveaway import (  # pylint: disable=import-outside-toplevel
             Giveaway,
             GiveawayCompleted,
             GiveawayCreated,
             GiveawayWinners,
@@ -1558,17 +1575,19 @@
         if reply_to_message_id is not None and reply_parameters is not None:
             raise ValueError(
                 "`reply_to_message_id` and `reply_parameters` are mutually exclusive."
             )
 
         if quote is not None:
             warn(
-                "The `quote` parameter is deprecated in favor of the `do_quote` parameter. Please "
-                "update your code to use `do_quote` instead.",
-                PTBDeprecationWarning,
+                PTBDeprecationWarning(
+                    "20.8",
+                    "The `quote` parameter is deprecated in favor of the `do_quote` parameter. "
+                    "Please update your code to use `do_quote` instead.",
+                ),
                 stacklevel=2,
             )
 
         effective_do_quote = quote or do_quote
         chat_id: Union[str, int] = self.chat_id
 
         # reply_parameters and reply_to_message_id overrule the do_quote parameter
@@ -2886,15 +2905,15 @@
             message_thread_id=message_thread_id,
             business_connection_id=self.business_connection_id,
         )
 
     async def reply_poll(
         self,
         question: str,
-        options: Sequence[str],
+        options: Sequence[Union[str, "InputPollOption"]],
         is_anonymous: Optional[bool] = None,
         type: Optional[str] = None,  # pylint: disable=redefined-builtin
         allows_multiple_answers: Optional[bool] = None,
         correct_option_id: Optional[CorrectOptionID] = None,
         is_closed: Optional[bool] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
@@ -2902,14 +2921,16 @@
         explanation_parse_mode: ODVInput[str] = DEFAULT_NONE,
         open_period: Optional[int] = None,
         close_date: Optional[Union[int, datetime.datetime]] = None,
         explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
+        question_parse_mode: ODVInput[str] = DEFAULT_NONE,
+        question_entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2972,14 +2993,16 @@
             close_date=close_date,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             explanation_entities=explanation_entities,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             business_connection_id=self.business_connection_id,
+            question_parse_mode=question_parse_mode,
+            question_entities=question_entities,
         )
 
     async def reply_dice(
         self,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         emoji: Optional[str] = None,
@@ -3649,14 +3672,15 @@
         self,
         latitude: Optional[float] = None,
         longitude: Optional[float] = None,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         horizontal_accuracy: Optional[float] = None,
         heading: Optional[int] = None,
         proximity_alert_radius: Optional[int] = None,
+        live_period: Optional[int] = None,
         *,
         location: Optional[Location] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
@@ -3690,14 +3714,15 @@
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             horizontal_accuracy=horizontal_accuracy,
             heading=heading,
             proximity_alert_radius=proximity_alert_radius,
+            live_period=live_period,
             inline_message_id=None,
         )
 
     async def stop_live_location(
         self,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
@@ -4180,17 +4205,15 @@
         Raises:
             RuntimeError: If the message has no text.
 
         """
         if not self.text:
             raise RuntimeError("This Message has no 'text'.")
 
-        entity_text = self.text.encode("utf-16-le")
-        entity_text = entity_text[entity.offset * 2 : (entity.offset + entity.length) * 2]
-        return entity_text.decode("utf-16-le")
+        return parse_message_entity(self.text, entity)
 
     def parse_caption_entity(self, entity: MessageEntity) -> str:
         """Returns the text from a given :class:`telegram.MessageEntity`.
 
         Note:
             This method is present because Telegram calculates the offset and length in
             UTF-16 codepoint pairs, which some versions of Python don't handle automatically.
@@ -4206,17 +4229,15 @@
         Raises:
             RuntimeError: If the message has no caption.
 
         """
         if not self.caption:
             raise RuntimeError("This Message has no 'caption'.")
 
-        entity_text = self.caption.encode("utf-16-le")
-        entity_text = entity_text[entity.offset * 2 : (entity.offset + entity.length) * 2]
-        return entity_text.decode("utf-16-le")
+        return parse_message_entity(self.caption, entity)
 
     def parse_entities(self, types: Optional[List[str]] = None) -> Dict[MessageEntity, str]:
         """
         Returns a :obj:`dict` that maps :class:`telegram.MessageEntity` to :obj:`str`.
         It contains entities from this message filtered by their
         :attr:`telegram.MessageEntity.type` attribute as the key, and the text that each entity
         belongs to as the value of the :obj:`dict`.
@@ -4233,20 +4254,15 @@
                 in :class:`telegram.MessageEntity`.
 
         Returns:
             Dict[:class:`telegram.MessageEntity`, :obj:`str`]: A dictionary of entities mapped to
             the text that belongs to them, calculated based on UTF-16 codepoints.
 
         """
-        if types is None:
-            types = MessageEntity.ALL_TYPES
-
-        return {
-            entity: self.parse_entity(entity) for entity in self.entities if entity.type in types
-        }
+        return parse_message_entities(self.text, self.entities, types=types)
 
     def parse_caption_entities(
         self, types: Optional[List[str]] = None
     ) -> Dict[MessageEntity, str]:
         """
         Returns a :obj:`dict` that maps :class:`telegram.MessageEntity` to :obj:`str`.
         It contains entities from this message's caption filtered by their
@@ -4265,22 +4281,15 @@
                 in :class:`telegram.MessageEntity`.
 
         Returns:
             Dict[:class:`telegram.MessageEntity`, :obj:`str`]: A dictionary of entities mapped to
             the text that belongs to them, calculated based on UTF-16 codepoints.
 
         """
-        if types is None:
-            types = MessageEntity.ALL_TYPES
-
-        return {
-            entity: self.parse_caption_entity(entity)
-            for entity in self.caption_entities
-            if entity.type in types
-        }
+        return parse_message_entities(self.caption, self.caption_entities, types=types)
 
     @classmethod
     def _parse_html(
         cls,
         message_text: Optional[str],
         entities: Dict[MessageEntity, str],
         urled: bool = False,
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_messageautodeletetimerchanged.py` & `python-telegram-bot-raw-21.2/telegram/_messageautodeletetimerchanged.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_messageentity.py` & `python-telegram-bot-raw-21.2/telegram/_messageentity.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_messageid.py` & `python-telegram-bot-raw-21.2/telegram/_messageid.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_messageorigin.py` & `python-telegram-bot-raw-21.2/telegram/_messageorigin.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_messagereactionupdated.py` & `python-telegram-bot-raw-21.2/telegram/_messagereactionupdated.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_passport/credentials.py` & `python-telegram-bot-raw-21.2/telegram/_passport/credentials.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_passport/data.py` & `python-telegram-bot-raw-21.2/telegram/_passport/data.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_passport/encryptedpassportelement.py` & `python-telegram-bot-raw-21.2/telegram/_passport/encryptedpassportelement.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,18 @@
         phone_number: Optional[str] = None,
         email: Optional[str] = None,
         files: Optional[Sequence[PassportFile]] = None,
         front_side: Optional[PassportFile] = None,
         reverse_side: Optional[PassportFile] = None,
         selfie: Optional[PassportFile] = None,
         translation: Optional[Sequence[PassportFile]] = None,
-        credentials: Optional["Credentials"] = None,  # pylint: disable=unused-argument
+        # TODO: Remove the credentials argument in 22.0 or later
+        credentials: Optional[  # pylint: disable=unused-argument  # noqa: ARG002
+            "Credentials"
+        ] = None,
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.type: str = type
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_passport/passportdata.py` & `python-telegram-bot-raw-21.2/telegram/_passport/passportdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_passport/passportelementerrors.py` & `python-telegram-bot-raw-21.2/telegram/_passport/passportelementerrors.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,17 +206,19 @@
     def file_hashes(self) -> List[str]:
         """List of base64-encoded file hashes.
 
         .. deprecated:: 20.6
             This attribute will return a tuple instead of a list in future major versions.
         """
         warn(
-            "The attribute `file_hashes` will return a tuple instead of a list in future major"
-            " versions.",
-            PTBDeprecationWarning,
+            PTBDeprecationWarning(
+                "20.6",
+                "The attribute `file_hashes` will return a tuple instead of a list in future major"
+                " versions.",
+            ),
             stacklevel=2,
         )
         return self._file_hashes
 
 
 class PassportElementErrorFrontSide(PassportElementError):
     """
@@ -423,18 +425,20 @@
     def file_hashes(self) -> List[str]:
         """List of base64-encoded file hashes.
 
         .. deprecated:: 20.6
             This attribute will return a tuple instead of a list in future major versions.
         """
         warn(
-            "The attribute `file_hashes` will return a tuple instead of a list in future major"
-            " versions. See the stability policy:"
-            " https://docs.python-telegram-bot.org/en/stable/stability_policy.html",
-            PTBDeprecationWarning,
+            PTBDeprecationWarning(
+                "20.6",
+                "The attribute `file_hashes` will return a tuple instead of a list in future major"
+                " versions. See the stability policy:"
+                " https://docs.python-telegram-bot.org/en/stable/stability_policy.html",
+            ),
             stacklevel=2,
         )
         return self._file_hashes
 
 
 class PassportElementErrorUnspecified(PassportElementError):
     """
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_passport/passportfile.py` & `python-telegram-bot-raw-21.2/telegram/_passport/passportfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,19 @@
     def file_date(self) -> int:
         """:obj:`int`: Unix time when the file was uploaded.
 
         .. deprecated:: 20.6
             This attribute will return a datetime instead of a integer in future major versions.
         """
         warn(
-            "The attribute `file_date` will return a datetime instead of an integer in future"
-            " major versions.",
-            PTBDeprecationWarning,
+            PTBDeprecationWarning(
+                "20.6",
+                "The attribute `file_date` will return a datetime instead of an integer in future"
+                " major versions.",
+            ),
             stacklevel=2,
         )
         return self._file_date
 
     @classmethod
     def de_json_decrypted(
         cls, data: Optional[JSONDict], bot: "Bot", credentials: "FileCredentials"
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_payment/invoice.py` & `python-telegram-bot-raw-21.2/telegram/_payment/invoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_payment/labeledprice.py` & `python-telegram-bot-raw-21.2/telegram/_payment/labeledprice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_payment/orderinfo.py` & `python-telegram-bot-raw-21.2/telegram/_payment/orderinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_payment/precheckoutquery.py` & `python-telegram-bot-raw-21.2/telegram/_payment/precheckoutquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_payment/shippingaddress.py` & `python-telegram-bot-raw-21.2/telegram/_payment/shippingaddress.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_payment/shippingoption.py` & `python-telegram-bot-raw-21.2/telegram/_payment/shippingoption.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_payment/shippingquery.py` & `python-telegram-bot-raw-21.2/telegram/_payment/shippingquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_payment/successfulpayment.py` & `python-telegram-bot-raw-21.2/telegram/_payment/successfulpayment.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_proximityalerttriggered.py` & `python-telegram-bot-raw-21.2/telegram/_proximityalerttriggered.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_reaction.py` & `python-telegram-bot-raw-21.2/telegram/_reaction.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_reply.py` & `python-telegram-bot-raw-21.2/telegram/_reply.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,15 @@
     .. versionadded:: 20.8
 
     Args:
         message_id (:obj:`int`): Identifier of the message that will be replied to in the current
             chat, or in the chat :paramref:`chat_id` if it is specified.
         chat_id (:obj:`int` | :obj:`str`, optional): If the message to be replied to is from a
             different chat, |chat_id_channel|
+            Not supported for messages sent on behalf of a business account.
         allow_sending_without_reply (:obj:`bool`, optional): |allow_sending_without_reply| Can be
             used only for replies in the same chat and forum topic.
         quote (:obj:`str`, optional): Quoted part of the message to be replied to; 0-1024
             characters after entities parsing. The quote must be an exact substring of the message
             to be replied to, including bold, italic, underline, strikethrough, spoiler, and
             custom_emoji entities. The message will fail to send if the quote isn't found in the
             original message.
@@ -372,14 +373,15 @@
             UTF-16 code units.
 
     Attributes:
         message_id (:obj:`int`): Identifier of the message that will be replied to in the current
             chat, or in the chat :paramref:`chat_id` if it is specified.
         chat_id (:obj:`int` | :obj:`str`): Optional. If the message to be replied to is from a
             different chat, |chat_id_channel|
+            Not supported for messages sent on behalf of a business account.
         allow_sending_without_reply (:obj:`bool`): Optional. |allow_sending_without_reply| Can be
             used only for replies in the same chat and forum topic.
         quote (:obj:`str`): Optional. Quoted part of the message to be replied to; 0-1024
             characters after entities parsing. The quote must be an exact substring of the message
             to be replied to, including bold, italic, underline, strikethrough, spoiler, and
             custom_emoji entities. The message will fail to send if the quote isn't found in the
             original message.
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_replykeyboardmarkup.py` & `python-telegram-bot-raw-21.2/telegram/_replykeyboardmarkup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 from telegram._keyboardbutton import KeyboardButton
 from telegram._telegramobject import TelegramObject
 from telegram._utils.markup import check_keyboard_type
 from telegram._utils.types import JSONDict
 
 
 class ReplyKeyboardMarkup(TelegramObject):
-    """This object represents a custom keyboard with reply options.
+    """This object represents a custom keyboard with reply options. Not supported in channels and
+    for messages sent on behalf of a Telegram Business account.
 
     Objects of this class are comparable in terms of equality. Two objects of this class are
     considered equal, if their size of :attr:`keyboard` and all the buttons are equal.
 
     .. figure:: https://core.telegram.org/file/464001950/1191a/2RwpmgU-swU.123554/b5\
         0478c124d5914c23
         :align: center
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_replykeyboardremove.py` & `python-telegram-bot-raw-21.2/telegram/_replykeyboardremove.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 class ReplyKeyboardRemove(TelegramObject):
     """
     Upon receiving a message with this object, Telegram clients will remove the current custom
     keyboard and display the default letter-keyboard. By default, custom keyboards are displayed
     until a new keyboard is sent by a bot. An exception is made for one-time keyboards that are
     hidden immediately after the user presses a button (see :class:`telegram.ReplyKeyboardMarkup`).
+    Not supported in channels and for messages sent on behalf of a Telegram Business account.
 
     Note:
         User will not be able to summon this keyboard; if you want to hide the keyboard from
         sight but keep it accessible, use :attr:`telegram.ReplyKeyboardMarkup.one_time_keyboard`.
 
     Examples:
         * Example usage: A user votes in a poll, bot returns confirmation message in reply to
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_sentwebappmessage.py` & `python-telegram-bot-raw-21.2/telegram/_sentwebappmessage.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_shared.py` & `python-telegram-bot-raw-21.2/telegram/_shared.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,20 +19,14 @@
 """This module contains two objects used for request chats/users service messages."""
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._files.photosize import PhotoSize
 from telegram._telegramobject import TelegramObject
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.types import JSONDict
-from telegram._utils.warnings import warn
-from telegram._utils.warnings_transition import (
-    build_deprecation_warning_message,
-    warn_about_deprecated_attr_in_property,
-)
-from telegram.warnings import PTBDeprecationWarning
 
 if TYPE_CHECKING:
     from telegram._bot import Bot
 
 
 class UsersShared(TelegramObject):
     """
@@ -40,78 +34,54 @@
     using a :class:`telegram.KeyboardButtonRequestUsers` button.
 
     Objects of this class are comparable in terms of equality. Two objects of this class are
     considered equal, if their :attr:`request_id` and :attr:`users` are equal.
 
     .. versionadded:: 20.8
        Bot API 7.0 replaces ``UserShared`` with this class. The only difference is that now
-       the :attr:`user_ids` is a sequence instead of a single integer.
+       the ``user_ids`` is a sequence instead of a single integer.
 
     .. versionchanged:: 21.1
        The argument :attr:`users` is now considered for the equality comparison instead of
-       :attr:`user_ids`.
+       ``user_ids``.
+
+    .. versionremoved:: 21.2
+       Removed the deprecated argument and attribute ``user_ids``.
 
     Args:
         request_id (:obj:`int`): Identifier of the request.
         users (Sequence[:class:`telegram.SharedUser`]): Information about users shared with the
             bot.
 
             .. versionadded:: 21.1
 
-            .. deprecated:: 21.1
-                In future versions, this argument will become keyword only.
-        user_ids (Sequence[:obj:`int`], optional): Identifiers of the shared users. These numbers
-            may have more than 32 significant bits and some programming languages may have
-            difficulty/silent defects in interpreting them. But they have at most 52 significant
-            bits, so 64-bit integers or double-precision float types are safe for storing these
-            identifiers. The bot may not have access to the users and could be unable to use
-            these identifiers, unless the users are already known to the bot by some other means.
-
-            .. deprecated:: 21.1
-               Bot API 7.2 introduced by :paramref:`users`, replacing this argument. Hence, this
-               argument is now optional and will be removed in future versions.
+            .. versionchanged:: 21.2
+               This argument is now required.
 
     Attributes:
         request_id (:obj:`int`): Identifier of the request.
         users (Tuple[:class:`telegram.SharedUser`]): Information about users shared with the
             bot.
 
             .. versionadded:: 21.1
     """
 
     __slots__ = ("request_id", "users")
 
     def __init__(
         self,
         request_id: int,
-        user_ids: Optional[Sequence[int]] = None,
-        users: Optional[Sequence["SharedUser"]] = None,
+        users: Sequence["SharedUser"],
         *,
         api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.request_id: int = request_id
-
-        if users is None:
-            raise TypeError("`users` is a required argument since Bot API 7.2")
-
         self.users: Tuple[SharedUser, ...] = parse_sequence_arg(users)
 
-        if user_ids is not None:
-            warn(
-                build_deprecation_warning_message(
-                    deprecated_name="user_ids",
-                    new_name="users",
-                    object_type="parameter",
-                    bot_api_version="7.2",
-                ),
-                PTBDeprecationWarning,
-                stacklevel=2,
-            )
-
         self._id_attrs = (self.request_id, self.users)
 
         self._freeze()
 
     @classmethod
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["UsersShared"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
@@ -126,36 +96,14 @@
         # This is a deprecated field that TG still returns for backwards compatibility
         # Let's filter it out to speed up the de-json process
         if user_ids := data.get("user_ids"):
             api_kwargs = {"user_ids": user_ids}
 
         return super()._de_json(data=data, bot=bot, api_kwargs=api_kwargs)
 
-    @property
-    def user_ids(self) -> Tuple[int, ...]:
-        """
-        Tuple[:obj:`int`]: Identifiers of the shared users. These numbers may have
-        more than 32 significant bits and some programming languages may have difficulty/silent
-        defects in interpreting them. But they have at most 52 significant bits, so 64-bit
-        integers or double-precision float types are safe for storing these identifiers. The
-        bot may not have access to the users and could be unable to use these identifiers,
-        unless the users are already known to the bot by some other means.
-
-        .. deprecated:: 21.1
-            As Bot API 7.2 replaces this attribute with :attr:`users`, this attribute will be
-            removed in future versions.
-        """
-        warn_about_deprecated_attr_in_property(
-            deprecated_attr_name="user_ids",
-            new_attr_name="users",
-            bot_api_version="7.2",
-            stacklevel=2,
-        )
-        return tuple(user.user_id for user in self.users)
-
 
 class ChatShared(TelegramObject):
     """
     This object contains information about the chat whose identifier was shared with the bot
     using a :class:`telegram.KeyboardButtonRequestChat` button.
 
     Objects of this class are comparable in terms of equality. Two objects of this class are
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_story.py` & `python-telegram-bot-raw-21.2/telegram/_story.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_switchinlinequerychosenchat.py` & `python-telegram-bot-raw-21.2/telegram/_switchinlinequerychosenchat.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_telegramobject.py` & `python-telegram-bot-raw-21.2/telegram/_telegramobject.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_update.py` & `python-telegram-bot-raw-21.2/telegram/_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,16 +137,16 @@
 
         business_connection (:class:`telegram.BusinessConnection`, optional): The bot was connected
             to or disconnected from a business account, or a user edited an existing connection
             with the bot.
 
             .. versionadded:: 21.1
 
-        business_message (:class:`telegram.Message`, optional): New non-service message
-            from a connected business account.
+        business_message (:class:`telegram.Message`, optional): New message from a connected
+            business account.
 
             .. versionadded:: 21.1
 
         edited_business_message (:class:`telegram.Message`, optional): New version of a message
             from a connected business account.
 
             .. versionadded:: 21.1
@@ -245,16 +245,16 @@
 
         business_connection (:class:`telegram.BusinessConnection`): Optional. The bot was connected
             to or disconnected from a business account, or a user edited an existing connection
             with the bot.
 
             .. versionadded:: 21.1
 
-        business_message (:class:`telegram.Message`): Optional. New non-service message
-            from a connected business account.
+        business_message (:class:`telegram.Message`): Optional. New message from a connected
+            business account.
 
             .. versionadded:: 21.1
 
         edited_business_message (:class:`telegram.Message`): Optional. New version of a message
             from a connected business account.
 
             .. versionadded:: 21.1
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_user.py` & `python-telegram-bot-raw-21.2/telegram/_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         Contact,
         Document,
         InlineKeyboardMarkup,
         InputMediaAudio,
         InputMediaDocument,
         InputMediaPhoto,
         InputMediaVideo,
+        InputPollOption,
         LabeledPrice,
         LinkPreviewOptions,
         Location,
         Message,
         MessageEntity,
         MessageId,
         PhotoSize,
@@ -1478,15 +1479,15 @@
             message_thread_id=message_thread_id,
             business_connection_id=business_connection_id,
         )
 
     async def send_poll(
         self,
         question: str,
-        options: Sequence[str],
+        options: Sequence[Union[str, "InputPollOption"]],
         is_anonymous: Optional[bool] = None,
         type: Optional[str] = None,
         allows_multiple_answers: Optional[bool] = None,
         correct_option_id: Optional[CorrectOptionID] = None,
         is_closed: Optional[bool] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
@@ -1495,14 +1496,16 @@
         open_period: Optional[int] = None,
         close_date: Optional[Union[int, datetime]] = None,
         explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
         message_thread_id: Optional[int] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         business_connection_id: Optional[str] = None,
+        question_parse_mode: ODVInput[str] = DEFAULT_NONE,
+        question_entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1544,14 +1547,16 @@
             close_date=close_date,
             api_kwargs=api_kwargs,
             allow_sending_without_reply=allow_sending_without_reply,
             explanation_entities=explanation_entities,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             business_connection_id=business_connection_id,
+            question_parse_mode=question_parse_mode,
+            question_entities=question_entities,
         )
 
     async def send_copy(
         self,
         from_chat_id: Union[str, int],
         message_id: int,
         caption: Optional[str] = None,
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_userprofilephotos.py` & `python-telegram-bot-raw-21.2/telegram/_userprofilephotos.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/argumentparsing.py` & `python-telegram-bot-raw-21.2/telegram/_utils/argumentparsing.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/datetime.py` & `python-telegram-bot-raw-21.2/telegram/_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/defaultvalue.py` & `python-telegram-bot-raw-21.2/telegram/_utils/defaultvalue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/enum.py` & `python-telegram-bot-raw-21.2/telegram/_utils/enum.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         return f"<{self.__class__.__name__}.{self.name}>"
 
     def __str__(self) -> str:
         return str.__str__(self)
 
 
 # Apply the __repr__ modification and __str__ fix to IntEnum
-class IntEnum(_enum.IntEnum):
+class IntEnum(_enum.IntEnum):  # pylint: disable=invalid-slots
     """Helper class for int enums where ``str(member)`` prints the value, but ``repr(member)``
     gives ``EnumName.MEMBER_NAME``.
     """
 
     __slots__ = ()
 
     def __repr__(self) -> str:
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/files.py` & `python-telegram-bot-raw-21.2/telegram/_utils/files.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/logging.py` & `python-telegram-bot-raw-21.2/telegram/_utils/logging.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/markup.py` & `python-telegram-bot-raw-21.2/telegram/_utils/markup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/repr.py` & `python-telegram-bot-raw-21.2/telegram/_utils/repr.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/strings.py` & `python-telegram-bot-raw-21.2/telegram/_utils/strings.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/types.py` & `python-telegram-bot-raw-21.2/telegram/_utils/types.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/warnings.py` & `python-telegram-bot-raw-21.2/telegram/_utils/warnings.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,26 +22,35 @@
 
 Warning:
     Contents of this module are intended to be used internally by the library and *not* by the
     user. Changes to this module are not considered breaking changes and may not be documented in
     the changelog.
 """
 import warnings
-from typing import Type
+from typing import Type, Union
 
 from telegram.warnings import PTBUserWarning
 
 
-def warn(message: str, category: Type[Warning] = PTBUserWarning, stacklevel: int = 0) -> None:
+def warn(
+    message: Union[str, PTBUserWarning],
+    category: Type[Warning] = PTBUserWarning,
+    stacklevel: int = 0,
+) -> None:
     """
     Helper function used as a shortcut for warning with default values.
 
     .. versionadded:: 20.0
 
     Args:
-        message (:obj:`str`): Specify the warnings message to pass to ``warnings.warn()``.
+        message (:obj:`str` | :obj:`PTBUserWarning`): Specify the warnings message to pass to
+            ``warnings.warn()``.
+
+            .. versionchanged:: 21.2
+                Now also accepts a :obj:`PTBUserWarning` instance.
+
         category (:obj:`Type[Warning]`, optional): Specify the Warning class to pass to
             ``warnings.warn()``. Defaults to :class:`telegram.warnings.PTBUserWarning`.
         stacklevel (:obj:`int`, optional): Specify the stacklevel to pass to ``warnings.warn()``.
             Pass the same value as you'd pass directly to ``warnings.warn()``. Defaults to ``0``.
     """
     warnings.warn(message, category=category, stacklevel=stacklevel + 1)
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_utils/warnings_transition.py` & `python-telegram-bot-raw-21.2/telegram/_utils/warnings_transition.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 """This module contains functionality used for transition warnings issued by this library.
 
 It was created to prevent circular imports that would be caused by creating the warnings
 inside warnings.py.
 
 .. versionadded:: 20.2
 """
-from typing import Any, Callable, Type
+from typing import Any, Callable, Type, Union
 
 from telegram._utils.warnings import warn
-from telegram.warnings import PTBDeprecationWarning
+from telegram.warnings import PTBDeprecationWarning, PTBUserWarning
 
 
 def build_deprecation_warning_message(
     deprecated_name: str,
     new_name: str,
     object_type: str,
     bot_api_version: str,
@@ -50,16 +50,17 @@
 # We'll use `Any` here and put type hints in the calling code.
 def warn_about_deprecated_arg_return_new_arg(
     deprecated_arg: Any,
     new_arg: Any,
     deprecated_arg_name: str,
     new_arg_name: str,
     bot_api_version: str,
+    ptb_version: str,
     stacklevel: int = 2,
-    warn_callback: Callable[[str, Type[Warning], int], None] = warn,
+    warn_callback: Callable[[Union[str, PTBUserWarning], Type[Warning], int], None] = warn,
 ) -> Any:
     """A helper function for the transition in API when argument is renamed.
 
     Checks the `deprecated_arg` and `new_arg` objects; warns if non-None `deprecated_arg` object
     was passed. Returns `new_arg` object (either the one originally passed by the user or the one
     that user passed as `deprecated_arg`).
 
@@ -76,33 +77,38 @@
         raise ValueError(
             f"You passed different entities as '{deprecated_arg_name}' and '{new_arg_name}'. "
             f"{base_message}"
         )
 
     if deprecated_arg:
         warn_callback(
-            f"Bot API {bot_api_version} renamed the argument '{deprecated_arg_name}' to "
-            f"'{new_arg_name}'.",
-            PTBDeprecationWarning,
-            stacklevel + 1,
+            PTBDeprecationWarning(
+                ptb_version,
+                f"Bot API {bot_api_version} renamed the argument '{deprecated_arg_name}' to "
+                f"'{new_arg_name}'.",
+            ),
+            stacklevel=stacklevel + 1,  # type: ignore[call-arg]
         )
         return deprecated_arg
 
     return new_arg
 
 
 def warn_about_deprecated_attr_in_property(
     deprecated_attr_name: str,
     new_attr_name: str,
     bot_api_version: str,
+    ptb_version: str,
     stacklevel: int = 2,
 ) -> None:
     """A helper function for the transition in API when attribute is renamed. Call from properties.
 
     The properties replace deprecated attributes in classes and issue these deprecation warnings.
     """
     warn(
-        f"Bot API {bot_api_version} renamed the attribute '{deprecated_attr_name}' to "
-        f"'{new_attr_name}'.",
-        PTBDeprecationWarning,
+        PTBDeprecationWarning(
+            ptb_version,
+            f"Bot API {bot_api_version} renamed the attribute '{deprecated_attr_name}' to "
+            f"'{new_attr_name}'.",
+        ),
         stacklevel=stacklevel + 1,
     )
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_version.py` & `python-telegram-bot-raw-21.2/telegram/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         if self.releaselevel != "final":
             version = f"{version}{self._rl_shorthand()}{self.serial}"
 
         return version
 
 
 __version_info__: Final[Version] = Version(
-    major=21, minor=1, micro=1, releaselevel="final", serial=0
+    major=21, minor=2, micro=0, releaselevel="final", serial=0
 )
 __version__: Final[str] = str(__version_info__)
 
 # # SETUP.PY MARKER
 # Lines above this line will be `exec`-cuted in setup.py. Make sure that this only contains
 # std-lib imports!
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_videochat.py` & `python-telegram-bot-raw-21.2/telegram/_videochat.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_webappdata.py` & `python-telegram-bot-raw-21.2/telegram/_webappdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_webappinfo.py` & `python-telegram-bot-raw-21.2/telegram/_webappinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_webhookinfo.py` & `python-telegram-bot-raw-21.2/telegram/_webhookinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/_writeaccessallowed.py` & `python-telegram-bot-raw-21.2/telegram/_writeaccessallowed.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/constants.py` & `python-telegram-bot-raw-21.2/telegram/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,26 @@
 those classes.
 
 .. versionchanged:: 20.0
 
     * Most of the constants in this module are grouped into enums.
 """
 # TODO: Remove this when https://github.com/PyCQA/pylint/issues/6887 is resolved.
-# pylint: disable=invalid-enum-extension
+# pylint: disable=invalid-enum-extension,invalid-slots
 
 __all__ = [
     "BOT_API_VERSION",
     "BOT_API_VERSION_INFO",
     "SUPPORTED_WEBHOOK_PORTS",
     "ZERO_DATE",
     "AccentColor",
+    "BackgroundFillLimit",
+    "BackgroundFillType",
+    "BackgroundTypeLimit",
+    "BackgroundTypeType",
     "BotCommandLimit",
     "BotCommandScopeType",
     "BotDescriptionLimit",
     "BotNameLimit",
     "BulkRequestLimit",
     "CallbackQueryLimit",
     "ChatAction",
@@ -138,15 +142,15 @@
 #: :class:`typing.NamedTuple`: A tuple containing the two components of the version number:
 # ``major`` and ``minor``. Both values are integers.
 #: The components can also be accessed by name, so ``BOT_API_VERSION_INFO[0]`` is equivalent
 #: to ``BOT_API_VERSION_INFO.major`` and so on. Also available as
 #: :data:`telegram.__bot_api_version_info__`.
 #:
 #: .. versionadded:: 20.0
-BOT_API_VERSION_INFO: Final[_BotAPIVersion] = _BotAPIVersion(major=7, minor=2)
+BOT_API_VERSION_INFO: Final[_BotAPIVersion] = _BotAPIVersion(major=7, minor=3)
 #: :obj:`str`: Telegram Bot API
 #: version supported by this version of `python-telegram-bot`. Also available as
 #: :data:`telegram.__bot_api_version__`.
 #:
 #: .. versionadded:: 13.4
 BOT_API_VERSION: Final[str] = str(BOT_API_VERSION_INFO)
 
@@ -818,14 +822,54 @@
     MAX_CHAT_TITLE_LENGTH = 128
     """:obj:`int`: Maximum length of a :obj:`str` passed as the
     :paramref:`~telegram.Bot.set_chat_title.title` parameter of
     :meth:`telegram.Bot.set_chat_title`.
     """
 
 
+class BackgroundTypeLimit(IntEnum):
+    """This enum contains limitations for :class:`telegram.BackgroundTypeFill`,
+    :class:`telegram.BackgroundTypeWallpaper` and :class:`telegram.BackgroundTypePattern`.
+    The enum members of this enumeration are instances of :class:`int` and can be treated as such.
+
+    .. versionadded:: 21.2
+    """
+
+    __slots__ = ()
+
+    MAX_DIMMING = 100
+    """:obj:`int`: Maximum value allowed for:
+
+    * :paramref:`~telegram.BackgroundTypeFill.dark_theme_dimming` parameter of
+        :class:`telegram.BackgroundTypeFill`
+    * :paramref:`~telegram.BackgroundTypeWallpaper.dark_theme_dimming` parameter of
+        :class:`telegram.BackgroundTypeWallpaper`
+    """
+    MAX_INTENSITY = 100
+    """:obj:`int`: Maximum value allowed for :paramref:`~telegram.BackgroundTypePattern.intensity`
+    parameter of :class:`telegram.BackgroundTypePattern`
+    """
+
+
+class BackgroundFillLimit(IntEnum):
+    """This enum contains limitations for :class:`telegram.BackgroundFillGradient`.
+    The enum members of this enumeration are instances of :class:`int` and can be treated as such.
+
+    .. versionadded:: 21.2
+    """
+
+    __slots__ = ()
+
+    MAX_ROTATION_ANGLE = 359
+    """:obj:`int`: Maximum value allowed for:
+        :paramref:`~telegram.BackgroundFillGradient.rotation_angle` parameter of
+        :class:`telegram.BackgroundFillGradient`
+    """
+
+
 class ChatMemberStatus(StringEnum):
     """This enum contains the available states for :class:`telegram.ChatMember`. The enum
     members of this enumeration are instances of :class:`str` and can be treated as such.
 
     .. versionadded:: 20.0
     """
 
@@ -1423,14 +1467,29 @@
       :class:`telegram.InputLocationMessageContent`
     * :paramref:`~telegram.Bot.edit_message_live_location.live_period` parameter of
       :meth:`telegram.Bot.edit_message_live_location`
     * :paramref:`~telegram.Bot.send_location.live_period` parameter of
       :meth:`telegram.Bot.send_location`
     """
 
+    LIVE_PERIOD_FOREVER = int(hex(0x7FFFFFFF), 16)
+    """:obj:`int`: Value for live locations that can be edited indefinitely. Passed in:
+
+    * :paramref:`~telegram.InlineQueryResultLocation.live_period` parameter of
+      :class:`telegram.InlineQueryResultLocation`
+    * :paramref:`~telegram.InputLocationMessageContent.live_period` parameter of
+      :class:`telegram.InputLocationMessageContent`
+    * :paramref:`~telegram.Bot.edit_message_live_location.live_period` parameter of
+      :meth:`telegram.Bot.edit_message_live_location`
+    * :paramref:`~telegram.Bot.send_location.live_period` parameter of
+      :meth:`telegram.Bot.send_location`
+
+    .. versionadded:: 21.2
+    """
+
     MIN_PROXIMITY_ALERT_RADIUS = 1
     """:obj:`int`: Minimum value allowed for:
 
     * :paramref:`~telegram.InlineQueryResultLocation.proximity_alert_radius` parameter of
       :class:`telegram.InlineQueryResultLocation`
     * :paramref:`~telegram.InputLocationMessageContent.proximity_alert_radius` parameter of
       :class:`telegram.InputLocationMessageContent`
@@ -1722,14 +1781,19 @@
     CHANNEL_CHAT_CREATED = "channel_chat_created"
     """:obj:`str`: Messages with :attr:`telegram.Message.channel_chat_created`."""
     CHAT_SHARED = "chat_shared"
     """:obj:`str`: Messages with :attr:`telegram.Message.chat_shared`.
 
     .. versionadded:: 20.8
     """
+    CHAT_BACKGROUND_SET = "chat_background_set"
+    """:obj:`str`: Messages with :attr:`telegram.Message.chat_background_set`.
+
+    .. versionadded:: 21.2
+    """
     CONNECTED_WEBSITE = "connected_website"
     """:obj:`str`: Messages with :attr:`telegram.Message.connected_website`."""
     CONTACT = "contact"
     """:obj:`str`: Messages with :attr:`telegram.Message.contact`."""
     DELETE_CHAT_PHOTO = "delete_chat_photo"
     """:obj:`str`: Messages with :attr:`telegram.Message.delete_chat_photo`."""
     DICE = "dice"
@@ -2874,7 +2938,43 @@
     """:obj:`str`: Man Shrugging"""
     SHRUG = "🤷"
     """:obj:`str`: Shrug"""
     WOMAN_SHRUGGING = "🤷‍♀️"
     """:obj:`str`: Woman Shrugging"""
     POUTING_FACE = "😡"
     """:obj:`str`: Pouting face"""
+
+
+class BackgroundTypeType(StringEnum):
+    """This enum contains the available types of :class:`telegram.BackgroundType`. The enum
+    members of this enumeration are instances of :class:`str` and can be treated as such.
+
+    .. versionadded:: 21.2
+    """
+
+    __slots__ = ()
+
+    FILL = "fill"
+    """:obj:`str`: A :class:`telegram.BackgroundType` with fill background."""
+    WALLPAPER = "wallpaper"
+    """:obj:`str`: A :class:`telegram.BackgroundType` with wallpaper background."""
+    PATTERN = "pattern"
+    """:obj:`str`: A :class:`telegram.BackgroundType` with pattern background."""
+    CHAT_THEME = "chat_theme"
+    """:obj:`str`: A :class:`telegram.BackgroundType` with chat_theme background."""
+
+
+class BackgroundFillType(StringEnum):
+    """This enum contains the available types of :class:`telegram.BackgroundFill`. The enum
+    members of this enumeration are instances of :class:`str` and can be treated as such.
+
+    .. versionadded:: 21.2
+    """
+
+    __slots__ = ()
+
+    SOLID = "solid"
+    """:obj:`str`: A :class:`telegram.BackgroundFill` with solid fill."""
+    GRADIENT = "gradient"
+    """:obj:`str`: A :class:`telegram.BackgroundFill` with gradient fill."""
+    FREEFORM_GRADIENT = "freeform_gradient"
+    """:obj:`str`: A :class:`telegram.BackgroundFill` with freeform_gradient fill."""
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/error.py` & `python-telegram-bot-raw-21.2/telegram/error.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/helpers.py` & `python-telegram-bot-raw-21.2/telegram/helpers.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/request/__init__.py` & `python-telegram-bot-raw-21.2/telegram/request/__init__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/request/_baserequest.py` & `python-telegram-bot-raw-21.2/telegram/request/_baserequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,18 +314,20 @@
         has_files = request_data and request_data.multipart_data
         if (
             has_files
             and not isinstance(self, HTTPXRequest)
             and isinstance(write_timeout, DefaultValue)
         ):
             warn(
-                f"The `write_timeout` parameter passed to {self.__class__.__name__}.do_request "
-                "will default to `BaseRequest.DEFAULT_NONE` instead of 20 in future versions "
-                "for *all* methods of the `Bot` class, including methods sending media.",
-                PTBDeprecationWarning,
+                PTBDeprecationWarning(
+                    "20.7",
+                    f"The `write_timeout` parameter passed to {self.__class__.__name__}.do_request"
+                    " will default to `BaseRequest.DEFAULT_NONE` instead of 20 in future versions "
+                    "for *all* methods of the `Bot` class, including methods sending media.",
+                ),
                 stacklevel=3,
             )
             write_timeout = 20
 
         try:
             code, payload = await self.do_request(
                 url=url,
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/request/_httpxrequest.py` & `python-telegram-bot-raw-21.2/telegram/request/_httpxrequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,17 +142,17 @@
     ):
         if proxy_url is not None and proxy is not None:
             raise ValueError("The parameters `proxy_url` and `proxy` are mutually exclusive.")
 
         if proxy_url is not None:
             proxy = proxy_url
             warn(
-                "The parameter `proxy_url` is deprecated since version 20.7. Use `proxy` "
-                "instead.",
-                PTBDeprecationWarning,
+                PTBDeprecationWarning(
+                    "20.7", "The parameter `proxy_url` is deprecated. Use `proxy` instead."
+                ),
                 stacklevel=2,
             )
 
         self._http_version = http_version
         self._media_write_timeout = media_write_timeout
         timeout = httpx.Timeout(
             connect=connect_timeout,
```

### Comparing `python-telegram-bot-raw-21.1.1/telegram/request/_requestdata.py` & `python-telegram-bot-raw-21.2/telegram/request/_requestdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/request/_requestparameter.py` & `python-telegram-bot-raw-21.2/telegram/request/_requestparameter.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1.1/telegram/warnings.py` & `python-telegram-bot-raw-21.2/telegram/warnings.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,10 +50,38 @@
 # warnings
 class PTBDeprecationWarning(PTBUserWarning, DeprecationWarning):
     """
     Custom warning class for deprecations in this library.
 
     .. versionchanged:: 20.0
        Renamed TelegramDeprecationWarning to PTBDeprecationWarning.
+
+    Args:
+        version (:obj:`str`): The version in which the feature was deprecated.
+
+            .. versionadded:: 21.2
+        message (:obj:`str`): The message to display.
+
+            .. versionadded:: 21.2
+
+    Attributes:
+        version (:obj:`str`): The version in which the feature was deprecated.
+
+            .. versionadded:: 21.2
+        message (:obj:`str`): The message to display.
+
+            .. versionadded:: 21.2
     """
 
-    __slots__ = ()
+    __slots__ = ("message", "version")
+
+    def __init__(self, version: str, message: str) -> None:
+        self.version: str = version
+        self.message: str = message
+
+    def __str__(self) -> str:
+        """Returns a string representation of the warning, using :attr:`message` and
+        :attr:`version`.
+
+        .. versionadded:: 21.2
+        """
+        return f"Deprecated since version {self.version}: {self.message}"
```

