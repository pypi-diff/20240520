# Comparing `tmp/ha_s3_tool-0.1.0.tar.gz` & `tmp/ha_s3_tool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha_s3_tool-0.1.0.tar", last modified: Mon May 20 16:58:59 2024, max compression
+gzip compressed data, was "ha_s3_tool-0.1.1.tar", last modified: Mon May 20 18:01:02 2024, max compression
```

## Comparing `ha_s3_tool-0.1.0.tar` & `ha_s3_tool-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 16:58:59.027182 ha_s3_tool-0.1.0/
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)     2676 2024-05-20 16:58:59.026929 ha_s3_tool-0.1.0/PKG-INFO
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)     2158 2024-05-20 15:43:24.000000 ha_s3_tool-0.1.0/README.md
-drwxr-xr-x   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 16:58:59.026695 ha_s3_tool-0.1.0/ha_s3_tool.egg-info/
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)     2676 2024-05-20 16:58:58.000000 ha_s3_tool-0.1.0/ha_s3_tool.egg-info/PKG-INFO
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)      285 2024-05-20 16:58:59.000000 ha_s3_tool-0.1.0/ha_s3_tool.egg-info/SOURCES.txt
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)        1 2024-05-20 16:58:58.000000 ha_s3_tool-0.1.0/ha_s3_tool.egg-info/dependency_links.txt
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)      108 2024-05-20 16:58:58.000000 ha_s3_tool-0.1.0/ha_s3_tool.egg-info/entry_points.txt
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)       11 2024-05-20 16:58:58.000000 ha_s3_tool-0.1.0/ha_s3_tool.egg-info/requires.txt
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)        8 2024-05-20 16:58:58.000000 ha_s3_tool-0.1.0/ha_s3_tool.egg-info/top_level.txt
-drwxr-xr-x   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 16:58:59.026100 ha_s3_tool-0.1.0/s3_tool/
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 13:17:26.000000 ha_s3_tool-0.1.0/s3_tool/__init__.py
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)     5859 2024-05-20 15:24:13.000000 ha_s3_tool-0.1.0/s3_tool/s3_tool.py
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)       38 2024-05-20 16:58:59.027240 ha_s3_tool-0.1.0/setup.cfg
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)     1215 2024-05-20 16:58:42.000000 ha_s3_tool-0.1.0/setup.py
-drwxr-xr-x   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 16:58:59.026378 ha_s3_tool-0.1.0/tests/
--rw-r--r--   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 13:17:49.000000 ha_s3_tool-0.1.0/tests/test_s3utils.py
+drwxr-xr-x   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 18:01:02.011343 ha_s3_tool-0.1.1/
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)     2676 2024-05-20 18:01:02.011157 ha_s3_tool-0.1.1/PKG-INFO
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)     2158 2024-05-20 15:43:24.000000 ha_s3_tool-0.1.1/README.md
+drwxr-xr-x   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 18:01:02.010951 ha_s3_tool-0.1.1/ha_s3_tool.egg-info/
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)     2676 2024-05-20 18:01:01.000000 ha_s3_tool-0.1.1/ha_s3_tool.egg-info/PKG-INFO
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)      285 2024-05-20 18:01:01.000000 ha_s3_tool-0.1.1/ha_s3_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)        1 2024-05-20 18:01:01.000000 ha_s3_tool-0.1.1/ha_s3_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)      108 2024-05-20 18:01:01.000000 ha_s3_tool-0.1.1/ha_s3_tool.egg-info/entry_points.txt
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)       11 2024-05-20 18:01:01.000000 ha_s3_tool-0.1.1/ha_s3_tool.egg-info/requires.txt
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)        8 2024-05-20 18:01:01.000000 ha_s3_tool-0.1.1/ha_s3_tool.egg-info/top_level.txt
+drwxr-xr-x   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 18:01:02.010609 ha_s3_tool-0.1.1/s3_tool/
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 13:17:26.000000 ha_s3_tool-0.1.1/s3_tool/__init__.py
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)     6108 2024-05-20 17:51:14.000000 ha_s3_tool-0.1.1/s3_tool/s3_tool.py
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)       38 2024-05-20 18:01:02.011387 ha_s3_tool-0.1.1/setup.cfg
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)     1271 2024-05-20 18:00:51.000000 ha_s3_tool-0.1.1/setup.py
+drwxr-xr-x   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 18:01:02.010753 ha_s3_tool-0.1.1/tests/
+-rw-r--r--   0 manuelrodriguez   (501) staff       (20)        0 2024-05-20 13:17:49.000000 ha_s3_tool-0.1.1/tests/test_s3utils.py
```

### Comparing `ha_s3_tool-0.1.0/PKG-INFO` & `ha_s3_tool-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-s3-tool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for uploading and downloading files and folders to/from S3.
 Home-page: https://github.com/manuelladron/s3_tool
 Author: Manuel Rodriguez Ladron de Guevara
 Author-email: manuelrodriguez@higharc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ha_s3_tool-0.1.0/README.md` & `ha_s3_tool-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ha_s3_tool-0.1.0/ha_s3_tool.egg-info/PKG-INFO` & `ha_s3_tool-0.1.1/ha_s3_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ha-s3-tool
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for uploading and downloading files and folders to/from S3.
 Home-page: https://github.com/manuelladron/s3_tool
 Author: Manuel Rodriguez Ladron de Guevara
 Author-email: manuelrodriguez@higharc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ha_s3_tool-0.1.0/s3_tool/s3_tool.py` & `ha_s3_tool-0.1.1/s3_tool/s3_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,21 @@
     if not config_path.exists():
         raise FileNotFoundError("AWS credentials file not found. Please run the installation script again.")
     
     config = configparser.ConfigParser()
     config.read(config_path)
     aws_credentials = config['default']
 
-    os.environ['AWS_ACCESS_KEY_ID'] = aws_credentials['AWS_ACCESS_KEY_ID']
-    os.environ['AWS_SECRET_ACCESS_KEY'] = aws_credentials['AWS_SECRET_ACCESS_KEY']
-    os.environ['AWS_REGION'] = aws_credentials['AWS_REGION']
+    os.environ['AWS_ACCESS_KEY_ID'] = aws_credentials.get('aws_access_key_id', '')
+    os.environ['AWS_SECRET_ACCESS_KEY'] = aws_credentials.get('aws_secret_access_key', '')
+    os.environ['AWS_REGION'] = aws_credentials.get('region', '')
+
+    if not os.environ['AWS_ACCESS_KEY_ID'] or not os.environ['AWS_SECRET_ACCESS_KEY'] or not os.environ['AWS_REGION']:
+        raise ValueError("AWS credentials are not set properly. Please run the installation script again.")
+
 
 def upload_file_to_s3(local_file_path, bucket_name, s3_file_path, region_name='us-east-1'):
     load_aws_credentials()
     s3_client = boto3.client('s3', region_name=region_name)
     
     if s3_file_exists(bucket_name, s3_file_path):
         print(f"File {s3_file_path} already exists in s3://{bucket_name}. Skipping upload.")
```

### Comparing `ha_s3_tool-0.1.0/setup.py` & `ha_s3_tool-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import subprocess
+import sys 
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
-        subprocess.call(['python', 'post_install.py'])
+        if 'install' in sys.argv:
+            subprocess.call([sys.executable, 'post_install.py'])
 
 setup(
     name="ha-s3-tool",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "boto3",
         "tqdm",
     ],
     entry_points={
         "console_scripts": [
```

