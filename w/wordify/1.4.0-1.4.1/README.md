# Comparing `tmp/wordify-1.4.0.tar.gz` & `tmp/wordify-1.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordify-1.4.0.tar", last modified: Sun Aug 27 22:42:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

