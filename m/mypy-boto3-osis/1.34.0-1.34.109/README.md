# Comparing `tmp/mypy-boto3-osis-1.34.0.tar.gz` & `tmp/mypy_boto3_osis-1.34.109-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-osis-1.34.0.tar", last modified: Wed Dec 13 21:23:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

