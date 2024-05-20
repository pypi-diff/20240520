# Comparing `tmp/pyproject_fmt_rust-1.1.1.tar.gz` & `tmp/pyproject_fmt_rust-1.1.2.tar.gz`

## Comparing `pyproject_fmt_rust-1.1.1.tar` & `pyproject_fmt_rust-1.1.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.1/Cargo.toml
--rw-r--r--   0     1001      127       36 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.github/FUNDING.yml
--rw-r--r--   0     1001      127      365 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.github/SECURITY.md
--rw-r--r--   0     1001      127      117 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.github/dependabot.yml
--rw-r--r--   0     1001      127       76 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.github/release.yml
--rw-r--r--   0     1001      127     2248 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.github/workflows/check.yml
--rw-r--r--   0     1001      127     3714 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.github/workflows/release.yml
--rw-r--r--   0     1001      127      158 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.gitignore
--rw-r--r--   0     1001      127      973 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      240 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127       16 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/.rustfmt.toml
--rw-r--r--   0     1001      127     3256 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1023 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/LICENSE.txt
--rw-r--r--   0     1001      127      861 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/README.md
--rw-r--r--   0     1001      127     3185 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/build_system.rs
--rw-r--r--   0     1001      127     3447 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/data/ruff-order.expected.toml
--rw-r--r--   0     1001      127     3281 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/data/ruff-order.start.toml
--rw-r--r--   0     1001      127     3755 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/global.rs
--rw-r--r--   0     1001      127     8964 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/helpers/array.rs
--rw-r--r--   0     1001      127     4529 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/helpers/create.rs
--rw-r--r--   0     1001      127       78 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/helpers/mod.rs
--rw-r--r--   0     1001      127     4595 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/helpers/pep508.rs
--rw-r--r--   0     1001      127     1605 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/helpers/string.rs
--rw-r--r--   0     1001      127    11500 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/helpers/table.rs
--rw-r--r--   0     1001      127     7134 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/main.rs
--rw-r--r--   0     1001      127    30465 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/project.rs
--rw-r--r--   0     1001      127     8213 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust/src/ruff.rs
--rw-r--r--   0     1001      127       29 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/rust-toolchain.toml
--rw-r--r--   0     1001      127      161 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/src/pyproject_fmt_rust/__init__.py
--rw-r--r--   0     1001      127      638 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/src/pyproject_fmt_rust/_lib.pyi
--rw-r--r--   0     1001      127        0 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/src/pyproject_fmt_rust/py.typed
--rw-r--r--   0     1001      127      991 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/tests/test_main.py
--rw-r--r--   0     1001      127     2081 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/tox.ini
--rw-r--r--   0     1001      127    26478 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/Cargo.lock
--rw-r--r--   0     1001      127     3312 2024-05-15 02:22:45.000000 pyproject_fmt_rust-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.2/Cargo.toml
+-rw-r--r--   0     1001      127       36 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      365 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.github/SECURITY.md
+-rw-r--r--   0     1001      127      117 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.github/dependabot.yml
+-rw-r--r--   0     1001      127       76 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.github/release.yml
+-rw-r--r--   0     1001      127     2248 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.github/workflows/check.yml
+-rw-r--r--   0     1001      127     3720 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      158 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.gitignore
+-rw-r--r--   0     1001      127      973 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      240 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127       16 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/.rustfmt.toml
+-rw-r--r--   0     1001      127     3256 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1023 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/LICENSE.txt
+-rw-r--r--   0     1001      127      861 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/README.md
+-rw-r--r--   0     1001      127     3185 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/build_system.rs
+-rw-r--r--   0     1001      127      309 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/data/ruff-21.expected.toml
+-rw-r--r--   0     1001      127      295 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/data/ruff-21.start.toml
+-rw-r--r--   0     1001      127     3447 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/data/ruff-order.expected.toml
+-rw-r--r--   0     1001      127     3281 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/data/ruff-order.start.toml
+-rw-r--r--   0     1001      127     3755 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/global.rs
+-rw-r--r--   0     1001      127     8859 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/helpers/array.rs
+-rw-r--r--   0     1001      127     4406 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/helpers/create.rs
+-rw-r--r--   0     1001      127       78 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/helpers/mod.rs
+-rw-r--r--   0     1001      127     4595 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/helpers/pep508.rs
+-rw-r--r--   0     1001      127     1531 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/helpers/string.rs
+-rw-r--r--   0     1001      127    12070 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/helpers/table.rs
+-rw-r--r--   0     1001      127     7134 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/main.rs
+-rw-r--r--   0     1001      127    29842 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/project.rs
+-rw-r--r--   0     1001      127     8547 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust/src/ruff.rs
+-rw-r--r--   0     1001      127       29 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/rust-toolchain.toml
+-rw-r--r--   0     1001      127      161 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/src/pyproject_fmt_rust/__init__.py
+-rw-r--r--   0     1001      127      638 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/src/pyproject_fmt_rust/_lib.pyi
+-rw-r--r--   0     1001      127        0 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/src/pyproject_fmt_rust/py.typed
+-rw-r--r--   0     1001      127      991 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/tests/test_main.py
+-rw-r--r--   0     1001      127     2081 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/tox.ini
+-rw-r--r--   0     1001      127    26478 2024-05-20 19:08:10.000000 pyproject_fmt_rust-1.1.2/Cargo.lock
+-rw-r--r--   0     1001      127     3312 2024-05-20 19:07:54.000000 pyproject_fmt_rust-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.1.2/PKG-INFO
```

### Comparing `pyproject_fmt_rust-1.1.1/Cargo.toml` & `pyproject_fmt_rust-1.1.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyproject-fmt-rust"
-version = "1.1.1"
+version = "1.1.2"
 description = "Format pyproject.toml files"
 repository = "https://github.com/tox-dev/pyproject-fmt"
 readme = "README.md"
 license = "MIT"
 edition = "2021"
 
 [lib]
```

### Comparing `pyproject_fmt_rust-1.1.1/.github/workflows/check.yml` & `pyproject_fmt_rust-1.1.2/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/.github/workflows/release.yml` & `pyproject_fmt_rust-1.1.2/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     environment:
       name: release
-      url: https://pypi.org/p/pyproject-fmt/rust
+      url: https://pypi.org/project/pyproject-fmt-rust
     permissions:
       id-token: write
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [ linux, windows, macos, sdist ]
     steps:
       - uses: actions/download-artifact@v4
       - name: Publish to PyPI
```

### Comparing `pyproject_fmt_rust-1.1.1/.pre-commit-config.yaml` & `pyproject_fmt_rust-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/CODE_OF_CONDUCT.md` & `pyproject_fmt_rust-1.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/LICENSE.txt` & `pyproject_fmt_rust-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/README.md` & `pyproject_fmt_rust-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/build_system.rs` & `pyproject_fmt_rust-1.1.2/rust/src/build_system.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/data/ruff-order.expected.toml` & `pyproject_fmt_rust-1.1.2/rust/src/data/ruff-order.expected.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/data/ruff-order.start.toml` & `pyproject_fmt_rust-1.1.2/rust/src/data/ruff-order.start.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/global.rs` & `pyproject_fmt_rust-1.1.2/rust/src/global.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/helpers/array.rs` & `pyproject_fmt_rust-1.1.2/rust/src/helpers/array.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 use std::cell::RefCell;
 use std::collections::HashMap;
 
 use lexical_sort::{natural_lexical_cmp, StringSort};
+use taplo::syntax::SyntaxKind::{ARRAY, COMMA, NEWLINE, STRING, VALUE, WHITESPACE};
 use taplo::syntax::{SyntaxElement, SyntaxKind, SyntaxNode};
 
 use crate::helpers::create::{make_comma, make_newline};
 use crate::helpers::string::{load_text, update_content};
 
 pub fn transform<F>(node: &SyntaxNode, transform: &F)
 where
     F: Fn(&str) -> String,
 {
     for array in node.children_with_tokens() {
-        if array.kind() == SyntaxKind::ARRAY {
+        if array.kind() == ARRAY {
             for array_entry in array.as_node().unwrap().children_with_tokens() {
-                if array_entry.kind() == SyntaxKind::VALUE {
+                if array_entry.kind() == VALUE {
                     update_content(array_entry.as_node().unwrap(), transform);
                 }
             }
         }
     }
 }
 
 pub fn sort<F>(node: &SyntaxNode, transform: F)
 where
     F: Fn(&str) -> String,
 {
     for array in node.children_with_tokens() {
-        if array.kind() == SyntaxKind::ARRAY {
+        if array.kind() == ARRAY {
             let array_node = array.as_node().unwrap();
             let mut value_set = Vec::<Vec<SyntaxElement>>::new();
             let entry_set = RefCell::new(Vec::<SyntaxElement>::new());
             let mut key_to_pos = HashMap::<String, usize>::new();
 
             let mut add_to_value_set = |entry: String| {
                 let mut entry_set_borrow = entry_set.borrow_mut();
@@ -49,21 +50,21 @@
             let mut count = 0;
 
             for entry in array_node.children_with_tokens() {
                 count += 1;
                 if previous_is_value {
                     // make sure ends with trailing comma
                     previous_is_value = false;
-                    if entry.kind() != SyntaxKind::COMMA {
+                    if entry.kind() != COMMA {
                         entry_set.borrow_mut().push(make_comma());
                     }
                 }
                 if previous_is_bracket_open {
                     // make sure ends with trailing comma
-                    if entry.kind() == SyntaxKind::NEWLINE || entry.kind() == SyntaxKind::WHITESPACE {
+                    if entry.kind() == NEWLINE || entry.kind() == WHITESPACE {
                         continue;
                     }
                     previous_is_bracket_open = false;
                 }
                 match &entry.kind() {
                     SyntaxKind::BRACKET_START => {
                         entries.push(entry);
@@ -74,39 +75,38 @@
                         if has_value {
                             add_to_value_set(entry_value.clone());
                         } else {
                             entries.extend(entry_set.borrow_mut().clone());
                         }
                         entries.push(entry);
                     }
-                    SyntaxKind::VALUE => {
+                    VALUE => {
                         if has_value {
                             entry_set.borrow_mut().push(make_newline());
                             add_to_value_set(entry_value.clone());
                         }
                         has_value = true;
                         let value_node = entry.as_node().unwrap();
                         let mut found_string = false;
                         for child in value_node.children_with_tokens() {
                             let kind = child.kind();
-                            if kind == SyntaxKind::STRING {
-                                entry_value =
-                                    transform(load_text(child.as_token().unwrap().text(), SyntaxKind::STRING).as_str());
+                            if kind == STRING {
+                                entry_value = transform(load_text(child.as_token().unwrap().text(), STRING).as_str());
                                 found_string = true;
                                 break;
                             }
                         }
                         if !found_string {
                             // abort if not correct types
                             return;
                         }
                         entry_set.borrow_mut().push(entry);
                         previous_is_value = true;
                     }
-                    SyntaxKind::NEWLINE => {
+                    NEWLINE => {
                         entry_set.borrow_mut().push(entry);
                         if has_value {
                             add_to_value_set(entry_value.clone());
                             has_value = false;
                         }
                     }
                     _ => {
@@ -129,15 +129,15 @@
 
 #[cfg(test)]
 mod tests {
     use indoc::indoc;
     use rstest::rstest;
     use taplo::formatter::{format_syntax, Options};
     use taplo::parser::parse;
-    use taplo::syntax::SyntaxKind;
+    use taplo::syntax::SyntaxKind::{ENTRY, VALUE};
 
     use crate::helpers::array::{sort, transform};
     use crate::helpers::pep508::format_requirement;
 
     #[rstest]
     #[case::strip_micro_no_keep(
         indoc ! {r#"
@@ -189,17 +189,17 @@
     a = ["importlib-metadata>=7; python_version<'3.8'"]
     "#},
         false
     )]
     fn test_normalize_requirement(#[case] start: &str, #[case] expected: &str, #[case] keep_full_version: bool) {
         let root_ast = parse(start).into_syntax().clone_for_update();
         for children in root_ast.children_with_tokens() {
-            if children.kind() == SyntaxKind::ENTRY {
+            if children.kind() == ENTRY {
                 for entry in children.as_node().unwrap().children_with_tokens() {
-                    if entry.kind() == SyntaxKind::VALUE {
+                    if entry.kind() == VALUE {
                         transform(entry.as_node().unwrap(), &|s| format_requirement(s, keep_full_version));
                     }
                 }
             }
         }
         let res = format_syntax(root_ast, Options::default());
         assert_eq!(expected, res);
@@ -271,17 +271,17 @@
       # extra
     ] # array comment
     "#}
     )]
     fn test_order_array(#[case] start: &str, #[case] expected: &str) {
         let root_ast = parse(start).into_syntax().clone_for_update();
         for children in root_ast.children_with_tokens() {
-            if children.kind() == SyntaxKind::ENTRY {
+            if children.kind() == ENTRY {
                 for entry in children.as_node().unwrap().children_with_tokens() {
-                    if entry.kind() == SyntaxKind::VALUE {
+                    if entry.kind() == VALUE {
                         sort(entry.as_node().unwrap(), str::to_lowercase);
                     }
                 }
             }
         }
         let opt = Options {
             column_width: 1,
```

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/helpers/create.rs` & `pyproject_fmt_rust-1.1.2/rust/src/helpers/create.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 use taplo::parser::parse;
-use taplo::syntax::{SyntaxElement, SyntaxKind};
+use taplo::syntax::SyntaxElement;
+use taplo::syntax::SyntaxKind::{ARRAY, COMMA, ENTRY, KEY, NEWLINE, STRING, VALUE};
 
 pub fn make_string_node(text: &str) -> SyntaxElement {
     let expr = &format!("a = \"{}\"", text.replace('"', "\\\""));
     for root in parse(expr)
         .into_syntax()
         .clone_for_update()
         .first_child()
         .unwrap()
         .children_with_tokens()
     {
-        if root.kind() == SyntaxKind::VALUE {
+        if root.kind() == VALUE {
             for entries in root.as_node().unwrap().children_with_tokens() {
-                if entries.kind() == SyntaxKind::STRING {
+                if entries.kind() == STRING {
                     return entries;
                 }
             }
         }
     }
     panic!("Could not create string element for {text:?}")
 }
 
 pub fn make_empty_newline() -> SyntaxElement {
     for root in parse("\n\n").into_syntax().clone_for_update().children_with_tokens() {
-        if root.kind() == SyntaxKind::NEWLINE {
+        if root.kind() == NEWLINE {
             return root;
         }
     }
     panic!("Could not create empty newline");
 }
 
 pub fn make_newline() -> SyntaxElement {
     for root in parse("\n").into_syntax().clone_for_update().children_with_tokens() {
-        if root.kind() == SyntaxKind::NEWLINE {
+        if root.kind() == NEWLINE {
             return root;
         }
     }
     panic!("Could not create newline");
 }
 
 pub fn make_comma() -> SyntaxElement {
     for root in parse("a=[1,2]").into_syntax().clone_for_update().children_with_tokens() {
-        if root.kind() == SyntaxKind::ENTRY {
+        if root.kind() == ENTRY {
             for value in root.as_node().unwrap().children_with_tokens() {
-                if value.kind() == SyntaxKind::VALUE {
+                if value.kind() == VALUE {
                     for array in value.as_node().unwrap().children_with_tokens() {
-                        if array.kind() == SyntaxKind::ARRAY {
+                        if array.kind() == ARRAY {
                             for e in array.as_node().unwrap().children_with_tokens() {
-                                if e.kind() == SyntaxKind::COMMA {
+                                if e.kind() == COMMA {
                                     return e;
                                 }
                             }
                         }
                     }
                 }
             }
@@ -62,17 +63,17 @@
 
 pub fn make_key(text: &str) -> SyntaxElement {
     for root in parse(format!("{text}=1").as_str())
         .into_syntax()
         .clone_for_update()
         .children_with_tokens()
     {
-        if root.kind() == SyntaxKind::ENTRY {
+        if root.kind() == ENTRY {
             for value in root.as_node().unwrap().children_with_tokens() {
-                if value.kind() == SyntaxKind::KEY {
+                if value.kind() == KEY {
                     return value;
                 }
             }
         }
     }
     panic!("Could not create key {text}");
 }
@@ -80,35 +81,35 @@
 pub fn make_array(key: &str) -> SyntaxElement {
     let txt = format!("{key} = []");
     for root in parse(txt.as_str())
         .into_syntax()
         .clone_for_update()
         .children_with_tokens()
     {
-        if root.kind() == SyntaxKind::ENTRY {
+        if root.kind() == ENTRY {
             return root;
         }
     }
     panic!("Could not create array");
 }
 
 pub fn make_array_entry(key: &str) -> SyntaxElement {
     let txt = format!("a = [\"{key}\"]");
     for root in parse(txt.as_str())
         .into_syntax()
         .clone_for_update()
         .children_with_tokens()
     {
-        if root.kind() == SyntaxKind::ENTRY {
+        if root.kind() == ENTRY {
             for value in root.as_node().unwrap().children_with_tokens() {
-                if value.kind() == SyntaxKind::VALUE {
+                if value.kind() == VALUE {
                     for array in value.as_node().unwrap().children_with_tokens() {
-                        if array.kind() == SyntaxKind::ARRAY {
+                        if array.kind() == ARRAY {
                             for e in array.as_node().unwrap().children_with_tokens() {
-                                if e.kind() == SyntaxKind::VALUE {
+                                if e.kind() == VALUE {
                                     return e;
                                 }
                             }
                         }
                     }
                 }
             }
@@ -120,15 +121,15 @@
 pub fn make_entry_of_string(key: &String, value: &String) -> SyntaxElement {
     let txt = format!("{key} = \"{value}\"\n");
     for root in parse(txt.as_str())
         .into_syntax()
         .clone_for_update()
         .children_with_tokens()
     {
-        if root.kind() == SyntaxKind::ENTRY {
+        if root.kind() == ENTRY {
             return root;
         }
     }
     panic!("Could not create entry of string");
 }
 
 pub fn make_table_entry(key: &str) -> Vec<SyntaxElement> {
```

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/helpers/pep508.rs` & `pyproject_fmt_rust-1.1.2/rust/src/helpers/pep508.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/helpers/string.rs` & `pyproject_fmt_rust-1.1.2/rust/src/helpers/string.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,48 @@
+use taplo::syntax::SyntaxKind::{IDENT, MULTI_LINE_STRING, MULTI_LINE_STRING_LITERAL, STRING, STRING_LITERAL};
 use taplo::syntax::{SyntaxElement, SyntaxKind, SyntaxNode};
 
 use crate::helpers::create::make_string_node;
 
 pub fn load_text(value: &str, kind: SyntaxKind) -> String {
     let mut chars = value.chars();
-    let offset = if [SyntaxKind::STRING, SyntaxKind::STRING_LITERAL].contains(&kind) {
+    let offset = if [STRING, STRING_LITERAL].contains(&kind) {
         1
-    } else if kind == SyntaxKind::IDENT {
+    } else if kind == IDENT {
         0
     } else {
         3
     };
     for _ in 0..offset {
         chars.next();
     }
     for _ in 0..offset {
         chars.next_back();
     }
     let mut res = chars.as_str().to_string();
-    if kind == SyntaxKind::STRING {
+    if kind == STRING {
         res = res.replace("\\\"", "\"");
     }
     res
 }
 
 pub fn update_content<F>(entry: &SyntaxNode, transform: F)
 where
     F: Fn(&str) -> String,
 {
     let (mut to_insert, mut count) = (Vec::<SyntaxElement>::new(), 0);
     let mut changed = false;
     for mut child in entry.children_with_tokens() {
         count += 1;
         let kind = child.kind();
-        if [
-            SyntaxKind::STRING,
-            SyntaxKind::STRING_LITERAL,
-            SyntaxKind::MULTI_LINE_STRING,
-            SyntaxKind::MULTI_LINE_STRING_LITERAL,
-        ]
-        .contains(&kind)
-        {
+        if [STRING, STRING_LITERAL, MULTI_LINE_STRING, MULTI_LINE_STRING_LITERAL].contains(&kind) {
             let found_str_value = load_text(child.as_token().unwrap().text(), kind);
             let output = transform(found_str_value.as_str());
 
-            changed = output != found_str_value || kind != SyntaxKind::STRING;
+            changed = output != found_str_value || kind != STRING;
             if changed {
                 child = make_string_node(output.as_str());
             }
         }
         to_insert.push(child);
     }
     if changed {
```

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/helpers/table.rs` & `pyproject_fmt_rust-1.1.2/rust/src/helpers/table.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::cell::{RefCell, RefMut};
 use std::collections::HashMap;
 use std::iter::zip;
 use std::ops::Index;
 
-use taplo::syntax::SyntaxKind::{TABLE_ARRAY_HEADER, TABLE_HEADER};
-use taplo::syntax::{SyntaxElement, SyntaxKind, SyntaxNode};
+use taplo::syntax::SyntaxKind::{ENTRY, IDENT, KEY, NEWLINE, TABLE_ARRAY_HEADER, TABLE_HEADER, VALUE};
+use taplo::syntax::{SyntaxElement, SyntaxNode};
 use taplo::HashSet;
 
 use crate::helpers::create::{make_empty_newline, make_key, make_newline, make_table_entry};
 use crate::helpers::string::load_text;
 
 #[derive(Debug)]
 pub struct Tables {
@@ -42,19 +42,25 @@
                 if kind == TABLE_ARRAY_HEADER || (kind == TABLE_HEADER && indexes.is_empty()) {
                     indexes.push(table_set.len());
                     table_set.push(RefCell::new(entry_set_borrow.clone()));
                 } else if kind == TABLE_HEADER && !indexes.is_empty() {
                     // join tables
                     let pos = indexes.first().unwrap();
                     let mut res = table_set.index(*pos).borrow_mut();
-                    for element in entry_set_borrow.clone() {
-                        if element.kind() != TABLE_HEADER {
-                            res.push(element);
-                        }
+                    let mut new = entry_set_borrow.clone();
+                    if let Some(last_non_trailing_newline_index) = new.iter().rposition(|x| x.kind() != NEWLINE) {
+                        new.truncate(last_non_trailing_newline_index + 1);
+                    }
+                    if res.last().unwrap().kind() != NEWLINE {
+                        res.push(make_newline());
                     }
+                    res.extend(
+                        new.into_iter()
+                            .skip_while(|x| [NEWLINE, TABLE_HEADER].contains(&x.kind())),
+                    );
                 }
                 entry_set_borrow.clear();
             }
         };
         for c in root_ast.children_with_tokens() {
             if [TABLE_ARRAY_HEADER, TABLE_HEADER].contains(&c.kind()) {
                 add_to_table_set(table_kind);
@@ -80,33 +86,32 @@
         next.push(String::new());
         for (name, next_name) in zip(order.iter(), next.iter()) {
             for entries in self.get(name).unwrap() {
                 let got = entries.borrow_mut();
                 if !got.is_empty() {
                     entry_count += got.len();
                     let last = got.last().unwrap();
-                    if name.is_empty() && last.kind() == SyntaxKind::NEWLINE && got.len() == 1 {
+                    if name.is_empty() && last.kind() == NEWLINE && got.len() == 1 {
                         continue;
                     }
                     let mut add = got.clone();
                     if get_key(name) != get_key(next_name) {
-                        if last.kind() == SyntaxKind::NEWLINE {
+                        if last.kind() == NEWLINE {
                             // replace existing newline to ensure single newline
                             add.pop();
                         }
                         add.push(make_empty_newline());
                     }
                     to_insert.extend(add);
                 }
             }
         }
         root_ast.splice_children(0..entry_count, to_insert);
     }
 }
-
 fn calculate_order(
     header_to_pos: &HashMap<String, Vec<usize>>,
     table_set: &[RefCell<Vec<SyntaxElement>>],
     ordering: &[&str],
 ) -> Vec<String> {
     let max_ordering = ordering.len() * 2;
     let key_to_pos = ordering
@@ -192,52 +197,64 @@
         if !entry_set_borrow.is_empty() {
             key_to_pos.insert(k, key_set.len());
             key_set.push(entry_set_borrow.clone());
             entry_set_borrow.clear();
         }
     };
     let mut key = String::new();
-    for c in table.iter() {
-        if c.kind() == SyntaxKind::ENTRY {
-            add_to_key_set(key.clone());
-            for e in c.as_node().unwrap().children_with_tokens() {
-                if e.kind() == SyntaxKind::KEY {
+    let mut cutoff = false;
+    for element in table.iter() {
+        let kind = element.kind();
+        if kind == ENTRY {
+            if cutoff {
+                add_to_key_set(key.clone());
+                cutoff = false;
+            }
+            for e in element.as_node().unwrap().children_with_tokens() {
+                if e.kind() == KEY {
                     key = e.as_node().unwrap().text().to_string().trim().to_string();
                     break;
                 }
             }
         }
-        entry_set.borrow_mut().push(c.clone());
+        if [ENTRY, TABLE_HEADER, TABLE_ARRAY_HEADER].contains(&kind) {
+            cutoff = true;
+        }
+        entry_set.borrow_mut().push(element.clone());
+        if cutoff && kind == NEWLINE {
+            add_to_key_set(key.clone());
+            cutoff = false;
+        }
     }
     add_to_key_set(key);
     (key_to_pos, key_set)
 }
 
 pub fn get_table_name(entry: &SyntaxElement) -> String {
-    if [SyntaxKind::TABLE_HEADER, SyntaxKind::TABLE_ARRAY_HEADER].contains(&entry.kind()) {
+    if [TABLE_HEADER, TABLE_ARRAY_HEADER].contains(&entry.kind()) {
         for child in entry.as_node().unwrap().children_with_tokens() {
-            if child.kind() == SyntaxKind::KEY {
+            if child.kind() == KEY {
                 return child.as_node().unwrap().text().to_string().trim().to_string();
             }
         }
     }
     String::new()
 }
 
 pub fn for_entries<F>(table: &RefMut<Vec<SyntaxElement>>, f: &mut F)
 where
     F: FnMut(String, &SyntaxNode),
 {
     let mut key = String::new();
     for table_entry in table.iter() {
-        if table_entry.kind() == SyntaxKind::ENTRY {
+        if table_entry.kind() == ENTRY {
             for entry in table_entry.as_node().unwrap().children_with_tokens() {
-                if entry.kind() == SyntaxKind::KEY {
+                if entry.kind() == KEY {
                     key = entry.as_node().unwrap().text().to_string().trim().to_string();
-                } else if entry.kind() == SyntaxKind::VALUE {
+                } else if entry.kind() == VALUE {
                     f(key.clone(), entry.as_node().unwrap());
                 }
             }
         }
     }
 }
 
@@ -265,39 +282,39 @@
             continue;
         }
         let mut sub = tables.table_set[*sub_positions.first().unwrap()].borrow_mut();
         let sub_name = key.strip_prefix(sub_name_prefix.as_str()).unwrap();
         let mut header = false;
         for child in sub.iter() {
             let kind = child.kind();
-            if kind == SyntaxKind::TABLE_HEADER {
+            if kind == TABLE_HEADER {
                 header = true;
                 continue;
             }
-            if header && kind == SyntaxKind::NEWLINE {
+            if header && kind == NEWLINE {
                 continue;
             }
-            if kind == SyntaxKind::ENTRY {
+            if kind == ENTRY {
                 let mut to_insert = Vec::<SyntaxElement>::new();
                 let child_node = child.as_node().unwrap();
                 for mut entry in child_node.children_with_tokens() {
-                    if entry.kind() == SyntaxKind::KEY {
+                    if entry.kind() == KEY {
                         for array_entry_value in entry.as_node().unwrap().children_with_tokens() {
-                            if array_entry_value.kind() == SyntaxKind::IDENT {
-                                let txt = load_text(array_entry_value.as_token().unwrap().text(), SyntaxKind::IDENT);
+                            if array_entry_value.kind() == IDENT {
+                                let txt = load_text(array_entry_value.as_token().unwrap().text(), IDENT);
                                 entry = make_key(format!("{sub_name}.{txt}").as_str());
                                 break;
                             }
                         }
                     }
                     to_insert.push(entry);
                 }
                 child_node.splice_children(0..to_insert.len(), to_insert);
             }
-            if main.last().unwrap().kind() != SyntaxKind::NEWLINE {
+            if main.last().unwrap().kind() != NEWLINE {
                 main.push(make_newline());
             }
             main.push(child.clone());
         }
         sub.clear();
     }
 }
```

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/main.rs` & `pyproject_fmt_rust-1.1.2/rust/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/project.rs` & `pyproject_fmt_rust-1.1.2/rust/src/project.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 use std::cell::RefMut;
 
 use regex::Regex;
-use taplo::syntax::{SyntaxElement, SyntaxKind, SyntaxNode};
+use taplo::syntax::SyntaxKind::{
+    ARRAY, BRACKET_END, BRACKET_START, COMMA, ENTRY, IDENT, INLINE_TABLE, KEY, NEWLINE, STRING, VALUE,
+};
+use taplo::syntax::{SyntaxElement, SyntaxNode};
 use taplo::util::StrExt;
 use taplo::HashSet;
 
 use crate::helpers::array::{sort, transform};
 use crate::helpers::create::{make_array, make_array_entry, make_comma, make_entry_of_string, make_newline};
 use crate::helpers::pep508::{format_requirement, get_canonic_requirement_name};
 use crate::helpers::string::{load_text, update_content};
@@ -98,46 +101,41 @@
     );
 }
 
 fn expand_entry_points_inline_tables(table: &mut RefMut<Vec<SyntaxElement>>) {
     let (mut to_insert, mut count, mut key) = (Vec::<SyntaxElement>::new(), 0, String::new());
     for s_table_entry in table.iter() {
         count += 1;
-        if s_table_entry.kind() == SyntaxKind::ENTRY {
+        if s_table_entry.kind() == ENTRY {
             let mut has_inline_table = false;
             for s_in_table in s_table_entry.as_node().unwrap().children_with_tokens() {
-                if s_in_table.kind() == SyntaxKind::KEY {
+                if s_in_table.kind() == KEY {
                     key = s_in_table.as_node().unwrap().text().to_string().trim().to_string();
-                } else if key.starts_with("entry-points.") && s_in_table.kind() == SyntaxKind::VALUE {
+                } else if key.starts_with("entry-points.") && s_in_table.kind() == VALUE {
                     for s_in_value in s_in_table.as_node().unwrap().children_with_tokens() {
-                        if s_in_value.kind() == SyntaxKind::INLINE_TABLE {
+                        if s_in_value.kind() == INLINE_TABLE {
                             has_inline_table = true;
                             for s_in_inline_table in s_in_value.as_node().unwrap().children_with_tokens() {
-                                if s_in_inline_table.kind() == SyntaxKind::ENTRY {
+                                if s_in_inline_table.kind() == ENTRY {
                                     let mut with_key = String::new();
                                     for s_in_entry in s_in_inline_table.as_node().unwrap().children_with_tokens() {
-                                        if s_in_entry.kind() == SyntaxKind::KEY {
+                                        if s_in_entry.kind() == KEY {
                                             for s_in_key in s_in_entry.as_node().unwrap().children_with_tokens() {
-                                                if s_in_key.kind() == SyntaxKind::IDENT {
-                                                    with_key = load_text(
-                                                        s_in_key.as_token().unwrap().text(),
-                                                        SyntaxKind::IDENT,
-                                                    );
+                                                if s_in_key.kind() == IDENT {
+                                                    with_key = load_text(s_in_key.as_token().unwrap().text(), IDENT);
                                                     with_key = String::from(with_key.strip_quotes());
                                                     break;
                                                 }
                                             }
-                                        } else if s_in_entry.kind() == SyntaxKind::VALUE {
+                                        } else if s_in_entry.kind() == VALUE {
                                             for s_in_b_value in s_in_entry.as_node().unwrap().children_with_tokens() {
-                                                if s_in_b_value.kind() == SyntaxKind::STRING {
-                                                    let value = load_text(
-                                                        s_in_b_value.as_token().unwrap().text(),
-                                                        SyntaxKind::STRING,
-                                                    );
-                                                    if to_insert.last().unwrap().kind() != SyntaxKind::NEWLINE {
+                                                if s_in_b_value.kind() == STRING {
+                                                    let value =
+                                                        load_text(s_in_b_value.as_token().unwrap().text(), STRING);
+                                                    if to_insert.last().unwrap().kind() != NEWLINE {
                                                         to_insert.push(make_newline());
                                                     }
                                                     let new_key = format!("{key}.{with_key}");
                                                     let got = make_entry_of_string(&new_key, &value);
                                                     to_insert.push(got);
                                                     break;
                                                 }
@@ -172,19 +170,19 @@
             let entry = make_array("classifiers");
             generate_classifiers_to_entry(entry.as_node().unwrap(), min, max, &omit, &HashSet::new());
             table.push(entry);
         }
         Some(c) => {
             let mut key_value = String::new();
             for table_row in table.iter() {
-                if table_row.kind() == SyntaxKind::ENTRY {
+                if table_row.kind() == ENTRY {
                     for entry in table_row.as_node().unwrap().children_with_tokens() {
-                        if entry.kind() == SyntaxKind::KEY {
+                        if entry.kind() == KEY {
                             key_value = entry.as_node().unwrap().text().to_string().trim().to_string();
-                        } else if entry.kind() == SyntaxKind::VALUE && key_value == "classifiers" {
+                        } else if entry.kind() == VALUE && key_value == "classifiers" {
                             generate_classifiers_to_entry(table_row.as_node().unwrap(), min, max, &omit, &c);
                         }
                     }
                 }
             }
         }
     };
@@ -194,17 +192,17 @@
     node: &SyntaxNode,
     min: (u8, u8),
     max: (u8, u8),
     omit: &[u8],
     existing: &HashSet<String>,
 ) {
     for array in node.children_with_tokens() {
-        if array.kind() == SyntaxKind::VALUE {
+        if array.kind() == VALUE {
             for root_value in array.as_node().unwrap().children_with_tokens() {
-                if root_value.kind() == SyntaxKind::ARRAY {
+                if root_value.kind() == ARRAY {
                     let mut must_have: HashSet<String> = HashSet::new();
                     must_have.insert(String::from("Programming Language :: Python :: 3 :: Only"));
                     must_have.extend(
                         (min.1..=max.1)
                             .filter(|i| !omit.contains(i))
                             .map(|i| format!("Programming Language :: Python :: 3.{i}")),
                     );
@@ -215,33 +213,32 @@
                         .filter(|e| e.starts_with("Programming Language :: Python :: 3") && !must_have.contains(*e))
                         .collect::<HashSet<&String>>();
                     let mut to_insert = Vec::<SyntaxElement>::new();
                     let mut delete_mode = false;
                     for array_entry in root_value.as_node().unwrap().children_with_tokens() {
                         count += 1;
                         let kind = array_entry.kind();
-                        if delete_mode & [SyntaxKind::NEWLINE, SyntaxKind::BRACKET_END].contains(&kind) {
+                        if delete_mode & [NEWLINE, BRACKET_END].contains(&kind) {
                             delete_mode = false;
-                            if kind == SyntaxKind::NEWLINE {
+                            if kind == NEWLINE {
                                 continue;
                             }
-                        } else if kind == SyntaxKind::VALUE {
+                        } else if kind == VALUE {
                             for array_entry_value in array_entry.as_node().unwrap().children_with_tokens() {
-                                if array_entry_value.kind() == SyntaxKind::STRING {
-                                    let txt =
-                                        load_text(array_entry_value.as_token().unwrap().text(), SyntaxKind::STRING);
+                                if array_entry_value.kind() == STRING {
+                                    let txt = load_text(array_entry_value.as_token().unwrap().text(), STRING);
                                     delete_mode = delete.contains(&txt);
                                     if delete_mode {
                                         // delete from previous comma/start until next newline
                                         let mut remove_count = to_insert.len();
                                         for (at, v) in to_insert.iter().rev().enumerate() {
-                                            if [SyntaxKind::COMMA, SyntaxKind::BRACKET_START].contains(&v.kind()) {
+                                            if [COMMA, BRACKET_START].contains(&v.kind()) {
                                                 remove_count = at;
                                                 for (i, e) in to_insert.iter().enumerate().skip(to_insert.len() - at) {
-                                                    if e.kind() == SyntaxKind::NEWLINE {
+                                                    if e.kind() == NEWLINE {
                                                         remove_count = i + 1;
                                                         break;
                                                     }
                                                 }
                                                 break;
                                             }
                                         }
@@ -257,25 +254,25 @@
                     }
                     let to_add: HashSet<_> = must_have.difference(existing).collect();
                     if !to_add.is_empty() {
                         // make sure we have a comma
                         let mut trail_at = 0;
                         for (at, v) in to_insert.iter().rev().enumerate() {
                             trail_at = to_insert.len() - at;
-                            if v.kind() == SyntaxKind::COMMA {
+                            if v.kind() == COMMA {
                                 for (i, e) in to_insert.iter().enumerate().skip(trail_at) {
-                                    if e.kind() == SyntaxKind::NEWLINE || e.kind() == SyntaxKind::BRACKET_END {
+                                    if e.kind() == NEWLINE || e.kind() == BRACKET_END {
                                         trail_at = i;
                                         break;
                                     }
                                 }
                                 break;
-                            } else if v.kind() == SyntaxKind::BRACKET_START {
+                            } else if v.kind() == BRACKET_START {
                                 break;
-                            } else if v.kind() == SyntaxKind::VALUE {
+                            } else if v.kind() == VALUE {
                                 to_insert.insert(trail_at, make_comma());
                                 trail_at += 1;
                                 break;
                             }
                         }
                         let trail = to_insert.split_off(trail_at);
                         for add in to_add {
@@ -304,16 +301,16 @@
     let mut omit: Vec<u8> = vec![];
     assert_eq!(max_supported_python.0, 3, "for now only Python 3 supported");
     assert_eq!(min_supported_python.0, 3, "for now only Python 3 supported");
 
     for_entries(table, &mut |key, entry| {
         if key == "requires-python" {
             for child in entry.children_with_tokens() {
-                if child.kind() == SyntaxKind::STRING {
-                    let found_str_value = load_text(child.as_token().unwrap().text(), SyntaxKind::STRING);
+                if child.kind() == STRING {
+                    let found_str_value = load_text(child.as_token().unwrap().text(), STRING);
                     let re = Regex::new(r"^(?<op><|<=|==|!=|>=|>)3[.](?<minor>\d+)").unwrap();
                     for part in found_str_value.split(',') {
                         let capture = re.captures(part);
                         if capture.is_some() {
                             let caps = capture.unwrap();
                             let minor = caps["minor"].parse::<u8>().unwrap();
                             match &caps["op"] {
@@ -340,20 +337,20 @@
                             }
                         }
                     }
                 }
             }
         } else if key == "classifiers" {
             for child in entry.children_with_tokens() {
-                if child.kind() == SyntaxKind::ARRAY {
+                if child.kind() == ARRAY {
                     let mut found_elements = HashSet::<String>::new();
                     for array in child.as_node().unwrap().children_with_tokens() {
-                        if array.kind() == SyntaxKind::VALUE {
+                        if array.kind() == VALUE {
                             for value in array.as_node().unwrap().children_with_tokens() {
-                                if value.kind() == SyntaxKind::STRING {
+                                if value.kind() == STRING {
                                     let found = value.as_token().unwrap().text();
                                     let found_str_value: String = String::from(&found[1..found.len() - 1]);
                                     found_elements.insert(found_str_value);
                                 }
                             }
                         }
                     }
@@ -769,15 +766,15 @@
       "covdefaults>=2.3",
       "pytest>=8.1.1",
     ]
     "#},
         true,
         (3, 8),
     )]
-    #[case::project_scritps_collapse(
+    #[case::project_scripts_collapse(
         indoc ! {r#"
     [project.scripts]
     c = 'd'
     a = "b"
     "#},
         indoc ! {r#"
     [project]
```

### Comparing `pyproject_fmt_rust-1.1.1/rust/src/ruff.rs` & `pyproject_fmt_rust-1.1.2/rust/src/ruff.rs`

 * *Files 3% similar despite different names*

```diff
@@ -138,14 +138,15 @@
             "format.skip-magic-trailing-comma",
             "format.docstring-code-line-length",
             "format.docstring-code-format ",
             "format.exclude",
             "format",
             "lint.select",
             "lint.extend-select",
+            "lint.ignore",
             "lint.explicit-preview-rules",
             "lint.exclude",
             "lint.extend-ignore",
             "lint.per-file-ignores",
             "lint.extend-per-file-ignores",
             "lint.fixable",
             "lint.extend-fixable",
@@ -228,8 +229,16 @@
     #[rstest]
     fn test_order_ruff(data: PathBuf) {
         let start = read_to_string(data.join("ruff-order.start.toml")).unwrap();
         let got = evaluate(start.as_str());
         let expected = read_to_string(data.join("ruff-order.expected.toml")).unwrap();
         assert_eq!(got, expected);
     }
+
+    #[rstest]
+    fn test_ruff_comment_21(data: PathBuf) {
+        let start = read_to_string(data.join("ruff-21.start.toml")).unwrap();
+        let got = evaluate(start.as_str());
+        let expected = read_to_string(data.join("ruff-21.expected.toml")).unwrap();
+        assert_eq!(got, expected);
+    }
 }
```

### Comparing `pyproject_fmt_rust-1.1.1/src/pyproject_fmt_rust/_lib.pyi` & `pyproject_fmt_rust-1.1.2/src/pyproject_fmt_rust/_lib.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/tests/test_main.py` & `pyproject_fmt_rust-1.1.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/tox.ini` & `pyproject_fmt_rust-1.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/Cargo.lock` & `pyproject_fmt_rust-1.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyproject-fmt-rust"
-version = "1.1.1"
+version = "1.1.2"
 dependencies = [
  "indoc",
  "lexical-sort",
  "pep440_rs",
  "pep508_rs",
  "pyo3",
  "regex",
```

### Comparing `pyproject_fmt_rust-1.1.1/pyproject.toml` & `pyproject_fmt_rust-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.1.1/PKG-INFO` & `pyproject_fmt_rust-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt-rust
-Version: 1.1.1
+Version: 1.1.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

