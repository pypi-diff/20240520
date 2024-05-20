# Comparing `tmp/aws_stuff_doer-0.1.0.tar.gz` & `tmp/aws_stuff_doer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_stuff_doer-0.1.0.tar", max compression
+gzip compressed data, was "aws_stuff_doer-0.1.1.tar", max compression
```

## Comparing `aws_stuff_doer-0.1.0.tar` & `aws_stuff_doer-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,5 @@
--rw-r--r--   0        0        0     1062 2024-02-14 22:48:24.540834 aws_stuff_doer-0.1.0/LICENSE
--rw-r--r--   0        0        0     2280 2024-02-14 22:48:24.540834 aws_stuff_doer-0.1.0/README.md
--rw-r--r--   0        0        0      807 2024-02-14 22:48:24.540834 aws_stuff_doer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       27 2024-02-14 22:48:24.540834 aws_stuff_doer-0.1.0/src/aws_stuff_doer/__init__.py
--rw-r--r--   0        0        0     8333 2024-02-14 22:48:24.540834 aws_stuff_doer-0.1.0/src/aws_stuff_doer/aws_stuff_doer.py
--rw-r--r--   0        0        0       36 2024-02-14 22:48:24.540834 aws_stuff_doer-0.1.0/src/aws_stuff_doer/pipeline/__init__.py
--rwxr-xr-x   0        0        0     6710 2024-02-14 22:48:24.540834 aws_stuff_doer-0.1.0/src/aws_stuff_doer/pipeline/cloudformation.py
--rw-r--r--   0        0        0     2365 2024-02-14 22:48:24.540834 aws_stuff_doer-0.1.0/src/aws_stuff_doer/pipeline/command_handler.py
--rw-r--r--   0        0        0     5584 2024-02-14 22:48:24.540834 aws_stuff_doer-0.1.0/src/aws_stuff_doer/pipeline/synth.py
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 aws_stuff_doer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-02-17 18:46:32.476469 aws_stuff_doer-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1770 2024-05-20 00:17:33.839532 aws_stuff_doer-0.1.1/README.md
+-rw-r--r--   0        0        0     1662 2024-05-20 00:13:26.495936 aws_stuff_doer-0.1.1/main.py
+-rw-r--r--   0        0        0      871 2024-05-20 01:06:40.734715 aws_stuff_doer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 aws_stuff_doer-0.1.1/PKG-INFO
```

### Comparing `aws_stuff_doer-0.1.0/LICENSE` & `aws_stuff_doer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_stuff_doer-0.1.0/README.md` & `aws_stuff_doer-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,43 @@
-# aws-stuff-doer: an inteactive CLI to help manage your AWS projects and sso sessions.
+# aws-stuff-doer: An Interactive CLI to Manage Your AWS Projects and SSO Sessions
 
 [![PyPI version](https://badge.fury.io/py/aws-stuff-doer.svg)](https://badge.fury.io/py/aws-stuff-doer)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-ASD is a simple and effective tool for managing AWS Single Sign-On (SSO). Tailored for both developers and administrators, ASD offers an easy way to streamline your AWS SSO process, including running custom shell commands with specific profiles and exporting temporary AWS credentials.
+**AWS Stuff Doer (ASD)** is your go-to tool for managing AWS Single Sign-On (SSO). Designed for both developers and administrators, ASD simplifies your AWS SSO workflow, allowing you to run custom shell commands with specific profiles and export temporary AWS credentials seamlessly.
 
 ## Features
 
-- **Easy Integration**: Seamlessly integrate with existing AWS infrastructure.
-- **Secure Authentication**: Enhance security with robust SSO capabilities.
-- **Customizable**: Extend and adapt ASD to suit your specific needs.
-- **Run Custom Commands**: Execute shell commands with AWS profiles and export temporary credentials in memory.
+- **Easy Integration**: Effortlessly integrate with your existing AWS infrastructure.
+- **Secure Authentication**: Improve security with robust SSO capabilities.
+- **Customizable**: Tailor ASD to meet your unique requirements.
+- **Run Custom Commands**: Execute shell commands using AWS profiles and export temporary credentials securely in memory.
 - **Temporary AWS Credentials**: Access temporary AWS credentials specific to a profile, securely available in memory.
 
 ## Installation
 
-You can install ASD via pip:
+Install ASD using pip:
 
 ```bash
 pip install aws-stuff-doer
 ```
-```
 
 ## Usage
 
-Getting started with ASD is easy:
-
-To generate temporary AWS credentials for a specific profile:
-```bash
-asd -p <profile_name>
-```
-This will generate temporary AWS credentials for the specified profile and store them in the ~/.aws/credentials file.
-
-To open your AWS console in a browser session:
-```bash
-asd <your_command_here> --profile <profile_name> --console
-```
+Invoke ASD with the following command syntax:
 
-To get help:
-```bash
-asd --help
-```
-or
 ```bash
-go see a therapist.
+asd [-h] [-p PROFILE] [--open-sso] [--open] [-l] [--version] [command ...]
 ```
 
-The project is available on [pypip](https://pypi.org/project/aws-stuff-doer/).
-
-## Contributing
-
-Contributions are welcome! Check out the [issues](https://github.com/aphexlog/aws-stuff-doer/issues) or submit a pull request.
-
-## License
-
-aws-stuff-doer is released under the [MIT License](https://github.com/aphexlog/aws-stuff-doer/blob/main/LICENSE).
-
----
-
-Feel free to reach out with questions, suggestions, or just to say hello. Happy coding!
-
-## Contact Information
-- **Author**: Aaron West
-- **Email**: aphexlog@gmail.com
+**ASD**: The AWS Utility to manage AWS SSO and AWS CLI profiles conveniently.
 
----
+### Positional Arguments:
+- **command**: Command followed by its arguments to run in the shell
 
-Thank you for your interest in aws-stuff-doer! Follow the project on [GitHub](https://github.com/aphexlog/aws-stuff-doer) for the latest updates...
+### Options:
+- **-h, --help**: Show this help message and exit
+- **-p PROFILE, --profile PROFILE**: Specify AWS profile name
+- **--open-sso**: Open AWS SSO user console
+- **--open**: Open AWS account console
+- **-l, --list**: List available profiles
+- **--version**: Show program's version number and exit
```

### Comparing `aws_stuff_doer-0.1.0/pyproject.toml` & `aws_stuff_doer-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "aws-stuff-doer"
-version = "0.1.0"
+version = "0.1.1"
 description = "ASD is a utility to help manage your AWS projects and sso sessions."
-authors = ["Aaron West <aphexlog@gmail.com>"]
+authors = ["Aaron West <aphexlog@gmail.com>", "ant <anthony.chiarello132@gmail.com>"]
 repository = "https://github.com/aphexlog/aws-stuff-doer"
 license = "MIT"
 readme = "README.md"
+packages = [{ from = ".", include = "main.py" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 boto3 = "^1.34.36"
 gitpython = "^3.1.41"
 aws-cdk-lib = "^2.126.0"
 boto3-stubs = "^1.34.36"
 setuptools = "^69.0.3"
 
 [tool.poetry.scripts]
-asd = "aws_stuff_doer.aws_stuff_doer:main"
+asd = "main:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

