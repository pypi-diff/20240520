# Comparing `tmp/hot_spot_analysis-0.1.4.tar.gz` & `tmp/hot_spot_analysis-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hot_spot_analysis-0.1.4.tar", max compression
+gzip compressed data, was "hot_spot_analysis-1.0.2.tar", max compression
```

## Comparing `hot_spot_analysis-0.1.4.tar` & `hot_spot_analysis-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-02-27 06:08:25.820723 hot_spot_analysis-0.1.4/LICENSE
--rw-r--r--   0        0        0     5165 2023-02-28 07:42:03.099596 hot_spot_analysis-0.1.4/README.md
--rw-r--r--   0        0        0       35 2023-02-05 21:14:53.032189 hot_spot_analysis-0.1.4/hot_spot_analysis/__init__.py
--rw-r--r--   0        0        0    16666 2023-02-28 07:07:36.335280 hot_spot_analysis-0.1.4/hot_spot_analysis/hot_spot_analysis.py
--rw-r--r--   0        0        0      465 2023-02-28 07:46:10.859932 hot_spot_analysis-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6028 1970-01-01 00:00:00.000000 hot_spot_analysis-0.1.4/setup.py
--rw-r--r--   0        0        0     5795 1970-01-01 00:00:00.000000 hot_spot_analysis-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-08 19:09:05.390182 hot_spot_analysis-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5164 2023-04-08 19:09:05.390418 hot_spot_analysis-1.0.2/README.md
+-rw-r--r--   0        0        0      512 2024-05-19 23:16:33.144203 hot_spot_analysis-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 21:29:20.208895 hot_spot_analysis-1.0.2/src/hot_spot_analysis/__init__.py
+-rw-r--r--   0        0        0    16706 2024-05-19 23:15:25.854133 hot_spot_analysis-1.0.2/src/hot_spot_analysis/hot_spot_analysis.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:29:20.211324 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-15 21:29:20.211724 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/analyze.py
+-rw-r--r--   0        0        0     1230 2024-05-15 21:29:20.212762 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/combos.py
+-rw-r--r--   0        0        0      454 2024-05-15 21:29:20.213727 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/demo.py
+-rw-r--r--   0        0        0      717 2024-05-15 21:29:20.214515 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/general.py
+-rw-r--r--   0        0        0     1654 2024-05-15 21:29:20.215885 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/grouped_df.py
+-rw-r--r--   0        0        0     3032 2024-05-15 21:29:20.216918 hot_spot_analysis-1.0.2/src/hot_spot_analysis/utils/lists.py
+-rw-r--r--   0        0        0     5909 1970-01-01 00:00:00.000000 hot_spot_analysis-1.0.2/PKG-INFO
```

### Comparing `hot_spot_analysis-0.1.4/LICENSE` & `hot_spot_analysis-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hot_spot_analysis-0.1.4/README.md` & `hot_spot_analysis-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,35 +7,35 @@
 ## Future updates plan to add the following functionality:
 - multiprocessing to improve module calculation speed
 - support for non-dataframe user functions (graphs, etc.)
 
 
 ## Short Theoretical Demonstration:
 
-If we have 3 columns [a, b, c], and we want to cut our data using those columns we would have to group our data as such to know all of the interactions' impact on our metric of interst. And this problem becomes increasingly complicated as we increase the number of columns. 
+If we have 3 columns [a, b, c], and we want to cut our data using those columns we would have to group our data as such to know all of the interactions' impact on our metric of interest. And this problem becomes increasingly complicated as we increase the number of columns. 
 
 **Using 3 columns:**
 [a, b, c] -> 7 valid data cuts
   - @ depth = 1: [a,b,c] <- 3 data cuts
   - @ depth = 2: [ab,ac,bc] <- 3 data cuts
   - @ depth = 3: [abc] <- 1 data cuts
 
 **HSA Output Data Structure:**
 
 | index | depth | data_cuts         | data_content        | data_cut_content      | user function output |
 | ----- | ----- | ----------------- | ------------------- | --------------------- | -------------------- |
 | 1     | 1     | [column a]        | [row_value x]       | ['a:x']               | [Int/float/etc.]     |
 | 2     | 1     | [column b]        | [row_value y]       | ['b:y']               | [Int/float/etc.]     |
-| 3     | 1     | [column c]        | [row_value z]       | ['b:y']               | [Int/float/etc.]     |
+| 3     | 1     | [column c]        | [row_value z]       | ['c:z']               | [Int/float/etc.]     |
 | 4     | 2     | [Columns a, b]    | [row_value x, y]    | ['a:x', 'b:y']        | [Int/float/etc.]     |
 | 5     | 2     | [Columns a, c]    | [row_value x, z]    | ['a:x', 'c:z']        | [Int/float/etc.]     |
-| 6     | 2     | [Columns c, b]    | [row_value y, z]    | ['b:y', 'c:z']        | [Int/float/etc.]     |
+| 6     | 2     | [Columns b, c]    | [row_value y, z]    | ['b:y', 'c:z']        | [Int/float/etc.]     |
 | 7     | 3     | [Columns a, b, c] | [row_value x, y, z] | ['a:x', 'b:y', 'c:z'] | [Int/float/etc.]     |
 
-***Note:*** Each column yields X rows equal determined by number of unique values. Thus 'ab' woudl yield a<sub>N</sub> * b<sub>M</sub> rows in the output where column a has N unique values, and column B has M unique values thus ab yields N*M rows.
+***Note:*** Each column yields X rows determined by the number of unique values. Thus 'ab' would yield a<sub>N</sub> * b<sub>M</sub> rows in the output where column a has N unique values, and column B has M unique values thus ab yields N*M rows.
 
 
 # An Example:
 
 Using the titanic data from seaborn we can look at a semi-practical example using some data.
 
 | survived | class | adult_male | embark_town |
```

### Comparing `hot_spot_analysis-0.1.4/setup.py` & `hot_spot_analysis-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,160 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hot-spot-analysis
+Version: 1.0.2
+Summary: A generalized method to find hot spots in your metrics without requiring regressions. Jumpstart a regression analysis or provide deeper insights to stakeholders.
+License: MIT
+Author: Philip Gundy
+Author-email: philipgundy@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['hot_spot_analysis']
 
-package_data = \
-{'': ['*']}
+# Overview
+tldr: Do you hate trying to breakdown which underlying trends or movements are driving topline metric movements? HSA can solve that.
+
+Hot Spot Analysis (HSA) is an analytic reporting framework that removes any statitical ambiguity. HSA is meant to enhance reporting, find insights, and easily dive further into the 'why' metrics have shifted. This is done by automatically running all viable cuts within the data across the provided features for any metrics.
+
+## Future updates plan to add the following functionality:
+- multiprocessing to improve module calculation speed
+- support for non-dataframe user functions (graphs, etc.)
+
+
+## Short Theoretical Demonstration:
+
+If we have 3 columns [a, b, c], and we want to cut our data using those columns we would have to group our data as such to know all of the interactions' impact on our metric of interest. And this problem becomes increasingly complicated as we increase the number of columns. 
+
+**Using 3 columns:**
+[a, b, c] -> 7 valid data cuts
+  - @ depth = 1: [a,b,c] <- 3 data cuts
+  - @ depth = 2: [ab,ac,bc] <- 3 data cuts
+  - @ depth = 3: [abc] <- 1 data cuts
+
+**HSA Output Data Structure:**
+
+| index | depth | data_cuts         | data_content        | data_cut_content      | user function output |
+| ----- | ----- | ----------------- | ------------------- | --------------------- | -------------------- |
+| 1     | 1     | [column a]        | [row_value x]       | ['a:x']               | [Int/float/etc.]     |
+| 2     | 1     | [column b]        | [row_value y]       | ['b:y']               | [Int/float/etc.]     |
+| 3     | 1     | [column c]        | [row_value z]       | ['c:z']               | [Int/float/etc.]     |
+| 4     | 2     | [Columns a, b]    | [row_value x, y]    | ['a:x', 'b:y']        | [Int/float/etc.]     |
+| 5     | 2     | [Columns a, c]    | [row_value x, z]    | ['a:x', 'c:z']        | [Int/float/etc.]     |
+| 6     | 2     | [Columns b, c]    | [row_value y, z]    | ['b:y', 'c:z']        | [Int/float/etc.]     |
+| 7     | 3     | [Columns a, b, c] | [row_value x, y, z] | ['a:x', 'b:y', 'c:z'] | [Int/float/etc.]     |
+
+***Note:*** Each column yields X rows determined by the number of unique values. Thus 'ab' would yield a<sub>N</sub> * b<sub>M</sub> rows in the output where column a has N unique values, and column B has M unique values thus ab yields N*M rows.
+
+
+# An Example:
+
+Using the titanic data from seaborn we can look at a semi-practical example using some data.
+
+| survived | class | adult_male | embark_town |
+| -------- | ----- | ---------- | ----------- |
+| 0        | Third | True       | Southampton |
+| 1        | First | False      | Cherbourg   |
+| 1        | First | False      | Southampton |
+| 0        | Third | True       | Queenstown  |
+*for each of the 891 passengers on the titanic*
+
+
+
+## A Simple Example Using hot_spot_analysis:
+```
+import numpy as np
+import pandas as pd
+import seaborn as sb
+from hot_spot_analysis.hot_spot_analysis import HotSpotAnalysis
+
+# Load our data
+df = sb.load_dataset('titanic')
+titanic = df[['survived', 'class',  'adult_male', 'embark_town']]
+
+# Define our metric function
+def survival_rate(data):
+    temp = data.agg(survival_rate = pd.NamedAgg('survived', np.mean))
+    return temp
+
+# Input our data cuts, depth limit, and data
+hsa = HotSpotAnalysis(
+    data_cuts=['class',  'adult_male', 'embark_town'],
+    depth_limit = 3,
+    data = titanic
+)
+
+# Run the hot spot analysis
+hsa.run_hsa(survival_rate)
+
+# Export the data
+hsa_output = hsa.get_hsa_data() # export the analysis results
+
+# Review some of the features
+print(hsa_output.head())
+print(hsa_output.tail())
+
+# Or use some of the built in search features
+hsa.search_hsa_data(
+    target_var = 'data_content', 
+    search_terms = 'Southampton'
+    )
+
+```
+
+
+## A (mostly) pandas example without hot_spot_analysis:
+
+Does using hot_spot_analysis actually make life that much easier?
+YES.
+
+Looking at the following for 
+
+```
+import numpy as np
+import pandas as pd
+import seaborn as sb
+
+df = sb.load_dataset('titanic')
+titanic = df[['survived', 'class',  'adult_male', 'embark_town']]
+
+def survival_rate(data):
+    temp = data.agg(survival_rate = pd.NamedAgg('survived', np.mean))
+    return temp
+
+titanic_by_class = survival_rate(titanic.groupby('class'))
+titanic_by_adult_male = survival_rate(titanic.groupby('adult_male'))
+titanic_by_embark_town = survival_rate(titanic.groupby('embark_town'))
+titanic_by_class_adult_male = survival_rate(titanic.groupby(['class', 'adult_male']))
+titanic_by_class_embark_town = survival_rate(titanic.groupby(['class', 'embark_town']))
+titanic_by_adult_male_embark_town = survival_rate(titanic.groupby(['adult_male', 'embark_town']))
+titanic_by_all = survival_rate(titanic.groupby(['class', 'adult_male', 'embark_town']))
+
+# Combine the data frames
+dfs = [
+    titanic_by_class,
+    titanic_by_adult_male,
+    titanic_by_embark_town,
+    titanic_by_class_adult_male,
+    titanic_by_class_embark_town,
+    titanic_by_adult_male_embark_town,
+    titanic_by_all
+]
+
+all_df = pd.concat(dfs, join='outer', axis=1).fillna(np.NaN)
+
+# Review some of the features
+print(all_df.head())
+print(all_df.tail())
+
+
+
+```
 
-install_requires = \
-['numpy>=1.21', 'pandas>=1.3.5', 'seaborn>=0.12.2,<0.13.0']
-
-setup_kwargs = {
-    'name': 'hot-spot-analysis',
-    'version': '0.1.4',
-    'description': 'Compute metrics across combinations of features. Stop clicking around in tableau.',
-    'long_description': "\n# Overview\ntldr: Do you hate trying to breakdown which underlying trends or movements are driving topline metric movements? HSA can solve that.\n\nHot Spot Analysis (HSA) is an analytic reporting framework that removes any statitical ambiguity. HSA is meant to enhance reporting, find insights, and easily dive further into the 'why' metrics have shifted. This is done by automatically running all viable cuts within the data across the provided features for any metrics.\n\n## Future updates plan to add the following functionality:\n- multiprocessing to improve module calculation speed\n- support for non-dataframe user functions (graphs, etc.)\n\n\n## Short Theoretical Demonstration:\n\nIf we have 3 columns [a, b, c], and we want to cut our data using those columns we would have to group our data as such to know all of the interactions' impact on our metric of interst. And this problem becomes increasingly complicated as we increase the number of columns. \n\n**Using 3 columns:**\n[a, b, c] -> 7 valid data cuts\n  - @ depth = 1: [a,b,c] <- 3 data cuts\n  - @ depth = 2: [ab,ac,bc] <- 3 data cuts\n  - @ depth = 3: [abc] <- 1 data cuts\n\n**HSA Output Data Structure:**\n\n| index | depth | data_cuts         | data_content        | data_cut_content      | user function output |\n| ----- | ----- | ----------------- | ------------------- | --------------------- | -------------------- |\n| 1     | 1     | [column a]        | [row_value x]       | ['a:x']               | [Int/float/etc.]     |\n| 2     | 1     | [column b]        | [row_value y]       | ['b:y']               | [Int/float/etc.]     |\n| 3     | 1     | [column c]        | [row_value z]       | ['b:y']               | [Int/float/etc.]     |\n| 4     | 2     | [Columns a, b]    | [row_value x, y]    | ['a:x', 'b:y']        | [Int/float/etc.]     |\n| 5     | 2     | [Columns a, c]    | [row_value x, z]    | ['a:x', 'c:z']        | [Int/float/etc.]     |\n| 6     | 2     | [Columns c, b]    | [row_value y, z]    | ['b:y', 'c:z']        | [Int/float/etc.]     |\n| 7     | 3     | [Columns a, b, c] | [row_value x, y, z] | ['a:x', 'b:y', 'c:z'] | [Int/float/etc.]     |\n\n***Note:*** Each column yields X rows equal determined by number of unique values. Thus 'ab' woudl yield a<sub>N</sub> * b<sub>M</sub> rows in the output where column a has N unique values, and column B has M unique values thus ab yields N*M rows.\n\n\n# An Example:\n\nUsing the titanic data from seaborn we can look at a semi-practical example using some data.\n\n| survived | class | adult_male | embark_town |\n| -------- | ----- | ---------- | ----------- |\n| 0        | Third | True       | Southampton |\n| 1        | First | False      | Cherbourg   |\n| 1        | First | False      | Southampton |\n| 0        | Third | True       | Queenstown  |\n*for each of the 891 passengers on the titanic*\n\n\n\n## A Simple Example Using hot_spot_analysis:\n```\nimport numpy as np\nimport pandas as pd\nimport seaborn as sb\nfrom hot_spot_analysis.hot_spot_analysis import HotSpotAnalysis\n\n# Load our data\ndf = sb.load_dataset('titanic')\ntitanic = df[['survived', 'class',  'adult_male', 'embark_town']]\n\n# Define our metric function\ndef survival_rate(data):\n    temp = data.agg(survival_rate = pd.NamedAgg('survived', np.mean))\n    return temp\n\n# Input our data cuts, depth limit, and data\nhsa = HotSpotAnalysis(\n    data_cuts=['class',  'adult_male', 'embark_town'],\n    depth_limit = 3,\n    data = titanic\n)\n\n# Run the hot spot analysis\nhsa.run_hsa(survival_rate)\n\n# Export the data\nhsa_output = hsa.get_hsa_data() # export the analysis results\n\n# Review some of the features\nprint(hsa_output.head())\nprint(hsa_output.tail())\n\n# Or use some of the built in search features\nhsa.search_hsa_data(\n    target_var = 'data_content', \n    search_terms = 'Southampton'\n    )\n\n```\n\n\n## A (mostly) pandas example without hot_spot_analysis:\n\nDoes using hot_spot_analysis actually make life that much easier?\nYES.\n\nLooking at the following for \n\n```\nimport numpy as np\nimport pandas as pd\nimport seaborn as sb\n\ndf = sb.load_dataset('titanic')\ntitanic = df[['survived', 'class',  'adult_male', 'embark_town']]\n\ndef survival_rate(data):\n    temp = data.agg(survival_rate = pd.NamedAgg('survived', np.mean))\n    return temp\n\ntitanic_by_class = survival_rate(titanic.groupby('class'))\ntitanic_by_adult_male = survival_rate(titanic.groupby('adult_male'))\ntitanic_by_embark_town = survival_rate(titanic.groupby('embark_town'))\ntitanic_by_class_adult_male = survival_rate(titanic.groupby(['class', 'adult_male']))\ntitanic_by_class_embark_town = survival_rate(titanic.groupby(['class', 'embark_town']))\ntitanic_by_adult_male_embark_town = survival_rate(titanic.groupby(['adult_male', 'embark_town']))\ntitanic_by_all = survival_rate(titanic.groupby(['class', 'adult_male', 'embark_town']))\n\n# Combine the data frames\ndfs = [\n    titanic_by_class,\n    titanic_by_adult_male,\n    titanic_by_embark_town,\n    titanic_by_class_adult_male,\n    titanic_by_class_embark_town,\n    titanic_by_adult_male_embark_town,\n    titanic_by_all\n]\n\nall_df = pd.concat(dfs, join='outer', axis=1).fillna(np.NaN)\n\n# Review some of the features\nprint(all_df.head())\nprint(all_df.tail())\n\n\n\n```\n\n\n",
-    'author': 'Philip Gundy',
-    'author_email': 'philipgundy@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1',
-}
 
 
-setup(**setup_kwargs)
```

