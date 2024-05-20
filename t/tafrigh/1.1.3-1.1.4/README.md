# Comparing `tmp/tafrigh-1.1.3.tar.gz` & `tmp/tafrigh-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tafrigh-1.1.3.tar", last modified: Mon Dec 11 15:10:24 2023, max compression
+gzip compressed data, was "tafrigh-1.1.4.tar", last modified: Mon May 20 19:12:45 2024, max compression
```

## Comparing `tafrigh-1.1.3.tar` & `tafrigh-1.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:24.330869 tafrigh-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-12-11 15:10:10.000000 tafrigh-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24782 2023-12-11 15:10:24.330869 tafrigh-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21949 2023-12-11 15:10:10.000000 tafrigh-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-12-11 15:10:10.000000 tafrigh-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 15:10:24.330869 tafrigh-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:24.326869 tafrigh-1.1.3/tafrigh/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/audio_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:24.330869 tafrigh-1.1.3/tafrigh/recognizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/recognizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/recognizers/whisper_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/recognizers/wit_calling_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/recognizers/wit_recognizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:24.330869 tafrigh-1.1.3/tafrigh/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/types/transcript_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:24.330869 tafrigh-1.1.3/tafrigh/types/whisper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/types/whisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/types/whisper/type_hints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:24.330869 tafrigh-1.1.3/tafrigh/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/utils/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/utils/time_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:24.330869 tafrigh-1.1.3/tafrigh/utils/whisper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/utils/whisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/utils/whisper/whisper_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:24.330869 tafrigh-1.1.3/tafrigh/utils/wit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/utils/wit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/utils/wit/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2023-12-11 15:10:10.000000 tafrigh-1.1.3/tafrigh/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 15:10:24.330869 tafrigh-1.1.3/tafrigh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24782 2023-12-11 15:10:24.000000 tafrigh-1.1.3/tafrigh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-12-11 15:10:24.000000 tafrigh-1.1.3/tafrigh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 15:10:24.000000 tafrigh-1.1.3/tafrigh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-11 15:10:24.000000 tafrigh-1.1.3/tafrigh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-11 15:10:24.000000 tafrigh-1.1.3/tafrigh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-11 15:10:24.000000 tafrigh-1.1.3/tafrigh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:45.359674 tafrigh-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 19:12:36.000000 tafrigh-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24832 2024-05-20 19:12:45.359674 tafrigh-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21949 2024-05-20 19:12:36.000000 tafrigh-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-20 19:12:36.000000 tafrigh-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:12:45.359674 tafrigh-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:45.351673 tafrigh-1.1.4/tafrigh/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/audio_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:45.355673 tafrigh-1.1.4/tafrigh/recognizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/recognizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/recognizers/whisper_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/recognizers/wit_calling_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/recognizers/wit_recognizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:45.355673 tafrigh-1.1.4/tafrigh/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/types/transcript_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:45.355673 tafrigh-1.1.4/tafrigh/types/whisper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/types/whisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/types/whisper/type_hints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:45.355673 tafrigh-1.1.4/tafrigh/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/utils/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/utils/time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:45.355673 tafrigh-1.1.4/tafrigh/utils/whisper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/utils/whisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/utils/whisper/whisper_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:45.355673 tafrigh-1.1.4/tafrigh/utils/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/utils/wit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/utils/wit/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-20 19:12:36.000000 tafrigh-1.1.4/tafrigh/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:12:45.355673 tafrigh-1.1.4/tafrigh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24832 2024-05-20 19:12:45.000000 tafrigh-1.1.4/tafrigh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 19:12:45.000000 tafrigh-1.1.4/tafrigh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:12:45.000000 tafrigh-1.1.4/tafrigh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 19:12:45.000000 tafrigh-1.1.4/tafrigh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-20 19:12:45.000000 tafrigh-1.1.4/tafrigh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 19:12:45.000000 tafrigh-1.1.4/tafrigh.egg-info/top_level.txt
```

### Comparing `tafrigh-1.1.3/LICENSE` & `tafrigh-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/PKG-INFO` & `tafrigh-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tafrigh
-Version: 1.1.3
+Version: 1.1.4
 Summary: تفريغ النصوص وإنشاء ملفات SRT و VTT باستخدام نماذج Whisper وتقنية wit.ai.
 Author-email: الكتب المٌيسّرة <easybooksdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 الكتب المُيسّرة
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,30 +34,31 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tqdm==4.65.1
-Requires-Dist: yt-dlp==2023.7.6
+Requires-Dist: tqdm>=4.66.4
+Requires-Dist: yt-dlp>=2024.4.9
 Provides-Extra: wit
-Requires-Dist: auditok==0.2.0; extra == "wit"
-Requires-Dist: numpy==1.23.5; extra == "wit"
-Requires-Dist: pydub==0.25.1; extra == "wit"
-Requires-Dist: requests==2.31.0; extra == "wit"
-Requires-Dist: scipy==1.11.1; extra == "wit"
+Requires-Dist: auditok>=0.2.0; extra == "wit"
+Requires-Dist: numpy>=1.26.4; extra == "wit"
+Requires-Dist: pydub>=0.25.1; extra == "wit"
+Requires-Dist: requests>=2.32.0; extra == "wit"
+Requires-Dist: scipy>=1.13.0; extra == "wit"
 Provides-Extra: whisper
-Requires-Dist: faster-whisper==0.10.0; extra == "whisper"
-Requires-Dist: openai-whisper==20231117; extra == "whisper"
-Requires-Dist: stable-ts==2.13.4; extra == "whisper"
+Requires-Dist: faster-whisper>=1.0.2; extra == "whisper"
+Requires-Dist: openai-whisper>=20231117; extra == "whisper"
+Requires-Dist: stable-ts>=2.17.2; extra == "whisper"
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/7662492/229289746-89c5a4c7-afa6-4d46-a0e6-63dfdeb98285.jpg" style="width: 100%;"/>
 </p>
 
 <div align="center">
   <a href="https://pypi.org/project/tafrigh" target="_blank"><img src="https://img.shields.io/pypi/v/tafrigh?label=PyPI%20Version&color=limegreen" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tafrigh Version: 1.1.3 Summary: ØªÙØ±ÙØº
+Metadata-Version: 2.1 Name: tafrigh Version: 1.1.4 Summary: ØªÙØ±ÙØº
 Ø§ÙÙØµÙØµ ÙØ¥ÙØ´Ø§Ø¡ ÙÙÙØ§Øª SRT Ù VTT Ø¨Ø§Ø³ØªØ®Ø¯Ø§Ù ÙÙØ§Ø°Ø¬
 Whisper ÙØªÙÙÙØ© wit.ai. Author-email: Ø§ÙÙØªØ¨ Ø§ÙÙÙÙØ³ÙØ±Ø©
 gmail.com> License: MIT License Copyright (c) 2023 Ø§ÙÙØªØ¨
 Ø§ÙÙÙÙØ³ÙØ±Ø© Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -20,24 +20,24 @@
 github.com/ieasybooks/tafrigh Keywords: tafrigh,speech-to-text,wit.ai,whisper
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.9 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: tqdm==4.65.1
-Requires-Dist: yt-dlp==2023.7.6 Provides-Extra: wit Requires-Dist:
-auditok==0.2.0; extra == "wit" Requires-Dist: numpy==1.23.5; extra == "wit"
-Requires-Dist: pydub==0.25.1; extra == "wit" Requires-Dist: requests==2.31.0;
-extra == "wit" Requires-Dist: scipy==1.11.1; extra == "wit" Provides-Extra:
-whisper Requires-Dist: faster-whisper==0.10.0; extra == "whisper" Requires-
-Dist: openai-whisper==20231117; extra == "whisper" Requires-Dist: stable-
-ts==2.13.4; extra == "whisper"
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.9 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: tqdm>=4.66.4 Requires-Dist: yt-
+dlp>=2024.4.9 Provides-Extra: wit Requires-Dist: auditok>=0.2.0; extra == "wit"
+Requires-Dist: numpy>=1.26.4; extra == "wit" Requires-Dist: pydub>=0.25.1;
+extra == "wit" Requires-Dist: requests>=2.32.0; extra == "wit" Requires-Dist:
+scipy>=1.13.0; extra == "wit" Provides-Extra: whisper Requires-Dist: faster-
+whisper>=1.0.2; extra == "whisper" Requires-Dist: openai-whisper>=20231117;
+extra == "whisper" Requires-Dist: stable-ts>=2.17.2; extra == "whisper"
   [https://user-images.githubusercontent.com/7662492/229289746-89c5a4c7-afa6-
                           4d46-a0e6-63dfdeb98285.jpg]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_a_f_r_i_g_h_?_l_a_b_e_l_=_P_y_P_I_%_2_0_V_e_r_s_i_o_n_&_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_a_f_r_i_g_h_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_t_a_f_r_i_g_h_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
 _t_a_f_r_i_g_h_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_i_e_a_s_y_b_o_o_k_s_/_t_a_f_r_i_g_h_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_f_o_r_m_a_t_t_e_r_._y_m_l_/
              _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
```

### Comparing `tafrigh-1.1.3/README.md` & `tafrigh-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/pyproject.toml` & `tafrigh-1.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tafrigh"
-version = "1.1.3"
+version = "1.1.4"
 description = "تفريغ النصوص وإنشاء ملفات SRT و VTT باستخدام نماذج Whisper وتقنية wit.ai."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -16,32 +16,33 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 authors = [{ name = "الكتب المٌيسّرة", email = "easybooksdev@gmail.com" }]
 keywords = ["tafrigh", "speech-to-text", "wit.ai", "whisper"]
-dependencies = ["tqdm==4.65.1", "yt-dlp==2023.7.6"]
+dependencies = ["tqdm>=4.66.4", "yt-dlp>=2024.4.9"]
 
 [project.optional-dependencies]
 wit = [
-    "auditok==0.2.0",
-    "numpy==1.23.5",
-    "pydub==0.25.1",
-    "requests==2.31.0",
-    "scipy==1.11.1",
+    "auditok>=0.2.0",
+    "numpy>=1.26.4",
+    "pydub>=0.25.1",
+    "requests>=2.32.0",
+    "scipy>=1.13.0",
 ]
 whisper = [
-    "faster-whisper==0.10.0",
-    "openai-whisper==20231117",
-    "stable-ts==2.13.4",
+    "faster-whisper>=1.0.2",
+    "openai-whisper>=20231117",
+    "stable-ts>=2.17.2",
 ]
 
 [project.urls]
 homepage = "https://github.com/ieasybooks/tafrigh"
 repository = "https://github.com/ieasybooks/tafrigh"
 
 [project.scripts]
```

### Comparing `tafrigh-1.1.3/tafrigh/audio_splitter.py` & `tafrigh-1.1.4/tafrigh/audio_splitter.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh/cli.py` & `tafrigh-1.1.4/tafrigh/cli.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh/config.py` & `tafrigh-1.1.4/tafrigh/config.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh/downloader.py` & `tafrigh-1.1.4/tafrigh/downloader.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh/recognizers/whisper_recognizer.py` & `tafrigh-1.1.4/tafrigh/recognizers/whisper_recognizer.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh/recognizers/wit_calling_throttle.py` & `tafrigh-1.1.4/tafrigh/recognizers/wit_calling_throttle.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh/recognizers/wit_recognizer.py` & `tafrigh-1.1.4/tafrigh/recognizers/wit_recognizer.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh/utils/cli_utils.py` & `tafrigh-1.1.4/tafrigh/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh/utils/time_utils.py` & `tafrigh-1.1.4/tafrigh/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh/writer.py` & `tafrigh-1.1.4/tafrigh/writer.py`

 * *Files identical despite different names*

### Comparing `tafrigh-1.1.3/tafrigh.egg-info/PKG-INFO` & `tafrigh-1.1.4/tafrigh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tafrigh
-Version: 1.1.3
+Version: 1.1.4
 Summary: تفريغ النصوص وإنشاء ملفات SRT و VTT باستخدام نماذج Whisper وتقنية wit.ai.
 Author-email: الكتب المٌيسّرة <easybooksdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 الكتب المُيسّرة
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,30 +34,31 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tqdm==4.65.1
-Requires-Dist: yt-dlp==2023.7.6
+Requires-Dist: tqdm>=4.66.4
+Requires-Dist: yt-dlp>=2024.4.9
 Provides-Extra: wit
-Requires-Dist: auditok==0.2.0; extra == "wit"
-Requires-Dist: numpy==1.23.5; extra == "wit"
-Requires-Dist: pydub==0.25.1; extra == "wit"
-Requires-Dist: requests==2.31.0; extra == "wit"
-Requires-Dist: scipy==1.11.1; extra == "wit"
+Requires-Dist: auditok>=0.2.0; extra == "wit"
+Requires-Dist: numpy>=1.26.4; extra == "wit"
+Requires-Dist: pydub>=0.25.1; extra == "wit"
+Requires-Dist: requests>=2.32.0; extra == "wit"
+Requires-Dist: scipy>=1.13.0; extra == "wit"
 Provides-Extra: whisper
-Requires-Dist: faster-whisper==0.10.0; extra == "whisper"
-Requires-Dist: openai-whisper==20231117; extra == "whisper"
-Requires-Dist: stable-ts==2.13.4; extra == "whisper"
+Requires-Dist: faster-whisper>=1.0.2; extra == "whisper"
+Requires-Dist: openai-whisper>=20231117; extra == "whisper"
+Requires-Dist: stable-ts>=2.17.2; extra == "whisper"
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/7662492/229289746-89c5a4c7-afa6-4d46-a0e6-63dfdeb98285.jpg" style="width: 100%;"/>
 </p>
 
 <div align="center">
   <a href="https://pypi.org/project/tafrigh" target="_blank"><img src="https://img.shields.io/pypi/v/tafrigh?label=PyPI%20Version&color=limegreen" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tafrigh Version: 1.1.3 Summary: ØªÙØ±ÙØº
+Metadata-Version: 2.1 Name: tafrigh Version: 1.1.4 Summary: ØªÙØ±ÙØº
 Ø§ÙÙØµÙØµ ÙØ¥ÙØ´Ø§Ø¡ ÙÙÙØ§Øª SRT Ù VTT Ø¨Ø§Ø³ØªØ®Ø¯Ø§Ù ÙÙØ§Ø°Ø¬
 Whisper ÙØªÙÙÙØ© wit.ai. Author-email: Ø§ÙÙØªØ¨ Ø§ÙÙÙÙØ³ÙØ±Ø©
 gmail.com> License: MIT License Copyright (c) 2023 Ø§ÙÙØªØ¨
 Ø§ÙÙÙÙØ³ÙØ±Ø© Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -20,24 +20,24 @@
 github.com/ieasybooks/tafrigh Keywords: tafrigh,speech-to-text,wit.ai,whisper
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.9 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: tqdm==4.65.1
-Requires-Dist: yt-dlp==2023.7.6 Provides-Extra: wit Requires-Dist:
-auditok==0.2.0; extra == "wit" Requires-Dist: numpy==1.23.5; extra == "wit"
-Requires-Dist: pydub==0.25.1; extra == "wit" Requires-Dist: requests==2.31.0;
-extra == "wit" Requires-Dist: scipy==1.11.1; extra == "wit" Provides-Extra:
-whisper Requires-Dist: faster-whisper==0.10.0; extra == "whisper" Requires-
-Dist: openai-whisper==20231117; extra == "whisper" Requires-Dist: stable-
-ts==2.13.4; extra == "whisper"
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.9 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: tqdm>=4.66.4 Requires-Dist: yt-
+dlp>=2024.4.9 Provides-Extra: wit Requires-Dist: auditok>=0.2.0; extra == "wit"
+Requires-Dist: numpy>=1.26.4; extra == "wit" Requires-Dist: pydub>=0.25.1;
+extra == "wit" Requires-Dist: requests>=2.32.0; extra == "wit" Requires-Dist:
+scipy>=1.13.0; extra == "wit" Provides-Extra: whisper Requires-Dist: faster-
+whisper>=1.0.2; extra == "whisper" Requires-Dist: openai-whisper>=20231117;
+extra == "whisper" Requires-Dist: stable-ts>=2.17.2; extra == "whisper"
   [https://user-images.githubusercontent.com/7662492/229289746-89c5a4c7-afa6-
                           4d46-a0e6-63dfdeb98285.jpg]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_a_f_r_i_g_h_?_l_a_b_e_l_=_P_y_P_I_%_2_0_V_e_r_s_i_o_n_&_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_a_f_r_i_g_h_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_t_a_f_r_i_g_h_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
 _t_a_f_r_i_g_h_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_i_e_a_s_y_b_o_o_k_s_/_t_a_f_r_i_g_h_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_f_o_r_m_a_t_t_e_r_._y_m_l_/
              _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
```

### Comparing `tafrigh-1.1.3/tafrigh.egg-info/SOURCES.txt` & `tafrigh-1.1.4/tafrigh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

