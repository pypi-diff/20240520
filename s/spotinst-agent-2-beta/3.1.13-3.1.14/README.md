# Comparing `tmp/spotinst-agent-2-beta-3.1.13.tar.gz` & `tmp/spotinst-agent-2-beta-3.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-2-beta-3.1.13.tar", last modified: Wed May  1 13:08:07 2024, max compression
+gzip compressed data, was "spotinst-agent-2-beta-3.1.14.tar", last modified: Sun May 19 12:27:28 2024, max compression
```

## Comparing `spotinst-agent-2-beta-3.1.13.tar` & `spotinst-agent-2-beta-3.1.14.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.439762 spotinst-agent-2-beta-3.1.13/
--rw-r--r--   0 mavni      (501) staff       (20)     1065 2024-05-01 09:00:13.000000 spotinst-agent-2-beta-3.1.13/LICENSE
--rw-r--r--   0 mavni      (501) staff       (20)      181 2024-05-01 09:00:13.000000 spotinst-agent-2-beta-3.1.13/MANIFEST.in
--rw-r--r--   0 mavni      (501) staff       (20)     2299 2024-05-01 13:08:07.439447 spotinst-agent-2-beta-3.1.13/PKG-INFO
--rw-r--r--   0 mavni      (501) staff       (20)     1287 2024-05-01 09:00:13.000000 spotinst-agent-2-beta-3.1.13/README.rst
--rw-r--r--   0 mavni      (501) staff       (20)       38 2024-05-01 13:08:07.439889 spotinst-agent-2-beta-3.1.13/setup.cfg
--rwxr-xr-x   0 mavni      (501) staff       (20)     1442 2024-05-01 13:00:03.000000 spotinst-agent-2-beta-3.1.13/setup.py
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.431605 spotinst-agent-2-beta-3.1.13/spotinst_agent/
--rw-r--r--   0 mavni      (501) staff       (20)    12950 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/__init__.py
--rw-r--r--   0 mavni      (501) staff       (20)     3383 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/agent.py
--rw-r--r--   0 mavni      (501) staff       (20)     9645 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/agentinit.py
--rw-r--r--   0 mavni      (501) staff       (20)     1157 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/basemodule.py
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.422354 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.433709 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/configuration/
--rw-r--r--   0 mavni      (501) staff       (20)      180 2024-05-01 09:00:13.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 mavni      (501) staff       (20)      727 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.434388 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/installation/
--rwxr-xr-x   0 mavni      (501) staff       (20)     6979 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 mavni      (501) staff       (20)    21721 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/scheduler.py
--rw-r--r--   0 mavni      (501) staff       (20)    11111 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/taskmanager.py
--rw-r--r--   0 mavni      (501) staff       (20)     9662 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/utils.py
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.438172 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/
--rw-r--r--   0 mavni      (501) staff       (20)     2299 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/PKG-INFO
--rw-r--r--   0 mavni      (501) staff       (20)      650 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/SOURCES.txt
--rw-r--r--   0 mavni      (501) staff       (20)        1 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/dependency_links.txt
--rw-r--r--   0 mavni      (501) staff       (20)       56 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/entry_points.txt
--rw-r--r--   0 mavni      (501) staff       (20)       23 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/requires.txt
--rw-r--r--   0 mavni      (501) staff       (20)       15 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/top_level.txt
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:27:28.359738 spotinst-agent-2-beta-3.1.14/
+-rw-r--r--   0 bsaada     (502) staff       (20)     1065 2024-05-19 12:02:06.000000 spotinst-agent-2-beta-3.1.14/LICENSE
+-rw-r--r--   0 bsaada     (502) staff       (20)      181 2024-05-19 12:02:06.000000 spotinst-agent-2-beta-3.1.14/MANIFEST.in
+-rw-r--r--   0 bsaada     (502) staff       (20)     1987 2024-05-19 12:27:28.358874 spotinst-agent-2-beta-3.1.14/PKG-INFO
+-rw-r--r--   0 bsaada     (502) staff       (20)     1287 2024-05-19 12:02:06.000000 spotinst-agent-2-beta-3.1.14/README.rst
+-rw-r--r--   0 bsaada     (502) staff       (20)       38 2024-05-19 12:27:28.359943 spotinst-agent-2-beta-3.1.14/setup.cfg
+-rwxr-xr-x   0 bsaada     (502) staff       (20)     1364 2024-05-19 12:27:06.000000 spotinst-agent-2-beta-3.1.14/setup.py
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:27:28.337828 spotinst-agent-2-beta-3.1.14/spotinst_agent/
+-rw-r--r--   0 bsaada     (502) staff       (20)    13098 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/__init__.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     3116 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/agent.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     9604 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/agentinit.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     1129 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/basemodule.py
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:27:28.326920 spotinst-agent-2-beta-3.1.14/spotinst_agent/data/
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:27:28.350992 spotinst-agent-2-beta-3.1.14/spotinst_agent/data/configuration/
+-rw-r--r--   0 bsaada     (502) staff       (20)      180 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 bsaada     (502) staff       (20)      727 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:27:28.351981 spotinst-agent-2-beta-3.1.14/spotinst_agent/data/installation/
+-rwxr-xr-x   0 bsaada     (502) staff       (20)     6691 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 bsaada     (502) staff       (20)    21605 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/scheduler.py
+-rw-r--r--   0 bsaada     (502) staff       (20)    10733 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/taskmanager.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     9420 2024-05-19 12:25:49.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent/utils.py
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:27:28.357927 spotinst-agent-2-beta-3.1.14/spotinst_agent_2_beta.egg-info/
+-rw-r--r--   0 bsaada     (502) staff       (20)     1987 2024-05-19 12:27:28.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent_2_beta.egg-info/PKG-INFO
+-rw-r--r--   0 bsaada     (502) staff       (20)      650 2024-05-19 12:27:28.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent_2_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)        1 2024-05-19 12:27:28.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent_2_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       55 2024-05-19 12:27:28.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent_2_beta.egg-info/entry_points.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       16 2024-05-19 12:27:28.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent_2_beta.egg-info/requires.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       15 2024-05-19 12:27:28.000000 spotinst-agent-2-beta-3.1.14/spotinst_agent_2_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-2-beta-3.1.13/LICENSE` & `spotinst-agent-2-beta-3.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-3.1.13/PKG-INFO` & `spotinst-agent-2-beta-3.1.14/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,59 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: spotinst-agent-2-beta
-Version: 3.1.13
+Version: 3.1.14
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
-Description: Agent
-        =======
-        
-        Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
-        
-        Note:
-        The agent must have token to communicate with spotinst API.
-        The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
-        
-        Application
-        ===========
-        
-        Manual Executing
-        ~~~~~~~~~~~~~~~~
-        The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
-        
-        Otherwise, you can use the following options:
-        
-        Usage:  ./agent [options]
-        
-        -c --config            Use alternate configuration yml file.
-        -l --log               Use alternate Log file for output.
-        -t --test              Test run.  Do not run remote script.
-        -v --verbose           verbose log
-        --stdout               redirect output to stdout
-        --debug                run with dummy credentials for debug purposes
-        
-        Configuration
-        ~~~~~~~~~~~~~
-        There are two levels of configuration representing in yml files.
-        The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
-        The worker configuration, located at the workers folder is responsible of the specific workers parameters.
-        
-        
-        MAKEFILE
-        ~~~~~~~~~~~~~
-        run 'make release'
-        output file is located in the /dist folder
-        
-        Documentation
-        =============
-        
 Keywords: spotinst agent infrastructure monitoring execution deployment
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ==3.*
+Classifier: Programming Language :: Python :: 2.7
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pyyaml
+
+Agent
+=======
+
+Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
+
+Note:
+The agent must have token to communicate with spotinst API.
+The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
+
+Application
+===========
+
+Manual Executing
+~~~~~~~~~~~~~~~~
+The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
+
+Otherwise, you can use the following options:
+
+Usage:  ./agent [options]
+
+-c --config            Use alternate configuration yml file.
+-l --log               Use alternate Log file for output.
+-t --test              Test run.  Do not run remote script.
+-v --verbose           verbose log
+--stdout               redirect output to stdout
+--debug                run with dummy credentials for debug purposes
+
+Configuration
+~~~~~~~~~~~~~
+There are two levels of configuration representing in yml files.
+The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
+The worker configuration, located at the workers folder is responsible of the specific workers parameters.
+
+
+MAKEFILE
+~~~~~~~~~~~~~
+run 'make release'
+output file is located in the /dist folder
+
+Documentation
+=============
```

### Comparing `spotinst-agent-2-beta-3.1.13/README.rst` & `spotinst-agent-2-beta-3.1.14/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent/__init__.py` & `spotinst-agent-2-beta-3.1.14/spotinst_agent/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-from __future__ import print_function
-from __future__ import absolute_import
-from future import standard_library
-standard_library.install_aliases()
-from builtins import str
 import argparse
 import os
 import subprocess
-import urllib.request, urllib.error, urllib.parse
-from . import utils
+import urllib2
+import utils
 import sys
 from shutil import copyfile
-from .agent import run_agent
+from agent import run_agent
 from time import sleep
 
 
 def main():
-    s3_base_link = 'https://s3.amazonaws.com/spotinst-public/services/spotinst-agent-2'
+    s3_base_link = 'https://s3.amazonaws.com/spotinst-public/services/spotinst-agent'
     s3_base_workers_link = s3_base_link + "/workers"
-    s3_base_collectors_link = s3_base_link + "/collectors"
     s3_base_initiator_link = s3_base_link + "/initiators"
+    s3_base_collectors_link = s3_base_link + "/collectors"
     modules_path = '/etc/spotinst/agent/modules'
     initiator_modules_path = '/etc/spotinst/agent/initiators/modules'
     instance_details_path = '/etc/spotinst'
 
     results = parse_arguments()
     action = results.action
     argument = results.argument
@@ -73,34 +68,35 @@
         while (not install_succeed) and (try_num <= 3):
             if try_num > 1:
                 sleep(20)
                 print("trying to Initializing agent again (retry %s/3)" % (format(try_num)))
             try_num += 1
             print ("Initializing agent")
             install_succeed = handle_cloud_provider(cloud_provider, instance_details_path) and install_and_init_agent(
-                argument, second_argument, third_argument, modules_path)
+                argument, second_argument, third_argument, modules_path, initiator_modules_path)
 
         if not install_succeed:
             print("init failed")
             exit(1)
         else:
             print("Spotinst agent installed successfully")
     else:
-        print ("Unrecognized action. Please use one of the following : add-worker, add-collector, configure")
+        print ("Unrecognized action. Please use one of the following : add-worker, add-collector, add-initiator, "
+               "configure")
 
 
-def install_and_init_agent(token, account_id, custom_host, modules_path):
+def install_and_init_agent(token, account_id, custom_host, modules_path, initiator_modules_path):
     # Paths
     runscript = None
     try:
         dirname, filename = os.path.split(os.path.abspath(__file__))
         script_full_path = os.path.join(dirname, 'data/installation/agent-init.sh')
         spotinst_agent_path = os.path.join(dirname, 'agent.py')
         create_agent_local_folders()
-        handle_base_modules(dirname, modules_path)
+        handle_base_modules(dirname, modules_path, initiator_modules_path)
         handle_yml_file(dirname)
         handle_credentials(account_id, script_full_path, spotinst_agent_path, token, custom_host)
         handle_agent_path(spotinst_agent_path)
         runscript = subprocess.Popen(script_full_path)
         runscript.wait()
         print ('result : ' + str(runscript.communicate()))
     except:
@@ -135,19 +131,25 @@
         os.makedirs('/etc/spotinst/agent')
     if not os.path.exists('/etc/spotinst/agent/config'):
         os.makedirs('/etc/spotinst/agent/config')
     if not os.path.exists('/var/log/spotinst'):
         os.makedirs('/var/log/spotinst')
 
 
-def handle_base_modules(dirname, modules_path):
+def handle_base_modules(dirname, modules_path, initiator_modules_path):
     basemodule_yml_path = os.path.join(dirname, 'data/configuration/basemodule.yml')
     utils_path = os.path.join(dirname, 'utils.py')
     basemodule_template_path = os.path.join(dirname, 'basemodule.py')
 
+    if not os.path.exists(initiator_modules_path):
+        os.makedirs(initiator_modules_path)
+    copyfile(basemodule_template_path, initiator_modules_path + '/basemodule.py')
+    copyfile(basemodule_yml_path, initiator_modules_path + '/basemodule.yml')
+    copyfile(utils_path, initiator_modules_path + '/utils.py')
+
     if not os.path.exists(modules_path):
         os.makedirs(modules_path)
     copyfile(basemodule_template_path, modules_path + '/basemodule.py')
     copyfile(basemodule_yml_path, modules_path + '/basemodule.yml')
     copyfile(utils_path, modules_path + '/utils.py')
 
 
@@ -248,55 +250,55 @@
     try:
         handle_prerequisites(s3_base_collectors_link, collector_name)
         get_collector_files(collector_name, modules_path, s3_base_collectors_link)
 
     except Exception as e:
         print ("Could not get collector " + collector_name + " Exception : " + str(e))
 
+
 def install_initiator(initiator_name, initiator_modules_path, s3_base_initiator_link):
     print("adding initiator " + initiator_name)
     try:
         get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link)
 
     except Exception as e:
         print("Could not get initiator " + initiator_name + " Exception : " + str(e))
 
+
 def get_worker_files(modules_path, s3_base_workers_link, worker_name):
-    py_response = urllib.request.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.py')
-    yml_response = urllib.request.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.yml')
+    py_response = urllib2.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.py')
+    yml_response = urllib2.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.yml')
 
     with open(modules_path + '/' + worker_name + '.py', 'wb') as worker:
         worker.write(py_response.read())
     with open(modules_path + '/' + worker_name + '.yml', 'wb') as worker_cfg:
         worker_cfg.write(yml_response.read())
 
 
 def get_collector_files(collector_name, modules_path, s3_base_collectors_link):
     with open(modules_path + '/' + collector_name + '.py', 'wb') as collector:
-        response = urllib.request.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.py')
+        response = urllib2.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.py')
         collector.write(response.read())
     with open(modules_path + '/' + collector_name + '.yml', 'wb') as collector_cfg:
-        response = urllib.request.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.yml')
+        response = urllib2.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.yml')
         collector_cfg.write(response.read())
 
 
 def get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link):
-    with open(initiator_modules_path + '/' + initiator_name + '.py', 'wb') as initiator:
-        response = urllib.request.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.py')
-        initiator.write(response.read())
-    with open(initiator_modules_path + '/' + initiator_name + '.yml', 'wb') as initiator_cfg:
-        response = urllib.request.urlopen(
-            s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.yml')
-        initiator_cfg.write(response.read())
-
+    with open(initiator_modules_path + '/' + initiator_name + '.py', 'wb') as collector:
+        response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.py')
+        collector.write(response.read())
+    with open(initiator_modules_path + '/' + initiator_name + '.yml', 'wb') as collector_cfg:
+        response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.yml')
+        collector_cfg.write(response.read())
 
 def handle_prerequisites(s3_base_module_link, module_name):
     try:
-        response = urllib.request.urlopen(s3_base_module_link + '/' + module_name + '/' + module_name + '.req')
-        requirements_file = response.read().decode('utf-8')
+        response = urllib2.urlopen(s3_base_module_link + '/' + module_name + '/' + module_name + '.req')
+        requirements_file = response.read()
         requirements_names = requirements_file.split("\n")
         print ("This module requires the following packages to be installed:")
         for requirement in requirements_names:
             print (requirement)
 
         if len(requirements_names) > 0:
             import pip
@@ -311,9 +313,9 @@
             if len(missing_packages) <= 0:
                 print ("All prerequisites have been met.")
                 pass
             else:
                 print ("Some prerequisites for this module have not been met. " \
                        "Please install the following before proceeding: " + str(missing_packages))
                 sys.exit(1)
-    except Exception as e:
+    except Exception:
         pass
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent/agent.py` & `spotinst-agent-2-beta-3.1.14/spotinst_agent/agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,32 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 """Executor:  execute remote scripts periodically.
 
 Usage:  spotinst-agent [options]
 --verbose           verbose logs
 --debug                run with dummy credentials for debug purposes
 """
-from __future__ import print_function
-from __future__ import absolute_import
 
 import logging.handlers
 import signal
 import sys
 import yaml
 from os.path import join
 from time import sleep
-
-if __name__ == '__main__' and __package__ is None:
-    from os import sys, path
-    sys.path.append(path.dirname(path.dirname(path.abspath(__file__))))
-
-from spotinst_agent.agentinit import init__configuration
-from spotinst_agent.taskmanager import TaskManager
+from agentinit import init__configuration
+from taskmanager import TaskManager
 
 
 def run_agent(debug=False, verbose=True):
     # Initialize Config
     cfg_file = join('/etc/spotinst/agent/config/spotinst-agent.yml')
     with open(cfg_file) as f:
         try:
-            config = yaml.safe_load(f)
+            config = yaml.load(f)
         except yaml.YAMLError:
             print("ERROR: Config file: %s does not exist." % cfg_file)
             sys.exit(1)
 
     cloud_provider = get_cloud_provider(config)
 
     # Initialize Logging
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent/agentinit.py` & `spotinst-agent-2-beta-3.1.14/spotinst_agent/agentinit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import absolute_import
 # load credentials
-from builtins import str
 import logging
-from . import utils
-from .utils import safe_read_simple_url, safe_get_json, safe_put_simple_url
+import utils
+from utils import safe_read_simple_url, safe_get_json, safe_put_simple_url
 import os
 
 """
 This is for Elastic group spotinst-agent specific
 """
 
 
@@ -16,16 +14,16 @@
     if debug:
         # for debug
         log.warning("spotinst-agent is running with mock credentials for debug purposes")
         instance_details = {'cloud_provider': 'AWS', 'instance_id': 'i-1234567890',
                             'spectrum_dimensions': ['instance_id'],
                             'authentication_token': 'DUMMY-TOKEN',
                             'host': 'host-123'}
-
-    metadata_token_url = config.get('aws_metadata_service_token_url', None)    
+    
+    metadata_token_url = config.get('aws_metadata_service_token_url', None)
     locator_url = config['aws_instance_id_locator_url']
     instance_id = getAwsInstanceId(locator_url, log, metadata_token_url=metadata_token_url)
     if instance_id and authentication_token:
         instance_details = {'cloud_provider': 'AWS', 'instance_id': instance_id,
                             'authentication_token': authentication_token,
                             'spectrum_dimensions': ['instance_id'],
                             'account_id': account_id,
@@ -124,15 +122,16 @@
     instance_details = None
     log = logging.getLogger('spotinst-agent')
 
     creds = utils.retrieve_creds()
     authentication_token = creds["token"]
     account_id = creds["account_id"]
     host = creds["host"]
-    
+    log.debug("host is {}".format(host))
+
     if cloud_provider.lower() == 'azure':
         instance_details = getAzureInstanceDetails(config, authentication_token, account_id, host, log, debug)
     elif cloud_provider.lower() == 'azure_spot':
         instance_details = getAzureSpotInstanceDetails(config, authentication_token, account_id, host, log, debug)
     elif cloud_provider.lower() == 'gcp':
         instance_details = getGcpInstanceDetails(config, authentication_token, account_id, host, log, debug)
     else:
@@ -141,22 +140,22 @@
 
 
 def getAwsInstanceId(locator_url, log, metadata_token_url=None):
     response = None
     if locator_url:
         if locator_url.startswith("http://"):
             aws_token = None
-
+            
             if metadata_token_url:
                 aws_token = _fetch_aws_metadata_token(metadata_token_url, log=log)
             else:
-                log.error("Url for fetching aws metadata token doen't exists in config")
+                log.error("Url for fetching aws metadata token is None in config")
 
             headers = {}
-            
+
             if aws_token:
                 headers['x-aws-ec2-metadata-token'] = aws_token
             else:
                 log.warn("Failed to retrieve aws token, using IMDSv1 instead")
 
             response = safe_read_simple_url(locator_url, log, headers=headers)
             response = str(response)
@@ -170,20 +169,20 @@
             log.error("response is null, can't get instance id")
             return None
 
     return response
 
 
 def _fetch_aws_metadata_token(token_url, log=logging.getLogger('spotinst-agent'), token_ttl=21600):
-    response = None
     headers = {
         'x-aws-ec2-metadata-token-ttl-seconds': str(token_ttl),
     }
 
     token_response = safe_put_simple_url(token_url, log, headers)
+    response = None
 
     if token_response:
         response = str(token_response)
 
     return response
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent/basemodule.py` & `spotinst-agent-2-beta-3.1.14/spotinst_agent/basemodule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from builtins import object
 import logging
 import traceback
 
 
 class Module(object):
     isModule = True
     """
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-2-beta-3.1.14/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 enable: True
 # interval in seconds
 reload_interval: 120
 aws_instance_id_locator_url: 'http://169.254.169.254/latest/meta-data/instance-id'
 aws_metadata_service_token_url: 'http://169.254.169.254/latest/api/token'
 gcp_instance_metadata_url: 'http://metadata.google.internal/computeMetadata/v1'
 azure_instance_id_locator_url: 'http://169.254.169.254/metadata/instance/compute/vmId?api-version=2017-08-01&format=text'
-azure_spot_instance_id_locator_url: 'http://169.254.169.254/metadata/instance/compute/vmId?api-version=2021-02-01&format=text'
+azure_spot_instance_id_locator_url: 'http://169.254.169.254/metadata/instance/compute/name?api-version=2017-08-01&format=text'
 gcp_instance_name: '/instance/name'
 azure_node_id_path: '/etc/spotinst/nodeId.txt'
 azure_pool_id_path: '/etc/spotinst/poolId.txt'
 cloud_provider_path: '/etc/spotinst/cloud_provider.txt'
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-2-beta-3.1.14/spotinst_agent/data/installation/agent-init.sh`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 	if [ -z "$lsb_dist" ] && [ -r /etc/centos-release ]; then
 		lsb_dist='centos'
 	fi
 	if [ -z "$lsb_dist" ] && [ -r /etc/redhat-release ]; then
 		lsb_dist='redhat'
 	fi
 	if [ -z "$lsb_dist" ] && [ -r /etc/SuSE-release ]; then
-		lsb_dist='sles'
+		lsb_dist='suse'
 	fi
 	if [ -z "$lsb_dist" ] && [ -r /etc/system-release ]; then
 		os=`cat /etc/system-release | awk -F ' ' {'print $1'}`
 
 		if [ "$os" = "CentOS" ]; then
 			lsb_dist='centos'
 		else
@@ -104,59 +104,59 @@
 	fi
 
 	# Run setup for each distro accordingly
 	case "$lsb_dist" in
 		amazon)
 			log_info "Amazon Linux dist detected"
 			log_info "Downloading init.d service file"
-			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent-2/linux-initd/spotinst-agent -o /etc/init.d/spotinst-agent
+			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent/linux-initd/spotinst-agent -o /etc/init.d/spotinst-agent
 			chmod +x /etc/init.d/spotinst-agent
 			return
 			;;
 
 		ubuntu14)
 			log_info "Old Ubuntu (initd) dist detected"
 			log_info "Downloading init.d service file"
-			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent-2/ubuntu-initd/spotinst-agent -o /etc/init.d/spotinst-agent
+			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent/ubuntu-initd/spotinst-agent -o /etc/init.d/spotinst-agent
 			chmod +x /etc/init.d/spotinst-agent
 			return
 			;;
 
-		sles)
+		suse)
 			log_info "SuSE dist detected"
 
 			log_info "Downloading systemd service file"
-			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent-2/spotinst-agent.service -o /etc/systemd/system/spotinst-agent.service
+			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent/spotinst-agent.service -o /etc/systemd/system/spotinst-agent.service
 			log_info "done.."
 			return
 			;;
 
 		ubuntu|debian)
 			log_info "Ubuntu/Debian dist detected"
             log_info "Install dependencies"
             apt-get update
 			apt-get install curl build-essential checkinstall libcap2-bin -y
 
 			log_info "Adding capability +ep"
 			setcap 'cap_net_bind_service=+ep' $SPOTINST_AGENT_PATH
 
 			log_info "Downloading systemd service file"
-			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent-2/spotinst-agent.service -o /lib/systemd/system/spotinst-agent.service
+			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent/spotinst-agent.service -o /lib/systemd/system/spotinst-agent.service
 
 			return
 			;;
 
 		fedora|centos|redhat)
 			log_info "Fedora/CentOS/RedHat dist detected"
 
 			log_info "Adding capability +ep"
 			setcap 'cap_net_bind_service=+ep' $SPOTINST_AGENT_PATH
 
 			log_info "Downloading systemd service file"
-			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent-2/spotinst-agent.service -o /lib/systemd/system/spotinst-agent.service
+			curl -sL http://spotinst-public.s3.amazonaws.com/services/spotinst-agent/spotinst-agent.service -o /lib/systemd/system/spotinst-agent.service
 
 			return
 			;;
 
 		*)
 			# intentionally mixed spaces and tabs here -- tabs are stripped by "<<-'EOF'", spaces are kept in the output
 			cat >&2 <<-'EOF'
@@ -201,15 +201,15 @@
 
 		ubuntu14)
 			log_info "Old Ubuntu (initd) dist detected"
 			/etc/init.d/spotinst-agent restart
 			return
 			;;
 
-		sles)
+		suse)
 			log_info "SuSE dist detected"
 			/bin/systemctl daemon-reload
 			/bin/systemctl restart spotinst-agent
 			/bin/systemctl enable spotinst-agent
 			return
 			;;
 
@@ -262,18 +262,14 @@
   local readonly timestamp="$1"
   shift
   local readonly log_level="$1"
   shift
   local readonly message="$@"
   echo -e "${timestamp} [${log_level}] ${message}"
 }
-log_info "Installation of the Spot Agent is governed by NetApp’s end user license agreement (“EULA”), which can be found at:
-          https://www.netapp.com/how-to-buy/sales-terms-and-conditions/
-          By installing the Spot Agent, you accept and approve the EULA."
-
 log_info "Validating before install..."
 validate
 
 log_info "Installing..."
 install
 
 log_info "Cleaning up after install..."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent/scheduler.py` & `spotinst-agent-2-beta-3.1.14/spotinst_agent/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,15 @@
 and slightly changed to be completely stand-alone again. Also some fixes
 have been made to make it work on Python 2.6 (sched module changes).
 The version in Turbogears is based on the original stand-alone Kronos.
 This is open-source software, released under the MIT Software License:
 http://www.opensource.org/licenses/mit-license.php
 
 """
-from __future__ import print_function
 
-from builtins import object
 __version__ = "2.0"
 
 __all__ = [
     "DayTaskRescheduler",
     "ForkedIntervalTask",
     "ForkedMonthdayTask",
     "ForkedScheduler",
@@ -76,15 +74,15 @@
 import sched
 import time
 import logging
 import traceback
 import weakref
 
 
-class method(object):
+class method:
     sequential = "sequential"
     forked = "forked"
     threaded = "threaded"
 
 
 class SchedulerNotRunning(Exception):
     """Interrupt a running scheduler.
@@ -92,15 +90,15 @@
     This exception is used to break out of sched.sched.run when we
     are not running.
 
     """
     pass
 
 
-class Scheduler(object):
+class Scheduler:
     """The Scheduler itself."""
 
     def __init__(self):
         self.running = True
         self.log = logging.getLogger('diamond')
         self.sched = sched.scheduler(time.time, self.__delayfunc)
 
@@ -292,15 +290,15 @@
     def _run(self):
         # Low-level run method to do the actual scheduling loop.
         while self.running:
             try:
                 self.sched.run()
             except SchedulerNotRunning:
                 self._clearschedqueue()
-            except Exception as x:
+            except Exception, x:
                 self.log.error(
                     "ERROR DURING SCHEDULER EXECUTION %s \n %s",
                     x,
                     "".join(traceback.format_exception(*sys.exc_info())))
             # queue is empty; sleep a short while before checking again
             if self.running:
                 time.sleep(5)
@@ -317,15 +315,15 @@
         self.kw = kw
         self.log = logging.getLogger('diamond')
 
     def __call__(self, schedulerref):
         """Execute the task action in the scheduler's thread."""
         try:
             self.execute()
-        except Exception as x:
+        except Exception, x:
             self.handle_exception(x)
         self.reschedule(schedulerref())
 
     def reschedule(self, scheduler):
         """This method should be defined in one of the sub classes!"""
         raise NotImplementedError("You're using the abstract class 'Task',"
                                   " use a concrete class instead")
@@ -370,15 +368,15 @@
                 scheduler.schedule_task(self, self.interval - self.duration)
             else:
                 scheduler.schedule_task(self, 0)
         else:
             scheduler.schedule_task(self, self.interval)
 
 
-class DayTaskRescheduler(object):
+class DayTaskRescheduler:
     """A mixin class that contains the reschedule logic for the DayTasks."""
 
     def __init__(self, timeonday):
         self.timeonday = timeonday
 
     def get_schedule_time(self, today):
         """Calculate the time value at which this task is to be scheduled."""
@@ -484,28 +482,28 @@
             """Lock the thread's task queue."""
             self._lock.acquire()
 
         def _release_lock(self):
             """Release the lock on the thread's task queue."""
             self._lock.release()
 
-    class ThreadedTaskMixin(object):
+    class ThreadedTaskMixin:
         """A mixin class to make a Task execute in a separate thread."""
 
         def __call__(self, schedulerref):
             """Execute the task action in its own thread."""
             threading.Thread(target=self.threadedcall).start()
             self.reschedule(schedulerref())
 
         def threadedcall(self):
             # This method is run within its own thread, so we have to
             # do the execute() call and exception handling here.
             try:
                 self.execute()
-            except Exception as x:
+            except Exception, x:
                 self.handle_exception(x)
 
     class ThreadedIntervalTask(ThreadedTaskMixin, IntervalTask):
         """Interval Task that executes in its own thread."""
 
         def __init__(self, name, interval, action, args=None, kw=None,
                      abs=False):
@@ -559,25 +557,25 @@
             """Stop the scheduler and wait for the process to finish."""
             os.kill(self.childpid, signal.SIGUSR1)
             os.waitpid(self.childpid, 0)
 
         def signalhandler(self, sig, stack):
             Scheduler.stop(self)
 
-    class ForkedTaskMixin(object):
+    class ForkedTaskMixin:
         """A mixin class to make a Task execute in a separate process."""
 
         def __call__(self, schedulerref):
             """Execute the task action in its own process."""
             pid = os.fork()
             if pid == 0:
                 # we are the child
                 try:
                     self.execute()
-                except Exception as x:
+                except Exception, x:
                     self.handle_exception(x)
                 os._exit(0)
             else:
                 # we are the parent
                 self.reschedule(schedulerref())
 
     class ForkedIntervalTask(ForkedTaskMixin, IntervalTask):
@@ -601,17 +599,17 @@
 
     class ForkedMonthdayTask(ForkedTaskMixin, MonthdayTask):
         """Monthday Task that executes in its own process."""
         pass
 
 if __name__ == "__main__":
     def testaction(arg):
-        print((">>>TASK", arg, "sleeping 3 seconds"))
+        print (">>>TASK", arg, "sleeping 3 seconds")
         time.sleep(3)
-        print(("<<<END_TASK", arg))
+        print ("<<<END_TASK", arg)
 
     s = ThreadedScheduler()
     s.add_interval_task(testaction,
                         "test action 1",
                         0,
                         4,
                         method.threaded,
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent/taskmanager.py` & `spotinst-agent-2-beta-3.1.14/spotinst_agent/taskmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from __future__ import absolute_import
-from builtins import str, object, dict
 import inspect
 import logging
 import os
 import sys
 import time
 import traceback
 
-from .scheduler import ThreadedScheduler, method
-from .utils import load_class_from_name
-from . import basemodule
+from scheduler import ThreadedScheduler, method
+from utils import load_class_from_name
+import basemodule
 
 
 class TaskManager(object):
     """
     Class
     """
 
@@ -129,15 +127,15 @@
                     continue
 
                 modname = f[:-3]
                 mod_modification_time = os.path.getmtime(os.path.join(path, f))
                 mod_modification_time_str = str(mod_modification_time)
                 self.log.info("Py file found: %s" % modname)
 
-                modules_list = [x.lower() for x in self.tasks]
+                modules_list = [x.lower() for x in self.tasks.keys()]
                 if modname in modules_list:
                     if self.tasks[modname]['modification_time'] == mod_modification_time_str:
                         self.log.info("Module '{0}' already loaded".format(modname))
                         continue
 
                 if modname == "utils" or modname == "basemodule":
                     continue
@@ -160,17 +158,15 @@
                 # Find all classes defined in the module
                 self.log.info("Finding classes defined in module " + str(modname))
                 for attrname in dir(mod):
                     attr = getattr(mod, attrname)
                     # Only attempt to load classes that are infact classes but not the base Module class
                     self.log.debug("Checking " + str(modname) + " Attribute " + str(attrname))
 
-                    # After upgrading to python 3 the condition of `attr != basemodule.Module` stopped working what caused
-                    # the code to try and load Module and failed to prevent this behaviour I added the condition `attrname != "Module"`
-                    if inspect.isclass(attr) and isModule(attr) and attr != basemodule.Module and attrname != "Module":
+                    if inspect.isclass(attr) and isModule(attr) and attr != basemodule.Module:
                         # Get class name
                         fqcn = '.'.join([modname, attrname])
                         self.log.info("Module loaded : " + fqcn)
                         try:
                             # Load Module class
                             cls = load_class_from_name(fqcn)
                             # Add Module class
@@ -261,15 +257,15 @@
                     self.scheduler.cancel(self.tasks[module['file_name']]['task'])
                     # Log
                     self.log.info("Canceled task: %s" % name)
                 except ValueError as e:
                     self.log.error("Unable to cancel task '{0}' - {1}".format(self.tasks[name], e))
 
             # Schedule Collector
-            self.log.info("Scheduled task {0} to run every {1}s (delayed of {2}s)".format(name, interval, splay))
+            self.log.info("Scheduled task {0} to run once. (delay of {1})".format(name, splay))
             task = self.scheduler.add_single_task(func, name, splay, method.sequential,
                                                   args, None)
 
             self.log.debug("Scheduled task: %s" % name)
             # Add task to list
             self.tasks[module['file_name']] = {'task': task, 'modification_time': module['modification_time']}
 
@@ -278,15 +274,15 @@
         Close and stop all tasks.
         """
         # Set Running Flag
         self.running = False
 
         self.log.info('Stopped task scheduler.')
 
-        for key, task in self.tasks.items():
+        for key, task in self.tasks.iteritems():
             try:
                 self.scheduler.cancel(task['task'])
                 # Log
                 self.log.info("Canceled task: %s" % key)
             except ValueError as e:
                 self.log.error("Cancel task exception '{0}' - {1}".format(key, e))
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent/utils.py` & `spotinst-agent-2-beta-3.1.14/spotinst_agent/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-from __future__ import print_function
-from future import standard_library
-standard_library.install_aliases()
-from builtins import str
 import inspect
-import http.client
+import httplib
 import json
 import logging
 import os
 import sys
 from _ssl import SSLError
 from json import loads
-from urllib.request import Request, urlopen
-from urllib.error import HTTPError, URLError
+from urllib2 import Request, urlopen, HTTPError, URLError
 import yaml
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
 
 def safeget(dct, *keys):
     ret = None
@@ -39,15 +34,15 @@
 
 def safe_read_simple_url(url, log=logging.getLogger('spotinst-agent'), headers={}):
     try:
         log.debug("reading simple {} ...".format(url))
         req = Request(url, headers=headers)
         req.add_header('Content-Type', 'application/json')
         response = urlopen(req, timeout=10)
-        return response.read().decode('utf-8')
+        return response.read()
     except HTTPError as e:
         log.error("The server can't fulfill the GET {} request. [reason: {}]".format(url, e.reason))
     except URLError as e:
         log.error("Unable to reach the server for GET request. [reason: {}]".format(e.reason))
     except Exception as e:
         log.error("There was an error of GET url {}: {}".format(url, e.__str__()))
     finally:
@@ -63,15 +58,15 @@
     try:
         log.debug("reading simple {} ...".format(url))
         req = Request(url, headers=headers)
         req.get_method = lambda: 'PUT'
         response = urlopen(req, timeout=10)
 
         if response.code == 200:
-            ret_val = response.read().decode('utf-8')
+            ret_val = response.read()
     except HTTPError as e:
         log.error("The server can't fulfill the PUT {} request. [reason: {}]".format(url, e.reason))
     except URLError as e:
         log.error("Unable to reach the server for PUT {} request. [reason: {}]".format(url, e.reason))
     except Exception as e:
         log.error("There was an error of PUT url {}: {}".format(url, e.__str__()))
     finally:
@@ -87,15 +82,15 @@
     try:
         url = url + path_params
         log.debug("reading simple {} ...".format(url))
         req = Request(url)
         #req.add_header('Content-Type', 'application/json')
         req.add_header('Metadata-Flavor','Google')
         response = urlopen(req, timeout=10)
-        return response.read().decode('utf-8')
+        return response.read()
     except HTTPError as e:
         log.error("The server can't fulfill the GET {} request. [reason: {}]".format(url, e.reason))
     except URLError as e:
         log.error("Unable to reach the server for GET request. [reason: {}]".format(e.reason))
     except Exception as e:
         log.error("There was an error of GET url {}: {}".format(url, e.__str__()))
     finally:
@@ -107,15 +102,15 @@
 # getting vmId - not whole the metadata
 def get_azure_metadata(url, log=logging.getLogger('spotinst-agent')):
     try:
         log.debug("reading simple {} ...".format(url))
         req = Request(url)
         req.add_header('Metadata', 'true')
         response = urlopen(req, timeout=10)
-        return response.read().decode('utf-8')
+        return response.read()
     except HTTPError as e:
         log.error("The server can't fulfill the GET {} request. [reason: {}]".format(url, e.reason))
     except URLError as e:
         log.error("Unable to reach the server for GET request. [reason: {}]".format(e.reason))
     except Exception as e:
         log.error("There was an error of GET url {}: {}".format(url, e.__str__()))
     finally:
@@ -189,15 +184,15 @@
         return body
     except HTTPError as e:
         log.error("The server can't fulfill the POST {} request. [reason: {}]".format(url, e.reason))
     except URLError as e:
         log.error("Unable to reach the server for POST request. [reason: {}]".format(e.reason))
     except SSLError as e:
         log.error("Connection to API timed out, retry in next iteration : {}".format(str(e)))
-    except http.client.BadStatusLine as e:
+    except httplib.BadStatusLine as e:
         log.error("Bad status line. The URL is most likely wrong.")
     except Exception as e:
         log.error("There was an error of POST url. Exceptions: " + str(sys.exc_info()[0]))
     finally:
         try:
             response.close()
         except NameError:
@@ -233,15 +228,15 @@
             pass
 
 
 def parse_yml(yml, log=logging.getLogger('spotinst-agent')):
     # Initialize Config
     with open(yml) as f:
         try:
-            return yaml.safe_load(f)
+            return yaml.load(f)
         except Exception as e:
             log.error("Can't parse yml file {}. Exception {}".format(yml, e))
             raise e
 
 
 def load_class_from_name(fqcn):
     # Break apart fqcn to get module and classname
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/PKG-INFO` & `spotinst-agent-2-beta-3.1.14/spotinst_agent_2_beta.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,59 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: spotinst-agent-2-beta
-Version: 3.1.13
+Version: 3.1.14
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
-Description: Agent
-        =======
-        
-        Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
-        
-        Note:
-        The agent must have token to communicate with spotinst API.
-        The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
-        
-        Application
-        ===========
-        
-        Manual Executing
-        ~~~~~~~~~~~~~~~~
-        The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
-        
-        Otherwise, you can use the following options:
-        
-        Usage:  ./agent [options]
-        
-        -c --config            Use alternate configuration yml file.
-        -l --log               Use alternate Log file for output.
-        -t --test              Test run.  Do not run remote script.
-        -v --verbose           verbose log
-        --stdout               redirect output to stdout
-        --debug                run with dummy credentials for debug purposes
-        
-        Configuration
-        ~~~~~~~~~~~~~
-        There are two levels of configuration representing in yml files.
-        The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
-        The worker configuration, located at the workers folder is responsible of the specific workers parameters.
-        
-        
-        MAKEFILE
-        ~~~~~~~~~~~~~
-        run 'make release'
-        output file is located in the /dist folder
-        
-        Documentation
-        =============
-        
 Keywords: spotinst agent infrastructure monitoring execution deployment
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ==3.*
+Classifier: Programming Language :: Python :: 2.7
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pyyaml
+
+Agent
+=======
+
+Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
+
+Note:
+The agent must have token to communicate with spotinst API.
+The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
+
+Application
+===========
+
+Manual Executing
+~~~~~~~~~~~~~~~~
+The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
+
+Otherwise, you can use the following options:
+
+Usage:  ./agent [options]
+
+-c --config            Use alternate configuration yml file.
+-l --log               Use alternate Log file for output.
+-t --test              Test run.  Do not run remote script.
+-v --verbose           verbose log
+--stdout               redirect output to stdout
+--debug                run with dummy credentials for debug purposes
+
+Configuration
+~~~~~~~~~~~~~
+There are two levels of configuration representing in yml files.
+The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
+The worker configuration, located at the workers folder is responsible of the specific workers parameters.
+
+
+MAKEFILE
+~~~~~~~~~~~~~
+run 'make release'
+output file is located in the /dist folder
+
+Documentation
+=============
```

### Comparing `spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/SOURCES.txt` & `spotinst-agent-2-beta-3.1.14/spotinst_agent_2_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

