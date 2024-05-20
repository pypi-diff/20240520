# Comparing `tmp/leverage-1.9.2.tar.gz` & `tmp/leverage-1.9.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leverage-1.9.2.tar", last modified: Mon Jan 30 14:41:21 2023, max compression
+gzip compressed data, was "leverage-1.9.4rc1.tar", max compression
```

## Comparing `leverage-1.9.2.tar` & `leverage-1.9.4rc1.tar`

### file list

```diff
@@ -1,33 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:41:21.986854 leverage-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-30 14:40:19.000000 leverage-1.9.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-01-30 14:41:21.986854 leverage-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-01-30 14:40:19.000000 leverage-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:41:21.986854 leverage-1.9.2/leverage/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/_internals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    27587 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/leverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:41:21.986854 leverage-1.9.2/leverage/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/modules/tfautomv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-01-30 14:40:19.000000 leverage-1.9.2/leverage/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:41:21.986854 leverage-1.9.2/leverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-30 14:41:21.000000 leverage-1.9.2/leverage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-30 14:40:19.000000 leverage-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-01-30 14:41:21.986854 leverage-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-30 14:40:19.000000 leverage-1.9.2/setup.py
+-rw-r--r--   0        0        0    11357 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/LICENSE.txt
+-rw-r--r--   0        0        0     7551 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/README.md
+-rw-r--r--   0        0        0      413 2024-04-25 14:02:06.807461 leverage-1.9.4rc1/leverage/__init__.py
+-rw-r--r--   0        0        0     1243 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/_internals.py
+-rw-r--r--   0        0        0     1413 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/_parsing.py
+-rw-r--r--   0        0        0     7888 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/_utils.py
+-rw-r--r--   0        0        0     1774 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/conf.py
+-rw-r--r--   0        0        0    28719 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/container.py
+-rw-r--r--   0        0        0     2633 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/containers/kubectl.py
+-rw-r--r--   0        0        0     1714 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/leverage.py
+-rw-r--r--   0        0        0     4857 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/logger.py
+-rw-r--r--   0        0        0      168 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/__init__.py
+-rw-r--r--   0        0        0     5830 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/auth.py
+-rw-r--r--   0        0        0     8304 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/aws.py
+-rw-r--r--   0        0        0    27859 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/credentials.py
+-rw-r--r--   0        0        0     1255 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/kubectl.py
+-rw-r--r--   0        0        0    11838 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/project.py
+-rw-r--r--   0        0        0     5350 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/run.py
+-rw-r--r--   0        0        0     1442 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/shell.py
+-rw-r--r--   0        0        0    19323 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/terraform.py
+-rw-r--r--   0        0        0     1325 2024-04-25 14:01:46.883397 leverage-1.9.4rc1/leverage/modules/tfautomv.py
+-rw-r--r--   0        0        0     1706 2024-04-25 14:01:46.887397 leverage-1.9.4rc1/leverage/modules/utils.py
+-rw-r--r--   0        0        0     9238 2024-04-25 14:01:46.887397 leverage-1.9.4rc1/leverage/path.py
+-rw-r--r--   0        0        0     8545 2024-04-25 14:01:46.887397 leverage-1.9.4rc1/leverage/tasks.py
+-rw-r--r--   0        0        0     1565 2024-04-25 14:02:06.807461 leverage-1.9.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     8857 1970-01-01 00:00:00.000000 leverage-1.9.4rc1/PKG-INFO
```

### Comparing `leverage-1.9.2/LICENSE.txt` & `leverage-1.9.4rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `leverage-1.9.2/leverage/_internals.py` & `leverage-1.9.4rc1/leverage/_internals.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,47 +5,48 @@
 
 import click
 
 from leverage.logger import get_verbosity
 
 
 class Module:
-    """ Module containing all tasks to be run. """
+    """Module containing all tasks to be run."""
+
     def __init__(self, name="build.py", tasks=None, default_task=None):
         self.name = name
         self.tasks = tasks if tasks is not None else []
         self.default_task = default_task
 
     def __eq__(self, other):
-        return (self.name == other.name
-                and self.tasks == other.tasks
-                and self.default_task == other.default_task)
+        return self.name == other.name and self.tasks == other.tasks and self.default_task == other.default_task
 
 
 class State:
-    """ Internal state of the application. """
+    """Internal state of the application."""
+
     def __init__(self):
         self._verbosity = None
         self.module = Module()
         self.container = None
 
     @property
     def verbosity(self):
         return self._verbosity
 
     @verbosity.setter
     def verbosity(self, verbose):
         self._verbosity = get_verbosity(verbose=verbose)
 
 
-pass_state =  click.make_pass_decorator(State, ensure=True)
+pass_state = click.make_pass_decorator(State, ensure=True)
 
 
 def pass_container(command):
-    """ Decorator to pass the current container to the command. """
+    """Decorator to pass the current container to the command."""
+
     @wraps(command)
     def new_command(*args, **kwargs):
         ctx = click.get_current_context()
 
         return command(ctx.obj.container, *args, **kwargs)
 
     return new_command
```

### Comparing `leverage-1.9.2/leverage/_parsing.py` & `leverage-1.9.4rc1/leverage/_parsing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
     Command line arguments and tasks arguments parsing utilities.
 """
+
+
 class InvalidArgumentOrderError(RuntimeError):
     pass
 
 
 class DuplicateKeywordArgumentError(RuntimeError):
     pass
 
 
 def parse_task_args(arguments):
-    """ Parse the arguments for a task and return args and kwargs appropriately
+    """Parse the arguments for a task and return args and kwargs appropriately
 
     Args:
         arguments (str): Arguments to parse.
 
     Raises:
         InvalidArgumentOrderError: When a positional argument is given after keyworded
             arguments are already been specified.
@@ -30,15 +32,17 @@
         return args, kwargs
 
     arguments = arguments.split(",")
 
     for argument in arguments:
         if "=" not in argument:
             if kwargs:
-                raise InvalidArgumentOrderError(f"Positional argument `{argument}` from task `{{task}}` cannot follow a keyword argument.")
+                raise InvalidArgumentOrderError(
+                    f"Positional argument `{argument}` from task `{{task}}` cannot follow a keyword argument."
+                )
 
             args.append(argument.strip())
 
         else:
             key, value = [part.strip() for part in argument.split("=")]
             if key in kwargs:
                 raise DuplicateKeywordArgumentError(f"Duplicated keyword argument `{key}` in task `{{task}}`.")
```

### Comparing `leverage-1.9.2/leverage/conf.py` & `leverage-1.9.4rc1/leverage/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from leverage.path import get_working_path
 
 
 ENV_CONFIG_FILE = "build.env"
 
 
 def load(config_filename=ENV_CONFIG_FILE):
-    """ Load all .env files with the given name in the current directory an all of its parents up to
+    """Load all .env files with the given name in the current directory an all of its parents up to
     the repository root directory and store them in a dictionary.
     Files are traversed from parent to child as to allow values in deeper directories to override possible
     previously existing values.
     Terminates if not ran within a git repository.
 
     Args:
         config_filename (str, optional): .env filenames to load. All must bear the same name. Defaults to "build.env".
```

### Comparing `leverage-1.9.2/leverage/container.py` & `leverage-1.9.4rc1/leverage/container.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,110 @@
 import json
+import os
+import re
+import webbrowser
 from pathlib import Path
 from datetime import datetime
-from datetime import timedelta
+from time import sleep
 
 import hcl2
 from click.exceptions import Exit
 import dockerpty
+from configupdater import ConfigUpdater
 from docker import DockerClient
 from docker.errors import APIError, NotFound
 from docker.types import Mount
+from typing import Tuple, Union
 
 from leverage import __toolbox_version__
 from leverage import logger
-from leverage.logger import console
+from leverage._utils import AwsCredsEntryPoint, CustomEntryPoint, ExitError, ContainerSession
+from leverage.modules.auth import refresh_layer_credentials
+from leverage.logger import console, raw_logger
 from leverage.logger import get_script_log_level
-from leverage.path import get_root_path
-from leverage.path import get_account_path
-from leverage.path import get_global_config_path
-from leverage.path import get_account_config_path
-from leverage.path import NotARepositoryError
+from leverage.path import PathsHandler
 from leverage.conf import load as load_env
 
+REGION = (
+    r"(.*)"  # project folder
+    # start region
+    r"(global|(?:[a-z]{2}-(?:gov-)?"
+    r"(?:central|north|south|east|west|northeast|northwest|southeast|southwest|secret|topsecret)-[1-4]))"
+    # end region
+    r"(.*)"  # layer
+)
+
 
 def get_docker_client():
-    """ Attempt to get a Docker client from the environment configuration. Halt application otherwise.
+    """Attempt to get a Docker client from the environment configuration. Halt application otherwise.
 
     Raises:
         Exit: If communication to Docker server could not be established.
 
     Returns:
         docker.DockerClient: Client for Docker daemon.
     """
     try:
         docker_client = DockerClient.from_env()
         docker_client.ping()
 
     except:
-        logger.error("Docker daemon doesn't seem to be responding. "
-                     "Please check it is up and running correctly before re-running the command.")
+        logger.error(
+            "Docker daemon doesn't seem to be responding. "
+            "Please check it is up and running correctly before re-running the command."
+        )
         raise Exit(1)
 
     return docker_client
 
 
 class LeverageContainer:
-    """ Basic Leverage Container. Holds the minimum information required to run the Docker image that Leverage uses
+    """Basic Leverage Container. Holds the minimum information required to run the Docker image that Leverage uses
     to perform its operations. Commands can be issued as interactive via `start` for when live output or user input is desired
     or the can be simply executed via `exec` to run silently and retrieve the command output.
 
     NOTE: An aggregation approach to this design should be considered instead of the current inheritance approach.
     """
-    LEVERAGE_IMAGE = "binbash/leverage-toolbox"
-
-    SSO_LOGIN_URL = "https://device.sso.{region}.amazonaws.com"
 
-    COMMON_TFVARS = "common.tfvars"
-    ACCOUNT_TFVARS = "account.tfvars"
-    BACKEND_TFVARS = "backend.tfvars"
+    LEVERAGE_IMAGE = "binbash/leverage-toolbox"
+    SHELL = "/bin/bash"
 
-    def __init__(self, client):
-        """ Project related paths are determined and stored. Project configuration is loaded.
+    def __init__(self, client, mounts: tuple = None, env_vars: dict = None):
+        """Project related paths are determined and stored. Project configuration is loaded.
 
         Args:
             client (docker.DockerClient): Client to interact with Docker daemon.
         """
         self.client = client
-
-        self.home = Path.home()
-        self.cwd = Path.cwd()
-        try:
-            self.root_dir = Path(get_root_path())
-            self.account_dir = Path(get_account_path())
-            self.common_config_dir = Path(get_global_config_path())
-            self.account_config_dir = Path(get_account_config_path())
-        except NotARepositoryError:
-            logger.error("Out of Leverage project context. Please cd into a Leverage project directory first.")
-            raise Exit(1)
-
         # Load configs
         self.env_conf = load_env()
 
-        common_config = self.common_config_dir / self.COMMON_TFVARS
-        self.common_conf = hcl2.loads(common_config.read_text()) if common_config.exists() else {}
-
-        account_config = self.account_config_dir / self.ACCOUNT_TFVARS
-        self.account_conf = hcl2.loads(account_config.read_text()) if account_config.exists() else {}
+        self.paths = PathsHandler(self.env_conf)
+        self.project = self.paths.project
 
         # Set image to use
         self.image = self.env_conf.get("TERRAFORM_IMAGE", self.LEVERAGE_IMAGE)
         self.image_tag = self.env_conf.get("TERRAFORM_IMAGE_TAG")
         if not self.image_tag:
-            logger.error("No docker image tag defined.\n"
-                         "Please set `TERRAFORM_IMAGE_TAG` variable before running a Leverage command.")
-            raise Exit(1)
-
-        # Get project name
-        self.project = self.common_conf.get("project", self.env_conf.get("PROJECT", False))
-        if not self.project:
-            logger.error("Project name has not been set. Exiting.")
+            logger.error(
+                "No docker image tag defined.\n"
+                "Please set `TERRAFORM_IMAGE_TAG` variable in the project's [bold]build.env[/bold] file before running a Leverage command."
+            )
             raise Exit(1)
 
-        # Project mount location
-        self.guest_base_path = f"/{self.common_conf.get('project_long', 'project')}"
-
-        # Ensure credentials directory
-        self.host_aws_credentials_dir = self.home / ".aws" / self.project
-        if not self.host_aws_credentials_dir.exists():
-            self.host_aws_credentials_dir.mkdir(parents=True)
-        self.sso_cache = self.host_aws_credentials_dir / "sso" / "cache"
-
-        self.host_config = self.client.api.create_host_config(
-            security_opt=["label:disable"],
-            mounts=[]
-        )
+        mounts = [Mount(source=source, target=target, type="bind") for source, target in mounts] if mounts else []
+        self.host_config = self.client.api.create_host_config(security_opt=["label:disable"], mounts=mounts)
         self.container_config = {
             "image": f"{self.image}:{self.image_tag}",
             "command": "",
             "stdin_open": True,
-            "environment": {},
+            "environment": env_vars or {},
             "entrypoint": "",
-            "working_dir": f"{self.guest_base_path}/{self.cwd.relative_to(self.root_dir).as_posix()}",
-            "host_config": self.host_config
+            "working_dir": f"{self.paths.guest_base_path}/{self.paths.cwd.relative_to(self.paths.root_dir).as_posix()}",
+            "host_config": self.host_config,
         }
 
     @property
     def environment(self):
         return self.container_config["environment"]
 
     @environment.setter
@@ -144,47 +124,40 @@
         return self.container_config["host_config"]["Mounts"]
 
     @mounts.setter
     def mounts(self, value):
         self.container_config["host_config"]["Mounts"] = value
 
     @property
-    def guest_account_base_path(self):
-        return f"{self.guest_base_path}/{self.account_dir.relative_to(self.root_dir).as_posix()}"
-
-    @property
-    def common_tfvars(self):
-        return f"{self.guest_base_path}/config/{self.COMMON_TFVARS}"
-
-    @property
-    def account_tfvars(self):
-        return f"{self.guest_account_base_path}/config/{self.ACCOUNT_TFVARS}"
+    def region(self):
+        """
+        Return the region of the layer.
+        """
+        if matches := re.match(REGION, self.paths.cwd.as_posix()):
+            # the region (group 1) is between the projects folders (group 0) and the layers (group 2)
+            return matches.groups()[1]
 
-    @property
-    def backend_tfvars(self):
-        return f"{self.guest_account_base_path}/config/{self.BACKEND_TFVARS}"
-
-    @property
-    def guest_aws_credentials_dir(self):
-        return f"/root/tmp/{self.project}"
+        raise ExitError(1, f"No valid region could be found at: {self.paths.cwd.as_posix()}")
 
     def ensure_image(self):
-        """ Make sure the required Docker image is available in the system. If not, pull it from registry. """
+        """Make sure the required Docker image is available in the system. If not, pull it from registry."""
         found_image = self.client.api.images(f"{self.image}:{self.image_tag}")
         if found_image:
             return
 
         logger.info("Required Docker image not found.")
 
         try:
             stream = self.client.api.pull(repository=self.image, tag=self.image_tag, stream=True, decode=True)
         except NotFound as e:
-            logger.error(f"The specified toolbox version, '{self.image_tag}' (toolbox image '{self.image}:{self.image_tag}') can not be found. "
-                         "If you come from a project created with an older version of Leverage CLI or have modified the 'build.env' file manually, "
-                         f"please consider either deleting the file, or configuring a valid toolbox version to use. (i.e. 'TERRAFORM_IMAGE_TAG={__toolbox_version__}')")
+            logger.error(
+                f"The specified toolbox version, '{self.image_tag}' (toolbox image '{self.image}:{self.image_tag}') can not be found. "
+                "If you come from a project created with an older version of Leverage CLI or have modified the 'build.env' file manually, "
+                f"please consider either deleting the file, or configuring a valid toolbox version to use. (i.e. 'TERRAFORM_IMAGE_TAG={__toolbox_version__}')"
+            )
             raise Exit(1)
         except APIError as pull:
             pull.__traceback__ = None
             pull.__context__.__traceback__ = None
             logger.exception("Error pulling image:", exc_info=pull)
             raise Exit(1)
         except Exception as e:
@@ -200,15 +173,15 @@
                 if status.startswith("Digest") or status.startswith("Status"):
                     imageinfo.append(status)
 
         for info in imageinfo:
             logger.info(info)
 
     def _create_container(self, tty, command="", *args):
-        """ Create the container that will run the command.
+        """Create the container that will run the command.
 
         Args:
             tty (bool): Whether the container will run interactively or not.
             command (str, optional): Command to run. Defaults to "".
 
         Raises:
             Exit: If the container could not be created.
@@ -227,15 +200,15 @@
         except APIError as exc:
             exc.__traceback__ = None
             exc.__context__.__traceback__ = None
             logger.exception("Error creating container:", exc_info=exc)
             raise Exit(1)
 
     def _run(self, container, run_func):
-        """ Apply the given run function to the given container, return its outputs and handle container cleanup.
+        """Apply the given run function to the given container, return its outputs and handle container cleanup.
 
         Args:
             container (dict): Reference to a Docker container.
             run_func (function): Function to apply to the given container.
 
         Returns:
             any: Whatever the given function returns.
@@ -248,455 +221,488 @@
             exc.__context__.__traceback__ = None
             logger.exception("Error during container execution:", exc_info=exc)
 
         finally:
             self.client.api.stop(container)
             self.client.api.remove_container(container)
 
-    def _start(self, command="/bin/sh", *args):
-        """ Create an interactive container, and run command with the given arguments.
+    def _start(self, command: str, *args):
+        """Create an interactive container, and run command with the given arguments.
 
         Args:
-            command (str, optional): Command to run. Defaults to "/bin/sh".
+            command: Command to run.
 
         Returns:
             int: Execution exit code.
         """
         container = self._create_container(True, command, *args)
 
         def run_func(client, container):
             dockerpty.start(client=client.api, container=container)
             return client.api.inspect_container(container)["State"]["ExitCode"]
 
         return self._run(container, run_func)
 
-    def start(self, command="/bin/sh", *arguments):
-        """ Run command with the given arguments in an interactive container.
+    def _start_with_output(self, command, *args):
+        """
+        Same than _start but also returns the outputs (by dumping the logs) of the container.
+        """
+        container = self._create_container(True, command, *args)
 
-        Args:
-            command (str, optional): Command. Defaults to "/bin/sh".
+        def run_func(client, container):
+            dockerpty.start(client=client.api, container=container)
+            exit_code = client.api.inspect_container(container)["State"]["ExitCode"]
+            logs = client.api.logs(container).decode("utf-8")
+            return exit_code, logs
 
-        Returns:
-            int: Execution exit code.
+        return self._run(container, run_func)
+
+    def start(self, command: str, *arguments) -> int:
+        """Run command with the given arguments in an interactive container.
+        Returns execution exit code.
         """
         return self._start(command, *arguments)
 
-    def _exec(self, command="", *args):
-        """ Create a non interactive container and execute command with the given arguments.
-
-        Args:
-            command (str, optional): Command. Defaults to "".
-
-        Returns:
-            int, str: Execution exit code and output.
+    def _exec(self, command: str, *args) -> Tuple[int, str]:
+        """Create a non interactive container and execute command with the given arguments.
+        Returns execution exit code and output.
         """
         container = self._create_container(False, command, *args)
 
         def run_func(client, container):
             client.api.start(container)
             exit_code = client.api.wait(container)["StatusCode"]
             output = client.api.logs(container).decode("utf-8")
             return exit_code, output
 
         return self._run(container, run_func)
 
-    def exec(self, command="", *arguments):
-        """ Execute command with the given arguments in a container.
+    def exec(self, command: str, *arguments) -> Tuple[int, str]:
+        """Execute command with the given arguments in a container.
+        Returns execution exit code and output.
+        """
+        return self._exec(command, *arguments)
 
-        Args:
-            command (str, optional): Command. Defaults to "".
+    def docker_logs(self, container):
+        return self.client.api.logs(container).decode("utf-8")
 
-        Returns:
-            int, str: Execution exit code and output/
+    def change_ownership_cmd(self, path: Union[Path, str], recursive=True) -> str:
+        recursive = "-R " if recursive else ""
+        user_id = os.getuid()
+        group_id = os.getgid()
+
+        return f"chown {user_id}:{group_id} {recursive}{path}"
+
+    def change_file_ownership(self, path: Union[Path, str], recursive=True):
         """
-        return self._exec(command, *arguments)
+        Change the file/folder ownership from the internal docker user (usually root)
+        to the user executing the CLI.
+        """
+        cmd = self.change_ownership_cmd(path, recursive=recursive)
+        with CustomEntryPoint(self, entrypoint=""):
+            self._exec(cmd)
+
 
-    def get_location_type(self):
+class SSOContainer(LeverageContainer):
+    def get_sso_access_token(self):
+        with open(self.paths.sso_token_file) as token_file:
+            return json.loads(token_file.read())["accessToken"]
+
+    @property
+    def sso_region_from_main_profile(self):
         """
-        Returns the location type:
-        - root
-        - account
-        - config
-        - layer
-        - sublayer
-        - not a project
-        """
-        if self.cwd == self.root_dir:
-            return 'root'
-        elif self.cwd == self.account_dir:
-            return 'account'
-        elif self.cwd in (self.common_config_dir, self.account_config_dir):
-            return 'config'
-        elif (self.cwd.as_posix().find(self.account_dir.as_posix()) >= 0) and list(self.cwd.glob("*.tf")):
-            return 'layer'
-        elif (self.cwd.as_posix().find(self.account_dir.as_posix()) >= 0) and not list(self.cwd.glob("*.tf")):
-            return 'layers-group'
-        else:
-            return 'not a project'
+        Same than AWSCLIContainer.get_sso_region but without using a container.
+        """
+        conf = ConfigUpdater()
+        conf.read(self.paths.host_aws_profiles_file)
+        return conf.get(f"profile {self.project}-sso", "sso_region").value
+
 
+class AWSCLIContainer(SSOContainer):
+    """Leverage Container specially tailored to run AWS CLI commands."""
 
-class AWSCLIContainer(LeverageContainer):
-    """ Leverage Container specially tailored to run AWS CLI commands. """
     AWS_CLI_BINARY = "/usr/local/bin/aws"
 
+    # SSO scripts
     AWS_SSO_LOGIN_SCRIPT = "/root/scripts/aws-sso/aws-sso-login.sh"
     AWS_SSO_LOGOUT_SCRIPT = "/root/scripts/aws-sso/aws-sso-logout.sh"
-    AWS_SSO_CONFIGURE_SCRIPT = "/root/scripts/aws-sso/aws-sso-configure.sh"
+
+    # SSO constants
+    AWS_SSO_LOGIN_URL = "https://device.sso.{region}.amazonaws.com/?user_code={user_code}"
+    AWS_SSO_CODE_WAIT_SECONDS = 2
+    AWS_SSO_CODE_ATTEMPTS = 10
+    FALLBACK_LINK_MSG = "Opening the browser... if it fails, open this link in your browser:\n{link}"
 
     def __init__(self, client):
         super().__init__(client)
 
         self.environment = {
-            "COMMON_CONFIG_FILE": self.common_tfvars,
-            "ACCOUNT_CONFIG_FILE": self.account_tfvars,
-            "BACKEND_CONFIG_FILE": self.backend_tfvars,
-            "AWS_SHARED_CREDENTIALS_FILE": f"{self.guest_aws_credentials_dir}/credentials",
-            "AWS_CONFIG_FILE": f"{self.guest_aws_credentials_dir}/config",
-            "SSO_CACHE_DIR": f"{self.guest_aws_credentials_dir}/sso/cache",
-            "SCRIPT_LOG_LEVEL": get_script_log_level()
+            "COMMON_CONFIG_FILE": self.paths.common_tfvars,
+            "ACCOUNT_CONFIG_FILE": self.paths.account_tfvars,
+            "BACKEND_CONFIG_FILE": self.paths.backend_tfvars,
+            "AWS_SHARED_CREDENTIALS_FILE": f"{self.paths.guest_aws_credentials_dir}/credentials",
+            "AWS_CONFIG_FILE": f"{self.paths.guest_aws_credentials_dir}/config",
+            "SSO_CACHE_DIR": f"{self.paths.guest_aws_credentials_dir}/sso/cache",
+            "SCRIPT_LOG_LEVEL": get_script_log_level(),
         }
         self.entrypoint = self.AWS_CLI_BINARY
         self.mounts = [
-            Mount(source=self.root_dir.as_posix(), target=self.guest_base_path, type="bind"),
-            Mount(source=self.host_aws_credentials_dir.as_posix(), target=self.guest_aws_credentials_dir, type="bind")
+            Mount(source=self.paths.root_dir.as_posix(), target=self.paths.guest_base_path, type="bind"),
+            Mount(
+                source=self.paths.host_aws_credentials_dir.as_posix(),
+                target=self.paths.guest_aws_credentials_dir,
+                type="bind",
+            ),
         ]
 
         logger.debug(f"[bold cyan]Container configuration:[/bold cyan]\n{json.dumps(self.container_config, indent=2)}")
 
-
     def start(self, command, profile=""):
         args = [] if not profile else ["--profile", profile]
         return self._start(command, *args)
 
+    # FIXME: we have a context manager for this now, remove this method later!
     def system_start(self, command):
-        """ Momentarily override the container's default entrypoint. To run arbitrary commands and not only AWS CLI ones. """
+        """Momentarily override the container's default entrypoint. To run arbitrary commands and not only AWS CLI ones."""
         self.entrypoint = ""
         exit_code = self._start(command)
         self.entrypoint = self.AWS_CLI_BINARY
         return exit_code
 
     def exec(self, command, profile=""):
         args = [] if not profile else ["--profile", profile]
         return self._exec(command, *args)
 
+    # FIXME: we have a context manager for this now, remove this method later!
     def system_exec(self, command):
-        """ Momentarily override the container's default entrypoint. To run arbitrary commands and not only AWS CLI ones. """
+        """Momentarily override the container's default entrypoint. To run arbitrary commands and not only AWS CLI ones."""
         self.entrypoint = ""
         exit_code, output = self._exec(command)
 
         self.entrypoint = self.AWS_CLI_BINARY
         return exit_code, output
 
+    def get_sso_code(self, container) -> str:
+        """
+        Find and return the SSO user code by periodically checking the logs.
+        Up until N attempts.
+        """
+        logger.info("Fetching SSO code...")
+        for _ in range(self.AWS_SSO_CODE_ATTEMPTS):
+            # pull logs periodically until we find our SSO code
+            logs = self.docker_logs(container)
+            if "Then enter the code:" in logs:
+                return logs.split("Then enter the code:")[1].split("\n")[2]
+
+            sleep(self.AWS_SSO_CODE_WAIT_SECONDS)
+
+        raise ExitError(1, "Get SSO code timed-out")
+
+    def get_sso_region(self):
+        # TODO: what about using the .region property we have now? that takes the value from the path of the layer
+        _, region = self.exec(f"configure get sso_region --profile {self.project}-sso")
+        return region
+
+    def sso_login(self) -> int:
+        region = self.get_sso_region()
+
+        with CustomEntryPoint(self, ""):
+            container = self._create_container(False, command=self.AWS_SSO_LOGIN_SCRIPT)
+
+        with ContainerSession(self.client, container):
+            # once inside this block, the SSO_LOGIN_SCRIPT is being executed in the "background"
+            # now let's grab the user code from the logs
+            user_code = self.get_sso_code(container)
+            # with the user code, we can now autocomplete the url
+            link = self.AWS_SSO_LOGIN_URL.format(region=region.strip(), user_code=user_code)
+            webbrowser.open_new_tab(link)
+            # The SSO code is only valid once: if the browser was able to open it, the fallback link will be invalid
+            logger.info(self.FALLBACK_LINK_MSG.format(link=link))
+            # now let's wait until the command locking the container resolve itself:
+            # aws sso login will wait for the user code
+            # once submitted to the browser, the authentication finish and the lock is released
+            exit_code = self.client.api.wait(container)["StatusCode"]
+            raw_logger.info(self.docker_logs(container))
+            # now return ownership of the token file back to the user
+            self.change_file_ownership(self.paths.guest_aws_credentials_dir)
+
+        return exit_code
+
+
+class TerraformContainer(SSOContainer):
+    """Leverage container specifically tailored to run Terraform commands.
+    It handles authentication and some checks regarding where the command is being executed."""
 
-class TerraformContainer(LeverageContainer):
-    """ Leverage container specifically tailored to run Terraform commands.
-    It handles authentication and some checks regarding where the command is being executed. """
     TF_BINARY = "/bin/terraform"
 
     TF_MFA_ENTRYPOINT = "/root/scripts/aws-mfa/aws-mfa-entrypoint.sh"
     TF_SSO_ENTRYPOINT = "/root/scripts/aws-sso/aws-sso-entrypoint.sh"
 
-    def __init__(self, client):
-        super().__init__(client)
+    def __init__(self, client, mounts=None, env_vars=None):
+        super().__init__(client, mounts=mounts, env_vars=env_vars)
 
-        if self.root_dir == self.account_dir == self.common_config_dir == self.account_config_dir == self.cwd:
-            logger.error("Not running in a Leverage project. Exiting.")
-            raise Exit(1)
+        self.paths.assert_running_leverage_project()
 
         # Set authentication methods
-        self.sso_enabled = self.common_conf.get("sso_enabled", False)
-        self.mfa_enabled = self.env_conf.get("MFA_ENABLED", "false") == "true" # TODO: Convert values to bool upon loading
-
-        self.environment = {
-            "COMMON_CONFIG_FILE": self.common_tfvars,
-            "ACCOUNT_CONFIG_FILE": self.account_tfvars,
-            "BACKEND_CONFIG_FILE": self.backend_tfvars,
-            "AWS_SHARED_CREDENTIALS_FILE": f"{self.guest_aws_credentials_dir}/credentials",
-            "AWS_CONFIG_FILE": f"{self.guest_aws_credentials_dir}/config",
-            "SRC_AWS_SHARED_CREDENTIALS_FILE": f"{self.guest_aws_credentials_dir}/credentials", # Legacy?
-            "SRC_AWS_CONFIG_FILE": f"{self.guest_aws_credentials_dir}/config", # Legacy?
-            "AWS_CACHE_DIR": f"{self.guest_aws_credentials_dir}/cache",
-            "SSO_CACHE_DIR": f"{self.guest_aws_credentials_dir}/sso/cache",
-            "SCRIPT_LOG_LEVEL": get_script_log_level(),
-            "MFA_SCRIPT_LOG_LEVEL": get_script_log_level() # Legacy
-        }
+        self.sso_enabled = self.paths.common_conf.get("sso_enabled", False)
+        self.mfa_enabled = (
+            self.env_conf.get("MFA_ENABLED", "false") == "true"
+        )  # TODO: Convert values to bool upon loading
+
+        # SSH AGENT
+        SSH_AUTH_SOCK = os.getenv("SSH_AUTH_SOCK")
+
+        self.environment.update(
+            {
+                "COMMON_CONFIG_FILE": self.paths.common_tfvars,
+                "ACCOUNT_CONFIG_FILE": self.paths.account_tfvars,
+                "BACKEND_CONFIG_FILE": self.paths.backend_tfvars,
+                "AWS_SHARED_CREDENTIALS_FILE": f"{self.paths.guest_aws_credentials_dir}/credentials",
+                "AWS_CONFIG_FILE": f"{self.paths.guest_aws_credentials_dir}/config",
+                "SRC_AWS_SHARED_CREDENTIALS_FILE": f"{self.paths.guest_aws_credentials_dir}/credentials",  # Legacy?
+                "SRC_AWS_CONFIG_FILE": f"{self.paths.guest_aws_credentials_dir}/config",  # Legacy?
+                "AWS_CACHE_DIR": f"{self.paths.guest_aws_credentials_dir}/cache",
+                "SSO_CACHE_DIR": f"{self.paths.guest_aws_credentials_dir}/sso/cache",
+                "SCRIPT_LOG_LEVEL": get_script_log_level(),
+                "MFA_SCRIPT_LOG_LEVEL": get_script_log_level(),  # Legacy
+                "SSH_AUTH_SOCK": "" if SSH_AUTH_SOCK is None else "/ssh-agent",
+            }
+        )
         self.entrypoint = self.TF_BINARY
-        self.mounts = [
-            Mount(source=self.root_dir.as_posix(), target=self.guest_base_path, type="bind"),
-            Mount(source=self.host_aws_credentials_dir.as_posix(), target=self.guest_aws_credentials_dir, type="bind"),
-            Mount(source=(self.home / ".ssh").as_posix(), target="/root/.ssh", type="bind"),
-            Mount(source=(self.home / ".gitconfig").as_posix(), target="/etc/gitconfig", type="bind")
+        extra_mounts = [
+            Mount(source=self.paths.root_dir.as_posix(), target=self.paths.guest_base_path, type="bind"),
+            Mount(
+                source=self.paths.host_aws_credentials_dir.as_posix(),
+                target=self.paths.guest_aws_credentials_dir,
+                type="bind",
+            ),
+            Mount(source=(self.paths.home / ".gitconfig").as_posix(), target="/etc/gitconfig", type="bind"),
         ]
+        self.mounts.extend(extra_mounts)
+        # if you have set the tf plugin cache locally
+        if self.paths.tf_cache_dir:
+            # then mount it too into the container
+            self.environment["TF_PLUGIN_CACHE_DIR"] = self.paths.tf_cache_dir
+            # given that terraform use symlinks to point from the .terraform folder into the plugin folder
+            # we need to use the same directory inside the container
+            # otherwise symlinks will be broken once outside the container
+            # which will break terraform usage outside Leverage
+            self.mounts.append(Mount(source=self.paths.tf_cache_dir, target=self.paths.tf_cache_dir, type="bind"))
+        if SSH_AUTH_SOCK is not None:
+            self.mounts.append(Mount(source=SSH_AUTH_SOCK, target="/ssh-agent", type="bind"))
 
         self._backend_key = None
 
         logger.debug(f"[bold cyan]Container configuration:[/bold cyan]\n{json.dumps(self.container_config, indent=2)}")
 
-    def _guest_config_file(self, file):
-        """ Map config file in host to location in guest.
-
-        Args:
-            file (pathlib.Path): File in host to map
-
-        Raises:
-            Exit: If file is not contained in any valid config directory
-
-        Returns:
-            str: Path in guest to config file
+    def auth_method(self) -> str:
         """
-        file_name = file.name
+        Return the expected auth method based on the SSO or MFA flags.
 
-        if file.parent == self.account_config_dir:
-            return f"{self.guest_account_base_path}/config/{file_name}"
-        if file.parent == self.common_config_dir:
-            return f"{self.guest_base_path}/config/{file_name}"
+        In the case of MFA, we also need to tweak some env variables for AWS credentials.
+        Once you are done with authentication, remember to revert the env var changes.
+        """
+        if self.sso_enabled:
+            self._check_sso_token()
+            # sso credentials needs to be refreshed right before we execute our command on the container
+            refresh_layer_credentials(self)
+        elif self.mfa_enabled:
+            self.environment.update(
+                {
+                    "AWS_SHARED_CREDENTIALS_FILE": self.environment["AWS_SHARED_CREDENTIALS_FILE"].replace(
+                        "tmp", ".aws"
+                    ),
+                    "AWS_CONFIG_FILE": self.environment["AWS_CONFIG_FILE"].replace("tmp", ".aws"),
+                }
+            )
+            return f"{self.TF_MFA_ENTRYPOINT} -- "
 
-        logger.error("File is not part of any config directory.")
-        raise Exit(1)
+        return ""
 
     @property
     def tf_default_args(self):
-        """ Array of strings containing all valid config files for layer as parameters for Terraform """
-        common_config_files = [f"-var-file={self._guest_config_file(common_file)}"
-                               for common_file in self.common_config_dir.glob("*.tfvars")]
-        account_config_files = [f"-var-file={self._guest_config_file(account_file)}"
-                                for account_file in self.account_config_dir.glob("*.tfvars")]
-        region_settings      = [f"-var=\"region={self.region}\""]
-        return common_config_files + account_config_files + region_settings
+        """Array of strings containing all valid config files for layer as parameters for Terraform"""
+        common_config_files = [
+            f"-var-file={self.paths.guest_config_file(common_file)}"
+            for common_file in self.paths.common_config_dir.glob("*.tfvars")
+        ]
+        account_config_files = [
+            f"-var-file={self.paths.guest_config_file(account_file)}"
+            for account_file in self.paths.account_config_dir.glob("*.tfvars")
+        ]
+        return common_config_files + account_config_files
 
     def enable_mfa(self):
-        """ Enable Multi-Factor Authentication. """
+        """Enable Multi-Factor Authentication."""
         self.mfa_enabled = True
 
     def enable_sso(self):
-        """ Enable Single Sign-On Authentication. """
+        """Enable Single Sign-On Authentication."""
         self.sso_enabled = True
 
     def disable_authentication(self):
-        """ Disable all authentication. """
+        """Disable all authentication."""
         self.mfa_enabled = False
         self.sso_enabled = False
 
     def _check_sso_token(self):
-        """ Check for the existence and validity of the SSO token to be used to get credentials. """
+        """Check for the existence and validity of the SSO token to be used to get credentials."""
 
         # Adding `token` file name to this function in order to
         # meet the requirement regarding to have just one
         # token file in the sso/cache
-        sso_role = self.account_conf.get("sso_role")
-        token_file = self.sso_cache / sso_role
+        sso_role = self.paths.account_conf.get("sso_role")
+        token_file = self.paths.sso_cache / sso_role
 
-        token_files = list(self.sso_cache.glob("*"))
+        token_files = list(self.paths.sso_cache.glob("*"))
         if not token_files:
             logger.error("No AWS SSO token found. Please log in or configure SSO.")
             raise Exit(1)
 
         if token_file not in token_files:
-            sso_role = 'token'
-            token_file = self.sso_cache / sso_role
+            sso_role = "token"
+            token_file = self.paths.sso_cache / sso_role
             if token_file not in token_files:
-                logger.error("No valid AWS SSO token found for current account.\n"
-                            "Please log out and reconfigure SSO before proceeding.")
+                logger.error(
+                    "No valid AWS SSO token found for current account.\n"
+                    "Please log out and reconfigure SSO before proceeding."
+                )
                 raise Exit(1)
 
         entrypoint = self.entrypoint
         self.entrypoint = ""
 
         _, cached_token = self._exec(f"sh -c 'cat $SSO_CACHE_DIR/{sso_role}'")
         token = json.loads(cached_token)
         expiry = datetime.strptime(token.get("expiresAt"), "%Y-%m-%dT%H:%M:%SZ")
         renewal = datetime.utcnow()
 
         if expiry < renewal:
-            logger.error("AWS SSO token has expired, please log back in.")
+            logger.error(
+                "AWS SSO token has expired, please log back in by running [bold]leverage aws sso login[/bold]"
+                " to refresh your credentials before re-running the last command."
+            )
             raise Exit(1)
 
         self.entrypoint = entrypoint
 
-    def _prepare_container(self):
-        """ Adjust entrypoint and environment variables for when SSO or MFA are used.
-        Note that SSO takes precedence over MFA when both are active. """
-        if self.sso_enabled:
-            self._check_sso_token()
-
-            self.entrypoint = f"{self.TF_SSO_ENTRYPOINT} -- {self.entrypoint}"
-
-        elif self.mfa_enabled:
-            self.entrypoint = f"{self.TF_MFA_ENTRYPOINT} -- {self.entrypoint}"
-
-            self.environment.update({
-                "AWS_SHARED_CREDENTIALS_FILE": self.environment.get("AWS_SHARED_CREDENTIALS_FILE").replace("tmp", ".aws"),
-                "AWS_CONFIG_FILE": self.environment.get("AWS_CONFIG_FILE").replace("tmp", ".aws"),
-            })
-
-        logger.debug(f"[bold cyan]Running with entrypoint:[/bold cyan] {self.entrypoint}")
-
-    def check_for_layer_location(self):
-        """ Make sure the command is being ran at layer level. If not, bail. """
-        if self.cwd in (self.common_config_dir, self.account_config_dir):
-            logger.error("Currently in a configuration directory, no Terraform command can be run here.")
-            raise Exit(1)
-
-        if self.cwd in (self.root_dir, self.account_dir):
-            logger.error("Terraform commands cannot run neither in the root of the project or in"
-                         " the root directory of an account.")
-            raise Exit(1)
-
-        if not list(self.cwd.glob("*.tf")):
-            logger.error("This command can only run at [bold]layer[/bold] level.")
-            raise Exit(1)
+    def refresh_credentials(self):
+        with AwsCredsEntryPoint(self, override_entrypoint=""):
+            if exit_code := self._start('echo "Done."'):
+                return exit_code
 
     def start(self, command, *arguments):
-        self._prepare_container()
-
-        return self._start(command, *arguments)
+        with AwsCredsEntryPoint(self, self.entrypoint):
+            return self._start(command, *arguments)
 
     def start_in_layer(self, command, *arguments):
-        """ Run a command that can only be performed in layer level. """
-        self.check_for_layer_location()
+        """Run a command that can only be performed in layer level."""
+        self.paths.check_for_layer_location()
 
         return self.start(command, *arguments)
 
     def exec(self, command, *arguments):
-        self._prepare_container()
-
-        return self._exec(command, *arguments)
+        with AwsCredsEntryPoint(self):
+            return self._exec(command, *arguments)
 
+    # FIXME: we have a context manager for this now, remove this method later!
     def system_exec(self, command):
-        """ Momentarily override the container's default entrypoint. To run arbitrary commands and not only AWS CLI ones. """
+        """Momentarily override the container's default entrypoint. To run arbitrary commands and not only AWS CLI ones."""
         original_entrypoint = self.entrypoint
         self.entrypoint = ""
         exit_code, output = self._exec(command)
 
         self.entrypoint = original_entrypoint
         return exit_code, output
 
-
     def start_shell(self):
-        """ Launch a shell in the container. """
+        """Launch a shell in the container."""
         if self.mfa_enabled or self.sso_enabled:
-            self.check_for_layer_location()
-
-        self.entrypoint = ""
-        self._prepare_container()
-        self._start()
-
-    @property
-    def region(self):
-        """ Determine the region based on PATH, account tfvars or project tfvars. Returns a string with the region name. """
-        region = self._find_region(self.cwd.relative_to(self.account_dir))
-
-        if not region is None:
-            return region
-
-        logger.error("No region found")
-        raise Exit(1)
+            self.paths.check_for_layer_location()
 
-    @property
-    def terraform_backend(self):
-        """ Determine the terraform backend for the account. Returns an object with backend information. """
-        # These are the possible backend layer names for Refarch v1 and v2
-        possible_layer_names = ['terraform-backend', 'base-tf-backend']
-        for layer_name in possible_layer_names:
-            for directory in Path(self.account_dir).glob(f"**/{layer_name}"):
-
-                region = self._find_region(Path(directory).relative_to(self.account_dir))
-
-                if not region is None:
-                    return {'directory': directory , 'region': region}
-                else:
-                    logger.error("No region found for backend layer")
-                    raise Exit(1)
-
-        logger.error("No backend layer found")
-        raise Exit(1)
-
-    def _find_region(self, local_directory):
-        local_directory = local_directory.as_posix().split('/')
-        if len(local_directory) > 1:
-            if local_directory[0] != 'global':
-                return local_directory[0]
-
-        if 'region' in self.account_conf:
-            return self.account_conf.get('region')
-        if 'region' in self.common_conf:
-            return self.common_conf.get('region')
-        if 'region_primary' in self.account_conf:
-            return self.account_conf.get('region_primary')
-        if 'region_primary' in self.common_conf:
-            return self.common_conf.get('region_primary')
-
-        return None
+        with AwsCredsEntryPoint(self, override_entrypoint=""):
+            self._start(self.SHELL)
 
     def set_backend_key(self, skip_validation=False):
         # Scenarios:
         #
         # scenario    |  s3 backend set   |  s3 key set  |  skip_validation  |  result
         # 0           |  false            |  false       |  false            |  fail
         # 1           |  false            |  false       |  true             |  ok
         # 2           |  true             |  false       |  false/true       |  set the key
         # 3           |  true             |  true        |  false/true       |  read the key
         try:
-            config_tf_file = self.cwd / "config.tf"
+            config_tf_file = self.paths.cwd / "config.tf"
             config_tf = hcl2.loads(config_tf_file.read_text()) if config_tf_file.exists() else {}
-            if 'terraform' in config_tf and 'backend' in config_tf["terraform"][0] and 's3' in config_tf["terraform"][0]["backend"][0]:
-                if 'key' in config_tf["terraform"][0]["backend"][0]["s3"]:
+            if (
+                "terraform" in config_tf
+                and "backend" in config_tf["terraform"][0]
+                and "s3" in config_tf["terraform"][0]["backend"][0]
+            ):
+                if "key" in config_tf["terraform"][0]["backend"][0]["s3"]:
                     backend_key = config_tf["terraform"][0]["backend"][0]["s3"]["key"]
                     self._backend_key = backend_key
                 else:
-                    self._backend_key = f"{self.cwd.relative_to(self.root_dir).as_posix()}/terraform.tfstate".replace('/base-','/').replace('/tools-','/')
-
-                    in_container_file_path = f"{self.guest_base_path}/{config_tf_file.relative_to(self.root_dir).as_posix()}"
-                    resp = self.system_exec("hcledit "
-                                             f"-f {in_container_file_path} -u"
-                                             f" attribute append terraform.backend.key \"\\\"{self._backend_key}\\\"\"")
+                    self._backend_key = (
+                        f"{self.paths.cwd.relative_to(self.paths.root_dir).as_posix()}/terraform.tfstate".replace(
+                            "/base-", "/"
+                        ).replace("/tools-", "/")
+                    )
+
+                    in_container_file_path = (
+                        f"{self.paths.guest_base_path}/{config_tf_file.relative_to(self.paths.root_dir).as_posix()}"
+                    )
+                    resp = self.system_exec(
+                        "hcledit "
+                        f"-f {in_container_file_path} -u"
+                        f' attribute append terraform.backend.key "\\"{self._backend_key}\\""'
+                    )
             else:
                 if not skip_validation:
                     raise KeyError()
         except (KeyError, IndexError):
-            logger.error("[red]✘[/red] Malformed [bold]config.tf[/bold] file. Missing Terraform backend bucket key.")
+            logger.error(
+                "[red]✘[/red] Malformed [bold]config.tf[/bold] file. Missing Terraform backend block. In some cases you may want to skip this check by using the --skip-validation flag, e.g. the first time you initialize a terraform-backend layer."
+            )
             raise Exit(1)
         except Exception as e:
             logger.error("[red]✘[/red] Malformed [bold]config.tf[/bold] file. Unable to parse.")
             logger.debug(e)
             raise Exit(1)
 
-
     @property
     def backend_key(self):
         return self._backend_key
 
     @backend_key.setter
     def backend_key(self, backend_key):
         self._backend_key = backend_key
 
 
 class TFautomvContainer(TerraformContainer):
-    """ Leverage Container tailored to run general commands. """
-    TFAUTOMV_CLI_BINARY = '/usr/local/bin/tfautomv'
+    """Leverage Container tailored to run general commands."""
+
+    TFAUTOMV_CLI_BINARY = "/usr/local/bin/tfautomv"
 
     def __init__(self, client):
         super().__init__(client)
 
-        self.environment['TF_CLI_ARGS_init'] = ' '.join(self.tf_default_args)
-        self.environment['TF_CLI_ARGS_plan'] = ' '.join(self.tf_default_args)
+        self.environment["TF_CLI_ARGS_init"] = " ".join(self.tf_default_args)
+        self.environment["TF_CLI_ARGS_plan"] = " ".join(self.tf_default_args)
 
         self.entrypoint = self.TFAUTOMV_CLI_BINARY
 
         logger.debug(f"[bold cyan]Container configuration:[/bold cyan]\n{json.dumps(self.container_config, indent=2)}")
 
     def start(self, *arguments):
-        self._prepare_container()
-
-        return self._start('', *arguments)
+        with AwsCredsEntryPoint(self):
+            return self._start("", *arguments)
 
     def start_in_layer(self, *arguments):
-        """ Run a command that can only be performed in layer level. """
-        self.check_for_layer_location()
+        """Run a command that can only be performed in layer level."""
+        self.paths.check_for_layer_location()
 
         return self.start(*arguments)
 
     def exec(self, command, *arguments):
-        self._prepare_container()
-
-        return self._exec(command, *arguments)
-
+        with AwsCredsEntryPoint(self):
+            return self._exec(command, *arguments)
```

### Comparing `leverage-1.9.2/leverage/leverage.py` & `leverage-1.9.4rc1/leverage/leverage.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,34 @@
 import click
 
 from leverage import __version__
 from leverage.tasks import load_tasks
 from leverage.tasks import list_tasks as _list_tasks
 from leverage._internals import pass_state
 
-from leverage.modules import aws
-from leverage.modules import run
-from leverage.modules import project
-from leverage.modules import terraform
-from leverage.modules import credentials
-from leverage.modules import tfautomv
+from leverage.modules.aws import aws
+from leverage.modules.credentials import credentials
+from leverage.modules import run, project, terraform, tfautomv, kubectl, shell
+
 
 @click.group(invoke_without_command=True)
-@click.option("--filename", "-f",
-              default="build.py",
-              show_default=True,
-              help="Name of the build file containing the tasks definitions.")
-@click.option("--list-tasks", "-l",
-              is_flag=True,
-              help="List available tasks to run.")
-@click.option("-v", "--verbose",
-              is_flag=True,
-              help="Increase output verbosity.")
+@click.option(
+    "--filename",
+    "-f",
+    default="build.py",
+    show_default=True,
+    help="Name of the build file containing the tasks definitions.",
+)
+@click.option("--list-tasks", "-l", is_flag=True, help="List available tasks to run.")
+@click.option("-v", "--verbose", is_flag=True, help="Increase output verbosity.")
 @click.version_option(version=__version__)
 @pass_state
 @click.pass_context
 def leverage(context, state, filename, list_tasks, verbose):
-    """ Leverage Reference Architecture projects command-line tool. """
+    """Leverage Reference Architecture projects command-line tool."""
     # --verbose | -v
     state.verbosity = verbose
 
     # Load build file as a module
     state.module = load_tasks(build_script_filename=filename)
 
     if context.invoked_subcommand is None:
@@ -51,7 +48,10 @@
 leverage.add_command(run)
 leverage.add_command(project)
 leverage.add_command(terraform)
 leverage.add_command(terraform, name="tf")
 leverage.add_command(credentials)
 leverage.add_command(aws)
 leverage.add_command(tfautomv)
+leverage.add_command(kubectl)
+leverage.add_command(kubectl, name="kc")
+leverage.add_command(shell)
```

### Comparing `leverage-1.9.2/leverage/logger.py` & `leverage-1.9.4rc1/leverage/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,154 +5,178 @@
 from functools import wraps
 
 from rich.console import Console
 from rich.logging import RichHandler
 from click import get_current_context
 
 
-_TASK_LOGGING_FORMAT = ("[bold light_yellow3][ %(build_script)s -[/bold light_yellow3]"
-                        " %(message)s [bold light_yellow3]][/bold light_yellow3]")
+_RAW_LOGGING_FORMAT = "%(message)s"
+_TASK_LOGGING_FORMAT = (
+    "[bold light_yellow3][ %(build_script)s -[/bold light_yellow3]"
+    " %(message)s [bold light_yellow3]][/bold light_yellow3]"
+)
 _TIME_FORMAT = lambda time: f"[{time:%H:%M:%S}.{time.microsecond//1000:03}]"
 
 _leverage_logger = logging.getLogger("leverage")
 
 
 # Use the same console for the logging handler and any other special cases like
 # spinners, tables or progress bars.
 # TODO: Deprecate in favor of using rich's global console.
 console = Console()
 
 
 def get_script_log_level():
-    """ Get the verbosity level from the application state and map it to the Leverage scripts log level.
+    """Get the verbosity level from the application state and map it to the Leverage scripts log level.
     Logging level in the Leverage scripts is implemented as:
         ERROR = 1
         INFO = 2
         DEBUG = 3
 
     Returns:
         int: Logging level as defined in the Leverage scripts.
     """
     log_level = {
         logging.ERROR: 1,
         logging.INFO: 2,
-        logging.DEBUG: 3
+        logging.DEBUG: 3,
     }
 
     verbosity = get_current_context().obj.verbosity
     return log_level[verbosity]
 
 
 def get_verbosity(verbose):
-    """ Transform the given verbosity level into the corresponding logging level.
+    """Transform the given verbosity level into the corresponding logging level.
 
     Args:
         verbose (bool): Whether the logging should be verbose or not
 
     Returns:
         int: Logging level
     """
     return logging.DEBUG if verbose else logging.INFO
 
 
 def _configure_logger(logger, show_level=True):
-    """ Provide the given logger with the most basic configuration possible to be used.
+    """Provide the given logger with the most basic configuration possible to be used.
 
     Args:
         logger (logging.Logger): Logger to be configured
         show_level (bool): Whether to display the logging level in the record. Defaults to True
     """
     state = get_current_context().obj
 
     level = state.verbosity
     logger.setLevel(level)
 
     logger.propagate = False
 
-    handler = RichHandler(level=level,
-                          console=console,
-                          show_level=show_level,
-                          show_path=False,
-                          enable_link_path=False,
-                          markup=True,
-                          rich_tracebacks=True,
-                          tracebacks_show_locals=True,
-                          log_time_format=_TIME_FORMAT)
+    handler = RichHandler(
+        level=level,
+        console=console,
+        show_level=show_level,
+        show_path=False,
+        enable_link_path=False,
+        markup=True,
+        rich_tracebacks=True,
+        tracebacks_show_locals=True,
+        log_time_format=_TIME_FORMAT,
+    )
 
     logger.handlers = []
     logger.addHandler(handler)
 
 
 def initialize_logger(log_func):
-    """ Decorator to initialize the global logger before logging a message if it wasn't already initialized. """
+    """Decorator to initialize the global logger before logging a message if it wasn't already initialized."""
+
     @wraps(log_func)
     def wrapper(*args, **kwargs):
         if not _leverage_logger.handlers:
             _configure_logger(logger=_leverage_logger)
         log_func(*args, **kwargs)
 
     return wrapper
 
 
 @initialize_logger
-def debug(message): #pragma: no cover
-    """ Utility debug function to ease logging. """
+def debug(message):  # pragma: no cover
+    """Utility debug function to ease logging."""
     _leverage_logger.debug(message)
 
 
 @initialize_logger
-def info(message): #pragma: no cover
-    """ Utility info function to ease logging. """
+def info(message):  # pragma: no cover
+    """Utility info function to ease logging."""
     _leverage_logger.info(message)
 
 
 @initialize_logger
-def warning(message): #pragma: no cover
-    """ Utility warning function to ease logging. """
+def warning(message):  # pragma: no cover
+    """Utility warning function to ease logging."""
     _leverage_logger.warning(message)
 
 
 @initialize_logger
-def error(message): #pragma: no cover
-    """ Utility error function to ease logging. """
+def error(message):  # pragma: no cover
+    """Utility error function to ease logging."""
     _leverage_logger.error(message)
 
 
 @initialize_logger
-def critical(message): #pragma: no cover
-    """ Utility critical function to ease logging. """
+def critical(message):  # pragma: no cover
+    """Utility critical function to ease logging."""
     _leverage_logger.critical(message)
 
 
 @initialize_logger
-def exception(message, exc_info=False): #pragma: no cover
-    """ Utility exception function to ease logging. """
+def exception(message, exc_info=False):  # pragma: no cover
+    """Utility exception function to ease logging."""
     _leverage_logger.exception(message, exc_info=exc_info)
 
 
 class BuildFilter(logging.Filter):
-    """ Filter class to add additional info to a log record. """
+    """Filter class to add additional info to a log record."""
+
     def __init__(self):
         super().__init__()
         self._build_script = None
 
     def filter(self, record):
         if self._build_script is None:
             state = get_current_context().obj
             self._build_script = state.module.name
 
         record.build_script = self._build_script
         return True
 
 
 def get_tasks_logger():
-    """ Provide a logger specially configured to display the status of tasks execution. """
+    """Provide a logger specially configured to display the status of tasks execution."""
     logger = logging.getLogger("build")
     _configure_logger(logger=logger, show_level=False)
 
     logfilter = BuildFilter()
     logger.handlers[0].addFilter(logfilter)
 
     formatter = logging.Formatter(_TASK_LOGGING_FORMAT)
     logger.handlers[0].setFormatter(formatter)
 
     return logger
+
+
+def _raw_logger():
+    """
+    Provide a raw logger, in case we need to print stuff that already comes formatted (like some container logs).
+    """
+    logger = logging.getLogger("raw")
+    logger.setLevel(logging.INFO)
+    handler = logging.StreamHandler()
+    formatter = logging.Formatter(_RAW_LOGGING_FORMAT)
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+
+    return logger
+
+
+raw_logger = _raw_logger()
```

### Comparing `leverage-1.9.2/leverage/modules/aws.py` & `leverage-1.9.4rc1/leverage/modules/aws.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,206 +1,225 @@
-import webbrowser
-
+import boto3
 import click
 from click.exceptions import Exit
+from configupdater import ConfigUpdater
 
 from leverage import logger
 from leverage._internals import pass_state
 from leverage._internals import pass_container
-from leverage.container import get_docker_client
+from leverage._utils import get_or_create_section
+from leverage.container import get_docker_client, SSOContainer
 from leverage.container import AWSCLIContainer
+from leverage.modules.utils import _handle_subcommand
+
+CONTEXT_SETTINGS = {"ignore_unknown_options": True}
+
+
+def get_account_roles(sso_client, access_token: str) -> dict:
+    """
+    Fetch the accounts and roles from the user.
+    """
+    account_roles = {}
 
+    accounts = sso_client.list_accounts(accessToken=access_token)
+    for account in accounts["accountList"]:
+        acc_role = sso_client.list_account_roles(
+            accessToken=access_token,
+            accountId=account["accountId"],
+            maxResults=1,  # assume the first role is always the correct one
+        )["roleList"][0]
+
+        account_roles[account["accountName"]] = {
+            "account_id": account["accountId"],
+            "role_name": acc_role["roleName"],
+        }
+
+    return account_roles
+
+
+def add_sso_profile(
+    config_updater: ConfigUpdater, section_name: str, role_name: str, account_id: str, region: str, start_url: str
+):
+    """
+    Add a profile to the config file.
+    """
+    section = get_or_create_section(config_updater, section_name)
+
+    data = {
+        "role_name": role_name,
+        "account_id": account_id,
+        "sso_region": region,
+        "sso_start_url": start_url,
+    }
+    for k, v in data.items():
+        # can't set a dict directly, so we need to go field by field
+        section[k] = v
 
-def _handle_subcommand(context, cli_container, args, caller_name=None):
-    """ Decide if command corresponds to a wrapped one or not and run accordingly.
 
-    Args:
-        context (click.context): Current context
-        cli_container (AWSCLIContainer): Container where commands will be executed
-        args (tuple(str)): Arguments received by Leverage
-        caller_name (str, optional): Calling command. Defaults to None.
-
-    Raises:
-        Exit: Whenever container execution returns a non zero exit code
-    """
-    caller_pos = args.index(caller_name) if caller_name is not None else 0
-
-    # Find if one of the wrapped subcommand was invoked
-    wrapped_subcommands = context.command.commands.keys()
-    subcommand = next((arg
-                       for arg in args[caller_pos:]
-                       if arg in wrapped_subcommands), None)
-
-    if subcommand is None:
-        # Pass command to aws cli directly
-        exit_code = cli_container.start(" ".join(args))
-        if not exit_code:
-            raise Exit(exit_code)
-
-    else:
-        # Invoke wrapped command
-        subcommand = context.command.commands.get(subcommand)
-        if not subcommand.params:
-            context.invoke(subcommand)
-        else:
-            context.forward(subcommand)
-
-
-CONTEXT_SETTINGS={
-    "ignore_unknown_options": True
-}
-
-
-@click.group(invoke_without_command=True,
-             add_help_option=False,
-             context_settings=CONTEXT_SETTINGS)
+def configure_sso_profiles(cli: SSOContainer):
+    """
+    Populate the ~./aws/<project>/config file with the sso profiles from the accounts.
+    """
+    updater = ConfigUpdater()
+    updater.read(cli.paths.host_aws_profiles_file)
+
+    # get values from the default profile first
+    default_sso_profile_name = f"profile {cli.project}-sso"
+    default_profile = updater[default_sso_profile_name]
+    region = default_profile["sso_region"].value
+    start_url = default_profile["sso_start_url"].value
+
+    # then set a profile for each account
+    access_token = cli.get_sso_access_token()
+    logger.info(f"Fetching accounts and roles...")
+    client = boto3.client("sso", region_name=region)
+    account_roles = get_account_roles(client, access_token)
+    for acc_name, values in account_roles.items():
+        # account names comes in the form of: {long project name}-{account name}
+        short_acc_name = acc_name.replace(cli.paths.project_long + "-", "")
+        section_name = f"profile {cli.project}-sso-{short_acc_name}"
+        logger.info(f"Adding {section_name}")
+        add_sso_profile(updater, section_name, values["role_name"], values["account_id"], region, start_url)
+
+    # save/update the profile file
+    updater.update_file()
+
+
+@click.group(invoke_without_command=True, add_help_option=False, context_settings=CONTEXT_SETTINGS)
 @click.argument("args", nargs=-1, type=click.UNPROCESSED)
 @pass_state
 @click.pass_context
 def aws(context, state, args):
-    """ Run AWS CLI commands in a custom containerized environment. """
+    """Run AWS CLI commands in a custom containerized environment."""
     cli = AWSCLIContainer(get_docker_client())
     state.container = cli
     state.container.ensure_image()
 
     _handle_subcommand(context=context, cli_container=cli, args=args)
 
 
-@aws.group(invoke_without_command=True,
-           add_help_option=False,
-           context_settings=CONTEXT_SETTINGS)
+@aws.group(invoke_without_command=True, add_help_option=False, context_settings=CONTEXT_SETTINGS)
 @click.argument("args", nargs=-1, type=click.UNPROCESSED)
 @pass_container
 @click.pass_context
 def configure(context, cli, args):
-    """ configure """
+    """configure"""
     _handle_subcommand(context=context, cli_container=cli, args=args, caller_name="configure")
 
 
 @configure.command("sso")
 @pass_container
 @click.pass_context
 def _sso(context, cli):
-    """ configure sso """
-    if (cli.cwd in (cli.root_dir, cli.account_dir) or
-        cli.account_dir.parent != cli.root_dir or
-        not list(cli.cwd.glob("*.tf"))):
-        logger.error("SSO configuration can only be performed at [bold]layer[/bold] level.")
-        raise Exit(1)
+    """configure sso"""
+    cli.paths.check_for_layer_location()
 
     # region_primary was added in refarch v1
     # for v2 it was replaced by region at project level
-    region_primary = 'region_primary'
-    if not 'region_primary' in cli.common_conf:
-        region_primary = 'region'
-    default_region = cli.common_conf.get(region_primary, cli.common_conf.get("sso_region"))
+    region_primary = "region_primary"
+    if "region_primary" not in cli.paths.common_conf:
+        region_primary = "region"
+    default_region = cli.paths.common_conf.get(region_primary, cli.paths.common_conf.get("sso_region"))
     if default_region is None:
         logger.error("No primary region configured in global config file.")
         raise Exit(1)
 
     logger.info("Configuring default profile.")
-    default_profile = {
-        "region": default_region,
-        "output": "json"
-    }
+    default_profile = {"region": default_region, "output": "json"}
     for key, value in default_profile.items():
         cli.exec(f"configure set {key} {value}", profile="default")
 
-    if not all(sso_key in cli.common_conf for sso_key in ("sso_start_url", "sso_region")):
+    if not all(sso_key in cli.paths.common_conf for sso_key in ("sso_start_url", "sso_region")):
         logger.error("Missing configuration values for SSO in global config file.")
         raise Exit(1)
 
-    sso_role = cli.account_conf.get("sso_role")
+    sso_role = cli.paths.account_conf.get("sso_role")
     if not sso_role:
         logger.error("Missing SSO role in account config file.")
         raise Exit(1)
 
-    current_account = cli.account_conf.get("environment")
+    current_account = cli.paths.account_conf.get("environment")
     try:
         # this is for refarch v1
-        account_id = cli.common_conf.get("accounts").get(current_account).get("id")
+        account_id = cli.paths.common_conf.get("accounts").get(current_account).get("id")
     except AttributeError:
         # this is for refarch v2
         try:
             # this is for accounts with no org unit on top of it
-            account_id = cli.common_conf.get("organization").get("accounts").get(current_account).get("id")
+            account_id = cli.paths.common_conf.get("organization").get("accounts").get(current_account).get("id")
         except AttributeError:
             try:
                 # this is for accounts with no org unit on top of it
                 found = False
-                for ou in cli.common_conf.get("organization").get("organizational_units"):
-                    if current_account in cli.common_conf.get("organization").get("organizational_units").get(ou).get("accounts"):
-                        account_id = cli.common_conf.get("organization").get("organizational_units").get(ou).get("accounts").get(current_account).get("id")
+                for ou in cli.paths.common_conf.get("organization").get("organizational_units"):
+                    if current_account in cli.paths.common_conf.get("organization").get("organizational_units").get(
+                        ou
+                    ).get("accounts"):
+                        account_id = (
+                            cli.paths.common_conf.get("organization")
+                            .get("organizational_units")
+                            .get(ou)
+                            .get("accounts")
+                            .get(current_account)
+                            .get("id")
+                        )
                         found = True
                         break
                 if not found:
                     raise AttributeError
             except AttributeError:
                 logger.error(f"Missing account configuration for [bold]{current_account}[/bold] in global config file.")
                 raise Exit(1)
     if not account_id:
         logger.error(f"Missing id for account [bold]{current_account}[/bold].")
         raise Exit(1)
 
     logger.info(f"Configuring [bold]{cli.project}-sso[/bold] profile.")
     sso_profile = {
-        "sso_start_url": cli.common_conf.get("sso_start_url"),
-        "sso_region": cli.common_conf.get("sso_region", cli.common_conf.get(region_primary)),
+        "sso_start_url": cli.paths.common_conf.get("sso_start_url"),
+        "sso_region": cli.paths.common_conf.get("sso_region", cli.paths.common_conf.get(region_primary)),
         "sso_account_id": account_id,
-        "sso_role_name": sso_role
+        "sso_role_name": sso_role,
     }
     for key, value in sso_profile.items():
         cli.exec(f"configure set {key} {value}", profile=f"{cli.project}-sso")
 
     context.invoke(login)
 
     logger.info("Storing account information.")
-    exit_code = cli.system_start(cli.AWS_SSO_CONFIGURE_SCRIPT)
-    if exit_code:
-        raise Exit(exit_code)
+    configure_sso_profiles(cli)
 
 
-@aws.group(invoke_without_command=True,
-           add_help_option=False,
-           context_settings=CONTEXT_SETTINGS)
+@aws.group(invoke_without_command=True, add_help_option=False, context_settings=CONTEXT_SETTINGS)
 @click.argument("args", nargs=-1, type=click.UNPROCESSED)
 @pass_container
 @click.pass_context
 def sso(context, cli, args):
-    """ sso """
+    """sso"""
     _handle_subcommand(context=context, cli_container=cli, args=args, caller_name="sso")
 
 
 @sso.command()
 @pass_container
 def login(cli):
-    """ Login """
-    # only from account or layer directories
-    # when to fail:
-    # - when this cond meets:
-    #   - no account dir
-    #   - no layer dir
-    if not cli.get_location_type() in ['account', 'layer', 'layers-group']:
-        logger.error("SSO configuration can only be performed at [bold]layer[/bold] or [bold]account[/bold] level.")
-        raise Exit(1)
-
+    """Login"""
     exit_code, region = cli.exec(f"configure get sso_region --profile {cli.project}-sso")
     if exit_code:
         logger.error(f"Region configuration for [bold]{cli.project}-sso[/bold] profile not found.")
         raise Exit(1)
 
-    webbrowser.open_new_tab(cli.SSO_LOGIN_URL.format(region=region.strip()))
-    exit_code = cli.system_start(cli.AWS_SSO_LOGIN_SCRIPT)
-    if exit_code:
+    if exit_code := cli.sso_login():
         raise Exit(exit_code)
 
 
 @sso.command()
 @pass_container
 def logout(cli):
-    """ Logout """
+    """Logout"""
     exit_code = cli.system_start(cli.AWS_SSO_LOGOUT_SCRIPT)
     if exit_code:
         raise Exit(exit_code)
 
-    logger.info(f"Don't forget to log out of your [bold]AWS SSO[/bold] start page {cli.common_conf.get('sso_start_url')}"
-                " and your external identity provider portal.")
+    logger.info(
+        f"Don't forget to log out of your [bold]AWS SSO[/bold] start page {cli.paths.common_conf.get('sso_start_url')}"
+        " and your external identity provider portal."
+    )
```

### Comparing `leverage-1.9.2/leverage/modules/credentials.py` & `leverage-1.9.4rc1/leverage/modules/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 """
     Credentials managing module.
 """
-import re
 import csv
 import json
-from pathlib import Path
+import re
 from functools import wraps
+from pathlib import Path
 
 import click
-from click.exceptions import Exit
 import questionary
+from click.exceptions import Exit
 from questionary import Choice
 from ruamel.yaml import YAML
 
 from leverage import __toolbox_version__
 from leverage import logger
-from leverage.path import get_root_path
-from leverage.path import get_global_config_path
-from leverage.path import NotARepositoryError
 from leverage._internals import pass_state
-from leverage.container import get_docker_client
+from leverage._utils import ExitError
 from leverage.container import AWSCLIContainer
-
+from leverage.container import get_docker_client
+from leverage.path import NotARepositoryError
+from leverage.path import get_global_config_path
+from leverage.path import get_project_root_or_current_dir_path
 
 # Regexes for general validation
 PROJECT_SHORT = r"[a-z]{2,4}"
-USERNAME = r"[a-zA-Z0-9\+,=\.@\-_]{1,64}" # https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html#id_users_create_console
-                                          # https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreateUser.html#API_CreateUser_RequestParameters
+USERNAME = r"[a-zA-Z0-9\+,=\.@\-_]{1,64}"  # https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html#id_users_create_console
+# https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreateUser.html#API_CreateUser_RequestParameters
 KEY_ID = r"[A-Z0-9]{20}"
 SECRET_KEY = r"[a-zA-Z0-9/\+]{40}"
-REGION = (r"[a-z]{2}-[gov-]?"
-          r"(?:central|north|south|east|west|northeast|northwest|southeast|southwest|secret|topsecret)-[1-3]")
+REGION = (
+    r"[a-z]{2}-[gov-]?"
+    r"(?:central|north|south|east|west|northeast|northwest|southeast|southwest|secret|topsecret)-[1-3]"
+)
 ACCOUNT_ID = r"[0-9]{12}"
-MFA_SERIAL = fr"arn:aws:iam::{ACCOUNT_ID}:mfa/{USERNAME}"
+MFA_SERIAL = rf"arn:aws:iam::{ACCOUNT_ID}:mfa/{USERNAME}"
 
 # TODO: Remove these and get them into the global app state
+PROJECT_ROOT = get_project_root_or_current_dir_path()
 try:
     PROJECT_COMMON_TFVARS = Path(get_global_config_path())
-    PROJECT_ROOT = Path(get_root_path())
 except NotARepositoryError:
-    PROJECT_COMMON_TFVARS = PROJECT_ROOT = Path.cwd()
+    PROJECT_COMMON_TFVARS = Path.cwd()
 
 PROJECT_COMMON_TFVARS_FILE = "common.tfvars"
 PROJECT_COMMON_TFVARS = PROJECT_COMMON_TFVARS / PROJECT_COMMON_TFVARS_FILE
 PROJECT_CONFIG = PROJECT_ROOT / "project.yaml"
 AWSCLI_CONFIG_DIR = Path.home() / ".aws"
 
 PROFILES = {
@@ -57,20 +59,20 @@
         "profile_role": "oaar",
         "role": "OrganizationAccountAccessRole",
     },
     "security": {
         "choice_title": "DevOps credentials",
         "profile_role": "devops",
         "role": "DevOps",
-    }
+    },
 }
 
 
 def _exit_if_user_cancels_input(question):
-    """ Prompt user for input, exit application if user cancels it.
+    """Prompt user for input, exit application if user cancels it.
 
     Args:
         question (callable): Question to be asked to user.
 
     Raises:
         Exit: When user cancels input.
 
@@ -86,138 +88,139 @@
         return answer
 
     return handle_keyboard_interrupt
 
 
 @_exit_if_user_cancels_input
 def _ask_for_short_name():
-    """ Prompt for project short name.
+    """Prompt for project short name.
 
     Returns:
         str: Project short name.
     """
     return questionary.text(
         message="Project short name:",
         qmark=">",
-        validate=lambda value: bool(re.fullmatch(PROJECT_SHORT, value)) or "The project short name should be a two letter lowercase word"
+        validate=lambda value: bool(re.fullmatch(PROJECT_SHORT, value))
+        or "The project short name should be a two letter lowercase word",
     ).ask()
 
 
 @_exit_if_user_cancels_input
 def _ask_for_region():
-    """ Prompt for region.
+    """Prompt for region.
 
     Returns:
         str: Region.
     """
     return questionary.text(
         message="Credentials default region:",
         qmark=">",
         default="us-east-1",
-        validate=lambda value: bool(re.fullmatch(REGION, value)) or "Invalid region."
+        validate=lambda value: bool(re.fullmatch(REGION, value)) or "Invalid region.",
     ).ask()
 
 
 @_exit_if_user_cancels_input
 def _ask_for_credentials_overwrite(profile, skip_option_title, overwrite_option_title):
-    """ Prompt user with options regarding already existing credentials, whether to
+    """Prompt user with options regarding already existing credentials, whether to
     skip their configuration or overwrite them.
 
     Args:
         profile (str): Name of the profile being configured.
         skip_option_title (str): Message to display in the `skip` option.
         overwrite_option_title (str): Message to display in the `overwrite` option.
 
     Returns:
         bool: Whether to overwrite the current credentials or not.
     """
     return questionary.select(
         message=f"Credentials already configured for {profile}:",
         qmark=">",
         choices=[
-            Choice(skip_option_title,
-                   value=False,
-                   shortcut_key="s",
-                   checked=True),
-            Choice(overwrite_option_title,
-                   value=True,
-                   shortcut_key="o")
+            Choice(skip_option_title, value=False, shortcut_key="s", checked=True),
+            Choice(overwrite_option_title, value=True, shortcut_key="o"),
         ],
-        use_shortcuts=True
+        use_shortcuts=True,
     ).ask()
 
 
 @_exit_if_user_cancels_input
 def _ask_for_credentials_location():
-    """ Prompt for credential input method and location if path is selected.
+    """Prompt for credential input method and location if path is selected.
 
     Returns:
         Path | str: Path to location or `manual` if `Manual` is selected.
     """
-    location = questionary.prompt([
-        {
-            "type": "select",
-            "name": "input_type",
-            "message": "Select the means by which you'll provide the programatic keys:",
-            "qmark": ">",
-            "choices": [
-                {"name": "Path to an access keys file obtained from AWS", "value": "path"},
-                {"name": "Manually", "value": "manual"}
-            ]
-        },
-        {
-            "type": "path",
-            "name": "path",
-            "message": "Path to access keys file:",
-            "qmark": ">",
-            "when": lambda qs: qs["input_type"] == "path",
-            "validate": lambda value: (Path(value).expanduser().is_file() and Path(value).expanduser().exists()) or "Path must be an existing file"
-        }
-    ])
+    location = questionary.prompt(
+        [
+            {
+                "type": "select",
+                "name": "input_type",
+                "message": "Select the means by which you'll provide the programatic keys:",
+                "qmark": ">",
+                "choices": [
+                    {"name": "Path to an access keys file obtained from AWS", "value": "path"},
+                    {"name": "Manually", "value": "manual"},
+                ],
+            },
+            {
+                "type": "path",
+                "name": "path",
+                "message": "Path to access keys file:",
+                "qmark": ">",
+                "when": lambda qs: qs["input_type"] == "path",
+                "validate": lambda value: (Path(value).expanduser().is_file() and Path(value).expanduser().exists())
+                or "Path must be an existing file",
+            },
+        ]
+    )
     if not location:
         return
 
     input_type = location.get("input_type")
     return Path(location.get("path")).expanduser() if input_type == "path" else input_type
 
 
 @_exit_if_user_cancels_input
 def _ask_for_credentials():
-    """ Prompt for key id and secret keys.
+    """Prompt for key id and secret keys.
 
     Returns:
         str, str: Kei ID, Secret Key
     """
-    credentials = questionary.prompt([
-        {
-            "type": "text",
-            "name": "key_id",
-            "message": "Key:",
-            "qmark": ">",
-            "validate": lambda value: bool(re.fullmatch(KEY_ID, value)) or "Invalid Key"
-        },
-        {
-            "type": "password",
-            "name": "secret_key",
-            "message": "Secret:",
-            "qmark": ">",
-            "validate": lambda value: bool(re.fullmatch(SECRET_KEY, value)) or "Invalid Secret",
-        }
-    ])
+    credentials = questionary.prompt(
+        [
+            {
+                "type": "text",
+                "name": "key_id",
+                "message": "Key:",
+                "qmark": ">",
+                "validate": lambda value: bool(re.fullmatch(KEY_ID, value)) or "Invalid Key",
+            },
+            {
+                "type": "password",
+                "name": "secret_key",
+                "message": "Secret:",
+                "qmark": ">",
+                "validate": lambda value: bool(re.fullmatch(SECRET_KEY, value)) or "Invalid Secret",
+            },
+        ]
+    )
     if not credentials:
         return
 
     return list(credentials.values())
 
 
 AWSCLI = None
 
 
 def _load_project_yaml():
-    """ Load project.yaml file contents. """
+    """Load project.yaml file contents."""
     if not PROJECT_CONFIG.exists():
         logger.debug("No project config file found.")
         return {}
 
     try:
         return YAML().load(PROJECT_CONFIG)
 
@@ -226,15 +229,15 @@
         logger.exception(message="Error loading configuration file.", exc_info=exc)
         raise Exit(1)
 
 
 @click.group()
 @pass_state
 def credentials(state):
-    """ Manage AWS cli credentials. """
+    """Manage AWS cli credentials."""
 
     """
     Scenarios on project.yaml, build.env and common.tfvars files:
     - if project is new project.yaml exists and build.env/common.tfvars don't
     - if project is already started is likely project.yaml won't exist but build.env or common.tfvars do
 
     In any case one of them should exist. E.g.
@@ -247,57 +250,57 @@
         else:
             if common.tfvars
             raise an exception
 
     If we reached the only common.tfvars scenario, we have no project name nor TERRAFORM_IMAGE_TAG.
     So the best chance is to read the common.tfvars directly without a conatiner, e.g. with sed or grep
     """
-    project_config =  _load_project_yaml()
+    project_config = _load_project_yaml()
     build_env = Path(f"{PROJECT_ROOT}/build.env")
 
     if project_config != {}:
-        logger.info('Reading info from project.yaml')
+        logger.info("Reading info from project.yaml")
         # project_config is not empty
         short_name = project_config.get("short_name")
         if short_name is None or not re.match("^[a-z]{2,4}$", short_name):
             logger.error("Invalid or missing project short name in project.yaml file.")
             raise Exit(1)
         if not build_env.exists():
             build_env.write_text(f"PROJECT={short_name}\nTERRAFORM_IMAGE_TAG={__toolbox_version__}")
     elif not build_env.exists():
         # project_config is not empty
         # and build.env does not exist
         # trying common.tfvars
         try:
             found = False
-            with open(PROJECT_COMMON_TFVARS,"r") as file:
-                r=r'project = "(.+)"'
+            with open(PROJECT_COMMON_TFVARS, "r") as file:
+                r = r'project = "(.+)"'
                 for line in file:
                     g = re.search(r, line)
                     if g:
                         found = True
-                        logger.info('Reading info from common.tfvars')
+                        logger.info("Reading info from common.tfvars")
                         build_env.write_text(f"PROJECT={g[1]}\nTERRAFORM_IMAGE_TAG=1.1.9")
                         break
             if not found:
-                raise Exception('Config file not found')
+                raise Exception("Config file not found")
         except Exception as e:
             logger.error(f"Neither project.yaml nor build.env nor common.tfvars files were found. {e}")
             raise Exit(1)
     else:
-        logger.info('Reading info from build.env')
-
+        logger.info("Reading info from build.env")
 
     state.container = AWSCLIContainer(get_docker_client())
     state.container.ensure_image()
     global AWSCLI
     AWSCLI = state.container
 
+
 def _load_configs_for_credentials():
-    """ Load all required values to configure credentials.
+    """Load all required values to configure credentials.
 
     Raises:
         Exit: If no project has been already initialized in the system.
 
     Returns:
         dict: Values needed to configure a credential and update the files accordingly.
     """
@@ -305,75 +308,75 @@
     project_config = _load_project_yaml()
 
     logger.info("Loading project environment configuration file.")
     env_config = AWSCLI.env_conf
 
     terraform_config = {}
     logger.info("Loading Terraform common configuration.")
-    terraform_config = AWSCLI.common_conf
+    terraform_config = AWSCLI.paths.common_conf
 
     config_values = {}
-    config_values["short_name"] = (project_config.get("short_name")
-                                       or env_config.get("PROJECT")
-                                       or terraform_config.get("project")
-                                       or _ask_for_short_name())
-    config_values["project_name"] = (project_config.get("project_name")
-                                         or terraform_config.get("project_long"))
+    config_values["short_name"] = (
+        project_config.get("short_name")
+        or env_config.get("PROJECT")
+        or terraform_config.get("project")
+        or _ask_for_short_name()
+    )
+    config_values["project_name"] = project_config.get("project_name") or terraform_config.get("project_long")
 
     # region_primary was added in refarch v1
     # for v2 it was replaced by region at project level
-    region_primary = 'region_primary'
-    if not 'region_primary' in project_config and not 'region_primary' in terraform_config:
-        region_primary = 'region'
-    config_values["primary_region"] = (project_config.get(region_primary)
-                                           or terraform_config.get(region_primary)
-                                           or _ask_for_region())
+    region_primary = "region_primary"
+    if not "region_primary" in project_config and not "region_primary" in terraform_config:
+        region_primary = "region"
+    config_values["primary_region"] = (
+        project_config.get(region_primary) or terraform_config.get(region_primary) or _ask_for_region()
+    )
     config_values["secondary_region"] = terraform_config.get("region_secondary")
 
     config_values["organization"] = {"accounts": []}
     # Accounts defined in Terraform code take priority
     terraform_accounts = terraform_config.get("accounts", {})
     if terraform_accounts:
-        config_values["organization"]["accounts"].extend([
-            {
-                "name": account_name,
-                "email": account_info.get("email"),
-                "id": account_info.get("id")
-            }
-            for account_name, account_info in terraform_accounts.items()
-        ])
+        config_values["organization"]["accounts"].extend(
+            [
+                {"name": account_name, "email": account_info.get("email"), "id": account_info.get("id")}
+                for account_name, account_info in terraform_accounts.items()
+            ]
+        )
     # Add accounts not found in terraform code
     project_accounts = [
-        account for account in project_config.get("organization", {}).get("accounts", [])
+        account
+        for account in project_config.get("organization", {}).get("accounts", [])
         if account.get("name") not in terraform_accounts
     ]
     if project_accounts:
         config_values["organization"]["accounts"].extend(project_accounts)
 
     config_values["mfa_enabled"] = env_config.get("MFA_ENABLED", "false")
 
     return config_values
 
 
 def _profile_is_configured(profile):
-    """ Check if given profile is already configured.
+    """Check if given profile is already configured.
 
     Args:
         profile (str): Profile to check.
 
     Returns:
         bool: Whether the profile was already configured or not.
     """
     exit_code, _ = AWSCLI.exec("configure list", profile)
 
     return not exit_code
 
 
 def _extract_credentials(file):
-    """ Extract AWS credentials from given file. Print message and quit application if file is malformed.
+    """Extract AWS credentials from given file. Print message and quit application if file is malformed.
     Access Keys files have the form:
        Access key ID,Secret access key
        AKUDKXXXXXXXXXXXXXXX,examplesecreteLkyvWWjxi29dJ63Geo1Ggl956b
 
     Args:
         file (Path): Credentials file as obtained from AWS Console.
 
@@ -403,30 +406,27 @@
         click.echo("\nMalformed keys in access keys file\n")
         raise Exit(1)
 
     return access_key_id, secret_access_key
 
 
 def _backup_file(filename):
-    """ Create backup of a credential file using docker image.
+    """Create backup of a credential file using docker image.
 
     Args:
         filename (str): File to backup, either `config` or `credentials`
     """
-    credential_files_env_vars = {
-        "config": "AWS_CONFIG_FILE",
-        "credentials": "AWS_SHARED_CREDENTIALS_FILE"
-    }
+    credential_files_env_vars = {"config": "AWS_CONFIG_FILE", "credentials": "AWS_SHARED_CREDENTIALS_FILE"}
     env_var = credential_files_env_vars.get(filename)
 
     AWSCLI.system_exec(f"sh -c 'cp ${env_var} \"${{{env_var}}}.bkp\"'")
 
 
 def configure_credentials(profile, file=None, make_backup=False):
-    """ Set credentials in `credentials` file for AWS cli. Make backup if required.
+    """Set credentials in `credentials` file for AWS cli. Make backup if required.
 
     Args:
         profile (str): Name of the profile to configure.
         file (Path, optional): Credentials file. Defaults to None.
         make_backup (bool, optional): Whether to make a backup of the credentials file. Defaults to False.
     """
     file = file or _ask_for_credentials_location()
@@ -437,28 +437,24 @@
     else:
         key_id, secret_key = _ask_for_credentials()
 
     if make_backup:
         logger.info("Backing up credentials file.")
         _backup_file("credentials")
 
-    values = {
-        "aws_access_key_id": key_id,
-        "aws_secret_access_key": secret_key
-    }
+    values = {"aws_access_key_id": key_id, "aws_secret_access_key": secret_key}
 
     for key, value in values.items():
         exit_code, output = AWSCLI.exec(f"configure set {key} {value}", profile)
         if exit_code:
-            logger.error(f"AWS CLI error: {output}")
-            raise Exit(exit_code)
+            raise ExitError(exit_code, f"AWS CLI error: {output}")
 
 
 def _credentials_are_valid(profile):
-    """ Check if credentials for given profile are valid.
+    """Check if credentials for given profile are valid.
     If credentials are invalid, the command output will be as follows:
     Exit code:
         255
     Error message:
         An error occurred (InvalidClientTokenId) when calling the GetCallerIdentity operation:
         The security token included in the request is invalid.
 
@@ -470,33 +466,32 @@
     """
     error_code, output = AWSCLI.exec("sts get-caller-identity", profile)
 
     return error_code != 255 and "InvalidClientTokenId" not in output
 
 
 def _get_management_account_id(profile):
-    """ Get management account id through AWS cli.
+    """Get management account id through AWS cli.
 
     Args:
         profile (str): Name of profile to configure.
 
     Returns:
         str: Management account id.
     """
     exit_code, caller_identity = AWSCLI.exec("--output json sts get-caller-identity", profile)
     if exit_code:
-        logger.error(f"AWS CLI error: {caller_identity}")
-        raise Exit(exit_code)
+        raise ExitError(exit_code, f"AWS CLI error: {caller_identity}")
 
     caller_identity = json.loads(caller_identity)
     return caller_identity["Account"]
 
 
 def _get_organization_accounts(profile, project_name):
-    """ Get organization accounts names and ids. Removing the prefixed project name from the account names.
+    """Get organization accounts names and ids. Removing the prefixed project name from the account names.
 
     Args:
         profile (str): Credentials profile.
         project_name (str): Full name of the project.
 
     Returns:
         dict: Mapping of organization accounts names to ids.
@@ -508,75 +503,79 @@
 
     organization_accounts = json.loads(organization_accounts)["Accounts"]
 
     prefix = f"{project_name}-"
     accounts = {}
     for account in organization_accounts:
         name = account["Name"]
-        name = name[len(prefix):] if name.startswith(prefix) else name
+        name = name[len(prefix) :] if name.startswith(prefix) else name
         accounts[name] = account["Id"]
 
     return accounts
 
 
 def _get_mfa_serial(profile):
-    """ Get MFA serial for the given profile credentials.
+    """Get MFA serial for the given profile credentials.
 
     Args:
         profile (str): Name of profile.
 
     Returns:
         str: MFA device serial.
     """
     exit_code, mfa_devices = AWSCLI.exec("--output json iam list-mfa-devices", profile)
     if exit_code:
-        logger.error(f"AWS CLI error: {mfa_devices}")
-        raise Exit(exit_code)
+        raise ExitError(exit_code, f"AWS CLI error: {mfa_devices}")
     mfa_devices = json.loads(mfa_devices)
 
     # Either zero or one MFA device should be configured for either `management` or `security` accounts users.
     # Just for safety, and because we only support VirtualMFA devices, we check that the `SerialNumber` is an `arn`
     # https://docs.aws.amazon.com/IAM/latest/APIReference/API_MFADevice.html
-    return next((device["SerialNumber"] for device in mfa_devices["MFADevices"] if re.fullmatch(MFA_SERIAL, device["SerialNumber"])), "")
+    return next(
+        (
+            device["SerialNumber"]
+            for device in mfa_devices["MFADevices"]
+            if re.fullmatch(MFA_SERIAL, device["SerialNumber"])
+        ),
+        "",
+    )
 
 
 def configure_profile(profile, values):
-    """ Set profile in `config` file for AWS cli.
+    """Set profile in `config` file for AWS cli.
 
     Args:
         profile (str): Profile name.
         values (dict): Mapping of values to be set in the profile.
     """
     logger.info(f"\tConfiguring profile [bold]{profile}[/bold]")
     for key, value in values.items():
         exit_code, output = AWSCLI.exec(f"configure set {key} {value}", profile)
         if exit_code:
-            logger.error(f"AWS CLI error: {output}")
-            raise Exit(exit_code)
+            raise ExitError(exit_code, f"AWS CLI error: {output}")
 
 
 def configure_accounts_profiles(profile, region, organization_accounts, project_accounts, fetch_mfa_device):
-    """ Set up the required profiles for all accounts to be used with AWS cli. Backup previous profiles.
+    """Set up the required profiles for all accounts to be used with AWS cli. Backup previous profiles.
 
     Args:
         profile(str): Name of the profile to configure.
         region (str): Region.
         organization_accounts (dict): Name and id of all accounts in the organization.
-        project_accounts (dict): Name and email of all accounts in project configuration file.
+        project_accounts (list): Name and email of all accounts in project configuration file.
         fetch_mfa_device (bool): Whether to fetch MFA device for profiles.
     """
-    short_name, type = profile.split("-")
+    short_name, _type = profile.split("-")
 
     mfa_serial = ""
     if fetch_mfa_device:
         logger.info("Fetching MFA device serial.")
         mfa_serial = _get_mfa_serial(profile)
         if not mfa_serial:
-            logger.error("No MFA device found for user.")
-            raise Exit(1)
+            raise ExitError(1, "No MFA device found for user.")
 
     account_profiles = {}
     for account in project_accounts:
         account_name = account["name"]
         # DevOps roles do not have permission over management account
         if "security" in profile and account_name == "management":
             continue
@@ -585,31 +584,31 @@
         account_id = organization_accounts.get(account_name, account.get("id"))
         if account_id is None:
             continue
 
         account_profile = {
             "output": "json",
             "region": region,
-            "role_arn": f"arn:aws:iam::{account_id}:role/{PROFILES[type]['role']}",
-            "source_profile": profile
+            "role_arn": f"arn:aws:iam::{account_id}:role/{PROFILES[_type]['role']}",
+            "source_profile": profile,
         }
         if mfa_serial:
             account_profile["mfa_serial"] = mfa_serial
         # A profile identifier looks like `le-security-oaar`
-        account_profiles[f"{short_name}-{account_name}-{PROFILES[type]['profile_role']}"] = account_profile   
+        account_profiles[f"{short_name}-{account_name}-{PROFILES[_type]['profile_role']}"] = account_profile
 
     logger.info("Backing up account profiles file.")
     _backup_file("config")
 
     for profile_identifier, profile_values in account_profiles.items():
         configure_profile(profile_identifier, profile_values)
 
 
 def _update_account_ids(config):
-    """ Update accounts ids in global configuration file.
+    """Update accounts ids in global configuration file.
     It updates both `[account name]_account_id` and `accounts` variables.
     This last one maintaning the format:
     ```
     account = {
       account_name = {
         email = account_email,
         id = account_id
@@ -626,79 +625,92 @@
     container_base_dir = f"/{config['project_name']}/config"
     container_common_tfvars_file = f"{container_base_dir}/{PROJECT_COMMON_TFVARS_FILE}"
 
     accs = []
     for account in config["organization"]["accounts"]:
         acc_name, acc_email, acc_id = account.values()
 
-        acc = [f"\n    email = \"{acc_email}\""]
+        acc = [f'\n    email = "{acc_email}"']
         if acc_id:
-            AWSCLI.system_exec("hcledit "
-                               f"-f {container_common_tfvars_file} -u"
-                               f" attribute set {acc_name}_account_id \"\\\"{acc_id}\\\"\"")
+            AWSCLI.system_exec(
+                "hcledit "
+                f"-f {container_common_tfvars_file} -u"
+                f' attribute set {acc_name}_account_id "\\"{acc_id}\\""'
+            )
 
-            acc.append(f"    id = \"{acc_id}\"")
+            acc.append(f'    id = "{acc_id}"')
         acc = ",\n".join(acc)
 
         accs.append(f"\n  {acc_name} = {{{acc}\n  }}")
 
     accs = ",".join(accs)
     accs = f"{{{accs}\n}}"
 
-    AWSCLI.system_exec("hcledit "
-                       f"-f {container_common_tfvars_file} -u"
-                       f" attribute set accounts '{accs}'")
+    AWSCLI.system_exec("hcledit " f"-f {container_common_tfvars_file} -u" f" attribute set accounts '{accs}'")
 
 
 def mutually_exclusive(context, param, value):
-    """ Callback for command options --overwrite-existing-credentials and --skip-access-keys-setup mutual exclusivity verification. """
+    """Callback for command options --overwrite-existing-credentials and --skip-access-keys-setup mutual exclusivity verification."""
     me_option = {
         "overwrite_existing_credentials": "skip_access_keys_setup",
-        "skip_access_keys_setup": "overwrite_existing_credentials"
+        "skip_access_keys_setup": "overwrite_existing_credentials",
     }
 
     if value and context.params.get(me_option[param.name], False):
-        raise click.BadOptionUsage(option_name=param,
-                                   message=(f"Option {param.opts[0]} is mutually exclusive"
-                                            f" with option --{me_option[param.name].replace('_', '-')}."),
-                                   ctx=context)
+        raise click.BadOptionUsage(
+            option_name=param,
+            message=(
+                f"Option {param.opts[0]} is mutually exclusive"
+                f" with option --{me_option[param.name].replace('_', '-')}."
+            ),
+            ctx=context,
+        )
 
     return value
 
 
 @credentials.command()
-@click.option("--type",
-              type=click.Choice(["BOOTSTRAP",
-                                 "MANAGEMENT",
-                                 "SECURITY"],
-                                case_sensitive=False),
-              required=True,
-              help="Type of credentials to set.")
-@click.option("--credentials-file",
-              type=click.Path(exists=True, path_type=Path),
-              help="Path to AWS cli credentials file.")
-@click.option("--fetch-mfa-device",
-              is_flag=True,
-              help="Fetch MFA device configured for user.")
-@click.option("--overwrite-existing-credentials",
-              is_flag=True,
-              callback=mutually_exclusive,
-              help=("Overwrite existing credentials if already configured.\n"
-                    "Mutually exclusive with --skip-access-keys-setup."))
-@click.option("--skip-access-keys-setup",
-              is_flag=True,
-              callback=mutually_exclusive,
-              help=("Skip access keys configuration. Continue on with assumable roles setup.\n"
-                    "Mutually exclusive with --overwrite-existing-credentials."))
-@click.option("--skip-assumable-roles-setup",
-              is_flag=True,
-              help="Don't configure the accounts assumable roles.")
+@click.option(
+    "--type",
+    type=click.Choice(["BOOTSTRAP", "MANAGEMENT", "SECURITY"], case_sensitive=False),
+    required=True,
+    help="Type of credentials to set.",
+)
+@click.option(
+    "--credentials-file", type=click.Path(exists=True, path_type=Path), help="Path to AWS cli credentials file."
+)
+@click.option("--fetch-mfa-device", is_flag=True, help="Fetch MFA device configured for user.")
+@click.option(
+    "--overwrite-existing-credentials",
+    is_flag=True,
+    callback=mutually_exclusive,
+    help=(
+        "Overwrite existing credentials if already configured.\n" "Mutually exclusive with --skip-access-keys-setup."
+    ),
+)
+@click.option(
+    "--skip-access-keys-setup",
+    is_flag=True,
+    callback=mutually_exclusive,
+    help=(
+        "Skip access keys configuration. Continue on with assumable roles setup.\n"
+        "Mutually exclusive with --overwrite-existing-credentials."
+    ),
+)
+@click.option("--skip-assumable-roles-setup", is_flag=True, help="Don't configure the accounts assumable roles.")
 # TODO: Add --override-role-name parameter for non-default roles in accounts
-def configure(type, credentials_file, fetch_mfa_device, overwrite_existing_credentials, skip_access_keys_setup, skip_assumable_roles_setup):
-    """ Configure credentials for the project.
+def configure(
+    type,
+    credentials_file,
+    fetch_mfa_device,
+    overwrite_existing_credentials,
+    skip_access_keys_setup,
+    skip_assumable_roles_setup,
+):
+    """Configure credentials for the project.
 
     It can handle the credentials required for the initial deployment of the project (BOOTSTRAP),
     a management user (MANAGEMENT) or a devops/secops user (SECURITY).
     """
     if skip_access_keys_setup and skip_assumable_roles_setup:
         logger.info("Nothing to do. Exiting.")
         return
@@ -712,37 +724,41 @@
     already_configured = _profile_is_configured(profile=profile)
     if already_configured and not (skip_access_keys_setup or overwrite_existing_credentials):
         title_extra = "" if skip_assumable_roles_setup else " Continue on with assumable roles setup."
 
         overwrite_existing_credentials = _ask_for_credentials_overwrite(
             profile=profile,
             skip_option_title=f"Skip credentials configuration.{title_extra}",
-            overwrite_option_title="Overwrite current credentials. Backups will be made."
+            overwrite_option_title="Overwrite current credentials. Backups will be made.",
         )
 
-    do_configure_credentials = False if skip_access_keys_setup else overwrite_existing_credentials or not already_configured
+    do_configure_credentials = (
+        False if skip_access_keys_setup else overwrite_existing_credentials or not already_configured
+    )
 
     if do_configure_credentials:
         logger.info(f"Configuring [bold]{type}[/bold] credentials.")
         configure_credentials(profile, credentials_file, make_backup=already_configured)
-        logger.info(f"[bold]{type.capitalize()} credentials configured in:[/bold]"
-                    f" {(AWSCLI_CONFIG_DIR / short_name / 'credentials').as_posix()}")
+        logger.info(
+            f"[bold]{type.capitalize()} credentials configured in:[/bold]"
+            f" {(AWSCLI_CONFIG_DIR / short_name / 'credentials').as_posix()}"
+        )
 
         if not _credentials_are_valid(profile):
             logger.error(f"Invalid {profile} credentials. Please check the given keys.")
             return
 
     accounts = config_values.get("organization", {}).get("accounts", False)
     # First time configuring bootstrap credentials
     if type == "bootstrap" and not already_configured:
         management_account = next((account for account in accounts if account["name"] == "management"), None)
 
         if management_account:
             logger.info("Fetching management account id.")
-            management_account_id =_get_management_account_id(profile=profile)
+            management_account_id = _get_management_account_id(profile=profile)
             management_account["id"] = management_account_id
 
             project_config_file = _load_project_yaml()
             if project_config_file and "accounts" in project_config_file.get("organization", {}):
                 project_config_file["organization"]["accounts"] = accounts
 
                 logger.info("Updating project configuration file.")
@@ -761,29 +777,34 @@
                 break
 
     if skip_assumable_roles_setup:
         logger.info("Skipping assumable roles configuration.")
 
     else:
         logger.info("Attempting to fetch organization accounts.")
-        organization_accounts = _get_organization_accounts(profile_for_organization,
-                                                           config_values.get("project_name"))
+        organization_accounts = _get_organization_accounts(profile_for_organization, config_values.get("project_name"))
         logger.debug(f"Organization Accounts fetched: {organization_accounts}")
 
         if organization_accounts or accounts:
             logger.info("Configuring assumable roles.")
 
-            configure_accounts_profiles(profile, config_values["primary_region"], organization_accounts, accounts, fetch_mfa_device)
-            logger.info(f"[bold]Account profiles configured in:[/bold]"
-                        f" {(AWSCLI_CONFIG_DIR / short_name / 'config').as_posix()}")
+            configure_accounts_profiles(
+                profile, config_values["primary_region"], organization_accounts, accounts, fetch_mfa_device
+            )
+            logger.info(
+                f"[bold]Account profiles configured in:[/bold]"
+                f" {(AWSCLI_CONFIG_DIR / short_name / 'config').as_posix()}"
+            )
 
             for account in accounts:
-                try: # Some account may not already be created
+                try:  # Some account may not already be created
                     account["id"] = organization_accounts[account["name"]]
                 except KeyError:
                     continue
 
         else:
-            logger.info("No organization has been created yet or no accounts were configured.\n"
-                        "Skipping assumable roles configuration.")
+            logger.info(
+                "No organization has been created yet or no accounts were configured.\n"
+                "Skipping assumable roles configuration."
+            )
 
     _update_account_ids(config=config_values)
```

### Comparing `leverage-1.9.2/leverage/modules/project.py` & `leverage-1.9.4rc1/leverage/modules/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,85 @@
 """
     Module for managing Leverage projects.
 """
+import re
 from pathlib import Path
 from shutil import copy2
 from shutil import copytree
 from shutil import ignore_patterns
 
 import click
 from click.exceptions import Exit
 from ruamel.yaml import YAML
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
 
 from leverage import __toolbox_version__
 from leverage import logger
 from leverage.logger import console
-from leverage.path import get_root_path
+from leverage.path import get_root_path, get_project_root_or_current_dir_path
 from leverage.path import NotARepositoryError
-from leverage._utils import git
+from leverage._utils import git, ExitError
 from leverage.container import get_docker_client
 from leverage.container import TerraformContainer
 
 # Leverage related base definitions
 LEVERAGE_DIR = Path.home() / ".leverage"
 TEMPLATES_REPO_DIR = LEVERAGE_DIR / "templates"
 TEMPLATE_DIR = TEMPLATES_REPO_DIR / "template"
 PROJECT_CONFIG_FILE = "project.yaml"
 TEMPLATE_PATTERN = "*.template"
 CONFIG_FILE_TEMPLATE = TEMPLATES_REPO_DIR / "le-resources" / PROJECT_CONFIG_FILE
 LEVERAGE_TEMPLATE_REPO = "https://github.com/binbashar/le-tf-infra-aws-template.git"
 IGNORE_PATTERNS = ignore_patterns(TEMPLATE_PATTERN, ".gitkeep")
 
 # Useful project related definitions
-try:
-    PROJECT_ROOT = Path(get_root_path())
-except NotARepositoryError:
-    PROJECT_ROOT = Path.cwd()
+PROJECT_ROOT = get_project_root_or_current_dir_path()
 PROJECT_CONFIG = PROJECT_ROOT / PROJECT_CONFIG_FILE
 
 CONFIG_DIRECTORY = "config"
 
 # TODO: Keep this structure in the project's directory
 PROJECT_STRUCTURE = {
     "management": {
         "global": [
-            "base-identities",
-            "organizations"
+            "organizations",
+            "sso",
         ],
         "primary_region": [
             "base-tf-backend",
-            "security-base"
-        ]
+            "security-base",
+        ],
     },
     "security": {
-        "global": [
-            "base-identities"
-        ],
+        "global": [],
         "primary_region": [
             "base-tf-backend",
-            "security-base"
-        ]
+            "security-base",
+        ],
     },
     "shared": {
-        "global": [
-            "base-identities"
-        ],
+        "global": [],
         "primary_region": [
             "base-network",
             "base-tf-backend",
-            "security-base"
-        ]
-    }
+            "security-base",
+        ],
+    },
 }
 
 
 @click.group()
 def project():
-    """ Manage a Leverage project. """
+    """Manage a Leverage project."""
 
 
 @project.command()
 def init():
-    """ Initializes and gets all the required resources to be able to create a new Leverage project. """
+    """Initializes and gets all the required resources to be able to create a new Leverage project."""
 
     # Application's directory
     if not LEVERAGE_DIR.exists():
         logger.info("No [bold]Leverage[/bold] config directory found in user's home. Creating.")
         LEVERAGE_DIR.mkdir()
 
     # Leverage project templates
@@ -105,117 +99,121 @@
 
     # Leverage projects are git repositories too
     logger.info("Initializing git repository in project directory.")
     git("init")
 
     # Project configuration file
     if not PROJECT_CONFIG.exists():
-        logger.info(f"No project configuration file found. Dropping configuration template [bold]{PROJECT_CONFIG_FILE}[/bold].")
-        copy2(src=CONFIG_FILE_TEMPLATE,
-              dst=PROJECT_CONFIG_FILE)
+        logger.info(
+            f"No project configuration file found. Dropping configuration template [bold]{PROJECT_CONFIG_FILE}[/bold]."
+        )
+        copy2(src=CONFIG_FILE_TEMPLATE, dst=PROJECT_CONFIG_FILE)
 
     else:
         logger.warning(f"Project configuration file [bold]{PROJECT_CONFIG_FILE}[/bold] already exists in directory.")
 
     logger.info("Project initialization finished.")
 
 
 def _copy_account(account, primary_region):
-    """ Copy account directory and all its files.
+    """Copy account directory and all its files.
 
     Args:
         account (str): Account name.
         primary_region (str): Projects primary region.
     """
     (PROJECT_ROOT / account).mkdir()
 
     # Copy config directory
-    copytree(src=TEMPLATE_DIR / account / CONFIG_DIRECTORY,
-             dst=PROJECT_ROOT / account / CONFIG_DIRECTORY,
-             ignore=IGNORE_PATTERNS)
+    copytree(
+        src=TEMPLATE_DIR / account / CONFIG_DIRECTORY,
+        dst=PROJECT_ROOT / account / CONFIG_DIRECTORY,
+        ignore=IGNORE_PATTERNS,
+    )
     # Copy all global layers in account
     for layer in PROJECT_STRUCTURE[account]["global"]:
-        copytree(src=TEMPLATE_DIR / account / "global" / layer,
-                 dst=PROJECT_ROOT / account / "global" / layer,
-                 ignore=IGNORE_PATTERNS)
+        copytree(
+            src=TEMPLATE_DIR / account / "global" / layer,
+            dst=PROJECT_ROOT / account / "global" / layer,
+            ignore=IGNORE_PATTERNS,
+        )
     # Copy all layers with a region in account
     for layer in PROJECT_STRUCTURE[account]["primary_region"]:
-        copytree(src=TEMPLATE_DIR / account / "primary_region" / layer,
-                 dst=PROJECT_ROOT / account / primary_region / layer,
-                 ignore=IGNORE_PATTERNS)
+        copytree(
+            src=TEMPLATE_DIR / account / "primary_region" / layer,
+            dst=PROJECT_ROOT / account / primary_region / layer,
+            ignore=IGNORE_PATTERNS,
+        )
 
 
 def _copy_project_template(config):
-    """ Copy all files and directories from the Leverage project template to the project directory.
+    """Copy all files and directories from the Leverage project template to the project directory.
     It excludes al jinja templates as those will be rendered directly to their final location.
 
     Args:
         config (dict): Project configuration.
     """
     logger.info("Creating project directory structure.")
 
     # Copy .gitignore file
-    copy2(src=TEMPLATE_DIR / ".gitignore",
-          dst=PROJECT_ROOT / ".gitignore")
+    copy2(src=TEMPLATE_DIR / ".gitignore", dst=PROJECT_ROOT / ".gitignore")
 
     # Root config directory
-    copytree(src=TEMPLATE_DIR / CONFIG_DIRECTORY,
-             dst=PROJECT_ROOT / CONFIG_DIRECTORY,
-             ignore=IGNORE_PATTERNS)
+    copytree(src=TEMPLATE_DIR / CONFIG_DIRECTORY, dst=PROJECT_ROOT / CONFIG_DIRECTORY, ignore=IGNORE_PATTERNS)
 
     # Accounts
     for account in PROJECT_STRUCTURE:
         _copy_account(account=account, primary_region=config["primary_region"])
 
     logger.info("Finished creating directory structure.")
 
 
 def value(dictionary, key):
-    """ Utility function to be used as jinja filter, to ease extraction of values from dictionaries,
+    """Utility function to be used as jinja filter, to ease extraction of values from dictionaries,
     which is sometimes necessary.
 
     Args:
         dictionary (dict): The dictionary from which a value is to be extracted
         key (str): Key corresponding to the value to be extracted
 
     Returns:
         any: The value stored in the key
     """
     return dictionary[key]
 
 
 # Jinja environment used for rendering the templates
-JINJA_ENV = Environment(loader=FileSystemLoader(TEMPLATES_REPO_DIR.as_posix()),
-                        trim_blocks=False,
-                        lstrip_blocks=False)
+JINJA_ENV = Environment(loader=FileSystemLoader(TEMPLATES_REPO_DIR.as_posix()), trim_blocks=False, lstrip_blocks=False)
 JINJA_ENV.filters["value"] = value
 
 
 def _render_templates(template_files, config, source=TEMPLATE_DIR, destination=PROJECT_ROOT):
-    """ Render the given templates using the given configuration values.
+    """Render the given templates using the given configuration values.
 
     Args:
         template_files (iterable(Path)): Iterable containing the Path objects corresponding to the
             templates to render.
         config (dict): Values to replace in the templates.
         source (Path, optional): Source directory of the templates. Defaults to TEMPLATE_DIR.
         destination (Path, optional): Destination where to render the templates. Defaults to PROJECT_ROOT.
     """
     for template_file in template_files:
         template_location = template_file.relative_to(TEMPLATES_REPO_DIR)
 
         template = JINJA_ENV.get_template(template_location.as_posix())
-        if not 'terraform_image_tag' in config:
-            config['terraform_image_tag'] = __toolbox_version__
+        if not "terraform_image_tag" in config:
+            config["terraform_image_tag"] = __toolbox_version__
         rendered_template = template.render(config)
 
         rendered_location = template_file.relative_to(source)
-        if (rendered_location.parent.name == ""
-                or rendered_location.parent.name == CONFIG_DIRECTORY
-                or rendered_location.parent.parent.name == "global"):
+        if (
+            rendered_location.parent.name == ""
+            or rendered_location.parent.name == CONFIG_DIRECTORY
+            or rendered_location.parent.parent.name == "global"
+        ):
             rendered_location = destination / rendered_location
 
         else:
             region_name = template_location.parent.parent.name
             rendered_location = rendered_location.as_posix().replace(region_name, config[region_name])
             rendered_location = destination / Path(rendered_location)
 
@@ -234,41 +232,35 @@
         layers = layers + [f"{account_name}/{layer}" for layer in account_layers]
 
     for layer in layers:
         logger.info(f"\tLayer: Setting up [bold]{layer.split('/')[-1]}[/bold].")
         layer_dir = account_dir / layer
 
         layer_templates = layer_dir.glob(TEMPLATE_PATTERN)
-        _render_templates(template_files=layer_templates,
-                          config=config,
-                          source=source)
+        _render_templates(template_files=layer_templates, config=config, source=source)
 
 
 def _render_project_template(config, source=TEMPLATE_DIR):
     # Render base and non account related templates
     template_files = list(source.glob(TEMPLATE_PATTERN))
     config_templates = list((source / CONFIG_DIRECTORY).rglob(TEMPLATE_PATTERN))
     template_files.extend(config_templates)
 
     logger.info("Setting up common base files.")
-    _render_templates(template_files=template_files,
-                      config=config,
-                      source=source)
+    _render_templates(template_files=template_files, config=config, source=source)
 
     # Render each account's templates
     for account in config["organization"]["accounts"]:
-        _render_account_templates(account=account,
-                                  config=config,
-                                  source=source)
+        _render_account_templates(account=account, config=config, source=source)
 
     logger.info("Project configuration finished.")
 
 
 def load_project_config():
-    """ Load project configuration file.
+    """Load project configuration file.
 
     Raises:
         Exit: For any error produced during configuration loading.
 
     Returns:
         dict:  Project configuration.
     """
@@ -281,28 +273,51 @@
 
     except Exception as exc:
         exc.__traceback__ = None
         logger.exception(message="Error loading configuration file.", exc_info=exc)
         raise Exit(1)
 
 
+def validate_config(config: dict):
+    """
+    Run a battery of validations over the config file (project.yaml).
+    """
+    if not re.match(r"^[a-z0-9]([a-z0-9]|-){1,23}[a-z0-9]$", config["project_name"]):
+        raise ExitError(
+            1,
+            "Project name is not valid. Only lowercase alphanumeric characters and hyphens are allowed. It must be 25 characters long at most.",
+        )
+
+    if not re.match(r"^[a-z]{2,4}$", config["short_name"]):
+        raise ExitError(
+            1,
+            "Project short name is not valid. Only lowercase alphabetic characters are allowed. It must be between 2 and 4 characters long.",
+        )
+
+    return True
+
+
 @project.command()
 def create():
-    """ Create the directory structure required by the project configuration and set up each account accordingly. """
+    """Create the directory structure required by the project configuration and set up each account accordingly."""
 
     config = load_project_config()
     if not config:
-        logger.error("No configuration file found for the project."
-                     " Make sure the project has already been initialized ([bold]leverage project init[/bold]).")
+        logger.error(
+            "No configuration file found for the project."
+            " Make sure the project has already been initialized ([bold]leverage project init[/bold])."
+        )
         return
 
     if (PROJECT_ROOT / "config").exists():
         logger.error("Project has already been created.")
         return
 
+    validate_config(config)
+
     # Make project structure
     _copy_project_template(config=config)
 
     # Render project
     _render_project_template(config=config)
 
     # Format the code correctly
@@ -314,15 +329,15 @@
     with console.status("Formatting..."):
         terraform.exec("fmt", "-recursive")
 
     logger.info("Finished setting up project.")
 
 
 def render_file(file, config=None):
-    """ Utility to re-render specific files.
+    """Utility to re-render specific files.
 
     Args:
         file (str): Relative path to file to render.
         config (dict, optional): Config used to render file.
 
     Returns:
         bool: Whether the action succeeded or not
```

### Comparing `leverage-1.9.2/leverage/modules/run.py` & `leverage-1.9.4rc1/leverage/modules/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,28 +29,27 @@
     pass
 
 
 @click.command()
 @click.argument("tasks", nargs=-1)
 @pass_state
 def run(state, tasks):
-    """ Perform specified task(s) and all of its dependencies.
+    """Perform specified task(s) and all of its dependencies.
 
     When no task is given, the default (__DEFAULT__) task is run, if no default task has been defined, all available tasks are listed.
     """
     global _logger
     _logger = get_tasks_logger()
 
     if tasks:
         # Run the given tasks
         try:
             tasks_to_run = _prepare_tasks_to_run(state.module, tasks)
 
-        except (TaskNotFoundError,
-                MalformedTaskArgumentError) as exc:
+        except (TaskNotFoundError, MalformedTaskArgumentError) as exc:
             logger.error(str(exc))
             raise Exit(1)
 
         _run_tasks(tasks=tasks_to_run)
 
     else:
         # Run the default task or list available tasks
@@ -60,15 +59,15 @@
             _run_tasks(prepared_default_task)
 
         else:
             list_tasks(state.module)
 
 
 def _prepare_tasks_to_run(module, input_tasks):
-    """ Validate input tasks and arguments and pair them with the corresponding module's task.
+    """Validate input tasks and arguments and pair them with the corresponding module's task.
 
     Args:
         module (dict): Dict containing the tasks from the build script.
         input_tasks (list): Strings containing the tasks to invoke and their arguments as received
             from user input.
 
     Raises:
@@ -87,44 +86,43 @@
 
         name = match.group("name")
         arguments = match.group("arguments")
 
         try:
             args, kwargs = parse_task_args(arguments=arguments)
 
-        except (InvalidArgumentOrderError,
-                DuplicateKeywordArgumentError) as exc:
+        except (InvalidArgumentOrderError, DuplicateKeywordArgumentError) as exc:
             logger.error(str(exc).format(task=name))
             raise Exit(1)
 
         task = [task for task in module.tasks if task.name == name]
 
         if not task:
             raise TaskNotFoundError(f"Unrecognized task `{name}`.")
 
         tasks.append((task[0], args, kwargs))
 
     return tasks
 
 
 def _run_tasks(tasks):
-    """ Run the tasks provided.
+    """Run the tasks provided.
 
     Args:
         tasks (list(tuple)): List of 3-tuples containing a task and it's positional and keyword arguments to run.
     """
     completed_tasks = set()
     for task, args, kwargs in tasks:
         # Remove current task from dependencies set to force it to run, as it was invoked by the user explicitly
         completed_tasks.discard(task)
         _run(task, completed_tasks, *args, **kwargs)
 
 
 def _run(task, completed_tasks, *args, **kwargs):
-    """ Run the given task and all it's required dependencies, keeping track of all the already
+    """Run the given task and all it's required dependencies, keeping track of all the already
     completed tasks as not to repeat them.
 
     Args:
         task (list): Tasks to run.
         completed_tasks (set): Tasks that have already ran.
 
     Returns:
@@ -132,30 +130,31 @@
     """
     # Satisfy dependencies recursively.
     for dependency in task.dependencies:
         _completed_tasks = _run(dependency, completed_tasks)
         completed_tasks.update(_completed_tasks)
 
     if task not in completed_tasks:
-
         if task.is_ignored:
             _logger.info(f"[bold yellow]⤳[/bold yellow] Ignoring task [bold italic]{task.name}[/bold italic]")
 
         else:
             _logger.info(f"[bold yellow]➜[/bold yellow] Starting task [bold italic]{task.name}[/bold italic]")
 
             try:
                 task(*args, **kwargs)
             except Exception as exc:
                 # Remove the two topmost frames of the traceback since they are internal leverage function calls,
                 # only frames pertaining to the build script and its dependencies are shown.
                 exc.__traceback__ = exc.__traceback__.tb_next.tb_next
                 exc = clean_exception_traceback(exception=exc)
 
-                _logger.exception(f"[bold red]![/bold red] Error in task [bold italic]{task.name}[/bold italic]", exc_info=exc)
+                _logger.exception(
+                    f"[bold red]![/bold red] Error in task [bold italic]{task.name}[/bold italic]", exc_info=exc
+                )
                 _logger.critical("[red]✘[/red] [bold on red]Aborting build[/bold on red]")
                 raise Exit(1)
 
             _logger.info(f"[green]✔[/green] Completed task [bold italic]{task.name}[/bold italic]")
 
         completed_tasks.add(task)
```

### Comparing `leverage-1.9.2/leverage/modules/terraform.py` & `leverage-1.9.4rc1/leverage/modules/terraform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,184 +1,214 @@
-import re
 import os
-from pathlib import Path
+import re
 
-import hcl2
 import click
+import dockerpty
+import hcl2
 from click.exceptions import Exit
 
 from leverage import logger
-from leverage._internals import pass_state
 from leverage._internals import pass_container
-from leverage.container import get_docker_client
+from leverage._internals import pass_state
+from leverage._utils import tar_directory, AwsCredsContainer, LiveContainer, ExitError
 from leverage.container import TerraformContainer
+from leverage.container import get_docker_client
+from leverage.modules.utils import env_var_option, mount_option, auth_mfa, auth_sso
+
+REGION = (
+    r"global|(?:[a-z]{2}-(?:gov-)?"
+    r"(?:central|north|south|east|west|northeast|northwest|southeast|southwest|secret|topsecret)-[1-4])"
+)
 
-REGION = (r"global|(?:[a-z]{2}-(?:gov-)?"
-          r"(?:central|north|south|east|west|northeast|northwest|southeast|southwest|secret|topsecret)-[1-4])")
 
 # ###########################################################################
 # CREATE THE TERRAFORM GROUP
 # ###########################################################################
 @click.group()
+@mount_option
+@env_var_option
 @pass_state
-def terraform(state):
-    """ Run Terraform commands in a custom containerized environment that provides extra functionality when interacting
+def terraform(state, env_var, mount):
+    """Run Terraform commands in a custom containerized environment that provides extra functionality when interacting
     with your cloud provider such as handling multi factor authentication for you.
     All terraform subcommands that receive extra args will pass the given strings as is to their corresponding Terraform
     counterparts in the container. For example as in `leverage terraform apply -auto-approve` or
     `leverage terraform init -reconfigure`
     """
-    state.container = TerraformContainer(get_docker_client())
+    if env_var:
+        env_var = dict(env_var)
+
+    state.container = TerraformContainer(get_docker_client(), mounts=mount, env_vars=env_var)
     state.container.ensure_image()
 
 
-CONTEXT_SETTINGS = {
-    "ignore_unknown_options": True
-}
+CONTEXT_SETTINGS = {"ignore_unknown_options": True}
 
 # ###########################################################################
 # CREATE THE TERRAFORM GROUP'S COMMANDS
 # ###########################################################################
 #
 # --layers is a ordered comma separated list of layer names
 # The layer names are the relative paths of those layers relative to the current directory
 # e.g. if CLI is called from /home/user/project/management and this is the tree:
 # home
 # ├── user
-# │   └── project
-# │       └── management
-# │           ├── global
-# │           |   └── security-base
-# │           |   └── sso
-# │           └── us-east-1
-# │               └── terraform-backend
+# │   └── project
+# │       └── management
+# │           ├── global
+# │           |   └── security-base
+# │           |   └── sso
+# │           └── us-east-1
+# │               └── terraform-backend
 #
 # Then all three layers can be initialized as follows:
 # leverage tf init --layers us-east-1/terraform-backend,global/security-base,global/sso
 #
 # It is an ordered list because the layers will be visited in the same order they were
 # supplied.
 #
-layers_option = click.option("--layers",
-                             type=str,
-                             default="",
-                             help="Layers to apply the action to. (an ordered, comma-separated list of layer names)")
+layers_option = click.option(
+    "--layers",
+    type=str,
+    default="",
+    help="Layers to apply the action to. (an ordered, comma-separated list of layer names)",
+)
+
 
 @terraform.command(context_settings=CONTEXT_SETTINGS)
-@click.option("--skip-validation",
-              is_flag=True,
-              help="Skip layout validation.")
+@click.option("--skip-validation", is_flag=True, help="Skip layout validation.")
 @layers_option
 @click.argument("args", nargs=-1)
 @pass_container
 @click.pass_context
-def init(context, tf, skip_validation, layers, args):
+def init(context, tf: TerraformContainer, skip_validation, layers, args):
     """
     Initialize this layer.
     """
-    invoke_for_all_commands(layers, _init, args, skip_validation)
+    layers = invoke_for_all_commands(layers, _init, args, skip_validation)
+
+    # now change ownership on all the downloaded modules and providers
+    for layer in layers:
+        tf.change_file_ownership(tf.paths.guest_base_path / layer.relative_to(tf.paths.root_dir) / ".terraform")
+    # and then providers in the cache folder
+    if tf.paths.tf_cache_dir:
+        tf.change_file_ownership(tf.paths.tf_cache_dir)
+
 
 @terraform.command(context_settings=CONTEXT_SETTINGS)
 @layers_option
 @click.argument("args", nargs=-1)
 @pass_container
 @click.pass_context
 def plan(context, tf, layers, args):
-    """ Generate an execution plan for this layer. """
+    """Generate an execution plan for this layer."""
     invoke_for_all_commands(layers, _plan, args)
 
+
 @terraform.command(context_settings=CONTEXT_SETTINGS)
 @layers_option
 @click.argument("args", nargs=-1)
 @pass_container
 @click.pass_context
 def apply(context, tf, layers, args):
-    """ Build or change the infrastructure in this layer. """
+    """Build or change the infrastructure in this layer."""
     invoke_for_all_commands(layers, _apply, args)
 
+
 @terraform.command(context_settings=CONTEXT_SETTINGS)
 @layers_option
 @click.argument("args", nargs=-1)
 @pass_container
 @click.pass_context
 def output(context, tf, layers, args):
-    """ Show all output variables of this layer. """
+    """Show all output variables of this layer."""
     invoke_for_all_commands(layers, _output, args)
 
+
 @terraform.command(context_settings=CONTEXT_SETTINGS)
 @layers_option
 @click.argument("args", nargs=-1)
 @pass_container
 @click.pass_context
 def destroy(context, tf, layers, args):
-    """ Destroy infrastructure in this layer. """
+    """Destroy infrastructure in this layer."""
     invoke_for_all_commands(layers, _destroy, args)
 
+
 @terraform.command()
 @pass_container
 def version(tf):
-    """ Print version. """
+    """Print version."""
     tf.disable_authentication()
     tf.start("version")
 
+
 @terraform.command()
-@click.option("--mfa",
-              is_flag=True,
-              default=False,
-              help="Enable Multi Factor Authentication upon launching shell.")
-@click.option("--sso",
-              is_flag=True,
-              default=False,
-              help="Enable SSO Authentication upon launching shell.")
+@auth_mfa
+@auth_sso
 @pass_container
 def shell(tf, mfa, sso):
-    """ Open a shell into the Terraform container in this layer. """
+    """Open a shell into the Terraform container in this layer."""
     tf.disable_authentication()
     if sso:
         tf.enable_sso()
 
     if mfa:
         tf.enable_mfa()
 
     tf.start_shell()
 
+
 @terraform.command("format", context_settings=CONTEXT_SETTINGS)
 @click.argument("args", nargs=-1)
 @pass_container
 def _format(tf, args):
-    """ Check if all files meet the canonical format and rewrite them accordingly. """
+    """Check if all files meet the canonical format and rewrite them accordingly."""
     args = args if "-recursive" in args else (*args, "-recursive")
     tf.disable_authentication()
     tf.start("fmt", *args)
 
+
 @terraform.command()
 @pass_container
 def validate(tf):
-    """ Validate code of the current directory. Previous initialization might be needed. """
+    """Validate code of the current directory. Previous initialization might be needed."""
     tf.disable_authentication()
     tf.start("validate")
 
+
 @terraform.command("validate-layout")
 @pass_container
 def validate_layout(tf):
-    """ Validate layer conforms to Leverage convention. """
+    """Validate layer conforms to Leverage convention."""
     tf.set_backend_key()
     return _validate_layout()
 
+
 @terraform.command("import")
 @click.argument("address")
 @click.argument("_id", metavar="ID")
 @pass_container
 def _import(tf, address, _id):
-    """ Import a resource. """
+    """Import a resource."""
     exit_code = tf.start_in_layer("import", *tf.tf_default_args, address, _id)
 
     if exit_code:
         raise Exit(exit_code)
 
+
+@terraform.command("refresh-credentials")
+@pass_container
+def refresh_credentials(tf):
+    """Refresh the AWS credentials used on the current layer."""
+    tf.paths.check_for_layer_location()
+    if exit_code := tf.refresh_credentials():
+        raise Exit(exit_code)
+
+
 # ###########################################################################
 # HANDLER FOR MANAGING THE BASE COMMANDS (init, plan, apply, destroy, output)
 # ###########################################################################
 @pass_container
 def invoke_for_all_commands(tf, layers, command, args, skip_validation=True):
     """
     Invoke helper for "all" commands.
@@ -186,159 +216,220 @@
     Args:
         layers: comma separated value of relative layer path
             e.g.: global/security_audit,us-east-1/tf-backend
         command: init, plan, apply
     """
 
     # convert layers from string to list
-    layers = layers.split(',') if len(layers) > 0 else []
+    layers = layers.split(",") if len(layers) > 0 else []
 
     # based on the location type manage the layers parameter
-    if tf.get_location_type() == 'layer' and len(layers) == 0:
+    location_type = tf.paths.get_location_type()
+    if location_type == "layer" and len(layers) == 0:
         # running on a layer
-        layers = [tf.cwd]
-    elif tf.get_location_type() == 'layer':
+        layers = [tf.paths.cwd]
+    elif location_type == "layer":
         # running on a layer but --layers was set
-        logger.error("Can not set [bold]--layers[/bold] inside a layer.")
-        raise Exit(1)
-    elif tf.get_location_type() in ['account','layers-group'] and len(layers) == 0:
+        raise ExitError(1, "Can not set [bold]--layers[/bold] inside a layer.")
+    elif location_type in ["account", "layers-group"] and len(layers) == 0:
         # running on an account but --layers was not set
-        logger.error("[bold]--layers[/bold] has to be set.")
-        raise Exit(1)
-    elif not tf.get_location_type() in ['account', 'layer', 'layers-group']:
+        raise ExitError(1, "[bold]--layers[/bold] has to be set.")
+    elif location_type not in ["account", "layer", "layers-group"]:
         # running outside a layer and account
-        logger.error('This command has to be run inside a layer or account directory.')
-        raise Exit(1)
+        raise ExitError(1, "This command has to be run inside a layer or account directory.")
     else:
         # running on an account with --layers set
-        layers = [ tf.cwd / x for x in layers]
+        layers = [tf.paths.cwd / x for x in layers]
 
     # get current location
-    original_location = tf.cwd
-    original_working_dir = tf.container_config['working_dir']
+    original_location = tf.paths.cwd
+    original_working_dir = tf.container_config["working_dir"]
 
     # validate each layer before calling the execute command
     for layer in layers:
         logger.debug(f"Checking for layer {layer}...")
         # change to current dir and set it in the container
-        tf.cwd = layer
+        tf.paths.cwd = layer
 
         # check layers existence
         if not layer.is_dir():
             logger.error(f"Directory [red]{layer}[/red] does not exist or is not a directory\n")
             raise Exit(1)
 
         # set the s3 key
         tf.set_backend_key(skip_validation)
 
-        #validate layer
+        # validate layer
         validate_for_all_commands(layer, skip_validation=skip_validation)
 
         # change to original dir and set it in the container
-        tf.cwd = original_location
+        tf.paths.cwd = original_location
 
     # check layers existence
     for layer in layers:
         if len(layers) > 1:
             logger.info(f"Invoking command for layer {layer}...")
 
         # change to current dir and set it in the container
-        tf.cwd = layer
+        tf.paths.cwd = layer
 
         # set the working dir
-        tf.container_config['working_dir'] = f"{tf.guest_base_path}/{tf.cwd.relative_to(tf.root_dir).as_posix()}"
+        working_dir = f"{tf.paths.guest_base_path}/{tf.paths.cwd.relative_to(tf.paths.root_dir).as_posix()}"
+        tf.container_config["working_dir"] = working_dir
 
         # execute the actual command
         command(args=args)
 
         # change to original dir and set it in the container
-        tf.cwd = original_location
+        tf.paths.cwd = original_location
 
         # change to original workgindir
-        tf.container_config['working_dir'] = original_working_dir
+        tf.container_config["working_dir"] = original_working_dir
+
+    return layers
+
 
 def validate_for_all_commands(layer, skip_validation=False):
     """
-    Validate existense of layer and, if set, all the Leverage related stuff
+    Validate existence of layer and, if set, all the Leverage related stuff
     of each of them
 
     Args:
         layer: a full layer directory
     """
 
     logger.debug(f"Checking layer {layer}...")
     if not skip_validation and not _validate_layout():
-        logger.error("Layer configuration doesn't seem to be valid. Exiting.\n"
-                    "If you are sure your configuration is actually correct "
-                    "you may skip this validation using the --skip-validation flag.")
+        logger.error(
+            "Layer configuration doesn't seem to be valid. Exiting.\n"
+            "If you are sure your configuration is actually correct "
+            "you may skip this validation using the --skip-validation flag."
+        )
         raise Exit(1)
 
+
 # ###########################################################################
 # BASE COMMAND EXECUTORS
 # ###########################################################################
 @pass_container
 def _init(tf, args):
-    """ Initialize this layer. """
-
-    args = [arg for index, arg in enumerate(args)
-            if not arg.startswith("-backend-config") or not arg[index - 1] == "-backend-config"]
-    args.append(f"-backend-config={tf.backend_tfvars}")
-    args.append(f"-backend-config=\"region={tf.terraform_backend.get('region')}\"")
-
-    exit_code = tf.start_in_layer("init", *args)
+    """Initialize this layer."""
 
-    if exit_code:
-        raise Exit(exit_code)
+    args = [
+        arg
+        for index, arg in enumerate(args)
+        if not arg.startswith("-backend-config") or not arg[index - 1] == "-backend-config"
+    ]
+    args.append(f"-backend-config={tf.paths.backend_tfvars}")
+
+    tf.paths.check_for_layer_location()
+
+    with LiveContainer(tf) as container:
+        # create the .ssh directory
+        container.exec_run("mkdir -p /root/.ssh")
+        # copy the entire ~/.ssh/ folder
+        tar_bytes = tar_directory(tf.paths.home / ".ssh")
+        # into /root/.ssh
+        container.put_archive("/root/.ssh/", tar_bytes)
+        # correct the owner of the files to match with the docker internal user
+        container.exec_run("chown root:root -R /root/.ssh/")
+
+        with AwsCredsContainer(container, tf):
+            dockerpty.exec_command(
+                client=tf.client.api,
+                container=container.id,
+                command="terraform init " + " ".join(args),
+                interactive=bool(int(os.environ.get("LEVERAGE_INTERACTIVE", 1))),
+            )
 
 
 @pass_container
 def _plan(tf, args):
-    """ Generate an execution plan for this layer. """
+    """Generate an execution plan for this layer."""
     exit_code = tf.start_in_layer("plan", *tf.tf_default_args, *args)
 
     if exit_code:
         raise Exit(exit_code)
 
 
+def handle_apply_arguments_parsing(args):
+    """Parse and process the arguments for the 'apply' command."""
+    # Initialize new_args to handle both '-key=value' and '-key value'
+    new_args = []
+    skip_next = False  # Flag to skip the next argument if it's part of '-key value'
+
+    for i, arg in enumerate(args):
+        if skip_next:
+            skip_next = False  # Reset flag and skip this iteration
+            continue
+
+        if arg.startswith("-") and not arg.startswith("-var"):
+            if i + 1 < len(args) and not args[i + 1].startswith("-"):
+                # Detected '-key value' pair; append them without merging
+                new_args.append(arg)
+                new_args.append(args[i + 1])
+                skip_next = True  # Mark to skip the next item as it's already processed
+                logger.debug(f"Detected '-key value' pair: {arg}, {args[i + 1]}")
+            else:
+                # Either '-key=value' or a standalone '-key'; just append
+                new_args.append(arg)
+                logger.debug(f"Appending standard -key=value or standalone argument: {arg}")
+        else:
+            # Handles '-var' and non '-' starting arguments
+            new_args.append(arg)
+            logger.debug(f"Appending argument (non '-' or '-var'): {arg}")
+
+    return new_args
+
+
 @pass_container
 def _apply(tf, args):
-    """ Build or change the infrastructure in this layer. """
+    """Build or change the infrastructure in this layer."""
     # if there is a plan, remove all "-var" from the default args
-    tf_default_args  = tf.tf_default_args
+    # Preserve the original `-var` removal logic and modify tf_default_args if necessary
+    tf_default_args = tf.tf_default_args
     for arg in args:
         if not arg.startswith("-"):
-            tf_default_args = [arg for index, arg in enumerate(tf_default_args)
-                    if not arg.startswith("-var")]
+            tf_default_args = [arg for index, arg in enumerate(tf_default_args) if not arg.startswith("-var")]
             break
-    exit_code = tf.start_in_layer("apply", *tf_default_args, *args)
+
+    # Process arguments using the new parsing logic
+    processed_args = handle_apply_arguments_parsing(args)
+
+    logger.debug(f"Original tf_default_args: {tf_default_args}")
+    logger.debug(f"Processed argument list for execution: {processed_args}")
+
+    # Execute the command with the modified arguments list
+    exit_code = tf.start_in_layer("apply", *tf_default_args, *processed_args)
 
     if exit_code:
+        logger.error(f"Command execution failed with exit code: {exit_code}")
         raise Exit(exit_code)
 
 
 @pass_container
 def _output(tf, args):
-    """ Show all output variables of this layer. """
+    """Show all output variables of this layer."""
     tf.start_in_layer("output", *args)
 
 
 @pass_container
 def _destroy(tf, args):
-    """ Destroy infrastructure in this layer. """
+    """Destroy infrastructure in this layer."""
     exit_code = tf.start_in_layer("destroy", *tf.tf_default_args, *args)
 
     if exit_code:
         raise Exit(exit_code)
 
 
 # ###########################################################################
 # MISC FUNCTIONS
 # ###########################################################################
 def _make_layer_backend_key(cwd, account_dir, account_name):
-    """ Create expected backend key.
+    """Create expected backend key.
 
     Args:
         cwd (pathlib.Path): Current Working Directory (Layer Directory)
         account_dir (pathlib.Path): Account Directory
         account_name (str): Account Name
 
     Returns:
@@ -346,113 +437,115 @@
     """
     resp = []
 
     layer_path = cwd.relative_to(account_dir)
     layer_path = layer_path.as_posix().split("/")
     # Check region directory to keep retro compat
     if re.match(REGION, layer_path[0]):
-        layer_paths = [layer_path[1:],layer_path]
+        layer_paths = [layer_path[1:], layer_path]
     else:
         layer_paths = [layer_path]
 
     curated_layer_paths = []
     # Remove layer name prefix
     for layer_path in layer_paths:
         curated_layer_path = []
         for lp in layer_path:
-            if lp.startswith('base-'):
-                lp = lp.replace('base-','')
-            elif lp.startswith('tools-'):
-                lp = lp.replace('tools-','')
+            if lp.startswith("base-"):
+                lp = lp.replace("base-", "")
+            elif lp.startswith("tools-"):
+                lp = lp.replace("tools-", "")
             curated_layer_path.append(lp)
         curated_layer_paths.append(curated_layer_path)
 
     curated_layer_paths_retrocomp = []
     for layer_path in curated_layer_paths:
         curated_layer_paths_retrocomp.append(layer_path)
         # check for tf/terraform variants
-        for idx,lp in enumerate(layer_path):
-            if lp.startswith('tf-'):
+        for idx, lp in enumerate(layer_path):
+            if lp.startswith("tf-"):
                 layer_path_tmp = layer_path.copy()
-                layer_path_tmp[idx] = layer_path_tmp[idx].replace('tf-','terraform-')
+                layer_path_tmp[idx] = layer_path_tmp[idx].replace("tf-", "terraform-")
                 curated_layer_paths_retrocomp.append(layer_path_tmp)
                 break
-            elif lp.startswith('terraform-'):
+            elif lp.startswith("terraform-"):
                 layer_path_tmp = layer_path.copy()
-                layer_path_tmp[idx] = layer_path_tmp[idx].replace('terraform-','tf-')
+                layer_path_tmp[idx] = layer_path_tmp[idx].replace("terraform-", "tf-")
                 curated_layer_paths_retrocomp.append(layer_path_tmp)
                 break
 
     curated_layer_paths_withDR = []
     for layer_path in curated_layer_paths_retrocomp:
         curated_layer_paths_withDR.append(layer_path)
         curated_layer_path = []
-        append_str = '-dr'
+        append_str = "-dr"
         for lp in layer_path:
             if re.match(REGION, lp):
                 curated_layer_path.append(lp)
             else:
-                curated_layer_path.append(lp+append_str)
-                append_str = ''
+                curated_layer_path.append(lp + append_str)
+                append_str = ""
         curated_layer_paths_withDR.append(curated_layer_path)
 
-
     for layer_path in curated_layer_paths_withDR:
         resp.append([account_name, *layer_path])
 
     return resp
 
 
 @pass_container
-def _validate_layout(tf):
-    tf.check_for_layer_location()
+def _validate_layout(tf: TerraformContainer):
+    tf.paths.check_for_layer_location()
 
     # Check for `environment = <account name>` in account.tfvars
-    account_name = tf.account_conf.get("environment")
+    account_name = tf.paths.account_conf.get("environment")
     logger.info("Checking environment name definition in [bold]account.tfvars[/bold]...")
     if account_name is None:
         logger.error("[red]✘ FAILED[/red]\n")
         raise Exit(1)
     logger.info("[green]✔ OK[/green]\n")
 
     # Check if account directory name matches with environment name
-    if tf.account_dir.stem != account_name:
-        logger.warning("[yellow]‼[/yellow] Account directory name does not match environment name.\n"
-                       f"  Expected [bold]{account_name}[/bold], found [bold]{tf.account_dir.stem}[/bold]\n")
+    if tf.paths.account_dir.stem != account_name:
+        logger.warning(
+            "[yellow]‼[/yellow] Account directory name does not match environment name.\n"
+            f"  Expected [bold]{account_name}[/bold], found [bold]{tf.paths.account_dir.stem}[/bold]\n"
+        )
 
-    backend_key = tf.backend_key.split('/')
+    backend_key = tf.backend_key.split("/")
 
     # Flag to report layout validity
     valid_layout = True
 
     # Check backend bucket key
-    expected_backend_keys = _make_layer_backend_key(tf.cwd, tf.account_dir, account_name)
+    expected_backend_keys = _make_layer_backend_key(tf.paths.cwd, tf.paths.account_dir, account_name)
     logger.info("Checking backend key...")
     logger.info(f"Found: '{'/'.join(backend_key)}'")
     backend_key = backend_key[:-1]
 
     if backend_key in expected_backend_keys:
         logger.info("[green]✔ OK[/green]\n")
     else:
         exp_message = [f"{'/'.join(x)}/terraform.tfstate" for x in expected_backend_keys]
-        logger.info(f"Expected on of: {';'.join(exp_message)}")
+        logger.info(f"Expected one of: {';'.join(exp_message)}")
         logger.error("[red]✘ FAILED[/red]\n")
         valid_layout = False
 
-    backend_tfvars = tf.account_config_dir / tf.BACKEND_TFVARS
+    backend_tfvars = tf.paths.account_config_dir / tf.paths.BACKEND_TF_VARS  # TODO use paths.backend_tfvars instead?
     backend_tfvars = hcl2.loads(backend_tfvars.read_text()) if backend_tfvars.exists() else {}
 
     logger.info("Checking [bold]backend.tfvars[/bold]:\n")
     names_prefix = f"{tf.project}-{account_name}"
     names_prefix_bootstrap = f"{tf.project}-bootstrap"
 
     # Check profile, bucket and dynamo table names:
     for field in ("profile", "bucket", "dynamodb_table"):
         logger.info(f"Checking if {field.replace('_', ' ')} starts with {names_prefix}...")
-        if backend_tfvars.get(field, "").startswith(names_prefix) or (field == 'profile' and backend_tfvars.get(field, "").startswith(names_prefix_bootstrap)):
+        if backend_tfvars.get(field, "").startswith(names_prefix) or (
+            field == "profile" and backend_tfvars.get(field, "").startswith(names_prefix_bootstrap)
+        ):
             logger.info("[green]✔ OK[/green]\n")
         else:
             logger.error("[red]✘ FAILED[/red]\n")
             valid_layout = False
 
     return valid_layout
-
```

### Comparing `leverage-1.9.2/leverage/modules/tfautomv.py` & `leverage-1.9.4rc1/leverage/modules/tfautomv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-import re
-
-import hcl2
 import click
 from click.exceptions import Exit
 
-from leverage import logger
 from leverage._internals import pass_state
 from leverage._internals import pass_container
 from leverage.container import get_docker_client
 from leverage.container import TFautomvContainer
 
-REGION = (r"global|(?:[a-z]{2}-(?:gov-)?"
-          r"(?:central|north|south|east|west|northeast|northwest|southeast|southwest|secret|topsecret)-[1-4])")
+REGION = (
+    r"global|(?:[a-z]{2}-(?:gov-)?"
+    r"(?:central|north|south|east|west|northeast|northwest|southeast|southwest|secret|topsecret)-[1-4])"
+)
+
 
 @click.group()
 @pass_state
 def tfautomv(state):
-    """ Run TFAutomv commands in a custom containerized environment that provides extra functionality when interacting
+    """Run TFAutomv commands in a custom containerized environment that provides extra functionality when interacting
     with your cloud provider such as handling multi factor authentication for you.
     All terraform subcommands that receive extra args will pass the given strings as is to their corresponding Terraform
     counterparts in the container. For example as in `leverage terraform apply -auto-approve` or
     `leverage terraform init -reconfigure`
     """
     state.container = TFautomvContainer(get_docker_client())
     state.container.ensure_image()
 
-CONTEXT_SETTINGS = {
-    "ignore_unknown_options": True
-}
+
+CONTEXT_SETTINGS = {"ignore_unknown_options": True}
+
 
 @tfautomv.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("args", nargs=-1)
 @pass_container
 def run(tf, args):
-    """ Generate a move tf file for this layer. """
+    """Generate a move tf file for this layer."""
     exit_code = tf.start_in_layer(*args)
 
     if exit_code:
         raise Exit(exit_code)
-
```

### Comparing `leverage-1.9.2/leverage/tasks.py` & `leverage-1.9.4rc1/leverage/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class MissingParensInDecoratorError(ImportError):
     pass
 
 
 def task(*dependencies, **options):
-    """ Task decorator to mark functions in a build script as tasks to be performed.
+    """Task decorator to mark functions in a build script as tasks to be performed.
 
     Raises:
         MissingParensInDecorator: When the decorator is most likely being used without parentheses
             on a function.
         NotATask: When any of the task dependencies is not a task.
 
     Returns:
@@ -48,39 +48,41 @@
     #     @task(function_not_task)
     #     def func():
     #         pass
     # ```
     # where the dependency provided is a function and not a task. So the need of parentheses is
     # enforced through this check below
     if len(dependencies) == 1 and isfunction(dependencies[0]):
-        raise MissingParensInDecoratorError("Possible parentheses missing in function "
-                                            f"`{dependencies[0].__name__}` decorator.")
+        raise MissingParensInDecoratorError(
+            "Possible parentheses missing in function " f"`{dependencies[0].__name__}` decorator."
+        )
 
-    not_tasks = [dependency.__name__
-                 for dependency in dependencies
-                 if not Task.is_task(dependency)]
+    not_tasks = [dependency.__name__ for dependency in dependencies if not Task.is_task(dependency)]
 
     if not_tasks:
-        raise NotATaskError(f"Dependencies {', '.join(not_tasks)} are not tasks. "
-                            "They all must be functions decorated with the `@task()` decorator.")
+        raise NotATaskError(
+            f"Dependencies {', '.join(not_tasks)} are not tasks. "
+            "They all must be functions decorated with the `@task()` decorator."
+        )
 
     def _task(func):
         return Task(func, list(dependencies), options)
 
     return _task
 
 
 class Task:
-    """ Task to be run by Leverage, created from a function with the @task() decorator.
+    """Task to be run by Leverage, created from a function with the @task() decorator.
     A task which name starts with an underscore is considered private and, as such, not shown
     when tasks are listed, this can also be explicitly indicated in the decorator.
     An ignored task won't be ran by Leverage.
     """
+
     def __init__(self, task, dependencies=None, options=None):
-        """ Task object initialization
+        """Task object initialization
 
         Args:
             task (function): Function to be called upon task execution.
             dependencies (list(Tasks), optional): List of tasks that must be performed before this
                 task is executed. Defaults to an empty list.
             options (dict, optional): Options regarding the task nature:
                 - private (bool): Whether the task is private or not. Defaults to False.
@@ -94,42 +96,40 @@
 
         options = {} if options is None else options
         self._private = self.name.startswith("_") or bool(options.get("private", False))
         self._ignored = bool(options.get("ignore", False))
 
     @classmethod
     def is_task(cls, obj):
-        """ Whether the given object is a task or not """
+        """Whether the given object is a task or not"""
         return isinstance(obj, cls)
 
     @property
     def is_private(self):
-        """ Whether the task is private or not """
+        """Whether the task is private or not"""
         return self._private
 
     @property
     def is_ignored(self):
-        """ Whether the task is ignored or not """
+        """Whether the task is ignored or not"""
         return self._ignored
 
     def __call__(self, *args, **kwargs):
-        """ Execute the task """
+        """Execute the task"""
         self.task(*args, **kwargs)
 
     def __eq__(self, other):
-        return (isinstance(other, Task)
-                and self.name == other.name
-                and self.doc == other.doc)
+        return isinstance(other, Task) and self.name == other.name and self.doc == other.doc
 
     def __hash__(self):
         return id(self)
 
 
 def load_tasks(build_script_filename="build.py"):
-    """ Load the tasks in the build script if there is one.
+    """Load the tasks in the build script if there is one.
 
     Args:
         build_script_filename (str, optional): Name of the file containing the defined tasks. Defaults to "build.py".
 
     Returns:
         Module: Module containing the loaded tasks. An empty module if no build script is found.
     """
@@ -138,15 +138,15 @@
     if build_script is None:
         return Module()
 
     return _load_build_script(build_script=build_script)
 
 
 def _load_build_script(build_script):
-    """ Load build script as module and return the useful bits.
+    """Load build script as module and return the useful bits.
     If build script is malformed the exception trace is printed and the application exits.
 
     Args:
         build_script (str): Path to the file containing the definition of the tasks.
 
     Returns:
         Module: Name, tasks and default tasks of the module.
@@ -159,38 +159,38 @@
     sys.path.append(package.parent.as_posix())
 
     # Package needs to be imported first
     importlib.import_module(package.name)
 
     # Load build script as module
     try:
-        module = importlib.import_module(f".{build_script.stem}",
-                                         package=package.name)
+        module = importlib.import_module(f".{build_script.stem}", package=package.name)
 
     except (ImportError, ModuleNotFoundError, SyntaxError) as exc:
         # Remove frames in the traceback until we reach the one pertaining to the build
         # script, as to avoid polluting the output with internal leverage calls,
         # only frames of the build script and its dependencies are shown.
         build_script = build_script.as_posix()
-        while (exc.__traceback__ is not None
-                and exc.__traceback__.tb_frame.f_code.co_filename != build_script):
+        while exc.__traceback__ is not None and exc.__traceback__.tb_frame.f_code.co_filename != build_script:
             exc.__traceback__ = exc.__traceback__.tb_next
 
         exc = clean_exception_traceback(exception=exc)
 
         logger.exception("Error in build script.", exc_info=exc)
         raise Exit(1)
 
-    return Module(name=Path(module.__file__).name,
-                  tasks=_get_tasks(module=module),
-                  default_task=getattr(module, "__DEFAULT__", None))
+    return Module(
+        name=Path(module.__file__).name,
+        tasks=_get_tasks(module=module),
+        default_task=getattr(module, "__DEFAULT__", None),
+    )
 
 
 def _get_tasks(module):
-    """ Extract all Task objects from a loaded module.
+    """Extract all Task objects from a loaded module.
 
     Args:
         module (module): Loaded module containing the definition of tasks.
 
     Returns:
         list: All tasks found in the given module.
     """
@@ -202,15 +202,15 @@
 
 _CREDIT_LINE = f"Powered by Leverage {__version__}"
 _IGNORED = "Ignored"
 _DEFAULT = "Default"
 
 
 def list_tasks(module):
-    """ Print all non-private tasks in a neat table-like format.
+    """Print all non-private tasks in a neat table-like format.
     Indicates whether the task is ignored and/or if it is the default one.
 
     Args:
         module (dict): Dictionary containing all tasks and the module name
     """
     visible_tasks = [task for task in module.tasks if not task.is_private]
 
@@ -234,15 +234,14 @@
             tasks_grid.append((task.name, task_attrs, doc_lines))
 
         name_column_width = max(len(name) for name, _, _ in tasks_grid)
         attr_column_width = max(len(attr) for _, attr, _ in tasks_grid)
 
         # Body
         for name, attr, doc in tasks_grid:
-
             doc_line = "" if not doc else doc[0]
             click.echo(f"  {name:<{name_column_width}}  {attr: ^{attr_column_width}}\t{doc_line}")
             # Print the remaining lines of the dosctring with the correct indentation
             for doc_line in doc[1:]:
                 click.echo(f"    {'': <{name_column_width + attr_column_width}}\t{doc_line}")
 
         # Footer
```

