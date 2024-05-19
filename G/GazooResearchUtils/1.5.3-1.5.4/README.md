# Comparing `tmp/GazooResearchUtils-1.5.3.tar.gz` & `tmp/GazooResearchUtils-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.5.3.tar", last modified: Thu May 16 15:55:14 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.5.4.tar", last modified: Sun May 19 23:36:51 2024, max compression
```

## Comparing `GazooResearchUtils-1.5.3.tar` & `GazooResearchUtils-1.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:55:14.890739 GazooResearchUtils-1.5.3/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-16 15:55:14.890489 GazooResearchUtils-1.5.3/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:55:14.888543 GazooResearchUtils-1.5.3/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:55:14.888997 GazooResearchUtils-1.5.3/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)      187 2024-05-16 13:57:19.000000 GazooResearchUtils-1.5.3/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:55:14.890152 GazooResearchUtils-1.5.3/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     8186 2024-05-16 15:55:12.000000 GazooResearchUtils-1.5.3/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.5.3/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:55:14.889719 GazooResearchUtils-1.5.3/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-16 15:55:14.000000 GazooResearchUtils-1.5.3/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-16 15:55:14.000000 GazooResearchUtils-1.5.3/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-16 15:55:14.000000 GazooResearchUtils-1.5.3/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-16 15:55:14.000000 GazooResearchUtils-1.5.3/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-16 15:55:14.000000 GazooResearchUtils-1.5.3/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-16 15:55:14.890789 GazooResearchUtils-1.5.3/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-16 15:55:09.000000 GazooResearchUtils-1.5.3/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.808697 GazooResearchUtils-1.5.4/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:36:51.808461 GazooResearchUtils-1.5.4/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.806529 GazooResearchUtils-1.5.4/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.806933 GazooResearchUtils-1.5.4/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      187 2024-05-16 13:57:19.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.808149 GazooResearchUtils-1.5.4/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     8724 2024-05-19 23:35:05.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-19 23:36:51.807747 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-19 23:36:51.000000 GazooResearchUtils-1.5.4/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-19 23:36:51.808756 GazooResearchUtils-1.5.4/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-19 23:36:19.000000 GazooResearchUtils-1.5.4/setup.py
```

### Comparing `GazooResearchUtils-1.5.3/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.5.4/app/GazooResearchUtils/src/Analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,16 +56,14 @@
   # Remove Duplicates
   dictionary = data.drop_duplicates()
   # Sort
   dictionary = dictionary.sort_values(['icd10', 'tag', 'field'], ascending=[True, True, True])
 
   return dictionary
 
-
-
 def pt_dates_and_events(df, start_tag, event_tags, occurance=0):
   """
   Determines starting date, date of event occurence or data censoring, and whether
   event occured or data was censored
 
   Parameters:
   data (DataFrame): dataframe for patient
@@ -79,15 +77,15 @@
       starting event
   event (int): 1 if event occurred, 0 if data censored; None if no starting event
   """
   # Convert String to Date
   convert_date = lambda date: datetime.strptime(date, '%Y-%m-%d')
 
   # Get Start Dates
-  test = get_data_filter(df, start_tag)
+  test = get_tags_where_filter(df, start_tag)
   start_dates = test.loc[(test['field']=='date')]['value'].to_numpy()
   start_dates = np.array(list(map(convert_date, start_dates)))
   start_dates = np.unique(start_dates)  # Remove Duplicates
   start_dates = np.sort(start_dates)  # Sort
 
   # Set Start Date
   if len(start_dates) >=1:
@@ -95,15 +93,15 @@
   else:
     # Return None if no start date
     return None, None, None
 
   # Get Event Dates
   event_dates = []
   for event_tag in event_tags:
-    test = get_data_filter(df, event_tag)
+    test = get_tags_where_filter(df, event_tag)
     events = test.loc[(test['field']=='date')]['value'].to_numpy()
     events = list(map(convert_date, events))
     # Append Dates
     event_dates = event_dates + events
 
   # Event Dates
   event_dates = np.asarray(event_dates)
@@ -124,51 +122,58 @@
   censor_dates = list(map(convert_date, censor_dates))
   censor_dates = np.sort(censor_dates) # sort
   last = censor_dates[-1]
   event = 0
 
   return start, last, event
 
-def get_data_filter(pt, filter):
+def get_tags_where_filter(pt, filter):
   """
-  Get filter if exists in dataframe
+  Get tags where filter criteria exists
 
   Parameters:
   data (DataFrame): dataframe
   filter (list of dicts): Structure of filter {'icd10':str, 'tag': str, 'field': str, 'exact': [str, str,...], 'between': [float, float]}
 
   Returns:
-  data (DataFrame): dataframe with filters
+  data (DataFrame): dataframe with tags where filter criteria exist
 
   """
-  if "value" in filter and "field" in filter and "tag" in filter and "icd10" in filter:
-    test = pt.loc[(pt['icd10'] == filter['icd10'])
-      & (pt['tag'] == filter['tag'])
-      & (pt['field'] == filter['field'])
-      & (pt['value'].isin(filter['value']))]
+  if "exact" in filter and "field" in filter and "tag" in filter and "icd10" in filter:
+    test = pt.loc[(pt['icd10'].astype(str) == filter['icd10'])
+      & (pt['tag'].astype(str) == filter['tag'])
+      & (pt['field'].astype(str) == filter['field'])
+      & (pt['value'].isin(filter['exact']))]
+    # Get Tags where tag_id
+    test = pt.loc[(pt['tag_id'].astype(str).isin(test.tag_id))]
   elif "between" in filter and "field" in filter and "tag" in filter and "icd10" in filter:
-    test = pt.loc[(pt['icd10'] == filter['icd10'])
-      & (pt['tag'] == filter['tag'])
-      & (pt['field'] == filter['field'])]
-    test = pd.to_numeric(test['value']).between(filter['between'][0], filter['between'][1])
+    test = pt.loc[(pt['icd10'].astype(str) == filter['icd10'])
+      & (pt['tag'].astype(str) == filter['tag'])
+      & (pt['field'].astype(str) == filter['field'])]
+    # Check Value
+    check = pd.to_numeric(test['value']).between(filter['between'][0], filter['between'][1])
+    # Get Tags where tag_id
+    test = pt.loc[pt['tag_id'].isin(test[check].tag_id)]
   elif "field" in filter and "tag" in filter and "icd10" in filter:
-    test = pt.loc[(pt['icd10'] == filter['icd10'])
-      & (pt['tag'] == filter['tag'])
-      & (pt['field'] == filter['field'])]
+    test = pt.loc[(pt['icd10'].astype(str) == filter['icd10'])
+      & (pt['tag'].astype(str) == filter['tag'])
+      & (pt['field'].astype(str) == filter['field'])]
+    test = pt.loc[(pt['tag_id'].astype(str).isin(test.tag_id))]
   elif "tag" in filter and "icd10" in filter:
-    test = pt.loc[(pt['icd10'] == filter['icd10'])
-      & (pt['tag'] == filter['tag'])]
+    test = pt.loc[(pt['icd10'].astype(str) == filter['icd10'])
+      & (pt['tag'].astype(str) == filter['tag'])]
   elif "icd10" in filter:
-    test = pt.loc[(pt['icd10'] == filter['icd10'])]
+    test = pt.loc[(pt['icd10'].astype(str) == filter['icd10'])]
+  elif "tag" in filter:
+    test = pt.loc[(pt['tag'].astype(str) == filter['tag'])]
   else:
     test = pd.DataFrame()
 
   return test
 
-
 def filter(data, filters):
   """
   Only include patients that matches the filter
 
   Parameters:
   data (DataFrame): dataframe with csv data
   filters (list of dicts): list of possible filters. Structure of filter {'icd10':str, 'tag': str, 'field': str, 'exact': [str, str,...], 'between': [float, float]}
@@ -186,15 +191,15 @@
     pt = data.loc[(data['id'] == mrn)]
 
     # Loop Through Conditions
     #print(filters)
     valid = []
     for filter in filters:
       # Get filter
-      test = get_data_filter(pt, filter)
+      test = get_tags_where_filter(pt, filter)
 
       # Is filter apply
       if len(test.index) >= 1: valid.append(True)
       else: valid.append(False)
 
     # Append mrn to list if all filters apply
     if all(valid):
```

