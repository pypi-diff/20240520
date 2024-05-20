# Comparing `tmp/spotinst-agent-beta-2.2.287.tar.gz` & `tmp/spotinst-agent-beta-2.2.288.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spotinst-agent-beta-2.2.287.tar", last modified: Wed May  1 12:50:39 2024, max compression
+gzip compressed data, was "dist/spotinst-agent-beta-2.2.288.tar", last modified: Sun May 19 12:19:48 2024, max compression
```

## Comparing `spotinst-agent-beta-2.2.287.tar` & `spotinst-agent-beta-2.2.288.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/
--rw-r--r--   0 mavni      (501) staff       (20)     2277 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/PKG-INFO
--rw-r--r--   0 mavni      (501) staff       (20)      181 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/MANIFEST.in
--rwxr-xr-x   0 mavni      (501) staff       (20)     1392 2024-05-01 12:30:29.000000 spotinst-agent-beta-2.2.287/setup.py
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent_beta.egg-info/
--rw-r--r--   0 mavni      (501) staff       (20)     2277 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 mavni      (501) staff       (20)      630 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 mavni      (501) staff       (20)       56 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 mavni      (501) staff       (20)       16 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 mavni      (501) staff       (20)       15 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent_beta.egg-info/top_level.txt
--rw-r--r--   0 mavni      (501) staff       (20)        1 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 mavni      (501) staff       (20)       38 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/setup.cfg
--rw-r--r--   0 mavni      (501) staff       (20)     1287 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/README.rst
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent/
--rw-r--r--   0 mavni      (501) staff       (20)     9604 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/spotinst_agent/agentinit.py
--rw-r--r--   0 mavni      (501) staff       (20)     1129 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/spotinst_agent/basemodule.py
--rw-r--r--   0 mavni      (501) staff       (20)    12676 2024-05-01 12:30:26.000000 spotinst-agent-beta-2.2.287/spotinst_agent/__init__.py
--rw-r--r--   0 mavni      (501) staff       (20)    10751 2024-05-01 12:30:26.000000 spotinst-agent-beta-2.2.287/spotinst_agent/taskmanager.py
--rw-r--r--   0 mavni      (501) staff       (20)     9420 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/spotinst_agent/utils.py
--rw-r--r--   0 mavni      (501) staff       (20)     3116 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/spotinst_agent/agent.py
--rw-r--r--   0 mavni      (501) staff       (20)    21605 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/spotinst_agent/scheduler.py
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent/data/
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent/data/configuration/
--rw-r--r--   0 mavni      (501) staff       (20)      180 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 mavni      (501) staff       (20)      727 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 12:50:39.000000 spotinst-agent-beta-2.2.287/spotinst_agent/data/installation/
--rwxr-xr-x   0 mavni      (501) staff       (20)     6691 2024-05-01 09:00:13.000000 spotinst-agent-beta-2.2.287/spotinst_agent/data/installation/agent-init.sh
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/
+-rw-r--r--   0 bsaada     (502) staff       (20)     2277 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/PKG-INFO
+-rw-r--r--   0 bsaada     (502) staff       (20)      181 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/MANIFEST.in
+-rwxr-xr-x   0 bsaada     (502) staff       (20)     1392 2024-05-19 12:10:11.000000 spotinst-agent-beta-2.2.288/setup.py
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 bsaada     (502) staff       (20)     2277 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 bsaada     (502) staff       (20)      630 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       56 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       16 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       15 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/top_level.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)        1 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 bsaada     (502) staff       (20)       38 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/setup.cfg
+-rw-r--r--   0 bsaada     (502) staff       (20)     1287 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/README.rst
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent/
+-rw-r--r--   0 bsaada     (502) staff       (20)     9604 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/agentinit.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     1129 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/basemodule.py
+-rw-r--r--   0 bsaada     (502) staff       (20)    13098 2024-05-19 12:02:38.000000 spotinst-agent-beta-2.2.288/spotinst_agent/__init__.py
+-rw-r--r--   0 bsaada     (502) staff       (20)    10733 2024-05-19 12:02:38.000000 spotinst-agent-beta-2.2.288/spotinst_agent/taskmanager.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     9420 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/utils.py
+-rw-r--r--   0 bsaada     (502) staff       (20)     3116 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/agent.py
+-rw-r--r--   0 bsaada     (502) staff       (20)    21605 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/scheduler.py
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/configuration/
+-rw-r--r--   0 bsaada     (502) staff       (20)      180 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 bsaada     (502) staff       (20)      727 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 bsaada     (502) staff       (20)        0 2024-05-19 12:19:48.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/installation/
+-rwxr-xr-x   0 bsaada     (502) staff       (20)     6691 2024-05-19 12:02:06.000000 spotinst-agent-beta-2.2.288/spotinst_agent/data/installation/agent-init.sh
```

### Comparing `spotinst-agent-beta-2.2.287/PKG-INFO` & `spotinst-agent-beta-2.2.288/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: spotinst-agent-beta
-Version: 2.2.287
+Version: 2.2.288
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Description: Agent
         =======
```

### Comparing `spotinst-agent-beta-2.2.287/setup.py` & `spotinst-agent-beta-2.2.288/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.287",
+    version="2.2.288",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: spotinst-agent-beta
-Version: 2.2.287
+Version: 2.2.288
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Description: Agent
         =======
```

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.288/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.287/README.rst` & `spotinst-agent-beta-2.2.288/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.288/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.288/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.288/spotinst_agent/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,34 +68,35 @@
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
@@ -113,15 +114,15 @@
         full_path = instance_details_path + "/cloud_provider.txt"
         cloud_provider_file = open(full_path, 'w')
         cloud_provider_file.write(cloud_provider)
         cloud_provider_file.close()
         os.chmod(full_path, 0o644)
         return True
     except IOError:
-        print "Unable to create /etc/spotinst/cloud_provider.txt"
+        print("Unable to create /etc/spotinst/cloud_provider.txt")
         if cloud_provider_file is not None:
             cloud_provider_file.close()
         return False
 
 
 def create_agent_local_folders():
     if not os.path.exists('/etc/spotinst'):
@@ -130,19 +131,25 @@
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
 
 
@@ -243,14 +250,15 @@
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
@@ -270,22 +278,22 @@
     with open(modules_path + '/' + collector_name + '.py', 'wb') as collector:
         response = urllib2.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.py')
         collector.write(response.read())
     with open(modules_path + '/' + collector_name + '.yml', 'wb') as collector_cfg:
         response = urllib2.urlopen(s3_base_collectors_link + '/' + collector_name + '/' + collector_name + '.yml')
         collector_cfg.write(response.read())
 
+
 def get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link):
-    with open(initiator_modules_path + '/' + initiator_name + '.py', 'wb') as initiator:
-        response = urllib2.request.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.py')
-        initiator.write(response.read())
-    with open(initiator_modules_path + '/' + initiator_name + '.yml', 'wb') as initiator_cfg:
-        response = urllib2.request.urlopen(
-            s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.yml')
-        initiator_cfg.write(response.read())
+    with open(initiator_modules_path + '/' + initiator_name + '.py', 'wb') as collector:
+        response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.py')
+        collector.write(response.read())
+    with open(initiator_modules_path + '/' + initiator_name + '.yml', 'wb') as collector_cfg:
+        response = urllib2.urlopen(s3_base_initiator_link + '/' + initiator_name + '/' + initiator_name + '.yml')
+        collector_cfg.write(response.read())
 
 def handle_prerequisites(s3_base_module_link, module_name):
     try:
         response = urllib2.urlopen(s3_base_module_link + '/' + module_name + '/' + module_name + '.req')
         requirements_file = response.read()
         requirements_names = requirements_file.split("\n")
         print ("This module requires the following packages to be installed:")
```

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.288/spotinst_agent/taskmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
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
```

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.288/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.288/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.288/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.288/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.287/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.288/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

