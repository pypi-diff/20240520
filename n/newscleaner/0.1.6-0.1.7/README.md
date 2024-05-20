# Comparing `tmp/newscleaner-0.1.6.tar.gz` & `tmp/newscleaner-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newscleaner-0.1.6.tar", last modified: Mon Apr  1 10:44:33 2024, max compression
+gzip compressed data, was "newscleaner-0.1.7.tar", last modified: Mon May 20 07:37:23 2024, max compression
```

## Comparing `newscleaner-0.1.6.tar` & `newscleaner-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 10:44:33.874589 newscleaner-0.1.6/
--rw-rw-rw-   0        0        0     1073 2023-05-10 10:09:49.000000 newscleaner-0.1.6/LICENCE.txt
--rw-rw-rw-   0        0        0       34 2023-05-10 10:10:08.000000 newscleaner-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2024-04-01 10:44:33.873571 newscleaner-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-05-29 11:40:52.000000 newscleaner-0.1.6/README.md
--rw-rw-rw-   0        0        0       84 2023-05-10 10:10:18.000000 newscleaner-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 10:44:33.874589 newscleaner-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      882 2024-04-01 10:41:36.000000 newscleaner-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 10:44:33.863584 newscleaner-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 10:44:33.869574 newscleaner-0.1.6/src/newscleaner/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:44.000000 newscleaner-0.1.6/src/newscleaner/__init__.py
--rw-rw-rw-   0        0        0   110920 2024-04-01 10:30:06.000000 newscleaner-0.1.6/src/newscleaner/cleaner.py
--rw-rw-rw-   0        0        0      885 2024-04-01 10:42:20.000000 newscleaner-0.1.6/src/newscleaner/setup.py
--rw-rw-rw-   0        0        0      841 2023-12-05 12:10:24.000000 newscleaner-0.1.6/src/newscleaner/strip_clean.py
-drwxrwxrwx   0        0        0        0 2024-04-01 10:44:33.873571 newscleaner-0.1.6/src/newscleaner.egg-info/
--rw-rw-rw-   0        0        0      559 2024-04-01 10:44:33.000000 newscleaner-0.1.6/src/newscleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-05-10 10:01:43.000000 newscleaner-0.1.6/src/newscleaner.egg-info/PKG-INFO.txt
--rw-rw-rw-   0        0        0      362 2024-04-01 10:44:33.000000 newscleaner-0.1.6/src/newscleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 10:44:33.000000 newscleaner-0.1.6/src/newscleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 10:44:33.000000 newscleaner-0.1.6/src/newscleaner.egg-info/top_level.txt
+drwxr-xr-x   0 lakshita   (501) staff       (20)        0 2024-05-20 07:37:23.576016 newscleaner-0.1.7/
+-rw-rw-r--   0 lakshita   (501) staff       (20)     1073 2023-05-10 10:09:49.000000 newscleaner-0.1.7/LICENCE.txt
+-rw-rw-r--   0 lakshita   (501) staff       (20)       34 2023-05-10 10:10:08.000000 newscleaner-0.1.7/MANIFEST.in
+-rw-r--r--   0 lakshita   (501) staff       (20)      543 2024-05-20 07:37:23.575855 newscleaner-0.1.7/PKG-INFO
+-rw-rw-r--   0 lakshita   (501) staff       (20)       17 2023-05-29 11:40:52.000000 newscleaner-0.1.7/README.md
+-rw-rw-r--   0 lakshita   (501) staff       (20)       84 2023-05-10 10:10:18.000000 newscleaner-0.1.7/pyproject.toml
+-rw-r--r--   0 lakshita   (501) staff       (20)       38 2024-05-20 07:37:23.576058 newscleaner-0.1.7/setup.cfg
+-rw-rw-r--   0 lakshita   (501) staff       (20)      882 2024-05-20 07:37:02.000000 newscleaner-0.1.7/setup.py
+drwxr-xr-x   0 lakshita   (501) staff       (20)        0 2024-05-20 07:37:23.573480 newscleaner-0.1.7/src/
+drwxr-xr-x   0 lakshita   (501) staff       (20)        0 2024-05-20 07:37:23.574860 newscleaner-0.1.7/src/newscleaner/
+-rw-rw-r--   0 lakshita   (501) staff       (20)        0 2023-05-15 10:03:44.000000 newscleaner-0.1.7/src/newscleaner/__init__.py
+-rw-r--r--   0 lakshita   (501) staff       (20)   129803 2024-05-20 06:51:14.000000 newscleaner-0.1.7/src/newscleaner/cleaner.py
+-rw-rw-r--   0 lakshita   (501) staff       (20)      885 2024-05-20 07:37:12.000000 newscleaner-0.1.7/src/newscleaner/setup.py
+-rw-rw-r--   0 lakshita   (501) staff       (20)      841 2023-12-05 12:10:24.000000 newscleaner-0.1.7/src/newscleaner/strip_clean.py
+drwxr-xr-x   0 lakshita   (501) staff       (20)        0 2024-05-20 07:37:23.575718 newscleaner-0.1.7/src/newscleaner.egg-info/
+-rw-r--r--   0 lakshita   (501) staff       (20)      543 2024-05-20 07:37:23.000000 newscleaner-0.1.7/src/newscleaner.egg-info/PKG-INFO
+-rw-rw-r--   0 lakshita   (501) staff       (20)      547 2023-05-10 10:01:43.000000 newscleaner-0.1.7/src/newscleaner.egg-info/PKG-INFO.txt
+-rw-rw-r--   0 lakshita   (501) staff       (20)      362 2024-05-20 07:37:23.000000 newscleaner-0.1.7/src/newscleaner.egg-info/SOURCES.txt
+-rw-rw-r--   0 lakshita   (501) staff       (20)        1 2024-05-20 07:37:23.000000 newscleaner-0.1.7/src/newscleaner.egg-info/dependency_links.txt
+-rw-rw-r--   0 lakshita   (501) staff       (20)       12 2024-05-20 07:37:23.000000 newscleaner-0.1.7/src/newscleaner.egg-info/top_level.txt
```

### Comparing `newscleaner-0.1.6/LICENCE.txt` & `newscleaner-0.1.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `newscleaner-0.1.6/PKG-INFO` & `newscleaner-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: newscleaner
-Version: 0.1.6
-Summary: Package to clean up noise from news articles
-Home-page: https://github.com/pankajjha/newscleaner
-Author: Lakshita Kain
-Author-email: mail@pankajjha.me
-Project-URL: Bug Tracker, https://github.com/pankajjha/newscleaner/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
-# Article Cleaner
+Metadata-Version: 2.1
+Name: newscleaner
+Version: 0.1.7
+Summary: Package to clean up noise from news articles
+Home-page: https://github.com/pankajjha/newscleaner
+Author: Lakshita Kain
+Author-email: mail@pankajjha.me
+Project-URL: Bug Tracker, https://github.com/pankajjha/newscleaner/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
+# Article Cleaner
```

### Comparing `newscleaner-0.1.6/setup.py` & `newscleaner-0.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="newscleaner",
-    version="0.1.6",
+    version="0.1.7",
     author="Lakshita Kain",
     author_email="mail@pankajjha.me",
     description="Package to clean up noise from news articles",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pankajjha/newscleaner",
     project_urls={
```

### Comparing `newscleaner-0.1.6/src/newscleaner/cleaner.py` & `newscleaner-0.1.7/src/newscleaner/cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # coding: utf-8
-#cleaner function 0.1.6
+#cleaner function 0.1.7
 
 
 # importing all the important libraries
 import re
 import json
 import html
 import unicodedata
-import pkg_resources
+# import pkg_resources
 from ftfy import fix_text
 
 
 # In[4]:
 
 
 #  Cleaning raw HTML and retaining tags
@@ -910,16 +910,14 @@
     clean_text = re.sub(r'{p}The News{/p}','', clean_text, flags=re.DOTALL)
     clean_text = re.sub(r'{p} making a tax-deductible gift {/p}','', clean_text, flags=re.DOTALL)
     clean_text = re.sub(r'{p} making a tax-deductible gift today. {/p}','', clean_text, flags=re.DOTALL)
 
     # For click2houston (continue.....)
     clean_text = re.sub(r'} Recommended Videos{','}{', clean_text, flags=re.DOTALL)
 
-
-    ########################################################################################
     # For everythinglubbock.com (continues.....) 
     clean_text = re.sub(r"{p}Note: The video above reflects top headlines from the morning of (January|February|March|April|May|June|July|August|September|October|November|December) \d+, \d+.{/p}",'', clean_text, flags=re.DOTALL)
     clean_text = re.sub(r'{p}If you or someone you know would like to give to the Hill family during this time, click  here.  {/p}','', clean_text, flags=re.DOTALL)
 
     # For kcbd.com
     clean_text = re.sub(r'{i}{b}PREVIOUS COVERAGE: {/b}{/i}{i}{b}.*?{/b}{/i}', '', clean_text, flags=re.DOTALL)
     clean_text = re.sub(r'} Specific information about the closures can be received through LBKAlert. The public can sign up for LBKAlert at  www.lbkalert.com  and register for the &#8216;Road Closure&#8217; alerts.{', '}{', clean_text, flags=re.DOTALL)
@@ -1147,14 +1145,245 @@
     clean_text = re.sub(r'{p}{strong}MORE:.*?{/strong}{/p}','', clean_text, flags=re.DOTALL)
 
     # For cinemablend.com
     clean_text = re.sub('} Your Daily Blend of Entertainment News{','}{', clean_text, flags=re.DOTALL)
     clean_text = re.sub('Contact me with news and offers from other Future brands Receive email from us on behalf of our trusted partners or sponsors','', clean_text, flags=re.DOTALL)
 
 
+
+#####################################################
+
+
+    # For kfyo.com
+    clean_text = re.sub(r'} More From News/Talk 95.1 &amp; 790 KFYO{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}READ MORE:  .*?{','}{', clean_text, flags=re.DOTALL)
+
+    # For kgns.tv
+    clean_text = re.sub(r'} For more headlines. click  here .{','}{', clean_text, flags=re.DOTALL)
+
+    # For travelandleisure.com
+    clean_text = re.sub(r"}\n \n \nLove a great deal\?  \+L Recommends newsletter  and we'll send you our favorite travel products each week.\n{",'}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Was this page helpful\?\n  \n  \n\n \n\nTell us why!','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'\nRelated Articles\n','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n \n{strong}Related:{/strong}  .*?\n{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n \n{strong} Related:{/strong}  .*?\n{','}{', clean_text, flags=re.DOTALL)
+
+    # For helenair.com
+    clean_text = re.sub(r'}\n\s*\d+{/p}\n\s*\n\s*Funny{/p}\n\s*\n\s*\n\s*{/p}\n\s*\d+{/p}\n\s*\n\s*Wow{/p}\n\s*\n\s*\n\s*{/p}\n\s*\d+{/p}\n\s*\n\s*Sad{/p}\n\s*\n \s*\n\s*{/p}\n\s*\d+{/p}\n\s*\n\s*Angry{/p}\n\s*\n\s*\n\s*{/p}\n\s*\d+{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Follow him on Twitter','', clean_text, flags=re.DOTALL)
+
+
+    # For wtaj.com
+    clean_text = re.sub(r'}Get daily updates on local news, weather and sports by signing up for the  WTAJ Newslette  r {','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Stay up to date with news that matters to you with the WTAJ app on iPhone and Android by&#160; clicking here .{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Download our WTAJ Your Weather Authority app on your&#160; Apple &#160;or&#160; Android &#160;phone to stay up to date with your local weather.{/strong}{/p}','', clean_text, flags=re.DOTALL)
+
+    # For wogx.com
+    clean_text = re.sub(r'{h3}MORE HEADLINES:{/h3}{span}.*?{/span}{/li}{span}.*?{/span}{/li}{span}.*?{/span}{/li}{span}.*?{/span}{/li}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h3}MORE HEADLINES:{/h3}','', clean_text, flags=re.DOTALL)
+
+    # For foodandwine.com
+    clean_text = re.sub(r'Was this page helpful\?\n \n  \n \n\nTell us why!','', clean_text, flags=re.DOTALL)
+
+    # For mlive.com
+    clean_text = re.sub(r'{li}{span}{b}RELATED: {/b}.*?{/span}{/li}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}{b}Related:{/b}{b}.*?{/b}{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{/p}{b}More on MLive:{/b}{/p}.*?{/p}.*?{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}{b}RELATED: {/b}{b}.*?{/b}{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}{b}Related: {/b}{b}.*?{/b}{','}{', clean_text, flags=re.DOTALL)
+
+    # For fremonttribune.com
+    clean_text = re.sub(r"editor's pick",'', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'top story','', clean_text, flags=re.DOTALL)
+
+    # For bismarcktribune.com
+    clean_text = re.sub(r'For more information, go to\xa0   .','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Published by The Bismarck Tribune on (Jan\.|Feb\.|Mar\.|Apr\.|May|June|July|Aug\.|Sep\.|Oct\.|Nov\.|Dec\.) \d+, \d+\.', '', clean_text, flags=re.DOTALL)
+
+    # For theindependent.com
+    clean_text = re.sub(r'Email her at  .','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Published by The Grand Island Independent on (Jan\.|Feb\.|Mar\.|Apr\.|May|June|July|Aug\.|Sep\.|Oct\.|Nov\.|Dec\.) \d+, \d+\.','', clean_text, flags=re.DOTALL)
+
+    # For rapidcityjournal.com
+    clean_text = re.sub(r'}\n You must be logged in to react.  Click any reaction to login.{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Published by Rapid City Journal on (Jan\.|Feb\.|Mar\.|Apr\.|May|June|July|Aug\.|Sep\.|Oct\.|Nov\.|Dec\.) \d+, \d+\.','', clean_text, flags=re.DOTALL)
+
+    # For vikingsterritory.com
+    clean_text = re.sub(r'} \nShare:\xa0\n \n{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{li}\n \n Share on Reddit{/span}\n \n{/li}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{li}\n \n Share on WhatsApp{/span}\n \n{/li}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{li}\n Copy Link{/span}\nLink Copied\n\n{/li}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'\n \n  \nShare:\xa0\n \n','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'if you like the Vikings:\xa0','', clean_text, flags=re.DOTALL)
+
+    # For agweek.com
+    clean_text = re.sub(r'}\n ADVERTISEMENT{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n \n Read more from Agweek: {','}{', clean_text, flags=re.DOTALL)
+
+    # For sunderlandecho.com
+    clean_text = re.sub(r'} Hide Ad  {','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{span}Sign up{/span} to our  Sunderland AFC   newsletter{/h2}Sign up','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h3}Thank you for signing up!{/h3}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Did you know with a Digital Subscription to Sunderland Echo, you can get unlimited access to the website including our premium content, as well as benefiting from fewer ads, loyalty rewards and much more.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}Sorry, there seem to be some issues. Please try again later.Submitting...{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Hide Ad {','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{span}Sign up{/span} to our  daily   newsletter{/h2}Sign up','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Watch more of our videos on Shots!\xa0 and live on Freeview channel 276 Visit Shots! now ','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p} Visit Shots!\xa0for more exclusive video content and find us on Freeview channel 276. {/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}Sorry, there seem to be some issues. Please try again later.Submitting...{','}{', clean_text, flags=re.DOTALL)
+
+    # For kttc.com
+    clean_text = re.sub(r'} Find stories like this and more,  in our apps .{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}  Find stories like this and more,  in our apps .{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Click  here  for more information. {','}{', clean_text, flags=re.DOTALL)
+
+    # For fox38corpuschristi.com
+    clean_text = re.sub(r'{p}{strong}Get reports like this and all the news of the day in Middle Tennessee delivered to your inbox each morning with the .{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}READ \|{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}WATCH \| {','}{', clean_text, flags=re.DOTALL)
+
+    # For krtv.com
+    clean_text = re.sub(r'}\n\nMTN News\n \n\n{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n\nMTN News\n\n{','}{', clean_text, flags=re.DOTALL)
+
+    # For kotatv.com
+    clean_text = re.sub(r'} In addition to the live coverage, Local News Live produced a half-hour special airing on all Gray affiliates to preview the momentous event.{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} For any KOTA Territory coverage of the eclipse, you can visit the  livestream page .{','}{', clean_text, flags=re.DOTALL)
+
+    # For nexttv.com
+    clean_text = re.sub(r'} NEXT TV NEWSLETTER{/h2} The smarter way to stay on top of the streaming and OTT industry. Sign up below.{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} \* To subscribe, you must consent to Future’s privacy policy.{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} \* To subscribe, you must consent to Future’s privacy policy.\n\n{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'} Broadcasting &amp; Cable Newsletter{/h2} The smarter way to stay on top of broadcasting and cable industry. Sign up below{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\nMore about broadcasting and cable {','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Analyst Raises Forecast for Netflix Subscribers, Revenue Per Sub{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Hallmark Leans on Traditional Strengths in Upfront Negotiations{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Amazon Prime Video Extends Rights Deal With WNBA{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Also Read: {/strong}.*? {/p}','', clean_text, flags=re.DOTALL)
+
+    # For devinenews.com
+    #clean_text = re.sub(r'{p}TO CONTINUE READING…or go to www.devinenewsmembers.com {/p}','', clean_text, flags=re.DOTALL)
+
+    # For livenowfox.com
+    clean_text = re.sub(r'article','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{i}{strong}To get the best local news, weather and sports in Seattle for free, sign up for the daily {/strong}{/i}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{strong}FOX 13 Seattle newsletter{/strong}{i}{strong}.{/strong}{/i}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h3}{strong}WATCH FOX 13 NEWS{/strong}{/h3}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{i}{strong}SIGN UP: {/strong}{/i}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{i}{strong}For more Lifestyle s, visit www.foxnews.com/lifestyle.{/strong}{/i}{/p}','', clean_text, flags=re.DOTALL)
+
+    # For chicagotribune.com
+    clean_text = re.sub(r'{p}Submit a letter, of no more than \d+ words, to the editor  here  or email  .{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}More top \w+ stories:{/strong}{/p}\n \n{li}.*?{/li}\n{li}.*?{/li}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}More top Eat. Watch. Do. stories:{/strong}{/p}\n \n{li}.*?{/li}\n{li}.*?{/li}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}More top stories from around the world:{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{strong}Read more here.{/strong}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h3}General Daily Insight for (January|February|March|April|May|June|July|August|September|October|November|December) \d+, \d+{/h3}','', clean_text, flags=re.DOTALL)
+
+    # For indiewire.com
+    clean_text = re.sub(r'{p}{strong} Read IndieWire’s Complete Review of “.*?.”  {/strong}{/p}','', clean_text, flags=re.DOTALL)
+
+    # For fox29.com
+    clean_text = re.sub(r'{p}{strong}MORE HEADLINES:\xa0{/strong}{/p}{span}{strong}.*?{/strong}{/span}{/li}{span}{strong}.*?{/strong}{/span}{/li}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}MORE HEADLINES{/strong}{/p}{span}{strong}.*?{/strong}{/span}{/li}{span}{strong}.*?{/strong}{/span}{/li}{span}{strong}.*?{/strong}{/span}{/li}','', clean_text, flags=re.DOTALL)
+
+    # For alligator.org
+    clean_text = re.sub(r'}\n\n\nSupport your local paper\n {strong}Donate Today{/strong}\s*The Independent Florida Alligator has been independent of the university since 1971, your donation today could help #SaveStudentNewsrooms. Please consider giving today.\s*{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}Contact \w+ \w+ at  . Follow \w+ on X your local paper\n {strong}Donate Today{/strong}\s*The Independent Florida Alligator has been independent of the university since 1971, your donation today could help #SaveStudentNewsrooms. Please consider giving today.\s*{','}{', clean_text, flags=re.DOTALL)
+
+    # For prospect.org
+    clean_text = re.sub(r'{p}{strong}More from .*?{/strong}{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong} More from .*?{/strong}{/p}','', clean_text, flags=re.DOTALL)
+
+    # For sevendaysvt.com
+    clean_text = re.sub(r'\n click to enlarge','', clean_text, flags=re.DOTALL)
+
+    # For bleacherreport.com
+    clean_text = re.sub(r'Copy Link Icon','', clean_text, flags=re.DOTALL)
+
+    # For onscene.tv
+    clean_text = re.sub(r'}\n Comments{/h3}\n \n Back to top button{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n Comments{','}{', clean_text, flags=re.DOTALL)
+
+    # For mychesco.com
+    clean_text = re.sub(r'{p}For the latest news on everything happening in  Chester County  and the surrounding area, be sure to follow MyChesCo on {strong} Google News {/strong}{strong} Microsoft Start {/strong}.{/p}','', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}. Stay updated on the latest news and information from MyChesCo with our\xa0 free newsletter . Follow MyChesCo on Twitter at\xa0 twitter.com/MyChesCo \xa0and like us on Facebook at\xa0 facebook.com/MyChesCo .{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}For the latest news on everything happening in Chester County and the surrounding area, be sure to follow MyChesCo on {strong} Google News {/strong}{strong} Microsoft Start {/strong}.{/p}','', clean_text, flags=re.DOTALL)
+
+
+    # For patch.com (continue.....)
+    clean_text = re.sub(r'}{li}Related:.*?{/li}{', '}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h6} Politics &amp; Government {/h6}', '', clean_text, flags=re.DOTALL)
+
+    # For elpasonews.org
+    clean_text = re.sub(r'}\n\t\t \n\t\t\n\t\t Like this:{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Get more local news delivered straight to your inbox.   \.', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n\n\n\n Like this:{','}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'In upcoming articles, we will explore further how the local news outlets decide what is newsworthy and what is not for El Paso&#8217;s news consumers. Stay tuned.', '',clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n\n\t\t \n\t\t\n\t\t Like this:{', '}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n\n\n\n Disclosure{', '}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Each election cycle, El Paso News publishes the names of the political candidates that the technology company owned by Mart&#237;n Paredes provides branding and technology services to. Although not required to, we provide this list to our readers for transparency purposes. Clients of  Cognent  have no influence over the stories we choose to cover.for more details.', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'}\n\n\n\n\n Disclosure{', '}{', clean_text, flags=re.DOTALL)
+
+    # For newsweek.com(continue.....)
+    clean_text = re.sub(r'}\n fairness meter{', '}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h2}fairness meter{/h2}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r"Newsweek is committed to journalism that\'s factual and fair.", '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'Hold us accountable and submit your rating of this article on the meter.', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{span}Click On Meter {/span}{span}To Rate This Article{/span}\n About the writer{/h3}\n \n  \w+ \w+  \n{/span}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r"{p}\w+ \w+ is a Weekend Reporter at Newsweek based in New York. Her focus is reporting on education, social justice.*?{/p}", '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'To read how Newsweek uses AI as a newsroom tool,.', '', clean_text, flags=re.DOTALL)
+
+    # For nbcnews.com(continue.....)
+    clean_text = re.sub(r'{strong}For more from NBC BLK, {/strong}{strong}sign up for our weekly newsletter{/strong}{strong}.{/strong}', '', clean_text, flags=re.DOTALL)
+
+    # For wfmz.com
+    clean_text = re.sub(r'{strong}Media Contact\xa0{/strong}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}\w+ for Placemakr{/p}   View original content to download multimedia:   {/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}SOURCE Placemakr{/p}', '', clean_text, flags=re.DOTALL)
+
+    # For ksat.com (continue.....)
+    clean_text = re.sub(r'{i}{b}ALSO ON KSAT.COM: {/b}{/i}{i}{b}.*?{/b}{/i}', '', clean_text, flags=re.DOTALL)
+
+    # For news.yahoo.com
+    clean_text = re.sub(r'{strong}SEAN ‘DIDDY’ {/strong}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r"{p}Knight\'s full remarks are available on  Breakbeat\'s YouTube .{/p}", '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}SEAN ‘DIDDY’ ‘DIRTYING’ JURY POOL, LEAKS{/strong}{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{b}Read also:{/b}.*?{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Read more:{/strong}.*?{/p}', '' , clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}Get the latest from \w+ \w+{/strong} Commentary on economics and more from a Pulitzer Prize winner.  {strong}Sign me up.{/strong}{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{b}READ:.*?{/b}{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Stay with  WFTV.com  and watch Eyewitness News for updates on this story.{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}&gt;&gt;{b}RELATED: {/b}{b}.*?{/b}{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Author Bio{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Do you have a question\?{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r"{p}A comment you\'d like to see published\?{/p}", '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}Or maybe a story idea for a future edition\?{/p}', '', clean_text, flags=re.DOTALL)
+
+    # For nme.com(continue.....)
+    clean_text = re.sub(r'{li}{b}READ MORE:.{/b}{b}.*?{/b}{/li}', '', clean_text, flags=re.DOTALL)
+
+    # For fox7austin.com(continue.....)
+    clean_text = re.sub(r'{h3}MORE STORIES{/h3}', '', clean_text, flags=re.DOTALL)
+
+    # For fox4news.com
+    clean_text = re.sub(r'{p}{strong}MORE STORIES:{/strong}{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}SUGGESTED:{/strong}{/p}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{h3}READ MORE{/h3}{span}{strong}.*?{/strong}{/span}', '', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'{p}{strong}MORE HEADLINES:{/strong}{/p}{span}{strong}.*?{/strong}{/span}', '', clean_text, flags=re.DOTALL)
+
+    # For businessinsider.com (continues.....)
+    clean_text = re.sub(r'}\n \n\s*Read next\n\s*{', '}{', clean_text, flags=re.DOTALL)
+    clean_text = re.sub(r'\n Congress \n Colorado \n Republican Party \n\n\n\n \n\n', '', clean_text, flags=re.DOTALL)
+
+    # For edition.cnn.com (continues.....)
+    clean_text = re.sub(r'} Read more\xa0 here .{', '}{', clean_text, flags=re.DOTALL)
+
+    # For indiatimes.com (continues....)
+    clean_text = re.sub(r'{p}{strong}Also Read:.*?{/strong}{/p}', '', clean_text, flags=re.DOTALL)
     
     # display(clean_text)
 
 
     clean_text = re.sub('(\\n)','',clean_text) #removing new line character
     clean_text = re.sub('(\\t)','',clean_text) #removing tabular character
     clean_text = re.sub('(\\r)','',clean_text) #removing carriage return character
```

### Comparing `newscleaner-0.1.6/src/newscleaner/setup.py` & `newscleaner-0.1.7/src/newscleaner/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="newscleaner",
-    version="0.1.6",
+    version="0.1.7",
     author="Lakshita Kain",
     author_email="mail@pankajjha.me",
     description="Package to clean up waste postfix from articles",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pankajjha/newscleaner",
     project_urls={
```

### Comparing `newscleaner-0.1.6/src/newscleaner/strip_clean.py` & `newscleaner-0.1.7/src/newscleaner/strip_clean.py`

 * *Files identical despite different names*

### Comparing `newscleaner-0.1.6/src/newscleaner.egg-info/PKG-INFO` & `newscleaner-0.1.7/src/newscleaner.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: newscleaner
-Version: 0.1.6
-Summary: Package to clean up noise from news articles
-Home-page: https://github.com/pankajjha/newscleaner
-Author: Lakshita Kain
-Author-email: mail@pankajjha.me
-Project-URL: Bug Tracker, https://github.com/pankajjha/newscleaner/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
-# Article Cleaner
+Metadata-Version: 2.1
+Name: newscleaner
+Version: 0.1.7
+Summary: Package to clean up noise from news articles
+Home-page: https://github.com/pankajjha/newscleaner
+Author: Lakshita Kain
+Author-email: mail@pankajjha.me
+Project-URL: Bug Tracker, https://github.com/pankajjha/newscleaner/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
+# Article Cleaner
```

### Comparing `newscleaner-0.1.6/src/newscleaner.egg-info/PKG-INFO.txt` & `newscleaner-0.1.7/src/newscleaner.egg-info/PKG-INFO.txt`

 * *Files identical despite different names*

