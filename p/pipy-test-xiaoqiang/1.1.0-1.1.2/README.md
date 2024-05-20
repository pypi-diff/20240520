# Comparing `tmp/pipy-test-xiaoqiang-1.1.0.tar.gz` & `tmp/pipy-test-xiaoqiang-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipy-test-xiaoqiang-1.1.0.tar", last modified: Mon May 20 09:21:06 2024, max compression
+gzip compressed data, was "pipy-test-xiaoqiang-1.1.2.tar", last modified: Mon May 20 09:27:24 2024, max compression
```

## Comparing `pipy-test-xiaoqiang-1.1.0.tar` & `pipy-test-xiaoqiang-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 09:21:06.813254 pipy-test-xiaoqiang-1.1.0/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      683 2024-05-20 09:21:06.813061 pipy-test-xiaoqiang-1.1.0/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       48 2024-05-20 07:13:42.000000 pipy-test-xiaoqiang-1.1.0/README.md
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 09:21:06.810765 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 06:56:45.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/__init__.py
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       82 2024-05-20 09:08:07.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/cli.py
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      519 2024-05-20 07:05:57.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/main.py
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 09:21:06.812724 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      683 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      365 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       56 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/entry_points.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        6 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/requires.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       20 2024-05-20 09:21:06.000000 pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/top_level.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-20 09:21:06.813331 pipy-test-xiaoqiang-1.1.0/setup.cfg
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)     1028 2024-05-20 09:21:03.000000 pipy-test-xiaoqiang-1.1.0/setup.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 09:27:24.393567 pipy-test-xiaoqiang-1.1.2/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      683 2024-05-20 09:27:24.393399 pipy-test-xiaoqiang-1.1.2/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       48 2024-05-20 07:13:42.000000 pipy-test-xiaoqiang-1.1.2/README.md
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 09:27:24.391018 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 06:56:45.000000 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang/__init__.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       82 2024-05-20 09:08:07.000000 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang/cli.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      519 2024-05-20 07:05:57.000000 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang/main.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-20 09:27:24.392485 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang.egg-info/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      683 2024-05-20 09:27:24.000000 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang.egg-info/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      365 2024-05-20 09:27:24.000000 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-20 09:27:24.000000 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       65 2024-05-20 09:27:24.000000 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang.egg-info/entry_points.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        6 2024-05-20 09:27:24.000000 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang.egg-info/requires.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       20 2024-05-20 09:27:24.000000 pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang.egg-info/top_level.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-20 09:27:24.393637 pipy-test-xiaoqiang-1.1.2/setup.cfg
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)     1037 2024-05-20 09:26:27.000000 pipy-test-xiaoqiang-1.1.2/setup.py
```

### Comparing `pipy-test-xiaoqiang-1.1.0/PKG-INFO` & `pipy-test-xiaoqiang-1.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipy-test-xiaoqiang
-Version: 1.1.0
+Version: 1.1.2
 Summary: A short description of your project
 Home-page: https://github.com/yourusername/my_project
 Author: Ma Xiaoqiang
 Author-email: 851788096@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang/main.py` & `pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang/main.py`

 * *Files identical despite different names*

### Comparing `pipy-test-xiaoqiang-1.1.0/pipy_test_xiaoqiang.egg-info/PKG-INFO` & `pipy-test-xiaoqiang-1.1.2/pipy_test_xiaoqiang.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipy-test-xiaoqiang
-Version: 1.1.0
+Version: 1.1.2
 Summary: A short description of your project
 Home-page: https://github.com/yourusername/my_project
 Author: Ma Xiaoqiang
 Author-email: 851788096@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pipy-test-xiaoqiang-1.1.0/setup.py` & `pipy-test-xiaoqiang-1.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pipy-test-xiaoqiang",
-    version="1.1.0",
+    version="1.1.2",
     packages=find_packages(),
     install_requires=[
         'click',  # 添加 click 作为依赖
     ],
     entry_points={
         'console_scripts': [
-            'my_project_init=my_project.cli:init',  # 使用命令组前缀
+            'my_project_init=pipy_test_xiaoqiang.cli:init',  # 使用命令组前缀
         ],
     },
     author="Ma Xiaoqiang",
     author_email="851788096@qq.com",
     description="A short description of your project",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

