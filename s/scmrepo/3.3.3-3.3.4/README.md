# Comparing `tmp/scmrepo-3.3.3.tar.gz` & `tmp/scmrepo-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmrepo-3.3.3.tar", last modified: Sun May 12 20:13:35 2024, max compression
+gzip compressed data, was "scmrepo-3.3.4.tar", last modified: Mon May 20 02:45:45 2024, max compression
```

## Comparing `scmrepo-3.3.3.tar` & `scmrepo-3.3.4.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.581308 scmrepo-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.569308 scmrepo-3.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.569308 scmrepo-3.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-12 20:13:21.000000 scmrepo-3.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-12 20:13:21.000000 scmrepo-3.3.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-12 20:13:21.000000 scmrepo-3.3.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-12 20:13:21.000000 scmrepo-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-12 20:13:35.581308 scmrepo-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-12 20:13:21.000000 scmrepo-3.3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-12 20:13:21.000000 scmrepo-3.3.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-12 20:13:21.000000 scmrepo-3.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:13:35.581308 scmrepo-3.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.565307 scmrepo-3.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.569308 scmrepo-3.3.3/src/scmrepo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/
--rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/
--rw-r--r--   0 runner    (1001) docker     (127)    34740 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25350 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/gitpython.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/
--rw-r--r--   0 runner    (1001) docker     (127)    37035 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.573308 scmrepo-3.3.3/src/scmrepo/git/lfs/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/smudge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/lfs/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/git/stash.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/noscm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-12 20:13:21.000000 scmrepo-3.3.3/src/scmrepo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.577308 scmrepo-3.3.3/src/scmrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 20:13:35.000000 scmrepo-3.3.3/src/scmrepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.577308 scmrepo-3.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.577308 scmrepo-3.3.3/tests/git-init/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_dulwich.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    36426 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_lfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_noscm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_pygit2.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_scmrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/user.key
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/user.key.pub
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:35.577308 scmrepo-3.3.3/tests/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-12 20:13:21.000000 scmrepo-3.3.3/tests/vendor/test_paramiko_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.547860 scmrepo-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 02:45:31.000000 scmrepo-3.3.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-20 02:45:31.000000 scmrepo-3.3.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 02:45:31.000000 scmrepo-3.3.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.535859 scmrepo-3.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 02:45:31.000000 scmrepo-3.3.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.535859 scmrepo-3.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-20 02:45:31.000000 scmrepo-3.3.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-20 02:45:31.000000 scmrepo-3.3.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-20 02:45:31.000000 scmrepo-3.3.4/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-20 02:45:31.000000 scmrepo-3.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-20 02:45:31.000000 scmrepo-3.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-20 02:45:31.000000 scmrepo-3.3.4/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-20 02:45:31.000000 scmrepo-3.3.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-20 02:45:31.000000 scmrepo-3.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-20 02:45:45.547860 scmrepo-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-20 02:45:31.000000 scmrepo-3.3.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-20 02:45:31.000000 scmrepo-3.3.4/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-20 02:45:31.000000 scmrepo-3.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:45:45.547860 scmrepo-3.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.531859 scmrepo-3.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.539860 scmrepo-3.3.4/src/scmrepo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.539860 scmrepo-3.3.4/src/scmrepo/git/
+-rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.539860 scmrepo-3.3.4/src/scmrepo/git/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/backend/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.539860 scmrepo-3.3.4/src/scmrepo/git/backend/dulwich/
+-rw-r--r--   0 runner    (1001) docker     (127)    34740 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/backend/dulwich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/backend/dulwich/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25350 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/backend/gitpython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.539860 scmrepo-3.3.4/src/scmrepo/git/backend/pygit2/
+-rw-r--r--   0 runner    (1001) docker     (127)    37132 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/backend/pygit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/backend/pygit2/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/backend/pygit2/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.543860 scmrepo-3.3.4/src/scmrepo/git/lfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/lfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/lfs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/lfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/lfs/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/lfs/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/lfs/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/lfs/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/lfs/smudge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/lfs/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/git/stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/noscm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-20 02:45:31.000000 scmrepo-3.3.4/src/scmrepo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.543860 scmrepo-3.3.4/src/scmrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-20 02:45:45.000000 scmrepo-3.3.4/src/scmrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-20 02:45:45.000000 scmrepo-3.3.4/src/scmrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:45:45.000000 scmrepo-3.3.4/src/scmrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 02:45:45.000000 scmrepo-3.3.4/src/scmrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 02:45:45.000000 scmrepo-3.3.4/src/scmrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.543860 scmrepo-3.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.543860 scmrepo-3.3.4/tests/git-init/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_dulwich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36426 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_lfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_noscm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_pygit2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_scmrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/user.key
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/user.key.pub
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:45.543860 scmrepo-3.3.4/tests/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-20 02:45:31.000000 scmrepo-3.3.4/tests/vendor/test_paramiko_vendor.py
```

### Comparing `scmrepo-3.3.3/.cruft.json` & `scmrepo-3.3.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/.github/workflows/release.yaml` & `scmrepo-3.3.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/.github/workflows/tests.yaml` & `scmrepo-3.3.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/.gitignore` & `scmrepo-3.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/.pre-commit-config.yaml` & `scmrepo-3.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/CODE_OF_CONDUCT.rst` & `scmrepo-3.3.4/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/CONTRIBUTING.rst` & `scmrepo-3.3.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/LICENSE` & `scmrepo-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/PKG-INFO` & `scmrepo-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 3.3.3
+Version: 3.3.4
 Summary: scmrepo
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/scmrepo/issues
 Project-URL: Source, https://github.com/iterative/scmrepo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scmrepo-3.3.3/README.rst` & `scmrepo-3.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/noxfile.py` & `scmrepo-3.3.4/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 @nox.session
 def safety(session: nox.Session) -> None:
     """Scan dependencies for insecure packages."""
     session.install(".[dev]")
     session.install("safety")
-    session.run("safety", "check", "--full-report")
+    session.run("safety", "check", "--full-report", "--ignore=67599")
 
 
 @nox.session
 def build(session: nox.Session) -> None:
     session.install("build", "setuptools", "twine")
     session.run("python", "-m", "build")
     dists = glob.glob("dist/*")
```

### Comparing `scmrepo-3.3.3/pyproject.toml` & `scmrepo-3.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/asyn.py` & `scmrepo-3.3.4/src/scmrepo/asyn.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/base.py` & `scmrepo-3.3.4/src/scmrepo/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/exceptions.py` & `scmrepo-3.3.4/src/scmrepo/exceptions.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/fs.py` & `scmrepo-3.3.4/src/scmrepo/fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/__init__.py` & `scmrepo-3.3.4/src/scmrepo/git/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/backend/base.py` & `scmrepo-3.3.4/src/scmrepo/git/backend/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/__init__.py` & `scmrepo-3.3.4/src/scmrepo/git/backend/dulwich/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py` & `scmrepo-3.3.4/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/backend/dulwich/client.py` & `scmrepo-3.3.4/src/scmrepo/git/backend/dulwich/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/backend/gitpython.py` & `scmrepo-3.3.4/src/scmrepo/git/backend/gitpython.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/__init__.py` & `scmrepo-3.3.4/src/scmrepo/git/backend/pygit2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 if raw:
                     blob_kwargs = {}
                 else:
                     assert key is not None
                     path = "/".join(key)
                     blob_kwargs = {
                         "as_path": path,
-                        "commit_id": commit.oid,
+                        "commit_id": commit.id,
                     }
                 blobio = BlobIO(self.obj, **blob_kwargs)
                 if mode == "rb":
                     return blobio
                 return TextIOWrapper(blobio, encoding=encoding)
             except GitError as exc:
                 raise SCMError("failed to read git blob") from exc
@@ -104,15 +104,15 @@
         try:
             return len(self.obj.read_raw())
         except KeyError:
             return 0
 
     @property
     def sha(self) -> str:
-        return self.obj.hex
+        return str(self.obj.id)
 
     def scandir(self) -> Iterable["Pygit2Object"]:
         for entry in self.obj:
             yield Pygit2Object(entry, backend=self.backend)
 
 
 class Pygit2Config(Config):
@@ -186,20 +186,21 @@
     @cached_property
     def _refdb(self):
         from pygit2 import RefdbFsBackend
 
         return RefdbFsBackend(self.repo)
 
     def _resolve_refish(self, refish: str):
-        from pygit2 import GIT_OBJ_COMMIT, Tag
+        from pygit2 import Tag
+        from pygit2.enums import ObjectType
 
         commit, ref = self.repo.resolve_refish(refish)
         if isinstance(commit, Tag):
             ref = commit
-            commit = commit.peel(GIT_OBJ_COMMIT)
+            commit = commit.peel(ObjectType.COMMIT)
         return commit, ref
 
     @property
     def default_signature(self) -> "Signature":
         try:
             return self.repo.default_signature
         except KeyError as exc:
@@ -391,24 +392,25 @@
     def tag(
         self,
         tag: str,
         target: Optional[str] = None,
         annotated: bool = False,
         message: Optional[str] = None,
     ):
-        from pygit2 import GIT_OBJ_COMMIT, GitError
+        from pygit2 import GitError
+        from pygit2.enums import ObjectType
 
         if annotated and not message:
             raise SCMError("message is required for annotated tag")
         target_obj = self.repo.revparse_single(target or "HEAD")
         with reraise(GitError, SCMError("Failed to create tag")):
             self.repo.create_tag(
                 tag,
                 target_obj.id,
-                GIT_OBJ_COMMIT,
+                ObjectType.COMMIT,
                 self.committer,
                 message or "",
             )
 
     def untracked_files(self) -> Iterable[str]:
         raise NotImplementedError
 
@@ -522,28 +524,29 @@
             self._refdb.ensure_log(name)
         if symbolic:
             self.repo.create_reference_symbolic(name, new_ref, True, message=message)
         else:
             self.repo.create_reference_direct(name, new_ref, True, message=message)
 
     def get_ref(self, name, follow: bool = True) -> Optional[str]:
-        from pygit2 import GIT_OBJ_COMMIT, GIT_REF_SYMBOLIC, InvalidSpecError, Tag
+        from pygit2 import InvalidSpecError, Tag
+        from pygit2.enums import ObjectType, ReferenceType
 
         try:
             ref = self.repo.references.get(name)
         except InvalidSpecError:
             return None
         if not ref:
             return None
-        if follow and ref.type == GIT_REF_SYMBOLIC:
+        if follow and ref.type == ReferenceType.SYMBOLIC:
             ref = ref.resolve()
         try:
             obj = self.repo[ref.target]
             if isinstance(obj, Tag):
-                return str(obj.peel(GIT_OBJ_COMMIT).id)
+                return str(obj.peel(ObjectType.COMMIT).id)
         except ValueError:
             pass
 
         return str(ref.target)
 
     def remove_ref(self, name: str, old_ref: Optional[str] = None):
         ref = self.repo.references.get(name)
@@ -837,15 +840,15 @@
         if paths is not None:
             tree = self.repo.revparse_single("HEAD").tree
             for path in paths:
                 rel = relpath(path, self.root_dir)
                 if os.name == "nt":
                     rel = rel.replace("\\", "/")
                 obj = tree[rel]
-                self.repo.index.add(IndexEntry(rel, obj.oid, obj.filemode))
+                self.repo.index.add(IndexEntry(rel, obj.id, obj.filemode))
             self.repo.index.write()
         elif hard:
             self.repo.reset(self.repo.head.target, GIT_RESET_HARD)
         else:
             self.repo.reset(self.repo.head.target, GIT_RESET_MIXED)
 
     def checkout_index(
@@ -1073,15 +1076,15 @@
         if not ref:
             return None
         try:
             tag = self.repo[ref.target]
             if isinstance(tag, Tag):
                 return GitTag(
                     tag.name,
-                    str(tag.oid),
+                    str(tag.id),
                     str(tag.target),
                     tag.tagger.name,
                     tag.tagger.email,
                     tag.tagger.time,
                     tag.tagger.offset * 60,
                     tag.message,
                 )
```

### Comparing `scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/callbacks.py` & `scmrepo-3.3.4/src/scmrepo/git/backend/pygit2/callbacks.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/backend/pygit2/filter.py` & `scmrepo-3.3.4/src/scmrepo/git/backend/pygit2/filter.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/config.py` & `scmrepo-3.3.4/src/scmrepo/git/config.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/credentials.py` & `scmrepo-3.3.4/src/scmrepo/git/credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/lfs/client.py` & `scmrepo-3.3.4/src/scmrepo/git/lfs/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/lfs/fetch.py` & `scmrepo-3.3.4/src/scmrepo/git/lfs/fetch.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/lfs/pointer.py` & `scmrepo-3.3.4/src/scmrepo/git/lfs/pointer.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/lfs/progress.py` & `scmrepo-3.3.4/src/scmrepo/git/lfs/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/lfs/smudge.py` & `scmrepo-3.3.4/src/scmrepo/git/lfs/smudge.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/lfs/storage.py` & `scmrepo-3.3.4/src/scmrepo/git/lfs/storage.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/objects.py` & `scmrepo-3.3.4/src/scmrepo/git/objects.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/git/stash.py` & `scmrepo-3.3.4/src/scmrepo/git/stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/progress.py` & `scmrepo-3.3.4/src/scmrepo/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/urls.py` & `scmrepo-3.3.4/src/scmrepo/urls.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo/utils.py` & `scmrepo-3.3.4/src/scmrepo/utils.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/src/scmrepo.egg-info/PKG-INFO` & `scmrepo-3.3.4/src/scmrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 3.3.3
+Version: 3.3.4
 Summary: scmrepo
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/scmrepo/issues
 Project-URL: Source, https://github.com/iterative/scmrepo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scmrepo-3.3.3/src/scmrepo.egg-info/SOURCES.txt` & `scmrepo-3.3.4/src/scmrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/conftest.py` & `scmrepo-3.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_credentials.py` & `scmrepo-3.3.4/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_dulwich.py` & `scmrepo-3.3.4/tests/test_dulwich.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_fs.py` & `scmrepo-3.3.4/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_git.py` & `scmrepo-3.3.4/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_lfs.py` & `scmrepo-3.3.4/tests/test_lfs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_noscm.py` & `scmrepo-3.3.4/tests/test_noscm.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_pygit2.py` & `scmrepo-3.3.4/tests/test_pygit2.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_scmrepo.py` & `scmrepo-3.3.4/tests/test_scmrepo.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_stash.py` & `scmrepo-3.3.4/tests/test_stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/test_urls.py` & `scmrepo-3.3.4/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/user.key` & `scmrepo-3.3.4/tests/user.key`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.3/tests/vendor/test_paramiko_vendor.py` & `scmrepo-3.3.4/tests/vendor/test_paramiko_vendor.py`

 * *Files identical despite different names*

