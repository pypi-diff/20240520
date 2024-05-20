# Comparing `tmp/sabctools-8.2.2.tar.gz` & `tmp/sabctools-8.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabctools-8.2.2.tar", last modified: Sun May 19 11:09:48 2024, max compression
+gzip compressed data, was "sabctools-8.2.3.tar", last modified: Mon May 20 19:28:56 2024, max compression
```

## Comparing `sabctools-8.2.2.tar` & `sabctools-8.2.3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.899271 sabctools-8.2.2/
--rw-r--r--   0 runner     (501) staff       (20)    17990 2024-05-19 11:06:14.000000 sabctools-8.2.2/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)       24 2024-05-19 11:06:14.000000 sabctools-8.2.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3122 2024-05-19 11:09:48.899075 sabctools-8.2.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2348 2024-05-19 11:06:14.000000 sabctools-8.2.2/README.md
--rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-19 11:06:14.000000 sabctools-8.2.2/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.870139 sabctools-8.2.2/sabctools.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3122 2024-05-19 11:09:48.000000 sabctools-8.2.2/sabctools.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3095 2024-05-19 11:09:48.000000 sabctools-8.2.2/sabctools.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-19 11:09:48.000000 sabctools-8.2.2/sabctools.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2024-05-19 11:09:48.000000 sabctools-8.2.2/sabctools.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-19 11:09:48.899316 sabctools-8.2.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)    17185 2024-05-19 11:06:14.000000 sabctools-8.2.2/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.872348 sabctools-8.2.2/src/
--rw-r--r--   0 runner     (501) staff       (20)      108 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2284 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crc32.cc
--rw-r--r--   0 runner     (501) staff       (20)     1127 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crc32.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.882966 sabctools-8.2.2/src/crcutil-1.0/
--rw-r--r--   0 runner     (501) staff       (20)       54 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/AUTHORS
--rw-r--r--   0 runner     (501) staff       (20)    11358 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/COPYING
--rw-r--r--   0 runner     (501) staff       (20)       58 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/ChangeLog
--rw-r--r--   0 runner     (501) staff       (20)     1700 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/INSTALL
--rw-r--r--   0 runner     (501) staff       (20)    11358 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    50573 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/Makefile
--rw-r--r--   0 runner     (501) staff       (20)     1210 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/Makefile.am
--rw-r--r--   0 runner     (501) staff       (20)    56163 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/Makefile.in
--rw-r--r--   0 runner     (501) staff       (20)     2076 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/Makefile.win
--rw-r--r--   0 runner     (501) staff       (20)       60 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/NEWS
--rw-r--r--   0 runner     (501) staff       (20)     6669 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/README
--rw-r--r--   0 runner     (501) staff       (20)    34611 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/aclocal.m4
--rw-r--r--   0 runner     (501) staff       (20)     2785 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/autogen.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.886583 sabctools-8.2.2/src/crcutil-1.0/code/
--rw-r--r--   0 runner     (501) staff       (20)     2368 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/base_types.h
--rw-r--r--   0 runner     (501) staff       (20)    12545 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4.cc
--rw-r--r--   0 runner     (501) staff       (20)     7511 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4.h
--rw-r--r--   0 runner     (501) staff       (20)     3336 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4_intrin.h
--rw-r--r--   0 runner     (501) staff       (20)     2223 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/crc_casts.h
--rw-r--r--   0 runner     (501) staff       (20)    21506 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/generic_crc.h
--rw-r--r--   0 runner     (501) staff       (20)     8663 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/gf_util.h
--rw-r--r--   0 runner     (501) staff       (20)     8211 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc
--rw-r--r--   0 runner     (501) staff       (20)     7459 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc
--rw-r--r--   0 runner     (501) staff       (20)     8601 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc
--rw-r--r--   0 runner     (501) staff       (20)     7945 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc
--rw-r--r--   0 runner     (501) staff       (20)     7379 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc
--rw-r--r--   0 runner     (501) staff       (20)     7264 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/platform.h
--rw-r--r--   0 runner     (501) staff       (20)     2266 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/protected_crc.h
--rw-r--r--   0 runner     (501) staff       (20)     3417 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/rolling_crc.h
--rw-r--r--   0 runner     (501) staff       (20)     1629 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/std_headers.h
--rw-r--r--   0 runner     (501) staff       (20)     8422 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/code/uint128_sse2.h
--rw-r--r--   0 runner     (501) staff       (20)     2231 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/config.h.in
--rw-r--r--   0 runner     (501) staff       (20)   212367 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/configure
--rw-r--r--   0 runner     (501) staff       (20)      744 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/configure.ac
--rw-r--r--   0 runner     (501) staff       (20)    18615 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/depcomp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.887005 sabctools-8.2.2/src/crcutil-1.0/examples/
--rw-r--r--   0 runner     (501) staff       (20)    10449 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/examples/interface.cc
--rw-r--r--   0 runner     (501) staff       (20)     8820 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/examples/interface.h
--rw-r--r--   0 runner     (501) staff       (20)     6390 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/examples/usage.cc
--rw-r--r--   0 runner     (501) staff       (20)    13663 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/install-sh
--rw-r--r--   0 runner     (501) staff       (20)    11419 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/missing
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.889545 sabctools-8.2.2/src/crcutil-1.0/tests/
--rw-r--r--   0 runner     (501) staff       (20)     2227 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/aligned_alloc.h
--rw-r--r--   0 runner     (501) staff       (20)     2538 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/bob_jenkins_rng.h
--rw-r--r--   0 runner     (501) staff       (20)     1915 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/rdtsc.h
--rw-r--r--   0 runner     (501) staff       (20)     1803 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/set_hi_pri.c
--rw-r--r--   0 runner     (501) staff       (20)     7593 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/unittest.cc
--rw-r--r--   0 runner     (501) staff       (20)    33870 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/unittest.h
--rw-r--r--   0 runner     (501) staff       (20)     1290 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/crcutil-1.0/tests/unittest_helper.h
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/py.typed
--rw-r--r--   0 runner     (501) staff       (20)     3961 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sabctools.cc
--rw-r--r--   0 runner     (501) staff       (20)      963 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sabctools.h
--rw-r--r--   0 runner     (501) staff       (20)      703 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sabctools.pyi
--rw-r--r--   0 runner     (501) staff       (20)     3243 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sparse.cc
--rw-r--r--   0 runner     (501) staff       (20)     1023 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/sparse.h
--rw-r--r--   0 runner     (501) staff       (20)     8637 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/unlocked_ssl.cc
--rw-r--r--   0 runner     (501) staff       (20)     1484 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/unlocked_ssl.h
--rw-r--r--   0 runner     (501) staff       (20)     1089 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/utils.cc
--rw-r--r--   0 runner     (501) staff       (20)      937 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/utils.h
--rw-r--r--   0 runner     (501) staff       (20)    10285 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yenc.cc
--rw-r--r--   0 runner     (501) staff       (20)     1388 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yenc.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.896058 sabctools-8.2.2/src/yencode/
--rw-r--r--   0 runner     (501) staff       (20)    10960 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/common.h
--rw-r--r--   0 runner     (501) staff       (20)     9326 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc.cc
--rw-r--r--   0 runner     (501) staff       (20)     2476 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc.h
--rw-r--r--   0 runner     (501) staff       (20)     6911 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_arm.cc
--rw-r--r--   0 runner     (501) staff       (20)     6864 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_arm_pmull.cc
--rw-r--r--   0 runner     (501) staff       (20)      589 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_common.h
--rw-r--r--   0 runner     (501) staff       (20)    17801 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_folding.cc
--rw-r--r--   0 runner     (501) staff       (20)     7011 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_folding_256.cc
--rw-r--r--   0 runner     (501) staff       (20)     7289 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/crc_riscv.cc
--rw-r--r--   0 runner     (501) staff       (20)    10917 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder.cc
--rw-r--r--   0 runner     (501) staff       (20)     1878 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder.h
--rw-r--r--   0 runner     (501) staff       (20)      704 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_avx.cc
--rw-r--r--   0 runner     (501) staff       (20)      760 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_avx2.cc
--rw-r--r--   0 runner     (501) staff       (20)    23461 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_avx2_base.h
--rw-r--r--   0 runner     (501) staff       (20)     7641 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_common.h
--rw-r--r--   0 runner     (501) staff       (20)    17142 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_neon.cc
--rw-r--r--   0 runner     (501) staff       (20)    17359 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_neon64.cc
--rw-r--r--   0 runner     (501) staff       (20)    10838 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_rvv.cc
--rw-r--r--   0 runner     (501) staff       (20)     1382 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_sse2.cc
--rw-r--r--   0 runner     (501) staff       (20)    25288 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_sse_base.h
--rw-r--r--   0 runner     (501) staff       (20)      664 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_ssse3.cc
--rw-r--r--   0 runner     (501) staff       (20)     1426 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/decoder_vbmi2.cc
--rw-r--r--   0 runner     (501) staff       (20)     5395 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder.cc
--rw-r--r--   0 runner     (501) staff       (20)      608 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder.h
--rw-r--r--   0 runner     (501) staff       (20)      383 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_avx.cc
--rw-r--r--   0 runner     (501) staff       (20)      383 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_avx2.cc
--rw-r--r--   0 runner     (501) staff       (20)    21399 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_avx_base.h
--rw-r--r--   0 runner     (501) staff       (20)     2907 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_common.h
--rw-r--r--   0 runner     (501) staff       (20)    19077 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_neon.cc
--rw-r--r--   0 runner     (501) staff       (20)     6214 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_rvv.cc
--rw-r--r--   0 runner     (501) staff       (20)      320 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_sse2.cc
--rw-r--r--   0 runner     (501) staff       (20)    24611 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_sse_base.h
--rw-r--r--   0 runner     (501) staff       (20)      719 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_ssse3.cc
--rw-r--r--   0 runner     (501) staff       (20)      930 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/encoder_vbmi2.cc
--rw-r--r--   0 runner     (501) staff       (20)    77413 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/hedley.h
--rw-r--r--   0 runner     (501) staff       (20)     6465 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/platform.cc
--rw-r--r--   0 runner     (501) staff       (20)     7722 2024-05-19 11:06:14.000000 sabctools-8.2.2/src/yencode/stdint.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-19 11:09:48.898753 sabctools-8.2.2/tests/
--rw-r--r--   0 runner     (501) staff       (20)      550 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test.py
--rw-r--r--   0 runner     (501) staff       (20)     2033 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_crc32.py
--rw-r--r--   0 runner     (501) staff       (20)     4092 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_decoder.py
--rw-r--r--   0 runner     (501) staff       (20)      204 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_encoder.py
--rw-r--r--   0 runner     (501) staff       (20)     1123 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_sparse.py
--rw-r--r--   0 runner     (501) staff       (20)    12761 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_unlocked_ssl.py
--rw-r--r--   0 runner     (501) staff       (20)      402 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/test_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     5879 2024-05-19 11:06:14.000000 sabctools-8.2.2/tests/testsupport.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-20 19:28:56.613401 sabctools-8.2.3/
+-rw-r--r--   0 runner     (501) staff       (20)    17990 2024-05-20 19:24:55.000000 sabctools-8.2.3/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)       24 2024-05-20 19:24:55.000000 sabctools-8.2.3/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3122 2024-05-20 19:28:56.613231 sabctools-8.2.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2348 2024-05-20 19:24:55.000000 sabctools-8.2.3/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-20 19:24:55.000000 sabctools-8.2.3/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-20 19:28:56.592933 sabctools-8.2.3/sabctools.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3122 2024-05-20 19:28:56.000000 sabctools-8.2.3/sabctools.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3095 2024-05-20 19:28:56.000000 sabctools-8.2.3/sabctools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-20 19:28:56.000000 sabctools-8.2.3/sabctools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-05-20 19:28:56.000000 sabctools-8.2.3/sabctools.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-20 19:28:56.613573 sabctools-8.2.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)    17278 2024-05-20 19:24:55.000000 sabctools-8.2.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-20 19:28:56.596657 sabctools-8.2.3/src/
+-rw-r--r--   0 runner     (501) staff       (20)      108 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2284 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crc32.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1127 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crc32.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-20 19:28:56.600144 sabctools-8.2.3/src/crcutil-1.0/
+-rw-r--r--   0 runner     (501) staff       (20)       54 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/AUTHORS
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/COPYING
+-rw-r--r--   0 runner     (501) staff       (20)       58 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/ChangeLog
+-rw-r--r--   0 runner     (501) staff       (20)     1700 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/INSTALL
+-rw-r--r--   0 runner     (501) staff       (20)    11358 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)    50573 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)     1210 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/Makefile.am
+-rw-r--r--   0 runner     (501) staff       (20)    56163 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/Makefile.in
+-rw-r--r--   0 runner     (501) staff       (20)     2076 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/Makefile.win
+-rw-r--r--   0 runner     (501) staff       (20)       60 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/NEWS
+-rw-r--r--   0 runner     (501) staff       (20)     6669 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/README
+-rw-r--r--   0 runner     (501) staff       (20)    34611 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/aclocal.m4
+-rw-r--r--   0 runner     (501) staff       (20)     2785 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/autogen.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-20 19:28:56.603281 sabctools-8.2.3/src/crcutil-1.0/code/
+-rw-r--r--   0 runner     (501) staff       (20)     2368 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/base_types.h
+-rw-r--r--   0 runner     (501) staff       (20)    12545 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/crc32c_sse4.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7511 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/crc32c_sse4.h
+-rw-r--r--   0 runner     (501) staff       (20)     3336 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/crc32c_sse4_intrin.h
+-rw-r--r--   0 runner     (501) staff       (20)     2223 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/crc_casts.h
+-rw-r--r--   0 runner     (501) staff       (20)    21506 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/generic_crc.h
+-rw-r--r--   0 runner     (501) staff       (20)     8663 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/gf_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     8211 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7459 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8601 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7945 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7379 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7264 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/platform.h
+-rw-r--r--   0 runner     (501) staff       (20)     2266 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/protected_crc.h
+-rw-r--r--   0 runner     (501) staff       (20)     3417 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/rolling_crc.h
+-rw-r--r--   0 runner     (501) staff       (20)     1629 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/std_headers.h
+-rw-r--r--   0 runner     (501) staff       (20)     8422 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/code/uint128_sse2.h
+-rw-r--r--   0 runner     (501) staff       (20)     2231 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/config.h.in
+-rw-r--r--   0 runner     (501) staff       (20)   212367 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/configure
+-rw-r--r--   0 runner     (501) staff       (20)      744 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/configure.ac
+-rw-r--r--   0 runner     (501) staff       (20)    18615 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/depcomp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-20 19:28:56.603949 sabctools-8.2.3/src/crcutil-1.0/examples/
+-rw-r--r--   0 runner     (501) staff       (20)    10449 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/examples/interface.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8820 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/examples/interface.h
+-rw-r--r--   0 runner     (501) staff       (20)     6390 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/examples/usage.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13663 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/install-sh
+-rw-r--r--   0 runner     (501) staff       (20)    11419 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/missing
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-20 19:28:56.605573 sabctools-8.2.3/src/crcutil-1.0/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     2227 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/tests/aligned_alloc.h
+-rw-r--r--   0 runner     (501) staff       (20)     2538 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/tests/bob_jenkins_rng.h
+-rw-r--r--   0 runner     (501) staff       (20)     1915 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/tests/rdtsc.h
+-rw-r--r--   0 runner     (501) staff       (20)     1803 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/tests/set_hi_pri.c
+-rw-r--r--   0 runner     (501) staff       (20)     7593 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/tests/unittest.cc
+-rw-r--r--   0 runner     (501) staff       (20)    33870 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/tests/unittest.h
+-rw-r--r--   0 runner     (501) staff       (20)     1290 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/crcutil-1.0/tests/unittest_helper.h
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/py.typed
+-rw-r--r--   0 runner     (501) staff       (20)     3961 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/sabctools.cc
+-rw-r--r--   0 runner     (501) staff       (20)      963 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/sabctools.h
+-rw-r--r--   0 runner     (501) staff       (20)      703 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/sabctools.pyi
+-rw-r--r--   0 runner     (501) staff       (20)     3243 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/sparse.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1023 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/sparse.h
+-rw-r--r--   0 runner     (501) staff       (20)     8637 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/unlocked_ssl.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1484 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/unlocked_ssl.h
+-rw-r--r--   0 runner     (501) staff       (20)     1089 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/utils.cc
+-rw-r--r--   0 runner     (501) staff       (20)      937 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/utils.h
+-rw-r--r--   0 runner     (501) staff       (20)    10285 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yenc.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1388 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yenc.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-20 19:28:56.611995 sabctools-8.2.3/src/yencode/
+-rw-r--r--   0 runner     (501) staff       (20)    10960 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     9326 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/crc.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2476 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/crc.h
+-rw-r--r--   0 runner     (501) staff       (20)     6911 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/crc_arm.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6864 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/crc_arm_pmull.cc
+-rw-r--r--   0 runner     (501) staff       (20)      589 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/crc_common.h
+-rw-r--r--   0 runner     (501) staff       (20)    17801 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/crc_folding.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7011 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/crc_folding_256.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7289 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/crc_riscv.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10917 2024-05-20 19:24:55.000000 sabctools-8.2.3/src/yencode/decoder.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1878 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder.h
+-rw-r--r--   0 runner     (501) staff       (20)      704 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_avx.cc
+-rw-r--r--   0 runner     (501) staff       (20)      760 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_avx2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    23461 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_avx2_base.h
+-rw-r--r--   0 runner     (501) staff       (20)     7641 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_common.h
+-rw-r--r--   0 runner     (501) staff       (20)    17142 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_neon.cc
+-rw-r--r--   0 runner     (501) staff       (20)    17359 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_neon64.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10838 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_rvv.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1382 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_sse2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    25288 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_sse_base.h
+-rw-r--r--   0 runner     (501) staff       (20)      664 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_ssse3.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1426 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/decoder_vbmi2.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5395 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder.cc
+-rw-r--r--   0 runner     (501) staff       (20)      608 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder.h
+-rw-r--r--   0 runner     (501) staff       (20)      383 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_avx.cc
+-rw-r--r--   0 runner     (501) staff       (20)      383 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_avx2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    21399 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_avx_base.h
+-rw-r--r--   0 runner     (501) staff       (20)     2907 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_common.h
+-rw-r--r--   0 runner     (501) staff       (20)    19077 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_neon.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6214 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_rvv.cc
+-rw-r--r--   0 runner     (501) staff       (20)      320 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_sse2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    24611 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_sse_base.h
+-rw-r--r--   0 runner     (501) staff       (20)      719 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_ssse3.cc
+-rw-r--r--   0 runner     (501) staff       (20)      930 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/encoder_vbmi2.cc
+-rw-r--r--   0 runner     (501) staff       (20)    77413 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/hedley.h
+-rw-r--r--   0 runner     (501) staff       (20)     6465 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/platform.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7722 2024-05-20 19:24:56.000000 sabctools-8.2.3/src/yencode/stdint.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-20 19:28:56.613013 sabctools-8.2.3/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      550 2024-05-20 19:24:56.000000 sabctools-8.2.3/tests/test.py
+-rw-r--r--   0 runner     (501) staff       (20)     2033 2024-05-20 19:24:56.000000 sabctools-8.2.3/tests/test_crc32.py
+-rw-r--r--   0 runner     (501) staff       (20)     4092 2024-05-20 19:24:56.000000 sabctools-8.2.3/tests/test_decoder.py
+-rw-r--r--   0 runner     (501) staff       (20)      204 2024-05-20 19:24:56.000000 sabctools-8.2.3/tests/test_encoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     1123 2024-05-20 19:24:56.000000 sabctools-8.2.3/tests/test_sparse.py
+-rw-r--r--   0 runner     (501) staff       (20)    12761 2024-05-20 19:24:56.000000 sabctools-8.2.3/tests/test_unlocked_ssl.py
+-rw-r--r--   0 runner     (501) staff       (20)      402 2024-05-20 19:24:56.000000 sabctools-8.2.3/tests/test_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     5879 2024-05-20 19:24:56.000000 sabctools-8.2.3/tests/testsupport.py
```

### Comparing `sabctools-8.2.2/LICENSE.md` & `sabctools-8.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/PKG-INFO` & `sabctools-8.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabctools
-Version: 8.2.2
+Version: 8.2.3
 Summary: C implementations of functions for use within SABnzbd
 Home-page: https://github.com/sabnzbd/sabctools/
 Author: Safihre
 Author-email: safihre@sabnzbd.org
 License: GPLv2+
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sabctools-8.2.2/README.md` & `sabctools-8.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/sabctools.egg-info/PKG-INFO` & `sabctools-8.2.3/sabctools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabctools
-Version: 8.2.2
+Version: 8.2.3
 Summary: C implementations of functions for use within SABnzbd
 Home-page: https://github.com/sabnzbd/sabctools/
 Author: Safihre
 Author-email: safihre@sabnzbd.org
 License: GPLv2+
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sabctools-8.2.2/sabctools.egg-info/SOURCES.txt` & `sabctools-8.2.3/sabctools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/setup.py` & `sabctools-8.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,22 +118,23 @@
             elif autoconf_check(self.compiler, flag_check="-std=c++0x"):
                 cflags.append("-std=c++0x")
                 ext.extra_compile_args.append("-std=c++0x")
             else:
                 log.info("==> C++11 flag not available")
 
             # Verify specific flags for ARM chips
-            # macOS M1 do not need any flags, they support everything
+            # macOS ARM does not need any flags, they support everything
             if IS_ARM and not IS_MACOS:
                 if not autoconf_check(self.compiler, define_check="__aarch64__"):
                     log.info("==> __aarch64__ not available, disabling 64bit extensions")
                     IS_AARCH64 = False
+                if autoconf_check(self.compiler, flag_check="-march=armv8-a+crc+crypto"):
+                    gcc_arm_crc_pmull_flags.append("-march=armv8-a+crc+crypto")
                 if autoconf_check(self.compiler, flag_check="-march=armv8-a+crc"):
                     gcc_arm_crc_flags.append("-march=armv8-a+crc")
-                    gcc_arm_crc_pmull_flags.append("-march=armv8-a+crc+crypto")
                     # Resolve problems on armv7, see issue #56
                     if not IS_AARCH64:
                         gcc_arm_crc_flags.append("-fno-lto")
                         gcc_arm_crc_pmull_flags.append("-fno-lto")
                 if not IS_AARCH64 and autoconf_check(self.compiler, flag_check="-mfpu=neon"):
                     gcc_arm_neon_flags.append("-mfpu=neon")
                     # Resolve problems on armv7, see issue #56
```

### Comparing `sabctools-8.2.2/src/crc32.cc` & `sabctools-8.2.3/src/crc32.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crc32.h` & `sabctools-8.2.3/src/crc32.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/COPYING` & `sabctools-8.2.3/src/crcutil-1.0/COPYING`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/INSTALL` & `sabctools-8.2.3/src/crcutil-1.0/INSTALL`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/LICENSE` & `sabctools-8.2.3/src/crcutil-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/Makefile` & `sabctools-8.2.3/src/crcutil-1.0/Makefile`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/Makefile.am` & `sabctools-8.2.3/src/crcutil-1.0/Makefile.am`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/Makefile.in` & `sabctools-8.2.3/src/crcutil-1.0/Makefile.in`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/Makefile.win` & `sabctools-8.2.3/src/crcutil-1.0/Makefile.win`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/README` & `sabctools-8.2.3/src/crcutil-1.0/README`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/aclocal.m4` & `sabctools-8.2.3/src/crcutil-1.0/aclocal.m4`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/autogen.sh` & `sabctools-8.2.3/src/crcutil-1.0/autogen.sh`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/base_types.h` & `sabctools-8.2.3/src/crcutil-1.0/code/base_types.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4.cc` & `sabctools-8.2.3/src/crcutil-1.0/code/crc32c_sse4.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4.h` & `sabctools-8.2.3/src/crcutil-1.0/code/crc32c_sse4.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/crc32c_sse4_intrin.h` & `sabctools-8.2.3/src/crcutil-1.0/code/crc32c_sse4_intrin.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/crc_casts.h` & `sabctools-8.2.3/src/crcutil-1.0/code/crc_casts.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/generic_crc.h` & `sabctools-8.2.3/src/crcutil-1.0/code/generic_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/gf_util.h` & `sabctools-8.2.3/src/crcutil-1.0/code/gf_util.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc` & `sabctools-8.2.3/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc` & `sabctools-8.2.3/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc` & `sabctools-8.2.3/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc` & `sabctools-8.2.3/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc` & `sabctools-8.2.3/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/platform.h` & `sabctools-8.2.3/src/crcutil-1.0/code/platform.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/protected_crc.h` & `sabctools-8.2.3/src/crcutil-1.0/code/protected_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/rolling_crc.h` & `sabctools-8.2.3/src/crcutil-1.0/code/rolling_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/std_headers.h` & `sabctools-8.2.3/src/crcutil-1.0/code/std_headers.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/code/uint128_sse2.h` & `sabctools-8.2.3/src/crcutil-1.0/code/uint128_sse2.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/config.h.in` & `sabctools-8.2.3/src/crcutil-1.0/config.h.in`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/configure` & `sabctools-8.2.3/src/crcutil-1.0/configure`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/configure.ac` & `sabctools-8.2.3/src/crcutil-1.0/configure.ac`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/depcomp` & `sabctools-8.2.3/src/crcutil-1.0/depcomp`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/examples/interface.cc` & `sabctools-8.2.3/src/crcutil-1.0/examples/interface.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/examples/interface.h` & `sabctools-8.2.3/src/crcutil-1.0/examples/interface.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/examples/usage.cc` & `sabctools-8.2.3/src/crcutil-1.0/examples/usage.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/install-sh` & `sabctools-8.2.3/src/crcutil-1.0/install-sh`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/missing` & `sabctools-8.2.3/src/crcutil-1.0/missing`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/tests/aligned_alloc.h` & `sabctools-8.2.3/src/crcutil-1.0/tests/aligned_alloc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/tests/bob_jenkins_rng.h` & `sabctools-8.2.3/src/crcutil-1.0/tests/bob_jenkins_rng.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/tests/rdtsc.h` & `sabctools-8.2.3/src/crcutil-1.0/tests/rdtsc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/tests/set_hi_pri.c` & `sabctools-8.2.3/src/crcutil-1.0/tests/set_hi_pri.c`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/tests/unittest.cc` & `sabctools-8.2.3/src/crcutil-1.0/tests/unittest.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/tests/unittest.h` & `sabctools-8.2.3/src/crcutil-1.0/tests/unittest.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/crcutil-1.0/tests/unittest_helper.h` & `sabctools-8.2.3/src/crcutil-1.0/tests/unittest_helper.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/sabctools.cc` & `sabctools-8.2.3/src/sabctools.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/sabctools.h` & `sabctools-8.2.3/src/sabctools.h`

 * *Files 14% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 
 #include <Python.h>
 #include <stdio.h>
 #include <fcntl.h>
 #include <string.h>
 
 /* Version information */
-#define SABCTOOLS_VERSION "8.2.2"
+#define SABCTOOLS_VERSION "8.2.3"
 
 PyMODINIT_FUNC PyInit_sabctools(void);
```

### Comparing `sabctools-8.2.2/src/sabctools.pyi` & `sabctools-8.2.3/src/sabctools.pyi`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/sparse.cc` & `sabctools-8.2.3/src/sparse.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/sparse.h` & `sabctools-8.2.3/src/sparse.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/unlocked_ssl.cc` & `sabctools-8.2.3/src/unlocked_ssl.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/unlocked_ssl.h` & `sabctools-8.2.3/src/unlocked_ssl.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/utils.cc` & `sabctools-8.2.3/src/utils.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/utils.h` & `sabctools-8.2.3/src/utils.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yenc.cc` & `sabctools-8.2.3/src/yenc.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yenc.h` & `sabctools-8.2.3/src/yenc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/common.h` & `sabctools-8.2.3/src/yencode/common.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/crc.cc` & `sabctools-8.2.3/src/yencode/crc.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/crc.h` & `sabctools-8.2.3/src/yencode/crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/crc_arm.cc` & `sabctools-8.2.3/src/yencode/crc_arm.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/crc_arm_pmull.cc` & `sabctools-8.2.3/src/yencode/crc_arm_pmull.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/crc_common.h` & `sabctools-8.2.3/src/yencode/crc_common.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/crc_folding.cc` & `sabctools-8.2.3/src/yencode/crc_folding.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/crc_folding_256.cc` & `sabctools-8.2.3/src/yencode/crc_folding_256.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/crc_riscv.cc` & `sabctools-8.2.3/src/yencode/crc_riscv.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder.cc` & `sabctools-8.2.3/src/yencode/decoder.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder.h` & `sabctools-8.2.3/src/yencode/decoder.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_avx.cc` & `sabctools-8.2.3/src/yencode/decoder_avx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_avx2.cc` & `sabctools-8.2.3/src/yencode/decoder_avx2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_avx2_base.h` & `sabctools-8.2.3/src/yencode/decoder_avx2_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_common.h` & `sabctools-8.2.3/src/yencode/decoder_common.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_neon.cc` & `sabctools-8.2.3/src/yencode/decoder_neon.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_neon64.cc` & `sabctools-8.2.3/src/yencode/decoder_neon64.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_rvv.cc` & `sabctools-8.2.3/src/yencode/decoder_rvv.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_sse2.cc` & `sabctools-8.2.3/src/yencode/decoder_sse2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_sse_base.h` & `sabctools-8.2.3/src/yencode/decoder_sse_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_ssse3.cc` & `sabctools-8.2.3/src/yencode/decoder_ssse3.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/decoder_vbmi2.cc` & `sabctools-8.2.3/src/yencode/decoder_vbmi2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/encoder.cc` & `sabctools-8.2.3/src/yencode/encoder.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/encoder.h` & `sabctools-8.2.3/src/yencode/encoder.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/encoder_avx_base.h` & `sabctools-8.2.3/src/yencode/encoder_avx_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/encoder_common.h` & `sabctools-8.2.3/src/yencode/encoder_common.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/encoder_neon.cc` & `sabctools-8.2.3/src/yencode/encoder_neon.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/encoder_rvv.cc` & `sabctools-8.2.3/src/yencode/encoder_rvv.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/encoder_sse_base.h` & `sabctools-8.2.3/src/yencode/encoder_sse_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/encoder_ssse3.cc` & `sabctools-8.2.3/src/yencode/encoder_ssse3.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/encoder_vbmi2.cc` & `sabctools-8.2.3/src/yencode/encoder_vbmi2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/hedley.h` & `sabctools-8.2.3/src/yencode/hedley.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/platform.cc` & `sabctools-8.2.3/src/yencode/platform.cc`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/src/yencode/stdint.h` & `sabctools-8.2.3/src/yencode/stdint.h`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/tests/test.py` & `sabctools-8.2.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/tests/test_crc32.py` & `sabctools-8.2.3/tests/test_crc32.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/tests/test_decoder.py` & `sabctools-8.2.3/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/tests/test_sparse.py` & `sabctools-8.2.3/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/tests/test_unlocked_ssl.py` & `sabctools-8.2.3/tests/test_unlocked_ssl.py`

 * *Files identical despite different names*

### Comparing `sabctools-8.2.2/tests/testsupport.py` & `sabctools-8.2.3/tests/testsupport.py`

 * *Files identical despite different names*

