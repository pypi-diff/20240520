# Comparing `tmp/imgori-0.2.9-py3-none-any.whl.zip` & `tmp/imgori-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11848 bytes, number of entries: 26
+Zip file size: 11847 bytes, number of entries: 26
 -rwxr-xr-x  2.0 unx      139 b- defN 80-Jan-01 00:00 imgori/__init__.py
 -rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 imgori/cli.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 imgori/commands/__init__.py
 -rw-r--r--  2.0 unx     1344 b- defN 80-Jan-01 00:00 imgori/commands/train.py
 -rwxr-xr-x  2.0 unx       72 b- defN 80-Jan-01 00:00 imgori/datasets/__init__.py
 -rw-r--r--  2.0 unx     2156 b- defN 80-Jan-01 00:00 imgori/datasets/imgori.py
 -rwxr-xr-x  2.0 unx      650 b- defN 80-Jan-01 00:00 imgori/datasets/mnist.py
@@ -17,12 +17,12 @@
 -rw-r--r--  2.0 unx     4073 b- defN 80-Jan-01 00:00 imgori/trainers/imgori.py
 -rw-r--r--  2.0 unx     4087 b- defN 80-Jan-01 00:00 imgori/trainers/mnist.py
 -rw-r--r--  2.0 unx       70 b- defN 80-Jan-01 00:00 imgori/trainers/trainer.py
 -rw-r--r--  2.0 unx     2398 b- defN 80-Jan-01 00:00 imgori/typing.py
 -rwxr-xr-x  2.0 unx      233 b- defN 80-Jan-01 00:00 imgori/utils/__init__.py
 -rw-r--r--  2.0 unx     1212 b- defN 80-Jan-01 00:00 imgori/utils/s3.py
 -rw-r--r--  2.0 unx      744 b- defN 80-Jan-01 00:00 imgori/utils/utils.py
--rw-r--r--  2.0 unx      681 b- defN 80-Jan-01 00:00 imgori-0.2.9.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 imgori-0.2.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 imgori-0.2.9.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2013 b- defN 16-Jan-01 00:00 imgori-0.2.9.dist-info/RECORD
-26 files, 24239 bytes uncompressed, 8630 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx      630 b- defN 80-Jan-01 00:00 imgori-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 imgori-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 imgori-0.3.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2013 b- defN 16-Jan-01 00:00 imgori-0.3.0.dist-info/RECORD
+26 files, 24188 bytes uncompressed, 8629 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -60,20 +60,20 @@
 
 Filename: imgori/utils/s3.py
 Comment: 
 
 Filename: imgori/utils/utils.py
 Comment: 
 
-Filename: imgori-0.2.9.dist-info/METADATA
+Filename: imgori-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: imgori-0.2.9.dist-info/WHEEL
+Filename: imgori-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: imgori-0.2.9.dist-info/entry_points.txt
+Filename: imgori-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: imgori-0.2.9.dist-info/RECORD
+Filename: imgori-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `imgori-0.2.9.dist-info/METADATA` & `imgori-0.3.0.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: imgori
-Version: 0.2.9
+Version: 0.3.0
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.15,<2.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: mlconfig (>=0.2.0,<0.3.0)
 Requires-Dist: mlflow-skinny (>=2.9.2,<3.0.0)
-Requires-Dist: torch (>=2.1.1,<3.0.0)
+Requires-Dist: torch (>=2.3.0,<3.0.0)
 Requires-Dist: torchmetrics (>=1.2.0,<2.0.0)
-Requires-Dist: torchvision (>=0.16.1,<0.17.0)
+Requires-Dist: torchvision (>=0.18.0,<0.19.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
```

## Comparing `imgori-0.2.9.dist-info/RECORD` & `imgori-0.3.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 imgori/trainers/imgori.py,sha256=cCUgTc2HkLOVSvzvLxVQpTHF3ImoG77AmfKHlk5w4zU,4073
 imgori/trainers/mnist.py,sha256=2DAhfGS5BYr9Bf9JVK_8FxwXbycvGansGqtAXfmieYI,4087
 imgori/trainers/trainer.py,sha256=72H5BlWgjYNV1YOwiePjP-PlSANx-kzz3jhCItsZxJs,70
 imgori/typing.py,sha256=2dVGFx8tHvn69yBb587pnvOFTaGGq0-XTGakXq1NUyM,2398
 imgori/utils/__init__.py,sha256=Z6XbCnKBP5UGMxt60JvwNu69XDJkVSHHZSW1SManhCA,233
 imgori/utils/s3.py,sha256=JA6NeafTO4JtGsbuohNKfKSEK7m9Mf9QPxzAUZJAN2c,1212
 imgori/utils/utils.py,sha256=cnfH6VaOeBzZNVfsEIesXG6eTP1RgivFW5qjk_msOxg,744
-imgori-0.2.9.dist-info/METADATA,sha256=hXsE4_GrGnQKYT-oSollnqdjk7_MBLan5eWk6f_ziMY,681
-imgori-0.2.9.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-imgori-0.2.9.dist-info/entry_points.txt,sha256=RBRze5SLMBGEr6NDoc_nszbzHABf-V8Wl_-VYMRwwic,41
-imgori-0.2.9.dist-info/RECORD,,
+imgori-0.3.0.dist-info/METADATA,sha256=0f-rnHtNYchkTP7Fly32ccITqIcmdZEDcP_GqC6PumI,630
+imgori-0.3.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+imgori-0.3.0.dist-info/entry_points.txt,sha256=RBRze5SLMBGEr6NDoc_nszbzHABf-V8Wl_-VYMRwwic,41
+imgori-0.3.0.dist-info/RECORD,,
```

