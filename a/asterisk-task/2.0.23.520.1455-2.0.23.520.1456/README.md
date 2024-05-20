# Comparing `tmp/asterisk_task-2.0.23.520.1455.tar.gz` & `tmp/asterisk_task-2.0.23.520.1456-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asterisk_task-2.0.23.520.1455.tar", last modified: Mon May 20 06:55:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

