# Comparing `tmp/mdformat_gfm_alerts-0.0.1.tar.gz` & `tmp/mdformat_gfm_alerts-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_gfm_alerts-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_gfm_alerts-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_gfm_alerts-0.0.1.tar` & `mdformat_gfm_alerts-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1819 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/.gitignore
--rw-r--r--   0        0        0     1444 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      295 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/.pre-commit-test.yaml
--rw-r--r--   0        0        0     2886 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/.ruff.toml
--rw-r--r--   0        0        0       21 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/.tool-versions
--rw-r--r--   0        0        0     1365 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/LICENSE
--rw-r--r--   0        0        0     2744 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/README.md
--rw-r--r--   0        0        0      110 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/mdformat_gfm_alerts/__init__.py
--rw-r--r--   0        0        0      133 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/mdformat_gfm_alerts/factories/__init__.py
--rw-r--r--   0        0        0     2841 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/mdformat_gfm_alerts/factories/_factories.py
--rw-r--r--   0        0        0      129 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/mdformat_gfm_alerts/mdit_plugins/__init__.py
--rw-r--r--   0        0        0     2710 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/mdformat_gfm_alerts/mdit_plugins/_gfm_alert.py
--rw-r--r--   0        0        0     1328 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/mdformat_gfm_alerts/plugin.py
--rw-r--r--   0        0        0     1132 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      679 2024-03-10 19:09:58.299668 mdformat_gfm_alerts-0.0.1/tox.ini
--rw-r--r--   0        0        0     3593 1970-01-01 00:00:00.000000 mdformat_gfm_alerts-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      612 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.copier-answers.yml
+-rw-r--r--   0        0        0     1819 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1592 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      295 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.pre-commit-test.yaml
+-rw-r--r--   0        0        0     2886 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.ruff.toml
+-rw-r--r--   0        0        0       21 2024-05-20 13:06:11.288616 mdformat_gfm_alerts-1.0.0/.tool-versions
+-rw-r--r--   0        0        0      276 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/.yamllint.yaml
+-rw-r--r--   0        0        0     1370 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2741 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/README.md
+-rw-r--r--   0        0        0      110 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/__init__.py
+-rw-r--r--   0        0        0      149 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/factories/__init__.py
+-rw-r--r--   0        0        0     3185 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/factories/_gfm_blockquote_factories.py
+-rw-r--r--   0        0        0       88 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/mdit_plugins/__init__.py
+-rw-r--r--   0        0        0     3002 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/mdit_plugins/_gfm_alerts.py
+-rw-r--r--   0        0        0     1300 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/plugin.py
+-rw-r--r--   0        0        0     1200 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      751 2024-05-20 13:06:11.292616 mdformat_gfm_alerts-1.0.0/tox.ini
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 mdformat_gfm_alerts-1.0.0/PKG-INFO
```

### Comparing `mdformat_gfm_alerts-0.0.1/.gitignore` & `mdformat_gfm_alerts-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-0.0.1/.pre-commit-config.yaml` & `mdformat_gfm_alerts-1.0.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
       - id: check-vcs-permalinks
       - id: check-yaml
         args: [--unsafe]
       - id: debug-statements
       - id: destroyed-symlinks
       - id: detect-private-key
       - id: end-of-file-fixer
+        exclude: \.copier-answers\.yml
       - id: fix-byte-order-marker
       - id: fix-encoding-pragma
         args: [--remove]
       - id: forbid-new-submodules
       - id: mixed-line-ending
         args: [--fix=auto]
       - id: pretty-format-json
@@ -27,25 +28,29 @@
       - id: trailing-whitespace
         exclude: tests/.*fixtures.*\.md
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.2
+    rev: v0.3.4
     hooks:
       - id: ruff
         args: [--fix]
       - id: ruff-format
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
       - id: mdformat
-        additional_dependencies: ['mdformat-mkdocs[recommended]>=1.0.6']
+        additional_dependencies:
+          - mdformat-mkdocs[recommended]>=2.0.6
+          - mdformat-gfm-alerts>=0.0.1
         exclude: tests/.+\.md
         args: [--wrap=no]
-  - repo: https://github.com/lyz-code/yamlfix/
-    rev: 1.16.0
+  - repo: https://github.com/adrienverge/yamllint.git
+    rev: v1.35.1
     hooks:
-      - id: yamlfix
-        types_or: []
-        types: [file, yaml]
+      - id: yamllint
+  - repo: https://github.com/pappasam/toml-sort
+    rev: v0.23.1
+    hooks:
+      - id: toml-sort-fix
```

### Comparing `mdformat_gfm_alerts-0.0.1/.ruff.toml` & `mdformat_gfm_alerts-1.0.0/.ruff.toml`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-0.0.1/CONTRIBUTING.md` & `mdformat_gfm_alerts-1.0.0/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -69,10 +69,10 @@
 # envchain --set FLIT FLIT_PASSWORD
 export FLIT_USERNAME=__token__
 export eval $(envchain FLIT env | grep FLIT_PASSWORD=)
 
 flit publish
 ```
 
-or trigger the GitHub Action job, by creating a release with a tag equal to the version, e.g. `v0.0.1` and updating the version in `mdformat_admon/__init__.py`.
+or trigger the GitHub Action job, by creating a release with a tag equal to the version, e.g. `v0.0.1` and updating the version in `mdformat_gfm_alerts/__init__.py`.
 
 Note, this requires generating an API key on PyPi and adding it to the repository `Settings/Secrets`, under the name `PYPI_KEY`.
```

### Comparing `mdformat_gfm_alerts-0.0.1/LICENSE` & `mdformat_gfm_alerts-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_gfm_alerts-0.0.1/README.md` & `mdformat_gfm_alerts-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,15 @@
 # <div class="markdown-alert markdown-alert-note">
 # <p class="markdown-alert-title">Note</p>
 # <p>Useful information that users should know, even when skimming content.</p>
 # </div>
 # </blockquote>
 ```
 
-> **Warning**
->
+> [!WARNING]
 > This package does not properly handle replacing the `blockquote` outer `div` with a `div` for accessibility. This should be possible with `markdown-it`, but I haven't yet found a way.
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/KyleKing/mdformat-gfm-alerts/blob/main/CONTRIBUTING.md)
 
 [ci-badge]: https://github.com/kyleking/mdformat-gfm-alerts/workflows/CI/badge.svg?branch=main
```

### Comparing `mdformat_gfm_alerts-0.0.1/mdformat_gfm_alerts/factories/_factories.py` & `mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/factories/_gfm_blockquote_factories.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-"""GitHub Alerts."""
+"""Logic Factories.
+
+Adapted from the implementation for `mdformat-admon`:
+<https://github.com/KyleKing/mdformat-admon/blob/cf9a81277e1feac0ce9bf1190efa965ac3d407b2/mdformat_admon/factories/_whitespace_admon_factories.py>
+
+Copied to `mdformat-obsidian`. Try to keep in-sync:
+<https://github.com/KyleKing/mdformat-obsidian/blob/8f260e168b3575e6a76b20f53e780c1ba7d68d13/mdformat_obsidian/factories/_obsidian_blockquote_factories.py>
+
+"""
 
 from __future__ import annotations
 
 import re
 from collections.abc import Generator
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Callable, NamedTuple
@@ -10,27 +18,24 @@
 from markdown_it import MarkdownIt
 from markdown_it.rules_block import StateBlock
 from mdit_py_plugins.utils import is_code_block
 
 if TYPE_CHECKING:
     from markdown_it.token import Token
 
-PREFIX = "gfm_alert"
-"""Prefix used to differentiate the parsed output."""
-
 
 # FYI: copied from mdformat_admon.factories
 @contextmanager
 def new_token(state: StateBlock, name: str, kind: str) -> Generator[Token, None, None]:
     """Creates scoped token."""
     yield state.push(f"{name}_open", kind, 1)
     state.push(f"{name}_close", kind, -1)
 
 
-# FYI: Adapted from mdformat_admon.factories._factories
+# FYI: Adapted from mdformat_admon.factories
 class AlertState(NamedTuple):
     """Frozen state."""
 
     parentType: str
     lineMax: int
 
 
@@ -40,14 +45,15 @@
     old_state: AlertState
     meta_text: str
     inline_content: str
     next_line: int
 
 
 def parse_possible_blockquote_admon_factory(
+    prefix: str,
     patterns: set[str],
 ) -> Callable[[StateBlock, int, int, bool], AlertData | bool]:
     """Generate the parser function.
 
     Accepts set of strings that will be compiled into regular expressions.
     They must have a capture group `title`.
 
@@ -63,44 +69,44 @@
             return False
 
         start = state.bMarks[start_line] + state.tShift[start_line]
 
         # Exit if no match for any pattern
         text = state.src[start:]
         regexes = [
-            re.compile(rf"{pat}(?P<inline_content>(?: |<br>)[^\n]+)?", re.IGNORECASE)
+            re.compile(rf"{pat}(?: |<br>)?(?P<inline_content>[^\n]+)?", re.IGNORECASE)
             for pat in patterns
         ]
         match = next((_m for rx in regexes if (_m := rx.match(text))), None)
         if not match:
             return False
 
         # Since start is found, we can report success here in validation mode
         if silent:
             return True
 
         old_state = AlertState(
             parentType=state.parentType,
             lineMax=state.lineMax,
         )
-        state.parentType = "gfm_alert"
+        state.parentType = prefix
 
         return AlertData(
             old_state=old_state,
             meta_text=match["title"],
             inline_content=match["inline_content"] or "",
             next_line=end_line,
         )
 
     return parse_possible_blockquote_admon
 
 
-def gfm_alert_plugin_factory(
+def gfm_alerts_plugin_factory(
     prefix: str,
     logic: Callable[[StateBlock, int, int, bool], bool],
 ) -> Callable[[MarkdownIt], None]:
     """Generate the plugin function."""
 
-    def gfm_alert_plugin(md: MarkdownIt) -> None:
+    def gfm_alerts_plugin(md: MarkdownIt) -> None:
         md.block.ruler.before("blockquote", prefix, logic)
 
-    return gfm_alert_plugin
+    return gfm_alerts_plugin
```

### Comparing `mdformat_gfm_alerts-0.0.1/mdformat_gfm_alerts/mdit_plugins/_gfm_alert.py` & `mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/mdit_plugins/_gfm_alerts.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,59 +2,63 @@
 
 from __future__ import annotations
 
 from markdown_it.rules_block import StateBlock
 
 from ..factories import (
     AlertData,
-    gfm_alert_plugin_factory,
+    gfm_alerts_plugin_factory,
     new_token,
     parse_possible_blockquote_admon_factory,
 )
 
-PREFIX = "gfm_alert"
+GFM_ALERTS_PREFIX = "gfm_alert"
 """Prefix used to differentiate the parsed output."""
 
 INLINE_SEP = "\n\n"
-"""Optional separator to differentiate the title and ineline content (if present)."""
+"""Separator to differentiate the title and inline content (if present)."""
 
 PATTERNS = {
     # Note '> ' prefix is removed when parsing
     r"^\*\*(?P<title>Note|Warning)\*\*",
     # FYI: This is intentionally strict. Keep in sync with supported titles
     r"^\\?\[!(?P<title>NOTE|TIP|IMPORTANT|WARNING|CAUTION)\\?\]",
 }
 """Patterns specific to GitHub Alerts."""
 
 
-def format_gfm_alert_markup(
+def format_gfm_alerts_markup(
     state: StateBlock,
     start_line: int,
     admonition: AlertData,
 ) -> None:
     """Format markup."""
-    title_line = (
-        f"[!{admonition.meta_text.upper()}]{INLINE_SEP}{admonition.inline_content}"
-    )
+    # To fix #2, when the admonition and text are on the same line, push the content
+    #  to the next line. While this is equivalent in the markdown spec, this is
+    #  required for Github
+    newline = "\n"
 
-    with new_token(state, PREFIX, "div") as token:
+    meta = f"[!{admonition.meta_text.upper()}]"
+    title_line = f"{meta}{newline}{admonition.inline_content}".rstrip()
+
+    with new_token(state, GFM_ALERTS_PREFIX, "div") as token:
         token.attrs = {
             "class": f"markdown-alert markdown-alert-{admonition.meta_text.lower()}",
         }
         token.block = True
         token.map = [start_line, admonition.next_line]
         token.markup = title_line
-        with new_token(state, f"{PREFIX}_title", "p") as tkn_title:
+        with new_token(state, f"{GFM_ALERTS_PREFIX}_title", "p") as tkn_title:
             tkn_title.attrs = {"class": "markdown-alert-title"}
 
             tkn_title_txt = state.push("inline", "", 0)
             tkn_title_txt.content = admonition.meta_text.title()
 
         if admonition.inline_content:
-            with new_token(state, f"{PREFIX}_inline", "p"):
+            with new_token(state, f"{GFM_ALERTS_PREFIX}_inline", "p"):
                 tkn_inline_txt = state.push("inline", "", 0)
                 tkn_inline_txt.content = admonition.inline_content.strip()
 
         state.md.block.tokenize(state, start_line + 1, admonition.next_line)
 
     # FIXME: this isn't actually replacing the block quote outer div?
     #
@@ -68,16 +72,16 @@
 def alert_logic(
     state: StateBlock,
     startLine: int,
     endLine: int,
     silent: bool,
 ) -> bool:
     """Parse GitHub Alerts."""
-    parser_func = parse_possible_blockquote_admon_factory(PATTERNS)
+    parser_func = parse_possible_blockquote_admon_factory(GFM_ALERTS_PREFIX, PATTERNS)
     result = parser_func(state, startLine, endLine, silent)
     if isinstance(result, AlertData):
-        format_gfm_alert_markup(state, startLine, admonition=result)
+        format_gfm_alerts_markup(state, startLine, admonition=result)
         return True
     return result
 
 
-gfm_alert_plugin = gfm_alert_plugin_factory(PREFIX, alert_logic)
+gfm_alerts_plugin = gfm_alerts_plugin_factory(GFM_ALERTS_PREFIX, alert_logic)
```

### Comparing `mdformat_gfm_alerts-0.0.1/mdformat_gfm_alerts/plugin.py` & `mdformat_gfm_alerts-1.0.0/mdformat_gfm_alerts/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 from typing import Mapping
 
 from markdown_it import MarkdownIt
 from mdformat.renderer import RenderContext, RenderTreeNode
 from mdformat.renderer.typing import Render
 
-from .mdit_plugins import GFM_ALERT_PREFIX, INLINE_SEP, gfm_alert_plugin
+from .mdit_plugins import GFM_ALERTS_PREFIX, gfm_alerts_plugin
 
 
 def update_mdit(mdit: MarkdownIt) -> None:
     """Update the parser to identify Alerts."""
-    mdit.use(gfm_alert_plugin)
+    mdit.use(gfm_alerts_plugin)
 
 
-def _render_gfm_alert(node: RenderTreeNode, context: RenderContext) -> str:
+def _render_gfm_alerts(node: RenderTreeNode, context: RenderContext) -> str:
     """Render a `RenderTreeNode`."""
-    title_line = node.markup.replace(INLINE_SEP, "")
+    title_line = node.markup
     elements = [render for child in node.children if (render := child.render(context))]
     # Do not separate the title line from the first row
     return "\n".join([title_line, "\n\n".join(elements)]).rstrip()
 
 
 def _no_render(
     node: RenderTreeNode,  # noqa: ARG001
@@ -32,11 +32,11 @@
     return ""
 
 
 # A mapping from syntax tree node type to a function that renders it.
 # This can be used to overwrite renderer functions of existing syntax
 # or add support for new syntax.
 RENDERERS: Mapping[str, Render] = {
-    GFM_ALERT_PREFIX: _render_gfm_alert,
-    f"{GFM_ALERT_PREFIX}_title": _no_render,
-    f"{GFM_ALERT_PREFIX}_inline": _no_render,
+    GFM_ALERTS_PREFIX: _render_gfm_alerts,
+    f"{GFM_ALERTS_PREFIX}_title": _no_render,
+    f"{GFM_ALERTS_PREFIX}_inline": _no_render,
 }
```

### Comparing `mdformat_gfm_alerts-0.0.1/PKG-INFO` & `mdformat_gfm_alerts-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mdformat_gfm_alerts
-Version: 0.0.1
+Version: 1.0.0
 Summary: An mdformat plugin for `gfm_alerts`.
-Keywords: mdformat,markdown,markdown-it
-Author-email: Kyle King <dev.act.kyle@gmail.com>
+Keywords: markdown,markdown-it,mdformat
+Author-email: kyleking <dev.act.kyle@gmail.com>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: mdformat >= 0.7.16
-Requires-Dist: mdformat-gfm >= 0.3.6
 Requires-Dist: mdit-py-plugins >= 0.4.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest >= 7.4.4 ; extra == "test"
+Requires-Dist: pytest-beartype >= 0.0.2 ; extra == "test"
 Requires-Dist: pytest-cov >= 4.1.0 ; extra == "test"
-Project-URL: Homepage, https://github.com/KyleKing/mdformat-gfm-alerts
+Project-URL: homepage, https://github.com/kyleking/mdformat-gfm-alerts
 Provides-Extra: dev
 Provides-Extra: test
 
 # mdformat-gfm-alerts
 
 [![Build Status][ci-badge]][ci-link] [![PyPI version][pypi-badge]][pypi-link]
 
@@ -72,16 +72,15 @@
 # <div class="markdown-alert markdown-alert-note">
 # <p class="markdown-alert-title">Note</p>
 # <p>Useful information that users should know, even when skimming content.</p>
 # </div>
 # </blockquote>
 ```
 
-> **Warning**
->
+> [!WARNING]
 > This package does not properly handle replacing the `blockquote` outer `div` with a `div` for accessibility. This should be possible with `markdown-it`, but I haven't yet found a way.
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/KyleKing/mdformat-gfm-alerts/blob/main/CONTRIBUTING.md)
 
 [ci-badge]: https://github.com/kyleking/mdformat-gfm-alerts/workflows/CI/badge.svg?branch=main
```

