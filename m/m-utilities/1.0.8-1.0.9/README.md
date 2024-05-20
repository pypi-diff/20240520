# Comparing `tmp/m-utilities-1.0.8.tar.gz` & `tmp/m-utilities-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-utilities-1.0.8.tar", last modified: Mon Oct 16 09:09:35 2023, max compression
+gzip compressed data, was "m-utilities-1.0.9.tar", last modified: Wed Jan  3 07:43:02 2024, max compression
```

## Comparing `m-utilities-1.0.8.tar` & `m-utilities-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 09:09:35.663391 m-utilities-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1046 2023-10-16 09:09:35.662391 m-utilities-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2023-10-16 09:06:41.000000 m-utilities-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 09:09:35.661391 m-utilities-1.0.8/m_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1046 2023-10-16 09:09:35.000000 m-utilities-1.0.8/m_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-10-16 09:09:35.000000 m-utilities-1.0.8/m_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 09:09:35.000000 m-utilities-1.0.8/m_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      187 2023-10-16 09:09:35.000000 m-utilities-1.0.8/m_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 09:09:35.000000 m-utilities-1.0.8/m_utilities.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-16 09:09:35.663391 m-utilities-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1287 2023-10-16 09:09:35.000000 m-utilities-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 07:43:02.361662 m-utilities-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-01-03 07:43:02.360661 m-utilities-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      735 2024-01-03 07:39:33.000000 m-utilities-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-03 07:43:02.359661 m-utilities-1.0.9/m_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-01-03 07:43:02.000000 m-utilities-1.0.9/m_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2024-01-03 07:43:02.000000 m-utilities-1.0.9/m_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-03 07:43:02.000000 m-utilities-1.0.9/m_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-01-03 07:43:02.000000 m-utilities-1.0.9/m_utilities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-03 07:43:02.000000 m-utilities-1.0.9/m_utilities.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-03 07:43:02.361662 m-utilities-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1280 2024-01-03 07:43:01.000000 m-utilities-1.0.9/setup.py
```

### Comparing `m-utilities-1.0.8/PKG-INFO` & `m-utilities-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-utilities
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio Utilities, tổng hợp thư viện được dùng thường xuyên trong các micro-service Mobio.
 Home-page: 
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -13,14 +13,14 @@
 
 Project tập trung các thư viện cơ bản dùng trong các Project Python của Mobio.
 
 Danh sách các thư viện:
 * m-singleton==0.3 (https://pypi.org/project/m-singleton)
 * m-monitor==0.6  (https://pypi.org/project/m-monitor)
 * m-validator==0.1 (https://pypi.org/project/m-validator)
-* m-filetypes==0.1.5 (https://pypi.org/project/m-filetypes)
+* m-filetypes (https://pypi.org/project/m-filetypes)
 * m-cipher==1.5.2 (https://pypi.org/project/m-cipher)
 * m-schedule==0.6.7 (https://pypi.org/project/m-schedule)
 * m-caching==0.1.14 (https://pypi.org/project/m-caching)
 * m-threadpool==0.2 (https://pypi.org/project/m-threadpool)
 * m-formatter-logging>=1.0.2 (https://pypi.org/project/m-formatter-logging)
 * m-kafka-sdk-v2==0.1.8 (https://pypi.org/project/m-kafka-sdk-v2)
```

### Comparing `m-utilities-1.0.8/README.md` & `m-utilities-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 
 Project tập trung các thư viện cơ bản dùng trong các Project Python của Mobio.
 
 Danh sách các thư viện:
 * m-singleton==0.3 (https://pypi.org/project/m-singleton)
 * m-monitor==0.6  (https://pypi.org/project/m-monitor)
 * m-validator==0.1 (https://pypi.org/project/m-validator)
-* m-filetypes==0.1.5 (https://pypi.org/project/m-filetypes)
+* m-filetypes (https://pypi.org/project/m-filetypes)
 * m-cipher==1.5.2 (https://pypi.org/project/m-cipher)
 * m-schedule==0.6.7 (https://pypi.org/project/m-schedule)
 * m-caching==0.1.14 (https://pypi.org/project/m-caching)
 * m-threadpool==0.2 (https://pypi.org/project/m-threadpool)
 * m-formatter-logging>=1.0.2 (https://pypi.org/project/m-formatter-logging)
 * m-kafka-sdk-v2==0.1.8 (https://pypi.org/project/m-kafka-sdk-v2)
```

### Comparing `m-utilities-1.0.8/m_utilities.egg-info/PKG-INFO` & `m-utilities-1.0.9/m_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-utilities
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio Utilities, tổng hợp thư viện được dùng thường xuyên trong các micro-service Mobio.
 Home-page: 
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -13,14 +13,14 @@
 
 Project tập trung các thư viện cơ bản dùng trong các Project Python của Mobio.
 
 Danh sách các thư viện:
 * m-singleton==0.3 (https://pypi.org/project/m-singleton)
 * m-monitor==0.6  (https://pypi.org/project/m-monitor)
 * m-validator==0.1 (https://pypi.org/project/m-validator)
-* m-filetypes==0.1.5 (https://pypi.org/project/m-filetypes)
+* m-filetypes (https://pypi.org/project/m-filetypes)
 * m-cipher==1.5.2 (https://pypi.org/project/m-cipher)
 * m-schedule==0.6.7 (https://pypi.org/project/m-schedule)
 * m-caching==0.1.14 (https://pypi.org/project/m-caching)
 * m-threadpool==0.2 (https://pypi.org/project/m-threadpool)
 * m-formatter-logging>=1.0.2 (https://pypi.org/project/m-formatter-logging)
 * m-kafka-sdk-v2==0.1.8 (https://pypi.org/project/m-kafka-sdk-v2)
```

### Comparing `m-utilities-1.0.8/setup.py` & `m-utilities-1.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 # read the contents of your README file
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 version_dev='1.0.0'
-version_prod='1.0.8'
+version_prod='1.0.9'
 
 run_mode=''
 
 setup(name='m-utilities' + run_mode,
-      version='1.0.8',
+      version='1.0.9',
       description='Mobio Utilities, tổng hợp thư viện được dùng thường xuyên trong các micro-service Mobio.',
       url='',
       author='MOBIO',
       author_email='contact@mobio.vn',
       license='MIT',
       package_dir={'': './'},
       packages=find_packages('./'),
       install_requires=['m-singleton==0.3',
                         'm-monitor==0.6',
                         'm-validator==0.1',
-                        'm-filetypes==0.1.5',
+                        'm-filetypes',
                         'm-cipher==1.5.2',
                         'm-schedule==0.6.7',
                         'm-caching==0.1.14',
                         'm-threadpool==0.2',
                         'm-formatter-logging>=1.0.2',
                         'm-kafka-sdk-v2==0.1.8',
                         ],
```

