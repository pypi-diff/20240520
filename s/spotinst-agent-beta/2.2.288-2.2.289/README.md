# Comparing `tmp/spotinst-agent-beta-2.2.288.tar.gz` & `tmp/spotinst-agent-beta-2.2.289.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spotinst-agent-beta-2.2.288.tar", last modified: Sun May 19 12:19:48 2024, max compression
+gzip compressed data, was "dist/spotinst-agent-beta-2.2.289.tar", last modified: Mon May 20 08:31:58 2024, max compression
```

## Comparing `spotinst-agent-beta-2.2.288.tar` & `spotinst-agent-beta-2.2.289.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/
--rw-r--r--   0 bsaada     (502) staff       (20)     2277 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/PKG-INFO
--rw-r--r--   0 bsaada     (502) staff       (20)      181 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/MANIFEST.in
--rwxr-xr-x   0 bsaada     (502) staff       (20)     1392 2024-05-19 12:10:11.000000 spotinst-agent-beta-2.2.288/setup.py
-drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/
--rw-r--r--   0 bsaada     (502) staff       (20)     2277 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 bsaada     (502) staff       (20)      630 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 bsaada     (502) staff       (20)       56 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 bsaada     (502) staff       (20)       16 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 bsaada     (502) staff       (20)       15 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/top_level.txt
--rw-r--r--   0 bsaada     (502) staff       (20)        1 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 bsaada     (502) staff       (20)       38 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/setup.cfg
--rw-r--r--   0 bsaada     (502) staff       (20)     1287 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/README.rst
-drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent/
--rw-r--r--   0 bsaada     (502) staff       (20)     9604 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/agentinit.py
--rw-r--r--   0 bsaada     (502) staff       (20)     1129 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/basemodule.py
--rw-r--r--   0 bsaada     (502) staff       (20)    13098 2024-05-19 12:02:38.000000 spotinst-agent-beta-2.2.288/spotinst_agent/__init__.py
--rw-r--r--   0 bsaada     (502) staff       (20)    10733 2024-05-19 12:02:38.000000 spotinst-agent-beta-2.2.288/spotinst_agent/taskmanager.py
--rw-r--r--   0 bsaada     (502) staff       (20)     9420 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/utils.py
--rw-r--r--   0 bsaada     (502) staff       (20)     3116 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/agent.py
--rw-r--r--   0 bsaada     (502) staff       (20)    21605 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/scheduler.py
-drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/
-drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/configuration/
--rw-r--r--   0 bsaada     (502) staff       (20)      180 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 bsaada     (502) staff       (20)      727 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/installation/
--rwxr-xr-x   0 bsaada     (502) staff       (20)     6691 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/installation/agent-init.sh
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/
+-rw-r--r--   0 bsaada     (502) staff       (20)     2277 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/PKG-INFO
+-rw-r--r--   0 bsaada     (502) staff       (20)      181 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.289/MANIFEST.in
+-rwxr-xr-x   0 bsaada     (502) staff       (20)     1363 2024-05-20 08:31:22.000000 spotinst-agent-beta-2.2.289/setup.py
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 bsaada     (502) staff       (20)     2277 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 bsaada     (502) staff       (20)      630 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       56 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       16 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       15 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent_beta.egg-info/top_level.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)        1 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       38 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/setup.cfg
+-rw-r--r--   0 bsaada     (502) staff       (20)     1287 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.289/README.rst
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent/
+-rw-r--r--   0 bsaada     (502) staff       (20)     9604 2024-05-19 12:25:49.000000 spotinst-agent-beta-2.2.289/spotinst_agent/agentinit.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     1129 2024-05-19 12:25:49.000000 spotinst-agent-beta-2.2.289/spotinst_agent/basemodule.py
+-rw-r--r--   0 bsaada     (502) staff       (20)    13098 2024-05-19 12:25:49.000000 spotinst-agent-beta-2.2.289/spotinst_agent/__init__.py
+-rw-r--r--   0 bsaada     (502) staff       (20)    10755 2024-05-20 08:29:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent/taskmanager.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     9420 2024-05-19 12:25:49.000000 spotinst-agent-beta-2.2.289/spotinst_agent/utils.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     3116 2024-05-19 12:25:49.000000 spotinst-agent-beta-2.2.289/spotinst_agent/agent.py
+-rw-r--r--   0 bsaada     (502) staff       (20)    21605 2024-05-19 12:25:49.000000 spotinst-agent-beta-2.2.289/spotinst_agent/scheduler.py
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent/data/
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent/data/configuration/
+-rw-r--r--   0 bsaada     (502) staff       (20)      180 2024-05-19 12:25:49.000000 spotinst-agent-beta-2.2.289/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 bsaada     (502) staff       (20)      727 2024-05-19 12:25:49.000000 spotinst-agent-beta-2.2.289/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-20 08:31:58.000000 spotinst-agent-beta-2.2.289/spotinst_agent/data/installation/
+-rwxr-xr-x   0 bsaada     (502) staff       (20)     6691 2024-05-19 12:25:49.000000 spotinst-agent-beta-2.2.289/spotinst_agent/data/installation/agent-init.sh
```

### Comparing `spotinst-agent-beta-2.2.288/PKG-INFO` & `spotinst-agent-beta-2.2.289/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: spotinst-agent-beta
-Version: 2.2.288
+Version: 2.2.289
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Description: Agent
         =======
```

### Comparing `spotinst-agent-beta-2.2.288/setup.py` & `spotinst-agent-beta-2.2.289/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,42 @@
 #!/usr/bin/env python
 from codecs import open
 from os import path
 
 from setuptools import setup
 
-with open('README.rst') as desc_file:
+with open("README.rst") as desc_file:
     description = desc_file.read()
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
+with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='spotinst-agent-beta',
-
-    version="2.2.288",
-
-    description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
-
+    name="spotinst-agent-beta",
+    version="2.2.289",
+    description="Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.",
     long_description=description,
-
     # The project's main homepage.
-    url='https://github.com/spotinst/spotinst-spectrum-agent',
-
+    url="https://github.com/spotinst/spotinst-spectrum-agent",
     # Author details
-    author='Spotinst',
-    author_email='service@spotinst.com',
-
+    author="Spotinst",
+    author_email="service@spotinst.com",
     # Choose your license
-    license='MIT',
-
+    license="MIT",
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Information Technology',
-        'Topic :: System :: Monitoring',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 2.7'
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Information Technology",
+        "Topic :: System :: Monitoring",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 2.7",
     ],
-
-    keywords='spotinst agent infrastructure monitoring execution deployment',
-    install_requires=['requests', 'pyyaml'],
+    keywords="spotinst agent infrastructure monitoring execution deployment",
+    install_requires=["requests", "pyyaml"],
     packages=["spotinst_agent"],
     include_package_data=True,
     entry_points={
-        'console_scripts': [
-            'spotinst-agent=spotinst_agent:main'
-        ],
-    }
-
+        "console_scripts": ["spotinst-agent=spotinst_agent:main"],
+    },
 )
```

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.289/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: spotinst-agent-beta
-Version: 2.2.288
+Version: 2.2.289
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Description: Agent
         =======
```

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.289/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.288/README.rst` & `spotinst-agent-beta-2.2.289/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.289/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.289/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.289/spotinst_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.289/spotinst_agent/taskmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self.reload_interval = reload_interval
         self.scheduler = ThreadedScheduler()
         self.running = True
         self.tasks = {}
         self.instance_details = instance_details
 
     def start(self):
+        time.sleep(3)
         initiators_folder = '/etc/spotinst/agent/initiators/modules'
 
         # Search for initiators in folder
         initiators = self.load_modules(initiators_folder)
 
         # Setup Modules
         for initiator in initiators.values():
```

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.289/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.289/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.289/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.289/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.288/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.289/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

