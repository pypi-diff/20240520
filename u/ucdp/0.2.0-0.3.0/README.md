# Comparing `tmp/ucdp-0.2.0.tar.gz` & `tmp/ucdp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucdp-0.2.0.tar", last modified: Wed May  8 15:34:46 2024, max compression
+gzip compressed data, was "ucdp-0.3.0.tar", last modified: Mon May 20 21:52:05 2024, max compression
```

## Comparing `ucdp-0.2.0.tar` & `ucdp-0.3.0.tar`

### file list

```diff
@@ -1,95 +1,99 @@
--rw-r--r--   0        0        0     1067 2024-05-08 15:34:32.481678 ucdp-0.2.0/LICENSE
--rw-r--r--   0        0        0      939 2024-05-08 15:34:32.481678 ucdp-0.2.0/README.md
--rw-r--r--   0        0        0     2635 2024-05-08 15:34:46.397773 ucdp-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6939 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/__init__.py
--rw-r--r--   0        0        0     2972 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/_modbuilder.py
--rw-r--r--   0        0        0    12128 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/assigns.py
--rw-r--r--   0        0        0     1959 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/baseclassinfo.py
--rw-r--r--   0        0        0      360 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/buildproduct.py
--rw-r--r--   0        0        0     5545 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/cli.py
--rw-r--r--   0        0        0     5680 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/config.py
--rw-r--r--   0        0        0     3332 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/const.py
--rw-r--r--   0        0        0     1350 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/consts.py
--rw-r--r--   0        0        0     2683 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/dict.py
--rw-r--r--   0        0        0     3492 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/doc.py
--rw-r--r--   0        0        0     2372 2024-05-08 15:34:32.481678 ucdp-0.2.0/src/ucdp/docutil.py
--rw-r--r--   0        0        0     1144 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/bad/glbl_bad/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/bad/glbl_bad/regf.py
--rw-r--r--   0        0        0     1443 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/filelist/filelist_lib/filelist.py
--rw-r--r--   0        0        0       67 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/filelist/filelist_lib/mod.f
--rw-r--r--   0        0        0     1758 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/fileliststandard.py
--rw-r--r--   0        0        0     1140 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/__init__.py
--rw-r--r--   0        0        0     2696 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/bus.py
--rw-r--r--   0        0        0     1565 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/clk_gate.py
--rw-r--r--   0        0        0     3405 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/regf.py
--rw-r--r--   0        0        0     1388 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/glbl/regf_tb.py
--rw-r--r--   0        0        0     1129 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/uart/__init__.py
--rw-r--r--   0        0        0     2607 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/examples/simple/uart/uart.py
--rw-r--r--   0        0        0     1587 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/exceptions.py
--rw-r--r--   0        0        0    16035 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/expr.py
--rw-r--r--   0        0        0    13341 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/exprparser.py
--rw-r--r--   0        0        0     5040 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/exprresolver.py
--rw-r--r--   0        0        0     3603 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/filelistparser.py
--rw-r--r--   0        0        0     2908 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/fileset.py
--rw-r--r--   0        0        0     1762 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/flipflop.py
--rw-r--r--   0        0        0     2817 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/generate.py
--rw-r--r--   0        0        0     1884 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/humannum.py
--rw-r--r--   0        0        0    12472 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/ident.py
--rw-r--r--   0        0        0     3472 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/iterutil.py
--rw-r--r--   0        0        0     2908 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/loader.py
--rw-r--r--   0        0        0     1179 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/logging.py
--rw-r--r--   0        0        0     2221 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/mod.py
--rw-r--r--   0        0        0    32207 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modbase.py
--rw-r--r--   0        0        0     2232 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modbasetop.py
--rw-r--r--   0        0        0     3761 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modconfigurable.py
--rw-r--r--   0        0        0     2772 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modcore.py
--rw-r--r--   0        0        0     7539 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modfilelist.py
--rw-r--r--   0        0        0    11630 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/moditer.py
--rw-r--r--   0        0        0     3190 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modref.py
--rw-r--r--   0        0        0     5551 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modtailored.py
--rw-r--r--   0        0        0     5808 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modtb.py
--rw-r--r--   0        0        0     3388 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modtopref.py
--rw-r--r--   0        0        0     1686 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/modutil.py
--rw-r--r--   0        0        0     4047 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/mux.py
--rw-r--r--   0        0        0     6419 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/namespace.py
--rw-r--r--   0        0        0     4942 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/nameutil.py
--rw-r--r--   0        0        0      514 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/note.py
--rw-r--r--   0        0        0     4690 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/object.py
--rw-r--r--   0        0        0     5440 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/orientation.py
--rw-r--r--   0        0        0     3970 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/param.py
--rw-r--r--   0        0        0     3898 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/pathutil.py
--rw-r--r--   0        0        0     5735 2024-05-08 15:34:32.485678 ucdp-0.2.0/src/ucdp/routepath.py
--rw-r--r--   0        0        0     7439 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/signal.py
--rw-r--r--   0        0        0     8021 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/slices.py
--rw-r--r--   0        0        0     1258 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/test.py
--rw-r--r--   0        0        0     3167 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/top.py
--rw-r--r--   0        0        0     3644 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typearray.py
--rw-r--r--   0        0        0     4922 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typebase.py
--rw-r--r--   0        0        0     5457 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typeclkrst.py
--rw-r--r--   0        0        0     7908 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typedescriptivestruct.py
--rw-r--r--   0        0        0    20080 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typeenum.py
--rw-r--r--   0        0        0    22840 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typescalar.py
--rw-r--r--   0        0        0     2043 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typestring.py
--rw-r--r--   0        0        0    12024 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/typestruct.py
--rw-r--r--   0        0        0     1476 2024-05-08 15:34:32.489678 ucdp-0.2.0/src/ucdp/util.py
--rw-r--r--   0        0        0       13 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      745 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0    16826 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_assigns.py
--rw-r--r--   0        0        0     2876 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_baseclassinfo.py
--rw-r--r--   0        0        0     1611 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_buildproduct.py
--rw-r--r--   0        0        0     1914 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_config.py
--rw-r--r--   0        0        0     2793 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_examples.py
--rw-r--r--   0        0        0     1637 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_exprparser.py
--rw-r--r--   0        0        0     1877 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_fileset.py
--rw-r--r--   0        0        0     2077 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_flipflop.py
--rw-r--r--   0        0        0     4756 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_light_object.py
--rw-r--r--   0        0        0     6054 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_loader.py
--rw-r--r--   0        0        0     2842 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_modfilelist.py
--rw-r--r--   0        0        0     1587 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_mux.py
--rw-r--r--   0        0        0    13658 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_namespace.py
--rw-r--r--   0        0        0     4665 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_object.py
--rw-r--r--   0        0        0     8485 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_pathutil.py
--rw-r--r--   0        0        0     3489 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_typeenum.py
--rw-r--r--   0        0        0     5436 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_typescalar.py
--rw-r--r--   0        0        0     4047 2024-05-08 15:34:32.489678 ucdp-0.2.0/tests/test_typestruct.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 ucdp-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-20 21:51:52.867201 ucdp-0.3.0/LICENSE
+-rw-r--r--   0        0        0      939 2024-05-20 21:51:52.867201 ucdp-0.3.0/README.md
+-rw-r--r--   0        0        0     2635 2024-05-20 21:52:05.087167 ucdp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7153 2024-05-20 21:51:52.867201 ucdp-0.3.0/src/ucdp/__init__.py
+-rw-r--r--   0        0        0     2977 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/_modbuilder.py
+-rw-r--r--   0        0        0    12421 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/assigns.py
+-rw-r--r--   0        0        0     2002 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/baseclassinfo.py
+-rw-r--r--   0        0        0      360 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/buildproduct.py
+-rw-r--r--   0        0        0     7337 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/cli.py
+-rw-r--r--   0        0        0     6692 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/config.py
+-rw-r--r--   0        0        0     3870 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/const.py
+-rw-r--r--   0        0        0     1446 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/consts.py
+-rw-r--r--   0        0        0     2942 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/dict.py
+-rw-r--r--   0        0        0     3740 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/doc.py
+-rw-r--r--   0        0        0     2531 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/docutil.py
+-rw-r--r--   0        0        0     1144 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/bad/glbl_bad_lib/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/bad/glbl_bad_lib/regf.py
+-rw-r--r--   0        0        0     1443 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/filelist/filelist_lib/filelist.py
+-rw-r--r--   0        0        0       67 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/filelist/filelist_lib/mod.f
+-rw-r--r--   0        0        0     1943 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/param/param_lib/param.py
+-rw-r--r--   0        0        0     1810 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/fileliststandard.py
+-rw-r--r--   0        0        0     1140 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/bus.py
+-rw-r--r--   0        0        0     1565 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/clk_gate.py
+-rw-r--r--   0        0        0     3405 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/regf.py
+-rw-r--r--   0        0        0     1388 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/regf_tb.py
+-rw-r--r--   0        0        0     1129 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/uart_lib/__init__.py
+-rw-r--r--   0        0        0     2762 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/examples/simple/uart_lib/uart.py
+-rw-r--r--   0        0        0     1587 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/exceptions.py
+-rw-r--r--   0        0        0    20667 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/expr.py
+-rw-r--r--   0        0        0    13228 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/exprparser.py
+-rw-r--r--   0        0        0     8039 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/exprresolver.py
+-rw-r--r--   0        0        0     4842 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/filelistparser.py
+-rw-r--r--   0        0        0     3008 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/fileset.py
+-rw-r--r--   0        0        0     1878 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/flipflop.py
+-rw-r--r--   0        0        0     5047 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/generate.py
+-rw-r--r--   0        0        0     1932 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/humannum.py
+-rw-r--r--   0        0        0    12474 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/ident.py
+-rw-r--r--   0        0        0     4036 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/iterutil.py
+-rw-r--r--   0        0        0     3303 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/loader.py
+-rw-r--r--   0        0        0     1179 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/logging.py
+-rw-r--r--   0        0        0     2380 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/mod.py
+-rw-r--r--   0        0        0    32835 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modbase.py
+-rw-r--r--   0        0        0     2232 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modbasetop.py
+-rw-r--r--   0        0        0     4113 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modconfigurable.py
+-rw-r--r--   0        0        0     2928 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modcore.py
+-rw-r--r--   0        0        0    10363 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modfilelist.py
+-rw-r--r--   0        0        0    12681 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/moditer.py
+-rw-r--r--   0        0        0     3521 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modref.py
+-rw-r--r--   0        0        0     5938 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modtailored.py
+-rw-r--r--   0        0        0     6332 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modtb.py
+-rw-r--r--   0        0        0     3541 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modtopref.py
+-rw-r--r--   0        0        0     1776 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/modutil.py
+-rw-r--r--   0        0        0     4072 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/mux.py
+-rw-r--r--   0        0        0     6793 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/namespace.py
+-rw-r--r--   0        0        0     6226 2024-05-20 21:51:52.871201 ucdp-0.3.0/src/ucdp/nameutil.py
+-rw-r--r--   0        0        0      551 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/note.py
+-rw-r--r--   0        0        0     4743 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/object.py
+-rw-r--r--   0        0        0     5440 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/orientation.py
+-rw-r--r--   0        0        0     4517 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/param.py
+-rw-r--r--   0        0        0     3898 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/pathutil.py
+-rw-r--r--   0        0        0     5735 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/routepath.py
+-rw-r--r--   0        0        0     7224 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/signal.py
+-rw-r--r--   0        0        0     8282 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/slices.py
+-rw-r--r--   0        0        0       33 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/templates/main.mako
+-rw-r--r--   0        0        0     1258 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/test.py
+-rw-r--r--   0        0        0     3443 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/top.py
+-rw-r--r--   0        0        0     3644 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typearray.py
+-rw-r--r--   0        0        0     5078 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typebase.py
+-rw-r--r--   0        0        0     5457 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typeclkrst.py
+-rw-r--r--   0        0        0     7908 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typedescriptivestruct.py
+-rw-r--r--   0        0        0    20080 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typeenum.py
+-rw-r--r--   0        0        0    22840 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typescalar.py
+-rw-r--r--   0        0        0     2043 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typestring.py
+-rw-r--r--   0        0        0    11994 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/typestruct.py
+-rw-r--r--   0        0        0     1570 2024-05-20 21:51:52.875201 ucdp-0.3.0/src/ucdp/util.py
+-rw-r--r--   0        0        0       13 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      936 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0    16882 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_assigns.py
+-rw-r--r--   0        0        0     2892 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_baseclassinfo.py
+-rw-r--r--   0        0        0     1611 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_buildproduct.py
+-rw-r--r--   0        0        0     1914 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_config.py
+-rw-r--r--   0        0        0     3962 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_examples.py
+-rw-r--r--   0        0        0     3086 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_exprparser.py
+-rw-r--r--   0        0        0     1856 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_exprresolver.py
+-rw-r--r--   0        0        0     2022 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_fileset.py
+-rw-r--r--   0        0        0     2077 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_flipflop.py
+-rw-r--r--   0        0        0     4756 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_light_object.py
+-rw-r--r--   0        0        0     6445 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_loader.py
+-rw-r--r--   0        0        0     2947 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_modfilelist.py
+-rw-r--r--   0        0        0     1587 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_mux.py
+-rw-r--r--   0        0        0    13658 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_namespace.py
+-rw-r--r--   0        0        0     4665 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_object.py
+-rw-r--r--   0        0        0     8485 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_pathutil.py
+-rw-r--r--   0        0        0     3362 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_routepath.py
+-rw-r--r--   0        0        0     3489 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_typeenum.py
+-rw-r--r--   0        0        0     5436 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_typescalar.py
+-rw-r--r--   0        0        0     4047 2024-05-20 21:51:52.875201 ucdp-0.3.0/tests/test_typestruct.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 ucdp-0.3.0/PKG-INFO
```

### Comparing `ucdp-0.2.0/LICENSE` & `ucdp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/README.md` & `ucdp-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/pyproject.toml` & `ucdp-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ucdp"
-version = "0.2.0"
+version = "0.3.0"
 description = "Unified Chip Design Platform"
 readme = "README.md"
 authors = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
@@ -12,15 +12,15 @@
 dependencies = [
     "anytree>=2.12.1",
     "case-converter>=1.1.0",
     "click>=8.1.7",
     "fuzzywuzzy>=0.18.0",
     "humannum>=1.0.0",
     "icdutil>=0.3.1",
-    "makolator>=2.4.0",
+    "makolator>=2.6.0",
     "matchor>=0.1.0",
     "pydantic>=2.7.0",
     "python-Levenshtein>=0.25.1",
     "rich>=13.7.1",
     "uniquer>=1.0.2",
 ]
```

### Comparing `ucdp-0.2.0/src/ucdp/__init__.py` & `ucdp-0.3.0/src/ucdp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,30 +53,30 @@
 from .exprresolver import ExprResolver
 from .filelistparser import FileListParser
 from .fileset import FileSet, LibPath
 from .flipflop import FlipFlop
 from .generate import generate
 from .humannum import Bin, Bytes, Hex
 from .ident import Ident, IdentFilter, Idents, IdentStop, get_ident
-from .iterutil import namefilter, split
+from .iterutil import Names, namefilter, split
 from .loader import load
 from .mod import AMod
 from .modbase import BaseMod
 from .modbasetop import BaseTopMod
 from .modconfigurable import AConfigurableMod
-from .modcore import CoreMod
+from .modcore import ACoreMod
 from .modfilelist import (
     ModFileList,
     ModFileLists,
     Paths,
     Placeholder,
     ToPaths,
     iter_modfilelists,
     resolve_modfilelist,
-    search_modfilelist,
+    search_modfilelists,
 )
 from .moditer import ModPostIter, ModPreIter, uniquemods
 from .modref import ModRef
 from .modtailored import ATailoredMod
 from .modtb import AGenericTbMod, ATbMod
 from .modtopref import TopModRef
 from .modutil import get_modbaseinfos, is_tb_from_modname
@@ -93,14 +93,15 @@
     OUT,
     AOrientation,
     Direction,
     Orientation,
 )
 from .param import Param
 from .pathutil import improved_glob, improved_resolve, startswith_envvar, use_envvars
+from .routepath import Routeable, Routeables, RoutePath, parse_routepath, parse_routepaths
 from .signal import BaseSignal, Port, Signal
 from .slices import DOWN, UP, Slice, SliceDirection
 from .test import Test
 from .typearray import ArrayType
 from .typebase import ACompositeType, AScalarType, AVecType, BaseScalarType, BaseType
 from .typeclkrst import ClkRstAnType, ClkType, DiffClkRstAnType, DiffClkType, RstAnType, RstAType, RstType
 from .typedescriptivestruct import DescriptiveStructType
@@ -118,14 +119,19 @@
     fwdfilter,
 )
 from .util import extend_sys_path
 
 __all__ = [
     "ABuildProduct",
     "ACompositeType",
+    "parse_routepath",
+    "parse_routepaths",
+    "Routeable",
+    "Routeables",
+    "RoutePath",
     "AConfig",
     "AConfigurableMod",
     "AEnumType",
     "AGenericTbMod",
     "AGlobalEnumType",
     "AGlobalStructType",
     "AMod",
@@ -162,15 +168,15 @@
     "Bytes",
     "ClkRstAnType",
     "ClkType",
     "ConcatExpr",
     "const",
     "Const",
     "ConstExpr",
-    "CoreMod",
+    "ACoreMod",
     "DescriptiveStructType",
     "Dict",
     "didyoumean",
     "DiffClkRstAnType",
     "DiffClkType",
     "Direction",
     "DirectionError",
@@ -229,14 +235,15 @@
     "ModPostIter",
     "ModPreIter",
     "ModRef",
     "Mux",
     "NamedLightObject",
     "NamedObject",
     "namefilter",
+    "Names",
     "Namespace",
     "Note",
     "Object",
     "Op",
     "OPEN",
     "Orientation",
     "OUT",
@@ -250,15 +257,15 @@
     "PrivateField",
     "RailType",
     "RangeExpr",
     "resolve_modfilelist",
     "RstAnType",
     "RstAType",
     "RstType",
-    "search_modfilelist",
+    "search_modfilelists",
     "Signal",
     "SintType",
     "Slice",
     "SliceDirection",
     "SliceOp",
     "SOp",
     "split_prefix",
```

### Comparing `ucdp-0.2.0/src/ucdp/_modbuilder.py` & `ucdp-0.3.0/src/ucdp/_modbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     return mod.is_locked
 
 
 def _build(mod: BaseMod, name: str):
     insts: set[int] = set()
 
     for iteration in range(1, TIMEOUT):
-        LOGGER.debug(f"{mod}: builder: {name} iteration {iteration}")
+        LOGGER.debug("%s: builder: %s iteration %s", mod, name, iteration)
         pending = False
         for inst in ModPreIter(mod=mod, stop=_stop_at_locked):
             instid = hash((inst.qualname, inst.inst))
 
             # build every instance just once
             if instid in insts:
                 continue
```

### Comparing `ucdp-0.2.0/src/ucdp/assigns.py` & `ucdp-0.3.0/src/ucdp/assigns.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,19 +96,19 @@
         'vec_c_s  ---->  None'
 
 """
 
 from collections.abc import Iterable, Iterator
 from typing import Any
 
-from .exceptions import DirectionError, LockError
+from .exceptions import LockError
 from .expr import Expr
-from .ident import Ident, Idents, get_expridents
+from .ident import Ident, Idents
 from .note import Note
-from .object import Field, LightObject, Object, PrivateField, model_validator
+from .object import Field, Object, PrivateField, model_validator
 from .orientation import BWD, FWD, IN, INOUT, OUT, Direction
 from .signal import BaseSignal, Port
 from .typebase import BaseScalarType
 
 _DIRECTION_MAP = {
     IN: "---->",
     OUT: "<----",
@@ -133,44 +133,60 @@
         drivers: Dictionary with drivers.
     """
 
     drivers: dict[str, AssignSource] = Field(default_factory=dict)
 
     def __setitem__(self, name, item):
         drivers = self.drivers
-        if name in drivers:
-            raise ValueError(f"'{item}' already driven by '{drivers[name]}'")
+        # if name in drivers:
+        #     raise ValueError(f"'{item}' already driven by '{drivers[name]}'")
         drivers[name] = item
 
     def __iter__(self) -> Iterator[tuple[str, AssignSource]]:  # type: ignore[override]
         yield from self.drivers.items()
 
 
-class Assign(LightObject):
+# class Assign(LightObject):
+class Assign(Object):
     """
     A Single Assignment of `expr` to `target`.
 
     Attributes:
         target: Assigned identifier.
         source: Assigned expression.
     """
 
     target: BaseSignal
     source: AssignSource | None = None
 
     @property
+    def name(self) -> str | None:
+        """Name."""
+        return self.target.name
+
+    @property
     def type_(self):
         """Type."""
-        return self.type_
+        return self.target.type_
+
+    @property
+    def doc(self):
+        """Doc."""
+        return self.target.doc
 
     @property
     def direction(self) -> Direction:
         """Direction."""
         return Direction.cast(self.target.direction)  # type: ignore[return-value]
 
+    @property
+    def ifdef(self) -> str | None:
+        """IFDEF."""
+        return self.target.ifdef
+
     def __str__(self):
         return f"{self.target}  {_DIRECTION_MAP[self.direction]}  {self.source}"
 
 
 _TargetAssigns = dict[str, AssignSource | None]
 
 
@@ -261,21 +277,21 @@
         sub = "sub-level " if self.sub else ""
         targetdir = isinstance(target, Port) and (target.direction * orient)
 
         # do not check INOUT
         if not targetdir or not targetdir.mode:
             return
 
-        # Check Expression Source Direction
-        for sourceident in get_expridents(source):
-            sourcedir = sourceident.direction
-            if sourcedir is None:
-                sourcedir = IN
-            if targetdir == sourcedir:
-                raise DirectionError(f"Cannot connect {sub}{target.direction} '{target}' and {sourcedir} '{source}'")
+        # # Check Expression Source Direction
+        # for sourceident in get_expridents(source):
+        #     sourcedir = sourceident.direction
+        #     if sourcedir is None:
+        #         sourcedir = IN
+        #     if targetdir == sourcedir:
+        #         raise DirectionError(f"Cannot connect {sub}{target.direction} '{target}' and {sourcedir} '{source}'")
 
         # Check Types
         connectable = target.type_.is_connectable(source.type_)
         if not connectable:
             msg = f"Cannot assign '{source}' of {source.type_} to {sub}'{target}' of {target.type_}"
             raise TypeError(msg)
```

### Comparing `ucdp-0.2.0/src/ucdp/baseclassinfo.py` & `ucdp-0.3.0/src/ucdp/baseclassinfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,27 +32,27 @@
 
 from .object import LightObject
 
 _RE_INFO = re.compile(r"^<class '(?P<libname>.+)\.(?P<modname>.+)\.(?P<clsname>.+)'>$")
 
 
 class BaseClassInfo(LightObject):
-    """Base Class Information."""
+    """Base Class Information.
 
-    cls: Any
-    """Class."""
+    Attributes:
+        cls: Class.
+        libname: Python Library Name.
+        modname: Python Module Name.
+        clsname: Python Class Name.
+    """
 
+    cls: Any
     libname: str
-    """Python Library Name."""
-
     modname: str
-    """Python Module Name."""
-
     clsname: str
-    """Python Class Name."""
 
 
 def get_baseclassinfos(cls_or_inst) -> Iterator[BaseClassInfo]:
     """Base Class Info."""
     if not isclass(cls_or_inst):
         cls_or_inst = cls_or_inst.__class__
     for mro in getmro(cls_or_inst):
```

### Comparing `ucdp-0.2.0/src/ucdp/cli.py` & `ucdp-0.3.0/src/ucdp/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,22 +28,23 @@
 from pathlib import Path
 
 import click
 from anytree import Node, RenderTree
 from pydantic import BaseModel, ConfigDict
 from rich.console import Console
 from rich.logging import RichHandler
+from rich.pretty import pprint
 
 from .fileset import FileSet
-from .generate import generate
+from .generate import clean, generate, get_makolator
 from .loader import load
+from .modfilelist import iter_modfilelists
 from .moditer import ModPreIter
 from .modtopref import PAT_TOPMODREF
 from .top import Top
-from .util import extend_sys_path
 
 _LOGLEVELMAP = {
     0: logging.WARNING,
     1: logging.INFO,
     2: logging.DEBUG,
 }
 
@@ -70,20 +71,24 @@
 Search Path For Data Model Files.
 This option can be specified multiple times.
 Environment Variable 'UCDP_PATH'.
 """,
 )
 arg_filelist = click.argument("filelist", envvar="UCDP_FILELIST")
 opt_target = click.option("--target", "-t", help="Filter File List for Target", envvar="UCDP_TARGET")
+opt_show_diff = click.option(
+    "--show-diff", "-s", default=False, is_flag=True, help="Show What Changed", envvar="UCDP_SHOW_DIFF"
+)
+opt_maxlevel = click.option("--maxlevel", "-L", type=int, help="Limit to maximum number of hierarchy levels.")
+opt_dry_run = click.option("--dry-run", default=False, is_flag=True, help="Do nothing.")
 
 
-def _load_top(ctx, top, path) -> Top:
+def _load_top(ctx, top, paths) -> Top:
     with ctx.console.status(f"Loading {top!r}"):
-        with extend_sys_path(path):
-            return load(top)
+        return load(top, paths=paths)
 
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.option("-v", "--verbose", count=True, help="Increase Verbosity.")
 @click.version_option()
 @click.pass_context
 def ucdp(ctx, verbose=0):
@@ -101,22 +106,24 @@
 Load Data Model and Check.
 
 TOP: Top Module. {PAT_TOPMODREF}. Environment Variable 'UCDP_TOP'
 """
 )
 @arg_top
 @opt_path
+@click.option("--stat", default=False, is_flag=True, help="Show Statistics.")
 @pass_ctx
-def check(ctx, top, path):
+def check(ctx, top, path, stat=False):
     """Check."""
     top = _load_top(ctx, top, path)
-
-    instcnt = len(top.get_mods())
-    modcnt = len(top.get_mods(unique=True))
-    ctx.console.log(f"{str(top.ref)!r} checked ({instcnt} instances of {modcnt} modules).")
+    ctx.console.log(f"{str(top.ref)!r} checked.")
+    if stat:
+        print("Statistics:")
+        for name, value in top.get_stat().items():
+            print(f"  {name}: {value}")
 
 
 @ucdp.command(
     help=f"""
 Load Data Model and Generate Files.
 
 TOP: Top Module. {PAT_TOPMODREF}. Environment Variable 'UCDP_TOP'
@@ -124,19 +131,44 @@
 FILELIST: Filelist name to render. Environment Variable 'UCDP_FILELIST'
 """
 )
 @arg_top
 @opt_path
 @arg_filelist
 @opt_target
+@opt_show_diff
 @pass_ctx
-def gen(ctx, top, path, filelist, target=None):
+def gen(ctx, top, path, filelist, target=None, show_diff=False):
     """Generate."""
     top = _load_top(ctx, top, path)
-    generate(top.mod, filelist, target=target)
+    makolator = get_makolator(show_diff=show_diff)
+    generate(top.mod, filelist, target=target, makolator=makolator)
+
+
+@ucdp.command(
+    help=f"""
+Load Data Model and REMOVE Generated Files.
+
+TOP: Top Module. {PAT_TOPMODREF}. Environment Variable 'UCDP_TOP'
+
+FILELIST: Filelist name to render. Environment Variable 'UCDP_FILELIST'
+"""
+)
+@arg_top
+@opt_path
+@arg_filelist
+@opt_target
+@opt_show_diff
+@opt_dry_run
+@pass_ctx
+def cleangen(ctx, top, path, filelist, target=None, show_diff=False, dry_run=False):
+    """Clean Generated Files."""
+    top = _load_top(ctx, top, path)
+    makolator = get_makolator(show_diff=show_diff)
+    clean(top.mod, filelist, target=target, makolator=makolator, dry_run=dry_run)
 
 
 @ucdp.command(
     help=f"""
 Load Data Model and Generate File List.
 
 TOP: Top Module. {PAT_TOPMODREF}. Environment Variable 'UCDP_TOP'
@@ -150,22 +182,49 @@
 @opt_target
 @pass_ctx
 def filelist(ctx, top, path, filelist, target=None):
     """File List."""
     top = _load_top(ctx, top, path)
 
     fileset = FileSet.from_mod(top.mod, filelist, target=target)
-    for incdir in fileset.incdirs:
+    for incdir in fileset.inc_dirs:
         print(f"-incdir {incdir}")
     for libfilepath in fileset.filepaths:
         print(str(libfilepath.path))
 
 
 @ucdp.command(
     help=f"""
+Load Data Model and Show File Information
+
+TOP: Top Module. {PAT_TOPMODREF}. Environment Variable 'UCDP_TOP'
+
+FILELIST: Filelist name to render. Environment Variable 'UCDP_FILELIST'
+"""
+)
+@arg_top
+@opt_path
+@arg_filelist
+@opt_target
+@opt_maxlevel
+@pass_ctx
+def fileinfo(ctx, top, path, filelist, target=None, maxlevel=None):
+    """File List."""
+    top = _load_top(ctx, top, path)
+    pprint(
+        {
+            str(mod): modfilelist
+            for mod, modfilelist in iter_modfilelists(top.mod, filelist, target=target, maxlevel=maxlevel)
+        },
+        indent_guides=False,
+    )
+
+
+@ucdp.command(
+    help=f"""
 Load Data Model and Show Module Overview.
 
 TOP: Top Module. {PAT_TOPMODREF}. Environment Variable 'UCDP_TOP'
 """
 )
 @arg_top
 @opt_path
```

### Comparing `ucdp-0.2.0/src/ucdp/config.py` & `ucdp-0.3.0/src/ucdp/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,67 +43,76 @@
     * how many instances or which instances should be created
 
     A configuration **MUST** have at least a name.
 
     Due to the frozen instance approach, configurations have to be implemented
     via `u.field()`.
 
-    Example:
-        >>> import ucdp as u
-        >>> class MyConfig(u.AConfig):
-        ...
-        ...     mem_baseaddr: u.Hex # required without default
-        ...     ram_size: u.Bytes
-        ...     rom_size: u.Bytes|None = None
-        ...     feature: bool = False
-
-        >>> variant0  = MyConfig(name='variant0', mem_baseaddr=4*1024, ram_size='16kB')
-        >>> variant0
-        MyConfig('variant0', mem_baseaddr=Hex('0x1000'), ram_size=Bytes('16 KB'))
-        >>> variant0.mem_baseaddr
-        Hex('0x1000')
-        >>> variant0.ram_size
-        Bytes('16 KB')
-        >>> variant0.rom_size
-        >>> variant0.feature
-        False
-
-        >>> for name, value in variant0:
-        ...     name, value
-        ('name', 'variant0')
-        ('mem_baseaddr', Hex('0x1000'))
-        ('ram_size', Bytes('16 KB'))
-        ('rom_size', None)
-        ('feature', False)
-
-        >>> variant1  = MyConfig('variant1', mem_baseaddr=8*1024, rom_size="2KB", ram_size="4KB", feature=True)
-        >>> variant1
-        MyConfig('variant1', mem_baseaddr=Hex('0x2000'), ram_size=Bytes('4 KB'), rom_size=Bytes('2 KB'), feature=True)
-        >>> variant1.mem_baseaddr
-        Hex('0x2000')
-        >>> variant1.ram_size
-        Bytes('4 KB')
-        >>> variant1.rom_size
-        Bytes('2 KB')
-        >>> variant1.feature
-        True
-
-    To create another variant based on an existing:
-
-    >>> variant2 = variant1.new(name='variant2', rom_size='8KB')
-    >>> variant2
-    MyConfig('variant2', mem_baseaddr=Hex('0x2000'), ram_size=Bytes('4 KB'), rom_size=Bytes('8 KB'), feature=True)
-    >>> variant2.mem_baseaddr
-    Hex('0x2000')
-    >>> variant2.ram_size
-    Bytes('4 KB')
-    >>> variant2.rom_size
-    Bytes('8 KB')
-    >>> variant2.feature
-    True
+    ??? Example "AConfig Examples"
+        Create a Config.
+
+            >>> import ucdp as u
+            >>> class MyConfig(u.AConfig):
+            ...
+            ...     base_addr: u.Hex # required without default
+            ...     ram_size: u.Bytes
+            ...     rom_size: u.Bytes|None = None
+            ...     feature: bool = False
+
+        To create 1st variant
+
+            >>> variant0  = MyConfig(name='variant0', base_addr=4*1024, ram_size='16kB')
+            >>> variant0
+            MyConfig('variant0', base_addr=Hex('0x1000'), ram_size=Bytes('16 KB'))
+            >>> variant0.base_addr
+            Hex('0x1000')
+            >>> variant0.ram_size
+            Bytes('16 KB')
+            >>> variant0.rom_size
+            >>> variant0.feature
+            False
+
+        To create 2nd variant
+
+            >>> for name, value in variant0:
+            ...     name, value
+            ('name', 'variant0')
+            ('base_addr', Hex('0x1000'))
+            ('ram_size', Bytes('16 KB'))
+            ('rom_size', None)
+            ('feature', False)
+
+            >>> variant1  = MyConfig('variant1', base_addr=8*1024, rom_size="2KB", ram_size="4KB", feature=True)
+            >>> variant1
+            MyConfig('variant1', base_addr=Hex('0x2000'), ram_size=Bytes('4 KB'), rom_size=Bytes('2 KB'), feature=True)
+            >>> variant1.base_addr
+            Hex('0x2000')
+            >>> variant1.ram_size
+            Bytes('4 KB')
+            >>> variant1.rom_size
+            Bytes('2 KB')
+            >>> variant1.feature
+            True
+
+        To create another variant based on an existing:
+
+            >>> variant2 = variant1.new(name='variant2', rom_size='8KB')
+            >>> variant2
+            MyConfig('variant2', base_addr=Hex('0x2000'), ram_size=Bytes('4 KB'), rom_size=Bytes('8 KB'), feature=True)
+            >>> variant2.base_addr
+            Hex('0x2000')
+            >>> variant2.ram_size
+            Bytes('4 KB')
+            >>> variant2.rom_size
+            Bytes('8 KB')
+            >>> variant2.feature
+            True
+
+    ???+ bug "Todo"
+        * fix name type
     """
 
     name: str = Field(pattern=PAT_IDENTIFIER)
 
     _posargs: tuple[str, ...] = ("name",)
 
     def __init__(self, name, **kwargs):
@@ -112,83 +121,95 @@
 
 class AUniqueConfig(LightObject):
     """
     A Unique Configuration.
 
     The configuration name is automatically derived from the attribute values.
 
-    >>> import ucdp as u
-    >>> import datetime
-    >>> from typing import Tuple
-    >>> class MyUniqueConfig(u.AUniqueConfig):
-    ...     mem_baseaddr: u.Hex
-    ...     width: int = 32
-    ...     feature: bool = False
-    ...     coeffs: tuple[int, ...] = tuple()
-
-    >>> config = MyUniqueConfig(
-    ...     mem_baseaddr=0x12340000,
-    ... )
-    >>> config.name
-    '5e813dde214238ae'
-
-    >>> for name, value in config:
-    ...     name, value
-    ('mem_baseaddr', Hex('0x12340000'))
-    ('width', 32)
-    ('feature', False)
-    ('coeffs', ())
-
-    >>> config = MyUniqueConfig(
-    ...     mem_baseaddr=0x12340000,
-    ...     coeffs=(1,2,3),
-    ... )
-    >>> config.name
-    '9818217751e9d3b4'
+    ??? Example "AUniqueConfig Examples"
+        Create a Config.
+
+            >>> import ucdp as u
+            >>> import datetime
+            >>> from typing import Tuple
+            >>> class MyUniqueConfig(u.AUniqueConfig):
+            ...     mem_baseaddr: u.Hex
+            ...     width: int = 32
+            ...     feature: bool = False
+            ...     coeffs: tuple[int, ...] = tuple()
+
+            >>> config = MyUniqueConfig(
+            ...     mem_baseaddr=0x12340000,
+            ... )
+            >>> config.name
+            '5e813dde214238ae'
+
+            >>> for name, value in config:
+            ...     name, value
+            ('mem_baseaddr', Hex('0x12340000'))
+            ('width', 32)
+            ('feature', False)
+            ('coeffs', ())
+
+            >>> config = MyUniqueConfig(
+            ...     mem_baseaddr=0x12340000,
+            ...     coeffs=(1,2,3),
+            ... )
+            >>> config.name
+            '9818217751e9d3b4'
     """
 
     @property
     def name(self) -> str:
         """Assembled name from configuration values."""
         return hashlib.sha256(str(self.model_dump()).encode("utf-8")).hexdigest()[:16]
 
 
 BaseConfig = AConfig | AUniqueConfig
+""" BaseConfig """
 
 
 class AVersionConfig(AConfig):
     """
     Version Configuration Container.
 
-    >>> import ucdp as u
-    >>> import datetime
-    >>> class MyVersionConfig(u.AVersionConfig):
-    ...     mem_baseaddr: u.Hex
-
-    >>> version = MyVersionConfig(
-    ...     'my',
-    ...     title="Title",
-    ...     version="1.2.3",
-    ...     timestamp=datetime.datetime(2020, 10, 17, 23, 42),
-    ...     mem_baseaddr=0x12340000
-    ... )
-    >>> version.name
-    'my'
-    >>> version.title
-    'Title'
-    >>> version.timestamp
-    datetime.datetime(2020, 10, 17, 23, 42)
-    >>> version.mem_baseaddr
-    Hex('0x12340000')
-
-    >>> for name, value in version:
-    ...     name, value
-    ('name', 'my')
-    ('title', 'Title')
-    ('version', '1.2.3')
-    ('timestamp', datetime.datetime(2020, 10, 17, 23, 42))
-    ('mem_baseaddr', Hex('0x12340000'))
+    Attributes:
+        title: Title.
+        version: Version
+        timestamp: Timestamp
+
+    ??? Example "AVersionConfig Examples"
+        Create a Config.
+
+            >>> import ucdp as u
+            >>> import datetime
+            >>> class MyVersionConfig(u.AVersionConfig):
+            ...     mem_baseaddr: u.Hex
+
+            >>> version = MyVersionConfig(
+            ...     'my',
+            ...     title="Title",
+            ...     version="1.2.3",
+            ...     timestamp=datetime.datetime(2020, 10, 17, 23, 42),
+            ...     mem_baseaddr=0x12340000
+            ... )
+            >>> version.name
+            'my'
+            >>> version.title
+            'Title'
+            >>> version.timestamp
+            datetime.datetime(2020, 10, 17, 23, 42)
+            >>> version.mem_baseaddr
+            Hex('0x12340000')
+
+            >>> for name, value in version:
+            ...     name, value
+            ('name', 'my')
+            ('title', 'Title')
+            ('version', '1.2.3')
+            ('timestamp', datetime.datetime(2020, 10, 17, 23, 42))
+            ('mem_baseaddr', Hex('0x12340000'))
     """
 
     title: str
     version: str
     timestamp: datetime.datetime
```

### Comparing `ucdp-0.2.0/src/ucdp/consts.py` & `ucdp-0.3.0/src/ucdp/consts.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,11 +24,20 @@
 
 """Constants."""
 
 import re
 from typing import Literal
 
 AUTO: str = "auto"
+""" AUTO. """
+
 PAT_IDENTIFIER: str = r"^[a-zA-Z]([a-zA-Z_0-9]*[a-zA-Z0-9])?$"
+""" PAT_IDENTIFIER. """
+
 RE_IDENTIFIER = re.compile(PAT_IDENTIFIER)
+""" PAT_IDENTIFIER. """
+
 UPWARDS: str = ".."
+""" UPWARDS. """
+
 Gen = Literal["no", "inplace", "full"]
+""" Gen. """
```

### Comparing `ucdp-0.2.0/src/ucdp/dict.py` & `ucdp-0.3.0/src/ucdp/dict.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,55 +29,58 @@
 from typing import Any
 
 from .object import Object, PrivateField
 
 
 class Dict(Object):
     """
-    Re-Implementation of python dictorary, compatible with :any:`Object`.
+    Re-Implementation of python dictorary, compatible with [Object][ucdp.object.Object].
 
-    >>> import ucdp as u
-    >>> data = u.Dict()
-    >>> data
-    Dict()
+    ??? Example "Dictorary Examples"
+        Basics:
 
-    Add items:
+            >>> import ucdp as u
+            >>> data = u.Dict()
+            >>> data
+            Dict()
 
-    >>> data['a'] = 1
-    >>> data['c'] = 3
-    >>> data['b'] = 2
+        Add items:
 
-    Get items:
+            >>> data['a'] = 1
+            >>> data['c'] = 3
+            >>> data['b'] = 2
 
-    >>> data['a']
-    1
-    >>> data['d']
-    Traceback (most recent call last):
-      ...
-    KeyError: 'd'
+        Get items:
 
-    Iteration:
+            >>> data['a']
+            1
+            >>> data['d']
+            Traceback (most recent call last):
+            ...
+            KeyError: 'd'
 
-    >>> tuple(data)
-    ('a', 'c', 'b')
+        Iteration:
 
-    Keys:
+            >>> tuple(data)
+            ('a', 'c', 'b')
 
-    >>> data.keys()
-    dict_keys(['a', 'c', 'b'])
+        Keys:
 
-    Values:
+            >>> data.keys()
+            dict_keys(['a', 'c', 'b'])
 
-    >>> data.values()
-    dict_values([1, 3, 2])
+        Values:
 
-    Key-Value Pairs:
+            >>> data.values()
+            dict_values([1, 3, 2])
 
-    >>> data.items()
-    dict_items([('a', 1), ('c', 3), ('b', 2)])
+        Key-Value Pairs:
+
+            >>> data.items()
+            dict_items([('a', 1), ('c', 3), ('b', 2)])
     """
 
     _items: dict[Any, Any] = PrivateField(default_factory=dict)
 
     def __iter__(self):
         yield from self._items.keys()
```

### Comparing `ucdp-0.2.0/src/ucdp/doc.py` & `ucdp-0.3.0/src/ucdp/doc.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,55 +22,59 @@
 # SOFTWARE.
 #
 
 """
 Documentation Container.
 
 The documentation container unifies and eases the handling of documentation strings.
-Especially :any:`Doc.from_type()` serves the standard approach, to create doc for a type related instance.
+Especially [doc_from_type()][ucdp.docutil.doc_from_type] serves the standard approach,
+to create doc for a type related instance.
 """
 
 from .object import LightObject
 
 
 class Doc(LightObject):
     """
     Documentation Container.
 
     Documentation is always about a title, a long description and an optional source code comment.
-    :any:`Doc` carries all 3 of them.
+    [Doc][ucdp.doc.Doc] carries all 3 of them.
 
-    Keyword Args:
+    Attributes:
         title: Full Spoken Name.
         descr: Documentation Description.
         comment: Source Code Comment. Default is 'title'
 
-    >>> from tabulate import tabulate
-    >>> import ucdp as u
-    >>> docs = (
-    ...     u.Doc(),
-    ...     u.Doc(title='title'),
-    ...     u.Doc(title='title', comment=None),
-    ...     u.Doc(descr='descr'),
-    ...     u.Doc(comment='comment')
-    ... )
-    >>> print(tabulate([(doc, doc.title, doc.descr, doc.comment, doc.comment_or_title) for doc in docs],
-    ...                headers=("Doc()", ".title", ".descr", ".comment", ".comment_or_title")))
-    Doc()                   .title    .descr    .comment    .comment_or_title
-    ----------------------  --------  --------  ----------  -------------------
-    Doc()
-    Doc(title='title')      title                           title
-    Doc(title='title')      title                           title
-    Doc(descr='descr')                descr
-    Doc(comment='comment')                      comment     comment
+    ??? Example "Dictorary Examples"
+        Basics:
 
-    Documentation instances are singleton and share the same memory:
+            >>> from tabulate import tabulate
+            >>> import ucdp as u
+            >>> docs = (
+            ...     u.Doc(),
+            ...     u.Doc(title='title'),
+            ...     u.Doc(title='title', comment=None),
+            ...     u.Doc(descr='descr'),
+            ...     u.Doc(comment='comment')
+            ... )
+            >>> print(tabulate([(doc, doc.title, doc.descr, doc.comment, doc.comment_or_title) for doc in docs],
+            ...                headers=("Doc()", ".title", ".descr", ".comment", ".comment_or_title")))
+            Doc()                   .title    .descr    .comment    .comment_or_title
+            ----------------------  --------  --------  ----------  -------------------
+            Doc()
+            Doc(title='title')      title                           title
+            Doc(title='title')      title                           title
+            Doc(descr='descr')                descr
+            Doc(comment='comment')                      comment     comment
 
-    >>> Doc(title='title') is Doc(title='title')
-    True
+        Documentation instances are singleton and share the same memory:
+
+            >>> Doc(title='title') is Doc(title='title')
+            True
     """
 
     title: str | None = None
     """
     Full Spoken Name.
 
     Identifier are often appreviations.
```

### Comparing `ucdp-0.2.0/src/ucdp/docutil.py` & `ucdp-0.3.0/src/ucdp/docutil.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,36 +28,39 @@
 
 from .doc import Doc
 from .typebase import BaseType
 
 
 def doc_from_type(type_: BaseType, title: str | None = None, descr: str | None = None, comment: str | None = None):
     """
-    Create :any:`Doc` with defaults from `type_`.
+    Create [Doc][ucdp.doc.Doc] with defaults from `type_`.
 
     Args:
         type_: Type to derive from.
 
     Keyword Args:
         title: Full Spoken Name.
         descr: Documentation Description.
         comment: Source Code Comment. Default is 'title'
 
-    >>> import ucdp as u
-    >>> class MyType(u.BitType):
-    ...     title:str = "My Bit Title"
-    ...     comment:str = "My Bit Comment"
-    >>> u.doc_from_type(MyType())
-    Doc(title='My Bit Title', comment='My Bit Comment')
-    >>> u.doc_from_type(MyType(), title="My Title")
-    Doc(title='My Title', comment='My Bit Comment')
-    >>> u.doc_from_type(MyType(), title="My Title", comment="")
-    Doc(title='My Title', comment='')
-    >>> u.doc_from_type(MyType(), comment="My Comment")
-    Doc(title='My Bit Title', comment='My Comment')
+    ??? Example "Dictorary Examples"
+        Basics:
+
+            >>> import ucdp as u
+            >>> class MyType(u.BitType):
+            ...     title:str = "My Bit Title"
+            ...     comment:str = "My Bit Comment"
+            >>> u.doc_from_type(MyType())
+            Doc(title='My Bit Title', comment='My Bit Comment')
+            >>> u.doc_from_type(MyType(), title="My Title")
+            Doc(title='My Title', comment='My Bit Comment')
+            >>> u.doc_from_type(MyType(), title="My Title", comment="")
+            Doc(title='My Title', comment='')
+            >>> u.doc_from_type(MyType(), comment="My Comment")
+            Doc(title='My Bit Title', comment='My Comment')
     """
     # Some kind of optimized default routine
     if title is None:
         title = type_.title
     if descr is None:
         descr = type_.descr
     if comment is None:
```

### Comparing `ucdp-0.2.0/src/ucdp/examples/bad/glbl_bad/__init__.py` & `ucdp-0.3.0/src/ucdp/examples/bad/glbl_bad_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/examples/bad/glbl_bad/regf.py` & `ucdp-0.3.0/src/ucdp/examples/bad/glbl_bad_lib/regf.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/examples/filelist/filelist_lib/filelist.py` & `ucdp-0.3.0/src/ucdp/examples/filelist/filelist_lib/filelist.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/examples/simple/fileliststandard.py` & `ucdp-0.3.0/src/ucdp/examples/simple/fileliststandard.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     filepaths: u.ToPaths = (
         # Path is relative to Module Python File
         # Environment variables are supported too
         # Wildcards are supported. Also in combination with environment variables!
         "../src/{mod.libname}/{mod.topmodname}/{view}/{mod.modname}.sv",
     )
 
+    template_filepaths: u.ToPaths = ("main.mako",)
+
     @staticmethod
     def get_mod_placeholder(mod) -> u.Placeholder:
         """Get Module Placeholder."""
         view = "tb" if mod.is_tb else "rtl"
         return {
             "mod": mod,
             "view": view,
```

### Comparing `ucdp-0.2.0/src/ucdp/examples/simple/glbl/__init__.py` & `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/examples/simple/glbl/bus.py` & `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/bus.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/examples/simple/glbl/clk_gate.py` & `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/clk_gate.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/examples/simple/glbl/regf.py` & `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/regf.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/examples/simple/glbl/regf_tb.py` & `ucdp-0.3.0/src/ucdp/examples/simple/glbl_lib/regf_tb.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/examples/simple/uart/__init__.py` & `ucdp-0.3.0/src/ucdp/examples/simple/uart_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/examples/simple/uart/uart.py` & `ucdp-0.3.0/src/ucdp/examples/simple/uart_lib/uart.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 #
 """UART Example."""
 
 from typing import ClassVar
 
 import ucdp as u  # (1)
 from fileliststandard import HdlFileList
-from glbl.bus import BusType  # (2)
-from glbl.clk_gate import ClkGateMod  # (3)
-from glbl.regf import RegfMod  # (4)
+from glbl_lib.bus import BusType  # (2)
+from glbl_lib.clk_gate import ClkGateMod  # (3)
+from glbl_lib.regf import RegfMod  # (4)
 
 
 class UartIoType(u.AStructType):
     """UART IO."""
 
     title: str = "UART"
     comment: str = "RX/TX"
@@ -50,24 +50,30 @@
 
     def _build(self) -> None:
         self.add_port(u.ClkRstAnType(), "main_i")
         self.add_port(UartIoType(), "uart_i", route="create(u_core/uart_i)")
         self.add_port(BusType(), "bus_i")
 
         clkgate = ClkGateMod(self, "u_clk_gate")
-        clkgate.con("clk_i", "clk_i")
+        clkgate.con("clk_i", "main_clk_i")
         clkgate.con("clk_o", "create(clk_s)")
 
         regf = RegfMod(self, "u_regf")
         regf.con("main_i", "main_i")
         regf.con("bus_i", "bus_i")
 
-        core = u.CoreMod(parent=self, name="u_core")
+        core = UartCoreMod(parent=self, name="u_core")
 
         core.add_port(u.ClkRstAnType(), "main_i")
         core.con("main_clk_i", "clk_s")
-        core.con("main_rst_an_i", "rst_an_i")
+        core.con("main_rst_an_i", "main_rst_an_i")
         core.con("create(regf_i)", "u_regf/regf_o")
 
         word = regf.add_word("ctrl")
         word.add_field("ena", u.EnaType(), is_readable=True, route="u_clk_gate/ena_i")
         word.add_field("strt", u.BitType(), is_writable=True, route="create(u_core/strt_i)")
+
+
+class UartCoreMod(u.ACoreMod):
+    """A Simple UART."""
+
+    filelists: ClassVar[u.ModFileLists] = (HdlFileList(gen="inplace"),)
```

### Comparing `ucdp-0.2.0/src/ucdp/exceptions.py` & `ucdp-0.3.0/src/ucdp/exceptions.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/expr.py` & `ucdp-0.3.0/src/ucdp/expr.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,182 +23,273 @@
 #
 """
 Expression Engine.
 """
 
 import math
 import operator
+import re
 from collections.abc import Callable, Iterator
 
+from icdutil.num import calc_signed_width, calc_unsigned_width, unsigned_to_signed
+from pydantic import ValidationError
+
+from .exceptions import InvalidExpr
 from .object import Field, LightObject, model_validator
 from .slices import Slice
 from .typebase import BaseScalarType, BaseType
-from .typescalar import SintType, UintType
+from .typescalar import BitType, IntegerType, SintType, UintType
 
-# TODO: check for BaseScalarType
+_RE_CONST = re.compile(
+    r"(?P<sign>[-+])?"
+    r"(((?P<width>\d+)'?(?P<is_signed>s)?(?P<bnum>(b[01]+)|(o[0-7]+)|(d[0-9]+)|(h[0-9a-fA-F]+))))|(?P<num>[+-]?\d+)\b"
+)
+_NUM_BASEMAP = {
+    "b": 2,
+    "o": 8,
+    "d": 10,
+    "h": 16,
+    None: 10,
+}
+_OPERMAP = {
+    "<": operator.lt,
+    "<=": operator.le,
+    "==": operator.eq,
+    "!=": operator.ne,
+    ">=": operator.ge,
+    ">": operator.gt,
+    "+": operator.add,
+    "-": operator.sub,
+    "*": operator.mul,
+    "//": operator.floordiv,
+    "%": operator.mod,
+    "**": operator.pow,
+    "<<": operator.lshift,
+    ">>": operator.rshift,
+    "|": operator.or_,
+    "&": operator.and_,
+    "^": operator.xor,
+}
 
 
 class Expr(LightObject):
     """Base Class for all Expressions.
 
     Attributes:
         type_: Type.
     """
 
     type_: BaseType = Field(repr=False)
 
     def __lt__(self, other):
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return BoolOp(self, operator.lt, "<", other)
+        return BoolOp(self, "<", other)
 
     def __le__(self, other):
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return BoolOp(self, operator.le, "<=", other)
+        return BoolOp(self, "<=", other)
 
     def __eq__(self, other):
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return BoolOp(self, operator.eq, "==", other)
+        return BoolOp(self, "==", other)
 
     def __ne__(self, other):
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return BoolOp(self, operator.ne, "!=", other)
+        return BoolOp(self, "!=", other)
 
     def __ge__(self, other):
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return BoolOp(self, operator.ge, ">=", other)
+        return BoolOp(self, ">=", other)
 
     def __gt__(self, other):
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return BoolOp(self, operator.gt, ">", other)
+        return BoolOp(self, ">", other)
 
     def __add__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.add, "+", other)
+        return Op(self, "+", other)
 
     def __sub__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.sub, "-", other)
+        return Op(self, "-", other)
 
     def __mul__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.mul, "*", other)
+        return Op(self, "*", other)
 
     def __floordiv__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.floordiv, "//", other)
+        return Op(self, "//", other)
 
     def __mod__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.mod, "%", other)
+        return Op(self, "%", other)
 
     def __pow__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.pow, "**", other)
+        return Op(self, "**", other)
 
     def __lshift__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.lshift, "<<", other)
+        return Op(self, "<<", other)
 
     def __rshift__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.rshift, ">>", other)
+        return Op(self, ">>", other)
 
     def __or__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.or_, "|", other)
+        return Op(self, "|", other)
 
     def __and__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.and_, "&", other)
+        return Op(self, "&", other)
 
     def __xor__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(self, operator.xor, "^", other)
+        return Op(self, "^", other)
 
     def __radd__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.add, "+", self)
+        return Op(other, "+", self)
 
     def __rsub__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.sub, "-", self)
+        return Op(other, "-", self)
 
     def __rmul__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.mul, "*", self)
+        return Op(other, "*", self)
 
     def __rfloordiv__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.floordiv, "//", self)
+        return Op(other, "//", self)
 
     def __rmod__(self, other) -> "Op":
-        return Op(other, operator.mod, "%", self)
+        return Op(other, "%", self)
 
     def __rpow__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.pow, "**", self)
+        return Op(other, "**", self)
 
     def __rlshift__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.lshift, "<<", self)
+        return Op(other, "<<", self)
 
     def __rrshift__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.rshift, ">>", self)
+        return Op(other, ">>", self)
 
     def __ror__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.or_, "|", self)
+        return Op(other, "|", self)
 
     def __rand__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.and_, "&", self)
+        return Op(other, "&", self)
 
     def __rxor__(self, other) -> "Op":
+        if isinstance(other, int):
+            other = _parse_const(other, reftype=self.type_)
         if not isinstance(other, Expr):
             return NotImplemented
-        return Op(other, operator.xor, "^", self)
+        return Op(other, "^", self)
 
     def __abs__(self) -> "SOp":
         return SOp(oper=operator.abs, sign="abs(", one=self, postsign=")")
 
     def __invert__(self) -> "SOp":
         return SOp(oper=operator.inv, sign="~", one=self)
 
     def __neg__(self) -> "SOp":
         return SOp(oper=operator.neg, sign="-", one=self)
 
     def __getitem__(self, slice_):
-        slice_ = Slice.cast(slice_)
+        if isinstance(slice_, Expr):
+            slice_ = Slice(left=slice_, right=slice_)
+        else:
+            slice_ = Slice.cast(slice_)
         return SliceOp(one=self, slice_=slice_)
 
 
 class Op(Expr):
     """Dual Operator Expression.
 
     Args:
@@ -217,15 +308,16 @@
     left: Expr
     oper: Callable = Field(repr=False)
     sign: str
     right: Expr
 
     _posargs: tuple[str, ...] = ("left", "sign", "right")
 
-    def __init__(self, left: Expr, oper: Callable, sign: str, right: Expr):
+    def __init__(self, left: Expr, sign: str, right: Expr):
+        oper = _OPERMAP[sign]
         super().__init__(left=left, oper=oper, sign=sign, right=right, type_=left.type_)  # type: ignore[call-arg]
 
     def __int__(self):
         return int(self.oper(int(self.left), int(self.right)))
 
 
 class BoolOp(Op):
@@ -261,20 +353,20 @@
         type_: Type.
 
     ???+ bug "Todo"
         * fix inherited_members / Attributes Types
 
     """
 
-    oper: Callable = Field(repr=False)
+    oper: Callable
     sign: str
     one: Expr
     postsign: str = ""
 
-    _posargs: tuple[str, ...] = ("sign", "one")
+    _posargs: tuple[str, ...] = ("sign", "oper", "one")
 
     def __init__(self, oper: Callable, sign: str, one: Expr, postsign: str = ""):
         super().__init__(oper=oper, sign=sign, one=one, postsign=postsign, type_=one.type_)  # type: ignore[call-arg]
 
     def __int__(self):
         return self.oper(int(self.one))
 
@@ -578,7 +670,56 @@
 
     @model_validator(mode="after")
     def __post_init(self) -> "RangeExpr":
         values = tuple(self.range_)
         self.type_.check(values[0], what="Start Value")
         self.type_.check(values[-1], what="End Value")
         return self
+
+
+def _parse_const(value, reftype: BaseType | None = None) -> ConstExpr:
+    strippedvalue = str(value).strip()
+    matnum = _RE_CONST.fullmatch(strippedvalue)
+    if matnum:
+        return __parse_const(reftype=reftype, **matnum.groupdict())
+    raise InvalidExpr(repr(value))
+
+
+def __parse_const(sign, width, is_signed, bnum, num, reftype) -> ConstExpr:
+    # Bin/Oct/Dec/Hex Number with given width
+    if num is None:
+        base, num = bnum[0], bnum[1:]
+        value = int(num, _NUM_BASEMAP[base])
+        if sign == "-":
+            value = -value
+        width = int(width)
+        type_: BaseType
+        if base == "b" and width == 1 and not is_signed:
+            type_ = BitType(default=value)
+        elif is_signed:
+            if value > 0:
+                value = unsigned_to_signed(value, width)
+            type_ = SintType(width, default=value)
+        else:
+            type_ = UintType(width, default=value)
+        return ConstExpr(type_)
+
+    # width-less integer
+    intnum = int(num)
+    if reftype is not None:
+        try:
+            return ConstExpr(reftype.new(default=intnum))
+        except ValidationError:
+            pass
+
+    # Integer
+    if IntegerType.min_ <= intnum <= IntegerType.max_:
+        return ConstExpr(IntegerType(default=intnum))
+
+    # signed vector
+    if intnum < 0:
+        width = calc_signed_width(intnum)
+        return ConstExpr(SintType(width, default=intnum))
+
+    # unsigned vector
+    width = calc_unsigned_width(intnum)
+    return ConstExpr(UintType(width, default=intnum))
```

### Comparing `ucdp-0.2.0/src/ucdp/exprparser.py` & `ucdp-0.3.0/src/ucdp/exprparser.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,96 +18,87 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """
-Expression ExprParser.
+Expression Parser.
 """
 
-import re
+from functools import cached_property
 from typing import Any
 
-from icdutil.num import calc_signed_width, unsigned_to_signed
-
 from .consts import RE_IDENTIFIER
 from .exceptions import InvalidExpr
 from .expr import (
     BoolOp,
     ConcatExpr,
     ConstExpr,
     Expr,
     Log2Expr,
     MaximumExpr,
     MinimumExpr,
     Op,
     SliceOp,
     SOp,
     TernaryExpr,
+    _parse_const,
 )
 from .namespace import Namespace
 from .note import Note
 from .object import Object, computed_field
 from .typebase import BaseType
 from .typeenum import BaseEnumType
-from .typescalar import BitType, BoolType, SintType, UintType
+from .typescalar import BitType, BoolType, UintType
 
-_RE_CONST = re.compile(
-    r"(?P<sign>[-+])?"
-    r"(((?P<width>\d+)'?(?P<is_signed>s)?(?P<bnum>(b[01]+)|(o[0-7]+)|(d[0-9]+)|(h[0-9a-fA-F]+))))|(?P<num>\d+)\b"
-)
-_NUM_BASEMAP = {
-    "b": 2,
-    "o": 8,
-    "d": 10,
-    "h": 16,
-    None: 10,
-}
 Parseable = Expr | str | int | BaseType | list | tuple
 Constable = int | str | ConstExpr
 Concatable = list | tuple | ConcatExpr
 
 
 class _Globals(dict):
-    def __init__(self, globals: dict, namespace: Namespace | None, strict: bool):
+    def __init__(self, globals: dict, namespace: Namespace | None, strict: bool, context: str | None):
         super().__init__(globals)
         self.namespace = namespace
         self.strict = strict
+        self.context = context
 
     def __missing__(self, key):
         if self.namespace:
             if self.strict:
                 try:
                     return self.namespace.get_dym(key)
                 except ValueError as err:
-                    raise NameError(err) from None
+                    raise NameError(f"{self.context}: {err}") from None
             try:
                 return self.namespace[key]
             except ValueError:
                 pass
         if self.strict:
             raise KeyError(key)
         return key
 
 
 class ExprParser(Object):
     """
     ExprParser.
 
-    Keyword Args:
+    Attributes:
         namespace (Namespace): Symbol namespace
         strict: Do not ignore missing symbols.
 
     """
 
     namespace: Namespace | None = None
     strict: bool = True
+    context: str | None = None
 
     @computed_field
+    @cached_property
     def _globals(self) -> _Globals:
         globals_ = {
             # Expressions
             "Op": Op,
             "SOp": SOp,
             "BoolOp": BoolOp,
             "SliceOp": SliceOp,
@@ -121,15 +112,15 @@
             "const": self.const,
             "concat": self.concat,
             "ternary": self.ternary,
             "log2": self.log2,
             "minimum": self.minimum,
             "maximum": self.maximum,
         }
-        return _Globals(globals=globals_, namespace=self.namespace, strict=self.strict)
+        return _Globals(globals=globals_, namespace=self.namespace, strict=self.strict, context=self.context)
 
     def parse_note(self, expr: Parseable | Note, only=None, types=None) -> Expr | Note:
         """
         Parse Expression or Note.
 
         Args:
             expr: Expression
@@ -150,56 +141,59 @@
         Args:
             expr: Expression
 
         Keyword Args:
             only: Limit expression to these final element type.
             types: Limit expression type to to these types.
 
-        >>> import ucdp as u
-        >>> p = u.ExprParser()
-        >>> p.parse(10)
-        ConstExpr(UintType(5, default=10))
-        >>> p.parse('3h3')
-        ConstExpr(UintType(3, default=3))
-        >>> p.parse('3h3') * p.const(2)
-        Op(ConstExpr(UintType(3, default=3)), '*', ConstExpr(UintType(3, default=2)))
-        >>> p.parse((10, '10'))
-        ConcatExpr((ConstExpr(UintType(5, default=10)), ConstExpr(UintType(5, default=10))))
-        >>> p = u.ExprParser(namespace=u.Idents([
-        ...     u.Signal(u.UintType(16, default=15), 'uint_s'),
-        ...     u.Signal(u.SintType(16, default=-15), 'sint_s'),
-        ... ]))
-        >>> expr = p.parse('uint_s[2]')
-        >>> expr
-        SliceOp(Signal(UintType(16, default=15), 'uint_s'), Slice('2'))
-        >>> expr = p.parse('uint_s * sint_s[2:1]')
-        >>> expr
-        Op(Signal(UintType(16, default=15), 'uint_s'), '*', SliceOp(Signal(SintType(16, ...), 'sint_s'), Slice('2:1')))
-        >>> int(expr)
-        0
-
-        A more complex:
-
-        >>> namespace = u.Idents([
-        ...     u.Signal(u.UintType(2), 'a_s'),
-        ...     u.Signal(u.UintType(4), 'b_s'),
-        ...     u.Signal(u.SintType(8), 'c_s'),
-        ...     u.Signal(u.SintType(16), 'd_s'),
-        ... ])
-        >>> p = u.ExprParser(namespace=namespace)
-        >>> expr = p.parse("ternary(b_s == const('4h3'), a_s, c_s)")
-        >>> expr
-        TernaryExpr(BoolOp(Signal(UintType(4), 'b_s'), '==', ..., Signal(SintType(8), 'c_s'))
-
-        Syntax Errors:
-
-        >>> parse("sig_s[2")  # doctest: +SKIP
-        Traceback (most recent call last):
-        ...
-        u.exceptions.InvalidExpr: 'sig_s[2': '[' was never closed (<string>, line 1)
+        ??? Example "Expression Parser Examples"
+            Basics:
+
+                >>> import ucdp as u
+                >>> p = u.ExprParser()
+                >>> p.parse(10)
+                ConstExpr(IntegerType(default=10))
+                >>> p.parse('3h3')
+                ConstExpr(UintType(3, default=3))
+                >>> p.parse('3h3') * p.const(2)
+                Op(ConstExpr(UintType(3, default=3)), '*', ConstExpr(IntegerType(default=2)))
+                >>> p.parse((10, '10'))
+                ConcatExpr((ConstExpr(IntegerType(default=10)), ConstExpr(IntegerType(default=10))))
+                >>> p = u.ExprParser(namespace=u.Idents([
+                ...     u.Signal(u.UintType(16, default=15), 'uint_s'),
+                ...     u.Signal(u.SintType(16, default=-15), 'sint_s'),
+                ... ]))
+                >>> expr = p.parse('uint_s[2]')
+                >>> expr
+                SliceOp(Signal(UintType(16, default=15), 'uint_s'), Slice('2'))
+                >>> expr = p.parse('uint_s * sint_s[2:1]')
+                >>> expr
+                Op(Signal(UintType(16, ...), 'uint_s'), '*', SliceOp(Signal(SintType(16, ...), 'sint_s'), Slice('2:1')))
+                >>> int(expr)
+                0
+
+            A more complex:
+
+                >>> namespace = u.Idents([
+                ...     u.Signal(u.UintType(2), 'a_s'),
+                ...     u.Signal(u.UintType(4), 'b_s'),
+                ...     u.Signal(u.SintType(8), 'c_s'),
+                ...     u.Signal(u.SintType(16), 'd_s'),
+                ... ])
+                >>> p = u.ExprParser(namespace=namespace)
+                >>> expr = p.parse("ternary(b_s == const('4h3'), a_s, c_s)")
+                >>> expr
+                TernaryExpr(BoolOp(Signal(UintType(4), 'b_s'), '==', ..., Signal(SintType(8), 'c_s'))
+
+                Syntax Errors:
+
+                >>> parse("sig_s[2")  # doctest: +SKIP
+                Traceback (most recent call last):
+                ...
+                u.exceptions.InvalidExpr: 'sig_s[2': '[' was never closed (<string>, line 1)
         """
         result: Expr
         if isinstance(expr, Expr):
             result = expr
         elif isinstance(expr, BaseType):
             result = ConstExpr(expr)
         else:
@@ -241,147 +235,137 @@
         except SyntaxError as exc:
             raise InvalidExpr(f"{expr!r}: {exc!s}") from None
 
     def const(self, value: Constable) -> ConstExpr:
         """
         Parse Constant.
 
-        >>> import ucdp as u
-        >>> p = u.ExprParser()
-        >>> p.const('10')
-        ConstExpr(UintType(5, default=10))
-        >>> p.const(10)
-        ConstExpr(UintType(5, default=10))
-        >>> p.const("10'd20")
-        ConstExpr(UintType(10, default=20))
-        >>> p.const(ConstExpr(UintType(10, default=20)))
-        ConstExpr(UintType(10, default=20))
-        >>> p.const("4'h4")
-        ConstExpr(UintType(4, default=4))
-        >>> p.const("4'sh4")
-        ConstExpr(SintType(4, default=4))
-        >>> p.const("4'shC")
-        ConstExpr(SintType(4, default=-4))
+        ??? Example "Parser Example"
+            Basics:
+
+                >>> import ucdp as u
+                >>> p = u.ExprParser()
+                >>> p.const('10')
+                ConstExpr(IntegerType(default=10))
+                >>> p.const(10)
+                ConstExpr(IntegerType(default=10))
+                >>> p.const("10'd20")
+                ConstExpr(UintType(10, default=20))
+                >>> p.const(ConstExpr(UintType(10, default=20)))
+                ConstExpr(UintType(10, default=20))
+                >>> p.const("4'h4")
+                ConstExpr(UintType(4, default=4))
+                >>> p.const("4'sh4")
+                ConstExpr(SintType(4, default=4))
+                >>> p.const("4'shC")
+                ConstExpr(SintType(4, default=-4))
         """
         if isinstance(value, ConstExpr):
             return value
-        strippedvalue = str(value).strip()
-        matnum = _RE_CONST.fullmatch(strippedvalue)
-        if matnum:
-            return self._parse_const(**matnum.groupdict())
-        raise InvalidExpr(repr(value))
-
-    @staticmethod
-    def _parse_const(sign, width, is_signed, bnum, num) -> ConstExpr:
-        if num is None:
-            base, num = bnum[0], bnum[1:]
-            value = int(num, _NUM_BASEMAP[base])
-            if sign == "-":
-                value = -value
-            width = int(width)
-            type_: BaseType
-            if base == "b" and width == 1 and not is_signed:
-                type_ = BitType(default=value)
-            elif is_signed:
-                if value > 0:
-                    value = unsigned_to_signed(value, width)
-                type_ = SintType(width, default=value)
-            else:
-                type_ = UintType(width, default=value)
-            return ConstExpr(type_)
-        intnum = int(num)
-        width = calc_signed_width(intnum)
-        return ConstExpr(UintType(width, default=intnum))
+        return _parse_const(value)
 
     def concat(self, value: Concatable) -> ConcatExpr:
         """
         Parse ConcatExpr.
 
-        >>> import ucdp as u
-        >>> p = u.ExprParser()
-        >>> p.concat((10, "20"))
-        ConcatExpr((ConstExpr(UintType(5, default=10)), ConstExpr(UintType(6, default=20))))
-        >>> p.concat(ConcatExpr((ConstExpr(UintType(5, default=10)), ConstExpr(UintType(6, default=20)))))
-        ConcatExpr((ConstExpr(UintType(5, default=10)), ConstExpr(UintType(6, default=20))))
+        ??? Example "Concat Parser Example"
+            Basics:
+
+                >>> import ucdp as u
+                >>> p = u.ExprParser()
+                >>> p.concat((10, "20"))
+                ConcatExpr((ConstExpr(IntegerType(default=10)), ConstExpr(IntegerType(default=20))))
 
-        >>> bool(p.concat((10, "20")))
-        True
+                >>> bool(p.concat((10, "20")))
+                True
         """
         if isinstance(value, ConcatExpr):
             return value
         return ConcatExpr(tuple(self.parse(item) for item in value))
 
     def ternary(self, cond: Parseable, one: Parseable, other: Parseable) -> TernaryExpr:
         """
         TernaryExpr Statement.
 
-        >>> import ucdp as u
-        >>> cond = u.Signal(u.UintType(2), 'if_s') == u.ConstExpr(UintType(2, default=1))
-        >>> one = u.Signal(u.UintType(16, default=10), 'one_s')
-        >>> other = u.Signal(u.UintType(16, default=20), 'other_s')
-        >>> p = u.ExprParser()
-        >>> expr = p.ternary(cond, one, other)
-        >>> expr
-        TernaryExpr(BoolOp(Signal(UintType(2), 'if_s'), '==', ..., Signal(UintType(16, default=20), 'other_s'))
-        >>> int(expr)
-        20
-        >>> expr.type_
-        UintType(16, default=10)
+        ??? Example "Ternary Parser Example"
+            Basics:
+
+                >>> import ucdp as u
+                >>> cond = u.Signal(u.UintType(2), 'if_s') == u.ConstExpr(UintType(2, default=1))
+                >>> one = u.Signal(u.UintType(16, default=10), 'one_s')
+                >>> other = u.Signal(u.UintType(16, default=20), 'other_s')
+                >>> p = u.ExprParser()
+                >>> expr = p.ternary(cond, one, other)
+                >>> expr
+                TernaryExpr(BoolOp(Signal(UintType(2), 'if_s'), '==', ..., Signal(UintType(16, default=20), 'other_s'))
+                >>> int(expr)
+                20
+                >>> expr.type_
+                UintType(16, default=10)
         """
         condp: BoolOp = self.parse(cond, only=BoolOp)  # type:ignore[assignment]
         onep = self.parse(one)
         otherp = self.parse(other)
         return TernaryExpr(cond=condp, one=onep, other=otherp)
 
     def log2(self, expr: Parseable):
         """
         Ceiling Logarithm to base of 2.
 
-        >>> import ucdp as u
-        >>> p = u.ExprParser()
-        >>> log = p.log2("8'h8")
-        >>> log
-        Log2Expr(ConstExpr(UintType(8, default=8)))
-        >>> int(log)
-        3
-        >>> p.parse("log2('8h8')")
-        Log2Expr(ConstExpr(UintType(8, default=8)))
+        ??? Example "Log2 Parser Example"
+            Basics:
+
+                >>> import ucdp as u
+                >>> p = u.ExprParser()
+                >>> log = p.log2("8'h8")
+                >>> log
+                Log2Expr(ConstExpr(UintType(8, default=8)))
+                >>> int(log)
+                3
+                >>> p.parse("log2('8h8')")
+                Log2Expr(ConstExpr(UintType(8, default=8)))
         """
         return Log2Expr(self.parse(expr))
 
     def minimum(self, *items):
         """
         Lower value of `one` and `other`.
 
-        >>> import ucdp as u
-        >>> p = u.ExprParser()
-        >>> val = p.minimum("8'h8", "8'h3")
-        >>> val
-        MinimumExpr((ConstExpr(UintType(8, default=8)), ConstExpr(UintType(8, default=3))))
-        >>> int(val)
-        3
-        >>> p.parse("minimum('8h8', '8h3')")
-        MinimumExpr((ConstExpr(UintType(8, default=8)), ConstExpr(UintType(8, default=3))))
+        ??? Example "Minimum Parser Example"
+            Basics:
+
+                >>> import ucdp as u
+                >>> p = u.ExprParser()
+                >>> val = p.minimum("8'h8", "8'h3")
+                >>> val
+                MinimumExpr((ConstExpr(UintType(8, default=8)), ConstExpr(UintType(8, default=3))))
+                >>> int(val)
+                3
+                >>> p.parse("minimum('8h8', '8h3')")
+                MinimumExpr((ConstExpr(UintType(8, default=8)), ConstExpr(UintType(8, default=3))))
         """
         parsed = tuple(self.parse(item) for item in items)
         return MinimumExpr(parsed)
 
     def maximum(self, *items):
         """
         Higher value of `one` and `other`.
 
-        >>> import ucdp as u
-        >>> p = u.ExprParser()
-        >>> val = p.maximum("8'h8", "8'h3")
-        >>> val
-        MaximumExpr((ConstExpr(UintType(8, default=8)), ConstExpr(UintType(8, default=3))))
-        >>> int(val)
-        8
-        >>> p.parse("maximum('8h8', '8h3')")
-        MaximumExpr((ConstExpr(UintType(8, default=8)), ConstExpr(UintType(8, default=3))))
+        ??? Example "Maximum Parser Example"
+            Basics:
+
+                >>> import ucdp as u
+                >>> p = u.ExprParser()
+                >>> val = p.maximum("8'h8", "8'h3")
+                >>> val
+                MaximumExpr((ConstExpr(UintType(8, default=8)), ConstExpr(UintType(8, default=3))))
+                >>> int(val)
+                8
+                >>> p.parse("maximum('8h8', '8h3')")
+                MaximumExpr((ConstExpr(UintType(8, default=8)), ConstExpr(UintType(8, default=3))))
         """
         parsed = tuple(self.parse(item) for item in items)
         return MaximumExpr(parsed)
 
 
 def cast_booltype(expr):
     """Cast to Boolean."""
```

### Comparing `ucdp-0.2.0/src/ucdp/filelistparser.py` & `ucdp-0.3.0/src/ucdp/filelistparser.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,65 +26,108 @@
 
 import re
 from collections.abc import Iterable
 from pathlib import Path
 
 from .logging import LOGGER
 from .object import Object
-from .pathutil import improved_resolve, use_envvars
+from .pathutil import improved_resolve
 
 _RE_COMMENT = re.compile(r"\A(.*?)(\s*(#|//).*)\Z")
 _RE_FILELIST = re.compile(r"\A-([fF])\s+(.*?)\Z")
 _RE_INCDIR = re.compile(r'\A[+\-]incdir[+\-\s]"?(?P<incdir>.*?)"?\Z')
 _RE_FILE = re.compile(r"\A((-sv|-v)\s+)?(?P<filepath>[^+-].*?)\Z")
 
 
 class FileListParser(Object):
     """File List Parser."""
 
-    envvarnames: tuple[str, ...] = ()
+    def parse_file(  # type: ignore[override]
+        self,
+        filepaths: list[Path],
+        inc_dirs: list[Path],
+        filepath: Path,
+        replace_envvars: bool = False,
+    ):
+        """Read File List File.
+
+        Args:
+            filepaths: File Paths Container.
+            inc_dirs: Include Directories Container.
+            filepath: File to be parsed.
+            replace_envvars: Resolve Environment Variables.
+        """
+        with filepath.open(encoding="utf-8") as file:
+            basepath = filepath.parent
+            self.parse(filepaths, inc_dirs, basepath, file)
 
-    def parse_file(self, filepaths: list[Path], incdirs: list[Path], filepath: Path):  # type: ignore[override]
-        """Read File List File."""
         with filepath.open(encoding="utf-8") as file:
             basepath = filepath.parent
-            self.parse(filepaths, incdirs, basepath, file)
+            self.parse(filepaths, inc_dirs, basepath, file, replace_envvars=replace_envvars, context=str(filepath))
 
-    def parse(self, filepaths: list[Path], incdirs: list[Path], basedir: Path, items: Iterable[str | Path]):
-        """File List File."""
-        for item in items:
+    def parse(
+        self,
+        filepaths: list[Path],
+        inc_dirs: list[Path],
+        basedir: Path,
+        items: Iterable[str | Path],
+        replace_envvars: bool = False,
+        context: str = "",
+    ):
+        """File List File.
+
+        Args:
+            filepaths: File Paths Container.
+            inc_dirs: Include Directories Container.
+            basedir: Base Directory for Relative Paths.
+            items: Items to be parsed.
+            replace_envvars: Resolve Environment Variables.
+            context: Context for error reporting.
+        """
+        for lineno, item in enumerate(items, 1):
             line = str(item).strip()
             # comment
             mat = _RE_COMMENT.match(line)
             if mat:
                 line = mat.group(1).strip()
             if not line:
                 continue
             # -f
             mat = _RE_FILELIST.match(line)
             if mat:
                 filelistpath = self.resolve(basedir, Path(mat.group(2)))
-                self.parse_file(filepaths, incdirs, filelistpath)
+                self.parse_file(filepaths, inc_dirs, filelistpath)
                 continue
             # -incdir
             mat = _RE_INCDIR.match(line)
             if mat:
-                incdir = self.normalize(basedir, Path(mat.group("incdir")))
-                if incdir not in incdirs:
-                    incdirs.append(incdir)
+                incdir = self.normalize(basedir, Path(mat.group("incdir")), replace_envvars)
+                if incdir not in inc_dirs:
+                    inc_dirs.append(incdir)
                 continue
             # file
             mat = _RE_FILE.match(line)
             if mat:
-                filepath = self.normalize(basedir, Path(mat.group("filepath")))
+                filepath = self.normalize(basedir, Path(mat.group("filepath")), replace_envvars)
                 if filepath not in filepaths:
                     filepaths.append(filepath)
                 continue
-            LOGGER.warning("Cannot parse %s", line)
+            LOGGER.warning("%s:%d Cannot parse %s", context, lineno, line)
 
     def resolve(self, basedir: Path, path: Path) -> Path:
-        """Return Valid Filepath With Resolved Environment Variables."""
+        """Return Valid Filepath With Resolved Environment Variables.
+
+        Args:
+            basedir: Base Directory.
+            path: Path.
+        """
         return improved_resolve(path, basedir=basedir, replace_envvars=True, strict=True)
 
-    def normalize(self, basedir: Path, path: Path) -> Path:
-        """Return Normalized Filepaths for File List."""
-        return use_envvars(improved_resolve(path, basedir=basedir), self.envvarnames)
+    def normalize(self, basedir: Path, path: Path, replace_envvars: bool) -> Path:
+        """Return Normalized Filepaths for File List.
+
+        Args:
+            basedir: Base Directory.
+            path: Path.
+            replace_envvars: Resolve Environment Variables.
+        """
+        return improved_resolve(path, basedir=basedir, replace_envvars=replace_envvars)
```

### Comparing `ucdp-0.2.0/src/ucdp/fileset.py` & `ucdp-0.3.0/src/ucdp/fileset.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,58 +29,64 @@
 from .filelistparser import FileListParser
 from .modbase import BaseMod
 from .modfilelist import Paths, iter_modfilelists
 from .object import LightObject, Object
 
 
 class LibPath(LightObject):
-    """Library and File Path."""
+    """
+    Library and File Path.
+
+    Attributes:
+        libname: Library Name
+        path: Path
+    """
 
     libname: str
     path: Path
 
 
 class FileSet(Object):
     """
     Module File List.
 
     Attributes:
         target: Target
         filepaths: Source Files
-        incdirs: Include Files
+        inc_dirs: Include Directories
     """
 
     target: str | None = None
     filepaths: tuple[LibPath, ...]
-    incdirs: tuple[Path, ...]
+    inc_dirs: tuple[Path, ...]
 
     @staticmethod
     def from_mod(
         topmod: BaseMod, name: str, target: str | None = None, filelistparser: FileListParser | None = None
     ) -> "FileSet":
         """Create ``FileSet` for ``mod``."""
         filepaths: list[LibPath] = []
-        incdirs: list[Path] = []
+        inc_dirs: list[Path] = []
         for mod, modfilelist in iter_modfilelists(topmod, name, target=target, filelistparser=filelistparser):
             libname = mod.libname
-            _process(filepaths, incdirs, libname, modfilelist.dep_filepaths, modfilelist.dep_incdirs)  # type: ignore[arg-type]
-            _process(filepaths, incdirs, libname, modfilelist.filepaths, modfilelist.incdirs)  # type: ignore[arg-type]
+            _process(filepaths, inc_dirs, libname, modfilelist.dep_filepaths, modfilelist.dep_inc_dirs)  # type: ignore[arg-type]
+            _process(filepaths, inc_dirs, libname, modfilelist.filepaths, modfilelist.inc_dirs)  # type: ignore[arg-type]
 
-        return FileSet(target=target, filepaths=tuple(filepaths), incdirs=tuple(incdirs))
+        return FileSet(target=target, filepaths=tuple(filepaths), inc_dirs=tuple(inc_dirs))
 
 
 def _process(
     filepaths: list[LibPath],
-    incdirs: list[Path],
+    inc_dirs: list[Path],
     libname: str,
     add_filepaths: Paths | None,
-    add_incdirs: Paths | None,
+    add_inc_dirs: Paths | None,
 ):
-    # incdir
-    for incdir in add_incdirs or []:
-        if incdir not in incdirs:
-            incdirs.append(incdir)
+    # inc_dir
+    for inc_dir in add_inc_dirs or []:
+        if inc_dir not in inc_dirs:
+            inc_dirs.append(inc_dir)
     # filepath
     for filepath in add_filepaths or []:
         libpath = LibPath(libname=libname, path=Path(filepath))
         if libpath not in filepaths:
             filepaths.append(libpath)
```

### Comparing `ucdp-0.2.0/src/ucdp/flipflop.py` & `ucdp-0.3.0/src/ucdp/flipflop.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,23 @@
 from .expr import BoolOp
 from .object import model_validator
 from .signal import BaseSignal
 from .typeclkrst import ClkType, RstAnType
 
 
 class FlipFlop(Assigns):
-    """FlipFlop."""
+    """FlipFlop.
+
+    Attributes:
+        clk: Clock
+        rst_an: Reset (low active)
+        rst: Reset
+        ena: Enable
+
+    """
 
     clk: BaseSignal
     rst_an: BaseSignal
     rst: BoolOp | None = None
     ena: BoolOp | None = None
 
     @model_validator(mode="after")
```

### Comparing `ucdp-0.2.0/src/ucdp/humannum.py` & `ucdp-0.3.0/src/ucdp/humannum.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-"""Configuration."""
+"""Human Friendly Numbers."""
 
 from typing import Annotated
 
 import humannum
 from pydantic import (
     BeforeValidator,
     PlainSerializer,
@@ -34,20 +34,24 @@
 
 Hex = Annotated[
     humannum.Hex,
     BeforeValidator(lambda x: humannum.hex_(x)),
     PlainSerializer(lambda x: str(x), return_type=str),
     WithJsonSchema({"type": "string"}, mode="serialization"),
 ]
+"""Hex. """
 
 Bytes = Annotated[
     humannum.Bytes,
     BeforeValidator(lambda x: humannum.bytes_(x)),
     PlainSerializer(lambda x: str(x), return_type=str),
     WithJsonSchema({"type": "string"}, mode="serialization"),
 ]
+"""Bytes. """
+
 Bin = Annotated[
     humannum.Bin,
     BeforeValidator(lambda x: humannum.bin_(x)),
     PlainSerializer(lambda x: str(x), return_type=str),
     WithJsonSchema({"type": "string"}, mode="serialization"),
 ]
+"""Bin. """
```

### Comparing `ucdp-0.2.0/src/ucdp/ident.py` & `ucdp-0.3.0/src/ucdp/ident.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
             except IndexError:
                 break
 
             if stop and stop(ident):
                 break
 
             type_ = ident.type_
-            assert value is None, "TODO"
+            # assert value is None, "TODO"
 
             if not filter_ or filter_(ident):
                 yield ident
             if isinstance(type_, BaseStructType):
                 for structitem in reversed(type_.values()):
                     direction = ident.direction and ident.direction * structitem.orientation
                     suffix = (direction and direction.suffix) or ident.suffix
```

### Comparing `ucdp-0.2.0/src/ucdp/iterutil.py` & `ucdp-0.3.0/src/ucdp/iterutil.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,77 +41,90 @@
 Names = Iterable[str] | str
 
 
 def split(items: Names, seps: str = ";") -> tuple[str, ...]:
     """
     Split items into tuple.
 
-    >>> split(['abc', 'def'])
-    ('abc', 'def')
-    >>> split(('abc', 'def'))
-    ('abc', 'def')
-    >>> split('abc; def')
-    ('abc', 'def')
-    >>> split('ab;c, def', seps=",")
-    ('ab;c', 'def')
-
-    Generators are also handled:
-
-    >>> def func():
-    ...     yield 'abc'
-    ...     yield 'def'
-    >>> split(func())
-    ('abc', 'def')
-
-    Empty strings or `None` just result in an empty tuple:
-
-    >>> split("")
-    ()
-    >>> split(None)
-    ()
+    Args:
+        items: Items.
+        seps: Separator
+
+    ??? Example "Split Examples"
+        Basics:
+
+            >>> split(['abc', 'def'])
+            ('abc', 'def')
+            >>> split(('abc', 'def'))
+            ('abc', 'def')
+            >>> split('abc; def')
+            ('abc', 'def')
+            >>> split('ab;c, def', seps=",")
+            ('ab;c', 'def')
+
+        Generators are also handled:
+
+            >>> def func():
+            ...     yield 'abc'
+            ...     yield 'def'
+            >>> split(func())
+            ('abc', 'def')
+
+        Empty strings or `None` just result in an empty tuple:
+
+            >>> split("")
+            ()
+            >>> split(None)
+            ()
     """
     if not items:
         items = []
     elif isinstance(items, str):
         items = [item.strip() for item in _translate(seps).split(items)]
     return tuple(items)
 
 
 def namefilter(namepats: Names):
     """
     Create filter for namepats.
 
-    >>> import ucdp as u
-    >>> def myfunc(items, filter_=None):
-    ...     for item in items:
-    ...         if not filter_ or filter_(item):
-    ...             print(item)
-
-    >>> items = ('abc', 'cde', 'efg')
-    >>> myfunc(items)
-    abc
-    cde
-    efg
-    >>> myfunc(items, filter_=u.namefilter(''))
-    abc
-    cde
-    efg
-    >>> myfunc(items, filter_=u.namefilter('cde; tuv'))
-    cde
-    >>> myfunc(items, filter_=u.namefilter('*c*'))
-    abc
-    cde
-    >>> myfunc(items, filter_=u.namefilter('!*c*'))
-    efg
-    >>> myfunc(items, filter_=u.namefilter('*c*; !*e'))
-    abc
-
-    >>> items = ['abc', 'cde', 'efg']
-    >>> myfunc(items, filter_=u.namefilter('*c*; !*e'))
-    abc
+    Args:
+        namepats: Name Filter Pattern.
+
+    ??? Example "Namefilter Examples"
+        Basics:
+
+            >>> import ucdp as u
+            >>> def myfunc(items, filter_=None):
+            ...     for item in items:
+            ...         if not filter_ or filter_(item):
+            ...             print(item)
+
+            >>> items = ('abc', 'cde', 'efg')
+            >>> myfunc(items)
+            abc
+            cde
+            efg
+            >>> myfunc(items, filter_=u.namefilter(''))
+            abc
+            cde
+            efg
+            >>> myfunc(items, filter_=u.namefilter('cde; tuv'))
+            cde
+            >>> myfunc(items, filter_=u.namefilter('*c*'))
+            abc
+            cde
+            >>> myfunc(items, filter_=u.namefilter('!*c*'))
+            efg
+            >>> myfunc(items, filter_=u.namefilter('*c*; !*e'))
+            abc
+
+            >>> items = ['abc', 'cde', 'efg']
+            >>> myfunc(items, filter_=u.namefilter('*c*; !*e'))
+            abc
     """
     _patterns: tuple[str, ...] = split(namepats)
 
     inclist = [pat for pat in _patterns if not pat.startswith("!")]
     exclist = [pat[1:] for pat in _patterns if pat.startswith("!")]
 
     if inclist:
```

### Comparing `ucdp-0.2.0/src/ucdp/loader.py` & `ucdp-0.3.0/src/ucdp/loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,45 +21,59 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 """
 Loader.
 
-* :any:`load()` is one and only method to pickup and instantiate the topmost hardware module.
+* [load()][ucdp.loader.load] is one and only method to pickup and instantiate the topmost hardware module.
 """
 
+from collections.abc import Iterable
 from functools import lru_cache
 from importlib import import_module
+from pathlib import Path
 
 from caseconverter import pascalcase
 
 from .logging import LOGGER
 from .modbase import BaseMod
 from .moditer import get_mod
 from .modref import ModRef
 from .modtb import ATbMod
 from .modtopref import TopModRef
 from .top import Top
+from .util import extend_sys_path
 
 
-def load(topmodref: TopModRef | str) -> Top:
+def load(topmodref: TopModRef | str, paths: Iterable[Path] | None = None) -> Top:
     """
     Load Module from ``topmodref`` and return :any:`Top`.
 
-    Load ``topref.top``.
-
     In case of a given ``topref.sub`` search for a submodule named ``sub`` within the
     module hierarchy of ``topmod`` using :any:`Top.get_mod()`.
 
     In case of a given ``tb`` search for a testbench ``tb`` and pair it.
+
+    Args:
+        topmodref: Items.
+
+    Keyword Args:
+        paths: Additional Search Paths for Python Modules.
+
+    Returns:
+        Top: Top
+
     """
-    topmodref = TopModRef.cast(topmodref)
-    mod = _load_topmod(topmodref)
-    return Top(ref=topmodref, mod=mod)
+    paths = tuple(paths or [])
+    LOGGER.debug("paths=%r", paths)
+    with extend_sys_path(paths):
+        topmodref = TopModRef.cast(topmodref)
+        mod = _load_topmod(topmodref)
+        return Top(ref=topmodref, mod=mod)
 
 
 @lru_cache
 def _load_topmod(ref: TopModRef) -> BaseMod:
     LOGGER.info("Loading %r", str(ref))
 
     modcls = _load_modcls(ref.top)
@@ -77,13 +91,13 @@
 @lru_cache
 def _build_top(modcls, **kwargs):
     return modcls.build_top(**kwargs)
 
 
 @lru_cache
 def _load_modcls(modref: ModRef):
-    pymod = import_module(f"{modref.lib}.{modref.mod}")
-    modclsname = modref.modcls or f"{pascalcase(modref.mod)}Mod"
+    pymod = import_module(f"{modref.libname}.{modref.modname}")
+    modclsname = modref.modclsname or f"{pascalcase(modref.modname)}Mod"
     modcls = getattr(pymod, modclsname)
     if not issubclass(modcls, BaseMod):
         raise ValueError(f"{modcls} is not a module aka child of <class ucdp.BaseMod>.")
     return modcls
```

### Comparing `ucdp-0.2.0/src/ucdp/logging.py` & `ucdp-0.3.0/src/ucdp/logging.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/mod.py` & `ucdp-0.3.0/src/ucdp/mod.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,30 +31,35 @@
 from .modbasetop import BaseTopMod
 
 
 class AMod(BaseTopMod):
     """
     A Normal Module With Parameters And A Fixed Number Of Ports (maybe `ifdef` encapsulated).
 
-    See :any:`BaseMod` for arguments, attributes and details.
+    See [BaseMod][ucdp.modbase.BaseMod] for arguments, attributes and details.
 
     All module parameter, local parameter, ports, signals and submodules
     **MUST** be added and created within the `_build` method:
 
-    >>> import ucdp as u
-    >>> class AdderMod(u.AMod):
-    ...
-    ...     def _build(self) -> None:
-    ...         width_p = self.add_param(u.IntegerType(default=16), 'width_p')
-    ...         datatype = u.UintType(width_p)
-    ...         self.add_port(datatype, "a_i")
-    ...         self.add_port(datatype, "b_i")
-    ...         self.add_port(datatype, "y_o")
 
-    .. note:: There is no other build method on purpose!
+    ???+ Example "AMod Build Examples"
+        _build(self):
+
+            >>> import ucdp as u
+            >>> class AdderMod(u.AMod):
+            ...
+            ...     def _build(self) -> None:
+            ...         width_p = self.add_param(u.IntegerType(default=16), 'width_p')
+            ...         datatype = u.UintType(width_p)
+            ...         self.add_port(datatype, "a_i")
+            ...         self.add_port(datatype, "b_i")
+            ...         self.add_port(datatype, "y_o")
+
+    Warning:
+        There is no other build method on purpose!
     """
 
     @property
     def modname(self) -> str:
         """Module Name."""
         return snakecase(self.__class__.__name__.removesuffix("Mod"))
```

### Comparing `ucdp-0.2.0/src/ucdp/modbase.py` & `ucdp-0.3.0/src/ucdp/modbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """
 Base Hardware Module.
 
-:any:`BaseMod` defines the base interface which is **common to all hardware modules**.
+[BaseMod][ucdp.modbase.BaseMod] defines the base interface which is **common to all hardware modules**.
 """
 
 from abc import abstractmethod
 from functools import cached_property
 from typing import Any, ClassVar, Optional, Union, no_type_check
 
 from caseconverter import snakecase
@@ -41,14 +41,15 @@
 from .docutil import doc_from_type
 from .exceptions import LockError
 from .expr import BoolOp, Expr
 from .exprparser import ExprParser, Parseable, cast_booltype
 from .flipflop import FlipFlop
 from .ident import Ident, Idents
 from .iterutil import namefilter
+from .logging import LOGGER
 from .modref import ModRef
 from .modutil import get_modbaseinfos
 from .mux import Mux
 from .namespace import Namespace
 from .nameutil import join_names, split_prefix
 from .object import Field, NamedObject, Object, PrivateField, computed_field
 from .orientation import FWD, IN, Direction, Orientation
@@ -83,14 +84,16 @@
 
     title: str | None = None
     descr: str | None = None
     comment: str | None = None
 
     has_hiername: bool = True
 
+    virtual: bool = False
+
     # private
 
     drivers: Drivers = Field(default_factory=Drivers, init=False, repr=False)
     namespace: Idents = Field(default_factory=Idents, init=False, repr=False)
     params: Idents = Field(default_factory=Idents, init=False, repr=False)
     ports: Idents = Field(default_factory=Idents, init=False, repr=False)
     portssignals: Idents = Field(default_factory=Idents, init=False, repr=False)
@@ -153,17 +156,17 @@
         return tuple(f"{baseclassinfo.libname}.{baseclassinfo.modname}" for baseclassinfo in get_modbaseinfos(self))
 
     @classmethod
     def get_modref(cls) -> ModRef:
         """Python Class Reference."""
         bci = next(get_baseclassinfos(cls))
         return ModRef(
-            lib=bci.libname,
-            mod=bci.modname,
-            modcls=bci.clsname,
+            libname=bci.libname,
+            modname=bci.modname,
+            modclsname=bci.clsname,
         )
 
     @property
     def hiername(self) -> str:
         """Hierarchical Name."""
         has_hiername = self.has_hiername
         basename = split_prefix(self.name)[1] if has_hiername else ""
@@ -194,27 +197,27 @@
         while mod.parent:
             parts.insert(0, mod.name)
             mod = mod.parent
         parts.insert(0, mod.modname)
         return "/".join(parts)
 
     @computed_field
-    @property
+    @cached_property
     def assigns(self) -> Assigns:
         """Assignments."""
         return Assigns(targets=self.portssignals, sources=self.namespace, drivers=self.drivers)
 
     @computed_field
-    @property
+    @cached_property
     def parser(self) -> ExprParser:
         """Expression Parser."""
-        return ExprParser(namespace=self.namespace)
+        return ExprParser(namespace=self.namespace, context=str(self))
 
     @computed_field
-    @property
+    @cached_property
     def _router(self) -> "Router":
         """Router."""
         return Router(mod=self)
 
     @property
     def parents(self) -> tuple["BaseMod", ...]:
         """Parents."""
@@ -250,15 +253,16 @@
             title: Full Spoken Name.
             descr: Documentation Description.
             comment: Source Code Comment.
             ifdef: IFDEF pragma
             exist_ok: Do not complain about already existing item
         """
         if isinstance(arg, Param):
-            param: Param = arg
+            value = self.paramdict.pop(arg.name, None)
+            param: Param = arg.new(value=value)
             assert name is None
         else:
             type_: BaseType = arg
             doc = doc_from_type(type_, title=title, descr=descr, comment=comment)
             value = self.paramdict.pop(name, None)
             param = Param(type_=type_, name=name, doc=doc, ifdef=ifdef, value=value)
         if self.__is_locked:
@@ -497,23 +501,25 @@
 
         Args:
             inst: Instance.
         """
         inst.set_parent(self)
         self.insts.add(inst)  # type: ignore[arg-type]
         assigns = Assigns(targets=inst.ports, sources=self.namespace, drivers=self.drivers, all=True, sub=True)
-        parser = ExprParser(namespace=inst.ports, strict=False)
+        parser = ExprParser(namespace=inst.ports, strict=False, context=str(inst))
         self.__instcons[inst.name] = assigns, parser
 
-    def get_inst(self, name: str) -> "BaseMod":
+    def get_inst(self, inst_or_name: Union["BaseMod", str]) -> "BaseMod":
         """
         Get Module Instance.
         """
+        if not isinstance(inst_or_name, str):
+            return self.insts[inst_or_name.name]
         inst = self
-        for part in name.split("/"):
+        for part in inst_or_name.split("/"):
             if part == UPWARDS:
                 if inst.parent is None:
                     raise ValueError(f"{self}: {inst} has no parent.")
                 inst = inst.parent
             else:
                 inst = inst.insts[part]
         return inst
@@ -683,17 +689,17 @@
         """
         Iterate over all Multiplexer.
         """
         return tuple(self.__muxes.values())
 
     def get_mux(self, mux: Mux | str) -> Mux:
         """Get Multiplexer."""
-        if isinstance(mux, str):
-            return self.__muxes[mux]
-        return self.__muxes[mux.name]
+        if not isinstance(mux, str):
+            return self.__muxes[mux.name]
+        return self.__muxes[mux]
 
     @property
     def is_locked(self) -> bool:
         """
         Return If Module Is Already Completed And Locked For Modification.
 
         Locking is done by the build process **automatically** and **MUST NOT** be done earlier or later.
@@ -749,14 +755,15 @@
     """The One And Only Router."""
 
     mod: BaseMod
     __routes: list[tuple[RoutePath, RoutePath]] = PrivateField(default_factory=list)
 
     def add(self, tpath: RoutePath, spath: RoutePath) -> None:
         """Add route from `source` to `tpath`."""
+        LOGGER.debug("%s: router: add '%s' to '%s'", self.mod, spath, tpath)
         self.__routes.append(self._create(tpath, spath))
 
     def flush(self) -> None:
         """Create Pending Routes."""
         for tpath, spath in self.__routes:
             tpathc, spathc = self._create(tpath, spath)
             self._route(tpathc, spathc)
@@ -786,14 +793,15 @@
             return False
         self.__create_port_or_signal(cmod, rident, cpath.expr)
         return True
 
     @no_type_check  # TODO: fix types
     def _route(self, tpath: RoutePath, spath: RoutePath):  # noqa: C901, PLR0912, PLR0915
         mod = self.mod
+        LOGGER.debug("%s router: routing %r to %r", mod, spath, tpath)
         # Referenced modules
         tmod = mod.get_inst(tpath.path) if tpath.path else mod
         smod = mod.get_inst(spath.path) if spath.path else mod
         # Referenced expression/signal
         texpr = tmod.parser.parse(tpath.expr)
         sexpr = smod.parser.parse(spath.expr)
         tident = None if not isinstance(texpr, Ident) else texpr
@@ -878,17 +886,21 @@
     @staticmethod
     def __create_port_or_signal(mod: BaseMod, rident: Ident, name: str) -> BaseSignal:
         assert isinstance(rident, Ident)
         assert name is not None
         assert rident is not None and rident.type_ is not None, (mod, name)
         type_ = rident.type_
         direction = Direction.from_name(name)
+        signal: BaseSignal
         if direction is not None:
-            return mod.add_port(type_, name, ifdef=rident.ifdef, direction=direction)
-        return mod.add_signal(type_, name, ifdef=rident.ifdef)
+            signal = mod.add_port(type_, name, ifdef=rident.ifdef, direction=direction)
+        else:
+            signal = mod.add_signal(type_, name, ifdef=rident.ifdef)
+        LOGGER.debug("%s: router: creating %r", mod, signal)
+        return signal
 
 
 def _merge_cast(one, other):
     # TODO: get rid of this.
     if one or other:
         return True
     if one is None or other is None:
```

### Comparing `ucdp-0.2.0/src/ucdp/modbasetop.py` & `ucdp-0.3.0/src/ucdp/modbasetop.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/modconfigurable.py` & `ucdp-0.3.0/src/ucdp/modconfigurable.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,58 +34,65 @@
 from .modbase import BaseMod
 from .modbasetop import BaseTopMod
 from .nameutil import join_names
 
 
 class AConfigurableMod(BaseTopMod):
     """
-    A Module Which Is Assembled According To A Receipe (:any:`AConfig`).
+    A Module Which Is Assembled According To A Receipe ([AConfig][ucdp.config.AConfig]).
 
-    See :any:`BaseMod` for arguments, attributes and details.
+    See : for arguments, attributes and details.
 
     Additionally the config has to be provided at instantiation.
-    A :any:`AConfigurableMod` may define a `default_config` which is taken if no `config` is provided at instantiaion.
+    A [AConfigurableMod][ucdp.modconfigurable.AConfigurableMod] may define a `default_config`
+    which is taken if no `config` is provided at instantiaion.
 
     All module parameter, local parameter, ports, signals and submodules
     **MUST** be added and created within the `_build` method depending on the config.
 
 
     .. attention:: It is forbidden to implement `add` methods or any other *tailored* functionality.
                    Use a tailored module instead!
 
     Configurable modules are located next to the python file and use the configuration name in the module name.
 
-    Example:
-    >>> import ucdp as u
-    >>> class MyConfig(u.AConfig):
-    ...
-    ...     feature: bool = False
-
-    >>> class ProcMod(u.AConfigurableMod):
-    ...
-    ...     default_config = MyConfig('default')
-    ...
-    ...     def _build(self) -> None:
-    ...         if self.config.feature:
-    ...             self.add_port(u.UintType(8), "feature_i")
-    ...             self.add_port(u.UintType(8), "feature_o")
-    ...         else:
-    ...             self.add_port(u.UintType(8), "default_o")
-
-    >>> my = ProcMod()
-    >>> my.modname
-    'proc_default'
-    >>> my.ports
-    Idents([Port(UintType(8), 'default_o', direction=OUT)])
-
-    >>> my = ProcMod(config=MyConfig('other', feature=True))
-    >>> my.modname
-    'proc_other'
-    >>> my.ports
-    Idents([Port(UintType(8), 'feature_i', direction=IN), Port(UintType(8), 'feature_o', direction=OUT)])
+    Attributes:
+        default_config: Direction.
+        config:
+
+    ??? Example "AConfigurableMod Example"
+            Basics:
+
+            >>> import ucdp as u
+            >>> class MyConfig(u.AConfig):
+            ...
+            ...     feature: bool = False
+
+            >>> class ProcMod(u.AConfigurableMod):
+            ...
+            ...     default_config = MyConfig('default')
+            ...
+            ...     def _build(self) -> None:
+            ...         if self.config.feature:
+            ...             self.add_port(u.UintType(8), "feature_i")
+            ...             self.add_port(u.UintType(8), "feature_o")
+            ...         else:
+            ...             self.add_port(u.UintType(8), "default_o")
+
+            >>> my = ProcMod()
+            >>> my.modname
+            'proc_default'
+            >>> my.ports
+            Idents([Port(UintType(8), 'default_o', direction=OUT)])
+
+            >>> my = ProcMod(config=MyConfig('other', feature=True))
+            >>> my.modname
+            'proc_other'
+            >>> my.ports
+            Idents([Port(UintType(8), 'feature_i', direction=IN), Port(UintType(8), 'feature_o', direction=OUT)])
     """
 
     default_config: ClassVar[BaseConfig | None] = None
     config: BaseConfig
 
     def __init__(
         self, parent: BaseMod | None = None, name: str | None = None, config: BaseConfig | None = None, **kwargs
```

### Comparing `ucdp-0.2.0/src/ucdp/modcore.py` & `ucdp-0.3.0/src/ucdp/modcore.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,27 +31,32 @@
 from .modbase import BaseMod
 from .modfilelist import ModFileLists
 from .modutil import is_tb_from_modname
 from .nameutil import join_names
 from .object import model_validator
 
 
-class CoreMod(BaseMod):
+class ACoreMod(BaseMod):
     """
     Intermediate Module Hierarchy.
 
-    See :any:`BaseMod` for arguments, attributes and details.
+    See [BaseMod][ucdp.modbase.BaseMod] for arguments, attributes and details.
 
-    A :any:`CoreMod` should be use to create intermediate module hierarchies.
-    :any:`CoreMod` do **not** have a `_build` method. They have to be built by the parent module.
+    A [ACoreMod][uart.uart.UartCoreMod] should be use to create intermediate module hierarchies.
+    [ACoreMod][uart.uart.UartCoreMod] do **not** have a `_build` method. They have to be built by the parent module.
 
     The source code files are typically generated/located next to the parent module of core module.
     Remember to set the `gen` attribute accordingly to control the file generation.
     Also the module name is based on the parent module and extended by the instance name.
-    A :any:`CoreMod` can have a Mako template.
+    A [ACoreMod][uart.uart.UartCoreMod] can have a Mako template.
+
+    Attributes:
+        filelists: File Lists.
+        parent: parent module.
+
     """
 
     filelists: ClassVar[ModFileLists] = ()
     """File Lists."""
 
     parent: BaseMod
 
@@ -74,10 +79,10 @@
     def is_tb(self) -> bool:
         """Determine if module belongs to Testbench or Design."""
         if self.parent:
             return self.parent.is_tb
         return is_tb_from_modname(self.modname)
 
     @model_validator(mode="after")
-    def __post_init(self) -> "CoreMod":
+    def __post_init(self) -> "ACoreMod":
         self.parent.add_inst(self)
         return self
```

### Comparing `ucdp-0.2.0/src/ucdp/moditer.py` & `ucdp-0.3.0/src/ucdp/moditer.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,70 +95,73 @@
 
     Keyword Args:
         filter_: function called with every `mod` as argument, `mod` is returned if `True`.
         stop: stop iteration at `mod` if `stop` function returns `True` for `mod`.
         maxlevel (int): maximum descending in the mod hierarchy.
         unique (bool): Just return module once.
 
-    >>> import ucdp as u
-    >>> class CMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         pass
-    >>> class EMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         pass
-    >>> class AMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         pass
-    >>> class DMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         CMod(self, "c")
-    ...         EMod(self, "e")
-    >>> class BMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         AMod(self, "a")
-    ...         DMod(self, "d")
-    >>> class HMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         pass
-    >>> class IMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         HMod(self, "h")
-    >>> class GMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         IMod(self, "i")
-    >>> class FMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         BMod(self, "b")
-    ...         GMod(self, "g")
-
-    >>> f = FMod(None, "f")
-    >>> [mod.name for mod in ModPreIter(f)]
-    ['f', 'b', 'a', 'd', 'c', 'e', 'g', 'i', 'h']
-    >>> [mod.name for mod in ModPreIter(f, maxlevel=3)]
-    ['f', 'b', 'a', 'd', 'g', 'i']
-    >>> [mod.name for mod in ModPreIter(f, maxlevel=3, filter_=lambda n: n.name not in 'eg')]
-    ['f', 'b', 'a', 'd', 'i']
-    >>> [mod.name for mod in ModPreIter(f, maxlevel=3, filter_=lambda n: n.name not in 'eg',
-    ...                                 stop=lambda n: n.name == 'd')]
-    ['f', 'b', 'a', 'i']
-    >>> [mod.name for mod in ModPreIter(f, maxlevel=3, stop=lambda n: n.name == 'd')]
-    ['f', 'b', 'a', 'g', 'i']
-    >>> [mod.name for mod in ModPreIter(f, filter_=lambda n: n.name not in 'eg')]
-    ['f', 'b', 'a', 'd', 'c', 'i', 'h']
-    >>> [mod.name for mod in ModPreIter(f, stop=lambda n: n.name == 'd')]
-    ['f', 'b', 'a', 'g', 'i', 'h']
-    >>> [mod.name for mod in ModPreIter(f, filter_=lambda n: n.name not in 'eg', stop=lambda n: n.name == 'd')]
-    ['f', 'b', 'a', 'i', 'h']
-    >>> [mod.name for mod in ModPreIter(f)]
-    ['f', 'b', 'a', 'd', 'c', 'e', 'g', 'i', 'h']
-    >>> [mod.modname for mod in ModPreIter(f, unique=True)]
-    ['f', 'b', 'a', 'd', 'c', 'e', 'g', 'i', 'h']
-    >>> [mod.name for mod in ModPreIter(f, stop_insts=lambda n: n.name == 'b')]
-    ['f', 'b', 'g', 'i', 'h']
+    ??? Example "Module Pre Iterator Examples"
+        pre-order strategy Examples.
+
+            >>> import ucdp as u
+            >>> class CMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         pass
+            >>> class EMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         pass
+            >>> class AMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         pass
+            >>> class DMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         CMod(self, "c")
+            ...         EMod(self, "e")
+            >>> class BMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         AMod(self, "a")
+            ...         DMod(self, "d")
+            >>> class HMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         pass
+            >>> class IMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         HMod(self, "h")
+            >>> class GMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         IMod(self, "i")
+            >>> class FMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         BMod(self, "b")
+            ...         GMod(self, "g")
+
+            >>> f = FMod(None, "f")
+            >>> [mod.name for mod in ModPreIter(f)]
+            ['f', 'b', 'a', 'd', 'c', 'e', 'g', 'i', 'h']
+            >>> [mod.name for mod in ModPreIter(f, maxlevel=3)]
+            ['f', 'b', 'a', 'd', 'g', 'i']
+            >>> [mod.name for mod in ModPreIter(f, maxlevel=3, filter_=lambda n: n.name not in 'eg')]
+            ['f', 'b', 'a', 'd', 'i']
+            >>> [mod.name for mod in ModPreIter(f, maxlevel=3, filter_=lambda n: n.name not in 'eg',
+            ...                                 stop=lambda n: n.name == 'd')]
+            ['f', 'b', 'a', 'i']
+            >>> [mod.name for mod in ModPreIter(f, maxlevel=3, stop=lambda n: n.name == 'd')]
+            ['f', 'b', 'a', 'g', 'i']
+            >>> [mod.name for mod in ModPreIter(f, filter_=lambda n: n.name not in 'eg')]
+            ['f', 'b', 'a', 'd', 'c', 'i', 'h']
+            >>> [mod.name for mod in ModPreIter(f, stop=lambda n: n.name == 'd')]
+            ['f', 'b', 'a', 'g', 'i', 'h']
+            >>> [mod.name for mod in ModPreIter(f, filter_=lambda n: n.name not in 'eg', stop=lambda n: n.name == 'd')]
+            ['f', 'b', 'a', 'i', 'h']
+            >>> [mod.name for mod in ModPreIter(f)]
+            ['f', 'b', 'a', 'd', 'c', 'e', 'g', 'i', 'h']
+            >>> [mod.modname for mod in ModPreIter(f, unique=True)]
+            ['f', 'b', 'a', 'd', 'c', 'e', 'g', 'i', 'h']
+            >>> [mod.name for mod in ModPreIter(f, stop_insts=lambda n: n.name == 'b')]
+            ['f', 'b', 'g', 'i', 'h']
     """
 
     @staticmethod
     def _iter(
         mods: Iterable[BaseMod], filter_: FilterFunc, stop: StopFunc, stop_insts: StopFunc, maxlevel: MaxLevel
     ) -> Iterator[BaseMod]:
         # TODO: heap impl
@@ -179,70 +182,73 @@
 
     Keyword Args:
         filter_: function called with every `mod` as argument, `mod` is returned if `True`.
         stop: stop iteration at `mod` if `stop` function returns `True` for `mod`.
         maxlevel (int): maximum descending in the mod hierarchy.
         unique (bool): Just return module once.
 
-    >>> import ucdp as u
-    >>> class CMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         pass
-    >>> class EMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         pass
-    >>> class AMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         pass
-    >>> class DMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         CMod(self, "c")
-    ...         EMod(self, "e")
-    >>> class BMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         AMod(self, "a")
-    ...         DMod(self, "d")
-    >>> class HMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         pass
-    >>> class IMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         HMod(self, "h")
-    >>> class GMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         IMod(self, "i")
-    >>> class FMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         BMod(self, "b")
-    ...         GMod(self, "g")
-
-    >>> f = FMod(None, "f")
-    >>> [mod.name for mod in ModPostIter(f)]
-    ['a', 'c', 'e', 'd', 'b', 'h', 'i', 'g', 'f']
-    >>> [mod.name for mod in ModPostIter(f, maxlevel=3)]
-    ['a', 'd', 'b', 'i', 'g', 'f']
-    >>> [mod.name for mod in ModPostIter(f, maxlevel=3, filter_=lambda n: n.name not in 'eg')]
-    ['a', 'd', 'b', 'i', 'f']
-    >>> [mod.name for mod in ModPostIter(f, maxlevel=3, filter_=lambda n: n.name not in 'eg',
-    ...                                  stop=lambda n: n.name == 'd')]
-    ['a', 'b', 'i', 'f']
-    >>> [mod.name for mod in ModPostIter(f, maxlevel=3, stop=lambda n: n.name == 'd')]
-    ['a', 'b', 'i', 'g', 'f']
-    >>> [mod.name for mod in ModPostIter(f, filter_=lambda n: n.name not in 'eg')]
-    ['a', 'c', 'd', 'b', 'h', 'i', 'f']
-    >>> [mod.name for mod in ModPostIter(f, stop=lambda n: n.name == 'd')]
-    ['a', 'b', 'h', 'i', 'g', 'f']
-    >>> [mod.name for mod in ModPostIter(f, filter_=lambda n: n.name not in 'eg', stop=lambda n: n.name == 'd')]
-    ['a', 'b', 'h', 'i', 'f']
-    >>> [mod.name for mod in ModPostIter(f)]
-    ['a', 'c', 'e', 'd', 'b', 'h', 'i', 'g', 'f']
-    >>> [mod.modname for mod in ModPostIter(f, unique=True)]
-    ['a', 'c', 'e', 'd', 'b', 'h', 'i', 'g', 'f']
-    >>> [mod.name for mod in ModPostIter(f, stop_insts=lambda n: n.name == 'b')]
-    ['b', 'h', 'i', 'g', 'f']
+    ??? Example "Module Post Iterator Examples"
+        pre-order strategy Examples.
+
+            >>> import ucdp as u
+            >>> class CMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         pass
+            >>> class EMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         pass
+            >>> class AMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         pass
+            >>> class DMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         CMod(self, "c")
+            ...         EMod(self, "e")
+            >>> class BMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         AMod(self, "a")
+            ...         DMod(self, "d")
+            >>> class HMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         pass
+            >>> class IMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         HMod(self, "h")
+            >>> class GMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         IMod(self, "i")
+            >>> class FMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         BMod(self, "b")
+            ...         GMod(self, "g")
+
+            >>> f = FMod(None, "f")
+            >>> [mod.name for mod in ModPostIter(f)]
+            ['a', 'c', 'e', 'd', 'b', 'h', 'i', 'g', 'f']
+            >>> [mod.name for mod in ModPostIter(f, maxlevel=3)]
+            ['a', 'd', 'b', 'i', 'g', 'f']
+            >>> [mod.name for mod in ModPostIter(f, maxlevel=3, filter_=lambda n: n.name not in 'eg')]
+            ['a', 'd', 'b', 'i', 'f']
+            >>> [mod.name for mod in ModPostIter(f, maxlevel=3, filter_=lambda n: n.name not in 'eg',
+            ...                                  stop=lambda n: n.name == 'd')]
+            ['a', 'b', 'i', 'f']
+            >>> [mod.name for mod in ModPostIter(f, maxlevel=3, stop=lambda n: n.name == 'd')]
+            ['a', 'b', 'i', 'g', 'f']
+            >>> [mod.name for mod in ModPostIter(f, filter_=lambda n: n.name not in 'eg')]
+            ['a', 'c', 'd', 'b', 'h', 'i', 'f']
+            >>> [mod.name for mod in ModPostIter(f, stop=lambda n: n.name == 'd')]
+            ['a', 'b', 'h', 'i', 'g', 'f']
+            >>> [mod.name for mod in ModPostIter(f, filter_=lambda n: n.name not in 'eg', stop=lambda n: n.name == 'd')]
+            ['a', 'b', 'h', 'i', 'f']
+            >>> [mod.name for mod in ModPostIter(f)]
+            ['a', 'c', 'e', 'd', 'b', 'h', 'i', 'g', 'f']
+            >>> [mod.modname for mod in ModPostIter(f, unique=True)]
+            ['a', 'c', 'e', 'd', 'b', 'h', 'i', 'g', 'f']
+            >>> [mod.name for mod in ModPostIter(f, stop_insts=lambda n: n.name == 'b')]
+            ['b', 'h', 'i', 'g', 'f']
     """
 
     @staticmethod
     def _iter(
         mods: Iterable[BaseMod], filter_: FilterFunc, stop: StopFunc, stop_insts: StopFunc, maxlevel: MaxLevel
     ) -> Iterator[BaseMod]:
         # TODO: heap impl
```

### Comparing `ucdp-0.2.0/src/ucdp/modref.py` & `ucdp-0.3.0/src/ucdp/modref.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,73 +30,76 @@
 from typing import Union
 
 from .consts import PAT_IDENTIFIER
 from .object import Field, LightObject
 
 RE_MODREF = re.compile(
     # lib
-    r"(?P<lib>[a-zA-Z][a-zA-Z_0-9]*)\."
+    r"(?P<libname>[a-zA-Z][a-zA-Z_0-9]*)\."
     # mod
-    r"(?P<mod>[a-zA-Z][a-zA-Z_0-9]*)"
+    r"(?P<modname>[a-zA-Z][a-zA-Z_0-9]*)"
     # cls
-    r"(\.(?P<modcls>[A-Z][a-zA-Z_0-9]*Mod))?"
+    r"(\.(?P<modclsname>[A-Z][a-zA-Z_0-9]*Mod))?"
 )
 PAT_MODREF = "lib.my[.MyMod]"
 
 
 class ModRef(LightObject):
     """
     Module Reference.
 
     Args:
-        lib: Library Name
-        mod: Module Name
+        libname: Library Name
+        modname: Module Name
 
     Keyword Args:
-        modcls: Class Name
+        modclsname: Class Name
 
-    >>> ModRef('glbl_lib', 'clk_gate', modcls='ClkGateMod')
-    ModRef('glbl_lib', 'clk_gate', modcls='ClkGateMod')
+    ??? Example "Module Reference Examples"
+        Examples.
 
-    Just a module:
+            >>> ModRef('glbl_lib', 'clk_gate', modclsname='ClkGateMod')
+            ModRef('glbl_lib', 'clk_gate', modclsname='ClkGateMod')
 
-    >>> spec = ModRef.cast('glbl_lib.clk_gate')
-    >>> spec
-    ModRef('glbl_lib', 'clk_gate')
-    >>> str(spec)
-    'glbl_lib.clk_gate'
+            Just a module:
 
-    Module from a package and explicit class:
+            >>> spec = ModRef.cast('glbl_lib.clk_gate')
+            >>> spec
+            ModRef('glbl_lib', 'clk_gate')
+            >>> str(spec)
+            'glbl_lib.clk_gate'
 
-    >>> spec = ModRef.cast('glbl_lib.clk_gate.ClkGateMod')
-    >>> spec
-    ModRef('glbl_lib', 'clk_gate', modcls='ClkGateMod')
-    >>> str(spec)
-    'glbl_lib.clk_gate.ClkGateMod'
+            Module from a package and explicit class:
 
-    Invalid Pattern:
+            >>> spec = ModRef.cast('glbl_lib.clk_gate.ClkGateMod')
+            >>> spec
+            ModRef('glbl_lib', 'clk_gate', modclsname='ClkGateMod')
+            >>> str(spec)
+            'glbl_lib.clk_gate.ClkGateMod'
 
-    >>> ModRef.cast('lib.my:c-ls')
-    Traceback (most recent call last):
-    ..
-    ValueError: 'lib.my:c-ls' does not match pattern 'lib.my[.MyMod]'
+            Invalid Pattern:
+
+            >>> ModRef.cast('lib.my:c-ls')
+            Traceback (most recent call last):
+            ..
+            ValueError: 'lib.my:c-ls' does not match pattern 'lib.my[.MyMod]'
     """
 
-    lib: str = Field(pattern=PAT_IDENTIFIER)
-    mod: str = Field(pattern=PAT_IDENTIFIER)
-    modcls: str | None = Field(pattern=PAT_IDENTIFIER, default=None)
+    libname: str = Field(pattern=PAT_IDENTIFIER)
+    modname: str = Field(pattern=PAT_IDENTIFIER)
+    modclsname: str | None = Field(pattern=PAT_IDENTIFIER, default=None)
 
-    _posargs: tuple[str, ...] = ("lib", "mod")
+    _posargs: tuple[str, ...] = ("libname", "modname")
 
-    def __init__(self, lib: str, mod: str, modcls: str | None = None):
-        super().__init__(lib=lib, mod=mod, modcls=modcls)  # type: ignore[call-arg]
+    def __init__(self, libname: str, modname: str, modclsname: str | None = None):
+        super().__init__(libname=libname, modname=modname, modclsname=modclsname)  # type: ignore[call-arg]
 
     def __str__(self) -> str:
-        modcls = f".{self.modcls}" if self.modcls else ""
-        return f"{self.lib}.{self.mod}{modcls}"
+        modclsname = f".{self.modclsname}" if self.modclsname else ""
+        return f"{self.libname}.{self.modname}{modclsname}"
 
     @staticmethod
     def cast(value: Union["ModRef", str]) -> "ModRef":
         """Cast `value` to `ModRef`."""
         if isinstance(value, ModRef):
             return value
```

### Comparing `ucdp-0.2.0/src/ucdp/modtailored.py` & `ucdp-0.3.0/src/ucdp/modtailored.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,55 +64,59 @@
 
     * `_build` should be used for all **static** code and initialization.
     * Tailored modules should provide `add` methods to tailor the module instance to the needs of
       the parent module.
     * `_build_dep` is called **after** all `add` methods have been called and should be used for all
       **dynamic** aspects which can only be known after the parent module made its adjustments.
 
-    Example Definition:
+    Attributes:
+        filelists: Filelists.
 
-    >>> import logging
-    >>> import ucdp as u
-    >>> LOGGER = logging.getLogger(__name__)
-    >>> class DmxMod(u.ATailoredMod):
-    ...     slaves: u.Namespace = u.Field(default_factory=u.Namespace, init=False)
-    ...
-    ...     def add_slave(self, name, route=None):
-    ...         self.slaves[name] = slave = Slave(dmx=self, name=name)
-    ...         portname = f"slv_{name}_o"
-    ...         self.add_port(u.UintType(16), portname)
-    ...         if route:
-    ...             self.con(portname, route)
-    ...         return slave
-    ...
-    ...     def _build(self) -> None:
-    ...         pass#self.add_port(u.UintType(16), "mst_i")
-    ...
-    ...     def _build_dep(self):
-    ...         if not self.slaves:
-    ...             LOGGER.warning("%r: has no APB slaves", self)
-    ...
-    >>> class Slave(u.NamedObject):
-    ...     dmx: u.BaseMod = u.Field(repr=False)
-
-    Example Usage:
-
-    >>> import ucdp as u
-    >>> class TopMod(u.AMod):
-    ...     def _build(self) -> None:
-    ...         dmx = DmxMod(self, 'u_dmx')
-    ...         dmx.add_slave('a')
-    ...         dmx.add_slave('b')
-    >>> top = TopMod()
-    >>> top
-    <ucdp.modtailored.TopMod(inst='top', libname='ucdp', modname='top')>
-    >>> top.get_inst('u_dmx')
-    <ucdp.modtailored.DmxMod(inst='top/u_dmx', libname='ucdp', modname='top_dmx')>
-    >>> top.get_inst('u_dmx').slaves
-    Namespace([Slave(name='a'), Slave(name='b')])
+    ??? Example "Module Reference Examples"
+        Example Definition:
+
+            >>> import logging
+            >>> import ucdp as u
+            >>> LOGGER = logging.getLogger(__name__)
+            >>> class DmxMod(u.ATailoredMod):
+            ...     slaves: u.Namespace = u.Field(default_factory=u.Namespace, init=False)
+            ...
+            ...     def add_slave(self, name, route=None):
+            ...         self.slaves[name] = slave = Slave(dmx=self, name=name)
+            ...         portname = f"slv_{name}_o"
+            ...         self.add_port(u.UintType(16), portname)
+            ...         if route:
+            ...             self.con(portname, route)
+            ...         return slave
+            ...
+            ...     def _build(self) -> None:
+            ...         pass#self.add_port(u.UintType(16), "mst_i")
+            ...
+            ...     def _build_dep(self):
+            ...         if not self.slaves:
+            ...             LOGGER.warning("%r: has no APB slaves", self)
+            ...
+            >>> class Slave(u.NamedObject):
+            ...     dmx: u.BaseMod = u.Field(repr=False)
+
+        Example Usage:
+
+            >>> import ucdp as u
+            >>> class TopMod(u.AMod):
+            ...     def _build(self) -> None:
+            ...         dmx = DmxMod(self, 'u_dmx')
+            ...         dmx.add_slave('a')
+            ...         dmx.add_slave('b')
+            >>> top = TopMod()
+            >>> top
+            <ucdp.modtailored.TopMod(inst='top', libname='ucdp', modname='top')>
+            >>> top.get_inst('u_dmx')
+            <ucdp.modtailored.DmxMod(inst='top/u_dmx', libname='ucdp', modname='top_dmx')>
+            >>> top.get_inst('u_dmx').slaves
+            Namespace([Slave(name='a'), Slave(name='b')])
     """
 
     filelists: ClassVar[ModFileLists] = ()
     """File Lists."""
 
     _has_build_dep: bool = PrivateField(default=True)
     _has_build_final: bool = PrivateField(default=True)
```

### Comparing `ucdp-0.2.0/src/ucdp/modtb.py` & `ucdp-0.3.0/src/ucdp/modtb.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,58 +42,66 @@
 from .test import Test
 
 
 class ATbMod(BaseMod):
     """
     Testbench Module.
 
-    Args:
+    Attributes:
+        filelists: File Lists.
+        dut_mods: Testbench is limited to these kind of modules.
+        title: Title.
         dut: Module Under Test.
+        parent: Parent.
+
 
     Create testbench for `dut`.
 
-    The :any:`TopModRef` and :any:`load` function allow to wrap any design module with a testbench.
+    The [TopModRef][ucdp.modtopref.TopModRef] and [load()][ucdp.loader.load] function
+    allow to wrap any design module with a testbench.
+
+    ??? Example "Module Testbench Examples"
+        Example:
 
-    Example:
-    >>> import ucdp as u
-    >>> class MyMod(u.AMod):
-    ...
-    ...     def _build(self):
-    ...         self.add_port(u.UintType(4), "data_i")
-    ...         self.add_port(u.UintType(4), "data_o")
-    ...
-    >>> class OtherMod(u.AMod):
-    ...
-    ...     def _build(self):
-    ...         self.add_port(u.UintType(4), "data_i")
-    ...         self.add_port(u.UintType(4), "data_o")
-    ...
-    >>> class GenTbMod(u.ATbMod):
-    ...
-    ...     def _build(self):
-    ...         # Build testbench for self.dut here
-    ...         pass
-    ...
-    ...     @staticmethod
-    ...     def build_dut():
-    ...         return MyMod()
-
-    >>> tb = GenTbMod()
-    >>> tb
-    <ucdp.modtb.GenTbMod(inst='gen_tb_my', libname='ucdp', modname='gen_tb_my', dut=<ucdp.modtb.MyMod(...)>)>
-    >>> tb.dut
-    <ucdp.modtb.MyMod(inst='my', libname='ucdp', modname='my')>
-    >>> tb = GenTbMod(OtherMod())
-    >>> tb
-    <ucdp.modtb.GenTbMod(inst='gen_tb_other', libname='ucdp', modname='gen_tb_other', dut=<ucdp.modtb.OtherMod(...)>)>
-    >>> tb.dut
-    <ucdp.modtb.OtherMod(inst='other', libname='ucdp', modname='other')>
+            >>> import ucdp as u
+            >>> class MyMod(u.AMod):
+            ...
+            ...     def _build(self):
+            ...         self.add_port(u.UintType(4), "data_i")
+            ...         self.add_port(u.UintType(4), "data_o")
+            ...
+            >>> class OtherMod(u.AMod):
+            ...
+            ...     def _build(self):
+            ...         self.add_port(u.UintType(4), "data_i")
+            ...         self.add_port(u.UintType(4), "data_o")
+            ...
+            >>> class GenTbMod(u.ATbMod):
+            ...
+            ...     def _build(self):
+            ...         # Build testbench for self.dut here
+            ...         pass
+            ...
+            ...     @staticmethod
+            ...     def build_dut():
+            ...         return MyMod()
+
+            >>> tb = GenTbMod()
+            >>> tb
+            <ucdp.modtb.GenTbMod(inst='gen_tb_my', libname='ucdp', modname='gen_tb_my', dut=<ucdp.modtb.MyMod(...)>)>
+            >>> tb.dut
+            <ucdp.modtb.MyMod(inst='my', libname='ucdp', modname='my')>
+            >>> tb = GenTbMod(OtherMod())
+            >>> tb
+            <ucdp.modtb.GenTbMod(inst='gen_tb_other', libname='ucdp', modname='...', dut=<ucdp.modtb.OtherMod(...)>)>
+            >>> tb.dut
+            <ucdp.modtb.OtherMod(inst='other', libname='ucdp', modname='other')>
 
-    :any:`TopRef` and :any:`load` handle that gracefully and allow pairing of testbench and dut on
-    command line and in configuration files.
+    [TopModRef][ucdp.modtopref.TopModRef] and [load()][ucdp.loader.load] handle that gracefully and
+    allow pairing of testbench and dut on command line and in configuration files.
     """
 
     filelists: ClassVar[ModFileLists] = ()
     """File Lists."""
 
     dut_mods: ClassVar[tuple[Any, ...]] = ()
     """Testbench is limited to these kind of modules."""
```

### Comparing `ucdp-0.2.0/src/ucdp/modtopref.py` & `ucdp-0.3.0/src/ucdp/modtopref.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,32 +45,35 @@
 class TopModRef(LightObject):
     """
     Top Module Reference.
 
     Args:
         top: Top Module Reference
 
-    Keyword Args:
+    Attributes:
         sub: Sub Module Reference
         tb: Testbench Module Reference
 
-    >>> import ucdp as u
-    >>> u.TopModRef.cast('top_lib.top_mod')
-    TopModRef(ModRef('top_lib', 'top_mod'))
-    >>> u.TopModRef.cast('top_lib.top_mod-sub_lib.sub_mod')
-    TopModRef(ModRef('top_lib', 'top_mod'), sub='sub_lib.sub_mod')
-    >>> u.TopModRef.cast('mod_tb_lib.mod_tb#top_lib.top_mod')
-    TopModRef(ModRef('top_lib', 'top_mod'), tb=ModRef('mod_tb_lib', 'mod_tb'))
-
-    Invalid Pattern:
-
-    >>> TopModRef.cast('lib.mod:c-ls.1')
-    Traceback (most recent call last):
-    ..
-    ValueError: 'lib.mod:c-ls.1' does not match pattern '[tb_lib.tb#]top_lib.top[-sub_lib.sub]'
+    ??? Example "Top Reference Examples"
+        Example:
+
+            >>> import ucdp as u
+            >>> u.TopModRef.cast('top_lib.top_mod')
+            TopModRef(ModRef('top_lib', 'top_mod'))
+            >>> u.TopModRef.cast('top_lib.top_mod-sub_lib.sub_mod')
+            TopModRef(ModRef('top_lib', 'top_mod'), sub='sub_lib.sub_mod')
+            >>> u.TopModRef.cast('mod_tb_lib.mod_tb#top_lib.top_mod')
+            TopModRef(ModRef('top_lib', 'top_mod'), tb=ModRef('mod_tb_lib', 'mod_tb'))
+
+            Invalid Pattern:
+
+            >>> TopModRef.cast('lib.mod:c-ls.1')
+            Traceback (most recent call last):
+            ..
+            ValueError: 'lib.mod:c-ls.1' does not match pattern '[tb_lib.tb#]top_lib.top[-sub_lib.sub]'
     """
 
     top: ModRef
     sub: str | None = Field(default=None, pattern=RE_MODREF)
     tb: ModRef | None = None
 
     _posargs: tuple[str, ...] = ("top",)
```

### Comparing `ucdp-0.2.0/src/ucdp/modutil.py` & `ucdp-0.3.0/src/ucdp/modutil.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,19 +30,25 @@
 
 from .baseclassinfo import BaseClassInfo, get_baseclassinfos
 
 
 def get_modbaseinfos(cls_or_inst) -> Iterator[BaseClassInfo]:
     """
     Get Base Classes of `mod`.
+
+    Args:
+        cls_or_inst: Class or Instance
     """
     for baseclassinfo in get_baseclassinfos(cls_or_inst):
         if baseclassinfo.libname == "ucdp":
             break
         yield baseclassinfo
 
 
 def is_tb_from_modname(modname: str) -> bool:
     """
     Determine if module is a testbench component by checking the name.
+
+    Args:
+        modname: Module Name
     """
     return modname.endswith("_tb") or "_tb_" in modname
```

### Comparing `ucdp-0.2.0/src/ucdp/mux.py` & `ucdp-0.3.0/src/ucdp/mux.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,21 @@
 MuxBranch = dict[Expr, Assigns]
 
 
 class Mux(NamedObject):
     """
     Multiplexer.
 
-    Args:
-        name (str): Name
-        targets (Idents): Ports and signals allowed to be assigned
-        namespace (Idents): Ports, signals, parameter and local parameter as source
-        drivers (dict): Drivers, for multiple-driver tracking.
+    Attributes:
+        name: Name
+        targets: Ports and signals allowed to be assigned
+        namespace: Ports, signals, parameter and local parameter as source
+        drivers: Drivers, for multiple-driver tracking.
+        parser: Parser
+        doc: Documentation
     """
 
     targets: Idents = Field(repr=False)
     namespace: Idents = Field(repr=False)
     drivers: Drivers = Field(repr=False, default_factory=dict)
     parser: ExprParser = Field(repr=False)
     doc: Doc = Doc()
```

### Comparing `ucdp-0.2.0/src/ucdp/namespace.py` & `ucdp-0.3.0/src/ucdp/namespace.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,59 +29,62 @@
 
 * items use `item.name` as dictionary key. This is checked.
 * items **cannot** be overwritten
 * items **cannot** be deleted
 * the namespace can be locked for modifications via `lock`.
 * iteration over the namespaces yields the items and not their keys.
 
->>> from collections import namedtuple
->>> NamedObject = namedtuple('NamedObject', 'name foo bar')
->>> namespace = Namespace([NamedObject('a', 1, 2)])
->>> namespace.add(NamedObject('b', 3, 4))
->>> namespace['c'] = NamedObject('c', 5, 6)
->>> namespace.is_locked
-False
->>> for item in namespace:
-...     item
-NamedObject(name='a', foo=1, bar=2)
-NamedObject(name='b', foo=3, bar=4)
-NamedObject(name='c', foo=5, bar=6)
->>> for item in namespace.keys():
-...     item
-'a'
-'b'
-'c'
->>> for item in namespace.values():
-...     item
-NamedObject(name='a', foo=1, bar=2)
-NamedObject(name='b', foo=3, bar=4)
-NamedObject(name='c', foo=5, bar=6)
->>> namespace['b']
-NamedObject(name='b', foo=3, bar=4)
->>> namespace['d']
-Traceback (most recent call last):
-  ...
-KeyError: 'd'
->>> namespace.get_dym('d')
-Traceback (most recent call last):
-  ...
-ValueError: 'd' Known are 'a', 'b' and 'c'.
-
-Locking:
-
->>> namespace.lock()
->>> namespace.is_locked
-True
->>> namespace['d'] = NamedObject('d', 7, 8)
-Traceback (most recent call last):
-  ...
-ValueError: Namespace is already locked
+??? Example "Namespace Examples"
+    Examples.
 
->>> len(namespace)
-3
+        >>> from collections import namedtuple
+        >>> NamedObject = namedtuple('NamedObject', 'name foo bar')
+        >>> namespace = Namespace([NamedObject('a', 1, 2)])
+        >>> namespace.add(NamedObject('b', 3, 4))
+        >>> namespace['c'] = NamedObject('c', 5, 6)
+        >>> namespace.is_locked
+        False
+        >>> for item in namespace:
+        ...     item
+        NamedObject(name='a', foo=1, bar=2)
+        NamedObject(name='b', foo=3, bar=4)
+        NamedObject(name='c', foo=5, bar=6)
+        >>> for item in namespace.keys():
+        ...     item
+        'a'
+        'b'
+        'c'
+        >>> for item in namespace.values():
+        ...     item
+        NamedObject(name='a', foo=1, bar=2)
+        NamedObject(name='b', foo=3, bar=4)
+        NamedObject(name='c', foo=5, bar=6)
+        >>> namespace['b']
+        NamedObject(name='b', foo=3, bar=4)
+        >>> namespace['d']
+        Traceback (most recent call last):
+        ...
+        KeyError: 'd'
+        >>> namespace.get_dym('d')
+        Traceback (most recent call last):
+        ...
+        ValueError: 'd' Known are 'a', 'b' and 'c'.
+
+    Locking:
+
+        >>> namespace.lock()
+        >>> namespace.is_locked
+        True
+        >>> namespace['d'] = NamedObject('d', 7, 8)
+        Traceback (most recent call last):
+        ...
+        ValueError: Namespace is already locked
+
+        >>> len(namespace)
+        3
 """
 
 from collections.abc import Iterable
 from typing import Any
 
 from .exceptions import DuplicateError
 from .nameutil import didyoumean
```

### Comparing `ucdp-0.2.0/src/ucdp/nameutil.py` & `ucdp-0.3.0/src/ucdp/nameutil.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,92 +40,133 @@
 
 
 @functools.lru_cache
 def split_prefix(name: str) -> tuple[str, str]:
     """
     Split Name Into Prefix and Basename.
 
-    >>> split_prefix("i_count")
-    ('i_', 'count')
-    >>> split_prefix("u_count")
-    ('u_', 'count')
-    >>> split_prefix("I_VERY_LONG_NAME")
-    ('I_', 'VERY_LONG_NAME')
-    >>> split_prefix("BT_VERY_LONG_NAME")
-    ('BT_', 'VERY_LONG_NAME')
-    >>> split_prefix("")
-    ('', '')
+    Args:
+        name: Name.
 
-    The counterpart to this function is `join_names`.
+    Returns:
+        tuple: Tuple of Prefix and Basename
+
+    ??? Example "split_prefix Examples"
+        Example:
+
+            >>> split_prefix("i_count")
+            ('i_', 'count')
+            >>> split_prefix("u_count")
+            ('u_', 'count')
+            >>> split_prefix("I_VERY_LONG_NAME")
+            ('I_', 'VERY_LONG_NAME')
+            >>> split_prefix("BT_VERY_LONG_NAME")
+            ('BT_', 'VERY_LONG_NAME')
+            >>> split_prefix("")
+            ('', '')
+
+            The counterpart to this function is `join_names`.
     """
     mat = _RE_SPLIT_PREFIX.match(name)
     if mat:
         return mat.group("prefix", "basename")  # type: ignore[return-value]
     return "", name
 
 
 @functools.lru_cache
 def split_suffix(name: str, suffixes=None) -> tuple[str, str]:
     """
     Split Name Into Basename And Suffix.
 
-    >>> split_suffix("count_i")
-    ('count', '_i')
-    >>> split_suffix("count_o")
-    ('count', '_o')
-    >>> split_suffix("count_io")
-    ('count', '_io')
-    >>> split_suffix("count_t")
-    ('count', '_t')
-    >>> split_suffix("count_s")
-    ('count', '_s')
-    >>> split_suffix("_s")
-    ('', '_s')
-    >>> split_suffix("very_long_name_s")
-    ('very_long_name', '_s')
-    >>> split_suffix("VERY_LONG_NAME_S")
-    ('VERY_LONG_NAME', '_S')
-    >>> split_suffix("")
-    ('', '')
+    Args:
+        name: Name.
+
+    Keyword Args:
+        suffixes: Suffixes.
+
+    Returns:
+        tuple: Tuple of Basename and Suffix
+
+    ??? Example "split_suffix Examples"
+        Example:
+
+            >>> split_suffix("count_i")
+            ('count', '_i')
+            >>> split_suffix("count_o")
+            ('count', '_o')
+            >>> split_suffix("count_io")
+            ('count', '_io')
+            >>> split_suffix("count_t")
+            ('count', '_t')
+            >>> split_suffix("count_s")
+            ('count', '_s')
+            >>> split_suffix("_s")
+            ('', '_s')
+            >>> split_suffix("very_long_name_s")
+            ('very_long_name', '_s')
+            >>> split_suffix("VERY_LONG_NAME_S")
+            ('VERY_LONG_NAME', '_S')
+            >>> split_suffix("")
+            ('', '')
 
-    The counterpart to this function is `join_names`.
+            The counterpart to this function is `join_names`.
     """
     mat = _RE_SPLIT_SUFFIX.match(name)
     if mat:
         return mat.group("basename", "suffix")  # type: ignore[return-value]
     return name, ""
 
 
 def join_names(*names, concat="_") -> str:
     """
     Join Names.
 
-    >>> join_names('foo', 'bar')
-    'foo_bar'
-    >>> join_names('', 'bar')
-    'bar'
-    >>> join_names('foo', '')
-    'foo'
+    Args:
+        names: Names.
+
+    Keyword Args:
+        concat: concat.
+
+    ??? Example "join_names Examples"
+        Example:
+
+            >>> join_names('foo', 'bar')
+            'foo_bar'
+            >>> join_names('', 'bar')
+            'bar'
+            >>> join_names('foo', '')
+            'foo'
 
     This function is the counterpart to `split_names`.
     """
     return concat.join(name for name in names if name)
 
 
 def didyoumean(name, names, known=False, multiline=False) -> str:
     """
     Propose matching names.
 
-    >>> didyoumean('abb', tuple())
-    ''
-    >>> didyoumean('abb', ('abba', 'ac/dc', 'beatles'), known=True)
-    " Known are 'abba', 'ac/dc' and 'beatles'. Did you mean 'abba'?"
-    >>> print(didyoumean('zz-top', ('abba', 'ac/dc', 'beatles'), known=True, multiline=True))
-    <BLANKLINE>
-    Known are 'abba', 'ac/dc' and 'beatles'.
+    Args:
+        name: Name.
+        names: Names.
+
+    Keyword Args:
+        known: Show known strings.
+        multiline: Add new line
+
+    ??? Example "didyoumean Examples"
+        Example:
+
+            >>> didyoumean('abb', tuple())
+            ''
+            >>> didyoumean('abb', ('abba', 'ac/dc', 'beatles'), known=True)
+            " Known are 'abba', 'ac/dc' and 'beatles'. Did you mean 'abba'?"
+            >>> print(didyoumean('zz-top', ('abba', 'ac/dc', 'beatles'), known=True, multiline=True))
+            <BLANKLINE>
+            Known are 'abba', 'ac/dc' and 'beatles'.
     """
     sep = "\n" if multiline else " "
     if known:
         knowns = concatenate(repr(name) for name in names)
         msg = f"{sep}Known are {knowns}."
     else:
         msg = ""
@@ -138,37 +179,46 @@
     return msg
 
 
 def get_snakecasename(item):
     """
     Get snakecase name of `cls`.
 
-    >>> class MyClass:
-    ...     pass
-    >>> get_snakecasename(MyClass)
-    'my_class'
-    >>> get_snakecasename("MyClass")
-    'my_class'
-    >>> get_snakecasename("MYClass")
-    'myclass'
+    ??? Example "get_snakecasename Examples"
+        Example:
+
+            >>> class MyClass:
+            ...     pass
+            >>> get_snakecasename(MyClass)
+            'my_class'
+            >>> get_snakecasename("MyClass")
+            'my_class'
+            >>> get_snakecasename("MYClass")
+            'myclass'
     """
     if not isinstance(item, str):
         item = item.__name__
     return snakecase(item).removeprefix("_")
 
 
 def str2identifier(value: str) -> str:
     """
     Convert Any String To Identifier.
 
-    >>> str2identifier('A B C')
-    'a_b_c'
-    >>> str2identifier('1 2 3')
-    'v1_2_3'
-    >>> str2identifier('12.3')
-    'v123'
+    Args:
+        value: Any String
+
+    ??? Example "str2identifier Examples"
+        Example:
+
+            >>> str2identifier('A B C')
+            'a_b_c'
+            >>> str2identifier('1 2 3')
+            'v1_2_3'
+            >>> str2identifier('12.3')
+            'v123'
     """
     value = snakecase(value)
     mat = _RE_STARTNUM.match(value)
     if mat:
         value = f"v{value}"
     return value
```

### Comparing `ucdp-0.2.0/src/ucdp/note.py` & `ucdp-0.3.0/src/ucdp/note.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,8 +27,11 @@
     note: str
 
     def __str__(self):
         return self.note
 
 
 OPEN = Note(note="OPEN")
+""" Open Note."""
+
 TODO = Note(note="TODO")
+""" Todo Note."""
```

### Comparing `ucdp-0.2.0/src/ucdp/object.py` & `ucdp-0.3.0/src/ucdp/object.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 
 Field = pyd.Field
 PrivateField = pyd.PrivateAttr
 ConfigDict = pyd.ConfigDict
 model_validator = pyd.model_validator
 computed_field = pyd.computed_field
 
+_CACHED_INSTANCES: int = 0
+
 
 class Object(pyd.BaseModel):
     """Read-Only :any:`pydantic` Base Model."""
 
     model_config = pyd.ConfigDict(
         extra="forbid",
         frozen=True,
@@ -92,14 +94,16 @@
     def __call__(self, *args, **kwargs):
         """Create New Instance or Return Existing One."""
         key = (self, *args, *sorted(kwargs.items()))
         try:
             try:
                 inst = self._cache[key]
             except KeyError:
+                global _CACHED_INSTANCES  # noqa: PLW0603
+                _CACHED_INSTANCES += 1
                 inst = self._cache[key] = super().__call__(*args, **kwargs)
         except TypeError as exc:
             try:
                 hash(self)
             except TypeError:
                 raise TypeError(f"{self} is not constant.") from None
             # Determine what caused TypeError
@@ -137,17 +141,14 @@
 
 
 class NamedLightObject(NamedObject, Light):
     """Cacheable NamedObject.
 
     Attributes:
         name: Name.
-
-    ???+ bug "Todo"
-        * fix inherited_members / Attributes Types
     """
 
 
 def get_repr(obj):
     """DOCME."""
     posargs = obj._posargs
     model_fields_set = obj.model_fields_set
```

### Comparing `ucdp-0.2.0/src/ucdp/orientation.py` & `ucdp-0.3.0/src/ucdp/orientation.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/param.py` & `ucdp-0.3.0/src/ucdp/param.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,54 +20,55 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """
 Module Parameter .
 
-Usage:
+??? Example "Parameter Examples"
+    Usage:
 
->>> from tabulate import tabulate
->>> import ucdp as u
->>> u.Param(u.UintType(6), "param_p")
-Param(UintType(6), 'param_p')
-
-Also complex types can simply be used:
-
->>> class AType(u.AStructType):
-...     def _build(self) -> None:
-...         self._add("req", u.BitType())
-...         self._add("data", u.ArrayType(u.UintType(16), 5))
-...         self._add("ack", u.BitType(), u.BWD)
->>> class MType(u.AEnumType):
-...     keytype: u.AScalarType = u.UintType(2)
-...     def _build(self) -> None:
-...         self._add(0, "Linear")
-...         self._add(1, "Cyclic")
->>> class BType(u.AStructType):
-...     def _build(self) -> None:
-...         self._add("foo", AType())
-...         self._add("mode", MType())
-...         self._add("bar", u.ArrayType(AType(), 3), u.BWD)
-
-These types are automatically resolved by iterating over the parameter:
-
->>> param = u.Param(BType(), "param_p")
->>> for item in param:
-...     print(repr(item))
-Param(BType(), 'param_p')
-Param(AType(), 'param_foo_p')
-Param(BitType(), 'param_foo_req_p')
-Param(ArrayType(UintType(16), 5), 'param_foo_data_p')
-Param(BitType(), 'param_foo_ack_p')
-Param(MType(), 'param_mode_p')
-Param(ArrayType(AType(), 3), 'param_bar_p')
-Param(ArrayType(BitType(), 3), 'param_bar_ack_p')
-Param(ArrayType(ArrayType(UintType(16), 5), 3), 'param_bar_data_p')
-Param(ArrayType(BitType(), 3), 'param_bar_req_p')
+        >>> from tabulate import tabulate
+        >>> import ucdp as u
+        >>> u.Param(u.UintType(6), "param_p")
+        Param(UintType(6), 'param_p')
+
+        Also complex types can simply be used:
+
+        >>> class AType(u.AStructType):
+        ...     def _build(self) -> None:
+        ...         self._add("req", u.BitType())
+        ...         self._add("data", u.ArrayType(u.UintType(16), 5))
+        ...         self._add("ack", u.BitType(), u.BWD)
+        >>> class MType(u.AEnumType):
+        ...     keytype: u.AScalarType = u.UintType(2)
+        ...     def _build(self) -> None:
+        ...         self._add(0, "Linear")
+        ...         self._add(1, "Cyclic")
+        >>> class BType(u.AStructType):
+        ...     def _build(self) -> None:
+        ...         self._add("foo", AType())
+        ...         self._add("mode", MType())
+        ...         self._add("bar", u.ArrayType(AType(), 3), u.BWD)
+
+    These types are automatically resolved by iterating over the parameter:
+
+        >>> param = u.Param(BType(), "param_p")
+        >>> for item in param:
+        ...     print(repr(item))
+        Param(BType(), 'param_p')
+        Param(AType(), 'param_foo_p')
+        Param(BitType(), 'param_foo_req_p')
+        Param(ArrayType(UintType(16), 5), 'param_foo_data_p')
+        Param(BitType(), 'param_foo_ack_p')
+        Param(MType(), 'param_mode_p')
+        Param(ArrayType(AType(), 3), 'param_bar_p')
+        Param(ArrayType(BitType(), 3), 'param_bar_ack_p')
+        Param(ArrayType(ArrayType(UintType(16), 5), 3), 'param_bar_data_p')
+        Param(ArrayType(BitType(), 3), 'param_bar_req_p')
 """
 
 from collections.abc import Iterator
 from typing import Any
 
 from .ident import Ident, _iters
 
@@ -80,43 +81,48 @@
         type_ (AType): Type.
         name (Name()): Name.
 
     Keyword Args:
         doc (Doc): Documentation Container
         value: Value.
 
-    Parameter names should end with '_p', but must not.
 
-    >>> import ucdp as u
-    >>> cnt = u.Param(u.UintType(6), "cnt_p")
-    >>> cnt
-    Param(UintType(6), 'cnt_p')
-    >>> cnt.type_
-    UintType(6)
-    >>> cnt.name
-    'cnt_p'
-    >>> cnt.basename
-    'cnt'
-    >>> cnt.suffix
-    '_p'
-    >>> cnt.doc
-    Doc()
-    >>> cnt.value
-
-    If the parameter is casted via `int()` it returns `value` if set, other `type_.default`.
-
-    >>> int(u.Param(u.UintType(6, default=2), "cnt_p"))
-    2
-    >>> int(u.Param(u.UintType(6, default=2), "cnt_p", value=4))
-    4
+    Note:
+        Parameter names should end with '_p', but must not.
 
-    Parameter are Singleton:
+    ??? Example "Param Examples"
+        Example:
 
-    >>> u.Param(u.UintType(6), "cnt_p") is u.Param(u.UintType(6), "cnt_p")
-    True
+            >>> import ucdp as u
+            >>> cnt = u.Param(u.UintType(6), "cnt_p")
+            >>> cnt
+            Param(UintType(6), 'cnt_p')
+            >>> cnt.type_
+            UintType(6)
+            >>> cnt.name
+            'cnt_p'
+            >>> cnt.basename
+            'cnt'
+            >>> cnt.suffix
+            '_p'
+            >>> cnt.doc
+            Doc()
+            >>> cnt.value
+
+        If the parameter is casted via `int()` it returns `value` if set, other `type_.default`.
+
+            >>> int(u.Param(u.UintType(6, default=2), "cnt_p"))
+            2
+            >>> int(u.Param(u.UintType(6, default=2), "cnt_p", value=4))
+            4
+
+        Parameter are Singleton:
+
+            >>> u.Param(u.UintType(6), "cnt_p") is u.Param(u.UintType(6), "cnt_p")
+            True
     """
 
     value: Any = None
 
     def __int__(self):
         value = self.value
         if value is None:
```

### Comparing `ucdp-0.2.0/src/ucdp/pathutil.py` & `ucdp-0.3.0/src/ucdp/pathutil.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/routepath.py` & `ucdp-0.3.0/src/ucdp/routepath.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/signal.py` & `ucdp-0.3.0/src/ucdp/signal.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,16 +106,14 @@
         name: Name.
 
     Attributes:
         direction: Direction.
         doc: Documentation Container
         ifdef: IFDEF encapsulation
 
-    ???+ bug "Todo"
-        * fix inherited_members / Attributes Types
     """
 
     direction: AOrientation = FWD
 
 
 class Signal(BaseSignal):
     """
@@ -126,17 +124,14 @@
         name: Name.
 
     Attributes:
         direction: Direction.
         doc: Documentation Container
         ifdef: IFDEF encapsulation
 
-    ???+ bug "Todo"
-        * fix inherited_members / Attributes Types
-
     ??? Example "Signal Examples"
         Examples.
 
             >>> import ucdp as u
             >>> count = u.Signal(u.UintType(6), "count_s")
             >>> count
             Signal(UintType(6), 'count_s')
@@ -170,17 +165,14 @@
         name: Name.
 
     Attributes:
         direction: Direction.
         doc: Documentation Container
         ifdef: IFDEF encapsulation
 
-    ???+ bug "Todo"
-        * fix inherited_members / Attributes Types
-
     ??? Example "Port Examples"
         Examples.
 
             >>> import ucdp as u
             >>> count = u.Port(u.UintType(6), "count_i")
             >>> count
             Port(UintType(6), 'count_i', direction=IN)
```

### Comparing `ucdp-0.2.0/src/ucdp/slices.py` & `ucdp-0.3.0/src/ucdp/slices.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     '9:6'
     >>> s.mask
     960
     >>> s.direction
     <SliceDirection.DOWN: 0>
     >>> s.slice
     slice(9, 6, -1)
+    >>> tuple(s)
+    (9, 8, 7, 6)
 
     >>> s = Slice(left=6, right=9)
     >>> s
     Slice('6:9')
     >>> s.left
     6
     >>> s.right
@@ -79,14 +81,16 @@
     '6:9'
     >>> s.mask
     960
     >>> s.direction
     <SliceDirection.UP: 1>
     >>> s.slice
     slice(6, 9, 1)
+    >>> tuple(s)
+    (6, 7, 8, 9)
 
     >>> Slice(left=7, right=4) in Slice(left=7, right=4)
     True
     >>> Slice(left=7, right=5) in Slice(left=7, right=4)
     True
     >>> Slice(left=6, right=4) in Slice(left=7, right=4)
     True
@@ -284,7 +288,13 @@
             direction = self.direction
             otherdirection = other.direction
             if direction and otherdirection and direction != otherdirection:
                 return False
             mask = self.mask
             return mask == mask | other.mask
         return NotImplemented
+
+    def __iter__(self):
+        if self.left > self.right:
+            yield from range(self.left, self.right - 1, -1)
+        else:
+            yield from range(self.left, self.right + 1, 1)
```

### Comparing `ucdp-0.2.0/src/ucdp/test.py` & `ucdp-0.3.0/src/ucdp/test.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/top.py` & `ucdp-0.3.0/src/ucdp/top.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 """Top."""
 
 from .iterutil import Names
 from .modbase import BaseMod
 from .moditer import ModPostIter, ModPreIter, get_mod, get_mods
 from .modtopref import TopModRef
-from .object import Field, Object
+from .object import _CACHED_INSTANCES, Field, Object
 
 
 class Top(Object):
     """
     Top Module Reference.
 
     Args:
@@ -75,7 +75,15 @@
 
         Iterate over `mod` and all its submodules and return matching one.
 
         Keyword Args:
             namepats: Iterable with name pattern (including `*` and `?`) or comma separated string
         """
         return get_mod(self.mod, namepats)
+
+    def get_stat(self) -> dict[str, int]:
+        """Get Statistics."""
+        return {
+            "Modules": len(self.get_mods(unique=True)),
+            "Module-Instances": len(self.get_mods()),
+            "LightObjects": _CACHED_INSTANCES,
+        }
```

### Comparing `ucdp-0.2.0/src/ucdp/typearray.py` & `ucdp-0.3.0/src/ucdp/typearray.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/typebase.py` & `ucdp-0.3.0/src/ucdp/typebase.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,12 +183,16 @@
 
     def __init__(self, width, **kwargs):
         super().__init__(width=width, **kwargs)
 
     @property
     def slice_(self):
         """Slice."""
-        return Slice(left=self.right + self.width - 1, right=self.right)
+        right = self.right
+        # Ensure slim expressions
+        if isinstance(right, int) and right == 0:
+            return Slice(left=self.width - 1, right=0)
+        return Slice(left=right + self.width - 1, right=right)
 
 
 class ACompositeType(BaseType):
     """Base Class For All Composite Types."""
```

### Comparing `ucdp-0.2.0/src/ucdp/typeclkrst.py` & `ucdp-0.3.0/src/ucdp/typeclkrst.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/typedescriptivestruct.py` & `ucdp-0.3.0/src/ucdp/typedescriptivestruct.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/typeenum.py` & `ucdp-0.3.0/src/ucdp/typeenum.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/typescalar.py` & `ucdp-0.3.0/src/ucdp/typescalar.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/typestring.py` & `ucdp-0.3.0/src/ucdp/typestring.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/src/ucdp/typestruct.py` & `ucdp-0.3.0/src/ucdp/typestruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,21 @@
 
 
 class StructItem(Object):
     """
     Struct NamedObject.
 
     Args:
-        name (str): Name of struct member
-        type_ (AType): Type of struct member
+        name: Name of struct member
+        type_: Type of struct member
 
     Keyword Args:
-        orient (Orient): Orientation of struct member. `FWD` by default
-        doc (Doc): Documentation Container
-        ifdef (str): IFDEF encapsulation
+        orientation: Orientation of struct member. `FWD` by default
+        doc: Documentation Container
+        ifdef: IFDEF encapsulation
     """
 
     name: str = Field(pattern=PAT_IDENTIFIER)
     type_: BaseType
     orientation: Orientation = FWD
     doc: Doc = Doc()
     ifdef: str | None = None
```

### Comparing `ucdp-0.2.0/src/ucdp/util.py` & `ucdp-0.3.0/src/ucdp/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,13 +28,20 @@
 from collections.abc import Iterable
 from contextlib import contextmanager
 from pathlib import Path
 
 
 @contextmanager
 def extend_sys_path(paths: Iterable[Path]):
-    """Context with extended sys.path."""
+    """Context with extended sys.path.
+
+    Args:
+        paths: Paths
+    """
     pathstrs = [str(path) for path in paths]
-    orig = sys.path
-    sys.path = [*sys.path, *pathstrs]
-    yield
-    sys.path = orig
+    if pathstrs:
+        orig = sys.path
+        sys.path = [*sys.path, *pathstrs]
+        yield
+        sys.path = orig
+    else:
+        yield
```

### Comparing `ucdp-0.2.0/tests/conftest.py` & `ucdp-0.3.0/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,7 +26,15 @@
 
 @fixture
 def example_filelist():
     """Add access to ``examples/filelist``."""
     example_path = EXAMPLES_PATH / "filelist"
     with u.extend_sys_path((example_path,)):
         yield example_path
+
+
+@fixture
+def example_param():
+    """Add access to ``examples/param``."""
+    example_path = EXAMPLES_PATH / "param"
+    with u.extend_sys_path((example_path,)):
+        yield example_path
```

### Comparing `ucdp-0.2.0/tests/test_assigns.py` & `ucdp-0.3.0/tests/test_assigns.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,31 +305,31 @@
 # #     assigns = u.Assigns(ports, signals, inst=True)
 # #     assigns.set(ports["vec_a_i"][4:3], ports["vec_d_o"][3:2])
 # #     assigns.set(ports["vec_b_o"][6:3], ports["vec_c_o"])
 # #     assigns.set(ports["vec_b_o"][12:9], ports["vec_c_o"])
 # #     assert_assigns(tmp_path, "test_assign_inst", assigns)
 
 
-def test_top_dir_err(top):
-    """Top - Direction Error."""
-    drivers = u.Drivers()
-    assigns = u.Assigns(targets=top, sources=top, drivers=drivers)
-
-    # top-input MUST NOT drive from top-input
-    with raises(u.DirectionError) as exc:
-        assigns.set(top["port_i"], top["other_i"])
-    assert str(exc.value) == "Cannot connect IN 'port_i' and IN 'other_i'"
-
-    # top-output MUST NOT drive output top-output
-    with raises(u.DirectionError) as exc:
-        assigns.set(top["port_o"], top["other_o"])
-    assert str(exc.value) == "Cannot connect OUT 'port_o' and OUT 'other_o'"
+# def test_top_dir_err(top):
+#     """Top - Direction Error."""
+#     drivers = u.Drivers()
+#     assigns = u.Assigns(targets=top, sources=top, drivers=drivers)
+
+#     # top-input MUST NOT drive from top-input
+#     with raises(u.DirectionError) as exc:
+#         assigns.set(top["port_i"], top["other_i"])
+#     assert str(exc.value) == "Cannot connect IN 'port_i' and IN 'other_i'"
+
+#     # top-output MUST NOT drive output top-output
+#     with raises(u.DirectionError) as exc:
+#         assigns.set(top["port_o"], top["other_o"])
+#     assert str(exc.value) == "Cannot connect OUT 'port_o' and OUT 'other_o'"
 
-    # Drivers not modified
-    assert tuple(drivers) == ()
+#     # Drivers not modified
+#     assert tuple(drivers) == ()
 
 
 def test_top_in(top):
     """Top - Input."""
     drivers = u.Drivers()
     assigns = u.Assigns(targets=top, sources=top, drivers=drivers)
     assigns.set(top["port_i"], top["port_o"])
@@ -376,31 +376,31 @@
         "port_my0_mode_o: port_my0_mode_i",
         "port_my0_send_o: port_my0_send_i",
         "port_my1_return_o: port_my1_return_i",
         "port_uint_o: port_uint_i",
     )
 
 
-def test_top_sub_dir_err(top, sub):
-    """Top with Sub - Direction Error."""
-    drivers = u.Drivers()
-    assigns = u.Assigns(targets=sub, sources=top, sub=True, drivers=drivers)
-
-    # sub-output MUST NOT drive against top-input
-    with raises(u.DirectionError) as exc:
-        assigns.set(sub["sub_o"], top["port_i"])
-    assert str(exc.value) == "Cannot connect sub-level OUT 'sub_o' and IN 'port_i'"
-
-    # sub-input MUST NOT drive from top-output
-    with raises(u.DirectionError) as exc:
-        assigns.set(sub["sub_i"], top["port_o"])
-    assert str(exc.value) == "Cannot connect sub-level IN 'sub_i' and OUT 'port_o'"
+# def test_top_sub_dir_err(top, sub):
+#     """Top with Sub - Direction Error."""
+#     drivers = u.Drivers()
+#     assigns = u.Assigns(targets=sub, sources=top, sub=True, drivers=drivers)
+
+#     # sub-output MUST NOT drive against top-input
+#     with raises(u.DirectionError) as exc:
+#         assigns.set(sub["sub_o"], top["port_i"])
+#     assert str(exc.value) == "Cannot connect sub-level OUT 'sub_o' and IN 'port_i'"
+
+#     # sub-input MUST NOT drive from top-output
+#     with raises(u.DirectionError) as exc:
+#         assigns.set(sub["sub_i"], top["port_o"])
+#     assert str(exc.value) == "Cannot connect sub-level IN 'sub_i' and OUT 'port_o'"
 
-    assert [str(assign) for assign in assigns] == []
-    assert tuple(f"{name}: {driver}" for name, driver in drivers) == ()
+#     assert [str(assign) for assign in assigns] == []
+#     assert tuple(f"{name}: {driver}" for name, driver in drivers) == ()
 
 
 def test_top_sub_in(top, sub):
     """Top with Sub - Input."""
     drivers = u.Drivers()
     assigns = u.Assigns(targets=sub, sources=top, sub=True, drivers=drivers)
     assigns.set(sub["sub_i"], top["port_i"])
```

### Comparing `ucdp-0.2.0/tests/test_baseclassinfo.py` & `ucdp-0.3.0/tests/test_baseclassinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,31 +25,31 @@
 
 import pydantic
 import ucdp as u
 
 
 def test_example_simple(example_simple):
     """Example."""
-    from glbl.clk_gate import ClkGateMod
-    from uart.uart import UartMod
+    from glbl_lib.clk_gate import ClkGateMod
+    from uart_lib.uart import UartMod
 
     assert tuple(u.get_baseclassinfos(UartMod)) == (
-        u.BaseClassInfo(cls=UartMod, libname="uart", modname="uart", clsname="UartMod"),
+        u.BaseClassInfo(cls=UartMod, libname="uart_lib", modname="uart", clsname="UartMod"),
         u.BaseClassInfo(cls=u.AMod, libname="ucdp", modname="mod", clsname="AMod"),
         u.BaseClassInfo(cls=u.BaseTopMod, libname="ucdp", modname="modbasetop", clsname="BaseTopMod"),
         u.BaseClassInfo(cls=u.BaseMod, libname="ucdp", modname="modbase", clsname="BaseMod"),
         u.BaseClassInfo(cls=u.NamedObject, libname="ucdp", modname="object", clsname="NamedObject"),
         u.BaseClassInfo(cls=u.Object, libname="ucdp", modname="object", clsname="Object"),
         u.BaseClassInfo(cls=pydantic.main.BaseModel, libname="pydantic", modname="main", clsname="BaseModel"),
     )
 
     assert tuple(u.get_baseclassinfos(UartMod())) == tuple(u.get_baseclassinfos(UartMod))
 
     assert tuple(u.get_baseclassinfos(ClkGateMod)) == (
-        u.BaseClassInfo(cls=ClkGateMod, libname="glbl", modname="clk_gate", clsname="ClkGateMod"),
+        u.BaseClassInfo(cls=ClkGateMod, libname="glbl_lib", modname="clk_gate", clsname="ClkGateMod"),
         u.BaseClassInfo(cls=u.AMod, libname="ucdp", modname="mod", clsname="AMod"),
         u.BaseClassInfo(cls=u.BaseTopMod, libname="ucdp", modname="modbasetop", clsname="BaseTopMod"),
         u.BaseClassInfo(cls=u.BaseMod, libname="ucdp", modname="modbase", clsname="BaseMod"),
         u.BaseClassInfo(cls=u.NamedObject, libname="ucdp", modname="object", clsname="NamedObject"),
         u.BaseClassInfo(cls=u.Object, libname="ucdp", modname="object", clsname="Object"),
         u.BaseClassInfo(cls=pydantic.main.BaseModel, libname="pydantic", modname="main", clsname="BaseModel"),
     )
```

### Comparing `ucdp-0.2.0/tests/test_buildproduct.py` & `ucdp-0.3.0/tests/test_buildproduct.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/tests/test_config.py` & `ucdp-0.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/tests/test_exprparser.py` & `ucdp-0.3.0/tests/test_flipflop.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,29 +17,52 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-"""Test :any:`Object`."""
+"""Test Flip-Flop."""
 
 import ucdp as u
 from pytest import fixture
 
 
 @fixture
-def parser() -> u.ExprParser:
-    """Some Identifier."""
-    namespace = u.Idents(
+def idents():
+    """Some Ports."""
+    return u.Idents(
         [
-            u.Signal(u.UintType(16, default=15), "uint_s"),
-            u.Signal(u.SintType(16, default=-15), "sint_s"),
+            u.Port(u.ClkRstAnType(), "main_i"),
+            u.Port(u.UintType(8), "vec_a_i"),
+            u.Signal(u.UintType(8), "vec_a_s"),
+            u.Signal(u.UintType(4), "vec_b_s"),
+            u.Signal(u.UintType(4), "vec_c_s"),
         ]
     )
-    return u.ExprParser(namespace=namespace)
 
 
-def test_parse(parser):
-    """Parse."""
-    expr = parser.parse("uint_s[2]")
-    assert expr == u.SliceOp(u.Signal(u.UintType(16, default=15), "uint_s"), u.Slice("2"))
+def test_flipflop(idents):
+    """Basics."""
+    rst_an = u.Signal(u.RstAnType(), "rst_s")
+    clk = u.Signal(u.ClkType(), "clk_s")
+    flipflop = u.FlipFlop(targets=idents, sources=idents, rst_an=rst_an, clk=clk)
+
+    assert flipflop.rst_an is rst_an
+    assert flipflop.clk is clk
+    assert flipflop.rst is None
+    assert flipflop.ena is None
+
+    # TESTME: rst_an type error
+    # TESTME: clk type error
+
+
+def test_flipflop_rst(idents):
+    """Flip Flop with Reset."""
+
+    # TESTME:
+
+
+def test_flipflop_ena(idents):
+    """Flip Flop with Ena."""
+
+    # TESTME:
```

### Comparing `ucdp-0.2.0/tests/test_fileset.py` & `ucdp-0.3.0/tests/test_fileset.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,24 +24,25 @@
 """Test Module File Information."""
 
 import ucdp as u
 
 
 def test_basic(example_simple):
     """Basic Testing."""
-    from uart.uart import UartMod
+    from uart_lib.uart import UartMod
 
     mod = UartMod()
 
     info = u.FileSet.from_mod(mod, "hdl")
     assert info.target is None
     assert info.filepaths == (
-        u.LibPath(libname="glbl", path=example_simple / "src" / "glbl" / "clk_gate" / "rtl" / "clk_gate.sv"),
-        u.LibPath(libname="uart", path=example_simple / "src" / "uart" / "uart" / "rtl" / "uart_regf.sv"),
-        u.LibPath(libname="uart", path=example_simple / "src" / "uart" / "uart" / "rtl" / "uart.sv"),
+        u.LibPath(libname="glbl_lib", path=example_simple / "src" / "glbl_lib" / "clk_gate" / "rtl" / "clk_gate.sv"),
+        u.LibPath(libname="uart_lib", path=example_simple / "src" / "uart_lib" / "uart" / "rtl" / "uart_regf.sv"),
+        u.LibPath(libname="uart_lib", path=example_simple / "src" / "uart_lib" / "uart" / "rtl" / "uart_core.sv"),
+        u.LibPath(libname="uart_lib", path=example_simple / "src" / "uart_lib" / "uart" / "rtl" / "uart.sv"),
     )
-    assert info.incdirs == ()
+    assert info.inc_dirs == ()
 
     info = u.FileSet.from_mod(mod, "systemc")
     assert info.target is None
     assert info.filepaths == ()
-    assert info.incdirs == ()
+    assert info.inc_dirs == ()
```

### Comparing `ucdp-0.2.0/tests/test_light_object.py` & `ucdp-0.3.0/tests/test_light_object.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/tests/test_modfilelist.py` & `ucdp-0.3.0/tests/test_modfilelist.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,25 @@
 
 import ucdp as u
 
 
 def test_basic(example_simple):
     """Basic Testing."""
     from fileliststandard import HdlFileList
-    from uart.uart import UartMod
+    from uart_lib.uart import UartMod
 
     mod = UartMod()
 
-    filepath = example_simple / "src" / "uart" / "uart" / "rtl" / "uart.sv"
+    filepath = example_simple / "src" / "uart_lib" / "uart" / "rtl" / "uart.sv"
     modfilelist = u.resolve_modfilelist(mod, "hdl")
-    assert modfilelist == HdlFileList(gen="full", filepaths=(filepath,))
+    assert modfilelist == HdlFileList(
+        gen="full",
+        filepaths=(filepath,),
+        template_filepaths=(example_simple / "uart_lib" / "main.mako",),
+    )
 
 
 # def test_target(example_simple):
 #     """Basic Testing."""
 #     from glbl.clk_gate import ClkGateMod
 
 #     mod = ClkGateMod()
@@ -65,9 +69,9 @@
     assert u.resolve_modfilelist(mod, "hdl") == u.ModFileList(
         name="hdl",
         filepaths=(
             example_filelist / "filelist_lib" / "mod0.sv",
             example_filelist / "filelist_lib" / "sub" / "mod2.sv",
             example_filelist / "mod2.sv",
         ),
-        incdirs=(example_filelist / "filelist_lib" / "inc",),
+        inc_dirs=(example_filelist / "filelist_lib" / "inc",),
     )
```

### Comparing `ucdp-0.2.0/tests/test_mux.py` & `ucdp-0.3.0/tests/test_mux.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/tests/test_namespace.py` & `ucdp-0.3.0/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/tests/test_object.py` & `ucdp-0.3.0/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/tests/test_pathutil.py` & `ucdp-0.3.0/tests/test_pathutil.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/tests/test_typeenum.py` & `ucdp-0.3.0/tests/test_typeenum.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/tests/test_typescalar.py` & `ucdp-0.3.0/tests/test_typescalar.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/tests/test_typestruct.py` & `ucdp-0.3.0/tests/test_typestruct.py`

 * *Files identical despite different names*

### Comparing `ucdp-0.2.0/PKG-INFO` & `ucdp-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ucdp
-Version: 0.2.0
+Version: 0.3.0
 Summary: Unified Chip Design Platform
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/nbiotcloud/ucdp
 Project-URL: Documentation, https://ucdp.readthedocs.io/en/latest/
 Project-URL: Bug tracker, https://github.com/nbiotcloud/ucdp/issues
 Requires-Python: <4.0,>=3.10.0
 Requires-Dist: anytree>=2.12.1
 Requires-Dist: case-converter>=1.1.0
 Requires-Dist: click>=8.1.7
 Requires-Dist: fuzzywuzzy>=0.18.0
 Requires-Dist: humannum>=1.0.0
 Requires-Dist: icdutil>=0.3.1
-Requires-Dist: makolator>=2.4.0
+Requires-Dist: makolator>=2.6.0
 Requires-Dist: matchor>=0.1.0
 Requires-Dist: pydantic>=2.7.0
 Requires-Dist: python-Levenshtein>=0.25.1
 Requires-Dist: rich>=13.7.1
 Requires-Dist: uniquer>=1.0.2
 Description-Content-Type: text/markdown
```

