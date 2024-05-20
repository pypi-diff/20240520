# Comparing `tmp/maisaedu-utilities-prefect-1.1.8.tar.gz` & `tmp/maisaedu-utilities-prefect-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maisaedu-utilities-prefect-1.1.8.tar", last modified: Thu Aug 17 14:28:24 2023, max compression
+gzip compressed data, was "maisaedu-utilities-prefect-1.1.9.tar", last modified: Tue Aug 29 14:08:15 2023, max compression
```

## Comparing `maisaedu-utilities-prefect-1.1.8.tar` & `maisaedu-utilities-prefect-1.1.9.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.916272 maisaedu-utilities-prefect-1.1.8/
--rw-r--r--   0 vsts      (1001) docker     (123)     1081 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      286 2023-08-17 14:28:24.916272 maisaedu-utilities-prefect-1.1.8/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.912272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/
--rw-r--r--   0 vsts      (1001) docker     (123)      679 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.912272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/constants/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/constants/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       41 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/constants/environment.py
--rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/constants/notification.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.912272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/database/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/database/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2908 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/database/postgres.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11374 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/deploy.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4239 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/dw.py
--rw-r--r--   0 vsts      (1001) docker     (123)      349 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/environment.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.912272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/googlesheet/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/googlesheet/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2063 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/googlesheet/gspread.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.912272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/associations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/company.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/contacts.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1659 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/contacts_lists.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4275 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/deals.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2267 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/email_events.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/form_submission_events.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/forms.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2184 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/forms_submissions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3845 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/landing_pages.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1629 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/lineItems.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1936 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/marketing_emails.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2864 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/objects.py
--rw-r--r--   0 vsts      (1001) docker     (123)      693 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/owners.py
--rw-r--r--   0 vsts      (1001) docker     (123)      916 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/pipelines.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7439 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/tickets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2341 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/notification.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.912272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/one_drive/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/one_drive/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/one_drive/document_handling.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.912272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.916272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/models/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1955 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1007 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/models/datasetDatasourceModel.py
--rw-r--r--   0 vsts      (1001) docker     (123)      981 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/models/datasetRefreshScheduleModel.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.916272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4921 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3371 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2584 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4403 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/dataset_service.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1111 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/user_service.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.916272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/scripts/
--rw-r--r--   0 vsts      (1001) docker     (123)     1771 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/scripts/flow-mem-limit
--rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-08-17 14:28:06.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/scripts/refresh-secrets
--rw-r--r--   0 vsts      (1001) docker     (123)     4543 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/secrets.py
--rw-r--r--   0 vsts      (1001) docker     (123)      783 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/tunnel.py
--rw-r--r--   0 vsts      (1001) docker     (123)      506 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:24.912272 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      286 2023-08-17 14:28:24.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2675 2023-08-17 14:28:24.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-17 14:28:24.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       94 2023-08-17 14:28:24.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       27 2023-08-17 14:28:24.000000 maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-17 14:28:24.916272 maisaedu-utilities-prefect-1.1.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-08-17 14:28:07.000000 maisaedu-utilities-prefect-1.1.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.111463 maisaedu-utilities-prefect-1.1.9/
+-rw-r--r--   0 vsts      (1001) docker     (999)     1081 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (999)      286 2023-08-29 14:08:15.111463 maisaedu-utilities-prefect-1.1.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.103462 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/
+-rw-r--r--   0 vsts      (1001) docker     (999)      679 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.107463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/constants/
+-rw-r--r--   0 vsts      (1001) docker     (999)       81 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/constants/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)       41 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/constants/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (999)       31 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/constants/notification.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.107463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/database/
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/database/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2908 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/database/postgres.py
+-rw-r--r--   0 vsts      (1001) docker     (999)    11374 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/deploy.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     4239 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/dw.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      349 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/environment.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.107463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/googlesheet/
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/googlesheet/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2063 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/googlesheet/gspread.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.107463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1456 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/associations.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1750 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/company.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     5244 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/contacts.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1659 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/contacts_lists.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     4275 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/deals.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2267 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/email_events.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2429 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/form_submission_events.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1523 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/forms.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2184 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/forms_submissions.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     3845 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/landing_pages.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1629 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/lineItems.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1936 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/marketing_emails.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2864 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/objects.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      693 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/owners.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      916 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/pipelines.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     7439 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/tickets.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2341 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/notification.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.107463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/one_drive/
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/one_drive/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     3045 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/one_drive/document_handling.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.107463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.107463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/models/
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1955 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1007 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/models/datasetDatasourceModel.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      981 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/models/datasetRefreshScheduleModel.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.107463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     4921 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     3371 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2584 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/client.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     4403 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/dataset_service.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1111 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/user_service.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.111463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/prefect_api/
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/prefect_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1157 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/prefect_api/flows.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.111463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/scripts/
+-rw-r--r--   0 vsts      (1001) docker     (999)     1771 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/scripts/flow-mem-limit
+-rw-r--r--   0 vsts      (1001) docker     (999)      140 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/scripts/refresh-secrets
+-rw-r--r--   0 vsts      (1001) docker     (999)     4543 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/secrets.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      783 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/tunnel.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      506 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:15.107463 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (999)      286 2023-08-29 14:08:15.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (999)     2774 2023-08-29 14:08:15.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (999)        1 2023-08-29 14:08:15.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (999)       94 2023-08-29 14:08:15.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (999)       27 2023-08-29 14:08:15.000000 maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (999)       38 2023-08-29 14:08:15.111463 maisaedu-utilities-prefect-1.1.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (999)      745 2023-08-29 14:07:59.000000 maisaedu-utilities-prefect-1.1.9/setup.py
```

### Comparing `maisaedu-utilities-prefect-1.1.8/LICENSE` & `maisaedu-utilities-prefect-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/__init__.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/__init__.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/database/postgres.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/database/postgres.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/deploy.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/deploy.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/dw.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/dw.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/googlesheet/gspread.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/googlesheet/gspread.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/associations.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/associations.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/company.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/company.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/contacts.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/contacts.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/contacts_lists.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/contacts_lists.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/deals.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/deals.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/email_events.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/email_events.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/form_submission_events.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/form_submission_events.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/forms.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/forms.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/forms_submissions.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/forms_submissions.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/landing_pages.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/landing_pages.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/lineItems.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/lineItems.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/marketing_emails.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/marketing_emails.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/objects.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/objects.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/owners.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/owners.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/pipelines.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/pipelines.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/hubspot/tickets.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/hubspot/tickets.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/notification.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/notification.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/one_drive/document_handling.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/one_drive/document_handling.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/models/datasetDatasourceModel.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/models/datasetDatasourceModel.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/models/datasetRefreshScheduleModel.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/models/datasetRefreshScheduleModel.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/client.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/client.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/dataset_service.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/dataset_service.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/powerbi_api/services/user_service.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/powerbi_api/services/user_service.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/scripts/flow-mem-limit` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/scripts/flow-mem-limit`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/secrets.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/secrets.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect/tunnel.py` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect/tunnel.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.1.8/maisaedu_utilities_prefect.egg-info/SOURCES.txt` & `maisaedu-utilities-prefect-1.1.9/maisaedu_utilities_prefect.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,9 +46,11 @@
 maisaedu_utilities_prefect/powerbi_api/models/datasetRefreshScheduleModel.py
 maisaedu_utilities_prefect/powerbi_api/services/__init__.py
 maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py
 maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py
 maisaedu_utilities_prefect/powerbi_api/services/client.py
 maisaedu_utilities_prefect/powerbi_api/services/dataset_service.py
 maisaedu_utilities_prefect/powerbi_api/services/user_service.py
+maisaedu_utilities_prefect/prefect_api/__init__.py
+maisaedu_utilities_prefect/prefect_api/flows.py
 maisaedu_utilities_prefect/scripts/flow-mem-limit
 maisaedu_utilities_prefect/scripts/refresh-secrets
```

### Comparing `maisaedu-utilities-prefect-1.1.8/setup.py` & `maisaedu-utilities-prefect-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="maisaedu-utilities-prefect",
-    version="1.1.8",
+    version="1.1.9",
     description="Utilities for interaction with Prefect, for +A Education",
     license="MIT License",
     author="A+ Educação",
     author_email="dataeng@maisaedu.com.br",
     packages=find_packages(),
     scripts=[
         "maisaedu_utilities_prefect/scripts/refresh-secrets",
```

