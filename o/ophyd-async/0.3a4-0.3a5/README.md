# Comparing `tmp/ophyd_async-0.3a4.tar.gz` & `tmp/ophyd_async-0.3a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd_async-0.3a4.tar", last modified: Mon May 13 12:05:11 2024, max compression
+gzip compressed data, was "ophyd_async-0.3a5.tar", last modified: Mon May 20 11:36:47 2024, max compression
```

## Comparing `ophyd_async-0.3a4.tar` & `ophyd_async-0.3a5.tar`

### file list

```diff
@@ -1,247 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.814739 ophyd_async-0.3a4/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.774739 ophyd_async-0.3a4/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-13 12:05:11.814739 ophyd_async-0.3a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/_templates/README
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/examples/epics_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/examples/foo_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0003-ophyd-async-migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0004-repository-structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0005-respect-black-line-length.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0006-procedural-device-definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/design-goals.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/event-loop-choice.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/flyscanning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/choose-interfaces-for-devices.md
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/compound-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/make-a-simple-device.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/make-a-standard-detector.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/write-tests-for-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.790739 ophyd_async-0.3a4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/bluesky_ophyd_epics_devices_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/bluesky_ophyd_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   253748 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/hardware-triggered-scan.png
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/ophyd_favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    89951 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/outer-scan.png
--rw-r--r--   0 runner    (1001) docker     (127)   128990 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/simple-hardware-scan.png
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.790739 ophyd_async-0.3a4/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.790739 ophyd_async-0.3a4/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/tutorials/using-existing-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:05:11.814739 ophyd_async-0.3a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.774739 ophyd_async-0.3a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.790739 ophyd_async-0.3a4/src/ophyd_async/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/mock_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/mock_signal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14674 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/soft_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/epics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/_aioca.py
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/_p4p.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/aravis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/ad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/kinetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/vimba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/_hdffile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/demo/mover.db
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/demo/sensor.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/motion/motor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/pvi/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/pvi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/pvi/pvi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/signal/_epics_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/signal/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/panda/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_common_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/panda/writers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/writers/_hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/writers/_panda_hdf_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/planstubs/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/planstubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/planstubs/prepare_trigger_and_dets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/demo/sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_detector_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_detector_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.810739 ophyd_async-0.3a4/src/ophyd_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_device_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_mock_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_soft_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/_backend/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_aravis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_kinetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_vimba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/demo/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/demo/test_demo_ad_sim_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/motion/test_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/test_pvi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/test_records.db
--rw-r--r--   0 runner    (1001) docker     (127)    18205 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/test_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/panda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/panda/db/
--rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/db/panda.db
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_panda_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_panda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/protocols/test_protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.810739 ophyd_async-0.3a4/tests/sim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.810739 ophyd_async-0.3a4/tests/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/demo/test_sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/test_pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/test_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/test_sim_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/test_streaming_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7655 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/test_flyer_with_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.821964 ophyd_async-0.3a5/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.781963 ophyd_async-0.3a5/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.781963 ophyd_async-0.3a5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.773963 ophyd_async-0.3a5/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.781963 ophyd_async-0.3a5/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.781963 ophyd_async-0.3a5/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-20 11:36:47.821964 ophyd_async-0.3a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/_templates/README
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/examples/epics_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/examples/foo_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.785963 ophyd_async-0.3a5/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0003-ophyd-async-migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0004-repository-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0005-respect-black-line-length.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/0006-procedural-device-definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/design-goals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/event-loop-choice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations/flyscanning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/choose-interfaces-for-devices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/compound-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/make-a-simple-device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/make-a-standard-detector.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to/write-tests-for-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/bluesky_ophyd_epics_devices_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/bluesky_ophyd_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   253748 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/hardware-triggered-scan.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/ophyd_favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    89951 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/outer-scan.png
+-rw-r--r--   0 runner    (1001) docker     (127)   128990 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/images/simple-hardware-scan.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/tutorials/using-existing-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:36:47.821964 ophyd_async-0.3a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.777963 ophyd_async-0.3a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.789963 ophyd_async-0.3a5/src/ophyd_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.793963 ophyd_async-0.3a5/src/ophyd_async/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/mock_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/mock_signal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16081 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/soft_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.793963 ophyd_async-0.3a5/src/ophyd_async/epics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.793963 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/_aioca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/_p4p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/_backend/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.797963 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/aravis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.797963 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.797963 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/ad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/vimba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.797963 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/_hdffile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/demo/mover.db
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/demo/sensor.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/motion/motor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/epics/pvi/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/pvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/pvi/pvi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/epics/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/signal/_epics_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/epics/signal/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/panda/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_common_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/panda/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/writers/_hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/panda/writers/_panda_hdf_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.801963 ophyd_async-0.3a5/src/ophyd_async/planstubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/planstubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/planstubs/ensure_connected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/planstubs/prepare_trigger_and_dets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.805963 ophyd_async-0.3a5/src/ophyd_async/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.805963 ophyd_async-0.3a5/src/ophyd_async/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/demo/sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_detector_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_detector_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/src/ophyd_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 11:36:47.000000 ophyd_async-0.3a5/src/ophyd_async.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.805963 ophyd_async-0.3a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.805963 ophyd_async-0.3a5/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_device_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_mock_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_soft_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/core/test_watchable_async_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/_backend/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_aravis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_vimba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/areadetector/test_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/demo/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/demo/test_demo_ad_sim_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.809964 ophyd_async-0.3a5/tests/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/motion/test_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/test_pvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/test_records.db
+-rw-r--r--   0 runner    (1001) docker     (127)    18205 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/epics/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/panda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/panda/db/
+-rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/db/panda.db
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_panda_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_panda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/panda/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/protocols/test_protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:47.813964 ophyd_async-0.3a5/tests/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/demo/test_sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/test_pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/test_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/test_sim_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/sim/test_streaming_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7655 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/test_flyer_with_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-20 11:36:44.000000 ophyd_async-0.3a5/tests/test_log.py
```

### Comparing `ophyd_async-0.3a4/.devcontainer/devcontainer.json` & `ophyd_async-0.3a5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/CONTRIBUTING.md` & `ophyd_async-0.3a5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/actions/install_requirements/action.yml` & `ophyd_async-0.3a5/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/dependabot.yml` & `ophyd_async-0.3a5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/pages/make_switcher.py` & `ophyd_async-0.3a5/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/workflows/_check.yml` & `ophyd_async-0.3a5/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/workflows/_dist.yml` & `ophyd_async-0.3a5/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/workflows/_docs.yml` & `ophyd_async-0.3a5/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/workflows/_release.yml` & `ophyd_async-0.3a5/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/workflows/_test.yml` & `ophyd_async-0.3a5/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.github/workflows/ci.yml` & `ophyd_async-0.3a5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.gitignore` & `ophyd_async-0.3a5/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.mailmap` & `ophyd_async-0.3a5/.mailmap`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/.pre-commit-config.yaml` & `ophyd_async-0.3a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/Dockerfile` & `ophyd_async-0.3a5/Dockerfile`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/LICENSE` & `ophyd_async-0.3a5/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/PKG-INFO` & `ophyd_async-0.3a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a4
+Version: 0.3a5
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ophyd_async-0.3a4/README.md` & `ophyd_async-0.3a5/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/_templates/custom-class-template.rst` & `ophyd_async-0.3a5/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/_templates/custom-module-template.rst` & `ophyd_async-0.3a5/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/conf.py` & `ophyd_async-0.3a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/examples/epics_demo.py` & `ophyd_async-0.3a5/docs/examples/epics_demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/examples/foo_detector.py` & `ophyd_async-0.3a5/docs/examples/foo_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `ophyd_async-0.3a5/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/explanations/decisions/0003-ophyd-async-migration.rst` & `ophyd_async-0.3a5/docs/explanations/decisions/0003-ophyd-async-migration.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/explanations/decisions/0004-repository-structure.rst` & `ophyd_async-0.3a5/docs/explanations/decisions/0004-repository-structure.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/explanations/decisions/0005-respect-black-line-length.rst` & `ophyd_async-0.3a5/docs/explanations/decisions/0005-respect-black-line-length.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/explanations/decisions/0006-procedural-device-definitions.rst` & `ophyd_async-0.3a5/docs/explanations/decisions/0006-procedural-device-definitions.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/explanations/design-goals.rst` & `ophyd_async-0.3a5/docs/explanations/design-goals.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/explanations/event-loop-choice.rst` & `ophyd_async-0.3a5/docs/explanations/event-loop-choice.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/explanations/flyscanning.rst` & `ophyd_async-0.3a5/docs/explanations/flyscanning.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/how-to/choose-interfaces-for-devices.md` & `ophyd_async-0.3a5/docs/how-to/choose-interfaces-for-devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/how-to/compound-devices.rst` & `ophyd_async-0.3a5/docs/how-to/compound-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/how-to/make-a-simple-device.rst` & `ophyd_async-0.3a5/docs/how-to/make-a-simple-device.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/how-to/make-a-standard-detector.rst` & `ophyd_async-0.3a5/docs/how-to/make-a-standard-detector.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/how-to/write-tests-for-devices.rst` & `ophyd_async-0.3a5/docs/how-to/write-tests-for-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/images/bluesky_ophyd_epics_devices_logo.svg` & `ophyd_async-0.3a5/docs/images/bluesky_ophyd_epics_devices_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/images/bluesky_ophyd_logo.svg` & `ophyd_async-0.3a5/docs/images/bluesky_ophyd_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/images/hardware-triggered-scan.png` & `ophyd_async-0.3a5/docs/images/hardware-triggered-scan.png`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/images/ophyd_favicon.svg` & `ophyd_async-0.3a5/docs/images/ophyd_favicon.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/images/outer-scan.png` & `ophyd_async-0.3a5/docs/images/outer-scan.png`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/images/simple-hardware-scan.png` & `ophyd_async-0.3a5/docs/images/simple-hardware-scan.png`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/index.md` & `ophyd_async-0.3a5/docs/index.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/reference/api.rst` & `ophyd_async-0.3a5/docs/reference/api.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/tutorials/installation.md` & `ophyd_async-0.3a5/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/docs/tutorials/using-existing-devices.rst` & `ophyd_async-0.3a5/docs/tutorials/using-existing-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/pyproject.toml` & `ophyd_async-0.3a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/__init__.py` & `ophyd_async-0.3a5/src/ophyd_async/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ._providers import (
     DirectoryInfo,
     DirectoryProvider,
     NameProvider,
     ShapeProvider,
     StaticDirectoryProvider,
 )
-from .async_status import AsyncStatus
+from .async_status import AsyncStatus, WatchableAsyncStatus
 from .detector import (
     DetectorControl,
     DetectorTrigger,
     DetectorWriter,
     StandardDetector,
     TriggerInfo,
 )
@@ -92,14 +92,15 @@
     "soft_signal_rw",
     "observe_value",
     "set_and_wait_for_value",
     "set_mock_put_proceeds",
     "set_mock_value",
     "wait_for_value",
     "AsyncStatus",
+    "WatchableAsyncStatus",
     "DirectoryInfo",
     "DirectoryProvider",
     "NameProvider",
     "ShapeProvider",
     "StaticDirectoryProvider",
     "StandardReadable",
     "ConfigSignal",
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/_providers.py` & `ophyd_async-0.3a5/src/ophyd_async/core/_providers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/detector.py` & `ophyd_async-0.3a5/src/ophyd_async/core/detector.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     StreamAsset,
     Triggerable,
     WritesStreamAssets,
 )
 
 from ophyd_async.protocols import AsyncConfigurable, AsyncReadable
 
-from .async_status import AsyncStatus
+from .async_status import AsyncStatus, WatchableAsyncStatus
 from .device import Device
-from .utils import DEFAULT_TIMEOUT, merge_gathered_dicts
+from .utils import DEFAULT_TIMEOUT, WatcherUpdate, merge_gathered_dicts
 
 T = TypeVar("T")
 
 
 class DetectorTrigger(str, Enum):
     """Type of mechanism for triggering a detector to take frames"""
 
@@ -184,15 +184,15 @@
         self._config_sigs = list(config_sigs)
         self._frame_writing_timeout = writer_timeout
         # For prepare
         self._arm_status: Optional[AsyncStatus] = None
         self._trigger_info: Optional[TriggerInfo] = None
         # For kickoff
         self._watchers: List[Callable] = []
-        self._fly_status: Optional[AsyncStatus] = None
+        self._fly_status: Optional[WatchableAsyncStatus] = None
         self._fly_start: float
 
         self._intial_frame: int
         self._last_frame: int
         super().__init__(name)
 
     @property
@@ -288,51 +288,45 @@
         self._last_frame = self._initial_frame + self._trigger_info.num
 
         required = self.controller.get_deadtime(self._trigger_info.livetime)
         assert required <= self._trigger_info.deadtime, (
             f"Detector {self.controller} needs at least {required}s deadtime, "
             f"but trigger logic provides only {self._trigger_info.deadtime}s"
         )
-
         self._arm_status = await self.controller.arm(
             num=self._trigger_info.num,
             trigger=self._trigger_info.trigger,
             exposure=self._trigger_info.livetime,
         )
-
-    @AsyncStatus.wrap
-    async def kickoff(self) -> None:
-        self._fly_status = AsyncStatus(self._fly(), self._watchers)
         self._fly_start = time.monotonic()
 
-    async def _fly(self) -> None:
-        await self._observe_writer_indicies(self._last_frame)
-
-    async def _observe_writer_indicies(self, end_observation: int):
+    @AsyncStatus.wrap
+    async def kickoff(self):
+        if not self._arm_status:
+            raise Exception("Detector not armed!")
+
+    @WatchableAsyncStatus.wrap
+    async def complete(self):
+        assert self._arm_status, "Prepare not run"
+        assert self._trigger_info
         async for index in self.writer.observe_indices_written(
             self._frame_writing_timeout
         ):
-            for watcher in self._watchers:
-                watcher(
-                    name=self.name,
-                    current=index,
-                    initial=self._initial_frame,
-                    target=end_observation,
-                    unit="",
-                    precision=0,
-                    time_elapsed=time.monotonic() - self._fly_start,
-                )
-            if index >= end_observation:
+            yield WatcherUpdate(
+                name=self.name,
+                current=index,
+                initial=self._initial_frame,
+                target=self._trigger_info.num,
+                unit="",
+                precision=0,
+                time_elapsed=time.monotonic() - self._fly_start,
+            )
+            if index >= self._trigger_info.num:
                 break
 
-    @AsyncStatus.wrap
-    async def complete(self) -> AsyncStatus:
-        assert self._fly_status, "Kickoff not run"
-        return await self._fly_status
-
     async def describe_collect(self) -> Dict[str, DataKey]:
         return self._describe
 
     async def collect_asset_docs(
         self, index: Optional[int] = None
     ) -> AsyncIterator[StreamAsset]:
         # Collect stream datum documents for all indices written.
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/device.py` & `ophyd_async-0.3a5/src/ophyd_async/core/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Base device"""
 
 from __future__ import annotations
 
+import asyncio
 import sys
 from functools import cached_property
 from logging import LoggerAdapter, getLogger
 from typing import (
     Any,
     Coroutine,
     Dict,
@@ -28,14 +29,17 @@
 
     By default, names and connects all Device children.
     """
 
     _name: str = ""
     #: The parent Device if it exists
     parent: Optional[Device] = None
+    # None if connect hasn't started, a Task if it has
+    _connect_task: Optional[asyncio.Task] = None
+    _connect_mock_arg: bool = False
 
     def __init__(self, name: str = "") -> None:
         self.set_name(name)
 
     @property
     def name(self) -> str:
         """Return the name of the Device"""
@@ -67,32 +71,51 @@
 
         self._name = name
         for attr_name, child in self.children():
             child_name = f"{name}-{attr_name.rstrip('_')}" if name else ""
             child.set_name(child_name)
             child.parent = self
 
-    async def connect(self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT):
+    async def connect(
+        self,
+        mock: bool = False,
+        timeout: float = DEFAULT_TIMEOUT,
+        force_reconnect: bool = False,
+    ):
         """Connect self and all child Devices.
 
         Contains a timeout that gets propagated to child.connect methods.
 
         Parameters
         ----------
         mock:
             If True then use ``MockSignalBackend`` for all Signals
         timeout:
             Time to wait before failing with a TimeoutError.
         """
-        coros = {
-            name: child_device.connect(mock=mock, timeout=timeout)
-            for name, child_device in self.children()
-        }
-        if coros:
-            await wait_for_connection(**coros)
+        # If previous connect with same args has started and not errored, can use it
+        can_use_previous_connect = (
+            self._connect_task
+            and not (self._connect_task.done() and self._connect_task.exception())
+            and self._connect_mock_arg == mock
+        )
+        if force_reconnect or not can_use_previous_connect:
+            # Kick off a connection
+            coros = {
+                name: child_device.connect(
+                    mock, timeout=timeout, force_reconnect=force_reconnect
+                )
+                for name, child_device in self.children()
+            }
+            self._connect_task = asyncio.create_task(wait_for_connection(**coros))
+            self._connect_mock_arg = mock
+
+        assert self._connect_task, "Connect task not created, this shouldn't happen"
+        # Wait for it to complete
+        await self._connect_task
 
 
 VT = TypeVar("VT", bound=Device)
 
 
 class DeviceVector(Dict[int, VT], Device):
     """
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/device_save_loader.py` & `ophyd_async-0.3a5/src/ophyd_async/core/device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/flyer.py` & `ophyd_async-0.3a5/src/ophyd_async/core/flyer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/mock_signal_backend.py` & `ophyd_async-0.3a5/src/ophyd_async/core/mock_signal_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
+from functools import cached_property
 from typing import Optional, Type
-from unittest.mock import MagicMock
+from unittest.mock import Mock
 
 from bluesky.protocols import Descriptor, Reading
 
 from ophyd_async.core.signal_backend import SignalBackend
 from ophyd_async.core.soft_signal_backend import SoftSignalBackend
 from ophyd_async.core.utils import DEFAULT_TIMEOUT, ReadingValueCallback, T
 
@@ -32,55 +33,53 @@
             # If the backend is a hard signal backend, or not provided,
             # then we create a soft signal to mimick it
 
             self.soft_backend = SoftSignalBackend(datatype=datatype)
         else:
             self.soft_backend = initial_backend
 
-        self.mock = MagicMock()
-
-        self.put_proceeds = asyncio.Event()
-        self.put_proceeds.set()
-
     def source(self, name: str) -> str:
-        self.mock.source(name)
         if self.initial_backend:
             return f"mock+{self.initial_backend.source(name)}"
         return f"mock+{name}"
 
     async def connect(self, timeout: float = DEFAULT_TIMEOUT) -> None:
-        self.mock.connect(timeout=timeout)
+        pass
+
+    @cached_property
+    def put_mock(self) -> Mock:
+        return Mock(name="put")
+
+    @cached_property
+    def put_proceeds(self) -> asyncio.Event:
+        put_proceeds = asyncio.Event()
+        put_proceeds.set()
+        return put_proceeds
 
     async def put(self, value: Optional[T], wait=True, timeout=None):
-        self.mock.put(value, wait=wait, timeout=timeout)
+        self.put_mock(value, wait=wait, timeout=timeout)
         await self.soft_backend.put(value, wait=wait, timeout=timeout)
 
         if wait:
             await asyncio.wait_for(self.put_proceeds.wait(), timeout=timeout)
 
     def set_value(self, value: T):
-        self.mock.set_value(value)
         self.soft_backend.set_value(value)
 
     async def get_descriptor(self, source: str) -> Descriptor:
-        self.mock.get_descriptor(source)
         return await self.soft_backend.get_descriptor(source)
 
     async def get_reading(self) -> Reading:
-        self.mock.get_reading()
         return await self.soft_backend.get_reading()
 
     async def get_value(self) -> T:
-        self.mock.get_value()
         return await self.soft_backend.get_value()
 
     async def get_setpoint(self) -> T:
         """For a soft signal, the setpoint and readback values are the same."""
-        self.mock.get_setpoint()
         return await self.soft_backend.get_setpoint()
 
     async def get_datakey(self, source: str) -> Descriptor:
         return await self.soft_backend.get_datakey(source)
 
     def set_callback(self, callback: Optional[ReadingValueCallback[T]]) -> None:
-        self.mock.set_callback(callback)
         self.soft_backend.set_callback(callback)
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/mock_signal_utils.py` & `ophyd_async-0.3a5/src/ophyd_async/core/mock_signal_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextlib import asynccontextmanager, contextmanager
 from typing import Any, Callable, Generator, Iterable, Iterator, List
-from unittest.mock import ANY
+from unittest.mock import ANY, Mock
 
 from ophyd_async.core.signal import Signal
 from ophyd_async.core.utils import T
 
 from .mock_signal_backend import MockSignalBackend
 
 
@@ -39,20 +39,20 @@
     yield
     for signal in signals:
         set_mock_put_proceeds(signal, True)
 
 
 def assert_mock_put_called_with(signal: Signal, value: Any, wait=ANY, timeout=ANY):
     backend = _get_mock_signal_backend(signal)
-    backend.mock.put.assert_called_with(value, wait=wait, timeout=timeout)
+    backend.put_mock.assert_called_with(value, wait=wait, timeout=timeout)
 
 
 def reset_mock_put_calls(signal: Signal):
     backend = _get_mock_signal_backend(signal)
-    backend.mock.put.reset_mock()
+    backend.put_mock.reset_mock()
 
 
 class _SetValuesIterator:
     # Garbage collected by the time __del__ is called unless we put it as a
     # global attrbute here.
     require_all_consumed: bool = False
 
@@ -118,17 +118,17 @@
         signal,
         values,
         require_all_consumed=require_all_consumed,
     )
 
 
 @contextmanager
-def _unset_side_effect_cm(mock):
+def _unset_side_effect_cm(put_mock: Mock):
     yield
-    mock.put.side_effect = None
+    put_mock.side_effect = None
 
 
 # linting isn't smart enought to realize @contextmanager will give use a
 # ContextManager[None]
 def callback_on_mock_put(
     signal: Signal, callback: Callable[[T], None]
 ) -> Generator[None, None, None]:
@@ -141,9 +141,9 @@
     ----------
     signal:
         A signal with a `MockSignalBackend` backend.
     callback:
         The callback to call when the backend is put to during the context.
     """
     backend = _get_mock_signal_backend(signal)
-    backend.mock.put.side_effect = callback
-    return _unset_side_effect_cm(backend.mock)
+    backend.put_mock.side_effect = callback
+    return _unset_side_effect_cm(backend.put_mock)
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/signal.py` & `ophyd_async-0.3a5/src/ophyd_async/core/signal.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from bluesky.protocols import (
     DataKey,
     Locatable,
     Location,
     Movable,
     Reading,
+    Status,
     Subscribable,
 )
 
 from ophyd_async.core.mock_signal_backend import MockSignalBackend
 from ophyd_async.protocols import AsyncConfigurable, AsyncReadable, AsyncStageable
 
 from .async_status import AsyncStatus
@@ -60,15 +61,17 @@
         timeout: Optional[float] = DEFAULT_TIMEOUT,
         name: str = "",
     ) -> None:
         self._timeout = timeout
         self._initial_backend = self._backend = backend
         super().__init__(name)
 
-    async def connect(self, mock=False, timeout=DEFAULT_TIMEOUT):
+    async def connect(
+        self, mock=False, timeout=DEFAULT_TIMEOUT, force_reconnect: bool = False
+    ):
         if mock and not isinstance(self._backend, MockSignalBackend):
             # Using a soft backend, look to the initial value
             self._backend = MockSignalBackend(
                 initial_backend=self._initial_backend,
             )
         self.log.debug(f"Connecting to {self.source}")
         await self._backend.connect(timeout=timeout)
@@ -274,14 +277,27 @@
     """
     backend = SoftSignalBackend(datatype, initial_value)
     signal = SignalR(backend, name=name)
 
     return (signal, backend.set_value)
 
 
+def _generate_assert_error_msg(
+    name: str, expected_result: str, actuall_result: str
+) -> str:
+    WARNING = "\033[93m"
+    FAIL = "\033[91m"
+    ENDC = "\033[0m"
+    return (
+        f"Expected {WARNING}{name}{ENDC} to produce"
+        + f"\n{FAIL}{actuall_result}{ENDC}"
+        + f"\nbut actually got \n{FAIL}{expected_result}{ENDC}"
+    )
+
+
 async def assert_value(signal: SignalR[T], value: Any) -> None:
     """Assert a signal's value and compare it an expected signal.
 
     Parameters
     ----------
     signal:
         signal with get_value.
@@ -290,19 +306,22 @@
 
     Notes
     -----
     Example usage::
         await assert_value(signal, value)
 
     """
-    assert await signal.get_value() == value
+    actual_value = await signal.get_value()
+    assert actual_value == value, _generate_assert_error_msg(
+        signal.name, value, actual_value
+    )
 
 
 async def assert_reading(
-    readable: AsyncReadable, reading: Mapping[str, Reading]
+    readable: AsyncReadable, expected_reading: Mapping[str, Reading]
 ) -> None:
     """Assert readings from readable.
 
     Parameters
     ----------
     readable:
         Callable with readable.read function that generate readings.
@@ -312,15 +331,18 @@
 
     Notes
     -----
     Example usage::
         await assert_reading(readable, reading)
 
     """
-    assert await readable.read() == reading
+    actual_reading = await readable.read()
+    assert expected_reading == actual_reading, _generate_assert_error_msg(
+        readable.name, expected_reading, actual_reading
+    )
 
 
 async def assert_configuration(
     configurable: AsyncConfigurable,
     configuration: Mapping[str, Reading],
 ) -> None:
     """Assert readings from Configurable.
@@ -335,15 +357,18 @@
 
     Notes
     -----
     Example usage::
         await assert_configuration(configurable configuration)
 
     """
-    assert await configurable.read_configuration() == configuration
+    actual_configurable = await configurable.read_configuration()
+    assert configuration == actual_configurable, _generate_assert_error_msg(
+        configurable.name, configuration, actual_configurable
+    )
 
 
 def assert_emitted(docs: Mapping[str, list[dict]], **numbers: int):
     """Assert emitted document generated by running a Bluesky plan
 
     Parameters
     ----------
@@ -355,46 +380,65 @@
 
     Notes
     -----
     Example usage::
         assert_emitted(docs, start=1, descriptor=1,
         resource=1, datum=1, event=1, stop=1)
     """
-    assert list(docs) == list(numbers)
-    assert {name: len(d) for name, d in docs.items()} == numbers
+    assert list(docs) == list(numbers), _generate_assert_error_msg(
+        "documents", list(numbers), list(docs)
+    )
+    actual_numbers = {name: len(d) for name, d in docs.items()}
+    assert actual_numbers == numbers, _generate_assert_error_msg(
+        "emitted", numbers, actual_numbers
+    )
 
 
-async def observe_value(signal: SignalR[T], timeout=None) -> AsyncGenerator[T, None]:
+async def observe_value(
+    signal: SignalR[T], timeout=None, done_status: Status | None = None
+) -> AsyncGenerator[T, None]:
     """Subscribe to the value of a signal so it can be iterated from.
 
     Parameters
     ----------
     signal:
         Call subscribe_value on this at the start, and clear_sub on it at the
         end
+    done_status:
+        If this status is complete, stop observing and make the iterator return.
 
     Notes
     -----
     Example usage::
 
         async for value in observe_value(sig):
             do_something_with(value)
     """
-    q: asyncio.Queue[T] = asyncio.Queue()
+
+    class StatusIsDone: ...
+
+    q: asyncio.Queue[T | StatusIsDone] = asyncio.Queue()
     if timeout is None:
         get_value = q.get
     else:
 
         async def get_value():
             return await asyncio.wait_for(q.get(), timeout)
 
+    if done_status is not None:
+        done_status.add_callback(lambda _: q.put_nowait(StatusIsDone()))
+
     signal.subscribe_value(q.put_nowait)
     try:
         while True:
-            yield await get_value()
+            item = await get_value()
+            if not isinstance(item, StatusIsDone):
+                yield item
+            else:
+                break
     finally:
         signal.clear_sub(q.put_nowait)
 
 
 class _ValueChecker(Generic[T]):
     def __init__(self, matcher: Callable[[T], bool], matcher_name: str):
         self._last_value: Optional[T] = None
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/signal_backend.py` & `ophyd_async-0.3a5/src/ophyd_async/core/signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/soft_signal_backend.py` & `ophyd_async-0.3a5/src/ophyd_async/core/soft_signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/standard_readable.py` & `ophyd_async-0.3a5/src/ophyd_async/core/standard_readable.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/core/utils.py` & `ophyd_async-0.3a5/src/ophyd_async/core/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from __future__ import annotations
 
 import asyncio
 import logging
+from dataclasses import dataclass
 from typing import (
     Awaitable,
     Callable,
     Dict,
+    Generic,
     Iterable,
     List,
     Optional,
+    ParamSpec,
     Type,
     TypeVar,
     Union,
 )
 
 import numpy as np
 from bluesky.protocols import Reading
 
 T = TypeVar("T")
+P = ParamSpec("P")
 Callback = Callable[[T], None]
 
 #: A function that will be called with the Reading and value when the
 #: monitor updates
 ReadingValueCallback = Callable[[Reading, T], None]
 DEFAULT_TIMEOUT = 10.0
 ErrorText = Union[str, Dict[str, Exception]]
@@ -73,14 +77,29 @@
             string += self._format_sub_errors(name, error, indent=indent)
         return string
 
     def __str__(self) -> str:
         return self.format_error_string(indent="")
 
 
+@dataclass(frozen=True)
+class WatcherUpdate(Generic[T]):
+    """A dataclass such that, when expanded, it provides the kwargs for a watcher"""
+
+    current: T
+    initial: T
+    target: T
+    name: str | None = None
+    unit: str | None = None
+    precision: float | None = None
+    fraction: float | None = None
+    time_elapsed: float | None = None
+    time_remaining: float | None = None
+
+
 async def wait_for_connection(**coros: Awaitable[None]):
     """Call many underlying signals, accumulating exceptions and returning them
 
     Expected kwargs should be a mapping of names to coroutine tasks to execute.
     """
     results = await asyncio.gather(*coros.values(), return_exceptions=True)
     exceptions = {}
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/_backend/_aioca.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/_backend/_aioca.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/_backend/_p4p.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/_backend/_p4p.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/_backend/common.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/_backend/common.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/aravis.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/aravis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import get_args
 
 from bluesky.protocols import HasHints, Hints
 
-from ophyd_async.core import DirectoryProvider, StandardDetector, TriggerInfo
+from ophyd_async.core import DirectoryProvider, StandardDetector
 from ophyd_async.epics.areadetector.controllers.aravis_controller import (
     AravisController,
 )
 from ophyd_async.epics.areadetector.drivers import ADBaseShapeProvider
 from ophyd_async.epics.areadetector.drivers.aravis_driver import AravisDriver
 from ophyd_async.epics.areadetector.writers import HDFWriter, NDFileHDF
 
@@ -41,18 +41,14 @@
                 lambda: self.name,
                 ADBaseShapeProvider(self.drv),
             ),
             config_sigs=(self.drv.acquire_time,),
             name=name,
         )
 
-    async def _prepare(self, value: TriggerInfo) -> None:
-        await self.drv.fetch_deadtime()
-        await super()._prepare(value)
-
     def get_external_trigger_gpio(self):
         return self._controller.gpio_number
 
     def set_external_trigger_gpio(self, gpio_number: AravisController.GPIO_NUMBER):
         supported_gpio_numbers = get_args(AravisController.GPIO_NUMBER)
         if gpio_number not in supported_gpio_numbers:
             raise ValueError(
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,24 +10,29 @@
 from ophyd_async.epics.areadetector.drivers.aravis_driver import (
     AravisDriver,
     AravisTriggerMode,
     AravisTriggerSource,
 )
 from ophyd_async.epics.areadetector.utils import ImageMode, stop_busy_record
 
+# The deadtime of an ADaravis controller varies depending on the exact model of camera.
+# Ideally we would maximize performance by dynamically retrieving the deadtime at
+# runtime. See https://github.com/bluesky/ophyd-async/issues/308
+_HIGHEST_POSSIBLE_DEADTIME = 1961e-6
+
 
 class AravisController(DetectorControl):
     GPIO_NUMBER = Literal[1, 2, 3, 4]
 
     def __init__(self, driver: AravisDriver, gpio_number: GPIO_NUMBER) -> None:
         self._drv = driver
         self.gpio_number = gpio_number
 
     def get_deadtime(self, exposure: float) -> float:
-        return self._drv.dead_time or 0
+        return _HIGHEST_POSSIBLE_DEADTIME
 
     async def arm(
         self,
         num: int = 0,
         trigger: DetectorTrigger = DetectorTrigger.internal,
         exposure: Optional[float] = None,
     ) -> AsyncStatus:
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/ad_base.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/ad_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/kinetix.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/kinetix.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/pilatus.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/pilatus.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/single_trigger_det.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/single_trigger_det.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/utils.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/vimba.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/vimba.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/_hdffile.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/_hdffile.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/hdf_writer.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/hdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/nd_plugin.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/areadetector/writers/nd_plugin.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/demo/__init__.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/demo/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 import asyncio
 import atexit
 import random
 import string
 import subprocess
 import sys
-import time
+from dataclasses import replace
 from enum import Enum
 from pathlib import Path
-from typing import Callable, List, Optional
 
 import numpy as np
 from bluesky.protocols import Movable, Stoppable
 
 from ophyd_async.core import (
-    AsyncStatus,
     ConfigSignal,
     Device,
     DeviceVector,
     HintedSignal,
     StandardReadable,
+    WatchableAsyncStatus,
     observe_value,
 )
+from ophyd_async.core.utils import WatcherUpdate
 
 from ..signal.signal import epics_signal_r, epics_signal_rw, epics_signal_x
 
 
 class EnergyMode(str, Enum):
     """Energy mode for `Sensor`"""
 
@@ -81,54 +81,49 @@
         super().__init__(name=name)
 
     def set_name(self, name: str):
         super().set_name(name)
         # Readback should be named the same as its parent in read()
         self.readback.set_name(name)
 
-    async def _move(self, new_position: float, watchers: List[Callable] = []):
+    async def _move(self, new_position: float):
         self._set_success = True
         # time.monotonic won't go backwards in case of NTP corrections
-        start = time.monotonic()
         old_position, units, precision = await asyncio.gather(
             self.setpoint.get_value(),
             self.units.get_value(),
             self.precision.get_value(),
         )
         # Wait for the value to set, but don't wait for put completion callback
-        await self.setpoint.set(new_position, wait=False)
-        async for current_position in observe_value(self.readback):
-            for watcher in watchers:
-                watcher(
-                    name=self.name,
-                    current=current_position,
-                    initial=old_position,
-                    target=new_position,
-                    unit=units,
-                    precision=precision,
-                    time_elapsed=time.monotonic() - start,
-                )
-            if np.isclose(current_position, new_position):
-                break
+        move_status = self.setpoint.set(new_position, wait=True)
         if not self._set_success:
             raise RuntimeError("Motor was stopped")
+        # return a template to set() which it can use to yield progress updates
+        return (
+            WatcherUpdate(
+                initial=old_position,
+                current=old_position,
+                target=new_position,
+                unit=units,
+                precision=precision,
+            ),
+            move_status,
+        )
 
-    def move(self, new_position: float, timeout: Optional[float] = None):
-        """Commandline only synchronous move of a Motor"""
-        from bluesky.run_engine import call_in_bluesky_event_loop, in_bluesky_event_loop
-
-        if in_bluesky_event_loop():
-            raise RuntimeError("Will deadlock run engine if run in a plan")
-        call_in_bluesky_event_loop(self._move(new_position), timeout)  # type: ignore
-
-    # TODO: this fails if we call from the cli, but works if we "ipython await" it
-    def set(self, new_position: float, timeout: Optional[float] = None) -> AsyncStatus:
-        watchers: List[Callable] = []
-        coro = asyncio.wait_for(self._move(new_position, watchers), timeout=timeout)
-        return AsyncStatus(coro, watchers)
+    @WatchableAsyncStatus.wrap  # uses the timeout argument from the function it wraps
+    async def set(self, new_position: float, timeout: float | None = None):
+        update, _ = await self._move(new_position)
+        async for current_position in observe_value(self.readback):
+            yield replace(
+                update,
+                name=self.name,
+                current=current_position,
+            )
+            if np.isclose(current_position, new_position):
+                break
 
     async def stop(self, success=True):
         self._set_success = success
         status = self.stop_.trigger()
         await status
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/demo/demo_ad_sim_detector.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/demo/demo_ad_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/demo/mover.db` & `ophyd_async-0.3a5/src/ophyd_async/epics/demo/mover.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/demo/sensor.db` & `ophyd_async-0.3a5/src/ophyd_async/epics/demo/sensor.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/motion/motor.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/motion/motor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import asyncio
-import time
-from typing import Callable, List, Optional
+from dataclasses import replace
 
 from bluesky.protocols import Movable, Stoppable
 
-from ophyd_async.core import AsyncStatus, ConfigSignal, HintedSignal, StandardReadable
+from ophyd_async.core import (
+    AsyncStatus,
+    ConfigSignal,
+    HintedSignal,
+    StandardReadable,
+    WatchableAsyncStatus,
+)
+from ophyd_async.core.signal import observe_value
+from ophyd_async.core.utils import WatcherUpdate
 
 from ..signal.signal import epics_signal_r, epics_signal_rw, epics_signal_x
 
 
 class Motor(StandardReadable, Movable, Stoppable):
     """Device that moves a motor record"""
 
@@ -37,58 +44,50 @@
 
     def set_name(self, name: str):
         super().set_name(name)
         # Readback should be named the same as its parent in read()
         self.user_readback.set_name(name)
 
     async def _move(
-        self, new_position: float, watchers: Optional[List[Callable]] = None
-    ):
-        if watchers is None:
-            watchers = []
+        self, new_position: float
+    ) -> tuple[WatcherUpdate[float], AsyncStatus]:
         self._set_success = True
-        start = time.monotonic()
         old_position, units, precision = await asyncio.gather(
             self.user_setpoint.get_value(),
             self.motor_egu.get_value(),
             self.precision.get_value(),
         )
-
-        def update_watchers(current_position: float):
-            for watcher in watchers:
-                watcher(
-                    name=self.name,
-                    current=current_position,
-                    initial=old_position,
-                    target=new_position,
-                    unit=units,
-                    precision=precision,
-                    time_elapsed=time.monotonic() - start,
-                )
-
-        self.user_readback.subscribe_value(update_watchers)
-        try:
-            await self.user_setpoint.set(new_position)
-        finally:
-            self.user_readback.clear_sub(update_watchers)
+        move_status = self.user_setpoint.set(new_position, wait=True)
         if not self._set_success:
             raise RuntimeError("Motor was stopped")
+        return (
+            WatcherUpdate(
+                initial=old_position,
+                current=old_position,
+                target=new_position,
+                unit=units,
+                precision=precision,
+            ),
+            move_status,
+        )
 
-    def move(self, new_position: float, timeout: Optional[float] = None):
-        """Commandline only synchronous move of a Motor"""
-        from bluesky.run_engine import call_in_bluesky_event_loop, in_bluesky_event_loop
-
-        if in_bluesky_event_loop():
-            raise RuntimeError("Will deadlock run engine if run in a plan")
-        call_in_bluesky_event_loop(self._move(new_position), timeout)  # type: ignore
-
-    def set(self, new_position: float, timeout: Optional[float] = None) -> AsyncStatus:
-        watchers: List[Callable] = []
-        coro = asyncio.wait_for(self._move(new_position, watchers), timeout=timeout)
-        return AsyncStatus(coro, watchers)
+    @WatchableAsyncStatus.wrap
+    async def set(self, new_position: float, timeout: float | None = None):
+        update, move_status = await self._move(new_position)
+        async for current_position in observe_value(
+            self.user_readback, done_status=move_status
+        ):
+            if not self._set_success:
+                raise RuntimeError("Motor was stopped")
+            yield replace(
+                update,
+                name=self.name,
+                current=current_position,
+            )
 
     async def stop(self, success=False):
         self._set_success = success
         # Put with completion will never complete as we are waiting for completion on
         # the move above, so need to pass wait=False
-        status = self.motor_stop.trigger(wait=False)
-        await status
+        await self.motor_stop.trigger(wait=False)
+        # Trigger any callbacks
+        await self.user_readback._backend.put(await self.user_readback.get_value())
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/pvi/pvi.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/pvi/pvi.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 def _verify_common_blocks(entry: PVIEntry, common_device: Type[Device]):
     if not entry.sub_entries:
         return
     common_sub_devices = get_type_hints(common_device)
     for sub_name, sub_device in common_sub_devices.items():
-        if sub_name in ("_name", "parent"):
+        if sub_name.startswith("_") or sub_name == "parent":
             continue
         assert entry.sub_entries
         device_t, is_optional = _strip_union(sub_device)
         if sub_name not in entry.sub_entries and not is_optional:
             raise RuntimeError(
                 f"sub device `{sub_name}:{type(sub_device)}` " "was not provided by pvi"
             )
@@ -157,15 +157,15 @@
 
 
 def _mock_common_blocks(device: Device, stripped_type: Optional[Type] = None):
     device_t = stripped_type or type(device)
     sub_devices = (
         (field, field_type)
         for field, field_type in get_type_hints(device_t).items()
-        if field not in ("_name", "parent")
+        if not field.startswith("_") and field != "parent"
     )
 
     for device_name, device_cls in sub_devices:
         device_cls, _ = _strip_union(device_cls)
         is_device_vector, device_cls = _strip_device_vector(device_cls)
         device_cls, device_args = _split_subscript(device_cls)
         assert issubclass(device_cls, Device)
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/signal/_epics_transport.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/signal/_epics_transport.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/epics/signal/signal.py` & `ophyd_async-0.3a5/src/ophyd_async/epics/signal/signal.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/log.py` & `ophyd_async-0.3a5/src/ophyd_async/log.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/panda/__init__.py` & `ophyd_async-0.3a5/src/ophyd_async/panda/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/panda/_common_blocks.py` & `ophyd_async-0.3a5/src/ophyd_async/panda/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/panda/_hdf_panda.py` & `ophyd_async-0.3a5/src/ophyd_async/panda/_hdf_panda.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/panda/_panda_controller.py` & `ophyd_async-0.3a5/src/ophyd_async/panda/_panda_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/panda/_table.py` & `ophyd_async-0.3a5/src/ophyd_async/panda/_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/panda/_trigger.py` & `ophyd_async-0.3a5/src/ophyd_async/panda/_trigger.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/panda/writers/_hdf_writer.py` & `ophyd_async-0.3a5/src/ophyd_async/panda/writers/_hdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/panda/writers/_panda_hdf_file.py` & `ophyd_async-0.3a5/src/ophyd_async/panda/writers/_panda_hdf_file.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/planstubs/prepare_trigger_and_dets.py` & `ophyd_async-0.3a5/src/ophyd_async/planstubs/prepare_trigger_and_dets.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/protocols.py` & `ophyd_async-0.3a5/src/ophyd_async/protocols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,24 @@
+from __future__ import annotations
+
 from abc import abstractmethod
-from typing import Dict, Protocol, runtime_checkable
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Generic,
+    Protocol,
+    TypeVar,
+    runtime_checkable,
+)
 
 from bluesky.protocols import DataKey, HasName, Reading
 
-from ophyd_async.core.async_status import AsyncStatus
+if TYPE_CHECKING:
+    from ophyd_async.core.async_status import AsyncStatus
 
 
 @runtime_checkable
 class AsyncReadable(HasName, Protocol):
     @abstractmethod
     async def read(self) -> Dict[str, Reading]:
         """Return an OrderedDict mapping string field name(s) to dictionaries
@@ -90,7 +101,26 @@
     def unstage(self) -> AsyncStatus:
         """A hook for "cleaning up" the device after acquisition.
 
         It should return a ``Status`` that is marked done when the device is finished
         unstaging.
         """
         ...
+
+
+C = TypeVar("C", contravariant=True)
+
+
+class Watcher(Protocol, Generic[C]):
+    @staticmethod
+    def __call__(
+        *,
+        current: C,
+        initial: C,
+        target: C,
+        name: str | None,
+        unit: str | None,
+        precision: float | None,
+        fraction: float | None,
+        time_elapsed: float | None,
+        time_remaining: float | None,
+    ) -> Any: ...
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async/sim/pattern_generator.py` & `ophyd_async-0.3a5/src/ophyd_async/sim/pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_detector_control.py` & `ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_detector_control.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_detector_writer.py` & `ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_detector_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_generator.py` & `ophyd_async-0.3a5/src/ophyd_async/sim/sim_pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/src/ophyd_async.egg-info/PKG-INFO` & `ophyd_async-0.3a5/src/ophyd_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a4
+Version: 0.3a5
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async.egg-info/SOURCES.txt` & `ophyd_async-0.3a5/src/ophyd_async.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 src/ophyd_async/panda/_table.py
 src/ophyd_async/panda/_trigger.py
 src/ophyd_async/panda/_utils.py
 src/ophyd_async/panda/writers/__init__.py
 src/ophyd_async/panda/writers/_hdf_writer.py
 src/ophyd_async/panda/writers/_panda_hdf_file.py
 src/ophyd_async/planstubs/__init__.py
+src/ophyd_async/planstubs/ensure_connected.py
 src/ophyd_async/planstubs/prepare_trigger_and_dets.py
 src/ophyd_async/sim/__init__.py
 src/ophyd_async/sim/pattern_generator.py
 src/ophyd_async/sim/sim_pattern_detector_control.py
 src/ophyd_async/sim/sim_pattern_detector_writer.py
 src/ophyd_async/sim/sim_pattern_generator.py
 src/ophyd_async/sim/demo/__init__.py
@@ -156,14 +157,15 @@
 tests/core/test_device_save_loader.py
 tests/core/test_flyer.py
 tests/core/test_mock_signal_backend.py
 tests/core/test_signal.py
 tests/core/test_soft_signal_backend.py
 tests/core/test_standard_readable.py
 tests/core/test_utils.py
+tests/core/test_watchable_async_status.py
 tests/epics/test_pvi.py
 tests/epics/test_records.db
 tests/epics/test_signals.py
 tests/epics/_backend/test_common.py
 tests/epics/areadetector/__init__.py
 tests/epics/areadetector/test_aravis.py
 tests/epics/areadetector/test_controllers.py
```

### Comparing `ophyd_async-0.3a4/src/ophyd_async.egg-info/requires.txt` & `ophyd_async-0.3a5/src/ophyd_async.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/conftest.py` & `ophyd_async-0.3a5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/core/test_async_status.py` & `ophyd_async-0.3a5/tests/core/test_async_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,21 +46,25 @@
 
     await status
 
     assert status.exception() is None
 
 
 async def test_async_status_success_if_cancelled(normal_coroutine):
-    status = AsyncStatus(normal_coroutine())
+    coro = normal_coroutine()
+    status = AsyncStatus(coro)
     assert status.exception() is None
     status.task.cancel()
     with pytest.raises(asyncio.CancelledError):
         await status
     assert status.success is False
     assert isinstance(status.exception(), asyncio.CancelledError)
+    # asyncio will RuntimeWarning us about this never being awaited if we don't.
+    # RunEngine handled this as a special case
+    await coro
 
 
 async def coroutine_to_wrap(time: float):
     await asyncio.sleep(time)
 
 
 async def test_async_status_wrap() -> None:
@@ -118,15 +122,15 @@
             self._fail()
 
     def set(self, value) -> AsyncStatus:
         return AsyncStatus(self._set(value))
 
 
 async def test_status_propogates_traceback_under_RE(RE) -> None:
-    expected_call_stack = ["_set", "_fail"]
+    expected_call_stack = ["wait_for", "_set", "_fail"]
     d = FailingMovable()
     with pytest.raises(FailedStatus) as ctx:
         RE(bps.mv(d, 3))
     # We get "The above exception was the direct cause of the following exception:",
     # so extract that first exception traceback and check
     assert ctx.value.__cause__
     assert expected_call_stack == [
@@ -141,7 +145,45 @@
     ]
 
 
 async def test_async_status_exception_timeout():
     st = AsyncStatus(asyncio.sleep(0.1))
     with pytest.raises(Exception):
         st.exception(timeout=1.0)
+
+
+@pytest.fixture
+def loop():
+    return asyncio.get_event_loop()
+
+
+def test_asyncstatus_wraps_bare_func(loop):
+    async def do_test():
+        @AsyncStatus.wrap
+        async def coro_status():
+            await asyncio.sleep(0.01)
+
+        st = coro_status()
+        assert isinstance(st, AsyncStatus)
+        await asyncio.wait_for(st.task, None)
+        assert st.done
+
+    loop.run_until_complete(do_test())
+
+
+def test_asyncstatus_wraps_bare_func_with_args_kwargs(loop):
+    async def do_test():
+        test_result = 5
+
+        @AsyncStatus.wrap
+        async def coro_status(x: int, y: int, *, z=False):
+            await asyncio.sleep(0.01)
+            nonlocal test_result
+            test_result = x * y if z else 0
+
+        st = coro_status(3, 4, z=True)
+        assert isinstance(st, AsyncStatus)
+        await asyncio.wait_for(st.task, None)
+        assert st.done
+        assert test_result == 12
+
+    loop.run_until_complete(do_test())
```

### Comparing `ophyd_async-0.3a4/tests/core/test_device_collector.py` & `ophyd_async-0.3a5/tests/core/test_device_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 
 import pytest
 from bluesky import plan_stubs as bps
-from bluesky.run_engine import RunEngine, TransitionError
+from bluesky.run_engine import RunEngine
+from super_state_machine.errors import TransitionError
 
 from ophyd_async.core import DEFAULT_TIMEOUT, Device, DeviceCollector, NotConnected
 from ophyd_async.epics.motion import motor
 
 
 class FailingDevice(Device):
     async def connect(self, mock: bool = False, timeout=DEFAULT_TIMEOUT):
```

### Comparing `ophyd_async-0.3a4/tests/core/test_device_save_loader.py` & `ophyd_async-0.3a5/tests/core/test_device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/core/test_flyer.py` & `ophyd_async-0.3a5/tests/core/test_flyer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/core/test_mock_signal_backend.py` & `ophyd_async-0.3a5/tests/core/test_mock_signal_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,15 @@
     # If mock is false it will be handled like a normal signal, otherwise it will
     # initalize a new backend from the one in the line above
     await mock_signal.connect(mock=connect_mock_mode)
 
     assert await mock_signal._backend.get_value() == ""
     await mock_signal._backend.put("test")
     assert await mock_signal._backend.get_value() == "test"
-
-    mock_signal._backend.mock.get_value.assert_called_once
-
-    mock_signal._backend.mock["get_value"].assert_called_once
-    assert mock_signal._backend.mock.put.call_args_list == [
+    assert mock_signal._backend.put_mock.call_args_list == [
         call("test", wait=True, timeout=None),
     ]
 
 
 @pytest.mark.parametrize("epics_protocol", ["ca", "pva"])
 async def test_mock_signal_backend_source(epics_protocol):
     mock_signal_rw = epics_signal_rw(
```

### Comparing `ophyd_async-0.3a4/tests/core/test_signal.py` & `ophyd_async-0.3a5/tests/core/test_signal.py`

 * *Files 8% similar despite different names*

```diff
@@ -168,14 +168,23 @@
     set_mock_value(mock_signal, 888)
     dummy_reading = {
         "mock_signal": Reading({"alarm_severity": 0, "timestamp": ANY, "value": 888})
     }
     await assert_reading(mock_signal, dummy_reading)
 
 
+async def test_failed_assert_reaading(mock_signal: SignalRW):
+    set_mock_value(mock_signal, 888)
+    dummy_reading = {
+        "mock_signal": Reading({"alarm_severity": 0, "timestamp": ANY, "value": 88})
+    }
+    with pytest.raises(AssertionError):
+        await assert_reading(mock_signal, dummy_reading)
+
+
 class DummyReadable(StandardReadable):
     """A demo Readable to produce read and config signal"""
 
     def __init__(self, prefix: str, name="") -> None:
         # Define some signals
         with self.add_children_as_readables(HintedSignal):
             self.value = epics_signal_r(float, prefix + "Value")
```

### Comparing `ophyd_async-0.3a4/tests/core/test_soft_signal_backend.py` & `ophyd_async-0.3a5/tests/core/test_soft_signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/core/test_standard_readable.py` & `ophyd_async-0.3a5/tests/core/test_standard_readable.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/core/test_utils.py` & `ophyd_async-0.3a5/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/_backend/test_common.py` & `ophyd_async-0.3a5/tests/epics/_backend/test_common.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_aravis.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_aravis.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,66 +20,20 @@
 ) -> AravisDetector:
     async with DeviceCollector(mock=True):
         adaravis = AravisDetector("ADARAVIS:", static_directory_provider)
 
     return adaravis
 
 
-@pytest.mark.parametrize(
-    "model,pixel_format,deadtime",
-    [
-        ("Manta G-125", "Mono12Packed", 63e-6),
-        ("Manta G-125B", "Mono12Packed", 63e-6),
-        ("Manta G-125", "Mono8", 63e-6),
-        ("Manta G-125B", "Mono8", 63e-6),
-        ("Manta G-235", "Mono8", 118e-6),
-        ("Manta G-235B", "Mono8", 118e-6),
-        ("Manta G-235", "RGB8Packed", 390e-6),
-        ("Manta G-235B", "RGB8Packed", 390e-6),
-        ("Manta G-609", "", 47e-6),
-        ("Manta G-609", "foo", 47e-6),
-        ("Manta G-609", None, 47e-6),
-    ],
-)
-async def test_deadtime_fetched(
-    model: str,
-    pixel_format: str,
-    deadtime: float,
+@pytest.mark.parametrize("exposure_time", [0.0, 0.1, 1.0, 10.0, 100.0])
+async def test_deadtime_invariant_with_exposure_time(
+    exposure_time: float,
     adaravis: AravisDetector,
 ):
-    set_mock_value(adaravis.drv.model, model)
-    set_mock_value(adaravis.drv.pixel_format, pixel_format)
-
-    await adaravis.drv.fetch_deadtime()
-    # deadtime invariant with exposure time
-    assert adaravis.controller.get_deadtime(0) == deadtime
-    assert adaravis.controller.get_deadtime(500) == deadtime
-
-
-async def test_unknown_model_deadtime(
-    adaravis: AravisDetector,
-):
-    set_mock_value(adaravis.drv.model, "FOO")
-
-    with pytest.raises(ValueError, match="Model FOO does not have defined deadtimes"):
-        await adaravis.drv.fetch_deadtime()
-
-
-async def test_unknown_pixel_format_deadtime(
-    adaravis: AravisDetector,
-):
-    set_mock_value(adaravis.drv.model, "Manta G-235")
-    set_mock_value(adaravis.drv.pixel_format, "BAR")
-
-    with pytest.raises(
-        ValueError,
-        match="Model Manta G-235 does not have a defined deadtime "
-        "for pixel format BAR",
-    ):
-        await adaravis.drv.fetch_deadtime()
+    assert adaravis.controller.get_deadtime(exposure_time) == 1961e-6
 
 
 async def test_trigger_source_set_to_gpio_line(adaravis: AravisDetector):
     set_mock_value(adaravis.drv.trigger_source, "Freerun")
 
     async def trigger_and_complete():
         await adaravis.controller.arm(num=1, trigger=DetectorTrigger.edge_trigger)
@@ -187,15 +141,13 @@
             "dtype": "array",
             "external": "STREAM:",
         }
     }
 
 
 async def test_unsupported_trigger_excepts(adaravis: AravisDetector):
-    set_mock_value(adaravis.drv.model, "Manta G-125")
-    set_mock_value(adaravis.drv.pixel_format, "Mono12Packed")
     with pytest.raises(
         ValueError,
         # str(EnumClass.value) handling changed in Python 3.11
         match=r"AravisController only supports the following trigger types: .* but",
     ):
         await adaravis.prepare(TriggerInfo(1, DetectorTrigger.variable_gate, 1, 1))
```

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_controllers.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_controllers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_drivers.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_drivers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_kinetix.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_kinetix.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_pilatus.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_pilatus.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_scans.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_single_trigger_det.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_single_trigger_det.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_utils.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_vimba.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_vimba.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/areadetector/test_writers.py` & `ophyd_async-0.3a5/tests/epics/areadetector/test_writers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/demo/test_demo.py` & `ophyd_async-0.3a5/tests/epics/demo/test_demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,34 +64,57 @@
         mock_mover.stop_, lambda v, *args, **kwargs: callbacks.append(v)
     )
 
     await mock_mover.stop()
     assert callbacks == [None]
 
 
-class Watcher:
+class DemoWatcher:
     def __init__(self) -> None:
         self._event = asyncio.Event()
         self._mock = Mock()
 
-    def __call__(self, *args, **kwargs):
-        self._mock(*args, **kwargs)
+    def __call__(
+        self,
+        *args,
+        current: float,
+        initial: float,
+        target: float,
+        name: str | None = None,
+        unit: str | None = None,
+        precision: float | None = None,
+        fraction: float | None = None,
+        time_elapsed: float | None = None,
+        time_remaining: float | None = None,
+        **kwargs,
+    ):
+        self._mock(
+            *args,
+            current=current,
+            initial=initial,
+            target=target,
+            name=name,
+            unit=unit,
+            precision=precision,
+            time_elapsed=time_elapsed,
+            **kwargs,
+        )
         self._event.set()
 
     async def wait_for_call(self, *args, **kwargs):
         await asyncio.wait_for(self._event.wait(), timeout=1)
         assert self._mock.call_count == 1
         assert self._mock.call_args == call(*args, **kwargs)
         self._mock.reset_mock()
         self._event.clear()
 
 
 async def test_mover_moving_well(mock_mover: demo.Mover) -> None:
     s = mock_mover.set(0.55)
-    watcher = Watcher()
+    watcher = DemoWatcher()
     s.watch(watcher)
     done = Mock()
     s.add_callback(done)
     await watcher.wait_for_call(
         name="mock_mover",
         current=0.0,
         initial=0.0,
@@ -244,26 +267,14 @@
     assert await thing.x.velocity.get_value() == 456
     thing.set_name("foo")
     assert thing.x.name == "foo-x"
     assert thing.x.velocity.name == "foo-x-velocity"
     assert thing.x.stop_.name == "foo-x-stop"
 
 
-def test_mover_in_re(mock_mover: demo.Mover, RE) -> None:
-    mock_mover.move(0)
-
-    def my_plan():
-        mock_mover.move(0)
-        return
-        yield
-
-    with pytest.raises(RuntimeError, match="Will deadlock run engine if run in a plan"):
-        RE(my_plan())
-
-
 async def test_dynamic_sensor_group_disconnected():
     with pytest.raises(NotConnected):
         async with DeviceCollector(timeout=0.1):
             mock_sensor_group_dynamic = demo.SensorGroup("MOCK:SENSOR:")
 
     assert mock_sensor_group_dynamic.name == "mock_sensor_group_dynamic"
```

### Comparing `ophyd_async-0.3a4/tests/epics/demo/test_demo_ad_sim_detector.py` & `ophyd_async-0.3a5/tests/epics/demo/test_demo_ad_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/motion/test_motor.py` & `ophyd_async-0.3a5/tests/epics/motion/test_motor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import time
 from typing import Dict
 from unittest.mock import Mock, call
 
 import pytest
 from bluesky.protocols import Reading
 
 from ophyd_async.core import (
@@ -10,35 +11,84 @@
     set_mock_put_proceeds,
     set_mock_value,
 )
 from ophyd_async.epics.motion import motor
 
 # Long enough for multiple asyncio event loop cycles to run so
 # all the tasks have a chance to run
-A_BIT = 0.01
+A_BIT = 0.001
 
 
 @pytest.fixture
 async def sim_motor():
     async with DeviceCollector(mock=True):
         sim_motor = motor.Motor("BLxxI-MO-TABLE-01:X", name="sim_motor")
 
     set_mock_value(sim_motor.motor_egu, "mm")
     set_mock_value(sim_motor.precision, 3)
     set_mock_value(sim_motor.velocity, 1)
     yield sim_motor
 
 
+async def wait_for_eq(item, attribute, comparison, timeout):
+    timeout_time = time.monotonic() + timeout
+    while getattr(item, attribute) != comparison:
+        await asyncio.sleep(A_BIT)
+        if time.monotonic() > timeout_time:
+            raise TimeoutError
+
+
 async def test_motor_moving_well(sim_motor: motor.Motor) -> None:
     set_mock_put_proceeds(sim_motor.user_setpoint, False)
     s = sim_motor.set(0.55)
     watcher = Mock()
     s.watch(watcher)
     done = Mock()
     s.add_callback(done)
+    await wait_for_eq(watcher, "call_count", 1, 1)
+    assert watcher.call_args == call(
+        name="sim_motor",
+        current=0.0,
+        initial=0.0,
+        target=0.55,
+        unit="mm",
+        precision=3,
+        time_elapsed=pytest.approx(0.0, abs=0.05),
+    )
+    watcher.reset_mock()
+    assert 0.55 == await sim_motor.user_setpoint.get_value()
+    assert not s.done
+    await asyncio.sleep(0.1)
+    set_mock_value(sim_motor.user_readback, 0.1)
+    await wait_for_eq(watcher, "call_count", 1, 1)
+    assert watcher.call_count == 1
+    assert watcher.call_args == call(
+        name="sim_motor",
+        current=0.1,
+        initial=0.0,
+        target=0.55,
+        unit="mm",
+        precision=3,
+        time_elapsed=pytest.approx(0.1, abs=0.05),
+    )
+    set_mock_value(sim_motor.motor_done_move, True)
+    set_mock_value(sim_motor.user_readback, 0.55)
+    set_mock_put_proceeds(sim_motor.user_setpoint, True)
+    await asyncio.sleep(A_BIT)
+    await wait_for_eq(s, "done", True, 1)
+    done.assert_called_once_with(s)
+
+
+async def test_motor_moving_well_2(sim_motor: motor.Motor) -> None:
+    set_mock_put_proceeds(sim_motor.user_setpoint, False)
+    s = sim_motor.set(0.55)
+    watcher = Mock()
+    s.watch(watcher)
+    done = Mock()
+    s.add_callback(done)
     await asyncio.sleep(A_BIT)
     assert watcher.call_count == 1
     assert watcher.call_args == call(
         name="sim_motor",
         current=0.0,
         initial=0.0,
         target=0.55,
@@ -47,14 +97,15 @@
         time_elapsed=pytest.approx(0.0, abs=0.05),
     )
     watcher.reset_mock()
     assert 0.55 == await sim_motor.user_setpoint.get_value()
     assert not s.done
     await asyncio.sleep(0.1)
     set_mock_value(sim_motor.user_readback, 0.1)
+    await asyncio.sleep(0.1)
     assert watcher.call_count == 1
     assert watcher.call_args == call(
         name="sim_motor",
         current=0.1,
         initial=0.0,
         target=0.55,
         unit="mm",
@@ -64,14 +115,15 @@
     set_mock_put_proceeds(sim_motor.user_setpoint, True)
     await asyncio.sleep(A_BIT)
     assert s.done
     done.assert_called_once_with(s)
 
 
 async def test_motor_moving_stopped(sim_motor: motor.Motor):
+    set_mock_value(sim_motor.motor_done_move, False)
     set_mock_put_proceeds(sim_motor.user_setpoint, False)
     s = sim_motor.set(1.5)
     s.add_callback(Mock())
     await asyncio.sleep(0.2)
     assert not s.done
     await sim_motor.stop()
     set_mock_put_proceeds(sim_motor.user_setpoint, True)
@@ -103,19 +155,7 @@
     assert (await q.get())["sim_motor-velocity"]["value"] == 1.0
     await v.set(2.0)
     assert (await q.get())["sim_motor-velocity"]["value"] == 2.0
     v.clear_sub(q.put_nowait)
     await v.set(3.0)
     assert (await v.read())["sim_motor-velocity"]["value"] == 3.0
     assert q.empty()
-
-
-def test_motor_in_re(sim_motor: motor.Motor, RE) -> None:
-    sim_motor.move(0)
-
-    def my_plan():
-        sim_motor.move(0)
-        return
-        yield
-
-    with pytest.raises(RuntimeError, match="Will deadlock run engine if run in a plan"):
-        RE(my_plan())
```

### Comparing `ophyd_async-0.3a4/tests/epics/test_pvi.py` & `ophyd_async-0.3a5/tests/epics/test_pvi.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/test_records.db` & `ophyd_async-0.3a5/tests/epics/test_records.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/epics/test_signals.py` & `ophyd_async-0.3a5/tests/epics/test_signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/panda/db/panda.db` & `ophyd_async-0.3a5/tests/panda/db/panda.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/panda/test_hdf_panda.py` & `ophyd_async-0.3a5/tests/panda/test_hdf_panda.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/panda/test_panda_connect.py` & `ophyd_async-0.3a5/tests/panda/test_panda_connect.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/panda/test_panda_controller.py` & `ophyd_async-0.3a5/tests/panda/test_panda_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/panda/test_panda_utils.py` & `ophyd_async-0.3a5/tests/panda/test_panda_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/panda/test_table.py` & `ophyd_async-0.3a5/tests/panda/test_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/panda/test_trigger.py` & `ophyd_async-0.3a5/tests/panda/test_trigger.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/panda/test_writer.py` & `ophyd_async-0.3a5/tests/panda/test_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/protocols/test_protocols.py` & `ophyd_async-0.3a5/tests/protocols/test_protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/sim/demo/test_sim_motor.py` & `ophyd_async-0.3a5/tests/sim/demo/test_sim_motor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import asyncio
 import time
 
 from bluesky.plans import spiral_square
 from bluesky.run_engine import RunEngine
 
+from ophyd_async.core.async_status import AsyncStatusBase
 from ophyd_async.core.device import DeviceCollector
 from ophyd_async.sim.demo.sim_motor import SimMotor
 
 
 async def test_move_sim_in_plan():
     RE = RunEngine()
 
     async with DeviceCollector():
-        m1 = SimMotor("M1", "sim_motor1")
-        m2 = SimMotor("M2", "sim_motor2")
+        m1 = SimMotor("M1")
+        m2 = SimMotor("M2")
 
     my_plan = spiral_square([], m1, m2, 0, 0, 4, 4, 10, 10)
 
     RE(my_plan)
 
     assert await m1.user_readback.get_value() == -2
     assert await m2.user_readback.get_value() == -2
@@ -40,17 +41,20 @@
 
 async def test_stop():
     async with DeviceCollector():
         m1 = SimMotor("M1", instant=False)
 
     # this move should take 10 seconds but we will stop it after 0.2
     move_status = m1.set(10)
+    while not m1._move_status:
+        # wait to actually get the move started
+        await asyncio.sleep(0)
     await asyncio.sleep(0.2)
     m1.stop()
-
+    await asyncio.sleep(0)
     new_pos = await m1.user_readback.get_value()
 
     assert move_status.done
     # move should not be successful as we stopped it
     assert not move_status.success
     assert new_pos < 10
     assert new_pos >= 0.1
@@ -66,20 +70,20 @@
     async with DeviceCollector():
         m1 = SimMotor("M1", instant=False)
 
     # do a 10 sec move that will timeout before arriving
     move_status = m1.set(10, timeout=0.1)
     await asyncio.sleep(0.2)
 
-    # verify status of inner task set up to run _move.update_position()
-    assert isinstance(m1._move_task, asyncio.Task)
-    assert m1._move_task.done
-    assert m1._move_task.cancelled
-
-    # verify status of outer task set up to run _move()
-    assert move_status.task.done
+    # check inner status
+    assert m1._move_status is not None
+    assert m1._move_status.done
+    assert not move_status.success
     assert move_status.task.cancelled
 
-    new_pos = await m1.user_readback.get_value()
-    assert new_pos < 10
+    # check outer status
+    assert isinstance(move_status, AsyncStatusBase)
     assert move_status.done
     assert not move_status.success
+    assert move_status.task.cancelled
+    new_pos = await m1.user_readback.get_value()
+    assert new_pos < 10
```

### Comparing `ophyd_async-0.3a4/tests/sim/test_pattern_generator.py` & `ophyd_async-0.3a5/tests/sim/test_pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/sim/test_sim_detector.py` & `ophyd_async-0.3a5/tests/sim/test_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/sim/test_sim_writer.py` & `ophyd_async-0.3a5/tests/sim/test_sim_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/sim/test_streaming_plan.py` & `ophyd_async-0.3a5/tests/sim/test_streaming_plan.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/test_flyer_with_panda.py` & `ophyd_async-0.3a5/tests/test_flyer_with_panda.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a4/tests/test_log.py` & `ophyd_async-0.3a5/tests/test_log.py`

 * *Files identical despite different names*

