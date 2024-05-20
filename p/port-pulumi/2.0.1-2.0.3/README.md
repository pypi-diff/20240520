# Comparing `tmp/port_pulumi-2.0.1.tar.gz` & `tmp/port_pulumi-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-2.0.1.tar", last modified: Mon May 13 06:36:54 2024, max compression
+gzip compressed data, was "port_pulumi-2.0.3.tar", last modified: Mon May 20 13:05:21 2024, max compression
```

## Comparing `port_pulumi-2.0.1.tar` & `port_pulumi-2.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   196235 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    43486 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30278 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/aggregation_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/aggregation_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    36508 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/blueprint_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    22571 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)   167091 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26699 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/page_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/scorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 06:36:54.550242 port_pulumi-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-13 06:36:54.000000 port_pulumi-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:05:21.719229 port_pulumi-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-20 13:05:21.719229 port_pulumi-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:05:21.719229 port_pulumi-2.0.3/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198369 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43486 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30278 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/aggregation_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/aggregation_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36508 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/blueprint_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:05:21.719229 port_pulumi-2.0.3/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22571 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169225 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26699 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/page_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/scorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:05:21.719229 port_pulumi-2.0.3/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:05:21.719229 port_pulumi-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-20 13:05:21.000000 port_pulumi-2.0.3/setup.py
```

### Comparing `port_pulumi-2.0.1/PKG-INFO` & `port_pulumi-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port_pulumi
-Version: 2.0.1
+Version: 2.0.3
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `port_pulumi-2.0.1/README.md` & `port_pulumi-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/__init__.py` & `port_pulumi-2.0.3/port_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/_inputs.py` & `port_pulumi-2.0.3/port_pulumi/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     def __init__(__self__, *,
                  org: pulumi.Input[str],
                  webhook: pulumi.Input[str],
                  payload: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] org: Required when selecting type AZURE. The Azure org that the workflow belongs to
         :param pulumi.Input[str] webhook: Required when selecting type AZURE. The Azure webhook that the workflow belongs to
-        :param pulumi.Input[str] payload: The Azure Devops workflow payload (array or object encoded to a string)
+        :param pulumi.Input[str] payload: The Azure Devops workflow payload to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         pulumi.set(__self__, "org", org)
         pulumi.set(__self__, "webhook", webhook)
         if payload is not None:
             pulumi.set(__self__, "payload", payload)
 
     @property
@@ -162,15 +162,15 @@
     def webhook(self, value: pulumi.Input[str]):
         pulumi.set(self, "webhook", value)
 
     @property
     @pulumi.getter
     def payload(self) -> Optional[pulumi.Input[str]]:
         """
-        The Azure Devops workflow payload (array or object encoded to a string)
+        The Azure Devops workflow payload to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "payload")
 
     @payload.setter
     def payload(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "payload", value)
 
@@ -184,15 +184,15 @@
                  report_workflow_status: Optional[pulumi.Input[str]] = None,
                  workflow_inputs: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] org: Required when selecting type GITHUB. The GitHub org that the workflow belongs to
         :param pulumi.Input[str] repo: Required when selecting type GITHUB. The GitHub repo that the workflow belongs to
         :param pulumi.Input[str] workflow: The GitHub workflow that the action belongs to
         :param pulumi.Input[str] report_workflow_status: Report the workflow status when invoking the action
-        :param pulumi.Input[str] workflow_inputs: The GitHub workflow inputs (key-value object encoded to a string)
+        :param pulumi.Input[str] workflow_inputs: The GitHub workflow inputs to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         pulumi.set(__self__, "org", org)
         pulumi.set(__self__, "repo", repo)
         pulumi.set(__self__, "workflow", workflow)
         if report_workflow_status is not None:
             pulumi.set(__self__, "report_workflow_status", report_workflow_status)
         if workflow_inputs is not None:
@@ -246,15 +246,15 @@
     def report_workflow_status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "report_workflow_status", value)
 
     @property
     @pulumi.getter(name="workflowInputs")
     def workflow_inputs(self) -> Optional[pulumi.Input[str]]:
         """
-        The GitHub workflow inputs (key-value object encoded to a string)
+        The GitHub workflow inputs to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "workflow_inputs")
 
     @workflow_inputs.setter
     def workflow_inputs(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "workflow_inputs", value)
 
@@ -266,15 +266,15 @@
                  project_name: pulumi.Input[str],
                  default_ref: Optional[pulumi.Input[str]] = None,
                  pipeline_variables: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] group_name: Required when selecting type GITLAB. The GitLab group name that the workflow belongs to
         :param pulumi.Input[str] project_name: Required when selecting type GITLAB. The GitLab project name that the workflow belongs to
         :param pulumi.Input[str] default_ref: The default ref of the action
-        :param pulumi.Input[str] pipeline_variables: The Gitlab pipeline variables (key-value object encoded to a string)
+        :param pulumi.Input[str] pipeline_variables: The Gitlab pipeline variables should be in `JSON` format, encoded as a string. Use jsonencode to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         pulumi.set(__self__, "group_name", group_name)
         pulumi.set(__self__, "project_name", project_name)
         if default_ref is not None:
             pulumi.set(__self__, "default_ref", default_ref)
         if pipeline_variables is not None:
             pulumi.set(__self__, "pipeline_variables", pipeline_variables)
@@ -315,38 +315,38 @@
     def default_ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_ref", value)
 
     @property
     @pulumi.getter(name="pipelineVariables")
     def pipeline_variables(self) -> Optional[pulumi.Input[str]]:
         """
-        The Gitlab pipeline variables (key-value object encoded to a string)
+        The Gitlab pipeline variables should be in `JSON` format, encoded as a string. Use jsonencode to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "pipeline_variables")
 
     @pipeline_variables.setter
     def pipeline_variables(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pipeline_variables", value)
 
 
 @pulumi.input_type
 class ActionKafkaMethodArgs:
     def __init__(__self__, *,
                  payload: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] payload: The Kafka message payload (array or object encoded to a string)
+        :param pulumi.Input[str] payload: The Kafka message payload to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         if payload is not None:
             pulumi.set(__self__, "payload", payload)
 
     @property
     @pulumi.getter
     def payload(self) -> Optional[pulumi.Input[str]]:
         """
-        The Kafka message payload (array or object encoded to a string)
+        The Kafka message payload to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "payload")
 
     @payload.setter
     def payload(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "payload", value)
 
@@ -2112,16 +2112,16 @@
                  body: Optional[pulumi.Input[str]] = None,
                  headers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  method: Optional[pulumi.Input[str]] = None,
                  synchronized: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] url: Required when selecting type WEBHOOK. The URL to invoke the action
         :param pulumi.Input[str] agent: Use the agent to invoke the action
-        :param pulumi.Input[str] body: The Webhook body (array or object encoded to a string)
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] headers: The HTTP method to invoke the action
+        :param pulumi.Input[str] body: The Webhook body should be in `JSON` format, encoded as a string. Use jsonencode to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] headers: The HTTP headers for invoking the action. They should be encoded as a key-value object to a string using jsonencode. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         :param pulumi.Input[str] method: The HTTP method to invoke the action
         :param pulumi.Input[str] synchronized: Synchronize the action
         """
         pulumi.set(__self__, "url", url)
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
         if body is not None:
@@ -2157,27 +2157,27 @@
     def agent(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "agent", value)
 
     @property
     @pulumi.getter
     def body(self) -> Optional[pulumi.Input[str]]:
         """
-        The Webhook body (array or object encoded to a string)
+        The Webhook body should be in `JSON` format, encoded as a string. Use jsonencode to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "body")
 
     @body.setter
     def body(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "body", value)
 
     @property
     @pulumi.getter
     def headers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        The HTTP method to invoke the action
+        The HTTP headers for invoking the action. They should be encoded as a key-value object to a string using jsonencode. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "headers")
 
     @headers.setter
     def headers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "headers", value)
 
@@ -2689,58 +2689,58 @@
                  register: pulumi.Input['BlueprintPermissionsEntitiesRegisterArgs'],
                  unregister: pulumi.Input['BlueprintPermissionsEntitiesUnregisterArgs'],
                  update: pulumi.Input['BlueprintPermissionsEntitiesUpdateArgs'],
                  update_metadata_properties: pulumi.Input['BlueprintPermissionsEntitiesUpdateMetadataPropertiesArgs'],
                  update_properties: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdatePropertiesArgs']]]] = None,
                  update_relations: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdateRelationsArgs']]]] = None):
         """
-        :param pulumi.Input['BlueprintPermissionsEntitiesRegisterArgs'] register: Enable permissions to register entities of the blueprint
-        :param pulumi.Input['BlueprintPermissionsEntitiesUnregisterArgs'] unregister: Enable permissions to unregister entities of the blueprint
-        :param pulumi.Input['BlueprintPermissionsEntitiesUpdateArgs'] update: Enable permissions to update entities of the blueprint
-        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdatePropertiesArgs']]] update_properties: Enable permissions to update the entity properties
-        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdateRelationsArgs']]] update_relations: Enable permissions to update the entity relations
+        :param pulumi.Input['BlueprintPermissionsEntitiesRegisterArgs'] register: Manage permissions to register entities of the blueprint
+        :param pulumi.Input['BlueprintPermissionsEntitiesUnregisterArgs'] unregister: Manage permissions to unregister entities of the blueprint
+        :param pulumi.Input['BlueprintPermissionsEntitiesUpdateArgs'] update: Manage permissions to update entities of the blueprint
+        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdatePropertiesArgs']]] update_properties: Manage permissions to update the entity properties
+        :param pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdateRelationsArgs']]] update_relations: Manage permissions to update the entity relations
         """
         pulumi.set(__self__, "register", register)
         pulumi.set(__self__, "unregister", unregister)
         pulumi.set(__self__, "update", update)
         pulumi.set(__self__, "update_metadata_properties", update_metadata_properties)
         if update_properties is not None:
             pulumi.set(__self__, "update_properties", update_properties)
         if update_relations is not None:
             pulumi.set(__self__, "update_relations", update_relations)
 
     @property
     @pulumi.getter
     def register(self) -> pulumi.Input['BlueprintPermissionsEntitiesRegisterArgs']:
         """
-        Enable permissions to register entities of the blueprint
+        Manage permissions to register entities of the blueprint
         """
         return pulumi.get(self, "register")
 
     @register.setter
     def register(self, value: pulumi.Input['BlueprintPermissionsEntitiesRegisterArgs']):
         pulumi.set(self, "register", value)
 
     @property
     @pulumi.getter
     def unregister(self) -> pulumi.Input['BlueprintPermissionsEntitiesUnregisterArgs']:
         """
-        Enable permissions to unregister entities of the blueprint
+        Manage permissions to unregister entities of the blueprint
         """
         return pulumi.get(self, "unregister")
 
     @unregister.setter
     def unregister(self, value: pulumi.Input['BlueprintPermissionsEntitiesUnregisterArgs']):
         pulumi.set(self, "unregister", value)
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Input['BlueprintPermissionsEntitiesUpdateArgs']:
         """
-        Enable permissions to update entities of the blueprint
+        Manage permissions to update entities of the blueprint
         """
         return pulumi.get(self, "update")
 
     @update.setter
     def update(self, value: pulumi.Input['BlueprintPermissionsEntitiesUpdateArgs']):
         pulumi.set(self, "update", value)
 
@@ -2753,27 +2753,27 @@
     def update_metadata_properties(self, value: pulumi.Input['BlueprintPermissionsEntitiesUpdateMetadataPropertiesArgs']):
         pulumi.set(self, "update_metadata_properties", value)
 
     @property
     @pulumi.getter(name="updateProperties")
     def update_properties(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdatePropertiesArgs']]]]:
         """
-        Enable permissions to update the entity properties
+        Manage permissions to update the entity properties
         """
         return pulumi.get(self, "update_properties")
 
     @update_properties.setter
     def update_properties(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdatePropertiesArgs']]]]):
         pulumi.set(self, "update_properties", value)
 
     @property
     @pulumi.getter(name="updateRelations")
     def update_relations(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdateRelationsArgs']]]]:
         """
-        Enable permissions to update the entity relations
+        Manage permissions to update the entity relations
         """
         return pulumi.get(self, "update_relations")
 
     @update_relations.setter
     def update_relations(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input['BlueprintPermissionsEntitiesUpdateRelationsArgs']]]]):
         pulumi.set(self, "update_relations", value)
 
@@ -3063,17 +3063,17 @@
     def __init__(__self__, *,
                  owned_by_team: Optional[pulumi.Input[bool]] = None,
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  users: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[bool] owned_by_team: Owned by team
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles with update $icon metadata permissions
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: Teams with update $icon metadata permissions
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] users: Users with update $icon metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles with update `$icon` metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: Teams with update `$icon` metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users: Users with update `$icon` metadata permissions
         """
         if owned_by_team is not None:
             pulumi.set(__self__, "owned_by_team", owned_by_team)
         if roles is not None:
             pulumi.set(__self__, "roles", roles)
         if teams is not None:
             pulumi.set(__self__, "teams", teams)
@@ -3092,39 +3092,39 @@
     def owned_by_team(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "owned_by_team", value)
 
     @property
     @pulumi.getter
     def roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Roles with update $icon metadata permissions
+        Roles with update `$icon` metadata permissions
         """
         return pulumi.get(self, "roles")
 
     @roles.setter
     def roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "roles", value)
 
     @property
     @pulumi.getter
     def teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Teams with update $icon metadata permissions
+        Teams with update `$icon` metadata permissions
         """
         return pulumi.get(self, "teams")
 
     @teams.setter
     def teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "teams", value)
 
     @property
     @pulumi.getter
     def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Users with update $icon metadata permissions
+        Users with update `$icon` metadata permissions
         """
         return pulumi.get(self, "users")
 
     @users.setter
     def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "users", value)
 
@@ -3134,17 +3134,17 @@
     def __init__(__self__, *,
                  owned_by_team: Optional[pulumi.Input[bool]] = None,
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  users: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[bool] owned_by_team: Owned by team
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles with update $identifier metadata permissions
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: Teams with update $identifier metadata permissions
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] users: Users with update $identifier metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles with update `$identifier` metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: Teams with update `$identifier` metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users: Users with update `$identifier` metadata permissions
         """
         if owned_by_team is not None:
             pulumi.set(__self__, "owned_by_team", owned_by_team)
         if roles is not None:
             pulumi.set(__self__, "roles", roles)
         if teams is not None:
             pulumi.set(__self__, "teams", teams)
@@ -3163,39 +3163,39 @@
     def owned_by_team(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "owned_by_team", value)
 
     @property
     @pulumi.getter
     def roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Roles with update $identifier metadata permissions
+        Roles with update `$identifier` metadata permissions
         """
         return pulumi.get(self, "roles")
 
     @roles.setter
     def roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "roles", value)
 
     @property
     @pulumi.getter
     def teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Teams with update $identifier metadata permissions
+        Teams with update `$identifier` metadata permissions
         """
         return pulumi.get(self, "teams")
 
     @teams.setter
     def teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "teams", value)
 
     @property
     @pulumi.getter
     def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Users with update $identifier metadata permissions
+        Users with update `$identifier` metadata permissions
         """
         return pulumi.get(self, "users")
 
     @users.setter
     def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "users", value)
 
@@ -3205,17 +3205,17 @@
     def __init__(__self__, *,
                  owned_by_team: Optional[pulumi.Input[bool]] = None,
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  users: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[bool] owned_by_team: Owned by team
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles with update $team metadata permissions
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: Teams with update $team metadata permissions
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] users: Users with update $team metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles with update `$team` metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: Teams with update `$team` metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users: Users with update `$team` metadata permissions
         """
         if owned_by_team is not None:
             pulumi.set(__self__, "owned_by_team", owned_by_team)
         if roles is not None:
             pulumi.set(__self__, "roles", roles)
         if teams is not None:
             pulumi.set(__self__, "teams", teams)
@@ -3234,39 +3234,39 @@
     def owned_by_team(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "owned_by_team", value)
 
     @property
     @pulumi.getter
     def roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Roles with update $team metadata permissions
+        Roles with update `$team` metadata permissions
         """
         return pulumi.get(self, "roles")
 
     @roles.setter
     def roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "roles", value)
 
     @property
     @pulumi.getter
     def teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Teams with update $team metadata permissions
+        Teams with update `$team` metadata permissions
         """
         return pulumi.get(self, "teams")
 
     @teams.setter
     def teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "teams", value)
 
     @property
     @pulumi.getter
     def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Users with update $team metadata permissions
+        Users with update `$team` metadata permissions
         """
         return pulumi.get(self, "users")
 
     @users.setter
     def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "users", value)
 
@@ -3276,17 +3276,17 @@
     def __init__(__self__, *,
                  owned_by_team: Optional[pulumi.Input[bool]] = None,
                  roles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  users: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[bool] owned_by_team: Owned by team
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles with update $title metadata permissions
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: Teams with update $title metadata permissions
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] users: Users with update $title metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Roles with update `$title` metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] teams: Teams with update `$title` metadata permissions
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] users: Users with update `$title` metadata permissions
         """
         if owned_by_team is not None:
             pulumi.set(__self__, "owned_by_team", owned_by_team)
         if roles is not None:
             pulumi.set(__self__, "roles", roles)
         if teams is not None:
             pulumi.set(__self__, "teams", teams)
@@ -3305,39 +3305,39 @@
     def owned_by_team(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "owned_by_team", value)
 
     @property
     @pulumi.getter
     def roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Roles with update $title metadata permissions
+        Roles with update `$title` metadata permissions
         """
         return pulumi.get(self, "roles")
 
     @roles.setter
     def roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "roles", value)
 
     @property
     @pulumi.getter
     def teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Teams with update $title metadata permissions
+        Teams with update `$title` metadata permissions
         """
         return pulumi.get(self, "teams")
 
     @teams.setter
     def teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "teams", value)
 
     @property
     @pulumi.getter
     def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Users with update $title metadata permissions
+        Users with update `$title` metadata permissions
         """
         return pulumi.get(self, "users")
 
     @users.setter
     def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "users", value)
```

### Comparing `port_pulumi-2.0.1/port_pulumi/_utilities.py` & `port_pulumi-2.0.3/port_pulumi/_utilities.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/action.py` & `port_pulumi-2.0.3/port_pulumi/action.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/action_permissions.py` & `port_pulumi-2.0.3/port_pulumi/action_permissions.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/aggregation_properties.py` & `port_pulumi-2.0.3/port_pulumi/aggregation_properties.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/aggregation_property.py` & `port_pulumi-2.0.3/port_pulumi/aggregation_property.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/blueprint.py` & `port_pulumi-2.0.3/port_pulumi/blueprint.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/blueprint_permissions.py` & `port_pulumi-2.0.3/port_pulumi/blueprint_permissions.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/config/vars.py` & `port_pulumi-2.0.3/port_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/entity.py` & `port_pulumi-2.0.3/port_pulumi/entity.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/outputs.py` & `port_pulumi-2.0.3/port_pulumi/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     def __init__(__self__, *,
                  org: str,
                  webhook: str,
                  payload: Optional[str] = None):
         """
         :param str org: Required when selecting type AZURE. The Azure org that the workflow belongs to
         :param str webhook: Required when selecting type AZURE. The Azure webhook that the workflow belongs to
-        :param str payload: The Azure Devops workflow payload (array or object encoded to a string)
+        :param str payload: The Azure Devops workflow payload to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         pulumi.set(__self__, "org", org)
         pulumi.set(__self__, "webhook", webhook)
         if payload is not None:
             pulumi.set(__self__, "payload", payload)
 
     @property
@@ -147,15 +147,15 @@
         """
         return pulumi.get(self, "webhook")
 
     @property
     @pulumi.getter
     def payload(self) -> Optional[str]:
         """
-        The Azure Devops workflow payload (array or object encoded to a string)
+        The Azure Devops workflow payload to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "payload")
 
 
 @pulumi.output_type
 class ActionGithubMethod(dict):
     @staticmethod
@@ -184,15 +184,15 @@
                  report_workflow_status: Optional[str] = None,
                  workflow_inputs: Optional[str] = None):
         """
         :param str org: Required when selecting type GITHUB. The GitHub org that the workflow belongs to
         :param str repo: Required when selecting type GITHUB. The GitHub repo that the workflow belongs to
         :param str workflow: The GitHub workflow that the action belongs to
         :param str report_workflow_status: Report the workflow status when invoking the action
-        :param str workflow_inputs: The GitHub workflow inputs (key-value object encoded to a string)
+        :param str workflow_inputs: The GitHub workflow inputs to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         pulumi.set(__self__, "org", org)
         pulumi.set(__self__, "repo", repo)
         pulumi.set(__self__, "workflow", workflow)
         if report_workflow_status is not None:
             pulumi.set(__self__, "report_workflow_status", report_workflow_status)
         if workflow_inputs is not None:
@@ -230,15 +230,15 @@
         """
         return pulumi.get(self, "report_workflow_status")
 
     @property
     @pulumi.getter(name="workflowInputs")
     def workflow_inputs(self) -> Optional[str]:
         """
-        The GitHub workflow inputs (key-value object encoded to a string)
+        The GitHub workflow inputs to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "workflow_inputs")
 
 
 @pulumi.output_type
 class ActionGitlabMethod(dict):
     @staticmethod
@@ -269,15 +269,15 @@
                  project_name: str,
                  default_ref: Optional[str] = None,
                  pipeline_variables: Optional[str] = None):
         """
         :param str group_name: Required when selecting type GITLAB. The GitLab group name that the workflow belongs to
         :param str project_name: Required when selecting type GITLAB. The GitLab project name that the workflow belongs to
         :param str default_ref: The default ref of the action
-        :param str pipeline_variables: The Gitlab pipeline variables (key-value object encoded to a string)
+        :param str pipeline_variables: The Gitlab pipeline variables should be in `JSON` format, encoded as a string. Use jsonencode to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         pulumi.set(__self__, "group_name", group_name)
         pulumi.set(__self__, "project_name", project_name)
         if default_ref is not None:
             pulumi.set(__self__, "default_ref", default_ref)
         if pipeline_variables is not None:
             pulumi.set(__self__, "pipeline_variables", pipeline_variables)
@@ -306,34 +306,34 @@
         """
         return pulumi.get(self, "default_ref")
 
     @property
     @pulumi.getter(name="pipelineVariables")
     def pipeline_variables(self) -> Optional[str]:
         """
-        The Gitlab pipeline variables (key-value object encoded to a string)
+        The Gitlab pipeline variables should be in `JSON` format, encoded as a string. Use jsonencode to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "pipeline_variables")
 
 
 @pulumi.output_type
 class ActionKafkaMethod(dict):
     def __init__(__self__, *,
                  payload: Optional[str] = None):
         """
-        :param str payload: The Kafka message payload (array or object encoded to a string)
+        :param str payload: The Kafka message payload to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         if payload is not None:
             pulumi.set(__self__, "payload", payload)
 
     @property
     @pulumi.getter
     def payload(self) -> Optional[str]:
         """
-        The Kafka message payload (array or object encoded to a string)
+        The Kafka message payload to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "payload")
 
 
 @pulumi.output_type
 class ActionPermissionsPermissions(dict):
     def __init__(__self__, *,
@@ -1924,16 +1924,16 @@
                  body: Optional[str] = None,
                  headers: Optional[Mapping[str, str]] = None,
                  method: Optional[str] = None,
                  synchronized: Optional[str] = None):
         """
         :param str url: Required when selecting type WEBHOOK. The URL to invoke the action
         :param str agent: Use the agent to invoke the action
-        :param str body: The Webhook body (array or object encoded to a string)
-        :param Mapping[str, str] headers: The HTTP method to invoke the action
+        :param str body: The Webhook body should be in `JSON` format, encoded as a string. Use jsonencode to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
+        :param Mapping[str, str] headers: The HTTP headers for invoking the action. They should be encoded as a key-value object to a string using jsonencode. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         :param str method: The HTTP method to invoke the action
         :param str synchronized: Synchronize the action
         """
         pulumi.set(__self__, "url", url)
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
         if body is not None:
@@ -1961,23 +1961,23 @@
         """
         return pulumi.get(self, "agent")
 
     @property
     @pulumi.getter
     def body(self) -> Optional[str]:
         """
-        The Webhook body (array or object encoded to a string)
+        The Webhook body should be in `JSON` format, encoded as a string. Use jsonencode to encode arrays or objects. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "body")
 
     @property
     @pulumi.getter
     def headers(self) -> Optional[Mapping[str, str]]:
         """
-        The HTTP method to invoke the action
+        The HTTP headers for invoking the action. They should be encoded as a key-value object to a string using jsonencode. Learn about how to [define the action payload](https://docs.getport.io/create-self-service-experiences/setup-backend/#define-the-actions-payload).
         """
         return pulumi.get(self, "headers")
 
     @property
     @pulumi.getter
     def method(self) -> Optional[str]:
         """
@@ -2468,71 +2468,71 @@
                  register: 'outputs.BlueprintPermissionsEntitiesRegister',
                  unregister: 'outputs.BlueprintPermissionsEntitiesUnregister',
                  update: 'outputs.BlueprintPermissionsEntitiesUpdate',
                  update_metadata_properties: 'outputs.BlueprintPermissionsEntitiesUpdateMetadataProperties',
                  update_properties: Optional[Mapping[str, 'outputs.BlueprintPermissionsEntitiesUpdateProperties']] = None,
                  update_relations: Optional[Mapping[str, 'outputs.BlueprintPermissionsEntitiesUpdateRelations']] = None):
         """
-        :param 'BlueprintPermissionsEntitiesRegisterArgs' register: Enable permissions to register entities of the blueprint
-        :param 'BlueprintPermissionsEntitiesUnregisterArgs' unregister: Enable permissions to unregister entities of the blueprint
-        :param 'BlueprintPermissionsEntitiesUpdateArgs' update: Enable permissions to update entities of the blueprint
-        :param Mapping[str, 'BlueprintPermissionsEntitiesUpdatePropertiesArgs'] update_properties: Enable permissions to update the entity properties
-        :param Mapping[str, 'BlueprintPermissionsEntitiesUpdateRelationsArgs'] update_relations: Enable permissions to update the entity relations
+        :param 'BlueprintPermissionsEntitiesRegisterArgs' register: Manage permissions to register entities of the blueprint
+        :param 'BlueprintPermissionsEntitiesUnregisterArgs' unregister: Manage permissions to unregister entities of the blueprint
+        :param 'BlueprintPermissionsEntitiesUpdateArgs' update: Manage permissions to update entities of the blueprint
+        :param Mapping[str, 'BlueprintPermissionsEntitiesUpdatePropertiesArgs'] update_properties: Manage permissions to update the entity properties
+        :param Mapping[str, 'BlueprintPermissionsEntitiesUpdateRelationsArgs'] update_relations: Manage permissions to update the entity relations
         """
         pulumi.set(__self__, "register", register)
         pulumi.set(__self__, "unregister", unregister)
         pulumi.set(__self__, "update", update)
         pulumi.set(__self__, "update_metadata_properties", update_metadata_properties)
         if update_properties is not None:
             pulumi.set(__self__, "update_properties", update_properties)
         if update_relations is not None:
             pulumi.set(__self__, "update_relations", update_relations)
 
     @property
     @pulumi.getter
     def register(self) -> 'outputs.BlueprintPermissionsEntitiesRegister':
         """
-        Enable permissions to register entities of the blueprint
+        Manage permissions to register entities of the blueprint
         """
         return pulumi.get(self, "register")
 
     @property
     @pulumi.getter
     def unregister(self) -> 'outputs.BlueprintPermissionsEntitiesUnregister':
         """
-        Enable permissions to unregister entities of the blueprint
+        Manage permissions to unregister entities of the blueprint
         """
         return pulumi.get(self, "unregister")
 
     @property
     @pulumi.getter
     def update(self) -> 'outputs.BlueprintPermissionsEntitiesUpdate':
         """
-        Enable permissions to update entities of the blueprint
+        Manage permissions to update entities of the blueprint
         """
         return pulumi.get(self, "update")
 
     @property
     @pulumi.getter(name="updateMetadataProperties")
     def update_metadata_properties(self) -> 'outputs.BlueprintPermissionsEntitiesUpdateMetadataProperties':
         return pulumi.get(self, "update_metadata_properties")
 
     @property
     @pulumi.getter(name="updateProperties")
     def update_properties(self) -> Optional[Mapping[str, 'outputs.BlueprintPermissionsEntitiesUpdateProperties']]:
         """
-        Enable permissions to update the entity properties
+        Manage permissions to update the entity properties
         """
         return pulumi.get(self, "update_properties")
 
     @property
     @pulumi.getter(name="updateRelations")
     def update_relations(self) -> Optional[Mapping[str, 'outputs.BlueprintPermissionsEntitiesUpdateRelations']]:
         """
-        Enable permissions to update the entity relations
+        Manage permissions to update the entity relations
         """
         return pulumi.get(self, "update_relations")
 
 
 @pulumi.output_type
 class BlueprintPermissionsEntitiesRegister(dict):
     @staticmethod
@@ -2822,17 +2822,17 @@
     def __init__(__self__, *,
                  owned_by_team: Optional[bool] = None,
                  roles: Optional[Sequence[str]] = None,
                  teams: Optional[Sequence[str]] = None,
                  users: Optional[Sequence[str]] = None):
         """
         :param bool owned_by_team: Owned by team
-        :param Sequence[str] roles: Roles with update $icon metadata permissions
-        :param Sequence[str] teams: Teams with update $icon metadata permissions
-        :param Sequence[str] users: Users with update $icon metadata permissions
+        :param Sequence[str] roles: Roles with update `$icon` metadata permissions
+        :param Sequence[str] teams: Teams with update `$icon` metadata permissions
+        :param Sequence[str] users: Users with update `$icon` metadata permissions
         """
         if owned_by_team is not None:
             pulumi.set(__self__, "owned_by_team", owned_by_team)
         if roles is not None:
             pulumi.set(__self__, "roles", roles)
         if teams is not None:
             pulumi.set(__self__, "teams", teams)
@@ -2847,31 +2847,31 @@
         """
         return pulumi.get(self, "owned_by_team")
 
     @property
     @pulumi.getter
     def roles(self) -> Optional[Sequence[str]]:
         """
-        Roles with update $icon metadata permissions
+        Roles with update `$icon` metadata permissions
         """
         return pulumi.get(self, "roles")
 
     @property
     @pulumi.getter
     def teams(self) -> Optional[Sequence[str]]:
         """
-        Teams with update $icon metadata permissions
+        Teams with update `$icon` metadata permissions
         """
         return pulumi.get(self, "teams")
 
     @property
     @pulumi.getter
     def users(self) -> Optional[Sequence[str]]:
         """
-        Users with update $icon metadata permissions
+        Users with update `$icon` metadata permissions
         """
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
 class BlueprintPermissionsEntitiesUpdateMetadataPropertiesIdentifier(dict):
     @staticmethod
@@ -2894,17 +2894,17 @@
     def __init__(__self__, *,
                  owned_by_team: Optional[bool] = None,
                  roles: Optional[Sequence[str]] = None,
                  teams: Optional[Sequence[str]] = None,
                  users: Optional[Sequence[str]] = None):
         """
         :param bool owned_by_team: Owned by team
-        :param Sequence[str] roles: Roles with update $identifier metadata permissions
-        :param Sequence[str] teams: Teams with update $identifier metadata permissions
-        :param Sequence[str] users: Users with update $identifier metadata permissions
+        :param Sequence[str] roles: Roles with update `$identifier` metadata permissions
+        :param Sequence[str] teams: Teams with update `$identifier` metadata permissions
+        :param Sequence[str] users: Users with update `$identifier` metadata permissions
         """
         if owned_by_team is not None:
             pulumi.set(__self__, "owned_by_team", owned_by_team)
         if roles is not None:
             pulumi.set(__self__, "roles", roles)
         if teams is not None:
             pulumi.set(__self__, "teams", teams)
@@ -2919,31 +2919,31 @@
         """
         return pulumi.get(self, "owned_by_team")
 
     @property
     @pulumi.getter
     def roles(self) -> Optional[Sequence[str]]:
         """
-        Roles with update $identifier metadata permissions
+        Roles with update `$identifier` metadata permissions
         """
         return pulumi.get(self, "roles")
 
     @property
     @pulumi.getter
     def teams(self) -> Optional[Sequence[str]]:
         """
-        Teams with update $identifier metadata permissions
+        Teams with update `$identifier` metadata permissions
         """
         return pulumi.get(self, "teams")
 
     @property
     @pulumi.getter
     def users(self) -> Optional[Sequence[str]]:
         """
-        Users with update $identifier metadata permissions
+        Users with update `$identifier` metadata permissions
         """
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
 class BlueprintPermissionsEntitiesUpdateMetadataPropertiesTeam(dict):
     @staticmethod
@@ -2966,17 +2966,17 @@
     def __init__(__self__, *,
                  owned_by_team: Optional[bool] = None,
                  roles: Optional[Sequence[str]] = None,
                  teams: Optional[Sequence[str]] = None,
                  users: Optional[Sequence[str]] = None):
         """
         :param bool owned_by_team: Owned by team
-        :param Sequence[str] roles: Roles with update $team metadata permissions
-        :param Sequence[str] teams: Teams with update $team metadata permissions
-        :param Sequence[str] users: Users with update $team metadata permissions
+        :param Sequence[str] roles: Roles with update `$team` metadata permissions
+        :param Sequence[str] teams: Teams with update `$team` metadata permissions
+        :param Sequence[str] users: Users with update `$team` metadata permissions
         """
         if owned_by_team is not None:
             pulumi.set(__self__, "owned_by_team", owned_by_team)
         if roles is not None:
             pulumi.set(__self__, "roles", roles)
         if teams is not None:
             pulumi.set(__self__, "teams", teams)
@@ -2991,31 +2991,31 @@
         """
         return pulumi.get(self, "owned_by_team")
 
     @property
     @pulumi.getter
     def roles(self) -> Optional[Sequence[str]]:
         """
-        Roles with update $team metadata permissions
+        Roles with update `$team` metadata permissions
         """
         return pulumi.get(self, "roles")
 
     @property
     @pulumi.getter
     def teams(self) -> Optional[Sequence[str]]:
         """
-        Teams with update $team metadata permissions
+        Teams with update `$team` metadata permissions
         """
         return pulumi.get(self, "teams")
 
     @property
     @pulumi.getter
     def users(self) -> Optional[Sequence[str]]:
         """
-        Users with update $team metadata permissions
+        Users with update `$team` metadata permissions
         """
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
 class BlueprintPermissionsEntitiesUpdateMetadataPropertiesTitle(dict):
     @staticmethod
@@ -3038,17 +3038,17 @@
     def __init__(__self__, *,
                  owned_by_team: Optional[bool] = None,
                  roles: Optional[Sequence[str]] = None,
                  teams: Optional[Sequence[str]] = None,
                  users: Optional[Sequence[str]] = None):
         """
         :param bool owned_by_team: Owned by team
-        :param Sequence[str] roles: Roles with update $title metadata permissions
-        :param Sequence[str] teams: Teams with update $title metadata permissions
-        :param Sequence[str] users: Users with update $title metadata permissions
+        :param Sequence[str] roles: Roles with update `$title` metadata permissions
+        :param Sequence[str] teams: Teams with update `$title` metadata permissions
+        :param Sequence[str] users: Users with update `$title` metadata permissions
         """
         if owned_by_team is not None:
             pulumi.set(__self__, "owned_by_team", owned_by_team)
         if roles is not None:
             pulumi.set(__self__, "roles", roles)
         if teams is not None:
             pulumi.set(__self__, "teams", teams)
@@ -3063,31 +3063,31 @@
         """
         return pulumi.get(self, "owned_by_team")
 
     @property
     @pulumi.getter
     def roles(self) -> Optional[Sequence[str]]:
         """
-        Roles with update $title metadata permissions
+        Roles with update `$title` metadata permissions
         """
         return pulumi.get(self, "roles")
 
     @property
     @pulumi.getter
     def teams(self) -> Optional[Sequence[str]]:
         """
-        Teams with update $title metadata permissions
+        Teams with update `$title` metadata permissions
         """
         return pulumi.get(self, "teams")
 
     @property
     @pulumi.getter
     def users(self) -> Optional[Sequence[str]]:
         """
-        Users with update $title metadata permissions
+        Users with update `$title` metadata permissions
         """
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
 class BlueprintPermissionsEntitiesUpdateProperties(dict):
     @staticmethod
```

### Comparing `port_pulumi-2.0.1/port_pulumi/page.py` & `port_pulumi-2.0.3/port_pulumi/page.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/page_permissions.py` & `port_pulumi-2.0.3/port_pulumi/page_permissions.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/provider.py` & `port_pulumi-2.0.3/port_pulumi/provider.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/scorecard.py` & `port_pulumi-2.0.3/port_pulumi/scorecard.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/team.py` & `port_pulumi-2.0.3/port_pulumi/team.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi/webhook.py` & `port_pulumi-2.0.3/port_pulumi/webhook.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-2.0.3/port_pulumi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-pulumi
-Version: 2.0.1
+Version: 2.0.3
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `port_pulumi-2.0.1/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-2.0.3/port_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `port_pulumi-2.0.1/setup.py` & `port_pulumi-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.0.1"
+VERSION = "2.0.3"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "port Pulumi Package - Development Version"
```

