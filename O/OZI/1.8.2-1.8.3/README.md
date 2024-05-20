# Comparing `tmp/OZI-1.8.2.tar.gz` & `tmp/OZI-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.8.2.tar", last modified: Sun May 19 22:29:41 2024, max compression
+gzip compressed data, was "OZI-1.8.3.tar", last modified: Sun May 19 23:17:52 2024, max compression
```

## Comparing `OZI-1.8.2.tar` & `OZI-1.8.3.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.671870 OZI-1.8.2/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.643869 OZI-1.8.2/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.643869 OZI-1.8.2/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.647869 OZI-1.8.2/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2901 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-19 22:26:36.000000 OZI-1.8.2/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-19 22:26:36.000000 OZI-1.8.2/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   312885 2024-05-19 22:26:36.000000 OZI-1.8.2/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-19 22:26:36.000000 OZI-1.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-19 22:29:25.439869 OZI-1.8.2/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6969 2024-05-19 22:26:36.000000 OZI-1.8.2/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    17469 2024-05-19 22:26:36.000000 OZI-1.8.2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7549 2024-05-19 22:26:36.000000 OZI-1.8.2/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.667870 OZI-1.8.2/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5880 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.655870 OZI-1.8.2/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.655870 OZI-1.8.2/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.655870 OZI-1.8.2/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.655870 OZI-1.8.2/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4097 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6391 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.659870 OZI-1.8.2/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.659870 OZI-1.8.2/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.659870 OZI-1.8.2/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.659870 OZI-1.8.2/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.659870 OZI-1.8.2/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.659870 OZI-1.8.2/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.659870 OZI-1.8.2/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.659870 OZI-1.8.2/ozi/lint/readme-renderer/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/readme-renderer/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       19 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/lint/readme-renderer/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.663869 OZI-1.8.2/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4745 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6940 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.663869 OZI-1.8.2/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.667870 OZI-1.8.2/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      503 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2501 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6164 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4480 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4564 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.667870 OZI-1.8.2/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.667870 OZI-1.8.2/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.667870 OZI-1.8.2/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.671870 OZI-1.8.2/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.671870 OZI-1.8.2/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-19 22:26:36.000000 OZI-1.8.2/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10976 2024-05-19 22:26:36.000000 OZI-1.8.2/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-05-19 22:26:36.000000 OZI-1.8.2/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.671870 OZI-1.8.2/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-19 22:26:36.000000 OZI-1.8.2/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:29:25.675870 OZI-1.8.2/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-19 22:26:36.000000 OZI-1.8.2/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-19 22:26:36.000000 OZI-1.8.2/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14348 2024-05-19 22:26:36.000000 OZI-1.8.2/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-19 22:26:36.000000 OZI-1.8.2/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.559202 OZI-1.8.3/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.531201 OZI-1.8.3/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.531201 OZI-1.8.3/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.531201 OZI-1.8.3/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2901 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-19 23:14:37.000000 OZI-1.8.3/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-19 23:14:37.000000 OZI-1.8.3/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   313133 2024-05-19 23:14:37.000000 OZI-1.8.3/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-19 23:14:37.000000 OZI-1.8.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-19 23:17:35.327201 OZI-1.8.3/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6969 2024-05-19 23:14:37.000000 OZI-1.8.3/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    17469 2024-05-19 23:14:37.000000 OZI-1.8.3/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7549 2024-05-19 23:14:37.000000 OZI-1.8.3/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.555202 OZI-1.8.3/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5880 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.543202 OZI-1.8.3/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.539202 OZI-1.8.3/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.543202 OZI-1.8.3/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.543202 OZI-1.8.3/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4097 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6391 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.547201 OZI-1.8.3/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.543202 OZI-1.8.3/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.543202 OZI-1.8.3/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.543202 OZI-1.8.3/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.547201 OZI-1.8.3/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.547201 OZI-1.8.3/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.547201 OZI-1.8.3/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.547201 OZI-1.8.3/ozi/lint/readme-renderer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/readme-renderer/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       19 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/lint/readme-renderer/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.547201 OZI-1.8.3/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4745 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6940 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.551202 OZI-1.8.3/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.555202 OZI-1.8.3/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      503 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2513 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6164 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4480 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4564 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.555202 OZI-1.8.3/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.555202 OZI-1.8.3/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.555202 OZI-1.8.3/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.559202 OZI-1.8.3/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.559202 OZI-1.8.3/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-19 23:14:37.000000 OZI-1.8.3/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10976 2024-05-19 23:14:37.000000 OZI-1.8.3/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-05-19 23:14:37.000000 OZI-1.8.3/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.559202 OZI-1.8.3/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-19 23:14:37.000000 OZI-1.8.3/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:17:35.559202 OZI-1.8.3/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-19 23:14:37.000000 OZI-1.8.3/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-19 23:14:37.000000 OZI-1.8.3/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14348 2024-05-19 23:14:37.000000 OZI-1.8.3/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-19 23:14:37.000000 OZI-1.8.3/tests/test_tap.py
```

### Comparing `OZI-1.8.2/.github/CODEOWNERS` & `OZI-1.8.3/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/CODE_OF_CONDUCT.md` & `OZI-1.8.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/CONTRIBUTING.md` & `OZI-1.8.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.8.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.8.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/SECURITY.md` & `OZI-1.8.3/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/workflows/codeql.yml` & `OZI-1.8.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/workflows/dependency-review.yml` & `OZI-1.8.3/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/workflows/dev-workflow.yml` & `OZI-1.8.3/.github/workflows/dev-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/workflows/dist-workflow.yml` & `OZI-1.8.3/.github/workflows/dist-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.github/workflows/scorecard.yml` & `OZI-1.8.3/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/.gitignore` & `OZI-1.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/CHANGELOG.md` & `OZI-1.8.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,16 @@
 # CHANGELOG
+## 1.8.3 (2024-05-19)
+
+### :bug:
+
+* :bug: fix unimplemented repr in ``ozi.spec.base.Default``
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`e7791d0`](https://github.com/OZI-Project/OZI/commit/e7791d017cf770d47fe847bc8d949d634e81ce95))
+
 ## 1.8.2 (2024-05-19)
 
 ### :children_crossing:
 
 * :children_crossing: truncated ``ozi.spec`` repr. ([`a5a3bd6`](https://github.com/OZI-Project/OZI/commit/a5a3bd605c33aad9c0431ff1ac983f8e32357634))
 
 ## 1.8.1 (2024-05-18)
```

### Comparing `OZI-1.8.2/LICENSE.txt` & `OZI-1.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/PKG-INFO` & `OZI-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.8.2
+Version: 1.8.3
 Summary: Package Python projects with Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.8.2.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.8.3.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
```

### Comparing `OZI-1.8.2/README.rst` & `OZI-1.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/meson.build` & `OZI-1.8.3/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/meson.options` & `OZI-1.8.3/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/__main__.py` & `OZI-1.8.3/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/actions.py` & `OZI-1.8.3/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/comment.py` & `OZI-1.8.3/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/fix/__main__.py` & `OZI-1.8.3/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/fix/build_definition.py` & `OZI-1.8.3/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/fix/meson.build` & `OZI-1.8.3/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/fix/missing.py` & `OZI-1.8.3/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/fix/parser.py` & `OZI-1.8.3/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/fix/rewrite_command.py` & `OZI-1.8.3/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/lint/meson.build` & `OZI-1.8.3/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/lint/pyright/meson.build` & `OZI-1.8.3/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/meson.build` & `OZI-1.8.3/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/meson.py` & `OZI-1.8.3/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/new/__main__.py` & `OZI-1.8.3/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/new/meson.build` & `OZI-1.8.3/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/new/parser.py` & `OZI-1.8.3/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/new/validate.py` & `OZI-1.8.3/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/pkg_extra.py` & `OZI-1.8.3/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/render.py` & `OZI-1.8.3/ozi/render.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/scripts/core_metadata_template.py` & `OZI-1.8.3/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/scripts/meson.build` & `OZI-1.8.3/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.8.3/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.8.3/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/scripts/render_requirements.py` & `OZI-1.8.3/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.8.3/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/scripts/scm_version_snip.py` & `OZI-1.8.3/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/scripts/to_distribution_template.py` & `OZI-1.8.3/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/scripts/version_metadata_template.py` & `OZI-1.8.3/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/spdx.py` & `OZI-1.8.3/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/spec/_license.py` & `OZI-1.8.3/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/spec/_spec.py` & `OZI-1.8.3/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/spec/base.py` & `OZI-1.8.3/ozi/spec/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     __dataclass_fields__: ClassVar[dict[str, _VT]]
 
     def asdict(self: Self) -> dict[str, _VT]: ...
 
     def __call__(self: Self) -> _FactoryMethod: ...
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class Default(_FactoryDataclass):
     """A dataclass that, when called, returns it's own default factory method."""
 
     def __call__(self: Self) -> _FactoryMethod:  # pragma: defer to python
         return field(default_factory=lambda: self())
 
     def asdict(self: Self) -> dict[str, _VT]:
```

### Comparing `OZI-1.8.2/ozi/spec/ci.py` & `OZI-1.8.3/ozi/spec/ci.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/spec/meson.build` & `OZI-1.8.3/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/spec/pkg.py` & `OZI-1.8.3/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/spec/project.py` & `OZI-1.8.3/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/spec/python.py` & `OZI-1.8.3/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/spec/src.py` & `OZI-1.8.3/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/tap.py` & `OZI-1.8.3/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/trove.py` & `OZI-1.8.3/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/vendor/email_validator/__init__.py` & `OZI-1.8.3/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/vendor/email_validator/__main__.py` & `OZI-1.8.3/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/vendor/email_validator/deliverability.py` & `OZI-1.8.3/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.8.3/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/vendor/email_validator/meson.build` & `OZI-1.8.3/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.8.3/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/vendor/email_validator/syntax.py` & `OZI-1.8.3/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/vendor/email_validator/validate_email.py` & `OZI-1.8.3/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/ozi/vendor/meson.build` & `OZI-1.8.3/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/pyproject.toml` & `OZI-1.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/templates/CHANGELOG.md.j2` & `OZI-1.8.3/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/tests/meson.build` & `OZI-1.8.3/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/tests/test_ozi_fix.py` & `OZI-1.8.3/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/tests/test_ozi_new.py` & `OZI-1.8.3/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.8.2/tests/test_tap.py` & `OZI-1.8.3/tests/test_tap.py`

 * *Files identical despite different names*

