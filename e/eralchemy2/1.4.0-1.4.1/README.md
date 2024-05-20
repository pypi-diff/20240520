# Comparing `tmp/eralchemy2-1.4.0.tar.gz` & `tmp/eralchemy2-1.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eralchemy2-1.4.0.tar", last modified: Sat May 11 20:30:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

