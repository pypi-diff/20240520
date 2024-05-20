# Comparing `tmp/bp3-0.0.8.tar.gz` & `tmp/bp3-0.0.9-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp3-0.0.8.tar", last modified: Mon Jul 25 13:18:59 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

