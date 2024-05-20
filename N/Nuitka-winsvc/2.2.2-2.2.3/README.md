# Comparing `tmp/nuitka_winsvc-2.2.2.tar.gz` & `tmp/nuitka_winsvc-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuitka_winsvc-2.2.2.tar", last modified: Wed May 15 06:23:06 2024, max compression
+gzip compressed data, was "nuitka_winsvc-2.2.3.tar", last modified: Mon May 20 02:47:27 2024, max compression
```

## Comparing `nuitka_winsvc-2.2.2.tar` & `nuitka_winsvc-2.2.3.tar`

### file list

```diff
@@ -1,1842 +1,1842 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.351518 nuitka_winsvc-2.2.2/
--rw-rw-rw-   0        0        0      235 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/Changelog.rst
--rw-rw-rw-   0        0        0   152288 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/Developer_Manual.rst
--rw-rw-rw-   0        0        0    11348 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1717 2024-05-15 06:22:00.000000 nuitka_winsvc-2.2.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.349517 nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/
--rw-rw-rw-   0        0        0     4853 2024-05-15 06:23:01.000000 nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    78230 2024-05-15 06:23:02.000000 nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 06:23:01.000000 nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      308 2024-05-15 06:23:01.000000 nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-02-05 02:20:24.000000 nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-05-15 06:23:01.000000 nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 06:23:01.000000 nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4853 2024-05-15 06:23:06.350518 nuitka_winsvc-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2860 2024-05-15 06:22:00.000000 nuitka_winsvc-2.2.2/README.md
--rw-rw-rw-   0        0        0    80812 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.278480 nuitka_winsvc-2.2.2/bin/
--rw-rw-rw-   0        0        0     1166 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/bin/autoformat-nuitka-source
--rw-rw-rw-   0        0        0     1165 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/bin/check-nuitka-with-pylint
--rw-rw-rw-   0        0        0     1181 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/bin/compare_with_cpython
--rw-rw-rw-   0        0        0     3105 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/bin/compare_with_xml
--rw-rw-rw-   0        0        0     1194 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/bin/measure-construct-performance
--rw-rw-rw-   0        0        0     1716 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/bin/nuitka
--rw-rw-rw-   0        0        0     1716 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/bin/nuitka-run
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.289480 nuitka_winsvc-2.2.2/doc/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.305720 nuitka_winsvc-2.2.2/doc/Logo/
--rw-rw-rw-   0        0        0     1797 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/doc/Logo/Nuitka-Logo-Horizontal.svg
--rw-rw-rw-   0        0        0     1553 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-rw-rw-   0        0        0     1793 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/doc/Logo/Nuitka-Logo-Vertical.svg
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.326258 nuitka_winsvc-2.2.2/doc/images/
--rw-rw-rw-   0        0        0     7585 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/doc/images/Nuitka-Logo-Horizontal.png
--rw-rw-rw-   0        0        0     4452 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/doc/images/Nuitka-Logo-Symbol.png
--rw-rw-rw-   0        0        0     9828 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/doc/images/Nuitka-Logo-Vertical.png
--rw-rw-rw-   0        0        0    33696 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/doc/nuitka-run.1
--rw-rw-rw-   0        0        0    33720 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/doc/nuitka.1
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.336025 nuitka_winsvc-2.2.2/lib/
--rw-rw-rw-   0        0        0     4640 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/lib/hints.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.346959 nuitka_winsvc-2.2.2/misc/
--rwxrwxrwx   0        0        0      924 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/misc/nuitka-run.bat
--rwxrwxrwx   0        0        0     1061 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/misc/nuitka.bat
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.376347 nuitka_winsvc-2.2.2/nuitka/
--rw-rw-rw-   0        0        0     7560 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/Builtins.py
--rw-rw-rw-   0        0        0     5787 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/BytecodeCaching.py
--rw-rw-rw-   0        0        0     3800 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/Bytecodes.py
--rw-rw-rw-   0        0        0     1855 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/CacheCleanup.py
--rw-rw-rw-   0        0        0    11181 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/Constants.py
--rw-rw-rw-   0        0        0     2570 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/Errors.py
--rw-rw-rw-   0        0        0    11098 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/HardImportRegistry.py
--rw-rw-rw-   0        0        0    38106 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/MainControl.py
--rw-rw-rw-   0        0        0     8616 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/ModuleRegistry.py
--rw-rw-rw-   0        0        0    64062 2024-05-15 06:22:00.000000 nuitka_winsvc-2.2.2/nuitka/OptionParsing.py
--rw-rw-rw-   0        0        0    76125 2024-05-15 06:22:00.000000 nuitka_winsvc-2.2.2/nuitka/Options.py
--rw-rw-rw-   0        0        0     5432 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/OutputDirectories.py
--rw-rw-rw-   0        0        0    15000 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/PostProcessing.py
--rw-rw-rw-   0        0        0     6805 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/Progress.py
--rw-rw-rw-   0        0        0     9654 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/PythonFlavors.py
--rw-rw-rw-   0        0        0     4093 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/PythonOperators.py
--rw-rw-rw-   0        0        0    14564 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/PythonVersions.py
--rw-rw-rw-   0        0        0     8989 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/Serialization.py
--rw-rw-rw-   0        0        0     4703 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/SourceCodeReferences.py
--rw-rw-rw-   0        0        0    13335 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/Tracing.py
--rw-rw-rw-   0        0        0     3512 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/TreeXML.py
--rw-rw-rw-   0        0        0    15470 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/Variables.py
--rw-rw-rw-   0        0        0     2466 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/Version.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/__main__.py
--rw-rw-rw-   0        0        0     5604 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/__past__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.397643 nuitka_winsvc-2.2.2/nuitka/build/
--rw-rw-rw-   0        0        0    36409 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/Backend.scons
--rw-rw-rw-   0        0        0     8583 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/CCompilerVersion.scons
--rw-rw-rw-   0        0        0     3486 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/DataComposerInterface.py
--rw-rw-rw-   0        0        0    17786 2024-05-15 06:22:00.000000 nuitka_winsvc-2.2.2/nuitka/build/Onefile.scons
--rw-rw-rw-   0        0        0    15361 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/SconsCaching.py
--rw-rw-rw-   0        0        0    35818 2024-05-15 06:22:00.000000 nuitka_winsvc-2.2.2/nuitka/build/SconsCompilerSettings.py
--rw-rw-rw-   0        0        0     5591 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/SconsHacks.py
--rw-rw-rw-   0        0        0    17868 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/SconsInterface.py
--rw-rw-rw-   0        0        0     2703 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/SconsProgress.py
--rw-rw-rw-   0        0        0    13210 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/SconsSpawn.py
--rw-rw-rw-   0        0        0    27035 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/SconsUtils.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.106320 nuitka_winsvc-2.2.2/nuitka/build/include/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.453642 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/
--rw-rw-rw-   0        0        0     8216 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/allocator.h
--rw-rw-rw-   0        0        0     3499 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/builtins.h
--rw-rw-rw-   0        0        0     5196 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/calling.h
--rw-rw-rw-   0        0        0     2006 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/checkers.h
--rw-rw-rw-   0        0        0     1123 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/checksum_tools.h
--rw-rw-rw-   0        0        0     9333 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-rw-rw-   0        0        0     2460 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_cell.h
--rw-rw-rw-   0        0        0     9233 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-rw-rw-   0        0        0    17661 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_frame.h
--rw-rw-rw-   0        0        0     7267 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_function.h
--rw-rw-rw-   0        0        0     9189 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_generator.h
--rw-rw-rw-   0        0        0     1866 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_method.h
--rw-rw-rw-   0        0        0     7688 2024-04-22 02:58:07.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/constants.h
--rw-rw-rw-   0        0        0     1345 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/constants_blob.h
--rw-rw-rw-   0        0        0     1187 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/environment_variables.h
--rw-rw-rw-   0        0        0     1872 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/environment_variables_system.h
--rw-rw-rw-   0        0        0     5302 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/exception_groups.h
--rw-rw-rw-   0        0        0    50867 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/exceptions.h
--rw-rw-rw-   0        0        0     3792 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/filesystem_paths.h
--rw-rw-rw-   0        0        0     6474 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/freelists.h
--rw-rw-rw-   0        0        0    86326 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/hedley.h
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.501546 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/
--rw-rw-rw-   0        0        0     3698 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/attributes.h
--rw-rw-rw-   0        0        0     2692 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/boolean.h
--rw-rw-rw-   0        0        0     1233 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-rw-rw-   0        0        0     1164 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/bytes.h
--rw-rw-rw-   0        0        0    11894 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-rw-rw-   0        0        0    13169 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-rw-rw-   0        0        0    10645 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-rw-rw-   0        0        0    10644 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-rw-rw-   0        0        0    13169 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-rw-rw-   0        0        0    13168 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-rw-rw-   0        0        0    10645 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-rw-rw-   0        0        0     1834 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/complex.h
--rw-rw-rw-   0        0        0    13606 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-rw-rw-   0        0        0     1235 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/floats.h
--rw-rw-rw-   0        0        0     4401 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/import_hard.h
--rw-rw-rw-   0        0        0     1827 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/indexes.h
--rw-rw-rw-   0        0        0     3625 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/ints.h
--rw-rw-rw-   0        0        0     9599 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/iterators.h
--rw-rw-rw-   0        0        0     3678 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/lists.h
--rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-rw-rw-   0        0        0     1386 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/mappings.h
--rw-rw-rw-   0        0        0     4671 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations.h
--rw-rw-rw-   0        0        0    12714 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-rw-rw-   0        0        0     5692 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-rw-rw-   0        0        0     5670 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-rw-rw-   0        0        0     5692 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-rw-rw-   0        0        0     5451 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-rw-rw-   0        0        0     5489 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-rw-rw-   0        0        0     5144 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-rw-rw-   0        0        0     2828 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-rw-rw-   0        0        0    15807 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-rw-rw-   0        0        0    13239 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-rw-rw-   0        0        0     5820 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-rw-rw-   0        0        0     4743 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-rw-rw-   0        0        0     5144 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-rw-rw-   0        0        0     5853 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-rw-rw-   0        0        0     5467 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-rw-rw-   0        0        0    20173 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-rw-rw-   0        0        0     8699 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-rw-rw-   0        0        0     3796 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-rw-rw-   0        0        0     3782 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-rw-rw-   0        0        0     3796 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-rw-rw-   0        0        0     4875 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-rw-rw-   0        0        0     2756 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-rw-rw-   0        0        0    10655 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-rw-rw-   0        0        0     9230 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-rw-rw-   0        0        0     5176 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-rw-rw-   0        0        0     4378 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-rw-rw-   0        0        0     5004 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-rw-rw-   0        0        0     4855 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-rw-rw-   0        0        0     4072 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/raising.h
--rw-rw-rw-   0        0        0     2367 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-rw-rw-   0        0        0     1175 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-rw-rw-   0        0        0     1141 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/sequences.h
--rw-rw-rw-   0        0        0     1054 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/sets.h
--rw-rw-rw-   0        0        0     8750 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/slices.h
--rw-rw-rw-   0        0        0     1363 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/strings.h
--rw-rw-rw-   0        0        0    17975 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/subscripts.h
--rw-rw-rw-   0        0        0     5926 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/tuples.h
--rw-rw-rw-   0        0        0    16773 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helpers.h
--rw-rw-rw-   0        0        0     6050 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/importing.h
--rw-rw-rw-   0        0        0    12979 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/incbin.h
--rw-rw-rw-   0        0        0     1086 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/jit_sources.h
--rw-rw-rw-   0        0        0    16556 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/prelude.h
--rw-rw-rw-   0        0        0     3239 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/printing.h
--rw-rw-rw-   0        0        0     1811 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/python_pgo.h
--rw-rw-rw-   0        0        0     2343 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/safe_string_ops.h
--rw-rw-rw-   0        0        0     3729 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/threading.h
--rw-rw-rw-   0        0        0     3447 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/tracing.h
--rw-rw-rw-   0        0        0     1145 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/type_aliases.h
--rw-rw-rw-   0        0        0     3135 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/unfreezing.h
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.138448 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.508560 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/appdirs/
--rw-rw-rw-   0        0        0     1097 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/appdirs/LICENSE.txt
--rw-rw-rw-   0        0        0    24824 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/appdirs/appdirs.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.510555 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/atomicwrites/
--rw-rw-rw-   0        0        0     1069 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-rw-rw-   0        0        0     6794 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.521578 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/bin/
--rw-rw-rw-   0        0        0     1695 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/bin/scons.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.107299 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/clcache/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.532379 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/clcache/clcache/
--rw-rw-rw-   0        0        0     1585 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-rw-rw-   0        0        0       93 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-rw-rw-   0        0        0    65424 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.534365 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/
--rw-rw-rw-   0        0        0     1491 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.536365 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/
--rw-rw-rw-   0        0        0      243 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-rw-rw-   0        0        0    10517 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.537366 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/
--rw-rw-rw-   0        0        0     1359 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.547380 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/glob2/
--rw-rw-rw-   0        0        0       82 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-rw-rw-   0        0        0     6859 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-rw-rw-   0        0        0     4463 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-rw-rw-   0        0        0     8304 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/glob2/impl.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.559121 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/
--rw-rw-rw-   0        0        0     1467 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/LICENSE.rst
--rw-rw-rw-   0        0        0       85 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.571965 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/
--rw-rw-rw-   0        0        0     2423 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17473 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.580991 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/
--rw-rw-rw-   0        0        0     1466 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
--rw-rw-rw-   0        0        0       84 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.593299 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-rw-rw-   0        0        0     2616 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17474 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.132960 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.125007 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.605033 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-rw-rw-   0        0        0    47844 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
--rw-rw-rw-   0        0        0    33996 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-rw-rw-   0        0        0     8083 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27693 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     6938 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    17622 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96183 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7358 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    21540 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16000 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9589 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.606033 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-rw-rw-   0        0        0     4197 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   121420 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     4164 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    49503 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.609039 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-rw-rw-   0        0        0     1965 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-rw-rw-   0        0        0     2736 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-rw-rw-   0        0        0     2614 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-rw-rw-   0        0        0     8467 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.614039 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-rw-rw-   0        0        0     9314 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3131 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     1989 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2483 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1718 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1605 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     2170 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4179 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1882 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0    15042 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    39700 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    12950 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.616040 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4810 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3751 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3233 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2011 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    14663 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.618867 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-rw-rw-   0        0        0    14029 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    52665 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    40719 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    24133 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14053 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-rw-rw-   0        0        0    34903 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    40510 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.657520 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2166 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0     2433 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-rw-rw-   0        0        0     2859 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-rw-rw-   0        0        0    18084 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.661182 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2078 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0     9248 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    14869 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    19499 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    20832 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     3763 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-rw-rw-   0        0        0     5149 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0     2290 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-rw-rw-   0        0        0     2328 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-rw-rw-   0        0        0     2657 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-rw-rw-   0        0        0    31283 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2267 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2681 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-rw-rw-   0        0        0     2720 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     2796 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2147 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2936 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2935 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     3432 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3785 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     2777 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1711 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-rw-rw-   0        0        0      142 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.661700 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29618 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3428 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     2681 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     2433 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-rw-rw-   0        0        0     1844 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3472 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     4782 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-rw-rw-   0        0        0     2025 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-rw-rw-   0        0        0     2256 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-rw-rw-   0        0        0     2460 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2639 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1810 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2333 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2140 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1902 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2077 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2043 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    18600 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25816 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     3328 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-rw-rw-   0        0        0     8394 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     3953 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2309 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2945 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     6919 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4381 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4658 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4224 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2168 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    13881 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1804 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    11380 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    72761 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6841 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3579 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2618 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4375 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2827 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2513 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1991 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1819 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2123 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2502 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     4695 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1927 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     2349 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2473 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     5992 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1831 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3730 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13016 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3415 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    48938 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.664831 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3007 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4380 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3557 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5612 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11034 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6824 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1563 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.670108 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-rw-rw-   0        0        0     8120 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     3596 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-rw-rw-   0        0        0     1818 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-rw-rw-   0        0        0     1742 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     2465 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-rw-rw-   0        0        0     1776 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-rw-rw-   0        0        0    19253 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-rw-rw-   0        0        0    44500 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-rw-rw-   0        0        0    19664 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     7509 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2107 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.129965 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.681582 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-rw-rw-   0        0        0    53545 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
--rw-rw-rw-   0        0        0    34985 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-rw-rw-   0        0        0    13596 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    28403 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7533 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    20988 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96818 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7752 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    22350 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16068 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9565 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.683579 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-rw-rw-   0        0        0     5239 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   135413 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     5758 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63474 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8354 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.689327 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-rw-rw-   0        0        0    11500 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3180 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2227 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2739 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1767 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1654 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1460 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2219 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4476 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1931 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     4003 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    17055 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41186 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    13880 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.691339 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4853 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3812 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3643 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2328 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15053 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.694477 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-rw-rw-   0        0        0    13779 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53260 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    39394 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26467 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14489 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    35863 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    42204 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.726870 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2211 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    18207 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.730785 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2152 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    10674 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2855 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15165 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    33537 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    21762 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4464 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    50660 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2316 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2475 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2840 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     8618 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2226 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2978 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2977 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1653 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3827 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3389 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.730785 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      313 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3631 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3444 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     8494 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1753 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.731797 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29765 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3472 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1630 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1977 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3686 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2580 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2948 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2655 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1645 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1859 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2765 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2386 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2189 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1944 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2123 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2085 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    15791 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    26195 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0    13924 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     4041 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2351 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2987 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     7808 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4956 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     5235 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4808 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2475 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14751 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1847 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12588 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    82939 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6883 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3663 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2660 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4904 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2877 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2567 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1652 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1868 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2088 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2176 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2366 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1658 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1976 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     5335 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2583 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2515 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6756 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1873 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3773 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13982 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3201 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    53803 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.735360 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3064 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3818 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4435 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3643 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5579 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11655 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6504 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1647 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.736358 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-rw-rw-   0        0        0     6869 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0    19816 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     9002 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2149 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.132960 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.747356 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-rw-rw-   0        0        0    56578 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-rw-rw-   0        0        0    35213 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
--rw-rw-rw-   0        0        0    11061 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27408 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7884 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-rw-rw-   0        0        0    21423 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-rw-rw-   0        0        0    97269 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-rw-rw-   0        0        0     3979 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
--rw-rw-rw-   0        0        0     7515 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-rw-rw-   0        0        0    21937 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-rw-rw-   0        0        0    16583 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-rw-rw-   0        0        0     9430 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.749105 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-rw-rw-   0        0        0     5126 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   136271 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     6167 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63768 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8183 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.756100 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-rw-rw-   0        0        0    12836 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2107 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2630 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1674 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1536 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1311 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2076 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4356 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1805 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     3860 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    14831 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41983 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-rw-rw-   0        0        0    14673 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.758702 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-rw-rw-   0        0        0     7394 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     4357 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3546 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     1972 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15577 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.760706 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-rw-rw-   0        0        0    13597 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53509 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    42760 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26676 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14272 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    36753 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-rw-rw-   0        0        0    41191 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.794608 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-rw-rw-   0        0        0     2122 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    15570 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.798451 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2014 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    13182 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2734 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15027 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    38783 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    22570 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4368 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    32724 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1578 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2228 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2386 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2616 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     7993 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2141 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     1661 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2893 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-rw-rw-   0        0        0     2889 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1567 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3742 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3296 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.798451 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      343 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3534 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3259 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     7461 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1663 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-rw-rw-   0        0        0     3379 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1544 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1891 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3616 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2377 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2437 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2526 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1557 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1772 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2677 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2206 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2096 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1851 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     1954 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     1995 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    19180 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25826 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     2588 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.801449 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-rw-rw-   0        0        0     4649 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-rw-rw-   0        0        0     7652 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-rw-rw-   0        0        0     6064 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-rw-rw-   0        0        0     3931 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2266 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2900 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     8622 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4577 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4517 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4113 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2387 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14473 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1752 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12902 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    84784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6788 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3576 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4817 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2788 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2479 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1563 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1780 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     1999 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2006 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2271 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1569 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1888 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     4879 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2419 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2429 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6412 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1786 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3687 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    12548 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     4076 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    71693 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.802447 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-rw-rw-   0        0        0     6632 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-rw-rw-   0        0        0    15278 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.805448 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-rw-rw-   0        0        0     3134 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3896 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4648 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3536 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5588 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    12708 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6785 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-rw-rw-   0        0        0      353 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.806448 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-rw-rw-   0        0        0     4307 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     3395 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-rw-rw-   0        0        0    21614 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-rw-rw-   0        0        0     9295 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-rw-rw-   0        0        0     2032 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.807448 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/
--rw-rw-rw-   0        0        0     1467 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.819463 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-rw-rw-   0        0        0    10126 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-rw-rw-   0        0        0      558 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-rw-rw-   0        0        0     4690 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-rw-rw-   0        0        0     1873 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.135968 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/pkg_resources/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.820467 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-rw-rw-   0        0        0   107335 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      538 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.135968 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.830747 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/
--rw-rw-rw-   0        0        0     1595 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-rw-rw-   0        0        0      283 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-rw-rw-   0        0        0     3687 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-rw-rw-   0        0        0      283 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-rw-rw-   0        0        0      307 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-rw-rw-   0        0        0      888 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-rw-rw-   0        0        0      596 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-rw-rw-   0        0        0     1106 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-rw-rw-   0        0        0      857 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-rw-rw-   0        0        0     1376 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-rw-rw-   0        0        0    10790 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-rw-rw-   0        0        0    57572 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-rw-rw-   0        0        0     6948 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/tk.py
--rw-rw-rw-   0        0        0     9726 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-rw-rw-   0        0        0       99 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/version.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.830747 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/
--rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.848584 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/
--rw-rw-rw-   0        0        0    13170 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-rw-rw-   0        0        0     4883 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-rw-rw-   0        0        0    28639 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-rw-rw-   0        0        0     3851 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2837 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/dumper.py
--rw-rw-rw-   0        0        0    43006 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-rw-rw-   0        0        0     2061 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-rw-rw-   0        0        0     6794 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-rw-rw-   0        0        0    14184 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-rw-rw-   0        0        0     8999 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-rw-rw-   0        0        0    51277 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.849583 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/
--rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.864410 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/
--rw-rw-rw-   0        0        0     9776 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-rw-rw-   0        0        0     4921 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-rw-rw-   0        0        0    25145 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-rw-rw-   0        0        0     3290 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2719 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
--rw-rw-rw-   0        0        0    43298 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-rw-rw-   0        0        0     2559 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-rw-rw-   0        0        0     1132 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-rw-rw-   0        0        0    25542 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-rw-rw-   0        0        0     6746 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-rw-rw-   0        0        0    17711 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-rw-rw-   0        0        0     9122 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-rw-rw-   0        0        0    52446 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-rw-rw-   0        0        0     4171 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.865408 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/
--rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.875417 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/
--rw-rw-rw-   0        0        0     9607 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-rw-rw-   0        0        0    25554 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-rw-rw-   0        0        0     3294 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2723 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
--rw-rw-rw-   0        0        0    42954 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-rw-rw-   0        0        0     1138 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-rw-rw-   0        0        0     6854 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-rw-rw-   0        0        0    14097 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-rw-rw-   0        0        0     8970 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-rw-rw-   0        0        0    51695 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.887171 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/
--rw-rw-rw-   0        0        0     1002 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/LICENSE
--rw-rw-rw-   0        0        0    31605 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/crc32.c
--rw-rw-rw-   0        0        0   591749 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/crc32.h
--rw-rw-rw-   0        0        0    16682 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/zconf.h
--rw-rw-rw-   0        0        0    96778 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/zlib.h
--rw-rw-rw-   0        0        0     7247 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/zutil.h
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.896085 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/
--rw-rw-rw-   0        0        0     1530 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.907094 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/
--rw-rw-rw-   0        0        0    18198 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-rw-rw-   0        0        0    10157 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/compiler.h
--rw-rw-rw-   0        0        0     4455 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-rw-rw-   0        0        0     3763 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/debug.h
--rw-rw-rw-   0        0        0    13662 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-rw-rw-   0        0        0     3009 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-rw-rw-   0        0        0     2441 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-rw-rw-   0        0        0    34422 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/fse.h
--rw-rw-rw-   0        0        0    14748 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-rw-rw-   0        0        0    20216 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/huf.h
--rw-rw-rw-   0        0        0    13930 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/mem.h
--rw-rw-rw-   0        0        0    26976 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-rw-rw-   0        0        0    11706 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-rw-rw-   0        0        0     2728 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-rw-rw-   0        0        0     2497 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-rw-rw-   0        0        0     3828 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-rw-rw-   0        0        0    15880 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/zstd_internal.h
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.911385 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/
--rw-rw-rw-   0        0        0    54982 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-rw-rw-   0        0        0     9164 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-rw-rw-   0        0        0     1321 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-rw-rw-   0        0        0    80283 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-rw-rw-   0        0        0    66784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-rw-rw-   0        0        0     2253 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-rw-rw-   0        0        0     7906 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-rw-rw-   0        0        0   138334 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/zstd.h
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.991952 nuitka_winsvc-2.2.2/nuitka/build/static_src/
--rw-rw-rw-   0        0        0    83526 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-rw-rw-   0        0        0     9142 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledCellType.c
--rw-rw-rw-   0        0        0    58846 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-rw-rw-   0        0        0    72002 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledCoroutineType.c
--rw-rw-rw-   0        0        0    40762 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledFrameType.c
--rw-rw-rw-   0        0        0   110213 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledFunctionType.c
--rw-rw-rw-   0        0        0    67599 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledGeneratorType.c
--rw-rw-rw-   0        0        0    56411 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-rw-rw-   0        0        0    22466 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledMethodType.c
--rw-rw-rw-   0        0        0    19054 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersAllocator.c
--rw-rw-rw-   0        0        0    37583 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersAttributes.c
--rw-rw-rw-   0        0        0    23690 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersBuiltin.c
--rw-rw-rw-   0        0        0   114017 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-rw-rw-   0        0        0     3062 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersBytes.c
--rw-rw-rw-   0        0        0    13376 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersCalling.c
--rw-rw-rw-   0        0        0   481627 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-rw-rw-   0        0        0     2065 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersChecksumTools.c
--rw-rw-rw-   0        0        0     3051 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersClasses.c
--rw-rw-rw-   0        0        0   318889 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonEq.c
--rw-rw-rw-   0        0        0     4762 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-rw-rw-   0        0        0   314072 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonGe.c
--rw-rw-rw-   0        0        0   313483 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonGt.c
--rw-rw-rw-   0        0        0   317286 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonLe.c
--rw-rw-rw-   0        0        0   316697 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonLt.c
--rw-rw-rw-   0        0        0   315637 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonNe.c
--rw-rw-rw-   0        0        0    36776 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-rw-rw-   0        0        0    20243 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersDeepcopy.c
--rw-rw-rw-   0        0        0    39785 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersDictionaries.c
--rw-rw-rw-   0        0        0    26620 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-rw-rw-   0        0        0     2066 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersDumpBacktraces.c
--rw-rw-rw-   0        0        0     2194 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersEnvironmentVariables.c
--rw-rw-rw-   0        0        0     2979 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c
--rw-rw-rw-   0        0        0     7966 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersExceptions.c
--rw-rw-rw-   0        0        0     8349 2024-04-22 02:58:07.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersFiles.c
--rw-rw-rw-   0        0        0    28776 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-rw-rw-   0        0        0     2455 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersFloats.c
--rw-rw-rw-   0        0        0     1803 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersHeapStorage.c
--rw-rw-rw-   0        0        0    16080 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersImport.c
--rw-rw-rw-   0        0        0    16843 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersImportHard.c
--rw-rw-rw-   0        0        0     1815 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersJitSources.c
--rw-rw-rw-   0        0        0    21107 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersLists.c
--rw-rw-rw-   0        0        0    13944 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersListsGenerated.c
--rw-rw-rw-   0        0        0     1669 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersMappings.c
--rw-rw-rw-   0        0        0     3587 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersMatching.c
--rw-rw-rw-   0        0        0   182227 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-rw-rw-   0        0        0    19904 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-rw-rw-   0        0        0    77972 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-rw-rw-   0        0        0    77811 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-rw-rw-   0        0        0    77972 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
--rw-rw-rw-   0        0        0    68218 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-rw-rw-   0        0        0     1265 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-rw-rw-   0        0        0    69479 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-rw-rw-   0        0        0     6300 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-rw-rw-   0        0        0    83954 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-rw-rw-   0        0        0    13805 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-rw-rw-   0        0        0   183867 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-rw-rw-   0        0        0   188543 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-rw-rw-   0        0        0     3593 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-rw-rw-   0        0        0    67184 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-rw-rw-   0        0        0    79484 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-rw-rw-   0        0        0     1052 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-rw-rw-   0        0        0    77854 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-rw-rw-   0        0        0    70851 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-rw-rw-   0        0        0    68736 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-rw-rw-   0        0        0   151107 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-rw-rw-   0        0        0     4242 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-rw-rw-   0        0        0    53253 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-rw-rw-   0        0        0    53151 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-rw-rw-   0        0        0    53253 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-rw-rw-   0        0        0    77119 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-rw-rw-   0        0        0    47857 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-rw-rw-   0        0        0    17771 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-rw-rw-   0        0        0   136385 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-rw-rw-   0        0        0   142240 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-rw-rw-   0        0        0    74749 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-rw-rw-   0        0        0    83262 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-rw-rw-   0        0        0    45341 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-rw-rw-   0        0        0    83275 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-rw-rw-   0        0        0    76950 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-rw-rw-   0        0        0     3294 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersProfiling.c
--rw-rw-rw-   0        0        0     3840 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersPythonPgo.c
--rw-rw-rw-   0        0        0    18257 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersRaising.c
--rw-rw-rw-   0        0        0     3868 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersSafeStrings.c
--rw-rw-rw-   0        0        0     3759 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersSequences.c
--rw-rw-rw-   0        0        0     1975 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersSlices.c
--rw-rw-rw-   0        0        0    32297 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersStrings.c
--rw-rw-rw-   0        0        0     4181 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersTuples.c
--rw-rw-rw-   0        0        0     6786 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersTypes.c
--rw-rw-rw-   0        0        0    12136 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/InspectPatcher.c
--rw-rw-rw-   0        0        0    54011 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/MainProgram.c
--rw-rw-rw-   0        0        0    63771 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-rw-rw-   0        0        0     4827 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-rw-rw-   0        0        0     6651 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-rw-rw-   0        0        0    21896 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-rw-rw-   0        0        0    37101 2024-05-15 06:22:00.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/OnefileBootstrap.c
--rw-rw-rw-   0        0        0     8050 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/build/static_src/OnefileSplashScreen.cpp
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.037817 nuitka_winsvc-2.2.2/nuitka/code_generation/
--rw-rw-rw-   0        0        0     6491 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/AsyncgenCodes.py
--rw-rw-rw-   0        0        0    10821 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/AttributeCodes.py
--rw-rw-rw-   0        0        0    21926 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-rw-rw-   0        0        0     2371 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/BranchCodes.py
--rw-rw-rw-   0        0        0    17006 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/BuiltinCodes.py
--rw-rw-rw-   0        0        0    36111 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/CallCodes.py
--rw-rw-rw-   0        0        0     4958 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ClassCodes.py
--rw-rw-rw-   0        0        0    53395 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/CodeGeneration.py
--rw-rw-rw-   0        0        0     2408 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/CodeHelperSelection.py
--rw-rw-rw-   0        0        0    14320 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/CodeHelpers.py
--rw-rw-rw-   0        0        0     5147 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/CodeObjectCodes.py
--rw-rw-rw-   0        0        0    17957 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ComparisonCodes.py
--rw-rw-rw-   0        0        0     4479 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-rw-rw-   0        0        0     7368 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ConditionalCodes.py
--rw-rw-rw-   0        0        0     6901 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ConstantCodes.py
--rw-rw-rw-   0        0        0    34299 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/Contexts.py
--rw-rw-rw-   0        0        0     8589 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/CoroutineCodes.py
--rw-rw-rw-   0        0        0     1607 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/CtypesCodes.py
--rw-rw-rw-   0        0        0    28934 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/DictCodes.py
--rw-rw-rw-   0        0        0     2159 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/Emission.py
--rw-rw-rw-   0        0        0     9289 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ErrorCodes.py
--rw-rw-rw-   0        0        0    12983 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/EvalCodes.py
--rw-rw-rw-   0        0        0     9243 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ExceptionCodes.py
--rw-rw-rw-   0        0        0     7384 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-rw-rw-   0        0        0     2126 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ExpressionCodes.py
--rw-rw-rw-   0        0        0    17852 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/FrameCodes.py
--rw-rw-rw-   0        0        0    28336 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/FunctionCodes.py
--rw-rw-rw-   0        0        0     7836 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/GeneratorCodes.py
--rw-rw-rw-   0        0        0     6363 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/GlobalConstants.py
--rw-rw-rw-   0        0        0     6985 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-rw-rw-   0        0        0     1870 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/IdCodes.py
--rw-rw-rw-   0        0        0    14727 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ImportCodes.py
--rw-rw-rw-   0        0        0     1429 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/Indentation.py
--rw-rw-rw-   0        0        0     1574 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/IndexCodes.py
--rw-rw-rw-   0        0        0     1066 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/InjectCCodes.py
--rw-rw-rw-   0        0        0     3567 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/IntegerCodes.py
--rw-rw-rw-   0        0        0    12211 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/IteratorCodes.py
--rw-rw-rw-   0        0        0     1620 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/JitCodes.py
--rw-rw-rw-   0        0        0     2055 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/LabelCodes.py
--rw-rw-rw-   0        0        0     2645 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/LineNumberCodes.py
--rw-rw-rw-   0        0        0    15849 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ListCodes.py
--rw-rw-rw-   0        0        0     6658 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/LoaderCodes.py
--rw-rw-rw-   0        0        0    10016 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/LocalsDictCodes.py
--rw-rw-rw-   0        0        0     3174 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/LoopCodes.py
--rw-rw-rw-   0        0        0     1637 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/MatchCodes.py
--rw-rw-rw-   0        0        0     6525 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ModuleCodes.py
--rw-rw-rw-   0        0        0     8224 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/Namify.py
--rw-rw-rw-   0        0        0     1860 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/NetworkxCodes.py
--rw-rw-rw-   0        0        0    12733 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/OperationCodes.py
--rw-rw-rw-   0        0        0    30198 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/PackageResourceCodes.py
--rw-rw-rw-   0        0        0     3054 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/PrintCodes.py
--rw-rw-rw-   0        0        0     5670 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/PythonAPICodes.py
--rw-rw-rw-   0        0        0    13251 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/RaisingCodes.py
--rw-rw-rw-   0        0        0     3476 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/Reports.py
--rw-rw-rw-   0        0        0     5267 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/ReturnCodes.py
--rw-rw-rw-   0        0        0     6591 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/SetCodes.py
--rw-rw-rw-   0        0        0    14005 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/SliceCodes.py
--rw-rw-rw-   0        0        0    10087 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/StringCodes.py
--rw-rw-rw-   0        0        0     8302 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/SubscriptCodes.py
--rw-rw-rw-   0        0        0     1939 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/TensorflowCodes.py
--rw-rw-rw-   0        0        0    11208 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/TryCodes.py
--rw-rw-rw-   0        0        0     3840 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/TupleCodes.py
--rw-rw-rw-   0        0        0     2362 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/TypeAliasCodes.py
--rw-rw-rw-   0        0        0    14811 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/VariableCodes.py
--rw-rw-rw-   0        0        0     9155 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/VariableDeclarations.py
--rw-rw-rw-   0        0        0     8129 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/YieldCodes.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.043812 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/
--rw-rw-rw-   0        0        0     6102 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeBases.py
--rw-rw-rw-   0        0        0     3432 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-rw-rw-   0        0        0     1837 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-rw-rw-   0        0        0     1410 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-rw-rw-   0        0        0     3642 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-rw-rw-   0        0        0     5161 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-rw-rw-   0        0        0     5243 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-rw-rw-   0        0        0     3988 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-rw-rw-   0        0        0    19696 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-rw-rw-   0        0        0     2886 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeVoids.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.050814 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/
--rw-rw-rw-   0        0        0     2948 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-rw-rw-   0        0        0     9455 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-rw-rw-   0        0        0     2439 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-rw-rw-   0        0        0     6483 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-rw-rw-   0        0        0     3460 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-rw-rw-   0        0        0     3390 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-rw-rw-   0        0        0     2408 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-rw-rw-   0        0        0     4534 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-rw-rw-   0        0        0    23021 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-rw-rw-   0        0        0     6840 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-rw-rw-   0        0        0     2507 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.139820 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/
--rw-rw-rw-   0        0        0    11318 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-rw-rw-   0        0        0     5829 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-rw-rw-   0        0        0    23986 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-rw-rw-   0        0        0     5438 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-rw-rw-   0        0        0     1755 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-rw-rw-   0        0        0     1693 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-rw-rw-   0        0        0     2706 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-rw-rw-   0        0        0    13624 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-rw-rw-   0        0        0     1894 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-rw-rw-   0        0        0     2618 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-rw-rw-   0        0        0     1394 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-rw-rw-   0        0        0     7047 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-rw-rw-   0        0        0    12700 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-rw-rw-   0        0        0     4138 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-rw-rw-   0        0        0     1938 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-rw-rw-   0        0        0     1968 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-rw-rw-   0        0        0     4081 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-rw-rw-   0        0        0     7257 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-rw-rw-   0        0        0     4142 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-rw-rw-   0        0        0     3710 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-rw-rw-   0        0        0     4447 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-rw-rw-   0        0        0    11758 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-rw-rw-   0        0        0    19167 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-rw-rw-   0        0        0     2693 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-rw-rw-   0        0        0     3485 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-rw-rw-   0        0        0    11336 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-rw-rw-   0        0        0    15540 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-rw-rw-   0        0        0     2829 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-rw-rw-   0        0        0    10395 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-rw-rw-   0        0        0     2407 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-rw-rw-   0        0        0     2870 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-rw-rw-   0        0        0     2834 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-rw-rw-   0        0        0     3128 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.145834 nuitka_winsvc-2.2.2/nuitka/containers/
--rw-rw-rw-   0        0        0     1467 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/containers/Namedtuples.py
--rw-rw-rw-   0        0        0     6553 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/containers/OrderedDicts.py
--rw-rw-rw-   0        0        0      554 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/nuitka/containers/OrderedSets.py
--rw-rw-rw-   0        0        0     4430 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/containers/OrderedSetsFallback.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.148814 nuitka_winsvc-2.2.2/nuitka/distutils/
--rw-rw-rw-   0        0        0     2308 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/distutils/Build.py
--rw-rw-rw-   0        0        0    15025 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/distutils/DistutilCommands.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/distutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.151813 nuitka_winsvc-2.2.2/nuitka/finalizations/
--rw-rw-rw-   0        0        0     1258 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/finalizations/Finalization.py
--rw-rw-rw-   0        0        0     6058 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/finalizations/FinalizeMarkups.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/finalizations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.159813 nuitka_winsvc-2.2.2/nuitka/freezer/
--rw-rw-rw-   0        0        0     7778 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/freezer/DependsExe.py
--rw-rw-rw-   0        0        0     2616 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/freezer/DllDependenciesCommon.py
--rw-rw-rw-   0        0        0    14396 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/freezer/DllDependenciesMacOS.py
--rw-rw-rw-   0        0        0     7468 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/freezer/DllDependenciesPosix.py
--rw-rw-rw-   0        0        0     6698 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/freezer/DllDependenciesWin32.py
--rw-rw-rw-   0        0        0    11979 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/freezer/ImportDetection.py
--rw-rw-rw-   0        0        0    19236 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/freezer/IncludedDataFiles.py
--rw-rw-rw-   0        0        0    11455 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/freezer/IncludedEntryPoints.py
--rw-rw-rw-   0        0        0    10516 2024-05-15 06:22:00.000000 nuitka_winsvc-2.2.2/nuitka/freezer/Onefile.py
--rw-rw-rw-   0        0        0    12245 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/freezer/Standalone.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/freezer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.164813 nuitka_winsvc-2.2.2/nuitka/importing/
--rw-rw-rw-   0        0        0    11040 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/importing/IgnoreListing.py
--rw-rw-rw-   0        0        0     2956 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/importing/ImportCache.py
--rw-rw-rw-   0        0        0     7784 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/importing/ImportResolving.py
--rw-rw-rw-   0        0        0    32895 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/importing/Importing.py
--rw-rw-rw-   0        0        0     4869 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/importing/PreloadedPackages.py
--rw-rw-rw-   0        0        0    18804 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/importing/Recursion.py
--rw-rw-rw-   0        0        0    12787 2024-04-07 02:15:13.000000 nuitka_winsvc-2.2.2/nuitka/importing/StandardLibrary.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/importing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.214813 nuitka_winsvc-2.2.2/nuitka/nodes/
--rw-rw-rw-   0        0        0     3670 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/AsyncgenNodes.py
--rw-rw-rw-   0        0        0     4115 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/AttributeLookupNodes.py
--rw-rw-rw-   0        0        0    13255 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/AttributeNodes.py
--rw-rw-rw-   0        0        0   379568 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/AttributeNodesGenerated.py
--rw-rw-rw-   0        0        0     3856 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinAllNodes.py
--rw-rw-rw-   0        0        0     4131 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinAnyNodes.py
--rw-rw-rw-   0        0        0     2530 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinComplexNodes.py
--rw-rw-rw-   0        0        0     1731 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinDecodingNodes.py
--rw-rw-rw-   0        0        0     2760 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-rw-rw-   0        0        0     4727 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinDictNodes.py
--rw-rw-rw-   0        0        0     4982 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinFormatNodes.py
--rw-rw-rw-   0        0        0     2275 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinHashNodes.py
--rw-rw-rw-   0        0        0     1457 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinInputNodes.py
--rw-rw-rw-   0        0        0     5367 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinIntegerNodes.py
--rw-rw-rw-   0        0        0    12812 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinIteratorNodes.py
--rw-rw-rw-   0        0        0     2029 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinLenNodes.py
--rw-rw-rw-   0        0        0     3639 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinNextNodes.py
--rw-rw-rw-   0        0        0     3787 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinOpenNodes.py
--rw-rw-rw-   0        0        0   246360 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-rw-rw-   0        0        0    18648 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinRangeNodes.py
--rw-rw-rw-   0        0        0     9468 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinRefNodes.py
--rw-rw-rw-   0        0        0     3353 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinSumNodes.py
--rw-rw-rw-   0        0        0    13576 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinTypeNodes.py
--rw-rw-rw-   0        0        0     1605 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinVarsNodes.py
--rw-rw-rw-   0        0        0    26146 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/BytesNodes.py
--rw-rw-rw-   0        0        0     6511 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/CallNodes.py
--rw-rw-rw-   0        0        0     1583 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/Checkers.py
--rw-rw-rw-   0        0        0   647748 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ChildrenHavingMixins.py
--rw-rw-rw-   0        0        0     8480 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ClassNodes.py
--rw-rw-rw-   0        0        0     6622 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/CodeObjectSpecs.py
--rw-rw-rw-   0        0        0    21716 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ComparisonNodes.py
--rw-rw-rw-   0        0        0    30191 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ConditionalNodes.py
--rw-rw-rw-   0        0        0    47737 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ConstantRefNodes.py
--rw-rw-rw-   0        0        0    12246 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ContainerMakingNodes.py
--rw-rw-rw-   0        0        0     2867 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ContainerOperationNodes.py
--rw-rw-rw-   0        0        0     4614 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/CoroutineNodes.py
--rw-rw-rw-   0        0        0     1746 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/CtypesNodes.py
--rw-rw-rw-   0        0        0    51053 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/DictionaryNodes.py
--rw-rw-rw-   0        0        0     8151 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ExceptionNodes.py
--rw-rw-rw-   0        0        0     7408 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ExecEvalNodes.py
--rw-rw-rw-   0        0        0    45046 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ExpressionBases.py
--rw-rw-rw-   0        0        0    55956 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ExpressionBasesGenerated.py
--rw-rw-rw-   0        0        0    21311 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ExpressionShapeMixins.py
--rw-rw-rw-   0        0        0    12024 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/FrameNodes.py
--rw-rw-rw-   0        0        0     3577 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/FunctionAttributeNodes.py
--rw-rw-rw-   0        0        0    41167 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/FunctionNodes.py
--rw-rw-rw-   0        0        0     5409 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/FutureSpecs.py
--rw-rw-rw-   0        0        0     6288 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/GeneratorNodes.py
--rw-rw-rw-   0        0        0     6961 2024-04-07 02:15:13.000000 nuitka_winsvc-2.2.2/nuitka/nodes/GlobalsLocalsNodes.py
--rw-rw-rw-   0        0        0    98222 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/HardImportNodesGenerated.py
--rw-rw-rw-   0        0        0     5631 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ImportHardNodes.py
--rw-rw-rw-   0        0        0    48286 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ImportNodes.py
--rw-rw-rw-   0        0        0     2766 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/IndicatorMixins.py
--rw-rw-rw-   0        0        0     1533 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/InjectCNodes.py
--rw-rw-rw-   0        0        0    11519 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/IterationHandles.py
--rw-rw-rw-   0        0        0    11035 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/KeyValuePairNodes.py
--rw-rw-rw-   0        0        0    16821 2024-03-14 05:29:37.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ListOperationNodes.py
--rw-rw-rw-   0        0        0    23177 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/LocalsDictNodes.py
--rw-rw-rw-   0        0        0    15007 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.2/nuitka/nodes/LocalsScopes.py
--rw-rw-rw-   0        0        0    15995 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/LoopNodes.py
--rw-rw-rw-   0        0        0     1745 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/MatchNodes.py
--rw-rw-rw-   0        0        0     6567 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ModuleAttributeNodes.py
--rw-rw-rw-   0        0        0    32830 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ModuleNodes.py
--rw-rw-rw-   0        0        0     1759 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/NetworkxNodes.py
--rw-rw-rw-   0        0        0    24461 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/NodeBases.py
--rw-rw-rw-   0        0        0    15147 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/NodeMakingHelpers.py
--rw-rw-rw-   0        0        0     5580 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/NodeMetaClasses.py
--rw-rw-rw-   0        0        0    31948 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/OperatorNodes.py
--rw-rw-rw-   0        0        0     8976 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/OperatorNodesUnary.py
--rw-rw-rw-   0        0        0     5228 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/OsSysNodes.py
--rw-rw-rw-   0        0        0    12468 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/OutlineNodes.py
--rw-rw-rw-   0        0        0    34735 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/PackageMetadataNodes.py
--rw-rw-rw-   0        0        0    12289 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/PackageResourceNodes.py
--rw-rw-rw-   0        0        0     3440 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/PrintNodes.py
--rw-rw-rw-   0        0        0     6805 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/ReturnNodes.py
--rw-rw-rw-   0        0        0     4748 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/SideEffectNodes.py
--rw-rw-rw-   0        0        0    12547 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/SliceNodes.py
--rw-rw-rw-   0        0        0    98808 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/StatementBasesGenerated.py
--rw-rw-rw-   0        0        0     9336 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/StatementNodes.py
--rw-rw-rw-   0        0        0    28691 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/StrNodes.py
--rw-rw-rw-   0        0        0     3538 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/StringConcatenationNodes.py
--rw-rw-rw-   0        0        0     8329 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/SubscriptNodes.py
--rw-rw-rw-   0        0        0     1411 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/TensorflowNodes.py
--rw-rw-rw-   0        0        0    17886 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/TryNodes.py
--rw-rw-rw-   0        0        0     2438 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/TypeMatchNodes.py
--rw-rw-rw-   0        0        0    11717 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/TypeNodes.py
--rw-rw-rw-   0        0        0    42396 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/VariableAssignNodes.py
--rw-rw-rw-   0        0        0    10779 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/VariableDelNodes.py
--rw-rw-rw-   0        0        0     4607 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/VariableNameNodes.py
--rw-rw-rw-   0        0        0    31274 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/VariableRefNodes.py
--rw-rw-rw-   0        0        0     4781 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/VariableReleaseNodes.py
--rw-rw-rw-   0        0        0     3937 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/YieldNodes.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.217814 nuitka_winsvc-2.2.2/nuitka/nodes/shapes/
--rw-rw-rw-   0        0        0   157357 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-rw-rw-   0        0        0     4420 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-rw-rw-   0        0        0     5076 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/shapes/ShapeMixins.py
--rw-rw-rw-   0        0        0    42509 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/shapes/StandardShapes.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/nodes/shapes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.221815 nuitka_winsvc-2.2.2/nuitka/optimizations/
--rw-rw-rw-   0        0        0     3358 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/optimizations/BytecodeDemotion.py
--rw-rw-rw-   0        0        0     3953 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/optimizations/FunctionInlining.py
--rw-rw-rw-   0        0        0     2177 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/optimizations/Graphs.py
--rw-rw-rw-   0        0        0    10917 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/optimizations/Optimization.py
--rw-rw-rw-   0        0        0    52575 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-rw-rw-   0        0        0     2287 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/optimizations/Tags.py
--rw-rw-rw-   0        0        0    42800 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/optimizations/TraceCollections.py
--rw-rw-rw-   0        0        0    25799 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/optimizations/ValueTraces.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/optimizations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.222814 nuitka_winsvc-2.2.2/nuitka/pgo/
--rw-rw-rw-   0        0        0     4932 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/pgo/PGO.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/pgo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.224816 nuitka_winsvc-2.2.2/nuitka/plugins/
--rw-rw-rw-   0        0        0    57735 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/PluginBase.py
--rw-rw-rw-   0        0        0    60905 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/Plugins.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.252722 nuitka_winsvc-2.2.2/nuitka/plugins/standard/
--rw-rw-rw-   0        0        0    30813 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-rw-rw-   0        0        0     3509 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-rw-rw-   0        0        0    10627 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/DataFilesPlugin.py
--rw-rw-rw-   0        0        0     5080 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/DelvewheelPlugin.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.260292 nuitka_winsvc-2.2.2/nuitka/plugins/standard/DillPlugin/
--rw-rw-rw-   0        0        0     1646 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/DillPlugin/DillPlugin.c
--rw-rw-rw-   0        0        0     9826 2024-03-25 02:50:30.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/DillPlugin/dill-postLoad.py
--rw-rw-rw-   0        0        0     2679 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/DillPlugin.py
--rw-rw-rw-   0        0        0    16496 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/DllFilesPlugin.py
--rw-rw-rw-   0        0        0     2095 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/EnumPlugin.py
--rw-rw-rw-   0        0        0     1938 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/EventletPlugin.py
--rw-rw-rw-   0        0        0     1913 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/GeventPlugin.py
--rw-rw-rw-   0        0        0     4018 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/GiPlugin.py
--rw-rw-rw-   0        0        0     4854 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/GlfwPlugin.py
--rw-rw-rw-   0        0        0    32325 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/ImplicitImports.py
--rw-rw-rw-   0        0        0     5024 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/KivyPlugin.py
--rw-rw-rw-   0        0        0     8824 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-rw-rw-   0        0        0     7080 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-rw-rw-   0        0        0     1220 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/NumpyPlugin.py
--rw-rw-rw-   0        0        0     7299 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-rw-rw-   0        0        0     1940 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/PbrPlugin.py
--rw-rw-rw-   0        0        0     4874 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-rw-rw-   0        0        0     7216 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/PmwPlugin.py
--rw-rw-rw-   0        0        0    51908 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-rw-rw-   0        0        0     3020 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/PywebViewPlugin.py
--rw-rw-rw-   0        0        0     1194 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/TensorflowPlugin.py
--rw-rw-rw-   0        0        0    13878 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/TkinterPlugin.py
--rw-rw-rw-   0        0        0     1174 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/TorchPlugin.py
--rw-rw-rw-   0        0        0    12838 2024-04-07 02:15:13.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/TransformersPlugin.py
--rw-rw-rw-   0        0        0     1107 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/TrioPlugin.py
--rw-rw-rw-   0        0        0     5668 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/UpxPlugin.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/__init__.py
--rw-rw-rw-   0        0        0   236441 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     2352 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-rw-rw-   0        0        0    12392 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.2/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.272857 nuitka_winsvc-2.2.2/nuitka/reports/
--rw-rw-rw-   0        0        0     2286 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/reports/CompilationReportReader.py
--rw-rw-rw-   0        0        0     2089 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/reports/LicenseReport.rst.j2
--rw-rw-rw-   0        0        0    28897 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/reports/Reports.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.279778 nuitka_winsvc-2.2.2/nuitka/specs/
--rw-rw-rw-   0        0        0     5943 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-rw-rw-   0        0        0     2818 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-rw-rw-   0        0        0     2573 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/specs/BuiltinListOperationSpecs.py
--rw-rw-rw-   0        0        0    27022 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/specs/BuiltinParameterSpecs.py
--rw-rw-rw-   0        0        0     6098 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-rw-rw-   0        0        0     1190 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-rw-rw-   0        0        0     4834 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-rw-rw-   0        0        0     7112 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/specs/HardImportSpecs.py
--rw-rw-rw-   0        0        0    18811 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/specs/ParameterSpecs.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/specs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.281777 nuitka_winsvc-2.2.2/nuitka/tools/
--rw-rw-rw-   0        0        0     1631 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/Basics.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.281777 nuitka_winsvc-2.2.2/nuitka/tools/commercial/
--rw-rw-rw-   0        0        0      847 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/commercial/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.284770 nuitka_winsvc-2.2.2/nuitka/tools/data_composer/
--rw-rw-rw-   0        0        0    15004 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/data_composer/DataComposer.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/data_composer/__init__.py
--rw-rw-rw-   0        0        0     1338 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/data_composer/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.285769 nuitka_winsvc-2.2.2/nuitka/tools/environments/
--rw-rw-rw-   0        0        0     2481 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/environments/CreateEnvironment.py
--rw-rw-rw-   0        0        0     4198 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/environments/Virtualenv.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/environments/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.286767 nuitka_winsvc-2.2.2/nuitka/tools/general/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/general/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.287364 nuitka_winsvc-2.2.2/nuitka/tools/general/dll_report/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/general/dll_report/__init__.py
--rw-rw-rw-   0        0        0     2352 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/general/dll_report/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.289368 nuitka_winsvc-2.2.2/nuitka/tools/general/find_module/
--rw-rw-rw-   0        0        0     3953 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/general/find_module/FindModuleCode.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/general/find_module/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.290357 nuitka_winsvc-2.2.2/nuitka/tools/onefile_compressor/
--rw-rw-rw-   0        0        0    12545 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/onefile_compressor/__init__.py
--rw-rw-rw-   0        0        0     1343 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/onefile_compressor/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.291365 nuitka_winsvc-2.2.2/nuitka/tools/podman/
--rw-rw-rw-   0        0        0     1905 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/podman/Podman.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/podman/__init__.py
--rw-rw-rw-   0        0        0    11623 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/podman/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.292358 nuitka_winsvc-2.2.2/nuitka/tools/profiler/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/profiler/__init__.py
--rw-rw-rw-   0        0        0     2561 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/profiler/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.293365 nuitka_winsvc-2.2.2/nuitka/tools/scanning/
--rw-rw-rw-   0        0        0     3590 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-rw-rw-   0        0        0     2314 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/scanning/DisplayPackageData.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/scanning/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.296358 nuitka_winsvc-2.2.2/nuitka/tools/specialize/
--rw-rw-rw-   0        0        0    51703 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/specialize/CTypeDescriptions.py
--rw-rw-rw-   0        0        0     7717 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/specialize/Common.py
--rw-rw-rw-   0        0        0    39747 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/specialize/SpecializeC.py
--rw-rw-rw-   0        0        0    36683 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/specialize/SpecializePython.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/specialize/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.300775 nuitka_winsvc-2.2.2/nuitka/tools/testing/
--rw-rw-rw-   0        0        0    56174 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/Common.py
--rw-rw-rw-   0        0        0     1516 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/Constructs.py
--rw-rw-rw-   0        0        0    10129 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/OutputComparison.py
--rw-rw-rw-   0        0        0     1310 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/Pythons.py
--rw-rw-rw-   0        0        0     8061 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/RuntimeTracing.py
--rw-rw-rw-   0        0        0     5413 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/SearchModes.py
--rw-rw-rw-   0        0        0     3408 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/Valgrind.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.301774 nuitka_winsvc-2.2.2/nuitka/tools/testing/check_reference_counts/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-rw-rw-   0        0        0     3095 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/check_reference_counts/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.302774 nuitka_winsvc-2.2.2/nuitka/tools/testing/compare_with_cpython/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-rw-rw-   0        0        0    29697 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/compare_with_cpython/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.303774 nuitka_winsvc-2.2.2/nuitka/tools/testing/find_sxs_modules/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/find_sxs_modules/__init__.py
--rw-rw-rw-   0        0        0     1980 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/find_sxs_modules/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.304772 nuitka_winsvc-2.2.2/nuitka/tools/testing/measure_construct_performance/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-rw-rw-   0        0        0     8758 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/measure_construct_performance/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.305771 nuitka_winsvc-2.2.2/nuitka/tools/testing/run_nuitka_tests/
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/run_nuitka_tests/__init__.py
--rw-rw-rw-   0        0        0    35342 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/testing/run_nuitka_tests/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.306779 nuitka_winsvc-2.2.2/nuitka/tools/watch/
--rw-rw-rw-   0        0        0     3543 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/watch/GitHub.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tools/watch/__init__.py
--rw-rw-rw-   0        0        0    21532 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tools/watch/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.325591 nuitka_winsvc-2.2.2/nuitka/tree/
--rw-rw-rw-   0        0        0    50436 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/Building.py
--rw-rw-rw-   0        0        0    75150 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ComplexCallHelperFunctions.py
--rw-rw-rw-   0        0        0     1733 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/Extractions.py
--rw-rw-rw-   0        0        0     2603 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/InternalModule.py
--rw-rw-rw-   0        0        0     1544 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/Operations.py
--rw-rw-rw-   0        0        0     2841 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationAssertStatements.py
--rw-rw-rw-   0        0        0    43887 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationAssignmentStatements.py
--rw-rw-rw-   0        0        0     2981 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationBooleanExpressions.py
--rw-rw-rw-   0        0        0    11746 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationCallExpressions.py
--rw-rw-rw-   0        0        0    15446 2024-03-20 02:57:24.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationClasses.py
--rw-rw-rw-   0        0        0    38202 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationClasses3.py
--rw-rw-rw-   0        0        0     6523 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationComparisonExpressions.py
--rw-rw-rw-   0        0        0    22207 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationContractionExpressions.py
--rw-rw-rw-   0        0        0    11266 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationDictionaryCreation.py
--rw-rw-rw-   0        0        0    14805 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationExecStatements.py
--rw-rw-rw-   0        0        0     7858 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationForLoopStatements.py
--rw-rw-rw-   0        0        0    30885 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationFunctionStatements.py
--rw-rw-rw-   0        0        0    14095 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationImportStatements.py
--rw-rw-rw-   0        0        0     6630 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationLambdaExpressions.py
--rw-rw-rw-   0        0        0    21311 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationMatchStatements.py
--rw-rw-rw-   0        0        0     2442 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationMultidist.py
--rw-rw-rw-   0        0        0     7608 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationNamespacePackages.py
--rw-rw-rw-   0        0        0     4711 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationPrintStatements.py
--rw-rw-rw-   0        0        0    15606 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationSequenceCreation.py
--rw-rw-rw-   0        0        0     4857 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-rw-rw-   0        0        0    14948 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationTryExceptStatements.py
--rw-rw-rw-   0        0        0     7014 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-rw-rw-   0        0        0     5707 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-rw-rw-   0        0        0    14439 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationWithStatements.py
--rw-rw-rw-   0        0        0     3852 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/ReformulationYieldExpressions.py
--rw-rw-rw-   0        0        0    13488 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/SourceHandling.py
--rw-rw-rw-   0        0        0     3790 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/SyntaxErrors.py
--rw-rw-rw-   0        0        0    23153 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/tree/TreeHelpers.py
--rw-rw-rw-   0        0        0    20465 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/VariableClosure.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.340334 nuitka_winsvc-2.2.2/nuitka/utils/
--rw-rw-rw-   0        0        0     3140 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/AppDirs.py
--rw-rw-rw-   0        0        0     4128 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/CStrings.py
--rw-rw-rw-   0        0        0     6394 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/CommandLineOptions.py
--rw-rw-rw-   0        0        0    14983 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/Distributions.py
--rw-rw-rw-   0        0        0     6477 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/Download.py
--rw-rw-rw-   0        0        0    13368 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/Execution.py
--rw-rw-rw-   0        0        0    42167 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/FileOperations.py
--rw-rw-rw-   0        0        0     3753 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/Hashing.py
--rw-rw-rw-   0        0        0     2395 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/Images.py
--rw-rw-rw-   0        0        0    10334 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/Importing.py
--rw-rw-rw-   0        0        0     7884 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/InstalledPythons.py
--rw-rw-rw-   0        0        0     2258 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/InstanceCounters.py
--rw-rw-rw-   0        0        0     4586 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/Jinja2.py
--rw-rw-rw-   0        0        0     1271 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/Json.py
--rw-rw-rw-   0        0        0     4478 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/MacOSApp.py
--rw-rw-rw-   0        0        0     5092 2024-03-25 02:50:30.000000 nuitka_winsvc-2.2.2/nuitka/utils/MemoryUsage.py
--rw-rw-rw-   0        0        0     9951 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/ModuleNames.py
--rw-rw-rw-   0        0        0     4588 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/ReExecute.py
--rw-rw-rw-   0        0        0     1889 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/Rest.py
--rw-rw-rw-   0        0        0    23857 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/SharedLibraries.py
--rw-rw-rw-   0        0        0     3698 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/Shebang.py
--rw-rw-rw-   0        0        0     3687 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/Signing.py
--rw-rw-rw-   0        0        0     2084 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/SlotMetaClasses.py
--rw-rw-rw-   0        0        0     6603 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/StaticLibraries.py
--rw-rw-rw-   0        0        0     2634 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/ThreadedExecutor.py
--rw-rw-rw-   0        0        0     2798 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/Timing.py
--rw-rw-rw-   0        0        0    12705 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/Utils.py
--rw-rw-rw-   0        0        0    10642 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/nuitka/utils/WindowsFileUsage.py
--rw-rw-rw-   0        0        0    19837 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/WindowsResources.py
--rw-rw-rw-   0        0        0     7014 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/Yaml.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/nuitka/utils/__init__.py
--rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 06:23:06.351518 nuitka_winsvc-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0    16351 2024-05-15 06:22:00.000000 nuitka_winsvc-2.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:03.341334 nuitka_winsvc-2.2.2/tests/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.297248 nuitka_winsvc-2.2.2/tests/basics/
--rw-rw-rw-   0        0        0     1798 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/AssertsTest.py
--rw-rw-rw-   0        0        0     5966 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/AssignmentsTest.py
--rw-rw-rw-   0        0        0     5910 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/AssignmentsTest32.py
--rw-rw-rw-   0        0        0     4086 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/BranchingTest.py
--rw-rw-rw-   0        0        0     1136 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/BuiltinOverload.py
--rw-rw-rw-   0        0        0     3781 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/BuiltinSuperTest.py
--rw-rw-rw-   0        0        0    17112 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/BuiltinsTest.py
--rw-rw-rw-   0        0        0      898 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ClassMinimalTest.py
--rw-rw-rw-   0        0        0     4796 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ClassesTest.py
--rw-rw-rw-   0        0        0     3446 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ClassesTest32.py
--rw-rw-rw-   0        0        0     1438 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ClassesTest34.py
--rw-rw-rw-   0        0        0     4729 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ComparisonChainsTest.py
--rw-rw-rw-   0        0        0     4672 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ConstantsTest.py
--rw-rw-rw-   0        0        0     1027 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ConstantsTest27.py
--rw-rw-rw-   0        0        0     1661 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/DecoratorsTest.py
--rw-rw-rw-   0        0        0     2349 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/DefaultParametersTest.py
--rw-rw-rw-   0        0        0     1159 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/DoubleDeletionsTest.py
--rw-rw-rw-   0        0        0      838 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/EmptyModuleTest.py
--rw-rw-rw-   0        0        0    14418 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ExceptionRaisingTest.py
--rw-rw-rw-   0        0        0      993 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ExceptionRaisingTest32.py
--rw-rw-rw-   0        0        0     1490 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ExceptionRaisingTest33.py
--rw-rw-rw-   0        0        0     6779 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ExecEvalTest.py
--rw-rw-rw-   0        0        0     1450 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/basics/ExtremeClosureTest.py
--rw-rw-rw-   0        0        0     1689 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/basics/FunctionObjectsTest.py
--rw-rw-rw-   0        0        0    12367 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/FunctionsTest.py
--rw-rw-rw-   0        0        0     3635 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/FunctionsTest32.py
--rw-rw-rw-   0        0        0     2658 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/basics/FunctionsTest_2.py
--rw-rw-rw-   0        0        0      922 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/FutureTest32.py
--rw-rw-rw-   0        0        0     5841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/GeneratorExpressionsTest.py
--rw-rw-rw-   0        0        0     1073 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/GeneratorExpressionsTest_37.py
--rw-rw-rw-   0        0        0     3856 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/GlobalStatementTest.py
--rw-rw-rw-   0        0        0     1318 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/HelloWorldTest_2.py
--rw-rw-rw-   0        0        0     2501 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ImportingTest.py
--rw-rw-rw-   0        0        0     1328 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/InplaceOperationsTest.py
--rw-rw-rw-   0        0        0     4259 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/InspectionTest.py
--rw-rw-rw-   0        0        0     1536 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/InspectionTest_35.py
--rw-rw-rw-   0        0        0     1650 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/InspectionTest_36.py
--rw-rw-rw-   0        0        0     1703 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/LambdasTest.py
--rw-rw-rw-   0        0        0     2763 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/LateClosureAssignmentTest.py
--rw-rw-rw-   0        0        0     2955 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ListContractionsTest.py
--rw-rw-rw-   0        0        0     3361 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/LoopingTest.py
--rw-rw-rw-   0        0        0     1568 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/MainProgramsTest.py
--rw-rw-rw-   0        0        0     1957 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ModuleAttributesTest.py
--rw-rw-rw-   0        0        0     2008 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/OperatorsTest.py
--rw-rw-rw-   0        0        0    14935 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/OrderChecksTest.py
--rw-rw-rw-   0        0        0     1859 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/OrderChecksTest27.py
--rw-rw-rw-   0        0        0     1484 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/OverflowFunctionsTest_2.py
--rw-rw-rw-   0        0        0     5885 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ParameterErrorsTest.py
--rw-rw-rw-   0        0        0     1931 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ParameterErrorsTest32.py
--rw-rw-rw-   0        0        0      895 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/PrintFutureTest.py
--rw-rw-rw-   0        0        0     1444 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/PrintingTest_2.py
--rw-rw-rw-   0        0        0      910 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/RecursionTest.py
--rw-rw-rw-   0        0        0    24798 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/basics/ReferencingTest.py
--rw-rw-rw-   0        0        0     2109 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ReferencingTest27.py
--rw-rw-rw-   0        0        0     7869 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/basics/ReferencingTest33.py
--rw-rw-rw-   0        0        0     5060 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/basics/ReferencingTest35.py
--rw-rw-rw-   0        0        0     5497 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/basics/ReferencingTest36.py
--rw-rw-rw-   0        0        0     2932 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ReferencingTest_2.py
--rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/SlotsTest.py
--rw-rw-rw-   0        0        0     1191 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/ThreadedGeneratorsTest.py
--rw-rw-rw-   0        0        0    22998 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/TrickAssignmentsTest32.py
--rw-rw-rw-   0        0        0     1573 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/TrickAssignmentsTest35.py
--rw-rw-rw-   0        0        0     1820 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/TrickAssignmentsTest_2.py
--rw-rw-rw-   0        0        0     2118 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/TryContinueFinallyTest.py
--rw-rw-rw-   0        0        0     2244 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/TryExceptContinueTest.py
--rw-rw-rw-   0        0        0     2307 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/TryExceptFinallyTest.py
--rw-rw-rw-   0        0        0     2336 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/TryExceptFramesTest.py
--rw-rw-rw-   0        0        0     2874 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/TryReturnFinallyTest.py
--rw-rw-rw-   0        0        0     2360 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/TryYieldFinallyTest.py
--rw-rw-rw-   0        0        0     1125 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/UnicodeTest.py
--rw-rw-rw-   0        0        0     1909 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/UnpackingTest35.py
--rw-rw-rw-   0        0        0     2143 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/VarargsTest.py
--rw-rw-rw-   0        0        0     4913 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/WithStatementsTest.py
--rw-rw-rw-   0        0        0     3103 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/YieldFromTest33.py
--rw-rw-rw-   0        0        0     3851 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/run_all.py
--rw-rw-rw-   0        0        0     2302 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/basics/run_xml.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.314832 nuitka_winsvc-2.2.2/tests/onefile/
--rw-rw-rw-   0        0        0     1341 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/onefile/HelloWorldTest.py
--rw-rw-rw-   0        0        0     1339 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/onefile/KeyboardInterruptTest.py
--rw-rw-rw-   0        0        0     5846 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/onefile/run_all.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.340830 nuitka_winsvc-2.2.2/tests/optimizations/
--rw-rw-rw-   0        0        0      991 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/optimizations/ArgumentTypes.py
--rw-rw-rw-   0        0        0     1087 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/AttributesTest.py
--rw-rw-rw-   0        0        0     1053 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/CallsTest.py
--rw-rw-rw-   0        0        0      953 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/ConditionsTest.py
--rw-rw-rw-   0        0        0      941 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/DecodingOperationsTest.py
--rw-rw-rw-   0        0        0     1246 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/FormatStringsTest36.py
--rw-rw-rw-   0        0        0     1183 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/HardImportsTest.py
--rw-rw-rw-   0        0        0     1007 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/HardImportsTest_2.py
--rw-rw-rw-   0        0        0      950 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/optimizations/Iterations.py
--rw-rw-rw-   0        0        0     1292 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/LenTest.py
--rw-rw-rw-   0        0        0     1133 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/MatchingTest310.py
--rw-rw-rw-   0        0        0     2295 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/OperationsTest.py
--rw-rw-rw-   0        0        0     1365 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/optimizations/SubscriptsTest.py
--rw-rw-rw-   0        0        0     8827 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/optimizations/run_all.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.347831 nuitka_winsvc-2.2.2/tests/packages/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.350832 nuitka_winsvc-2.2.2/tests/packages/package_data_files_embedding/
--rw-rw-rw-   0        0        0     1576 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py
--rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/package_data_files_embedding/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.352836 nuitka_winsvc-2.2.2/tests/packages/package_import_success_after_failure/
--rw-rw-rw-   0        0        0     2414 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.356838 nuitka_winsvc-2.2.2/tests/packages/package_import_success_after_failure/variable_package/
--rw-rw-rw-   0        0        0      975 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
--rw-rw-rw-   0        0        0     1201 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rw-rw-rw-   0        0        0     4138 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/run_all.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.150151 nuitka_winsvc-2.2.2/tests/packages/sub_package/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.361832 nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/
--rw-rw-rw-   0        0        0     1262 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/__init__.py
--rw-rw-rw-   0        0        0      940 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/bigkitty.py
--rw-rw-rw-   0        0        0      942 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/smallkitty.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.364834 nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/speak/
--rw-rw-rw-   0        0        0      961 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/speak/__init__.py
--rw-rw-rw-   0        0        0     1085 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/speak/hello.py
--rw-rw-rw-   0        0        0      999 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/speak/miau.py
--rw-rw-rw-   0        0        0     1001 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/speak/purr.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.151162 nuitka_winsvc-2.2.2/tests/packages/top_level_attributes_3/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.366833 nuitka_winsvc-2.2.2/tests/packages/top_level_attributes_3/some_package/
--rw-rw-rw-   0        0        0     2368 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-rw-rw-   0        0        0      939 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.367835 nuitka_winsvc-2.2.2/tests/plugins/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.369834 nuitka_winsvc-2.2.2/tests/plugins/code_signing/
--rw-rw-rw-   0        0        0     1202 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/plugins/code_signing/CodeSigningMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.383831 nuitka_winsvc-2.2.2/tests/plugins/data_files/
--rw-rw-rw-   0        0        0     1474 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/plugins/data_files/DataFilesMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.393833 nuitka_winsvc-2.2.2/tests/plugins/data_files/data_files_package/
--rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/plugins/data_files/data_files_package/__init__.py
--rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/tests/plugins/data_files/data_files_package/lala.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.394834 nuitka_winsvc-2.2.2/tests/plugins/data_files/data_files_package/sub_dir/
--rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-rw-rw-   0        0        0      309 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.2/tests/plugins/data_files/test_case.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.395832 nuitka_winsvc-2.2.2/tests/plugins/parameters/
--rw-rw-rw-   0        0        0     1162 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/plugins/parameters/ParametersMain.py
--rw-rw-rw-   0        0        0     2218 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/plugins/parameters/parameter-using-plugin.py
--rw-rw-rw-   0        0        0     3778 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/plugins/run_all.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.400831 nuitka_winsvc-2.2.2/tests/programs/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.401832 nuitka_winsvc-2.2.2/tests/programs/absolute_import/
--rw-rw-rw-   0        0        0      899 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.433833 nuitka_winsvc-2.2.2/tests/programs/absolute_import/foobar/
--rw-rw-rw-   0        0        0      828 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/absolute_import/foobar/__init__.py
--rw-rw-rw-   0        0        0     1076 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/absolute_import/foobar/foobar.py
--rw-rw-rw-   0        0        0      911 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/absolute_import/foobar/local.py
--rw-rw-rw-   0        0        0      893 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/absolute_import/foobar/util.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.439833 nuitka_winsvc-2.2.2/tests/programs/case_imports1/
--rw-rw-rw-   0        0        0      840 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports1/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.445832 nuitka_winsvc-2.2.2/tests/programs/case_imports1/path1/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports1/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.453661 nuitka_winsvc-2.2.2/tests/programs/case_imports1/path1/Some_Package/
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports1/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.462671 nuitka_winsvc-2.2.2/tests/programs/case_imports1/path2/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports1/path2/some_module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.469678 nuitka_winsvc-2.2.2/tests/programs/case_imports1/path2/some_package/
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports1/path2/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.474673 nuitka_winsvc-2.2.2/tests/programs/case_imports2/
--rw-rw-rw-   0        0        0      840 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports2/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.481886 nuitka_winsvc-2.2.2/tests/programs/case_imports2/path1/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports2/path1/some_module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.486882 nuitka_winsvc-2.2.2/tests/programs/case_imports2/path1/some_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.490904 nuitka_winsvc-2.2.2/tests/programs/case_imports2/path2/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports2/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.499904 nuitka_winsvc-2.2.2/tests/programs/case_imports2/path2/Some_Package/
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports2/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.510120 nuitka_winsvc-2.2.2/tests/programs/case_imports3/
--rw-rw-rw-   0        0        0     1107 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports3/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.511120 nuitka_winsvc-2.2.2/tests/programs/case_imports3/path1/
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports3/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.521121 nuitka_winsvc-2.2.2/tests/programs/case_imports3/path1/Some_Package/
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports3/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.525120 nuitka_winsvc-2.2.2/tests/programs/case_imports3/path2/
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports3/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.532119 nuitka_winsvc-2.2.2/tests/programs/case_imports3/path2/Some_Package/
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/case_imports3/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.537775 nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.544775 nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
--rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.567011 nuitka_winsvc-2.2.2/tests/programs/dash_import/
--rw-rw-rw-   0        0        0      920 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/dash_import/DashImportMain.py
--rw-rw-rw-   0        0        0      849 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/dash_import/dash-module.py
--rw-rw-rw-   0        0        0      849 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/dash_import/plus+module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.574031 nuitka_winsvc-2.2.2/tests/programs/dash_main/
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/dash_main/Dash-Main.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.579503 nuitka_winsvc-2.2.2/tests/programs/deep/
--rw-rw-rw-   0        0        0      930 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/deep/DeepProgramMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.599287 nuitka_winsvc-2.2.2/tests/programs/deep/some_package/
--rw-rw-rw-   0        0        0     1012 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/deep/some_package/DeepBrother.py
--rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/deep/some_package/DeepChild.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/deep/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.611444 nuitka_winsvc-2.2.2/tests/programs/deep/some_package/deep_package/
--rw-rw-rw-   0        0        0      908 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
--rw-rw-rw-   0        0        0      984 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/deep/some_package/deep_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.615444 nuitka_winsvc-2.2.2/tests/programs/dunderinit_imports/
--rw-rw-rw-   0        0        0      826 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.619730 nuitka_winsvc-2.2.2/tests/programs/dunderinit_imports/package/
--rw-rw-rw-   0        0        0      829 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/dunderinit_imports/package/SubModule.py
--rw-rw-rw-   0        0        0      889 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/dunderinit_imports/package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.629160 nuitka_winsvc-2.2.2/tests/programs/import_variants/
--rw-rw-rw-   0        0        0     1037 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/import_variants/ImportVariationsMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.647151 nuitka_winsvc-2.2.2/tests/programs/import_variants/some_package/
--rw-rw-rw-   0        0        0      978 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/import_variants/some_package/Child1.py
--rw-rw-rw-   0        0        0     1130 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/import_variants/some_package/Child2.py
--rw-rw-rw-   0        0        0      854 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/import_variants/some_package/Child3.py
--rw-rw-rw-   0        0        0     1026 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/import_variants/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.663492 nuitka_winsvc-2.2.2/tests/programs/main_raises/
--rw-rw-rw-   0        0        0      943 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/main_raises/ErrorMain.py
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/main_raises/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.678255 nuitka_winsvc-2.2.2/tests/programs/main_raises2/
--rw-rw-rw-   0        0        0     1112 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/main_raises2/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.691051 nuitka_winsvc-2.2.2/tests/programs/module_attributes/
--rw-rw-rw-   0        0        0     1561 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.697765 nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/
--rw-rw-rw-   0        0        0     1800 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/Nearby1.py
--rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.707358 nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/
--rw-rw-rw-   0        0        0     1800 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.714712 nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-rw-rw-   0        0        0     1800 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.720616 nuitka_winsvc-2.2.2/tests/programs/module_exits/
--rw-rw-rw-   0        0        0      901 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/module_exits/ErrorExitingModule.py
--rw-rw-rw-   0        0        0      899 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/module_exits/Main.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.736419 nuitka_winsvc-2.2.2/tests/programs/module_object_replacing/
--rw-rw-rw-   0        0        0     1110 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-rw-rw-   0        0        0     1391 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.746110 nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/
--rw-rw-rw-   0        0        0     1022 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.769740 nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/foo/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/foo/__init__.py
--rw-rw-rw-   0        0        0      868 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/foo/__main__.py
--rw-rw-rw-   0        0        0     1791 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/foo/entry.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.773743 nuitka_winsvc-2.2.2/tests/programs/named_imports/
--rw-rw-rw-   0        0        0      878 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/named_imports/NamedImportsMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.783741 nuitka_winsvc-2.2.2/tests/programs/named_imports/some_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/named_imports/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      856 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/named_imports/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.788481 nuitka_winsvc-2.2.2/tests/programs/named_imports/some_package/sub_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.798352 nuitka_winsvc-2.2.2/tests/programs/package_code/
--rw-rw-rw-   0        0        0      832 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_code/PackageInitCodeMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.816662 nuitka_winsvc-2.2.2/tests/programs/package_code/some_package/
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_code/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_code/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.838311 nuitka_winsvc-2.2.2/tests/programs/package_contains_main/
--rw-rw-rw-   0        0        0      821 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_contains_main/PackageContainsMain.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_contains_main/__init__.py
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_contains_main/local.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.843905 nuitka_winsvc-2.2.2/tests/programs/package_init_import/
--rw-rw-rw-   0        0        0      855 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_init_import/PackageInitImportMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.847905 nuitka_winsvc-2.2.2/tests/programs/package_init_import/some_package/
--rw-rw-rw-   0        0        0     1064 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/programs/package_init_import/some_package/PackageLocal.py
--rw-rw-rw-   0        0        0     1225 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/programs/package_init_import/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.859198 nuitka_winsvc-2.2.2/tests/programs/package_init_issue/
--rw-rw-rw-   0        0        0      821 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.866529 nuitka_winsvc-2.2.2/tests/programs/package_init_issue/some_package/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_init_issue/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.870704 nuitka_winsvc-2.2.2/tests/programs/package_init_issue/some_package/child_package/
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-rw-rw-   0        0        0      827 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_init_issue/some_package/child_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.877557 nuitka_winsvc-2.2.2/tests/programs/package_missing_init/
--rw-rw-rw-   0        0        0      958 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.887585 nuitka_winsvc-2.2.2/tests/programs/package_missing_init/some_package/
--rw-rw-rw-   0        0        0      997 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_missing_init/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.892082 nuitka_winsvc-2.2.2/tests/programs/package_missing_init/some_package/sub_package/
--rw-rw-rw-   0        0        0     1009 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.912543 nuitka_winsvc-2.2.2/tests/programs/package_module_collision/
--rw-rw-rw-   0        0        0      933 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.918182 nuitka_winsvc-2.2.2/tests/programs/package_module_collision/Something/
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_module_collision/Something/__init__.py
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_module_collision/something.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.928455 nuitka_winsvc-2.2.2/tests/programs/package_overload/
--rw-rw-rw-   0        0        0      884 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_overload/Main.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.952716 nuitka_winsvc-2.2.2/tests/programs/package_overload/foo/
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_overload/foo/__init__.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_overload/foo/bar.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_overload/foo/bar2.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.960426 nuitka_winsvc-2.2.2/tests/programs/package_prevents_submodule/
--rw-rw-rw-   0        0        0     3079 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.972568 nuitka_winsvc-2.2.2/tests/programs/package_prevents_submodule/some_package/
--rw-rw-rw-   0        0        0     1111 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:02.162220 nuitka_winsvc-2.2.2/tests/programs/package_program/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.981549 nuitka_winsvc-2.2.2/tests/programs/package_program/PackageAsMain/
--rw-rw-rw-   0        0        0      920 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/package_program/PackageAsMain/__init__.py
--rw-rw-rw-   0        0        0     1661 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/programs/package_program/PackageAsMain/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.982072 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/
--rw-rw-rw-   0        0        0     1760 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:05.991205 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.004310 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.023375 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.026509 nuitka_winsvc-2.2.2/tests/programs/pkgutil_usage/
--rw-rw-rw-   0        0        0     1328 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.039069 nuitka_winsvc-2.2.2/tests/programs/pkgutil_usage/package/
--rw-rw-rw-   0        0        0       13 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-rw-rw-   0        0        0       14 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
--rw-rw-rw-   0        0        0       14 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-rw-rw-   0        0        0     1585 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/pkgutil_usage/package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.042587 nuitka_winsvc-2.2.2/tests/programs/plugin_import/
--rw-rw-rw-   0        0        0      891 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/plugin_import/PluginImportMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.055364 nuitka_winsvc-2.2.2/tests/programs/plugin_import/some_package/
--rw-rw-rw-   0        0        0      803 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/plugin_import/some_package/__init__.py
--rw-rw-rw-   0        0        0      813 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/plugin_import/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.059824 nuitka_winsvc-2.2.2/tests/programs/reimport_main_dynamic/
--rw-rw-rw-   0        0        0      943 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.064819 nuitka_winsvc-2.2.2/tests/programs/reimport_main_static/
--rw-rw-rw-   0        0        0      930 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.073860 nuitka_winsvc-2.2.2/tests/programs/relative_import/
--rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/relative_import/RelativeImportMain.py
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/relative_import/dircache.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.078587 nuitka_winsvc-2.2.2/tests/programs/resource_reader37/
--rw-rw-rw-   0        0        0     1202 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.079586 nuitka_winsvc-2.2.2/tests/programs/resource_reader37/some_package/
--rw-rw-rw-   0        0        0       13 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.2/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/resource_reader37/some_package/__init__.py
--rw-rw-rw-   0        0        0     6614 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/programs/run_all.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.094101 nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/
--rw-rw-rw-   0        0        0     1203 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/pyexpat.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.109875 nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/some_package/
--rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/some_package/__init__.py
--rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/some_package/normal_importing.py
--rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-rw-rw-   0        0        0     1268 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/some_package/star_importing.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.122200 nuitka_winsvc-2.2.2/tests/programs/syntax_errors/
--rw-rw-rw-   0        0        0      822 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/syntax_errors/IndentationErroring.py
--rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/syntax_errors/SyntaxErroring.py
--rw-rw-rw-   0        0        0     1111 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/syntax_errors/SyntaxErrorsMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.133392 nuitka_winsvc-2.2.2/tests/programs/unicode_bom/
--rw-rw-rw-   0        0        0      995 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-rw-rw-   0        0        0      878 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/unicode_bom/unicode_bom.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.134392 nuitka_winsvc-2.2.2/tests/programs/with space/
--rw-rw-rw-   0        0        0      858 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/programs/with space/Space Main.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.140389 nuitka_winsvc-2.2.2/tests/reflected/
--rw-rw-rw-   0        0        0    14254 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/reflected/compile_itself.py
--rw-rw-rw-   0        0        0     1274 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/run-tests
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.208969 nuitka_winsvc-2.2.2/tests/standalone/
--rw-rw-rw-   0        0        0     1090 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/BrotliUsing.py
--rw-rw-rw-   0        0        0     2586 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/CtypesUsing.py
--rw-rw-rw-   0        0        0     1950 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/DateutilsUsing.py
--rw-rw-rw-   0        0        0     1168 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/FlaskUsing.py
--rw-rw-rw-   0        0        0     1307 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/standalone/GiUsing.py
--rw-rw-rw-   0        0        0     1022 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/GlfwUsing.py
--rw-rw-rw-   0        0        0     1216 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/GtkUsing.py
--rw-rw-rw-   0        0        0     1057 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/HexEncodingTest_2.py
--rw-rw-rw-   0        0        0     1118 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/IdnaUsing.py
--rw-rw-rw-   0        0        0     1215 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/LxmlUsing.py
--rw-rw-rw-   0        0        0     1598 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/MatplotlibUsing.py
--rw-rw-rw-   0        0        0     2570 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/MetadataPackagesUsing.py
--rw-rw-rw-   0        0        0     1759 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/NumpyUsing.py
--rw-rw-rw-   0        0        0      979 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/OpenGLUsing.py
--rw-rw-rw-   0        0        0     1479 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PandasUsing.py
--rw-rw-rw-   0        0        0     1098 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PasslibUsing.py
--rw-rw-rw-   0        0        0     1248 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PendulumUsing.py
--rw-rw-rw-   0        0        0     2106 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PkgResourcesRequiresUsing.py
--rw-rw-rw-   0        0        0     1099 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PmwUsing.py
--rw-rw-rw-   0        0        0     1369 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PyQt5Plugins.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PyQt5SSLSupport.py
--rw-rw-rw-   0        0        0     2198 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PyQt5Using.py
--rw-rw-rw-   0        0        0     1203 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PyQt6Plugins.py
--rw-rw-rw-   0        0        0     2168 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PyQt6Using.py
--rw-rw-rw-   0        0        0     1789 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PySide2Using.py
--rw-rw-rw-   0        0        0     1123 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PySide6Plugins.py
--rw-rw-rw-   0        0        0     1789 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/PySide6Using.py
--rw-rw-rw-   0        0        0     1371 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/RsaUsing.py
--rw-rw-rw-   0        0        0     1227 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.2/tests/standalone/SetuptoolsUsing_311.py
--rw-rw-rw-   0        0        0     1005 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/ShlibUsing.py
--rw-rw-rw-   0        0        0     1569 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/SocketUsing.py
--rw-rw-rw-   0        0        0     1973 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/TkInterUsing.py
--rw-rw-rw-   0        0        0     3260 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/Urllib3Using.py
--rw-rw-rw-   0        0        0     1232 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/Win32ComUsing.py
--rw-rw-rw-   0        0        0     9912 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/run_all.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.232668 nuitka_winsvc-2.2.2/tests/standalone/zip_importer/
--rw-rw-rw-   0        0        0     1296 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/standalone/zip_importer/ZipImporterMain.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:23:06.342030 nuitka_winsvc-2.2.2/tests/syntax/
--rw-rw-rw-   0        0        0      844 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/AsyncgenReturn36.py
--rw-rw-rw-   0        0        0      818 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/AwaitInModule36.py
--rw-rw-rw-   0        0        0      901 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/BreakWithoutLoop.py
--rw-rw-rw-   0        0        0      824 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/ClassReturn.py
--rw-rw-rw-   0        0        0     1002 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/ClosureDel_2.py
--rw-rw-rw-   0        0        0      882 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/ContinueWithoutLoop.py
--rw-rw-rw-   0        0        0      824 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/DuplicateArgument.py
--rw-rw-rw-   0        0        0     1142 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/ExecWithNesting_2.py
--rw-rw-rw-   0        0        0      858 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/FutureBraces.py
--rw-rw-rw-   0        0        0      837 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/FutureUnknown.py
--rw-rw-rw-   0        0        0     1073 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/GeneratorExpressions38.py
--rw-rw-rw-   0        0        0      911 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/GeneratorReturn_2.py
--rw-rw-rw-   0        0        0      825 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/GlobalForParameter.py
--rw-rw-rw-   0        0        0     1027 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/Importing32.py
--rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/IndentationError.py
--rw-rw-rw-   0        0        0      947 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/LateFutureImport.py
--rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/MisplacedFutureImport.py
--rw-rw-rw-   0        0        0      832 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/ModuleReturn.py
--rw-rw-rw-   0        0        0      915 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-rw-rw-   0        0        0      827 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/NonlocalForParameter32.py
--rw-rw-rw-   0        0        0      900 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/NonlocalNotFound32.py
--rw-rw-rw-   0        0        0      939 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/StarImportExtra.py
--rw-rw-rw-   0        0        0      900 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/SyntaxError.py
--rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/TryExceptAllNotLast.py
--rw-rw-rw-   0        0        0      908 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/TryFinallyContinue_37.py
--rw-rw-rw-   0        0        0      808 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/UnpackNoTuple.py
--rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/UnpackTwoStars32.py
--rw-rw-rw-   0        0        0      825 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/YieldFromInModule.py
--rw-rw-rw-   0        0        0      837 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/YieldInAsync35.py
--rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/YieldInGenexp38.py
--rw-rw-rw-   0        0        0      813 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/YieldInModule.py
--rw-rw-rw-   0        0        0     2234 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.2/tests/syntax/run_all.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:27.278778 nuitka_winsvc-2.2.3/
+-rw-rw-rw-   0        0        0      235 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/Changelog.rst
+-rw-rw-rw-   0        0        0   152288 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/Developer_Manual.rst
+-rw-rw-rw-   0        0        0    11348 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1717 2024-05-20 02:40:51.000000 nuitka_winsvc-2.2.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:27.277689 nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/
+-rw-rw-rw-   0        0        0     4853 2024-05-20 02:47:20.000000 nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    78230 2024-05-20 02:47:21.000000 nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 02:47:20.000000 nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      308 2024-05-20 02:47:20.000000 nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-02-05 02:20:24.000000 nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-05-20 02:47:20.000000 nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 02:47:20.000000 nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4853 2024-05-20 02:47:27.278778 nuitka_winsvc-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2860 2024-05-20 02:40:51.000000 nuitka_winsvc-2.2.3/README.md
+-rw-rw-rw-   0        0        0    80812 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.273268 nuitka_winsvc-2.2.3/bin/
+-rw-rw-rw-   0        0        0     1166 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/bin/autoformat-nuitka-source
+-rw-rw-rw-   0        0        0     1165 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/bin/check-nuitka-with-pylint
+-rw-rw-rw-   0        0        0     1181 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/bin/compare_with_cpython
+-rw-rw-rw-   0        0        0     3105 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/bin/compare_with_xml
+-rw-rw-rw-   0        0        0     1194 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/bin/measure-construct-performance
+-rw-rw-rw-   0        0        0     1716 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/bin/nuitka
+-rw-rw-rw-   0        0        0     1716 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/bin/nuitka-run
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.304507 nuitka_winsvc-2.2.3/doc/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.334769 nuitka_winsvc-2.2.3/doc/Logo/
+-rw-rw-rw-   0        0        0     1797 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/doc/Logo/Nuitka-Logo-Horizontal.svg
+-rw-rw-rw-   0        0        0     1553 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-rw-rw-   0        0        0     1793 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/doc/Logo/Nuitka-Logo-Vertical.svg
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.364298 nuitka_winsvc-2.2.3/doc/images/
+-rw-rw-rw-   0        0        0     7585 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/doc/images/Nuitka-Logo-Horizontal.png
+-rw-rw-rw-   0        0        0     4452 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/doc/images/Nuitka-Logo-Symbol.png
+-rw-rw-rw-   0        0        0     9828 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/doc/images/Nuitka-Logo-Vertical.png
+-rw-rw-rw-   0        0        0    33696 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/doc/nuitka-run.1
+-rw-rw-rw-   0        0        0    33720 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/doc/nuitka.1
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.381068 nuitka_winsvc-2.2.3/lib/
+-rw-rw-rw-   0        0        0     4640 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/lib/hints.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.391067 nuitka_winsvc-2.2.3/misc/
+-rwxrwxrwx   0        0        0      924 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/misc/nuitka-run.bat
+-rwxrwxrwx   0        0        0     1061 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/misc/nuitka.bat
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.415395 nuitka_winsvc-2.2.3/nuitka/
+-rw-rw-rw-   0        0        0     7560 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/Builtins.py
+-rw-rw-rw-   0        0        0     5787 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/BytecodeCaching.py
+-rw-rw-rw-   0        0        0     3800 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/Bytecodes.py
+-rw-rw-rw-   0        0        0     1855 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/CacheCleanup.py
+-rw-rw-rw-   0        0        0    11181 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/Constants.py
+-rw-rw-rw-   0        0        0     2570 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/Errors.py
+-rw-rw-rw-   0        0        0    11098 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/HardImportRegistry.py
+-rw-rw-rw-   0        0        0    38106 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/MainControl.py
+-rw-rw-rw-   0        0        0     8616 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/ModuleRegistry.py
+-rw-rw-rw-   0        0        0    64062 2024-05-20 02:40:51.000000 nuitka_winsvc-2.2.3/nuitka/OptionParsing.py
+-rw-rw-rw-   0        0        0    76125 2024-05-20 02:40:51.000000 nuitka_winsvc-2.2.3/nuitka/Options.py
+-rw-rw-rw-   0        0        0     5432 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/OutputDirectories.py
+-rw-rw-rw-   0        0        0    15000 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/PostProcessing.py
+-rw-rw-rw-   0        0        0     6805 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/Progress.py
+-rw-rw-rw-   0        0        0     9654 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/PythonFlavors.py
+-rw-rw-rw-   0        0        0     4093 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/PythonOperators.py
+-rw-rw-rw-   0        0        0    14564 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/PythonVersions.py
+-rw-rw-rw-   0        0        0     8989 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/Serialization.py
+-rw-rw-rw-   0        0        0     4703 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/SourceCodeReferences.py
+-rw-rw-rw-   0        0        0    13335 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/Tracing.py
+-rw-rw-rw-   0        0        0     3512 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/TreeXML.py
+-rw-rw-rw-   0        0        0    15470 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/Variables.py
+-rw-rw-rw-   0        0        0     2466 2024-05-20 02:39:31.000000 nuitka_winsvc-2.2.3/nuitka/Version.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/__main__.py
+-rw-rw-rw-   0        0        0     5604 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/__past__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.441681 nuitka_winsvc-2.2.3/nuitka/build/
+-rw-rw-rw-   0        0        0    36409 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/Backend.scons
+-rw-rw-rw-   0        0        0     8583 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/CCompilerVersion.scons
+-rw-rw-rw-   0        0        0     3486 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/DataComposerInterface.py
+-rw-rw-rw-   0        0        0    17786 2024-05-20 02:40:51.000000 nuitka_winsvc-2.2.3/nuitka/build/Onefile.scons
+-rw-rw-rw-   0        0        0    15361 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/SconsCaching.py
+-rw-rw-rw-   0        0        0    35818 2024-05-20 02:40:51.000000 nuitka_winsvc-2.2.3/nuitka/build/SconsCompilerSettings.py
+-rw-rw-rw-   0        0        0     5591 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/SconsHacks.py
+-rw-rw-rw-   0        0        0    17868 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/SconsInterface.py
+-rw-rw-rw-   0        0        0     2703 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/SconsProgress.py
+-rw-rw-rw-   0        0        0    13210 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/SconsSpawn.py
+-rw-rw-rw-   0        0        0    27035 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/SconsUtils.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.110921 nuitka_winsvc-2.2.3/nuitka/build/include/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.792606 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/
+-rw-rw-rw-   0        0        0     8216 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/allocator.h
+-rw-rw-rw-   0        0        0     3499 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/builtins.h
+-rw-rw-rw-   0        0        0     5196 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/calling.h
+-rw-rw-rw-   0        0        0     2006 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/checkers.h
+-rw-rw-rw-   0        0        0     1123 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/checksum_tools.h
+-rw-rw-rw-   0        0        0     9333 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-rw-rw-   0        0        0     2460 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_cell.h
+-rw-rw-rw-   0        0        0     9233 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-rw-rw-   0        0        0    17661 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_frame.h
+-rw-rw-rw-   0        0        0     7267 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_function.h
+-rw-rw-rw-   0        0        0     9189 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_generator.h
+-rw-rw-rw-   0        0        0     1866 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_method.h
+-rw-rw-rw-   0        0        0     7688 2024-04-22 02:58:07.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/constants.h
+-rw-rw-rw-   0        0        0     1345 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/constants_blob.h
+-rw-rw-rw-   0        0        0     1187 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/environment_variables.h
+-rw-rw-rw-   0        0        0     1872 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/environment_variables_system.h
+-rw-rw-rw-   0        0        0     5302 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/exception_groups.h
+-rw-rw-rw-   0        0        0    50867 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/exceptions.h
+-rw-rw-rw-   0        0        0     3792 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-rw-rw-   0        0        0     6474 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/freelists.h
+-rw-rw-rw-   0        0        0    86326 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/hedley.h
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.254327 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/
+-rw-rw-rw-   0        0        0     3698 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/attributes.h
+-rw-rw-rw-   0        0        0     2692 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/boolean.h
+-rw-rw-rw-   0        0        0     1233 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-rw-rw-   0        0        0     1164 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/bytes.h
+-rw-rw-rw-   0        0        0    11894 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-rw-rw-   0        0        0    13169 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-rw-rw-   0        0        0    10645 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-rw-rw-   0        0        0    10644 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-rw-rw-   0        0        0    13169 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-rw-rw-   0        0        0    13168 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-rw-rw-   0        0        0    10645 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-rw-rw-   0        0        0     1834 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/complex.h
+-rw-rw-rw-   0        0        0    13606 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-rw-rw-   0        0        0     1235 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/floats.h
+-rw-rw-rw-   0        0        0     4401 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-rw-rw-   0        0        0     1827 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/indexes.h
+-rw-rw-rw-   0        0        0     3625 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/ints.h
+-rw-rw-rw-   0        0        0     9599 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/iterators.h
+-rw-rw-rw-   0        0        0     3678 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/lists.h
+-rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-rw-rw-   0        0        0     1386 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/mappings.h
+-rw-rw-rw-   0        0        0     4671 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations.h
+-rw-rw-rw-   0        0        0    12714 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-rw-rw-   0        0        0     5692 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-rw-rw-   0        0        0     5670 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-rw-rw-   0        0        0     5692 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-rw-rw-   0        0        0     5451 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-rw-rw-   0        0        0     5489 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-rw-rw-   0        0        0     5144 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-rw-rw-   0        0        0     2828 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-rw-rw-   0        0        0    15807 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-rw-rw-   0        0        0    13239 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-rw-rw-   0        0        0     5820 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-rw-rw-   0        0        0     4743 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-rw-rw-   0        0        0     5144 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-rw-rw-   0        0        0     5853 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-rw-rw-   0        0        0     5467 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-rw-rw-   0        0        0    20173 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-rw-rw-   0        0        0     8699 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-rw-rw-   0        0        0     3796 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-rw-rw-   0        0        0     3782 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-rw-rw-   0        0        0     3796 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-rw-rw-   0        0        0     4875 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-rw-rw-   0        0        0     2756 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-rw-rw-   0        0        0    10655 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-rw-rw-   0        0        0     9230 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-rw-rw-   0        0        0     5176 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-rw-rw-   0        0        0     4378 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-rw-rw-   0        0        0     5004 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-rw-rw-   0        0        0     4855 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-rw-rw-   0        0        0     4072 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/raising.h
+-rw-rw-rw-   0        0        0     2367 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-rw-rw-   0        0        0     1175 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-rw-rw-   0        0        0     1141 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/sequences.h
+-rw-rw-rw-   0        0        0     1054 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/sets.h
+-rw-rw-rw-   0        0        0     8750 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/slices.h
+-rw-rw-rw-   0        0        0     1363 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/strings.h
+-rw-rw-rw-   0        0        0    17975 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-rw-rw-   0        0        0     5926 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/tuples.h
+-rw-rw-rw-   0        0        0    16773 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helpers.h
+-rw-rw-rw-   0        0        0     6050 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/importing.h
+-rw-rw-rw-   0        0        0    12979 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/incbin.h
+-rw-rw-rw-   0        0        0     1086 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/jit_sources.h
+-rw-rw-rw-   0        0        0    16556 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/prelude.h
+-rw-rw-rw-   0        0        0     3239 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/printing.h
+-rw-rw-rw-   0        0        0     1811 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/python_pgo.h
+-rw-rw-rw-   0        0        0     2343 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-rw-rw-   0        0        0     3729 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/threading.h
+-rw-rw-rw-   0        0        0     3447 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/tracing.h
+-rw-rw-rw-   0        0        0     1145 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/type_aliases.h
+-rw-rw-rw-   0        0        0     3135 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/unfreezing.h
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.125870 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.261341 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/appdirs/
+-rw-rw-rw-   0        0        0     1097 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/appdirs/LICENSE.txt
+-rw-rw-rw-   0        0        0    24824 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/appdirs/appdirs.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.264333 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/atomicwrites/
+-rw-rw-rw-   0        0        0     1069 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-rw-rw-   0        0        0     6794 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.265327 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/bin/
+-rw-rw-rw-   0        0        0     1695 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/bin/scons.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.112869 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/clcache/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.268326 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/clcache/clcache/
+-rw-rw-rw-   0        0        0     1585 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-rw-rw-   0        0        0    65424 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.269326 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/
+-rw-rw-rw-   0        0        0     1491 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.272326 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/
+-rw-rw-rw-   0        0        0      243 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10517 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.273327 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/
+-rw-rw-rw-   0        0        0     1359 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.284327 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/glob2/
+-rw-rw-rw-   0        0        0       82 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-rw-rw-   0        0        0     6859 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-rw-rw-   0        0        0     4463 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-rw-rw-   0        0        0     8304 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/glob2/impl.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.296328 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/
+-rw-rw-rw-   0        0        0     1467 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/LICENSE.rst
+-rw-rw-rw-   0        0        0       85 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.313328 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-rw-rw-   0        0        0     2423 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17473 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.325329 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/
+-rw-rw-rw-   0        0        0     1466 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+-rw-rw-rw-   0        0        0       84 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.339330 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-rw-rw-   0        0        0     2616 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17474 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.120869 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.115870 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.351329 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-rw-rw-   0        0        0    47844 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    33996 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0     8083 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27693 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     6938 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    17622 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96183 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7358 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21540 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16000 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9589 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.353331 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-rw-rw-   0        0        0     4197 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   121420 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     4164 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    49503 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.356330 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-rw-rw-   0        0        0     1950 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-rw-rw-   0        0        0     1965 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-rw-rw-   0        0        0     2736 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-rw-rw-   0        0        0     2614 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-rw-rw-   0        0        0     8467 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.361330 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-rw-rw-   0        0        0     9314 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3131 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     1989 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2483 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1718 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1605 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     2170 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4179 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1882 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0    15042 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    39700 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    12950 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.363330 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4810 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3751 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3233 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2011 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    14663 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.366330 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-rw-rw-   0        0        0    14029 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    52665 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    40719 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    24133 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14053 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-rw-rw-   0        0        0    34903 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    40510 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.403332 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2166 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0     2433 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-rw-rw-   0        0        0     2859 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-rw-rw-   0        0        0    18084 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.407331 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2078 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0     9248 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    14869 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    19499 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    20832 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     3763 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-rw-rw-   0        0        0     5149 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0     2290 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-rw-rw-   0        0        0     2328 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-rw-rw-   0        0        0     2657 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-rw-rw-   0        0        0    31283 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2267 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2681 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-rw-rw-   0        0        0     2720 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     2796 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2147 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2936 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2935 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     3432 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3785 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     2777 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1711 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0      142 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.408332 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29618 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3428 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     2681 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     2433 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-rw-rw-   0        0        0     1844 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3472 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     4782 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-rw-rw-   0        0        0     2025 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-rw-rw-   0        0        0     2256 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-rw-rw-   0        0        0     2460 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2639 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1810 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2333 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2140 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1902 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2077 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2043 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    18600 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25816 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     3328 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-rw-rw-   0        0        0     8394 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     3953 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2309 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2945 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     6919 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4381 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4658 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4224 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2168 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    13881 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1804 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    11380 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    72761 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6841 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3579 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2618 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4375 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2827 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2513 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1991 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1819 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2123 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2502 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     4695 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1927 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     2349 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2473 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     5992 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1831 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3730 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13016 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3415 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    48938 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.411332 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3007 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4380 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3557 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5612 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11034 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6824 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1563 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.415331 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-rw-rw-   0        0        0     8120 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     3596 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-rw-rw-   0        0        0     1818 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-rw-rw-   0        0        0     1742 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     2465 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-rw-rw-   0        0        0     1776 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-rw-rw-   0        0        0    19253 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-rw-rw-   0        0        0    44500 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-rw-rw-   0        0        0    19664 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     7509 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2107 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.117870 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.428333 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-rw-rw-   0        0        0    53545 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    34985 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0    13596 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    28403 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7533 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    20988 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96818 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7752 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    22350 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16068 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9565 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.430333 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-rw-rw-   0        0        0     5239 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   135413 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     5758 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63474 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8354 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.436332 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-rw-rw-   0        0        0    11500 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3180 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2227 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2739 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1767 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1654 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1460 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2219 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4476 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1931 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     4003 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    17055 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41186 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    13880 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.438332 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4853 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3812 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3643 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2328 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15053 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.441332 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-rw-rw-   0        0        0    13779 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53260 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    39394 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26467 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14489 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    35863 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    42204 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.475392 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2211 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    18207 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.479394 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2152 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    10674 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2855 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15165 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    33537 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    21762 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4464 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    50660 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2316 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2475 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2840 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     8618 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2226 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2978 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2977 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1653 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3827 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3389 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.480393 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      313 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3631 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3444 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     8494 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1753 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.480393 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29765 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3472 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1630 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1977 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3686 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2580 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2948 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2655 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1645 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1859 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2765 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2386 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2189 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1944 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2123 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2085 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    15791 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    26195 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0    13924 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     4041 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2351 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2987 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     7808 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4956 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     5235 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4808 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2475 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14751 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1847 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12588 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    82939 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6883 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3663 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2660 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4904 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2877 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2567 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1652 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1868 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2088 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2176 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2366 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1658 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1976 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     5335 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2583 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2515 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6756 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1873 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3773 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13982 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3201 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    53803 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.483393 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3064 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3818 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4435 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3643 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5579 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11655 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6504 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1647 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.484393 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-rw-rw-   0        0        0     6869 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0    19816 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9002 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2149 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.120869 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.505393 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-rw-rw-   0        0        0    56578 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-rw-rw-   0        0        0    35213 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+-rw-rw-rw-   0        0        0    11061 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27408 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7884 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-rw-rw-   0        0        0    21423 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    97269 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-rw-rw-   0        0        0     3979 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+-rw-rw-rw-   0        0        0     7515 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21937 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16583 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-rw-rw-   0        0        0     9430 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.508394 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-rw-rw-   0        0        0     5126 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   136271 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     6167 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63768 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8183 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.515396 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-rw-rw-   0        0        0    12836 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2107 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2630 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1674 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1536 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1311 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2076 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4356 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1805 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     3860 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    14831 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41983 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-rw-rw-   0        0        0    14673 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.518395 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-rw-rw-   0        0        0     7394 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     4357 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3546 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     1972 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15577 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.521396 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-rw-rw-   0        0        0    13597 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53509 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    42760 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26676 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14272 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    36753 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-rw-rw-   0        0        0    41191 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.558395 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-rw-rw-   0        0        0     2122 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    15570 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.564397 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2014 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    13182 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2734 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15027 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    38783 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    22570 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4368 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    32724 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1578 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2228 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2386 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2616 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     7993 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2141 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     1661 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2893 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-rw-rw-   0        0        0     2889 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1567 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3742 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3296 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.565395 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      343 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3534 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3259 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     7461 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1663 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0     3379 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1544 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1891 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3616 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2377 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2437 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2526 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1557 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1772 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2677 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2206 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2096 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1851 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     1954 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     1995 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    19180 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25826 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     2588 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.579843 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-rw-rw-   0        0        0     4649 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-rw-rw-   0        0        0     7652 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-rw-rw-   0        0        0     6064 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-rw-rw-   0        0        0     3931 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2266 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2900 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     8622 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4577 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4517 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4113 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2387 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14473 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1752 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12902 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    84784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6788 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3576 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4817 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2788 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2479 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1563 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1780 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     1999 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2006 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2271 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1569 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1888 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     4879 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2419 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2429 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6412 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1786 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3687 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    12548 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     4076 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    71693 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.585352 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-rw-rw-   0        0        0     6632 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-rw-rw-   0        0        0    15278 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.588353 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-rw-rw-   0        0        0     3134 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3896 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4648 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3536 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5588 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    12708 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-rw-rw-   0        0        0      353 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.590352 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-rw-rw-   0        0        0     4307 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     3395 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-rw-rw-   0        0        0    21614 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9295 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2032 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.590352 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/
+-rw-rw-rw-   0        0        0     1467 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.604353 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-rw-rw-   0        0        0    10126 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-rw-rw-   0        0        0     4690 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-rw-rw-   0        0        0     1873 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.123869 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/pkg_resources/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.605352 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-rw-rw-   0        0        0   107335 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.124870 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.613898 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-rw-rw-   0        0        0     1595 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-rw-rw-   0        0        0     3687 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-rw-rw-   0        0        0      283 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-rw-rw-   0        0        0      307 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-rw-rw-   0        0        0      888 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-rw-rw-   0        0        0      596 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-rw-rw-   0        0        0     1106 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-rw-rw-   0        0        0      857 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-rw-rw-   0        0        0     1376 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-rw-rw-   0        0        0    10790 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-rw-rw-   0        0        0    57572 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-rw-rw-   0        0        0     6948 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+-rw-rw-rw-   0        0        0     9726 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-rw-rw-   0        0        0       99 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/version.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.613898 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/
+-rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.632898 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/
+-rw-rw-rw-   0        0        0    13170 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4883 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-rw-rw-   0        0        0    28639 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3851 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2837 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43006 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-rw-rw-   0        0        0     2061 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-rw-rw-   0        0        0     6794 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-rw-rw-   0        0        0    14184 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-rw-rw-   0        0        0     8999 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51277 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.632898 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/
+-rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.671904 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-rw-rw-   0        0        0     9776 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4921 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-rw-rw-   0        0        0    25145 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3290 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2719 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43298 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2559 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-rw-rw-   0        0        0     1132 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25542 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-rw-rw-   0        0        0     6746 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-rw-rw-   0        0        0    17711 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-rw-rw-   0        0        0     9122 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-rw-rw-   0        0        0    52446 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4171 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.671904 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/
+-rw-rw-rw-   0        0        0     1101 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.685901 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-rw-rw-   0        0        0     9607 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4881 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-rw-rw-   0        0        0    25554 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3294 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2723 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+-rw-rw-rw-   0        0        0    42954 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-rw-rw-   0        0        0     1138 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-rw-rw-   0        0        0     6854 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-rw-rw-   0        0        0    14097 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-rw-rw-   0        0        0     8970 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51695 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.728901 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/
+-rw-rw-rw-   0        0        0     1002 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/LICENSE
+-rw-rw-rw-   0        0        0    31605 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/crc32.c
+-rw-rw-rw-   0        0        0   591749 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/crc32.h
+-rw-rw-rw-   0        0        0    16682 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/zconf.h
+-rw-rw-rw-   0        0        0    96778 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/zlib.h
+-rw-rw-rw-   0        0        0     7247 2023-12-06 01:19:25.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/zutil.h
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.748902 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/
+-rw-rw-rw-   0        0        0     1530 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.826905 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/
+-rw-rw-rw-   0        0        0    18198 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-rw-rw-   0        0        0    10157 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/compiler.h
+-rw-rw-rw-   0        0        0     4455 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-rw-rw-   0        0        0     3763 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-rw-rw-   0        0        0    13662 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-rw-rw-   0        0        0     3009 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-rw-rw-   0        0        0     2441 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-rw-rw-   0        0        0    34422 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-rw-rw-   0        0        0    14748 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-rw-rw-   0        0        0    20216 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-rw-rw-   0        0        0    13930 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-rw-rw-   0        0        0    26976 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-rw-rw-   0        0        0    11706 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-rw-rw-   0        0        0     2728 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-rw-rw-   0        0        0     2497 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-rw-rw-   0        0        0     3828 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-rw-rw-   0        0        0    15880 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:22.839512 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/
+-rw-rw-rw-   0        0        0    54982 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-rw-rw-   0        0        0     9164 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-rw-rw-   0        0        0     1321 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-rw-rw-   0        0        0    80283 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-rw-rw-   0        0        0    66784 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-rw-rw-   0        0        0     2253 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-rw-rw-   0        0        0     7906 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-rw-   0        0        0   138334 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/zstd.h
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.807495 nuitka_winsvc-2.2.3/nuitka/build/static_src/
+-rw-rw-rw-   0        0        0    83526 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-rw-rw-   0        0        0     9142 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledCellType.c
+-rw-rw-rw-   0        0        0    58846 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-rw-rw-   0        0        0    72002 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-rw-rw-   0        0        0    40762 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledFrameType.c
+-rw-rw-rw-   0        0        0   110213 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledFunctionType.c
+-rw-rw-rw-   0        0        0    67599 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-rw-rw-   0        0        0    56411 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-rw-rw-   0        0        0    22466 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledMethodType.c
+-rw-rw-rw-   0        0        0    19054 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersAllocator.c
+-rw-rw-rw-   0        0        0    37583 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersAttributes.c
+-rw-rw-rw-   0        0        0    23690 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersBuiltin.c
+-rw-rw-rw-   0        0        0   114017 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-rw-rw-   0        0        0     3062 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersBytes.c
+-rw-rw-rw-   0        0        0    13376 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersCalling.c
+-rw-rw-rw-   0        0        0   481627 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-rw-rw-   0        0        0     2065 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-rw-rw-   0        0        0     3051 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersClasses.c
+-rw-rw-rw-   0        0        0   318889 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-rw-rw-   0        0        0     4762 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-rw-rw-   0        0        0   314072 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-rw-rw-   0        0        0   313483 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-rw-rw-   0        0        0   317286 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-rw-rw-   0        0        0   316697 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-rw-rw-   0        0        0   315637 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-rw-rw-   0        0        0    36776 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-rw-rw-   0        0        0    20243 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-rw-rw-   0        0        0    39785 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersDictionaries.c
+-rw-rw-rw-   0        0        0    26620 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-rw-rw-   0        0        0     2066 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersDumpBacktraces.c
+-rw-rw-rw-   0        0        0     2194 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersEnvironmentVariables.c
+-rw-rw-rw-   0        0        0     2979 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c
+-rw-rw-rw-   0        0        0     7966 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersExceptions.c
+-rw-rw-rw-   0        0        0     8349 2024-04-22 02:58:07.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersFiles.c
+-rw-rw-rw-   0        0        0    28776 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-rw-rw-   0        0        0     2455 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersFloats.c
+-rw-rw-rw-   0        0        0     1803 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-rw-rw-   0        0        0    16080 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersImport.c
+-rw-rw-rw-   0        0        0    16843 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersImportHard.c
+-rw-rw-rw-   0        0        0     1815 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersJitSources.c
+-rw-rw-rw-   0        0        0    21107 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersLists.c
+-rw-rw-rw-   0        0        0    13944 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-rw-rw-   0        0        0     1669 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersMappings.c
+-rw-rw-rw-   0        0        0     3587 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersMatching.c
+-rw-rw-rw-   0        0        0   182227 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-rw-rw-   0        0        0    19904 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-rw-rw-   0        0        0    77972 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-rw-rw-   0        0        0    77811 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-rw-rw-   0        0        0    77972 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+-rw-rw-rw-   0        0        0    68218 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-rw-rw-   0        0        0     1265 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-rw-rw-   0        0        0    69479 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-rw-rw-   0        0        0     6300 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-rw-rw-   0        0        0    83954 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-rw-rw-   0        0        0    13805 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-rw-rw-   0        0        0   183867 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-rw-rw-   0        0        0   188543 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-rw-rw-   0        0        0     3593 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-rw-rw-   0        0        0    67184 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-rw-rw-   0        0        0    79484 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-rw-rw-   0        0        0     1052 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-rw-rw-   0        0        0    77854 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-rw-rw-   0        0        0    70851 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-rw-rw-   0        0        0    68736 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-rw-rw-   0        0        0   151107 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-rw-rw-   0        0        0     4242 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-rw-rw-   0        0        0    53253 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-rw-rw-   0        0        0    53151 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-rw-rw-   0        0        0    53253 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-rw-rw-   0        0        0    77119 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-rw-rw-   0        0        0    47857 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-rw-rw-   0        0        0    17771 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-rw-rw-   0        0        0   136385 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-rw-rw-   0        0        0   142240 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-rw-rw-   0        0        0    74749 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-rw-rw-   0        0        0    83262 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-rw-rw-   0        0        0    45341 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-rw-rw-   0        0        0    83275 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-rw-rw-   0        0        0    76950 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-rw-rw-   0        0        0     3294 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersProfiling.c
+-rw-rw-rw-   0        0        0     3840 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-rw-rw-   0        0        0    18257 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersRaising.c
+-rw-rw-rw-   0        0        0     3868 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-rw-rw-   0        0        0     3759 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersSequences.c
+-rw-rw-rw-   0        0        0     1975 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersSlices.c
+-rw-rw-rw-   0        0        0    32297 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersStrings.c
+-rw-rw-rw-   0        0        0     4181 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersTuples.c
+-rw-rw-rw-   0        0        0     6786 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersTypes.c
+-rw-rw-rw-   0        0        0    12136 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/InspectPatcher.c
+-rw-rw-rw-   0        0        0    54011 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/MainProgram.c
+-rw-rw-rw-   0        0        0    63771 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-rw-rw-   0        0        0     4827 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-rw-rw-   0        0        0     6651 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-rw-rw-   0        0        0    21896 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-rw-rw-   0        0        0    37074 2024-05-20 02:40:51.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/OnefileBootstrap.c
+-rw-rw-rw-   0        0        0     8050 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/build/static_src/OnefileSplashScreen.cpp
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.851512 nuitka_winsvc-2.2.3/nuitka/code_generation/
+-rw-rw-rw-   0        0        0     6491 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/AsyncgenCodes.py
+-rw-rw-rw-   0        0        0    10821 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/AttributeCodes.py
+-rw-rw-rw-   0        0        0    21926 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-rw-rw-   0        0        0     2371 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/BranchCodes.py
+-rw-rw-rw-   0        0        0    17006 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/BuiltinCodes.py
+-rw-rw-rw-   0        0        0    36111 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/CallCodes.py
+-rw-rw-rw-   0        0        0     4958 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ClassCodes.py
+-rw-rw-rw-   0        0        0    53395 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/CodeGeneration.py
+-rw-rw-rw-   0        0        0     2408 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/CodeHelperSelection.py
+-rw-rw-rw-   0        0        0    14320 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/CodeHelpers.py
+-rw-rw-rw-   0        0        0     5147 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/CodeObjectCodes.py
+-rw-rw-rw-   0        0        0    17957 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ComparisonCodes.py
+-rw-rw-rw-   0        0        0     4479 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-rw-rw-   0        0        0     7368 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ConditionalCodes.py
+-rw-rw-rw-   0        0        0     6901 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ConstantCodes.py
+-rw-rw-rw-   0        0        0    34299 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/Contexts.py
+-rw-rw-rw-   0        0        0     8589 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/CoroutineCodes.py
+-rw-rw-rw-   0        0        0     1607 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/CtypesCodes.py
+-rw-rw-rw-   0        0        0    28934 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/DictCodes.py
+-rw-rw-rw-   0        0        0     2159 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/Emission.py
+-rw-rw-rw-   0        0        0     9289 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ErrorCodes.py
+-rw-rw-rw-   0        0        0    12983 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/EvalCodes.py
+-rw-rw-rw-   0        0        0     9243 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ExceptionCodes.py
+-rw-rw-rw-   0        0        0     7384 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-rw-rw-   0        0        0     2126 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ExpressionCodes.py
+-rw-rw-rw-   0        0        0    17852 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/FrameCodes.py
+-rw-rw-rw-   0        0        0    28336 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/FunctionCodes.py
+-rw-rw-rw-   0        0        0     7836 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/GeneratorCodes.py
+-rw-rw-rw-   0        0        0     6363 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/GlobalConstants.py
+-rw-rw-rw-   0        0        0     6985 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-rw-rw-   0        0        0     1870 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/IdCodes.py
+-rw-rw-rw-   0        0        0    14727 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ImportCodes.py
+-rw-rw-rw-   0        0        0     1429 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/Indentation.py
+-rw-rw-rw-   0        0        0     1574 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/IndexCodes.py
+-rw-rw-rw-   0        0        0     1066 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/InjectCCodes.py
+-rw-rw-rw-   0        0        0     3567 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/IntegerCodes.py
+-rw-rw-rw-   0        0        0    12211 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/IteratorCodes.py
+-rw-rw-rw-   0        0        0     1620 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/JitCodes.py
+-rw-rw-rw-   0        0        0     2055 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/LabelCodes.py
+-rw-rw-rw-   0        0        0     2645 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/LineNumberCodes.py
+-rw-rw-rw-   0        0        0    15849 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ListCodes.py
+-rw-rw-rw-   0        0        0     6658 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/LoaderCodes.py
+-rw-rw-rw-   0        0        0    10016 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/LocalsDictCodes.py
+-rw-rw-rw-   0        0        0     3174 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/LoopCodes.py
+-rw-rw-rw-   0        0        0     1637 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/MatchCodes.py
+-rw-rw-rw-   0        0        0     6525 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ModuleCodes.py
+-rw-rw-rw-   0        0        0     8224 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/Namify.py
+-rw-rw-rw-   0        0        0     1860 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/NetworkxCodes.py
+-rw-rw-rw-   0        0        0    12733 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/OperationCodes.py
+-rw-rw-rw-   0        0        0    30198 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/PackageResourceCodes.py
+-rw-rw-rw-   0        0        0     3054 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/PrintCodes.py
+-rw-rw-rw-   0        0        0     5670 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/PythonAPICodes.py
+-rw-rw-rw-   0        0        0    13251 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/RaisingCodes.py
+-rw-rw-rw-   0        0        0     3476 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/Reports.py
+-rw-rw-rw-   0        0        0     5267 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/ReturnCodes.py
+-rw-rw-rw-   0        0        0     6591 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/SetCodes.py
+-rw-rw-rw-   0        0        0    14005 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/SliceCodes.py
+-rw-rw-rw-   0        0        0    10087 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/StringCodes.py
+-rw-rw-rw-   0        0        0     8302 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/SubscriptCodes.py
+-rw-rw-rw-   0        0        0     1939 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/TensorflowCodes.py
+-rw-rw-rw-   0        0        0    11208 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/TryCodes.py
+-rw-rw-rw-   0        0        0     3840 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/TupleCodes.py
+-rw-rw-rw-   0        0        0     2362 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/TypeAliasCodes.py
+-rw-rw-rw-   0        0        0    14811 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/VariableCodes.py
+-rw-rw-rw-   0        0        0     9155 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/VariableDeclarations.py
+-rw-rw-rw-   0        0        0     8129 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/YieldCodes.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.858497 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/
+-rw-rw-rw-   0        0        0     6102 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeBases.py
+-rw-rw-rw-   0        0        0     3432 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-rw-rw-   0        0        0     1837 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-rw-rw-   0        0        0     1410 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-rw-rw-   0        0        0     3642 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-rw-rw-   0        0        0     5161 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-rw-rw-   0        0        0     5243 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-rw-rw-   0        0        0     3988 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-rw-rw-   0        0        0    19696 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-rw-rw-   0        0        0     2886 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.864497 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/
+-rw-rw-rw-   0        0        0     2948 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-rw-rw-   0        0        0     9455 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-rw-rw-   0        0        0     3040 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-rw-rw-   0        0        0     2439 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-rw-rw-   0        0        0     6483 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-rw-rw-   0        0        0     3460 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-rw-rw-   0        0        0     3390 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-rw-rw-   0        0        0     2408 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-rw-rw-   0        0        0     4534 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-rw-rw-   0        0        0    23021 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-rw-rw-   0        0        0     6840 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-rw-rw-   0        0        0     2507 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.975929 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/
+-rw-rw-rw-   0        0        0    11318 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-rw-rw-   0        0        0     5829 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-rw-rw-   0        0        0    23986 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-rw-rw-   0        0        0     5438 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-rw-rw-   0        0        0     1755 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-rw-rw-   0        0        0     1693 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-rw-rw-   0        0        0     2706 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-rw-rw-   0        0        0    13624 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-rw-rw-   0        0        0     1894 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-rw-rw-   0        0        0     2618 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-rw-rw-   0        0        0     1394 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-rw-rw-   0        0        0     7047 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-rw-rw-   0        0        0    12700 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-rw-rw-   0        0        0     4138 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-rw-rw-   0        0        0     1938 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-rw-rw-   0        0        0     1968 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-rw-rw-   0        0        0     4081 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-rw-rw-   0        0        0     7257 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-rw-rw-   0        0        0     4142 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-rw-rw-   0        0        0     3710 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-rw-rw-   0        0        0     4447 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-rw-rw-   0        0        0    11758 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-rw-rw-   0        0        0    19167 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-rw-rw-   0        0        0     2693 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-rw-rw-   0        0        0     3485 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-rw-rw-   0        0        0    11336 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-rw-rw-   0        0        0    15540 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-rw-rw-   0        0        0     2829 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-rw-rw-   0        0        0    10395 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-rw-rw-   0        0        0     2407 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-rw-rw-   0        0        0     2870 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-rw-rw-   0        0        0     2834 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-rw-rw-   0        0        0     3128 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.978929 nuitka_winsvc-2.2.3/nuitka/containers/
+-rw-rw-rw-   0        0        0     1467 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/containers/Namedtuples.py
+-rw-rw-rw-   0        0        0     6553 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/containers/OrderedDicts.py
+-rw-rw-rw-   0        0        0      554 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/nuitka/containers/OrderedSets.py
+-rw-rw-rw-   0        0        0     4430 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/containers/OrderedSetsFallback.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.980929 nuitka_winsvc-2.2.3/nuitka/distutils/
+-rw-rw-rw-   0        0        0     2308 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/distutils/Build.py
+-rw-rw-rw-   0        0        0    15025 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/distutils/DistutilCommands.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/distutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.982929 nuitka_winsvc-2.2.3/nuitka/finalizations/
+-rw-rw-rw-   0        0        0     1258 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/finalizations/Finalization.py
+-rw-rw-rw-   0        0        0     6058 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/finalizations/FinalizeMarkups.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/finalizations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.988929 nuitka_winsvc-2.2.3/nuitka/freezer/
+-rw-rw-rw-   0        0        0     7778 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/freezer/DependsExe.py
+-rw-rw-rw-   0        0        0     2616 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/freezer/DllDependenciesCommon.py
+-rw-rw-rw-   0        0        0    14396 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/freezer/DllDependenciesMacOS.py
+-rw-rw-rw-   0        0        0     7468 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/freezer/DllDependenciesPosix.py
+-rw-rw-rw-   0        0        0     6698 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.3/nuitka/freezer/DllDependenciesWin32.py
+-rw-rw-rw-   0        0        0    11979 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/freezer/ImportDetection.py
+-rw-rw-rw-   0        0        0    19236 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/freezer/IncludedDataFiles.py
+-rw-rw-rw-   0        0        0    11455 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/freezer/IncludedEntryPoints.py
+-rw-rw-rw-   0        0        0    10516 2024-05-20 02:40:51.000000 nuitka_winsvc-2.2.3/nuitka/freezer/Onefile.py
+-rw-rw-rw-   0        0        0    12245 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/freezer/Standalone.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/freezer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:24.992929 nuitka_winsvc-2.2.3/nuitka/importing/
+-rw-rw-rw-   0        0        0    11040 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/importing/IgnoreListing.py
+-rw-rw-rw-   0        0        0     2956 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/importing/ImportCache.py
+-rw-rw-rw-   0        0        0     7784 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/importing/ImportResolving.py
+-rw-rw-rw-   0        0        0    32895 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/importing/Importing.py
+-rw-rw-rw-   0        0        0     4869 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/importing/PreloadedPackages.py
+-rw-rw-rw-   0        0        0    18804 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/importing/Recursion.py
+-rw-rw-rw-   0        0        0    12787 2024-04-07 02:15:13.000000 nuitka_winsvc-2.2.3/nuitka/importing/StandardLibrary.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/importing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.040931 nuitka_winsvc-2.2.3/nuitka/nodes/
+-rw-rw-rw-   0        0        0     3670 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/AsyncgenNodes.py
+-rw-rw-rw-   0        0        0     4115 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/AttributeLookupNodes.py
+-rw-rw-rw-   0        0        0    13255 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/AttributeNodes.py
+-rw-rw-rw-   0        0        0   379568 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/AttributeNodesGenerated.py
+-rw-rw-rw-   0        0        0     3856 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinAllNodes.py
+-rw-rw-rw-   0        0        0     4131 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinAnyNodes.py
+-rw-rw-rw-   0        0        0     2530 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinComplexNodes.py
+-rw-rw-rw-   0        0        0     1731 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-rw-rw-   0        0        0     2760 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-rw-rw-   0        0        0     4727 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinDictNodes.py
+-rw-rw-rw-   0        0        0     4982 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinFormatNodes.py
+-rw-rw-rw-   0        0        0     2275 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinHashNodes.py
+-rw-rw-rw-   0        0        0     1457 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinInputNodes.py
+-rw-rw-rw-   0        0        0     5367 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-rw-rw-   0        0        0    12812 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-rw-rw-   0        0        0     2029 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinLenNodes.py
+-rw-rw-rw-   0        0        0     3639 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinNextNodes.py
+-rw-rw-rw-   0        0        0     3787 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinOpenNodes.py
+-rw-rw-rw-   0        0        0   246360 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-rw-rw-   0        0        0    18648 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinRangeNodes.py
+-rw-rw-rw-   0        0        0     9468 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinRefNodes.py
+-rw-rw-rw-   0        0        0     3353 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinSumNodes.py
+-rw-rw-rw-   0        0        0    13576 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinTypeNodes.py
+-rw-rw-rw-   0        0        0     1605 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinVarsNodes.py
+-rw-rw-rw-   0        0        0    26146 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/BytesNodes.py
+-rw-rw-rw-   0        0        0     6511 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/CallNodes.py
+-rw-rw-rw-   0        0        0     1583 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/Checkers.py
+-rw-rw-rw-   0        0        0   647748 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ChildrenHavingMixins.py
+-rw-rw-rw-   0        0        0     8480 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ClassNodes.py
+-rw-rw-rw-   0        0        0     6622 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/CodeObjectSpecs.py
+-rw-rw-rw-   0        0        0    21716 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ComparisonNodes.py
+-rw-rw-rw-   0        0        0    30191 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ConditionalNodes.py
+-rw-rw-rw-   0        0        0    47737 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ConstantRefNodes.py
+-rw-rw-rw-   0        0        0    12246 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ContainerMakingNodes.py
+-rw-rw-rw-   0        0        0     2867 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ContainerOperationNodes.py
+-rw-rw-rw-   0        0        0     4614 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/CoroutineNodes.py
+-rw-rw-rw-   0        0        0     1746 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/CtypesNodes.py
+-rw-rw-rw-   0        0        0    51053 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/DictionaryNodes.py
+-rw-rw-rw-   0        0        0     8151 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ExceptionNodes.py
+-rw-rw-rw-   0        0        0     7408 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ExecEvalNodes.py
+-rw-rw-rw-   0        0        0    45046 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ExpressionBases.py
+-rw-rw-rw-   0        0        0    55956 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-rw-rw-   0        0        0    21311 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ExpressionShapeMixins.py
+-rw-rw-rw-   0        0        0    12024 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/FrameNodes.py
+-rw-rw-rw-   0        0        0     3577 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/FunctionAttributeNodes.py
+-rw-rw-rw-   0        0        0    41167 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/FunctionNodes.py
+-rw-rw-rw-   0        0        0     5409 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/FutureSpecs.py
+-rw-rw-rw-   0        0        0     6288 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/GeneratorNodes.py
+-rw-rw-rw-   0        0        0     6961 2024-04-07 02:15:13.000000 nuitka_winsvc-2.2.3/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-rw-rw-   0        0        0    98222 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/HardImportNodesGenerated.py
+-rw-rw-rw-   0        0        0     5631 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ImportHardNodes.py
+-rw-rw-rw-   0        0        0    48286 2024-05-15 06:21:28.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ImportNodes.py
+-rw-rw-rw-   0        0        0     2766 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/IndicatorMixins.py
+-rw-rw-rw-   0        0        0     1533 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/InjectCNodes.py
+-rw-rw-rw-   0        0        0    11519 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/IterationHandles.py
+-rw-rw-rw-   0        0        0    11035 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/KeyValuePairNodes.py
+-rw-rw-rw-   0        0        0    16821 2024-03-14 05:29:37.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ListOperationNodes.py
+-rw-rw-rw-   0        0        0    23177 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/LocalsDictNodes.py
+-rw-rw-rw-   0        0        0    15007 2024-03-06 05:39:35.000000 nuitka_winsvc-2.2.3/nuitka/nodes/LocalsScopes.py
+-rw-rw-rw-   0        0        0    15995 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/LoopNodes.py
+-rw-rw-rw-   0        0        0     1745 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/MatchNodes.py
+-rw-rw-rw-   0        0        0     6567 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ModuleAttributeNodes.py
+-rw-rw-rw-   0        0        0    32830 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ModuleNodes.py
+-rw-rw-rw-   0        0        0     1759 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/NetworkxNodes.py
+-rw-rw-rw-   0        0        0    24461 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/NodeBases.py
+-rw-rw-rw-   0        0        0    15147 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/NodeMakingHelpers.py
+-rw-rw-rw-   0        0        0     5580 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/NodeMetaClasses.py
+-rw-rw-rw-   0        0        0    31948 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/OperatorNodes.py
+-rw-rw-rw-   0        0        0     8976 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/OperatorNodesUnary.py
+-rw-rw-rw-   0        0        0     5228 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/OsSysNodes.py
+-rw-rw-rw-   0        0        0    12468 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/OutlineNodes.py
+-rw-rw-rw-   0        0        0    34735 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/PackageMetadataNodes.py
+-rw-rw-rw-   0        0        0    12289 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/PackageResourceNodes.py
+-rw-rw-rw-   0        0        0     3440 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/PrintNodes.py
+-rw-rw-rw-   0        0        0     6805 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/ReturnNodes.py
+-rw-rw-rw-   0        0        0     4748 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/SideEffectNodes.py
+-rw-rw-rw-   0        0        0    12547 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/SliceNodes.py
+-rw-rw-rw-   0        0        0    98808 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/StatementBasesGenerated.py
+-rw-rw-rw-   0        0        0     9336 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/StatementNodes.py
+-rw-rw-rw-   0        0        0    28691 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/StrNodes.py
+-rw-rw-rw-   0        0        0     3538 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/StringConcatenationNodes.py
+-rw-rw-rw-   0        0        0     8329 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/SubscriptNodes.py
+-rw-rw-rw-   0        0        0     1411 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/TensorflowNodes.py
+-rw-rw-rw-   0        0        0    17886 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/TryNodes.py
+-rw-rw-rw-   0        0        0     2438 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/TypeMatchNodes.py
+-rw-rw-rw-   0        0        0    11717 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/TypeNodes.py
+-rw-rw-rw-   0        0        0    42396 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/VariableAssignNodes.py
+-rw-rw-rw-   0        0        0    10779 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/VariableDelNodes.py
+-rw-rw-rw-   0        0        0     4607 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/VariableNameNodes.py
+-rw-rw-rw-   0        0        0    31274 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/VariableRefNodes.py
+-rw-rw-rw-   0        0        0     4781 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/VariableReleaseNodes.py
+-rw-rw-rw-   0        0        0     3937 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/YieldNodes.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.042932 nuitka_winsvc-2.2.3/nuitka/nodes/shapes/
+-rw-rw-rw-   0        0        0   157357 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-rw-rw-   0        0        0     4420 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-rw-rw-   0        0        0     5076 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/shapes/ShapeMixins.py
+-rw-rw-rw-   0        0        0    42509 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/shapes/StandardShapes.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/nodes/shapes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.047933 nuitka_winsvc-2.2.3/nuitka/optimizations/
+-rw-rw-rw-   0        0        0     3358 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/optimizations/BytecodeDemotion.py
+-rw-rw-rw-   0        0        0     3953 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/optimizations/FunctionInlining.py
+-rw-rw-rw-   0        0        0     2177 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/optimizations/Graphs.py
+-rw-rw-rw-   0        0        0    10917 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/optimizations/Optimization.py
+-rw-rw-rw-   0        0        0    52575 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-rw-rw-   0        0        0     2287 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/optimizations/Tags.py
+-rw-rw-rw-   0        0        0    42800 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/optimizations/TraceCollections.py
+-rw-rw-rw-   0        0        0    25799 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/optimizations/ValueTraces.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/optimizations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.048941 nuitka_winsvc-2.2.3/nuitka/pgo/
+-rw-rw-rw-   0        0        0     4932 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/pgo/PGO.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/pgo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.049932 nuitka_winsvc-2.2.3/nuitka/plugins/
+-rw-rw-rw-   0        0        0    57735 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/PluginBase.py
+-rw-rw-rw-   0        0        0    60905 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/Plugins.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.071932 nuitka_winsvc-2.2.3/nuitka/plugins/standard/
+-rw-rw-rw-   0        0        0    30813 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-rw-rw-   0        0        0     3509 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-rw-rw-   0        0        0    10627 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-rw-rw-   0        0        0     5080 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/DelvewheelPlugin.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.086817 nuitka_winsvc-2.2.3/nuitka/plugins/standard/DillPlugin/
+-rw-rw-rw-   0        0        0     1646 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/DillPlugin/DillPlugin.c
+-rw-rw-rw-   0        0        0     9826 2024-03-25 02:50:30.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/DillPlugin/dill-postLoad.py
+-rw-rw-rw-   0        0        0     2679 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/DillPlugin.py
+-rw-rw-rw-   0        0        0    16496 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-rw-rw-   0        0        0     2095 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/EnumPlugin.py
+-rw-rw-rw-   0        0        0     1938 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/EventletPlugin.py
+-rw-rw-rw-   0        0        0     1913 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/GeventPlugin.py
+-rw-rw-rw-   0        0        0     4018 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/GiPlugin.py
+-rw-rw-rw-   0        0        0     4854 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/GlfwPlugin.py
+-rw-rw-rw-   0        0        0    32325 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/ImplicitImports.py
+-rw-rw-rw-   0        0        0     5024 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/KivyPlugin.py
+-rw-rw-rw-   0        0        0     8824 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-rw-rw-   0        0        0     7080 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-rw-rw-   0        0        0     1220 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/NumpyPlugin.py
+-rw-rw-rw-   0        0        0     7299 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-rw-rw-   0        0        0     1940 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/PbrPlugin.py
+-rw-rw-rw-   0        0        0     4874 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-rw-rw-   0        0        0     7216 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/PmwPlugin.py
+-rw-rw-rw-   0        0        0    51929 2024-05-20 02:39:31.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-rw-rw-   0        0        0     3020 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-rw-rw-   0        0        0     1194 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-rw-rw-   0        0        0    13878 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/TkinterPlugin.py
+-rw-rw-rw-   0        0        0     1174 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/TorchPlugin.py
+-rw-rw-rw-   0        0        0    12838 2024-04-07 02:15:13.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/TransformersPlugin.py
+-rw-rw-rw-   0        0        0     1107 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/TrioPlugin.py
+-rw-rw-rw-   0        0        0     5668 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/UpxPlugin.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/__init__.py
+-rw-rw-rw-   0        0        0   236681 2024-05-20 02:39:31.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     2352 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0    12392 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.3/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.100818 nuitka_winsvc-2.2.3/nuitka/reports/
+-rw-rw-rw-   0        0        0     2286 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/reports/CompilationReportReader.py
+-rw-rw-rw-   0        0        0     2089 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/reports/LicenseReport.rst.j2
+-rw-rw-rw-   0        0        0    28897 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/reports/Reports.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.106820 nuitka_winsvc-2.2.3/nuitka/specs/
+-rw-rw-rw-   0        0        0     5943 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-rw-rw-   0        0        0     2818 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-rw-rw-   0        0        0     2573 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-rw-rw-   0        0        0    27022 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/specs/BuiltinParameterSpecs.py
+-rw-rw-rw-   0        0        0     6098 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-rw-rw-   0        0        0     1190 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-rw-rw-   0        0        0     4834 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-rw-rw-   0        0        0     7112 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/specs/HardImportSpecs.py
+-rw-rw-rw-   0        0        0    18811 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/specs/ParameterSpecs.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/specs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.107818 nuitka_winsvc-2.2.3/nuitka/tools/
+-rw-rw-rw-   0        0        0     1631 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/Basics.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.108818 nuitka_winsvc-2.2.3/nuitka/tools/commercial/
+-rw-rw-rw-   0        0        0      847 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/commercial/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.109818 nuitka_winsvc-2.2.3/nuitka/tools/data_composer/
+-rw-rw-rw-   0        0        0    15004 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/data_composer/DataComposer.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/data_composer/__init__.py
+-rw-rw-rw-   0        0        0     1338 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/data_composer/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.111818 nuitka_winsvc-2.2.3/nuitka/tools/environments/
+-rw-rw-rw-   0        0        0     2481 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/environments/CreateEnvironment.py
+-rw-rw-rw-   0        0        0     4198 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/environments/Virtualenv.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/environments/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.112824 nuitka_winsvc-2.2.3/nuitka/tools/general/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/general/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.113819 nuitka_winsvc-2.2.3/nuitka/tools/general/dll_report/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/general/dll_report/__init__.py
+-rw-rw-rw-   0        0        0     2352 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/general/dll_report/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.114818 nuitka_winsvc-2.2.3/nuitka/tools/general/find_module/
+-rw-rw-rw-   0        0        0     3953 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/general/find_module/FindModuleCode.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/general/find_module/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.115818 nuitka_winsvc-2.2.3/nuitka/tools/onefile_compressor/
+-rw-rw-rw-   0        0        0    12545 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/onefile_compressor/__init__.py
+-rw-rw-rw-   0        0        0     1343 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/onefile_compressor/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.117694 nuitka_winsvc-2.2.3/nuitka/tools/podman/
+-rw-rw-rw-   0        0        0     1905 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/podman/Podman.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/podman/__init__.py
+-rw-rw-rw-   0        0        0    11623 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/podman/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.118816 nuitka_winsvc-2.2.3/nuitka/tools/profiler/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/profiler/__init__.py
+-rw-rw-rw-   0        0        0     2561 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/profiler/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.120507 nuitka_winsvc-2.2.3/nuitka/tools/scanning/
+-rw-rw-rw-   0        0        0     3590 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-rw-rw-   0        0        0     2314 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/scanning/DisplayPackageData.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/scanning/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.123381 nuitka_winsvc-2.2.3/nuitka/tools/specialize/
+-rw-rw-rw-   0        0        0    51703 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-rw-rw-   0        0        0     7717 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/specialize/Common.py
+-rw-rw-rw-   0        0        0    39747 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/specialize/SpecializeC.py
+-rw-rw-rw-   0        0        0    36683 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/specialize/SpecializePython.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/specialize/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.128064 nuitka_winsvc-2.2.3/nuitka/tools/testing/
+-rw-rw-rw-   0        0        0    56174 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/Common.py
+-rw-rw-rw-   0        0        0     1516 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/Constructs.py
+-rw-rw-rw-   0        0        0    10129 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/OutputComparison.py
+-rw-rw-rw-   0        0        0     1310 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/Pythons.py
+-rw-rw-rw-   0        0        0     8061 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/RuntimeTracing.py
+-rw-rw-rw-   0        0        0     5413 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/SearchModes.py
+-rw-rw-rw-   0        0        0     3408 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/Valgrind.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.129153 nuitka_winsvc-2.2.3/nuitka/tools/testing/check_reference_counts/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-rw-rw-   0        0        0     3095 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/check_reference_counts/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.130734 nuitka_winsvc-2.2.3/nuitka/tools/testing/compare_with_cpython/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-rw-rw-   0        0        0    29697 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/compare_with_cpython/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.131824 nuitka_winsvc-2.2.3/nuitka/tools/testing/find_sxs_modules/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/find_sxs_modules/__init__.py
+-rw-rw-rw-   0        0        0     1980 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/find_sxs_modules/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.132365 nuitka_winsvc-2.2.3/nuitka/tools/testing/measure_construct_performance/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-rw-rw-   0        0        0     8758 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/measure_construct_performance/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.133470 nuitka_winsvc-2.2.3/nuitka/tools/testing/run_nuitka_tests/
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/run_nuitka_tests/__init__.py
+-rw-rw-rw-   0        0        0    35342 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/testing/run_nuitka_tests/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.135030 nuitka_winsvc-2.2.3/nuitka/tools/watch/
+-rw-rw-rw-   0        0        0     3543 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/watch/GitHub.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tools/watch/__init__.py
+-rw-rw-rw-   0        0        0    21532 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tools/watch/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.152368 nuitka_winsvc-2.2.3/nuitka/tree/
+-rw-rw-rw-   0        0        0    50436 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/Building.py
+-rw-rw-rw-   0        0        0    75150 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-rw-rw-   0        0        0     1733 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/Extractions.py
+-rw-rw-rw-   0        0        0     2603 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/InternalModule.py
+-rw-rw-rw-   0        0        0     1544 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/Operations.py
+-rw-rw-rw-   0        0        0     2841 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationAssertStatements.py
+-rw-rw-rw-   0        0        0    43887 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-rw-rw-   0        0        0     2981 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-rw-rw-   0        0        0    11746 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationCallExpressions.py
+-rw-rw-rw-   0        0        0    15446 2024-03-20 02:57:24.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationClasses.py
+-rw-rw-rw-   0        0        0    38202 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationClasses3.py
+-rw-rw-rw-   0        0        0     6523 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-rw-rw-   0        0        0    22207 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationContractionExpressions.py
+-rw-rw-rw-   0        0        0    11266 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-rw-rw-   0        0        0    14805 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationExecStatements.py
+-rw-rw-rw-   0        0        0     7858 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationForLoopStatements.py
+-rw-rw-rw-   0        0        0    30885 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationFunctionStatements.py
+-rw-rw-rw-   0        0        0    14095 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationImportStatements.py
+-rw-rw-rw-   0        0        0     6630 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-rw-rw-   0        0        0    21311 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationMatchStatements.py
+-rw-rw-rw-   0        0        0     2442 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationMultidist.py
+-rw-rw-rw-   0        0        0     7608 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationNamespacePackages.py
+-rw-rw-rw-   0        0        0     4711 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationPrintStatements.py
+-rw-rw-rw-   0        0        0    15606 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationSequenceCreation.py
+-rw-rw-rw-   0        0        0     4857 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-rw-rw-   0        0        0    14948 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-rw-rw-   0        0        0     7014 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-rw-rw-   0        0        0     5707 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-rw-rw-   0        0        0    14439 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationWithStatements.py
+-rw-rw-rw-   0        0        0     3852 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/ReformulationYieldExpressions.py
+-rw-rw-rw-   0        0        0    13488 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/SourceHandling.py
+-rw-rw-rw-   0        0        0     3790 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/SyntaxErrors.py
+-rw-rw-rw-   0        0        0    23153 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/tree/TreeHelpers.py
+-rw-rw-rw-   0        0        0    20465 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/VariableClosure.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.169644 nuitka_winsvc-2.2.3/nuitka/utils/
+-rw-rw-rw-   0        0        0     3140 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/AppDirs.py
+-rw-rw-rw-   0        0        0     4128 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/CStrings.py
+-rw-rw-rw-   0        0        0     6394 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/CommandLineOptions.py
+-rw-rw-rw-   0        0        0    14983 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/Distributions.py
+-rw-rw-rw-   0        0        0     6477 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/Download.py
+-rw-rw-rw-   0        0        0    13368 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/Execution.py
+-rw-rw-rw-   0        0        0    42167 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/FileOperations.py
+-rw-rw-rw-   0        0        0     3753 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/Hashing.py
+-rw-rw-rw-   0        0        0     2391 2024-05-20 02:39:32.000000 nuitka_winsvc-2.2.3/nuitka/utils/Images.py
+-rw-rw-rw-   0        0        0    10334 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/Importing.py
+-rw-rw-rw-   0        0        0     7884 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/InstalledPythons.py
+-rw-rw-rw-   0        0        0     2258 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/InstanceCounters.py
+-rw-rw-rw-   0        0        0     4586 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/Jinja2.py
+-rw-rw-rw-   0        0        0     1271 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/Json.py
+-rw-rw-rw-   0        0        0     4478 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/MacOSApp.py
+-rw-rw-rw-   0        0        0     5092 2024-03-25 02:50:30.000000 nuitka_winsvc-2.2.3/nuitka/utils/MemoryUsage.py
+-rw-rw-rw-   0        0        0     9951 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/ModuleNames.py
+-rw-rw-rw-   0        0        0     4588 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/ReExecute.py
+-rw-rw-rw-   0        0        0     1889 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/Rest.py
+-rw-rw-rw-   0        0        0    23857 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/SharedLibraries.py
+-rw-rw-rw-   0        0        0     3698 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/Shebang.py
+-rw-rw-rw-   0        0        0     3687 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/Signing.py
+-rw-rw-rw-   0        0        0     2084 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/SlotMetaClasses.py
+-rw-rw-rw-   0        0        0     6603 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/StaticLibraries.py
+-rw-rw-rw-   0        0        0     2634 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/ThreadedExecutor.py
+-rw-rw-rw-   0        0        0     2798 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/Timing.py
+-rw-rw-rw-   0        0        0    12705 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/Utils.py
+-rw-rw-rw-   0        0        0    10642 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/nuitka/utils/WindowsFileUsage.py
+-rw-rw-rw-   0        0        0    19837 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/WindowsResources.py
+-rw-rw-rw-   0        0        0     7014 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/Yaml.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/nuitka/utils/__init__.py
+-rw-rw-rw-   0        0        0      865 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 02:47:27.279295 nuitka_winsvc-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0    16351 2024-05-20 02:40:51.000000 nuitka_winsvc-2.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.170161 nuitka_winsvc-2.2.3/tests/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.724895 nuitka_winsvc-2.2.3/tests/basics/
+-rw-rw-rw-   0        0        0     1798 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/AssertsTest.py
+-rw-rw-rw-   0        0        0     5966 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/AssignmentsTest.py
+-rw-rw-rw-   0        0        0     5910 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/AssignmentsTest32.py
+-rw-rw-rw-   0        0        0     4086 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/BranchingTest.py
+-rw-rw-rw-   0        0        0     1136 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/BuiltinOverload.py
+-rw-rw-rw-   0        0        0     3781 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/BuiltinSuperTest.py
+-rw-rw-rw-   0        0        0    17112 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/BuiltinsTest.py
+-rw-rw-rw-   0        0        0      898 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ClassMinimalTest.py
+-rw-rw-rw-   0        0        0     4796 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ClassesTest.py
+-rw-rw-rw-   0        0        0     3446 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ClassesTest32.py
+-rw-rw-rw-   0        0        0     1438 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ClassesTest34.py
+-rw-rw-rw-   0        0        0     4729 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ComparisonChainsTest.py
+-rw-rw-rw-   0        0        0     4672 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ConstantsTest.py
+-rw-rw-rw-   0        0        0     1027 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ConstantsTest27.py
+-rw-rw-rw-   0        0        0     1661 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/DecoratorsTest.py
+-rw-rw-rw-   0        0        0     2349 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/DefaultParametersTest.py
+-rw-rw-rw-   0        0        0     1159 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/DoubleDeletionsTest.py
+-rw-rw-rw-   0        0        0      838 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/EmptyModuleTest.py
+-rw-rw-rw-   0        0        0    14418 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ExceptionRaisingTest.py
+-rw-rw-rw-   0        0        0      993 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ExceptionRaisingTest32.py
+-rw-rw-rw-   0        0        0     1490 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ExceptionRaisingTest33.py
+-rw-rw-rw-   0        0        0     6779 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ExecEvalTest.py
+-rw-rw-rw-   0        0        0     1450 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/basics/ExtremeClosureTest.py
+-rw-rw-rw-   0        0        0     1689 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/basics/FunctionObjectsTest.py
+-rw-rw-rw-   0        0        0    12367 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/FunctionsTest.py
+-rw-rw-rw-   0        0        0     3635 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/FunctionsTest32.py
+-rw-rw-rw-   0        0        0     2658 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/basics/FunctionsTest_2.py
+-rw-rw-rw-   0        0        0      922 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/FutureTest32.py
+-rw-rw-rw-   0        0        0     5841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/GeneratorExpressionsTest.py
+-rw-rw-rw-   0        0        0     1073 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/GeneratorExpressionsTest_37.py
+-rw-rw-rw-   0        0        0     3856 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/GlobalStatementTest.py
+-rw-rw-rw-   0        0        0     1318 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/HelloWorldTest_2.py
+-rw-rw-rw-   0        0        0     2501 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ImportingTest.py
+-rw-rw-rw-   0        0        0     1328 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/InplaceOperationsTest.py
+-rw-rw-rw-   0        0        0     4259 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/InspectionTest.py
+-rw-rw-rw-   0        0        0     1536 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/InspectionTest_35.py
+-rw-rw-rw-   0        0        0     1650 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/InspectionTest_36.py
+-rw-rw-rw-   0        0        0     1703 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/LambdasTest.py
+-rw-rw-rw-   0        0        0     2763 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/LateClosureAssignmentTest.py
+-rw-rw-rw-   0        0        0     2955 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ListContractionsTest.py
+-rw-rw-rw-   0        0        0     3361 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/LoopingTest.py
+-rw-rw-rw-   0        0        0     1568 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/MainProgramsTest.py
+-rw-rw-rw-   0        0        0     1957 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ModuleAttributesTest.py
+-rw-rw-rw-   0        0        0     2008 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/OperatorsTest.py
+-rw-rw-rw-   0        0        0    14935 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/OrderChecksTest.py
+-rw-rw-rw-   0        0        0     1859 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/OrderChecksTest27.py
+-rw-rw-rw-   0        0        0     1484 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/OverflowFunctionsTest_2.py
+-rw-rw-rw-   0        0        0     5885 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ParameterErrorsTest.py
+-rw-rw-rw-   0        0        0     1931 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ParameterErrorsTest32.py
+-rw-rw-rw-   0        0        0      895 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/PrintFutureTest.py
+-rw-rw-rw-   0        0        0     1444 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/PrintingTest_2.py
+-rw-rw-rw-   0        0        0      910 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/RecursionTest.py
+-rw-rw-rw-   0        0        0    24798 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/basics/ReferencingTest.py
+-rw-rw-rw-   0        0        0     2109 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ReferencingTest27.py
+-rw-rw-rw-   0        0        0     7869 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/basics/ReferencingTest33.py
+-rw-rw-rw-   0        0        0     5060 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/basics/ReferencingTest35.py
+-rw-rw-rw-   0        0        0     5497 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/basics/ReferencingTest36.py
+-rw-rw-rw-   0        0        0     2932 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ReferencingTest_2.py
+-rw-rw-rw-   0        0        0     1662 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/SlotsTest.py
+-rw-rw-rw-   0        0        0     1191 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/ThreadedGeneratorsTest.py
+-rw-rw-rw-   0        0        0    22998 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/TrickAssignmentsTest32.py
+-rw-rw-rw-   0        0        0     1573 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/TrickAssignmentsTest35.py
+-rw-rw-rw-   0        0        0     1820 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/TrickAssignmentsTest_2.py
+-rw-rw-rw-   0        0        0     2118 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/TryContinueFinallyTest.py
+-rw-rw-rw-   0        0        0     2244 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/TryExceptContinueTest.py
+-rw-rw-rw-   0        0        0     2307 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/TryExceptFinallyTest.py
+-rw-rw-rw-   0        0        0     2336 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/TryExceptFramesTest.py
+-rw-rw-rw-   0        0        0     2874 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/TryReturnFinallyTest.py
+-rw-rw-rw-   0        0        0     2360 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/TryYieldFinallyTest.py
+-rw-rw-rw-   0        0        0     1125 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/UnicodeTest.py
+-rw-rw-rw-   0        0        0     1909 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/UnpackingTest35.py
+-rw-rw-rw-   0        0        0     2143 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/VarargsTest.py
+-rw-rw-rw-   0        0        0     4913 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/WithStatementsTest.py
+-rw-rw-rw-   0        0        0     3103 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/YieldFromTest33.py
+-rw-rw-rw-   0        0        0     3851 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/run_all.py
+-rw-rw-rw-   0        0        0     2302 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/basics/run_xml.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.748901 nuitka_winsvc-2.2.3/tests/onefile/
+-rw-rw-rw-   0        0        0     1341 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/onefile/HelloWorldTest.py
+-rw-rw-rw-   0        0        0     1339 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/onefile/KeyboardInterruptTest.py
+-rw-rw-rw-   0        0        0     5846 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/onefile/run_all.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.856510 nuitka_winsvc-2.2.3/tests/optimizations/
+-rw-rw-rw-   0        0        0      991 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/optimizations/ArgumentTypes.py
+-rw-rw-rw-   0        0        0     1087 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/AttributesTest.py
+-rw-rw-rw-   0        0        0     1053 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/CallsTest.py
+-rw-rw-rw-   0        0        0      953 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/ConditionsTest.py
+-rw-rw-rw-   0        0        0      941 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/DecodingOperationsTest.py
+-rw-rw-rw-   0        0        0     1246 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/FormatStringsTest36.py
+-rw-rw-rw-   0        0        0     1183 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/HardImportsTest.py
+-rw-rw-rw-   0        0        0     1007 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/HardImportsTest_2.py
+-rw-rw-rw-   0        0        0      950 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/optimizations/Iterations.py
+-rw-rw-rw-   0        0        0     1292 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/LenTest.py
+-rw-rw-rw-   0        0        0     1133 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/MatchingTest310.py
+-rw-rw-rw-   0        0        0     2295 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/OperationsTest.py
+-rw-rw-rw-   0        0        0     1365 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/optimizations/SubscriptsTest.py
+-rw-rw-rw-   0        0        0     8827 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/optimizations/run_all.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.867526 nuitka_winsvc-2.2.3/tests/packages/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.882511 nuitka_winsvc-2.2.3/tests/packages/package_data_files_embedding/
+-rw-rw-rw-   0        0        0     1576 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py
+-rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/package_data_files_embedding/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.890511 nuitka_winsvc-2.2.3/tests/packages/package_import_success_after_failure/
+-rw-rw-rw-   0        0        0     2414 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.907511 nuitka_winsvc-2.2.3/tests/packages/package_import_success_after_failure/variable_package/
+-rw-rw-rw-   0        0        0      975 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+-rw-rw-rw-   0        0        0     1201 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rw-rw-rw-   0        0        0     4138 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/run_all.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.137870 nuitka_winsvc-2.2.3/tests/packages/sub_package/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.932513 nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/
+-rw-rw-rw-   0        0        0     1262 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/__init__.py
+-rw-rw-rw-   0        0        0      940 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/bigkitty.py
+-rw-rw-rw-   0        0        0      942 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/smallkitty.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.966067 nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/speak/
+-rw-rw-rw-   0        0        0      961 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-rw-rw-   0        0        0     1085 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/speak/hello.py
+-rw-rw-rw-   0        0        0      999 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/speak/miau.py
+-rw-rw-rw-   0        0        0     1001 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/speak/purr.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.138870 nuitka_winsvc-2.2.3/tests/packages/top_level_attributes_3/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.983257 nuitka_winsvc-2.2.3/tests/packages/top_level_attributes_3/some_package/
+-rw-rw-rw-   0        0        0     2368 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-rw-rw-   0        0        0      939 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:25.991171 nuitka_winsvc-2.2.3/tests/plugins/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.001959 nuitka_winsvc-2.2.3/tests/plugins/code_signing/
+-rw-rw-rw-   0        0        0     1202 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/plugins/code_signing/CodeSigningMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.021062 nuitka_winsvc-2.2.3/tests/plugins/data_files/
+-rw-rw-rw-   0        0        0     1474 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/plugins/data_files/DataFilesMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.030046 nuitka_winsvc-2.2.3/tests/plugins/data_files/data_files_package/
+-rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/plugins/data_files/data_files_package/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/tests/plugins/data_files/data_files_package/lala.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.031067 nuitka_winsvc-2.2.3/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-rw-rw-   0        0        0        0 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-rw-rw-   0        0        0      309 2024-01-29 03:39:42.000000 nuitka_winsvc-2.2.3/tests/plugins/data_files/test_case.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.033640 nuitka_winsvc-2.2.3/tests/plugins/parameters/
+-rw-rw-rw-   0        0        0     1162 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/plugins/parameters/ParametersMain.py
+-rw-rw-rw-   0        0        0     2218 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/plugins/parameters/parameter-using-plugin.py
+-rw-rw-rw-   0        0        0     3778 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/plugins/run_all.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.037621 nuitka_winsvc-2.2.3/tests/programs/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.046621 nuitka_winsvc-2.2.3/tests/programs/absolute_import/
+-rw-rw-rw-   0        0        0      899 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.086633 nuitka_winsvc-2.2.3/tests/programs/absolute_import/foobar/
+-rw-rw-rw-   0        0        0      828 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/absolute_import/foobar/__init__.py
+-rw-rw-rw-   0        0        0     1076 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/absolute_import/foobar/foobar.py
+-rw-rw-rw-   0        0        0      911 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/absolute_import/foobar/local.py
+-rw-rw-rw-   0        0        0      893 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/absolute_import/foobar/util.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.093622 nuitka_winsvc-2.2.3/tests/programs/case_imports1/
+-rw-rw-rw-   0        0        0      840 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports1/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.098622 nuitka_winsvc-2.2.3/tests/programs/case_imports1/path1/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports1/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.106622 nuitka_winsvc-2.2.3/tests/programs/case_imports1/path1/Some_Package/
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports1/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.140624 nuitka_winsvc-2.2.3/tests/programs/case_imports1/path2/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports1/path2/some_module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.146632 nuitka_winsvc-2.2.3/tests/programs/case_imports1/path2/some_package/
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports1/path2/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.151631 nuitka_winsvc-2.2.3/tests/programs/case_imports2/
+-rw-rw-rw-   0        0        0      840 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports2/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.159342 nuitka_winsvc-2.2.3/tests/programs/case_imports2/path1/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports2/path1/some_module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.165338 nuitka_winsvc-2.2.3/tests/programs/case_imports2/path1/some_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.168328 nuitka_winsvc-2.2.3/tests/programs/case_imports2/path2/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports2/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.177328 nuitka_winsvc-2.2.3/tests/programs/case_imports2/path2/Some_Package/
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports2/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.188329 nuitka_winsvc-2.2.3/tests/programs/case_imports3/
+-rw-rw-rw-   0        0        0     1107 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports3/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.189329 nuitka_winsvc-2.2.3/tests/programs/case_imports3/path1/
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports3/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.199329 nuitka_winsvc-2.2.3/tests/programs/case_imports3/path1/Some_Package/
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports3/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.202329 nuitka_winsvc-2.2.3/tests/programs/case_imports3/path2/
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports3/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.210330 nuitka_winsvc-2.2.3/tests/programs/case_imports3/path2/Some_Package/
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/case_imports3/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.216330 nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.222330 nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+-rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.244331 nuitka_winsvc-2.2.3/tests/programs/dash_import/
+-rw-rw-rw-   0        0        0      920 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/dash_import/DashImportMain.py
+-rw-rw-rw-   0        0        0      849 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/dash_import/dash-module.py
+-rw-rw-rw-   0        0        0      849 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/dash_import/plus+module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.251333 nuitka_winsvc-2.2.3/tests/programs/dash_main/
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/dash_main/Dash-Main.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.283332 nuitka_winsvc-2.2.3/tests/programs/deep/
+-rw-rw-rw-   0        0        0      930 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/deep/DeepProgramMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.303335 nuitka_winsvc-2.2.3/tests/programs/deep/some_package/
+-rw-rw-rw-   0        0        0     1012 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/deep/some_package/DeepBrother.py
+-rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/deep/some_package/DeepChild.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/deep/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.364571 nuitka_winsvc-2.2.3/tests/programs/deep/some_package/deep_package/
+-rw-rw-rw-   0        0        0      908 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+-rw-rw-rw-   0        0        0      984 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/deep/some_package/deep_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.367574 nuitka_winsvc-2.2.3/tests/programs/dunderinit_imports/
+-rw-rw-rw-   0        0        0      826 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.381572 nuitka_winsvc-2.2.3/tests/programs/dunderinit_imports/package/
+-rw-rw-rw-   0        0        0      829 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-rw-rw-   0        0        0      889 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/dunderinit_imports/package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.390585 nuitka_winsvc-2.2.3/tests/programs/import_variants/
+-rw-rw-rw-   0        0        0     1037 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/import_variants/ImportVariationsMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.408583 nuitka_winsvc-2.2.3/tests/programs/import_variants/some_package/
+-rw-rw-rw-   0        0        0      978 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/import_variants/some_package/Child1.py
+-rw-rw-rw-   0        0        0     1130 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/import_variants/some_package/Child2.py
+-rw-rw-rw-   0        0        0      854 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/import_variants/some_package/Child3.py
+-rw-rw-rw-   0        0        0     1026 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/import_variants/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.415577 nuitka_winsvc-2.2.3/tests/programs/main_raises/
+-rw-rw-rw-   0        0        0      943 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/main_raises/ErrorMain.py
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/main_raises/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.431573 nuitka_winsvc-2.2.3/tests/programs/main_raises2/
+-rw-rw-rw-   0        0        0     1112 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/main_raises2/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.443573 nuitka_winsvc-2.2.3/tests/programs/module_attributes/
+-rw-rw-rw-   0        0        0     1561 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.463574 nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/
+-rw-rw-rw-   0        0        0     1800 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/Nearby1.py
+-rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.484575 nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/
+-rw-rw-rw-   0        0        0     1800 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.504576 nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-rw-rw-   0        0        0     1800 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-rw-rw-   0        0        0     1643 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.520428 nuitka_winsvc-2.2.3/tests/programs/module_exits/
+-rw-rw-rw-   0        0        0      901 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/module_exits/ErrorExitingModule.py
+-rw-rw-rw-   0        0        0      899 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/module_exits/Main.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.538435 nuitka_winsvc-2.2.3/tests/programs/module_object_replacing/
+-rw-rw-rw-   0        0        0     1110 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-rw-rw-   0        0        0     1391 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.548443 nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/
+-rw-rw-rw-   0        0        0     1022 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.580434 nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/foo/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-rw-rw-   0        0        0      868 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-rw-rw-   0        0        0     1791 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/foo/entry.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.584435 nuitka_winsvc-2.2.3/tests/programs/named_imports/
+-rw-rw-rw-   0        0        0      878 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/named_imports/NamedImportsMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.595436 nuitka_winsvc-2.2.3/tests/programs/named_imports/some_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/named_imports/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      856 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/named_imports/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.600436 nuitka_winsvc-2.2.3/tests/programs/named_imports/some_package/sub_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.608448 nuitka_winsvc-2.2.3/tests/programs/package_code/
+-rw-rw-rw-   0        0        0      832 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_code/PackageInitCodeMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.620436 nuitka_winsvc-2.2.3/tests/programs/package_code/some_package/
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_code/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_code/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.631438 nuitka_winsvc-2.2.3/tests/programs/package_contains_main/
+-rw-rw-rw-   0        0        0      821 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_contains_main/PackageContainsMain.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_contains_main/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_contains_main/local.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.637436 nuitka_winsvc-2.2.3/tests/programs/package_init_import/
+-rw-rw-rw-   0        0        0      855 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_init_import/PackageInitImportMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.652438 nuitka_winsvc-2.2.3/tests/programs/package_init_import/some_package/
+-rw-rw-rw-   0        0        0     1064 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/programs/package_init_import/some_package/PackageLocal.py
+-rw-rw-rw-   0        0        0     1225 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/programs/package_init_import/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.660437 nuitka_winsvc-2.2.3/tests/programs/package_init_issue/
+-rw-rw-rw-   0        0        0      821 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.669594 nuitka_winsvc-2.2.3/tests/programs/package_init_issue/some_package/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_init_issue/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.681602 nuitka_winsvc-2.2.3/tests/programs/package_init_issue/some_package/child_package/
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-rw-rw-   0        0        0      827 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_init_issue/some_package/child_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.688595 nuitka_winsvc-2.2.3/tests/programs/package_missing_init/
+-rw-rw-rw-   0        0        0      958 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.698597 nuitka_winsvc-2.2.3/tests/programs/package_missing_init/some_package/
+-rw-rw-rw-   0        0        0      997 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_missing_init/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.703596 nuitka_winsvc-2.2.3/tests/programs/package_missing_init/some_package/sub_package/
+-rw-rw-rw-   0        0        0     1009 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.723624 nuitka_winsvc-2.2.3/tests/programs/package_module_collision/
+-rw-rw-rw-   0        0        0      933 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.728641 nuitka_winsvc-2.2.3/tests/programs/package_module_collision/Something/
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_module_collision/Something/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_module_collision/something.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.730625 nuitka_winsvc-2.2.3/tests/programs/package_overload/
+-rw-rw-rw-   0        0        0      884 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_overload/Main.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.755625 nuitka_winsvc-2.2.3/tests/programs/package_overload/foo/
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_overload/foo/__init__.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_overload/foo/bar.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_overload/foo/bar2.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.763626 nuitka_winsvc-2.2.3/tests/programs/package_prevents_submodule/
+-rw-rw-rw-   0        0        0     3079 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.775106 nuitka_winsvc-2.2.3/tests/programs/package_prevents_submodule/some_package/
+-rw-rw-rw-   0        0        0     1111 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:21.181051 nuitka_winsvc-2.2.3/tests/programs/package_program/
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.783746 nuitka_winsvc-2.2.3/tests/programs/package_program/PackageAsMain/
+-rw-rw-rw-   0        0        0      920 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/package_program/PackageAsMain/__init__.py
+-rw-rw-rw-   0        0        0     1661 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/programs/package_program/PackageAsMain/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.794759 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/
+-rw-rw-rw-   0        0        0     1760 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.802746 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.821756 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.843364 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.853364 nuitka_winsvc-2.2.3/tests/programs/pkgutil_usage/
+-rw-rw-rw-   0        0        0     1328 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.868365 nuitka_winsvc-2.2.3/tests/programs/pkgutil_usage/package/
+-rw-rw-rw-   0        0        0       13 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0       14 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+-rw-rw-rw-   0        0        0       14 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-rw-rw-   0        0        0     1585 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/pkgutil_usage/package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.878366 nuitka_winsvc-2.2.3/tests/programs/plugin_import/
+-rw-rw-rw-   0        0        0      891 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/plugin_import/PluginImportMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.891367 nuitka_winsvc-2.2.3/tests/programs/plugin_import/some_package/
+-rw-rw-rw-   0        0        0      803 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/plugin_import/some_package/__init__.py
+-rw-rw-rw-   0        0        0      813 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/plugin_import/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.896921 nuitka_winsvc-2.2.3/tests/programs/reimport_main_dynamic/
+-rw-rw-rw-   0        0        0      943 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.901915 nuitka_winsvc-2.2.3/tests/programs/reimport_main_static/
+-rw-rw-rw-   0        0        0      930 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.909913 nuitka_winsvc-2.2.3/tests/programs/relative_import/
+-rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/relative_import/RelativeImportMain.py
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/relative_import/dircache.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.914915 nuitka_winsvc-2.2.3/tests/programs/resource_reader37/
+-rw-rw-rw-   0        0        0     1202 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.925914 nuitka_winsvc-2.2.3/tests/programs/resource_reader37/some_package/
+-rw-rw-rw-   0        0        0       13 2023-09-05 03:06:57.000000 nuitka_winsvc-2.2.3/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/resource_reader37/some_package/__init__.py
+-rw-rw-rw-   0        0        0     6614 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/programs/run_all.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.946915 nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/
+-rw-rw-rw-   0        0        0     1203 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-rw-rw-   0        0        0      831 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/pyexpat.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.963916 nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/some_package/
+-rw-rw-rw-   0        0        0      767 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-rw-rw-   0        0        0      941 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rw-rw-rw-   0        0        0      842 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-rw-rw-   0        0        0     1268 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/some_package/star_importing.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.976918 nuitka_winsvc-2.2.3/tests/programs/syntax_errors/
+-rw-rw-rw-   0        0        0      822 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/syntax_errors/IndentationErroring.py
+-rw-rw-rw-   0        0        0      833 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-rw-rw-   0        0        0     1111 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/syntax_errors/SyntaxErrorsMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.985968 nuitka_winsvc-2.2.3/tests/programs/unicode_bom/
+-rw-rw-rw-   0        0        0      995 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-rw-rw-   0        0        0      878 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/unicode_bom/unicode_bom.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.986968 nuitka_winsvc-2.2.3/tests/programs/with space/
+-rw-rw-rw-   0        0        0      858 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/programs/with space/Space Main.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:26.992977 nuitka_winsvc-2.2.3/tests/reflected/
+-rw-rw-rw-   0        0        0    14254 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/reflected/compile_itself.py
+-rw-rw-rw-   0        0        0     1274 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/run-tests
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:27.110652 nuitka_winsvc-2.2.3/tests/standalone/
+-rw-rw-rw-   0        0        0     1090 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/BrotliUsing.py
+-rw-rw-rw-   0        0        0     2586 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/CtypesUsing.py
+-rw-rw-rw-   0        0        0     1950 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/DateutilsUsing.py
+-rw-rw-rw-   0        0        0     1168 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/FlaskUsing.py
+-rw-rw-rw-   0        0        0     1307 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/standalone/GiUsing.py
+-rw-rw-rw-   0        0        0     1022 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/GlfwUsing.py
+-rw-rw-rw-   0        0        0     1216 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/GtkUsing.py
+-rw-rw-rw-   0        0        0     1057 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/HexEncodingTest_2.py
+-rw-rw-rw-   0        0        0     1118 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/IdnaUsing.py
+-rw-rw-rw-   0        0        0     1215 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/LxmlUsing.py
+-rw-rw-rw-   0        0        0     1598 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/MatplotlibUsing.py
+-rw-rw-rw-   0        0        0     2570 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/MetadataPackagesUsing.py
+-rw-rw-rw-   0        0        0     1759 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/NumpyUsing.py
+-rw-rw-rw-   0        0        0      979 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/OpenGLUsing.py
+-rw-rw-rw-   0        0        0     1479 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PandasUsing.py
+-rw-rw-rw-   0        0        0     1098 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PasslibUsing.py
+-rw-rw-rw-   0        0        0     1248 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PendulumUsing.py
+-rw-rw-rw-   0        0        0     2106 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-rw-rw-   0        0        0     1099 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PmwUsing.py
+-rw-rw-rw-   0        0        0     1369 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PyQt5Plugins.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PyQt5SSLSupport.py
+-rw-rw-rw-   0        0        0     2198 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PyQt5Using.py
+-rw-rw-rw-   0        0        0     1203 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PyQt6Plugins.py
+-rw-rw-rw-   0        0        0     2168 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PyQt6Using.py
+-rw-rw-rw-   0        0        0     1789 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PySide2Using.py
+-rw-rw-rw-   0        0        0     1123 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PySide6Plugins.py
+-rw-rw-rw-   0        0        0     1789 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/PySide6Using.py
+-rw-rw-rw-   0        0        0     1371 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/RsaUsing.py
+-rw-rw-rw-   0        0        0     1227 2024-05-06 03:08:54.000000 nuitka_winsvc-2.2.3/tests/standalone/SetuptoolsUsing_311.py
+-rw-rw-rw-   0        0        0     1005 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/ShlibUsing.py
+-rw-rw-rw-   0        0        0     1569 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/SocketUsing.py
+-rw-rw-rw-   0        0        0     1973 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/TkInterUsing.py
+-rw-rw-rw-   0        0        0     3260 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/Urllib3Using.py
+-rw-rw-rw-   0        0        0     1232 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/Win32ComUsing.py
+-rw-rw-rw-   0        0        0     9912 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/run_all.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:27.118652 nuitka_winsvc-2.2.3/tests/standalone/zip_importer/
+-rw-rw-rw-   0        0        0     1296 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/standalone/zip_importer/ZipImporterMain.py
+drwxrwxrwx   0        0        0        0 2024-05-20 02:47:27.269799 nuitka_winsvc-2.2.3/tests/syntax/
+-rw-rw-rw-   0        0        0      844 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/AsyncgenReturn36.py
+-rw-rw-rw-   0        0        0      818 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/AwaitInModule36.py
+-rw-rw-rw-   0        0        0      901 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/BreakWithoutLoop.py
+-rw-rw-rw-   0        0        0      824 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/ClassReturn.py
+-rw-rw-rw-   0        0        0     1002 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/ClosureDel_2.py
+-rw-rw-rw-   0        0        0      882 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/ContinueWithoutLoop.py
+-rw-rw-rw-   0        0        0      824 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/DuplicateArgument.py
+-rw-rw-rw-   0        0        0     1142 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/ExecWithNesting_2.py
+-rw-rw-rw-   0        0        0      858 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/FutureBraces.py
+-rw-rw-rw-   0        0        0      837 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/FutureUnknown.py
+-rw-rw-rw-   0        0        0     1073 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/GeneratorExpressions38.py
+-rw-rw-rw-   0        0        0      911 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/GeneratorReturn_2.py
+-rw-rw-rw-   0        0        0      825 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/GlobalForParameter.py
+-rw-rw-rw-   0        0        0     1027 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/Importing32.py
+-rw-rw-rw-   0        0        0      830 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/IndentationError.py
+-rw-rw-rw-   0        0        0      947 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/LateFutureImport.py
+-rw-rw-rw-   0        0        0      874 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/MisplacedFutureImport.py
+-rw-rw-rw-   0        0        0      832 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/ModuleReturn.py
+-rw-rw-rw-   0        0        0      915 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-rw-rw-   0        0        0      827 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/NonlocalForParameter32.py
+-rw-rw-rw-   0        0        0      900 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/NonlocalNotFound32.py
+-rw-rw-rw-   0        0        0      939 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/StarImportExtra.py
+-rw-rw-rw-   0        0        0      900 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/SyntaxError.py
+-rw-rw-rw-   0        0        0      907 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/TryExceptAllNotLast.py
+-rw-rw-rw-   0        0        0      908 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/TryFinallyContinue_37.py
+-rw-rw-rw-   0        0        0      808 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/UnpackNoTuple.py
+-rw-rw-rw-   0        0        0      841 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/UnpackTwoStars32.py
+-rw-rw-rw-   0        0        0      825 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/YieldFromInModule.py
+-rw-rw-rw-   0        0        0      837 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/YieldInAsync35.py
+-rw-rw-rw-   0        0        0      956 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/YieldInGenexp38.py
+-rw-rw-rw-   0        0        0      813 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/YieldInModule.py
+-rw-rw-rw-   0        0        0     2234 2024-03-06 05:39:36.000000 nuitka_winsvc-2.2.3/tests/syntax/run_all.py
```

### Comparing `nuitka_winsvc-2.2.2/Developer_Manual.rst` & `nuitka_winsvc-2.2.3/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/LICENSE.txt` & `nuitka_winsvc-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/MANIFEST.in` & `nuitka_winsvc-2.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/PKG-INFO` & `nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 2.2.2
+Version: 2.2.3
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `nuitka_winsvc-2.2.2/Nuitka_winsvc.egg-info/SOURCES.txt` & `nuitka_winsvc-2.2.3/Nuitka_winsvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/PKG-INFO` & `nuitka_winsvc-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 2.2.2
+Version: 2.2.3
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `nuitka_winsvc-2.2.2/README.md` & `nuitka_winsvc-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/README.rst` & `nuitka_winsvc-2.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/bin/autoformat-nuitka-source` & `nuitka_winsvc-2.2.3/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/bin/check-nuitka-with-pylint` & `nuitka_winsvc-2.2.3/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/bin/compare_with_cpython` & `nuitka_winsvc-2.2.3/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/bin/compare_with_xml` & `nuitka_winsvc-2.2.3/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/bin/measure-construct-performance` & `nuitka_winsvc-2.2.3/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/bin/nuitka` & `nuitka_winsvc-2.2.3/bin/nuitka`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/bin/nuitka-run` & `nuitka_winsvc-2.2.3/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/doc/Logo/Nuitka-Logo-Horizontal.svg` & `nuitka_winsvc-2.2.3/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/doc/Logo/Nuitka-Logo-Symbol.svg` & `nuitka_winsvc-2.2.3/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/doc/Logo/Nuitka-Logo-Vertical.svg` & `nuitka_winsvc-2.2.3/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/doc/images/Nuitka-Logo-Horizontal.png` & `nuitka_winsvc-2.2.3/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/doc/images/Nuitka-Logo-Symbol.png` & `nuitka_winsvc-2.2.3/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/doc/images/Nuitka-Logo-Vertical.png` & `nuitka_winsvc-2.2.3/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/doc/nuitka-run.1` & `nuitka_winsvc-2.2.3/doc/nuitka-run.1`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/doc/nuitka.1` & `nuitka_winsvc-2.2.3/doc/nuitka.1`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/lib/hints.py` & `nuitka_winsvc-2.2.3/lib/hints.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/misc/nuitka-run.bat` & `nuitka_winsvc-2.2.3/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/misc/nuitka.bat` & `nuitka_winsvc-2.2.3/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Builtins.py` & `nuitka_winsvc-2.2.3/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/BytecodeCaching.py` & `nuitka_winsvc-2.2.3/nuitka/BytecodeCaching.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Bytecodes.py` & `nuitka_winsvc-2.2.3/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/CacheCleanup.py` & `nuitka_winsvc-2.2.3/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Constants.py` & `nuitka_winsvc-2.2.3/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Errors.py` & `nuitka_winsvc-2.2.3/nuitka/Errors.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/HardImportRegistry.py` & `nuitka_winsvc-2.2.3/nuitka/HardImportRegistry.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/MainControl.py` & `nuitka_winsvc-2.2.3/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/ModuleRegistry.py` & `nuitka_winsvc-2.2.3/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/OptionParsing.py` & `nuitka_winsvc-2.2.3/nuitka/OptionParsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Options.py` & `nuitka_winsvc-2.2.3/nuitka/Options.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/OutputDirectories.py` & `nuitka_winsvc-2.2.3/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/PostProcessing.py` & `nuitka_winsvc-2.2.3/nuitka/PostProcessing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Progress.py` & `nuitka_winsvc-2.2.3/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/PythonFlavors.py` & `nuitka_winsvc-2.2.3/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/PythonOperators.py` & `nuitka_winsvc-2.2.3/nuitka/PythonOperators.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/PythonVersions.py` & `nuitka_winsvc-2.2.3/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Serialization.py` & `nuitka_winsvc-2.2.3/nuitka/Serialization.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/SourceCodeReferences.py` & `nuitka_winsvc-2.2.3/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Tracing.py` & `nuitka_winsvc-2.2.3/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/TreeXML.py` & `nuitka_winsvc-2.2.3/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Variables.py` & `nuitka_winsvc-2.2.3/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/Version.py` & `nuitka_winsvc-2.2.3/nuitka/Version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V2.2.2
+Nuitka V2.2.3
 Copyright (C) 2024 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `nuitka_winsvc-2.2.2/nuitka/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/__past__.py` & `nuitka_winsvc-2.2.3/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/Backend.scons` & `nuitka_winsvc-2.2.3/nuitka/build/Backend.scons`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/CCompilerVersion.scons` & `nuitka_winsvc-2.2.3/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/DataComposerInterface.py` & `nuitka_winsvc-2.2.3/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/Onefile.scons` & `nuitka_winsvc-2.2.3/nuitka/build/Onefile.scons`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/SconsCaching.py` & `nuitka_winsvc-2.2.3/nuitka/build/SconsCaching.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/SconsCompilerSettings.py` & `nuitka_winsvc-2.2.3/nuitka/build/SconsCompilerSettings.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/SconsHacks.py` & `nuitka_winsvc-2.2.3/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/SconsInterface.py` & `nuitka_winsvc-2.2.3/nuitka/build/SconsInterface.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/SconsProgress.py` & `nuitka_winsvc-2.2.3/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/SconsSpawn.py` & `nuitka_winsvc-2.2.3/nuitka/build/SconsSpawn.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/SconsUtils.py` & `nuitka_winsvc-2.2.3/nuitka/build/SconsUtils.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/allocator.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/builtins.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/calling.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/checkers.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/checksum_tools.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_asyncgen.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_cell.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_coroutine.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_frame.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_function.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_generator.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/compiled_method.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/constants.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/constants.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/constants_blob.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/environment_variables.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/environment_variables.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/environment_variables_system.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/environment_variables_system.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/exception_groups.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/exception_groups.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/exceptions.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/filesystem_paths.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/freelists.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/hedley.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/attributes.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/boolean.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/bytearrays.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/bytes.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/calling_generated.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_le.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/complex.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/dictionaries.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/floats.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/import_hard.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/indexes.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/ints.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/iterators.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/lists.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/lists_generated.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/mappings.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/raising.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/rangeobjects.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/richcomparisons.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/sequences.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/sets.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/slices.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/strings.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/subscripts.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helper/tuples.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/helpers.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/helpers.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/importing.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/incbin.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/jit_sources.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/jit_sources.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/prelude.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/prelude.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/printing.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/python_pgo.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/safe_string_ops.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/threading.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/tracing.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/type_aliases.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/type_aliases.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/include/nuitka/unfreezing.h` & `nuitka_winsvc-2.2.3/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/appdirs/appdirs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/atomicwrites/LICENSE` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/bin/scons.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/clcache/clcache/caching.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/LICENSE.txt` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/win32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/LICENSE` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/glob2/compat.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/glob2/glob2/impl.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/LICENSE` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/composer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/error.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/events.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/loader.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/parser.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/reader.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/representer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/LICENSE` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/LICENSE` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/LICENSE` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/LICENSE`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/crc32.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/crc32.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/zconf.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/zlib.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zlib/zutil.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/LICENSE.txt` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/bitstream.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/compiler.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/cpu.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/debug.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/error_private.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/error_private.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/fse.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/huf.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/mem.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/xxhash.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/xxhash.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/inline_copy/zstd/zstd.h` & `nuitka_winsvc-2.2.3/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledAsyncgenType.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledCellType.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledCodeHelpers.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledCoroutineType.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledFrameType.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledFunctionType.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledGeneratorType.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/CompiledMethodType.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersAllocator.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersAttributes.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersBuiltin.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersBytes.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersCalling.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersCallingGenerated.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersChecksumTools.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersClasses.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonEq.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonGe.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonGt.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonLe.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonLt.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersComparisonNe.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersConstantsBlob.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersDeepcopy.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersDictionaries.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersDumpBacktraces.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersDumpBacktraces.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersEnvironmentVariables.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersEnvironmentVariables.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersExceptions.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersFiles.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersFiles.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersFilesystemPaths.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersFloats.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersHeapStorage.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersImport.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersImportHard.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersJitSources.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersJitSources.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersLists.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersLists.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersListsGenerated.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersMappings.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersMatching.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinarySub.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplacePow.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersProfiling.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersPythonPgo.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersRaising.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersSafeStrings.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersSequences.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersSlices.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersStrings.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersTuples.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/HelpersTypes.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/InspectPatcher.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/MainProgram.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/MainProgram.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/MetaPathBasedLoader.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/OnefileBootstrap.c` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files 0% similar despite different names*

```diff
@@ -40,17 +40,15 @@
 #include <wchar.h>
 
 /* Type bool */
 #ifndef __cplusplus
 #include "stdbool.h"
 #endif
 
-#if defined(_WIN32)
-#include <imagehlp.h>
-#else
+#if !defined(_WIN32)
 #include <dirent.h>
 #include <signal.h>
 #include <sys/stat.h>
 #include <sys/types.h>
 #include <sys/wait.h>
 #include <unistd.h>
 #endif
```

### Comparing `nuitka_winsvc-2.2.2/nuitka/build/static_src/OnefileSplashScreen.cpp` & `nuitka_winsvc-2.2.3/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/AsyncgenCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/AttributeCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/BranchCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/BuiltinCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/BuiltinCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/CallCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ClassCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/CodeGeneration.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/CodeGeneration.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/CodeHelperSelection.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/CodeHelpers.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/CodeObjectCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ComparisonCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ComparisonHelperDefinitions.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ConditionalCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ConstantCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/Contexts.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/CoroutineCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/CtypesCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/DictCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/Emission.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ErrorCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/EvalCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ExceptionCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ExceptionCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ExpressionCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/FrameCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/FunctionCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/GeneratorCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/GlobalConstants.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/GlobalConstants.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/GlobalsLocalsCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/IdCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ImportCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/Indentation.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/IndexCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/InjectCCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/IntegerCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/IteratorCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/JitCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/JitCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/LabelCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/LineNumberCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ListCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/LoaderCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/LocalsDictCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/LoopCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/MatchCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ModuleCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/Namify.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/NetworkxCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/NetworkxCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/OperationCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/PackageResourceCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/PrintCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/PythonAPICodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/RaisingCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/Reports.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/ReturnCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/SetCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/SliceCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/StringCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/SubscriptCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/TensorflowCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/TensorflowCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/TryCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/TupleCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/TypeAliasCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/TypeAliasCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/VariableCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/VariableDeclarations.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/YieldCodes.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/YieldCodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeBases.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeBooleans.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeCFloats.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeCLongs.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/CTypeVoids.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/c_types/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesModules.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `nuitka_winsvc-2.2.3/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/containers/Namedtuples.py` & `nuitka_winsvc-2.2.3/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/containers/OrderedDicts.py` & `nuitka_winsvc-2.2.3/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/containers/OrderedSets.py` & `nuitka_winsvc-2.2.3/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/containers/OrderedSetsFallback.py` & `nuitka_winsvc-2.2.3/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/containers/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/distutils/Build.py` & `nuitka_winsvc-2.2.3/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/distutils/DistutilCommands.py` & `nuitka_winsvc-2.2.3/nuitka/distutils/DistutilCommands.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/distutils/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/finalizations/Finalization.py` & `nuitka_winsvc-2.2.3/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/finalizations/FinalizeMarkups.py` & `nuitka_winsvc-2.2.3/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/finalizations/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/DependsExe.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/DllDependenciesCommon.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/DllDependenciesMacOS.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/DllDependenciesPosix.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/DllDependenciesWin32.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/ImportDetection.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/ImportDetection.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/IncludedDataFiles.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/IncludedEntryPoints.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/Onefile.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/Onefile.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/Standalone.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/Standalone.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/freezer/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/importing/IgnoreListing.py` & `nuitka_winsvc-2.2.3/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/importing/ImportCache.py` & `nuitka_winsvc-2.2.3/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/importing/ImportResolving.py` & `nuitka_winsvc-2.2.3/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/importing/Importing.py` & `nuitka_winsvc-2.2.3/nuitka/importing/Importing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/importing/PreloadedPackages.py` & `nuitka_winsvc-2.2.3/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/importing/Recursion.py` & `nuitka_winsvc-2.2.3/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/importing/StandardLibrary.py` & `nuitka_winsvc-2.2.3/nuitka/importing/StandardLibrary.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/importing/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/AsyncgenNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/AttributeLookupNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/AttributeNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/AttributeNodesGenerated.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinAllNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinAnyNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinComplexNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinDecodingNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinDecoratorNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinDictNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinFormatNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinHashNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinInputNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinInputNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinIntegerNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinIteratorNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinLenNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinNextNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinOpenNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinRangeNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinRefNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinRefNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinSumNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinTypeNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BuiltinVarsNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/BytesNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/CallNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/Checkers.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ChildrenHavingMixins.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ClassNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/CodeObjectSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ComparisonNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ConditionalNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ConstantRefNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ContainerMakingNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ContainerOperationNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/CoroutineNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/CtypesNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/DictionaryNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/DictionaryNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ExceptionNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ExceptionNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ExecEvalNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ExpressionBases.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ExpressionBasesGenerated.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ExpressionShapeMixins.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/FrameNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/FunctionAttributeNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/FunctionNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/FunctionNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/FutureSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/GeneratorNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/GlobalsLocalsNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/HardImportNodesGenerated.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ImportHardNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ImportNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ImportNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/IndicatorMixins.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/InjectCNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/IterationHandles.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/KeyValuePairNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ListOperationNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/LocalsDictNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/LocalsScopes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/LoopNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/MatchNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ModuleAttributeNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ModuleNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ModuleNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/NetworkxNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/NetworkxNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/NodeBases.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/NodeMakingHelpers.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/NodeMetaClasses.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/NodeMetaClasses.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/OperatorNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/OperatorNodesUnary.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/OsSysNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/OutlineNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/PackageMetadataNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/PackageResourceNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/PrintNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/ReturnNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/SideEffectNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/SliceNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/StatementBasesGenerated.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/StatementNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/StrNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/StringConcatenationNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/SubscriptNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/TensorflowNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/TensorflowNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/TryNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/TypeMatchNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/TypeNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/VariableAssignNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/VariableDelNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/VariableNameNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/VariableRefNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/VariableReleaseNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/YieldNodes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/shapes/ShapeMixins.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/shapes/StandardShapes.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/nodes/shapes/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/optimizations/BytecodeDemotion.py` & `nuitka_winsvc-2.2.3/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/optimizations/FunctionInlining.py` & `nuitka_winsvc-2.2.3/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/optimizations/Graphs.py` & `nuitka_winsvc-2.2.3/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/optimizations/Optimization.py` & `nuitka_winsvc-2.2.3/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/optimizations/OptimizeBuiltinCalls.py` & `nuitka_winsvc-2.2.3/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/optimizations/Tags.py` & `nuitka_winsvc-2.2.3/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/optimizations/TraceCollections.py` & `nuitka_winsvc-2.2.3/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/optimizations/ValueTraces.py` & `nuitka_winsvc-2.2.3/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/optimizations/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/pgo/PGO.py` & `nuitka_winsvc-2.2.3/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/pgo/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/PluginBase.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/PluginBase.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/Plugins.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/Plugins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/AntiBloatPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/DataFilesPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/DelvewheelPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/DillPlugin/DillPlugin.c` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/DillPlugin/DillPlugin.c`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/DillPlugin/dill-postLoad.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/DillPlugin/dill-postLoad.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/DillPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/DllFilesPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/EnumPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/EventletPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/GeventPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/GiPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/GlfwPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/ImplicitImports.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/ImplicitImports.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/KivyPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/MatplotlibPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/MultiprocessingPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/NumpyPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/OptionsNannyPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/PbrPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/PkgResourcesPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/PmwPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/PySidePyQtPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,14 +402,15 @@
             ".json",
             ".png",
             ".ttf",
             ".metainfo",
             ".mesh",
             ".frag",
             "qmldir",
+            ".webp",
         )
 
         if dlls:
             ignore_suffixes = datafile_suffixes
             only_suffixes = ()
         else:
             ignore_suffixes = ()
```

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/PywebViewPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/TensorflowPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/TkinterPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/TorchPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/TransformersPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/TransformersPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/TrioPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/UpxPlugin.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 0% similar despite different names*

```diff
@@ -3751,19 +3751,27 @@
         - 'autograd.numpy'
 
 - module-name: 'pymssql' # checksum: 1767fe26
   implicit-imports:
     - depends:
         - 'pymssql._mssql'
 
-- module-name: 'pyocd' # checksum: 5c06f0b9
+- module-name: 'pyocd' # checksum: f450220c
   data-files:
     patterns:
       - 'debug/sequences/*.lark'
       - 'debug/svd/*.zip'
+    include-metadata:
+      - 'pyocd'
+  implicit-imports:
+    - depends:
+        - 'pyocd.probe.*'
+        - 'pyocd.rtos.*'
+        - 'pylink-square'
+        - 'pyusb'
 
 - module-name: 'pyodbc' # checksum: 893567d5
   implicit-imports:
     - depends:
         - 'hashlib'
         - 'decimal'
 
@@ -4006,15 +4014,15 @@
       - description: 'PySide2 cannot be signed unless onefile'
         macos_bundle_as_onefile: 'yes'
         when: 'macos and use_pyside2'
   import-hacks:
     - find-dlls-near-module:
         - 'shiboken2'
 
-- module-name: 'PySide6' # checksum: db68a9cc
+- module-name: 'PySide6' # checksum: 8852cddf
   implicit-imports:
     - post-import-code:
         - |
           def patched_disconnect(self, slot=None):
               if hasattr(slot, "im_func"):
                   if hasattr(slot.im_func, "__compiled__"):
                       patched_disconnect._protected = getattr(patched_disconnect, "_protected", [])
@@ -4057,14 +4065,16 @@
     - acceptable-missing-dlls:
         - 'libeffectsplugin'
         - 'libeffects'
         - 'libpdfquickplugin'
         - 'libqpdf'
         - 'libqtquick3dhelpersimplplugin'
         - 'libquick3dspatialaudioplugin'
+        - 'libqtvkbcomponentsplugin'
+        - 'libqtvkbsettingsplugin'
 
 - module-name: 'PySide6.QtCore' # checksum: be0d99ac
   implicit-imports:
     - depends:
         - 'PySide6.support.deprecated'
 
 - module-name: 'pysnmp.smi' # checksum: d8623e4b
```

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `nuitka_winsvc-2.2.3/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/reports/CompilationReportReader.py` & `nuitka_winsvc-2.2.3/nuitka/reports/CompilationReportReader.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/reports/LicenseReport.rst.j2` & `nuitka_winsvc-2.2.3/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/reports/Reports.py` & `nuitka_winsvc-2.2.3/nuitka/reports/Reports.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/reports/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/BuiltinBytesOperationSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/BuiltinDictOperationSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/BuiltinListOperationSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/BuiltinParameterSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/BuiltinStrOperationSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/BuiltinTypeOperationSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/HardImportSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/ParameterSpecs.py` & `nuitka_winsvc-2.2.3/nuitka/specs/ParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/specs/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/Basics.py` & `nuitka_winsvc-2.2.3/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/commercial/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/data_composer/DataComposer.py` & `nuitka_winsvc-2.2.3/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/data_composer/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/data_composer/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/environments/CreateEnvironment.py` & `nuitka_winsvc-2.2.3/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/environments/Virtualenv.py` & `nuitka_winsvc-2.2.3/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/environments/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/general/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/general/dll_report/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/general/dll_report/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/general/find_module/FindModuleCode.py` & `nuitka_winsvc-2.2.3/nuitka/tools/general/find_module/FindModuleCode.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/general/find_module/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `nuitka_winsvc-2.2.3/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/onefile_compressor/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/onefile_compressor/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/podman/Podman.py` & `nuitka_winsvc-2.2.3/nuitka/tools/podman/Podman.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/podman/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/podman/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/podman/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/podman/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/profiler/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/profiler/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/scanning/DisplayPackageDLLs.py` & `nuitka_winsvc-2.2.3/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/scanning/DisplayPackageData.py` & `nuitka_winsvc-2.2.3/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/scanning/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/specialize/CTypeDescriptions.py` & `nuitka_winsvc-2.2.3/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/specialize/Common.py` & `nuitka_winsvc-2.2.3/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/specialize/SpecializeC.py` & `nuitka_winsvc-2.2.3/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/specialize/SpecializePython.py` & `nuitka_winsvc-2.2.3/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/specialize/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/Common.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/Common.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/Constructs.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/OutputComparison.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/Pythons.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/RuntimeTracing.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/SearchModes.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/Valgrind.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/check_reference_counts/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/check_reference_counts/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/compare_with_cpython/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/compare_with_cpython/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/find_sxs_modules/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/find_sxs_modules/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/measure_construct_performance/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/measure_construct_performance/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/watch/GitHub.py` & `nuitka_winsvc-2.2.3/nuitka/tools/watch/GitHub.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/watch/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tools/watch/__main__.py` & `nuitka_winsvc-2.2.3/nuitka/tools/watch/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/Building.py` & `nuitka_winsvc-2.2.3/nuitka/tree/Building.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ComplexCallHelperFunctions.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/Extractions.py` & `nuitka_winsvc-2.2.3/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/InternalModule.py` & `nuitka_winsvc-2.2.3/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/Operations.py` & `nuitka_winsvc-2.2.3/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationAssertStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationAssignmentStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationBooleanExpressions.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationCallExpressions.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationClasses.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationClasses3.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationComparisonExpressions.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationContractionExpressions.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationDictionaryCreation.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationExecStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationForLoopStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationFunctionStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationImportStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationLambdaExpressions.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationMatchStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationMultidist.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationNamespacePackages.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationPrintStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationSequenceCreation.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationSubscriptExpressions.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationTryExceptStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationTryFinallyStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationWhileLoopStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationWithStatements.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/ReformulationYieldExpressions.py` & `nuitka_winsvc-2.2.3/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/SourceHandling.py` & `nuitka_winsvc-2.2.3/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/SyntaxErrors.py` & `nuitka_winsvc-2.2.3/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/TreeHelpers.py` & `nuitka_winsvc-2.2.3/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/VariableClosure.py` & `nuitka_winsvc-2.2.3/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/tree/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/AppDirs.py` & `nuitka_winsvc-2.2.3/nuitka/utils/AppDirs.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/CStrings.py` & `nuitka_winsvc-2.2.3/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/CommandLineOptions.py` & `nuitka_winsvc-2.2.3/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Distributions.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Distributions.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Download.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Execution.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Execution.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/FileOperations.py` & `nuitka_winsvc-2.2.3/nuitka/utils/FileOperations.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Hashing.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Images.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Images.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     if needs_conversion:
         try:
             import imageio  # pylint: disable=I0021,import-error,unused-import
         except ImportError:
             logger.sysexit(
                 """\
-Need to install 'imageio' to let automatically convert the non native \
+Need to install 'imageio' to automatically convert the non native \
 icon image (%s) in file in '%s'."""
                 % (icon_format[1:].upper(), icon_path)
             )
 
 
 def convertImageToIconFormat(logger, image_filename, converted_icon_filename):
     """Convert image file to icon file."""
```

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Importing.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Importing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/InstalledPythons.py` & `nuitka_winsvc-2.2.3/nuitka/utils/InstalledPythons.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/InstanceCounters.py` & `nuitka_winsvc-2.2.3/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Jinja2.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Json.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/MacOSApp.py` & `nuitka_winsvc-2.2.3/nuitka/utils/MacOSApp.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/MemoryUsage.py` & `nuitka_winsvc-2.2.3/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/ModuleNames.py` & `nuitka_winsvc-2.2.3/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/ReExecute.py` & `nuitka_winsvc-2.2.3/nuitka/utils/ReExecute.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Rest.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/SharedLibraries.py` & `nuitka_winsvc-2.2.3/nuitka/utils/SharedLibraries.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Shebang.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Signing.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/SlotMetaClasses.py` & `nuitka_winsvc-2.2.3/nuitka/utils/SlotMetaClasses.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/StaticLibraries.py` & `nuitka_winsvc-2.2.3/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/ThreadedExecutor.py` & `nuitka_winsvc-2.2.3/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Timing.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Utils.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/WindowsFileUsage.py` & `nuitka_winsvc-2.2.3/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/WindowsResources.py` & `nuitka_winsvc-2.2.3/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/Yaml.py` & `nuitka_winsvc-2.2.3/nuitka/utils/Yaml.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/nuitka/utils/__init__.py` & `nuitka_winsvc-2.2.3/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/pyproject.toml` & `nuitka_winsvc-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/setup.py` & `nuitka_winsvc-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/AssertsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/AssignmentsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/AssignmentsTest32.py` & `nuitka_winsvc-2.2.3/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/BranchingTest.py` & `nuitka_winsvc-2.2.3/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/BuiltinOverload.py` & `nuitka_winsvc-2.2.3/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/BuiltinSuperTest.py` & `nuitka_winsvc-2.2.3/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/BuiltinsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ClassMinimalTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ClassesTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ClassesTest32.py` & `nuitka_winsvc-2.2.3/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ClassesTest34.py` & `nuitka_winsvc-2.2.3/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ComparisonChainsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ConstantsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ConstantsTest27.py` & `nuitka_winsvc-2.2.3/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/DecoratorsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/DefaultParametersTest.py` & `nuitka_winsvc-2.2.3/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/DoubleDeletionsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/EmptyModuleTest.py` & `nuitka_winsvc-2.2.3/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ExceptionRaisingTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ExceptionRaisingTest32.py` & `nuitka_winsvc-2.2.3/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ExceptionRaisingTest33.py` & `nuitka_winsvc-2.2.3/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ExecEvalTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ExtremeClosureTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/FunctionObjectsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/FunctionsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/FunctionsTest32.py` & `nuitka_winsvc-2.2.3/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/FunctionsTest_2.py` & `nuitka_winsvc-2.2.3/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/FutureTest32.py` & `nuitka_winsvc-2.2.3/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/GeneratorExpressionsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/GeneratorExpressionsTest_37.py` & `nuitka_winsvc-2.2.3/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/GlobalStatementTest.py` & `nuitka_winsvc-2.2.3/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/HelloWorldTest_2.py` & `nuitka_winsvc-2.2.3/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ImportingTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/InplaceOperationsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/InspectionTest.py` & `nuitka_winsvc-2.2.3/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/InspectionTest_35.py` & `nuitka_winsvc-2.2.3/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/InspectionTest_36.py` & `nuitka_winsvc-2.2.3/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/LambdasTest.py` & `nuitka_winsvc-2.2.3/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/LateClosureAssignmentTest.py` & `nuitka_winsvc-2.2.3/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ListContractionsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/LoopingTest.py` & `nuitka_winsvc-2.2.3/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/MainProgramsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ModuleAttributesTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/OperatorsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/OrderChecksTest.py` & `nuitka_winsvc-2.2.3/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/OrderChecksTest27.py` & `nuitka_winsvc-2.2.3/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/OverflowFunctionsTest_2.py` & `nuitka_winsvc-2.2.3/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ParameterErrorsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ParameterErrorsTest32.py` & `nuitka_winsvc-2.2.3/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/PrintFutureTest.py` & `nuitka_winsvc-2.2.3/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/PrintingTest_2.py` & `nuitka_winsvc-2.2.3/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/RecursionTest.py` & `nuitka_winsvc-2.2.3/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ReferencingTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ReferencingTest27.py` & `nuitka_winsvc-2.2.3/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ReferencingTest33.py` & `nuitka_winsvc-2.2.3/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ReferencingTest35.py` & `nuitka_winsvc-2.2.3/tests/basics/ReferencingTest35.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ReferencingTest36.py` & `nuitka_winsvc-2.2.3/tests/basics/ReferencingTest36.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ReferencingTest_2.py` & `nuitka_winsvc-2.2.3/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/SlotsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/ThreadedGeneratorsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/TrickAssignmentsTest32.py` & `nuitka_winsvc-2.2.3/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/TrickAssignmentsTest35.py` & `nuitka_winsvc-2.2.3/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/TrickAssignmentsTest_2.py` & `nuitka_winsvc-2.2.3/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/TryContinueFinallyTest.py` & `nuitka_winsvc-2.2.3/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/TryExceptContinueTest.py` & `nuitka_winsvc-2.2.3/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/TryExceptFinallyTest.py` & `nuitka_winsvc-2.2.3/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/TryExceptFramesTest.py` & `nuitka_winsvc-2.2.3/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/TryReturnFinallyTest.py` & `nuitka_winsvc-2.2.3/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/TryYieldFinallyTest.py` & `nuitka_winsvc-2.2.3/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/UnicodeTest.py` & `nuitka_winsvc-2.2.3/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/UnpackingTest35.py` & `nuitka_winsvc-2.2.3/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/VarargsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/WithStatementsTest.py` & `nuitka_winsvc-2.2.3/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/YieldFromTest33.py` & `nuitka_winsvc-2.2.3/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/run_all.py` & `nuitka_winsvc-2.2.3/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/basics/run_xml.py` & `nuitka_winsvc-2.2.3/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/onefile/HelloWorldTest.py` & `nuitka_winsvc-2.2.3/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/onefile/KeyboardInterruptTest.py` & `nuitka_winsvc-2.2.3/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/onefile/run_all.py` & `nuitka_winsvc-2.2.3/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/ArgumentTypes.py` & `nuitka_winsvc-2.2.3/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/AttributesTest.py` & `nuitka_winsvc-2.2.3/tests/optimizations/AttributesTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/CallsTest.py` & `nuitka_winsvc-2.2.3/tests/optimizations/CallsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/ConditionsTest.py` & `nuitka_winsvc-2.2.3/tests/optimizations/ConditionsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/DecodingOperationsTest.py` & `nuitka_winsvc-2.2.3/tests/optimizations/DecodingOperationsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/FormatStringsTest36.py` & `nuitka_winsvc-2.2.3/tests/optimizations/FormatStringsTest36.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/HardImportsTest.py` & `nuitka_winsvc-2.2.3/tests/optimizations/HardImportsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/HardImportsTest_2.py` & `nuitka_winsvc-2.2.3/tests/optimizations/HardImportsTest_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/Iterations.py` & `nuitka_winsvc-2.2.3/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/LenTest.py` & `nuitka_winsvc-2.2.3/tests/optimizations/LenTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/MatchingTest310.py` & `nuitka_winsvc-2.2.3/tests/optimizations/MatchingTest310.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/OperationsTest.py` & `nuitka_winsvc-2.2.3/tests/optimizations/OperationsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/SubscriptsTest.py` & `nuitka_winsvc-2.2.3/tests/optimizations/SubscriptsTest.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/optimizations/run_all.py` & `nuitka_winsvc-2.2.3/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py` & `nuitka_winsvc-2.2.3/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/package_data_files_embedding/__init__.py` & `nuitka_winsvc-2.2.3/tests/packages/package_data_files_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `nuitka_winsvc-2.2.3/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `nuitka_winsvc-2.2.3/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/run_all.py` & `nuitka_winsvc-2.2.3/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/__init__.py` & `nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/bigkitty.py` & `nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/smallkitty.py` & `nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/speak/__init__.py` & `nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/speak/hello.py` & `nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/speak/miau.py` & `nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/sub_package/kitty/speak/purr.py` & `nuitka_winsvc-2.2.3/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/top_level_attributes_3/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/packages/top_level_attributes_3/some_package/some_module.py` & `nuitka_winsvc-2.2.3/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/plugins/code_signing/CodeSigningMain.py` & `nuitka_winsvc-2.2.3/tests/plugins/code_signing/CodeSigningMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/plugins/data_files/DataFilesMain.py` & `nuitka_winsvc-2.2.3/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/plugins/data_files/data_files_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/plugins/parameters/ParametersMain.py` & `nuitka_winsvc-2.2.3/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/plugins/parameters/parameter-using-plugin.py` & `nuitka_winsvc-2.2.3/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/plugins/run_all.py` & `nuitka_winsvc-2.2.3/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/absolute_import/AbsoluteImportMain.py` & `nuitka_winsvc-2.2.3/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/absolute_import/foobar/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/absolute_import/foobar/foobar.py` & `nuitka_winsvc-2.2.3/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/absolute_import/foobar/local.py` & `nuitka_winsvc-2.2.3/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/absolute_import/foobar/util.py` & `nuitka_winsvc-2.2.3/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports1/CasedImportingMain.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports1/path1/Some_Module.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports1/path2/some_module.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports1/path2/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports2/CasedImportingMain.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports2/path1/some_module.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports2/path1/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports2/path2/Some_Module.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports3/CasedImportingMain.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports3/path1/Some_Module.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports3/path2/Some_Module.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/CyclicImportsMain.py` & `nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/dash_import/DashImportMain.py` & `nuitka_winsvc-2.2.3/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/dash_import/dash-module.py` & `nuitka_winsvc-2.2.3/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/dash_import/plus+module.py` & `nuitka_winsvc-2.2.3/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/dash_main/Dash-Main.py` & `nuitka_winsvc-2.2.3/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/deep/DeepProgramMain.py` & `nuitka_winsvc-2.2.3/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/deep/some_package/DeepBrother.py` & `nuitka_winsvc-2.2.3/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/deep/some_package/DeepChild.py` & `nuitka_winsvc-2.2.3/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/deep/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `nuitka_winsvc-2.2.3/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/deep/some_package/deep_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `nuitka_winsvc-2.2.3/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/dunderinit_imports/package/SubModule.py` & `nuitka_winsvc-2.2.3/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/dunderinit_imports/package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/import_variants/ImportVariationsMain.py` & `nuitka_winsvc-2.2.3/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/import_variants/some_package/Child1.py` & `nuitka_winsvc-2.2.3/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/import_variants/some_package/Child2.py` & `nuitka_winsvc-2.2.3/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/import_variants/some_package/Child3.py` & `nuitka_winsvc-2.2.3/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/import_variants/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/main_raises/ErrorMain.py` & `nuitka_winsvc-2.2.3/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/main_raises/ErrorRaising.py` & `nuitka_winsvc-2.2.3/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/main_raises2/ErrorInFunctionMain.py` & `nuitka_winsvc-2.2.3/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/main_raises2/ErrorRaising.py` & `nuitka_winsvc-2.2.3/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_attributes/ModuleAttributesMain.py` & `nuitka_winsvc-2.2.3/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/Nearby1.py` & `nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_exits/ErrorExitingModule.py` & `nuitka_winsvc-2.2.3/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_exits/Main.py` & `nuitka_winsvc-2.2.3/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `nuitka_winsvc-2.2.3/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/module_object_replacing/SelfReplacingModule.py` & `nuitka_winsvc-2.2.3/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/foo/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/foo/__main__.py` & `nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/multiprocessing_using/foo/entry.py` & `nuitka_winsvc-2.2.3/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/named_imports/NamedImportsMain.py` & `nuitka_winsvc-2.2.3/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/named_imports/some_package/SomeModule.py` & `nuitka_winsvc-2.2.3/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/named_imports/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `nuitka_winsvc-2.2.3/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_code/PackageInitCodeMain.py` & `nuitka_winsvc-2.2.3/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_code/some_package/SomeModule.py` & `nuitka_winsvc-2.2.3/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_code/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_contains_main/PackageContainsMain.py` & `nuitka_winsvc-2.2.3/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_contains_main/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_contains_main/local.py` & `nuitka_winsvc-2.2.3/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_init_import/PackageInitImportMain.py` & `nuitka_winsvc-2.2.3/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_init_import/some_package/PackageLocal.py` & `nuitka_winsvc-2.2.3/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_init_import/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_init_issue/PackageInitIssueMain.py` & `nuitka_winsvc-2.2.3/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_init_issue/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `nuitka_winsvc-2.2.3/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_missing_init/PackageMissingInitMain.py` & `nuitka_winsvc-2.2.3/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_missing_init/some_package/some_module.py` & `nuitka_winsvc-2.2.3/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `nuitka_winsvc-2.2.3/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `nuitka_winsvc-2.2.3/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_module_collision/Something/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_module_collision/something.py` & `nuitka_winsvc-2.2.3/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_overload/Main.py` & `nuitka_winsvc-2.2.3/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_overload/foo/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_overload/foo/bar.py` & `nuitka_winsvc-2.2.3/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_overload/foo/bar2.py` & `nuitka_winsvc-2.2.3/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `nuitka_winsvc-2.2.3/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_prevents_submodule/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_prevents_submodule/some_package/some_module.py` & `nuitka_winsvc-2.2.3/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_program/PackageAsMain/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/package_program/PackageAsMain/__main__.py` & `nuitka_winsvc-2.2.3/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/pkgutil_usage/package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/plugin_import/PluginImportMain.py` & `nuitka_winsvc-2.2.3/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/plugin_import/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/plugin_import/some_package/some_module.py` & `nuitka_winsvc-2.2.3/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `nuitka_winsvc-2.2.3/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `nuitka_winsvc-2.2.3/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/relative_import/RelativeImportMain.py` & `nuitka_winsvc-2.2.3/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/relative_import/dircache.py` & `nuitka_winsvc-2.2.3/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/resource_reader37/ResourceReaderMain.py` & `nuitka_winsvc-2.2.3/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/resource_reader37/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/run_all.py` & `nuitka_winsvc-2.2.3/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/pyexpat.py` & `nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/some_package/__init__.py` & `nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/some_package/normal_importing.py` & `nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/some_package/pyexpat.py` & `nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/stdlib_overload/some_package/star_importing.py` & `nuitka_winsvc-2.2.3/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/syntax_errors/IndentationErroring.py` & `nuitka_winsvc-2.2.3/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/syntax_errors/SyntaxErroring.py` & `nuitka_winsvc-2.2.3/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `nuitka_winsvc-2.2.3/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/unicode_bom/UnicodeBomMain.py` & `nuitka_winsvc-2.2.3/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/unicode_bom/unicode_bom.py` & `nuitka_winsvc-2.2.3/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/programs/with space/Space Main.py` & `nuitka_winsvc-2.2.3/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/reflected/compile_itself.py` & `nuitka_winsvc-2.2.3/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/run-tests` & `nuitka_winsvc-2.2.3/tests/run-tests`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/BrotliUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/CtypesUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/DateutilsUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/DateutilsUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/FlaskUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/GiUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/GiUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/GlfwUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/GtkUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/HexEncodingTest_2.py` & `nuitka_winsvc-2.2.3/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/IdnaUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/LxmlUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/MatplotlibUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/MetadataPackagesUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/NumpyUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/OpenGLUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PandasUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PasslibUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PendulumUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PkgResourcesRequiresUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PmwUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PyQt5Plugins.py` & `nuitka_winsvc-2.2.3/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PyQt5SSLSupport.py` & `nuitka_winsvc-2.2.3/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PyQt5Using.py` & `nuitka_winsvc-2.2.3/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PyQt6Plugins.py` & `nuitka_winsvc-2.2.3/tests/standalone/PyQt6Plugins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PyQt6Using.py` & `nuitka_winsvc-2.2.3/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PySide2Using.py` & `nuitka_winsvc-2.2.3/tests/standalone/PySide2Using.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PySide6Plugins.py` & `nuitka_winsvc-2.2.3/tests/standalone/PySide6Plugins.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/PySide6Using.py` & `nuitka_winsvc-2.2.3/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/RsaUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/SetuptoolsUsing_311.py` & `nuitka_winsvc-2.2.3/tests/standalone/SetuptoolsUsing_311.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/ShlibUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/SocketUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/TkInterUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/Urllib3Using.py` & `nuitka_winsvc-2.2.3/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/Win32ComUsing.py` & `nuitka_winsvc-2.2.3/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/run_all.py` & `nuitka_winsvc-2.2.3/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/standalone/zip_importer/ZipImporterMain.py` & `nuitka_winsvc-2.2.3/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/AsyncgenReturn36.py` & `nuitka_winsvc-2.2.3/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/AwaitInModule36.py` & `nuitka_winsvc-2.2.3/tests/syntax/AwaitInModule36.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/BreakWithoutLoop.py` & `nuitka_winsvc-2.2.3/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/ClassReturn.py` & `nuitka_winsvc-2.2.3/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/ClosureDel_2.py` & `nuitka_winsvc-2.2.3/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/ContinueWithoutLoop.py` & `nuitka_winsvc-2.2.3/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/DuplicateArgument.py` & `nuitka_winsvc-2.2.3/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/ExecWithNesting_2.py` & `nuitka_winsvc-2.2.3/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/FutureBraces.py` & `nuitka_winsvc-2.2.3/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/FutureUnknown.py` & `nuitka_winsvc-2.2.3/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/GeneratorExpressions38.py` & `nuitka_winsvc-2.2.3/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/GeneratorReturn_2.py` & `nuitka_winsvc-2.2.3/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/GlobalForParameter.py` & `nuitka_winsvc-2.2.3/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/Importing32.py` & `nuitka_winsvc-2.2.3/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/IndentationError.py` & `nuitka_winsvc-2.2.3/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/LateFutureImport.py` & `nuitka_winsvc-2.2.3/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/MisplacedFutureImport.py` & `nuitka_winsvc-2.2.3/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/ModuleReturn.py` & `nuitka_winsvc-2.2.3/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/NonAsciiWithoutEncoding_2.py` & `nuitka_winsvc-2.2.3/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/NonlocalForParameter32.py` & `nuitka_winsvc-2.2.3/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/NonlocalNotFound32.py` & `nuitka_winsvc-2.2.3/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/StarImportExtra.py` & `nuitka_winsvc-2.2.3/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/SyntaxError.py` & `nuitka_winsvc-2.2.3/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/TryExceptAllNotLast.py` & `nuitka_winsvc-2.2.3/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/TryFinallyContinue_37.py` & `nuitka_winsvc-2.2.3/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/UnpackNoTuple.py` & `nuitka_winsvc-2.2.3/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/UnpackTwoStars32.py` & `nuitka_winsvc-2.2.3/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/YieldFromInModule.py` & `nuitka_winsvc-2.2.3/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/YieldInAsync35.py` & `nuitka_winsvc-2.2.3/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/YieldInGenexp38.py` & `nuitka_winsvc-2.2.3/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/YieldInModule.py` & `nuitka_winsvc-2.2.3/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `nuitka_winsvc-2.2.2/tests/syntax/run_all.py` & `nuitka_winsvc-2.2.3/tests/syntax/run_all.py`

 * *Files identical despite different names*

