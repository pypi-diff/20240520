# Comparing `tmp/user-local-0.0.8.tar.gz` & `tmp/user-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-local-0.0.8.tar", last modified: Fri Nov 10 10:23:47 2023, max compression
+gzip compressed data, was "user-local-0.0.9.tar", last modified: Sat Feb 24 18:11:54 2024, max compression
```

## Comparing `user-local-0.0.8.tar` & `user-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:23:47.692134 user-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-11-10 10:23:47.692134 user-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-11-10 10:23:09.000000 user-local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-11-10 10:23:09.000000 user-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 10:23:47.696133 user-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-11-10 10:23:09.000000 user-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:23:47.692134 user-local-0.0.8/user_local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:23:09.000000 user-local-0.0.8/user_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:23:47.692134 user-local-0.0.8/user_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 10:23:09.000000 user-local-0.0.8/user_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2023-11-10 10:23:09.000000 user-local-0.0.8/user_local/src/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-11-10 10:23:09.000000 user-local-0.0.8/user_local/src/user_local_constans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 10:23:47.692134 user-local-0.0.8/user_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-11-10 10:23:47.000000 user-local-0.0.8/user_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-11-10 10:23:47.000000 user-local-0.0.8/user_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 10:23:47.000000 user-local-0.0.8/user_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-10 10:23:47.000000 user-local-0.0.8/user_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 18:11:54.158143 user-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-24 18:11:54.154143 user-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-02-24 18:11:13.000000 user-local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-24 18:11:13.000000 user-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 18:11:54.158143 user-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-24 18:11:13.000000 user-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 18:11:54.154143 user-local-0.0.9/user_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 18:11:54.154143 user-local-0.0.9/user_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 18:11:13.000000 user-local-0.0.9/user_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-24 18:11:13.000000 user-local-0.0.9/user_local/src/constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-02-24 18:11:13.000000 user-local-0.0.9/user_local/src/user_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 18:11:54.154143 user-local-0.0.9/user_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-24 18:11:54.000000 user-local-0.0.9/user_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-24 18:11:54.000000 user-local-0.0.9/user_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 18:11:54.000000 user-local-0.0.9/user_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-24 18:11:54.000000 user-local-0.0.9/user_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-24 18:11:54.000000 user-local-0.0.9/user_local.egg-info/top_level.txt
```

### Comparing `user-local-0.0.8/README.md` & `user-local-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 # python-package-template
+
 To create local package and remote package layers (not to create GraphQL and REST-API layers)
 
 # directory structure
-Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e. location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br> 
+
+Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e.
+location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br>
 /location_local<br>
 /location_local/get_country_name<br>
 /location_local/get_country_name/src<br>
 /location_local/get_country_name/src/get_country_name.py<br>
 /location_local/get_country_name/tests<br>
 /location_local/get_country_name/tests/test_get_country_name.py<br>
 
 # database Python scripts in /db folder
+
 Please place <table-name>.py in /db<br>
 No need for seperate file for _ml table<br>
 Please delete the example file if not needed<br>
-  
+
 # Create the files to create the database schema, tables, view and populate Meta Data and Test Date
+
 /db/<table-name>.py - CREATE SCHEMA ... CREATE TABLE ... CREATE VIEW ...<br>
 /db/<table-name>_insert.py to create records
 
 # Update the setup.py (i.e.name, version)
- 
+
 # Please create test directory inside the directory of the project i.e. /<project-name>/tests
 
 # Update the serverless.yml in the root directory
+
 provider:
-  stage: play1
-  
+stage: play1
+
 Update the endpoints in serverless.yml
 
 # Working with VS Code
+
 Please make sure you push to the repo launch.json fie that enables to run and debug the code<br>
 
 # Unit-Test
+
 We prefer using pytest and not unittest package<br>
 
 Please create pytest.init in the project directory and not in the root directory
+
 ```
 [pytest]
 markers =
     test: custom mark for tests
 ```
```

### Comparing `user-local-0.0.8/pyproject.toml` & `user-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user-local-0.0.8/user_local/src/user_local_constans.py` & `user-local-0.0.9/user_local/src/constans.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from database_infrastructure_local.number_generator import NumberGenerator
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
-from circles_number_generator.number_generator import NumberGenerator  # noqa: E402
 
 USER_LOCAL_PYTHON_PACKAGE_COMPONENT_ID = 171
 USER_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME = "user_local/src/user.py"
-USER_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME_TEST = 'user/tests/user_test.py'
+USER_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME_TEST = 'user_local/tests/user_test.py'
 
 user_local_python_code_logger_object = {
     'component_id': USER_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
     'component_name': USER_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': 'sahar.g@circ.zone'
 }
@@ -32,8 +32,7 @@
 TEST_FIRST_NAME1 = "test_first_name" + str(number)
 TEST_LAST_NAME1 = "test_last_name" + str(number)
 
 TEST_USERNAME2 = "test_username" + str(number)
 TEST_MAIN_EMAIL2 = "test_email@address" + str(number)
 TEST_FIRST_NAME2 = "test_first_name" + str(number)
 TEST_LAST_NAME2 = "test_last_name" + str(number)
-
```

