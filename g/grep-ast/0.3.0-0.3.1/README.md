# Comparing `tmp/grep_ast-0.3.0.tar.gz` & `tmp/grep_ast-0.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grep_ast-0.3.0.tar", last modified: Fri May 17 21:41:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

