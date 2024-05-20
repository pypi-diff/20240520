# Comparing `tmp/eulertools-2.1.0.tar.gz` & `tmp/eulertools-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulertools-2.1.0.tar", max compression
+gzip compressed data, was "eulertools-3.0.0.tar", max compression
```

## Comparing `eulertools-2.1.0.tar` & `eulertools-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     2117 2023-10-28 22:11:02.232347 eulertools-2.1.0/docs/README.md
--rw-r--r--   0        0        0     2772 2023-12-06 18:29:34.714699 eulertools-2.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-15 11:17:41.471041 eulertools-2.1.0/src/eulertools/__init__.py
--rw-r--r--   0        0        0       22 2023-12-06 18:29:43.397824 eulertools-2.1.0/src/eulertools/__version__.py
--rw-r--r--   0        0        0     2801 2023-10-26 11:54:22.746975 eulertools-2.1.0/src/eulertools/compare.py
--rw-r--r--   0        0        0      207 2023-10-26 22:44:37.486503 eulertools-2.1.0/src/eulertools/exceptions.py
--rw-r--r--   0        0        0      871 2023-10-24 22:48:32.565182 eulertools-2.1.0/src/eulertools/generate.py
--rw-r--r--   0        0        0     4016 2023-12-06 10:22:40.033365 eulertools-2.1.0/src/eulertools/main.py
--rw-r--r--   0        0        0     4054 2023-12-06 10:15:47.720028 eulertools-2.1.0/src/eulertools/run.py
--rw-r--r--   0        0        0      939 2023-10-19 19:07:44.300476 eulertools-2.1.0/src/eulertools/statement.py
--rw-r--r--   0        0        0      910 2023-10-26 11:54:22.866975 eulertools-2.1.0/src/eulertools/test.py
--rw-r--r--   0        0        0     3813 2023-12-06 10:24:35.050032 eulertools-2.1.0/src/eulertools/time.py
--rw-r--r--   0        0        0     8394 2023-10-27 14:04:24.151212 eulertools-2.1.0/src/eulertools/utils.py
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 eulertools-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7696 2024-05-03 11:21:21.641696 eulertools-3.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2121 2024-05-02 15:56:28.389983 eulertools-3.0.0/docs/README.md
+-rw-r--r--   0        0        0     3151 2024-05-20 15:09:14.967193 eulertools-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-15 11:17:41.471041 eulertools-3.0.0/src/eulertools/__init__.py
+-rw-r--r--   0        0        0     3918 2024-05-20 10:31:59.098734 eulertools-3.0.0/src/eulertools/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-20 15:09:20.647070 eulertools-3.0.0/src/eulertools/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-17 14:48:27.711640 eulertools-3.0.0/src/eulertools/lib/__init__.py
+-rw-r--r--   0        0        0      207 2023-10-26 22:44:37.486503 eulertools-3.0.0/src/eulertools/lib/exceptions.py
+-rw-r--r--   0        0        0     8962 2024-05-20 12:55:58.679818 eulertools-3.0.0/src/eulertools/lib/utils.py
+-rw-r--r--   0        0        0        0 2024-05-17 14:45:18.800978 eulertools-3.0.0/src/eulertools/subcommands/__init__.py
+-rw-r--r--   0        0        0     2980 2024-05-20 11:04:41.521205 eulertools-3.0.0/src/eulertools/subcommands/compare.py
+-rw-r--r--   0        0        0      917 2024-05-20 10:34:28.119065 eulertools-3.0.0/src/eulertools/subcommands/generate.py
+-rw-r--r--   0        0        0     4253 2024-05-20 12:55:58.516489 eulertools-3.0.0/src/eulertools/subcommands/run.py
+-rw-r--r--   0        0        0      956 2024-05-20 10:35:55.387334 eulertools-3.0.0/src/eulertools/subcommands/statement.py
+-rw-r--r--   0        0        0      979 2024-05-20 11:22:55.712555 eulertools-3.0.0/src/eulertools/subcommands/test.py
+-rw-r--r--   0        0        0     3885 2024-05-20 12:12:16.951976 eulertools-3.0.0/src/eulertools/subcommands/time.py
+-rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 eulertools-3.0.0/PKG-INFO
```

### Comparing `eulertools-2.1.0/docs/README.md` & `eulertools-3.0.0/docs/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 the timings between solutions in different languages.
 
 For the required project structure, installation instructions, and usage,
 please view the detailed [Documentation].
 
 ## Links
 
-- [Documentation]
-- [Changelog]
+-   [Documentation]
+-   [Changelog]
 
 [test_badge]: https://github.com/spapanik/eulertools/actions/workflows/tests.yml/badge.svg
 [test_url]: https://github.com/spapanik/eulertools/actions/workflows/tests.yml
 [licence_badge]: https://img.shields.io/github/license/spapanik/eulertools
 [licence_url]: https://github.com/spapanik/eulertools/blob/main/docs/LICENSE.md
 [pypi_badge]: https://img.shields.io/pypi/v/eulertools
 [pypi_url]: https://pypi.org/project/eulertools
```

### Comparing `eulertools-2.1.0/pyproject.toml` & `eulertools-3.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,74 +25,88 @@
 warn_return_any = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_unreachable = true
 warn_unused_configs = true
 
 [tool.ruff]
+src = [
+    "src",
+]
+target-version = "py311"
+
+[tool.ruff.lint]
 select = [
     "A",
     "ARG",
+    "ASYNC",
     "B",
     "BLE",
     "C4",
+    "COM",
     "DTZ",
     "E",
+    "EM",
     "ERA",
     "EXE",
     "F",
+    "FA",
     "FBT",
+    "FLY",
     "G",
     "I",
+    "ICN",
     "INP",
     "ISC",
+    "LOG",
     "N",
     "PGH",
+    "PERF",
     "PIE",
     "PLC",
     "PLE",
     "PLW",
     "PT",
     "PTH",
+    "Q",
     "RET",
     "RSE",
     "RUF",
     "S",
     "SIM",
     "SLF",
+    "SLOT",
     "T10",
     "TID",
     "TRY",
     "UP",
     "W",
+    "YTT",
 ]
 ignore = [
+    "COM812",
     "E501",
     "TRY003",
 ]
-src = [
-    "src",
-]
-target-version = "py311"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**" = [
     "FBT001",
     "PT011",
     "S101",
 ]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.flake8-tidy-imports.banned-api]
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
 "mock".msg = "Use unittest.mock"
 "pytz".msg = "Use zoneinfo"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 forced-separate = [
     "tests",
 ]
 split-on-trailing-comma = false
 
 [tool.pytest.ini_options]
@@ -108,59 +122,63 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "eulertools"
-version = "2.1.0"
+version = "3.0.0"
 description = "Multilanguage competitive coding toolbox"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "docs/README.md"
 
-homepage = "https://eulertools.readthedocs.io/en/latest/"
+homepage = "https://eulertools.readthedocs.io/en/stable/"
 repository = "https://github.com/spapanik/eulertools"
 documentation = "https://eulertools.readthedocs.io/en/stable/"
 
 keywords = [
     "leetcode",
     "topcoder",
     "project_euler",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.scripts]
-euler = "eulertools.main:main"
+euler = "eulertools.__main__:main"
 
 [tool.poetry.dependencies]
 # python version
 python = "^3.11"
 
 # dependencies
-dj_settings = "^4.2"
+dj_settings = "^5.0"
 jinja2 = "^3.1"
+pyutilkit = "^0.4"
 
 [tool.poetry.group.dev.dependencies]
-ipdb = "^0.13"
-ipython = "^8.12"
-pipdeptree = "^2.7"
+ipdb = { version = "^0.13", python = "^3.10" }
+ipython = { version = "^8.21", python = "^3.10" }
+pickleshare = { version = "^0.7", python = "^3.10" }
+pipdeptree = "^2.13"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.3"
-mypy = "^1.2"
-ruff = "^0.1"
+black = "^24.1"
+mypy = "^1.8"
+ruff = "^0.4"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3"
-pytest-cov = "^4.0"
+pytest = "^8.0"
+pytest-cov = "^5.0"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "^1.5"
-mkdocs-material = "^9.4"
-pygments = "^2.16"
+mkdocs = "^1.6"
+mkdocs-material = "^9.5"
+mkdocs-material-extensions = "^1.3"
+Pygments = "^2.17"
+pymdown-extensions = "^10.8"
```

### Comparing `eulertools-2.1.0/src/eulertools/compare.py` & `eulertools-3.0.0/src/eulertools/subcommands/compare.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from itertools import chain
 
-from eulertools.utils import Language, get_all_keyed_problems, get_timings
+from eulertools.lib.utils import Language, Problem, get_all_keyed_problems, get_timings
 
 
 class Compare:
-    def __init__(self, languages: list[Language], problems: list[str]):
+    def __init__(self, languages: list[Language], problems: list[Problem]):
         self.languages = languages
         self.timings = {language: get_timings(language) for language in languages}
         self.keyed_problems = self.get_keyed_problems(languages, problems)
         self.pad_length = self._pad_length()
 
     def run(self) -> None:
+        labels = [
+            ["problem", "id"],
+            *[[problem, str(key)] for problem, key in self.keyed_problems],
+        ]
         matrix = [
-            ["problem", *(f"{problem}/{key}" for problem, key in self.keyed_problems)],
+            *self.transpose(labels),
             *(self.get_language_timings(language) for language in self.languages),
         ]
         self.print_table(self.transpose(matrix))
 
     def print_table(self, matrix: list[list[str]]) -> None:
-        n = len(self.languages) + 1
+        n = len(self.languages) + 2
         spacing = ["─" * self.pad_length for _ in range(n)]
         top = "┌" + "┬".join(spacing) + "┐"
         mid = "├" + "┼".join(spacing) + "┤"
         btm = "└" + "┴".join(spacing) + "┘"
         print(top)
         for i, row in enumerate(matrix):
             if i % 4 == 1:
@@ -52,27 +56,28 @@
 
     def padded_print(self, string: str, *, heading: bool) -> str:
         if heading:
             return string.center(self.pad_length)
         return string.rjust(self.pad_length)
 
     def get_keyed_problems(
-        self, languages: list[Language], problems: list[str]
+        self, languages: list[Language], problems: list[Problem]
     ) -> list[tuple[str, int]]:
+        problem_ids = {problem.id for problem in problems}
         return [
             (problem, key)
             for problem, key in get_all_keyed_problems()
             if any(
                 problem_key
                 for language in languages
                 for problem_key in self.timings[language].get(problem, {})
             )
-            and problem in problems
+            and problem in problem_ids
         ]
 
     def _pad_length(self) -> int:
         lengths = chain(
             (len(problem) + len(str(key)) for problem, key in self.keyed_problems),
             (len(language.name) for language in self.languages),
-            [len("problem")],
+            [len("problem"), len("id")],
         )
         return max(lengths) + 2
```

### Comparing `eulertools-2.1.0/src/eulertools/generate.py` & `eulertools-3.0.0/src/eulertools/subcommands/generate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import jinja2
 
-from eulertools.utils import Language, get_context, get_solution, get_template
+from eulertools.lib.utils import (
+    Language,
+    Problem,
+    get_context,
+    get_solution,
+    get_template,
+)
 
 
 class Generate:
-    def __init__(self, languages: list[Language], problems: list[str]):
+    def __init__(self, languages: list[Language], problems: list[Problem]):
         self.languages = languages
         self.problems = problems
 
     def run(self) -> None:
         for problem in self.problems:
             for language in self.languages:
                 self.generate_solution(language, problem)
 
     @staticmethod
-    def generate_solution(language: Language, problem: str) -> None:
+    def generate_solution(language: Language, problem: Problem) -> None:
         template_path = get_template(language)
         solution = get_solution(language, problem)
         context = get_context(language, problem)
         if solution.exists():
             return
 
         template = jinja2.Template(
```

### Comparing `eulertools-2.1.0/src/eulertools/main.py` & `eulertools-3.0.0/src/eulertools/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 import sys
 
 from eulertools.__version__ import __version__
-from eulertools.compare import Compare
-from eulertools.generate import Generate
-from eulertools.run import Run
-from eulertools.statement import Statement
-from eulertools.test import Test
-from eulertools.time import Time
-from eulertools.utils import filter_languages, filter_problems
+from eulertools.lib.utils import filter_languages, filter_problems
+from eulertools.subcommands.compare import Compare
+from eulertools.subcommands.generate import Generate
+from eulertools.subcommands.run import Run
+from eulertools.subcommands.statement import Statement
+from eulertools.subcommands.test import Test
+from eulertools.subcommands.time import Time
 
 sys.tracebacklimit = 0
 
 
 def language_specific(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-l", "--language", nargs="*", dest="languages")
 
@@ -39,15 +39,15 @@
         "--verbose",
         action="count",
         default=0,
         dest="verbosity",
         help="increase the level of verbosity",
     )
 
-    subparsers = parser.add_subparsers(dest="command", required=True)
+    subparsers = parser.add_subparsers(dest="subcommand", required=True)
 
     generate_parser = subparsers.add_parser("generate", parents=[parent_parser])
     language_specific(generate_parser)
     problem_specific(generate_parser)
 
     run_parser = subparsers.add_parser("run", parents=[parent_parser])
     language_specific(run_parser)
@@ -71,47 +71,43 @@
     problem_specific(test_parser)
     test_parser.add_argument("-t", "--times", type=int, default=2)
 
     statement_parser = subparsers.add_parser("statement", parents=[parent_parser])
     problem_specific(statement_parser)
     statement_parser.add_argument("-s", "--show-hints", action="store_true")
 
-    options = parser.parse_args()
-    if options.verbosity > 0:
+    args = parser.parse_args()
+    if args.verbosity > 0:
         sys.tracebacklimit = 1000
-    if hasattr(options, "languages"):
-        options.languages = filter_languages(options.languages)
-        options.problems = filter_problems(options.problems, options.languages)
-    elif hasattr(options, "problems"):
-        options.problems = filter_problems(options.problems)
-    return options
+    if hasattr(args, "languages"):
+        args.languages = filter_languages(args.languages)
+        args.problems = filter_problems(args.problems, args.languages)
+    elif hasattr(args, "problems"):
+        args.problems = filter_problems(args.problems)
+
+    return args
 
 
 def main() -> None:
-    options = parse_args()
-    match options.command:
+    args = parse_args()
+    match args.subcommand:
         case "generate":
-            Generate(options.languages, options.problems).run()
+            Generate(args.languages, args.problems).run()
         case "run":
             Run(
-                options.languages,
-                options.problems,
-                options.verbosity,
-                run_update=options.update,
+                args.languages, args.problems, args.verbosity, run_update=args.update
             ).run()
         case "time":
             Time(
-                options.languages,
-                options.problems,
-                options.times,
-                options.verbosity,
-                run_update=options.update,
-                append_new=options.append,
+                args.languages,
+                args.problems,
+                args.times,
+                args.verbosity,
+                run_update=args.update,
+                append_new=args.append,
             ).run()
         case "test":
-            Test(
-                options.languages, options.problems, options.times, options.verbosity
-            ).run()
+            Test(args.languages, args.problems, args.times, args.verbosity).run()
         case "compare":
-            Compare(options.languages, options.problems).run()
+            Compare(args.languages, args.problems).run()
         case "statement":
-            Statement(options.problems, show_hints=options.show_hints).run()
+            Statement(args.problems, show_hints=args.show_hints).run()
```

### Comparing `eulertools-2.1.0/src/eulertools/run.py` & `eulertools-3.0.0/src/eulertools/subcommands/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import subprocess
 import sys
 from itertools import product
 
-from eulertools.exceptions import FailedRunError
-from eulertools.utils import (
+from pyutilkit.timing import Timing
+
+from eulertools.lib.exceptions import FailedRunError
+from eulertools.lib.utils import (
     Language,
     Modes,
-    Timing,
+    Problem,
     get_answers,
     get_line_answer,
     get_line_timing,
     get_solution,
     update_answers,
 )
 
 
 class Run:
     def __init__(
         self,
         languages: list[Language],
-        problems: list[str],
+        problems: list[Problem],
         verbosity: int,
         *,
         run_update: bool = False,
         times: int = 1,
         mode: str = Modes.RUN,
     ):
         self.languages = languages
@@ -34,27 +36,27 @@
         self.expected_answers = get_answers()
         self.run_update = run_update
 
     def run(self) -> dict[Language, dict[str, dict[int, list[Timing]]]]:
         output: dict[Language, dict[str, dict[int, list[Timing]]]] = {}
         for language, problem in product(self.languages, self.problems):
             timings = self.run_single_problem(language, problem)
-            output.setdefault(language, {})[problem] = timings
+            output.setdefault(language, {})[problem.id] = timings
         if self.run_update:
             update_answers(self.expected_answers)
         return output
 
     def run_single_problem(
-        self, language: Language, problem: str
+        self, language: Language, problem: Problem
     ) -> dict[int, list[Timing]]:
         solution = get_solution(language, problem)
         if not solution.exists():
             return {}
         raw_output = subprocess.run(
-            [language.runner, problem, str(self.times)],  # noqa: S603
+            [language.runner, problem.id, str(self.times)],  # noqa: S603
             capture_output=True,
             check=True,
         )
         output = raw_output.stdout.decode()
         if self.verbosity > 3:
             print(output)
         actual_answers: dict[int, set[str]] = {}
@@ -64,46 +66,49 @@
                 _, run_id, timing = get_line_timing(line)
                 timings.setdefault(run_id, []).append(timing)
             elif line.startswith("Answer"):
                 _, run_id, answer = get_line_answer(line)
                 actual_answers.setdefault(run_id, set()).add(answer)
             else:
                 print(
-                    f"🔴 Running {language.name}/{problem}... Cannot parse `{line}`.",
+                    f"🔴 Running {language.name} // {problem.id}... Cannot parse `{line}`.",
                     file=sys.stderr,
                 )
-                raise FailedRunError(f"Unsuccessful run of {language.name}/{problem}")
-        expected_answers = self.expected_answers.setdefault(problem, {})
+                msg = f"Unsuccessful run of {language.name} // {problem.id}"
+                raise FailedRunError(msg)
+        expected_answers = self.expected_answers.setdefault(problem.id, {})
         if missing_answers := {
             answer for answer in expected_answers if answer not in actual_answers
         }:
             print(
-                f"🔴 Running {language.name}/{problem}... Missing answers with keys {missing_answers}.",
+                f"🔴 Running {language.name} // {problem.id}... Missing answers with keys {missing_answers}.",
                 file=sys.stderr,
             )
-            raise FailedRunError(f"Unsuccessful run of {language.name}/{problem}")
+            msg = f"Unsuccessful run of {language.name} // {problem.id}"
+            raise FailedRunError(msg)
         success = True
         for key, values in actual_answers.items():
             value = values.pop()
             if len(values) != 0:
                 success = False
                 print(
-                    f"🔴 Running {language.name}/{problem}/{key}... Not deterministic answer.",
+                    f"🔴 Running {language.name} // {problem.id} // {key}... Not deterministic answer.",
                     file=sys.stderr,
                 )
             elif key not in expected_answers:
                 if self.mode != Modes.TIMING:
                     print(
-                        f"🟠 Running {language.name}/{problem}/{key}... new response: {value}"
+                        f"🟠 Running {language.name} // {problem.id} // {key}... new response: {value}"
                     )
                 expected_answers[key] = value
             elif value != expected_answers[key]:
                 success = False
                 print(
-                    f"🔴 Running {language.name}/{problem}/{key}... expected: {expected_answers[key]}, got: {value}",
+                    f"🔴 Running {language.name} // {problem.id} // {key}... expected: {expected_answers[key]}, got: {value}",
                     file=sys.stderr,
                 )
             elif self.mode != Modes.TIMING:
-                print(f"🟢 Running {language.name}/{problem}/{key}... {value}")
+                print(f"🟢 Running {language.name} // {problem.id} // {key}... {value}")
         if not success:
-            raise FailedRunError(f"Unsuccessful run of {language.name}/{problem}")
+            msg = f"Unsuccessful run of {language.name} // {problem.id}"
+            raise FailedRunError(msg)
         return timings
```

### Comparing `eulertools-2.1.0/src/eulertools/test.py` & `eulertools-3.0.0/src/eulertools/subcommands/test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from itertools import product
 
-from eulertools.run import Run
-from eulertools.utils import Language, Modes, get_solution
+from eulertools.lib.utils import Language, Modes, Problem, get_solution
+from eulertools.subcommands.run import Run
 
 
 class Test:
     def __init__(
-        self, languages: list[Language], problems: list[str], times: int, verbosity: int
+        self,
+        languages: list[Language],
+        problems: list[Problem],
+        times: int,
+        verbosity: int,
     ):
         self.languages = languages
         self.problems = problems
         self.times = times
         self.verbosity = verbosity
 
     def run(self) -> None:
         for language, problem in product(self.languages, self.problems):
             self.test_single_problem(language, problem)
 
-    def test_single_problem(self, language: Language, problem: str) -> None:
+    def test_single_problem(self, language: Language, problem: Problem) -> None:
         solution = get_solution(language, problem)
         if not solution.exists():
             return
 
         Run(
             [language],
             [problem],
             verbosity=self.verbosity,
             mode=Modes.RUN,
             times=self.times,
-        ).run()[language][problem]
+        ).run()[language][problem.id]
```

### Comparing `eulertools-2.1.0/src/eulertools/time.py` & `eulertools-3.0.0/src/eulertools/subcommands/time.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from itertools import product
 
-from eulertools.run import Run
-from eulertools.utils import (
-    ANSIEscape,
+from pyutilkit.term import SGRCodes, SGRString
+
+from eulertools.lib.utils import (
     Language,
     Modes,
+    Problem,
     get_average,
     get_solution,
     get_timings,
     update_timings,
 )
+from eulertools.subcommands.run import Run
 
 
 class Time:
     def __init__(
         self,
         languages: list[Language],
-        problems: list[str],
+        problems: list[Problem],
         times: int,
         verbosity: int,
         *,
         run_update: bool,
         append_new: bool,
     ):
         self.languages = languages
@@ -37,29 +39,29 @@
         ):
             self.time_single_problem(language, problem, run_index)
         if self.run_update or self.append_new:
             for language in self.languages:
                 update_timings(language, self.timings[language])
 
     def time_single_problem(
-        self, language: Language, problem: str, run_index: int
+        self, language: Language, problem: Problem, run_index: int
     ) -> None:
-        self.timings[language].setdefault(problem, {})
+        self.timings[language].setdefault(problem.id, {})
         solution = get_solution(language, problem)
         if not solution.exists():
             return
 
         raw_timings = Run(
             [language],
             [problem],
             verbosity=self.verbosity,
             mode=Modes.TIMING,
             times=self.times,
-        ).run()[language][problem]
-        old_timings = self.timings[language][problem]
+        ).run()[language][problem.id]
+        old_timings = self.timings[language][problem.id]
         new_timings = {
             run_id: get_average(timings) for run_id, timings in raw_timings.items()
         }
         for key_index, key in enumerate(sorted(new_timings)):
             old_timing = old_timings.get(key)
             raw_timing = raw_timings[key]
             new_timing = new_timings[key]
@@ -68,20 +70,20 @@
             elif old_timing < new_timing:
                 overall_difference = "🔴"
             elif old_timing > new_timing:
                 overall_difference = "🟢"
             else:
                 overall_difference = "🔵"
             if self.run_update or (self.append_new and old_timing is None):
-                self.timings[language][problem][key] = new_timing
-            title = f"Timing {language.name}/{problem}/{key}..."
+                self.timings[language][problem.id][key] = new_timing
+            title = f"Timing {language.name} // {problem.id} // {key}..."
             if run_index or key_index:
                 print()
-            print(ANSIEscape.OKGREEN, title, ANSIEscape.ENDC, sep="")
-            print(ANSIEscape.OKGREEN, "~" * len(title), ANSIEscape.ENDC, sep="")
+            print(SGRString(title, params=[SGRCodes.GREEN]))
+            print(SGRString("~" * len(title), params=[SGRCodes.GREEN]))
             if old_timing:
                 print(f"🟤 Old timing: {old_timing}")
             prefix = (
                 f"{overall_difference} New" if old_timing is not None else "🔵 Initial"
             )
             print(f"{prefix} timing: {new_timing}")
             if self.verbosity > 0:
```

### Comparing `eulertools-2.1.0/src/eulertools/utils.py` & `eulertools-3.0.0/src/eulertools/lib/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,93 @@
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass, field
-from decimal import Decimal
 from enum import StrEnum, unique
 from pathlib import Path
 from typing import Any, Self
 
-from dj_settings import SettingsParser
+from dj_settings import ConfigParser
+from pyutilkit.timing import Timing
 
-from eulertools.exceptions import (
+from eulertools.__version__ import __version__
+from eulertools.lib.exceptions import (
     InvalidLanguageError,
     InvalidProblemError,
     MissingProjectRootError,
 )
 
 TIME_UNIT = re.compile(r"(\d+(?:\.\d+)?)\s?(.{0,2})")
 
 
 @unique
-class ANSIEscape(StrEnum):
-    ENDC = "\033[0m"
-    BOLD = "\033[1m"
-    FAIL = "\033[31m"
-    OKGREEN = "\033[32m"
-    OKBLUE = "\033[34m"
-    WARNING = "\033[33m"
-
-
-@unique
 class Modes(StrEnum):
     TIMING = "timing"
     RUN = "run"
 
 
 @dataclass(frozen=True, slots=True, order=True)
-class Timing:
-    time: Decimal = field(compare=False)
-    unit: str = field(compare=False)
-    nanoseconds: int = field(repr=False)
-
-    @classmethod
-    def from_nanoseconds(cls, nanoseconds: int) -> Self:
-        if nanoseconds < 1000:
-            return cls(time=Decimal(nanoseconds), unit="ns", nanoseconds=nanoseconds)
-        microseconds = nanoseconds / 1000
-        if microseconds < 1000:
-            return cls(
-                time=Decimal(f"{microseconds:.1f}"), unit="µs", nanoseconds=nanoseconds
-            )
-        milliseconds = microseconds / 1000
-        if milliseconds < 1000:
-            return cls(
-                time=Decimal(f"{milliseconds:.1f}"), unit="ms", nanoseconds=nanoseconds
-            )
-        seconds = milliseconds / 1000
-        return cls(time=Decimal(f"{seconds:.2f}"), unit="s", nanoseconds=nanoseconds)
-
-    def __str__(self) -> str:
-        return f"{self.time}{self.unit}"
-
-
-@dataclass(frozen=True, slots=True, order=True)
 class Language:
     name: str
     extension: str = field(repr=False, compare=False)
     path: Path = field(repr=False, compare=False)
+    solutions_path: Path = field(repr=False, compare=False)
     runner: Path = field(repr=False, compare=False)
 
     @classmethod
     def from_settings(cls, name: str) -> Self:
         project_root = _get_project_root()
         settings = get_settings()
         language = settings["languages"][name]
+        path = project_root.joinpath(language.get("path", name))
+        solutions = language.get("solutions", "src/solutions")
         return cls(
             name=name,
             extension=language.get("extension", name),
-            path=project_root.joinpath(language.get("path", name)),
-            runner=project_root.joinpath(language["runner"]),
+            path=path,
+            runner=path.joinpath(language["runner"]),
+            solutions_path=path.joinpath(solutions),
         )
 
     def get_settings_root(self) -> Path:
         project_root = _get_project_root()
         project_settings_root = _get_settings_root()
         path = project_settings_root.joinpath(self.path.relative_to(project_root))
         if not path.exists():
             path.mkdir(parents=True)
         return path
 
 
+@dataclass(frozen=True, slots=True, order=True)
+class Problem:
+    id: str
+    statement: Path
+    path: Path
+
+
+@dataclass(frozen=True, slots=True, order=True)
+class Version:
+    major: int
+    minor: int
+    patch: int
+
+    @classmethod
+    def from_string(cls, version: str) -> Version:
+        version = re.sub("[^.0-9].*", "", version)
+        if version.endswith("."):
+            version += "0"
+        while version.count(".") < 2:
+            version += ".0"
+        major, minor, patch, *_ = map(int, version.split("."))
+        return cls(major, minor, patch)
+
+    def __str__(self) -> str:
+        return f"{self.major}.{self.minor}.{self.patch}"
+
+
 def _get_project_root() -> Path:
     cwd = Path.cwd().resolve()
     while not cwd.joinpath(".euler").is_dir():
         if cwd.as_posix() == "/":
             message = f"Could not find .euler/euler.toml in {Path.cwd().resolve()} or any parent directory"
             raise MissingProjectRootError(message)
         cwd = cwd.parent
@@ -121,37 +116,47 @@
     return file
 
 
 def _get_statements_dir() -> Path:
     return _get_settings_root().joinpath("statements")
 
 
-def _get_statement(problem: str) -> Path:
-    return _get_statements_dir().joinpath(f"{problem}.toml")
-
-
 def get_template(language: Language) -> Path:
     return language.get_settings_root().joinpath("solution.jinja")
 
 
-def get_solution(language: Language, problem: str) -> Path:
-    return language.path.joinpath("src", "solutions", f"{problem}.{language.extension}")
+def get_solution(language: Language, problem: Problem) -> Path:
+    suffix = f".{language.extension}"
+    return language.solutions_path.joinpath(problem.path).with_suffix(suffix)
+
 
+def get_config(path: Path) -> dict[str, Any]:
+    return ConfigParser([path]).data
 
-def get_statement(problem: str) -> dict[str, Any]:
-    return SettingsParser(_get_statement(problem)).data
+
+def get_statement(problem: Problem) -> dict[str, Any]:
+    return ConfigParser([problem.statement]).data
 
 
 def get_settings() -> dict[str, Any]:
-    return SettingsParser(_get_settings()).data
+    data = ConfigParser([_get_settings()]).data
+    version_string = data.get("$meta", {}).get("version")
+    if version_string is None:
+        msg = "This `euler.toml` is missing a version"
+        raise RuntimeError(msg)
+    min_version = Version.from_string(data["$meta"]["version"])
+    if min_version > Version.from_string(__version__):
+        msg = f"This `euler.toml` requires an eulertools >= v{min_version}"
+        raise RuntimeError(msg)
+    return data
 
 
 def get_line_timing(line: str) -> tuple[str, int, Timing]:
     prefix, run_id, timing = line.split(maxsplit=2)
-    return prefix, int(run_id), Timing.from_nanoseconds(int(timing) or 1)
+    return prefix, int(run_id), Timing(nanoseconds=int(timing) or 1)
 
 
 def get_line_answer(line: str) -> tuple[str, int, str]:
     prefix, run_id, *answers = line.split(maxsplit=2)
     try:
         answer = answers.pop()
     except IndexError:
@@ -173,17 +178,17 @@
     output: dict[str, dict[int, Timing]] = {}
     for line in timings.read_text().splitlines():
         problem, mode_id, timing = get_line_timing(line)
         output.setdefault(problem, {})[mode_id] = timing
     return output
 
 
-def get_context(language: Language, problem: str) -> dict[str, str]:
+def get_context(language: Language, problem: Problem) -> dict[str, str]:
     statement = get_statement(problem)
-    output = {"problem": problem}
+    output = {"problem": problem.id}
     output |= statement.get(language.name, {})
     return output
 
 
 def update_answers(answers: dict[str, dict[int, str]]) -> None:
     answers_path = _get_answers()
     with answers_path.open("w") as file:
@@ -199,37 +204,46 @@
         for problem in sorted(timings):
             for key in sorted(timings[problem]):
                 timing = timings[problem][key]
                 file.write(f"{problem} {key} {timing.nanoseconds}\n")
 
 
 def get_average(values: list[Timing]) -> Timing:
+    if not values:
+        return Timing()
     if len(values) >= 3:
         values = sorted(values)[1:-1]
-    average_ns = sum(value.nanoseconds for value in values) // len(values)
-    return Timing.from_nanoseconds(average_ns)
+    return sum(values, start=Timing()) // len(values)
 
 
 def get_all_languages() -> list[Language]:
     languages = get_settings()["languages"]
     return sorted(Language.from_settings(language) for language in languages)
 
 
-def get_all_problems(languages: list[Language] | None = None) -> list[str]:
+def get_all_problems(languages: list[Language] | None = None) -> dict[str, Problem]:
     statement_dir = _get_statements_dir()
     if languages is None:
         languages = get_all_languages()
-    return sorted(
-        file.stem
-        for file in statement_dir.iterdir()
-        if any(
-            get_statement(file.stem).get(language.name) is not None
-            for language in languages
-        )
-    )
+
+    output = {}
+    for file in sorted(statement_dir.rglob("*")):
+        if not file.is_file():
+            continue
+        statement = get_config(file)
+        if any(statement.get(language.name) is not None for language in languages):
+            path = file.relative_to(statement_dir)
+            id_ = statement["common"].get("id", path.as_posix())
+            problem = Problem(id=id_, statement=file, path=path)
+            if id_ in output:
+                msg = f"Duplicate problem id: {id_}"
+                raise ValueError(msg)
+            output[id_] = problem
+
+    return output
 
 
 def get_all_keyed_problems() -> list[tuple[str, int]]:
     output = [
         (problem, key)
         for problem, problem_info in get_answers().items()
         for key in problem_info
@@ -241,30 +255,30 @@
     all_languages = get_all_languages()
     if parsed_languages is None:
         return all_languages
     filtered_languages = []
     language_names = {language.name for language in all_languages}
     for language in parsed_languages:
         if language not in language_names:
-            raise InvalidLanguageError(f"{language} is not a valid language")
+            msg = f"{language} is not a valid language"
+            raise InvalidLanguageError(msg)
         filtered_languages.append(Language.from_settings(language))
     return filtered_languages
 
 
 def filter_problems(
     parsed_problems: list[str], languages: list[Language] | None = None
-) -> list[str]:
+) -> list[Problem]:
     all_problems = get_all_problems(languages)
     if not parsed_problems:
-        return sorted(all_problems)
+        return sorted(all_problems.values())
     filtered_problems = []
     for problem in parsed_problems:
         if problem not in all_problems:
             if languages is None:
-                raise InvalidProblemError(
-                    f"{problem} is not a valid problem for any language"
-                )
-            raise InvalidProblemError(
-                f"{problem} is not a valid problem for {', '.join(language.name for language in languages)}"
-            )
-        filtered_problems.append(problem)
+                language_names = "any language"
+            else:
+                language_names = ", ".join(language.name for language in languages)
+            msg = f"{problem} is not a valid problem for {language_names}"
+            raise InvalidProblemError(msg)
+        filtered_problems.append(all_problems[problem])
     return filtered_problems
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eulertools-2.1.0/PKG-INFO` & `eulertools-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: eulertools
-Version: 2.1.0
+Version: 3.0.0
 Summary: Multilanguage competitive coding toolbox
-Home-page: https://eulertools.readthedocs.io/en/latest/
+Home-page: https://eulertools.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: leetcode,topcoder,project_euler
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: dj_settings (>=4.2,<5.0)
+Requires-Dist: dj_settings (>=5.0,<6.0)
 Requires-Dist: jinja2 (>=3.1,<4.0)
+Requires-Dist: pyutilkit (>=0.4,<0.5)
 Project-URL: Documentation, https://eulertools.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/spapanik/eulertools
 Description-Content-Type: text/markdown
 
 # eulertools: Multilanguage competitive coding toolbox
 
 [![tests][test_badge]][test_url]
@@ -41,16 +42,16 @@
 the timings between solutions in different languages.
 
 For the required project structure, installation instructions, and usage,
 please view the detailed [Documentation].
 
 ## Links
 
-- [Documentation]
-- [Changelog]
+-   [Documentation]
+-   [Changelog]
 
 [test_badge]: https://github.com/spapanik/eulertools/actions/workflows/tests.yml/badge.svg
 [test_url]: https://github.com/spapanik/eulertools/actions/workflows/tests.yml
 [licence_badge]: https://img.shields.io/github/license/spapanik/eulertools
 [licence_url]: https://github.com/spapanik/eulertools/blob/main/docs/LICENSE.md
 [pypi_badge]: https://img.shields.io/pypi/v/eulertools
 [pypi_url]: https://pypi.org/project/eulertools
```

