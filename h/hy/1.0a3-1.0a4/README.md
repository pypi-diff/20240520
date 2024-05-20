# Comparing `tmp/hy-1.0a3.tar.gz` & `tmp/hy-1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hy-1.0a3.tar", last modified: Fri Jul  9 16:59:19 2021, max compression
+gzip compressed data, was "hy-1.0a4.tar", last modified: Sun Jan  9 19:27:11 2022, max compression
```

## Comparing `hy-1.0a3.tar` & `hy-1.0a4.tar`

### file list

```diff
@@ -1,56 +1,45 @@
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2021-07-09 16:59:19.658144 hy-1.0a3/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4323 2021-03-11 17:24:40.000000 hy-1.0a3/AUTHORS
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1267 2021-03-11 17:24:40.000000 hy-1.0a3/LICENSE
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       94 2021-02-20 13:52:05.000000 hy-1.0a3/MANIFEST.in
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    45681 2021-07-09 16:52:43.000000 hy-1.0a3/NEWS.rst
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1147 2021-07-09 16:59:19.658144 hy-1.0a3/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     2044 2021-07-07 18:10:25.000000 hy-1.0a3/README.md
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4042 2021-02-20 13:52:05.000000 hy-1.0a3/fastentrypoints.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      785 2021-02-20 13:52:05.000000 hy-1.0a3/get_version.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2021-07-09 16:59:19.654144 hy-1.0a3/hy/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1443 2021-07-07 18:10:25.000000 hy-1.0a3/hy/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      162 2021-07-07 18:10:25.000000 hy-1.0a3/hy/__main__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      567 2021-07-07 18:10:25.000000 hy-1.0a3/hy/_compat.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    27524 2021-07-07 18:10:25.000000 hy-1.0a3/hy/cmdline.py
--rwxrwxr-x   0 hippo     (1000) hippo     (1000)    29202 2021-07-07 18:10:25.000000 hy-1.0a3/hy/compiler.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     3029 2021-07-07 18:10:25.000000 hy-1.0a3/hy/completer.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2021-07-09 16:59:19.654144 hy-1.0a3/hy/contrib/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        0 2021-02-20 13:52:05.000000 hy-1.0a3/hy/contrib/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    14496 2021-07-07 19:36:30.000000 hy-1.0a3/hy/contrib/destructure.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     3549 2021-07-07 19:36:30.000000 hy-1.0a3/hy/contrib/loop.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    12996 2021-07-07 19:36:30.000000 hy-1.0a3/hy/contrib/pprint.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1763 2021-07-07 19:36:30.000000 hy-1.0a3/hy/contrib/profile.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4397 2021-07-07 19:36:30.000000 hy-1.0a3/hy/contrib/sequences.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     6675 2021-07-07 18:10:25.000000 hy-1.0a3/hy/contrib/slicing.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    21241 2021-07-07 19:36:30.000000 hy-1.0a3/hy/contrib/walk.hy
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2021-07-09 16:59:19.658144 hy-1.0a3/hy/core/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        0 2021-07-07 18:10:25.000000 hy-1.0a3/hy/core/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     7644 2021-07-07 19:36:30.000000 hy-1.0a3/hy/core/hy_repr.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     9473 2021-07-07 19:36:30.000000 hy-1.0a3/hy/core/language.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    19446 2021-07-09 16:50:47.000000 hy-1.0a3/hy/core/macros.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    54044 2021-07-07 19:36:30.000000 hy-1.0a3/hy/core/result_macros.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     7241 2021-07-07 19:36:30.000000 hy-1.0a3/hy/core/shadow.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    10833 2021-07-07 18:10:25.000000 hy-1.0a3/hy/errors.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2021-07-09 16:59:19.658144 hy-1.0a3/hy/extra/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        0 2021-02-20 13:52:05.000000 hy-1.0a3/hy/extra/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     8049 2021-07-07 19:36:30.000000 hy-1.0a3/hy/extra/anaphoric.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1030 2021-07-07 18:10:25.000000 hy-1.0a3/hy/extra/reserved.hy
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     6289 2021-07-07 18:10:25.000000 hy-1.0a3/hy/importer.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2021-07-09 16:59:19.658144 hy-1.0a3/hy/lex/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     8661 2021-07-07 18:10:25.000000 hy-1.0a3/hy/lex/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1158 2021-03-11 17:24:40.000000 hy-1.0a3/hy/lex/exceptions.py
--rwxrwxr-x   0 hippo     (1000) hippo     (1000)     1860 2021-03-11 17:24:40.000000 hy-1.0a3/hy/lex/lexer.py
--rwxrwxr-x   0 hippo     (1000) hippo     (1000)    11465 2021-07-07 18:10:25.000000 hy-1.0a3/hy/lex/parser.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    12999 2021-07-07 18:10:25.000000 hy-1.0a3/hy/macros.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     3420 2021-07-07 18:10:25.000000 hy-1.0a3/hy/model_patterns.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    15142 2021-07-07 18:10:25.000000 hy-1.0a3/hy/models.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       22 2021-07-09 16:59:19.000000 hy-1.0a3/hy/version.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2021-07-09 16:59:19.654144 hy-1.0a3/hy.egg-info/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1147 2021-07-09 16:59:19.000000 hy-1.0a3/hy.egg-info/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      868 2021-07-09 16:59:19.000000 hy-1.0a3/hy.egg-info/SOURCES.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2021-07-09 16:59:19.000000 hy-1.0a3/hy.egg-info/dependency_links.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      182 2021-07-09 16:59:19.000000 hy-1.0a3/hy.egg-info/entry_points.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      116 2021-07-09 16:59:19.000000 hy-1.0a3/hy.egg-info/requires.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        3 2021-07-09 16:59:19.000000 hy-1.0a3/hy.egg-info/top_level.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      402 2021-07-09 16:59:19.662144 hy-1.0a3/setup.cfg
--rwxrwxr-x   0 hippo     (1000) hippo     (1000)     4035 2021-07-09 16:53:51.000000 hy-1.0a3/setup.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2022-01-09 19:27:11.193733 hy-1.0a4/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4418 2021-11-27 17:25:30.000000 hy-1.0a4/AUTHORS
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1267 2022-01-09 19:26:25.000000 hy-1.0a4/LICENSE
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       94 2021-11-27 17:25:30.000000 hy-1.0a4/MANIFEST.in
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    48864 2022-01-09 19:26:25.000000 hy-1.0a4/NEWS.rst
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1232 2022-01-09 19:27:11.193733 hy-1.0a4/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2044 2021-11-27 17:25:30.000000 hy-1.0a4/README.md
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4042 2021-11-27 17:25:30.000000 hy-1.0a4/fastentrypoints.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      785 2021-11-27 17:25:30.000000 hy-1.0a4/get_version.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2022-01-09 19:27:11.189733 hy-1.0a4/hy/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1357 2021-12-18 18:47:47.000000 hy-1.0a4/hy/__init__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      162 2021-11-27 17:25:30.000000 hy-1.0a4/hy/__main__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      944 2021-12-18 18:47:47.000000 hy-1.0a4/hy/_compat.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    26519 2022-01-01 14:02:21.000000 hy-1.0a4/hy/cmdline.py
+-rwxrwxr-x   0 hippo     (1000) hippo     (1000)    29538 2022-01-01 14:02:27.000000 hy-1.0a4/hy/compiler.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2949 2021-11-27 17:25:30.000000 hy-1.0a4/hy/completer.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2022-01-09 19:27:11.193733 hy-1.0a4/hy/core/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        0 2021-11-27 17:25:30.000000 hy-1.0a4/hy/core/__init__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     9400 2021-11-27 17:25:30.000000 hy-1.0a4/hy/core/hy_repr.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     3114 2021-11-27 17:25:30.000000 hy-1.0a4/hy/core/macros.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    57887 2022-01-01 14:02:27.000000 hy-1.0a4/hy/core/result_macros.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2897 2021-11-27 17:25:30.000000 hy-1.0a4/hy/core/util.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    10954 2021-11-27 17:25:30.000000 hy-1.0a4/hy/errors.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     5599 2021-11-27 17:25:30.000000 hy-1.0a4/hy/importer.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2022-01-09 19:27:11.193733 hy-1.0a4/hy/lex/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     8573 2021-11-27 17:25:30.000000 hy-1.0a4/hy/lex/__init__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1025 2021-11-27 17:25:30.000000 hy-1.0a4/hy/lex/exceptions.py
+-rwxrwxr-x   0 hippo     (1000) hippo     (1000)     1726 2021-11-27 17:25:30.000000 hy-1.0a4/hy/lex/lexer.py
+-rwxrwxr-x   0 hippo     (1000) hippo     (1000)    11264 2021-11-27 17:25:30.000000 hy-1.0a4/hy/lex/parser.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    12467 2021-12-18 18:47:47.000000 hy-1.0a4/hy/macros.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     3433 2021-12-18 18:47:47.000000 hy-1.0a4/hy/model_patterns.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    16531 2021-11-27 17:25:30.000000 hy-1.0a4/hy/models.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     8020 2021-11-27 17:25:30.000000 hy-1.0a4/hy/pyops.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      830 2021-11-27 17:25:30.000000 hy-1.0a4/hy/reserved.hy
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    11492 2022-01-01 14:02:27.000000 hy-1.0a4/hy/scoping.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       22 2022-01-09 19:27:11.000000 hy-1.0a4/hy/version.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2022-01-09 19:27:11.193733 hy-1.0a4/hy.egg-info/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1232 2022-01-09 19:27:11.000000 hy-1.0a4/hy.egg-info/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      647 2022-01-09 19:27:11.000000 hy-1.0a4/hy.egg-info/SOURCES.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2022-01-09 19:27:11.000000 hy-1.0a4/hy.egg-info/dependency_links.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      182 2022-01-09 19:27:11.000000 hy-1.0a4/hy.egg-info/entry_points.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       82 2022-01-09 19:27:11.000000 hy-1.0a4/hy.egg-info/requires.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        3 2022-01-09 19:27:11.000000 hy-1.0a4/hy.egg-info/top_level.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      214 2022-01-09 19:27:11.193733 hy-1.0a4/setup.cfg
+-rwxrwxr-x   0 hippo     (1000) hippo     (1000)     2391 2022-01-09 19:04:01.000000 hy-1.0a4/setup.py
```

### Comparing `hy-1.0a3/AUTHORS` & `hy-1.0a4/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -102,7 +102,9 @@
 * Xi Jin <xij@usc.edu>
 * Alexey Yurchenko <homonoidian@yandex.ru>
 * Allie Jo Casey <allie.jo.casey@gmail.com>
 * Joshua Munn <public@elysee-munn.family>
 * Peter Andreev <appa@gmx.co.uk>
 * Sunjay Cauligi <scauligi@eng.ucsd.edu>
 * David Tscheppen <david.tscheppen@gmail.com>
+* Dmitry Ivanov <dmitry.ivanov@divanov.eu>
+* Andrey Vlasovskikh <andrey.vlasovskikh@gmail.com>
```

### Comparing `hy-1.0a3/LICENSE` & `hy-1.0a4/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2021 the authors.
+Copyright 2022 the authors.
 Portions of setup.py, copyright 2016 Jason R Coombs <jaraco@jaraco.com>.
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
```

### Comparing `hy-1.0a3/NEWS.rst` & `hy-1.0a4/NEWS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,70 @@
 .. default-role:: code
 
+1.0a4 (released 2022-01-09)
+==============================
+
+Removals
+------------------------------
+* Python 3.6 is no longer supported.
+
+Other Breaking Changes
+------------------------------
+* `import` and `require` no longer need outer brackets.
+  `(import [foo [bar]])` is now `(import foo [bar])`
+  and `(import [foo :as baz])` is now `(import foo :as baz)`.
+  To import all names from a module, use `(import foo *)`.
+* Lots of objects (listed below) have been spun off to a new package
+  called `Hyrule`_, from which you can `import` or `require` them.
+  Thus Hy now brings only the `hy` module and a limited set of core
+  macros into scope automatically.
+
+  * Functions: `butlast`, `coll?`, `constantly`, `dec`, `destructure`, `distinct`, `drop-last`, `end-sequence`, `flatten`, `inc`, `macroexpand-all`, `parse-args`, `pformat`, `postwalk`, `pp`, `pprint`, `prewalk`, `readable?`, `recursive?`, `rest`, `saferepr`, `walk`
+  * Classes: `PrettyPrinter`, `Sequence`
+  * Macros: `#%`, `#:`, `->`, `->>`, `ap-dotimes`, `ap-each`, `ap-each-while`, `ap-filter`, `ap-first`, `ap-if`, `ap-last`, `ap-map`, `ap-map-when`, `ap-reduce`, `ap-reject`, `as->`, `assoc`, `cfor`, `comment`, `defmacro!`, `defmacro/g!`, `defmain`, `defn+`, `defn/a+`, `defseq`, `dict=:`, `do-n`, `doto`, `fn+`, `fn/a+`, `ifp`, `let+`, `lif`, `list-n`, `loop`, `ncut`, `of`, `profile/calls`, `profile/cpu`, `seq`, `setv+`, `smacrolet`, `unless`, `with-gensyms`
+
+* Functions that provide first-class Python operators, such as `+`
+  in constructs like `(reduce + xs)`, are no longer brought
+  into scope automatically. Say `(import hy.pyops *)` to get them.
+* Hy scoping rules more closely follow Python scoping in certain edge
+  cases.
+* `let` is now a core macro with somewhat different semantics. In
+  particular, definition-like core macros (`defn`, `defclass`,
+  `import`) now introduce new names that shadow corresponding
+  `let`-bound names and persist outside the body of the `let`.
+* The constructors of `String` and `FString` now check that the input
+  would be syntactically legal as a literal.
+* `hy.extra.reserved` has been renamed to `hy.reserved`.
+
+Bug Fixes
+------------------------------
+* In comprehension forms other than `for`, assignments (other than
+  `:setv` and loop clauses) are now always visible in the surrounding
+  scope.
+* `match` now only evaluates the subject once.
+* `let` will no longer re-evaluate the default arguments of a
+  function it's used in.
+* `hy.repr` now properly formats bracket strings.
+* The `repr` and `str` of string models now include `brackets` if
+  necessary.
+* When standard output can't accommodate Unicode, `hy2py` now crashes
+  instead of emitting incorrect Python code.
+* Fixed a bug with self-requiring files on Windows.
+* Improved error messages for illegal uses of `finally` and `else`.
+
+New Features
+------------------------------
+* `hy.repr` now supports several more standard types.
+* The attribute access macro `.` now allows method calls. For example,
+  `(. x (f a))` is equivalent to `(x.f a)`.
+* `hy.as-model` checks for self-references in its argument.
+* New function `hy.model_patterns.keepsym`.
+
+.. _Hyrule: https://github.com/hylang/hyrule
+
 1.0a3 (released 2021-07-09)
 ==============================
 
 Bug Fixes
 ------------------------------
 * Fixed a dependency-management bug that prevented installation of Hy
   from a wheel on Pythons < 3.9.
```

### Comparing `hy-1.0a3/PKG-INFO` & `hy-1.0a4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: hy
-Version: 1.0a3
+Version: 1.0a4
 Summary: Lisp and Python love each other.
 Home-page: http://hylang.org/
 Author: Paul Tagliamonte
 Author-email: tag@pault.ag
 License: Expat
+Project-URL: Documentation, https://docs.hylang.org/
+Project-URL: Source, https://github.com/hylang/hy
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Lisp
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >= 3.7, < 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
 Hy is a Python <--> Lisp layer. It helps
 make things work nicer, and lets Python and the Hy lisp variant play
 nice together.
```

### Comparing `hy-1.0a3/README.md` & `hy-1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `hy-1.0a3/fastentrypoints.py` & `hy-1.0a4/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `hy-1.0a3/get_version.py` & `hy-1.0a4/get_version.py`

 * *Files identical despite different names*

### Comparing `hy-1.0a3/hy/cmdline.py` & `hy-1.0a4/hy/cmdline.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-
-from __future__ import print_function
-
 import colorama
 colorama.init()
 
 import argparse
 import code
 import ast
 import sys
 import os
-import io
 import importlib
 import py_compile
 import traceback
 import runpy
 import types
 import time
 import linecache
@@ -40,15 +33,15 @@
 
 
 sys.last_type = None
 sys.last_value = None
 sys.last_traceback = None
 
 
-class HyQuitter(object):
+class HyQuitter:
     def __init__(self, name):
         self.name = name
 
     def __repr__(self):
         return "Use (%s) or Ctrl-D (i.e. EOF) to exit" % (self.name)
 
     __str__ = __repr__
@@ -56,15 +49,15 @@
     def __call__(self, code=None):
         try:
             sys.stdin.close()
         except:
             pass
         raise SystemExit(code)
 
-class HyHelper(object):
+class HyHelper:
     def __repr__(self):
         return ("Use (help) for interactive help, or (help object) for help "
                 "about object.")
 
     def __call__(self, *args, **kwds):
         import pydoc
         return pydoc.help(*args, **kwds)
@@ -111,27 +104,27 @@
 
     return compiler(source, filename, symbol)
 
 
 codeop._maybe_compile = _hy_maybe_compile
 
 
-class HyCompile(codeop.Compile, object):
+class HyCompile(codeop.Compile):
     """This compiler uses `linecache` like
     `IPython.core.compilerop.CachingCompiler`.
     """
 
     def __init__(self, module, locals, ast_callback=None,
                  hy_compiler=None, cmdline_cache={}):
         self.module = module
         self.locals = locals
         self.ast_callback = ast_callback
         self.hy_compiler = hy_compiler
 
-        super(HyCompile, self).__init__()
+        super().__init__()
 
         self.flags |= hy_ast_compile_flags
 
         self.cmdline_cache = cmdline_cache
 
     def _cache(self, source, name):
         entry = (len(source),
@@ -182,67 +175,67 @@
                                             compiler=self.hy_compiler,
                                             filename=filename, source=source,
                                             import_stdlib=False)
 
             if self.ast_callback:
                 self.ast_callback(exec_ast, eval_ast)
 
-            exec_code = super(HyCompile, self).__call__(exec_ast, name, symbol)
-            eval_code = super(HyCompile, self).__call__(eval_ast, name, 'eval')
+            exec_code = super().__call__(exec_ast, name, symbol)
+            eval_code = super().__call__(eval_ast, name, 'eval')
 
         except HyLanguageError:
             # Hy will raise exceptions during compile-time that Python would
             # raise during run-time (e.g. import errors for `require`).  In
             # order to work gracefully with the Python world, we convert such
             # Hy errors to code that purposefully reraises those exceptions in
             # the places where Python code expects them.
             sys.last_type, sys.last_value, sys.last_traceback = sys.exc_info()
             self._update_exc_info()
-            exec_code = super(HyCompile, self).__call__(
+            exec_code = super().__call__(
                 'raise _hy_last_value.with_traceback(_hy_last_traceback)',
                 name, symbol)
-            eval_code = super(HyCompile, self).__call__('None', name, 'eval')
+            eval_code = super().__call__('None', name, 'eval')
 
         except SyntaxError:
             # Capture and save the error before we get to the superclass handler
             sys.last_type, sys.last_value, sys.last_traceback = sys.exc_info()
             # Per the python REPL, SyntaxErrors should not display a traceback
             sys.last_traceback = None
             self._update_exc_info()
             raise
 
         return exec_code, eval_code
 
 
-class HyCommandCompiler(codeop.CommandCompiler, object):
+class HyCommandCompiler(codeop.CommandCompiler):
     def __init__(self, *args, **kwargs):
         self.compiler = HyCompile(*args, **kwargs)
 
     def __call__(self, *args, **kwargs):
         try:
-            return super(HyCommandCompiler, self).__call__(*args, **kwargs)
+            return super().__call__(*args, **kwargs)
         except PrematureEndOfInput:
             # We have to do this here, because `codeop._maybe_compile` won't
             # take `None` for a return value (at least not in Python 2.7) and
             # this exception type is also a `SyntaxError`, so it will be caught
             # by `code.InteractiveConsole` base methods before it reaches our
             # `runsource`.
             return None
 
 
-class HyREPL(code.InteractiveConsole, object):
+class HyREPL(code.InteractiveConsole):
     def __init__(self, spy=False, output_fn=None, locals=None,
                  filename="<stdin>"):
 
         # Create a proper module for this REPL so that we can obtain it easily
         # (e.g. using `importlib.import_module`).
         # We let `InteractiveConsole` initialize `self.locals` when it's
         # `None`.
-        super(HyREPL, self).__init__(locals=locals,
-                                     filename=filename)
+        super().__init__(locals=locals,
+                         filename=filename)
 
         module_name = self.locals.get('__name__', '__console__')
         # Make sure our newly created module is properly introduced to
         # `sys.modules`, and consistently use its namespace as `self.locals`
         # from here on.
         self.module = sys.modules.setdefault(module_name,
                                              types.ModuleType(module_name))
@@ -330,32 +323,28 @@
         if exc_info_override:
             # Use a traceback that doesn't have the REPL frames.
             sys.last_type = self.locals.get('_hy_last_type', sys.last_type)
             sys.last_value = self.locals.get('_hy_last_value', sys.last_value)
             sys.last_traceback = self.locals.get('_hy_last_traceback',
                                                  sys.last_traceback)
 
-        # Sadly, this method in Python 2.7 ignores an overridden `sys.excepthook`.
-        if sys.excepthook is sys.__excepthook__:
-            error_fn(*args, **kwargs)
-        else:
-            sys.excepthook(sys.last_type, sys.last_value, sys.last_traceback)
+        sys.excepthook(sys.last_type, sys.last_value, sys.last_traceback)
 
         self.locals[mangle("*e")] = sys.last_value
 
     def showsyntaxerror(self, filename=None):
         if filename is None:
             filename = self.filename
 
-        self._error_wrap(super(HyREPL, self).showsyntaxerror,
+        self._error_wrap(super().showsyntaxerror,
                          exc_info_override=True,
                          filename=filename)
 
     def showtraceback(self):
-        self._error_wrap(super(HyREPL, self).showtraceback)
+        self._error_wrap(super().showtraceback)
 
     def runcode(self, code):
         try:
             eval(code[0], self.locals)
             self.last_value = eval(code[1], self.locals)
             # Don't print `None` values.
             self.print_last_value = self.last_value is not None
@@ -364,15 +353,15 @@
         except Exception as e:
             # Set this to avoid a print-out of the last value on errors.
             self.print_last_value = False
             self.showtraceback()
 
     def runsource(self, source, filename='<stdin>', symbol='exec'):
         try:
-            res = super(HyREPL, self).runsource(source, filename, symbol)
+            res = super().runsource(source, filename, symbol)
         except (HyMacroExpansionError, HyRequireError):
             # We need to handle these exceptions ourselves, because the base
             # method only handles `OverflowError`, `SyntaxError` and
             # `ValueError`.
             self.showsyntaxerror(filename)
             return False
         except (HyLanguageError):
@@ -433,14 +422,15 @@
 
 
 ;;; string things
 (.join ", " ["what" "the" "heck"])
 
 
 ;;; this one plays with command line bits
+(require hyrule [->])
 (import [sh [cat grep]])
 (-> (cat "/usr/share/dict/words") (grep "-E" "bro$"))
 
 
 ;;; filtering a list w/ a lambda
 (filter (fn [x] (= (% x 2) 0)) (range 0 10))
 
@@ -483,31 +473,30 @@
     if not hr:
         hr = HyREPL(**kwargs)
 
     namespace = hr.locals
     with filtered_hy_exceptions(), \
          extend_linecache(hr.cmdline_cache), \
          completion(Completer(namespace)):
-        hr.interact("{appname} {version} using "
+        hr.interact("Hy {version} using "
                     "{py}({build}) {pyversion} on {os}".format(
-                        appname=hy.__appname__,
                         version=hy.__version__,
                         py=platform.python_implementation(),
                         build=platform.python_build()[0],
                         pyversion=platform.python_version(),
                         os=platform.system()
                     ))
 
     return 0
 
 
 def run_icommand(source, **kwargs):
     if os.path.exists(source):
         set_path(source)
-        with io.open(source, "r", encoding='utf-8') as f:
+        with open(source, "r", encoding='utf-8') as f:
             source = f.read()
         filename = source
     else:
         filename = '<string>'
 
     hr = HyREPL(**kwargs)
     with filtered_hy_exceptions():
@@ -670,15 +659,15 @@
 
             try:
                 sys.argv = argv
                 with filtered_hy_exceptions():
                     runhy.run_path(filename, run_name='__main__')
                 return 0
             except FileNotFoundError as e:
-                print("hy: Can't open file '{0}': [Errno {1}] {2}".format(
+                print("hy: Can't open file '{}': [Errno {}] {}".format(
                       e.filename, e.errno, e.strerror), file=sys.stderr)
                 sys.exit(e.errno)
             except HyLanguageError:
                 hy_exc_handler(*sys.exc_info())
                 sys.exit(1)
 
     return run_repl(
@@ -758,51 +747,38 @@
     if options.FILE is None or options.FILE == '-':
         sys.path.insert(0, "")
         filename = '<stdin>'
         source = sys.stdin.read()
     else:
         filename = options.FILE
         set_path(filename)
-        with io.open(options.FILE, 'r', encoding='utf-8') as source_file:
+        with open(options.FILE, 'r', encoding='utf-8') as source_file:
             source = source_file.read()
 
     with filtered_hy_exceptions():
         hst = hy_parse(source, filename=filename)
 
     if options.with_source:
-        _print_for_windows(hst)
+        print(hst)
         print()
         print()
 
     with filtered_hy_exceptions():
         _ast = hy_compile(hst, '__main__', filename=filename, source=source)
 
     if options.with_ast:
-        _print_for_windows(ast.dump(_ast))
+        print(ast.dump(_ast))
         print()
         print()
 
     if not options.without_python:
-        _print_for_windows(ast.unparse(_ast))
+        print(ast.unparse(_ast))
 
     parser.exit(0)
 
 
-# need special printing on Windows in case the
-# codepage doesn't support utf-8 characters
-def _print_for_windows(src):
-    import platform
-    if platform.system() == "Windows":
-        for line in src.split("\n"):
-            try:
-                print(line)
-            except:
-                print(line.encode('utf-8'))
-    else:
-        print(src)
-
 # remove PYTHON* environment variables,
 # such as "PYTHONPATH"
 def _remove_python_envs():
     for key in list(os.environ.keys()):
         if key.startswith("PYTHON"):
             os.environ.pop(key)
```

### Comparing `hy-1.0a3/hy/compiler.py` & `hy-1.0a4/hy/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,51 @@
-# -*- encoding: utf-8 -*-
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-
-import __future__
-import ast, copy, importlib, inspect, keyword, pkgutil
+import ast, copy, importlib, inspect, keyword
 import traceback, types
 
 from funcparserlib.parser import NoParseError, many
 
 from hy.models import (Object, Expression, Keyword, Integer, Complex,
     String, FComponent, FString, Bytes, Symbol, Float, List, Set,
     Dict, as_model, is_unpack)
 from hy.model_patterns import (FORM, KEYWORD, unpack)
 from hy.errors import (HyCompileError, HyLanguageError, HySyntaxError)
 from hy.lex import mangle
 from hy.macros import macroexpand
+from hy.scoping import ScopeGlobal
 
 
-hy_ast_compile_flags = (__future__.CO_FUTURE_DIVISION |
-                        __future__.CO_FUTURE_PRINT_FUNCTION)
+hy_ast_compile_flags = 0
 
 
 def ast_compile(a, filename, mode):
     """Compile AST.
 
-    Parameters
-    ----------
-    a : instance of `ast.AST`
-
-    filename : str
-        Filename used for run-time error messages
-
-    mode: str
-        `compile` mode parameter
-
-    Returns
-    -------
-    out : instance of `types.CodeType`
+    Args:
+        a (ast.AST): instance of `ast.AST`
+        filename (str): Filename used for run-time error messages
+        mode (str): `compile` mode parameter
+
+    Returns:
+        types.CodeType: instance of `types.CodeType`
     """
     return compile(a, filename, mode, hy_ast_compile_flags)
 
 
 def calling_module(n=1):
     """Get the module calling, if available.
 
     As a fallback, this will import a module using the calling frame's
     globals value of `__name__`.
 
-    Parameters
-    ----------
-    n: int, optional
-        The number of levels up the stack from this function call.
-        The default is one level up.
-
-    Returns
-    -------
-    out: types.ModuleType
-        The module at stack level `n + 1` or `None`.
+    Args:
+        n (int): The number of levels up the stack from this function call.
+            The default is `1` (level up).
+
+    Returns:
+        types.ModuleType: The module at stack level `n + 1` or `None`.
     """
     frame_up = inspect.stack(0)[n + 1][0]
     module = inspect.getmodule(frame_up)
     if module is None:
         # This works for modules like `__main__`
         module_name = frame_up.f_globals.get('__name__', None)
         if module_name:
@@ -82,33 +66,54 @@
         return fn
     return _dec
 
 
 # Provide asty.Foo(x, ...) as shorthand for
 # ast.Foo(..., lineno=x.start_line, col_offset=x.start_column) or
 # ast.Foo(..., lineno=x.lineno, col_offset=x.col_offset)
-class Asty(object):
+# Also provides asty.parse(x, ...) which recursively
+# copies x's position data onto the parse result.
+class Asty:
+    POS_ATTRS = {
+        'lineno': 'start_line',
+        'col_offset': 'start_column',
+        'end_lineno': 'end_line',
+        'end_col_offset': 'end_column',
+    }
+
+    @staticmethod
+    def _get_pos(node):
+        return {
+            attr: getattr(node, hy_attr,
+                          getattr(node, attr, None))
+            for attr, hy_attr in Asty.POS_ATTRS.items()
+        }
+
+    @staticmethod
+    def _replace_pos(node, pos):
+        for attr, value in pos.items():
+            if hasattr(node, attr):
+                setattr(node, attr, value)
+        for child in ast.iter_child_nodes(node):
+            Asty._replace_pos(child, pos)
+
+    def parse(self, x, *args, **kwargs):
+        res = ast.parse(*args, **kwargs)
+        Asty._replace_pos(res, Asty._get_pos(x))
+        return res
+
     def __getattr__(self, name):
-        setattr(Asty, name, staticmethod(lambda x, **kwargs: getattr(ast, name)(
-            lineno=getattr(
-                x, 'start_line', getattr(x, 'lineno', None)),
-            col_offset=getattr(
-                x, 'start_column', getattr(x, 'col_offset', None)),
-            end_lineno=getattr(
-                x, 'end_line', getattr(x, 'end_lineno', None)
-            ),
-            end_col_offset=getattr(
-                x, 'end_column', getattr(x, 'end_col_offset', None)
-            ),
-            **kwargs)))
+        setattr(Asty, name, staticmethod(
+            lambda x, **kwargs: getattr(ast, name)(**Asty._get_pos(x), **kwargs)))
         return getattr(Asty, name)
+
 asty = Asty()
 
 
-class Result(object):
+class Result:
     """
     Smart representation of the result of a hy->AST compilation
 
     This object tries to reconcile the hy world, where everything can be used
     as an expression, with the Python world, where statements and expressions
     need to coexist.
 
@@ -208,24 +213,24 @@
 
         If there is no expression context, return an empty result.
         """
         if self.expr and not (isinstance(self.expr, ast.Name) and self.stmts):
             return Result() + asty.Expr(self.expr, value=self.expr)
         return Result()
 
-    def rename(self, new_name):
+    def rename(self, compiler, new_name):
         """Rename the Result's temporary variables to a `new_name`.
 
         We know how to handle ast.Names and ast.FunctionDefs.
         """
         new_name = mangle(new_name)
         for var in self.temp_variables:
             if isinstance(var, ast.Name):
                 var.id = new_name
-                var.arg = new_name
+                compiler.scope.assign(var)
             elif isinstance(var, (ast.FunctionDef, ast.AsyncFunctionDef)):
                 var.name = new_name
             else:
                 raise TypeError("Don't know how to rename a %s!" % (
                     var.__class__.__name__))
         self.temp_variables = []
 
@@ -238,21 +243,20 @@
         if isinstance(other, ast.expr):
             return self + Result(expr=other)
 
         if isinstance(other, ast.excepthandler):
             return self + Result(stmts=[other])
 
         if not isinstance(other, Result):
-            raise TypeError("Can't add %r with non-compiler result %r" % (
-                self, other))
+            raise TypeError(f"Can't add {self!r} with non-compiler result {other!r}")
 
         # Check for expression context clobbering
         if self.expr and not self.__used_expr:
             traceback.print_stack()
-            print("Bad boy clobbered expr %s with %s" % (
+            print("Bad boy clobbered expr {} with {}".format(
                 ast.dump(self.expr),
                 ast.dump(other.expr)))
 
         # Fairly obvious addition
         result = Result()
         result.stmts = self.stmts + other.stmts
         result.expr = other.expr
@@ -282,30 +286,26 @@
 
 
 def is_annotate_expression(model):
     return (isinstance(model, Expression) and model
             and model[0] == Symbol("annotate"))
 
 
-class HyASTCompiler(object):
+class HyASTCompiler:
     """A Hy-to-Python AST compiler"""
 
     def __init__(self, module, filename=None, source=None):
         """
-        Parameters
-        ----------
-        module: str or types.ModuleType
-            Module name or object in which the Hy tree is evaluated.
-        filename: str, optional
-            The name of the file for the source to be compiled.
-            This is optional information for informative error messages and
-            debugging.
-        source: str, optional
-            The source for the file, if any, being compiled.  This is optional
-            information for informative error messages and debugging.
+        Args:
+            module (Union[str, types.ModuleType]): Module name or object in which the Hy tree is evaluated.
+            filename (Optional[str]): The name of the file for the source to be compiled.
+                This is optional information for informative error messages and
+                debugging.
+            source (Optional[str]): The source for the file, if any, being compiled.  This is optional
+                information for informative error messages and debugging.
         """
         self.anon_var_count = 0
         self.temp_if = None
 
         if not inspect.ismodule(module):
             self.module = importlib.import_module(module)
         else:
@@ -320,17 +320,19 @@
           # Set in `macroexpand` to the current expression being
           # macro-expanded, so it can be accessed as `&compiler.this`.
 
         # Hy expects this to be present, so we prep the module for Hy
         # compilation.
         self.module.__dict__.setdefault('__macros__', {})
 
-    def get_anon_var(self):
+        self.scope = ScopeGlobal(self)
+
+    def get_anon_var(self, base="_hy_anon_var"):
         self.anon_var_count += 1
-        return "_hy_anon_var_%s" % self.anon_var_count
+        return f"{base}_{self.anon_var_count}"
 
     def compile_atom(self, atom):
         # Compilation methods may mutate the atom, so copy it first.
         atom = copy.copy(atom)
         return Result() + _model_compilers[type(atom)](self, atom)
 
     def compile(self, tree):
@@ -440,14 +442,16 @@
             typ = type(name)
             new_elts = []
             for x in name.elts:
                 new_elts.append(self._storeize(expr, x, func))
             new_name = typ(elts=new_elts)
         elif isinstance(name, ast.Name):
             new_name = ast.Name(id=name.id)
+            if func == ast.Store:
+                self.scope.assign(new_name)
         elif isinstance(name, ast.Subscript):
             new_name = ast.Subscript(value=name.value, slice=name.slice)
         elif isinstance(name, ast.Attribute):
             new_name = ast.Attribute(value=name.value, attr=name.attr)
         elif isinstance(name, ast.Starred):
             new_name = ast.Starred(
                 value=self._storeize(expr, name.value, func))
@@ -567,15 +571,16 @@
                 attr=mangle(local),
                 ctx=ast.Load())
 
         if mangle(symbol) in ("None", "False", "True"):
             return asty.Constant(symbol, value =
                 ast.literal_eval(mangle(symbol)))
 
-        return asty.Name(symbol, id=mangle(symbol), ctx=ast.Load())
+        return self.scope.access(asty.Name(
+            symbol, id=mangle(symbol), ctx=ast.Load()))
 
     @builds_model(Keyword)
     def compile_keyword(self, obj):
         ret = Result()
         ret += asty.Call(
             obj,
             func=asty.Attribute(obj,
@@ -645,16 +650,24 @@
 
     if not inspect.ismodule(module):
         raise TypeError('Invalid module type: {}'.format(type(module)))
 
     return module
 
 
-def hy_eval(hytree, locals=None, module=None, ast_callback=None,
-            compiler=None, filename=None, source=None, import_stdlib=True):
+def hy_eval(
+    hytree,
+    locals=None,
+    module=None,
+    ast_callback=None,
+    compiler=None,
+    filename=None,
+    source=None,
+    import_stdlib=True,
+):
     """Evaluates a quoted expression and returns the value.
 
     If you're evaluating hand-crafted AST trees, make sure the line numbers
     are set properly.  Try `fix_missing_locations` and related functions in the
     Python `ast` library.
 
     Examples:
@@ -666,52 +679,52 @@
       If you want to evaluate a string, use ``read-str`` to convert it to a
       form first::
 
          => (hy.eval (hy.read-str "(+ 1 1)"))
          2
 
     Args:
-      hytree (hy.models.Object):
+      hytree (Object):
           The Hy AST object to evaluate.
 
-      locals (dict, optional):
+      locals (Optional[dict]):
           Local environment in which to evaluate the Hy tree.  Defaults to the
           calling frame.
 
-      module (str or types.ModuleType, optional):
+      module (Optional[Union[str, types.ModuleType]]):
           Module, or name of the module, to which the Hy tree is assigned and
           the global values are taken.
           The module associated with `compiler` takes priority over this value.
           When neither `module` nor `compiler` is specified, the calling frame's
           module is used.
 
-      ast_callback (callable, optional):
+      ast_callback (Optional[Callable]):
           A callback that is passed the Hy compiled tree and resulting
           expression object, in that order, after compilation but before
           evaluation.
 
-      compiler (HyASTCompiler, optional):
+      compiler (Optional[HyASTCompiler]):
           An existing Hy compiler to use for compilation.  Also serves as
           the `module` value when given.
 
-      filename (str, optional):
+      filename (Optional[str]):
           The filename corresponding to the source for `tree`.  This will be
           overridden by the `filename` field of `tree`, if any; otherwise, it
           defaults to "<string>".  When `compiler` is given, its `filename` field
           value is always used.
 
-      source (str, optional):
+      source (Optional[str]):
           A string containing the source code for `tree`.  This will be
           overridden by the `source` field of `tree`, if any; otherwise,
           if `None`, an attempt will be made to obtain it from the module given by
           `module`.  When `compiler` is given, its `source` field value is always
           used.
 
     Returns:
-      Result of evaluating the Hy compiled tree.
+      Any: Result of evaluating the Hy compiled tree.
     """
 
     module = get_compiler_module(module, compiler, True)
 
     if locals is None:
         frame = inspect.stack()[1][0]
         locals = inspect.getargvalues(frame).locals
@@ -735,53 +748,46 @@
          module.__dict__, locals)
 
     # Then eval the expression context and return that
     return eval(ast_compile(expr, filename, "eval"),
                 module.__dict__, locals)
 
 
-def hy_compile(tree, module, root=ast.Module, get_expr=False,
-               compiler=None, filename=None, source=None, import_stdlib=True):
+def hy_compile(
+    tree,
+    module,
+    root=ast.Module,
+    get_expr=False,
+    compiler=None,
+    filename=None,
+    source=None,
+    import_stdlib=True,
+):
     """Compile a hy.models.Object tree into a Python AST Module.
 
-    Parameters
-    ----------
-    tree: hy.models.Object
-        The Hy AST object to compile.
-
-    module: str or types.ModuleType, optional
-        Module, or name of the module, in which the Hy tree is evaluated.
-        The module associated with `compiler` takes priority over this value.
-
-    root: ast object, optional (ast.Module)
-        Root object for the Python AST tree.
-
-    get_expr: bool, optional (False)
-        If true, return a tuple with `(root_obj, last_expression)`.
-
-    compiler: HyASTCompiler, optional
-        An existing Hy compiler to use for compilation.  Also serves as
-        the `module` value when given.
-
-    filename: str, optional
-        The filename corresponding to the source for `tree`.  This will be
-        overridden by the `filename` field of `tree`, if any; otherwise, it
-        defaults to "<string>".  When `compiler` is given, its `filename` field
-        value is always used.
-
-    source: str, optional
-        A string containing the source code for `tree`.  This will be
-        overridden by the `source` field of `tree`, if any; otherwise,
-        if `None`, an attempt will be made to obtain it from the module given by
-        `module`.  When `compiler` is given, its `source` field value is always
-        used.
-
-    Returns
-    -------
-    out : A Python AST tree
+    Args:
+        tree (Object): The Hy AST object to compile.
+        module (Union[str, types.ModuleType]): Module, or name of the module, in which the Hy tree is evaluated.
+            The module associated with `compiler` takes priority over this value.
+        root (Type[ast.AST]): Root object for the Python AST tree.
+        get_expr (bool): If true, return a tuple with `(root_obj, last_expression)`.
+        compiler (Optional[HyASTCompiler]): An existing Hy compiler to use for compilation.  Also serves as
+            the `module` value when given.
+        filename (Optional[str]): The filename corresponding to the source for `tree`.  This will be
+            overridden by the `filename` field of `tree`, if any; otherwise, it
+            defaults to "<string>".  When `compiler` is given, its `filename` field
+            value is always used.
+        source (Optional[str]): A string containing the source code for `tree`.  This will be
+            overridden by the `source` field of `tree`, if any; otherwise,
+            if `None`, an attempt will be made to obtain it from the module given by
+            `module`.  When `compiler` is given, its `source` field value is always
+            used.
+
+    Returns:
+        ast.AST: A Python AST tree
     """
     module = get_compiler_module(module, compiler, False)
 
     if isinstance(module, str):
         if module.startswith('<') and module.endswith('>'):
             module = types.ModuleType(module)
         else:
@@ -800,15 +806,16 @@
 
     compiler = compiler or HyASTCompiler(module, filename=filename, source=source)
 
     if import_stdlib:
         # Import hy for compile time, but save the compiled AST.
         stdlib_ast = compiler.compile(mkexpr("eval-and-compile", mkexpr("import", "hy")))
 
-    result = compiler.compile(tree)
+    with compiler.scope:
+        result = compiler.compile(tree)
     expr = result.force_expr
 
     if not get_expr:
         result += result.expr_as_stmt()
 
     body = []
```

### Comparing `hy-1.0a3/hy/completer.py` & `hy-1.0a4/hy/completer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-
 import contextlib
 import os
 import re
 import sys
 import builtins
 
 import hy.macros
 import hy.compiler
 
 
 docomplete = True
 
 try:
     import readline
-except ImportError:
-    try:
-        import pyreadline.rlmain
-        import pyreadline.unicode_helper  # NOQA
-        import readline
-    except ImportError:
+except AttributeError as e:
+    # https://github.com/pyreadline/pyreadline/issues/65
+    if "module 'collections' has no attribute 'Callable'" in str(e):
         docomplete = False
+    else:
+        raise
+except ImportError:
+    docomplete = False
 
 if docomplete:
     if sys.platform == 'darwin' and 'libedit' in readline.__doc__:
         readline_bind = "bind ^I rl_complete"
     else:
         readline_bind = "tab: complete"
 
 
-class Completer(object):
+class Completer:
 
     def __init__(self, namespace={}):
         if not isinstance(namespace, dict):
             raise TypeError('namespace must be a dictionary')
         self.namespace = namespace
         self.path = [builtins.__dict__,
                      namespace]
@@ -102,20 +99,20 @@
 
         history = os.environ.get(
             "HY_HISTORY", os.path.expanduser("~/.hy-history"))
         readline.parse_and_bind("set blink-matching-paren on")
 
         try:
             readline.read_history_file(history)
-        except IOError:
+        except OSError:
             pass
 
         readline.parse_and_bind(readline_bind)
 
     try:
         yield
     finally:
         if docomplete:
             try:
                 readline.write_history_file(history)
-            except IOError:
+            except OSError:
                 pass
```

### Comparing `hy-1.0a3/hy/core/hy_repr.hy` & `hy-1.0a4/hy/core/hy_repr.hy`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,14 @@
-;; Copyright 2021 the authors.
-;; This file is part of Hy, which is free software licensed under the Expat
-;; license. See the LICENSE.
-
 (import
-  [math [isnan]]
-  [fractions [Fraction]]
+  math [isnan]
+  fractions [Fraction]
   re
   datetime
-  collections)
-
-(try
-  (import [_collections_abc [dict-keys dict-values dict-items]])
-  (except [ImportError]
-    (defclass C)
-    (setv [dict-keys dict-values dict-items] [C C C])))
+  collections
+  _collections_abc [dict-keys dict-values dict-items])
 
 (setv _registry {})
 (defn hy-repr-register [types f [placeholder None]]
   "``hy.repr-register`` lets you set the function that ``hy.repr`` calls to
   represent a type.
 
   Examples:
@@ -109,44 +100,65 @@
   (setv syntax {
     'quote "'"
     'quasiquote "`"
     'unquote "~"
     'unquote-splice "~@"
     'unpack-iterable "#* "
     'unpack-mapping "#** "})
-  (if (and x (in (get x 0) syntax))
-    (+ (get syntax (get x 0)) (hy-repr (get x 1)))
-    (+ "(" (_cat x) ")"))))
+  (cond
+    [(and x (in (get x 0) syntax))
+      (+ (get syntax (get x 0)) (hy-repr (get x 1)))]
+    [(and
+         (= (len x) 3)
+         (= (get x 0) 'hy._Fraction)
+         (all (gfor
+           i (cut x 1 None)
+           (isinstance i (, int hy.models.Integer)))))
+        (.join "/" (map hy-repr (cut x 1 None)))]
+    [True
+      (+ "(" (_cat x) ")")])))
 
 (hy-repr-register [hy.models.Symbol hy.models.Keyword] str)
 (hy-repr-register [hy.models.String str hy.models.Bytes bytes] (fn [x]
   (setv r (.lstrip (_base-repr x) "ub"))
-  (+
-    (if (isinstance x bytes) "b" "")
-    (if (.startswith "\"" r)
-      ; If Python's built-in repr produced a double-quoted string, use
-      ; that.
-      r
-      ; Otherwise, we have a single-quoted string, which isn't valid Hy, so
-      ; convert it.
-      (+ "\"" (.replace (cut r 1 -1) "\"" "\\\"") "\"")))))
+  (if (is-not None (getattr x "brackets" None))
+    f"#[{x.brackets}[{x}]{x.brackets}]"
+    (+
+      (if (isinstance x bytes) "b" "")
+      (if (.startswith "\"" r)
+        ; If Python's built-in repr produced a double-quoted string, use
+        ; that.
+        r
+        ; Otherwise, we have a single-quoted string, which isn't valid Hy, so
+        ; convert it.
+        (+ "\"" (.replace (cut r 1 -1) "\"" "\\\"") "\""))))))
+(hy-repr-register bytearray (fn [x]
+  f"(bytearray {(hy-repr (bytes x))})"))
 (hy-repr-register bool str)
 (hy-repr-register [hy.models.Float float] (fn [x]
   (setv fx (float x))
   (cond
     [(isnan fx)  "NaN"]
     [(= fx Inf)  "Inf"]
     [(= fx -Inf) "-Inf"]
     [True (_base-repr x)])))
 
 (hy-repr-register [hy.models.Complex complex] (fn [x]
   (.replace (.replace (.strip (_base-repr x) "()") "inf" "Inf") "nan" "NaN")))
 (hy-repr-register Fraction (fn [x]
   (.format "{}/{}" (hy-repr x.numerator) (hy-repr x.denominator))))
 
+(hy-repr-register [range slice] (fn [x]
+  (setv op (. (type x) __name__))
+  (if (= x.step (if (is (type x) range) 1))
+    (if (= x.start (if (is (type x) range) 0))
+      f"({op} {x.stop})"
+      f"({op} {x.start} {x.stop})")
+    f"({op} {x.start} {x.stop} {x.step})")))
+
 (hy-repr-register
   hy.models.FComponent
   (fn [x] (+
     "{"
     (hy-repr (get x 0))
     (if x.conversion f" !{x.conversion}" "")
     (if (> (len x) 1)
@@ -155,29 +167,58 @@
         (hy-repr (get x 1))))
       "")
     "}")))
 
 (hy-repr-register
   hy.models.FString
   (fn [fstring]
-    (+ "f\""
-       #* (lfor component fstring
-                :setv s (hy-repr component)
-                (if (isinstance component hy.models.String)
-                    (-> s (cut 1 -1) (.replace "{" "{{") (.replace "}" "}}"))
-                    s))
-       "\"")))
+    (if (is-not None fstring.brackets)
+      (+ "#[" fstring.brackets "["
+         #* (lfor component fstring
+                  (if (isinstance component hy.models.String)
+                      (.replace (.replace (str component)
+                        "{" "{{")
+                        "}" "}}")
+                      (hy-repr component)))
+         "]" fstring.brackets "]")
+      (+ "f\""
+         #* (lfor component fstring
+                  :setv s (hy-repr component)
+                  (if (isinstance component hy.models.String)
+                      (.replace (.replace (cut s 1 -1)
+                        "{" "{{")
+                        "}" "}}")
+                      s))
+         "\""))))
 
 (setv _matchobject-type (type (re.match "" "")))
 (hy-repr-register _matchobject-type (fn [x]
   (.format "<{}.{} object; :span {} :match {}>"
     _matchobject-type.__module__
     _matchobject-type.__name__
     (hy-repr (.span x))
     (hy-repr (.group x 0)))))
+(hy-repr-register re.Pattern (fn [x]
+  (setv flags (& x.flags (~ re.UNICODE)))
+    ; We remove re.UNICODE since it's redundant with the type
+    ; of the pattern, and Python's `repr` omits it, too.
+  (.format "(re.compile {}{})"
+    (hy-repr x.pattern)
+    (if flags
+      (+ " " (do
+        ; Convert `flags` from an integer to a list of names.
+        (setv flags (re.RegexFlag flags))
+        (setv flags (lfor
+          f (sorted re.RegexFlag)
+          :if (& f flags)
+          (+ "re." f.name)))
+        (if (= (len flags) 1)
+          (get flags 0)
+          (.format "(| {})" (.join " " flags)))))
+      ""))))
 
 (hy-repr-register datetime.datetime (fn [x]
   (.format "(datetime.datetime {}{})"
     (_strftime-0 x "%Y %m %d %H %M %S")
     (_repr-time-innards x))))
 (hy-repr-register datetime.date (fn [x]
   (_strftime-0 x "(datetime.date %Y %m %d)")))
@@ -191,26 +232,33 @@
     (if (is-not x.tzinfo None) (+ ":tzinfo " (hy-repr x.tzinfo)))
     (if x.fold (+ ":fold " (hy-repr x.fold)))])))))
 (defn _strftime-0 [x fmt]
   ; Remove leading 0s in `strftime`. This is a substitute for the `-`
   ; flag for when Python isn't built with glibc.
   (re.sub r"(\A| )0([0-9])" r"\1\2" (.strftime x fmt)))
 
+(hy-repr-register collections.ChainMap (fn [x]
+  (.format "(ChainMap {})"
+    (_cat x.maps))))
 (hy-repr-register collections.Counter (fn [x]
   (.format "(Counter {})"
     (hy-repr (dict x)))))
+(hy-repr-register collections.OrderedDict (fn [x]
+  (.format "(OrderedDict {})"
+    (hy-repr (list (.items x))))))
 (hy-repr-register collections.defaultdict (fn [x]
   (.format "(defaultdict {} {})"
     (hy-repr x.default-factory)
     (hy-repr (dict x)))))
 
 (for [[types fmt] [
     [[list hy.models.List] "[...]"]
     [[set hy.models.Set] "#{...}"]
     [frozenset "(frozenset #{...})"]
+    [collections.deque "(deque [...])"]
     [dict-keys "(dict-keys [...])"]
     [dict-values "(dict-values [...])"]
     [dict-items "(dict-items [...])"]]]
   (defn mkrepr [fmt]
     (fn [x] (.replace fmt "..." (_cat x) 1)))
   (hy-repr-register types :placeholder fmt (mkrepr fmt)))
 
@@ -222,15 +270,15 @@
     ; It's a named tuple. (We can't use `isinstance` or so because
     ; generated named-tuple classes don't actually inherit from
     ; collections.namedtuple.)
     (return (.format "({} {})"
                      (. (type x) __name__)
                      (.join " " (gfor [k v] (zip x._fields x) (+ ":" k " " (hy-repr v)))))))
 
-  (unless (isinstance x hy.models.Object)
+  (when (not (isinstance x hy.models.Object))
     (return (repr x)))
   ; Call (.repr x) using the first class of x that doesn't inherit from
   ; hy.models.Object.
   (.__repr__
     (next (gfor
       t (. (type x) __mro__)
       :if (not (issubclass t hy.models.Object))
```

### Comparing `hy-1.0a3/hy/core/result_macros.py` & `hy-1.0a4/hy/core/result_macros.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-
 """This file contains Hy's core macros that are written in Python and
 return compiler Result objects (or Python AST objects) rather than Hy
 model trees. These macros serve the role of special forms in other
 Lisps: all ordinary macros should eventually compile down to one of
 these, or to one of the model builders in hy.compiler."""
 
 # ------------------------------------------------
 # * Imports
 # ------------------------------------------------
 
 import ast, keyword, textwrap
 from itertools import dropwhile
+from contextlib import nullcontext
 
 from funcparserlib.parser import (some, many, oneplus, maybe,
     forward_decl)
 
 from hy.models import (Expression, Keyword, Integer, Complex, String,
     FComponent, FString, Bytes, Symbol, Float, List, Dict, Sequence,
     is_unpack)
 from hy.model_patterns import (FORM, SYM, KEYWORD, STR, LITERAL, sym,
-    brackets, notpexpr, dolike, pexpr, times, Tag, tag, unpack, braces)
+    brackets, notpexpr, dolike, pexpr, times, Tag, tag, unpack, braces,
+    keepsym)
 from hy.lex import mangle, unmangle
 from hy.macros import pattern_macro, require
 from hy.errors import (HyTypeError, HyEvalError, HyInternalError)
 from hy.compiler import Result, asty, mkexpr, hy_eval
+from hy.scoping import ScopeFn, ScopeGen, ScopeGlobal, ScopeLet, is_inside_function_scope
 
 # ------------------------------------------------
 # * Helpers
 # ------------------------------------------------
 
 Inf = float('inf')
 
@@ -77,15 +76,16 @@
             else Result())
 
 @pattern_macro(["py", "pys"], [STR])
 def compile_inline_python(compiler, expr, root, code):
     exec_mode = root == "pys"
 
     try:
-        o = ast.parse(
+        o = asty.parse(
+            expr,
             textwrap.dedent(code) if exec_mode else code,
             compiler.filename,
             'exec' if exec_mode else 'eval').body
     except (SyntaxError, ValueError) as e:
         raise compiler._syntax_error(
             expr,
             "Python parse error in '{}': {}".format(root, e))
@@ -135,25 +135,18 @@
     body = [form]
 
     if isinstance(form, Sequence):
         contents = []
         for x in form:
             f_contents, splice = render_quoted_form(compiler, x, level)
             if splice:
-                contents.append(Expression([
-                    Symbol("list"),
-                    Expression([Symbol("or"), f_contents, List()])]))
-            else:
-                contents.append(List([f_contents]))
-        if form:
-            # If there are arguments, they can be spliced
-            # so we build a sum...
-            body = [Expression([Symbol("+"), List()] + contents)]
-        else:
-            body = [List()]
+                f_contents = Expression([Symbol("unpack-iterable"),
+                                         Expression([Symbol("or"), f_contents, List()])])
+            contents.append(f_contents)
+        body = [List(contents)]
 
         if isinstance(form, FString) and form.brackets is not None:
             body.extend([Keyword("brackets"), form.brackets])
         elif isinstance(form, FComponent) and form.conversion is not None:
             body.extend([Keyword("conversion"), String(form.conversion)])
 
     elif isinstance(form, Symbol):
@@ -162,15 +155,15 @@
     elif isinstance(form, Keyword):
         body = [String(form.name)]
 
     elif isinstance(form, String):
         if form.brackets is not None:
             body.extend([Keyword("brackets"), form.brackets])
 
-    ret = Expression([Symbol(name)] + body).replace(form)
+    ret = Expression([Symbol(name), *body]).replace(form)
     return ret, False
 
 # ------------------------------------------------
 # * Python operators
 # ------------------------------------------------
 
 @pattern_macro(["not", "~"], [FORM], shadow = True)
@@ -363,30 +356,33 @@
             is_assignment_expr=is_assignment_expr)
     return result
 
 @pattern_macro(["annotate"], [FORM, FORM])
 def compile_basic_annotation(compiler, expr, root, ann, target):
     return compile_assign(compiler, ann, target, None)
 
-def compile_assign(compiler, ann, name, value, *, is_assignment_expr = False):
+def compile_assign(compiler, ann, name, value, *, is_assignment_expr = False, let_scope = None):
     # Ensure that assignment expressions have a result and no annotation.
     assert not is_assignment_expr or (value is not None and ann is None)
 
-    ld_name = compiler.compile(name)
-
     annotate_only = value is None
     if annotate_only:
         result = Result()
     else:
-        result = compiler.compile(value)
+        with let_scope or nullcontext():
+            result = compiler.compile(value)
+        if let_scope:
+            name = let_scope.add(name)
+
+    ld_name = compiler.compile(name)
 
     if (result.temp_variables
             and isinstance(name, Symbol)
             and '.' not in name):
-        result.rename(compiler._nonconst(name))
+        result.rename(compiler, compiler._nonconst(name))
         if not is_assignment_expr:
             # Throw away .expr to ensure that (setv ...) returns None.
             result.expr = None
     else:
         st_name = compiler._storeize(name, ld_name)
 
         if ann is not None:
@@ -408,15 +404,22 @@
             target=st_name, targets=[st_name])
 
     return result
 
 @pattern_macro(["global", "nonlocal"], [oneplus(SYM)])
 def compile_global_or_nonlocal(compiler, expr, root, syms):
     node = asty.Global if root == "global" else asty.Nonlocal
-    return node(expr, names=list(map(mangle, syms)))
+    ret = node(expr, names=[mangle(s) for s in syms])
+
+    try:
+        compiler.scope.define_nonlocal(ret, root)
+    except SyntaxError as e:
+        raise compiler._syntax_error(expr, e.msg)
+
+    return ret if ret.names else Result()
 
 @pattern_macro("del", [many(FORM)])
 def compile_del_expression(compiler, expr, name, args):
     if not args:
         return asty.Pass(expr)
 
     del_targets = []
@@ -443,31 +446,64 @@
             expr,
             value=ret.force_expr,
             slice=ast.Index(value=ix),
             ctx=ast.Load())
 
     return ret
 
-@pattern_macro(".", [FORM, many(SYM | brackets(FORM))])
+
+
+notsym = lambda *dissallowed: some(
+    lambda x: isinstance(x, Symbol) and str(x) not in dissallowed
+)
+
+
+@pattern_macro(
+    ".",
+    [
+        FORM,
+        many(
+            SYM
+            | brackets(FORM)
+            | pexpr(notsym("unpack-iterable", "unpack-mapping"), many(FORM))
+        ),
+    ],
+)
 def compile_attribute_access(compiler, expr, name, invocant, keys):
     ret = compiler.compile(invocant)
 
     for attr in keys:
         if isinstance(attr, Symbol):
-            ret += asty.Attribute(attr,
-                                  value=ret.force_expr,
-                                  attr=mangle(attr),
-                                  ctx=ast.Load())
-        else: # attr is a hy List
+            ret += asty.Attribute(
+                attr, value=ret.force_expr, attr=mangle(attr), ctx=ast.Load()
+            )
+        elif isinstance(attr, Expression):
+            root, args = attr
+            func = asty.Attribute(
+                root, value=ret.force_expr, attr=mangle(root), ctx=ast.Load()
+            )
+
+            args, funcret, keywords = compiler._compile_collect(args, with_kwargs=True)
+            ret += (
+                funcret
+                + func
+                + asty.Call(expr, func=func, args=args, keywords=keywords)
+            )
+        else:  # attr is a hy List
             compiled_attr = compiler.compile(attr[0])
-            ret = compiled_attr + ret + asty.Subscript(
-                attr,
-                value=ret.force_expr,
-                slice=ast.Index(value=compiled_attr.force_expr),
-                ctx=ast.Load())
+            ret = (
+                compiled_attr
+                + ret
+                + asty.Subscript(
+                    attr,
+                    value=ret.force_expr,
+                    slice=ast.Index(value=compiled_attr.force_expr),
+                    ctx=ast.Load(),
+                )
+            )
 
     return ret
 
 @pattern_macro("cut", [FORM, maybe(FORM), maybe(FORM), maybe(FORM)])
 def compile_cut_expression(compiler, expr, name, obj, lower, upper, step):
     ret = [Result()]
     def c(e):
@@ -598,133 +634,178 @@
         "for":  asty.For,
         "lfor": asty.ListComp,
         "dfor": asty.DictComp,
         "sfor": asty.SetComp,
         "gfor": asty.GeneratorExp}[root]
     is_for = root == "for"
 
-    orel = []
-    if is_for:
-        # Get the `else`.
-        body, else_expr = final
-        if else_expr is not None:
-            orel.append(compiler._compile_branch(else_expr))
-            orel[0] += orel[0].expr_as_stmt()
-    else:
-        # Get the final value (and for dictionary
-        # comprehensions, the final key).
-        if node_class is asty.DictComp:
-            key, elt = map(compiler.compile, final)
+    ctx = nullcontext() if is_for else compiler.scope.create(ScopeGen)
+    with ctx as scope:
+
+        # Compile the parts.
+        if is_for:
+            parts = parts[0]
+        if not parts:
+            return Result(expr=asty.parse(
+                expr, {
+                    asty.For: "None",
+                    asty.ListComp: "[]",
+                    asty.DictComp: "{}",
+                    asty.SetComp: "{1}.__class__()",
+                    asty.GeneratorExp: "(_ for _ in [])"
+                }[node_class]).body[0].value)
+        new_parts = []
+        for p in parts:
+            if p.tag in ("if", "do"):
+                tag_value = compiler.compile(p.value)
+            else:
+                tag_value = [compiler._storeize(p.value[0], compiler.compile(p.value[0])),
+                        compiler.compile(p.value[1])]
+                if not is_for:
+                    scope.iterator(tag_value[0])
+            new_parts.append(Tag(p.tag, tag_value))
+        parts = new_parts
+
+        orel = []
+        if is_for:
+            # Get the `else`.
+            body, else_expr = final
+            if else_expr is not None:
+                orel.append(compiler._compile_branch(else_expr))
+                orel[0] += orel[0].expr_as_stmt()
         else:
-            key = None
-            elt = compiler.compile(final)
+            # Get the final value (and for dictionary
+            # comprehensions, the final key).
+            if node_class is asty.DictComp:
+                key, elt = map(compiler.compile, final)
+            else:
+                key = None
+                elt = compiler.compile(final)
 
-    # Compile the parts.
-    if is_for:
-        parts = parts[0]
-    if not parts:
-        return Result(expr=ast.parse({
-            asty.For: "None",
-            asty.ListComp: "[]",
-            asty.DictComp: "{}",
-            asty.SetComp: "{1}.__class__()",
-            asty.GeneratorExp: "(_ for _ in [])"}[node_class]).body[0].value)
-    parts = [
-        Tag(p.tag, compiler.compile(p.value) if p.tag in ["if", "do"] else [
-            compiler._storeize(p.value[0], compiler.compile(p.value[0])),
-            compiler.compile(p.value[1])])
-        for p in parts]
-
-    # Produce a result.
-    if (is_for or elt.stmts or (key is not None and key.stmts) or
-        any(p.tag == 'do' or (p.value[1].stmts if p.tag in ("for", "afor", "setv") else p.value.stmts)
-            for p in parts)):
-        # The desired comprehension can't be expressed as a
-        # real Python comprehension. We'll write it as a nested
-        # loop in a function instead.
-        def f(parts):
-            # This function is called recursively to construct
-            # the nested loop.
-            if not parts:
-                if is_for:
-                    if body:
-                        bd = compiler._compile_branch(body)
-                        return bd + bd.expr_as_stmt()
-                    return Result(stmts=[asty.Pass(expr)])
-                if node_class is asty.DictComp:
-                    ret = key + elt
-                    val = asty.Tuple(
-                        key, ctx=ast.Load(),
-                        elts=[key.force_expr, elt.force_expr])
+        # Produce a result.
+        if (is_for or elt.stmts or (key is not None and key.stmts) or
+            any(p.tag == 'do' or (p.value[1].stmts if p.tag in ("for", "afor", "setv") else p.value.stmts)
+                for p in parts)):
+            # The desired comprehension can't be expressed as a
+            # real Python comprehension. We'll write it as a nested
+            # loop in a function instead.
+            def f(parts):
+                # This function is called recursively to construct
+                # the nested loop.
+                if not parts:
+                    if is_for:
+                        if body:
+                            bd = compiler._compile_branch(body)
+                            return bd + bd.expr_as_stmt()
+                        return Result(stmts=[asty.Pass(expr)])
+                    if node_class is asty.DictComp:
+                        ret = key + elt
+                        val = asty.Tuple(
+                            key, ctx=ast.Load(),
+                            elts=[key.force_expr, elt.force_expr])
+                    else:
+                        ret = elt
+                        val = elt.force_expr
+                    return ret + asty.Expr(
+                        elt, value=asty.Yield(elt, value=val))
+                (tagname, v), parts = parts[0], parts[1:]
+                if tagname in ("for", "afor"):
+                    orelse = orel and orel.pop().stmts
+                    node = asty.AsyncFor if tagname == "afor" else asty.For
+                    return v[1] + node(
+                        v[1], target=v[0], iter=v[1].force_expr, body=f(parts).stmts,
+                        orelse=orelse)
+                elif tagname == "setv":
+                    return v[1] + asty.Assign(
+                        v[1], targets=[v[0]], value=v[1].force_expr) + f(parts)
+                elif tagname == "if":
+                    return v + asty.If(
+                        v, test=v.force_expr, body=f(parts).stmts, orelse=[])
+                elif tagname == "do":
+                    return v + v.expr_as_stmt() + f(parts)
                 else:
-                    ret = elt
-                    val = elt.force_expr
-                return ret + asty.Expr(
-                    elt, value=asty.Yield(elt, value=val))
-            (tagname, v), parts = parts[0], parts[1:]
+                    raise ValueError("can't happen")
+            if is_for:
+                return f(parts)
+            fname = compiler.get_anon_var()
+            # Define the generator function.
+            stmts = []
+            ret = Result()
+            assignment_names = scope.finalize()
+            if scope.exposing_assignments and assignment_names:
+                # expose inner assignments to outer scope
+                unlocal_type = (
+                    asty.Nonlocal
+                    if is_inside_function_scope(scope.parent)
+                    else asty.Global
+                )
+                stmts.append(unlocal_type(expr, names=assignment_names))
+
+                # create a fake assignment statement so python places these
+                # names in the immediately outer scope
+                if_body = []
+                if scope.nonlocal_vars:
+                    if_body.append(
+                        asty.Nonlocal(expr, names=list(sorted(scope.nonlocal_vars)))
+                    )
+                assignments = asty.Tuple(
+                    expr,
+                    elts=[asty.Name(expr, id=var, ctx=ast.Store())
+                          for var in assignment_names],
+                    ctx=ast.Store())
+                if_body.append(
+                    asty.Assign(
+                        expr,
+                        targets=[assignments],
+                        value=asty.Constant(expr, value=None),
+                    )
+                )
+                ret += asty.If(expr, test=asty.Constant(expr, value=False), body=if_body, orelse=[])
+
+            ret += asty.FunctionDef(
+                expr,
+                name=fname,
+                args=ast.arguments(
+                    args=[], vararg=None, kwarg=None, posonlyargs=[],
+                    kwonlyargs=[], kw_defaults=[], defaults=[]),
+                body=stmts + f(parts).stmts,
+                decorator_list=[])
+            # Immediately call the new function. Unless the user asked
+            # for a generator, wrap the call in `[].__class__(...)` or
+            # `{}.__class__(...)` or `{1}.__class__(...)` to get the
+            # right type. We don't want to just use e.g. `list(...)`
+            # because the name `list` might be rebound.
+            return ret + Result(expr=asty.parse(
+                expr,
+                "{}({}())".format(
+                    {asty.ListComp: "[].__class__",
+                     asty.DictComp: "{}.__class__",
+                     asty.SetComp: "{1}.__class__",
+                     asty.GeneratorExp: ""}[node_class],
+                    fname)).body[0].value)
+
+        # We can produce a real comprehension.
+        generators = []
+        for tagname, v in parts:
             if tagname in ("for", "afor"):
-                orelse = orel and orel.pop().stmts
-                node = asty.AsyncFor if tagname == "afor" else asty.For
-                return v[1] + node(
-                    v[1], target=v[0], iter=v[1].force_expr, body=f(parts).stmts,
-                    orelse=orelse)
+                generators.append(ast.comprehension(
+                    target=v[0], iter=v[1].expr, ifs=[],
+                    is_async=int(tagname == "afor")))
             elif tagname == "setv":
-                return v[1] + asty.Assign(
-                    v[1], targets=[v[0]], value=v[1].force_expr) + f(parts)
+                generators.append(ast.comprehension(
+                    target=v[0],
+                    iter=asty.Tuple(v[1], elts=[v[1].expr], ctx=ast.Load()),
+                    ifs=[], is_async=0))
             elif tagname == "if":
-                return v + asty.If(
-                    v, test=v.force_expr, body=f(parts).stmts, orelse=[])
-            elif tagname == "do":
-                return v + v.expr_as_stmt() + f(parts)
+                generators[-1].ifs.append(v.expr)
             else:
                 raise ValueError("can't happen")
-        if is_for:
-            return f(parts)
-        fname = compiler.get_anon_var()
-        # Define the generator function.
-        ret = Result() + asty.FunctionDef(
-            expr,
-            name=fname,
-            args=ast.arguments(
-                args=[], vararg=None, kwarg=None, posonlyargs=[],
-                kwonlyargs=[], kw_defaults=[], defaults=[]),
-            body=f(parts).stmts,
-            decorator_list=[])
-        # Immediately call the new function. Unless the user asked
-        # for a generator, wrap the call in `[].__class__(...)` or
-        # `{}.__class__(...)` or `{1}.__class__(...)` to get the
-        # right type. We don't want to just use e.g. `list(...)`
-        # because the name `list` might be rebound.
-        return ret + Result(expr=ast.parse(
-            "{}({}())".format(
-                {asty.ListComp: "[].__class__",
-                 asty.DictComp: "{}.__class__",
-                 asty.SetComp: "{1}.__class__",
-                 asty.GeneratorExp: ""}[node_class],
-                fname)).body[0].value)
-
-    # We can produce a real comprehension.
-    generators = []
-    for tagname, v in parts:
-        if tagname in ("for", "afor"):
-            generators.append(ast.comprehension(
-                target=v[0], iter=v[1].expr, ifs=[],
-                is_async=int(tagname == "afor")))
-        elif tagname == "setv":
-            generators.append(ast.comprehension(
-                target=v[0],
-                iter=asty.Tuple(v[1], elts=[v[1].expr], ctx=ast.Load()),
-                ifs=[], is_async=0))
-        elif tagname == "if":
-            generators[-1].ifs.append(v.expr)
-        else:
-            raise ValueError("can't happen")
-    if node_class is asty.DictComp:
-        return asty.DictComp(expr, key=key.expr, value=elt.expr, generators=generators)
-    return node_class(expr, elt=elt.expr, generators=generators)
+        if node_class is asty.DictComp:
+            return asty.DictComp(expr, key=key.expr, value=elt.expr, generators=generators)
+        return node_class(expr, elt=elt.expr, generators=generators)
 
 # ------------------------------------------------
 # * More looping
 # ------------------------------------------------
 
 @pattern_macro(["while"], [FORM, many(notpexpr("else")), maybe(dolike("else"))])
 def compile_while_expression(compiler, expr, root, cond, body, else_expr):
@@ -779,16 +860,16 @@
     return (asty.Break if root == "break" else asty.Continue)(expr)
 
 # ------------------------------------------------
 # * `with`
 # ------------------------------------------------
 
 @pattern_macro(["with", "with/a"], [
-    brackets(times(1, Inf, FORM + FORM)) |
-        brackets((FORM >> (lambda x: [(Symbol('_'), x)]))),
+    brackets(oneplus(FORM + FORM)) |
+        brackets(FORM >> (lambda x: [(Symbol('_'), x)])),
     many(FORM)])
 def compile_with_expression(compiler, expr, root, args, body):
     body = compiler._compile_branch(body)
 
     # Store the result of the body in a tempvar
     temp_var = compiler.get_anon_var()
     name = asty.Name(expr, id=mangle(temp_var), ctx=ast.Store())
@@ -823,18 +904,14 @@
 
     return ret
 
 # ------------------------------------------------
 # * `switch`
 # ------------------------------------------------
 
-notsym = lambda *dissallowed: some(
-    lambda x: isinstance(x, Symbol) and str(x) not in dissallowed
-)
-keepsym = lambda wanted: some(lambda x: x == Symbol(wanted))
 _pattern = forward_decl()
 _pattern.define(
     (
         SYM
         | LITERAL
         | brackets(many(_pattern | unpack("iterable")))
         | pexpr(keepsym("."), many(SYM))
@@ -889,47 +966,46 @@
                         kw_defaults=[],
                         defaults=[],
                     ),
                     body=guard.stmts + [asty.Return(guard.expr, value=guard.expr)],
                     decorator_list=[],
                 )
                 lifted_if_defs.append(guardret)
-                guard = Result(expr=ast.parse(f"{fname}()").body[0].value)
+                guard = Result(expr=asty.parse(guard, f"{fname}()").body[0].value)
 
         match_cases.append(
             ast.match_case(
                 pattern=pattern,
                 guard=guard.force_expr if guard else None,
                 body=body,
             )
         )
 
     returnable = Result(
         expr=asty.Name(expr, id=return_var.id, ctx=ast.Load()),
         temp_variables=[return_var],
     )
     ret = Result() + subject
-    ret += subject.expr_as_stmt()
     ret += asty.Assign(expr, targets=[return_var], value=asty.Constant(expr, value=None))
     if not match_cases:
         return ret + returnable
 
     for lifted_if in lifted_if_defs:
         ret += lifted_if
     ret += asty.Match(expr, subject=subject.force_expr, cases=match_cases)
     return ret + returnable
 
 def compile_pattern(compiler, pattern):
     value, assignment = pattern
     if assignment is not None:
-        return asty.MatchAs(
+        return compiler.scope.assign(asty.MatchAs(
             value,
             pattern=compile_pattern(compiler, (value, None)),
-            name=mangle(compiler._nonconst(assignment)),
-        )
+            name=mangle(compiler._nonconst(assignment))
+        ))
 
     if str(value) in ("None", "True", "False"):
         return asty.MatchSingleton(
             value,
             value=compiler.compile(value).force_expr.value,
         )
     elif (
@@ -940,15 +1016,15 @@
         return asty.MatchValue(
             value,
             value=compiler.compile(value).expr,
         )
     elif value == Symbol("_"):
         return asty.MatchAs(value)
     elif isinstance(value, Symbol):
-        return asty.MatchAs(value, name=mangle(value))
+        return compiler.scope.assign(asty.MatchAs(value, name=mangle(value)))
     elif isinstance(value, Expression) and value[0] == Symbol("|"):
         return asty.MatchOr(
             value,
             patterns=[compile_pattern(compiler, v) for v in value[1]],
         )
     elif isinstance(value, Expression) and value[0] == Symbol("."):
         root, syms = value
@@ -965,37 +1041,38 @@
         patterns = value[0] if isinstance(value, List) else value[1:][0]
         patterns = [
             compile_pattern(compiler, (v, None) if is_unpack("iterable", v) else v)
             for v in patterns
         ]
         return asty.MatchSequence(value, patterns=patterns)
     elif is_unpack("iterable", value):
-        return asty.MatchStar(value, name=mangle(value[1]))
+        return compiler.scope.assign(asty.MatchStar(value, name=mangle(value[1])))
 
     elif isinstance(value, Dict):
         kvs, rest = value
         keys, values = zip(*kvs) if kvs else ([], [])
-        return asty.MatchMapping(
+        # Call `scope.assign` for the assignment to `rest`.
+        return compiler.scope.assign(asty.MatchMapping(
             value,
             keys=[compiler.compile(key).expr for key in keys],
             patterns=[compile_pattern(compiler, v) for v in values],
             rest=mangle(rest) if rest else None,
-        )
+        ))
     elif isinstance(value, Expression):
         root, args, kwargs = value
         keywords, values = zip(*kwargs) if kwargs else ([], [])
         return asty.MatchClass(
             value,
-            cls=asty.Name(root, id=mangle(root), ctx=ast.Load()),
+            cls=compiler.scope.access(asty.Name(root, id=mangle(root), ctx=ast.Load())),
             patterns=[compile_pattern(compiler, v) for v in args],
             kwd_attrs=[kwd.name for kwd in keywords],
             kwd_patterns=[compile_pattern(compiler, value) for value in values],
         )
     else:
-        raise compiler._syntax_error(value, "unsuported")
+        raise compiler._syntax_error(value, "unsupported")
 
 # ------------------------------------------------
 # * `raise` and `try`
 # ------------------------------------------------
 
 @pattern_macro("raise", [maybe(FORM), maybe(sym(":from") + FORM)])
 def compile_raise_expression(compiler, expr, root, exc, cause):
@@ -1099,15 +1176,20 @@
             types += asty.Tuple(exceptions_list, elts=elts, ctx=ast.Load())
         else:
             # [] → all exceptions caught
             types = Result()
     else:
         types = compiler.compile(exceptions_list)
 
-    body = compiler._compile_branch(body)
+    # Create a "fake" scope for the exception variable.
+    # See: https://docs.python.org/3/reference/compound_stmts.html#the-try-statement
+    with compiler.scope.create(ScopeLet) as scope:
+        if name:
+            scope.add(name, name)
+        body = compiler._compile_branch(body)
     body += asty.Assign(expr, targets=[var], value=body.force_expr)
     body += body.expr_as_stmt()
 
     return types + asty.ExceptHandler(
         expr, type=types.expr, name=name,
         body=body.stmts or [asty.Pass(expr)])
 
@@ -1129,42 +1211,46 @@
 @pattern_macro(["fn", "fn/a"], [OPTIONAL_ANNOTATION, lambda_list, many(FORM)])
 def compile_function_lambda(compiler, expr, root, returns, params, body):
     posonly, args, rest, kwonly, kwargs = params
     has_annotations = returns is not None or any(
         isinstance(param, tuple) and param[0] is not None
         for param in (posonly or []) + args + kwonly + [rest, kwargs]
     )
-    body = compiler._compile_branch(body)
+    args, ret = compile_lambda_list(compiler, params)
+    with compiler.scope.create(ScopeFn, args):
+        body = compiler._compile_branch(body)
 
     # Compile to lambda if we can
     if not has_annotations and not body.stmts and root != "fn/a":
-        args, ret = compile_lambda_list(compiler, params, Result())
         return ret + asty.Lambda(expr, args=args, body=body.force_expr)
 
     # Otherwise create a standard function
     node = asty.AsyncFunctionDef if root == "fn/a" else asty.FunctionDef
     name = compiler.get_anon_var()
-    ret = compile_function_node(compiler, expr, node, name, params, returns, body)
+    ret += compile_function_node(compiler, expr, node, name, args, returns, body)
 
     # return its name as the final expr
     return ret + Result(expr=ret.temp_variables[0])
 
 @pattern_macro(["defn", "defn/a"], [OPTIONAL_ANNOTATION, SYM, lambda_list, many(FORM)])
 def compile_function_def(compiler, expr, root, returns, name, params, body):
     node = asty.FunctionDef if root == "defn" else asty.AsyncFunctionDef
-    body = compiler._compile_branch(body)
+    args, ret = compile_lambda_list(compiler, params)
+    name = mangle(compiler._nonconst(name))
+    compiler.scope.define(name)
+    with compiler.scope.create(ScopeFn, args):
+        body = compiler._compile_branch(body)
 
-    return compile_function_node(
+    return ret + compile_function_node(
         compiler, expr, node,
-        mangle(compiler._nonconst(name)), params, returns, body
+        name, args, returns, body
     )
 
-def compile_function_node(compiler, expr, node, name, params, returns, body):
+def compile_function_node(compiler, expr, node, name, args, returns, body):
     ret = Result()
-    args, ret = compile_lambda_list(compiler, params, ret)
 
     if body.expr:
         body += asty.Return(body.expr, value=body.expr)
 
     ret += node(
         expr,
         name=name,
@@ -1201,15 +1287,16 @@
                 *body
             ])
         ])
     ]).replace(expr))
 
     return ret + ret.expr_as_stmt()
 
-def compile_lambda_list(compiler, params, ret):
+def compile_lambda_list(compiler, params):
+    ret = Result()
     posonly_parms, args_parms, rest_parms, kwonly_parms, kwargs_parms = params
 
     py_reserved_param = next(
         (
             sym
             for param in (
                 (posonly_parms or [])
@@ -1355,92 +1442,93 @@
         compiler._compile_collect(base_list[0], with_kwargs=True))
 
     bodyr = Result()
 
     if docstring is not None:
         bodyr += compiler.compile(docstring).expr_as_stmt()
 
-    e = compiler._compile_branch(body)
-    bodyr += e + e.expr_as_stmt()
+    name = mangle(compiler._nonconst(name))
+    compiler.scope.define(name)
+
+    with compiler.scope.create(ScopeFn):
+        e = compiler._compile_branch(body)
+        bodyr += e + e.expr_as_stmt()
 
     return bases + asty.ClassDef(
         expr,
         decorator_list=[],
-        name=mangle(compiler._nonconst(name)),
+        name=name,
         keywords=keywords,
         starargs=None,
         kwargs=None,
         bases=bases_expr,
         body=bodyr.stmts or [asty.Pass(expr)])
 
 # ------------------------------------------------
 # * `import` and `require`
 # ------------------------------------------------
 
 def importlike(*name_types):
     name = some(lambda x: isinstance(x, name_types) and "." not in x)
     return [many(
-        SYM |
-        brackets(SYM, sym(":as"), name) |
-        brackets(SYM, brackets(many(
-            name + maybe(sym(":as") + name)))))]
+        SYM + maybe(keepsym("*")
+                    | (keepsym(":as") + name)
+                    | brackets(many(
+                        name + maybe(sym(":as") + name)))))]
 
 @pattern_macro("import", importlike(Symbol))
 @pattern_macro("require", importlike(Symbol, String))
 def compile_import_or_require(compiler, expr, root, entries):
     ret = Result()
 
     for entry in entries:
         assignments = "ALL"
         prefix = ""
 
-        if isinstance(entry, Symbol):
+        module, rest = entry
+        if rest is None:
             # e.g., (import foo)
-            module, prefix = entry, entry
-        elif isinstance(entry, List) and isinstance(entry[1], Symbol):
-            # e.g., (import [foo :as bar])
-            module, prefix = entry
+            prefix = module
+        elif rest == Symbol("*"):
+            # e.g., (import foo *)
+            pass
+        elif rest[0] == Keyword("as"):
+            # e.g., (import foo :as bar)
+            prefix = rest[1]
         else:
-            # e.g., (import [foo [bar baz :as MyBaz bing]])
-            # or (import [foo [*]])
-            module, kids = entry
-            kids = kids[0]
-            if (Symbol('*'), None) in kids:
-                if len(kids) != 1:
-                    star = kids[kids.index((Symbol('*'), None))][0]
-                    raise compiler._syntax_error(star,
-                        "* in an import name list must be on its own")
-            else:
-                assignments = [(k, v or k) for k, v in kids]
+            # e.g., (import foo [bar baz :as MyBaz bing])
+            assignments = [(k, v or k) for k, v in rest[0]]
 
         ast_module = mangle(module)
 
         if root == "import":
-            module = ast_module.lstrip(".")
-            level = len(ast_module) - len(module)
+            module_name = ast_module.lstrip(".")
+            level = len(ast_module) - len(module_name)
             if assignments == "ALL" and prefix == "":
                 node = asty.ImportFrom
-                names = [asty.alias(entry, name="*", asname=None)]
+                names = [asty.alias(module, name="*", asname=None)]
             elif assignments == "ALL":
+                compiler.scope.define(mangle(prefix))
                 node = asty.Import
-                prefix = mangle(prefix)
                 names = [asty.alias(
-                    entry,
+                    module,
                     name=ast_module,
-                    asname=prefix if prefix != module else None)]
+                    asname=mangle(prefix) if prefix != module else None)]
             else:
                 node = asty.ImportFrom
-                names = [
-                    asty.alias(
-                        entry,
-                        name=mangle(k),
-                        asname=None if v == k else mangle(v))
-                    for k, v in assignments]
+                names = []
+                for k, v in assignments:
+                    compiler.scope.define(mangle(v))
+                    names.append(
+                        asty.alias(
+                            module,
+                            name=mangle(k),
+                            asname=None if v == k else mangle(v)))
             ret += node(
-                expr, module=module or None, names=names, level=level)
+                expr, module=module_name or None, names=names, level=level)
 
         elif require(ast_module, compiler.module, assignments=assignments,
                      prefix=prefix):
             # Actually calling `require` is necessary for macro expansions
             # occurring during compilation.
             # The `require` we're creating in AST is the same as above, but used at
             # run-time (e.g. when modules are loaded via bytecode).
@@ -1480,7 +1568,19 @@
     # form to set `msg` to a variable.
     msg_var = compiler.get_anon_var()
     return compiler.compile(mkexpr(
         'if', mkexpr('and', '__debug__', mkexpr('not', [test])),
             mkexpr('do',
                 mkexpr('setv', msg_var, [msg]),
                 mkexpr('assert', 'False', msg_var))).replace(expr))
+
+@pattern_macro("let", [brackets(many(OPTIONAL_ANNOTATION + FORM + FORM)), many(FORM)])
+def compile_let(compiler, expr, root, bindings, body):
+    res = Result()
+    bindings = bindings[0]
+    scope = compiler.scope.create(ScopeLet)
+
+    for ann, target, value in bindings:
+        res += compile_assign(compiler, ann, target, value, let_scope=scope)
+
+    with scope:
+       return res + compiler.compile(mkexpr("do", *body).replace(expr))
```

### Comparing `hy-1.0a3/hy/core/shadow.hy` & `hy-1.0a4/hy/pyops.hy`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,30 @@
-;; Copyright 2021 the authors.
-;; This file is part of Hy, which is free software licensed under the Expat
-;; license. See the LICENSE.
+"Python provides various :ref:`binary and unary operators
+<py:expressions>`. These are usually invoked in Hy using core macros of
+the same name: for example, ``(+ 1 2)`` calls the core macro named
+``+``, which uses Python's addition operator. An exception to the names
+being the same is that Python's ``==`` is called ``=`` in Hy.
+
+By importing from the module ``hy.pyops`` (typically with a star import,
+as in ``(import hy.pyops *)``), you can also use these operators as
+functions. Functions are first-class objects, so you can say things like
+``(map - xs)`` to negate all the numbers in the list ``xs``. Since
+macros shadow functions, forms like ``(- 1 2)`` will still call the
+macro instead of the function.
+
+The functions in ``hy.pyops`` have the same semantics as their macro
+equivalents, with one exception: functions can't short-circuit, so the
+functions for the logical operators, such as ``and``, unconditionally
+evaluate all arguments."
 
 ;;;; Hy shadow functions
 
-(import operator)
-
-(import [hy.lex [mangle]])
-
-(import [functools [reduce]])
+(import
+  functools [reduce]
+  operator)
 
 (defn + [#* args]
   "Shadowed `+` operator adds `args`."
   (if (= (len args) 0)
       0
       (if (= (len args) 1)
           (+ (get args 0))
@@ -261,14 +273,14 @@
   "
   (setv coll (get coll key1))
   (for [k keys]
     (setv coll (get coll k)))
   coll)
 
 (setv __all__
-  (list (map mangle [
+  (list (map hy.mangle [
     '+ '- '* '** '/ '// '% '@
     '<< '>> '& '| '^ '~
     '< '> '<= '>= '= '!=
     'and 'or 'not
     'is 'is-not 'in 'not-in
     'get])))
```

### Comparing `hy-1.0a3/hy/errors.py` & `hy-1.0a4/hy/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# -*- encoding: utf-8 -*-
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
 import os
 import re
 import sys
 import traceback
 import pkgutil
 
 from functools import reduce
 from colorama import Fore
 from contextlib import contextmanager
 from hy import _initialize_env_var
+from hy._compat import PYPY
 
 _hy_filter_internal_errors = _initialize_env_var('HY_FILTER_INTERNAL_ERRORS',
                                                  True)
 COLORED = _initialize_env_var('HY_COLORED_ERRORS', False)
 
 
 class HyError(Exception):
@@ -32,45 +29,45 @@
 
 class HyLanguageError(HyError):
     """Errors caused by invalid use of the Hy language.
 
     This, and any errors inheriting from this, are user-facing.
     """
 
-    def __init__(self, message, expression=None, filename=None, source=None,
-                 lineno=1, colno=1):
+    def __init__(
+        self,
+        message,
+        expression=None,
+        filename=None,
+        source=None,
+        lineno=1,
+        colno=1,
+    ):
         """
-        Parameters
-        ----------
-        message: str
-            The message to display for this error.
-        expression: HyObject, optional
-            The Hy expression generating this error.
-        filename: str, optional
-            The filename for the source code generating this error.
-            Expression-provided information will take precedence of this value.
-        source: str, optional
-            The actual source code generating this error.  Expression-provided
-            information will take precedence of this value.
-        lineno: int, optional
-            The line number of the error.  Expression-provided information will
-            take precedence of this value.
-        colno: int, optional
-            The column number of the error.  Expression-provided information
-            will take precedence of this value.
+        Args:
+            message (str): The message to display for this error.
+            expression (Optional[Object]): The Hy expression generating this error.
+            filename (Optional[str]): The filename for the source code generating this error.
+                Expression-provided information will take precedence of this value. Defaults to `None`.
+            source (Optional[str]): The actual source code generating this error.  Expression-provided
+                information will take precedence of this value. Defaults to `None`.
+            lineno (int): The line number of the error.  Expression-provided information will
+                take precedence of this value. Defaults to `1`.
+            colno (int): The column number of the error.  Expression-provided information
+                will take precedence of this value. Defaults to `1`.
         """
         self.msg = message
         self.compute_lineinfo(expression, filename, source, lineno, colno)
 
         if isinstance(self, SyntaxError):
             syntax_error_args = (self.filename, self.lineno, self.offset,
                                  self.text)
-            super(HyLanguageError, self).__init__(message, syntax_error_args)
+            super().__init__(message, syntax_error_args)
         else:
-            super(HyLanguageError, self).__init__(message)
+            super().__init__(message)
 
     def compute_lineinfo(self, expression, filename, source, lineno, colno):
 
         # NOTE: We use `SyntaxError`'s field names (i.e. `text`, `offset`,
         # `msg`) for compatibility and print-outs.
         self.text = getattr(expression, 'source', source)
         self.filename = getattr(expression, 'filename', filename)
@@ -106,18 +103,18 @@
     def __str__(self):
         """Provide an exception message that includes SyntaxError-like source
         line information when available.
         """
         # Syntax errors are special and annotate the traceback (instead of what
         # we would do in the message that follows the traceback).
         if isinstance(self, SyntaxError):
-            return super(HyLanguageError, self).__str__()
+            return super().__str__()
         # When there isn't extra source information, use the normal message.
         elif not self.text:
-            return super(HyLanguageError, self).__str__()
+            return super().__str__()
 
         # Re-purpose Python's builtin syntax error formatting.
         output = traceback.format_exception_only(
             SyntaxError,
             SyntaxError(self.msg, (self.filename, self.lineno, self.offset,
                                    self.text)))
 
@@ -238,14 +235,21 @@
                                       'hy.cmdline', 'hy.lex.parser',
                                       'hy.importer', 'hy._compat',
                                       'hy.macros', 'hy.models',
                                       'hy.core.result_macros',
                                       'rply'])
                       if m is not None}
 
+# We can't derive these easily from just their module names due
+# to missing magic attributes in internal importlib modules
+_tb_hidden_modules.update(
+    f"<builtin>/frozen {x}" if PYPY else f"<frozen {x}>"
+    for x in ("importlib._bootstrap", "importlib._bootstrap_external")
+)
+
 
 def hy_exc_filter(exc_type, exc_value, exc_traceback):
     """Produce exceptions print-outs with all frames originating from the
     modules in `_tb_hidden_modules` filtered out.
 
     The frames are actually filtered by each module's filename and only when a
     subclass of `HyLanguageError` is emitted.
```

### Comparing `hy-1.0a3/hy/importer.py` & `hy-1.0a4/hy/importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-
-from __future__ import absolute_import
-
 import sys
 import os
 import inspect
 import pkgutil
 import types
 import importlib
 import builtins
@@ -163,26 +157,13 @@
     spec = importlib.util.spec_from_file_location(name, path)
     mod = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(mod)
     return mod
 
 
 def _inject_builtins():
-    """Inject the hy core/stdlib into python's builtins if necessary"""
+    """Inject the Hy core macros into Python's builtins if necessary"""
     if hasattr(builtins, '__hy_injected__'):
         return
-
-    # Load the standard macros first.
     hy.macros.load_macros(builtins)
-
-    # Load the standard functions directly into builtins. We have to
-    # do this manually, or else we end up in a weird circular import
-    # problem in `load_macros` with importlib trying to import
-    # `hy.core` before macros have been injected.
-    for m in "hy.core.shadow", "hy.core.language":
-        builtins.__dict__.update({
-            k: v
-            for k, v in importlib.import_module(m).__dict__.items()
-            if not k.startswith("_") and k != "hy"})
-
     # Set the marker so we don't inject again.
     builtins.__hy_injected__ = True
```

### Comparing `hy-1.0a3/hy/lex/__init__.py` & `hy-1.0a4/hy/lex/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-
-from __future__ import unicode_literals
-
 import keyword
 import re
 import sys
 import unicodedata
 
 from hy.lex.exceptions import PrematureEndOfInput, LexException  # NOQA
 from hy.models import Expression, Symbol
@@ -18,41 +12,44 @@
     from StringIO import StringIO
 
 
 def hy_parse(source, filename='<string>'):
     """Parse a Hy source string.
 
     Args:
-      source (string): Source code to parse.
-      filename (string, optional): File name corresponding to source.  Defaults to "<string>".
+      source (str): Source code to parse.
+      filename (str): File name corresponding to source.  Defaults to "<string>".
 
     Returns:
-      out : hy.models.Expression
+      Expression: the parsed models wrapped in an hy.models.Expression
     """
     _source = re.sub(r'\A#!.*', '', source)
     res = Expression([Symbol("do")] +
                        tokenize(_source + "\n",
                                 filename=filename))
     res.source = source
     res.filename = filename
     return res
 
 
-class ParserState(object):
+class ParserState:
     def __init__(self, source, filename):
         self.source = source
         self.filename = filename
 
 
 def tokenize(source, filename=None):
     """ Tokenize a Lisp file or string buffer into internal Hy objects.
 
     Args:
-    source (str): The source to tokenize.
-    filename (str, optional): The filename corresponding to `source`.
+       source (str): The source to tokenize.
+       filename (Optional[str]): The filename corresponding to `source`.
+
+    Returns:
+       typing.List[Object]: list of hy object models
     """
     from hy.lex.lexer import lexer
     from hy.lex.parser import parser
     from rply.errors import LexingError
     try:
         return parser.parse(lexer.lex(source),
                             state=ParserState(source, filename))
```

### Comparing `hy-1.0a3/hy/lex/exceptions.py` & `hy-1.0a4/hy/lex/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
 from hy.errors import HySyntaxError
 
 
 class LexException(HySyntaxError):
 
     @classmethod
     def from_lexer(cls, message, state, token):
```

### Comparing `hy-1.0a3/hy/lex/lexer.py` & `hy-1.0a4/hy/lex/lexer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-
 from rply import LexerGenerator
 
 
 lg = LexerGenerator()
 
 
 # A regexp for something that should end a quoting/unquoting operator
```

### Comparing `hy-1.0a3/hy/lex/parser.py` & `hy-1.0a4/hy/lex/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-# -*- encoding: utf-8 -*-
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-
-from __future__ import unicode_literals
-
 import re
 from functools import wraps
 
 from rply import ParserGenerator
 
 from hy.models import (Bytes, Complex, Dict, Expression, FComponent, FString,
                        Float, Integer, Keyword, List, Set, String, Symbol)
```

### Comparing `hy-1.0a3/hy/macros.py` & `hy-1.0a4/hy/macros.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
 import sys
+import os
 import builtins
 import importlib
 import inspect
 import pkgutil
 import traceback
 from ast import AST
 
 from funcparserlib.parser import NoParseError
 
-from hy._compat import PY3_8
+from hy._compat import code_replace
 from hy.model_patterns import whole
 from hy.models import replace_hy_obj, Expression, Symbol, as_model, is_unpack
 from hy.lex import mangle, unmangle
 from hy.errors import (HyLanguageError, HyMacroExpansionError, HyTypeError,
                        HyRequireError)
 import hy.compiler
 
@@ -39,15 +37,15 @@
         def wrapper_maker(name):
             def wrapper(hy_compiler, *args):
 
                 if (shadow and
                         any(is_unpack("iterable", x) for x in args)):
                     # Try a shadow function call with this name instead.
                     return Expression([
-                        Symbol('hy.core.shadow.' + name),
+                        Symbol('hy.pyops.' + name),
                         *args]).replace(hy_compiler.this)
 
                 expr = hy_compiler.this
                 root = unmangle(expr[0])
 
                 if (py_version_required and
                         sys.version_info < py_version_required):
@@ -106,44 +104,35 @@
 
         return filename
 
     source_filename = _get_filename(source_module)
     target_filename = _get_filename(target_module)
 
     return (source_filename and target_filename and
-            source_filename == target_filename)
+            os.path.samefile(source_filename, target_filename))
 
 
 def require(source_module, target_module, assignments, prefix=""):
     """Load macros from one module into the namespace of another.
 
     This function is called from the macro also named `require`.
 
-    Parameters
-    ----------
-    source_module: str or types.ModuleType
-        The module from which macros are to be imported.
-
-    target_module: str, types.ModuleType or None
-        The module into which the macros will be loaded.  If `None`, then
-        the caller's namespace.
-        The latter is useful during evaluation of generated AST/bytecode.
-
-    assignments: str or list of tuples of strs
-        The string "ALL" or a list of macro name and alias pairs.
-
-    prefix: str, optional ("")
-        If nonempty, its value is prepended to the name of each imported macro.
-        This allows one to emulate namespaced macros, like
-        "mymacromodule.mymacro", which looks like an attribute of a module.
-
-    Returns
-    -------
-    out: boolean
-        Whether or not macros were actually transferred.
+    Args:
+        source_module (Union[str, ModuleType]): The module from which macros are
+            to be imported.
+        target_module (Optional[Union[str, ModuleType]]): The module into which the
+            macros will be loaded.  If `None`, then the caller's namespace.
+            The latter is useful during evaluation of generated AST/bytecode.
+        assignments (Union[str, typing.Sequence[str]]): The string "ALL" or a list of macro name and alias pairs.
+        prefix (str): If nonempty, its value is prepended to the name of each imported macro.
+            This allows one to emulate namespaced macros, like "mymacromodule.mymacro",
+            which looks like an attribute of a module. Defaults to ""
+
+    Returns:
+        bool: Whether or not macros were actually transferred.
     """
     if target_module is None:
         parent_frame = inspect.stack()[1][0]
         target_namespace = parent_frame.f_globals
         target_module = target_namespace.get('__name__', None)
     elif isinstance(target_module, str):
         target_module = importlib.import_module(target_module)
@@ -286,32 +275,26 @@
     If the resulting `Expression` is itself macro expanded, then the namespace
     of the assigned module is checked first for a macro corresponding to the
     expression's head/car symbol.  If the head/car symbol of such a `Expression`
     is not found among the macros of its assigned module's namespace, the
     outer-most namespace--e.g.  the one given by the `module` parameter--is used
     as a fallback.
 
-    Parameters
-    ----------
-    tree: hy.models.Object or list
-        Hy AST tree.
-
-    module: str or types.ModuleType
-        Module used to determine the local namespace for macros.
-
-    compiler: HyASTCompiler, optional
-        The compiler object passed to expanded macros.
-
-    once: boolean, optional
-        Only expand the first macro in `tree`.
-
-    Returns
-    ------
-    out: hy.models.Object
-        Returns a mutated tree with macros expanded.
+    Args:
+        tree (Union[Object, list]): Hy AST tree.
+        module (Union[str, ModuleType]): Module used to determine the local
+            namespace for macros.
+        compiler (Optional[HyASTCompiler] ): The compiler object passed to
+            expanded macros. Defaults to None
+        once (bool): Only expand the first macro in `tree`. Defaults to False
+        result_ok (bool): Whether or not it's okay to return a compiler `Result` instance.
+            Defaults to True.
+
+    Returns:
+        Union[Object, Result]: A mutated tree with macros expanded.
     """
     if not inspect.ismodule(module):
         module = importlib.import_module(module)
 
     assert not compiler or compiler.module == module
 
     while isinstance(tree, Expression) and tree:
@@ -354,27 +337,14 @@
 
 def macroexpand_1(tree, module, compiler=None):
     """Expand the toplevel macro from `tree` once, in the context of
     `compiler`."""
     return macroexpand(tree, module, compiler, once=True)
 
 
-def rename_function(func, new_name):
-    """Creates a copy of a function and [re]sets the name at the code-object
-    level.
-    """
-    c = func.__code__
-    new_code = type(c)(*[getattr(c, 'co_{}'.format(a))
-                         if a != 'name' else str(new_name)
-                         for a in code_obj_args])
-
-    _fn = type(func)(new_code, func.__globals__, str(new_name),
-                     func.__defaults__, func.__closure__)
-    _fn.__dict__.update(func.__dict__)
-
-    return _fn
-
-code_obj_args = ['argcount', 'posonlyargcount', 'kwonlyargcount', 'nlocals', 'stacksize',
-                 'flags', 'code', 'consts', 'names', 'varnames', 'filename', 'name',
-                 'firstlineno', 'lnotab', 'freevars', 'cellvars']
-if not PY3_8:
-    code_obj_args.remove("posonlyargcount")
+def rename_function(f, new_name):
+    """Create a copy of a function, but with a new name."""
+    f = type(f)(
+        code_replace(f.__code__, co_name = new_name), f.__globals__,
+        str(new_name), f.__defaults__, f.__closure__)
+    f.__dict__.update(f.__dict__)
+    return f
```

### Comparing `hy-1.0a3/hy/model_patterns.py` & `hy-1.0a4/hy/model_patterns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-
 "Parser combinators for pattern-matching Hy model trees."
 
 from hy.models import Expression, Symbol, Keyword, String, List, Dict, Integer, Float, Complex, Bytes
 from funcparserlib.parser import (
     some, skip, many, finished, a, Parser, NoParseError, State)
 from functools import reduce
 from itertools import repeat
@@ -18,17 +14,24 @@
 KEYWORD = some(lambda x: isinstance(x, Keyword))
 STR = some(lambda x: isinstance(x, String))  # matches literal strings only!
 LITERAL = some(lambda x: isinstance(x, (String, Integer, Float, Complex, Bytes)))
 
 
 def sym(wanted):
     "Parse and skip the given symbol or keyword."
+    return _sym(wanted, skip)
+
+def keepsym(wanted):
+    "Parse the given symbol or keyword."
+    return _sym(wanted)
+
+def _sym(wanted, f = lambda x: x):
     if wanted.startswith(":"):
-        return skip(a(Keyword(wanted[1:])))
-    return skip(some(lambda x: x == Symbol(wanted)))
+        return f(a(Keyword(wanted[1:])))
+    return f(some(lambda x: x == Symbol(wanted)))
 
 def whole(parsers):
     """Parse the parsers in the given list one after another, then
     expect the end of the input."""
     if len(parsers) == 0:
         return finished >> (lambda x: [])
     if len(parsers) == 1:
```

### Comparing `hy-1.0a3/hy/models.py` & `hy-1.0a4/hy/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-# Copyright 2021 the authors.
-# This file is part of Hy, which is free software licensed under the Expat
-# license. See the LICENSE.
-from __future__ import unicode_literals
-
 from contextlib import contextmanager
 import re
 from math import isnan, isinf
 from hy import _initialize_env_var
 from hy.errors import HyWrapperError
 from fractions import Fraction
 import operator
@@ -40,15 +35,15 @@
     def _colored(self, text):
         if COLORED:
             return self.color + text + Fore.RESET
         else:
             return text
 
 
-class Object(object):
+class Object:
     """
     Generic Hy Object model. This is helpful to inject things into all the
     Hy lexing Objects at once.
 
     The position properties (`start_line`, `end_line`, `start_column`,
     `end_column`) are each 1-based and inclusive. For example, a symbol
     `abc` starting at the first column would have `start_column` 1 and
@@ -103,22 +98,22 @@
         return (f"hy.models.{self.__class__.__name__}"
                 f"({super(Object, self).__repr__()})")
 
     def __eq__(self, other):
         if type(self) != type(other):
             return False
         else:
-            return super(Object, self).__eq__(other)
+            return super().__eq__(other)
 
     def __hash__(self):
         return super().__hash__()
 
 
 _wrappers = {}
-
+_seen = set()
 
 def as_model(x):
     """Recurisvely promote an object ``x`` into its canonical model form.
 
     When creating macros its possible to return non-Hy model objects or
     even create an expression with non-Hy model elements::
 
@@ -144,14 +139,17 @@
               ; equal to the ``(hy.model.Integer 2)`` value in the known form.
 
        => (= (hy.as-model `(print ~(+ 1 1)) '(print 2)))
        True  ; True because ``as-model`` has walked the expression and promoted
              ; the literal int ``2`` to its model for ``(hy.model.Integer 2)``
     """
 
+    if id(x) in _seen:
+        raise HyWrapperError("Self-referential structure detected in {!r}".format(x))
+
     new = _wrappers.get(type(x), lambda y: y)(x)
     if not isinstance(new, Object):
         raise HyWrapperError("Don't know how to wrap {!r}: {!r}".format(type(x), x))
     if isinstance(x, Object):
         new = new.replace(x, recursive=False)
     return new
 
@@ -172,19 +170,29 @@
 
 class String(Object, str):
     """
     Generic Hy String object. Helpful to store string literals from Hy
     scripts. It's either a ``str`` or a ``unicode``, depending on the
     Python version.
     """
+
     def __new__(cls, s=None, brackets=None):
-        value = super(String, cls).__new__(cls, s)
+        value = super().__new__(cls, s)
+        if brackets is not None and f"]{brackets}]" in value:
+            raise ValueError(f"Syntactically illegal bracket string: {s!r}")
         value.brackets = brackets
         return value
 
+    def __repr__(self):
+        return 'hy.models.String({}{})'.format(
+            super(Object, self).__repr__(),
+            '' if self.brackets is None else
+                f', brackets={self.brackets!r}')
+
+
 _wrappers[str] = String
 
 
 class Bytes(Object, bytes):
     """
     Generic Hy Bytes object. It's either a ``bytes`` or a ``str``, depending
     on the Python version.
@@ -203,15 +211,15 @@
         s = str(s)
         if not from_parser:
             # Check that the symbol is syntactically legal.
             from hy.lex.lexer import identifier
             from hy.lex.parser import symbol_like
             if not re.fullmatch(identifier, s) or symbol_like(s) is not None:
                 raise ValueError(f'Syntactically illegal symbol: {s!r}')
-        return super(Symbol, cls).__new__(cls, s)
+        return super().__new__(cls, s)
 
 _wrappers[bool] = lambda x: Symbol("True") if x else Symbol("False")
 _wrappers[type(None)] = lambda foo: Symbol("None")
 
 
 class Keyword(Object):
     """Generic Hy Keyword object."""
@@ -295,15 +303,15 @@
                     break
             else:
                 # We've got a string, no known leader; base 10.
                 number = int(number, base=10)
         else:
             # We've got a non-string; convert straight.
             number = int(number)
-        return super(Integer, cls).__new__(cls, number)
+        return super().__new__(cls, number)
 
 
 _wrappers[int] = Integer
 
 
 def check_inf_nan_cap(arg, value):
     if isinstance(arg, str):
@@ -316,38 +324,38 @@
 class Float(Object, float):
     """
     Internal representation of a Hy Float. May raise a ValueError as if
     float(foo) was called, given Float(foo).
     """
 
     def __new__(cls, num, *args, **kwargs):
-        value = super(Float, cls).__new__(cls, strip_digit_separators(num))
+        value = super().__new__(cls, strip_digit_separators(num))
         check_inf_nan_cap(num, value)
         return value
 
 _wrappers[float] = Float
 
 
 class Complex(Object, complex):
     """
     Internal representation of a Hy Complex. May raise a ValueError as if
     complex(foo) was called, given Complex(foo).
     """
 
     def __new__(cls, real, imag=0, *args, **kwargs):
         if isinstance(real, str):
-            value = super(Complex, cls).__new__(
+            value = super().__new__(
                 cls, strip_digit_separators(real)
             )
             p1, _, p2 = real.lstrip("+-").replace("-", "+").partition("+")
             check_inf_nan_cap(p1, value.imag if "j" in p1 else value.real)
             if p2:
                 check_inf_nan_cap(p2, value.imag)
             return value
-        return super(Complex, cls).__new__(cls, real, imag)
+        return super().__new__(cls, real, imag)
 
 _wrappers[complex] = Complex
 
 
 class Sequence(Object, tuple, _ColoredModel):
     """
     An abstract type for sequence-like models to inherit from.
@@ -357,34 +365,37 @@
         if recursive:
             for x in self:
                 replace_hy_obj(x, other)
         Object.replace(self, other)
         return self
 
     def __add__(self, other):
-        return self.__class__(super(Sequence, self).__add__(
+        return self.__class__(super().__add__(
             tuple(other) if isinstance(other, list) else other))
 
     def __getslice__(self, start, end):
-        return self.__class__(super(Sequence, self).__getslice__(start, end))
+        return self.__class__(super().__getslice__(start, end))
 
     def __getitem__(self, item):
-        ret = super(Sequence, self).__getitem__(item)
+        ret = super().__getitem__(item)
 
         if isinstance(item, slice):
             return self.__class__(ret)
 
         return ret
 
     color = None
 
     def __repr__(self):
-        return str(self) if PRETTY else super(Sequence, self).__repr__()
+        return self._pretty_str() if PRETTY else super().__repr__()
 
     def __str__(self):
+        return self._pretty_str()
+
+    def _pretty_str(self):
         with pretty():
             if self:
                 return self._colored("hy.models.{}{}\n  {}{}".format(
                     self._colored(self.__class__.__name__),
                     self._colored("(["),
                     self._colored(",\n  ").join(map(repr_indent, self)),
                     self._colored("])"),
@@ -411,53 +422,88 @@
         return self
 
     def __repr__(self):
         return 'hy.models.FComponent({})'.format(
             super(Object, self).__repr__() +
             ', conversion=' + repr(self.conversion))
 
+
+def _string_in_node(string, node):
+    if isinstance(node, String) and string in node:
+        return True
+    elif isinstance(node, (FComponent, FString)):
+        return any(_string_in_node(string, node) for node in node)
+    else:
+        return False
+
+
 class FString(Sequence):
     """
     Generic Hy F-String object, for smarter f-string handling.
     Mimics ast.JoinedStr, but using String and FComponent.
     """
     def __new__(cls, s=None, brackets=None):
         value = super().__new__(cls,
           # Join adjacent string nodes for the sake of equality
           # testing.
               (node
                   for is_string, components in groupby(s,
                       lambda x: isinstance(x, String))
-                  for node in ([reduce(operator.add, components)]
+                  for node in ([reduce(lambda left, right: String(left + right), components)]
                       if is_string else components)))
+
+        if brackets is not None and _string_in_node(f"]{brackets}]", value):
+            raise ValueError(f"Syntactically illegal bracket string: {s!r}")
         value.brackets = brackets
         return value
 
+    def __repr__(self):
+        return self._suffixize(super().__repr__())
+    def __str__(self):
+        return self._suffixize(super().__str__())
+    def _suffixize(self, x):
+        if self.brackets is None:
+           return x
+        return '{}{}brackets={!r})'.format(
+           x[:-1],  # Clip off the final close paren
+           '' if x[-2] == '(' else ', ',
+           self.brackets)
+
 
 class List(Sequence):
     color = Fore.CYAN
 
 
 def recwrap(f):
-    return lambda l: f(as_model(x) for x in l)
+
+    def lambda_to_return(l):
+        _seen.add(id(l))
+        try:
+            return f(as_model(x) for x in l)
+        finally:
+            _seen.remove(id(l))
+
+    return lambda_to_return
 
 _wrappers[FComponent] = recwrap(FComponent)
-_wrappers[FString] = recwrap(FString)
+_wrappers[FString] = lambda fstr: FString(
+    (as_model(x) for x in fstr), brackets=fstr.brackets
+)
 _wrappers[List] = recwrap(List)
 _wrappers[list] = recwrap(List)
 _wrappers[tuple] = recwrap(List)
 
 
 class Dict(Sequence, _ColoredModel):
     """
     Dict (just a representation of a dict)
     """
     color = Fore.GREEN
 
-    def __str__(self):
+    def _pretty_str(self):
         with pretty():
             if self:
                 pairs = []
                 for k, v in zip(self[::2],self[1::2]):
                     k, v = repr_indent(k), repr_indent(v)
                     pairs.append(
                         ("{0}{c}\n  {1}\n  "
@@ -478,16 +524,23 @@
 
     def values(self):
         return list(self[1::2])
 
     def items(self):
         return list(zip(self.keys(), self.values()))
 
+def _dict_wrapper(d):
+    _seen.add(id(d))
+    try:
+        return Dict(as_model(x) for x in sum(d.items(), ()))
+    finally:
+        _seen.remove(id(d))
+
 _wrappers[Dict] = recwrap(Dict)
-_wrappers[dict] = lambda d: Dict(as_model(x) for x in sum(d.items(), ()))
+_wrappers[dict] = _dict_wrapper
 
 
 class Expression(Sequence):
     """
     Hy S-Expression. Basically just a list.
     """
     color = Fore.YELLOW
```

### Comparing `hy-1.0a3/hy.egg-info/PKG-INFO` & `hy-1.0a4/hy.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: hy
-Version: 1.0a3
+Version: 1.0a4
 Summary: Lisp and Python love each other.
 Home-page: http://hylang.org/
 Author: Paul Tagliamonte
 Author-email: tag@pault.ag
 License: Expat
+Project-URL: Documentation, https://docs.hylang.org/
+Project-URL: Source, https://github.com/hylang/hy
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Lisp
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >= 3.7, < 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
 Hy is a Python <--> Lisp layer. It helps
 make things work nicer, and lets Python and the Hy lisp variant play
 nice together.
```

