# Comparing `tmp/pacroller-0.1.8.tar.gz` & `tmp/pacroller-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacroller-0.1.8.tar", last modified: Sun Sep  3 07:17:56 2023, max compression
+gzip compressed data, was "pacroller-0.1.9.tar", last modified: Mon May 20 08:53:33 2024, max compression
```

## Comparing `pacroller-0.1.8.tar` & `pacroller-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-09-03 07:17:56.796162 pacroller-0.1.8/
--rw-r--r--   0 jerry     (1000) users      (100)    35141 2023-09-03 07:14:38.000000 pacroller-0.1.8/LICENSE
--rw-r--r--   0 jerry     (1000) users      (100)     3714 2023-09-03 07:17:56.796162 pacroller-0.1.8/PKG-INFO
--rw-r--r--   0 jerry     (1000) users      (100)     3204 2023-09-03 07:14:38.000000 pacroller-0.1.8/README.md
--rw-r--r--   0 jerry     (1000) users      (100)       38 2023-09-03 07:17:56.796162 pacroller-0.1.8/setup.cfg
--rw-r--r--   0 jerry     (1000) users      (100)      974 2023-09-03 07:15:39.000000 pacroller-0.1.8/setup.py
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-09-03 07:17:56.792829 pacroller-0.1.8/src/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-09-03 07:17:56.796162 pacroller-0.1.8/src/pacroller/
--rw-r--r--   0 jerry     (1000) users      (100)        0 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/__init__.py
--rw-r--r--   0 jerry     (1000) users      (100)     4426 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/analyze.py
--rw-r--r--   0 jerry     (1000) users      (100)    12794 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/checker.py
--rw-r--r--   0 jerry     (1000) users      (100)     4078 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/config.py
--rw-r--r--   0 jerry     (1000) users      (100)     4298 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/known_output.py
--rw-r--r--   0 jerry     (1000) users      (100)      103 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/known_output_override.py
--rw-r--r--   0 jerry     (1000) users      (100)     3385 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/mailer.py
--rw-r--r--   0 jerry     (1000) users      (100)    16561 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/main.py
--rw-r--r--   0 jerry     (1000) users      (100)     1174 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/news.py
--rw-r--r--   0 jerry     (1000) users      (100)     1873 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/update-merge-config.py
--rw-r--r--   0 jerry     (1000) users      (100)     6610 2023-09-03 07:14:38.000000 pacroller-0.1.8/src/pacroller/utils.py
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-09-03 07:17:56.796162 pacroller-0.1.8/src/pacroller.egg-info/
--rw-r--r--   0 jerry     (1000) users      (100)     3714 2023-09-03 07:17:56.000000 pacroller-0.1.8/src/pacroller.egg-info/PKG-INFO
--rw-r--r--   0 jerry     (1000) users      (100)      547 2023-09-03 07:17:56.000000 pacroller-0.1.8/src/pacroller.egg-info/SOURCES.txt
--rw-r--r--   0 jerry     (1000) users      (100)        1 2023-09-03 07:17:56.000000 pacroller-0.1.8/src/pacroller.egg-info/dependency_links.txt
--rw-r--r--   0 jerry     (1000) users      (100)       93 2023-09-03 07:17:56.000000 pacroller-0.1.8/src/pacroller.egg-info/entry_points.txt
--rw-r--r--   0 jerry     (1000) users      (100)        7 2023-09-03 07:17:56.000000 pacroller-0.1.8/src/pacroller.egg-info/requires.txt
--rw-r--r--   0 jerry     (1000) users      (100)       10 2023-09-03 07:17:56.000000 pacroller-0.1.8/src/pacroller.egg-info/top_level.txt
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2024-05-20 08:53:33.724868 pacroller-0.1.9/
+-rw-r--r--   0 jerry     (1000) users      (100)    35141 2021-01-15 15:27:56.000000 pacroller-0.1.9/LICENSE
+-rw-r--r--   0 jerry     (1000) users      (100)     3737 2024-05-20 08:53:33.724868 pacroller-0.1.9/PKG-INFO
+-rw-r--r--   0 jerry     (1000) users      (100)     3204 2023-08-22 06:37:54.000000 pacroller-0.1.9/README.md
+-rw-r--r--   0 jerry     (1000) users      (100)       38 2024-05-20 08:53:33.724868 pacroller-0.1.9/setup.cfg
+-rw-r--r--   0 jerry     (1000) users      (100)      975 2024-05-20 08:49:56.000000 pacroller-0.1.9/setup.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2024-05-20 08:53:33.721534 pacroller-0.1.9/src/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2024-05-20 08:53:33.724868 pacroller-0.1.9/src/pacroller/
+-rw-r--r--   0 jerry     (1000) users      (100)        0 2021-01-14 10:49:43.000000 pacroller-0.1.9/src/pacroller/__init__.py
+-rw-r--r--   0 jerry     (1000) users      (100)     4426 2021-10-11 07:38:47.000000 pacroller-0.1.9/src/pacroller/analyze.py
+-rw-r--r--   0 jerry     (1000) users      (100)    12800 2024-04-08 05:03:48.000000 pacroller-0.1.9/src/pacroller/checker.py
+-rw-r--r--   0 jerry     (1000) users      (100)     4078 2023-08-22 06:37:54.000000 pacroller-0.1.9/src/pacroller/config.py
+-rw-r--r--   0 jerry     (1000) users      (100)     4456 2024-05-04 06:07:59.000000 pacroller-0.1.9/src/pacroller/known_output.py
+-rw-r--r--   0 jerry     (1000) users      (100)      103 2021-02-09 03:43:35.000000 pacroller-0.1.9/src/pacroller/known_output_override.py
+-rw-r--r--   0 jerry     (1000) users      (100)     3385 2023-08-22 06:37:54.000000 pacroller-0.1.9/src/pacroller/mailer.py
+-rw-r--r--   0 jerry     (1000) users      (100)    16687 2024-01-22 15:38:17.000000 pacroller-0.1.9/src/pacroller/main.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1174 2023-08-22 06:37:54.000000 pacroller-0.1.9/src/pacroller/news.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1873 2021-04-23 05:11:11.000000 pacroller-0.1.9/src/pacroller/update-merge-config.py
+-rw-r--r--   0 jerry     (1000) users      (100)     6663 2024-04-28 13:56:36.000000 pacroller-0.1.9/src/pacroller/utils.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2024-05-20 08:53:33.724868 pacroller-0.1.9/src/pacroller.egg-info/
+-rw-r--r--   0 jerry     (1000) users      (100)     3737 2024-05-20 08:53:33.000000 pacroller-0.1.9/src/pacroller.egg-info/PKG-INFO
+-rw-r--r--   0 jerry     (1000) users      (100)      547 2024-05-20 08:53:33.000000 pacroller-0.1.9/src/pacroller.egg-info/SOURCES.txt
+-rw-r--r--   0 jerry     (1000) users      (100)        1 2024-05-20 08:53:33.000000 pacroller-0.1.9/src/pacroller.egg-info/dependency_links.txt
+-rw-r--r--   0 jerry     (1000) users      (100)       93 2024-05-20 08:53:33.000000 pacroller-0.1.9/src/pacroller.egg-info/entry_points.txt
+-rw-r--r--   0 jerry     (1000) users      (100)        7 2024-05-20 08:53:33.000000 pacroller-0.1.9/src/pacroller.egg-info/requires.txt
+-rw-r--r--   0 jerry     (1000) users      (100)       10 2024-05-20 08:53:33.000000 pacroller-0.1.9/src/pacroller.egg-info/top_level.txt
```

### Comparing `pacroller-0.1.8/LICENSE` & `pacroller-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pacroller-0.1.8/PKG-INFO` & `pacroller-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pacroller
-Version: 0.1.8
+Version: 0.1.9
 Summary: unattended upgrade for archlinux
 Home-page: https://github.com/isjerryxiao/pacroller
 Author: Jerry Xiao
 Author-email: pacroller@mail.jerryxiao.cc
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyalpm
 
 # Pacroller
 The "Unattended Upgrades" for Arch Linux.
 
 ## Concept
 Parsing the output of pacman and pacman.log, searching for known patterns and notifying the user whether there is a potential error.
 Currently the design is regex-based, any output that is unable to match a set of regex is reported back to the user.
```

### Comparing `pacroller-0.1.8/README.md` & `pacroller-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pacroller-0.1.8/setup.py` & `pacroller-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pacroller",
-    version="0.1.8",
+    version="0.1.9",
     author="Jerry Xiao",
     author_email="pacroller@mail.jerryxiao.cc",
     description="unattended upgrade for archlinux",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/isjerryxiao/pacroller",
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: POSIX :: Linux",
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.12',
     entry_points={
         'console_scripts': [
             'pacroller=pacroller.main:main',
             'pacroller-analyze=pacroller.analyze:main'
         ]
     },
     install_requires=['pyalpm']
```

### Comparing `pacroller-0.1.8/src/pacroller/analyze.py` & `pacroller-0.1.9/src/pacroller/analyze.py`

 * *Files identical despite different names*

### Comparing `pacroller-0.1.8/src/pacroller/checker.py` & `pacroller-0.1.9/src/pacroller/checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
         elif source == 'ALPM-SCRIPTLET':
             (_sourcem1, _, _pmsg) = _split_log_line(log[ln-1])
             for action in {'upgrade', 'install', 'remove', 'downgrade', 'reinstall'}:
                 if _m := REGEX[f"l_{action}"].match(_pmsg):
                     pkg, *_ = _m.groups()
                     break
             else:
-                report.crit(f'[NOM-SCRIPTLET] {_pmsg}')
+                report.crit(f'[NOM-SCRIPTLET] {msg} {_pmsg}')
                 ln += 1
                 action = 'unknown'
                 continue
             logger.debug(f'.install start {pkg=} {action=}')
             while True:
                 line = log[ln]
                 (_, source, msg) = _split_log_line(line)
```

### Comparing `pacroller-0.1.8/src/pacroller/config.py` & `pacroller-0.1.9/src/pacroller/config.py`

 * *Files identical despite different names*

### Comparing `pacroller-0.1.8/src/pacroller/known_output.py` & `pacroller-0.1.9/src/pacroller/known_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,33 @@
     ],
     '90-mkinitcpio-install.hook': [
         r'==> Building image from preset: .+',
         r'==> Starting build: .+',
         r'==> WARNING: Possibly missing firmware for module: .+',
         r'==> Generating module dependencies',
         r'==> Creating (?:.+)-compressed initcpio image: .+',
-        r'==> Image generation successful.*',
+        r'==> Initcpio image generation successful',
         r'[ ]+-> .+',
         r'ssh-.* .*',
-        r'==> Using default configuration file: \'/etc/mkinitcpio\.conf\'',
+        r'==> Using configuration file: .+',
+        r'==> Using default configuration file: .+',
         r'==> WARNING: consolefont: no font found in configuration',
+        r'==> Decompressing (?:.+)-compressed firmware files',
     ],
     '70-dkms-install.hook': [
         r'==> dkms install --no-depmod [^ ]+ -k [^ ]+',
         r'==> depmod [^ ]+',
     ],
     '71-dkms-remove.hook': [
+        r'==> dkms remove [^ ]+',
         r'==> dkms remove --no-depmod [^ ]+ -k [^ ]+',
         r'==> depmod [^ ]+',
     ],
     '70-dkms-upgrade.hook': [
+        r'==> dkms remove [^ ]+',
         r'==> dkms remove --no-depmod [^ ]+ -k [^ ]+',
         r'==> depmod [^ ]+',
     ],
     '90-update-appstream-cache.hook': [
         r'✔ Metadata cache was updated successfully\.',
     ],
     **KNOWN_HOOK_OUTPUT_OVERRIDE
@@ -94,16 +98,16 @@
         {'action': ['upgrade'], 'regex': r'==> first time you run it as your normal user\. Just start it and have fun!'},
     ],
     'grub': [
         {'action': ['upgrade'], 'regex': r':: To use the new features provided in this GRUB update, it is recommended'},
         {'action': ['upgrade'], 'regex': r'   to install it to the MBR or UEFI\. Due to potential configuration'},
         {'action': ['upgrade'], 'regex': r'   incompatibilities, it is advised to run both, installation and generation'},
         {'action': ['upgrade'], 'regex': r'   of configuration:'},
-        {'action': ['upgrade'], 'regex': r'     \$ grub-install \.\.\.'},
-        {'action': ['upgrade'], 'regex': r'     \$ grub-mkconfig -o /boot/grub/grub\.cfg'},
+        {'action': ['upgrade'], 'regex': r'     # grub-install \.\.\.'},
+        {'action': ['upgrade'], 'regex': r'     # grub-mkconfig -o /boot/grub/grub\.cfg'},
     ],
     'nvidia-utils': [
         {'action': ['upgrade'], 'regex': r'If you run into trouble with CUDA not being available, run nvidia-modprobe first\.'},
         {'action': ['upgrade'], 'regex': r'If you use GDM on Wayland, you might have to run systemctl enable --now nvidia-resume\.service'},
     ],
     **KNOWN_PACKAGE_OUTPUT_OVERRIDE
 }
```

### Comparing `pacroller-0.1.8/src/pacroller/mailer.py` & `pacroller-0.1.9/src/pacroller/mailer.py`

 * *Files identical despite different names*

### Comparing `pacroller-0.1.8/src/pacroller/main.py` & `pacroller-0.1.9/src/pacroller/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,22 +254,25 @@
                             stderr=subprocess.DEVNULL,
                             encoding='utf-8',
                             timeout=20,
                             check=True
         )
         locales = [l.lower() for l in p.stdout.strip().split('\n')]
         preferred = ['en_US.UTF-8', 'C.UTF-8']
+        env_vars = ['LANG', 'LC_ALL']
         for l in preferred:
             if l.lower() in locales:
                 logger.debug(f'using locale {l}')
-                environ['LANG'] = l
+                for env_var in env_vars:
+                    environ[env_var] = l
                 break
         else:
             logger.debug('using fallback locale C')
-            environ['LANG'] = 'C'
+            for env_var in env_vars:
+                environ[env_var] = 'C'
     def clear_pkg_cache() -> None:
         logger.debug('clearing package cache')
         for i in Path(PACMAN_PKG_DIR).iterdir():
             if i.is_file():
                 i.unlink()
     def run_needrestart(ignore_error=False) -> None:
         logger.debug('running needrestart')
```

### Comparing `pacroller-0.1.8/src/pacroller/news.py` & `pacroller-0.1.9/src/pacroller/news.py`

 * *Files identical despite different names*

### Comparing `pacroller-0.1.8/src/pacroller/update-merge-config.py` & `pacroller-0.1.9/src/pacroller/update-merge-config.py`

 * *Files identical despite different names*

### Comparing `pacroller-0.1.8/src/pacroller/utils.py` & `pacroller-0.1.9/src/pacroller/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     output = ANSI_ESCAPE.sub('', output)
     return output.split('\n')
 
 def pacman_time_to_timestamp(stime: str) -> int:
     ''' the format pacman is using seems to be not iso compatible '''
     dt = datetime.strptime(stime, "%Y-%m-%dT%H:%M:%S%z")
     return mktime(dt.astimezone().timetuple())
+pacman_time_to_timestamp('2024-01-01T00:00:00+0000')
 
 def back_readline(fp: BinaryIO) -> Iterator[str]:
     pos = fp.seek(0, 2)
     if pos == 0:
         return
     previous = b''
     while pos > 0:
```

### Comparing `pacroller-0.1.8/src/pacroller.egg-info/PKG-INFO` & `pacroller-0.1.9/src/pacroller.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pacroller
-Version: 0.1.8
+Version: 0.1.9
 Summary: unattended upgrade for archlinux
 Home-page: https://github.com/isjerryxiao/pacroller
 Author: Jerry Xiao
 Author-email: pacroller@mail.jerryxiao.cc
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyalpm
 
 # Pacroller
 The "Unattended Upgrades" for Arch Linux.
 
 ## Concept
 Parsing the output of pacman and pacman.log, searching for known patterns and notifying the user whether there is a potential error.
 Currently the design is regex-based, any output that is unable to match a set of regex is reported back to the user.
```

### Comparing `pacroller-0.1.8/src/pacroller.egg-info/SOURCES.txt` & `pacroller-0.1.9/src/pacroller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

