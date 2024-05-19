# Comparing `tmp/mo-parsing-8.6.21337.tar.gz` & `tmp/mo_parsing-8.639.24140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-parsing-8.6.21337.tar", last modified: Fri Dec  3 13:44:41 2021, max compression
+gzip compressed data, was "mo_parsing-8.639.24140.tar", last modified: Sun May 19 22:36:51 2024, max compression
```

## Comparing `mo-parsing-8.6.21337.tar` & `mo_parsing-8.639.24140.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-12-03 13:44:41.600689 mo-parsing-8.6.21337/
--rw-rw-rw-   0        0        0     1023 2019-10-01 00:43:04.000000 mo-parsing-8.6.21337/LICENSE
--rw-rw-rw-   0        0        0     8516 2021-12-03 13:44:41.600689 mo-parsing-8.6.21337/PKG-INFO
--rw-rw-rw-   0        0        0     6701 2021-11-20 14:07:33.000000 mo-parsing-8.6.21337/README.md
-drwxrwxrwx   0        0        0        0 2021-12-03 13:44:41.579491 mo-parsing-8.6.21337/mo_parsing/
--rw-rw-rw-   0        0        0     2732 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/__init__.py
--rw-rw-rw-   0        0        0    25527 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/core.py
--rw-rw-rw-   0        0        0     2989 2021-11-23 00:49:40.000000 mo-parsing-8.6.21337/mo_parsing/debug.py
--rw-rw-rw-   0        0        0    29279 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/enhancement.py
--rw-rw-rw-   0        0        0     5385 2021-11-20 14:07:33.000000 mo-parsing-8.6.21337/mo_parsing/exceptions.py
--rw-rw-rw-   0        0        0    25413 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/expressions.py
--rw-rw-rw-   0        0        0    31835 2021-10-30 18:24:02.000000 mo-parsing-8.6.21337/mo_parsing/helpers.py
--rw-rw-rw-   0        0        0    12894 2021-11-16 18:07:06.000000 mo-parsing-8.6.21337/mo_parsing/infix.py
--rw-rw-rw-   0        0        0     3125 2021-10-30 18:24:02.000000 mo-parsing-8.6.21337/mo_parsing/profile.py
--rw-rw-rw-   0        0        0    10120 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/regex.py
--rw-rw-rw-   0        0        0    13735 2021-12-03 13:44:36.000000 mo-parsing-8.6.21337/mo_parsing/results.py
--rw-rw-rw-   0        0        0    23879 2021-11-22 23:33:23.000000 mo-parsing-8.6.21337/mo_parsing/tokens.py
--rw-rw-rw-   0        0        0    17765 2021-12-03 13:44:36.000000 mo-parsing-8.6.21337/mo_parsing/utils.py
--rw-rw-rw-   0        0        0     6116 2021-10-30 18:24:02.000000 mo-parsing-8.6.21337/mo_parsing/whitespaces.py
-drwxrwxrwx   0        0        0        0 2021-12-03 13:44:41.590093 mo-parsing-8.6.21337/mo_parsing.egg-info/
--rw-rw-rw-   0        0        0     8516 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-12-03 13:44:41.000000 mo-parsing-8.6.21337/mo_parsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-12-03 13:44:41.600689 mo-parsing-8.6.21337/setup.cfg
--rw-rw-rw-   0        0        0     7564 2021-12-03 13:44:36.000000 mo-parsing-8.6.21337/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:36:51.561325 mo_parsing-8.639.24140/
+-rw-rw-rw-   0        0        0     1023 2019-10-01 00:43:04.000000 mo_parsing-8.639.24140/LICENSE
+-rw-rw-rw-   0        0        0     7824 2024-05-19 22:36:51.560325 mo_parsing-8.639.24140/PKG-INFO
+-rw-rw-rw-   0        0        0     6582 2024-04-03 00:06:27.000000 mo_parsing-8.639.24140/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 22:36:51.548293 mo_parsing-8.639.24140/mo_parsing/
+-rw-rw-rw-   0        0        0     2970 2024-04-03 00:08:27.000000 mo_parsing-8.639.24140/mo_parsing/__init__.py
+-rw-rw-rw-   0        0        0    26520 2024-04-03 00:08:27.000000 mo_parsing-8.639.24140/mo_parsing/core.py
+-rw-rw-rw-   0        0        0     3281 2022-12-28 00:45:47.000000 mo_parsing-8.639.24140/mo_parsing/debug.py
+-rw-rw-rw-   0        0        0    29257 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/enhancement.py
+-rw-rw-rw-   0        0        0     6015 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/exceptions.py
+-rw-rw-rw-   0        0        0    26465 2023-12-26 14:01:39.000000 mo_parsing-8.639.24140/mo_parsing/expressions.py
+-rw-rw-rw-   0        0        0    31918 2022-12-04 23:23:35.000000 mo_parsing-8.639.24140/mo_parsing/helpers.py
+-rw-rw-rw-   0        0        0    12851 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/infix.py
+-rw-rw-rw-   0        0        0     3125 2022-12-04 23:23:36.000000 mo_parsing-8.639.24140/mo_parsing/profile.py
+-rw-rw-rw-   0        0        0    10153 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/regex.py
+-rw-rw-rw-   0        0        0    12064 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/results.py
+-rw-rw-rw-   0        0        0    24539 2023-12-26 14:01:39.000000 mo_parsing-8.639.24140/mo_parsing/tokens.py
+-rw-rw-rw-   0        0        0    16529 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/utils.py
+-rw-rw-rw-   0        0        0     6212 2023-11-26 15:19:47.000000 mo_parsing-8.639.24140/mo_parsing/whitespaces.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:36:51.559315 mo_parsing-8.639.24140/mo_parsing.egg-info/
+-rw-rw-rw-   0        0        0     7824 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 22:36:51.561325 mo_parsing-8.639.24140/setup.cfg
+-rw-rw-rw-   0        0        0     7815 2024-05-19 22:36:46.000000 mo_parsing-8.639.24140/setup.py
```

### Comparing `mo-parsing-8.6.21337/LICENSE` & `mo_parsing-8.639.24140/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.6.21337/PKG-INFO` & `mo_parsing-8.639.24140/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,170 +1,146 @@
-Metadata-Version: 2.1
-Name: mo-parsing
-Version: 8.6.21337
-Summary: Another PEG Parsing Tool
-Home-page: https://github.com/klahnakoski/mo-parsing
-Author: Various
-Author-email: kyle@lahnakoski.com
-License: MIT
-Description: # More Parsing!
-        
-        [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-parsing.svg)](https://pypi.org/project/mo-parsing/)
-        [![Build Status](https://app.travis-ci.com/klahnakoski/mo-parsing.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-parsing)
-        [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-parsing/badge.svg?branch=master)](https://coveralls.io/github/klahnakoski/mo-parsing?branch=master)
-        
-        A fork of [pyparsing](https://github.com/pyparsing/pyparsing) for faster parsing
-        
-        
-        ## Installation
-        
-        This is a pypi package
-        
-            pip install mo-parsing
-            
-        ## Usage
-        
-        This module allows you to define a PEG parser using predefined patterns and Python operators.  Here is an example 
-        
-        ```
-        >>> from mo_parsing import Word
-        >>> from mo_parsing.utils import alphas
-        >>>
-        >>> greet = Word(alphas)("greeting") + "," + Word(alphas)("person") + "!"
-        >>> result = greet.parse_string("Hello, World!")
-        ```
-        
-        The `result` can be accessed as a nested list
-        
-        ```
-        >>> list(result)
-        ['Hello', ',', 'World', '!']
-        ```
-        
-        The `result` can also be accessed as a dictionary
-        
-        ```
-        >>> dict(result)
-        {'greeting': 'Hello', 'person': 'World'}
-        ```
-        
-        Read the [pyparsing documentation](https://github.com/pyparsing/pyparsing/#readme) for more
-        
-        ### The `Whitespace` Skipper
-        
-        The `mo_parsing.whitespaces.CURRENT` is used during parser creation: It is effectively defines what "whitespace" to skip during parsing, with additional features to simplify the language definition.  You declare "standard" `Whitespace` like so:
-        
-            with Whitespace() as whitespace:
-                # PUT YOUR LANGUAGE DEFINITION HERE (space, tab and CR are "whitespace")
-        
-        If you are declaring a large language, and you want to minimize indentation, and you are careful, you may also use this pattern:
-        
-            whitespace = Whitespace().use()
-            # PUT YOUR LANGUAGE DEFINITION HERE
-            whitespace.release()
-        
-        The whitespace can be used to set global parsing parameters, like
-        
-        * `set_whitespace()` - set the ignored characters (default: `"\t\n "`)
-        * `add_ignore()` - include whole patterns that are ignored (like comments)
-        * `set_literal()` - Set the definition for what `Literal()` means
-        * `set_keyword_chars()` - For default `Keyword()` (important for defining word boundary)
-        
-        
-        ### Navigating ParseResults
-        
-        The results of parsing are in `ParseResults` and are in the form of an n-ary tree; with the children found in `ParseResults.tokens`.  Each `ParseResult.type` points to the `ParserElement` that made it.  In general, if you want to get fancy with post processing (or in a `parse_action`), you will be required to navigate the raw `tokens` to generate a final result
-        
-        There are some convenience methods;  
-        * `__iter__()` - allows you to iterate through parse results in **depth first search**. Empty results are skipped, and `Group`ed results are treated as atoms (which can be further iterated if required) 
-        * `name` is a convenient property for `ParseResults.type.token_name`
-        * `__getitem__()` - allows you to jump into the parse tree to the given `name`. This is blocked by any names found inside `Group`ed results (because groups are considered atoms).      
-        
-        ### Parse Actions
-        
-        Parse actions are methods that are run after a ParserElement found a match. 
-        
-        * Parameters must be accepted in `(tokens, index, string)` order (the opposite of pyparsing)
-        * Parse actions are wrapped to ensure the output is a legitimate ParseResult
-          * If your parse action returns `None` then the result is the original `tokens`
-          * If your parse action returns an object, or list, or tuple, then it will be packaged in a `ParseResult` with same type as `tokens`.
-          * If your parse action returns a `ParseResult` then it is accepted ***even if is belongs to some other pattern***
-          
-        #### Simple example:
-        
-        ```
-        integer = Word("0123456789").add_parse_action(lambda t, i, s: int(t[0]))
-        result = integer.parse_string("42")
-        assert (result[0] == 42)
-        ```
-        
-        For slightly shorter specification, you may use the `/` operator and only parameters you need:
-        
-        ```
-        integer = Word("0123456789") / (lambda t: int(t[0]))
-        result = integer.parse_string("42")
-        assert (result[0] == 42)
-        ```
-        
-        ### Debugging
-        
-        The PEG-style of mo-parsing (from pyparsing) makes a very expressible and readable specification, but debugging a parser is still hard.  To look deeper into what the parser is doing use the `Debugger`:
-        
-        ```
-        with Debugger():
-            expr.parse_string("my new language")
-        ```
-        
-        The debugger will print out details of what's happening
-        
-        * Each attempt, and if it matched or failed
-        * A small number of bytes to show you the current position
-        * location, line and column for more info about the current position
-        * whitespace indicating stack depth
-        * print out of the ParserElement performing the attempt
-        
-        This should help to isolate the exact position your grammar is failing. 
-        
-        ### Regular Expressions
-        
-        `mo-parsing` can parse and generate regular expressions. `ParserElement` has a `__regex__()` function that returns the regular expression for the given grammar; which works up to a limit, and is used internally to accelerate parsing.  The `Regex` class parses regular expressions into a grammar; it is used to optimize parsing, and you may find it useful to decompose regular expressions that look like line noise.
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        ## Differences from PyParsing
-        
-        This fork was originally created to support faster parsing for [mo-sql-parsing](https://github.com/klahnakoski/moz-sql-parser).  Since then it has deviated sufficiently to be it's own collection of parser specification functions.  Here are the differences:
-        
-        * Added `Whitespace`, which controls parsing context and whitespace.  It replaces the whitespace modifying methods of pyparsing
-        * the wildcard ("`*`") could be used in pyparsing to indicate multi-values are expected; this is not allowed in `mo-parsing`: all values are multi-values
-        * ParserElements are static: For example, `expr.add_parse_action(action)` creates a new ParserElement, so must be assigned to variable or it is lost. **This is the biggest source of bugs when converting from pyparsing**
-        * removed all backward-compatibility settings
-        * no support for binary serialization (no pickle)
-        
-        Faster Parsing
-        
-        * faster infix operator parsing (main reason for this fork)
-        * ParseResults point to ParserElement for reduced size
-        * regex used to reduce the number of failed parse attempts  
-        * packrat parser is not need
-        * less stack used 
-        
-        
-        
-        ## Contributing
-        
-        If you plan to extend or enhance this code, please [see the README in the tests directory](https://github.com/klahnakoski/mo-parsing/blob/dev/tests/README.md)
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: tests
+# More Parsing!
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-parsing.svg)](https://pypi.org/project/mo-parsing/)
+ [![Build Status](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml)
+[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-parsing/badge.svg?branch=master)](https://coveralls.io/github/klahnakoski/mo-parsing?branch=master)
+
+A fork of [pyparsing](https://github.com/pyparsing/pyparsing) for faster parsing
+
+
+## Installation
+
+This is a pypi package
+
+    pip install mo-parsing
+    
+## Usage
+
+This module allows you to define a PEG parser using predefined patterns and Python operators.  Here is an example 
+
+```
+>>> from mo_parsing import Word
+>>> from mo_parsing.utils import alphas
+>>>
+>>> greet = Word(alphas)("greeting") + "," + Word(alphas)("person") + "!"
+>>> result = greet.parse_string("Hello, World!")
+```
+
+The `result` can be accessed as a nested list
+
+```
+>>> list(result)
+['Hello', ',', 'World', '!']
+```
+
+The `result` can also be accessed as a dictionary
+
+```
+>>> dict(result)
+{'greeting': 'Hello', 'person': 'World'}
+```
+
+Read the [pyparsing documentation](https://github.com/pyparsing/pyparsing/#readme) for more
+
+### The `Whitespace` Context
+
+The `mo_parsing.whitespaces.CURRENT` is used during parser creation: It is effectively defines what "whitespace" to skip during parsing, with additional features to simplify the language definition.  You declare "standard" `Whitespace` like so:
+
+    with Whitespace() as whitespace:
+        # PUT YOUR LANGUAGE DEFINITION HERE (space, tab and CR are "whitespace")
+
+If you are declaring a large language, and you want to minimize indentation, and you are careful, you may also use this pattern:
+
+    whitespace = Whitespace().use()
+    # PUT YOUR LANGUAGE DEFINITION HERE
+    whitespace.release()
+
+The whitespace can be used to set global parsing parameters, like
+
+* `set_whitespace()` - set the ignored characters (default: `"\t\n "`)
+* `add_ignore()` - include whole patterns that are ignored (like comments)
+* `set_literal()` - Set the definition for what `Literal()` means
+* `set_keyword_chars()` - For default `Keyword()` (important for defining word boundary)
+
+
+### Navigating ParseResults
+
+The results of parsing are in `ParseResults` and are in the form of an n-ary tree; with the children found in `ParseResults.tokens`.  Each `ParseResult.type` points to the `ParserElement` that made it.  In general, if you want to get fancy with post processing (or in a `parse_action`), you will be required to navigate the raw `tokens` to generate a final result
+
+There are some convenience methods;  
+* `__iter__()` - allows you to iterate through parse results in **depth first search**. Empty results are skipped, and `Group`ed results are treated as atoms (which can be further iterated if required) 
+* `name` is a convenient property for `ParseResults.type.token_name`
+* `__getitem__()` - allows you to jump into the parse tree to the given `name`. This is blocked by any names found inside `Group`ed results (because groups are considered atoms).      
+
+### Parse Actions
+
+Parse actions are methods that run after a ParserElement found a match. 
+
+* Parameters must be accepted in `(tokens, index, string)` order (the opposite of pyparsing)
+* Parse actions are wrapped to ensure the output is a legitimate ParseResult
+  * If your parse action returns `None` then the result is the original `tokens`
+  * If your parse action returns an object, or list, or tuple, then it will be packaged in a `ParseResult` with same type as `tokens`.
+  * If your parse action returns a `ParseResult` then it is accepted ***even if is belongs to some other pattern***
+  
+#### Simple example:
+
+```
+integer = Word("0123456789").add_parse_action(lambda t, i, s: int(t[0]))
+result = integer.parse_string("42")
+assert (result[0] == 42)
+```
+
+For slightly shorter specification, you may use the `/` operator and only parameters you need:
+
+```
+integer = Word("0123456789") / (lambda t: int(t[0]))
+result = integer.parse_string("42")
+assert (result[0] == 42)
+```
+
+### Debugging
+
+The PEG-style of mo-parsing (from pyparsing) makes a very expressible and readable specification, but debugging a parser is still hard.  To look deeper into what the parser is doing use the `Debugger`:
+
+```
+with Debugger():
+    expr.parse_string("my new language")
+```
+
+The debugger will print out details of what's happening
+
+* Each attempt, and if it matched or failed
+* A small number of bytes to show you the current position
+* location, line and column for more info about the current position
+* whitespace indicating stack depth
+* print out of the ParserElement performing the attempt
+
+This should help to isolate the exact position your grammar is failing. 
+
+### Regular Expressions
+
+`mo-parsing` can parse and generate regular expressions. `ParserElement` has a `__regex__()` function that returns the regular expression for the given grammar; which works up to a limit, and is used internally to accelerate parsing.  The `Regex` class parses regular expressions into a grammar; it is used to optimize parsing, and you may find it useful to decompose regular expressions that look like line noise.
+
+
+## Differences from PyParsing
+
+This fork was originally created to support faster parsing for [mo-sql-parsing](https://github.com/klahnakoski/moz-sql-parser).  Since then it has deviated sufficiently to be it's own collection of parser specification functions.  Here are the differences:
+
+* Added `Whitespace`, which controls parsing context and whitespace.  It replaces the whitespace modifying methods of pyparsing
+* the wildcard ("`*`") could be used in pyparsing to indicate multi-values are expected; this is not allowed in `mo-parsing`: all values are multi-values
+* ParserElements are static: For example, `expr.add_parse_action(action)` creates a new ParserElement, so must be assigned to variable or it is lost. **This is the biggest source of bugs when converting from pyparsing**
+* removed all backward-compatibility settings
+* no support for binary serialization (no pickle)
+
+Faster Parsing
+
+* faster infix operator parsing (main reason for this fork)
+* ParseResults point to ParserElement for reduced size
+* regex used to reduce the number of failed parse attempts  
+* packrat parser is not need
+* less stack used 
+
+
+
+## Contributing
+
+If you plan to extend or enhance this code, please [see the README in the tests directory](https://github.com/klahnakoski/mo-parsing/blob/dev/tests/README.md)
```

### Comparing `mo-parsing-8.6.21337/README.md` & `mo_parsing-8.639.24140/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,38 @@
+Metadata-Version: 2.1
+Name: mo-parsing
+Version: 8.639.24140
+Summary: Another PEG Parsing Tool
+Home-page: https://github.com/klahnakoski/mo-parsing
+Author: Various
+Author-email: kyle@lahnakoski.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: mo-dots==10.632.24139
+Requires-Dist: mo-future==7.584.24095
+Provides-Extra: tests
+Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
+Requires-Dist: mo-threads>=6.562.24075; extra == "tests"
+Requires-Dist: mo-logs>=8.562.24075; extra == "tests"
+Requires-Dist: mo-files>=6.562.24075; extra == "tests"
+
 # More Parsing!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-parsing.svg)](https://pypi.org/project/mo-parsing/)
-[![Build Status](https://app.travis-ci.com/klahnakoski/mo-parsing.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-parsing)
+ [![Build Status](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-parsing/badge.svg?branch=master)](https://coveralls.io/github/klahnakoski/mo-parsing?branch=master)
 
 A fork of [pyparsing](https://github.com/pyparsing/pyparsing) for faster parsing
 
 
 ## Installation
 
@@ -37,15 +64,15 @@
 ```
 >>> dict(result)
 {'greeting': 'Hello', 'person': 'World'}
 ```
 
 Read the [pyparsing documentation](https://github.com/pyparsing/pyparsing/#readme) for more
 
-### The `Whitespace` Skipper
+### The `Whitespace` Context
 
 The `mo_parsing.whitespaces.CURRENT` is used during parser creation: It is effectively defines what "whitespace" to skip during parsing, with additional features to simplify the language definition.  You declare "standard" `Whitespace` like so:
 
     with Whitespace() as whitespace:
         # PUT YOUR LANGUAGE DEFINITION HERE (space, tab and CR are "whitespace")
 
 If you are declaring a large language, and you want to minimize indentation, and you are careful, you may also use this pattern:
@@ -69,15 +96,15 @@
 There are some convenience methods;  
 * `__iter__()` - allows you to iterate through parse results in **depth first search**. Empty results are skipped, and `Group`ed results are treated as atoms (which can be further iterated if required) 
 * `name` is a convenient property for `ParseResults.type.token_name`
 * `__getitem__()` - allows you to jump into the parse tree to the given `name`. This is blocked by any names found inside `Group`ed results (because groups are considered atoms).      
 
 ### Parse Actions
 
-Parse actions are methods that are run after a ParserElement found a match. 
+Parse actions are methods that run after a ParserElement found a match. 
 
 * Parameters must be accepted in `(tokens, index, string)` order (the opposite of pyparsing)
 * Parse actions are wrapped to ensure the output is a legitimate ParseResult
   * If your parse action returns `None` then the result is the original `tokens`
   * If your parse action returns an object, or list, or tuple, then it will be packaged in a `ParseResult` with same type as `tokens`.
   * If your parse action returns a `ParseResult` then it is accepted ***even if is belongs to some other pattern***
   
@@ -117,22 +144,14 @@
 This should help to isolate the exact position your grammar is failing. 
 
 ### Regular Expressions
 
 `mo-parsing` can parse and generate regular expressions. `ParserElement` has a `__regex__()` function that returns the regular expression for the given grammar; which works up to a limit, and is used internally to accelerate parsing.  The `Regex` class parses regular expressions into a grammar; it is used to optimize parsing, and you may find it useful to decompose regular expressions that look like line noise.
 
 
-
-
-
-
-
-
-
-
 ## Differences from PyParsing
 
 This fork was originally created to support faster parsing for [mo-sql-parsing](https://github.com/klahnakoski/moz-sql-parser).  Since then it has deviated sufficiently to be it's own collection of parser specification functions.  Here are the differences:
 
 * Added `Whitespace`, which controls parsing context and whitespace.  It replaces the whitespace modifying methods of pyparsing
 * the wildcard ("`*`") could be used in pyparsing to indicate multi-values are expected; this is not allowed in `mo-parsing`: all values are multi-values
 * ParserElements are static: For example, `expr.add_parse_action(action)` creates a new ParserElement, so must be assigned to variable or it is lost. **This is the biggest source of bugs when converting from pyparsing**
@@ -147,8 +166,8 @@
 * packrat parser is not need
 * less stack used 
 
 
 
 ## Contributing
 
-If you plan to extend or enhance this code, please [see the README in the tests directory](https://github.com/klahnakoski/mo-parsing/blob/dev/tests/README.md)
+If you plan to extend or enhance this code, please [see the README in the tests directory](https://github.com/klahnakoski/mo-parsing/blob/dev/tests/README.md)
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/__init__.py` & `mo_parsing-8.639.24140/mo_parsing/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,79 +22,82 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 from mo_parsing import whitespaces
-from mo_parsing.core import ParserElement, _PendingSkip
+from mo_parsing.core import ParserElement, _PendingSkip, set_parser_names
 from mo_parsing.enhancement import *
-from mo_parsing.exceptions import (
-    ParseException,
-    ParseException,
-    ParseSyntaxException,
-    RecursiveGrammarException,
-)
+from mo_parsing.exceptions import ParseException, ParseException, ParseSyntaxException, RecursiveGrammarException
 from mo_parsing.expressions import And, MatchAll, MatchFirst, Or, ParseExpression
 from mo_parsing.whitespaces import Whitespace
 
-whitespaces.NO_WHITESPACE = Whitespace("").use()
-whitespaces.STANDARD_WHITESPACE = Whitespace().use()
+NO_WHITESPACE = whitespaces.NO_WHITESPACE = Whitespace("").use()
+STANDARD_WHITESPACE = whitespaces.STANDARD_WHITESPACE = Whitespace().use()
 
-from mo_parsing.infix import LEFT_ASSOC, RIGHT_ASSOC, infix_notation
+from mo_parsing.infix import LEFT_ASSOC, RIGHT_ASSOC, infix_notation, delimited_list, one_of
 from mo_parsing.regex import Regex
 from mo_parsing.tokens import *
 
-
 __all__ = [
     "And",
     "AnyChar",
     "CaselessKeyword",
     "CaselessLiteral",
+    "Char",
     "CharsNotIn",
+    "CloseMatch",
     "Combine",
+    "delimited_list",
+    "delimited_list",
     "Dict",
-    "MatchAll",
     "Empty",
     "FollowedBy",
     "Forward",
     "Group",
+    "infix_notation",
+    "infix_notation",
     "Keyword",
+    "LEFT_ASSOC",
+    "LEFT_ASSOC",
     "LineEnd",
     "LineStart",
     "Literal",
     "LookAhead",
     "LookBehind",
-    "PrecededBy",
     "Many",
+    "MatchAll",
     "MatchFirst",
+    "NO_WHITESPACE",
     "NoMatch",
     "NotAny",
+    "one_of",
     "OneOrMore",
     "Optional",
     "Or",
-    "ParseException",
     "ParseEnhancement",
     "ParseException",
+    "ParseException",
     "ParseExpression",
+    "ParserElement",
     "ParseResults",
     "ParseSyntaxException",
-    "ParserElement",
+    "PrecededBy",
     "RecursiveGrammarException",
     "Regex",
+    "RIGHT_ASSOC",
+    "RIGHT_ASSOC",
+    "set_parser_names",
     "SkipTo",
     "StringEnd",
     "StringStart",
     "Suppress",
     "Token",
     "TokenConverter",
     "White",
+    "Whitespace",
     "Word",
     "WordEnd",
     "WordStart",
     "ZeroOrMore",
-    "Char",
-    "LEFT_ASSOC",
-    "RIGHT_ASSOC",
-    "infix_notation",
-    "CloseMatch",
 ]
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/core.py` & `mo_parsing-8.639.24140/mo_parsing/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # encoding: utf-8
+import sys
 from collections import namedtuple
 from threading import RLock
+from typing import List
 
-from mo_future import text
+from mo_future import text, first
 from mo_imports import export, expect
 
 from mo_parsing import whitespaces
 from mo_parsing.exceptions import ParseException
 from mo_parsing.results import ParseResults
 from mo_parsing.utils import Log, MAX_INT, wrap_parse_action, empty_tuple
 
@@ -24,14 +26,15 @@
     MatchAll,
     Empty,
     StringEnd,
     Literal,
     Token,
     Group,
     regex_parameters,
+    _suppress_post_parse
 ) = expect(
     "SkipTo",
     "Many",
     "ZeroOrMore",
     "OneOrMore",
     "Optional",
     "NotAny",
@@ -42,19 +45,19 @@
     "MatchAll",
     "Empty",
     "StringEnd",
     "Literal",
     "Token",
     "Group",
     "regex_parameters",
+    "_suppress_post_parse"
 )
 
 DEBUG = False
 
-
 # TODO: Replace with a stack of parse state
 _reset_actions = []
 
 
 def add_reset_action(action):
     """
     ADD A FUNCTION THAT WILL RESET GLOBAL STATE THAT A PARSER MAY USE
@@ -77,26 +80,33 @@
                     Log.error("reset action failed", cause=e)
 
             return func(*args, **kwargs)
 
     return output
 
 
-def _verify_whitespace(eng):
-    if eng is None:
+def _verify_whitespace(whi: List):
+    if whi is None:
         return None
-    if isinstance(eng, list):
-        engs = [v for e in eng for v in [_verify_whitespace(e)] if v is not None]
-        if not engs:
+    if isinstance(whi, list):
+        whis = [
+            v
+            for e in whi
+            for v in [_verify_whitespace(e)]
+            if v is not None and v.regex.pattern  # IGNORE NO_WHITESPACE
+        ]
+        if not whis:
             return None
-        whitespace = engs[0]
-        if any(e.id != whitespace.id for e in engs[1:]):
+        whitespace = whis[0]
+        if any(e.id != whitespace.id for e in whis[1:]):
+            # THE TOP-MOST WHITESPACE RULES ARE DIFFERENT FOR EACH ParserElement,
+            # SO PROGRAM DOES NOT KNOW WHICH IS THE MASTER WHITESPACE
             Log.error("must dis-ambiguate the whitespace before parsing")
         return whitespace
-    return eng
+    return whi
 
 
 class Parser(object):
     def __init__(self, element):
         self.element = element = element.streamline()
         try:
             self.whitespace = (
@@ -354,30 +364,33 @@
         output = self.copy()
         output.parse_action = []
         return output
 
     def add_parse_action(self, *fns, callDuringTry=False):
         """
         Add one or more parse actions to expression's list of parse actions. See `setParseAction`.
-
-        See examples in `copy`.
+        Also you can use `/` operator
         """
         output = self.copy()
         output.parse_action += list(map(wrap_parse_action, fns))
         output.set_config(
             callDuringTry=self.parser_config.callDuringTry or callDuringTry
         )
         return output
 
     def __truediv__(self, func):
         """
         Shortform for add_parse_action
         """
         output = self.copy()
-        output.parse_action.append(wrap_parse_action(func))
+        try:
+            output.parse_action.append(wrap_parse_action(func))
+        except:
+            # REPLACE WITH CONSTANT
+            output.parse_action.append(lambda t, i, s: ParseResults(t.type, t.start, t.end, [func], []))
         return output
 
     def add_condition(self, *fns, message=None, callDuringTry=False, fatal=False):
         """
         Add a boolean predicate function to expression's list of parse actions. See
         `setParseAction` for function call signatures. Unlike ``setParseAction``,
         functions passed to ``add_condition`` need to return boolean success/fail of the condition.
@@ -419,15 +432,16 @@
         - err = the exception thrown
         The function returns no value.  It may throw `ParseFatalException`
         if it is desired to stop parsing immediately."""
         self.set_config(fail_action=fn)
         return self
 
     def is_annotated(self):
-        return self.parse_action or self.token_name or self.parser_name
+        action = first(a for a in self.parse_action if a is not _suppress_post_parse)
+        return action or self.token_name or self.parser_name
 
     def expecting(self):
         """
         RETURN EXPECTED CHARACTER SEQUENCE, IF ANY
         :return:
         """
         return {}
@@ -460,15 +474,16 @@
             raise ParseException(self, start, string, cause=cause) from None
 
         if do_actions or self.parser_config.callDuringTry:
             for fn in self.parse_action:
                 next_result = fn(result, result.start, string)
                 if next_result.end < result.end:
                     Log.error(
-                        "parse action not allowed to roll back the end of parsing"
+                        "parse action {{name}} not allowed to roll back the end of parsing",
+                        name=fn.__name__
                     )
                 result = next_result
         return result
 
     def finalize(self):
         """
         Return a Parser for use in parsing (optimization only)
@@ -641,19 +656,17 @@
         """
         Implementation of ^ operator when left operand is not a `ParserElement`
         """
         return whitespaces.CURRENT.normalize(other) ^ self
 
     def __and__(self, other):
         """
-        Implementation of & operator - returns `Each`
+        Implementation of & operator - returns `MatchAll`
         """
-        return MatchAll(
-            [self, whitespaces.CURRENT.normalize(other)], whitespaces.CURRENT
-        )
+        return MatchAll([self, whitespaces.CURRENT.normalize(other)])
 
     def __rand__(self, other):
         """
         Implementation of & operator when left operand is not a `ParserElement`
         """
         return whitespaces.CURRENT.normalize(other) & self
 
@@ -689,15 +702,15 @@
         return output
 
     def suppress(self):
         """
         Suppresses the output of this `ParserElement`; useful to keep punctuation from
         cluttering up returned output.
         """
-        return Suppress(self)
+        return self / _suppress_post_parse
 
     def __str__(self):
         return self.parser_name
 
     def __repr__(self):
         return text(self)
 
@@ -772,16 +785,29 @@
         skipper = SkipTo(other)("_skipped")
         return self.anchor + skipper + other
 
     def parse_impl(self, *args):
         Log.error("use of `...` expression without following SkipTo target expression")
 
 
+def set_parser_names():
+    """
+    ASSIGN parser_name FOR All ParserElements FOUND IN CALLER
+    """
+    frame = sys._getframe(1)
+    items = list(frame.f_locals.items())
+    for k, v in items:
+        try:
+            if isinstance(v, ParserElement) and not v.parser_name:
+                v.parser_name = k.lower()
+        except Exception:
+            pass
+
+
 NO_PARSER = (
     ParserElement().set_parser_name("<nothing>")
 )  # USE THIS WHEN YOU DO NOT CARE ABOUT THE PARSER TYPE
 NO_RESULTS = ParseResults(NO_PARSER, -1, 0, [], [])
 
-
 export("mo_parsing.results", ParserElement)
 export("mo_parsing.results", NO_PARSER)
 export("mo_parsing.results", NO_RESULTS)
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/debug.py` & `mo_parsing-8.639.24140/mo_parsing/debug.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,40 +5,42 @@
 
 from mo_parsing.core import ParserElement
 from mo_parsing.utils import (
     quote,
     lineno,
     col,
     stack_depth,
-    quote as plain_quote, ParseException,
+    quote as plain_quote,
+    ParseException,
 )
 
-DEBUGGING = False
+DEBUGGER = None
+_max_preamble = 60
 
 
 class Debugger(object):
     def __init__(self, silent=False):
         self.previous_parse = None
-        self.was_debugging = False
+        self.was_debugging = None
         self.parse_count = 0
         self.max_stack_depth = 0
         self.silent = silent
 
     def __enter__(self):
-        global DEBUGGING
-        self.was_debugging = DEBUGGING
-        DEBUGGING = True
+        global DEBUGGER
+        self.was_debugging = DEBUGGER
+        DEBUGGER = self
         self.previous_parse = ParserElement._parse
         ParserElement._parse = _debug_parse(self)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        global DEBUGGING
+        global DEBUGGER
         ParserElement._parse = self.previous_parse
-        DEBUGGING = self.was_debugging
+        DEBUGGER = self.was_debugging
 
 
 def _debug_parse(debugger):
     def debug_parse(self, string, start, do_actions=True):
         if not debugger.silent:
             _try(self, start, string)
         loc = start
@@ -66,36 +68,38 @@
 
         return tokens
 
     return debug_parse
 
 
 def _try(expr, start, string):
+    global _max_preamble
+    preamble = f"  Attempt {quote(string, start)} at loc ({lineno(start, string)},{col(start, string)}), index={start}"
+    length = len(preamble)
+    _max_preamble = max(_max_preamble, length)
     print(
-        "  Attempt "
-        + quote(string, start)
-        + " at loc "
-        + text(start)
-        + "(%d,%d)" % (lineno(start, string), col(start, string))
-        + " for "
+        preamble
+        + " " * (_max_preamble - length)
+        + "for"
         + " " * stack_depth()
         + text(expr)[:300]
     )
 
 
 def match(expr, start, end, string, tokens):
+    global _max_preamble
+    preamble = f"> Matched {quote(string[start:end])} at loc ({lineno(start, string)},{col(start, string)}), length={end-start}"
+    length = len(preamble)
+    _max_preamble = max(_max_preamble, length)
     print(
-        "> Matched "
-        + quote(string[start:end])
-        + "between "
-        + f"[{start}, {end}] for"
+        preamble
+        + " " * (_max_preamble - length)
+        + "for"
         + " " * stack_depth()
-        + text(expr)
-        + " -> "
-        + str(tokens)
+        + f"{expr} -> {tokens}"
     )
 
 
 def fail(expr, start, string, cause):
     quoted = plain_quote(text(cause))
     print("  Except  " + quoted)
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/enhancement.py` & `mo_parsing-8.639.24140/mo_parsing/enhancement.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,32 @@
 # encoding: utf-8
-import re
 from collections import OrderedDict
 
 from mo_dots import Null, is_null
 from mo_future import text, is_text
 from mo_imports import export, expect
 
 from mo_parsing import whitespaces
 from mo_parsing.core import ParserElement
-from mo_parsing.exceptions import (
-    ParseException,
-    RecursiveGrammarException,
-)
-from mo_parsing.results import ParseResults, Annotation
+from mo_parsing.exceptions import ParseException, RecursiveGrammarException
+from mo_parsing.results import ParseResults, ForwardResults, Annotation
 from mo_parsing.utils import (
     Log,
-    listwrap,
+    enlist,
     empty_tuple,
     regex_iso,
     append_config,
     regex_compile,
     wrap_parse_action,
 )
 from mo_parsing.utils import MAX_INT, is_forward
 
 Word: object
-(
-    Token,
-    NoMatch,
-    Literal,
-    Keyword,
-    Word,
-    CharsNotIn,
-    StringEnd,
-    Empty,
-    Char,
-) = expect(
-    "Token",
-    "NoMatch",
-    "Literal",
-    "Keyword",
-    "Word",
-    "CharsNotIn",
-    "StringEnd",
-    "Empty",
-    "Char",
+(Token, NoMatch, Literal, Keyword, Word, CharsNotIn, StringEnd, Empty, Char,) = expect(
+    "Token", "NoMatch", "Literal", "Keyword", "Word", "CharsNotIn", "StringEnd", "Empty", "Char",
 )
 
 _get = object.__getattribute__
 
 
 class ParseEnhancement(ParserElement):
     """
@@ -79,16 +57,19 @@
         return self.expr.min_length()
 
     @property
     def whitespace(self):
         return self.expr.whitespace
 
     def parse_impl(self, string, start, do_actions=True):
-        result = self.expr._parse(string, start, do_actions)
-        return ParseResults(self, result.start, result.end, [result], result.failures)
+        try:
+            result = self.expr._parse(string, start, do_actions)
+            return ParseResults(self, result.start, result.end, [result], result.failures)
+        except ParseException as cause:
+            raise ParseException(self, start, string, cause=cause) from None
 
     def streamline(self):
         if self.streamlined:
             return self
 
         expr = self.expr.streamline()
         if expr is self.expr:
@@ -154,16 +135,16 @@
     """
 
     zero_length = True
     __slots__ = ["regex"]
 
     def __init__(self, expr):
         super(NotAny, self).__init__(expr)
-        prec, pattern = self.expr.__regex__()
         try:
+            prec, pattern = self.expr.__regex__()
             self.regex = regex_compile(f"(?!{pattern})")
         except Exception as c:
             self.regex = None
 
     def copy(self):
         output = ParseEnhancement.copy(self)
         output.regex = self.regex
@@ -171,19 +152,19 @@
 
     def parse_impl(self, string, start, do_actions=True):
         regex = self.regex
         if regex:
             found = regex.match(string, start)
             if found:
                 return ParseResults(self, start, start, [], [])
-            raise ParseException(self, start, string)
+            raise ParseException(self, start, string) from None
         else:
             try:
                 self.expr.parse(string, start, do_actions=True)
-                raise ParseException(self, start, string)
+                raise ParseException(self, start, string) from None
             except:
                 return ParseResults(self, start, start, [], [])
 
     def streamline(self):
         output = ParseEnhancement.streamline(self)
         if isinstance(output, Empty):
             return NoMatch()
@@ -206,43 +187,36 @@
         if self.parser_name:
             return self.parser_name
         return "~{" + str(self.expr) + "}"
 
 
 class Many(ParseEnhancement):
     __slots__ = []
-    Config = append_config(
-        ParseEnhancement, "whitespace", "min_match", "max_match", "end"
-    )
+    Config = append_config(ParseEnhancement, "whitespace", "min_match", "max_match", "end")
 
     def __init__(
-            self,
-            expr,
-            whitespace=None,
-            stop_on=None,
-            min_match=0,
-            max_match=MAX_INT,
-            exact=None,
+        self, expr, whitespace=None, stop_on=None, min_match=0, max_match=MAX_INT, exact=None,
     ):
         """
         MATCH expr SOME NUMBER OF TIMES (OR UNTIL stop_on IS REACHED
         :param expr: THE EXPRESSION TO MATCH
         :param stop_on: THE PATTERN TO INDICATE STOP MATCHING (NOT REQUIRED IN PATTERN, JUST A QUICK STOP)
         :param min_match: MINIMUM MATCHES REQUIRED FOR SUCCESS (-1 IS INVALID)
         :param max_match: MAXIMUM MATCH REQUIRED FOR SUCCESS (-1 IS INVALID)
         """
         ParseEnhancement.__init__(self, expr)
+        if isinstance(self.expr, LookBehind):
+            # TODO: support Optional(LookBehind()))
+            Log.error("can only look behind once")
         if exact is not None:
             min_match = exact
             max_match = exact
 
         self.set_config(
-            whitespace=whitespace or whitespaces.CURRENT,
-            min_match=min_match,
-            max_match=max_match,
+            whitespace=whitespace or whitespaces.CURRENT, min_match=min_match, max_match=max_match,
         )
         self.stop_on(stop_on)
 
     def stop_on(self, ender):
         if ender:
             end = self.parser_config.whitespace.normalize(ender)
             self.set_config(end=regex_compile(end.__regex__()[1]))
@@ -255,88 +229,58 @@
 
     @property
     def whitespace(self):
         return self.parser_config.whitespace
 
     def parse_impl(self, string, start, do_actions=True):
         acc = []
-        end = index = start
+        end = start
         max = self.parser_config.max_match
+        min = self.parser_config.min_match
         stopper = self.parser_config.end
         count = 0
         failures = []
         try:
-            while end < len(string) and count < max:
-                if end > index:
-                    if isinstance(self.expr, LookBehind):
-                        index = end
-                    else:
-                        index = self.parser_config.whitespace.skip(string, end)
+            while end < len(string):
+                index = self.parser_config.whitespace.skip(string, end)
                 if stopper:
                     if stopper.match(string, index):
-                        if self.parser_config.min_match <= count:
+                        if min <= count:
                             break
                         else:
-                            raise ParseException(
-                                self, end, string, msg="found stopper too soon"
-                            )
+                            raise ParseException(self, end, string, msg="found stopper too soon")
                 result = self.expr._parse(string, index, do_actions)
                 end = result.end
-                if result:
+                if result.end - result.start:
                     acc.append(result)
+                    failures.extend(result.failures)
                     count += 1
+                    if count >= max:
+                        break
+
         except ParseException as cause:
-            if self.parser_config.min_match <= count <= max:
-                failures.append(cause)
-            else:
-                raise ParseException(
-                    self,
-                    start,
-                    string,
-                    msg="Not correct amount of matches",
-                    cause=cause,
-                ) from None
-        if count:
-            if (
-                    count < self.parser_config.min_match
-                    or self.parser_config.max_match < count
-            ):
-                raise ParseException(
-                    self,
-                    acc[0].start,
-                    string,
-                    msg=(
-                        f"Expecting between {self.parser_config.min_match} and"
-                        f" {self.parser_config.max_match} of {self.expr}"
-                    ),
-                )
-            else:
-                return ParseResults(self, acc[0].start, acc[-1].end, acc, failures)
+            failures.append(cause)
+
+        if count < min:
+            raise ParseException(self, start, string, f"Expecting at least {min} of {self}", failures)
+        elif max < count:
+            raise ParseException(
+                self, acc[0].start, string, f"Expecting less than {max} of {self.expr}", failures,
+            )
         else:
-            if not self.parser_config.min_match:
-                return ParseResults(self, start, start, [], failures)
+            if count:
+                return ParseResults(self, acc[0].start, acc[-1].end, acc, failures)
             else:
-                raise ParseException(
-                    self,
-                    start,
-                    string,
-                    msg=f"Expecting at least {self.parser_config.min_match} of {self}",
-                )
+                return ParseResults(self, start, end, acc, failures)
 
     def streamline(self):
         if self.streamlined:
             return self
-        try:
-            expr = self.expr.streamline()
-        except Exception as e:
-            print(e)
-        if (
-                self.parser_config.min_match == self.parser_config.max_match
-                and not self.is_annotated()
-        ):
+        expr = self.expr.streamline()
+        if self.parser_config.min_match == self.parser_config.max_match and not self.is_annotated():
             if self.parser_config.min_match == 0:
                 return Empty()
             elif self.parser_config.min_match == 1:
                 return expr
 
         if self.expr is expr:
             self.streamlined = True
@@ -362,37 +306,28 @@
                 suffix = "{" + text(self.parser_config.min_match) + ",}"
         elif self.parser_config.min_match == self.parser_config.max_match:
             if self.parser_config.min_match == 1:
                 suffix = ""
             else:
                 suffix = "{" + text(self.parser_config.min_match) + "}"
         else:
-            suffix = (
-                    "{"
-                    + text(self.parser_config.min_match)
-                    + ","
-                    + text(self.parser_config.max_match)
-                    + "}"
-            )
+            suffix = "{" + text(self.parser_config.min_match) + "," + text(self.parser_config.max_match) + "}"
 
         if end:
             return "+", regex + suffix + end
         else:
             return "*", regex + suffix
 
     def __call__(self, name):
         if not name:
             return self
 
         for e in [self.expr]:
             if isinstance(e, ParserElement) and e.token_name == name:
-                Log.error(
-                    "can not set token name, already set in one of the other"
-                    " expressions"
-                )
+                Log.error("can not set token name, already set in one of the other expressions")
 
         return ParseEnhancement.__call__(self, name)
 
     def __str__(self):
         if self.parser_name:
             return self.parser_name
         return f"{self.__class__.__name__}:({self.expr})"
@@ -434,15 +369,15 @@
     __slots__ = []
 
     def __init__(self, expr, whitespace=None, stop_on=None):
         Many.__init__(self, expr, whitespace, stop_on=stop_on, min_match=0, max_match=MAX_INT)
 
     def parse_impl(self, string, start, do_actions=True):
         try:
-            return super(ZeroOrMore, self).parse_impl(string, start, do_actions)
+            return Many.parse_impl(self, string, start, do_actions)
         except ParseException as pe:
             return ParseResults(self, start, start, [], [pe])
 
     def __str__(self):
         if self.parser_name:
             return self.parser_name
 
@@ -458,24 +393,22 @@
     """
 
     __slots__ = []
     Config = append_config(Many, "default_value")
 
     def __init__(self, expr, whitespace=None, default=None):
         Many.__init__(self, expr, whitespace, stop_on=None, min_match=0, max_match=1)
-        self.set_config(default_value=listwrap(default))
+        self.set_config(default_value=enlist(default))
 
     def parse_impl(self, string, start, do_actions=True):
         try:
             results = self.expr._parse(string, start, do_actions)
-            return ParseResults(self, results.start, results.end, [results], [])
+            return ParseResults(self, results.start, results.end, [results], results.failures)
         except ParseException as pe:
-            return ParseResults(
-                self, start, start, self.parser_config.default_value, [pe]
-            )
+            return ParseResults(self, start, start, self.parser_config.default_value, [pe])
 
     def __str__(self):
         if self.parser_name:
             return self.parser_name
 
         return "[" + text(self.expr) + "]"
 
@@ -506,14 +439,22 @@
             whitespace=engine_ or whitespaces.CURRENT,
         )
         self.parser_name = str(self)
 
     def min_length(self):
         return 0
 
+    def __regex__(self):
+        prec, pattern = self.expr.__regex__()
+        pattern = regex_iso(prec, pattern, "+")
+        if self.parser_config.include:
+            return "*", f"(.*?{pattern})"
+        else:
+            return "+", f"(.*?)(?={pattern})"
+
     def parse_impl(self, string, start, do_actions=True):
         instrlen = len(string)
         fail = self.parser_config.fail
         ignore = self.parser_config.ignore
 
         loc = start
         while loc <= instrlen:
@@ -529,30 +470,28 @@
 
             if ignore:
                 # advance past ignore expressions
                 while 1:
                     try:
                         loc = ignore._parse(string, loc).end
                         skip_end = loc
-                        loc = before_end = self.parser_config.whitespace.skip(
-                            string, loc
-                        )
+                        loc = before_end = self.parser_config.whitespace.skip(string, loc)
                     except ParseException:
                         break
             try:
                 loc = self.expr._parse(string, loc, do_actions=False).end
             except ParseException:
                 # no match, advance loc in string
                 loc += 1
             else:
                 # matched skipto expr, done
                 break
         else:
             # ran off the end of the input string without matching skipto expr, fail
-            raise ParseException(self, start, string)
+            raise ParseException(self, start, string) from None
 
         # build up return values
         end = loc
         skiptext = string[start:skip_end]
         skip_result = []
         if skiptext:
             skip_result.append(skiptext)
@@ -589,33 +528,42 @@
 
     Converting to use the '<<=' operator instead will avoid this problem.
 
     See `ParseResults.pprint` for an example of a recursive
     parser created using ``Forward``.
     """
 
-    __slots__ = ["expr", "used_by", "_str", "_reg", "_eng"]
+    __slots__ = [
+        "expr",
+        "used_by",
+        "_str",
+        "_in_regex",
+        "_in_expecting",
+        "__in_whitespace",
+    ]
 
     def __init__(self, expr=Null):
         ParserElement.__init__(self)
         self.expr = None
         self.used_by = []
 
         self._str = None  # avoid recursion
-        self._reg = None  # avoid recursion
-        self._eng = False
+        self._in_regex = None  # avoid recursion
+        self._in_expecting = None  # avoid recursion
+        self.__in_whitespace = False
         if expr:
             self << whitespaces.CURRENT.normalize(expr)
 
     def copy(self):
         output = ParserElement.copy(self)
         output.expr = self
         output._str = None
-        output._reg = None
-        output._eng = False
+        output._in_regex = None
+        output._in_expecting = None
+        output.__in_whitespace = False
 
         output.used_by = []
         return output
 
     @property
     def name(self):
         return self.type.expr.token_name
@@ -627,21 +575,23 @@
         self._str = ""
         if is_forward(self.expr):
             return self.expr << other
 
         while is_forward(other):
             other = other.expr
         norm = whitespaces.CURRENT.normalize(other)
-        if norm is None:
-            Log.error("problem")
         self.expr = norm.streamline()
         self.check_recursion()
         return self
 
     def add_parse_action(self, action):
+        """
+        Add one or more parse actions to expression's list of parse actions. See `setParseAction`.
+        Also you can use `/` operator
+        """
         self.parse_action.append(wrap_parse_action(action))
         return self
 
     def leave_whitespace(self):
         with whitespaces.NO_WHITESPACE:
             output = self.copy()
             output.expr = self.expr.leave_whitespace()
@@ -657,61 +607,69 @@
 
     def check_recursion(self, seen=empty_tuple):
         if self in seen:
             raise RecursiveGrammarException(seen + (self,))
         if self.expr != None:
             self.expr.check_recursion(seen + (self,))
 
+    def expecting(self):
+        if self._in_expecting:
+            return {}
+        self._in_expecting = True
+        try:
+            if not self.expr:
+                return {}
+            return self.expr.expecting()
+        finally:
+            self._in_expecting = False
+
     def min_length(self):
         if self.min_length_cache is None and self.expr:
             self.min_length_cache = 0  # BREAK CYCLE
             try:
                 return self.expr.min_length()
             finally:
                 self.min_length_cache = None
         return 0
 
     @property
     def whitespace(self):
-        try:
-            if self._eng:
-                return None
-        except Exception as cause:
-            Log.error("", cause=cause)
+        if self.__in_whitespace:
+            return None
 
         # Avoid infinite recursion by setting a temporary
-        self._eng = True
+        self.__in_whitespace = True
         try:
             return self.expr.whitespace
         finally:
-            self._eng = False
+            self.__in_whitespace = False
 
     def parse_impl(self, string, loc, do_actions=True):
         try:
             result = self.expr._parse(string, loc, do_actions)
-            return ParseResults(
-                self, result.start, result.end, [result], result.failures
-            )
+            return ForwardResults(self, result.start, result.end, [result], result.failures)
         except Exception as cause:
             if is_null(self.expr):
                 Log.warning(
-                    "Ensure you have assigned a ParserElement (<<) to this Forward",
-                    cause=cause,
+                    "Ensure you have assigned a ParserElement (<<) to this Forward", cause=cause,
                 )
             raise cause from None
 
     def __regex__(self):
-        if self._reg or not self.expr:
-            return None
+        if self._in_regex:
+            Log.error("recursion not supported")
+
+        if not self.expr:
+            Log.error("Forward is incomplete")
 
         try:
-            self._reg = True
+            self._in_regex = True
             return self.expr.__regex__()
         finally:
-            self._reg = None
+            self._in_regex = None
 
     def __str__(self):
         if self.parser_name:
             return self.parser_name
 
         if self._str:
             return self._str
@@ -749,44 +707,44 @@
     Config = append_config(TokenConverter, "separator")
 
     def __init__(self, expr, separator=""):
         super(Combine, self).__init__(expr.streamline())
         self.set_config(separator=separator)
 
     def parse_impl(self, string, start, do_actions=True):
-        result = self.expr.parse_impl(string, start, do_actions=do_actions)
-        output = ParseResults(
-            self,
-            start,
-            result.end,
-            [result.as_string(sep=self.parser_config.separator)],
-            result.failures,
-        )
-        return output
+        try:
+            result = self.expr.parse_impl(string, start, do_actions=do_actions)
+            return ParseResults(
+                self, start, result.end, [result.as_string(sep=self.parser_config.separator)], result.failures,
+            )
+        except ParseException as cause:
+            raise ParseException(self, start, string, cause=cause)
 
     def streamline(self):
         if self.streamlined:
             return self
 
         expr = self.expr.streamline()
         if expr is self.expr:
             self.streamlined = True
             return self
-        return Combine(expr, self.parser_config.separator)
+        return Combine(expr, self.parser_config.separator).set_parser_name(self.parser_name)
 
     def expecting(self):
         return OrderedDict((k, [self]) for k in self.expr.expecting().keys())
 
     def min_length(self):
         return self.expr.min_length()
 
     def __regex__(self):
         return self.expr.__regex__()
 
     def __str__(self):
+        if self.parser_name:
+            return self.parser_name
         return text(self.expr)
 
 
 class Group(TokenConverter):
     """
     MARK A CLOSED PARSE RESULT
     """
@@ -853,14 +811,16 @@
     """
     Converter for ignoring the results of a parsed expression.
     """
 
     __slots__ = []
 
     def __init__(self, expr):
+        if isinstance(expr, text):
+            expr = Literal(expr)
         TokenConverter.__init__(self, expr)
         self.parse_action.append(_suppress_post_parse)
 
     def suppress(self):
         return self
 
     def __regex__(self):
@@ -945,23 +905,24 @@
         if self.parser_config.exact:
             return "*", f"(?<={self.expr.__regex__()[1]})"
         raise NotImplemented()
 
 
 LookBehind = PrecededBy
 
-
 export("mo_parsing.core", SkipTo)
 export("mo_parsing.core", Many)
 export("mo_parsing.core", ZeroOrMore)
 export("mo_parsing.core", OneOrMore)
 export("mo_parsing.core", Optional)
 export("mo_parsing.core", NotAny)
 export("mo_parsing.core", Suppress)
 export("mo_parsing.core", Group)
+export("mo_parsing.core",_suppress_post_parse)
+
 
 export("mo_parsing.results", Group)
 export("mo_parsing.results", Dict)
 export("mo_parsing.results", Suppress)
 
 export("mo_parsing.whitespaces", Empty)
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/exceptions.py` & `mo_parsing-8.639.24140/mo_parsing/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # encoding: utf-8
 import json
-from mo_future import text, is_text
+
+from mo_future import text, is_text, sort_using_cmp
 from mo_imports import export, expect
 
-from mo_parsing.utils import Log, listwrap, quote, indent
+from mo_parsing.utils import Log, enlist, quote, indent
 from mo_parsing.utils import col, line, lineno
 
 MatchFirst = expect("MatchFirst")
 
 
 class ParseException(Exception):
     """base exception class for all parsing runtime exceptions"""
@@ -25,45 +26,43 @@
         self.unsorted_cause = cause
         self._msg = msg
         self._causes = None
 
     @property
     def causes(self):
         if self._causes is None:
-            self._causes = sort_causes(self.unsorted_cause)
+            self._causes = sort_causes(enlist(self.unsorted_cause))
         return self._causes
 
     @property
     def __cause__(self):
-        if self.causes:
-            return self._causes[0]
-        else:
-            return None
+        return None
 
     @property
     def best_cause(self):
         if not self.causes:
             return self
 
-        best = sort_causes([
-            c.best_cause for c in self.causes if isinstance(c, ParseException)
-        ])
+        best = [c.best_cause for c in self.causes if isinstance(c, ParseException)]
         if not best:
             return self
-        elif self.expr.parser_name and self.start >= best[0].start:
+
+        best_0 = best[0]
+        if self.expr.parser_name and self.start >= best_0.start and not best_0.expr.parser_name:
             return self
         elif len(best) == 1:
-            return best[0]
+            return best_0
         else:
-            best_0 = best[0]
-            best_loc = best_0.loc
             return ParseException(
-                MatchFirst([b.expr for b in best if b.loc == best_loc]).streamline(),
+                MatchFirst([
+                    b.expr for b in best if compare_causes(b, best_0) == 0
+                ]).streamline(),
                 best_0.start,
                 best_0.string,
+                msg=best_0._msg,
                 cause=best,
             )
 
     @property
     def best_message(self):
         return self.best_cause.message
 
@@ -83,15 +82,15 @@
             expecting = f"{self._msg} ({self.expr})"
         else:
             expecting = f"Expecting {self.expr}"
 
         if self.loc >= len(self.string):
             found = ", found end of text"
         else:
-            found = f", found {quote(self.string[self.loc : self.loc + 10])}"
+            found = f", found {quote(self.string[self.loc: self.loc + 10])}"
 
         if self.causes and not isinstance(self.causes[0], ParseException):
             describe_cause = f", caused by {self.causes[0]}"
         else:
             describe_cause = ""
 
         location = f" (at char {self.loc}), (line:{self.lineno}, col:{self.column})"
@@ -183,14 +182,40 @@
 
     def __str__(self):
         return "RecursiveGrammarException: " + json.dumps([
             str(e) for e in self.parseElementTrace
         ])
 
 
+def compare_causes(a, b):
+    if isinstance(a, ParseException):
+        if isinstance(b, ParseException):
+            if a.loc < b.loc:
+                return 1
+            elif a.loc > b.loc:
+                return -1
+            elif b.expr.parser_name:
+                if a.expr.parser_name:
+                    return 0
+                else:
+                    return 1
+            elif a.expr.parser_name:
+                return -1
+            elif b._msg:
+                return 1
+            elif a._msg:
+                return -1
+            else:
+                return 0
+        else:
+            return 1
+    elif isinstance(b, ParseException):
+        return -1
+    else:
+        return 0
+
+
 def sort_causes(causes):
-    return list(sorted(
-        listwrap(causes), key=lambda e: -e.loc if isinstance(e, ParseException) else 0,
-    ))
+    return list(sort_using_cmp(causes, cmp=compare_causes))
 
 
 export("mo_parsing.utils", ParseException)
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/expressions.py` & `mo_parsing-8.639.24140/mo_parsing/expressions.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     Log,
     append_config,
     regex_caseless,
     regex_compile,
 )
 from mo_parsing.whitespaces import Whitespace
 
-LOOKUP_COST = 4
-
 
 class ParseExpression(ParserElement):
     """Abstract subclass of ParserElement, for combining and
     post-processing parsed tokens.
     """
 
     __slots__ = ["exprs"]
@@ -263,26 +261,29 @@
                 else:
                     index = self.parser_config.whitespace.skip(string, end)
             if isinstance(expr, And.SyntaxErrorGuard):
                 encountered_syntax_error = True
                 continue
             try:
                 result = expr._parse(string, index, do_actions)
+                failures.extend(result.failures)
+                if not result and index == result.end and isinstance(result.type, Many) and result.type.parser_config.min_match == 0:
+                    continue
                 acc.append(result)
-
                 end = result.end
-                if end > index:
-                    failures = result.failures
-                else:
-                    failures.extend(result.failures)
             except ParseException as pe:
+                failures.append(pe)
                 if encountered_syntax_error:
-                    raise ParseSyntaxException(pe.expr, pe.loc, pe.string, cause=pe) from None
+                    raise ParseSyntaxException(
+                        pe.expr, pe.loc, pe.string, cause=failures
+                    ) from None
                 else:
-                    raise pe from None
+                    raise ParseException(
+                        pe.expr, pe.loc, pe.string, cause=failures
+                    ) from None
 
         return ParseResults(self, start, end, acc, failures)
 
     def __add__(self, other):
         if other is Ellipsis:
             return _PendingSkip(self)
 
@@ -299,15 +300,23 @@
 
     def reverse(self):
         return And(
             [e.reverse() for e in self.exprs[::-1]], self.parser_config.whitespace
         )
 
     def __regex__(self):
-        return "+", "".join(regex_iso(*e.__regex__(), "+") for e in self.exprs)
+        if self.whitespace is whitespaces.NO_WHITESPACE:
+            return "+", "".join(regex_iso(*e.__regex__(), "+") for e in self.exprs)
+
+        return (
+            "+",
+            regex_iso(*self.whitespace.__regex__(), "+").join(
+                regex_iso(*e.__regex__(), "+") for e in self.exprs
+            ),
+        )
 
     def __str__(self):
         if self.parser_name:
             return self.parser_name
 
         subs = [text(e) for e in self.exprs]
         if all(len(s) == 1 for s in subs):
@@ -393,57 +402,52 @@
                 string,
                 msg="no defined alternatives to match",
                 cause=failures,
             )
         if len(matches) == 1:
             _, expr = matches[0]
             result = expr._parse(string, start, do_actions)
-            return ParseResults(
-                self, result.start, result.end, [result], result.failures
-            )
+            failures.extend(result.failures)
+            return ParseResults(self, result.start, result.end, [result], failures)
 
         if matches:
             # re-evaluate all matches in descending order of length of match, in case attached actions
             # might change whether or how much they match of the input.
             matches.sort(key=itemgetter(0), reverse=True)
 
             if not do_actions:
                 # no further conditions or parse actions to change the selection of
                 # alternative, so the first match will be the best match
                 _, expr = matches[0]
                 result = expr._parse(string, start, do_actions)
-                return ParseResults(
-                    self, result.start, result.end, [result], result.failures
-                )
+                failures.extend(result.failures)
+                return ParseResults(self, result.start, result.end, [result], failures)
 
             longest = -1, None
             for loc, expr in matches:
                 if loc <= longest[0]:
                     # already have a longer match than this one will deliver, we are done
                     return longest
 
                 try:
                     result = expr._parse(string, start, do_actions)
                 except ParseException as err:
                     failures.append(err)
                 else:
+                    failures.extend(result.failures)
                     if result.end >= loc:
                         return ParseResults(
-                            self, result.start, result.end, [result], result.failures
+                            self, result.start, result.end, [result], failures
                         )
                     # didn't match as much as before
                     elif result.end > longest[0]:
                         longest = (
                             result.end,
                             ParseResults(
-                                self,
-                                result.start,
-                                result.end,
-                                [result],
-                                result.failures,
+                                self, result.start, result.end, [result], failures,
                             ),
                         )
 
             if longest != (-1, None):
                 return longest
 
     def check_recursion(self, seen=empty_tuple):
@@ -494,26 +498,25 @@
             return 0
 
     @property
     def whitespace(self):
         return [e.whitespace for e in self.exprs]
 
     def parse_impl(self, string, start, do_actions=True):
-        causes = []
+        failures = []
 
         for e in self.alternate:
             try:
                 result = e._parse(string, start, do_actions)
-                return ParseResults(
-                    self, result.start, result.end, [result], result.failures
-                )
+                failures.extend(result.failures)
+                return ParseResults(self, result.start, result.end, [result], failures)
             except ParseException as cause:
-                causes.append(cause)
+                failures.append(cause)
 
-        raise ParseException(self, start, string, cause=causes)
+        raise ParseException(self, start, string, cause=failures)
 
     def streamline(self):
         if self.streamlined:
             return self
 
         output = ParseExpression.streamline(self)
 
@@ -566,15 +569,15 @@
     """
     BUILD A LOOKUP ARRAY TO MATCH ANY OF THE GIVEN exprs
     PERFORMS A REGEX, AND USES THE lower() CHARACTERS TO JUMP TO A SHORTLIST OF exprs THAT CAN MATCH
     :param exprs:
     :return: LESS EXPRESSIONS
     """
 
-    if len(exprs) < LOOKUP_COST:
+    if len(exprs) == 1:
         return exprs
 
     alternating = []
     # SOME NUMBER OF CONSTANT PATTERNS
     acc = []
     out = []
     has_expecting = True
@@ -629,20 +632,21 @@
     def __init__(self, maps):
         ParserElement.__init__(self)
 
         all_keys = set()
         lookup = OrderedDict()
         for m in maps:
             for k, ee in m.items():
+                k = k.lower()
                 all_keys.add(k)
                 lookup.setdefault(k, []).extend(ee)
 
         # patterns must be mutually exclusive to work
         items = list(lookup.items())
-        if len(maps) - max(len(v) for k, v in items) < LOOKUP_COST:
+        if len(maps) - max(len(v) for k, v in items) <= 1:
             Log.error("not useful")
 
         compact = []
         for k, e in items:
             min_k = k
             # FIND SHORTEST PREFIX
             for kk, ee in items:
@@ -652,15 +656,15 @@
             acc = []
             for kk, ee in items:
                 if kk.startswith(min_k):
                     acc.extend(ee)
                     ee.clear()
             if acc:
                 compact.append((min_k, acc))
-        if len(maps) - max(len(v) for k, v in compact) < LOOKUP_COST:
+        if len(maps) - max(len(v) for k, v in compact) <= 1:
             Log.error("not useful")
 
         # patterns can be shortened so far as they remain exclusive
         shorter = [
             (k[:min_length], e)
             for k, e in sorted(compact, key=lambda p: p[0])
             for min_length in [max(_distinct(k, kk) for kk, _ in compact if kk != k)]
@@ -680,14 +684,18 @@
             return self.lookup[index]
         return []
 
     def parse_impl(self, string, start, do_actions=True):
         found = self.regex.match(string, start)
         if found:
             index = found.group(0).lower()
+            if index not in self.lookup:
+                raise ParseException(
+                    self, start, string, "expecting one of " + json.dumps(self.all_keys)
+                )
             exprs = self.lookup[index]
 
             causes = []
             for e in exprs:
                 try:
                     return e._parse(string, start, do_actions)
                 except ParseException as cause:
@@ -707,34 +715,45 @@
 
     May be constructed using the ``'&'`` operator.
     """
 
     __slots__ = []
     Config = append_config(ParseExpression, "min_match", "max_match", "whitespace")
 
-    def __init__(self, exprs, whitespace):
+    def __init__(self, exprs):
         """
         :param exprs: The expressions to be matched
         :param mins: list of integers indincating any minimums
         """
-        super(MatchAll, self).__init__(exprs)
+        ParseExpression.__init__(self, exprs)
         self.set_config(
-            whitespace=whitespace,
+            whitespace=whitespaces.CURRENT,
             min_match=[
                 e.parser_config.min_match if isinstance(e, Many) else 1 for e in exprs
             ],
             max_match=[
                 e.parser_config.max_match if isinstance(e, Many) else 1 for e in exprs
             ],
         )
 
     def streamline(self):
         if self.streamlined:
             return self
-        return super(MatchAll, self).streamline()
+        output = ParseExpression.streamline(self)
+        output.set_config(
+            min_match=[
+                e.parser_config.min_match if isinstance(e, Many) else 1
+                for e in output.exprs
+            ],
+            max_match=[
+                e.parser_config.max_match if isinstance(e, Many) else 1
+                for e in output.exprs
+            ],
+        )
+        return output
 
     def _min_length(self):
         # TODO: MAY BE TOO CONSERVATIVE, WE MAY BE ABLE TO PROVE self CAN CONSUME A CHARACTER
         return min(e.min_length() for e in self.exprs)
 
     @property
     def whitespace(self):
@@ -793,14 +812,17 @@
                 f"Missing one or more required elements ({missing})",
                 failures,
             )
 
         # add any unmatched Optionals, in case they have default values defined
         match_order += [e for e in self.exprs if id(e) not in found]
 
+        if not match_order:
+            return ParseResults(self, start, start, [], failures)
+
         # TODO: CAN WE AVOID THIS RE-PARSE?
         results = []
         end = start
         for e in match_order:
             result = e._parse(string, end, do_actions)
             end = self.parser_config.whitespace.skip(string, result.end)
             results.append(result)
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/helpers.py` & `mo_parsing-8.639.24140/mo_parsing/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import re
 from datetime import datetime
 
 from mo_future import text
 
 from mo_parsing import whitespaces
 from mo_parsing.core import add_reset_action
-from mo_parsing.whitespaces import Whitespace, STANDARD_WHITESPACE, NO_WHITESPACE
 from mo_parsing.enhancement import (
     Combine,
     Dict,
     Forward,
     Group,
     OneOrMore,
     Optional,
@@ -40,14 +39,15 @@
     alphas,
     col,
     hexnums,
     nums,
     printables,
     Log,
 )
+from mo_parsing.whitespaces import Whitespace, STANDARD_WHITESPACE, NO_WHITESPACE
 
 
 def QuotedString(
     quote_char,
     esc_char=None,
     esc_quote=None,
     multiline=False,
@@ -91,28 +91,29 @@
 
     if multiline:
         anychar = AnyChar()
     else:
         anychar = Char(exclude="\n")
         excluded |= Char("\r\n")
 
-    included = ~Literal(end_quote_char) + anychar
+    with whitespaces.NO_WHITESPACE:
+        included = ~Literal(end_quote_char) + anychar
 
-    if esc_quote:
-        included = Literal(esc_quote) | included
-    if esc_char:
-        excluded |= Literal(esc_char)
-        included = esc_char + Char(printables) | included
-        esc_char_replace_pattern = re.escape(esc_char) + "(.)"
-
-    prec, pattern = (
-        Literal(quote_char) + ((~excluded + anychar) | included)[0:]
-    ).__regex__()
-    # IMPORTANT: THE end_quote_char IS OUTSIDE THE Regex BECAUSE OF PATHOLOGICAL BACKTRACKING
-    output = Combine(Regex(pattern) + Literal(end_quote_char))
+        if esc_quote:
+            included = Literal(esc_quote) | included
+        if esc_char:
+            excluded |= Literal(esc_char)
+            included = esc_char + Char(printables) | included
+            esc_char_replace_pattern = re.escape(esc_char) + "(.)"
+
+        prec, pattern = (
+            Literal(quote_char) + ((~excluded + anychar) | included)[0:]
+        ).__regex__()
+        # IMPORTANT: THE end_quote_char IS OUTSIDE THE Regex BECAUSE OF PATHOLOGICAL BACKTRACKING
+        output = Combine(Regex(pattern) + Literal(end_quote_char))
 
     def post_parse(tokens):
         ret = tokens[0]
         if unquote_results:
             # strip off quotes
             ret = ret[len(quote_char) : -len(end_quote_char)]
 
@@ -802,15 +803,14 @@
 _commasepitem = Combine(OneOrMore(
     Word(printables, exclude=",") + Optional(Word(" \t") + ~Literal(",") + ~LineEnd())
 )).set_parser_name("comma_item") / (lambda t: text(t).strip())
 commaSeparatedList = delimited_list(Optional(
     quoted_string | _commasepitem, default=""
 )).set_parser_name("commaSeparatedList")
 
-
 convertToInteger = token_map(int)
 convertToFloat = token_map(float)
 
 integer = Word(nums).set_parser_name("integer") / convertToInteger
 
 hex_integer = Word(hexnums).set_parser_name("hex integer") / token_map(int, 16)
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/infix.py` & `mo_parsing-8.639.24140/mo_parsing/infix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # encoding: utf-8
 import re
 import warnings
 
-from mo_dots import listwrap
 from mo_future import text, Iterable
 from mo_imports import delay_import
 
 from mo_parsing import whitespaces
 from mo_parsing.enhancement import (
     Combine,
     Forward,
@@ -19,16 +18,17 @@
 from mo_parsing.tokens import (
     CaselessKeyword,
     CaselessLiteral,
     Keyword,
     NoMatch,
     Literal,
     Empty,
+    Log,
 )
-from mo_parsing.utils import regex_range, wrap_parse_action
+from mo_parsing.utils import regex_range, wrap_parse_action, enlist
 
 Regex = delay_import("mo_parsing.regex.Regex")
 
 
 def delimited_list(expr, separator=",", combine=False):
     """
     PARSE DELIMITED LIST OF expr
@@ -54,19 +54,18 @@
 
      - strs - a string of space-delimited literals, or a collection of
        string literals
      - caseless - (default= ``False``) - treat all literals as caseless
      - as_keyword - (default=``False``) - enforce Keyword-style matching on the
        generated expressions
     """
-    if isinstance(caseless, text):
-        warnings.warn(
-            "More than one string argument passed to one_of, pass "
-            "choices as a list or space-delimited string",
-            stacklevel=2,
+    if isinstance(caseless, str):
+        Log.error(
+            "More than one string argument passed to one_of, pass choices as a list or"
+            " space-delimited string"
         )
 
     if caseless:
         isequal = lambda a, b: a.upper() == b.upper()
         masks = lambda a, b: b.upper().startswith(a.upper())
         parseElementClass = CaselessKeyword if as_keyword else CaselessLiteral
     else:
@@ -182,15 +181,15 @@
     * arity - same
     * assoc - same
     * parse_actions - same
     """
 
     for oper_def in spec:
         op, arity, assoc, rest = oper_def[0], oper_def[1], oper_def[2], oper_def[3:]
-        parse_actions = list(map(wrap_parse_action, listwrap(rest[0]))) if rest else []
+        parse_actions = list(map(wrap_parse_action, enlist(rest[0]))) if rest else []
         if arity == 1:
             is_suppressed, op = norm(op)
             if assoc == RIGHT_ASSOC:
                 op_list.append((
                     Group(base_expr + op),
                     op,
                     is_suppressed,
@@ -364,11 +363,11 @@
         result.end = tokens.end
         result.failures = tokens.failures
         return result
 
     flat = Forward()
     iso = lpar.suppress() + flat + rpar.suppress()
     atom = (base_expr | iso) / record_op(base_expr)
-    modified = ZeroOrMore(prefix_ops) + atom + ZeroOrMore(suffix_ops)
-    flat << ((modified + ZeroOrMore(ops + modified)) / make_tree).streamline()
+    decorated = ZeroOrMore(prefix_ops) + atom + ZeroOrMore(suffix_ops)
+    flat << ((decorated + ZeroOrMore(ops + decorated)) / make_tree).streamline()
 
     return flat.streamline()
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/profile.py` & `mo_parsing-8.639.24140/mo_parsing/profile.py`

 * *Files identical despite different names*

### Comparing `mo-parsing-8.6.21337/mo_parsing/regex.py` & `mo_parsing-8.639.24140/mo_parsing/regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from collections import OrderedDict
 from string import whitespace
 
 from mo_future import unichr, is_text
 from mo_imports import export
 
 from mo_parsing.core import add_reset_action
-from mo_parsing.whitespaces import Whitespace, NO_WHITESPACE
 from mo_parsing.enhancement import (
     Char,
     NotAny,
     ZeroOrMore,
     OneOrMore,
     Optional,
     Many,
     Combine,
     Group,
     Forward,
     LookAhead,
-    ParseEnhancement, LookBehind,
+    ParseEnhancement,
+    LookBehind,
 )
 from mo_parsing.expressions import MatchFirst, And
 from mo_parsing.infix import delimited_list
 from mo_parsing.results import ParseResults, Annotation
 from mo_parsing.tokens import (
     Literal,
     AnyChar,
@@ -38,18 +38,19 @@
 from mo_parsing.utils import (
     printables,
     alphas,
     alphanums,
     nums,
     hexnums,
     Log,
-    listwrap,
+    enlist,
     regex_compile,
     ParseException,
 )
+from mo_parsing.whitespaces import Whitespace, NO_WHITESPACE
 
 __all__ = ["Regex"]
 
 
 def hex_to_char(t):
     return Literal(unichr(int(t.value().lower().split("x")[1], 16)))
 
@@ -58,15 +59,15 @@
     min_ = tokens["min"].parser_config.match
     max_ = tokens["max"].parser_config.match
     return Char("".join(unichr(i) for i in range(ord(min_), ord(max_) + 1)))
 
 
 def to_bracket(tokens):
     acc = []
-    for e in listwrap(tokens["body"].value()):
+    for e in enlist(tokens["body"].value()):
         if isinstance(e, SingleCharLiteral):
             acc.append(e.parser_config.match)
         elif isinstance(e, Char):
             acc.extend(e.parser_config.include)
         else:
             Log.error("programmer error")
     if tokens["negate"]:
@@ -249,15 +250,15 @@
     | group
 )
 
 more = (term + Optional(repetition, NO_WHITESPACE)) / repeat
 sequence = OneOrMore(more, NO_WHITESPACE) / (lambda t: And(t, NO_WHITESPACE))
 regex << (
     delimited_list(sequence, separator="|").set_token_name("value")
-    / (lambda t: MatchFirst(listwrap(t.value())).streamline())
+    / (lambda t: MatchFirst(enlist(t.value())).streamline())
 ).streamline()
 regex = regex.finalize()
 
 parameters = (
     "\\" + Char(alphanums)("name") | "\\g<" + Word(alphas, alphanums)("name") + ">"
 ) / (lambda t: t["name"])
 NO_WHITESPACE.release()
@@ -366,7 +367,8 @@
         else:
             return self.expr.__regex__()
 
 
 _plain_group = Group(None)
 
 export("mo_parsing.core", "regex_parameters", parameters)
+export("mo_parsing.tokens", Regex)
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/results.py` & `mo_parsing-8.639.24140/mo_parsing/results.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,67 @@
 # encoding: utf-8
 import inspect
 
-from mo_dots import is_many, is_null
-from mo_future import is_text, text, NEXT, zip_longest, MutableMapping
+from mo_dots import is_many, is_null, register_data, register_list, exists
+from mo_future import is_text, text, zip_longest, MutableMapping
 from mo_imports import expect, export
 
-from mo_parsing.utils import Log, listwrap, is_forward, forward_type
+from mo_parsing.utils import Log, enlist
 
 Suppress, ParserElement, NO_PARSER, NO_RESULTS, Group, Dict, Token, Empty = expect(
     "Suppress",
     "ParserElement",
     "NO_PARSER",
     "NO_RESULTS",
     "Group",
     "Dict",
     "Token",
     "Empty",
 )
 
 
 class ParseResults(object):
-    __slots__ = ["type", "start", "end", "tokens", "timing", "failures"]
+    __slots__ = ["_type", "start", "end", "tokens", "timing", "failures"]
 
     @property
     def name(self):
-        return self.type.token_name
+        return self._type.token_name
+
+    @property
+    def type(self):
+        return self._type
 
     def __init__(self, result_type, start, end, tokens, failures):
         if end == -1:
             Log.error("not allowed")
-        self.type = result_type
+        self._type = result_type
         self.start = start
         self.end = end
         self.tokens = tokens
         self.timing = None
         self.failures = failures
 
     def _get_item_by_name(self, name):
-        # return open list of (modal, value) pairs
-        # modal==True means only the last value is relevant
+        # return open list of values for given name
         for tok in self.tokens:
             if isinstance(tok, ParseResults):
                 if tok.name == name:
                     if isinstance(tok.type, Group):
                         yield tok
                     else:
                         for t in tok.tokens:
-                            for tt in _flatten(t):
-                                yield tt
+                            yield from _flatten(t)
                     continue
                 elif tok.name:
                     continue
                 elif isinstance(tok.type, Group):
                     continue
-                elif is_forward(tok.type) and isinstance(tok.tokens[0].type, Group):
-                    continue
-                for f in tok._get_item_by_name(name):
-                    yield f
+                yield from tok._get_item_by_name(name)
 
     def __getitem__(self, item):
-        if is_forward(self.type):
-            return self.tokens[0][item]
-
         if is_text(item):
             values = list(self._get_item_by_name(item))
             if len(values) == 0:
                 return NO_RESULTS
             if len(values) == 1:
                 return values[0]
             # ENCAPSULATE IN A ParseResults FOR FURTHER NAVIGATION
@@ -84,40 +80,34 @@
     def __setitem__(self, k, v):
         if isinstance(k, (slice, int)):
             Log.error("not supported")
 
         if v is None:
             v = NO_RESULTS
 
-        if is_forward(self.type):
-            self.tokens[0][k] = v
-            return
-
         for i, tok in enumerate(self.tokens):
             if isinstance(tok, ParseResults):
                 if tok.name == k:
                     self.tokens[i] = v
                     v = NO_RESULTS  # ERASE ALL OTHERS
                 elif isinstance(tok.type, Group):
                     continue
-                elif is_forward(tok.type) and isinstance(tok.tokens[0].type, Group):
-                    continue
                 elif tok.name:
                     continue
 
                 tok.__setitem__(k, NO_RESULTS)  # ERASE ALL CHILDREN
 
         if v is not NO_RESULTS:
             tokens = self.tokens
-            if is_forward(self.type):
+            if isinstance(self, ForwardResults):
                 tokens = tokens[0].tokens
             if isinstance(v, ParseResults):
                 tokens.append(Annotation(k, v.start, v.end, v.tokens))
             else:
-                tokens.append(Annotation(k, -1, 0, listwrap(v)))
+                tokens.append(Annotation(k, -1, 0, enlist(v)))
 
     def __contains__(self, k):
         return any((r.name) == k for r in self.tokens)
 
     def length(self):
         return sum(1 for _ in self)
 
@@ -140,81 +130,55 @@
                 if self[k] != v:
                     return False
             return True
         else:
             Log.error("do not know how to handle")
 
     def __bool__(self):
-        try:
-            NEXT(self.items())()
-            return True
-        except Exception:
-            pass
-
-        try:
-            NEXT(self.__iter__())()
-            return True
-        except Exception:
+        if not self.tokens:
             return False
 
-    __nonzero__ = __bool__
+        for r in self.tokens:
+            if not isinstance(r, ParseResults):
+                return True
+            elif r.name:
+                return True
+            elif isinstance(r.type, Group):
+                return True
+            else:
+                if r.__bool__():
+                    return True
 
-    def __iter__(self):
-        if is_forward(self.type):
-            if len(self.tokens) != 1:
-                Log.error("not expected")
+        return False
 
-            yield from self.tokens[0]
-            return
+    __nonzero__ = __bool__
+
+    def __len__(self):
+        return sum(1 for _ in self)
 
+    def __iter__(self):
         for r in self.tokens:
             if isinstance(r, Annotation):
                 continue
-            elif isinstance(r, ParseResults):
-                if isinstance(r, Annotation):
-                    return
-                elif isinstance(r.type, Group):
-                    yield r
-                elif is_forward(r.type) and isinstance(forward_type(r), Group):
-                    yield r
-                # elif is_forward(r.type):
-                #     r = self.tokens[0]
-                #     if isinstance(r.type, Group):
-                #         yield r
-                #     else:
-                #         yield from r
-                elif not isinstance(r.type, Group):
-                    yield from r
-            else:
+            elif not isinstance(r, ParseResults):
+                yield r
+            elif isinstance(r.type, Group):
                 yield r
+            else:
+                yield from r
 
     def __delitem__(self, key):
         if isinstance(key, (int, slice)):
             Log.error("not allowed")
         else:
             self[key] = NO_RESULTS
 
     def __reversed__(self):
         return reversed(self.tokens)
 
-    # def __getattr__(self, item):
-    #     """
-    #     IF THERE IS ONLY ONE VALUE, THEN DEFER TO IT
-    #     """
-    #     iter = self.__iter__()
-    #     try:
-    #         v1 = iter.__next__()
-    #         try:
-    #             iter.__next__()
-    #             raise Log.error("No attribute {{item}} for mutiple tokens", item=item)
-    #         except Exception:
-    #             return getattr(v1, item)
-    #     except Exception as cause:
-    #         raise AttributeError(f"No attribute {item}")
-
     def value(self):
         """
         RETURN WHATEVER PRIMITIVE VALUES ARE LEFT
         """
         value = [v.value() if isinstance(v, ParseResults) else v for v in self]
         if not value:
             return None
@@ -228,33 +192,27 @@
             yield k
 
     def values(self):
         for _, v in self.items():
             yield v
 
     def items(self):
-        if is_forward(self.type):
-            for k, v in self.tokens[0].items():
-                yield k, v
-            return
-
         output = {}
         for tok in self.tokens:
             if isinstance(tok, ParseResults):
+                if isinstance(tok.type, Suppress):
+                    continue
                 if tok.name:
                     add(output, tok.name, [tok])
                     continue
                 if isinstance(tok.type, Group):
                     continue
-                if is_forward(tok.type) and isinstance(tok.tokens[0].type, Group):
-                    continue
                 for k, v in tok.items():
                     add(output, k, v)
-        for k, v in output.items():
-            yield k, v
+        yield from output.items()
 
     def get(self, key, default_value=None):
         """
         Returns named result matching the given key, or if there is no
         such name, then returns the given ``default_value``
 
         Similar to ``dict.get()``.
@@ -263,15 +221,15 @@
             return self[key]
         else:
             return default_value
 
     def __contains__(self, item):
         if item is Ellipsis:
             return False
-        return bool(self[item])
+        return exists(self[item])
 
     def __add__(self, other):
         # if not isinstance(other, ParseResults):
         #     return self.value() + other
         #
         return ParseResults(
             Group(self.type + other.type),
@@ -370,43 +328,49 @@
         )
         return ret
 
     def get_name(self):
         r"""
         Returns the results name for this token expression. Useful when several
         different expressions might match at a particular location.
-
-        Example::
-
-            integer = Word(nums)
-            ssn_expr = Regex(r"\d\d\d-\d\d-\d\d\d\d")
-            house_number_expr = Suppress('#') + Word(nums, alphanums)
-            user_data = (Group(house_number_expr)("house_number")
-                        | Group(ssn_expr)("ssn")
-                        | Group(integer)("age"))
-            user_info = OneOrMore(user_data)
-
-            result = user_info.parse_string("22 111-22-3333 #221B")
-            for item in result:
-                print(item.get_name(), ':', item[0])
-
-        prints::
-
-            age : 22
-            ssn : 111-22-3333
-            house_number : 221B
         """
         if self.name:
             return self.name
         elif len(self.tokens) == 1:
             return self.tokens[0].name
         else:
             return ""
 
 
+class ForwardResults(ParseResults):
+    __slots__ = []
+
+    @property
+    def type(self):
+        return self.tokens[0].type
+
+    def __getitem__(self, item):
+        return self.tokens[0][item]
+
+    def __setitem__(self, k, v):
+        self.tokens[0][k] = v
+
+    def __bool__(self):
+        return self.tokens[0].__bool__()
+
+    def __iter__(self):
+        if len(self.tokens) != 1:
+            Log.error("not expected")
+
+        yield from self.tokens[0]
+
+    def items(self):
+        yield from self.tokens[0].items()
+
+
 def _flatten(token):
     """
     FLATTEN SOME, LEAVING ANY IMPORTANT FEATURES (names or groups)
     """
     if not isinstance(token, ParseResults):
         yield token
     elif isinstance(token.type, Group):
@@ -448,12 +412,12 @@
         return "{" + text(self.name) + ": " + text(self.tokens) + "}"
 
     def __repr__(self):
         return "Annotation(" + repr(self.name) + ", " + repr(self.tokens) + ")"
 
 
 MutableMapping.register(ParseResults)
+register_data(ParseResults)
+register_list(ParseResults)
 
-from mo_parsing import utils
-utils.register_type(ParseResults)
-
+from mo_parsing import whitespaces
 export("mo_parsing.utils", ParseResults)
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/tokens.py` & `mo_parsing-8.639.24140/mo_parsing/tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # encoding: utf-8
 
 from mo_future import is_text
 from mo_imports import export
 
-from mo_parsing import whitespaces, LookBehind
+from mo_parsing import whitespaces
 from mo_parsing.core import ParserElement
-from mo_parsing.whitespaces import Whitespace
 from mo_parsing.exceptions import ParseException
 from mo_parsing.results import ParseResults
 from mo_parsing.utils import *
+from mo_parsing.whitespaces import Whitespace
+
+Regex = expect("Regex")
 
 
 class Token(ParserElement):
     """
     Represent some contiguous set for characters, no whitespace
     """
 
@@ -115,15 +117,15 @@
     __slots__ = []
 
     def __init__(self, match):
         if not is_text(match):
             Log.error("Expecting string for literal")
         Token.__init__(self)
 
-        self.set_config(match=match)
+        self.set_config(match=match, regex=regex_compile(re.escape(match)))
 
         if len(match) == 0:
             Log.error("Literal must be at least one character")
         elif len(match) == 1:
             self.__class__ = SingleCharLiteral
 
     def parse_impl(self, string, start, do_actions=True):
@@ -139,17 +141,19 @@
     def _min_length(self):
         return len(self.parser_config.match)
 
     def reverse(self):
         return Literal(self.parser_config.match[::-1])
 
     def __regex__(self):
-        return "+", re.escape(self.parser_config.match)
+        return "+", self.parser_config.regex.pattern
 
     def __str__(self):
+        if self.parser_name:
+            return self.parser_name
         return self.parser_config.match
 
 
 class SingleCharLiteral(Literal):
     __slots__ = []
 
     def parse_impl(self, string, start, do_actions=True):
@@ -165,33 +169,35 @@
 
     def min_length(self):
         return 1
 
     def reverse(self):
         return self
 
-    def __regex__(self):
-        return "*", re.escape(self.parser_config.match)
-
 
 class Keyword(Token):
     __slots__ = []
     Config = append_config(Token, "ident_chars")
 
     def __init__(
         self,
         match,
-        ident_chars=None,  # required to identify word boundary
+        ident_chars = None,  # required to identify word boundary
         caseless=None,
     ):
         Token.__init__(self)
         if ident_chars is None:
             ident_chars = whitespaces.CURRENT.keyword_chars
-        else:
-            ident_chars = "".join(sorted(set(ident_chars)))
+        elif isinstance(ident_chars, Regex):
+            ident_chars = ident_chars.expr.parser_config.include
+
+        if caseless:
+            ident_chars = ident_chars.lower() + ident_chars.upper()
+
+        ident_chars = "".join(sorted(set(ident_chars)))
 
         if caseless:
             pattern = regex_caseless(match)
         else:
             pattern = re.escape(match)
 
         non_word = "($|(?!" + regex_range(ident_chars) + "))"
@@ -246,19 +252,23 @@
     Note: the matched results will always be in the case of the given
     match string, NOT the case of the input text.
     """
 
     __slots__ = []
 
     def __init__(self, match):
-        Literal.__init__(self, match.upper())
+        if not is_text(match):
+            Log.error("Expecting string for literal")
+        if len(match) == 0:
+            Log.error("Literal must be at least one character")
+        Token.__init__(self)
         self.set_config(
-            match=match, regex=regex_compile(regex_caseless(match)),
+            match=match, regex=regex_compile(regex_caseless(re.escape(match))),
         )
-        self.parser_name = repr(self.parser_config.regex.pattern)
+        self.parser_name = match
 
     def parse_impl(self, string, start, do_actions=True):
         found = self.parser_config.regex.match(string, start)
         if found:
             return ParseResults(
                 self, start, found.end(), [self.parser_config.match], []
             )
@@ -343,37 +353,42 @@
         max=None,
         exact=0,
         as_keyword=False,  # IF WE EXPECT NON-WORD CHARACTERS BEFORE AND AFTER
         exclude="",
     ):
         Token.__init__(self)
 
+        # TODO: REPLACE body_chars AND init_chars WITH ANY PATTERN?
         if body_chars is None:
             body_chars = init_chars
         if exact:
             min = max = exact
 
         if min < 1:
             raise ValueError(
                 "cannot specify a minimum length < 1; use Optional(Word()) if"
                 " zero-length word is permitted"
             )
 
         if body_chars == init_chars:
+            if init_chars.__class__.__name__ == "Regex":
+                init_chars = init_chars.expecting().keys()
             prec, regexp = Char(init_chars, exclude=exclude)[min:max].__regex__()
         elif max is None or max == MAX_INT:
-            prec, regexp = (
-                Char(init_chars, exclude=exclude)
-                + Char(body_chars, exclude=exclude)[min - 1 :]
-            ).__regex__()
+            with whitespaces.NO_WHITESPACE:
+                prec, regexp = (
+                    Char(init_chars, exclude=exclude)
+                    + Char(body_chars, exclude=exclude)[min - 1 :]
+                ).__regex__()
         else:
-            prec, regexp = (
-                Char(init_chars, exclude=exclude)
-                + Char(body_chars, exclude=exclude)[min - 1 : max - 1]
-            ).__regex__()
+            with whitespaces.NO_WHITESPACE:
+                prec, regexp = (
+                    Char(init_chars, exclude=exclude)
+                    + Char(body_chars, exclude=exclude)[min - 1 : max - 1]
+                ).__regex__()
 
         if as_keyword:
             regexp = r"\b" + regexp + r"\b"
 
         self.regex = regex_compile(regexp)
         self.set_config(min=min, init_chars=init_chars)
 
@@ -546,32 +561,32 @@
 
     white_strs = {
         " ": "<SP>",
         "\t": "<TAB>",
         "\n": "<LF>",
         "\r": "<CR>",
         "\f": "<FF>",
-        "u\00A0": "<NBSP>",
-        "u\1680": "<OGHAM_SPACE_MARK>",
-        "u\180E": "<MONGOLIAN_VOWEL_SEPARATOR>",
-        "u\2000": "<EN_QUAD>",
-        "u\2001": "<EM_QUAD>",
-        "u\2002": "<EN_SPACE>",
-        "u\2003": "<EM_SPACE>",
-        "u\2004": "<THREE-PER-EM_SPACE>",
-        "u\2005": "<FOUR-PER-EM_SPACE>",
-        "u\2006": "<SIX-PER-EM_SPACE>",
-        "u\2007": "<FIGURE_SPACE>",
-        "u\2008": "<PUNCTUATION_SPACE>",
-        "u\2009": "<THIN_SPACE>",
-        "u\200A": "<HAIR_SPACE>",
-        "u\200B": "<ZERO_WIDTH_SPACE>",
-        "u\202F": "<NNBSP>",
-        "u\205F": "<MMSP>",
-        "u\3000": "<IDEOGRAPHIC_SPACE>",
+        "\u00A0": "<NBSP>",
+        "\u1680": "<OGHAM_SPACE_MARK>",
+        "\u180E": "<MONGOLIAN_VOWEL_SEPARATOR>",
+        "\u2000": "<EN_QUAD>",
+        "\u2001": "<EM_QUAD>",
+        "\u2002": "<EN_SPACE>",
+        "\u2003": "<EM_SPACE>",
+        "\u2004": "<THREE-PER-EM_SPACE>",
+        "\u2005": "<FOUR-PER-EM_SPACE>",
+        "\u2006": "<SIX-PER-EM_SPACE>",
+        "\u2007": "<FIGURE_SPACE>",
+        "\u2008": "<PUNCTUATION_SPACE>",
+        "\u2009": "<THIN_SPACE>",
+        "\u200A": "<HAIR_SPACE>",
+        "\u200B": "<ZERO_WIDTH_SPACE>",
+        "\u202F": "<NNBSP>",
+        "\u205F": "<MMSP>",
+        "\u3000": "<IDEOGRAPHIC_SPACE>",
     }
 
     __slots__ = []
     Config = append_config(Token, "min_len", "max_len", "white_chars")
 
     def __init__(self, ws=" \t\r\n", min=1, max=0, exact=0):
         Token.__init__(self)
@@ -636,14 +651,15 @@
 class LineEnd(Token):
     """
     Matches if current position is at the end of a line
     """
 
     zero_length = True
     __slots__ = []
+
     # Config = append_config(Token, "regex")
 
     def __init__(self):
         with Whitespace(" \t"):
             Token.__init__(self)
             self.parser_name = self.__class__.__name__
             self.set_config(regex=regex_compile("\\r?(\\n|$)"))
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/utils.py` & `mo_parsing-8.639.24140/mo_parsing/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import string
 import sys
 import warnings
 from collections import namedtuple
 from math import isnan
 from types import FunctionType
 
-from mo_dots import is_null, Null
+from mo_dots import is_null, Null, is_many
 from mo_future import unichr, text, generator_types, get_function_name
 from mo_imports import expect
 
 ParseResults, ParseException, Many = expect("ParseResults", "ParseException", "Many")
 
 
 def append_config(base, *slots):
@@ -42,42 +42,20 @@
 
         @classmethod
         def alert(cls, template, cause=None, **params):
             print()
 
         @classmethod
         def error(cls, template, cause=None, **params):
-            raise ParseException(Null, -1, -1, "", msg=template, cause=cause)
+            raise ParseException(Null, -1, "", msg=template, cause=cause)
 
 
 MAX_INT = sys.maxsize
 empty_list = []
 empty_tuple = tuple()
-many_types = (list, tuple, set) + generator_types
-
-
-def register_type(t):
-    global many_types
-    many_types = many_types + (t,)
-
-
-def extend(cls):
-    """
-    DECORATOR TO ADD METHODS TO CLASSES
-    :param cls: THE CLASS TO ADD THE METHOD TO
-    :return:
-    """
-
-    def extender(func):
-        setattr(cls, get_function_name(func), func)
-        return func
-
-    return extender
-
-
 _prec = {"|": 0, "+": 1, "*": 2}
 
 
 def regex_compile(pattern):
     """REGEX COMPILE WITHOUT THE ON-A-SINGLE-LINE ASSUMPTION"""
     try:
         return re.compile(pattern, re.DOTALL)
@@ -192,27 +170,28 @@
     try:
         s = float(s)
         return not isnan(s)
     except Exception:
         return False
 
 
-def listwrap(value):
+def enlist(value):
     """
     PERFORMS THE FOLLOWING TRANSLATION
     None -> []
     value -> [value]
     [...] -> [...]  (unchanged list)
     """
     if is_null(value):
         return []
-    elif isinstance(value, many_types):
+    elif is_many(value):
         return value
     else:
         return [value]
+listwrap = enlist
 
 
 def coalesce(*args):
     # pick the first not null value
     # http://en.wikipedia.org/wiki/Null_coalescing_operator
     for a in args:
         if a != None:
@@ -237,14 +216,15 @@
 
 singleArgTypes = [
     int,
     float,
     str,
     bool,
     complex,
+    dict,
 ]
 
 builtin_lookup = {"".join.__name__: ("iterable",)}
 
 
 def is_forward(expr):
     return expr.__class__.__name__ == "Forward"
@@ -256,24 +236,14 @@
     """
     return (
         isinstance(expr, Many)
         and expr.parser_config.max_match - expr.parser_config.min_match > 3
     )
 
 
-def forward_type(expr):
-    """
-    :param expr:
-    :return:  Effective type of this Forward
-    """
-    while is_forward(expr.type):
-        expr = expr.tokens[0]
-    return expr.type
-
-
 def stack_depth():
     count = 0
     f = sys._getframe()
     while f:
         f = f.f_back
         count += 1
     return count
@@ -282,37 +252,14 @@
 def get_function_arguments(func):
     try:
         return func.__code__.co_varnames[: func.__code__.co_argcount]
     except Exception as e:
         return builtin_lookup.get(func.__name__, ("unknown",))
 
 
-class __config_flags:
-    """Internal class for defining compatibility and debugging flags"""
-
-    _all_names = []
-    _fixed_names = []
-    _type_desc = "configuration"
-
-    @classmethod
-    def _set(cls, dname, value):
-        if dname in cls._fixed_names:
-            warnings.warn("{}.{} {} is {} and cannot be overridden".format(
-                cls.__name__, dname, cls._type_desc, str(getattr(cls, dname)).upper(),
-            ))
-            return
-        if dname in cls._all_names:
-            setattr(cls, dname, value)
-        else:
-            raise ValueError("no such {} {!r}".format(cls._type_desc, dname))
-
-    enable = classmethod(lambda cls, name: cls._set(name, True))
-    disable = classmethod(lambda cls, name: cls._set(name, False))
-
-
 alphas = string.ascii_uppercase + string.ascii_lowercase
 nums = "0123456789"
 hexnums = nums + "ABCDEFabcdef"
 alphanums = alphas + nums
 printables = "".join(c for c in string.printable if c not in string.whitespace)
 
 
@@ -387,28 +334,29 @@
             args = token, index, string
             result = func(*args[:num_args])
             if result is None:
                 return token
             elif isinstance(result, ParseResults):
                 if (result.start < token.start) or (token.end < result.end):
                     Log.error("Tokens must be ordered")
+                result.failures.extend(token.failures)
                 return result
 
             if isinstance(result, (list, tuple)):
                 return ParseResults(
                     token.type, token.start, token.end, result, token.failures
                 )
             else:
                 return ParseResults(
                     token.type, token.start, token.end, [result], token.failures
                 )
         except ParseException as pe:
             raise
         except Exception as cause:
-            Log.error("parse action should not raise exception", cause=cause)
+            Log.error("parse action {{name}} should not raise exception", name=func_name, cause=cause)
 
     # copy func name to wrapper for sensible debug output
     try:
         func_name = getattr(func, "__name__", getattr(func, "__class__").__name__)
     except Exception:
         func_name = str(func)
     wrapper.__name__ = func_name
```

### Comparing `mo-parsing-8.6.21337/mo_parsing/whitespaces.py` & `mo_parsing-8.639.24140/mo_parsing/whitespaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,18 @@
         self.ignore_list = []
         self.debug_actions = DebugActions(noop, noop, noop)
         self.all_exceptions = {}
         self.content = None
         self.skips = {}
         self.regex = None
         self.expr = None
-        self.set_whitespace(white)
         self.parent = None
         self.copies = []
+        self._in_regex = False
+        self.set_whitespace(white)
 
     def copy(self):
         output = Whitespace(self.white_chars)
         output.id = self.id
         output.literal = self.literal
         output.keyword_chars = self.keyword_chars
         output.ignore_list = list(self.ignore_list)
@@ -58,15 +59,14 @@
         return new_whitespace
 
     use = __enter__
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
         REMOVE THIS WHITESPACE CONTEXT
-        :return:
         """
         global CURRENT
         if self.copies and self.copies[-1] is CURRENT:
             self.copies.pop()
             CURRENT = whitespace_stack.pop()
             return
 
@@ -80,18 +80,15 @@
     def release(self):
         self.__exit__(None, None, None)
 
     def normalize(self, expr):
         if expr == None:
             return None
         if is_text(expr):
-            if issubclass(self.literal, Token):
-                return self.literal(expr)
-            else:
-                return self.literal(Literal(expr))
+            return self.literal(expr)
         if isinstance(expr, type) and issubclass(expr, ParserElement):
             return expr()  # ALLOW Empty WHEN Empty() WAS INTENDED
         if not isinstance(expr, ParserElement):
             Log.error("expecting string, or ParserElemenet")
 
         return expr
 
@@ -108,28 +105,28 @@
         self.keyword_chars = "".join(sorted(set(chars)))
 
     def set_whitespace(self, chars):
         self.id = id(self)
         self.white_chars = "".join(sorted(set(chars)))
         self.content = None
         self.expr = None if isinstance(Empty, Expecting) else Empty()
-        self.regex = re.compile(self.__regex__()[1])
+        self.regex = re.compile(self.__regex__()[1], re.DOTALL)
 
     def add_ignore(self, *ignore_exprs):
         """
         ADD TO THE LIST OF IGNORED EXPRESSIONS
         :param ignore_expr:
         """
         self.id = id(self)
         for ignore_expr in ignore_exprs:
             ignore_expr = ignore_expr.suppress()
             self.ignore_list.append(ignore_expr)
             self.content = None
             self.expr = None if isinstance(Empty, Expecting) else Empty()
-            self.regex = re.compile(self.__regex__()[1])
+            self.regex = re.compile(self.__regex__()[1], re.DOTALL)
             return self
 
     def backup(self):
         return Backup(self)
 
     def parse_impl(self, string, start, do_actions=True):
         end = self.skip(string, start)
@@ -161,23 +158,29 @@
         found = self.regex.match(string, start)
         if found:
             end = found.end()
         self.skips[start] = end  # THE REAL VALUE
         return end
 
     def __regex__(self):
-        white = regex_range(self.white_chars)
-        if not self.ignore_list:
-            if not white:
-                return "*", ""
-            else:
-                return "*", white + "*"
-
-        ignored = "|".join(regex_iso(*i.__regex__(), "|") for i in self.ignore_list)
-        return "+", f"(?:{white}*(?:{ignored}))*{white}*"
+        if self._in_regex:
+            return "*", ""
+        self._in_regex = True
+        try:
+            white = regex_range(self.white_chars)
+            if not self.ignore_list:
+                if not white:
+                    return "*", ""
+                else:
+                    return "*", white + "*"
+
+            ignored = "|".join(regex_iso(*i.__regex__(), "|") for i in self.ignore_list)
+            return "+", f"(?:{white}*(?:{ignored}))*{white}*"
+        finally:
+            self._in_regex = False
 
     def __str__(self):
         output = ["{"]
         for k, v in self.__dict__.items():
             value = str(v)
             output.append(indent(quote(k) + ":" + value))
         output.append("}")
```

### Comparing `mo-parsing-8.6.21337/setup.py` & `mo_parsing-8.639.24140/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # encoding: utf-8
 # THIS FILE IS AUTOGENERATED!
-from __future__ import unicode_literals
 from setuptools import setup
 setup(
     author='Various',
     author_email='kyle@lahnakoski.com',
-    classifiers=["Development Status :: 4 - Beta","License :: OSI Approved :: MIT License","Programming Language :: Python :: 3.7","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules"],
+    classifiers=["Development Status :: 4 - Beta","License :: OSI Approved :: MIT License","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='Another PEG Parsing Tool',
-    extras_require={"tests":["mo-testing","mo-threads","mo-logs","mo-files"]},
-    install_requires=["mo-dots==8.4.21326","mo-future==6.2.21303"],
+    description_content_type='text/plain',
+    extras_require={"tests":["mo-testing>=7.562.24075","mo-threads>=6.562.24075","mo-logs>=8.562.24075","mo-files>=6.562.24075"]},
+    install_requires=["mo-dots==10.632.24139","mo-future==7.584.24095"],
     license='MIT',
-    long_description='# More Parsing!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-parsing.svg)](https://pypi.org/project/mo-parsing/)\n[![Build Status](https://app.travis-ci.com/klahnakoski/mo-parsing.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-parsing)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-parsing/badge.svg?branch=master)](https://coveralls.io/github/klahnakoski/mo-parsing?branch=master)\n\nA fork of [pyparsing](https://github.com/pyparsing/pyparsing) for faster parsing\n\n\n## Installation\n\nThis is a pypi package\n\n    pip install mo-parsing\n    \n## Usage\n\nThis module allows you to define a PEG parser using predefined patterns and Python operators.  Here is an example \n\n```\n>>> from mo_parsing import Word\n>>> from mo_parsing.utils import alphas\n>>>\n>>> greet = Word(alphas)("greeting") + "," + Word(alphas)("person") + "!"\n>>> result = greet.parse_string("Hello, World!")\n```\n\nThe `result` can be accessed as a nested list\n\n```\n>>> list(result)\n[\'Hello\', \',\', \'World\', \'!\']\n```\n\nThe `result` can also be accessed as a dictionary\n\n```\n>>> dict(result)\n{\'greeting\': \'Hello\', \'person\': \'World\'}\n```\n\nRead the [pyparsing documentation](https://github.com/pyparsing/pyparsing/#readme) for more\n\n### The `Whitespace` Skipper\n\nThe `mo_parsing.whitespaces.CURRENT` is used during parser creation: It is effectively defines what "whitespace" to skip during parsing, with additional features to simplify the language definition.  You declare "standard" `Whitespace` like so:\n\n    with Whitespace() as whitespace:\n        # PUT YOUR LANGUAGE DEFINITION HERE (space, tab and CR are "whitespace")\n\nIf you are declaring a large language, and you want to minimize indentation, and you are careful, you may also use this pattern:\n\n    whitespace = Whitespace().use()\n    # PUT YOUR LANGUAGE DEFINITION HERE\n    whitespace.release()\n\nThe whitespace can be used to set global parsing parameters, like\n\n* `set_whitespace()` - set the ignored characters (default: `"\\t\\n "`)\n* `add_ignore()` - include whole patterns that are ignored (like comments)\n* `set_literal()` - Set the definition for what `Literal()` means\n* `set_keyword_chars()` - For default `Keyword()` (important for defining word boundary)\n\n\n### Navigating ParseResults\n\nThe results of parsing are in `ParseResults` and are in the form of an n-ary tree; with the children found in `ParseResults.tokens`.  Each `ParseResult.type` points to the `ParserElement` that made it.  In general, if you want to get fancy with post processing (or in a `parse_action`), you will be required to navigate the raw `tokens` to generate a final result\n\nThere are some convenience methods;  \n* `__iter__()` - allows you to iterate through parse results in **depth first search**. Empty results are skipped, and `Group`ed results are treated as atoms (which can be further iterated if required) \n* `name` is a convenient property for `ParseResults.type.token_name`\n* `__getitem__()` - allows you to jump into the parse tree to the given `name`. This is blocked by any names found inside `Group`ed results (because groups are considered atoms).      \n\n### Parse Actions\n\nParse actions are methods that are run after a ParserElement found a match. \n\n* Parameters must be accepted in `(tokens, index, string)` order (the opposite of pyparsing)\n* Parse actions are wrapped to ensure the output is a legitimate ParseResult\n  * If your parse action returns `None` then the result is the original `tokens`\n  * If your parse action returns an object, or list, or tuple, then it will be packaged in a `ParseResult` with same type as `tokens`.\n  * If your parse action returns a `ParseResult` then it is accepted ***even if is belongs to some other pattern***\n  \n#### Simple example:\n\n```\ninteger = Word("0123456789").add_parse_action(lambda t, i, s: int(t[0]))\nresult = integer.parse_string("42")\nassert (result[0] == 42)\n```\n\nFor slightly shorter specification, you may use the `/` operator and only parameters you need:\n\n```\ninteger = Word("0123456789") / (lambda t: int(t[0]))\nresult = integer.parse_string("42")\nassert (result[0] == 42)\n```\n\n### Debugging\n\nThe PEG-style of mo-parsing (from pyparsing) makes a very expressible and readable specification, but debugging a parser is still hard.  To look deeper into what the parser is doing use the `Debugger`:\n\n```\nwith Debugger():\n    expr.parse_string("my new language")\n```\n\nThe debugger will print out details of what\'s happening\n\n* Each attempt, and if it matched or failed\n* A small number of bytes to show you the current position\n* location, line and column for more info about the current position\n* whitespace indicating stack depth\n* print out of the ParserElement performing the attempt\n\nThis should help to isolate the exact position your grammar is failing. \n\n### Regular Expressions\n\n`mo-parsing` can parse and generate regular expressions. `ParserElement` has a `__regex__()` function that returns the regular expression for the given grammar; which works up to a limit, and is used internally to accelerate parsing.  The `Regex` class parses regular expressions into a grammar; it is used to optimize parsing, and you may find it useful to decompose regular expressions that look like line noise.\n\n\n\n\n\n\n\n\n\n\n## Differences from PyParsing\n\nThis fork was originally created to support faster parsing for [mo-sql-parsing](https://github.com/klahnakoski/moz-sql-parser).  Since then it has deviated sufficiently to be it\'s own collection of parser specification functions.  Here are the differences:\n\n* Added `Whitespace`, which controls parsing context and whitespace.  It replaces the whitespace modifying methods of pyparsing\n* the wildcard ("`*`") could be used in pyparsing to indicate multi-values are expected; this is not allowed in `mo-parsing`: all values are multi-values\n* ParserElements are static: For example, `expr.add_parse_action(action)` creates a new ParserElement, so must be assigned to variable or it is lost. **This is the biggest source of bugs when converting from pyparsing**\n* removed all backward-compatibility settings\n* no support for binary serialization (no pickle)\n\nFaster Parsing\n\n* faster infix operator parsing (main reason for this fork)\n* ParseResults point to ParserElement for reduced size\n* regex used to reduce the number of failed parse attempts  \n* packrat parser is not need\n* less stack used \n\n\n\n## Contributing\n\nIf you plan to extend or enhance this code, please [see the README in the tests directory](https://github.com/klahnakoski/mo-parsing/blob/dev/tests/README.md)',
+    long_description='# More Parsing!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-parsing.svg)](https://pypi.org/project/mo-parsing/)\n [![Build Status](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-parsing/badge.svg?branch=master)](https://coveralls.io/github/klahnakoski/mo-parsing?branch=master)\n\nA fork of [pyparsing](https://github.com/pyparsing/pyparsing) for faster parsing\n\n\n## Installation\n\nThis is a pypi package\n\n    pip install mo-parsing\n    \n## Usage\n\nThis module allows you to define a PEG parser using predefined patterns and Python operators.  Here is an example \n\n```\n>>> from mo_parsing import Word\n>>> from mo_parsing.utils import alphas\n>>>\n>>> greet = Word(alphas)("greeting") + "," + Word(alphas)("person") + "!"\n>>> result = greet.parse_string("Hello, World!")\n```\n\nThe `result` can be accessed as a nested list\n\n```\n>>> list(result)\n[\'Hello\', \',\', \'World\', \'!\']\n```\n\nThe `result` can also be accessed as a dictionary\n\n```\n>>> dict(result)\n{\'greeting\': \'Hello\', \'person\': \'World\'}\n```\n\nRead the [pyparsing documentation](https://github.com/pyparsing/pyparsing/#readme) for more\n\n### The `Whitespace` Context\n\nThe `mo_parsing.whitespaces.CURRENT` is used during parser creation: It is effectively defines what "whitespace" to skip during parsing, with additional features to simplify the language definition.  You declare "standard" `Whitespace` like so:\n\n    with Whitespace() as whitespace:\n        # PUT YOUR LANGUAGE DEFINITION HERE (space, tab and CR are "whitespace")\n\nIf you are declaring a large language, and you want to minimize indentation, and you are careful, you may also use this pattern:\n\n    whitespace = Whitespace().use()\n    # PUT YOUR LANGUAGE DEFINITION HERE\n    whitespace.release()\n\nThe whitespace can be used to set global parsing parameters, like\n\n* `set_whitespace()` - set the ignored characters (default: `"\\t\\n "`)\n* `add_ignore()` - include whole patterns that are ignored (like comments)\n* `set_literal()` - Set the definition for what `Literal()` means\n* `set_keyword_chars()` - For default `Keyword()` (important for defining word boundary)\n\n\n### Navigating ParseResults\n\nThe results of parsing are in `ParseResults` and are in the form of an n-ary tree; with the children found in `ParseResults.tokens`.  Each `ParseResult.type` points to the `ParserElement` that made it.  In general, if you want to get fancy with post processing (or in a `parse_action`), you will be required to navigate the raw `tokens` to generate a final result\n\nThere are some convenience methods;  \n* `__iter__()` - allows you to iterate through parse results in **depth first search**. Empty results are skipped, and `Group`ed results are treated as atoms (which can be further iterated if required) \n* `name` is a convenient property for `ParseResults.type.token_name`\n* `__getitem__()` - allows you to jump into the parse tree to the given `name`. This is blocked by any names found inside `Group`ed results (because groups are considered atoms).      \n\n### Parse Actions\n\nParse actions are methods that run after a ParserElement found a match. \n\n* Parameters must be accepted in `(tokens, index, string)` order (the opposite of pyparsing)\n* Parse actions are wrapped to ensure the output is a legitimate ParseResult\n  * If your parse action returns `None` then the result is the original `tokens`\n  * If your parse action returns an object, or list, or tuple, then it will be packaged in a `ParseResult` with same type as `tokens`.\n  * If your parse action returns a `ParseResult` then it is accepted ***even if is belongs to some other pattern***\n  \n#### Simple example:\n\n```\ninteger = Word("0123456789").add_parse_action(lambda t, i, s: int(t[0]))\nresult = integer.parse_string("42")\nassert (result[0] == 42)\n```\n\nFor slightly shorter specification, you may use the `/` operator and only parameters you need:\n\n```\ninteger = Word("0123456789") / (lambda t: int(t[0]))\nresult = integer.parse_string("42")\nassert (result[0] == 42)\n```\n\n### Debugging\n\nThe PEG-style of mo-parsing (from pyparsing) makes a very expressible and readable specification, but debugging a parser is still hard.  To look deeper into what the parser is doing use the `Debugger`:\n\n```\nwith Debugger():\n    expr.parse_string("my new language")\n```\n\nThe debugger will print out details of what\'s happening\n\n* Each attempt, and if it matched or failed\n* A small number of bytes to show you the current position\n* location, line and column for more info about the current position\n* whitespace indicating stack depth\n* print out of the ParserElement performing the attempt\n\nThis should help to isolate the exact position your grammar is failing. \n\n### Regular Expressions\n\n`mo-parsing` can parse and generate regular expressions. `ParserElement` has a `__regex__()` function that returns the regular expression for the given grammar; which works up to a limit, and is used internally to accelerate parsing.  The `Regex` class parses regular expressions into a grammar; it is used to optimize parsing, and you may find it useful to decompose regular expressions that look like line noise.\n\n\n## Differences from PyParsing\n\nThis fork was originally created to support faster parsing for [mo-sql-parsing](https://github.com/klahnakoski/moz-sql-parser).  Since then it has deviated sufficiently to be it\'s own collection of parser specification functions.  Here are the differences:\n\n* Added `Whitespace`, which controls parsing context and whitespace.  It replaces the whitespace modifying methods of pyparsing\n* the wildcard ("`*`") could be used in pyparsing to indicate multi-values are expected; this is not allowed in `mo-parsing`: all values are multi-values\n* ParserElements are static: For example, `expr.add_parse_action(action)` creates a new ParserElement, so must be assigned to variable or it is lost. **This is the biggest source of bugs when converting from pyparsing**\n* removed all backward-compatibility settings\n* no support for binary serialization (no pickle)\n\nFaster Parsing\n\n* faster infix operator parsing (main reason for this fork)\n* ParseResults point to ParserElement for reduced size\n* regex used to reduce the number of failed parse attempts  \n* packrat parser is not need\n* less stack used \n\n\n\n## Contributing\n\nIf you plan to extend or enhance this code, please [see the README in the tests directory](https://github.com/klahnakoski/mo-parsing/blob/dev/tests/README.md)',
     long_description_content_type='text/markdown',
     name='mo-parsing',
     packages=["mo_parsing"],
     url='https://github.com/klahnakoski/mo-parsing',
-    version='8.6.21337'
+    version='8.639.24140'
 )
```

