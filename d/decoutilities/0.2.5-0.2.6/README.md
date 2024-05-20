# Comparing `tmp/decoutilities-0.2.5.tar.gz` & `tmp/decoutilities-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.5.tar", last modified: Mon May 20 11:41:38 2024, max compression
+gzip compressed data, was "decoutilities-0.2.6.tar", last modified: Mon May 20 11:57:12 2024, max compression
```

## Comparing `decoutilities-0.2.5.tar` & `decoutilities-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.395916 decoutilities-0.2.5/
--rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.2.5/LICENSE
--rw-rw-rw-   0        0        0    12193 2024-05-20 11:41:38.351916 decoutilities-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    11722 2024-05-20 10:37:54.000000 decoutilities-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:37.663917 decoutilities-0.2.5/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.5/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:37.952917 decoutilities-0.2.5/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.5/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.5/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.5/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.065916 decoutilities-0.2.5/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.5/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.5/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.5/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.108918 decoutilities-0.2.5/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.5/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.2.5/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.136917 decoutilities-0.2.5/decoutilities/logger/
--rw-rw-rw-   0        0        0     1212 2024-05-20 11:36:36.000000 decoutilities-0.2.5/decoutilities/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.197917 decoutilities-0.2.5/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.5/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.223918 decoutilities-0.2.5/decoutilities/textUtils/
--rw-rw-rw-   0        0        0     2427 2024-05-20 10:37:30.000000 decoutilities-0.2.5/decoutilities/textUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:38.249918 decoutilities-0.2.5/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    12193 2024-05-20 11:41:36.000000 decoutilities-0.2.5/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-20 11:41:37.000000 decoutilities-0.2.5/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 11:41:36.000000 decoutilities-0.2.5/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-20 11:41:36.000000 decoutilities-0.2.5/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 11:41:38.396917 decoutilities-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-20 10:38:59.000000 decoutilities-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.375856 decoutilities-0.2.6/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0    15668 2024-05-20 11:57:12.360853 decoutilities-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    15197 2024-05-20 11:56:43.000000 decoutilities-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.018468 decoutilities-0.2.6/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.6/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.171467 decoutilities-0.2.6/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.6/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.6/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.6/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.225471 decoutilities-0.2.6/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.6/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.6/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.6/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.266468 decoutilities-0.2.6/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.6/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.2.6/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.282856 decoutilities-0.2.6/decoutilities/logger/
+-rw-rw-rw-   0        0        0     1212 2024-05-20 11:36:36.000000 decoutilities-0.2.6/decoutilities/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.314856 decoutilities-0.2.6/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.6/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.326855 decoutilities-0.2.6/decoutilities/textUtils/
+-rw-rw-rw-   0        0        0     2427 2024-05-20 10:37:30.000000 decoutilities-0.2.6/decoutilities/textUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.346855 decoutilities-0.2.6/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    15668 2024-05-20 11:57:11.000000 decoutilities-0.2.6/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-20 11:57:11.000000 decoutilities-0.2.6/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 11:57:11.000000 decoutilities-0.2.6/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 11:57:11.000000 decoutilities-0.2.6/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 11:57:12.376853 decoutilities-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-20 11:56:57.000000 decoutilities-0.2.6/setup.py
```

### Comparing `decoutilities-0.2.5/LICENSE` & `decoutilities-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/PKG-INFO` & `decoutilities-0.2.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: decoutilities
-Version: 0.2.5
-Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
-Author: Hugo Torres
-Author-email: contact@redactado.es
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # decoutilities
 
 A simple python package that allows using decorators for multiple things like easily setting up singleton or config files.
 
 ## Installation
 
 You can install `decoutilities` using pip:
@@ -381,14 +368,100 @@
 
 The key generation process in `keyManager` is designed to be secure. It uses a large random number as the basis for the key, which makes it difficult for an attacker to guess. The length of the key also contributes to its security. The longer the key, the more possible combinations there are, making it harder for an attacker to crack.
 
 ### Notes
 
 This module uses XOR encryption, which is not secure for most practical uses. It is recommended to use a more secure encryption algorithm for any data that needs protection in the real world.
 
+## Text Utilities
+
+The `textUtils` class provides methods for formatting and decorating text in the console. It includes methods for coloring text, adding decorations such as bold, underline, and italic, and a general format method that replaces aliases with their corresponding ANSI escape codes.
+
+### Usage
+
+To use this class, you first need to create an instance of `textUtils`:
+
+```python
+text_utils = textUtils()
+```
+
+You can then use the `color`, `decorate`, and `format` methods to format your text:
+
+```python
+# Color text
+colored_text = text_utils.color('red', 'Hello, World!')
+
+# Decorate text
+bold_text = text_utils.decorate('bold', 'Hello, World!')
+
+# Format text
+formatted_text = text_utils.format('bold red Hello, World!')
+```
+
+### Methods
+
+- `color(color, text)`: Colors the text with the specified color. The available colors are: red, green, yellow, blue, purple, cyan, white, dark_red, dark_green, gold, gray, dark_gray, black, and reset.
+
+- `decorate(decoration, text)`: Decorates the text with the specified decoration. The available decorations are: bold, underline, and italic.
+
+- `format(text)`: Replaces aliases in the text with their corresponding ANSI escape codes. The available aliases are the same as the colors and decorations listed above.
+
+### Notes
+
+The `format` method applies the ANSI escape codes in the order they appear in the text. If the same alias appears multiple times in the text, all instances will be replaced. The `reset` alias resets all formatting, so it can be used to stop the effect of a previous alias.
+
+## Logger
+
+The `Logger` class provides methods for logging events and messages with different levels of severity. It includes methods for logging info, warning, error, success, debug, and announcement messages. The messages can be formatted using the `textUtils` class and can optionally be written to a log file.
+
+### Usage
+
+To use this class, you first need to create an instance of `Logger`:
+
+```python
+logger = Logger(prefix='MyApp', debug=True, log='app.log')
+```
+
+You can then use the `info`, `warning`, `error`, `success`, `debug`, and `announce` methods to log messages:
+
+```python
+# Log an info message
+logger.info('This is an info message.')
+
+# Log a warning message
+logger.warning('This is a warning message.')
+
+# Log an error message
+logger.error('This is an error message.')
+
+# Log a success message
+logger.success('This is a success message.')
+
+# Log a debug message
+logger.debug('This is a debug message.')
+
+# Log an announcement
+logger.announce('This is an announcement.')
+```
+
+### Methods
+
+- `info(message)`: Logs an info message.
+- `warning(message)`: Logs a warning message.
+- `error(message)`: Logs an error message.
+- `success(message)`: Logs a success message.
+- `debug(message)`: Logs a debug message if the `debug` attribute of the `Logger` instance is `True`.
+- `announce(message)`: Logs an announcement.
+
+### Notes
+
+The `Logger` class uses the `textUtils` class to format the messages. The format of the messages can be specified when creating a `Logger` instance with the `format` parameter. The `{event}` placeholder in the format string is replaced with the event type (e.g., "INFO", "WARNING"), and the `{message}` placeholder is replaced with the actual message.
+
+If a `log` parameter is provided when creating a `Logger` instance, the logged messages will also be written to the specified log file.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
@@ -409,8 +482,8 @@
 - FEATURE: For new features, include a explanation mentioning why it should be inside `decoutilities`.
 - BUGFIX: For general bugfixes.
 - SECURITY: For fixes related with security issues.
 - QoL: For QoL improvements
 
 ## Author
 
-- [Hugo Torres](https://github.com/Reddishye)
+- [Hugo Torres](https://github.com/Reddishye)
```

### Comparing `decoutilities-0.2.5/README.md` & `decoutilities-0.2.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: decoutilities
+Version: 0.2.6
+Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
+Author: Hugo Torres
+Author-email: contact@redactado.es
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # decoutilities
 
 A simple python package that allows using decorators for multiple things like easily setting up singleton or config files.
 
 ## Installation
 
 You can install `decoutilities` using pip:
@@ -368,14 +381,100 @@
 
 The key generation process in `keyManager` is designed to be secure. It uses a large random number as the basis for the key, which makes it difficult for an attacker to guess. The length of the key also contributes to its security. The longer the key, the more possible combinations there are, making it harder for an attacker to crack.
 
 ### Notes
 
 This module uses XOR encryption, which is not secure for most practical uses. It is recommended to use a more secure encryption algorithm for any data that needs protection in the real world.
 
+## Text Utilities
+
+The `textUtils` class provides methods for formatting and decorating text in the console. It includes methods for coloring text, adding decorations such as bold, underline, and italic, and a general format method that replaces aliases with their corresponding ANSI escape codes.
+
+### Usage
+
+To use this class, you first need to create an instance of `textUtils`:
+
+```python
+text_utils = textUtils()
+```
+
+You can then use the `color`, `decorate`, and `format` methods to format your text:
+
+```python
+# Color text
+colored_text = text_utils.color('red', 'Hello, World!')
+
+# Decorate text
+bold_text = text_utils.decorate('bold', 'Hello, World!')
+
+# Format text
+formatted_text = text_utils.format('bold red Hello, World!')
+```
+
+### Methods
+
+- `color(color, text)`: Colors the text with the specified color. The available colors are: red, green, yellow, blue, purple, cyan, white, dark_red, dark_green, gold, gray, dark_gray, black, and reset.
+
+- `decorate(decoration, text)`: Decorates the text with the specified decoration. The available decorations are: bold, underline, and italic.
+
+- `format(text)`: Replaces aliases in the text with their corresponding ANSI escape codes. The available aliases are the same as the colors and decorations listed above.
+
+### Notes
+
+The `format` method applies the ANSI escape codes in the order they appear in the text. If the same alias appears multiple times in the text, all instances will be replaced. The `reset` alias resets all formatting, so it can be used to stop the effect of a previous alias.
+
+## Logger
+
+The `Logger` class provides methods for logging events and messages with different levels of severity. It includes methods for logging info, warning, error, success, debug, and announcement messages. The messages can be formatted using the `textUtils` class and can optionally be written to a log file.
+
+### Usage
+
+To use this class, you first need to create an instance of `Logger`:
+
+```python
+logger = Logger(prefix='MyApp', debug=True, log='app.log')
+```
+
+You can then use the `info`, `warning`, `error`, `success`, `debug`, and `announce` methods to log messages:
+
+```python
+# Log an info message
+logger.info('This is an info message.')
+
+# Log a warning message
+logger.warning('This is a warning message.')
+
+# Log an error message
+logger.error('This is an error message.')
+
+# Log a success message
+logger.success('This is a success message.')
+
+# Log a debug message
+logger.debug('This is a debug message.')
+
+# Log an announcement
+logger.announce('This is an announcement.')
+```
+
+### Methods
+
+- `info(message)`: Logs an info message.
+- `warning(message)`: Logs a warning message.
+- `error(message)`: Logs an error message.
+- `success(message)`: Logs a success message.
+- `debug(message)`: Logs a debug message if the `debug` attribute of the `Logger` instance is `True`.
+- `announce(message)`: Logs an announcement.
+
+### Notes
+
+The `Logger` class uses the `textUtils` class to format the messages. The format of the messages can be specified when creating a `Logger` instance with the `format` parameter. The `{event}` placeholder in the format string is replaced with the event type (e.g., "INFO", "WARNING"), and the `{message}` placeholder is replaced with the actual message.
+
+If a `log` parameter is provided when creating a `Logger` instance, the logged messages will also be written to the specified log file.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
@@ -396,8 +495,8 @@
 - FEATURE: For new features, include a explanation mentioning why it should be inside `decoutilities`.
 - BUGFIX: For general bugfixes.
 - SECURITY: For fixes related with security issues.
 - QoL: For QoL improvements
 
 ## Author
 
-- [Hugo Torres](https://github.com/Reddishye)
+- [Hugo Torres](https://github.com/Reddishye)
```

### Comparing `decoutilities-0.2.5/decoutilities/__init__.py` & `decoutilities-0.2.6/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/decoutilities/config/config.py` & `decoutilities-0.2.6/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/decoutilities/config/configContainer.py` & `decoutilities-0.2.6/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/decoutilities/data/dataEncryptor.py` & `decoutilities-0.2.6/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/decoutilities/data/keyManager.py` & `decoutilities-0.2.6/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/decoutilities/inject/injector.py` & `decoutilities-0.2.6/decoutilities/inject/injector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/decoutilities/logger/__init__.py` & `decoutilities-0.2.6/decoutilities/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/decoutilities/queue/__init__.py` & `decoutilities-0.2.6/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/decoutilities/textUtils/__init__.py` & `decoutilities-0.2.6/decoutilities/textUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.2.6/decoutilities.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.5
+Version: 0.2.6
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -381,14 +381,100 @@
 
 The key generation process in `keyManager` is designed to be secure. It uses a large random number as the basis for the key, which makes it difficult for an attacker to guess. The length of the key also contributes to its security. The longer the key, the more possible combinations there are, making it harder for an attacker to crack.
 
 ### Notes
 
 This module uses XOR encryption, which is not secure for most practical uses. It is recommended to use a more secure encryption algorithm for any data that needs protection in the real world.
 
+## Text Utilities
+
+The `textUtils` class provides methods for formatting and decorating text in the console. It includes methods for coloring text, adding decorations such as bold, underline, and italic, and a general format method that replaces aliases with their corresponding ANSI escape codes.
+
+### Usage
+
+To use this class, you first need to create an instance of `textUtils`:
+
+```python
+text_utils = textUtils()
+```
+
+You can then use the `color`, `decorate`, and `format` methods to format your text:
+
+```python
+# Color text
+colored_text = text_utils.color('red', 'Hello, World!')
+
+# Decorate text
+bold_text = text_utils.decorate('bold', 'Hello, World!')
+
+# Format text
+formatted_text = text_utils.format('bold red Hello, World!')
+```
+
+### Methods
+
+- `color(color, text)`: Colors the text with the specified color. The available colors are: red, green, yellow, blue, purple, cyan, white, dark_red, dark_green, gold, gray, dark_gray, black, and reset.
+
+- `decorate(decoration, text)`: Decorates the text with the specified decoration. The available decorations are: bold, underline, and italic.
+
+- `format(text)`: Replaces aliases in the text with their corresponding ANSI escape codes. The available aliases are the same as the colors and decorations listed above.
+
+### Notes
+
+The `format` method applies the ANSI escape codes in the order they appear in the text. If the same alias appears multiple times in the text, all instances will be replaced. The `reset` alias resets all formatting, so it can be used to stop the effect of a previous alias.
+
+## Logger
+
+The `Logger` class provides methods for logging events and messages with different levels of severity. It includes methods for logging info, warning, error, success, debug, and announcement messages. The messages can be formatted using the `textUtils` class and can optionally be written to a log file.
+
+### Usage
+
+To use this class, you first need to create an instance of `Logger`:
+
+```python
+logger = Logger(prefix='MyApp', debug=True, log='app.log')
+```
+
+You can then use the `info`, `warning`, `error`, `success`, `debug`, and `announce` methods to log messages:
+
+```python
+# Log an info message
+logger.info('This is an info message.')
+
+# Log a warning message
+logger.warning('This is a warning message.')
+
+# Log an error message
+logger.error('This is an error message.')
+
+# Log a success message
+logger.success('This is a success message.')
+
+# Log a debug message
+logger.debug('This is a debug message.')
+
+# Log an announcement
+logger.announce('This is an announcement.')
+```
+
+### Methods
+
+- `info(message)`: Logs an info message.
+- `warning(message)`: Logs a warning message.
+- `error(message)`: Logs an error message.
+- `success(message)`: Logs a success message.
+- `debug(message)`: Logs a debug message if the `debug` attribute of the `Logger` instance is `True`.
+- `announce(message)`: Logs an announcement.
+
+### Notes
+
+The `Logger` class uses the `textUtils` class to format the messages. The format of the messages can be specified when creating a `Logger` instance with the `format` parameter. The `{event}` placeholder in the format string is replaced with the event type (e.g., "INFO", "WARNING"), and the `{message}` placeholder is replaced with the actual message.
+
+If a `log` parameter is provided when creating a `Logger` instance, the logged messages will also be written to the specified log file.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
```

### Comparing `decoutilities-0.2.5/decoutilities.egg-info/SOURCES.txt` & `decoutilities-0.2.6/decoutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.5/setup.py` & `decoutilities-0.2.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.5',
+version='0.2.6',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

