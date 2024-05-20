# Comparing `tmp/tempclone-1.0.0.tar.gz` & `tmp/tempclone-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempclone-1.0.0.tar", last modified: Mon May 20 01:29:27 2024, max compression
+gzip compressed data, was "tempclone-1.0.1.tar", last modified: Mon May 20 12:41:40 2024, max compression
```

## Comparing `tempclone-1.0.0.tar` & `tempclone-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 01:29:27.089196 tempclone-1.0.0/
--rw-rw-rw-   0        0        0     1094 2024-05-20 01:23:35.000000 tempclone-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1112 2024-05-20 01:29:27.088194 tempclone-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      585 2024-05-20 01:13:01.000000 tempclone-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-20 01:29:27.089196 tempclone-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      948 2024-05-20 01:18:36.000000 tempclone-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:29:27.053197 tempclone-1.0.0/tempclone/
--rw-rw-rw-   0        0        0        0 2024-05-19 17:58:11.000000 tempclone-1.0.0/tempclone/__init__.py
--rw-rw-rw-   0        0        0     6512 2024-05-20 01:08:14.000000 tempclone-1.0.0/tempclone/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:29:27.086197 tempclone-1.0.0/tempclone.egg-info/
--rw-rw-rw-   0        0        0     1112 2024-05-20 01:29:26.000000 tempclone-1.0.0/tempclone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-05-20 01:29:27.000000 tempclone-1.0.0/tempclone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 01:29:26.000000 tempclone-1.0.0/tempclone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-20 01:29:26.000000 tempclone-1.0.0/tempclone.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-05-20 01:29:26.000000 tempclone-1.0.0/tempclone.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-20 01:29:26.000000 tempclone-1.0.0/tempclone.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 01:29:27.085195 tempclone-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-20 00:42:03.000000 tempclone-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2681 2024-05-20 01:07:43.000000 tempclone-1.0.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:40.983719 tempclone-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 12:41:26.000000 tempclone-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 12:41:40.983719 tempclone-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-20 12:41:26.000000 tempclone-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:41:40.983719 tempclone-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-20 12:41:26.000000 tempclone-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:40.979719 tempclone-1.0.1/tempclone/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:26.000000 tempclone-1.0.1/tempclone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-20 12:41:26.000000 tempclone-1.0.1/tempclone/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:40.979719 tempclone-1.0.1/tempclone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 12:41:40.000000 tempclone-1.0.1/tempclone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 12:41:40.000000 tempclone-1.0.1/tempclone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:41:40.000000 tempclone-1.0.1/tempclone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 12:41:40.000000 tempclone-1.0.1/tempclone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 12:41:40.000000 tempclone-1.0.1/tempclone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 12:41:40.000000 tempclone-1.0.1/tempclone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:40.979719 tempclone-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:41:26.000000 tempclone-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-20 12:41:26.000000 tempclone-1.0.1/tests/test_cli.py
```

### Comparing `tempclone-1.0.0/PKG-INFO` & `tempclone-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-Metadata-Version: 2.1
-Name: tempclone
-Version: 1.0.0
-Summary: CLI to automate the creation of new projects from GitHub templates
-Home-page: https://github.com/yourusername/tempclone
-Author: Matheus
-Author-email: matheusmlfg@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: requests
-
-# Temp Clone
-
-Temp Clone is a command-line interface (CLI) tool to automate the creation of new projects from GitHub templates. This tool helps streamline the setup process for new projects by cloning from predefined templates.
-
-## Features
-
-- Configure GitHub access token and user nickname.
-- List available templates from a specified GitHub user or organization.
-- Create a new project repository from a selected template.
-- Automatically clone the newly created repository.
-
-## Installation
-
-You can install `tempclone` using `pip`:
-
-```bash
-pip install tempclone
+Metadata-Version: 2.1
+Name: tempclone
+Version: 1.0.1
+Summary: CLI to automate the creation of new projects from GitHub templates
+Home-page: https://github.com/yourusername/tempclone
+Author: Matheus
+Author-email: matheusmlfg@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Temp Clone
+
+Temp Clone is a command-line interface (CLI) tool to automate the creation of new projects from GitHub templates. This tool helps streamline the setup process for new projects by cloning from predefined templates.
+
+## Features
+
+- Configure GitHub access token and user nickname.
+- List available templates from a specified GitHub user or organization.
+- Create a new project repository from a selected template.
+- Automatically clone the newly created repository.
+
+## Installation
+
+You can install `tempclone` using `pip`:
+
+```bash
+pip install tempclone
+
+
```

### Comparing `tempclone-1.0.0/README.md` & `tempclone-1.0.1/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Temp Clone
-
-Temp Clone is a command-line interface (CLI) tool to automate the creation of new projects from GitHub templates. This tool helps streamline the setup process for new projects by cloning from predefined templates.
-
-## Features
-
-- Configure GitHub access token and user nickname.
-- List available templates from a specified GitHub user or organization.
-- Create a new project repository from a selected template.
-- Automatically clone the newly created repository.
-
-## Installation
-
-You can install `tempclone` using `pip`:
-
-```bash
-pip install tempclone
+# Temp Clone
+
+Temp Clone is a command-line interface (CLI) tool to automate the creation of new projects from GitHub templates. This tool helps streamline the setup process for new projects by cloning from predefined templates.
+
+## Features
+
+- Configure GitHub access token and user nickname.
+- List available templates from a specified GitHub user or organization.
+- Create a new project repository from a selected template.
+- Automatically clone the newly created repository.
+
+## Installation
+
+You can install `tempclone` using `pip`:
+
+```bash
+pip install tempclone
```

### Comparing `tempclone-1.0.0/setup.py` & `tempclone-1.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from setuptools import setup, find_packages
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setup(
-    name="tempclone",
-    version="1.0.0",
-    author="Matheus",
-    author_email="matheusmlfg@gmail.com",
-    description="CLI to automate the creation of new projects from GitHub templates",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/yourusername/tempclone",  # URL do repositório do seu projeto
-    packages=find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    install_requires=[
-        "click",
-        "requests"
-    ],
-    entry_points={
-        'console_scripts': [
-            'tempclone=tempclone.cli:cli',
-        ],
-    },
-)
+from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setup(
+    name="tempclone",
+    version="1.0.1",
+    author="Matheus",
+    author_email="matheusmlfg@gmail.com",
+    description="CLI to automate the creation of new projects from GitHub templates",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/yourusername/tempclone",  # URL do repositório do seu projeto
+    packages=find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.6',
+    install_requires=[
+        "click",
+        "requests"
+    ],
+    entry_points={
+        'console_scripts': [
+            'tempclone=tempclone.cli:cli',
+        ],
+    },
+)
```

### Comparing `tempclone-1.0.0/tempclone/cli.py` & `tempclone-1.0.1/tempclone/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-import click
-import requests
-import subprocess
-import os
-import json
-from pathlib import Path
-import time
-
-GITHUB_API_URL = "https://api.github.com"
-VERSION = "0.1.0"
-CONFIG_FILE = Path.home() / ".tempclone_config"
-
-ASCII_ART = r"""
- /$$$$$$$$ /$$$$$$$$ /$$      /$$ /$$$$$$$         /$$$$$$  /$$        /$$$$$$  /$$   /$$ /$$$$$$$$
-|__  $$__/| $$_____/| $$$    /$$$| $$__  $$       /$$__  $$| $$       /$$__  $$| $$$ | $$| $$_____/
-   | $$   | $$      | $$$$  /$$$$| $$  \ $$      | $$  \__/| $$      | $$  \ $$| $$$$| $$| $$      
-   | $$   | $$$$$   | $$ $$/$$ $$| $$$$$$$/      | $$      | $$      | $$  | $$| $$ $$ $$| $$$$$   
-   | $$   | $$__/   | $$  $$$| $$| $$____/       | $$      | $$      | $$  | $$| $$  $$$$| $$__/   
-   | $$   | $$      | $$\  $ | $$| $$            | $$    $$| $$      | $$  | $$| $$\  $$$| $$      
-   | $$   | $$$$$$$$| $$ \/  | $$| $$            |  $$$$$$/| $$$$$$$$|  $$$$$$/| $$ \  $$| $$$$$$$$
-   |__/   |________/|__/     |__/|__/             \______/ |________/ \______/ |__/  \__/|________/
-"""
-
-def get_config():
-    if CONFIG_FILE.exists():
-        try:
-            with open(CONFIG_FILE, "r") as file:
-                return json.load(file)
-        except json.JSONDecodeError:
-            return {}
-    else:
-        return {}
-
-def save_config(config):
-    with open(CONFIG_FILE, "w") as file:
-        json.dump(config, file)
-
-@click.group()
-@click.version_option(version=VERSION, prog_name="tempclone", message=ASCII_ART + f"\nVersion: {VERSION}")
-def cli():
-    """CLI to automate the creation of new projects from GitHub templates."""
-    pass
-
-@click.command()
-def configure():
-    """Configure GitHub access token and user nickname.
-
-    For more information on managing your personal access tokens, visit:
-    https://docs.github.com/en/authentication/
-    """
-    token = click.prompt('Please enter your GitHub access token', hide_input=True)
-    nickname = click.prompt('Please enter your GitHub nickname')
-    
-    config = get_config()
-    config['token'] = token
-    config['nickname'] = nickname
-    save_config(config)
-    click.echo("Configuration saved successfully.")
-
-@click.command()
-def list_templates():
-    """List available templates on GitHub."""
-    config = get_config()
-    token = config.get('token')
-    if not token:
-        click.echo("Token not found. Run 'tempclone configure' to set up your access token.")
-        return
-
-    headers = {
-        "Authorization": f"token {token}"
-    }
-    owner = click.prompt('Please enter the template repository owner (user or organization)', default=config.get('nickname'))
-
-    templates = []
-    page = 1
-    while True:
-        url = f"{GITHUB_API_URL}/users/{owner}/repos?page={page}&per_page=100"
-        click.echo(f"Fetching URL: {url}")  # Debug output
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            click.echo(f"Error listing templates: {response.json()}")
-            return
-
-        repos = response.json()
-        if not repos:
-            break
-
-        templates.extend([repo['name'] for repo in repos if repo.get('is_template')])
-        page += 1
-
-    click.echo("Available templates:")
-    for template in templates:
-        click.echo(f"- {template}")
-
-@click.command()
-@click.argument('new_repo_name')
-def new_project(new_repo_name):
-    """Create a new project from a template."""
-    config = get_config()
-    token = config.get('token')
-    if not token:
-        click.echo("Token not found. Run 'tempclone configure' to set up your access token.")
-        return
-
-    headers = {
-        "Authorization": f"token {token}",
-        "Accept": "application/vnd.github.baptiste-preview+json"
-    }
-
-    owner = click.prompt('Please enter the template repository owner (user or organization)', default=config.get('nickname'))
-    
-    templates = []
-    page = 1
-    while True:
-        url = f"{GITHUB_API_URL}/users/{owner}/repos?page={page}&per_page=100"
-        click.echo(f"Fetching URL: {url}")  # Debug output
-        response = requests.get(url, headers=headers)
-        if response.status_code != 200:
-            click.echo(f"Error listing templates: {response.json()}")
-            return
-
-        repos = response.json()
-        if not repos:
-            break
-
-        templates.extend([repo for repo in repos if repo.get('is_template')])
-        page += 1
-
-    click.echo("Available templates:")
-    for i, template in enumerate(templates, 1):
-        click.echo(f"{i}. {template['name']}")
-
-    template_index = click.prompt("Select the template by number", type=int)
-    template_repo = templates[template_index - 1]
-
-    new_repo_data = {
-        "owner": owner,
-        "name": new_repo_name,
-        "private": False  # or True if you want the repository to be private
-    }
-
-    create_url = f"{GITHUB_API_URL}/repos/{owner}/{template_repo['name']}/generate"
-    response = requests.post(create_url, headers=headers, json=new_repo_data)
-    
-    if response.status_code == 201:
-        new_repo = response.json()
-        new_repo_clone_url = new_repo['clone_url'].replace('.git', '')  # Remove .git extension
-        click.echo(f'New repository created: {new_repo_clone_url}')
-
-        # Pause and check if the repository is ready
-        click.echo('Waiting for the repository to be configured...')
-        time.sleep(5)  # Pause for 5 seconds
-
-        for _ in range(5):  # Try 5 times
-            click.echo(f'Checking repository status: {new_repo_clone_url}')  # Debug output
-            api_repo_url = new_repo_clone_url.replace('https://github.com/', 'https://api.github.com/repos/')
-            response = requests.get(api_repo_url, headers=headers)
-            if response.status_code == 200 and response.json().get('size') > 0:
-                break
-            click.echo('Waiting for the repository to be populated...')
-            time.sleep(10)
-
-        # Clone the new repository
-        click.echo(f'Cloning the repository: {new_repo_clone_url}')
-        subprocess.run(['git', 'clone', f"{new_repo_clone_url}.git", new_repo_name])
-
-        click.echo(f"Project {new_repo_name} successfully set up!")
-    else:
-        click.echo(f"Error creating repository: {response.json()}")
-
-cli.add_command(configure)
-cli.add_command(list_templates)
-cli.add_command(new_project)
-
-if __name__ == '__main__':
-    cli()
+import click
+import requests
+import subprocess
+import os
+import json
+from pathlib import Path
+import time
+
+GITHUB_API_URL = "https://api.github.com"
+VERSION = "1.0.1"
+CONFIG_FILE = Path.home() / ".tempclone_config"
+
+ASCII_ART = r"""
+ /$$$$$$$$ /$$$$$$$$ /$$      /$$ /$$$$$$$         /$$$$$$  /$$        /$$$$$$  /$$   /$$ /$$$$$$$$
+|__  $$__/| $$_____/| $$$    /$$$| $$__  $$       /$$__  $$| $$       /$$__  $$| $$$ | $$| $$_____/
+   | $$   | $$      | $$$$  /$$$$| $$  \ $$      | $$  \__/| $$      | $$  \ $$| $$$$| $$| $$      
+   | $$   | $$$$$   | $$ $$/$$ $$| $$$$$$$/      | $$      | $$      | $$  | $$| $$ $$ $$| $$$$$   
+   | $$   | $$__/   | $$  $$$| $$| $$____/       | $$      | $$      | $$  | $$| $$  $$$$| $$__/   
+   | $$   | $$      | $$\  $ | $$| $$            | $$    $$| $$      | $$  | $$| $$\  $$$| $$      
+   | $$   | $$$$$$$$| $$ \/  | $$| $$            |  $$$$$$/| $$$$$$$$|  $$$$$$/| $$ \  $$| $$$$$$$$
+   |__/   |________/|__/     |__/|__/             \______/ |________/ \______/ |__/  \__/|________/
+"""
+
+def get_config():
+    if CONFIG_FILE.exists():
+        try:
+            with open(CONFIG_FILE, "r") as file:
+                return json.load(file)
+        except json.JSONDecodeError:
+            return {}
+    else:
+        return {}
+
+def save_config(config):
+    with open(CONFIG_FILE, "w") as file:
+        json.dump(config, file)
+
+@click.group()
+@click.version_option(version=VERSION, prog_name="tempclone", message=ASCII_ART + f"\nVersion: {VERSION}")
+def cli():
+    """CLI to automate the creation of new projects from GitHub templates."""
+    pass
+
+@click.command()
+def configure():
+    """Configure GitHub access token and user nickname.
+
+    For more information on managing your personal access tokens, visit:
+    https://docs.github.com/en/authentication/
+    """
+    token = click.prompt('Please enter your GitHub access token', hide_input=True)
+    nickname = click.prompt('Please enter your GitHub nickname')
+    
+    config = get_config()
+    config['token'] = token
+    config['nickname'] = nickname
+    save_config(config)
+    click.echo("Configuration saved successfully.")
+
+@click.command()
+def list_templates():
+    """List available templates on GitHub."""
+    config = get_config()
+    token = config.get('token')
+    if not token:
+        click.echo("Token not found. Run 'tempclone configure' to set up your access token.")
+        return
+
+    headers = {
+        "Authorization": f"token {token}"
+    }
+    owner = click.prompt('Please enter the template repository owner (user or organization)', default=config.get('nickname'))
+
+    templates = []
+    page = 1
+    while True:
+        url = f"{GITHUB_API_URL}/users/{owner}/repos?page={page}&per_page=100"
+        click.echo(f"Fetching URL: {url}")  # Debug output
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            click.echo(f"Error listing templates: {response.json()}")
+            return
+
+        repos = response.json()
+        if not repos:
+            break
+
+        templates.extend([repo['name'] for repo in repos if repo.get('is_template')])
+        page += 1
+
+    click.echo("Available templates:")
+    for template in templates:
+        click.echo(f"- {template}")
+
+@click.command()
+@click.argument('new_repo_name')
+def new_project(new_repo_name):
+    """Create a new project from a template."""
+    config = get_config()
+    token = config.get('token')
+    if not token:
+        click.echo("Token not found. Run 'tempclone configure' to set up your access token.")
+        return
+
+    headers = {
+        "Authorization": f"token {token}",
+        "Accept": "application/vnd.github.baptiste-preview+json"
+    }
+
+    owner = click.prompt('Please enter the template repository owner (user or organization)', default=config.get('nickname'))
+    
+    templates = []
+    page = 1
+    while True:
+        url = f"{GITHUB_API_URL}/users/{owner}/repos?page={page}&per_page=100"
+        click.echo(f"Fetching URL: {url}")  # Debug output
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            click.echo(f"Error listing templates: {response.json()}")
+            return
+
+        repos = response.json()
+        if not repos:
+            break
+
+        templates.extend([repo for repo in repos if repo.get('is_template')])
+        page += 1
+
+    click.echo("Available templates:")
+    for i, template in enumerate(templates, 1):
+        click.echo(f"{i}. {template['name']}")
+
+    template_index = click.prompt("Select the template by number", type=int)
+    template_repo = templates[template_index - 1]
+
+    new_repo_data = {
+        "owner": owner,
+        "name": new_repo_name,
+        "private": False  # or True if you want the repository to be private
+    }
+
+    create_url = f"{GITHUB_API_URL}/repos/{owner}/{template_repo['name']}/generate"
+    response = requests.post(create_url, headers=headers, json=new_repo_data)
+    
+    if response.status_code == 201:
+        new_repo = response.json()
+        new_repo_clone_url = new_repo['clone_url'].replace('.git', '')  # Remove .git extension
+        click.echo(f'New repository created: {new_repo_clone_url}')
+
+        # Pause and check if the repository is ready
+        click.echo('Waiting for the repository to be configured...')
+        time.sleep(5)  # Pause for 5 seconds
+
+        for _ in range(5):  # Try 5 times
+            click.echo(f'Checking repository status: {new_repo_clone_url}')  # Debug output
+            api_repo_url = new_repo_clone_url.replace('https://github.com/', 'https://api.github.com/repos/')
+            response = requests.get(api_repo_url, headers=headers)
+            if response.status_code == 200 and response.json().get('size') > 0:
+                break
+            click.echo('Waiting for the repository to be populated...')
+            time.sleep(10)
+
+        # Clone the new repository
+        click.echo(f'Cloning the repository: {new_repo_clone_url}')
+        subprocess.run(['git', 'clone', f"{new_repo_clone_url}.git", new_repo_name])
+
+        click.echo(f"Project {new_repo_name} successfully set up!")
+    else:
+        click.echo(f"Error creating repository: {response.json()}")
+
+cli.add_command(configure)
+cli.add_command(list_templates)
+cli.add_command(new_project)
+
+if __name__ == '__main__':
+    cli()
```

### Comparing `tempclone-1.0.0/tempclone.egg-info/PKG-INFO` & `tempclone-1.0.1/tempclone.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-Metadata-Version: 2.1
-Name: tempclone
-Version: 1.0.0
-Summary: CLI to automate the creation of new projects from GitHub templates
-Home-page: https://github.com/yourusername/tempclone
-Author: Matheus
-Author-email: matheusmlfg@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: requests
-
-# Temp Clone
-
-Temp Clone is a command-line interface (CLI) tool to automate the creation of new projects from GitHub templates. This tool helps streamline the setup process for new projects by cloning from predefined templates.
-
-## Features
-
-- Configure GitHub access token and user nickname.
-- List available templates from a specified GitHub user or organization.
-- Create a new project repository from a selected template.
-- Automatically clone the newly created repository.
-
-## Installation
-
-You can install `tempclone` using `pip`:
-
-```bash
-pip install tempclone
+Metadata-Version: 2.1
+Name: tempclone
+Version: 1.0.1
+Summary: CLI to automate the creation of new projects from GitHub templates
+Home-page: https://github.com/yourusername/tempclone
+Author: Matheus
+Author-email: matheusmlfg@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Temp Clone
+
+Temp Clone is a command-line interface (CLI) tool to automate the creation of new projects from GitHub templates. This tool helps streamline the setup process for new projects by cloning from predefined templates.
+
+## Features
+
+- Configure GitHub access token and user nickname.
+- List available templates from a specified GitHub user or organization.
+- Create a new project repository from a selected template.
+- Automatically clone the newly created repository.
+
+## Installation
+
+You can install `tempclone` using `pip`:
+
+```bash
+pip install tempclone
+
+
```

### Comparing `tempclone-1.0.0/tests/test_cli.py` & `tempclone-1.0.1/tests/test_cli.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import pytest
-from click.testing import CliRunner
-import requests_mock
-import subprocess
-from tempclone.cli import cli, get_config, save_config
-
-@pytest.fixture
-def runner():
-    return CliRunner()
-
-@pytest.fixture
-def mock_config(monkeypatch):
-    config = {
-        'token': 'fake_token',
-        'nickname': 'fake_user'
-    }
-    monkeypatch.setattr('tempclone.cli.get_config', lambda: config)
-    return config
-
-def test_configure(runner):
-    result = runner.invoke(cli, ['configure'], input='fake_token\nfake_user\n')
-    assert result.exit_code == 0
-    assert "Configuration saved successfully." in result.output
-
-def test_list_templates(runner, mock_config):
-    with requests_mock.Mocker() as m:
-        m.get('https://api.github.com/users/fake_user/repos?page=1&per_page=100', json=[
-            {'name': 'template1', 'is_template': True},
-            {'name': 'template2', 'is_template': True},
-            {'name': 'not_a_template', 'is_template': False},
-        ])
-        m.get('https://api.github.com/users/fake_user/repos?page=2&per_page=100', json=[])
-        result = runner.invoke(cli, ['list-templates'])
-        print(result.output)  # Debug output
-        assert result.exit_code == 0
-        assert "template1" in result.output
-        assert "template2" in result.output
-        assert "not_a_template" not in result.output
-
-def test_new_project(runner, mock_config, monkeypatch):
-    with requests_mock.Mocker() as m:
-        m.get('https://api.github.com/users/fake_user/repos?page=1&per_page=100', json=[
-            {'name': 'template1', 'is_template': True},
-        ])
-        m.get('https://api.github.com/users/fake_user/repos?page=2&per_page=100', json=[])
-        m.post('https://api.github.com/repos/fake_user/template1/generate', json={
-            'clone_url': 'https://github.com/fake_user/new_project'
-        }, status_code=201)
-        m.get('https://api.github.com/repos/fake_user/new_project', json={
-            'size': 1
-        })
-
-        def mock_subprocess_run(*args, **kwargs):
-            print(f"Mocked subprocess.run called with: {args}")
-            return subprocess.CompletedProcess(args, 0)
-        
-        monkeypatch.setattr(subprocess, 'run', mock_subprocess_run)
-        
-        result = runner.invoke(cli, ['new-project', 'new_project'], input='fake_user\n1\n')
-        print(result.output)  # Debug output
-        assert result.exit_code == 0
-        assert "New repository created" in result.output
-        assert "https://github.com/fake_user/new_project" in result.output
-        assert "Project new_project successfully set up!" in result.output
+import pytest
+from click.testing import CliRunner
+import requests_mock
+import subprocess
+from tempclone.cli import cli, get_config, save_config
+
+@pytest.fixture
+def runner():
+    return CliRunner()
+
+@pytest.fixture
+def mock_config(monkeypatch):
+    config = {
+        'token': 'fake_token',
+        'nickname': 'fake_user'
+    }
+    monkeypatch.setattr('tempclone.cli.get_config', lambda: config)
+    return config
+
+def test_configure(runner):
+    result = runner.invoke(cli, ['configure'], input='fake_token\nfake_user\n')
+    assert result.exit_code == 0
+    assert "Configuration saved successfully." in result.output
+
+def test_list_templates(runner, mock_config):
+    with requests_mock.Mocker() as m:
+        m.get('https://api.github.com/users/fake_user/repos?page=1&per_page=100', json=[
+            {'name': 'template1', 'is_template': True},
+            {'name': 'template2', 'is_template': True},
+            {'name': 'not_a_template', 'is_template': False},
+        ])
+        m.get('https://api.github.com/users/fake_user/repos?page=2&per_page=100', json=[])
+        result = runner.invoke(cli, ['list-templates'])
+        print(result.output)  # Debug output
+        assert result.exit_code == 0
+        assert "template1" in result.output
+        assert "template2" in result.output
+        assert "not_a_template" not in result.output
+
+def test_new_project(runner, mock_config, monkeypatch):
+    with requests_mock.Mocker() as m:
+        m.get('https://api.github.com/users/fake_user/repos?page=1&per_page=100', json=[
+            {'name': 'template1', 'is_template': True},
+        ])
+        m.get('https://api.github.com/users/fake_user/repos?page=2&per_page=100', json=[])
+        m.post('https://api.github.com/repos/fake_user/template1/generate', json={
+            'clone_url': 'https://github.com/fake_user/new_project'
+        }, status_code=201)
+        m.get('https://api.github.com/repos/fake_user/new_project', json={
+            'size': 1
+        })
+
+        def mock_subprocess_run(*args, **kwargs):
+            print(f"Mocked subprocess.run called with: {args}")
+            return subprocess.CompletedProcess(args, 0)
+        
+        monkeypatch.setattr(subprocess, 'run', mock_subprocess_run)
+        
+        result = runner.invoke(cli, ['new-project', 'new_project'], input='fake_user\n1\n')
+        print(result.output)  # Debug output
+        assert result.exit_code == 0
+        assert "New repository created" in result.output
+        assert "https://github.com/fake_user/new_project" in result.output
+        assert "Project new_project successfully set up!" in result.output
```

