# Comparing `tmp/cfv-3.1.0.tar.gz` & `tmp/cfv-3.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfv-3.1.0.tar", last modified: Mon May 20 15:46:40 2024, max compression
+gzip compressed data, was "cfv-3.1.0.dev0.tar", last modified: Mon May 20 14:05:07 2024, max compression
```

## Comparing `cfv-3.1.0.tar` & `cfv-3.1.0.dev0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0     1000     1000        0 2024-05-20 15:46:40.675437 cfv-3.1.0/
--rw-rw-r--   0     1000     1000    17992 2018-03-13 00:55:28.000000 cfv-3.1.0/COPYING
--rw-rw-r--   0     1000     1000    12490 2024-05-20 15:24:10.000000 cfv-3.1.0/Changelog
--rw-rw-r--   0     1000     1000      146 2021-10-29 01:02:50.000000 cfv-3.1.0/MANIFEST.in
--rw-r--r--   0     1000     1000     5651 2024-05-20 15:46:40.675437 cfv-3.1.0/PKG-INFO
--rw-rw-r--   0     1000     1000     4283 2024-05-20 14:56:39.000000 cfv-3.1.0/README.md
--rw-rw-r--   0     1000     1000    13105 2024-05-20 14:56:05.000000 cfv-3.1.0/cfv.1
-drwxr-xr-x   0     1000     1000        0 2024-05-20 15:46:40.651437 cfv-3.1.0/lib/
-drwxr-xr-x   0     1000     1000        0 2024-05-20 15:46:40.667437 cfv-3.1.0/lib/cfv/
-drwxr-xr-x   0     1000     1000        0 2024-05-20 15:46:40.671437 cfv-3.1.0/lib/cfv/BitTorrent/
--rw-rw-r--   0     1000     1000     1182 2018-03-13 02:17:59.000000 cfv-3.1.0/lib/cfv/BitTorrent/LICENSE.txt
--rw-rw-r--   0     1000     1000        0 2018-03-13 02:17:59.000000 cfv-3.1.0/lib/cfv/BitTorrent/__init__.py
--rw-rw-r--   0     1000     1000     6815 2022-10-28 22:11:18.000000 cfv-3.1.0/lib/cfv/BitTorrent/bencode.py
--rw-rw-r--   0     1000     1000     3830 2024-05-16 02:03:45.000000 cfv-3.1.0/lib/cfv/BitTorrent/btformats.py
--rw-rw-r--   0     1000     1000        0 2018-03-13 02:17:59.000000 cfv-3.1.0/lib/cfv/__init__.py
--rw-rw-r--   0     1000     1000     5155 2021-10-29 01:02:50.000000 cfv-3.1.0/lib/cfv/caching.py
--rw-rw-r--   0     1000     1000     1543 2021-10-29 01:02:50.000000 cfv-3.1.0/lib/cfv/cftypes.py
--rw-rw-r--   0     1000     1000    81524 2024-05-20 15:23:33.000000 cfv-3.1.0/lib/cfv/common.py
--rw-rw-r--   0     1000     1000     5672 2024-05-20 12:02:06.000000 cfv-3.1.0/lib/cfv/fileutil.py
--rw-rw-r--   0     1000     1000     2676 2024-05-20 12:02:06.000000 cfv-3.1.0/lib/cfv/hash.py
--rw-rw-r--   0     1000     1000     3291 2022-10-28 22:11:18.000000 cfv-3.1.0/lib/cfv/osutil.py
--rw-rw-r--   0     1000     1000     3429 2021-10-29 01:02:50.000000 cfv-3.1.0/lib/cfv/progress.py
--rw-rw-r--   0     1000     1000     2943 2022-10-28 22:11:18.000000 cfv-3.1.0/lib/cfv/strutil.py
--rw-r--r--   0     1000     1000      691 2019-03-24 20:41:28.000000 cfv-3.1.0/lib/cfv/term.py
--rw-rw-r--   0     1000     1000     7149 2021-10-29 01:02:50.000000 cfv-3.1.0/lib/cfv/ui.py
-drwxr-xr-x   0     1000     1000        0 2024-05-20 15:46:40.675437 cfv-3.1.0/lib/cfv.egg-info/
--rw-r--r--   0     1000     1000     5651 2024-05-20 15:46:40.000000 cfv-3.1.0/lib/cfv.egg-info/PKG-INFO
--rw-r--r--   0     1000     1000      535 2024-05-20 15:46:40.000000 cfv-3.1.0/lib/cfv.egg-info/SOURCES.txt
--rw-r--r--   0     1000     1000        1 2024-05-20 15:46:40.000000 cfv-3.1.0/lib/cfv.egg-info/dependency_links.txt
--rw-r--r--   0     1000     1000       40 2024-05-20 15:46:40.000000 cfv-3.1.0/lib/cfv.egg-info/entry_points.txt
--rw-r--r--   0     1000     1000        4 2024-05-20 15:46:40.000000 cfv-3.1.0/lib/cfv.egg-info/top_level.txt
--rw-r--r--   0     1000     1000       38 2024-05-20 15:46:40.675437 cfv-3.1.0/setup.cfg
--rw-rw-r--   0     1000     1000     2238 2024-05-20 14:52:02.000000 cfv-3.1.0/setup.py
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

### Comparing `cfv-3.1.0/COPYING` & `cfv-3.1.0.dev0/COPYING`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/Changelog` & `cfv-3.1.0.dev0/Changelog`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-2024-05-20 - v3.1.0:
+2024-05-20 - v3.1.0.dev0:
+	* WARNING: This is a development snapshot, not a stable release.
 	* Drop support for Python 3.5.
 	* Python 3.6 is now the minimum supported version.
 	* Add support for Python 3.12 (Thanks to Louis Sautier).
 	* Add support for Python 3.13.
 	* Correctly close files in various situations.
 
 2022-10-30 - v3.0.0:
```

### Comparing `cfv-3.1.0/PKG-INFO` & `cfv-3.1.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cfv
-Version: 3.1.0
+Version: 3.1.0.dev0
 Summary: Command-line File Verify - versatile file checksum creator and verifier
 Home-page: https://github.com/cfv-project/cfv
-Author: David Lisa Gnedt (Current Maintainer)
+Author: David Gnedt (Current Maintainer)
 Author-email: cfv-project@davizone.at
 License: GPL
 Project-URL: Bug Tracker, https://github.com/cfv-project/cfv/issues
 Project-URL: Source Code, https://github.com/cfv-project/cfv
 Project-URL: Original Project, http://cfv.sourceforge.net/
 Keywords: cfv checksum verify sfv csv crc bsdmd5 md5sum sha1sum sha224sum sha256sum sha384sum sha512sum torrent par par2
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,15 +32,15 @@
 
 cfv is a utility to test and create a wide range of checksum verification files.
 It currently supports testing and creating sfv, sfvmd5, csv, csv2, csv4, md5, bsdmd5, sha1, sha224,
 sha256, sha384, sha512, torrent and crc files.
 Test-only support is available for par, par2.
 
 cfv was originally written by Matthew Mueller ([original project home](http://cfv.sourceforge.net/)).
-This is a [friendly fork of cfv](https://github.com/cfv-project/cfv) maintained by David Lisa Gnedt.
+This is a [friendly fork of cfv](https://github.com/cfv-project/cfv) maintained by David Gnedt.
 
 [![Build Status Linux](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml?query=branch%3Apython3)
 [![Build Status FreeBSD](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml?query=branch%3Apython3)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cfv.svg)](https://pypi.org/project/cfv/)
 [![License](https://img.shields.io/pypi/l/cfv.svg)](https://pypi.org/project/cfv/)
 [![Latest PyPI version](https://img.shields.io/pypi/v/cfv.svg)](https://pypi.org/project/cfv/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/cfv.svg)](https://pypi.org/project/cfv/)
```

### Comparing `cfv-3.1.0/README.md` & `cfv-3.1.0.dev0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 cfv is a utility to test and create a wide range of checksum verification files.
 It currently supports testing and creating sfv, sfvmd5, csv, csv2, csv4, md5, bsdmd5, sha1, sha224,
 sha256, sha384, sha512, torrent and crc files.
 Test-only support is available for par, par2.
 
 cfv was originally written by Matthew Mueller ([original project home](http://cfv.sourceforge.net/)).
-This is a [friendly fork of cfv](https://github.com/cfv-project/cfv) maintained by David Lisa Gnedt.
+This is a [friendly fork of cfv](https://github.com/cfv-project/cfv) maintained by David Gnedt.
 
 [![Build Status Linux](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml?query=branch%3Apython3)
 [![Build Status FreeBSD](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml?query=branch%3Apython3)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cfv.svg)](https://pypi.org/project/cfv/)
 [![License](https://img.shields.io/pypi/l/cfv.svg)](https://pypi.org/project/cfv/)
 [![Latest PyPI version](https://img.shields.io/pypi/v/cfv.svg)](https://pypi.org/project/cfv/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/cfv.svg)](https://pypi.org/project/cfv/)
```

### Comparing `cfv-3.1.0/cfv.1` & `cfv-3.1.0.dev0/cfv.1`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
 Where to look for cfvrc file.
 Note that win9x doesn't set this to anything automatically.
 .IP "CFV_NOMMAP"
 Set to a non-empty value to disable usage of mmap.
 .SH AUTHOR
 Matthew Mueller <donut AT dakotacom DOT net>
 .br
-David Lisa Gnedt <cfv-project AT davizone DOT at>
+David Gnedt <cfv-project AT davizone DOT at>
 .P
 The latest version can be found at:
 .br
 https://github.com/cfv-project/cfv
 .P
 The original project can be found at:
 .br
```

### Comparing `cfv-3.1.0/lib/cfv/BitTorrent/LICENSE.txt` & `cfv-3.1.0.dev0/lib/cfv/BitTorrent/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/BitTorrent/bencode.py` & `cfv-3.1.0.dev0/lib/cfv/BitTorrent/bencode.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/BitTorrent/btformats.py` & `cfv-3.1.0.dev0/lib/cfv/BitTorrent/btformats.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/caching.py` & `cfv-3.1.0.dev0/lib/cfv/caching.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/cftypes.py` & `cfv-3.1.0.dev0/lib/cfv/cftypes.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/common.py` & `cfv-3.1.0.dev0/lib/cfv/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 #    cfv - Command-line File Verify
 #    Copyright (C) 2000-2013  Matthew Mueller <donut AT dakotacom DOT net>
-#    Copyright (C) 2018-2024  David Lisa Gnedt <cfv-project AT davizone DOT at>
+#    Copyright (C) 2018-2022  David Gnedt <cfv-project AT davizone DOT at>
 #
 #    This program is free software; you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation; either version 2 of the License, or
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
@@ -22,15 +22,15 @@
 from __future__ import print_function
 
 from builtins import map
 from builtins import object
 from builtins import range
 from builtins import str
 
-__version__ = '3.1.0'
+__version__ = '3.1.0.dev0'
 __homepage__ = 'https://github.com/cfv-project/cfv'
 
 import contextlib
 import copy
 import errno
 import getopt
 import os
@@ -2007,15 +2007,15 @@
     phelp(' --announceurl=URL    tracker announce url')
     phelp(' --piece_size_pow2=N  power of two to set the piece size to (default 18)')
     phelp(' --private_torrent    set private flag in torrent')
     sys.exit(err)
 
 
 def printhelp():
-    view.pinfo('cfv v%s - Copyright (C) 2000-2013 Matthew Mueller - Copyright (C) 2018-2024 David Lisa Gnedt - GPL license' % __version__)
+    view.pinfo('cfv v%s - Copyright (C) 2000-2013 Matthew Mueller - Copyright (C) 2018-2022 David Gnedt - GPL license' % __version__)
     printusage()
 
 
 def printcftypehelp(err):
     phelp = err and view.perror or view.pinfo
     phelp('Valid types:')
```

### Comparing `cfv-3.1.0/lib/cfv/fileutil.py` & `cfv-3.1.0.dev0/lib/cfv/fileutil.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/hash.py` & `cfv-3.1.0.dev0/lib/cfv/hash.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/osutil.py` & `cfv-3.1.0.dev0/lib/cfv/osutil.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/progress.py` & `cfv-3.1.0.dev0/lib/cfv/progress.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/strutil.py` & `cfv-3.1.0.dev0/lib/cfv/strutil.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/term.py` & `cfv-3.1.0.dev0/lib/cfv/term.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv/ui.py` & `cfv-3.1.0.dev0/lib/cfv/ui.py`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/lib/cfv.egg-info/PKG-INFO` & `cfv-3.1.0.dev0/lib/cfv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cfv
-Version: 3.1.0
+Version: 3.1.0.dev0
 Summary: Command-line File Verify - versatile file checksum creator and verifier
 Home-page: https://github.com/cfv-project/cfv
-Author: David Lisa Gnedt (Current Maintainer)
+Author: David Gnedt (Current Maintainer)
 Author-email: cfv-project@davizone.at
 License: GPL
 Project-URL: Bug Tracker, https://github.com/cfv-project/cfv/issues
 Project-URL: Source Code, https://github.com/cfv-project/cfv
 Project-URL: Original Project, http://cfv.sourceforge.net/
 Keywords: cfv checksum verify sfv csv crc bsdmd5 md5sum sha1sum sha224sum sha256sum sha384sum sha512sum torrent par par2
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,15 +32,15 @@
 
 cfv is a utility to test and create a wide range of checksum verification files.
 It currently supports testing and creating sfv, sfvmd5, csv, csv2, csv4, md5, bsdmd5, sha1, sha224,
 sha256, sha384, sha512, torrent and crc files.
 Test-only support is available for par, par2.
 
 cfv was originally written by Matthew Mueller ([original project home](http://cfv.sourceforge.net/)).
-This is a [friendly fork of cfv](https://github.com/cfv-project/cfv) maintained by David Lisa Gnedt.
+This is a [friendly fork of cfv](https://github.com/cfv-project/cfv) maintained by David Gnedt.
 
 [![Build Status Linux](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3.yml?query=branch%3Apython3)
 [![Build Status FreeBSD](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml/badge.svg?branch=python3)](https://github.com/cfv-project/cfv/actions/workflows/ci-python3-freebsd.yml?query=branch%3Apython3)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cfv.svg)](https://pypi.org/project/cfv/)
 [![License](https://img.shields.io/pypi/l/cfv.svg)](https://pypi.org/project/cfv/)
 [![Latest PyPI version](https://img.shields.io/pypi/v/cfv.svg)](https://pypi.org/project/cfv/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/cfv.svg)](https://pypi.org/project/cfv/)
```

### Comparing `cfv-3.1.0/lib/cfv.egg-info/SOURCES.txt` & `cfv-3.1.0.dev0/lib/cfv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfv-3.1.0/setup.py` & `cfv-3.1.0.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 setup(
     name='cfv',
     version=version,
     description='Command-line File Verify - versatile file checksum creator and verifier',
     long_description=_read('README.md'),
     long_description_content_type='text/markdown',
     url='https://github.com/cfv-project/cfv',
-    author='David Lisa Gnedt (Current Maintainer)',
+    author='David Gnedt (Current Maintainer)',
     author_email='%s@%s' % ('cfv-project', 'davizone.at'),
     license='GPL',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Topic :: System :: Archiving',
         'Topic :: Utilities',
```

