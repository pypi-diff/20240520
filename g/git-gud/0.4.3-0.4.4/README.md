# Comparing `tmp/git-gud-0.4.3.tar.gz` & `tmp/git_gud-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-gud-0.4.3.tar", last modified: Tue May 17 21:49:40 2022, max compression
+gzip compressed data, was "git_gud-0.4.4.tar", last modified: Mon May 20 08:59:36 2024, max compression
```

## Comparing `git-gud-0.4.3.tar` & `git_gud-0.4.4.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.641347 git-gud-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-05-17 21:49:30.000000 git-gud-0.4.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-05-17 21:49:40.641347 git-gud-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-05-17 21:49:30.000000 git-gud-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-05-17 21:49:30.000000 git-gud-0.4.3/git-gud.1
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/git_gud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-05-17 21:49:40.000000 git-gud-0.4.3/git_gud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5677 2022-05-17 21:49:40.000000 git-gud-0.4.3/git_gud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-17 21:49:40.000000 git-gud-0.4.3/git_gud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-17 21:49:40.000000 git-gud-0.4.3/git_gud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-17 21:49:40.000000 git-gud-0.4.3/git_gud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-17 21:49:40.000000 git-gud-0.4.3/git_gud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/gitgud/
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19225 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/gitgud/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/hooks/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      209 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/hooks/postrewrite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/gitgud/skills/
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/gitgud/skills/basics/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/gitgud/skills/basics/_branching/
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_branching/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_branching/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_branching/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_branching/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_branching/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/gitgud/skills/basics/_committing/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_committing/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_committing/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_committing/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_committing/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_committing/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/gitgud/skills/basics/_merging/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_merging/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_merging/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_merging/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_merging/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_merging/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/gitgud/skills/basics/_rebasing/
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_rebasing/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_rebasing/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_rebasing/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_rebasing/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/_rebasing/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/basics/test_levels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.629347 git-gud-0.4.3/gitgud/skills/extras/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.633347 git-gud-0.4.3/gitgud/skills/extras/_octopus/
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/extras/_octopus/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/extras/_octopus/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/extras/_octopus/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/extras/_octopus/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/extras/_octopus/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/extras/test_levels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.633347 git-gud-0.4.3/gitgud/skills/intro/
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.633347 git-gud-0.4.3/gitgud/skills/intro/_config/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_config/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_config/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_config/passed.txt
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_config/post-setup.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_config/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_config/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_config/status-1.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_config/status-2.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_config/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.633347 git-gud-0.4.3/gitgud/skills/intro/_init/
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_init/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_init/failed.txt
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_init/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_init/passed.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_init/post-setup.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_init/solution.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.633347 git-gud-0.4.3/gitgud/skills/intro/_welcome/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/details.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/passed.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/post-setup.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/status.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/_welcome/welcome.txt
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/intro/test_levels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.633347 git-gud-0.4.3/gitgud/skills/mixedbag/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/mixedbag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.633347 git-gud-0.4.3/gitgud/skills/mixedbag/_onecommit/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/mixedbag/_onecommit/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/mixedbag/_onecommit/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/mixedbag/_onecommit/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/mixedbag/_onecommit/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/mixedbag/_onecommit/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/mixedbag/test_levels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.633347 git-gud-0.4.3/gitgud/skills/newbasics/
--rw-r--r--   0 runner    (1001) docker     (121)     6879 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.633347 git-gud-0.4.3/gitgud/skills/newbasics/_firstcommit/
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_firstcommit/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_firstcommit/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_firstcommit/post-setup.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_firstcommit/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_firstcommit/solution.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/newbasics/_five/
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_five/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_five/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_five/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_five/solution.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/newbasics/_two/
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_two/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_two/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_two/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/_two/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/newbasics/test_levels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/rampup/
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/rampup/_detaching/
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_detaching/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_detaching/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_detaching/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_detaching/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_detaching/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/rampup/_relrefs1/
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs1/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs1/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs1/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs1/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs1/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/rampup/_relrefs2/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs2/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs2/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs2/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs2/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_relrefs2/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/rampup/_reversing/
--rw-r--r--   0 runner    (1001) docker     (121)     4093 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_reversing/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_reversing/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_reversing/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_reversing/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/_reversing/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rampup/test_levels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/rework/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/rework/_cherrypicking/
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_cherrypicking/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_cherrypicking/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_cherrypicking/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_cherrypicking/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_cherrypicking/test.spec
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/rework/_irebase/
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_irebase/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_irebase/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_irebase/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_irebase/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/_irebase/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rework/test_levels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.637347 git-gud-0.4.3/gitgud/skills/rewriting/
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rewriting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.641347 git-gud-0.4.3/gitgud/skills/rewriting/_easy/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rewriting/_easy/details.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rewriting/_easy/explanation.txt
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rewriting/_easy/goal.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rewriting/_easy/setup.spec
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rewriting/_easy/solution.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rewriting/_easy/test.spec
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/skills/rewriting/test_levels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.641347 git-gud-0.4.3/gitgud/user_messages/
--rw-r--r--   0 runner    (1001) docker     (121)     6674 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/user_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/user_messages/stateful.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 21:49:40.641347 git-gud-0.4.3/gitgud/util/
--rw-r--r--   0 runner    (1001) docker     (121)     1908 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6576 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/util/level_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    20356 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/util/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     8455 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/util/parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/util/test_levels.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/util/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/util/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/util/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-17 21:49:30.000000 git-gud-0.4.3/gitgud/version.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-17 21:49:40.641347 git-gud-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-05-17 21:49:30.000000 git-gud-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.825287 git_gud-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-20 08:59:26.000000 git_gud-0.4.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-20 08:59:36.825287 git_gud-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-20 08:59:26.000000 git_gud-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-20 08:59:26.000000 git_gud-0.4.4/git-gud.1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.821287 git_gud-0.4.4/git_gud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-20 08:59:36.000000 git_gud-0.4.4/git_gud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-20 08:59:36.000000 git_gud-0.4.4/git_gud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:59:36.000000 git_gud-0.4.4/git_gud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 08:59:36.000000 git_gud-0.4.4/git_gud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 08:59:36.000000 git_gud-0.4.4/git_gud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 08:59:36.000000 git_gud-0.4.4/git_gud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.801287 git_gud-0.4.4/gitgud/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19225 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.801287 git_gud-0.4.4/gitgud/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/hooks/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      209 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/hooks/postrewrite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.801287 git_gud-0.4.4/gitgud/skills/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.801287 git_gud-0.4.4/gitgud/skills/basics/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.801287 git_gud-0.4.4/gitgud/skills/basics/_branching/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_branching/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_branching/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_branching/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_branching/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_branching/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.805287 git_gud-0.4.4/gitgud/skills/basics/_committing/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_committing/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_committing/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_committing/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_committing/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_committing/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.805287 git_gud-0.4.4/gitgud/skills/basics/_merging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_merging/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_merging/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_merging/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_merging/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_merging/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.805287 git_gud-0.4.4/gitgud/skills/basics/_rebasing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_rebasing/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_rebasing/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_rebasing/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_rebasing/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/_rebasing/test.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/basics/test_levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.805287 git_gud-0.4.4/gitgud/skills/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.805287 git_gud-0.4.4/gitgud/skills/extras/_octopus/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/extras/_octopus/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/extras/_octopus/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/extras/_octopus/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/extras/_octopus/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/extras/_octopus/test.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/extras/test_levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.809287 git_gud-0.4.4/gitgud/skills/intro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.809287 git_gud-0.4.4/gitgud/skills/intro/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_config/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_config/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_config/passed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_config/post-setup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_config/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_config/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_config/status-1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_config/status-2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_config/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.809287 git_gud-0.4.4/gitgud/skills/intro/_init/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_init/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_init/failed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_init/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_init/passed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_init/post-setup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_init/solution.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.813287 git_gud-0.4.4/gitgud/skills/intro/_welcome/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/details.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/passed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/post-setup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/status.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/test.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/_welcome/welcome.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/intro/test_levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.813287 git_gud-0.4.4/gitgud/skills/mixedbag/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/mixedbag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.813287 git_gud-0.4.4/gitgud/skills/mixedbag/_onecommit/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/mixedbag/_onecommit/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/mixedbag/_onecommit/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/mixedbag/_onecommit/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/mixedbag/_onecommit/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/mixedbag/_onecommit/test.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/mixedbag/test_levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.813287 git_gud-0.4.4/gitgud/skills/newbasics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.813287 git_gud-0.4.4/gitgud/skills/newbasics/_firstcommit/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_firstcommit/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_firstcommit/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_firstcommit/post-setup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_firstcommit/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_firstcommit/solution.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.813287 git_gud-0.4.4/gitgud/skills/newbasics/_five/
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_five/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_five/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_five/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_five/solution.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.813287 git_gud-0.4.4/gitgud/skills/newbasics/_two/
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_two/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_two/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_two/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/_two/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/newbasics/test_levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.813287 git_gud-0.4.4/gitgud/skills/rampup/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.817287 git_gud-0.4.4/gitgud/skills/rampup/_detaching/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_detaching/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_detaching/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_detaching/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_detaching/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_detaching/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.817287 git_gud-0.4.4/gitgud/skills/rampup/_relrefs1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs1/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs1/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs1/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs1/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs1/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.817287 git_gud-0.4.4/gitgud/skills/rampup/_relrefs2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs2/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs2/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs2/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs2/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_relrefs2/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.817287 git_gud-0.4.4/gitgud/skills/rampup/_reversing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_reversing/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_reversing/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_reversing/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_reversing/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/_reversing/test.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rampup/test_levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.817287 git_gud-0.4.4/gitgud/skills/rework/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.821287 git_gud-0.4.4/gitgud/skills/rework/_cherrypicking/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_cherrypicking/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_cherrypicking/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_cherrypicking/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_cherrypicking/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_cherrypicking/test.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.821287 git_gud-0.4.4/gitgud/skills/rework/_irebase/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_irebase/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_irebase/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_irebase/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_irebase/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/_irebase/test.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rework/test_levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.821287 git_gud-0.4.4/gitgud/skills/rewriting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rewriting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.821287 git_gud-0.4.4/gitgud/skills/rewriting/_easy/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rewriting/_easy/details.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rewriting/_easy/explanation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rewriting/_easy/goal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rewriting/_easy/setup.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rewriting/_easy/solution.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rewriting/_easy/test.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/skills/rewriting/test_levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.821287 git_gud-0.4.4/gitgud/user_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/user_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/user_messages/stateful.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:59:36.821287 git_gud-0.4.4/gitgud/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/util/level_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/util/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/util/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/util/test_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/util/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/util/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/util/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 08:59:26.000000 git_gud-0.4.4/gitgud/version.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:59:36.825287 git_gud-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-20 08:59:26.000000 git_gud-0.4.4/setup.py
```

### Comparing `git-gud-0.4.3/LICENSE.md` & `git_gud-0.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/PKG-INFO` & `git_gud-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: git-gud
-Version: 0.4.3
+Version: 0.4.4
 Summary: A command line game to learn git
 Home-page: https://github.com/benthayer/git-gud/
 Author: Ben Thayer
 Author-email: ben@benthayer.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: gitpython==3.1.7
+Requires-Dist: importlib_resources
+Requires-Dist: pyyaml
 
 # Git Gud
 
 ![Demonstration](./preview.gif)
 
 ## What is it?
 Welcome to Git Gud, a command line game designed to help you learn how to use the popular version control system known as Git!
@@ -61,9 +63,7 @@
 Git Gud will guide you through what to do
 
 If either of those command don't work, there are verious things you can try:
  - Use `pip` instead of `pip3`
  - Make sure your PATH variable includes Python executables
  - User install: `pip3 install --user git-gud`
  - Use Anaconda
-
-
```

### Comparing `git-gud-0.4.3/README.md` & `git_gud-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/git-gud.1` & `git_gud-0.4.4/git-gud.1`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/git_gud.egg-info/PKG-INFO` & `git_gud-0.4.4/git_gud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: git-gud
-Version: 0.4.3
+Version: 0.4.4
 Summary: A command line game to learn git
 Home-page: https://github.com/benthayer/git-gud/
 Author: Ben Thayer
 Author-email: ben@benthayer.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: gitpython==3.1.7
+Requires-Dist: importlib_resources
+Requires-Dist: pyyaml
 
 # Git Gud
 
 ![Demonstration](./preview.gif)
 
 ## What is it?
 Welcome to Git Gud, a command line game designed to help you learn how to use the popular version control system known as Git!
@@ -61,9 +63,7 @@
 Git Gud will guide you through what to do
 
 If either of those command don't work, there are verious things you can try:
  - Use `pip` instead of `pip3`
  - Make sure your PATH variable includes Python executables
  - User install: `pip3 install --user git-gud`
  - Use Anaconda
-
-
```

### Comparing `git-gud-0.4.3/git_gud.egg-info/SOURCES.txt` & `git_gud-0.4.4/git_gud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/__init__.py` & `git_gud-0.4.4/gitgud/__init__.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/__main__.py` & `git_gud-0.4.4/gitgud/__main__.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/__init__.py` & `git_gud-0.4.4/gitgud/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/basics/_branching/explanation.txt` & `git_gud-0.4.4/gitgud/skills/basics/_branching/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/basics/_committing/explanation.txt` & `git_gud-0.4.4/gitgud/skills/basics/_committing/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/basics/_merging/explanation.txt` & `git_gud-0.4.4/gitgud/skills/basics/_merging/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/basics/_rebasing/explanation.txt` & `git_gud-0.4.4/gitgud/skills/basics/_rebasing/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/extras/_octopus/explanation.txt` & `git_gud-0.4.4/gitgud/skills/extras/_octopus/explanation.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 In this skill, we're going to go over a feature only a few people know about and even fewer know how to use properly: the octopus merge!
 >>>
 Performing an octopus merge is very similar to creating a normal merge,
  the only difference is the number of commits specified.
-An octopus merge can be a merge between 8 branches, but despite its' name,
+An octopus merge can be a merge between 8 branches, but despite its name,
  it can also be less than that... or more! The only requirement is that there be more than two commits.
 >>>
 Remember: the branch that is currently checked out is always included in the merge!
-Run `git merge feature1 feature2` to create an octopus merge and complete the skill!
+Run `git merge feature1 feature2` to create an octopus merge and complete the skill!
```

### Comparing `git-gud-0.4.3/gitgud/skills/intro/__init__.py` & `git_gud-0.4.4/gitgud/skills/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/intro/_init/explanation.txt` & `git_gud-0.4.4/gitgud/skills/intro/_init/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/intro/_welcome/welcome.txt` & `git_gud-0.4.4/gitgud/skills/intro/_welcome/welcome.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/mixedbag/_onecommit/explanation.txt` & `git_gud-0.4.4/gitgud/skills/mixedbag/_onecommit/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/newbasics/__init__.py` & `git_gud-0.4.4/gitgud/skills/newbasics/__init__.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/newbasics/_firstcommit/explanation.txt` & `git_gud-0.4.4/gitgud/skills/newbasics/_firstcommit/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/newbasics/_firstcommit/post-setup.txt` & `git_gud-0.4.4/gitgud/skills/newbasics/_firstcommit/post-setup.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/newbasics/_five/explanation.txt` & `git_gud-0.4.4/gitgud/skills/newbasics/_five/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/newbasics/_two/explanation.txt` & `git_gud-0.4.4/gitgud/skills/newbasics/_two/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/rampup/_detaching/explanation.txt` & `git_gud-0.4.4/gitgud/skills/rampup/_detaching/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/rampup/_relrefs1/explanation.txt` & `git_gud-0.4.4/gitgud/skills/rampup/_relrefs1/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/rampup/_relrefs2/explanation.txt` & `git_gud-0.4.4/gitgud/skills/rampup/_relrefs2/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/rampup/_reversing/explanation.txt` & `git_gud-0.4.4/gitgud/skills/rampup/_reversing/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/rework/_cherrypicking/explanation.txt` & `git_gud-0.4.4/gitgud/skills/rework/_cherrypicking/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/rework/_irebase/explanation.txt` & `git_gud-0.4.4/gitgud/skills/rework/_irebase/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/rewriting/__init__.py` & `git_gud-0.4.4/gitgud/skills/rewriting/__init__.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/skills/rewriting/_easy/explanation.txt` & `git_gud-0.4.4/gitgud/skills/rewriting/_easy/explanation.txt`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/user_messages/__init__.py` & `git_gud-0.4.4/gitgud/user_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/user_messages/stateful.py` & `git_gud-0.4.4/gitgud/user_messages/stateful.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/util/__init__.py` & `git_gud-0.4.4/gitgud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/util/level_builder.py` & `git_gud-0.4.4/gitgud/util/level_builder.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/util/operations.py` & `git_gud-0.4.4/gitgud/util/operations.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/util/parsing.py` & `git_gud-0.4.4/gitgud/util/parsing.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/util/test_levels.py` & `git_gud-0.4.4/gitgud/util/test_levels.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/util/test_parsing.py` & `git_gud-0.4.4/gitgud/util/test_parsing.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/util/test_util.py` & `git_gud-0.4.4/gitgud/util/test_util.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/gitgud/util/testing.py` & `git_gud-0.4.4/gitgud/util/testing.py`

 * *Files identical despite different names*

### Comparing `git-gud-0.4.3/setup.py` & `git_gud-0.4.4/setup.py`

 * *Files identical despite different names*

