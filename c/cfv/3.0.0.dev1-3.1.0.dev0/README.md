# Comparing `tmp/cfv-3.0.0.dev1.tar.gz` & `tmp/cfv-3.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cfv-3.0.0.dev1.tar", last modified: Sun Oct 30 21:30:34 2022, max compression
+gzip compressed data, was "cfv-3.1.0.dev0.tar", last modified: Mon May 20 14:05:07 2024, max compression
```

## Comparing `cfv-3.0.0.dev1.tar` & `cfv-3.1.0.dev0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 r00t      (1000) r00t      (1000)        0 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/
--rw-rw-r--   0 r00t      (1000) r00t      (1000)    17992 2018-03-13 00:55:28.000000 cfv-3.0.0.dev1/COPYING
--rw-rw-r--   0 r00t      (1000) r00t      (1000)    13100 2021-10-29 01:02:50.000000 cfv-3.0.0.dev1/cfv.1
--rw-rw-r--   0 r00t      (1000) r00t      (1000)      146 2021-10-29 01:02:50.000000 cfv-3.0.0.dev1/MANIFEST.in
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     2176 2022-10-30 21:19:27.000000 cfv-3.0.0.dev1/setup.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     4689 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/PKG-INFO
--rw-rw-r--   0 r00t      (1000) r00t      (1000)       38 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/setup.cfg
--rw-rw-r--   0 r00t      (1000) r00t      (1000)    12317 2022-10-30 21:20:59.000000 cfv-3.0.0.dev1/Changelog
-drwxrwxr-x   0 r00t      (1000) r00t      (1000)        0 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/lib/
-drwxrwxr-x   0 r00t      (1000) r00t      (1000)        0 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/lib/cfv.egg-info/
--rw-rw-r--   0 r00t      (1000) r00t      (1000)      535 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/lib/cfv.egg-info/SOURCES.txt
--rw-rw-r--   0 r00t      (1000) r00t      (1000)       41 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/lib/cfv.egg-info/entry_points.txt
--rw-rw-r--   0 r00t      (1000) r00t      (1000)        1 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/lib/cfv.egg-info/dependency_links.txt
--rw-rw-r--   0 r00t      (1000) r00t      (1000)        4 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/lib/cfv.egg-info/top_level.txt
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     4689 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/lib/cfv.egg-info/PKG-INFO
-drwxrwxr-x   0 r00t      (1000) r00t      (1000)        0 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/lib/cfv/
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     3291 2022-10-28 22:11:18.000000 cfv-3.0.0.dev1/lib/cfv/osutil.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)    81271 2022-10-28 22:11:18.000000 cfv-3.0.0.dev1/lib/cfv/common.py
-drwxrwxr-x   0 r00t      (1000) r00t      (1000)        0 2022-10-30 21:30:34.000000 cfv-3.0.0.dev1/lib/cfv/BitTorrent/
--rw-rw-r--   0 r00t      (1000) r00t      (1000)        0 2018-03-13 02:17:59.000000 cfv-3.0.0.dev1/lib/cfv/BitTorrent/__init__.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     3730 2021-10-29 01:02:50.000000 cfv-3.0.0.dev1/lib/cfv/BitTorrent/btformats.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     6815 2022-10-28 22:11:18.000000 cfv-3.0.0.dev1/lib/cfv/BitTorrent/bencode.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     1182 2018-03-13 02:17:59.000000 cfv-3.0.0.dev1/lib/cfv/BitTorrent/LICENSE.txt
--rw-rw-r--   0 r00t      (1000) r00t      (1000)        0 2018-03-13 02:17:59.000000 cfv-3.0.0.dev1/lib/cfv/__init__.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     2521 2021-10-30 20:50:48.000000 cfv-3.0.0.dev1/lib/cfv/hash.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     2943 2022-10-28 22:11:18.000000 cfv-3.0.0.dev1/lib/cfv/strutil.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     3429 2021-10-29 01:02:50.000000 cfv-3.0.0.dev1/lib/cfv/progress.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     5586 2021-10-29 01:02:50.000000 cfv-3.0.0.dev1/lib/cfv/fileutil.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     1543 2021-10-29 01:02:50.000000 cfv-3.0.0.dev1/lib/cfv/cftypes.py
--rw-r--r--   0 r00t      (1000) r00t      (1000)      691 2019-03-24 20:41:28.000000 cfv-3.0.0.dev1/lib/cfv/term.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     7149 2021-10-29 01:02:50.000000 cfv-3.0.0.dev1/lib/cfv/ui.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     5155 2021-10-29 01:02:50.000000 cfv-3.0.0.dev1/lib/cfv/caching.py
--rw-rw-r--   0 r00t      (1000) r00t      (1000)     3353 2022-10-30 21:19:27.000000 cfv-3.0.0.dev1/README.md
+drwxr-xr-x   0     1000     1000        0 2024-05-20 14:05:07.028704 cfv-3.1.0.dev0/
+-rw-rw-r--   0     1000     1000    17992 2018-03-13 00:55:28.000000 cfv-3.1.0.dev0/COPYING
+-rw-rw-r--   0     1000     1000    12561 2024-05-20 12:09:10.000000 cfv-3.1.0.dev0/Changelog
+-rw-rw-r--   0     1000     1000      146 2021-10-29 01:02:50.000000 cfv-3.1.0.dev0/MANIFEST.in
+-rw-r--r--   0     1000     1000     5646 2024-05-20 14:05:07.028704 cfv-3.1.0.dev0/PKG-INFO
+-rw-rw-r--   0     1000     1000     4278 2024-05-16 02:03:45.000000 cfv-3.1.0.dev0/README.md
+-rw-rw-r--   0     1000     1000    13100 2021-10-29 01:02:50.000000 cfv-3.1.0.dev0/cfv.1
+drwxr-xr-x   0     1000     1000        0 2024-05-20 14:05:07.000704 cfv-3.1.0.dev0/lib/
+drwxr-xr-x   0     1000     1000        0 2024-05-20 14:05:07.024704 cfv-3.1.0.dev0/lib/cfv/
+drwxr-xr-x   0     1000     1000        0 2024-05-20 14:05:07.024704 cfv-3.1.0.dev0/lib/cfv/BitTorrent/
+-rw-rw-r--   0     1000     1000     1182 2018-03-13 02:17:59.000000 cfv-3.1.0.dev0/lib/cfv/BitTorrent/LICENSE.txt
+-rw-rw-r--   0     1000     1000        0 2018-03-13 02:17:59.000000 cfv-3.1.0.dev0/lib/cfv/BitTorrent/__init__.py
+-rw-rw-r--   0     1000     1000     6815 2022-10-28 22:11:18.000000 cfv-3.1.0.dev0/lib/cfv/BitTorrent/bencode.py
+-rw-rw-r--   0     1000     1000     3830 2024-05-16 02:03:45.000000 cfv-3.1.0.dev0/lib/cfv/BitTorrent/btformats.py
+-rw-rw-r--   0     1000     1000        0 2018-03-13 02:17:59.000000 cfv-3.1.0.dev0/lib/cfv/__init__.py
+-rw-rw-r--   0     1000     1000     5155 2021-10-29 01:02:50.000000 cfv-3.1.0.dev0/lib/cfv/caching.py
+-rw-rw-r--   0     1000     1000     1543 2021-10-29 01:02:50.000000 cfv-3.1.0.dev0/lib/cfv/cftypes.py
+-rw-rw-r--   0     1000     1000    81519 2024-05-20 12:08:20.000000 cfv-3.1.0.dev0/lib/cfv/common.py
+-rw-rw-r--   0     1000     1000     5672 2024-05-20 12:02:06.000000 cfv-3.1.0.dev0/lib/cfv/fileutil.py
+-rw-rw-r--   0     1000     1000     2676 2024-05-20 12:02:06.000000 cfv-3.1.0.dev0/lib/cfv/hash.py
+-rw-rw-r--   0     1000     1000     3291 2022-10-28 22:11:18.000000 cfv-3.1.0.dev0/lib/cfv/osutil.py
+-rw-rw-r--   0     1000     1000     3429 2021-10-29 01:02:50.000000 cfv-3.1.0.dev0/lib/cfv/progress.py
+-rw-rw-r--   0     1000     1000     2943 2022-10-28 22:11:18.000000 cfv-3.1.0.dev0/lib/cfv/strutil.py
+-rw-r--r--   0     1000     1000      691 2019-03-24 20:41:28.000000 cfv-3.1.0.dev0/lib/cfv/term.py
+-rw-rw-r--   0     1000     1000     7149 2021-10-29 01:02:50.000000 cfv-3.1.0.dev0/lib/cfv/ui.py
+drwxr-xr-x   0     1000     1000        0 2024-05-20 14:05:07.024704 cfv-3.1.0.dev0/lib/cfv.egg-info/
+-rw-r--r--   0     1000     1000     5646 2024-05-20 14:05:06.000000 cfv-3.1.0.dev0/lib/cfv.egg-info/PKG-INFO
+-rw-r--r--   0     1000     1000      535 2024-05-20 14:05:06.000000 cfv-3.1.0.dev0/lib/cfv.egg-info/SOURCES.txt
+-rw-r--r--   0     1000     1000        1 2024-05-20 14:05:06.000000 cfv-3.1.0.dev0/lib/cfv.egg-info/dependency_links.txt
+-rw-r--r--   0     1000     1000       40 2024-05-20 14:05:06.000000 cfv-3.1.0.dev0/lib/cfv.egg-info/entry_points.txt
+-rw-r--r--   0     1000     1000        4 2024-05-20 14:05:06.000000 cfv-3.1.0.dev0/lib/cfv.egg-info/top_level.txt
+-rw-r--r--   0     1000     1000       38 2024-05-20 14:05:07.028704 cfv-3.1.0.dev0/setup.cfg
+-rw-rw-r--   0     1000     1000     2233 2024-05-20 12:02:06.000000 cfv-3.1.0.dev0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cfv-3.0.0.dev1/COPYING` & `cfv-3.1.0.dev0/COPYING`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/cfv.1` & `cfv-3.1.0.dev0/cfv.1`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/setup.py` & `cfv-3.1.0.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,32 +38,33 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Topic :: System :: Archiving',
         'Topic :: Utilities',
         'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13',
     ],
     keywords='cfv checksum verify sfv csv crc bsdmd5 md5sum sha1sum sha224sum sha256sum sha384sum sha512sum torrent par par2',
     project_urls={
         'Bug Tracker': 'https://github.com/cfv-project/cfv/issues',
         'Source Code': 'https://github.com/cfv-project/cfv',
         'Original Project': 'http://cfv.sourceforge.net/',
     },
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     include_package_data=True,
-    data_files=[('man/man1', ['cfv.1'])],
+    data_files=[('share/man/man1', ['cfv.1'])],
     entry_points={
         'console_scripts': [
             'cfv=cfv.common:main',
         ],
     },
 )
```

### Comparing `cfv-3.0.0.dev1/PKG-INFO` & `cfv-3.1.0.dev0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,27 @@
-Metadata-Version: 2.1
-Name: cfv
-Version: 3.0.0.dev1
-Summary: Command-line File Verify - versatile file checksum creator and verifier
-Home-page: https://github.com/cfv-project/cfv
-Author: David Gnedt (Current Maintainer)
-Author-email: cfv-project@davizone.at
-License: GPL
-Project-URL: Bug Tracker, https://github.com/cfv-project/cfv/issues
-Project-URL: Source Code, https://github.com/cfv-project/cfv
-Project-URL: Original Project, http://cfv.sourceforge.net/
-Keywords: cfv checksum verify sfv csv crc bsdmd5 md5sum sha1sum sha224sum sha256sum sha384sum sha512sum torrent par par2
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Topic :: System :: Archiving
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: COPYING
-
 # cfv – Command-line File Verify
 
 cfv is a utility to test and create a wide range of checksum verification files.
 It currently supports testing and creating sfv, sfvmd5, csv, csv2, csv4, md5, bsdmd5, sha1, sha224,
 sha256, sha384, sha512, torrent and crc files.
 Test-only support is available for par, par2.
 
 cfv was originally written by Matthew Mueller ([original project home](http://cfv.sourceforge.net/)).
 This is a [friendly fork of cfv](https://github.com/cfv-project/cfv) maintained by David Gnedt.
 
-[![Build Status](https://img.shields.io/github/checks-status/cfv-project/cfv/python3)](https://github.com/cfv-project/cfv/actions?query=branch%3Apython3)
+[![Build Status Linux](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml?query=branch%3Apython3)
+[![Build Status FreeBSD](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml?query=branch%3Apython3)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cfv.svg)](https://pypi.org/project/cfv/)
 [![License](https://img.shields.io/pypi/l/cfv.svg)](https://pypi.org/project/cfv/)
 [![Latest PyPI version](https://img.shields.io/pypi/v/cfv.svg)](https://pypi.org/project/cfv/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/cfv.svg)](https://pypi.org/project/cfv/)
 
 ## Requirements
 
-Python ≥ 3.5 – older versions might work, but are unsupported.
+Python ≥ 3.6 – older versions might work, but are unsupported.
 For Python 2 support, see the [python2 branch](https://github.com/cfv-project/cfv/tree/python2).
 
 ### Optional
 
 * [Python Imaging Library (PIL)](https://www.pythonware.com/products/pil/) or
   [Pillow](https://python-pillow.org/) – only needed if you want to create the
   dimensions column of .crc files.
@@ -59,27 +30,73 @@
 
 You can get the latest releases via the [Python Package Index (PyPI)](https://pypi.org/project/cfv/)
 or from the [Github releases page](https://github.com/cfv-project/cfv/releases).
 Other distribution ways are work-in-progress, see [issue #4](https://github.com/cfv-project/cfv/issues/4).
 
 ### From PyPI
 
-If you have a working Python installation with pip, you can follow these installation steps:
+If you have a working Python installation with pip, you can install via PyPI:
 
-1. `pip install cfv`
-2. read man page `man cfv` or read usage `cfv -h` and have fun ☺️
+```sh
+pip install cfv
+```
 
 ### From Source
 
 Download a snapshot from the [Github releases page](https://github.com/cfv-project/cfv/releases)
 or checkout the development version via Git.
 
-1. `python setup.py install`
-2. read man page `man cfv` or read usage `cfv -h` and have fun ☺️
-3. optional: run tests to verify correct operation: `cd test; ./test.py`
+```sh
+python setup.py install
+# optional: run tests to verify correct operation
+cd test; ./test.py
+```
+
+### From OS-specific Repositories
+
+#### Arch Linux
+
+To install the development version from [AUR](https://aur.archlinux.org/packages/cfv-git) (maintained by @vestingz):
+
+```sh
+yay -S cfv-git
+```
+
+#### FreeBSD
+
+A FreeBSD port is available (maintained by @Terry-Kennedy).
+
+To install the pre-built package (updated quarterly, so may be out-of-date):
+
+```sh
+pkg install cfv
+```
+
+To build from source (make sure your source tree is up-to-date via any of the usual methods):
+
+```sh
+cd /usr/ports/security/cfv
+make; make install; make clean
+```
+
+To update the pre-built package:
+
+```sh
+pkg upgrade cfv
+```
+
+To update from source (again, make sure your source tree is up-to-date):
+
+```sh
+portupgrade cfv
+```
+
+## Usage
+
+Please read the man page `man cfv` or the usage `cfv -h` and have fun ☺️
 
 ## Contributions
 
 Contributions are welcome, just open a pull request ☺️
 
 ## Alternative Tools
 
@@ -96,9 +113,7 @@
 ## Copying
 
 This program is free software; you can redistribute it and/or modify it under
 the terms of the GNU General Public License as published by the Free Software
 Foundation; either version 2 of the License, or (at your option) any later
 version.
 See the file `COPYING` for more information.
-
-
```

### Comparing `cfv-3.0.0.dev1/Changelog` & `cfv-3.1.0.dev0/Changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
-2022-10-30 - v3.0.0.dev1:
+2024-05-20 - v3.1.0.dev0:
 	* WARNING: This is a development snapshot, not a stable release.
+	* Drop support for Python 3.5.
+	* Python 3.6 is now the minimum supported version.
+	* Add support for Python 3.12 (Thanks to Louis Sautier).
+	* Add support for Python 3.13.
+	* Correctly close files in various situations.
+
+2022-10-30 - v3.0.0:
 	* Tested platforms: Linux and FreeBSD. If there is interest in supporting more platforms (e.g. OSX and Windows), please get in contact with the project.
 	* Support for Python 3 (Thanks to Steven Xu for major contributions).
 	* Python 3.5 is now the minimum supported version.
 	* Dropped fchksum support, as it does not support Python 3.
 
 2019-03-27 - v2.0.0:
 	* Now fully unicode aware.  Work is done internally in unicode, only translating to encoded form on input/output.
```

### Comparing `cfv-3.0.0.dev1/lib/cfv.egg-info/SOURCES.txt` & `cfv-3.1.0.dev0/lib/cfv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/lib/cfv.egg-info/PKG-INFO` & `cfv-3.1.0.dev0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
 Name: cfv
-Version: 3.0.0.dev1
+Version: 3.1.0.dev0
 Summary: Command-line File Verify - versatile file checksum creator and verifier
 Home-page: https://github.com/cfv-project/cfv
 Author: David Gnedt (Current Maintainer)
 Author-email: cfv-project@davizone.at
 License: GPL
 Project-URL: Bug Tracker, https://github.com/cfv-project/cfv/issues
 Project-URL: Source Code, https://github.com/cfv-project/cfv
 Project-URL: Original Project, http://cfv.sourceforge.net/
 Keywords: cfv checksum verify sfv csv crc bsdmd5 md5sum sha1sum sha224sum sha256sum sha384sum sha512sum torrent par par2
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # cfv – Command-line File Verify
 
 cfv is a utility to test and create a wide range of checksum verification files.
 It currently supports testing and creating sfv, sfvmd5, csv, csv2, csv4, md5, bsdmd5, sha1, sha224,
 sha256, sha384, sha512, torrent and crc files.
 Test-only support is available for par, par2.
 
 cfv was originally written by Matthew Mueller ([original project home](http://cfv.sourceforge.net/)).
 This is a [friendly fork of cfv](https://github.com/cfv-project/cfv) maintained by David Gnedt.
 
-[![Build Status](https://img.shields.io/github/checks-status/cfv-project/cfv/python3)](https://github.com/cfv-project/cfv/actions?query=branch%3Apython3)
+[![Build Status Linux](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml?query=branch%3Apython3)
+[![Build Status FreeBSD](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml?query=branch%3Apython3)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cfv.svg)](https://pypi.org/project/cfv/)
 [![License](https://img.shields.io/pypi/l/cfv.svg)](https://pypi.org/project/cfv/)
 [![Latest PyPI version](https://img.shields.io/pypi/v/cfv.svg)](https://pypi.org/project/cfv/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/cfv.svg)](https://pypi.org/project/cfv/)
 
 ## Requirements
 
-Python ≥ 3.5 – older versions might work, but are unsupported.
+Python ≥ 3.6 – older versions might work, but are unsupported.
 For Python 2 support, see the [python2 branch](https://github.com/cfv-project/cfv/tree/python2).
 
 ### Optional
 
 * [Python Imaging Library (PIL)](https://www.pythonware.com/products/pil/) or
   [Pillow](https://python-pillow.org/) – only needed if you want to create the
   dimensions column of .crc files.
@@ -59,27 +60,73 @@
 
 You can get the latest releases via the [Python Package Index (PyPI)](https://pypi.org/project/cfv/)
 or from the [Github releases page](https://github.com/cfv-project/cfv/releases).
 Other distribution ways are work-in-progress, see [issue #4](https://github.com/cfv-project/cfv/issues/4).
 
 ### From PyPI
 
-If you have a working Python installation with pip, you can follow these installation steps:
+If you have a working Python installation with pip, you can install via PyPI:
 
-1. `pip install cfv`
-2. read man page `man cfv` or read usage `cfv -h` and have fun ☺️
+```sh
+pip install cfv
+```
 
 ### From Source
 
 Download a snapshot from the [Github releases page](https://github.com/cfv-project/cfv/releases)
 or checkout the development version via Git.
 
-1. `python setup.py install`
-2. read man page `man cfv` or read usage `cfv -h` and have fun ☺️
-3. optional: run tests to verify correct operation: `cd test; ./test.py`
+```sh
+python setup.py install
+# optional: run tests to verify correct operation
+cd test; ./test.py
+```
+
+### From OS-specific Repositories
+
+#### Arch Linux
+
+To install the development version from [AUR](https://aur.archlinux.org/packages/cfv-git) (maintained by @vestingz):
+
+```sh
+yay -S cfv-git
+```
+
+#### FreeBSD
+
+A FreeBSD port is available (maintained by @Terry-Kennedy).
+
+To install the pre-built package (updated quarterly, so may be out-of-date):
+
+```sh
+pkg install cfv
+```
+
+To build from source (make sure your source tree is up-to-date via any of the usual methods):
+
+```sh
+cd /usr/ports/security/cfv
+make; make install; make clean
+```
+
+To update the pre-built package:
+
+```sh
+pkg upgrade cfv
+```
+
+To update from source (again, make sure your source tree is up-to-date):
+
+```sh
+portupgrade cfv
+```
+
+## Usage
+
+Please read the man page `man cfv` or the usage `cfv -h` and have fun ☺️
 
 ## Contributions
 
 Contributions are welcome, just open a pull request ☺️
 
 ## Alternative Tools
 
@@ -96,9 +143,7 @@
 ## Copying
 
 This program is free software; you can redistribute it and/or modify it under
 the terms of the GNU General Public License as published by the Free Software
 Foundation; either version 2 of the License, or (at your option) any later
 version.
 See the file `COPYING` for more information.
-
-
```

### Comparing `cfv-3.0.0.dev1/lib/cfv/osutil.py` & `cfv-3.1.0.dev0/lib/cfv/osutil.py`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/lib/cfv/common.py` & `cfv-3.1.0.dev0/lib/cfv/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 from __future__ import print_function
 
 from builtins import map
 from builtins import object
 from builtins import range
 from builtins import str
 
-__version__ = '3.0.0.dev1'
+__version__ = '3.1.0.dev0'
 __homepage__ = 'https://github.com/cfv-project/cfv'
 
+import contextlib
 import copy
 import errno
 import getopt
 import os
 import re
 import struct
 import sys
@@ -462,16 +463,14 @@
 
 class ChksumType(object):
     def test_chksumfile(self, file, filename):
         if config.showunverified:  # we can't expect the checksum file itself to be checksummed
             cache.set_verified(filename)
         try:
             cf_stats = stats.make_sub_stats()
-            if not file:
-                file = fileutil.open_read(filename, config)
             self.do_test_chksumfile(file)
             cf_stats.sub_stats_end(stats)
             view.ev_test_cf_done(filename, cf_stats)
         except EnvironmentError as a:
             stats.cferror += 1
             view.ev_cf_enverror(filename, a)
 
@@ -1528,16 +1527,16 @@
 # ---------- jpegsheriff .crc ----------
 
 def getimagedimensions(filename):
     if filename == '':
         return '0', '0'
     try:
         from PIL import Image
-        im1 = Image.open(filename)
-        return list(map(str, im1.size))
+        with Image.open(filename) as im1:
+            return list(map(str, im1.size))
     except (ImportError, IOError):
         return '0', '0'
 
 
 def commaize(n):
     n = '%d' % n
     s = n[-3:]
@@ -1690,34 +1689,41 @@
                 return 0
             _visited_dirs.add(dir_key)
         return 1
     return 0
 
 
 def test(filename, typename, restrict_typename='auto'):
-    if typename != 'auto':
-        cf = cftypes.get_handler(typename)()
-        cf.test_chksumfile(None, filename)
-        return
+    class UnexpectedHandlerException(Exception):
+        pass
 
-    try:
-        file = fileutil.open_read(filename, config)
+    def get_cf_handler(file, typename, restrict_typename):
+        if typename != 'auto':
+            return cftypes.get_handler(typename)()
         cftype = cftypes.auto_chksumfile_match(file)
         if restrict_typename != 'auto' and cftypes.get_handler(restrict_typename) != cftype:
-            return
+            raise UnexpectedHandlerException()
         if cftype:
-            cf = cftype()
+            return cftype()
+
+    try:
+        with contextlib.closing(fileutil.open_read(filename, config)) as file:
+            cf = get_cf_handler(file, typename, restrict_typename)
+            if not cf:
+                view.ev_test_cf_unrecognized(filename, file._decode_errs)
+                stats.cferror += 1
+                return
+
             cf.test_chksumfile(file, filename)
-            return
+    except UnexpectedHandlerException:
+        return
     except EnvironmentError as a:
         stats.cferror += 1
         view.ev_cf_enverror(filename, a)
         return -1
-    view.ev_test_cf_unrecognized(filename, file._decode_errs)
-    stats.cferror += 1
 
 
 def make(cftype, ifilename, testfiles):
     file = None
     if ifilename:
         filename = ifilename
     else:
```

### Comparing `cfv-3.0.0.dev1/lib/cfv/BitTorrent/bencode.py` & `cfv-3.1.0.dev0/lib/cfv/BitTorrent/bencode.py`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/lib/cfv/BitTorrent/LICENSE.txt` & `cfv-3.1.0.dev0/lib/cfv/BitTorrent/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/lib/cfv/hash.py` & `cfv-3.1.0.dev0/lib/cfv/hash.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,35 +41,39 @@
             if not x:
                 return m.digest(), s
             s += len(x)
             m.update(x)
             if callback:
                 callback(s)
 
-    if f == sys.stdin.buffer or _nommap or callback:
-        return finish(hasher(), 0)
-    else:
-        s = os.path.getsize(filename)
-        try:
-            if s > _MAX_MMAP:
-                # Work around python 2.[56] problem with md5 of large mmap objects
-                raise OverflowError
-            m = hasher(dommap(f.fileno(), s))
-        except OverflowError:
-            # mmap size is limited by C's int type, which even on 64 bit
-            # arches is often 32 bits, so we can't use sys.maxint
-            # either.  If we get the error, just assume 32 bits.
-            mmapsize = min(s, _FALLBACK_MMAP)
-            m = hasher(dommap(f.fileno(), mmapsize))
-            f.seek(mmapsize)
-            # unfortunatly, python's mmap module doesn't support the
-            # offset parameter, so we just have to do the rest of the
-            # file the old fashioned way.
-            return finish(m, mmapsize)
-        return m.digest(), s
+    try:
+        if f == sys.stdin.buffer or _nommap or callback:
+            return finish(hasher(), 0)
+        else:
+            s = os.path.getsize(filename)
+            try:
+                if s > _MAX_MMAP:
+                    # Work around python 2.[56] problem with md5 of large mmap objects
+                    raise OverflowError
+                m = hasher(dommap(f.fileno(), s))
+            except OverflowError:
+                # mmap size is limited by C's int type, which even on 64 bit
+                # arches is often 32 bits, so we can't use sys.maxint
+                # either.  If we get the error, just assume 32 bits.
+                mmapsize = min(s, _FALLBACK_MMAP)
+                m = hasher(dommap(f.fileno(), mmapsize))
+                f.seek(mmapsize)
+                # unfortunatly, python's mmap module doesn't support the
+                # offset parameter, so we just have to do the rest of the
+                # file the old fashioned way.
+                return finish(m, mmapsize)
+            return m.digest(), s
+    finally:
+        if filename != '':
+            f.close()
 
 
 def getfilechecksumgeneric(algo):
     if hasattr(hashlib, algo):
         hasher = getattr(hashlib, algo)
     else:
         def hasher():
```

### Comparing `cfv-3.0.0.dev1/lib/cfv/strutil.py` & `cfv-3.1.0.dev0/lib/cfv/strutil.py`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/lib/cfv/progress.py` & `cfv-3.1.0.dev0/lib/cfv/progress.py`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/lib/cfv/fileutil.py` & `cfv-3.1.0.dev0/lib/cfv/fileutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,27 +100,31 @@
         self.peeknextline = None
         self.peekdecoded = None
         self.peekline = None
         self.peek = None
         self.readline = self._readline
         self.read = fileobj.read
         self.seek = fileobj.seek
+        self.close = fileobj.close
 
     def seek(self, *args):
         self._done_peeking(raw=1)
         return self.seek(*args)
 
     def readline(self, *args):
         self._done_peeking(raw=0)
         return self._readline(*args)
 
     def read(self, *args):
         self._done_peeking(raw=1)
         return self.read(*args)
 
+    def close(self):
+        self.fileobj.close()
+
 
 def PeekFileNonseekable(fileobj, filename, encoding):
     return PeekFile(BytesIO(fileobj.read()), filename, encoding)
 
 
 def PeekFileGzip(filename, encoding):
     import gzip
```

### Comparing `cfv-3.0.0.dev1/lib/cfv/cftypes.py` & `cfv-3.1.0.dev0/lib/cfv/cftypes.py`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/lib/cfv/term.py` & `cfv-3.1.0.dev0/lib/cfv/term.py`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/lib/cfv/ui.py` & `cfv-3.1.0.dev0/lib/cfv/ui.py`

 * *Files identical despite different names*

### Comparing `cfv-3.0.0.dev1/lib/cfv/caching.py` & `cfv-3.1.0.dev0/lib/cfv/caching.py`

 * *Files identical despite different names*

