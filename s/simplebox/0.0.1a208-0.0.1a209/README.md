# Comparing `tmp/simplebox-0.0.1a208-py3-none-any.whl.zip` & `tmp/simplebox-0.0.1a209-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 470161 bytes, number of entries: 166
--rw-rw-rw-  2.0 fat     5191 b- defN 24-May-17 16:08 simplebox/__init__.py
+Zip file size: 470165 bytes, number of entries: 166
+-rw-rw-rw-  2.0 fat     5191 b- defN 24-May-19 13:27 simplebox/__init__.py
 -rw-rw-rw-  2.0 fat     2090 b- defN 24-Apr-07 16:46 simplebox/backend.py
 -rw-rw-rw-  2.0 fat    17626 b- defN 24-Apr-07 16:46 simplebox/character.py
 -rw-rw-rw-  2.0 fat     4829 b- defN 24-Apr-14 15:04 simplebox/classes.py
 -rw-rw-rw-  2.0 fat    16962 b- defN 24-Apr-20 14:21 simplebox/cmd.py
 -rw-rw-rw-  2.0 fat     5481 b- defN 23-Nov-14 15:01 simplebox/converter.py
 -rw-rw-rw-  2.0 fat     1638 b- defN 24-Apr-07 15:02 simplebox/enums.py
 -rw-rw-rw-  2.0 fat      306 b- defN 23-May-31 16:53 simplebox/generic.py
--rw-rw-rw-  2.0 fat    60083 b- defN 24-May-17 16:08 simplebox/http.py
+-rw-rw-rw-  2.0 fat    60095 b- defN 24-May-19 13:27 simplebox/http.py
 -rw-rw-rw-  2.0 fat     5165 b- defN 24-Apr-27 14:18 simplebox/jsonparser.py
 -rw-rw-rw-  2.0 fat    21577 b- defN 24-Apr-27 14:26 simplebox/number.py
 -rw-rw-rw-  2.0 fat     1006 b- defN 24-Apr-07 17:05 simplebox/singleton.py
 -rw-rw-rw-  2.0 fat     1400 b- defN 24-Apr-07 17:02 simplebox/version.py
 -rw-rw-rw-  2.0 fat     4561 b- defN 24-Apr-14 15:04 simplebox/void.py
 -rw-rw-rw-  2.0 fat       86 b- defN 24-Mar-27 14:40 simplebox/_h2/__init__.py
 -rw-rw-rw-  2.0 fat     5764 b- defN 24-Mar-27 14:40 simplebox/_h2/config.py
@@ -157,12 +157,12 @@
 -rw-rw-rw-  2.0 fat     2735 b- defN 24-Apr-27 14:18 simplebox/utils/locks.py
 -rw-rw-rw-  2.0 fat    14864 b- defN 24-Apr-28 15:25 simplebox/utils/objects.py
 -rw-rw-rw-  2.0 fat     3258 b- defN 24-Apr-14 14:42 simplebox/utils/optionals.py
 -rw-rw-rw-  2.0 fat     5653 b- defN 24-Apr-28 17:58 simplebox/utils/reflect.py
 -rw-rw-rw-  2.0 fat    19546 b- defN 24-Apr-07 15:48 simplebox/utils/strings.py
 -rw-rw-rw-  2.0 fat      247 b- defN 23-Feb-28 15:31 simplebox/valid/__init__.py
 -rw-rw-rw-  2.0 fat    17399 b- defN 24-May-06 14:40 simplebox/valid/_validator.py
--rw-rw-rw-  2.0 fat     1360 b- defN 24-May-17 16:09 simplebox-0.0.1a208.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-17 16:09 simplebox-0.0.1a208.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-17 16:09 simplebox-0.0.1a208.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    14453 b- defN 24-May-17 16:09 simplebox-0.0.1a208.dist-info/RECORD
-166 files, 1486409 bytes uncompressed, 447369 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     1360 b- defN 24-May-19 13:29 simplebox-0.0.1a209.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-19 13:29 simplebox-0.0.1a209.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-19 13:29 simplebox-0.0.1a209.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    14453 b- defN 24-May-19 13:29 simplebox-0.0.1a209.dist-info/RECORD
+166 files, 1486421 bytes uncompressed, 447373 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -480,20 +480,20 @@
 
 Filename: simplebox/valid/__init__.py
 Comment: 
 
 Filename: simplebox/valid/_validator.py
 Comment: 
 
-Filename: simplebox-0.0.1a208.dist-info/METADATA
+Filename: simplebox-0.0.1a209.dist-info/METADATA
 Comment: 
 
-Filename: simplebox-0.0.1a208.dist-info/WHEEL
+Filename: simplebox-0.0.1a209.dist-info/WHEEL
 Comment: 
 
-Filename: simplebox-0.0.1a208.dist-info/top_level.txt
+Filename: simplebox-0.0.1a209.dist-info/top_level.txt
 Comment: 
 
-Filename: simplebox-0.0.1a208.dist-info/RECORD
+Filename: simplebox-0.0.1a209.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplebox/__init__.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
-__version__ = "0.0.1.alpha208"
+__version__ = "0.0.1.alpha209"
 
 banner = f"""
  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------. 
 | .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. |
 | |    _______   | || |     _____    | || | ____    ____ | || |   ______     | || |   _____      | || |  _________   | || |   ______     | || |     ____     | || |  ____  ____  | |
 | |   /  ___  |  | || |    |_   _|   | || ||_   \  /   _|| || |  |_   __ \   | || |  |_   _|     | || | |_   ___  |  | || |  |_   _ \    | || |   .'    `.   | || | |_  _||_  _| | |
 | |  |  (__ \_|  | || |      | |     | || |  |   \/   |  | || |    | |__) |  | || |    | |       | || |   | |_  \_|  | || |    | |_) |   | || |  /  .--.  \  | || |   \ \  / /   | |
```

## simplebox/http.py

```diff
@@ -1071,15 +1071,15 @@
             kwargs[_Constant.RESPONSE] = rest_resp
             url_ = url if not resp else resp.url
             arguments = "".join([f'\t{k.ljust(20, " ")} => {v}\n' for k, v in optional_args_tmp.items()])
             try:
                 content = rest_resp.content.decode(encoding_)[:10240]
             except BaseException as e:
                 _LOGGER.log(level=LogLevel.ERROR.value, msg=f"RestResponse content decode error: {str(e)}", stacklevel=2)
-                content = ""
+                content = rest_resp.text
             content = content if content.endswith("\n") else f"{content}\n"
             self.__build_log_message(log_builder,
                                      f"[Server     Description]: {server_description}\n"
                                      f"[Api        Description]: {api_description}\n"
                                      f"[Request    Information]: \n"
                                      f"\t{'url'.ljust(20, ' ')} => {url_}\n"
                                      f"\t{'method'.ljust(20, ' ')} => {method_.upper()}\n"
```

## Comparing `simplebox-0.0.1a208.dist-info/METADATA` & `simplebox-0.0.1a209.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplebox
-Version: 0.0.1a208
+Version: 0.0.1a209
 Summary: 简易工具箱。
 Author: fuck
 License: MIT Licence
 Keywords: pip,simplebox,backend,fast,fasttools,box,simple
 Platform: any
 Requires-Python: >=3.9
 Requires-Dist: psutil (==5.9.2)
```

## Comparing `simplebox-0.0.1a208.dist-info/RECORD` & `simplebox-0.0.1a209.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-simplebox/__init__.py,sha256=3qJXmtUjczd4vs4TnYXfmzjKa4gzcWLW2xfHNDLRx5w,5191
+simplebox/__init__.py,sha256=8iiZ8zrXvhU-LB8mXo_8Nc9s_vOMMn_yOu-kFDvMT24,5191
 simplebox/backend.py,sha256=yR3gveO0iKcTKWKW5K57513u-s7O3oGes84Kp8HUZho,2090
 simplebox/character.py,sha256=NEbQqFmD3rpkl_E3MeES7rRfAmtc_DJHoKcF8GNK92g,17626
 simplebox/classes.py,sha256=vGD0PVglh-Nlz8I3PTqDmDquQf_Z2BNoXIvp9aRS140,4829
 simplebox/cmd.py,sha256=5SK-ne4vAyjNdEztS0TyMWUuQC6bBc4RCtnbdQBvVF4,16962
 simplebox/converter.py,sha256=DZ_sb-ZBIorTZAlpuNyGjxnlPAjtSp7yKMIDSiwws0g,5481
 simplebox/enums.py,sha256=KzziG7TboPMIENPrc4HrsUagSEMd4JfLFG6Bn2T0HAs,1638
 simplebox/generic.py,sha256=tBDzlqFHQ7I6bb8_iC9PEqyMaD0sxJee9a7zR3YwxRw,306
-simplebox/http.py,sha256=1D5ZckBwFsnrGhGeyfa4VFcomZslPERHq89VD5ZVTDc,60083
+simplebox/http.py,sha256=Vob2MJLTMIKejEU9k4ugLgvJI48B3qvSXpA_WpO7B5Q,60095
 simplebox/jsonparser.py,sha256=QD_nY7PCdTOXBjpRZ6iysx386pmS2kMULGRmsMRaVUo,5165
 simplebox/number.py,sha256=hpSLKIoRFnjt-lk4SUCvYNKbcBD8lP_vaOFtD4JQIUQ,21577
 simplebox/singleton.py,sha256=zhyjjhQfg9Y1UYgYFYF31ybNjX0A0oMzBaOG1UZerXo,1006
 simplebox/version.py,sha256=5H3eNzxQOzLT5meyjzOZ1-dg1R9U3h5lCGNzWXwU4Lg,1400
 simplebox/void.py,sha256=wHIojA2oOc5jRYetX4xJxIYFHZNtrYb6hLHSP-HiJfc,4561
 simplebox/_h2/__init__.py,sha256=7aSRL7tUP7vhMpV5uORROh1XlS-pzzxzS0F4mSAFa70,86
 simplebox/_h2/config.py,sha256=9zQSxQ2bpFs07AoPSGa5s6sFzkmRkD8GS5sJAPD10YQ,5764
@@ -156,11 +156,11 @@
 simplebox/utils/locks.py,sha256=KP_utNUBYeWjJhsWzu1-rn5sG6jzi2cDrFXtSmgJCHE,2735
 simplebox/utils/objects.py,sha256=jaTS8DaHdrdspANFzol2ad6UKRQnFCPCvHHnSu5R2d4,14864
 simplebox/utils/optionals.py,sha256=XDlteLGkfbWHOgJPdGykE-a79Ae-P7Fbfsabmiwdjuw,3258
 simplebox/utils/reflect.py,sha256=ih_-fw49DzYSNyauvDbpEW5ixf5wi5UVhE6nlq_zfUk,5653
 simplebox/utils/strings.py,sha256=yvdvMVI-ULs-DIWElpmjdYHp9CPLbETc5M-16L9gflk,19546
 simplebox/valid/__init__.py,sha256=7deSv2vW7Wj-83Db3JbO0SZK9Pf-G9pDqbCAgkxr8PI,247
 simplebox/valid/_validator.py,sha256=MPJRmSsrPLq3ZaKzqPs71iZYP5dRzpI1K2dUF6oqFDI,17399
-simplebox-0.0.1a208.dist-info/METADATA,sha256=K61Q3qIxzfxKuTkuSgRkqfyVUWuCf8sQjRNftaPmPFY,1360
-simplebox-0.0.1a208.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-simplebox-0.0.1a208.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
-simplebox-0.0.1a208.dist-info/RECORD,,
+simplebox-0.0.1a209.dist-info/METADATA,sha256=M6B86h7Rji9rjPHFoGWRWLdRYp0Cd9To4mZlwW5sLYU,1360
+simplebox-0.0.1a209.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+simplebox-0.0.1a209.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
+simplebox-0.0.1a209.dist-info/RECORD,,
```

