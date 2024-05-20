# Comparing `tmp/boman-cli-1.5.tar.gz` & `tmp/boman-cli-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boman-cli-1.5.tar", last modified: Tue Apr 25 09:57:24 2023, max compression
+gzip compressed data, was "boman-cli-1.6.tar", last modified: Mon May 20 13:24:06 2024, max compression
```

## Comparing `boman-cli-1.5.tar` & `boman-cli-1.6.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2023-04-25 09:57:24.104062 boman-cli-1.5/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2064 2023-04-25 09:57:24.104062 boman-cli-1.5/PKG-INFO
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1189 2023-04-25 09:54:14.000000 boman-cli-1.5/README.md
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2023-04-25 09:57:24.100062 boman-cli-1.5/boman_cli.egg-info/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2064 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/PKG-INFO
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      388 2023-04-25 09:57:24.000000 boman-cli-1.5/boman_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        1 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       53 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/entry_points.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       45 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/requires.txt
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        9 2023-04-25 09:57:23.000000 boman-cli-1.5/boman_cli.egg-info/top_level.txt
-drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2023-04-25 09:57:24.104062 boman-cli-1.5/bomancli/
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1774 2023-04-25 09:51:00.000000 boman-cli-1.5/bomancli/Config.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        0 2023-04-25 09:42:53.000000 boman-cli-1.5/bomancli/_init_.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2176 2023-04-25 09:45:35.000000 boman-cli-1.5/bomancli/auth.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      968 2022-11-21 13:35:27.000000 boman-cli-1.5/bomancli/base_logger.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1340 2022-11-21 13:35:27.000000 boman-cli-1.5/bomancli/loc_finder.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)    32981 2023-04-25 09:55:05.000000 boman-cli-1.5/bomancli/main.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     9230 2023-04-25 09:52:22.000000 boman-cli-1.5/bomancli/utils.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     7848 2023-04-25 09:42:53.000000 boman-cli-1.5/bomancli/validation.py
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      101 2023-04-25 09:57:24.104062 boman-cli-1.5/setup.cfg
--rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1575 2023-04-25 09:42:53.000000 boman-cli-1.5/setup.py
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-20 13:24:06.644035 boman-cli-1.6/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2657 2024-05-20 13:24:06.644035 boman-cli-1.6/PKG-INFO
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1607 2024-05-20 13:21:01.000000 boman-cli-1.6/README.md
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-20 13:24:06.640035 boman-cli-1.6/boman_cli.egg-info/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2657 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      426 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        1 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       53 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)       45 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/requires.txt
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        9 2024-05-20 13:24:06.000000 boman-cli-1.6/boman_cli.egg-info/top_level.txt
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-20 13:24:06.640035 boman-cli-1.6/bomancli/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2353 2024-05-20 12:43:07.000000 boman-cli-1.6/bomancli/Config.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)        0 2023-12-12 08:27:09.000000 boman-cli-1.6/bomancli/_init_.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     2306 2024-05-14 06:41:19.000000 boman-cli-1.6/bomancli/auth.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1203 2024-03-20 08:09:57.000000 boman-cli-1.6/bomancli/base_logger.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1702 2024-03-23 11:50:57.000000 boman-cli-1.6/bomancli/loc_finder.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)    39585 2024-05-20 13:14:09.000000 boman-cli-1.6/bomancli/main.py
+drwxrwxr-x   0 boxuser   (1000) boxuser   (1000)        0 2024-05-20 13:24:06.644035 boman-cli-1.6/bomancli/templates/
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     4529 2024-05-15 08:44:53.000000 boman-cli-1.6/bomancli/templates/template_plan.yaml
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)    25357 2024-05-20 12:42:11.000000 boman-cli-1.6/bomancli/utils.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     7696 2024-02-14 08:06:15.000000 boman-cli-1.6/bomancli/validation.py
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)      144 2024-05-20 13:24:06.644035 boman-cli-1.6/setup.cfg
+-rw-rw-r--   0 boxuser   (1000) boxuser   (1000)     1768 2024-05-20 12:43:34.000000 boman-cli-1.6/setup.py
```

### Comparing `boman-cli-1.5/PKG-INFO` & `boman-cli-1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boman-cli
-Version: 1.5
+Version: 1.6
 Summary: CLI tool of boman.ai
 Home-page: https://boman.ai
 Author: Sumeru Software Solutions Pvt. Ltd.
 Author-email: support@boman.ai
 License: BSD 2-clause
 Description: # Introduction 
         Boman CLI is a Orchestration script written in python to run security scans on the customer's local or CI/CD environment and upload the results to Boman.ai SaaS server.
@@ -34,39 +34,64 @@
         ` boman-cli -a run`
         
         ### To run the scan on specific Boman SaaS URL (On prem)
         
         ` boman-cli -a run -u {URL}`
         
         
-        ### releases:
+        ### To fail build on high/medium/low finding is detected
         
-        #### v1.02 with following changes:
+        `boman-cli -a run -fb {severity}`
         
-        Version with synk integration, codeql csharp build, exit code sorted
-        added option to fail/pass build, dast error sorted
-        Snyk feature added and upload logs to saas function added
+        Severity can be high, medium or low.
         
+        Example: boman-cli -a run -fb high
         
-        ### v1.3:
         
+        ### To custom change the boman.yaml file, pass the custom file name as input for -config argument
         
-        SCA scan bug fixed
+        `boman-cli -a run -config <custom_boman_yaml_file_name_here>`
         
+        Example: boman-cli -a run -config ./customboman.yaml
         
         
-        ### V1.4
+        ### To inject custom zap auth session script file, pass the custom file name as input for -zap_session_script argument
+        
+        `boman-cli -a run -zap_session_script <custom_session_script_file_name_here>`
+        
+        Example: boman-cli -a run -zap_session_script ./session.js
+        
+        
+        
+        
+        # Error codes & meannings
+        
+        0  : Successfull scan
+        1  : Server/SaaS error
+        2  : Auth error
+        3  : Docker/System error
+        4  : Misconfig error
+        
+        
+        
+        
+        ### Release Note:
+        
+        
+        ### V1.6:
+        
+            - Zap Authenticated scan 
+            - Fetch Git details
+            - custom boman.yaml and zap session script load option
+        
+        Released on: 20 May 2024
         
-        Added scanning on jenkins env with limited permission for SAST/DAST scans.
-        check-user argument added in --action, to check the permssion of the running user.
         
         
         
-        ### V1.5
         
-        Failing Build Filter implemented, you can now pass values sucha as 'only-high,only-medium,only-low' to the -fb argument.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `boman-cli-1.5/boman_cli.egg-info/PKG-INFO` & `boman-cli-1.6/boman_cli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boman-cli
-Version: 1.5
+Version: 1.6
 Summary: CLI tool of boman.ai
 Home-page: https://boman.ai
 Author: Sumeru Software Solutions Pvt. Ltd.
 Author-email: support@boman.ai
 License: BSD 2-clause
 Description: # Introduction 
         Boman CLI is a Orchestration script written in python to run security scans on the customer's local or CI/CD environment and upload the results to Boman.ai SaaS server.
@@ -34,39 +34,64 @@
         ` boman-cli -a run`
         
         ### To run the scan on specific Boman SaaS URL (On prem)
         
         ` boman-cli -a run -u {URL}`
         
         
-        ### releases:
+        ### To fail build on high/medium/low finding is detected
         
-        #### v1.02 with following changes:
+        `boman-cli -a run -fb {severity}`
         
-        Version with synk integration, codeql csharp build, exit code sorted
-        added option to fail/pass build, dast error sorted
-        Snyk feature added and upload logs to saas function added
+        Severity can be high, medium or low.
         
+        Example: boman-cli -a run -fb high
         
-        ### v1.3:
         
+        ### To custom change the boman.yaml file, pass the custom file name as input for -config argument
         
-        SCA scan bug fixed
+        `boman-cli -a run -config <custom_boman_yaml_file_name_here>`
         
+        Example: boman-cli -a run -config ./customboman.yaml
         
         
-        ### V1.4
+        ### To inject custom zap auth session script file, pass the custom file name as input for -zap_session_script argument
+        
+        `boman-cli -a run -zap_session_script <custom_session_script_file_name_here>`
+        
+        Example: boman-cli -a run -zap_session_script ./session.js
+        
+        
+        
+        
+        # Error codes & meannings
+        
+        0  : Successfull scan
+        1  : Server/SaaS error
+        2  : Auth error
+        3  : Docker/System error
+        4  : Misconfig error
+        
+        
+        
+        
+        ### Release Note:
+        
+        
+        ### V1.6:
+        
+            - Zap Authenticated scan 
+            - Fetch Git details
+            - custom boman.yaml and zap session script load option
+        
+        Released on: 20 May 2024
         
-        Added scanning on jenkins env with limited permission for SAST/DAST scans.
-        check-user argument added in --action, to check the permssion of the running user.
         
         
         
-        ### V1.5
         
-        Failing Build Filter implemented, you can now pass values sucha as 'only-high,only-medium,only-low' to the -fb argument.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `boman-cli-1.5/bomancli/auth.py` & `boman-cli-1.6/bomancli/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 
 ## function to authorize and get the images form SAAS --------------------------------------------------------
 def authorize():
     logging.info('Authenticating with boman server')
     url = Config.boman_url+"/api/app/authorize"
-    data = {'app_token': Config.app_token, 'customer_token': Config.customer_token, 'sast':Config.sast_present,"dast":Config.dast_present,"dast_type":Config.dast_type,"sast_langs":Config.sast_lang,"sca":Config.sca_present,"sca_langs":Config.sca_lang,"secret_scan":Config.secret_scan_present}
+    data = {'app_token': Config.app_token, 'customer_token': Config.customer_token, 'sast':Config.sast_present,"dast":Config.dast_present,"dast_type":Config.dast_type,"dast_auth_enabled":Config.dast_auth_present,"sast_langs":Config.sast_lang,"sca":Config.sca_present,"sca_langs":Config.sca_lang,"secret_scan":Config.secret_scan_present}
     headers = {'Content-type': 'application/json', 'Accept': 'text/plain'}
     try:
         res = requests.post(url, json=data, headers=headers)
         #print('req:', json.dumps(data))
         #print('res:',json.loads(res.content))
     except requests.ConnectionError:
        logging.error("Can't connect to the Server while authorizing, Please check your Internet connection.")
@@ -34,14 +34,15 @@
                 Config.sca_response = json_response['data']['sca']
                 Config.secret_scan_response = json_response['data']['secret_scan']
                 Config.scan_token = json_response['data']['scan_token']    
                 Config.scan_name = json_response['data']['scan_name']    
 
                 return 1    
             except:
-                logging.error('Problem when authenticating with server, Check with boman.ai team id scan doesnt completed')  
+                logging.error('Problem when authenticating with server, Check with boman.ai team id scan doesnt completed') 
+                #uploadLogs() this wont work because the scan is not initated.
                 exit(1) ## server error  
                     
 
         elif res.status_code == 401:
-            logging.error('Unauthorized Access. Check the tokens')	
+            logging.error('Unauthorized Access. Check the tokens')	       
     exit(2) ##auth error
```

### Comparing `boman-cli-1.5/bomancli/main.py` & `boman-cli-1.6/bomancli/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 from bomancli import utils as Utils
 from bomancli import auth as Auth
 
 
 parser = argparse.ArgumentParser(
 	prog='bomancli',
 	description='''
-	#This is a CLI tool to communicate with Boman.ai server
+	#This is a CLI tool to communicate with Boman.ai SaaS server
 	''',
-	epilog='copyright (c) 2022 SUMERU'
+	epilog='copyright (c) 2024 SUMERU'
 	)
 
 
 docker = Config.docker_client
 
 ### function to init the scan and will check the docker is in place
 def init():
@@ -96,17 +96,19 @@
         uid = os.getuid()
         gid = os.getgid()
 
 
         if Config.jenkins == 'yes':
             logging.info('Checking user permission for jenkins environment')
             userid = 'root'
+            Config.userid = userid
         else:
             logging.info('Checking user permission')
             userid= f"{uid}:{gid}"
+            Config.userid = userid
 
     except:
         userid= 'root'
 
     logging.info('Running all the scans/docker with the user %s',userid)
 
 
@@ -269,31 +271,92 @@
             msg='Error while uploading the report'
             Utils.logError(msg,e)
 
     if type == 'DAST':
 
         Utils.checkImageAlreadyExsist(docker_image)
         logging.info('Running %s on %s ',tool_name, Config.dast_target)
+        logging.info('Checking DAST Auth is configuration..')
+
+
+        if Config.dast_auth_present == True:
+            logging.info('DAST Auth is configured')
+
+            # if Config.custom_zap_auth_method == True:
+            #     logging.info('Custom auth method is choosen')
+            # else:
+
+            logging.info('Auth config details will be fetched from saas')
+            logging.info('Fetching DAST Auth from SaaS')
+            Utils.fetchDASTConigFromSaas()
+            if Config.zap_plan_config is None:
+                logging.info('Failed getting DAST Auth from SaaS')
+                logging.info('Proceeding with DAST Baseline Scan') 
+                
+            else:
+                logging.info('Configured Auth method is : %s',str(Config.zap_plan_config['auth_method']))
+
+                if Config.zap_plan_config['auth_method'] == 'form':
+                    logging.info('Creating Zap plan')
+                    # if Config.custom_zap_plan_present:
+                    #     logging.info('Custom Zap plan is configured %s',Config.zap_plan_config_file_name)   
+                    # else:
+                    Utils.createZapPlan(Config.zap_plan_config,output_file)          
+                    #return 0
+                elif Config.zap_plan_config['auth_method'] == 'json':
+                    logging.info('Creating Zap plan')
+                    # if Config.custom_zap_plan_present:
+                    #     logging.info('Custom Zap plan is configured %s',Config.zap_plan_config_file_name)   
+                    # else:
+                    Utils.createZapPlan(Config.zap_plan_config,output_file)     
+                    #Utils.createZapPlan(Config.zap_plan_config,output_file)
+                    logging.info('checking session management script configuration')
+
+                    if Config.custom_zap_script_present:
+                        logging.info('Custom Zap script is configured %s',Config.zap_script_config_file_name)     
+                    else:
+                        logging.info('Creating session management script for zap')
+                        Utils.createZapScript(Config.zap_plan_config)
+                          
+                    #return 0
+                else:
+                    Utils.createZapPlan(Config.zap_plan_config,output_file)    
+
+
+               
+
+        else: 
+            logging.info('DAST Auth is not configured')       
+
+            
+
         #command_line = '-h '+Config.dast_target+' -maxtime 10 -o tmp/'+output_file
         #print(command_line_nikto)
         detach = True if data['detach'] == 1 else False
 
         if Config.sast_build_dir == None:
             Config.sast_build_dir = os.getcwd()+'/'
 
         if data['dynamic_comment'] == 1:
+            
             target_url = Config.dast_target
 
             if Config.dast_type == "API":
                 api_type = Config.dast_api_type
                 command_line = "% s" % command_line.format(target_url = target_url, api_type=api_type)
+            elif Config.dast_auth_present == True:
+                # if Config.custom_zap_plan_present:
+                #     Config.zap_plan_config_file_name = Config.zap_plan_config_file_name
+                # else:
+                #     Config.zap_plan_config_file_name = Config.zap_plan_config_file_name+'.yaml'
+                command_line = "% s" % command_line.format(zap_plan_file = 'boman_zap_auth_plan.yaml')     
             else:
                 command_line = "% s" % command_line.format(target_url = target_url)
 
-            #print(command_line)
+            logging.info('Command for zap is : %s',command_line)
 
 
             ## context file appending -- MM
 
    #         if Config.zap_context_configured == 'true':
 
     #            context_file_name = Config.zap_context_file_nmae
@@ -328,15 +391,15 @@
         else:    
 
             logging.info('Preparing %s scan for non-jenkins environment with user %s',tool_name, userid)  
 
             try:
                 Config.build_dir = Config.sast_build_dir
                 container= docker.containers.run(docker_image, command_line, volumes={Config.sast_build_dir: {
-                    'bind': data['bind'], 'mode': 'rw'}},user=userid,detach=detach)
+                   'bind': data['bind'], 'mode': 'rw'}},user=userid,detach=detach)
 
                 #print(output_file,toolname,tool_id,scan_details_id)
                 logging.info('[SUCCESS]: %s Scan Completed',tool_name)
                 Config.dast_scan_status ='Completed'
             except errors.ContainerError as exc:
                 Config.dast_scan_status ='Completed'
                 logging.error('[ERROR]: Error recorded while Scanning %s',tool_name)
@@ -469,26 +532,31 @@
         url = Config.boman_url+"/api/app/upload" 
         # with open(path) as f: 
         #     file_obj = f
         r = requests.post(url,json=values)
         #print(r.status_code)
         if r.status_code == 200:
             logging.info('[COMPLETED]: %s Report uploaded Successfully! Report Name: %s',toolname,filename)
+            logging.info('Removing the result file')
+            os.remove(path)
             return 1
         elif r.status_code == 401 :
             logging.error('Unauthorized Access while uploading the results. Please check the app/customer tokens')
             exit(2)  ## Auth error
         else:
             logging.error('Problem While uploading the results.')
             logging.error('response code is %s',r.status_code)
             return 0
     else:
        logging.error(toolname,' Report cant be uploaded filename: %s',filename)
        return 0 ## need to write a logic here
 
+
+
+   
     return 1
 
 
 
 
 ## function for seceert scan using trufflehog
 def initSecertScan(path,data):
@@ -610,26 +678,50 @@
         content = Auth.authorize()
         logging.info('Nothing configured to be scan.')
         return 0
 
     content = Auth.authorize()
     global scan_token
 
+    if Utils.isGitDirectory(Config.sast_build_dir):
+        logging.info('Git repository is found in the directroy')
+        Config.git_present = True
+        logging.info('Fetching git details')
+        git_data = Utils.getGitDetails() 
+        logging.info(git_data)
+        Config.git_branch =git_data['branch']
+        Config.git_repo =git_data['repo']
+        
+        try:   
+            logging.info('Detecting languages in repository')
+            loc = Utils.getLoc()
+        except Exception as e:
+            logging.error('some error occured while detecing languages: %s',e)
+            loc = 0    
+
+
+
+            
+    else:
+        logging.info('Cant Fetch Git Details, Git repository not found in the directroy %s',Config.sast_build_dir)
+
+
+
     if Config.secret_scan_present == True:
 
         if Utils.isGitDirectory(Config.sast_build_dir):
-            logging.info('Git repository is found in the directroy')
             logging.info('Initizating Secret Scanning')
             for data in Config.secret_scan_response:
                 initSecertScan(Config.sast_build_dir,data=Config.secret_scan_response)
+                
         else:
             logging.info('Git repository not found in the directroy %s',Config.sast_build_dir)
             logging.info('Sikping secret scanning')
     else:
-        logging.warning('Sikping secret scanning, since there is no git found in the directory %s',Config.sast_build_dir)
+        logging.warning('Sikping secret scanning, since it is not configured.')
 
 
     scan_token = Config.scan_token
 
 
     if Config.sast_present is True:
 
@@ -639,33 +731,14 @@
         if Config.sast_lang is None:
             #findLang()
             logging.error('Language Not Defined. Exiting')
             exit(4) ## misconfig error
 
 
 
-        sast_len = len(Config.sast_lang)
-
-        if sast_len > 1: ## if the mentioned languages are more than one
-            logging.info('Detected Languges %s',Config.sast_lang)
-            for lang in Config.sast_lang:
-                try:   
-                    loc = Utils.getLoc(Config.sast_build_dir, lang)
-                except:
-                    loc = 0    
-                #print(loc)
-                logging.info('Running scanner with language: %s',lang)
-
-
-        else:
-            logging.info("Detected Language is : %s",Config.sast_lang)
-            loc =  Utils.getLoc(Config.sast_build_dir, Config.sast_lang[0])
-            Config.app_loc = loc
-            logging.info('Loc found in the %s : %s',Config.sast_build_dir,Config.app_loc)
-
         for data in Config.sast_response:
 
             #data =  json.loads(Config.sast_response)
 
             if data['scan_status'] == 0 :   
                 logging.info('No SAST Configuration found from SaaS')    
                 logging.info('Ignoring SAST Scan')
@@ -729,19 +802,25 @@
 
     exitFunction()
     return 1
 
 def default():
 
     parser.add_argument('-a','--action',default='init',help="Action arugment, you need to pass the value for action (eg: test-saas, test-docker, run , test-yaml, version, check-user)")
-    parser.add_argument('-u','--url',default='https://dashboard.boman.ai/v2/',help="Provide the URL of the boman saas (eg: Prod, On-prem)")
+    parser.add_argument('-u','--url',default='https://dashboard.boman.ai/v2/',help="Provide the URL of the boman saas (eg: On-Prem URL)")
     parser.add_argument('-v','--version',default='show',help="Will show the version of boman-cli tool",action='store_true')
-    parser.add_argument('-fb','--failBuild',default='pass',help="This is for failing the boman scan, pass value 'fail' if you want to fail the build when boman successfully runs the scan")
+    parser.add_argument('-fb','--failBuild',default='pass',help="This is for failing the boman scan based on the severity of the findings, pass -fb high for failing the build when any high issue is found, similarly you can pass medium,low")
     parser.add_argument('-cicd','--cicd',default='other',help="Pass jenkins if the cicd you are using is jenkins (value: jenkins). if your are using non-jenkins cicd you can ignore this option.")
-    #parser.add_argument('-check-docker',help='Check you docker is present in your system is compatable to run the boma n.ai')
+    #parser.add_argument('-check-docker',help='Check you docker is present in your system is compatable to run the boman.ai')
+    parser.add_argument('-config','--config',default='boman.yaml',help="Pass the file name if you have any custom file name for the boman config. eg:boman-prod.yaml")
+    # parser.add_argument('-custom_dast_auth_config','--custom_dast_auth_config',default=False,help="Pass True in the case of custom zap auth scan, this requires , -zap_auth_method , -zap_plan and -zap_session_script (incase of json auth method)")
+    # parser.add_argument('-zap_auth_method','--zap_auth_method',default='form',help="Pass the auth method of DAST(zap) scan, supported method [form, json]. default value is form based")
+    # parser.add_argument('-zap_plan','--zap_custom_plan',default='boman_zap_auth_plan.yaml',help="Pass the file name if you have any custom zap context plan. eg:custom-zap-plan.yaml")
+    parser.add_argument('-zap_session_script','--zap_custom_session_script',default='session_management.js',help="Pass the file name if you have any custom zap session script file name. eg:custom-script.js")
+    # parser.add_argument('-uid','--user_id',default='1000:1000',help="[internal] Pass the custom userid:groupid incase the lingu detec function is failed")
     args = parser.parse_args()
 
     # if len(sys.args) == 1:
     #     # display help message when no args are passed.
     #     print('Welcome to Boman CLI, pass bomancli --help to view the commands args ')
     #     exit(1)
 
@@ -756,54 +835,126 @@
     if args.cicd == 'jenkins':
         ##logging.info('jenkins is choosen')
         Config.jenkins = 'yes'
     else:
         ###logging.info('jenkins is not choosen')
         Config.jenkins = 'no'  
 
+    ## lingu user id set
+    if args.user_id == '1000:1000':
+        ##logging.info('jenkins is choosen')
+        Config.lingu_user = '1000:1000'
+    else:
+        ###logging.info('jenkins is not choosen')
+        Config.lingu_user = args.user_id  
+
+
+    if args.config == 'boman.yaml':
+        ##logging.info('jenkins is choosen')
+        Config.boman_config_file = 'boman.yaml'
+    else:
+        ###logging.info('jenkins is not choosen')
+        Config.boman_config_file = args.config
+
+
+##custom zap auth method
+
+    # if args.zap_auth_method == 'form':
+    #     Config.zap_custom_auth_method = 'form'
+    # elif args.zap_auth_method == 'json':
+    #     Config.zap_custom_auth_method = 'json'
+    # else:
+    #     Config.zap_custom_auth_method = 'form'
+
+
+
+
+## custom script for zap auth scan automation
+    # if args.zap_custom_plan == 'boman_zap_auth_plan.yaml':
+    #     Config.zap_plan_config_file_name = 'boman_zap_auth_plan.yaml'
+    #     #exit(1)
+    # else:
+    #     #logging.info('custom zap contct plan option is choosen')
+    #     #Config.custom_zap_plan_present = True
+    #     Config.zap_plan_config_file_name = args.zap_custom_plan
+    #     #exit(1)
+
+    ## custom script for zap auth scan automation
+    if args.zap_custom_session_script == 'session_management.js':
+        Config.zap_script_config_file_name = 'session_management.js'
+    else:
+        ###logging.info('jenkins is not choosen')
+        Config.custom_zap_script_present = True
+        Config.zap_script_config_file_name = args.zap_custom_session_script
+
+## auth method args validation
+
+    # if args.custom_dast_auth_config == True:
+    #     if Config.zap_custom_auth_method == 'json':
+    #         if Config.custom_zap_plan_present & Config.custom_zap_script_present:
+    #             Config.dast_auth_present == True
+    #             Config.custom_zap_plan_present = True
+    #         else:
+    #             logging.error('Zap auth method "json" needs both plan and session script files')
+    #             exit(4)    
+
+
+    #     if Config.zap_custom_auth_method == 'form':
+    #         if Config.custom_zap_plan_present :
+    #             Config.dast_auth_present == True
+    #             Config.custom_zap_plan_present = True
+    #         else:
+    #             logging.error('Zap auth method "form" needs plan file')
+    #             exit(4)
+    
+
+
+
+
+
 
 ## Action argument
     if args.action == 'init':
         print('Welcome to Boman CLI',Config.version,'pass bomancli --help to view the commands args ')
         exit(0)
     elif args.action =='run':
         logging.info("#################################### -  BOMAN Scanner Initiated - ####################################")
         if main():
             logging.info('################################ BOMAN Scanning Done ################################')
             logging.info('#####################################################################################')
-            Utils.uploadLogs()
             Utils.showSummary()
+            Utils.uploadLogs()
 
            ## checking the failbuild argument
             if args.failBuild == 'fail':
                 total_vuln = Config.high_count + Config.medium_count + Config.low_count + Config.critical_count
                 if total_vuln > 0:
                     exit(-1)
                 else:
                     exit(0)    
 
-            elif args.failBuild == 'only-high':
-                if Config.high_count > 0:
+            elif args.failBuild == 'high':
+                if Config.high_count > 0 or Config.critical_count > 0:
                     exit(-1)
                 else:
                     exit(0)     
 
-            elif args.failBuild == 'only-medium':
-                if Config.medium_count > 0:
+            elif args.failBuild == 'medium':
+                if Config.medium_count > 0 or Config.high_count > 0:
                     exit(-1)
                 else:
                     exit(0)    
 
-            elif args.failBuild == 'only-low':
-                if Config.low_count > 0:
+            elif args.failBuild == 'low':
+                if Config.low_count > 0 or Config.medium_count > 0 or Config.high_count > 0:
                     exit(-1)
                 else:
                     exit(0)  
 
-            elif args.failBuild == 'only-critical':
+            elif args.failBuild == 'critical':
                 if Config.critical_count > 0:
                     exit(-1)
                 else:
                     exit(0)                     
 
 
             else:
@@ -847,12 +998,13 @@
         exit(0)
 
 ## version argument 
     if args.version == 'show':
         print('boman-cli '.Config.version)
 
 
+
 ## starting the cli
 
 
 
 default()
```

### Comparing `boman-cli-1.5/bomancli/utils.py` & `boman-cli-1.6/bomancli/validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,308 +1,202 @@
-
 # from base_logger import logging
 # from Config import Config
-# import loc_finder as loc
-#from datetime import datetime
-
+# import utils as Utils
 
+from bomancli import utils as Utils
 from bomancli.base_logger import logging
 from bomancli.Config import Config
-from bomancli import loc_finder as loc
-
-
-import requests
 
 
-import os 
-import subprocess
+import yaml
 import json
-import xmltodict
- 
- 
-docker = Config.docker_client
+import requests
+import os
 
 
-##fucntion to check the docker image is already present or not
-def checkImageAlreadyExsist(imagename):
-    #print(imagename)
-    try:
-        
-        image_list = docker.images.list()
-        logging.info('Checking the scanner image (%s) locally',imagename)  
-    except Exception as e:
-        logging.error('Docker throwing a error , please check the docker installation')
-        #print(str(e))
-        exit(3) ## docker/system error
-
-    for image in image_list:
-       #print(image.tags)
-        if imagename in image.tags:
-            logging.info('Image is already in the local machine')
-            return True
-    
-    logging.info('Image is not present in the local machine')
-    logging.info('Pulling the required image [%s]',imagename)
+#### read the input from the yaml file -- MM ------------------------------------------------------------
 
-    try:
-        pulled = docker.images.pull(imagename)
-        return 1
-    except:
-        logging.error('Error pulling the image [%s]',imagename)
-        exit(3) ## docker/system error
+def yamlValidation():
 
-            
+    logging.info('Finding boman.yaml file')
 
+    #Config.boman_config_file 
 
-### fucntion to check the git is present or not
-def isGitDirectory(path):
-    try:
-        isdir = os.path.isdir(path+'/.git/') 
-        #print(isdir) 
-        return isdir
-        #return subprocess.call(['git', '-C', path, 'status'], stderr=subprocess.STDOUT, stdout = open(os.devnull, 'w')) == 0
+    try: 
+        with open(Config.boman_config_file, 'r') as file:
+            Config.config_data = yaml.safe_load(file)    
+        logging.info('Config yaml file found')    
     except:
-        return 0
-
-    
-
+        
+        logging.error('No config yaml file found')
+        exit(4) ## validation error 
 
+    logging.info('Prasing and Validating the config yaml file')
+   
 
 
-### fucntion to test SaaS server, whether is up or not:
-def testServer():
-    logging.info('Testing Boman.ai Server')
-    url = Config.boman_url+"/api/app/ping"
     try:
-        x = requests.get(url)  #var ="renga"
-    except requests.ConnectionError as e:
-        print(e)
-        logging.error("Can't connect to the Server, Please check your Internet connection.")
-        exit(1) #server/saas error
-    else:
-        if str(x.content):
-            logging.info("Server is reachable ")
-            return 1
-        else:
-            logging.error("Boman.ai Server is not reachable")	
-            exit(1) ## docker/system error
-
+        Config.config_data['Auth']
+        if Config.config_data['Auth'] != '':
+            Config.app_token = Config.config_data['Auth']['project_token']
+            Config.customer_token =Config.config_data['Auth']['customer_token']
 
 
-### function to check docker is available in the machine or not -- MM
-def testDockerAvailable():
-    logging.info('Checking for docker in the machine')
-    try:
-        
-        if docker.ping():
-           logging.info('Docker is running in the machine. Good to go!')
-        else:
-            logging.error('Unable to connect to docker, Please install docker in your environment')    
-    except Exception as e:
-        logging.error('Docker not found in your machine, Please install docker to continue the scanning')
-        #print(str(e))
-        exit(3) ## docker/system error
+    except KeyError:
 
+        logging.error('Project and Customer token is mandatory to run the scan. Refer the documentation.')    
 
 
-### function to test the dast url is accesible or not --- MM
+    try: 
 
+        if  Config.config_data['SAST'] != '':
+            Config.sast_lang = Config.config_data['SAST']['language'].split(",") ## comma sperated if mulitple
+            
+            Config.sast_present = True
+            Config.sast_message = 'SAST is properly configured'
+            logging.info('SAST is properly configured with %s and ready to scan',Config.sast_lang)
+
+            try:
+                logging.info('choosing the sast working directory')
+                Config.sast_build_dir  = Config.config_data['SAST']['work_dir']
+            except KeyError: 
+                logging.info('work dir not specified in config, choosing the default sast working directory')
+                Config.sast_build_dir = os.getcwd()+'/'
 
-def testDastUrl(url):
-    logging.info('Testing %s target', url)
-    #url = Config.boman_url+"/api/app/ping"
-    #print(url)
-    try:
-        x = requests.get(url)
-    except requests.ConnectionError:
-        logging.error("Can't connect to the %s, Please check your Internet connection.", url)
-        return 0
-    else:
-        logging.info("DAST target is reachable")
-        return 1
-        # if x.status_code == 200:
-           
-        #     return 1
-        # else:
-        #     logging.error("Boman.ai Server is not reachable")	
-        #     exit(3)
+            #logging.info('snyk is choosen, and the env var declared was %s', str('s'))
 
 
+            
 
 
-### fucntion to get the loc in given directory and lang
-
-def getLoc(build_dir,lang):
-
-    lang_extensions = {
-        'nodejs':'.js',
-        'python':'.py',
-        'php':'.php',
-        'ruby':'.rb',
-        'go':'.go',
-        'java':'.java',
-        'python-snyk':'.py',
-        'node-snyk':'.js',
-        'ruby-snyk':'.rb',
-        'csharp':'.cs'
-    }
 
-    #print(lang_extensions['js'])
+        if 'java' in Config.sast_lang:
 
-    logging.info('Counting the lines of code of the given language. Found: %s',build_dir)
-    try:
-        return loc.countlines(build_dir,extentsion=lang_extensions[lang])
-    except:
-        return 0
-
-## this function will mask the middle charecters depending on the lenght of given value and return -- used in trufflehog -- MM
-def masker(n):
-    var1 = str(n)
-    str_length = len(n)
-
-    if str_length > 15:
-        total_unmask_char_len = 8
-        prefix_char_len = 4
-        sufix_char_len = 4
-    elif str_length < 10:
-        total_unmask_char_len = 4
-        prefix_char_len = 2
-        sufix_char_len = 2
-    elif str_length < 5:
-        total_unmask_char_len = 2
-        prefix_char_len = 1
-        sufix_char_len = 1
-    elif str_length < 3:
-        masked = '#' * str_length
-        return masked
-
-    unmasked_len = str_length - total_unmask_char_len
-    masked_value = '#' * unmasked_len
-
-    prefix = var1[:prefix_char_len]
+            try:
+                Config.sast_target =  Config.config_data['SAST']['target']
+            except KeyError: 
+                logging.error('Java requires a target file to be mentioned in the boman.yaml file. refer the documentation')
+                Config.sast_present = False       
+                Config.sast_message = 'SAST is not configured properly, Java requires a target file to be mentioned in the boman.yaml file. refer the documentation'    
+        
 
-    sufix = var1[-sufix_char_len:]
 
-    masked = prefix+masked_value+sufix
-    return masked
+        # if 'python-snyk' in Config.sast_lang:
 
+        #         try:
+        #             Config.sast_env = Config.config_data['SAST']['env']
+        #             logging.info('snyk is choosen, and the env var declared was %s', str(Config.sast_env))
+        #         except KeyError: 
+        #             logging.error('Snyk requires a enviromenet var for snyk auth token to be mentioned in the boman.yaml file. refer the documentation')
+        #             Config.sast_present = False 
 
+        
+    except KeyError:    
+        Config.sast_present = False
+        Config.sast_message = 'SAST was not properly defined in the config, Please check your boman.yaml file.'
+        logging.warning('SAST was not properly defined in the config')
+        logging.warning('Ignoring SAST, Please provide all mandatory inputs incase you like to run SAST scan.')
+        
 
-def convertXmlToJson(file_name,path,output_file):
     
-    # open the input xml file and read
-    # data in form of python dictionary
-    # using xmltodict module
-    target = path+file_name
-    output_target = path+output_file
+    ## DAST
 
-    try:
-        with open(target) as xml_file:
-            
-            data_dict = xmltodict.parse(xml_file.read())
-            xml_file.close()
-            
-            # generate the object using json.dumps()
-            # corresponding to json data
-            
-            json_data = json.dumps(data_dict)
-            
-            # Write the json data to output
-            # json file
-            with open(output_target, "w") as json_file:
-                json_file.write(json_data)
-                json_file.close()
-            return 1
-
-    except Exception as e:
-        return 0
+    try: 
+        Config.dast_target = Config.config_data['DAST']['URL']
+        Config.dast_type = Config.config_data['DAST']['type']
 
+        Config.dast_present = True
 
+        try:        
+            if Config.config_data['DAST']['auth'] == 'yes':
+                Config.dast_auth_present = True
+        except KeyError: 
+            Config.dast_auth_present = False 
 
 
-def logError(msg,error):
-    f = open("bomancli.errors.log", "a")
-    msg = msg+'\n'
-    # writing in the file
-    now = 'ss'
-    f.write('\n===========================================================\n')
-    f.write(str(now))
-    f.write(str(msg))
-    f.write(str(error)) 
-     # closing the file
-    f.close()
+        if Utils.testDastUrl(Config.dast_target):
+            logging.info('DAST is properly configured and ready to scan')
+            
+            if Config.dast_type == 'API':
+                try:  
+                    logging.info('DAST is configured for API scan, checking API type.')    
+                    Config.dast_api_type = Config.config_data['DAST']['api_type']
+                    
+                except KeyError:
+                    logging.info('DAST API type is not given, proceeding with default value: OPENAPI')
+                    Config.dast_api_type = 'openapi'  
+
+
+        else:    
+            logging.info('DAST target is not reachable, ignoring DAST scan')
+            Config.dast_present = False
+            Config.dast_message = 'DAST target is not reachable. DAST scan was ignored'
+                
+    except KeyError:    
+        Config.dast_present = False
+        Config.dast_message = 'DAST was not properly defined in the config.'
+        logging.warning('DAST was not properly defined in the config.')
+        logging.warning('Ignoring DAST, Please provide all mandatory inputs incase you like to run DAST scan.')
+        
 
+        
+               
 
 
-## summary function
-
-def showSummary():
-    logging.info('---------------------------------------------------------------------------------------------------------------')
-    logging.info('--------------------------  SUMMARY FOR SCAN: %s  -----------------------------------------------',Config.scan_name,)
-    logging.info('--------------------------- Scan Token: %s --------------------------------------------------------',Config.scan_token)
-    logging.info('---------------------------------------------------------------------------------------------------------------')
-    logging.info('----------------------------------------')
-    logging.info('-------- Vulnerabilities Found ---------')
-    logging.info('HIGH : %s | MEDIUM : %s | LOW : %s ', Config.high_count, Config.medium_count, Config.low_count)
-    logging.info('----------------------------------------')
-    logging.info('----------------------------------------')
-    logging.info('-------- SAST STATUS ---------')
-    if Config.sast_present == True:
-        logging.info('SCAN STATUS: %s',Config.sast_scan_status)
-        logging.info('UPLOAD STATUS: %s',Config.sast_upload_status)
-        logging.info('SCAN MESSAGE : %s', Config.sast_message)
-
-        logging.info('ERRORS: %s',Config.sast_errors)
-    else:
-        logging.info('SCAN MESSAGE : %s', Config.sast_message)   
-    logging.info('----------------------------------------')
-
-    logging.info('-------- DAST STATUS ---------')
-    if Config.dast_present == True:
-        logging.info('SCAN STATUS: %s',Config.dast_scan_status)
-        logging.info('UPLOAD STATUS: %s',Config.dast_upload_status)
-        logging.info('SCAN MESSAGE : %s', Config.dast_message)
-
-        logging.info('ERRORS: %s',Config.dast_errors)
-    else:
-        logging.info('SCAN MESSAGE : %s', Config.dast_message)    
-    logging.info('--------------------------------------')
+    ## SCA
 
+    try: 
+        if  Config.config_data['SCA'] != '':
+            Config.sca_lang = Config.config_data['SCA']['language'].split(",") ## comma sperated if mulitple
+            
+            Config.sca_present =  True
 
-    
-    logging.info('-------- SCA STATUS ---------')
-    if Config.sca_present == True:
-        logging.info('SCAN STATUS: %s',Config.sca_scan_status)
-        logging.info('UPLOAD STATUS: %s',Config.sca_upload_status)
-        logging.info('SCAN MESSAGE : %s', Config.sca_message)
+            try:
+                Config.sca_build_dir = Config.config_data['SCA']['work_dir']
+            except KeyError: 
+                Config.sca_build_dir = os.getcwd()+'/'
+
+            Config.sca_message ='SCA is properly configured'
+            logging.info('SCA is properly configured and ready to scan')    
+    except KeyError:    
+        Config.sca_present =  False
+        Config.sca_message ='SCA was not properly defined in the config'
+        logging.warning('SCA was not properly defined in the config')
+        logging.warning('Ignoring SCA, Please provide all mandatory inputs incase you like to run SCA scan.')
         
-        logging.info('ERRORS: %s',Config.sca_errors)
-    else:
-        logging.info('SCAN MESSAGE : %s', Config.sca_message)     
-    logging.info('--------------------------------------')
-
+#ss
+    try:
+        if Config.config_data['Secret_Scan'] == False:
+            Config.secret_scan_present = False
+        else:   
+            try:
+                Config.sast_build_dir  = Config.config_data['SAST']['work_dir']
+            except KeyError: 
+                Config.sast_build_dir = os.getcwd()+'/'
+                 
+            try:
+                Config.secret_scan_present =  True if Utils.isGitDirectory(Config.sast_build_dir) else False
+
+                if Config.secret_scan_present:
+                    logging.info('Secret scanning is properly configured and ready to scan')
+                    Config.secret_scan_message ='Secret scanning is properly configured and ready to scan'
+                else:
+                    logging.warning('Secret scanning is properly configured, but working directory is not a git repository.') 
+                    logging.warning('Ignoring Secret scanning.')    
+                    Config.secret_scan_message ='Secret scanning is properly configured, but working directory is not a git repository.'       
+            except KeyError:
+                Config.secret_scan_present = False
+                logging.warning('Secret scanning is not properly configured, Working directory is not git.') 
+                Config.secret_scan_message ='Secret scanning is not properly configured'     
+    except KeyError:
+        Config.secret_scan_present = False  
+        logging.warning('Secret scanning is not properly configured. Cant read the Secret_Scan configuration.')   
+        Config.secret_scan_message ='Secret scanning is not properly configured'  
 
 
-    logging.info('-------- SECRET SCAN STATUS --------- ')
-    if Config.secret_scan_present:
-        logging.info('SCAN STATUS: %s',Config.secret_scan_status)
-        logging.info('UPLOAD STATUS: %s',Config.secret_scan_upload_status)
-        logging.info('SCAN MESSAGE : %s', Config.secret_scan_message)
         
-        logging.info('ERRORS: %s',Config.secret_scan_errors)
-    else:
-        logging.info('SCAN MESSAGE : %s', Config.secret_scan_message)   
-    logging.info('-------------------------------------')
-
-
-
-
-    # logging.info(Config.sast_message)
-    # logging.info(Config.dast_message)
-    # logging.info(Config.sca_message)
-    # logging.info(Config.secret_scan_message)
-
 
+    
 
-def uploadLogs():
-    logging.info('Uploading logs for the scan token %s',str(Config.scan_token))
-    return 1
+## need to use lingudetect here, but the results are not trustable and misleading ------ MM -------------------
+def findLang():
+    print('[INFO]: Detecting Language')
```

### Comparing `boman-cli-1.5/setup.py` & `boman-cli-1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 import configparser
+from bomancli.Config import Config
 
 config = configparser.ConfigParser()
 config.read('setup.cfg')
 environment = config['metadata']['environment']
 version = config['metadata']['version']
 name = config['metadata']['name']
-
-
+base_url = config['metadata']['saas_base_url']
+Config.boman_base_url = base_url
 
 try:
     import pypandoc
     long_description = pypandoc.convert_file('README.md', 'rst')
 except(IOError, ImportError):
     long_description = open('README.md').read()
 
@@ -39,16 +40,17 @@
     description='CLI tool of boman.ai',
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='https://boman.ai',
     author='Sumeru Software Solutions Pvt. Ltd.',
     author_email='support@boman.ai',
     license='BSD 2-clause',
-    packages=['bomancli'],
     entry_points = entry_points,
+    packages=['bomancli'],
+    package_data={'bomancli': ['templates/template_plan.yaml']},
     install_requires=['docker',
                       'requests',
                       'pyyaml',
                       'coloredlogs','xmltodict'                     
                       ],
 
     classifiers=[
```

