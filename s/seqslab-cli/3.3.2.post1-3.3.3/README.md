# Comparing `tmp/seqslab-cli-3.3.2.post1.tar.gz` & `tmp/seqslab-cli-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslab-cli-3.3.2.post1.tar", last modified: Fri Mar  8 00:30:44 2024, max compression
+gzip compressed data, was "seqslab-cli-3.3.3.tar", last modified: Mon May 20 10:11:24 2024, max compression
```

## Comparing `seqslab-cli-3.3.2.post1.tar` & `seqslab-cli-3.3.3.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.141300 seqslab-cli-3.3.2.post1/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-03-08 00:30:44.141300 seqslab-cli-3.3.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.121300 seqslab-cli-3.3.2.post1/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.125300 seqslab-cli-3.3.2.post1/python/seqslab/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.125300 seqslab-cli-3.3.2.post1/python/seqslab/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/auth/azuread.py
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/auth/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.125300 seqslab-cli-3.3.2.post1/python/seqslab/drs/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.125300 seqslab-cli-3.3.2.post1/python/seqslab/drs/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15620 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/api/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    17006 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/api/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/api/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    49915 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.125300 seqslab-cli-3.3.2.post1/python/seqslab/drs/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/internal/aiocopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/drs/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28712 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/storage/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/drs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/utils/atgxmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/utils/biomimetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/drs/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/organization/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/organization/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/organization/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/organization/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/organization/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/role/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/role/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/role/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/role/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/role/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/role/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/role/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/role/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/role/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/runsheet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/runsheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/runsheet/runsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (127)    56711 2024-03-08 00:30:31.000000 seqslab-cli-3.3.2.post1/python/seqslab/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-08 00:30:31.000000 seqslab-cli-3.3.2.post1/python/seqslab/sample_sheet/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-08 00:30:31.000000 seqslab-cli-3.3.2.post1/python/seqslab/sample_sheet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.129300 seqslab-cli-3.3.2.post1/python/seqslab/scr/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/scr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/scr/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.133300 seqslab-cli-3.3.2.post1/python/seqslab/scr/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/scr/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/scr/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.133300 seqslab-cli-3.3.2.post1/python/seqslab/scr/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/scr/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/scr/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/scr/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/session_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/statusbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.133300 seqslab-cli-3.3.2.post1/python/seqslab/trs/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23164 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.133300 seqslab-cli-3.3.2.post1/python/seqslab/trs/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.133300 seqslab-cli-3.3.2.post1/python/seqslab/trs/register/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/register/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/register/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/register/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/register/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.133300 seqslab-cli-3.3.2.post1/python/seqslab/trs/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/resource/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.133300 seqslab-cli-3.3.2.post1/python/seqslab/trs/template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/template/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/trs/template/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/usage_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.133300 seqslab-cli-3.3.2.post1/python/seqslab/user/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/user/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.133300 seqslab-cli-3.3.2.post1/python/seqslab/user/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/user/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/user/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.137300 seqslab-cli-3.3.2.post1/python/seqslab/user/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/user/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/user/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/user/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.137300 seqslab-cli-3.3.2.post1/python/seqslab/wes/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25096 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.137300 seqslab-cli-3.3.2.post1/python/seqslab/wes/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/internal/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.137300 seqslab-cli-3.3.2.post1/python/seqslab/wes/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12057 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.137300 seqslab-cli-3.3.2.post1/python/seqslab/wes/template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/template/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/wes/template/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.137300 seqslab-cli-3.3.2.post1/python/seqslab/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/workspace/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.137300 seqslab-cli-3.3.2.post1/python/seqslab/workspace/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/workspace/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/workspace/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.137300 seqslab-cli-3.3.2.post1/python/seqslab/workspace/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/workspace/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/workspace/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/python/seqslab/workspace/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 00:30:44.141300 seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-03-08 00:30:43.000000 seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-03-08 00:30:44.000000 seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 00:30:43.000000 seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-08 00:30:43.000000 seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-08 00:30:43.000000 seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-08 00:30:43.000000 seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 00:30:43.000000 seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-08 00:30:44.141300 seqslab-cli-3.3.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-08 00:30:30.000000 seqslab-cli-3.3.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.447486 seqslab-cli-3.3.3/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.447486 seqslab-cli-3.3.3/python/seqslab/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/auth/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/auth/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17051 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49945 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/internal/aiocopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28712 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/storage/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/utils/atgxmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/utils/biomimetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/organization/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/organization/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/organization/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/organization/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/role/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/role/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/role/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/runsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/runsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/runsheet/runsheet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (127)    56711 2024-05-20 10:11:11.000000 seqslab-cli-3.3.3/python/seqslab/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 10:11:11.000000 seqslab-cli-3.3.3/python/seqslab/sample_sheet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-20 10:11:11.000000 seqslab-cli-3.3.3/python/seqslab/sample_sheet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/scr/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/scr/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/scr/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/session_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/statusbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/trs/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23164 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/trs/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/trs/register/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/trs/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/resource/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/trs/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/usage_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/user/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/user/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/wes/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27990 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/wes/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/internal/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/wes/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/wes/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/template/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/python/seqslab/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/python/seqslab/workspace/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/python/seqslab/workspace/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-20 10:11:24.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/setup.py
```

### Comparing `seqslab-cli-3.3.2.post1/LICENSE` & `seqslab-cli-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/PKG-INFO` & `seqslab-cli-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-cli
-Version: 3.3.2.post1
+Version: 3.3.3
 Summary: Atgenomix SeqsLab Command Line Tool
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang
 Author-email: allen.chang@atgenomix.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslab-cli Version: 3.3.2.post1 Summary: Atgenomix
+Metadata-Version: 2.1 Name: seqslab-cli Version: 3.3.3 Summary: Atgenomix
 SeqsLab Command Line Tool Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang Author-email: allen.chang@atgenomix.com License: Apache
 License, Version 2.0 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli Description:
 This package provides a unified command line interface to Atgenomix SeqsLab, a
 cloud-native biomedical informatics (BioMed IT) platform. Table of Contents
    1. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
```

### Comparing `seqslab-cli-3.3.2.post1/README.md` & `seqslab-cli-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/__init__.py` & `seqslab-cli-3.3.3/python/seqslab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 """
 
 name = "seqslab"
 
 __all__ = []
 
 
-__version__ = "3.3.2.post1"
+__version__ = "3.3.3"
 
 LOGGING = {"DIR_PATH": "/var/log/seqslab"}
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/auth/azuread.py` & `seqslab-cli-3.3.3/python/seqslab/auth/azuread.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/auth/commands.py` & `seqslab-cli-3.3.3/python/seqslab/auth/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/cli.py` & `seqslab-cli-3.3.3/python/seqslab/cli.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/context.py` & `seqslab-cli-3.3.3/python/seqslab/context.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/api/azure.py` & `seqslab-cli-3.3.3/python/seqslab/drs/api/azure.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datetime import datetime
 from functools import lru_cache
 from typing import List
 
 import requests
 from nubia import context
 from seqslab.auth.commands import BaseAuth
+from seqslab.drs.storage.azure import BlobStorage
 from seqslab.drs.utils.biomimetype import get_mime_type
 from tenacity import retry, stop_after_attempt, wait_fixed
 from termcolor import cprint
 from yarl import URL
 
 from .base import DRSregister
 
@@ -392,7 +393,18 @@
                             break
             else:
                 raise ValueError(
                     f"Index {index}, does not have access_url in access_methods."
                 )
 
         return dsts_list
+
+    def common_root(self, dsts: List[URL], **kwargs) -> str:
+        root_dst = super().common_root(dsts)
+        blob_root = BlobStorage(kwargs.get("workspace")).get_token(path=None)[
+            "register_url"
+        ]
+        if URL(root_dst).path == URL(blob_root).path:
+            raise ValueError(
+                "access_url pointing to cloud storage root path is not allowed"
+            )
+        return root_dst
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/api/base.py` & `seqslab-cli-3.3.3/python/seqslab/drs/api/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             folder_stdin["access_methods"] = json.loads(kwargs.get("access_methods"))
         else:
             folder_stdin["access_methods"].clear()
             for i, dsts in enumerate(dsts_list):
                 folder_stdin["access_methods"].append(access_method_infos[i])
                 folder_stdin["access_methods"][i]["access_url"][
                     "url"
-                ] = self.common_root(dsts=dsts)
+                ] = self.common_root(dsts=dsts, workspace=kwargs.get("workspace"))
 
         folder_stdin["name"] = kwargs.get(
             "name",
             os.path.basename(
                 str(folder_stdin["access_methods"][0]["access_url"]["url"]).strip("/")
             ),
         )
@@ -356,15 +356,15 @@
 
     @staticmethod
     def sum_fsize(sizes: List[int]) -> int:
         if not all(sizes) or not sizes:
             raise ValueError("Make sure all the sizes are filled.")
         return sum(sizes)
 
-    def common_root(self, dsts: List[URL]) -> str:
+    def common_root(self, dsts: List[URL], **kwargs) -> str:
         """
         e.g. http://user:password@example.com:8042/over/there?name=ferret#nose
         URL.scheme: http
         URL.user: user
         URL.password: password
         URL.host: example.com
         URL.port: 8042
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/api/common.py` & `seqslab-cli-3.3.3/python/seqslab/drs/api/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/api/template.py` & `seqslab-cli-3.3.3/python/seqslab/drs/api/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/commands.py` & `seqslab-cli-3.3.3/python/seqslab/drs/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         positional=False,
         description="Specify the source directory, file path, or DRS URL (required).",
     )
     @argument(
         "dst",
         type=str,
         positional=False,
-        description="Specify the destination directory, file path, or DRS URL (optional, default =' /'). ",
+        description="Specify the destination directory, file path, or DRS URL (optional, default ='MyDir/'). ",
     )
     @argument(
         "recursive",
         type=bool,
         positional=False,
         description="Copy an entire directory tree (optional, default = False).",
         aliases=["r"],
@@ -219,15 +219,15 @@
         description="Whether to run in non-interactive mode, i.e. without prompt (default = False).",
         aliases=["ni"],
     )
     def upload(
         self,
         workspace: str,
         src: str,
-        dst: str = "/",
+        dst: str = "MyDir/",
         recursive: bool = False,
         output: str = "json",
         concurrency: int = 0,
         multiprocessing: int = 1,
         chunk_size: str = "8",
         expiry_time: str = None,
         non_interactive: bool = False,
@@ -702,15 +702,15 @@
     @exception_handler
     def _register_blob(
         drs_type: str, stdin: bool, workspace: str, **kwargs
     ) -> List[dict]:
         backend = drs_register().load_register(workspace)
         if stdin:
             payloads = backend.create_payload(
-                stdin=BaseDatahub._stdin(), type=drs_type, **kwargs
+                stdin=BaseDatahub._stdin(), type=drs_type, workspace=workspace, **kwargs
             )
         else:
             if not kwargs["is_integrity"]:
                 checksums = []
             else:
                 checksums = [
                     {
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/internal/aiocopy.py` & `seqslab-cli-3.3.3/python/seqslab/drs/internal/aiocopy.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/internal/common.py` & `seqslab-cli-3.3.3/python/seqslab/drs/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/internal/utils.py` & `seqslab-cli-3.3.3/python/seqslab/drs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/storage/azure.py` & `seqslab-cli-3.3.3/python/seqslab/drs/storage/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/storage/base.py` & `seqslab-cli-3.3.3/python/seqslab/drs/storage/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/utils/atgxmetadata.py` & `seqslab-cli-3.3.3/python/seqslab/drs/utils/atgxmetadata.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/utils/biomimetype.py` & `seqslab-cli-3.3.3/python/seqslab/drs/utils/biomimetype.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/drs/utils/progressbar.py` & `seqslab-cli-3.3.3/python/seqslab/drs/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/exceptions.py` & `seqslab-cli-3.3.3/python/seqslab/exceptions.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/organization/commands.py` & `seqslab-cli-3.3.3/python/seqslab/organization/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/organization/resource/base.py` & `seqslab-cli-3.3.3/python/seqslab/organization/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/plugin.py` & `seqslab-cli-3.3.3/python/seqslab/plugin.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/role/commands.py` & `seqslab-cli-3.3.3/python/seqslab/role/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/role/internal/common.py` & `seqslab-cli-3.3.3/python/seqslab/role/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/role/resource/azure.py` & `seqslab-cli-3.3.3/python/seqslab/role/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/role/resource/base.py` & `seqslab-cli-3.3.3/python/seqslab/role/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/runsheet/runsheet.py` & `seqslab-cli-3.3.3/python/seqslab/runsheet/runsheet.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/sample_sheet/__init__.py` & `seqslab-cli-3.3.3/python/seqslab/sample_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/sample_sheet/util.py` & `seqslab-cli-3.3.3/python/seqslab/sample_sheet/util.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/scr/commands.py` & `seqslab-cli-3.3.3/python/seqslab/scr/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/scr/internal/common.py` & `seqslab-cli-3.3.3/python/seqslab/scr/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/scr/resource/azure.py` & `seqslab-cli-3.3.3/python/seqslab/scr/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/scr/resource/base.py` & `seqslab-cli-3.3.3/python/seqslab/scr/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/settings.py` & `seqslab-cli-3.3.3/python/seqslab/settings.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/statusbar.py` & `seqslab-cli-3.3.3/python/seqslab/statusbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/commands.py` & `seqslab-cli-3.3.3/python/seqslab/trs/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/internal/utils.py` & `seqslab-cli-3.3.3/python/seqslab/trs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/register/azure.py` & `seqslab-cli-3.3.3/python/seqslab/trs/register/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/register/base.py` & `seqslab-cli-3.3.3/python/seqslab/trs/register/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/register/common.py` & `seqslab-cli-3.3.3/python/seqslab/trs/register/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/register/template.py` & `seqslab-cli-3.3.3/python/seqslab/trs/register/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/resource/azure.py` & `seqslab-cli-3.3.3/python/seqslab/trs/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/resource/base.py` & `seqslab-cli-3.3.3/python/seqslab/trs/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/resource/common.py` & `seqslab-cli-3.3.3/python/seqslab/trs/resource/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/template/base.py` & `seqslab-cli-3.3.3/python/seqslab/trs/template/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Standard Library
+import re
 from typing import List
 
 import pydot
 from seqslab.wes.commands import BaseJobs
 
 from .template import get_template
 
@@ -17,15 +18,15 @@
         oconfig: List,
         **kwargs,
     ) -> dict:
         parameter = BaseJobs.parameter(
             primary_descriptor=primary_descriptor, zip_file=zip_file
         )
         workflow = self.desc_template(parameter)
-        calls = self.call_template(parameter)
+        calls = self.workflow_call_template(parameter)
         inputs_connections = self.inputs_connections(
             parameter=parameter, inputs_json=inputs_json
         )
         iconfig = self.import_conf(parameter.get("i_configs"), iconfig)
         oconfig = self.import_conf(parameter.get("o_configs"), oconfig)
         return get_template().create(
             parameters=parameter,
@@ -54,14 +55,40 @@
 
         for subgraph in graph.get_subgraphs():
             for node in subgraph.get_nodes():
                 if node.get_name().startswith("CALL_"):
                     calls.add(node.get_name().replace("CALL_", ""))
         return calls
 
+    def workflow_call_template(self, parameter: dict) -> list:
+        # adding main workflow
+        runtime_cell_select = [
+            pydot.graph_from_dot_data(
+                TrsCreateTemplate.dot_cleaning(parameter["graph"])
+            )[0].get_name()
+        ]
+
+        # parsing workflow>call information from graph string
+        graphRex = re.compile(r'graph\s\w+|}|label="call\s\w+', re.IGNORECASE)
+        wnames = []
+        matches = graphRex.findall(parameter.get("graph"))
+        if matches:
+            for e in matches:
+                if e.startswith("graph "):
+                    wnames.append(e.split(" ")[1].replace("cluster_", ""))
+                elif e.startswith("}"):
+                    wnames.pop()
+                elif e.startswith("label="):
+                    call = e.replace('label="', "").strip('"')
+                    if call.lower().startswith("call"):
+                        runtime_cell_select.append(
+                            "" + wnames[-1] + ">" + call.replace("call ", "")
+                        )
+        return runtime_cell_select
+
     def call_template(self, parameter: dict) -> list:
         calls = [
             pydot.graph_from_dot_data(
                 TrsCreateTemplate.dot_cleaning(parameter["graph"])
             )[0].get_name()
         ]
         for workflow in [
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/trs/template/template.py` & `seqslab-cli-3.3.3/python/seqslab/trs/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/usage_logger.py` & `seqslab-cli-3.3.3/python/seqslab/usage_logger.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/user/commands.py` & `seqslab-cli-3.3.3/python/seqslab/user/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/user/internal/common.py` & `seqslab-cli-3.3.3/python/seqslab/user/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/user/resource/azure.py` & `seqslab-cli-3.3.3/python/seqslab/user/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/user/resource/base.py` & `seqslab-cli-3.3.3/python/seqslab/user/resource/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,11 +108,13 @@
         return r
 
     @exception_handler
     @retry(stop=stop_after_attempt(3), wait=wait_fixed(2), reraise=True)
     def is_global_admin(self, **kwargs) -> bool:
         token = BaseAuth.get_token()
         response = self.get_user(token.get("attrs").get("user_id"))
-        if "Global administrator" in response.get("roles"):
+        if "Global administrator" in [
+            item.get("name") for item in response.get("roles")
+        ]:
             return True
 
         return False
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/wes/commands.py` & `seqslab-cli-3.3.3/python/seqslab/wes/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -454,19 +454,19 @@
         description="Specify the execs.json needed to create a WES request.  If not given, the command will "
         "get the execs.json from the TRS object specified by the workflow_url "
         "(optional, default = None).",
     )
     @argument(
         "runtimes",
         type=str,
-        description="Key:value pairs indicating the workflow name -> SeqsLab supported runtime_options names. "
-        "Multiple configuration pairs can be provided using ':' as separator, "
-        "e.g. main=m4-cluster:subworkflow=m4-8xcluster "
-        "(optional, default = None, which indicates running the whole workflow.wdl using m4-cluster for "
-        "a single node cluster on the Azure backend).",
+        description="String of key-value pairs using : as a separator, indicating the execution runtimes for each task "
+        "or workflow defined in workflow-url. For example, Main=m4-cluster:Main>Fq2Bam=m4-8xcluster. To "
+        "list tasks/workflows for a given workflow, use the execs command. To find available runtime "
+        "options, use the request runtimes_options command. (Optional, defaults to None, which runs the "
+        "entire workflow using m4-cluster.)",
     )
     @argument(
         "integrity",
         type=bool,
         description="Specify whether to enable data and runtime integrity check for the workflow engine "
         "(optional, default = False).",
     )
@@ -657,14 +657,109 @@
                 cprint(json.dumps(result, indent=4), "yellow")
         except requests.HTTPError:
             cprint(f"given run_id {run_id} is not valid.", "red")
             return -1
 
         return 0
 
+    @command(aliases=["rt"])
+    @argument(
+        "page",
+        type=int,
+        positional=False,
+        description="Specify the page number in the set of paginated records (optional, default = 1).",
+    )
+    @argument(
+        "page_size",
+        type=int,
+        positional=False,
+        description="Specify the number of records to return in each page (optional, default = 10).",
+    )
+    @command
+    @argument(
+        "output",
+        type=str,
+        positional=False,
+        description="Specify the output format of the stdout file (optional, default = json).",
+        choices=["json", "table"],
+    )
+    def runtime_options(
+        self, workspace: str, page: int = 1, page_size: int = 10, output="json"
+    ) -> int:
+        """
+        List registered cluster runtimes settings.
+        """
+        resource = get_factory().load_resource(workspace)
+        r = resource.list_runtime_options(page=page, page_size=page_size)
+
+        if isinstance(r, int):
+            return r
+
+        self._stdout(r["results"], output)
+        return 0
+
+    @command(aliases=["op"])
+    @argument(
+        "page",
+        type=int,
+        positional=False,
+        description="Specify the page number in the set of paginated records (optional, default = 1).",
+    )
+    @argument(
+        "page_size",
+        type=int,
+        positional=False,
+        description="Specify the number of records to return in each page (optional, default = 10).",
+    )
+    @command
+    @argument(
+        "output",
+        type=str,
+        positional=False,
+        description="Specify the output format of the stdout file (optional, default = json).",
+        choices=["json", "table"],
+    )
+    def operator_pipelines(
+        self, workspace: str, page: int = 1, page_size: int = 10, output="json"
+    ) -> int:
+        """
+        List registered operator pipelines.
+        """
+        resource = get_factory().load_resource(workspace)
+        r = resource.list_runtime_options(page=page, page_size=page_size)
+
+        if isinstance(r, int):
+            return r
+
+        self._stdout(r["results"], output)
+        return 0
+
+    @staticmethod
+    def _stdout(results, output: str) -> int:
+        # Standard Library
+        import csv
+        from io import StringIO
+
+        from tabulate import tabulate
+
+        """
+            stdout:: TODO: support different format ex: json, tsv, table
+        """
+        if output == "json":
+            cprint(json.dumps(results, indent=4))
+        elif output == "table":
+            table_header = list(results[0].keys())
+            table_datas = [result.values() for result in results]
+            cprint(
+                tabulate(
+                    tabular_data=table_datas, headers=table_header, tablefmt="pipe"
+                )
+            )
+        return 0
+
 
 @command
 class Jobs(BaseJobs):
     """Workflow execution commands"""
 
     @command
     @argument(
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/wes/internal/common.py` & `seqslab-cli-3.3.3/python/seqslab/wes/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/wes/internal/parameters.py` & `seqslab-cli-3.3.3/python/seqslab/wes/internal/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,21 +226,41 @@
     resource = get_factory().load_resource(workspace)
     clusters = []
     for k, v in rt_dict.items():
         if k not in calls:
             raise RuntimeError(
                 f"given call name {k} not in TRS registered call name list {calls}!"
             )
-        clusters.append(
-            WorkflowBackendParamsClusterTemplate(
-                run_time=resource.get_runtime_setting(v),
-                workflow_name=k,
-                kernel_version=kernel_version,
+
+        # general workflow>call handling
+        ids = k.split(">")
+        if len(ids) == 2:
+            clusters.append(
+                WorkflowBackendParamsClusterTemplate(
+                    run_time=resource.get_runtime_setting(v),
+                    call_name=ids[1],
+                    workflow_name=ids[0],
+                    kernel_version=kernel_version,
+                )
             )
-        )
+        else:
+            # main workflow name
+            if k == primary_workflow_name:
+                clusters.append(
+                    WorkflowBackendParamsClusterTemplate(
+                        run_time=resource.get_runtime_setting(v),
+                        call_name=k,
+                        kernel_version=kernel_version,
+                    )
+                )
+            else:
+                # raise exception for incorrect format of k
+                raise RuntimeError(
+                    f"given identifier {k} does not in format of in TRS registered call name list {calls}!"
+                )
 
     bk_template = WorkflowBackendParamsTemplate(
         graph=execs.get("graph"),
         clusters=clusters,
         workspace=workspace,
         integrity=integrity,
         trust=trust,
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/wes/resource/azure.py` & `seqslab-cli-3.3.3/python/seqslab/wes/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/wes/resource/base.py` & `seqslab-cli-3.3.3/python/seqslab/wes/resource/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         f"https://{API_HOSTNAME}/wes/{__version__}/service-info/workspaces/{{"
         f"name}}/resources/?backend={{backend}}"
     )
     WES_RUNS_URL = f"{WES_BASE_URL}runs/?backend={{backend}}"
     WES_RUNS_DRY_URL = f"{WES_BASE_URL}runs/dryrun/?backend={{backend}}"
     WES_RUNS_FILE_URL = f"{WES_BASE_URL}runs/{{id}}/files/?backend={{backend}}"
     WES_RUNS_STATUS_URL = f"{WES_BASE_URL}runs/{{id}}/status/?backend={{backend}}"
+    WES_RUNTIME_OPTIONS_BASE_URL = f"{WES_BASE_URL}runtime-options/"
+    WES_OPERATOR_PIPELINES_BASE_URL = f"{WES_BASE_URL}operator-pipelines/"
     WES_RUNTIME_OPTIONS_URL = (
         f"{WES_BASE_URL}runtime-options/{{name}}?backend={{backend}}"
     )
 
     class Response(NamedTuple):
         status: int
         headers: CIMultiDictProxy[str]
@@ -306,7 +308,39 @@
         with requests.delete(
             url=f"{self.WES_BASE_URL}runs/{run_id}/cancel",
             headers={"Authorization": f"Bearer {token}"},
         ) as response:
             if response.status_code not in [requests.codes.ok]:
                 raise requests.HTTPError(response.text)
             return json.loads(response.content)
+
+    def list_runtime_options(self, page=1, page_size=10):
+        try:
+            token = BaseAuth.get_token().get("tokens").get("access")
+            with requests.get(
+                url=f"{self.WES_RUNTIME_OPTIONS_BASE_URL}?page={page}&page_size={page_size}",
+                headers={"Authorization": f"Bearer {token}"},
+            ) as response:
+                if response.status_code not in [requests.codes.ok]:
+                    raise requests.HTTPError(
+                        f"{response.status_code}: {repr(response.text)}"
+                    )
+        except Exception as err:
+            print(err)
+            raise err
+        return response.json()
+
+    def list_operator_pipelines(self, page=1, page_size=10):
+        try:
+            token = BaseAuth.get_token().get("tokens").get("access")
+            with requests.get(
+                url=f"{self.WES_OPERATOR_PIPELINES_BASE_URL}?page={page}&page_size={page_size}",
+                headers={"Authorization": f"Bearer {token}"},
+            ) as response:
+                if response.status_code not in [requests.codes.ok]:
+                    raise requests.HTTPError(
+                        f"{response.status_code}: {repr(response.text)}"
+                    )
+        except Exception as err:
+            print(err)
+            raise err
+        return response.json()
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/wes/template/base.py` & `seqslab-cli-3.3.3/python/seqslab/wes/template/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,16 @@
                     "description": "demo operator"
                 }
             }
         """
         tasks = {}
         pl_keys = [pipeline["id"] for pipeline in ex_template["operator_pipelines"]]
         for k, v in dict(ex_template["i_configs"], **ex_template["o_configs"]).items():
+            if not v:
+                continue
             assert (
                 v in pl_keys
             ), f"given operator pipeline ID {v} for FQN {k} not in operator pipeline list from execs: {pl_keys}"
             for pipeline in ex_template["operator_pipelines"]:
                 if pipeline["id"] == v:
                     tasks[k] = {
                         "id": v,
@@ -109,15 +111,18 @@
     }
     if graph:
         ret.update({"graph": graph})
     return ret
 
 
 def WorkflowBackendParamsClusterTemplate(
-    run_time: dict, workflow_name: str, kernel_version: str
+    run_time: dict, call_name: str, kernel_version: str, workflow_name: str = ""
 ) -> dict:
     if kernel_version:
         opts = run_time["options"]
         opts.append(f"seqslab.kernel.version {kernel_version}")
         run_time.update({"options": opts})
-    run_time.update({"call": workflow_name})
+    if workflow_name:
+        run_time.update({"call": call_name, "workflow": workflow_name})
+    else:
+        run_time.update({"call": call_name})
     return run_time
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/wes/template/template.py` & `seqslab-cli-3.3.3/python/seqslab/wes/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/workspace/commands.py` & `seqslab-cli-3.3.3/python/seqslab/workspace/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/workspace/internal/common.py` & `seqslab-cli-3.3.3/python/seqslab/workspace/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/workspace/resource/azure.py` & `seqslab-cli-3.3.3/python/seqslab/workspace/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab/workspace/resource/base.py` & `seqslab-cli-3.3.3/python/seqslab/workspace/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/PKG-INFO` & `seqslab-cli-3.3.3/python/seqslab_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-cli
-Version: 3.3.2.post1
+Version: 3.3.3
 Summary: Atgenomix SeqsLab Command Line Tool
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang
 Author-email: allen.chang@atgenomix.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslab-cli Version: 3.3.2.post1 Summary: Atgenomix
+Metadata-Version: 2.1 Name: seqslab-cli Version: 3.3.3 Summary: Atgenomix
 SeqsLab Command Line Tool Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang Author-email: allen.chang@atgenomix.com License: Apache
 License, Version 2.0 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli Description:
 This package provides a unified command line interface to Atgenomix SeqsLab, a
 cloud-native biomedical informatics (BioMed IT) platform. Table of Contents
    1. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
```

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/SOURCES.txt` & `seqslab-cli-3.3.3/python/seqslab_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.2.post1/python/seqslab_cli.egg-info/requires.txt` & `seqslab-cli-3.3.3/python/seqslab_cli.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 pip>=22.0.4
 click==8.1.7
 tabulate==0.9.0
 terminaltables==3.1.10
-cryptography==41.0.7
+cryptography==42.0.6
 jeepney==0.8.0
 secretstorage==3.3.3
 dbus-python==1.2.16
 keyring==24.3.0
 numba==0.58.1
 python-nubia==0.2b5
 msal==1.26.0
 tenacity==8.2.3
 aiofiles==23.2.1
-aiohttp[speedups]==3.9.1
+aiohttp[speedups]==3.9.5
 aioretry==5.0.2
 uvloop==0.19.0
 arrow==1.3.0
 yarl==1.4.2
 requests-toolbelt==1.0.0
 PyJWT==2.8.0
 django-environ==0.11.2
 validators==0.22.0
 pydot==2.0.0
-orjson==3.9.10
-pydantic~=2.5.3
+orjson==3.10.3
+pydantic~=2.7.1
 aiohttp_retry==2.8.3
 requests~=2.31.0
-setuptools~=69.0.3
+setuptools~=69.5.1
 jsonpath-ng==1.6.0
```

### Comparing `seqslab-cli-3.3.2.post1/setup.py` & `seqslab-cli-3.3.3/setup.py`

 * *Files identical despite different names*

