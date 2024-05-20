# Comparing `tmp/fortls-3.0.0rc6.tar.gz` & `tmp/fortls-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortls-3.0.0rc6.tar", last modified: Fri May 10 13:31:50 2024, max compression
+gzip compressed data, was "fortls-3.1.0.tar", last modified: Mon May 20 01:04:48 2024, max compression
```

## Comparing `fortls-3.0.0rc6.tar` & `fortls-3.1.0.tar`

### file list

```diff
@@ -1,259 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.805577 fortls-3.0.0rc6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.805577 fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.805577 fortls-3.0.0rc6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/docs_preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.github/workflows/update-intrinsics.yml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    41497 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.809577 fortls-3.0.0rc6/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.809577 fortls-3.0.0rc6/assets/animations/
--rw-r--r--   0 runner    (1001) docker     (127)  1647490 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/animations/intro-demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/f.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/logo2-animated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    78094 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/logos.workspace.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.821576 fortls-3.0.0rc6/assets/lsp/
--rw-r--r--   0 runner    (1001) docker     (127)   791746 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/completion-ani.gif
--rw-r--r--   0 runner    (1001) docker     (127)   450880 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/completion-ani.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/completion.png
--rw-r--r--   0 runner    (1001) docker     (127)   597393 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/definition-goto.gif
--rw-r--r--   0 runner    (1001) docker     (127)   335329 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/definition-goto.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/definition-peek.png
--rw-r--r--   0 runner    (1001) docker     (127)    49007 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/diagnostics1.png
--rw-r--r--   0 runner    (1001) docker     (127)    43464 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/doc-highlight.png
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/hover.png
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/hover2.png
--rw-r--r--   0 runner    (1001) docker     (127)    65080 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/references-peek.png
--rw-r--r--   0 runner    (1001) docker     (127)   703611 2024-05-10 13:31:44.000000 fortls-3.0.0rc6/assets/lsp/rename.gif
--rw-r--r--   0 runner    (1001) docker     (127)   355841 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/rename.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   304764 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/rename2.gif
--rw-r--r--   0 runner    (1001) docker     (127)   151579 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/rename2.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   628798 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/sig-help.gif
--rw-r--r--   0 runner    (1001) docker     (127)   418094 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/sig-help.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    50499 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/symbols-crop.png
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/symbols-doc.png
--rw-r--r--   0 runner    (1001) docker     (127)    25726 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/symbols-workspace.png
--rw-r--r--   0 runner    (1001) docker     (127)    54934 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/lsp/symbols.png
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/assets/symbol-class.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.821576 fortls-3.0.0rc6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/editor_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/fortls.parsers.internal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/fortls.parsers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/fortls.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.825576 fortls-3.0.0rc6/docs/html_extra/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/html_extra/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/html_extra/google3e426562ce42e98f.html
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/html_extra/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/options.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.825576 fortls-3.0.0rc6/fortls/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/fortls.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/ftypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/json_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/jsonrpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    74006 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/langserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.829576 fortls-3.0.0rc6/fortls/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.833576 fortls-3.0.0rc6/fortls/parsers/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/associate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12267 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/do.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/if_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    72890 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.modules.json
--rw-r--r--   0 runner    (1001) docker     (127)    44156 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)   630782 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.procedures.markdown.json
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/intrinsics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/keywords.json
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    86115 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/statements.json
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/subroutine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/use.py
--rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/parsers/internal/where.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/regex_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/fortls/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/fortls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 13:31:50.000000 fortls-3.0.0rc6/fortls.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.833576 fortls-3.0.0rc6/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/licenses/fortran-language-server-license.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.837576 fortls-3.0.0rc6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/setup_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_preproc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_regex_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26297 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_hover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_server_signature_help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.837576 fortls-3.0.0rc6/test/test_source/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/.fortls
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.837576 fortls-3.0.0rc6/test/test_source/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/completion/test_vis_mod_completion.f90
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/completion/use_only_interface.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.841576 fortls-3.0.0rc6/test/test_source/diag/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/conf_long_lines.json
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_contains.f90
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_critical.f90
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_enum.f90
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_external.f90
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_forall.f90
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_function.f90
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_function_arg_list.f90
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_implicit_none.f90
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_lines.f90
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_scope_end_name_var.f90
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_scope_overreach.f90
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_semicolon.f90
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_use_ordering.f90
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_var_shadowing_keyword_arg.f90
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_variable.f90
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_visibility.f90
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/diag/test_where.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.841576 fortls-3.0.0rc6/test/test_source/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/docs/test_doxygen.f90
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/docs/test_ford.f90
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/docs/test_module_and_type_doc.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.801577 fortls-3.0.0rc6/test/test_source/excldir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.841576 fortls-3.0.0rc6/test/test_source/excldir/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/excldir/sub1/tmp.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.841576 fortls-3.0.0rc6/test/test_source/excldir/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/excldir/sub2/fake2.f90
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/f90_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/hover/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/associate_block.f90
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/associate_block_2.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/functions.f90
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/intent.f90
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/parameters.f90
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/pointers.f90
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/recursive.f90
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/spaced_keywords.f90
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/hover/types.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/imp/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/imp/import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/imp/submodule.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/include/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/include/empty.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/parse/line_continuations.f90
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/parse/submodule.f90
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/parse/test_incomplete_dims.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/parse/test_kinds_and_dims.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/pp/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/.fortls
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/.pp_conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/pp/include/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/include/petscerror.h
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/include/petscpc.h
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc.F90
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_elif.F90
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_elif_elif_skip.F90
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_else.F90
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_if_elif_else.F90
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_if_elif_skip.F90
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/pp/preproc_keywords.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/rename/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/rename/test_rename_imp_type_bound_proc.f90
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/rename/test_rename_intrinsic.f90
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/rename/test_rename_nested.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.845576 fortls-3.0.0rc6/test/test_source/signature/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/signature/help.f90
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/signature/nested_sigs.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/test/test_source/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_abstract.f90
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_fixed.f
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_free.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_generic.f90
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_inc2.f90
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_inherit.f90
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_rename.F90
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_select.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_submod.F90
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/subdir/test_vis.f90
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test.f90
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_block.f08
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_diagnostic_int.f90
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_inc.f90
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_nonintrinsic.f90
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_prog.f08
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/test_submodule.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/test/test_source/use/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/use/use.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:50.849576 fortls-3.0.0rc6/test/test_source/vis/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/vis/private.f90
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 13:31:45.000000 fortls-3.0.0rc6/test/test_source/wrong_syntax.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.880902 fortls-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 01:04:40.000000 fortls-3.1.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.832902 fortls-3.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.836902 fortls-3.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.836902 fortls-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/workflows/docs_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 01:04:40.000000 fortls-3.1.0/.github/workflows/update-intrinsics.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-20 01:04:40.000000 fortls-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-20 01:04:40.000000 fortls-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42183 2024-05-20 01:04:40.000000 fortls-3.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-20 01:04:40.000000 fortls-3.1.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-20 01:04:40.000000 fortls-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-20 01:04:40.000000 fortls-3.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-20 01:04:40.000000 fortls-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12635 2024-05-20 01:04:48.880902 fortls-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-05-20 01:04:40.000000 fortls-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-20 01:04:40.000000 fortls-3.1.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.836902 fortls-3.1.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.836902 fortls-3.1.0/assets/animations/
+-rw-r--r--   0 runner    (1001) docker     (127)  1647490 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/animations/intro-demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/f.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/logo2-animated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    78094 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/logos.workspace.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.848902 fortls-3.1.0/assets/lsp/
+-rw-r--r--   0 runner    (1001) docker     (127)   791746 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/completion-ani.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   450880 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/completion-ani.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/completion.png
+-rw-r--r--   0 runner    (1001) docker     (127)   597393 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/definition-goto.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   335329 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/definition-goto.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/definition-peek.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49007 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/diagnostics1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43464 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/doc-highlight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/hover2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65080 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/references-peek.png
+-rw-r--r--   0 runner    (1001) docker     (127)   703611 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/rename.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   355841 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/rename.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   304764 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/rename2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   151579 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/rename2.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   628798 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/sig-help.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   418094 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/sig-help.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    50499 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/symbols-crop.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/symbols-doc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25726 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/symbols-workspace.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54934 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/lsp/symbols.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 01:04:40.000000 fortls-3.1.0/assets/symbol-class.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.852902 fortls-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/editor_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/fortls.parsers.internal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/fortls.parsers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/fortls.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.852902 fortls-3.1.0/docs/html_extra/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/html_extra/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/html_extra/google3e426562ce42e98f.html
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/html_extra/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-20 01:04:40.000000 fortls-3.1.0/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.852902 fortls-3.1.0/fortls/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 01:04:48.000000 fortls-3.1.0/fortls/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/fortls.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/ftypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18350 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/json_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/jsonrpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74006 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/langserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.856902 fortls-3.1.0/fortls/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.860902 fortls-3.1.0/fortls/parsers/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/do.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/if_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72890 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/intrinsic.modules.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44156 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/intrinsic.procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)   630782 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/intrinsic.procedures.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/intrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/keywords.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86113 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/statements.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/subroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/use.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/parsers/internal/where.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/regex_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-20 01:04:40.000000 fortls-3.1.0/fortls/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.876902 fortls-3.1.0/fortls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12635 2024-05-20 01:04:48.000000 fortls-3.1.0/fortls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-05-20 01:04:48.000000 fortls-3.1.0/fortls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:04:48.000000 fortls-3.1.0/fortls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-20 01:04:48.000000 fortls-3.1.0/fortls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-20 01:04:48.000000 fortls-3.1.0/fortls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 01:04:48.000000 fortls-3.1.0/fortls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.860902 fortls-3.1.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-20 01:04:40.000000 fortls-3.1.0/licenses/fortran-language-server-license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-20 01:04:40.000000 fortls-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 01:04:48.880902 fortls-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 01:04:40.000000 fortls-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.864902 fortls-3.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-20 01:04:40.000000 fortls-3.1.0/test/setup_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_preproc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_regex_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27422 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_hover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_server_signature_help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.864902 fortls-3.1.0/test/test_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/.fortls
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.864902 fortls-3.1.0/test/test_source/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/completion/test_vis_mod_completion.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/completion/use_only_interface.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.868902 fortls-3.1.0/test/test_source/diag/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/conf_long_lines.json
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_contains.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_critical.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_enum.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_external.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_forall.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_function.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_function_arg_list.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_implicit_none.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_lines.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_scope_end_name_var.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_scope_overreach.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_semicolon.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_use_ordering.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_var_shadowing_keyword_arg.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_variable.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_visibility.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/diag/test_where.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.868902 fortls-3.1.0/test/test_source/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/docs/test_doxygen.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/docs/test_ford.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/docs/test_module_and_type_doc.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.828902 fortls-3.1.0/test/test_source/excldir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.868902 fortls-3.1.0/test/test_source/excldir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/excldir/sub1/tmp.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.868902 fortls-3.1.0/test/test_source/excldir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/excldir/sub2/fake2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/f90_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.872902 fortls-3.1.0/test/test_source/hover/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/associate_block.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/associate_block_2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/complicated_kind_spec.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/functions.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/intent.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/multiline_lexical_tokens.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/parameters.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/pointers.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/recursive.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/spaced_keywords.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/hover/types.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.872902 fortls-3.1.0/test/test_source/imp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/imp/import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/imp/submodule.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.872902 fortls-3.1.0/test/test_source/include/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/include/empty.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.872902 fortls-3.1.0/test/test_source/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/parse/.fortls
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/parse/line_continuations.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.872902 fortls-3.1.0/test/test_source/parse/mixed/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/parse/mixed/multilines.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/parse/mixed/preproc_and_normal_syntax.F90
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/parse/submodule.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/parse/test_incomplete_dims.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/parse/test_kinds_and_dims.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/parse/trailing_semicolon.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.872902 fortls-3.1.0/test/test_source/pp/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/.fortls
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/.pp_conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.872902 fortls-3.1.0/test/test_source/pp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/include/petscerror.h
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/include/petscpc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/preproc.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/preproc_elif.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/preproc_elif_elif_skip.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/preproc_else.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/preproc_if_elif_else.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/preproc_if_elif_skip.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/pp/preproc_keywords.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.876902 fortls-3.1.0/test/test_source/rename/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/rename/test_rename_imp_type_bound_proc.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/rename/test_rename_intrinsic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/rename/test_rename_nested.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.876902 fortls-3.1.0/test/test_source/signature/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/signature/help.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/signature/nested_sigs.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.876902 fortls-3.1.0/test/test_source/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_abstract.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_fixed.f
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_free.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_generic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_inc2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_inherit.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_rename.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_select.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_submod.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/subdir/test_vis.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/test.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/test_block.f08
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/test_diagnostic_int.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/test_import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/test_inc.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/test_nonintrinsic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/test_prog.f08
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/test_submodule.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.876902 fortls-3.1.0/test/test_source/use/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/use/use.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:04:48.876902 fortls-3.1.0/test/test_source/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/vis/private.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 01:04:40.000000 fortls-3.1.0/test/test_source/wrong_syntax.json
```

### Comparing `fortls-3.0.0rc6/.github/FUNDING.yml` & `fortls-3.1.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md` & `fortls-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/.github/ISSUE_TEMPLATE/feature_request.md` & `fortls-3.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/.github/workflows/codeql-analysis.yml` & `fortls-3.1.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/.github/workflows/docs.yml` & `fortls-3.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/.github/workflows/docs_preview.yml` & `fortls-3.1.0/.github/workflows/docs_preview.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/.github/workflows/main.yml` & `fortls-3.1.0/.github/workflows/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
           python3 -m fortls.schema
           git diff --exit-code ./fortls/fortls.schema.json
 
       - name: Unittests
         run: pytest --doctest-modules -n auto
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v4.3.1
+        uses: codecov/codecov-action@v4.4.0
         with:
           fail_ci_if_error: true
           verbose: true
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `fortls-3.0.0rc6/.github/workflows/python-publish.yml` & `fortls-3.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/.github/workflows/update-intrinsics.yml` & `fortls-3.1.0/.github/workflows/update-intrinsics.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/.pre-commit-config.yaml` & `fortls-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/CHANGELOG.md` & `fortls-3.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # CHANGELOG
 
 ## Unreleased
 
+## 3.1.0
+
+### Fixed
+
+- Fixed bug where parser would crash when trying to retrieve an invalid line no.
+  ([#398](https://github.com/fortran-lang/fortls/issues/398))
+- Fixed bug with string quotes not being escaped when looking for parenthesis
+  ([#250](https://github.com/fortran-lang/fortls/issues/250))
+- Fixed bug with line continuations in lexical tokens
+  ([#235](https://github.com/fortran-lang/fortls/issues/235))
+
 ## 3.0.0
 
 ### Added
 
 - Added support for changing the default Python recursion depth
   ([#312](https://github.com/fortran-lang/fortls/issues/312))
 - Added support for preprocessor macro expansions
@@ -38,14 +49,18 @@
 - Moved project setup from `setup.cfg` to `pyproject.toml`
   ([#384](https://github.com/fortran-lang/fortls/pull/384))
 - Bumped `setuptools` version to `>=61.0.0`
   ([#384](https://github.com/fortran-lang/fortls/pull/384))
 
 ### Fixed
 
+- Fixed end of scope errors raised by trailing semicolon in native parser
+  ([#265](https://github.com/fortran-lang/fortls/issues/265))
+- Fixed bug where parent scope for includes in AST could be `None`
+  ([#329](https://github.com/fortran-lang/fortls/issues/329))
 - Fixed preprocessor bug with `if` and `elif` conditionals
   ([#322](https://github.com/fortran-lang/fortls/issues/322))
 - Fixed bug where type fields or methods were not detected if spaces were
   used around `%`
   ([#286](https://github.com/fortran-lang/fortls/issues/286))
 - Fixed bug where Go To Implementation would not work for submodules
   ([#74](https://github.com/fortran-lang/fortls/issues/74))
```

### Comparing `fortls-3.0.0rc6/CODE_OF_CONDUCT.md` & `fortls-3.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/CONTRIBUTING.md` & `fortls-3.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/LICENSE` & `fortls-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/PKG-INFO` & `fortls-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortls
-Version: 3.0.0rc6
+Version: 3.1.0
 Summary: fortls - Fortran Language Server
 Author-email: Giannis Nikiteas <giannis.nikiteas@gmail.com>
 License: MIT
 Project-URL: homepage, https://fortls.fortran-lang.org
 Project-URL: Documentation, https://fortls.fortran-lang.org
 Project-URL: Changes, https://github.com/fortran-lang/fortls/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/fortran-lang/fortls/issues
```

### Comparing `fortls-3.0.0rc6/README.md` & `fortls-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/SECURITY.md` & `fortls-3.1.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/LICENSE` & `fortls-3.1.0/assets/LICENSE`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/README.md` & `fortls-3.1.0/assets/README.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/animations/intro-demo.gif` & `fortls-3.1.0/assets/animations/intro-demo.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/f.svg` & `fortls-3.1.0/assets/f.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/icon.svg` & `fortls-3.1.0/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/logo.png` & `fortls-3.1.0/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/logo.svg` & `fortls-3.1.0/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/logo2-animated.svg` & `fortls-3.1.0/assets/logo2-animated.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/logos.workspace.svg` & `fortls-3.1.0/assets/logos.workspace.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/completion-ani.gif` & `fortls-3.1.0/assets/lsp/completion-ani.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/completion-ani.mp4` & `fortls-3.1.0/assets/lsp/completion-ani.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/completion.png` & `fortls-3.1.0/assets/lsp/completion.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/definition-goto.gif` & `fortls-3.1.0/assets/lsp/definition-goto.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/definition-goto.mp4` & `fortls-3.1.0/assets/lsp/definition-goto.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/definition-peek.png` & `fortls-3.1.0/assets/lsp/definition-peek.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/diagnostics1.png` & `fortls-3.1.0/assets/lsp/diagnostics1.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/doc-highlight.png` & `fortls-3.1.0/assets/lsp/doc-highlight.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/hover.png` & `fortls-3.1.0/assets/lsp/hover.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/hover2.png` & `fortls-3.1.0/assets/lsp/hover2.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/references-peek.png` & `fortls-3.1.0/assets/lsp/references-peek.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/rename.gif` & `fortls-3.1.0/assets/lsp/rename.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/rename.mp4` & `fortls-3.1.0/assets/lsp/rename.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/rename2.gif` & `fortls-3.1.0/assets/lsp/rename2.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/rename2.mp4` & `fortls-3.1.0/assets/lsp/rename2.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/sig-help.gif` & `fortls-3.1.0/assets/lsp/sig-help.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/sig-help.mp4` & `fortls-3.1.0/assets/lsp/sig-help.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/symbols-crop.png` & `fortls-3.1.0/assets/lsp/symbols-crop.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/symbols-doc.png` & `fortls-3.1.0/assets/lsp/symbols-doc.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/symbols-workspace.png` & `fortls-3.1.0/assets/lsp/symbols-workspace.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/lsp/symbols.png` & `fortls-3.1.0/assets/lsp/symbols.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/assets/symbol-class.svg` & `fortls-3.1.0/assets/symbol-class.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/Makefile` & `fortls-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/conf.py` & `fortls-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/contact.rst` & `fortls-3.1.0/docs/contact.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/contributing.rst` & `fortls-3.1.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/editor_integration.rst` & `fortls-3.1.0/docs/editor_integration.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/features.rst` & `fortls-3.1.0/docs/features.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/fortls.parsers.internal.rst` & `fortls-3.1.0/docs/fortls.parsers.internal.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/fortls.rst` & `fortls-3.1.0/docs/fortls.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/index.rst` & `fortls-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/make.bat` & `fortls-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/docs/options.rst` & `fortls-3.1.0/docs/options.rst`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,15 @@
 ---------------------------------
 
 Options for debugging language server
 
 -  ``--debug_filepath DEBUG_FILEPATH``         File path for language server tests
 -  ``--debug_rootpath DEBUG_ROOTPATH``         Root path for language server tests
 -  ``--debug_parser``                          Test source code parser on specified file
+-  ``--debug_preproc``                         Test preprocessor on specified file
 -  ``--debug_hover``                           Test `textDocument/hover` request for specified file and position
 -  ``--debug_rename RENAME_STRING``            Test `textDocument/rename` request for specified file and position
 -  ``--debug_actions``                         Test `textDocument/codeAction` request for specified file and position
 -  ``--debug_symbols``                         Test `textDocument/documentSymbol` request for specified file
 -  ``--debug_completion``                      Test `textDocument/completion` request for specified file and position
 -  ``--debug_signature``                       Test `textDocument/signatureHelp` request for specified file and position
 -  ``--debug_definition``                      Test `textDocument/definition` request for specified file and position
```

### Comparing `fortls-3.0.0rc6/docs/quickstart.rst` & `fortls-3.1.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/__init__.py` & `fortls-3.1.0/fortls/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from __future__ import annotations
 
 import sys
 from multiprocessing import freeze_support
 
-from .debug import DebugError, debug_lsp, debug_parser, is_debug_mode
+from .debug import (
+    DebugError,
+    debug_lsp,
+    debug_parser,
+    debug_preprocessor,
+    is_debug_mode,
+)
 from .interface import cli
 from .jsonrpc import JSONRPC2Connection, ReadWriter
 from .langserver import LangServer
 from .version import __version__
 
 __all__ = ["__version__"]
 
@@ -16,14 +22,17 @@
     freeze_support()
     args = cli(__name__).parse_args()
 
     try:
         if args.debug_parser:
             debug_parser(args)
 
+        elif args.debug_preproc:
+            debug_preprocessor(args)
+
         elif is_debug_mode(args):
             debug_lsp(args, vars(args))
 
         else:
             stdin, stdout = sys.stdin.buffer, sys.stdout.buffer
             LangServer(
                 conn=JSONRPC2Connection(ReadWriter(stdin, stdout)),
```

### Comparing `fortls-3.0.0rc6/fortls/constants.py` & `fortls-3.1.0/fortls/constants.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/debug.py` & `fortls-3.1.0/fortls/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
+import logging
 import os
 import pprint
+import sys
 
 import json5
 
 from .helper_functions import only_dirs, resolve_globs
 from .jsonrpc import JSONRPC2Connection, ReadWriter, path_from_uri
 from .langserver import LangServer
-from .parsers.internal.parser import FortranFile
+from .parsers.internal.parser import FortranFile, preprocess_file
 
 
 class DebugError(Exception):
     """Base class for debug CLI."""
 
 
 class ParameterError(DebugError):
@@ -411,61 +413,19 @@
 
     Parameters
     ----------
     args : Namespace
         The arguments parsed from the `ArgumentParser`
     """
 
-    def locate_config(root: str) -> str | None:
-        default_conf_files = [args.config, ".fortlsrc", ".fortls.json5", ".fortls"]
-        present_conf_files = [
-            os.path.isfile(os.path.join(root, f)) for f in default_conf_files
-        ]
-        if not any(present_conf_files):
-            return None
-
-        # Load the first config file found
-        for f, present in zip(default_conf_files, present_conf_files):
-            if not present:
-                continue
-            config_path = os.path.join(root, f)
-            return config_path
-
-    def read_config(root: str | None):
-        pp_suffixes = None
-        pp_defs = {}
-        include_dirs = set()
-        if root is None:
-            return pp_suffixes, pp_defs, include_dirs
-
-        # Check for config files
-        config_path = locate_config(root)
-        if not os.path.isfile(config_path):
-            return pp_suffixes, pp_defs, include_dirs
-
-        try:
-            with open(config_path, encoding="utf-8") as fhandle:
-                config_dict = json5.load(fhandle)
-                pp_suffixes = config_dict.get("pp_suffixes", None)
-                pp_defs = config_dict.get("pp_defs", {})
-                for path in config_dict.get("include_dirs", set()):
-                    include_dirs.update(only_dirs(resolve_globs(path, root)))
-
-                if isinstance(pp_defs, list):
-                    pp_defs = {key: "" for key in pp_defs}
-        except ValueError as e:
-            print(f"Error {e} while parsing '{config_path}' settings file")
-
-        return pp_suffixes, pp_defs, include_dirs
-
     print("\nTesting parser")
     separator()
 
     ensure_file_accessible(args.debug_filepath)
-    pp_suffixes, pp_defs, include_dirs = read_config(args.debug_rootpath)
+    pp_suffixes, pp_defs, include_dirs = read_config(args.debug_rootpath, args.config)
 
     print(f'  File = "{args.debug_filepath}"')
     file_obj = FortranFile(args.debug_filepath, pp_suffixes)
     err_str, _ = file_obj.load_from_disk()
     if err_str:
         raise DebugError(f"Reading file failed: {err_str}")
     print(f"  Detected format: {'fixed' if file_obj.fixed else 'free'}")
@@ -477,14 +437,64 @@
         print_children(obj)
     print("\n" + "=" * 80 + "\nExportable Objects\n" + "=" * 80 + "\n")
     for _, obj in file_ast.global_dict.items():
         print(f"{obj.get_type()}: {obj.FQSN}")
     separator()
 
 
+def debug_preprocessor(args):
+    """Debug the preprocessor of the Language Server
+    Triggered by `--debug_preprocessor` option.
+
+    Parameters
+    ----------
+    args : Namespace
+        The arguments parsed from the `ArgumentParser`
+    """
+
+    def sep_lvl2(heading: str):
+        print("\n" + "=" * 75 + f"\n{heading}\n" + "=" * 75)
+
+    print("\nTesting preprocessor")
+    separator()
+
+    logging.basicConfig(level=logging.DEBUG, stream=sys.stdout, format="%(message)s")
+
+    file = args.debug_filepath
+    ensure_file_accessible(file)
+    with open(file, encoding="utf-8") as f:
+        lines = f.readlines()
+
+    root = args.debug_rootpath if args.debug_rootpath else os.path.dirname(file)
+    _, pp_defs, include_dirs = read_config(root, args.config)
+
+    sep_lvl2("Preprocessor Pass:")
+    output, skips, defines, defs = preprocess_file(
+        lines, file, pp_defs, include_dirs, debug=True
+    )
+
+    sep_lvl2("Preprocessor Skipped Lines:")
+    for line in skips:
+        print(f"  {line}")
+
+    sep_lvl2("Preprocessor Macros:")
+    for key, value in defs.items():
+        print(f"  {key} = {value}")
+
+    sep_lvl2("Preprocessor Defines (#define):")
+    for line in defines:
+        print(f"  {line}")
+
+    sep_lvl2("Preprocessor Final Output:")
+    for line in output:
+        print(rf"  {line.rstrip()}")
+
+    separator()
+
+
 def ensure_file_accessible(filepath: str):
     """Ensure the file exists and is accessible, raising an error if not."""
     if not os.path.isfile(filepath):
         raise DebugError(f"File '{filepath}' does not exist or is not accessible")
     print(f'  File = "{filepath}"')
 
 
@@ -495,14 +505,59 @@
             raise ParameterError("'debug_line' not specified for debug request")
         print(f"  Line = {args.debug_line}")
         if args.debug_char is None:
             raise ParameterError("'debug_char' not specified for debug request")
         print(f"  Char = {args.debug_char}\n")
 
 
+def locate_config(root: str, input_config: str) -> str | None:
+    default_conf_files = [input_config, ".fortlsrc", ".fortls.json5", ".fortls"]
+    present_conf_files = [
+        os.path.isfile(os.path.join(root, f)) for f in default_conf_files
+    ]
+    if not any(present_conf_files):
+        return None
+
+    # Load the first config file found
+    for f, present in zip(default_conf_files, present_conf_files):
+        if not present:
+            continue
+        config_path = os.path.join(root, f)
+        return config_path
+
+
+def read_config(root: str | None, input_config: str):
+    pp_suffixes = None
+    pp_defs = {}
+    include_dirs = set()
+    if root is None:
+        return pp_suffixes, pp_defs, include_dirs
+
+    # Check for config files
+    config_path = locate_config(root, input_config)
+    print(f"  Config file = {config_path}")
+    if config_path is None or not os.path.isfile(config_path):
+        return pp_suffixes, pp_defs, include_dirs
+
+    try:
+        with open(config_path, encoding="utf-8") as fhandle:
+            config_dict = json5.load(fhandle)
+            pp_suffixes = config_dict.get("pp_suffixes", None)
+            pp_defs = config_dict.get("pp_defs", {})
+            for path in config_dict.get("include_dirs", set()):
+                include_dirs.update(only_dirs(resolve_globs(path, root)))
+
+            if isinstance(pp_defs, list):
+                pp_defs = {key: "" for key in pp_defs}
+    except ValueError as e:
+        print(f"Error {e} while parsing '{config_path}' settings file")
+
+    return pp_suffixes, pp_defs, include_dirs
+
+
 def debug_generic(args, test_label, lsp_request, format_results, loc_needed=True):
     print(f'\nTesting "{test_label}" request:')
     check_request_params(args, loc_needed)
     results = lsp_request()
     separator()
     print_results(results, format_results, args)
```

### Comparing `fortls-3.0.0rc6/fortls/fortls.schema.json` & `fortls-3.1.0/fortls/fortls.schema.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/ftypes.py` & `fortls-3.1.0/fortls/ftypes.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/helper_functions.py` & `fortls-3.1.0/fortls/helper_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,17 +256,29 @@
     >>> find_paren_match('a, (b, c), d)')
     12
 
     If the outermost parenthesis is not closed function returns -1
 
     >>> find_paren_match('a, (b, (c, d)')
     -1
+
+    >>> find_paren_match('nt(sin(0.5))+8+len("ab((c")-3) :: y')
+    29
+
+    >>> find_paren_match("nt(sin(0.5))+8+len('ab))c')-3) :: y")
+    29
     """
     paren_count = 1
+    quote_state = {"'": False, '"': False}
     for i, char in enumerate(string):
+        if char in quote_state:
+            quote_state[char] = not quote_state[char]
+        if any(quote_state.values()):
+            continue
+
         if char == "(":
             paren_count += 1
         elif char == ")":
             paren_count -= 1
         if paren_count == 0:
             return i
     return -1
```

### Comparing `fortls-3.0.0rc6/fortls/interface.py` & `fortls-3.1.0/fortls/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,19 @@
     )
     group.add_argument(
         "--debug_parser",
         action="store_true",
         help=hide_opt("Test source code parser on specified file"),
     )
     group.add_argument(
+        "--debug_preproc",
+        action="store_true",
+        help=hide_opt("Test source code preprocessor parser on specified file"),
+    )
+    group.add_argument(
         "--debug_hover",
         action="store_true",
         help=hide_opt(
             "Test `textDocument/hover` request for specified file and position"
         ),
     )
     group.add_argument(
```

### Comparing `fortls-3.0.0rc6/fortls/json_templates.py` & `fortls-3.1.0/fortls/json_templates.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/jsonrpc.py` & `fortls-3.1.0/fortls/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/langserver.py` & `fortls-3.1.0/fortls/langserver.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/associate.py` & `fortls-3.1.0/fortls/parsers/internal/associate.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/ast.py` & `fortls-3.1.0/fortls/parsers/internal/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,16 +268,17 @@
                         include_ast.inc_scope = include_ast.none_scope
                     # Remove old objects
                     for obj in added_entities:
                         parent_scope.children.remove(obj)
                     added_entities = []
                     for child in include_ast.inc_scope.children:
                         added_entities.append(child)
-                        parent_scope.add_child(child)
-                        child.update_fqsn(parent_scope.FQSN)
+                        if parent_scope is not None:
+                            parent_scope.add_child(child)
+                            child.update_fqsn(parent_scope.FQSN)
                     include_ast.none_scope = parent_scope
                     inc.scope_objs = added_entities
 
     def resolve_links(self, obj_tree, link_version):
         for inherit_obj in self.inherit_objs:
             inherit_obj.resolve_inherit(obj_tree, inherit_version=link_version)
         for linkable_obj in self.linkable_objs:
```

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/base.py` & `fortls-3.1.0/fortls/parsers/internal/base.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/block.py` & `fortls-3.1.0/fortls/parsers/internal/block.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/diagnostics.py` & `fortls-3.1.0/fortls/parsers/internal/diagnostics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/function.py` & `fortls-3.1.0/fortls/parsers/internal/function.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/imports.py` & `fortls-3.1.0/fortls/parsers/internal/imports.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/interface.py` & `fortls-3.1.0/fortls/parsers/internal/interface.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.modules.json` & `fortls-3.1.0/fortls/parsers/internal/intrinsic.modules.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.procedures.json` & `fortls-3.1.0/fortls/parsers/internal/intrinsic.procedures.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/intrinsic.procedures.markdown.json` & `fortls-3.1.0/fortls/parsers/internal/intrinsic.procedures.markdown.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/intrinsics.py` & `fortls-3.1.0/fortls/parsers/internal/intrinsics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/keywords.json` & `fortls-3.1.0/fortls/parsers/internal/keywords.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/method.py` & `fortls-3.1.0/fortls/parsers/internal/method.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/module.py` & `fortls-3.1.0/fortls/parsers/internal/module.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/parser.py` & `fortls-3.1.0/fortls/parsers/internal/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1100,32 +1100,32 @@
                 # Read the next line if needed
                 while (iAmper >= 0) and (iAmper < iComm):
                     if line_ind == line_no + 1:
                         curr_line = curr_line[:iAmper]
                     elif next_line != "":
                         post_lines[-1] = next_line[:iAmper]
                     next_line = self.get_line(line_ind, pp_content)
+                    if next_line is None:
+                        break
+
                     line_ind += 1
                     # Skip any preprocessor statements when seeking the next line
                     if FRegex.PP_ANY.match(next_line):
                         next_line = ""
                         post_lines.append("")
                         continue
                     # Skip empty or comment lines
                     match = FRegex.FREE_COMMENT.match(next_line)
                     if next_line.rstrip() == "" or match:
                         next_line = ""
                         post_lines.append("")
                         continue
                     opt_cont_match = FRegex.FREE_CONT.match(next_line)
                     if opt_cont_match:
-                        next_line = (
-                            " " * opt_cont_match.end(0)
-                            + next_line[opt_cont_match.end(0) :]
-                        )
+                        next_line = next_line[opt_cont_match.end(0) :]
                     post_lines.append(next_line)
                     line_stripped = strip_strings(next_line, maintain_len=True)
                     iAmper = line_stripped.find("&")
                     iComm = line_stripped.find("!")
                     if iComm < 0:
                         iComm = iAmper + 1
         # Detect start of comment in current line
@@ -1346,14 +1346,15 @@
             else:
                 line_no_comment = line
             # Split lines with semicolons, place the multiple lines into a stack
             if line_stripped.find(";") >= 0:
                 multi_lines.extendleft(line_stripped.split(";"))
                 line = multi_lines.pop()
                 line_stripped = line
+                line_no_comment = line
             # Test for scope end
             if file_ast.end_scope_regex is not None:
                 match = FRegex.END_WORD.match(line_no_comment)
                 # Handle end statement
                 if self.parse_end_scope_word(line_no_comment, line_no, file_ast, match):
                     continue
                 # Look for old-style end of DO loops with line labels
```

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/scope.py` & `fortls-3.1.0/fortls/parsers/internal/scope.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/select.py` & `fortls-3.1.0/fortls/parsers/internal/select.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/statements.json` & `fortls-3.1.0/fortls/parsers/internal/statements.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/submodule.py` & `fortls-3.1.0/fortls/parsers/internal/submodule.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/subroutine.py` & `fortls-3.1.0/fortls/parsers/internal/subroutine.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/type.py` & `fortls-3.1.0/fortls/parsers/internal/type.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/use.py` & `fortls-3.1.0/fortls/parsers/internal/use.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/utilities.py` & `fortls-3.1.0/fortls/parsers/internal/utilities.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/parsers/internal/variable.py` & `fortls-3.1.0/fortls/parsers/internal/variable.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/regex_patterns.py` & `fortls-3.1.0/fortls/regex_patterns.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls/schema.py` & `fortls-3.1.0/fortls/schema.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/fortls.egg-info/PKG-INFO` & `fortls-3.1.0/fortls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortls
-Version: 3.0.0rc6
+Version: 3.1.0
 Summary: fortls - Fortran Language Server
 Author-email: Giannis Nikiteas <giannis.nikiteas@gmail.com>
 License: MIT
 Project-URL: homepage, https://fortls.fortran-lang.org
 Project-URL: Documentation, https://fortls.fortran-lang.org
 Project-URL: Changes, https://github.com/fortran-lang/fortls/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/fortran-lang/fortls/issues
```

### Comparing `fortls-3.0.0rc6/fortls.egg-info/SOURCES.txt` & `fortls-3.1.0/fortls.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -177,28 +177,34 @@
 test/test_source/docs/test_doxygen.f90
 test/test_source/docs/test_ford.f90
 test/test_source/docs/test_module_and_type_doc.f90
 test/test_source/excldir/sub1/tmp.f90
 test/test_source/excldir/sub2/fake2.f90
 test/test_source/hover/associate_block.f90
 test/test_source/hover/associate_block_2.f90
+test/test_source/hover/complicated_kind_spec.f90
 test/test_source/hover/functions.f90
 test/test_source/hover/intent.f90
+test/test_source/hover/multiline_lexical_tokens.f90
 test/test_source/hover/parameters.f90
 test/test_source/hover/pointers.f90
 test/test_source/hover/recursive.f90
 test/test_source/hover/spaced_keywords.f90
 test/test_source/hover/types.f90
 test/test_source/imp/import.f90
 test/test_source/imp/submodule.f90
 test/test_source/include/empty.h
+test/test_source/parse/.fortls
 test/test_source/parse/line_continuations.f90
 test/test_source/parse/submodule.f90
 test/test_source/parse/test_incomplete_dims.f90
 test/test_source/parse/test_kinds_and_dims.f90
+test/test_source/parse/trailing_semicolon.f90
+test/test_source/parse/mixed/multilines.F90
+test/test_source/parse/mixed/preproc_and_normal_syntax.F90
 test/test_source/pp/.fortls
 test/test_source/pp/.pp_conf.json
 test/test_source/pp/preproc.F90
 test/test_source/pp/preproc_elif.F90
 test/test_source/pp/preproc_elif_elif_skip.F90
 test/test_source/pp/preproc_else.F90
 test/test_source/pp/preproc_if_elif_else.F90
```

### Comparing `fortls-3.0.0rc6/licenses/fortran-language-server-license.txt` & `fortls-3.1.0/licenses/fortran-language-server-license.txt`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/pyproject.toml` & `fortls-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/setup_tests.py` & `fortls-3.1.0/test/setup_tests.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_interface.py` & `fortls-3.1.0/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_preproc.py` & `fortls-3.1.0/test/test_preproc.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_preproc_parser.py` & `fortls-3.1.0/test/test_preproc_parser.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_regex_patterns.py` & `fortls-3.1.0/test/test_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server.py` & `fortls-3.1.0/test/test_server.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server_completion.py` & `fortls-3.1.0/test/test_server_completion.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server_definitions.py` & `fortls-3.1.0/test/test_server_definitions.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server_diagnostics.py` & `fortls-3.1.0/test/test_server_diagnostics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server_documentation.py` & `fortls-3.1.0/test/test_server_documentation.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server_hover.py` & `fortls-3.1.0/test/test_server_hover.py`

 * *Files 2% similar despite different names*

```diff
@@ -662,7 +662,35 @@
     assert errcode == 0
     ref_results = [
         "```fortran90\nTYPE, ABSTRACT :: base_t\n```",
         "```fortran90\nTYPE, ABSTRACT, EXTENDS(base_t) :: extends_t\n```",
         "```fortran90\nTYPE, EXTENDS(extends_t) :: a_t\n```",
     ]
     validate_hover(results, ref_results)
+
+
+def test_complicated_kind_spec():
+    string = write_rpc_request(1, "initialize", {"rootPath": str(test_dir / "hover")})
+    file_path = test_dir / "hover" / "complicated_kind_spec.f90"
+    string += hover_req(file_path, 1, 40)
+    string += hover_req(file_path, 2, 40)
+    errcode, results = run_request(string, fortls_args=["-n", "1"])
+    assert errcode == 0
+    ref_results = [
+        '```fortran90\nREAL(int(sin(0.5))+8+len("ab((c")-3) :: y\n```',
+        '```fortran90\nREAL(int(sin(0.5))+8+len("ab))c")-3) :: z\n```',
+    ]
+    validate_hover(results, ref_results)
+
+
+def test_multiline_lexical_token():
+    string = write_rpc_request(1, "initialize", {"rootPath": str(test_dir / "hover")})
+    file_path = test_dir / "hover" / "multiline_lexical_tokens.f90"
+    string += hover_req(file_path, 4, 8)
+    string += hover_req(file_path, 8, 16)
+    errcode, results = run_request(string, fortls_args=["-n", "1"])
+    assert errcode == 0
+    ref_results = [
+        "```fortran90\nINTEGER :: i\n```",
+        '```fortran90\nREAL(int(sin(0.5))+8+len("ab))c")-3) :: Z\n```',
+    ]
+    validate_hover(results, ref_results)
```

### Comparing `fortls-3.0.0rc6/test/test_server_implementation.py` & `fortls-3.1.0/test/test_server_implementation.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server_messages.py` & `fortls-3.1.0/test/test_server_messages.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server_references.py` & `fortls-3.1.0/test/test_server_references.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server_rename.py` & `fortls-3.1.0/test/test_server_rename.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_server_signature_help.py` & `fortls-3.1.0/test/test_server_signature_help.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/completion/use_only_interface.f90` & `fortls-3.1.0/test/test_source/completion/use_only_interface.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/diag/test_function_arg_list.f90` & `fortls-3.1.0/test/test_source/diag/test_function_arg_list.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/diag/test_scope_overreach.f90` & `fortls-3.1.0/test/test_source/diag/test_scope_overreach.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/diag/test_semicolon.f90` & `fortls-3.1.0/test/test_source/diag/test_semicolon.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/docs/test_doxygen.f90` & `fortls-3.1.0/test/test_source/docs/test_doxygen.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/docs/test_ford.f90` & `fortls-3.1.0/test/test_source/docs/test_ford.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/excldir/sub1/tmp.f90` & `fortls-3.1.0/test/test_source/excldir/sub1/tmp.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/f90_config.json` & `fortls-3.1.0/test/test_source/f90_config.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/hover/functions.f90` & `fortls-3.1.0/test/test_source/hover/functions.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/hover/parameters.f90` & `fortls-3.1.0/test/test_source/hover/parameters.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/hover/recursive.f90` & `fortls-3.1.0/test/test_source/hover/recursive.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/imp/import.f90` & `fortls-3.1.0/test/test_source/imp/import.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/imp/submodule.f90` & `fortls-3.1.0/test/test_source/imp/submodule.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/parse/test_kinds_and_dims.f90` & `fortls-3.1.0/test/test_source/parse/test_kinds_and_dims.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/pp/preproc_elif.F90` & `fortls-3.1.0/test/test_source/pp/preproc_elif.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/pp/preproc_elif_elif_skip.F90` & `fortls-3.1.0/test/test_source/pp/preproc_elif_elif_skip.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/pp/preproc_if_elif_else.F90` & `fortls-3.1.0/test/test_source/pp/preproc_if_elif_else.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/pp/preproc_if_elif_skip.F90` & `fortls-3.1.0/test/test_source/pp/preproc_if_elif_skip.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/rename/test_rename_intrinsic.f90` & `fortls-3.1.0/test/test_source/rename/test_rename_intrinsic.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/signature/help.f90` & `fortls-3.1.0/test/test_source/signature/help.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/subdir/test_fixed.f` & `fortls-3.1.0/test/test_source/subdir/test_fixed.f`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/subdir/test_free.f90` & `fortls-3.1.0/test/test_source/subdir/test_free.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/subdir/test_generic.f90` & `fortls-3.1.0/test/test_source/subdir/test_generic.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/subdir/test_select.f90` & `fortls-3.1.0/test/test_source/subdir/test_select.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/subdir/test_submod.F90` & `fortls-3.1.0/test/test_source/subdir/test_submod.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/test_diagnostic_int.f90` & `fortls-3.1.0/test/test_source/test_diagnostic_int.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc6/test/test_source/test_prog.f08` & `fortls-3.1.0/test/test_source/test_prog.f08`

 * *Files identical despite different names*

