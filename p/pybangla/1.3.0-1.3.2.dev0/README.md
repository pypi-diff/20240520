# Comparing `tmp/pybangla-1.3.0.tar.gz` & `tmp/pybangla-1.3.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-1.3.0.tar", last modified: Thu May 16 19:00:04 2024, max compression
+gzip compressed data, was "pybangla-1.3.2.dev0.tar", last modified: Mon May 20 12:48:03 2024, max compression
```

## Comparing `pybangla-1.3.0.tar` & `pybangla-1.3.2.dev0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:00:04.533579 pybangla-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:59:58.000000 pybangla-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20331 2024-05-16 19:00:04.533579 pybangla-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19713 2024-05-16 18:59:58.000000 pybangla-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:00:04.529579 pybangla-1.3.0/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:00:04.533579 pybangla-1.3.0/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    27661 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-05-16 18:59:58.000000 pybangla-1.3.0/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:00:04.533579 pybangla-1.3.0/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20331 2024-05-16 19:00:04.000000 pybangla-1.3.0/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-16 19:00:04.000000 pybangla-1.3.0/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:00:04.000000 pybangla-1.3.0/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 19:00:04.000000 pybangla-1.3.0/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 19:00:04.000000 pybangla-1.3.0/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:00:04.533579 pybangla-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-16 18:59:58.000000 pybangla-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:00:04.533579 pybangla-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-16 18:59:58.000000 pybangla-1.3.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19713 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.511443 pybangla-1.3.2.dev0/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28329 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/tests/test.py
```

### Comparing `pybangla-1.3.0/PKG-INFO` & `pybangla-1.3.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.3.0
+Version: 1.3.2.dev0
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.3.0/README.md` & `pybangla-1.3.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.0/pybangla/matching.py` & `pybangla-1.3.2.dev0/pybangla/matching.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.0/pybangla/module/config.py` & `pybangla-1.3.2.dev0/pybangla/module/config.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.0/pybangla/module/date_extractor.py` & `pybangla-1.3.2.dev0/pybangla/module/date_extractor.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.0/pybangla/module/main.py` & `pybangla-1.3.2.dev0/pybangla/module/main.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.0/pybangla/module/number_parser.py` & `pybangla-1.3.2.dev0/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.0/pybangla/module/parser.py` & `pybangla-1.3.2.dev0/pybangla/module/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         
         """
         # print("number  : ", number, language)
 
         if language=="en":
             extracted_number = list(re.finditer(self.bn_regex, str(number), re.UNICODE))
             if extracted_number:
-                print("language", number)
+                # print("language", number)
                 # [i[1] for i in number if i[0]=="0"]
                 if number[0]=="0":
                     number = number[1:]
                 number = "".join([cfg._bangla2english_digits_mapping[i.replance(",", "")] for i in number if i[0]=="0"])
                 # print("extracted : ", number)
         c_number = ""
         for n in number:
@@ -151,30 +151,37 @@
     
     def get_weekday(self, date_:list=[], language="bn"):
 
         """
         Get weekday name Bangla or English
         
         """
-        if date_[0] is None or date_[1] is None or  date_[2] is None:
-            return None
-        
-        d, y = list(re.finditer(self.bn_regex, str(date_[0]), re.UNICODE)), list(re.finditer(self.bn_regex, str(date_[2]), re.UNICODE))
-        
-        if d:
-            date_[0] = self._digit_converter(date_[0], language="bn")
-        if y:
-            date_[2] = self._digit_converter(date_[2], language="bn")
-
-        current_date_object = datetime.datetime(int(date_[2]), int(date_[1]), int(date_[0]))
-        if language in data:
-            weekday = data[language]["weekdays"][current_date_object.weekday()]
-        else:
-            print("language not handel")
-            weekday = ""
+
+        # print("date_", date_)
+        try:
+            if date_[0] is None or date_[1] is None or  date_[2] is None:
+                return None
+            elif date_[1].isdigit():
+                if int(date_[1])> 12:
+                    return None
+            d, y = list(re.finditer(self.bn_regex, str(date_[0]), re.UNICODE)), list(re.finditer(self.bn_regex, str(date_[2]), re.UNICODE))
+            
+            if d:
+                date_[0] = self._digit_converter(date_[0], language="bn")
+            if y:
+                date_[2] = self._digit_converter(date_[2], language="bn")
+
+            current_date_object = datetime.datetime(int(date_[2]), int(date_[1]), int(date_[0]))
+            if language in data:
+                weekday = data[language]["weekdays"][current_date_object.weekday()]
+            else:
+                print("language not handel")
+                weekday = ""
+        except:
+            weekday = None
         # print("weekday : ", weekday)
         return weekday
     
     def search_month(self, search_key, language="bn"):
         """
         Search for a month or month abbreviation in the month_data dictionary.
         
@@ -185,19 +192,21 @@
         
         Returns:
             list: A list containing additional information about the month if found, 
             formatted based on the specified language. 
             The list contains [month_name, season_name, number_of_days].
             If the month or abbreviation is not found, returns [None, None, None].
         """
-        search_key = int(self._replace_starting_zero(search_key))-1
-        month = data[language]["months"][search_key]
-        seasons = data[language]["seasons"][search_key//2]
-        option_name = data[language]["option_name"][search_key]
-
+        try:
+            search_key = int(self._replace_starting_zero(search_key))-1
+            month = data[language]["months"][search_key]
+            seasons = data[language]["seasons"][search_key//2]
+            option_name = data[language]["option_name"][search_key]
+        except:
+            month, option_name, seasons = None, None, None
         return [month, option_name, seasons]
     
     
     def find_word_index(self, text:str, word:str)->list:
         """
         Word spanning position
         """
@@ -352,14 +361,16 @@
                 year = date_list[idx]
                 # print(year)
                 day, month = self.get_day_and_month(year_idx, idx, date_list)
                 # print(day, month)
         return [day, month, year]
     
     def date_processing(self, date_, language="bn"):
+
+        # print(date_)
         if isinstance(date_, list):
             if len(date_):
                 formatted_date = date_
         else:
             split_date = self.data_splitter(date_)
             # print("split_date : ", split_date)
             split_date = [i for i in split_date if i]
@@ -597,14 +608,16 @@
     
     def replance_date_processing(self, text):
         text = self.extract_year(text)
         original_text = text
         r_text = text
         # print("original_text : ", original_text)
         dates = dt.get_dates(text)
+
+        # print("dates : ", dates)
         # print("+++++++++++++++++++++++++++ date :++++++++++++++++++++++++", dates)
         for date in dates:
             r_date = date
             # spanning_position = self.npr.find_word_index(text, date)
             # print(spanning_position)
             date = self.add_spaces_to_numbers(date)
             # print("date:", date)
@@ -619,36 +632,44 @@
                 for k, v in formated_date.items():
                     if v in date_list:
                         key = k if "txt" in k else f"txt_{k}"
                         index = date_list.index(v)
                         date_list[index] = formated_date[key]
 
                 process_date = " ".join(date_list).strip()
-                original_text = original_text.replace(r_date, " "+process_date+" ")
+                # print("process_date", process_date)
+                if process_date.isdigit():
+                    continue
+                else:
+                    original_text = original_text.replace(r_date, " "+process_date+" ")
                 # search for only year
         
         _only_years = re.findall(self.year_pattern, original_text)
         # print(_only_years)
         for y in _only_years:
-            original_text = original_text.replace(y, " " +self.npr.year_in_number(y) + " ")
+            if y.isdigit():
+                continue
+            else:
+                original_text = original_text.replace(y, " " +self.npr.year_in_number(y) + " ")
         return original_text
 
     
 
     def processing(self, text):
         text = self.exception_year_processing(text)
         text = self.unwanted_puntuation_removing(text)
         text = self.expand_symbols(text)
         text = self.expand_abbreviations(text)
         text = self.expand_position(text)
         text = self.extract_currency_amounts(text)
         text = self.replance_date_processing(text)
         # handel the exception year like 2017-18
-        
 
+        # print("text : ", text)
+        
         text = self.npr.number_processing(text)
         text = self.collapse_whitespace(text)
         return text
     
 
 class EmojiRemoval:
```

### Comparing `pybangla-1.3.0/pybangla/module/word_to_number.py` & `pybangla-1.3.2.dev0/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.0/pybangla/test.py` & `pybangla-1.3.2.dev0/pybangla/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 import time
 from module.main import Normalizer
 
 if __name__ == "__main__":
 
 
     # # Testing Date format
-    date_list = [
+    # date_list = [
     #     "০১-এপ্রিল/২০২৩",
     #     "সেপ্টেম্বর ০৫ ২০২৩",
-        "01-Apr/2023"
+        # "01-Apr/2023"
         # "এপ্রিল ২০২৩" 
         # "2023-04-05",  
         # "06-04-2023", 
         # "04/01/2023",  
         # "07 April, 2023", 
         # "Apr 1, 2023",  
         # "2023/04/01", 
         # "01-Apr-2023", 
         # "01-Apr/2023",  
         # "20230401",  
         # "20042024",
         # "20230401",
         # ["1", "4", "2025"]
-    ]
+    # ]
     # # # # number = "123456" or "২০২৩"
     # # number = "২০২৩"
     nrml = Normalizer()
-    # # # # print("++++++++++++++++++++ Date testing ++++++++++++++++++++++")
-    # # # print("Date format Testing : ", end ="", flush=True)
-    for date_ in date_list:
-        start_time = time.time()
-        print("date_:", date_)
-        formated_date = nrml.date_format(date_, language="en")
-        print(formated_date)
-    # print("++++++++++++++++++++ end of Date testing ++++++++++++++++++++++")
-
-    # print("++++++++++++++++++++ en number to bn number convert ++++++++++++++++++++++")
-    number = "1234"
-    number = nrml.number_convert(number, language="en")
+    # # # # # print("++++++++++++++++++++ Date testing ++++++++++++++++++++++")
+    # # # # print("Date format Testing : ", end ="", flush=True)
+    # for date_ in date_list:
+    #     start_time = time.time()
+    #     print("date_:", date_)
+    #     formated_date = nrml.date_format(date_, language="en")
+    #     print(formated_date)
+    # # print("++++++++++++++++++++ end of Date testing ++++++++++++++++++++++")
+
+    # # print("++++++++++++++++++++ en number to bn number convert ++++++++++++++++++++++")
+    # number = "1234"
+    # number = nrml.number_convert(number, language="en")
     
     
     # number = nrml.number_convert(number, language="bn")
 
-    print("Bn Number : ", number)
+    # print("Bn Number : ", number)
     # print("++++++++++++++++++++ stop number convert ++++++++++++++++++++++")
 
     # # print("++++++++++++++++ Today +++++++++++++++++++++")
     # today_date = nrml.today(language="bn")
     # # today_date = nrml.today(language="en")
     # print(today_date)
 
@@ -216,25 +216,26 @@
     # " সাঃ কিমি হাফিক বিডিটি এয়ারলাইনসসহ তিনটি এয়ারলাইনসের ৫১টি কিমি. ফ্লাইটে মোট ২০ হাজার ২৯১ জন হজযাত্রী সৌদি আরবে গেছেন। এ বছর হজ করতে ৮৫ হাজার ২৫৭ জনের সৌদি আরবে যাওয়ার কথা রয়েছে। ৫ম",
     # "প্রদর্শনীটি চলার কথা ছিল ১২ মে পর্যন্ত, তবে দর্শকদের ব্যাপক আগ্রহের কারণে তিন দিন সময় বাড়িয়ে ১৫ মে পর্যন্ত করা হয়েছিল ১৫.১৫",
     # "The numbers are 10 নন-ক্যাডার 20.5  30, and 40.75. সুপারিশ ২০৩০.৩০ 12 23 45",
     # "[১৯৯৬]-সালের-৬:তারিখে-নির্ধারিত করা হয়েছে"
     # ]
 
     # # solving steps is have number need to give extra space both side
-    # issue = [
+    issue = [
     # "[১৯৯৬]-সালের-৬:তারিখে-নির্ধারিত করা হয়েছে.",
     # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর",
     # "আজকের তাপমাত্রা ৪৪°F",
     # "আজকের তাপমাত্রা ৪৪°C",
     # "যেমন ১৯৬১ সালে দেশটির তৎকালীন প্রেসিডেন্ট ডোয়াইট ডি আইজেনহাওয়ার শিক্ষা খাতে সামরিক শিল্পের প্রবেশের বিপদ নিয়ে সতর্ক করেছিলেন।",
-    # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর"
-    # ]
+    # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর",
+    "উদাহরণস্বরূপ, আপনার মোটরযানের রেজিস্ট্রেশন নাম্বার ঢাকা মেট্রো-গ-12-1212 এবং টাকা জমা রশিদের ট্রানজেকশন নাম্বার 2001011325989"
+    ]
 
 
 
-    # for i in issue:
+    for i in issue:
 
-    #     print("input : ", i)
-    #     text = nrml.text_normalizer(i)
-    #     print("output : ", text)
-    #     print("+"*40)
+        print("input : ", i)
+        text = nrml.text_normalizer(i)
+        print("output : ", text)
+        print("+"*40)
```

### Comparing `pybangla-1.3.0/pybangla.egg-info/PKG-INFO` & `pybangla-1.3.2.dev0/pybangla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.3.0
+Version: 1.3.2.dev0
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.3.0/setup.py` & `pybangla-1.3.2.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='1.3.0',
+    version='1.3.2-dev',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-1.3.0/tests/test.py` & `pybangla-1.3.2.dev0/tests/test.py`

 * *Files identical despite different names*

