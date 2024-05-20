# Comparing `tmp/fast_flights-0.2.tar.gz` & `tmp/fast_flights-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_flights-0.2.tar", last modified: Mon May 13 10:25:37 2024, max compression
+gzip compressed data, was "fast_flights-0.3.tar", last modified: Mon May 20 08:33:24 2024, max compression
```

## Comparing `fast_flights-0.2.tar` & `fast_flights-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:37.917029 fast_flights-0.2/
--rw-rw-rw-   0        0        0     7501 2024-05-13 10:25:37.917029 fast_flights-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6770 2024-05-13 10:18:38.000000 fast_flights-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:37.838833 fast_flights-0.2/fast_flights/
--rw-rw-rw-   0        0        0      389 2024-05-13 10:24:57.000000 fast_flights-0.2/fast_flights/__init__.py
--rw-rw-rw-   0        0        0   116049 2024-05-12 14:47:32.000000 fast_flights-0.2/fast_flights/_generated_enum.py
--rw-rw-rw-   0        0        0     2920 2024-05-12 15:02:16.000000 fast_flights-0.2/fast_flights/core.py
--rw-rw-rw-   0        0        0      769 2024-05-13 10:25:00.000000 fast_flights-0.2/fast_flights/filter.py
--rw-rw-rw-   0        0        0     4625 2024-05-13 10:25:00.000000 fast_flights-0.2/fast_flights/flights_impl.py
--rw-rw-rw-   0        0        0     2246 2024-05-12 13:57:26.000000 fast_flights-0.2/fast_flights/flights_pb2.py
--rw-rw-rw-   0        0        0      422 2024-05-12 13:57:26.000000 fast_flights-0.2/fast_flights/schema.py
--rw-rw-rw-   0        0        0      411 2024-05-13 10:24:47.000000 fast_flights-0.2/fast_flights/search.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:37.914945 fast_flights-0.2/fast_flights.egg-info/
--rw-rw-rw-   0        0        0     7501 2024-05-13 10:25:37.000000 fast_flights-0.2/fast_flights.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-05-13 10:25:37.000000 fast_flights-0.2/fast_flights.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 10:25:37.000000 fast_flights-0.2/fast_flights.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-13 10:25:37.000000 fast_flights-0.2/fast_flights.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-13 10:25:37.000000 fast_flights-0.2/fast_flights.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      946 2024-05-13 10:25:19.000000 fast_flights-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 10:25:37.917029 fast_flights-0.2/setup.cfg
--rw-rw-rw-   0        0        0       73 2024-05-12 15:08:19.000000 fast_flights-0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 08:33:24.870207 fast_flights-0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     7315 2024-05-20 08:33:24.870207 fast_flights-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     6613 2024-05-20 08:27:08.000000 fast_flights-0.3/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 08:33:24.870207 fast_flights-0.3/fast_flights/
+-rw-r--r--   0 runner    (1000) runner    (1000)      372 2024-05-20 08:27:08.000000 fast_flights-0.3/fast_flights/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   116049 2024-05-20 08:27:08.000000 fast_flights-0.3/fast_flights/_generated_enum.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2888 2024-05-20 08:28:29.000000 fast_flights-0.3/fast_flights/core.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      747 2024-05-20 08:27:08.000000 fast_flights-0.3/fast_flights/filter.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4467 2024-05-20 08:27:08.000000 fast_flights-0.3/fast_flights/flights_impl.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2209 2024-05-20 08:27:08.000000 fast_flights-0.3/fast_flights/flights_pb2.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      400 2024-05-20 08:27:08.000000 fast_flights-0.3/fast_flights/schema.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      393 2024-05-20 08:27:08.000000 fast_flights-0.3/fast_flights/search.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-20 08:33:24.870207 fast_flights-0.3/fast_flights.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     7315 2024-05-20 08:33:24.000000 fast_flights-0.3/fast_flights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      416 2024-05-20 08:33:24.000000 fast_flights-0.3/fast_flights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-20 08:33:24.000000 fast_flights-0.3/fast_flights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-05-20 08:33:24.000000 fast_flights-0.3/fast_flights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2024-05-20 08:33:24.000000 fast_flights-0.3/fast_flights.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      901 2024-05-20 08:33:04.000000 fast_flights-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-20 08:33:24.870207 fast_flights-0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)       69 2024-05-20 08:27:08.000000 fast_flights-0.3/setup.py
```

### Comparing `fast_flights-0.2/PKG-INFO` & `fast_flights-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-Metadata-Version: 2.1
-Name: fast-flights
-Version: 0.2
-Summary: The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python.
-Author-email: AWeirdDev <aweirdscratcher@gmail.com>
-Project-URL: Homepage, https://github.com/AWeirdScratcher/flights
-Project-URL: Bug Tracker, https://github.com/AWeirdScratcher/flights/issues
-Keywords: flights,google,google-flights,scraper,protobuf,travel,trip,passengers,airport
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: protobuf
-Requires-Dist: selectolax
-
-<div align="center">
-
-# flights (fast-flights)
-
-The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python. Based on Base64-encoded Protobuf string.
-
-```haskell
-$ pip install fast-flights
-```
-
-</div>
-
-## Usage
-
-To use `fast-flights`, you'll first create a filter (inherited from `?tfs=`) to perform a request.
-Then, add `flight_data`, `trip`, `seat` and `passengers` info to use the API directly.
-
-Honorable mention: I like birds. Yes, I like birds.
-
-```python
-from fast_flights import FlightData, Passengers, create_filter, get_flights
-
-# Create a new filter
-filter = create_filter(
-    flight_data=[
-        # Include more if it's not a one-way trip
-        FlightData(
-            date="2024-07-02",  # Date of departure
-            from_airport="TPE", 
-            to_airport="MYJ"
-        ),
-        # ... include more for round trips and multi-city trips
-    ],
-    trip="one-way",  # Trip (round-trip, one-way, multi-city)
-    seat="economy",  # Seat (economy, premium economy, business or first)
-    passengers=Passengers(
-        adults=2,
-        children=1,
-        infants_in_seat=0,
-        infants_on_lap=0
-    ),
-)
-
-# Get flights with a filter
-result = get_flights(filter)
-
-# The price is currently... low/typical/high
-print("The price is currently", result.current_price)
-
-# Display the first flight
-print(result.flights[0])
-```
-
-Additionally, you can use the `Airport` enum to search for airports in code (as you type)! (See `_generated_enum.py` in source)
-
-```python
-Airport.TAIPEI
-              |---------------------------------|
-              | TAIPEI_SONGSHAN_AIRPORT         |
-              | TAPACHULA_INTERNATIONAL_AIRPORT |
-              | TAMPA_INTERNATIONAL_AIRPORT     |
-              | ... 5 more                      |
-              |---------------------------------|
-```
-
-## How it's made
-
-The other day, I was making a chat-interface-based trip recommendation app and wanted to add a feature that can search for flights available for booking. My personal choice is definitely [Google Flights](https://flights.google.com) since Google always has the best and most organized data on the web. Therefore, I searched for APIs on Google.
-
-> 🔎 **Search** <br />
-> google flights api
-
-The results? Bad. It seems like they discontinued this service and it now lives in the Graveyard of Google.
-
-> <sup><a href="https://duffel.com/blog/google-flights-api" target="_blank">🧏‍♂️ <b>duffel.com</b></a></sup><br />
-> <sup><i>Google Flights API: How did it work & what happened to it?</i></b>
->
-> The Google Flights API offered developers access to aggregated airline data, including flight times, availability, and prices. Over a decade ago, Google announced the acquisition of ITA Software Inc. which it used to develop its API. **However, in 2018, Google ended access to the public-facing API and now only offers access through the QPX enterprise product**.
-
-That's awful! I've also looked for free alternatives but their rate limits and pricing are just 😬 (not a good fit/deal for everyone).
-
-<br />
-
-However, Google Flights has their UI – [flights.google.com](https://flights.google.com). So, maybe I could just use Developer Tools to log the requests made and just replicate all of that? Undoubtedly not! Their requests are just full of numbers and unreadable text, so that's not the solution.
-
-Perhaps, we could scrape it? I mean, Google allowed many companies like [Serpapi](https://google.com/search?q=serpapi) to scrape their web just pretending like nothing happened... So let's scrape our own.
-
-> 🔎 **Search** <br />
-> google flights ~~api~~ scraper pypi
-
-Excluding the ones that are not active, I came across [hugoglvs/google-flights-scraper](https://pypi.org/project/google-flights-scraper) on Pypi. I thought to myself: "aint no way this is the solution!"
-
-I checked hugoglvs's code on [GitHub](https://github.com/hugoglvs/google-flights-scraper), and I immediately detected "playwright," my worst enemy. One word can describe it well: slow. Two words? Extremely slow. What's more, it doesn't even run on the **🗻 Edge** because of configuration errors, missing libraries... etc. I could just reverse [try.playwright.tech](https://try.playwright.tech) and use a better environment, but that's just too risky if they added Cloudflare as an additional security barrier 😳.
-
-Life tells me to never give up. Let's just take a look at their URL params...
-
-```markdown
-https://www.google.com/travel/flights/search?tfs=CBwQAhoeEgoyMDI0LTA1LTI4agcIARIDVFBFcgcIARIDTVlKGh4SCjIwMjQtMDUtMzBqBwgBEgNNWUpyBwgBEgNUUEVAAUgBcAGCAQsI____________AZgBAQ&hl=en
-```
-
-| Param | Content | My past understanding |
-|-------|---------|-----------------------|
-| hl    | en      | Sets the language.    |
-| tfs   | CBwQAhoeEgoyMDI0LTA1LTI4agcIARID… | What is this???? 🤮🤮 |
-
-I removed the `?tfs=` parameter and found out that this is the control of our request! And it looks so base64-y.
-
-If we decode it to raw text, we can still see the dates, but we're not quite there — there's too much unwanted Unicode text.
-
-Or maybe it's some kind of a **data-storing method** Google uses? What if it's something like JSON? Let's look it up.
-
-> 🔎 **Search** <br />
-> google's json alternative
-
-> 🐣 **Result**<br />
-> Solution: The Power of **Protocol Buffers**
-> 
-> LinkedIn turned to Protocol Buffers, often referred to as **protobuf**, a binary serialization format developed by Google. The key advantage of Protocol Buffers is its efficiency, compactness, and speed, making it significantly faster than JSON for serialization and deserialization.
-
-Gotcha, Protobuf! Let's feed it to an online decoder and see how it does:
-
-> 🔎 **Search** <br />
-> protobuf decoder
-
-> 🐣 **Result**<br />
-> [protobuf-decoder.netlify.app](https://protobuf-decoder.netlify.app)
-
-I then pasted the Base64-encoded string to the decoder and no way! It DID return valid data!
-
-![annotated, Protobuf Decoder screenshot](https://github.com/AWeirdDev/flights/assets/90096971/77dfb097-f961-4494-be88-3640763dbc8c)
-
-I immediately recognized the values — that's my data, that's my query!
-
-So, I wrote some simple Protobuf code to decode the data.
-
-```protobuf
-syntax = "proto3"
-
-message Airport {
-    string name = 2;
-}
-
-message FlightInfo {
-    string date = 2;
-    Airport dep_airport = 13;
-    Airport arr_airport = 14;
-}
-
-message GoogleSucks {
-    repeated FlightInfo = 3;
-}
-```
-
-It works! Now, I won't consider myself an "experienced Protobuf developer" but rather a complete beginner.
-
-I have no idea what I wrote but... it worked! And here it is, `fast-flights`.
-
+Metadata-Version: 2.1
+Name: fast-flights
+Version: 0.3
+Summary: The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python.
+Author-email: AWeirdDev <aweirdscratcher@gmail.com>
+Project-URL: Homepage, https://github.com/AWeirdDev/flights
+Project-URL: Bug Tracker, https://github.com/AWeirdDev/flights/issues
+Keywords: flights,google,google-flights,scraper,protobuf,travel,trip,passengers,airport
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: protobuf
+Requires-Dist: selectolax
+
+<div align="center">
+
+# flights (fast-flights)
+
+The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python. Based on Base64-encoded Protobuf string.
+
+```haskell
+$ pip install fast-flights
+```
+
+</div>
+
+## Usage
+
+To use `fast-flights`, you'll first create a filter (inherited from `?tfs=`) to perform a request.
+Then, add `flight_data`, `trip`, `seat` and `passengers` info to use the API directly.
+
+Honorable mention: I like birds. Yes, I like birds.
+
+```python
+from fast_flights import FlightData, Passengers, create_filter, get_flights
+
+# Create a new filter
+filter = create_filter(
+    flight_data=[
+        # Include more if it's not a one-way trip
+        FlightData(
+            date="2024-07-02",  # Date of departure
+            from_airport="TPE", 
+            to_airport="MYJ"
+        ),
+        # ... include more for round trips and multi-city trips
+    ],
+    trip="one-way",  # Trip (round-trip, one-way, multi-city)
+    seat="economy",  # Seat (economy, premium economy, business or first)
+    passengers=Passengers(
+        adults=2,
+        children=1,
+        infants_in_seat=0,
+        infants_on_lap=0
+    ),
+)
+
+# Get flights with a filter
+result = get_flights(filter)
+
+# The price is currently... low/typical/high
+print("The price is currently", result.current_price)
+
+# Display the first flight
+print(result.flights[0])
+```
+
+Additionally, you can use the `Airport` enum to search for airports in code (as you type)! (See `_generated_enum.py` in source)
+
+```python
+Airport.TAIPEI
+              |---------------------------------|
+              | TAIPEI_SONGSHAN_AIRPORT         |
+              | TAPACHULA_INTERNATIONAL_AIRPORT |
+              | TAMPA_INTERNATIONAL_AIRPORT     |
+              | ... 5 more                      |
+              |---------------------------------|
+```
+
+## How it's made
+
+The other day, I was making a chat-interface-based trip recommendation app and wanted to add a feature that can search for flights available for booking. My personal choice is definitely [Google Flights](https://flights.google.com) since Google always has the best and most organized data on the web. Therefore, I searched for APIs on Google.
+
+> 🔎 **Search** <br />
+> google flights api
+
+The results? Bad. It seems like they discontinued this service and it now lives in the Graveyard of Google.
+
+> <sup><a href="https://duffel.com/blog/google-flights-api" target="_blank">🧏‍♂️ <b>duffel.com</b></a></sup><br />
+> <sup><i>Google Flights API: How did it work & what happened to it?</i></b>
+>
+> The Google Flights API offered developers access to aggregated airline data, including flight times, availability, and prices. Over a decade ago, Google announced the acquisition of ITA Software Inc. which it used to develop its API. **However, in 2018, Google ended access to the public-facing API and now only offers access through the QPX enterprise product**.
+
+That's awful! I've also looked for free alternatives but their rate limits and pricing are just 😬 (not a good fit/deal for everyone).
+
+<br />
+
+However, Google Flights has their UI – [flights.google.com](https://flights.google.com). So, maybe I could just use Developer Tools to log the requests made and just replicate all of that? Undoubtedly not! Their requests are just full of numbers and unreadable text, so that's not the solution.
+
+Perhaps, we could scrape it? I mean, Google allowed many companies like [Serpapi](https://google.com/search?q=serpapi) to scrape their web just pretending like nothing happened... So let's scrape our own.
+
+> 🔎 **Search** <br />
+> google flights ~~api~~ scraper pypi
+
+Excluding the ones that are not active, I came across [hugoglvs/google-flights-scraper](https://pypi.org/project/google-flights-scraper) on Pypi. I thought to myself: "aint no way this is the solution!"
+
+I checked hugoglvs's code on [GitHub](https://github.com/hugoglvs/google-flights-scraper), and I immediately detected "playwright," my worst enemy. One word can describe it well: slow. Two words? Extremely slow. What's more, it doesn't even run on the **🗻 Edge** because of configuration errors, missing libraries... etc. I could just reverse [try.playwright.tech](https://try.playwright.tech) and use a better environment, but that's just too risky if they added Cloudflare as an additional security barrier 😳.
+
+Life tells me to never give up. Let's just take a look at their URL params...
+
+```markdown
+https://www.google.com/travel/flights/search?tfs=CBwQAhoeEgoyMDI0LTA1LTI4agcIARIDVFBFcgcIARIDTVlKGh4SCjIwMjQtMDUtMzBqBwgBEgNNWUpyBwgBEgNUUEVAAUgBcAGCAQsI____________AZgBAQ&hl=en
+```
+
+| Param | Content | My past understanding |
+|-------|---------|-----------------------|
+| hl    | en      | Sets the language.    |
+| tfs   | CBwQAhoeEgoyMDI0LTA1LTI4agcIARID… | What is this???? 🤮🤮 |
+
+I removed the `?tfs=` parameter and found out that this is the control of our request! And it looks so base64-y.
+
+If we decode it to raw text, we can still see the dates, but we're not quite there — there's too much unwanted Unicode text.
+
+Or maybe it's some kind of a **data-storing method** Google uses? What if it's something like JSON? Let's look it up.
+
+> 🔎 **Search** <br />
+> google's json alternative
+
+> 🐣 **Result**<br />
+> Solution: The Power of **Protocol Buffers**
+> 
+> LinkedIn turned to Protocol Buffers, often referred to as **protobuf**, a binary serialization format developed by Google. The key advantage of Protocol Buffers is its efficiency, compactness, and speed, making it significantly faster than JSON for serialization and deserialization.
+
+Gotcha, Protobuf! Let's feed it to an online decoder and see how it does:
+
+> 🔎 **Search** <br />
+> protobuf decoder
+
+> 🐣 **Result**<br />
+> [protobuf-decoder.netlify.app](https://protobuf-decoder.netlify.app)
+
+I then pasted the Base64-encoded string to the decoder and no way! It DID return valid data!
+
+![annotated, Protobuf Decoder screenshot](https://github.com/AWeirdDev/flights/assets/90096971/77dfb097-f961-4494-be88-3640763dbc8c)
+
+I immediately recognized the values — that's my data, that's my query!
+
+So, I wrote some simple Protobuf code to decode the data.
+
+```protobuf
+syntax = "proto3"
+
+message Airport {
+    string name = 2;
+}
+
+message FlightInfo {
+    string date = 2;
+    Airport dep_airport = 13;
+    Airport arr_airport = 14;
+}
+
+message GoogleSucks {
+    repeated FlightInfo = 3;
+}
+```
+
+It works! Now, I won't consider myself an "experienced Protobuf developer" but rather a complete beginner.
+
+I have no idea what I wrote but... it worked! And here it is, `fast-flights`.
+
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: fast-flights Version: 0.2 Summary: The fast,
+Metadata-Version: 2.1 Name: fast-flights Version: 0.3 Summary: The fast,
 robust, strongly-typed Google Flights scraper (API) implemented in Python.
 Author-email: AWeirdDev
-gmail.com> Project-URL: Homepage, https://github.com/AWeirdScratcher/flights
-Project-URL: Bug Tracker, https://github.com/AWeirdScratcher/flights/issues
-Keywords: flights,google,google-
-flights,scraper,protobuf,travel,trip,passengers,airport Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Requires-Dist: requests Requires-Dist:
-protobuf Requires-Dist: selectolax
+gmail.com> Project-URL: Homepage, https://github.com/AWeirdDev/flights Project-
+URL: Bug Tracker, https://github.com/AWeirdDev/flights/issues Keywords:
+flights,google,google-flights,scraper,protobuf,travel,trip,passengers,airport
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist:
+requests Requires-Dist: protobuf Requires-Dist: selectolax
    # flights (fast-flights) The fast, robust, strongly-typed Google Flights
  scraper (API) implemented in Python. Based on Base64-encoded Protobuf string.
                    ```haskell $ pip install fast-flights ```
 ## Usage To use `fast-flights`, you'll first create a filter (inherited from
 `?tfs=`) to perform a request. Then, add `flight_data`, `trip`, `seat` and
 `passengers` info to use the API directly. Honorable mention: I like birds.
 Yes, I like birds. ```python from fast_flights import FlightData, Passengers,
```

### Comparing `fast_flights-0.2/README.md` & `fast_flights-0.3/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-<div align="center">
-
-# flights (fast-flights)
-
-The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python. Based on Base64-encoded Protobuf string.
-
-```haskell
-$ pip install fast-flights
-```
-
-</div>
-
-## Usage
-
-To use `fast-flights`, you'll first create a filter (inherited from `?tfs=`) to perform a request.
-Then, add `flight_data`, `trip`, `seat` and `passengers` info to use the API directly.
-
-Honorable mention: I like birds. Yes, I like birds.
-
-```python
-from fast_flights import FlightData, Passengers, create_filter, get_flights
-
-# Create a new filter
-filter = create_filter(
-    flight_data=[
-        # Include more if it's not a one-way trip
-        FlightData(
-            date="2024-07-02",  # Date of departure
-            from_airport="TPE", 
-            to_airport="MYJ"
-        ),
-        # ... include more for round trips and multi-city trips
-    ],
-    trip="one-way",  # Trip (round-trip, one-way, multi-city)
-    seat="economy",  # Seat (economy, premium economy, business or first)
-    passengers=Passengers(
-        adults=2,
-        children=1,
-        infants_in_seat=0,
-        infants_on_lap=0
-    ),
-)
-
-# Get flights with a filter
-result = get_flights(filter)
-
-# The price is currently... low/typical/high
-print("The price is currently", result.current_price)
-
-# Display the first flight
-print(result.flights[0])
-```
-
-Additionally, you can use the `Airport` enum to search for airports in code (as you type)! (See `_generated_enum.py` in source)
-
-```python
-Airport.TAIPEI
-              |---------------------------------|
-              | TAIPEI_SONGSHAN_AIRPORT         |
-              | TAPACHULA_INTERNATIONAL_AIRPORT |
-              | TAMPA_INTERNATIONAL_AIRPORT     |
-              | ... 5 more                      |
-              |---------------------------------|
-```
-
-## How it's made
-
-The other day, I was making a chat-interface-based trip recommendation app and wanted to add a feature that can search for flights available for booking. My personal choice is definitely [Google Flights](https://flights.google.com) since Google always has the best and most organized data on the web. Therefore, I searched for APIs on Google.
-
-> 🔎 **Search** <br />
-> google flights api
-
-The results? Bad. It seems like they discontinued this service and it now lives in the Graveyard of Google.
-
-> <sup><a href="https://duffel.com/blog/google-flights-api" target="_blank">🧏‍♂️ <b>duffel.com</b></a></sup><br />
-> <sup><i>Google Flights API: How did it work & what happened to it?</i></b>
->
-> The Google Flights API offered developers access to aggregated airline data, including flight times, availability, and prices. Over a decade ago, Google announced the acquisition of ITA Software Inc. which it used to develop its API. **However, in 2018, Google ended access to the public-facing API and now only offers access through the QPX enterprise product**.
-
-That's awful! I've also looked for free alternatives but their rate limits and pricing are just 😬 (not a good fit/deal for everyone).
-
-<br />
-
-However, Google Flights has their UI – [flights.google.com](https://flights.google.com). So, maybe I could just use Developer Tools to log the requests made and just replicate all of that? Undoubtedly not! Their requests are just full of numbers and unreadable text, so that's not the solution.
-
-Perhaps, we could scrape it? I mean, Google allowed many companies like [Serpapi](https://google.com/search?q=serpapi) to scrape their web just pretending like nothing happened... So let's scrape our own.
-
-> 🔎 **Search** <br />
-> google flights ~~api~~ scraper pypi
-
-Excluding the ones that are not active, I came across [hugoglvs/google-flights-scraper](https://pypi.org/project/google-flights-scraper) on Pypi. I thought to myself: "aint no way this is the solution!"
-
-I checked hugoglvs's code on [GitHub](https://github.com/hugoglvs/google-flights-scraper), and I immediately detected "playwright," my worst enemy. One word can describe it well: slow. Two words? Extremely slow. What's more, it doesn't even run on the **🗻 Edge** because of configuration errors, missing libraries... etc. I could just reverse [try.playwright.tech](https://try.playwright.tech) and use a better environment, but that's just too risky if they added Cloudflare as an additional security barrier 😳.
-
-Life tells me to never give up. Let's just take a look at their URL params...
-
-```markdown
-https://www.google.com/travel/flights/search?tfs=CBwQAhoeEgoyMDI0LTA1LTI4agcIARIDVFBFcgcIARIDTVlKGh4SCjIwMjQtMDUtMzBqBwgBEgNNWUpyBwgBEgNUUEVAAUgBcAGCAQsI____________AZgBAQ&hl=en
-```
-
-| Param | Content | My past understanding |
-|-------|---------|-----------------------|
-| hl    | en      | Sets the language.    |
-| tfs   | CBwQAhoeEgoyMDI0LTA1LTI4agcIARID… | What is this???? 🤮🤮 |
-
-I removed the `?tfs=` parameter and found out that this is the control of our request! And it looks so base64-y.
-
-If we decode it to raw text, we can still see the dates, but we're not quite there — there's too much unwanted Unicode text.
-
-Or maybe it's some kind of a **data-storing method** Google uses? What if it's something like JSON? Let's look it up.
-
-> 🔎 **Search** <br />
-> google's json alternative
-
-> 🐣 **Result**<br />
-> Solution: The Power of **Protocol Buffers**
-> 
-> LinkedIn turned to Protocol Buffers, often referred to as **protobuf**, a binary serialization format developed by Google. The key advantage of Protocol Buffers is its efficiency, compactness, and speed, making it significantly faster than JSON for serialization and deserialization.
-
-Gotcha, Protobuf! Let's feed it to an online decoder and see how it does:
-
-> 🔎 **Search** <br />
-> protobuf decoder
-
-> 🐣 **Result**<br />
-> [protobuf-decoder.netlify.app](https://protobuf-decoder.netlify.app)
-
-I then pasted the Base64-encoded string to the decoder and no way! It DID return valid data!
-
-![annotated, Protobuf Decoder screenshot](https://github.com/AWeirdDev/flights/assets/90096971/77dfb097-f961-4494-be88-3640763dbc8c)
-
-I immediately recognized the values — that's my data, that's my query!
-
-So, I wrote some simple Protobuf code to decode the data.
-
-```protobuf
-syntax = "proto3"
-
-message Airport {
-    string name = 2;
-}
-
-message FlightInfo {
-    string date = 2;
-    Airport dep_airport = 13;
-    Airport arr_airport = 14;
-}
-
-message GoogleSucks {
-    repeated FlightInfo = 3;
-}
-```
-
-It works! Now, I won't consider myself an "experienced Protobuf developer" but rather a complete beginner.
-
-I have no idea what I wrote but... it worked! And here it is, `fast-flights`.
-
+<div align="center">
+
+# flights (fast-flights)
+
+The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python. Based on Base64-encoded Protobuf string.
+
+```haskell
+$ pip install fast-flights
+```
+
+</div>
+
+## Usage
+
+To use `fast-flights`, you'll first create a filter (inherited from `?tfs=`) to perform a request.
+Then, add `flight_data`, `trip`, `seat` and `passengers` info to use the API directly.
+
+Honorable mention: I like birds. Yes, I like birds.
+
+```python
+from fast_flights import FlightData, Passengers, create_filter, get_flights
+
+# Create a new filter
+filter = create_filter(
+    flight_data=[
+        # Include more if it's not a one-way trip
+        FlightData(
+            date="2024-07-02",  # Date of departure
+            from_airport="TPE", 
+            to_airport="MYJ"
+        ),
+        # ... include more for round trips and multi-city trips
+    ],
+    trip="one-way",  # Trip (round-trip, one-way, multi-city)
+    seat="economy",  # Seat (economy, premium economy, business or first)
+    passengers=Passengers(
+        adults=2,
+        children=1,
+        infants_in_seat=0,
+        infants_on_lap=0
+    ),
+)
+
+# Get flights with a filter
+result = get_flights(filter)
+
+# The price is currently... low/typical/high
+print("The price is currently", result.current_price)
+
+# Display the first flight
+print(result.flights[0])
+```
+
+Additionally, you can use the `Airport` enum to search for airports in code (as you type)! (See `_generated_enum.py` in source)
+
+```python
+Airport.TAIPEI
+              |---------------------------------|
+              | TAIPEI_SONGSHAN_AIRPORT         |
+              | TAPACHULA_INTERNATIONAL_AIRPORT |
+              | TAMPA_INTERNATIONAL_AIRPORT     |
+              | ... 5 more                      |
+              |---------------------------------|
+```
+
+## How it's made
+
+The other day, I was making a chat-interface-based trip recommendation app and wanted to add a feature that can search for flights available for booking. My personal choice is definitely [Google Flights](https://flights.google.com) since Google always has the best and most organized data on the web. Therefore, I searched for APIs on Google.
+
+> 🔎 **Search** <br />
+> google flights api
+
+The results? Bad. It seems like they discontinued this service and it now lives in the Graveyard of Google.
+
+> <sup><a href="https://duffel.com/blog/google-flights-api" target="_blank">🧏‍♂️ <b>duffel.com</b></a></sup><br />
+> <sup><i>Google Flights API: How did it work & what happened to it?</i></b>
+>
+> The Google Flights API offered developers access to aggregated airline data, including flight times, availability, and prices. Over a decade ago, Google announced the acquisition of ITA Software Inc. which it used to develop its API. **However, in 2018, Google ended access to the public-facing API and now only offers access through the QPX enterprise product**.
+
+That's awful! I've also looked for free alternatives but their rate limits and pricing are just 😬 (not a good fit/deal for everyone).
+
+<br />
+
+However, Google Flights has their UI – [flights.google.com](https://flights.google.com). So, maybe I could just use Developer Tools to log the requests made and just replicate all of that? Undoubtedly not! Their requests are just full of numbers and unreadable text, so that's not the solution.
+
+Perhaps, we could scrape it? I mean, Google allowed many companies like [Serpapi](https://google.com/search?q=serpapi) to scrape their web just pretending like nothing happened... So let's scrape our own.
+
+> 🔎 **Search** <br />
+> google flights ~~api~~ scraper pypi
+
+Excluding the ones that are not active, I came across [hugoglvs/google-flights-scraper](https://pypi.org/project/google-flights-scraper) on Pypi. I thought to myself: "aint no way this is the solution!"
+
+I checked hugoglvs's code on [GitHub](https://github.com/hugoglvs/google-flights-scraper), and I immediately detected "playwright," my worst enemy. One word can describe it well: slow. Two words? Extremely slow. What's more, it doesn't even run on the **🗻 Edge** because of configuration errors, missing libraries... etc. I could just reverse [try.playwright.tech](https://try.playwright.tech) and use a better environment, but that's just too risky if they added Cloudflare as an additional security barrier 😳.
+
+Life tells me to never give up. Let's just take a look at their URL params...
+
+```markdown
+https://www.google.com/travel/flights/search?tfs=CBwQAhoeEgoyMDI0LTA1LTI4agcIARIDVFBFcgcIARIDTVlKGh4SCjIwMjQtMDUtMzBqBwgBEgNNWUpyBwgBEgNUUEVAAUgBcAGCAQsI____________AZgBAQ&hl=en
+```
+
+| Param | Content | My past understanding |
+|-------|---------|-----------------------|
+| hl    | en      | Sets the language.    |
+| tfs   | CBwQAhoeEgoyMDI0LTA1LTI4agcIARID… | What is this???? 🤮🤮 |
+
+I removed the `?tfs=` parameter and found out that this is the control of our request! And it looks so base64-y.
+
+If we decode it to raw text, we can still see the dates, but we're not quite there — there's too much unwanted Unicode text.
+
+Or maybe it's some kind of a **data-storing method** Google uses? What if it's something like JSON? Let's look it up.
+
+> 🔎 **Search** <br />
+> google's json alternative
+
+> 🐣 **Result**<br />
+> Solution: The Power of **Protocol Buffers**
+> 
+> LinkedIn turned to Protocol Buffers, often referred to as **protobuf**, a binary serialization format developed by Google. The key advantage of Protocol Buffers is its efficiency, compactness, and speed, making it significantly faster than JSON for serialization and deserialization.
+
+Gotcha, Protobuf! Let's feed it to an online decoder and see how it does:
+
+> 🔎 **Search** <br />
+> protobuf decoder
+
+> 🐣 **Result**<br />
+> [protobuf-decoder.netlify.app](https://protobuf-decoder.netlify.app)
+
+I then pasted the Base64-encoded string to the decoder and no way! It DID return valid data!
+
+![annotated, Protobuf Decoder screenshot](https://github.com/AWeirdDev/flights/assets/90096971/77dfb097-f961-4494-be88-3640763dbc8c)
+
+I immediately recognized the values — that's my data, that's my query!
+
+So, I wrote some simple Protobuf code to decode the data.
+
+```protobuf
+syntax = "proto3"
+
+message Airport {
+    string name = 2;
+}
+
+message FlightInfo {
+    string date = 2;
+    Airport dep_airport = 13;
+    Airport arr_airport = 14;
+}
+
+message GoogleSucks {
+    repeated FlightInfo = 3;
+}
+```
+
+It works! Now, I won't consider myself an "experienced Protobuf developer" but rather a complete beginner.
+
+I have no idea what I wrote but... it worked! And here it is, `fast-flights`.
+
```

### Comparing `fast_flights-0.2/fast_flights/_generated_enum.py` & `fast_flights-0.3/fast_flights/_generated_enum.py`

 * *Files identical despite different names*

### Comparing `fast_flights-0.2/fast_flights/filter.py` & `fast_flights-0.3/fast_flights/filter.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Literal, List
-from .flights_impl import FlightData, Passengers, TFSData
-
-
-def create_filter(
-    *,
-    flight_data: List[FlightData],
-    trip: Literal["round-trip", "one-way", "multi-city"],
-    passengers: Passengers,
-    seat: Literal["economy", "premium-economy", "business", "first"],
-) -> TFSData:
-    """Create a filter. (``?tfs=``)
-
-    Args:
-        flight_data (list[FlightData]): Flight data as a list.
-        trip ("one-way" | "round-trip" | "multi-city"): Trip type.
-        passengers (Passengers): Passengers.
-        seat ("economy" | "premium-economy" | "business" | "first"): Seat.
-    """
-    return TFSData.from_interface(
-        flight_data=flight_data, trip=trip, passengers=passengers, seat=seat
-    )
+from typing import Literal, List
+from .flights_impl import FlightData, Passengers, TFSData
+
+
+def create_filter(
+    *,
+    flight_data: List[FlightData],
+    trip: Literal["round-trip", "one-way", "multi-city"],
+    passengers: Passengers,
+    seat: Literal["economy", "premium-economy", "business", "first"],
+) -> TFSData:
+    """Create a filter. (``?tfs=``)
+
+    Args:
+        flight_data (list[FlightData]): Flight data as a list.
+        trip ("one-way" | "round-trip" | "multi-city"): Trip type.
+        passengers (Passengers): Passengers.
+        seat ("economy" | "premium-economy" | "business" | "first"): Seat.
+    """
+    return TFSData.from_interface(
+        flight_data=flight_data, trip=trip, passengers=passengers, seat=seat
+    )
```

### Comparing `fast_flights-0.2/fast_flights/flights_impl.py` & `fast_flights-0.3/fast_flights/flights_impl.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-"""Typed implementation of flights_pb2.py"""
-
-import base64
-from typing import Any, List, TYPE_CHECKING, Literal, Union
-
-from . import flights_pb2 as PB
-from ._generated_enum import Airport
-
-if TYPE_CHECKING:
-    PB: Any
-
-
-class FlightData:
-    """Represents flight data.
-
-    Args:
-        date (str): Date.
-        from_airport (str): Departure (airport). Where from?
-        to_airport (str): Arrival (airport). Where to?
-    """
-
-    __slots__ = ("date", "from_airport", "to_airport")
-    date: str
-    from_airport: str
-    to_airport: str
-
-    def __init__(
-        self,
-        *,
-        date: str,
-        from_airport: Union[Airport, str],
-        to_airport: Union[Airport, str],
-    ):
-        self.date = date
-        self.from_airport = (
-            from_airport.value if isinstance(from_airport, Airport) else from_airport
-        )
-        self.to_airport = (
-            to_airport.value if isinstance(to_airport, Airport) else to_airport
-        )
-
-    def attach(self, info: PB.Info) -> None:  # type: ignore
-        data = info.data.add()
-        data.date = self.date
-        data.from_flight.airport = self.from_airport
-        data.to_flight.airport = self.to_airport
-
-    def __repr__(self) -> str:
-        return (
-            f"FlightData(date={self.date!r}, "
-            f"from_airport={self.from_airport}, "
-            f"to_airport={self.to_airport})"
-        )
-
-
-class Passengers:
-    def __init__(
-        self,
-        *,
-        adults: int = 0,
-        children: int = 0,
-        infants_in_seat: int = 0,
-        infants_on_lap: int = 0,
-    ):
-        assert (
-            sum((adults, children, infants_in_seat, infants_on_lap)) <= 9
-        ), "Too many passengers (> 9)"
-        assert (
-            infants_on_lap <= adults
-        ), "You must have at least one adult per infant on lap"
-
-        self.pb = []
-        self.pb += [PB.Passenger.ADULT for _ in range(adults)]
-        self.pb += [PB.Passenger.CHILD for _ in range(children)]
-        self.pb += [PB.Passenger.INFANT_IN_SEAT for _ in range(infants_in_seat)]
-        self.pb += [PB.Passenger.INFANT_ON_LAP for _ in range(infants_on_lap)]
-
-        self._data = (adults, children, infants_in_seat, infants_on_lap)
-
-    def attach(self, info: PB.Info) -> None:  # type: ignore
-        for p in self.pb:
-            info.passengers.append(p)
-
-    def __repr__(self) -> str:
-        return f"Passengers({self._data})"
-
-
-class TFSData:
-    """``?tfs=`` data. (internal)
-
-    Use `TFSData.from_interface` instead.
-    """
-
-    def __init__(
-        self,
-        *,
-        flight_data: List[FlightData],
-        seat: PB.Seat,  # type: ignore
-        trip: PB.Trip,  # type: ignore
-        passengers: Passengers,
-    ):
-        self.flight_data = flight_data
-        self.seat = seat
-        self.trip = trip
-        self.passengers = passengers
-
-    def pb(self) -> PB.Info:  # type: ignore
-        info = PB.Info()
-        info.seat = self.seat
-        info.trip = self.trip
-
-        self.passengers.attach(info)
-
-        for fd in self.flight_data:
-            fd.attach(info)
-
-        return info
-
-    def to_string(self) -> bytes:
-        return self.pb().SerializeToString()
-
-    def as_b64(self) -> bytes:
-        return base64.b64encode(self.to_string())
-
-    @staticmethod
-    def from_interface(
-        *,
-        flight_data: List[FlightData],
-        trip: Literal["round-trip", "one-way", "multi-city"],
-        passengers: Passengers,
-        seat: Literal["economy", "premium-economy", "business", "first"],
-    ):
-        """Use ``?tfs=`` from an interface.
-
-        Args:
-            flight_data (list[FlightData]): Flight data as a list.
-            trip ("one-way" | "round-trip" | "multi-city"): Trip type.
-            passengers (Passengers): Passengers.
-            seat ("economy" | "premium-economy" | "business" | "first"): Seat.
-        """
-        trip_t = {
-            "round-trip": PB.Trip.ROUND_TRIP,
-            "one-way": PB.Trip.ONE_WAY,
-            "multi-city": PB.Trip.MULTI_CITY,
-        }[trip]
-        seat_t = {
-            "economy": PB.Seat.ECONOMY,
-            "premium-economy": PB.Seat.PREMIUM_ECONOMY,
-            "business": PB.Seat.BUSINESS,
-            "first": PB.Seat.FIRST,
-        }[seat]
-
-        return TFSData(
-            flight_data=flight_data, seat=seat_t, trip=trip_t, passengers=passengers
-        )
-
-    def __repr__(self) -> str:
-        return f"TFSData({'hello'!r}, flight_data={self.flight_data!r})"
+"""Typed implementation of flights_pb2.py"""
+
+import base64
+from typing import Any, List, TYPE_CHECKING, Literal, Union
+
+from . import flights_pb2 as PB
+from ._generated_enum import Airport
+
+if TYPE_CHECKING:
+    PB: Any
+
+
+class FlightData:
+    """Represents flight data.
+
+    Args:
+        date (str): Date.
+        from_airport (str): Departure (airport). Where from?
+        to_airport (str): Arrival (airport). Where to?
+    """
+
+    __slots__ = ("date", "from_airport", "to_airport")
+    date: str
+    from_airport: str
+    to_airport: str
+
+    def __init__(
+        self,
+        *,
+        date: str,
+        from_airport: Union[Airport, str],
+        to_airport: Union[Airport, str],
+    ):
+        self.date = date
+        self.from_airport = (
+            from_airport.value if isinstance(from_airport, Airport) else from_airport
+        )
+        self.to_airport = (
+            to_airport.value if isinstance(to_airport, Airport) else to_airport
+        )
+
+    def attach(self, info: PB.Info) -> None:  # type: ignore
+        data = info.data.add()
+        data.date = self.date
+        data.from_flight.airport = self.from_airport
+        data.to_flight.airport = self.to_airport
+
+    def __repr__(self) -> str:
+        return (
+            f"FlightData(date={self.date!r}, "
+            f"from_airport={self.from_airport}, "
+            f"to_airport={self.to_airport})"
+        )
+
+
+class Passengers:
+    def __init__(
+        self,
+        *,
+        adults: int = 0,
+        children: int = 0,
+        infants_in_seat: int = 0,
+        infants_on_lap: int = 0,
+    ):
+        assert (
+            sum((adults, children, infants_in_seat, infants_on_lap)) <= 9
+        ), "Too many passengers (> 9)"
+        assert (
+            infants_on_lap <= adults
+        ), "You must have at least one adult per infant on lap"
+
+        self.pb = []
+        self.pb += [PB.Passenger.ADULT for _ in range(adults)]
+        self.pb += [PB.Passenger.CHILD for _ in range(children)]
+        self.pb += [PB.Passenger.INFANT_IN_SEAT for _ in range(infants_in_seat)]
+        self.pb += [PB.Passenger.INFANT_ON_LAP for _ in range(infants_on_lap)]
+
+        self._data = (adults, children, infants_in_seat, infants_on_lap)
+
+    def attach(self, info: PB.Info) -> None:  # type: ignore
+        for p in self.pb:
+            info.passengers.append(p)
+
+    def __repr__(self) -> str:
+        return f"Passengers({self._data})"
+
+
+class TFSData:
+    """``?tfs=`` data. (internal)
+
+    Use `TFSData.from_interface` instead.
+    """
+
+    def __init__(
+        self,
+        *,
+        flight_data: List[FlightData],
+        seat: PB.Seat,  # type: ignore
+        trip: PB.Trip,  # type: ignore
+        passengers: Passengers,
+    ):
+        self.flight_data = flight_data
+        self.seat = seat
+        self.trip = trip
+        self.passengers = passengers
+
+    def pb(self) -> PB.Info:  # type: ignore
+        info = PB.Info()
+        info.seat = self.seat
+        info.trip = self.trip
+
+        self.passengers.attach(info)
+
+        for fd in self.flight_data:
+            fd.attach(info)
+
+        return info
+
+    def to_string(self) -> bytes:
+        return self.pb().SerializeToString()
+
+    def as_b64(self) -> bytes:
+        return base64.b64encode(self.to_string())
+
+    @staticmethod
+    def from_interface(
+        *,
+        flight_data: List[FlightData],
+        trip: Literal["round-trip", "one-way", "multi-city"],
+        passengers: Passengers,
+        seat: Literal["economy", "premium-economy", "business", "first"],
+    ):
+        """Use ``?tfs=`` from an interface.
+
+        Args:
+            flight_data (list[FlightData]): Flight data as a list.
+            trip ("one-way" | "round-trip" | "multi-city"): Trip type.
+            passengers (Passengers): Passengers.
+            seat ("economy" | "premium-economy" | "business" | "first"): Seat.
+        """
+        trip_t = {
+            "round-trip": PB.Trip.ROUND_TRIP,
+            "one-way": PB.Trip.ONE_WAY,
+            "multi-city": PB.Trip.MULTI_CITY,
+        }[trip]
+        seat_t = {
+            "economy": PB.Seat.ECONOMY,
+            "premium-economy": PB.Seat.PREMIUM_ECONOMY,
+            "business": PB.Seat.BUSINESS,
+            "first": PB.Seat.FIRST,
+        }[seat]
+
+        return TFSData(
+            flight_data=flight_data, seat=seat_t, trip=trip_t, passengers=passengers
+        )
+
+    def __repr__(self) -> str:
+        return f"TFSData({'hello'!r}, flight_data={self.flight_data!r})"
```

### Comparing `fast_flights-0.2/fast_flights/flights_pb2.py` & `fast_flights-0.3/fast_flights/flights_pb2.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# type: ignore
-
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: flights.proto
-"""Generated protocol buffer code."""
-
-from google.protobuf.internal import builder as _builder
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\rflights.proto"\x1a\n\x07\x41irport\x12\x0f\n\x07\x61irport\x18\x02 \x01(\t"V\n\nFlightData\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\t\x12\x1d\n\x0b\x66rom_flight\x18\r \x01(\x0b\x32\x08.Airport\x12\x1b\n\tto_flight\x18\x0e \x01(\x0b\x32\x08.Airport"k\n\x04Info\x12\x19\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32\x0b.FlightData\x12\x13\n\x04seat\x18\t \x01(\x0e\x32\x05.Seat\x12\x1e\n\npassengers\x18\x08 \x03(\x0e\x32\n.Passenger\x12\x13\n\x04trip\x18\x13 \x01(\x0e\x32\x05.Trip*S\n\x04Seat\x12\x10\n\x0cUNKNOWN_SEAT\x10\x00\x12\x0b\n\x07\x45\x43ONOMY\x10\x01\x12\x13\n\x0fPREMIUM_ECONOMY\x10\x02\x12\x0c\n\x08\x42USINESS\x10\x03\x12\t\n\x05\x46IRST\x10\x04*E\n\x04Trip\x12\x10\n\x0cUNKNOWN_TRIP\x10\x00\x12\x0e\n\nROUND_TRIP\x10\x01\x12\x0b\n\x07ONE_WAY\x10\x02\x12\x0e\n\nMULTI_CITY\x10\x03*_\n\tPassenger\x12\x15\n\x11UNKNOWN_PASSENGER\x10\x00\x12\t\n\x05\x41\x44ULT\x10\x01\x12\t\n\x05\x43HILD\x10\x02\x12\x12\n\x0eINFANT_IN_SEAT\x10\x03\x12\x11\n\rINFANT_ON_LAP\x10\x04\x62\x06proto3'
-)
-
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "flights_pb2", globals())
-if _descriptor._USE_C_DESCRIPTORS == False:
-    DESCRIPTOR._options = None
-    _SEAT._serialized_start = 242
-    _SEAT._serialized_end = 325
-    _TRIP._serialized_start = 327
-    _TRIP._serialized_end = 396
-    _PASSENGER._serialized_start = 398
-    _PASSENGER._serialized_end = 493
-    _AIRPORT._serialized_start = 17
-    _AIRPORT._serialized_end = 43
-    _FLIGHTDATA._serialized_start = 45
-    _FLIGHTDATA._serialized_end = 131
-    _INFO._serialized_start = 133
-    _INFO._serialized_end = 240
-# @@protoc_insertion_point(module_scope)
+# type: ignore
+
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: flights.proto
+"""Generated protocol buffer code."""
+
+from google.protobuf.internal import builder as _builder
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\rflights.proto"\x1a\n\x07\x41irport\x12\x0f\n\x07\x61irport\x18\x02 \x01(\t"V\n\nFlightData\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\t\x12\x1d\n\x0b\x66rom_flight\x18\r \x01(\x0b\x32\x08.Airport\x12\x1b\n\tto_flight\x18\x0e \x01(\x0b\x32\x08.Airport"k\n\x04Info\x12\x19\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32\x0b.FlightData\x12\x13\n\x04seat\x18\t \x01(\x0e\x32\x05.Seat\x12\x1e\n\npassengers\x18\x08 \x03(\x0e\x32\n.Passenger\x12\x13\n\x04trip\x18\x13 \x01(\x0e\x32\x05.Trip*S\n\x04Seat\x12\x10\n\x0cUNKNOWN_SEAT\x10\x00\x12\x0b\n\x07\x45\x43ONOMY\x10\x01\x12\x13\n\x0fPREMIUM_ECONOMY\x10\x02\x12\x0c\n\x08\x42USINESS\x10\x03\x12\t\n\x05\x46IRST\x10\x04*E\n\x04Trip\x12\x10\n\x0cUNKNOWN_TRIP\x10\x00\x12\x0e\n\nROUND_TRIP\x10\x01\x12\x0b\n\x07ONE_WAY\x10\x02\x12\x0e\n\nMULTI_CITY\x10\x03*_\n\tPassenger\x12\x15\n\x11UNKNOWN_PASSENGER\x10\x00\x12\t\n\x05\x41\x44ULT\x10\x01\x12\t\n\x05\x43HILD\x10\x02\x12\x12\n\x0eINFANT_IN_SEAT\x10\x03\x12\x11\n\rINFANT_ON_LAP\x10\x04\x62\x06proto3'
+)
+
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "flights_pb2", globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+    DESCRIPTOR._options = None
+    _SEAT._serialized_start = 242
+    _SEAT._serialized_end = 325
+    _TRIP._serialized_start = 327
+    _TRIP._serialized_end = 396
+    _PASSENGER._serialized_start = 398
+    _PASSENGER._serialized_end = 493
+    _AIRPORT._serialized_start = 17
+    _AIRPORT._serialized_end = 43
+    _FLIGHTDATA._serialized_start = 45
+    _FLIGHTDATA._serialized_end = 131
+    _INFO._serialized_start = 133
+    _INFO._serialized_end = 240
+# @@protoc_insertion_point(module_scope)
```

### Comparing `fast_flights-0.2/fast_flights.egg-info/PKG-INFO` & `fast_flights-0.3/fast_flights.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-Metadata-Version: 2.1
-Name: fast-flights
-Version: 0.2
-Summary: The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python.
-Author-email: AWeirdDev <aweirdscratcher@gmail.com>
-Project-URL: Homepage, https://github.com/AWeirdScratcher/flights
-Project-URL: Bug Tracker, https://github.com/AWeirdScratcher/flights/issues
-Keywords: flights,google,google-flights,scraper,protobuf,travel,trip,passengers,airport
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: protobuf
-Requires-Dist: selectolax
-
-<div align="center">
-
-# flights (fast-flights)
-
-The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python. Based on Base64-encoded Protobuf string.
-
-```haskell
-$ pip install fast-flights
-```
-
-</div>
-
-## Usage
-
-To use `fast-flights`, you'll first create a filter (inherited from `?tfs=`) to perform a request.
-Then, add `flight_data`, `trip`, `seat` and `passengers` info to use the API directly.
-
-Honorable mention: I like birds. Yes, I like birds.
-
-```python
-from fast_flights import FlightData, Passengers, create_filter, get_flights
-
-# Create a new filter
-filter = create_filter(
-    flight_data=[
-        # Include more if it's not a one-way trip
-        FlightData(
-            date="2024-07-02",  # Date of departure
-            from_airport="TPE", 
-            to_airport="MYJ"
-        ),
-        # ... include more for round trips and multi-city trips
-    ],
-    trip="one-way",  # Trip (round-trip, one-way, multi-city)
-    seat="economy",  # Seat (economy, premium economy, business or first)
-    passengers=Passengers(
-        adults=2,
-        children=1,
-        infants_in_seat=0,
-        infants_on_lap=0
-    ),
-)
-
-# Get flights with a filter
-result = get_flights(filter)
-
-# The price is currently... low/typical/high
-print("The price is currently", result.current_price)
-
-# Display the first flight
-print(result.flights[0])
-```
-
-Additionally, you can use the `Airport` enum to search for airports in code (as you type)! (See `_generated_enum.py` in source)
-
-```python
-Airport.TAIPEI
-              |---------------------------------|
-              | TAIPEI_SONGSHAN_AIRPORT         |
-              | TAPACHULA_INTERNATIONAL_AIRPORT |
-              | TAMPA_INTERNATIONAL_AIRPORT     |
-              | ... 5 more                      |
-              |---------------------------------|
-```
-
-## How it's made
-
-The other day, I was making a chat-interface-based trip recommendation app and wanted to add a feature that can search for flights available for booking. My personal choice is definitely [Google Flights](https://flights.google.com) since Google always has the best and most organized data on the web. Therefore, I searched for APIs on Google.
-
-> 🔎 **Search** <br />
-> google flights api
-
-The results? Bad. It seems like they discontinued this service and it now lives in the Graveyard of Google.
-
-> <sup><a href="https://duffel.com/blog/google-flights-api" target="_blank">🧏‍♂️ <b>duffel.com</b></a></sup><br />
-> <sup><i>Google Flights API: How did it work & what happened to it?</i></b>
->
-> The Google Flights API offered developers access to aggregated airline data, including flight times, availability, and prices. Over a decade ago, Google announced the acquisition of ITA Software Inc. which it used to develop its API. **However, in 2018, Google ended access to the public-facing API and now only offers access through the QPX enterprise product**.
-
-That's awful! I've also looked for free alternatives but their rate limits and pricing are just 😬 (not a good fit/deal for everyone).
-
-<br />
-
-However, Google Flights has their UI – [flights.google.com](https://flights.google.com). So, maybe I could just use Developer Tools to log the requests made and just replicate all of that? Undoubtedly not! Their requests are just full of numbers and unreadable text, so that's not the solution.
-
-Perhaps, we could scrape it? I mean, Google allowed many companies like [Serpapi](https://google.com/search?q=serpapi) to scrape their web just pretending like nothing happened... So let's scrape our own.
-
-> 🔎 **Search** <br />
-> google flights ~~api~~ scraper pypi
-
-Excluding the ones that are not active, I came across [hugoglvs/google-flights-scraper](https://pypi.org/project/google-flights-scraper) on Pypi. I thought to myself: "aint no way this is the solution!"
-
-I checked hugoglvs's code on [GitHub](https://github.com/hugoglvs/google-flights-scraper), and I immediately detected "playwright," my worst enemy. One word can describe it well: slow. Two words? Extremely slow. What's more, it doesn't even run on the **🗻 Edge** because of configuration errors, missing libraries... etc. I could just reverse [try.playwright.tech](https://try.playwright.tech) and use a better environment, but that's just too risky if they added Cloudflare as an additional security barrier 😳.
-
-Life tells me to never give up. Let's just take a look at their URL params...
-
-```markdown
-https://www.google.com/travel/flights/search?tfs=CBwQAhoeEgoyMDI0LTA1LTI4agcIARIDVFBFcgcIARIDTVlKGh4SCjIwMjQtMDUtMzBqBwgBEgNNWUpyBwgBEgNUUEVAAUgBcAGCAQsI____________AZgBAQ&hl=en
-```
-
-| Param | Content | My past understanding |
-|-------|---------|-----------------------|
-| hl    | en      | Sets the language.    |
-| tfs   | CBwQAhoeEgoyMDI0LTA1LTI4agcIARID… | What is this???? 🤮🤮 |
-
-I removed the `?tfs=` parameter and found out that this is the control of our request! And it looks so base64-y.
-
-If we decode it to raw text, we can still see the dates, but we're not quite there — there's too much unwanted Unicode text.
-
-Or maybe it's some kind of a **data-storing method** Google uses? What if it's something like JSON? Let's look it up.
-
-> 🔎 **Search** <br />
-> google's json alternative
-
-> 🐣 **Result**<br />
-> Solution: The Power of **Protocol Buffers**
-> 
-> LinkedIn turned to Protocol Buffers, often referred to as **protobuf**, a binary serialization format developed by Google. The key advantage of Protocol Buffers is its efficiency, compactness, and speed, making it significantly faster than JSON for serialization and deserialization.
-
-Gotcha, Protobuf! Let's feed it to an online decoder and see how it does:
-
-> 🔎 **Search** <br />
-> protobuf decoder
-
-> 🐣 **Result**<br />
-> [protobuf-decoder.netlify.app](https://protobuf-decoder.netlify.app)
-
-I then pasted the Base64-encoded string to the decoder and no way! It DID return valid data!
-
-![annotated, Protobuf Decoder screenshot](https://github.com/AWeirdDev/flights/assets/90096971/77dfb097-f961-4494-be88-3640763dbc8c)
-
-I immediately recognized the values — that's my data, that's my query!
-
-So, I wrote some simple Protobuf code to decode the data.
-
-```protobuf
-syntax = "proto3"
-
-message Airport {
-    string name = 2;
-}
-
-message FlightInfo {
-    string date = 2;
-    Airport dep_airport = 13;
-    Airport arr_airport = 14;
-}
-
-message GoogleSucks {
-    repeated FlightInfo = 3;
-}
-```
-
-It works! Now, I won't consider myself an "experienced Protobuf developer" but rather a complete beginner.
-
-I have no idea what I wrote but... it worked! And here it is, `fast-flights`.
-
+Metadata-Version: 2.1
+Name: fast-flights
+Version: 0.3
+Summary: The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python.
+Author-email: AWeirdDev <aweirdscratcher@gmail.com>
+Project-URL: Homepage, https://github.com/AWeirdDev/flights
+Project-URL: Bug Tracker, https://github.com/AWeirdDev/flights/issues
+Keywords: flights,google,google-flights,scraper,protobuf,travel,trip,passengers,airport
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: requests
+Requires-Dist: protobuf
+Requires-Dist: selectolax
+
+<div align="center">
+
+# flights (fast-flights)
+
+The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python. Based on Base64-encoded Protobuf string.
+
+```haskell
+$ pip install fast-flights
+```
+
+</div>
+
+## Usage
+
+To use `fast-flights`, you'll first create a filter (inherited from `?tfs=`) to perform a request.
+Then, add `flight_data`, `trip`, `seat` and `passengers` info to use the API directly.
+
+Honorable mention: I like birds. Yes, I like birds.
+
+```python
+from fast_flights import FlightData, Passengers, create_filter, get_flights
+
+# Create a new filter
+filter = create_filter(
+    flight_data=[
+        # Include more if it's not a one-way trip
+        FlightData(
+            date="2024-07-02",  # Date of departure
+            from_airport="TPE", 
+            to_airport="MYJ"
+        ),
+        # ... include more for round trips and multi-city trips
+    ],
+    trip="one-way",  # Trip (round-trip, one-way, multi-city)
+    seat="economy",  # Seat (economy, premium economy, business or first)
+    passengers=Passengers(
+        adults=2,
+        children=1,
+        infants_in_seat=0,
+        infants_on_lap=0
+    ),
+)
+
+# Get flights with a filter
+result = get_flights(filter)
+
+# The price is currently... low/typical/high
+print("The price is currently", result.current_price)
+
+# Display the first flight
+print(result.flights[0])
+```
+
+Additionally, you can use the `Airport` enum to search for airports in code (as you type)! (See `_generated_enum.py` in source)
+
+```python
+Airport.TAIPEI
+              |---------------------------------|
+              | TAIPEI_SONGSHAN_AIRPORT         |
+              | TAPACHULA_INTERNATIONAL_AIRPORT |
+              | TAMPA_INTERNATIONAL_AIRPORT     |
+              | ... 5 more                      |
+              |---------------------------------|
+```
+
+## How it's made
+
+The other day, I was making a chat-interface-based trip recommendation app and wanted to add a feature that can search for flights available for booking. My personal choice is definitely [Google Flights](https://flights.google.com) since Google always has the best and most organized data on the web. Therefore, I searched for APIs on Google.
+
+> 🔎 **Search** <br />
+> google flights api
+
+The results? Bad. It seems like they discontinued this service and it now lives in the Graveyard of Google.
+
+> <sup><a href="https://duffel.com/blog/google-flights-api" target="_blank">🧏‍♂️ <b>duffel.com</b></a></sup><br />
+> <sup><i>Google Flights API: How did it work & what happened to it?</i></b>
+>
+> The Google Flights API offered developers access to aggregated airline data, including flight times, availability, and prices. Over a decade ago, Google announced the acquisition of ITA Software Inc. which it used to develop its API. **However, in 2018, Google ended access to the public-facing API and now only offers access through the QPX enterprise product**.
+
+That's awful! I've also looked for free alternatives but their rate limits and pricing are just 😬 (not a good fit/deal for everyone).
+
+<br />
+
+However, Google Flights has their UI – [flights.google.com](https://flights.google.com). So, maybe I could just use Developer Tools to log the requests made and just replicate all of that? Undoubtedly not! Their requests are just full of numbers and unreadable text, so that's not the solution.
+
+Perhaps, we could scrape it? I mean, Google allowed many companies like [Serpapi](https://google.com/search?q=serpapi) to scrape their web just pretending like nothing happened... So let's scrape our own.
+
+> 🔎 **Search** <br />
+> google flights ~~api~~ scraper pypi
+
+Excluding the ones that are not active, I came across [hugoglvs/google-flights-scraper](https://pypi.org/project/google-flights-scraper) on Pypi. I thought to myself: "aint no way this is the solution!"
+
+I checked hugoglvs's code on [GitHub](https://github.com/hugoglvs/google-flights-scraper), and I immediately detected "playwright," my worst enemy. One word can describe it well: slow. Two words? Extremely slow. What's more, it doesn't even run on the **🗻 Edge** because of configuration errors, missing libraries... etc. I could just reverse [try.playwright.tech](https://try.playwright.tech) and use a better environment, but that's just too risky if they added Cloudflare as an additional security barrier 😳.
+
+Life tells me to never give up. Let's just take a look at their URL params...
+
+```markdown
+https://www.google.com/travel/flights/search?tfs=CBwQAhoeEgoyMDI0LTA1LTI4agcIARIDVFBFcgcIARIDTVlKGh4SCjIwMjQtMDUtMzBqBwgBEgNNWUpyBwgBEgNUUEVAAUgBcAGCAQsI____________AZgBAQ&hl=en
+```
+
+| Param | Content | My past understanding |
+|-------|---------|-----------------------|
+| hl    | en      | Sets the language.    |
+| tfs   | CBwQAhoeEgoyMDI0LTA1LTI4agcIARID… | What is this???? 🤮🤮 |
+
+I removed the `?tfs=` parameter and found out that this is the control of our request! And it looks so base64-y.
+
+If we decode it to raw text, we can still see the dates, but we're not quite there — there's too much unwanted Unicode text.
+
+Or maybe it's some kind of a **data-storing method** Google uses? What if it's something like JSON? Let's look it up.
+
+> 🔎 **Search** <br />
+> google's json alternative
+
+> 🐣 **Result**<br />
+> Solution: The Power of **Protocol Buffers**
+> 
+> LinkedIn turned to Protocol Buffers, often referred to as **protobuf**, a binary serialization format developed by Google. The key advantage of Protocol Buffers is its efficiency, compactness, and speed, making it significantly faster than JSON for serialization and deserialization.
+
+Gotcha, Protobuf! Let's feed it to an online decoder and see how it does:
+
+> 🔎 **Search** <br />
+> protobuf decoder
+
+> 🐣 **Result**<br />
+> [protobuf-decoder.netlify.app](https://protobuf-decoder.netlify.app)
+
+I then pasted the Base64-encoded string to the decoder and no way! It DID return valid data!
+
+![annotated, Protobuf Decoder screenshot](https://github.com/AWeirdDev/flights/assets/90096971/77dfb097-f961-4494-be88-3640763dbc8c)
+
+I immediately recognized the values — that's my data, that's my query!
+
+So, I wrote some simple Protobuf code to decode the data.
+
+```protobuf
+syntax = "proto3"
+
+message Airport {
+    string name = 2;
+}
+
+message FlightInfo {
+    string date = 2;
+    Airport dep_airport = 13;
+    Airport arr_airport = 14;
+}
+
+message GoogleSucks {
+    repeated FlightInfo = 3;
+}
+```
+
+It works! Now, I won't consider myself an "experienced Protobuf developer" but rather a complete beginner.
+
+I have no idea what I wrote but... it worked! And here it is, `fast-flights`.
+
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: fast-flights Version: 0.2 Summary: The fast,
+Metadata-Version: 2.1 Name: fast-flights Version: 0.3 Summary: The fast,
 robust, strongly-typed Google Flights scraper (API) implemented in Python.
 Author-email: AWeirdDev
-gmail.com> Project-URL: Homepage, https://github.com/AWeirdScratcher/flights
-Project-URL: Bug Tracker, https://github.com/AWeirdScratcher/flights/issues
-Keywords: flights,google,google-
-flights,scraper,protobuf,travel,trip,passengers,airport Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown Requires-Dist: requests Requires-Dist:
-protobuf Requires-Dist: selectolax
+gmail.com> Project-URL: Homepage, https://github.com/AWeirdDev/flights Project-
+URL: Bug Tracker, https://github.com/AWeirdDev/flights/issues Keywords:
+flights,google,google-flights,scraper,protobuf,travel,trip,passengers,airport
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist:
+requests Requires-Dist: protobuf Requires-Dist: selectolax
    # flights (fast-flights) The fast, robust, strongly-typed Google Flights
  scraper (API) implemented in Python. Based on Base64-encoded Protobuf string.
                    ```haskell $ pip install fast-flights ```
 ## Usage To use `fast-flights`, you'll first create a filter (inherited from
 `?tfs=`) to perform a request. Then, add `flight_data`, `trip`, `seat` and
 `passengers` info to use the API directly. Honorable mention: I like birds.
 Yes, I like birds. ```python from fast_flights import FlightData, Passengers,
```

### Comparing `fast_flights-0.2/pyproject.toml` & `fast_flights-0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-[build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "fast-flights"
-version = "0.2"
-description = "The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python."
-keywords = ["flights", "google", "google-flights", "scraper", "protobuf", "travel", "trip", "passengers", "airport"]
-authors = [
-  { name = "AWeirdDev", email = "aweirdscratcher@gmail.com" },
-]
-license = { file = "LICENSE" }
-readme = "README.md"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-requires-python = ">=3.7"
-dependencies = [
-  "requests",
-  "protobuf",
-  "selectolax"
-]
-
-[project.urls]
-"Homepage" = "https://github.com/AWeirdScratcher/flights"
-"Bug Tracker" = "https://github.com/AWeirdScratcher/flights/issues"
-
-[tool.setuptools]
-packages = [
-    "fast_flights"
+[build-system]
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "fast-flights"
+version = "0.3"
+description = "The fast, robust, strongly-typed Google Flights scraper (API) implemented in Python."
+keywords = ["flights", "google", "google-flights", "scraper", "protobuf", "travel", "trip", "passengers", "airport"]
+authors = [
+  { name = "AWeirdDev", email = "aweirdscratcher@gmail.com" },
+]
+license = { file = "LICENSE" }
+readme = "README.md"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+requires-python = ">=3.7"
+dependencies = [
+  "requests",
+  "protobuf",
+  "selectolax"
+]
+
+[project.urls]
+"Homepage" = "https://github.com/AWeirdDev/flights"
+"Bug Tracker" = "https://github.com/AWeirdDev/flights/issues"
+
+[tool.setuptools]
+packages = [
+    "fast_flights"
 ]
```

