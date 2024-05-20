# Comparing `tmp/types-pygit2-1.14.0.20240317.tar.gz` & `tmp/types-pygit2-1.15.0.20240520.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pygit2-1.14.0.20240317.tar", last modified: Sun Mar 17 02:14:57 2024, max compression
+gzip compressed data, was "types-pygit2-1.15.0.20240520.tar", last modified: Mon May 20 02:23:50 2024, max compression
```

## Comparing `types-pygit2-1.14.0.20240317.tar` & `types-pygit2-1.15.0.20240520.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 02:14:57.219846 types-pygit2-1.14.0.20240317/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-17 02:14:56.000000 types-pygit2-1.14.0.20240317/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-17 02:14:56.000000 types-pygit2-1.14.0.20240317/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-17 02:14:57.219846 types-pygit2-1.14.0.20240317/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 02:14:57.219846 types-pygit2-1.14.0.20240317/pygit2-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-17 02:14:56.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/_build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/_libgit2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25644 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/_pygit2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/_run.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/blame.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/blob.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/branches.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/callbacks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/ffi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/filter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/index.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/legacyenums.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/packbuilder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/references.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/refspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/remotes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/repository.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/settings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/submodules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-17 02:14:35.000000 types-pygit2-1.14.0.20240317/pygit2-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 02:14:57.219846 types-pygit2-1.14.0.20240317/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-17 02:14:56.000000 types-pygit2-1.14.0.20240317/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 02:14:57.219846 types-pygit2-1.14.0.20240317/types_pygit2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-17 02:14:57.000000 types-pygit2-1.14.0.20240317/types_pygit2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-17 02:14:57.000000 types-pygit2-1.14.0.20240317/types_pygit2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 02:14:57.000000 types-pygit2-1.14.0.20240317/types_pygit2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-17 02:14:57.000000 types-pygit2-1.14.0.20240317/types_pygit2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-17 02:14:57.000000 types-pygit2-1.14.0.20240317/types_pygit2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:50.732027 types-pygit2-1.15.0.20240520/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-20 02:23:50.732027 types-pygit2-1.15.0.20240520/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:50.732027 types-pygit2-1.15.0.20240520/pygit2-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/_build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/_libgit2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25387 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/_pygit2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/_run.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/blame.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/blob.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/branches.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/callbacks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/ffi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/filter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/index.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/legacyenums.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/packbuilder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/references.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/refspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/remotes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7636 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/repository.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/submodules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-20 02:23:29.000000 types-pygit2-1.15.0.20240520/pygit2-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:23:50.732027 types-pygit2-1.15.0.20240520/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:50.732027 types-pygit2-1.15.0.20240520/types_pygit2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/types_pygit2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/types_pygit2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/types_pygit2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/types_pygit2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 02:23:50.000000 types-pygit2-1.15.0.20240520/types_pygit2.egg-info/top_level.txt
```

### Comparing `types-pygit2-1.14.0.20240317/CHANGELOG.md` & `types-pygit2-1.15.0.20240520/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.15.0.20240520 (2024-05-20)
+
+Bump pygit2 to 1.15 and fix enums (#11983)
+
 ## 1.14.0.20240317 (2024-03-17)
 
 pygit2: Workaround python/mypy#16972 (#11584)
 
 To fix the signatures of `clone_repository` and `init_repository` as
 seen by type checkers.
```

### Comparing `types-pygit2-1.14.0.20240317/PKG-INFO` & `types-pygit2-1.15.0.20240520/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pygit2
-Version: 1.14.0.20240317
+Version: 1.15.0.20240520
 Summary: Typing stubs for pygit2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pygit2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pygit2`.
 
 This version of `types-pygit2` aims to provide accurate annotations
-for `pygit2==1.14.*`.
+for `pygit2==1.15.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pygit2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d436110d1361ec82ae3971ed10d94c0090647b63` and was tested
-with mypy 1.9.0, pyright 1.1.354, and
-pytype 2024.3.11.
+This package was generated from typeshed commit `b8d144d49106e14ab6bfcf40a5b8aea7639d6150` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
```

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/__init__.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/_pygit2.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/_pygit2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 GIT_CHECKOUT_SKIP_LOCKED_DIRECTORIES: int
 GIT_CHECKOUT_SKIP_UNMERGED: int
 GIT_CHECKOUT_UPDATE_ONLY: int
 GIT_CHECKOUT_USE_OURS: int
 GIT_CHECKOUT_USE_THEIRS: int
 GIT_CONFIG_HIGHEST_LEVEL: int
 GIT_CONFIG_LEVEL_APP: int
+GIT_CONFIG_LEVEL_WORKTREE: int
 GIT_CONFIG_LEVEL_GLOBAL: int
 GIT_CONFIG_LEVEL_LOCAL: int
 GIT_CONFIG_LEVEL_PROGRAMDATA: int
 GIT_CONFIG_LEVEL_SYSTEM: int
 GIT_CONFIG_LEVEL_XDG: int
 GIT_DELTA_ADDED: int
 GIT_DELTA_CONFLICTED: int
@@ -171,19 +172,14 @@
 GIT_OBJECT_BLOB: int
 GIT_OBJECT_COMMIT: int
 GIT_OBJECT_INVALID: int
 GIT_OBJECT_OFS_DELTA: int
 GIT_OBJECT_REF_DELTA: int
 GIT_OBJECT_TAG: int
 GIT_OBJECT_TREE: int
-GIT_OBJ_ANY: int
-GIT_OBJ_BLOB: int
-GIT_OBJ_COMMIT: int
-GIT_OBJ_TAG: int
-GIT_OBJ_TREE: int
 GIT_OID_HEXSZ: int
 GIT_OID_HEX_ZERO: str
 GIT_OID_MINPREFIXLEN: int
 GIT_OID_RAWSZ: int
 GIT_OPT_DISABLE_PACK_KEEP_FILE_CHECKS: int
 GIT_OPT_ENABLE_CACHING: int
 GIT_OPT_ENABLE_FSYNC_GITDIR: int
@@ -213,24 +209,17 @@
 GIT_OPT_SET_SSL_CIPHERS: int
 GIT_OPT_SET_TEMPLATE_PATH: int
 GIT_OPT_SET_USER_AGENT: int
 GIT_OPT_SET_WINDOWS_SHAREMODE: int
 GIT_REFERENCES_ALL: int
 GIT_REFERENCES_BRANCHES: int
 GIT_REFERENCES_TAGS: int
-GIT_REF_INVALID: int
-GIT_REF_LISTALL: int
-GIT_REF_OID: int
-GIT_REF_SYMBOLIC: int
 GIT_RESET_HARD: int
 GIT_RESET_MIXED: int
 GIT_RESET_SOFT: int
-GIT_REVPARSE_MERGE_BASE: int
-GIT_REVPARSE_RANGE: int
-GIT_REVPARSE_SINGLE: int
 GIT_REVSPEC_MERGE_BASE: int
 GIT_REVSPEC_RANGE: int
 GIT_REVSPEC_SINGLE: int
 GIT_SORT_NONE: int
 GIT_SORT_REVERSE: int
 GIT_SORT_TIME: int
 GIT_SORT_TOPOLOGICAL: int
@@ -283,18 +272,16 @@
 _GIT_OBJ_COMMIT: TypeAlias = Literal[1]
 _GIT_OBJ_TAG: TypeAlias = Literal[4]
 _GIT_OBJ_TREE: TypeAlias = Literal[2]
 
 class Object:
     _pointer: bytes
     filemode: FileMode
-    hex: str
     id: Oid
     name: str | None
-    oid: Oid
     raw_name: bytes | None
     short_id: str
     type: Literal[_GIT_OBJ_COMMIT, _GIT_OBJ_TREE, _GIT_OBJ_TAG, _GIT_OBJ_BLOB]
     type_str: Literal["commit", "tree", "tag", "blob"]
     @overload
     def peel(self, target_type: Literal[_GIT_OBJ_COMMIT]) -> Commit: ...
     @overload
@@ -522,15 +509,14 @@
 
 @final
 class OdbBackendPack(OdbBackend):
     def __init__(self, path: StrOrBytesPath) -> None: ...
 
 @final
 class Oid:
-    hex: str
     raw: bytes
     def __init__(self, raw: bytes = ..., hex: str = ...) -> None: ...
     def __eq__(self, other: object) -> bool: ...
     def __ge__(self, other: object) -> bool: ...
     def __gt__(self, other: object) -> bool: ...
     def __hash__(self) -> int: ...
     def __le__(self, other: object) -> bool: ...
```

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/blame.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/blame.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/blob.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/blob.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/branches.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/branches.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/callbacks.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/callbacks.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/config.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/credentials.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/credentials.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/index.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/index.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from _typeshed import StrOrBytesPath, StrPath
 from collections.abc import Iterator
-from typing_extensions import Self
+from typing_extensions import Self, deprecated
 
 from _cffi_backend import _CDataBase
 
 from ._pygit2 import Diff, Oid, Tree
 from .enums import DiffOption, FileMode
 from .repository import BaseRepository
 from .utils import _IntoStrArray
@@ -36,14 +36,15 @@
     path: str
     id: Oid
     mode: FileMode
     def __init__(self, path: str, object_id: Oid, mode: FileMode) -> None: ...
     @property
     def oid(self) -> Oid: ...
     @property
+    @deprecated("Use str(entry.id)")
     def hex(self) -> str: ...
     def __eq__(self, other: object) -> bool: ...
 
 class ConflictCollection:
     def __init__(self, index: Index) -> None: ...
     def __getitem__(self, path: StrOrBytesPath) -> tuple[IndexEntry, IndexEntry, IndexEntry]: ...
     def __delitem__(self, path: StrOrBytesPath) -> None: ...
```

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/legacyenums.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/legacyenums.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/packbuilder.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/packbuilder.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/references.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/references.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/refspec.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/refspec.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/remotes.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/remotes.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,21 @@
     @property
     def refspec_count(self) -> int: ...
     def get_refspec(self, n: int) -> Refspec: ...
     @property
     def fetch_refspecs(self) -> list[str]: ...
     @property
     def push_refspecs(self) -> list[str]: ...
-    def push(self, specs: _IntoStrArray, callbacks: RemoteCallbacks | None = None, proxy: _ProxySpec = None) -> None: ...
+    def push(
+        self,
+        specs: _IntoStrArray,
+        callbacks: RemoteCallbacks | None = None,
+        proxy: _ProxySpec = None,
+        push_options: _IntoStrArray | None = None,
+    ) -> None: ...
 
 _RemoteName: TypeAlias = bytes | str
 
 class RemoteCollection:
     def __init__(self, repo: BaseRepository) -> None: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[Remote]: ...
```

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/repository.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/repository.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from _typeshed import StrOrBytesPath
-from collections.abc import Callable, Iterable, Iterator
+from collections.abc import Callable, Iterator
 from tarfile import TarInfo
 from typing import IO, Any, Protocol
-from typing_extensions import TypeAlias, deprecated
+from typing_extensions import TypeAlias
 
 from ._pygit2 import Blob, Commit, Diff, Object, Oid, Reference, Repository as _Repository, Signature, Tree, _OidArg
 from .blame import Blame
 from .branches import Branches
-from .callbacks import CheckoutCallbacks, RemoteCallbacks, StashApplyCallbacks
+from .callbacks import CheckoutCallbacks, StashApplyCallbacks
 from .config import Config
 from .enums import (
     AttrCheck,
     BlameFlag,
     BranchType as BranchType,
     CheckoutStrategy,
     DescribeStrategy,
@@ -22,15 +22,15 @@
     RepositoryOpenFlag,
     RepositoryState,
 )
 from .index import Index, IndexEntry
 from .packbuilder import PackBuilder
 from .references import References
 from .remotes import RemoteCollection
-from .submodules import Submodule, SubmoduleCollection
+from .submodules import SubmoduleCollection
 from .utils import _IntoStrArray
 
 _PackDelegate: TypeAlias = Callable[[PackBuilder], None]
 
 class _SupportsAddfile(Protocol):
     def addfile(self, tarinfo: TarInfo, fileobj: IO[bytes] | None = None) -> None: ...
 
@@ -43,24 +43,14 @@
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...  # not meant for direct use
     def read(self, oid: _OidArg) -> tuple[int, int, bytes]: ...
     def write(self, type: int, data: bytes) -> Oid: ...
     def pack(
         self, path: StrOrBytesPath | None = None, pack_delegate: _PackDelegate | None = None, n_threads: int | None = None
     ) -> int: ...
     def __iter__(self) -> Iterator[Oid]: ...
-    @deprecated("Use repo.submodules.add(...)")
-    def add_submodule(self, url: str, path: str, link: bool = True, callbacks: RemoteCallbacks | None = None) -> Submodule: ...
-    @deprecated("Use repo.submodules[...]")
-    def lookup_submodule(self, path: str) -> Submodule: ...
-    @deprecated("Use repo.submodules.init(...)")
-    def init_submodules(self, submodules: Iterable[str] | None = None, overwrite: bool = False) -> None: ...
-    @deprecated("Use repo.submodules.update(...)")
-    def update_submodules(
-        self, submodules: Iterable[str] | None = None, init: bool = False, callbacks: RemoteCallbacks | None = None
-    ) -> None: ...
     def get(self, key: _OidArg, default: Object | None = None) -> Object | None: ...
     def __getitem__(self, key: _OidArg) -> Object: ...
     def __contains__(self, key: _OidArg) -> bool: ...
     @property
     def config(self) -> Config: ...
     @property
     def config_snapshot(self) -> Config: ...
```

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/settings.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/settings.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/pygit2-stubs/submodules.pyi` & `types-pygit2-1.15.0.20240520/pygit2-stubs/submodules.pyi`

 * *Files identical despite different names*

### Comparing `types-pygit2-1.14.0.20240317/setup.py` & `types-pygit2-1.15.0.20240520/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pygit2`.
 
 This version of `types-pygit2` aims to provide accurate annotations
-for `pygit2==1.14.*`.
+for `pygit2==1.15.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pygit2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d436110d1361ec82ae3971ed10d94c0090647b63` and was tested
-with mypy 1.9.0, pyright 1.1.354, and
-pytype 2024.3.11.
+This package was generated from typeshed commit `b8d144d49106e14ab6bfcf40a5b8aea7639d6150` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="1.14.0.20240317",
+      version="1.15.0.20240520",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pygit2.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-cffi'],
       packages=['pygit2-stubs'],
-      package_data={'pygit2-stubs': ['__init__.pyi', '_build.pyi', '_libgit2.pyi', '_pygit2.pyi', '_run.pyi', 'blame.pyi', 'blob.pyi', 'branches.pyi', 'callbacks.pyi', 'config.pyi', 'credentials.pyi', 'enums.pyi', 'errors.pyi', 'ffi.pyi', 'filter.pyi', 'index.pyi', 'legacyenums.pyi', 'packbuilder.pyi', 'references.pyi', 'refspec.pyi', 'remotes.pyi', 'repository.pyi', 'settings.pyi', 'submodules.pyi', 'utils.pyi', 'METADATA.toml']},
+      package_data={'pygit2-stubs': ['__init__.pyi', '_build.pyi', '_libgit2.pyi', '_pygit2.pyi', '_run.pyi', 'blame.pyi', 'blob.pyi', 'branches.pyi', 'callbacks.pyi', 'config.pyi', 'credentials.pyi', 'enums.pyi', 'errors.pyi', 'ffi.pyi', 'filter.pyi', 'index.pyi', 'legacyenums.pyi', 'packbuilder.pyi', 'references.pyi', 'refspec.pyi', 'remotes.pyi', 'repository.pyi', 'settings.pyi', 'submodules.pyi', 'utils.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-pygit2-1.14.0.20240317/types_pygit2.egg-info/PKG-INFO` & `types-pygit2-1.15.0.20240520/types_pygit2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pygit2
-Version: 1.14.0.20240317
+Version: 1.15.0.20240520
 Summary: Typing stubs for pygit2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pygit2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pygit2`.
 
 This version of `types-pygit2` aims to provide accurate annotations
-for `pygit2==1.14.*`.
+for `pygit2==1.15.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pygit2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d436110d1361ec82ae3971ed10d94c0090647b63` and was tested
-with mypy 1.9.0, pyright 1.1.354, and
-pytype 2024.3.11.
+This package was generated from typeshed commit `b8d144d49106e14ab6bfcf40a5b8aea7639d6150` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
```

### Comparing `types-pygit2-1.14.0.20240317/types_pygit2.egg-info/SOURCES.txt` & `types-pygit2-1.15.0.20240520/types_pygit2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 pygit2-stubs/enums.pyi
 pygit2-stubs/errors.pyi
 pygit2-stubs/ffi.pyi
 pygit2-stubs/filter.pyi
 pygit2-stubs/index.pyi
 pygit2-stubs/legacyenums.pyi
 pygit2-stubs/packbuilder.pyi
+pygit2-stubs/py.typed
 pygit2-stubs/references.pyi
 pygit2-stubs/refspec.pyi
 pygit2-stubs/remotes.pyi
 pygit2-stubs/repository.pyi
 pygit2-stubs/settings.pyi
 pygit2-stubs/submodules.pyi
 pygit2-stubs/utils.pyi
```

