# Comparing `tmp/randevu-2.0.0.tar.gz` & `tmp/randevu-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randevu-2.0.0.tar", last modified: Tue May 14 20:59:10 2024, max compression
+gzip compressed data, was "randevu-2.0.1.tar", last modified: Mon May 20 00:38:09 2024, max compression
```

## Comparing `randevu-2.0.0.tar` & `randevu-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 20:59:10.629728 randevu-2.0.0/
--rw-rw-rw-   0        0        0    13768 2024-05-09 12:32:07.000000 randevu-2.0.0/LICENSE
--rw-rw-rw-   0        0        0    11865 2024-05-14 20:59:10.628767 randevu-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10946 2024-05-14 20:33:59.000000 randevu-2.0.0/README.md
--rw-rw-rw-   0        0        0      590 2024-05-14 20:59:04.000000 randevu-2.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-14 20:59:10.625044 randevu-2.0.0/randevu.egg-info/
--rw-rw-rw-   0        0        0    11865 2024-05-14 20:59:10.000000 randevu-2.0.0/randevu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-14 20:59:10.000000 randevu-2.0.0/randevu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 20:59:10.000000 randevu-2.0.0/randevu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 20:59:10.000000 randevu-2.0.0/randevu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 20:59:10.629728 randevu-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      860 2024-05-14 20:33:59.000000 randevu-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 20:59:10.625044 randevu-2.0.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-09 14:39:59.000000 randevu-2.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1654 2024-05-14 20:34:00.000000 randevu-2.0.0/tests/test_randevu.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:09.603393 randevu-2.0.1/
+-rw-rw-rw-   0        0        0     3018 2024-05-19 21:28:55.000000 randevu-2.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0    15557 2024-05-20 00:38:09.603393 randevu-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10908 2024-05-19 19:38:52.000000 randevu-2.0.1/README.md
+-rw-rw-rw-   0        0        0      856 2024-05-20 00:21:43.000000 randevu-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 00:38:09.603393 randevu-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:09.544255 randevu-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:09.550325 randevu-2.0.1/src/randevu/
+-rw-rw-rw-   0        0        0       31 2024-05-19 20:33:32.000000 randevu-2.0.1/src/randevu/__init__.py
+-rw-rw-rw-   0        0        0     3453 2024-05-19 20:33:37.000000 randevu-2.0.1/src/randevu/randevu.py
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:09.602214 randevu-2.0.1/src/randevu.egg-info/
+-rw-rw-rw-   0        0        0    15557 2024-05-20 00:38:09.000000 randevu-2.0.1/src/randevu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-20 00:38:09.000000 randevu-2.0.1/src/randevu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 00:38:09.000000 randevu-2.0.1/src/randevu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 00:38:09.000000 randevu-2.0.1/src/randevu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 00:38:09.000000 randevu-2.0.1/src/randevu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 00:38:09.601214 randevu-2.0.1/tests/
+-rw-rw-rw-   0        0        0     1496 2024-05-20 00:36:42.000000 randevu-2.0.1/tests/test_randevu.py
```

### Comparing `randevu-2.0.0/PKG-INFO` & `randevu-2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,235 +1,218 @@
-Metadata-Version: 2.1
-Name: randevu
-Version: 2.0.0
-Summary: The official Python implementation of the RANDEVU algorithm
-Home-page: https://github.com/TypicalHog/randevu-py
-Author: TypicalHog
-Project-URL: Homepage, https://github.com/TypicalHog/randevu-py
-Project-URL: Issues, https://github.com/TypicalHog/randevu-py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# RANDEVU
-**Universal Probabilistic Daily Reminder Coordination System for Anything**  
-
-- UNIVERSAL - reminders for the same object are the same for everyone  
-- PROBABILISTIC - reminders are calculated using a simple probabilistic
-algorithm based on powers of 2  
-- DAILY - reminders are following a daily schedule/interval (UTC)  
-- INTRADAY - infinite optional intraday reminder times (RDVT - added in version
-2.0 as an extension to the existing system)  
-- GENERIC - applicable to anything and everything, literally (where it makes
-sense, see use cases)  
-- FOSS - in the public domain (Unlicense or MIT or Apache-2.0)  
-- OFFLINE - no internet connection required  
-- PORTABLE - simple code, easy to port anywhere where blake3 is available  
-- DETERMINISTIC - easily computable and predictable for any object and any date  
-- PSEUDORANDOM - reminders are spaced randomly and uniformly  
-- ADJUSTABLE - user can decide how frequently (roughly) they'd like to see
-reminders for each object  
-
-https://github.com/TypicalHog/randevu (Rust - **REFERENCE IMPLEMENTATION**)  
-https://github.com/TypicalHog/randevu-ts (TypeScript)  
-**https://github.com/TypicalHog/randevu-py (Python)**  
-The above implementations are available on Crates.io, PyPI, and npm as **randevu**.  
-Feel free to contribute, create an implementation in another (missing) language,
-or even an alternative one for 1 (or more) of the 3 languages I've already
-created a repository and crate/module/package for.  
-
-## EXAMPLE USAGE
-```python
-from datetime import datetime
-from randevu import rdv, rdvt
-
-object = "THE_SIMPSONS"
-date = datetime.now().date()
-rdv_value = rdv(object, date)
-rdvt_value = rdvt(0, object, date)
-
-print(f"Object {object} has RDV{rdv_value} today with RDVT0 at {rdvt_value}")
-
-```
-
----
-
-**I'm aware of the fact that README.md is a confusing jungle of words, random**
-**thoughts, and ideas. (Will work on it)**  
-I kinda suck at explaining stuff and structuring text in an organized manner.
-I'm sorry about that. :/  
-I gave it my best, and I'll keep trying to improve it in the future.  
-This whole document will probably be revamped entirely. Stuff will be explained
-better, irrelevant things, tangents, thoughts and rambles removed, etc.  
-I would also like to write something like a proper spec for the RANDEVU
-algorithm/system.  
-I'm thinking about creating a FAQ section/document where I'll explain various
-aspects of the system and anything else I'd like to clarify or expand on in more
-detail.  
-Also thinking about adding some visual analogies (infographics) with coin
-tossing and such which I believe have enormous potential in terms of making the
-system easier to explain, as well as understand.  
-
----
-
-## KEY CONCEPTS
-- OBJECT - a string representing anything that is representable with a string of
-characters (a game, a movie, a person, a song, a place, a video, a topic,
-a word, a book, a number, a brand, a post, an event, an item, a website, an app,
-a quote, an action, a movement or **literally** anything else)  
-- DATE - a date (UTC) for which we want to calculate the RDV for  
-- RDV - a positive integer representing the level/significance/rarity of a
-reminder for a certain OBJECT on a specific DATE  
-
-**(New feature of version 2.0)**  
-- RDVT - one of an infinite number of random moments in a day (0-24h UTC) when
-an object has its reminders for that day, allows for infinite precission  
-- RANK - RDVT rank, ranked 0 (most significant) to infinity - RDVT0, RDVT1...  
-
-## RDV CALCULATION
-`RDV = number of leading zero bits in blake3::keyed_hash(key: DATE, data: OBJECT)`  
-Note: The previous version (1.0) used a different algorithm, so the RDV values
-between the two versions have changed and are completely un-correlated.  
-By implementing this change, I've eliminated 2/3 blake3 hash calculations and
-improved performance (not that it mattered).  
-But now I can calculate about 10 million RDV values per second on my PC.  
-I have strong reasons to believe such major changes won't be happening in the
-future and that this is the final version of the algorithm.  
-It was still a good time to do such a fundamental change to the algorithm, since
-RANDEVU had essentially no adoption apart from myself and a small community I'm
-a part of.  
-
-## HOW IT WORKS AND POTENTIAL USE CASES
-Imagine a system that assigns a special number (RDV) to every object each day.  
-The number assigned to each object is different for each object and changes
-daily.  
-The number has a 50% chance to be 0, 25% chance to be 1, 12.5% to be 2, and so
-on (each number being twice as rare).  
-I've based everything around base-2 (simplest numerical base after unary), it
-makes everything fit together so perfectly (you'll probably see why when you
-learn more about how the system works).  
-By making each reminder level twice as rare - we can achive effectively
-infinitely infrequent reminders, as well as daily ones, and a pretty good range
-of reminders of various frequencies in between.  
-If an object has a reminder RDV4, that also implies RDV3, RDV2, RDV1 and RDV0.  
-Users can then choose to set a threshold value for each object and if the RDV
-value for a specific object is greater than or equal to the threshold - the user
-may decide to do something with that object.  
-For example, one may decide to watch a certain video once its RDV value (RDV
-value for that specific video) hits their desired threshold.  
-Threshold allows one to decide how often they would like to be "reminded of" a
-certain object.  
-0 -> every day, 1 -> every 2 days (on average - it's random), 2 -> 4 days, 3 ->
-8 days, and so on (allows for essentially infinite frequencies of reminders,
-though ones above 10 happen quite rarely - 2^10 = 1024 days).  
-If multiple people used this system to get reminded of the same things - they
-would all get reminded of them on the same days and thus be able to coordinate
-meetings/actions related to the objects in question.  
-This could allow fans of a "dead" game (game with no or little players online)
-to all meet and play it on the same day, let's say once every 256 days.  
-People could re-watch their favorite movies or videos and discuss them with
-other fellow fans on the same days.  
-This system can be applied to anything.  
-It can be used to assign special appreciation/remembrance days to your favorite
-books, songs, artists, events, or (as I already said) - ANYTHING.  
-One could have a huge list of objects they care about and never again risk
-forgetting any of them - since they will be reminded of them eventually (for
-example - bookmarks).  
-
-## RDVT CALCULATION AND USE CASES
-RDVT is a newly added (version 2.0) feature of the RANDEVU system and an
-optional extension of the RDV algorithm.  
-We calculate the hash the same way as for RDV, except we append a RANK integer
-to the DATE inside the key, separated by an '_'. And we don't count leading zero
-bits.  
-Instead, we iterate over the bits in the hash and add increments to the RDVT
-time (which starts at 00:00h, midnight). For each 1 we add an increment, and do
-nothing if the bit is 0.  
-An increment starts at 12h, and we divide it by half after processing each bit.  
-For example, if the first 4 bits are 0110 - this will result in a time value of
-09:00h (0 * 12h + 1 * 6h + 1 * 3h + 0 * 1.5h...).  
-Note that there are 256 bits and we keep doing this until we reach 1 ns (or
-millisecond/microsecond, depending on the implementation).  
-This means we get a different uniform pseudorandom time (0-24h) for each RANK.  
-If users find the daily RDV reminder too broad and would like a more specific
-time for the reminder - they can calculate one or more RDVT times and choose
-one.  
-Since RDVT0 is the most important/main time, users should choose the
-lowest-ranked RDVT that works for them - this increases the chances other people
-will also choose the same RDVT time as them, thus increasing the chances of an
-interaction.  
-Let's say a certain YouTube video has an RDV10 today. We could have a browser
-extension or a website that would schedule streams (like video premieres) for
-that video at the first 10 RDVT times (RDVT0-9).  
-Fans of that video could all come re-watch it live with others at one of the
-RDVT times, and perhaps chat about it in the live chat (assuming the feature
-existed) while experiencing it together.  
-This is just one super specific hypothetical use case I came up with.  
-
----
-
-## OBJECT NAMING CONVENTION (non-exhaustive examples)
-OBJECT is a string (preferably uppercase A-Z, 0-9). No spaces allowed.  
-Spaces and any other characters should be replaced with a single underscore
-('_').  
-Characters outside of this set should only be used for external identifiers that
-are case-sensitive or contain other symbols, for example, YOUTUBE video IDs.  
-
-```
-XONOTIC (all letters should be uppercase)
-
-STAR_WARS (spaces and dashes in multi-word objects should be replaced with _)
-
-THE_MATRIX_1999 (movies should have a year of release at the end)
-
-GRAND_THEFT_AUTO_5 (objects should be referenced by their full name, Roman
-numerals should be replaced with Arabic ones)
-
-ASAP_ROCKY ($ should be replaced with S, same for other similar instances)
-
-C_PLUS_PLUS (++ should be replaced with _PLUS_PLUS)
-
-C_SHARP (# should be replaced with _SHARP, in other contexts it could be _HASH
-or omitted)
-
-YEAR_2000 (years should have a YEAR_ prefix)
-
-FRIDAY (weekdays and months should not be abbreviated, same as all other
-objects)
-
-2023-08-25 (dates should be in ISO 8601 format, YYYY-MM-DD)
-
-NO_MANS_SKY (apostrophe in MAN'S should be dropped)
-
-HARRY_POTTER_SMOKES_WEED_Cdfkq2Nmb3c (video ID should be appended to the video
-title, double underscore is fine if the ID starts with one, IDs are allowed to
-use dashes and lowercase letters)
-
-GETTING_BANGED_BY_GREEN_BOOMERS_MINECRAFT_BETA_1_7_3_SOLO_SURVIVAL_NO_COMMENTARY_OJzsmWBQE3I
-(brackets, quotation marks, colons, and other punctuation should be dropped,
-periods in version numbers like 1.7.3 should be replaced with _)
-
-NUMBER_69 (numbers should have a NUMBER_ prefix)
-
-```
-
-### WHY THIS VERY SPECIFIC AND STRICT CONVENTION THO?
-
-**TO MAKE SURE EVERYONE GETS THE SAME REMINDERS FOR THE SAME THINGS ON THE SAME**
-**DAYS.**  
-
-Due to how the algorithm works - even just a single character difference between
-two objects causes the system to generate completely different reminders for
-each.  
-For example: WEED, weed, Weed, and W33D would all be treated as different and
-independent objects with completely unrelated reminders.  
-One can think of objects like passwords - the same password gets you the same
-reminders as everyone else using said password.  
-If one wanted to get completely different reminders from other people for a
-specific object - they could append extra characters to it.  
-However, this is not the focus of the system. The whole point is to help people
-coordinate getting reminded about stuff at the same time as everyone else.  
+# RANDEVU
+**Universal Probabilistic Daily Reminder Coordination System for Anything**  
+
+- UNIVERSAL - reminders for the same object are the same for everyone  
+- PROBABILISTIC - reminders are calculated using a simple probabilistic
+algorithm based on powers of 2  
+- DAILY - reminders are following a daily schedule/interval (UTC)  
+- INTRADAY - infinite optional intraday reminder times (RDVT - added in version
+2.0 as an extension to the existing system)  
+- GENERIC - applicable to anything and everything, literally (where it makes
+sense, see use cases)  
+- FOSS - in the public domain (Unlicense or MIT or Apache-2.0)  
+- OFFLINE - no internet connection required  
+- PORTABLE - simple code, easy to port anywhere where blake3 is available  
+- DETERMINISTIC - easily computable and predictable for any object and any date  
+- PSEUDORANDOM - reminders are spaced randomly and uniformly  
+- ADJUSTABLE - user can decide how frequently (roughly) they'd like to see
+reminders for each object  
+
+https://github.com/TypicalHog/randevu (Rust - **REFERENCE IMPLEMENTATION**)  
+https://github.com/TypicalHog/randevu-ts (TypeScript)  
+**https://github.com/TypicalHog/randevu-py (Python)**  
+The above implementations are available on Crates.io, PyPI, and npm as **randevu**.  
+Feel free to contribute, create an implementation in another (missing) language,
+or even an alternative one for 1 (or more) of the 3 languages I've already
+created a repository and crate/module/package for.  
+
+## EXAMPLE USAGE
+```python
+from datetime import datetime
+from randevu import rdv, rdvt
+
+object = "THE_SIMPSONS"
+date = datetime.now().date()
+rdv_value = rdv(object, date)
+rdvt_value = rdvt(0, object, date)
+
+print(f"Object {object} has RDV{rdv_value} today with RDVT0 at {rdvt_value}")
+
+```
+
+---
+
+**I'm aware of the fact that README.md is a confusing jungle of words, random**
+**thoughts, and ideas. (Will work on it)**  
+I kinda suck at explaining stuff and structuring text in an organized manner.
+I'm sorry about that. :/  
+I gave it my best, and I'll keep trying to improve it in the future.  
+This whole document will probably be revamped entirely. Stuff will be explained
+better, irrelevant things, tangents, thoughts and rambles removed, etc.  
+I would also like to write something like a proper spec for the RANDEVU
+algorithm/system.  
+I'm thinking about creating a FAQ section/document where I'll explain various
+aspects of the system and anything else I'd like to clarify or expand on in more
+detail.  
+Also thinking about adding some visual analogies (infographics) with coin
+tossing and such which I believe have enormous potential in terms of making the
+system easier to explain, as well as understand.  
+
+---
+
+## KEY CONCEPTS
+- OBJECT - a string representing anything that is representable with a string of
+characters (a game, a movie, a person, a song, a place, a video, a topic,
+a word, a book, a number, a brand, a post, an event, an item, a website, an app,
+a quote, an action, a movement or **literally** anything else)  
+- DATE - a date (UTC) for which we want to calculate the RDV for  
+- RDV - a positive integer representing the level/significance/rarity of a
+reminder for a certain OBJECT on a specific DATE  
+
+**(New feature of version 2.0)**  
+- RDVT - one of an infinite number of random moments in a day (0-24h UTC) when
+an object has its reminders for that day, allows for infinite precission  
+- RANK - RDVT rank, ranked 0 (most significant) to infinity - RDVT0, RDVT1...  
+
+## RDV CALCULATION
+`RDV = number of leading zero bits in blake3::keyed_hash(key: DATE, data: OBJECT)`  
+Note: The previous version (1.0) used a different algorithm, so the RDV values
+between the two versions have changed and are completely un-correlated.  
+By implementing this change, I've eliminated 2/3 blake3 hash calculations and
+improved performance (not that it mattered).  
+But now I can calculate about 10 million RDV values per second on my PC.  
+I have strong reasons to believe such major changes won't be happening in the
+future and that this is the final version of the algorithm.  
+It was still a good time to do such a fundamental change to the algorithm, since
+RANDEVU had essentially no adoption apart from myself and a small community I'm
+a part of.  
+
+## HOW IT WORKS AND POTENTIAL USE CASES
+Imagine a system that assigns a special number (RDV) to every object each day.  
+The number assigned to each object is different for each object and changes
+daily.  
+The number has a 50% chance to be 0, 25% chance to be 1, 12.5% to be 2, and so
+on (each number being twice as rare).  
+I've based everything around base-2 (simplest numerical base after unary), it
+makes everything fit together so perfectly (you'll probably see why when you
+learn more about how the system works).  
+By making each reminder level twice as rare - we can achive effectively
+infinitely infrequent reminders, as well as daily ones, and a pretty good range
+of reminders of various frequencies in between.  
+If an object has a reminder RDV4, that also implies RDV3, RDV2, RDV1 and RDV0.  
+Users can then choose to set a threshold value for each object and if the RDV
+value for a specific object is greater than or equal to the threshold - the user
+may decide to do something with that object.  
+For example, one may decide to watch a certain video once its RDV value (RDV
+value for that specific video) hits their desired threshold.  
+Threshold allows one to decide how often they would like to be "reminded of" a
+certain object.  
+0 -> every day, 1 -> every 2 days (on average - it's random), 2 -> 4 days, 3 ->
+8 days, and so on (allows for essentially infinite frequencies of reminders,
+though ones above 10 happen quite rarely - 2^10 = 1024 days).  
+If multiple people used this system to get reminded of the same things - they
+would all get reminded of them on the same days and thus be able to coordinate
+meetings/actions related to the objects in question.  
+This could allow fans of a "dead" game (game with no or little players online)
+to all meet and play it on the same day, let's say once every 256 days.  
+People could re-watch their favorite movies or videos and discuss them with
+other fellow fans on the same days.  
+This system can be applied to anything.  
+It can be used to assign special appreciation/remembrance days to your favorite
+books, songs, artists, events, or (as I already said) - ANYTHING.  
+One could have a huge list of objects they care about and never again risk
+forgetting any of them - since they will be reminded of them eventually (for
+example - bookmarks).  
+
+## RDVT CALCULATION AND USE CASES
+RDVT is a newly added (version 2.0) feature of the RANDEVU system and an
+optional extension of the RDV algorithm.  
+We calculate the hash the same way as for RDV, except we append a RANK integer
+to the DATE inside the key, separated by an '_'. And we don't count leading zero
+bits.  
+Instead, we iterate over the bits in the hash and add increments to the RDVT
+time (which starts at 00:00h, midnight). For each 1 we add an increment, and do
+nothing if the bit is 0.  
+An increment starts at 12h, and we divide it by half after processing each bit.  
+For example, if the first 4 bits are 0110 - this will result in a time value of
+09:00h (0 * 12h + 1 * 6h + 1 * 3h + 0 * 1.5h...).  
+Note that there are 256 bits and we keep doing this until we reach 1 ns (or
+millisecond/microsecond, depending on the implementation).  
+This means we get a different uniform pseudorandom time (0-24h) for each RANK.  
+If users find the daily RDV reminder too broad and would like a more specific
+time for the reminder - they can calculate one or more RDVT times and choose
+one.  
+Since RDVT0 is the most important/main time, users should choose the
+lowest-ranked RDVT that works for them - this increases the chances other people
+will also choose the same RDVT time as them, thus increasing the chances of an
+interaction.  
+Let's say a certain YouTube video has an RDV10 today. We could have a browser
+extension or a website that would schedule streams (like video premieres) for
+that video at the first 10 RDVT times (RDVT0-9).  
+Fans of that video could all come re-watch it live with others at one of the
+RDVT times, and perhaps chat about it in the live chat (assuming the feature
+existed) while experiencing it together.  
+This is just one super specific hypothetical use case I came up with.  
+
+---
+
+## OBJECT NAMING CONVENTION (non-exhaustive examples)
+OBJECT is a string (preferably uppercase A-Z, 0-9). No spaces allowed.  
+Spaces and any other characters should be replaced with a single underscore
+('_').  
+Characters outside of this set should only be used for external identifiers that
+are case-sensitive or contain other symbols, for example, YOUTUBE video IDs.  
+
+```
+XONOTIC (all letters should be uppercase)
+
+STAR_WARS (spaces and dashes in multi-word objects should be replaced with _)
+
+THE_MATRIX_1999 (movies should have a year of release at the end)
+
+GRAND_THEFT_AUTO_5 (objects should be referenced by their full name, Roman
+numerals should be replaced with Arabic ones)
+
+ASAP_ROCKY ($ should be replaced with S, same for other similar instances)
+
+C_PLUS_PLUS (++ should be replaced with _PLUS_PLUS)
+
+C_SHARP (# should be replaced with _SHARP, in other contexts it could be _HASH
+or omitted)
+
+YEAR_2000 (years should have a YEAR_ prefix)
+
+FRIDAY (weekdays and months should not be abbreviated, same as all other
+objects)
+
+2023-08-25 (dates should be in ISO 8601 format, YYYY-MM-DD)
+
+NO_MANS_SKY (apostrophe in MAN'S should be dropped)
+
+HARRY_POTTER_SMOKES_WEED_Cdfkq2Nmb3c (video ID should be appended to the video
+title, double underscore is fine if the ID starts with one, IDs are allowed to
+use dashes and lowercase letters)
+
+GETTING_BANGED_BY_GREEN_BOOMERS_MINECRAFT_BETA_1_7_3_SOLO_SURVIVAL_NO_COMMENTARY_OJzsmWBQE3I
+(brackets, quotation marks, colons, and other punctuation should be dropped,
+periods in version numbers like 1.7.3 should be replaced with _)
+
+NUMBER_69 (numbers should have a NUMBER_ prefix)
+
+```
+
+### WHY THIS VERY SPECIFIC AND STRICT CONVENTION THO?
+
+**TO MAKE SURE EVERYONE GETS THE SAME REMINDERS FOR THE SAME THINGS ON THE SAME**
+**DAYS.**  
+
+Due to how the algorithm works - even just a single character difference between
+two objects causes the system to generate completely different reminders for
+each.  
+For example: WEED, weed, Weed, and W33D would all be treated as different and
+independent objects with completely unrelated reminders.  
+One can think of objects like passwords - the same password gets you the same
+reminders as everyone else using said password.  
+If one wanted to get completely different reminders from other people for a
+specific object - they could append extra characters to it.  
+However, this is not the focus of the system. The whole point is to help people
+coordinate getting reminded about stuff at the same time as everyone else.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `randevu-2.0.0/README.md` & `randevu-2.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,218 +1,309 @@
-# RANDEVU
-**Universal Probabilistic Daily Reminder Coordination System for Anything**  
-
-- UNIVERSAL - reminders for the same object are the same for everyone  
-- PROBABILISTIC - reminders are calculated using a simple probabilistic
-algorithm based on powers of 2  
-- DAILY - reminders are following a daily schedule/interval (UTC)  
-- INTRADAY - infinite optional intraday reminder times (RDVT - added in version
-2.0 as an extension to the existing system)  
-- GENERIC - applicable to anything and everything, literally (where it makes
-sense, see use cases)  
-- FOSS - in the public domain (Unlicense or MIT or Apache-2.0)  
-- OFFLINE - no internet connection required  
-- PORTABLE - simple code, easy to port anywhere where blake3 is available  
-- DETERMINISTIC - easily computable and predictable for any object and any date  
-- PSEUDORANDOM - reminders are spaced randomly and uniformly  
-- ADJUSTABLE - user can decide how frequently (roughly) they'd like to see
-reminders for each object  
-
-https://github.com/TypicalHog/randevu (Rust - **REFERENCE IMPLEMENTATION**)  
-https://github.com/TypicalHog/randevu-ts (TypeScript)  
-**https://github.com/TypicalHog/randevu-py (Python)**  
-The above implementations are available on Crates.io, PyPI, and npm as **randevu**.  
-Feel free to contribute, create an implementation in another (missing) language,
-or even an alternative one for 1 (or more) of the 3 languages I've already
-created a repository and crate/module/package for.  
-
-## EXAMPLE USAGE
-```python
-from datetime import datetime
-from randevu import rdv, rdvt
-
-object = "THE_SIMPSONS"
-date = datetime.now().date()
-rdv_value = rdv(object, date)
-rdvt_value = rdvt(0, object, date)
-
-print(f"Object {object} has RDV{rdv_value} today with RDVT0 at {rdvt_value}")
-
-```
-
----
-
-**I'm aware of the fact that README.md is a confusing jungle of words, random**
-**thoughts, and ideas. (Will work on it)**  
-I kinda suck at explaining stuff and structuring text in an organized manner.
-I'm sorry about that. :/  
-I gave it my best, and I'll keep trying to improve it in the future.  
-This whole document will probably be revamped entirely. Stuff will be explained
-better, irrelevant things, tangents, thoughts and rambles removed, etc.  
-I would also like to write something like a proper spec for the RANDEVU
-algorithm/system.  
-I'm thinking about creating a FAQ section/document where I'll explain various
-aspects of the system and anything else I'd like to clarify or expand on in more
-detail.  
-Also thinking about adding some visual analogies (infographics) with coin
-tossing and such which I believe have enormous potential in terms of making the
-system easier to explain, as well as understand.  
-
----
-
-## KEY CONCEPTS
-- OBJECT - a string representing anything that is representable with a string of
-characters (a game, a movie, a person, a song, a place, a video, a topic,
-a word, a book, a number, a brand, a post, an event, an item, a website, an app,
-a quote, an action, a movement or **literally** anything else)  
-- DATE - a date (UTC) for which we want to calculate the RDV for  
-- RDV - a positive integer representing the level/significance/rarity of a
-reminder for a certain OBJECT on a specific DATE  
-
-**(New feature of version 2.0)**  
-- RDVT - one of an infinite number of random moments in a day (0-24h UTC) when
-an object has its reminders for that day, allows for infinite precission  
-- RANK - RDVT rank, ranked 0 (most significant) to infinity - RDVT0, RDVT1...  
-
-## RDV CALCULATION
-`RDV = number of leading zero bits in blake3::keyed_hash(key: DATE, data: OBJECT)`  
-Note: The previous version (1.0) used a different algorithm, so the RDV values
-between the two versions have changed and are completely un-correlated.  
-By implementing this change, I've eliminated 2/3 blake3 hash calculations and
-improved performance (not that it mattered).  
-But now I can calculate about 10 million RDV values per second on my PC.  
-I have strong reasons to believe such major changes won't be happening in the
-future and that this is the final version of the algorithm.  
-It was still a good time to do such a fundamental change to the algorithm, since
-RANDEVU had essentially no adoption apart from myself and a small community I'm
-a part of.  
-
-## HOW IT WORKS AND POTENTIAL USE CASES
-Imagine a system that assigns a special number (RDV) to every object each day.  
-The number assigned to each object is different for each object and changes
-daily.  
-The number has a 50% chance to be 0, 25% chance to be 1, 12.5% to be 2, and so
-on (each number being twice as rare).  
-I've based everything around base-2 (simplest numerical base after unary), it
-makes everything fit together so perfectly (you'll probably see why when you
-learn more about how the system works).  
-By making each reminder level twice as rare - we can achive effectively
-infinitely infrequent reminders, as well as daily ones, and a pretty good range
-of reminders of various frequencies in between.  
-If an object has a reminder RDV4, that also implies RDV3, RDV2, RDV1 and RDV0.  
-Users can then choose to set a threshold value for each object and if the RDV
-value for a specific object is greater than or equal to the threshold - the user
-may decide to do something with that object.  
-For example, one may decide to watch a certain video once its RDV value (RDV
-value for that specific video) hits their desired threshold.  
-Threshold allows one to decide how often they would like to be "reminded of" a
-certain object.  
-0 -> every day, 1 -> every 2 days (on average - it's random), 2 -> 4 days, 3 ->
-8 days, and so on (allows for essentially infinite frequencies of reminders,
-though ones above 10 happen quite rarely - 2^10 = 1024 days).  
-If multiple people used this system to get reminded of the same things - they
-would all get reminded of them on the same days and thus be able to coordinate
-meetings/actions related to the objects in question.  
-This could allow fans of a "dead" game (game with no or little players online)
-to all meet and play it on the same day, let's say once every 256 days.  
-People could re-watch their favorite movies or videos and discuss them with
-other fellow fans on the same days.  
-This system can be applied to anything.  
-It can be used to assign special appreciation/remembrance days to your favorite
-books, songs, artists, events, or (as I already said) - ANYTHING.  
-One could have a huge list of objects they care about and never again risk
-forgetting any of them - since they will be reminded of them eventually (for
-example - bookmarks).  
-
-## RDVT CALCULATION AND USE CASES
-RDVT is a newly added (version 2.0) feature of the RANDEVU system and an
-optional extension of the RDV algorithm.  
-We calculate the hash the same way as for RDV, except we append a RANK integer
-to the DATE inside the key, separated by an '_'. And we don't count leading zero
-bits.  
-Instead, we iterate over the bits in the hash and add increments to the RDVT
-time (which starts at 00:00h, midnight). For each 1 we add an increment, and do
-nothing if the bit is 0.  
-An increment starts at 12h, and we divide it by half after processing each bit.  
-For example, if the first 4 bits are 0110 - this will result in a time value of
-09:00h (0 * 12h + 1 * 6h + 1 * 3h + 0 * 1.5h...).  
-Note that there are 256 bits and we keep doing this until we reach 1 ns (or
-millisecond/microsecond, depending on the implementation).  
-This means we get a different uniform pseudorandom time (0-24h) for each RANK.  
-If users find the daily RDV reminder too broad and would like a more specific
-time for the reminder - they can calculate one or more RDVT times and choose
-one.  
-Since RDVT0 is the most important/main time, users should choose the
-lowest-ranked RDVT that works for them - this increases the chances other people
-will also choose the same RDVT time as them, thus increasing the chances of an
-interaction.  
-Let's say a certain YouTube video has an RDV10 today. We could have a browser
-extension or a website that would schedule streams (like video premieres) for
-that video at the first 10 RDVT times (RDVT0-9).  
-Fans of that video could all come re-watch it live with others at one of the
-RDVT times, and perhaps chat about it in the live chat (assuming the feature
-existed) while experiencing it together.  
-This is just one super specific hypothetical use case I came up with.  
-
----
-
-## OBJECT NAMING CONVENTION (non-exhaustive examples)
-OBJECT is a string (preferably uppercase A-Z, 0-9). No spaces allowed.  
-Spaces and any other characters should be replaced with a single underscore
-('_').  
-Characters outside of this set should only be used for external identifiers that
-are case-sensitive or contain other symbols, for example, YOUTUBE video IDs.  
-
-```
-XONOTIC (all letters should be uppercase)
-
-STAR_WARS (spaces and dashes in multi-word objects should be replaced with _)
-
-THE_MATRIX_1999 (movies should have a year of release at the end)
-
-GRAND_THEFT_AUTO_5 (objects should be referenced by their full name, Roman
-numerals should be replaced with Arabic ones)
-
-ASAP_ROCKY ($ should be replaced with S, same for other similar instances)
-
-C_PLUS_PLUS (++ should be replaced with _PLUS_PLUS)
-
-C_SHARP (# should be replaced with _SHARP, in other contexts it could be _HASH
-or omitted)
-
-YEAR_2000 (years should have a YEAR_ prefix)
-
-FRIDAY (weekdays and months should not be abbreviated, same as all other
-objects)
-
-2023-08-25 (dates should be in ISO 8601 format, YYYY-MM-DD)
-
-NO_MANS_SKY (apostrophe in MAN'S should be dropped)
-
-HARRY_POTTER_SMOKES_WEED_Cdfkq2Nmb3c (video ID should be appended to the video
-title, double underscore is fine if the ID starts with one, IDs are allowed to
-use dashes and lowercase letters)
-
-GETTING_BANGED_BY_GREEN_BOOMERS_MINECRAFT_BETA_1_7_3_SOLO_SURVIVAL_NO_COMMENTARY_OJzsmWBQE3I
-(brackets, quotation marks, colons, and other punctuation should be dropped,
-periods in version numbers like 1.7.3 should be replaced with _)
-
-NUMBER_69 (numbers should have a NUMBER_ prefix)
-
-```
-
-### WHY THIS VERY SPECIFIC AND STRICT CONVENTION THO?
-
-**TO MAKE SURE EVERYONE GETS THE SAME REMINDERS FOR THE SAME THINGS ON THE SAME**
-**DAYS.**  
-
-Due to how the algorithm works - even just a single character difference between
-two objects causes the system to generate completely different reminders for
-each.  
-For example: WEED, weed, Weed, and W33D would all be treated as different and
-independent objects with completely unrelated reminders.  
-One can think of objects like passwords - the same password gets you the same
-reminders as everyone else using said password.  
-If one wanted to get completely different reminders from other people for a
-specific object - they could append extra characters to it.  
-However, this is not the focus of the system. The whole point is to help people
-coordinate getting reminded about stuff at the same time as everyone else.  
+Metadata-Version: 2.1
+Name: randevu
+Version: 2.0.1
+Summary: The official Python implementation of the RANDEVU algorithm
+Author: TypicalHog
+License: This work is released into the public domain with The Unlicense.
+        Alternatively, it is licensed under MIT License or Apache License 2.0.
+        
+        ---
+        
+        The Unlicense
+        
+        This is free and unencumbered software released into the public domain.
+        
+        Anyone is free to copy, modify, publish, use, compile, sell, or
+        distribute this software, either in source code form or as a compiled
+        binary, for any purpose, commercial or non-commercial, and by any
+        means.
+        
+        In jurisdictions that recognize copyright laws, the author or authors
+        of this software dedicate any and all copyright interest in the
+        software to the public domain. We make this dedication for the benefit
+        of the public at large and to the detriment of our heirs and
+        successors. We intend this dedication to be an overt act of
+        relinquishment in perpetuity of all present and future rights to this
+        software under copyright law.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+        OTHER DEALINGS IN THE SOFTWARE.
+        
+        For more information, please refer to <http://unlicense.org/>
+        
+        ---
+        
+        MIT License
+        
+        Copyright (c) 2024 TypicalHog
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of
+        this software and associated documentation files (the "Software"), to deal in
+        the Software without restriction, including without limitation the rights to
+        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+        the Software, and to permit persons to whom the Software is furnished to do so,
+        subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+        FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+        COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+        IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+        CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+        ---
+        
+        Apache License 2.0
+        
+        Copyright (c) 2024 TypicalHog
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+        http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+        
+Project-URL: Homepage, https://github.com/TypicalHog/randevu-py
+Project-URL: Issues, https://github.com/TypicalHog/randevu-py/issues
+Keywords: randevu,rdv,rdvt,universal,daily,reminder,coordination,blake3
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: blake3>=0.4.1
+
+# RANDEVU
+**Universal Probabilistic Daily Reminder Coordination System for Anything**  
+
+- UNIVERSAL - reminders for the same object are the same for everyone  
+- PROBABILISTIC - reminders are calculated using a simple probabilistic
+algorithm based on powers of 2  
+- DAILY - reminders are following a daily schedule/interval (UTC)  
+- INTRADAY - infinite optional intraday reminder times (RDVT - added in version
+2.0 as an extension to the existing system)  
+- GENERIC - applicable to anything and everything, literally (where it makes
+sense, see use cases)  
+- FOSS - in the public domain (Unlicense or MIT or Apache-2.0)  
+- OFFLINE - no internet connection required  
+- PORTABLE - simple code, easy to port anywhere where blake3 is available  
+- DETERMINISTIC - easily computable and predictable for any object and any date  
+- PSEUDORANDOM - reminders are spaced randomly and uniformly  
+- ADJUSTABLE - user can decide how frequently (roughly) they'd like to see
+reminders for each object  
+
+https://github.com/TypicalHog/randevu (Rust - **REFERENCE IMPLEMENTATION**)  
+https://github.com/TypicalHog/randevu-ts (TypeScript)  
+**https://github.com/TypicalHog/randevu-py (Python)**  
+The above implementations are available on Crates.io, PyPI, and npm as **randevu**.  
+Feel free to contribute, create an implementation in another (missing) language,
+or even an alternative one for 1 (or more) of the 3 languages I've already
+created a repository and crate/module/package for.  
+
+## EXAMPLE USAGE
+```python
+from datetime import datetime
+from randevu import rdv, rdvt
+
+object = "THE_SIMPSONS"
+date = datetime.now().date()
+rdv_value = rdv(object, date)
+rdvt_value = rdvt(0, object, date)
+
+print(f"Object {object} has RDV{rdv_value} today with RDVT0 at {rdvt_value}")
+
+```
+
+---
+
+**I'm aware of the fact that README.md is a confusing jungle of words, random**
+**thoughts, and ideas. (Will work on it)**  
+I kinda suck at explaining stuff and structuring text in an organized manner.
+I'm sorry about that. :/  
+I gave it my best, and I'll keep trying to improve it in the future.  
+This whole document will probably be revamped entirely. Stuff will be explained
+better, irrelevant things, tangents, thoughts and rambles removed, etc.  
+I would also like to write something like a proper spec for the RANDEVU
+algorithm/system.  
+I'm thinking about creating a FAQ section/document where I'll explain various
+aspects of the system and anything else I'd like to clarify or expand on in more
+detail.  
+Also thinking about adding some visual analogies (infographics) with coin
+tossing and such which I believe have enormous potential in terms of making the
+system easier to explain, as well as understand.  
+
+---
+
+## KEY CONCEPTS
+- OBJECT - a string representing anything that is representable with a string of
+characters (a game, a movie, a person, a song, a place, a video, a topic,
+a word, a book, a number, a brand, a post, an event, an item, a website, an app,
+a quote, an action, a movement or **literally** anything else)  
+- DATE - a date (UTC) for which we want to calculate the RDV for  
+- RDV - a positive integer representing the level/significance/rarity of a
+reminder for a certain OBJECT on a specific DATE  
+
+**(New feature of version 2.0)**  
+- RDVT - one of an infinite number of random moments in a day (0-24h UTC) when
+an object has its reminders for that day, allows for infinite precission  
+- RANK - RDVT rank, ranked 0 (most significant) to infinity - RDVT0, RDVT1...  
+
+## RDV CALCULATION
+`RDV = number of leading zero bits in blake3::keyed_hash(key: DATE, data: OBJECT)`  
+Note: The previous version (1.0) used a different algorithm, so the RDV values
+between the two versions have changed and are completely un-correlated.  
+By implementing this change, I've eliminated 2/3 blake3 hash calculations and
+improved performance (not that it mattered).  
+But now I can calculate about 10 million RDV values per second on my PC.  
+I have strong reasons to believe such major changes won't be happening in the
+future and that this is the final version of the algorithm.  
+It was still a good time to do such a fundamental change to the algorithm, since
+RANDEVU had essentially no adoption apart from myself and a small community I'm
+a part of.  
+
+## HOW IT WORKS AND POTENTIAL USE CASES
+Imagine a system that assigns a special number (RDV) to every object each day.  
+The number assigned to each object is different for each object and changes
+daily.  
+The number has a 50% chance to be 0, 25% chance to be 1, 12.5% to be 2, and so
+on (each number being twice as rare).  
+I've based everything around base-2 (simplest numerical base after unary), it
+makes everything fit together so perfectly (you'll probably see why when you
+learn more about how the system works).  
+By making each reminder level twice as rare - we can achive effectively
+infinitely infrequent reminders, as well as daily ones, and a pretty good range
+of reminders of various frequencies in between.  
+If an object has a reminder RDV4, that also implies RDV3, RDV2, RDV1 and RDV0.  
+Users can then choose to set a threshold value for each object and if the RDV
+value for a specific object is greater than or equal to the threshold - the user
+may decide to do something with that object.  
+For example, one may decide to watch a certain video once its RDV value (RDV
+value for that specific video) hits their desired threshold.  
+Threshold allows one to decide how often they would like to be "reminded of" a
+certain object.  
+0 -> every day, 1 -> every 2 days (on average - it's random), 2 -> 4 days, 3 ->
+8 days, and so on (allows for essentially infinite frequencies of reminders,
+though ones above 10 happen quite rarely - 2^10 = 1024 days).  
+If multiple people used this system to get reminded of the same things - they
+would all get reminded of them on the same days and thus be able to coordinate
+meetings/actions related to the objects in question.  
+This could allow fans of a "dead" game (game with no or little players online)
+to all meet and play it on the same day, let's say once every 256 days.  
+People could re-watch their favorite movies or videos and discuss them with
+other fellow fans on the same days.  
+This system can be applied to anything.  
+It can be used to assign special appreciation/remembrance days to your favorite
+books, songs, artists, events, or (as I already said) - ANYTHING.  
+One could have a huge list of objects they care about and never again risk
+forgetting any of them - since they will be reminded of them eventually (for
+example - bookmarks).  
+
+## RDVT CALCULATION AND USE CASES
+RDVT is a newly added (version 2.0) feature of the RANDEVU system and an
+optional extension of the RDV algorithm.  
+We calculate the hash the same way as for RDV, except we append a RANK integer
+to the DATE inside the key, separated by an '_'. And we don't count leading zero
+bits.  
+Instead, we iterate over the bits in the hash and add increments to the RDVT
+time (which starts at 00:00h, midnight). For each 1 we add an increment, and do
+nothing if the bit is 0.  
+An increment starts at 12h, and we divide it by half after processing each bit.  
+For example, if the first 4 bits are 0110 - this will result in a time value of
+09:00h (0 * 12h + 1 * 6h + 1 * 3h + 0 * 1.5h...).  
+Note that there are 256 bits and we keep doing this until we reach 1 ns (or
+millisecond/microsecond, depending on the implementation).  
+This means we get a different uniform pseudorandom time (0-24h) for each RANK.  
+If users find the daily RDV reminder too broad and would like a more specific
+time for the reminder - they can calculate one or more RDVT times and choose
+one.  
+Since RDVT0 is the most important/main time, users should choose the
+lowest-ranked RDVT that works for them - this increases the chances other people
+will also choose the same RDVT time as them, thus increasing the chances of an
+interaction.  
+Let's say a certain YouTube video has an RDV10 today. We could have a browser
+extension or a website that would schedule streams (like video premieres) for
+that video at the first 10 RDVT times (RDVT0-9).  
+Fans of that video could all come re-watch it live with others at one of the
+RDVT times, and perhaps chat about it in the live chat (assuming the feature
+existed) while experiencing it together.  
+This is just one super specific hypothetical use case I came up with.  
+
+---
+
+## OBJECT NAMING CONVENTION (non-exhaustive examples)
+OBJECT is a string (preferably uppercase A-Z, 0-9). No spaces allowed.  
+Spaces and any other characters should be replaced with a single underscore
+('_').  
+Characters outside of this set should only be used for external identifiers that
+are case-sensitive or contain other symbols, for example, YOUTUBE video IDs.  
+
+```
+XONOTIC (all letters should be uppercase)
+
+STAR_WARS (spaces and dashes in multi-word objects should be replaced with _)
+
+THE_MATRIX_1999 (movies should have a year of release at the end)
+
+GRAND_THEFT_AUTO_5 (objects should be referenced by their full name, Roman
+numerals should be replaced with Arabic ones)
+
+ASAP_ROCKY ($ should be replaced with S, same for other similar instances)
+
+C_PLUS_PLUS (++ should be replaced with _PLUS_PLUS)
+
+C_SHARP (# should be replaced with _SHARP, in other contexts it could be _HASH
+or omitted)
+
+YEAR_2000 (years should have a YEAR_ prefix)
+
+FRIDAY (weekdays and months should not be abbreviated, same as all other
+objects)
+
+2023-08-25 (dates should be in ISO 8601 format, YYYY-MM-DD)
+
+NO_MANS_SKY (apostrophe in MAN'S should be dropped)
+
+HARRY_POTTER_SMOKES_WEED_Cdfkq2Nmb3c (video ID should be appended to the video
+title, double underscore is fine if the ID starts with one, IDs are allowed to
+use dashes and lowercase letters)
+
+GETTING_BANGED_BY_GREEN_BOOMERS_MINECRAFT_BETA_1_7_3_SOLO_SURVIVAL_NO_COMMENTARY_OJzsmWBQE3I
+(brackets, quotation marks, colons, and other punctuation should be dropped,
+periods in version numbers like 1.7.3 should be replaced with _)
+
+NUMBER_69 (numbers should have a NUMBER_ prefix)
+
+```
+
+### WHY THIS VERY SPECIFIC AND STRICT CONVENTION THO?
+
+**TO MAKE SURE EVERYONE GETS THE SAME REMINDERS FOR THE SAME THINGS ON THE SAME**
+**DAYS.**  
+
+Due to how the algorithm works - even just a single character difference between
+two objects causes the system to generate completely different reminders for
+each.  
+For example: WEED, weed, Weed, and W33D would all be treated as different and
+independent objects with completely unrelated reminders.  
+One can think of objects like passwords - the same password gets you the same
+reminders as everyone else using said password.  
+If one wanted to get completely different reminders from other people for a
+specific object - they could append extra characters to it.  
+However, this is not the focus of the system. The whole point is to help people
+coordinate getting reminded about stuff at the same time as everyone else.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `randevu-2.0.0/randevu.egg-info/PKG-INFO` & `randevu-2.0.1/src/randevu.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,97 @@
 Metadata-Version: 2.1
 Name: randevu
-Version: 2.0.0
+Version: 2.0.1
 Summary: The official Python implementation of the RANDEVU algorithm
-Home-page: https://github.com/TypicalHog/randevu-py
 Author: TypicalHog
+License: This work is released into the public domain with The Unlicense.
+        Alternatively, it is licensed under MIT License or Apache License 2.0.
+        
+        ---
+        
+        The Unlicense
+        
+        This is free and unencumbered software released into the public domain.
+        
+        Anyone is free to copy, modify, publish, use, compile, sell, or
+        distribute this software, either in source code form or as a compiled
+        binary, for any purpose, commercial or non-commercial, and by any
+        means.
+        
+        In jurisdictions that recognize copyright laws, the author or authors
+        of this software dedicate any and all copyright interest in the
+        software to the public domain. We make this dedication for the benefit
+        of the public at large and to the detriment of our heirs and
+        successors. We intend this dedication to be an overt act of
+        relinquishment in perpetuity of all present and future rights to this
+        software under copyright law.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+        OTHER DEALINGS IN THE SOFTWARE.
+        
+        For more information, please refer to <http://unlicense.org/>
+        
+        ---
+        
+        MIT License
+        
+        Copyright (c) 2024 TypicalHog
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of
+        this software and associated documentation files (the "Software"), to deal in
+        the Software without restriction, including without limitation the rights to
+        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+        the Software, and to permit persons to whom the Software is furnished to do so,
+        subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+        FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+        COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+        IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+        CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+        ---
+        
+        Apache License 2.0
+        
+        Copyright (c) 2024 TypicalHog
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+        http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+        
 Project-URL: Homepage, https://github.com/TypicalHog/randevu-py
 Project-URL: Issues, https://github.com/TypicalHog/randevu-py/issues
+Keywords: randevu,rdv,rdvt,universal,daily,reminder,coordination,blake3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
+Requires-Dist: blake3>=0.4.1
 
 # RANDEVU
 **Universal Probabilistic Daily Reminder Coordination System for Anything**  
 
 - UNIVERSAL - reminders for the same object are the same for everyone  
 - PROBABILISTIC - reminders are calculated using a simple probabilistic
 algorithm based on powers of 2  
@@ -31,16 +105,16 @@
 - PORTABLE - simple code, easy to port anywhere where blake3 is available  
 - DETERMINISTIC - easily computable and predictable for any object and any date  
 - PSEUDORANDOM - reminders are spaced randomly and uniformly  
 - ADJUSTABLE - user can decide how frequently (roughly) they'd like to see
 reminders for each object  
 
 https://github.com/TypicalHog/randevu (Rust - **REFERENCE IMPLEMENTATION**)  
-https://github.com/TypicalHog/randevu-ts (TypeScript)  
-**https://github.com/TypicalHog/randevu-py (Python)**  
+https://github.com/TypicalHog/randevu-ts (TypeScript)  
+**https://github.com/TypicalHog/randevu-py (Python)**  
 The above implementations are available on Crates.io, PyPI, and npm as **randevu**.  
 Feel free to contribute, create an implementation in another (missing) language,
 or even an alternative one for 1 (or more) of the 3 languages I've already
 created a repository and crate/module/package for.  
 
 ## EXAMPLE USAGE
 ```python
@@ -55,15 +129,15 @@
 print(f"Object {object} has RDV{rdv_value} today with RDVT0 at {rdvt_value}")
 
 ```
 
 ---
 
 **I'm aware of the fact that README.md is a confusing jungle of words, random**
-**thoughts, and ideas. (Will work on it)**  
+**thoughts, and ideas. (Will work on it)**  
 I kinda suck at explaining stuff and structuring text in an organized manner.
 I'm sorry about that. :/  
 I gave it my best, and I'll keep trying to improve it in the future.  
 This whole document will probably be revamped entirely. Stuff will be explained
 better, irrelevant things, tangents, thoughts and rambles removed, etc.  
 I would also like to write something like a proper spec for the RANDEVU
 algorithm/system.  
@@ -76,110 +150,110 @@
 
 ---
 
 ## KEY CONCEPTS
 - OBJECT - a string representing anything that is representable with a string of
 characters (a game, a movie, a person, a song, a place, a video, a topic,
 a word, a book, a number, a brand, a post, an event, an item, a website, an app,
-a quote, an action, a movement or **literally** anything else)  
+a quote, an action, a movement or **literally** anything else)  
 - DATE - a date (UTC) for which we want to calculate the RDV for  
 - RDV - a positive integer representing the level/significance/rarity of a
-reminder for a certain OBJECT on a specific DATE  
+reminder for a certain OBJECT on a specific DATE  
 
-**(New feature of version 2.0)**  
+**(New feature of version 2.0)**  
 - RDVT - one of an infinite number of random moments in a day (0-24h UTC) when
-an object has its reminders for that day, allows for infinite precission  
-- RANK - RDVT rank, ranked 0 (most significant) to infinity - RDVT0, RDVT1...  
+an object has its reminders for that day, allows for infinite precission  
+- RANK - RDVT rank, ranked 0 (most significant) to infinity - RDVT0, RDVT1...  
 
 ## RDV CALCULATION
-`RDV = number of leading zero bits in blake3::keyed_hash(key: DATE, data: OBJECT)`  
+`RDV = number of leading zero bits in blake3::keyed_hash(key: DATE, data: OBJECT)`  
 Note: The previous version (1.0) used a different algorithm, so the RDV values
-between the two versions have changed and are completely un-correlated.  
+between the two versions have changed and are completely un-correlated.  
 By implementing this change, I've eliminated 2/3 blake3 hash calculations and
-improved performance (not that it mattered).  
+improved performance (not that it mattered).  
 But now I can calculate about 10 million RDV values per second on my PC.  
 I have strong reasons to believe such major changes won't be happening in the
-future and that this is the final version of the algorithm.  
+future and that this is the final version of the algorithm.  
 It was still a good time to do such a fundamental change to the algorithm, since
 RANDEVU had essentially no adoption apart from myself and a small community I'm
-a part of.  
+a part of.  
 
 ## HOW IT WORKS AND POTENTIAL USE CASES
-Imagine a system that assigns a special number (RDV) to every object each day.  
+Imagine a system that assigns a special number (RDV) to every object each day.  
 The number assigned to each object is different for each object and changes
-daily.  
+daily.  
 The number has a 50% chance to be 0, 25% chance to be 1, 12.5% to be 2, and so
-on (each number being twice as rare).  
+on (each number being twice as rare).  
 I've based everything around base-2 (simplest numerical base after unary), it
 makes everything fit together so perfectly (you'll probably see why when you
 learn more about how the system works).  
 By making each reminder level twice as rare - we can achive effectively
 infinitely infrequent reminders, as well as daily ones, and a pretty good range
 of reminders of various frequencies in between.  
-If an object has a reminder RDV4, that also implies RDV3, RDV2, RDV1 and RDV0.  
+If an object has a reminder RDV4, that also implies RDV3, RDV2, RDV1 and RDV0.  
 Users can then choose to set a threshold value for each object and if the RDV
 value for a specific object is greater than or equal to the threshold - the user
-may decide to do something with that object.  
+may decide to do something with that object.  
 For example, one may decide to watch a certain video once its RDV value (RDV
-value for that specific video) hits their desired threshold.  
+value for that specific video) hits their desired threshold.  
 Threshold allows one to decide how often they would like to be "reminded of" a
-certain object.  
+certain object.  
 0 -> every day, 1 -> every 2 days (on average - it's random), 2 -> 4 days, 3 ->
 8 days, and so on (allows for essentially infinite frequencies of reminders,
-though ones above 10 happen quite rarely - 2^10 = 1024 days).  
+though ones above 10 happen quite rarely - 2^10 = 1024 days).  
 If multiple people used this system to get reminded of the same things - they
 would all get reminded of them on the same days and thus be able to coordinate
-meetings/actions related to the objects in question.  
+meetings/actions related to the objects in question.  
 This could allow fans of a "dead" game (game with no or little players online)
 to all meet and play it on the same day, let's say once every 256 days.  
 People could re-watch their favorite movies or videos and discuss them with
-other fellow fans on the same days.  
-This system can be applied to anything.  
+other fellow fans on the same days.  
+This system can be applied to anything.  
 It can be used to assign special appreciation/remembrance days to your favorite
-books, songs, artists, events, or (as I already said) - ANYTHING.  
+books, songs, artists, events, or (as I already said) - ANYTHING.  
 One could have a huge list of objects they care about and never again risk
 forgetting any of them - since they will be reminded of them eventually (for
-example - bookmarks).  
+example - bookmarks).  
 
 ## RDVT CALCULATION AND USE CASES
 RDVT is a newly added (version 2.0) feature of the RANDEVU system and an
-optional extension of the RDV algorithm.  
+optional extension of the RDV algorithm.  
 We calculate the hash the same way as for RDV, except we append a RANK integer
 to the DATE inside the key, separated by an '_'. And we don't count leading zero
-bits.  
+bits.  
 Instead, we iterate over the bits in the hash and add increments to the RDVT
 time (which starts at 00:00h, midnight). For each 1 we add an increment, and do
 nothing if the bit is 0.  
 An increment starts at 12h, and we divide it by half after processing each bit.  
 For example, if the first 4 bits are 0110 - this will result in a time value of
 09:00h (0 * 12h + 1 * 6h + 1 * 3h + 0 * 1.5h...).  
 Note that there are 256 bits and we keep doing this until we reach 1 ns (or
 millisecond/microsecond, depending on the implementation).  
-This means we get a different uniform pseudorandom time (0-24h) for each RANK.  
+This means we get a different uniform pseudorandom time (0-24h) for each RANK.  
 If users find the daily RDV reminder too broad and would like a more specific
 time for the reminder - they can calculate one or more RDVT times and choose
 one.  
 Since RDVT0 is the most important/main time, users should choose the
 lowest-ranked RDVT that works for them - this increases the chances other people
 will also choose the same RDVT time as them, thus increasing the chances of an
-interaction.  
+interaction.  
 Let's say a certain YouTube video has an RDV10 today. We could have a browser
 extension or a website that would schedule streams (like video premieres) for
 that video at the first 10 RDVT times (RDVT0-9).  
 Fans of that video could all come re-watch it live with others at one of the
 RDVT times, and perhaps chat about it in the live chat (assuming the feature
 existed) while experiencing it together.  
-This is just one super specific hypothetical use case I came up with.  
+This is just one super specific hypothetical use case I came up with.  
 
 ---
 
 ## OBJECT NAMING CONVENTION (non-exhaustive examples)
-OBJECT is a string (preferably uppercase A-Z, 0-9). No spaces allowed.  
+OBJECT is a string (preferably uppercase A-Z, 0-9). No spaces allowed.  
 Spaces and any other characters should be replaced with a single underscore
-('_').  
+('_').  
 Characters outside of this set should only be used for external identifiers that
 are case-sensitive or contain other symbols, for example, YOUTUBE video IDs.  
 
 ```
 XONOTIC (all letters should be uppercase)
 
 STAR_WARS (spaces and dashes in multi-word objects should be replaced with _)
@@ -220,16 +294,16 @@
 ### WHY THIS VERY SPECIFIC AND STRICT CONVENTION THO?
 
 **TO MAKE SURE EVERYONE GETS THE SAME REMINDERS FOR THE SAME THINGS ON THE SAME**
 **DAYS.**  
 
 Due to how the algorithm works - even just a single character difference between
 two objects causes the system to generate completely different reminders for
-each.  
+each.  
 For example: WEED, weed, Weed, and W33D would all be treated as different and
-independent objects with completely unrelated reminders.  
+independent objects with completely unrelated reminders.  
 One can think of objects like passwords - the same password gets you the same
-reminders as everyone else using said password.  
+reminders as everyone else using said password.  
 If one wanted to get completely different reminders from other people for a
-specific object - they could append extra characters to it.  
+specific object - they could append extra characters to it.  
 However, this is not the focus of the system. The whole point is to help people
 coordinate getting reminded about stuff at the same time as everyone else.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

