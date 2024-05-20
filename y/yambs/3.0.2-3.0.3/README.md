# Comparing `tmp/yambs-3.0.2.tar.gz` & `tmp/yambs-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-3.0.2.tar", last modified: Sat May 18 07:35:04 2024, max compression
+gzip compressed data, was "yambs-3.0.3.tar", last modified: Mon May 20 04:03:45 2024, max compression
```

## Comparing `yambs-3.0.2.tar` & `yambs-3.0.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-18 07:32:49.000000 yambs-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-18 07:35:04.015226 yambs-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-18 07:32:49.000000 yambs-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-18 07:32:49.000000 yambs-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 07:35:04.015226 yambs-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-18 07:32:49.000000 yambs-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.003225 yambs-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-18 07:32:49.000000 yambs-3.0.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-18 07:32:49.000000 yambs-3.0.2/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.003225 yambs-3.0.2/yambs/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.003225 yambs-3.0.2/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.007225 yambs-3.0.2/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/compile_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.007225 yambs-3.0.2/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.007225 yambs-3.0.2/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.007225 yambs-3.0.2/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/includes/wasm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/CommonConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Dependency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Github.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/regenerate.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/data/yambs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/dependency/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/github.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/dependency/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/dependency/handlers/yambs/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/yambs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/handlers/yambs/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dependency/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.011226 yambs-3.0.2/yambs/dist/
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/generate/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/github/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-18 07:32:49.000000 yambs-3.0.2/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:35:04.015226 yambs-3.0.2/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 07:35:03.000000 yambs-3.0.2/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.588759 yambs-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 04:01:26.000000 yambs-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-20 04:03:45.588759 yambs-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-05-20 04:01:26.000000 yambs-3.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-20 04:01:26.000000 yambs-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 04:03:45.588759 yambs-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-20 04:01:26.000000 yambs-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.572759 yambs-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-20 04:01:26.000000 yambs-3.0.3/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-20 04:01:26.000000 yambs-3.0.3/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.572759 yambs-3.0.3/yambs/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.576758 yambs-3.0.3/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.576758 yambs-3.0.3/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/commands/compile_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/commands/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.576758 yambs-3.0.3/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.576758 yambs-3.0.3/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.580759 yambs-3.0.3/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/includes/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/includes/wasm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.580759 yambs-3.0.3/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/CommonConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Dependency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Github.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.584759 yambs-3.0.3/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/regenerate.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/data/yambs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.584759 yambs-3.0.3/yambs/dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.584759 yambs-3.0.3/yambs/dependency/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/handlers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.584759 yambs-3.0.3/yambs/dependency/handlers/yambs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/handlers/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/handlers/yambs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/handlers/yambs/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dependency/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.584759 yambs-3.0.3/yambs/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.584759 yambs-3.0.3/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.588759 yambs-3.0.3/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.588759 yambs-3.0.3/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/generate/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.588759 yambs-3.0.3/yambs/github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.588759 yambs-3.0.3/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.588759 yambs-3.0.3/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-05-20 04:01:26.000000 yambs-3.0.3/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:03:45.588759 yambs-3.0.3/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-20 04:03:45.000000 yambs-3.0.3/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-20 04:03:45.000000 yambs-3.0.3/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 04:03:45.000000 yambs-3.0.3/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 04:03:45.000000 yambs-3.0.3/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-20 04:03:45.000000 yambs-3.0.3/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 04:03:45.000000 yambs-3.0.3/yambs.egg-info/top_level.txt
```

### Comparing `yambs-3.0.2/LICENSE` & `yambs-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/PKG-INFO` & `yambs-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 3.0.2
+Version: 3.0.3
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: datazen
 Requires-Dist: rcmpy>=1.5.0
 Requires-Dist: requests
 Requires-Dist: vcorelib>=2.4.2
-Requires-Dist: datazen
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -37,19 +37,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=72271a00d30bf23159c35289b5ff7a00
+    hash=934a1cb8be74864c521e3c3d3875e01d
     =====================================
 -->
 
-# yambs ([3.0.2](https://pypi.org/project/yambs/))
+# yambs ([3.0.3](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -251,15 +251,15 @@
 
 options:
   -h, --help            show this help message and exit
   -o OWNER, --owner OWNER
                         repository owner (default: 'vkottler')
   -r REPO, --repo REPO  repository name (default: 'toolchains')
   -O OUTPUT, --output OUTPUT
-                        output directory (default: 'toolchains')
+                        output directory (default: '.')
   -p PATTERN, --pattern PATTERN
                         a pattern to use to select project specifications
                         filtered by name
 
 ```
 
 ### `gen`
```

### Comparing `yambs-3.0.2/README.md` & `yambs-3.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=72271a00d30bf23159c35289b5ff7a00
+    hash=934a1cb8be74864c521e3c3d3875e01d
     =====================================
 -->
 
-# yambs ([3.0.2](https://pypi.org/project/yambs/))
+# yambs ([3.0.3](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -212,15 +212,15 @@
 
 options:
   -h, --help            show this help message and exit
   -o OWNER, --owner OWNER
                         repository owner (default: 'vkottler')
   -r REPO, --repo REPO  repository name (default: 'toolchains')
   -O OUTPUT, --output OUTPUT
-                        output directory (default: 'toolchains')
+                        output directory (default: '.')
   -p PATTERN, --pattern PATTERN
                         a pattern to use to select project specifications
                         filtered by name
 
 ```
 
 ### `gen`
```

### Comparing `yambs-3.0.2/pyproject.toml` & `yambs-3.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "3.0.2"
+version = "3.0.3"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-3.0.2/setup.py` & `yambs-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/tests/test_entry.py` & `yambs-3.0.3/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/aggregation/__init__.py` & `yambs-3.0.3/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/app.py` & `yambs-3.0.3/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/commands/all.py` & `yambs-3.0.3/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/commands/common.py` & `yambs-3.0.3/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/commands/compile_config.py` & `yambs-3.0.3/yambs/commands/compile_config.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/commands/dist.py` & `yambs-3.0.3/yambs/commands/dist.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/commands/download.py` & `yambs-3.0.3/yambs/commands/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 
 # internal
 from yambs.dependency.github import GithubDependency, default_filt
 
+DEFAULT_PATTERN = ".*"
+
 
 def download_cmd(args: _Namespace) -> int:
     """Execute the download command."""
 
     dep = GithubDependency(args.owner, args.repo)
 
     # Download and extract things.
+    args.output.mkdir(parents=True, exist_ok=True)
     dep.download_release_assets(
-        default_filt(args.output, pattern=args.pattern)
+        default_filt(args.output.joinpath(args.repo), pattern=args.pattern),
+        strict=args.pattern == DEFAULT_PATTERN,
     )
 
     return 0
 
 
 def add_download_cmd(parser: _ArgumentParser) -> _CommandFunction:
     """Add download-command arguments to its parser."""
@@ -42,21 +46,21 @@
         default="toolchains",
         help="repository name (default: '%(default)s')",
     )
     parser.add_argument(
         "-O",
         "--output",
         type=Path,
-        default=Path("toolchains"),
+        default=Path(),
         help="output directory (default: '%(default)s')",
     )
     parser.add_argument(
         "-p",
         "--pattern",
-        default=".*",
+        default=DEFAULT_PATTERN,
         help=(
             "a pattern to use to select project "
             "specifications filtered by name"
         ),
     )
 
     return download_cmd
```

### Comparing `yambs-3.0.2/yambs/commands/gen.py` & `yambs-3.0.3/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/commands/native.py` & `yambs-3.0.3/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/commands/uf2conv.py` & `yambs-3.0.3/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/config/__init__.py` & `yambs-3.0.3/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/config/board.py` & `yambs-3.0.3/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/config/common.py` & `yambs-3.0.3/yambs/config/common.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/config/native.py` & `yambs-3.0.3/yambs/config/native.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/includes/chips.yaml` & `yambs-3.0.3/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/includes/infineon.yaml` & `yambs-3.0.3/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/includes/microchip.yaml` & `yambs-3.0.3/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/native.yaml` & `yambs-3.0.3/yambs/data/native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/schemas/Chip.yaml` & `yambs-3.0.3/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/schemas/Config.yaml` & `yambs-3.0.3/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/schemas/Native.yaml` & `yambs-3.0.3/yambs/data/schemas/Native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/schemas/config_common.yaml` & `yambs-3.0.3/yambs/data/schemas/config_common.yaml`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/templates/native_rules.ninja.j2` & `yambs-3.0.3/yambs/data/templates/native_rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/templates/regenerate.ninja.j2` & `yambs-3.0.3/yambs/data/templates/regenerate.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/templates/rules.ninja.j2` & `yambs-3.0.3/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/templates/variant.ninja.j2` & `yambs-3.0.3/yambs/data/templates/variant.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/data/uf2families.json` & `yambs-3.0.3/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/dependency/config.py` & `yambs-3.0.3/yambs/dependency/config.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/dependency/github.py` & `yambs-3.0.3/yambs/dependency/github.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,17 @@
             result = output.joinpath(name)
 
         return result
 
     return filt
 
 
-def ensure_extracted(path: Path, logger: LoggerType = None) -> None:
+def ensure_extracted(
+    path: Path, strict: bool = True, logger: LoggerType = None
+) -> None:
     """Ensure that all archive files in a directory are extracted."""
 
     for item in path.iterdir():
         ext = FileExtension.from_path(item)
         if ext is not None and ext.is_archive() and item.is_file():
             dest = item.parent.joinpath(item.name.replace(f".{ext}", ""))
             if not dest.is_dir():
@@ -71,15 +73,15 @@
                 if logger is not None:
                     logger.info(
                         "Extracted '%s' in %s.",
                         dest,
                         nano_str(result[1], is_time=True),
                     )
 
-                assert dest.is_dir(), dest
+                assert not strict or dest.is_dir(), dest
 
 
 class GithubDependency(LoggerMixin):
     """A class for managing GitHub dependencies."""
 
     def __init__(
         self,
@@ -107,18 +109,20 @@
         # Collect URLs for release content.
         self.download_urls: Dict[str, str] = {
             item["name"]: item["browser_download_url"]
             for item in self.data["assets"]
         }
 
     def download_release_assets(
-        self, filt: AssetFilter, extract: bool = True
+        self, filt: AssetFilter, extract: bool = True, strict: bool = True
     ) -> None:
         """Ensure release assets are downloaded."""
 
         for asset in self.data["assets"]:
             dest = filt(asset)
             if dest is not None:
                 download_file_if_missing(asset["browser_download_url"], dest)
 
                 if extract:
-                    ensure_extracted(dest.parent, logger=self.logger)
+                    ensure_extracted(
+                        dest.parent, strict=strict, logger=self.logger
+                    )
```

### Comparing `yambs-3.0.2/yambs/dependency/handlers/types.py` & `yambs-3.0.3/yambs/dependency/handlers/types.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/dependency/handlers/yambs/__init__.py` & `yambs-3.0.3/yambs/dependency/handlers/yambs/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/dependency/handlers/yambs/config.py` & `yambs-3.0.3/yambs/dependency/handlers/yambs/config.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/dependency/handlers/yambs/github.py` & `yambs-3.0.3/yambs/dependency/handlers/yambs/github.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/dependency/manager.py` & `yambs-3.0.3/yambs/dependency/manager.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/dist/__init__.py` & `yambs-3.0.3/yambs/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/entry.py` & `yambs-3.0.3/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/environment/__init__.py` & `yambs-3.0.3/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/environment/native.py` & `yambs-3.0.3/yambs/environment/native.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/generate/__init__.py` & `yambs-3.0.3/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/generate/architectures.py` & `yambs-3.0.3/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/generate/boards.py` & `yambs-3.0.3/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/generate/chips.py` & `yambs-3.0.3/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/generate/common.py` & `yambs-3.0.3/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/generate/ninja/__init__.py` & `yambs-3.0.3/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/generate/ninja/format.py` & `yambs-3.0.3/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/generate/toolchains.py` & `yambs-3.0.3/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/generate/variants.py` & `yambs-3.0.3/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/github/__init__.py` & `yambs-3.0.3/yambs/github/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/paths.py` & `yambs-3.0.3/yambs/paths.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/schemas.py` & `yambs-3.0.3/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/translation/__init__.py` & `yambs-3.0.3/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs/uf2/__init__.py` & `yambs-3.0.3/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-3.0.2/yambs.egg-info/PKG-INFO` & `yambs-3.0.3/yambs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 3.0.2
+Version: 3.0.3
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: datazen
 Requires-Dist: rcmpy>=1.5.0
 Requires-Dist: requests
 Requires-Dist: vcorelib>=2.4.2
-Requires-Dist: datazen
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -37,19 +37,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: types-requests; extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=72271a00d30bf23159c35289b5ff7a00
+    hash=934a1cb8be74864c521e3c3d3875e01d
     =====================================
 -->
 
-# yambs ([3.0.2](https://pypi.org/project/yambs/))
+# yambs ([3.0.3](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
 
@@ -251,15 +251,15 @@
 
 options:
   -h, --help            show this help message and exit
   -o OWNER, --owner OWNER
                         repository owner (default: 'vkottler')
   -r REPO, --repo REPO  repository name (default: 'toolchains')
   -O OUTPUT, --output OUTPUT
-                        output directory (default: 'toolchains')
+                        output directory (default: '.')
   -p PATTERN, --pattern PATTERN
                         a pattern to use to select project specifications
                         filtered by name
 
 ```
 
 ### `gen`
```

### Comparing `yambs-3.0.2/yambs.egg-info/SOURCES.txt` & `yambs-3.0.3/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

