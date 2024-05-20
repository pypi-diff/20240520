# Comparing `tmp/cmdline_provenance-1.0.0.tar.gz` & `tmp/cmdline_provenance-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdline_provenance-1.0.0.tar", last modified: Mon Apr 12 06:30:51 2021, max compression
+gzip compressed data, was "cmdline_provenance-1.1.0.tar", last modified: Mon May 20 05:40:46 2024, max compression
```

## Comparing `cmdline_provenance-1.0.0.tar` & `cmdline_provenance-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 irv033     (502) staff       (20)        0 2021-04-12 06:30:51.450206 cmdline_provenance-1.0.0/
--rw-r--r--   0 irv033     (502) staff       (20)     1069 2021-04-08 05:38:15.000000 cmdline_provenance-1.0.0/LICENSE
--rw-r--r--   0 irv033     (502) staff       (20)       17 2021-04-12 05:53:45.000000 cmdline_provenance-1.0.0/MANIFEST.in
--rw-r--r--   0 irv033     (502) staff       (20)     2799 2021-04-12 06:30:51.450058 cmdline_provenance-1.0.0/PKG-INFO
--rw-r--r--   0 irv033     (502) staff       (20)     1966 2021-04-12 06:30:15.000000 cmdline_provenance-1.0.0/README.md
-drwxr-xr-x   0 irv033     (502) staff       (20)        0 2021-04-12 06:30:51.449026 cmdline_provenance-1.0.0/cmdline_provenance/
--rw-r--r--   0 irv033     (502) staff       (20)      252 2021-04-12 05:54:48.000000 cmdline_provenance-1.0.0/cmdline_provenance/__init__.py
--rw-r--r--   0 irv033     (502) staff       (20)     2855 2021-04-12 01:08:30.000000 cmdline_provenance-1.0.0/cmdline_provenance/cmdline_provenance.py
--rw-r--r--   0 irv033     (502) staff       (20)      839 2021-04-12 05:40:15.000000 cmdline_provenance-1.0.0/cmdline_provenance/test_script.py
-drwxr-xr-x   0 irv033     (502) staff       (20)        0 2021-04-12 06:30:51.449851 cmdline_provenance-1.0.0/cmdline_provenance.egg-info/
--rw-r--r--   0 irv033     (502) staff       (20)     2799 2021-04-12 06:30:51.000000 cmdline_provenance-1.0.0/cmdline_provenance.egg-info/PKG-INFO
--rw-r--r--   0 irv033     (502) staff       (20)      394 2021-04-12 06:30:51.000000 cmdline_provenance-1.0.0/cmdline_provenance.egg-info/SOURCES.txt
--rw-r--r--   0 irv033     (502) staff       (20)        1 2021-04-12 06:30:51.000000 cmdline_provenance-1.0.0/cmdline_provenance.egg-info/dependency_links.txt
--rw-r--r--   0 irv033     (502) staff       (20)        1 2021-04-12 05:25:08.000000 cmdline_provenance-1.0.0/cmdline_provenance.egg-info/not-zip-safe
--rw-r--r--   0 irv033     (502) staff       (20)       10 2021-04-12 06:30:51.000000 cmdline_provenance-1.0.0/cmdline_provenance.egg-info/requires.txt
--rw-r--r--   0 irv033     (502) staff       (20)       19 2021-04-12 06:30:51.000000 cmdline_provenance-1.0.0/cmdline_provenance.egg-info/top_level.txt
--rw-r--r--   0 irv033     (502) staff       (20)       38 2021-04-12 06:30:51.450248 cmdline_provenance-1.0.0/setup.cfg
--rw-r--r--   0 irv033     (502) staff       (20)      782 2021-04-12 05:56:36.000000 cmdline_provenance-1.0.0/setup.py
+drwxr-xr-x   0 irv033     (502) staff       (20)        0 2024-05-20 05:40:46.723631 cmdline_provenance-1.1.0/
+-rw-r--r--   0 irv033     (502) staff       (20)     1069 2021-04-08 05:38:15.000000 cmdline_provenance-1.1.0/LICENSE
+-rw-r--r--   0 irv033     (502) staff       (20)       17 2021-04-12 05:53:45.000000 cmdline_provenance-1.1.0/MANIFEST.in
+-rw-r--r--   0 irv033     (502) staff       (20)     2500 2024-05-20 05:40:46.723018 cmdline_provenance-1.1.0/PKG-INFO
+-rw-r--r--   0 irv033     (502) staff       (20)     1966 2021-04-12 06:30:15.000000 cmdline_provenance-1.1.0/README.md
+drwxr-xr-x   0 irv033     (502) staff       (20)        0 2024-05-20 05:40:46.716842 cmdline_provenance-1.1.0/cmdline_provenance/
+-rw-r--r--   0 irv033     (502) staff       (20)      252 2021-04-12 05:54:48.000000 cmdline_provenance-1.1.0/cmdline_provenance/__init__.py
+-rw-r--r--   0 irv033     (502) staff       (20)     6601 2024-05-20 05:33:10.000000 cmdline_provenance-1.1.0/cmdline_provenance/cmdline_provenance.py
+-rw-r--r--   0 irv033     (502) staff       (20)     1108 2024-05-20 05:23:55.000000 cmdline_provenance-1.1.0/cmdline_provenance/test_script.py
+drwxr-xr-x   0 irv033     (502) staff       (20)        0 2024-05-20 05:40:46.722488 cmdline_provenance-1.1.0/cmdline_provenance.egg-info/
+-rw-r--r--   0 irv033     (502) staff       (20)     2500 2024-05-20 05:40:46.000000 cmdline_provenance-1.1.0/cmdline_provenance.egg-info/PKG-INFO
+-rw-r--r--   0 irv033     (502) staff       (20)      394 2024-05-20 05:40:46.000000 cmdline_provenance-1.1.0/cmdline_provenance.egg-info/SOURCES.txt
+-rw-r--r--   0 irv033     (502) staff       (20)        1 2024-05-20 05:40:46.000000 cmdline_provenance-1.1.0/cmdline_provenance.egg-info/dependency_links.txt
+-rw-r--r--   0 irv033     (502) staff       (20)        1 2021-04-12 05:25:08.000000 cmdline_provenance-1.1.0/cmdline_provenance.egg-info/not-zip-safe
+-rw-r--r--   0 irv033     (502) staff       (20)       16 2024-05-20 05:40:46.000000 cmdline_provenance-1.1.0/cmdline_provenance.egg-info/requires.txt
+-rw-r--r--   0 irv033     (502) staff       (20)       19 2024-05-20 05:40:46.000000 cmdline_provenance-1.1.0/cmdline_provenance.egg-info/top_level.txt
+-rw-r--r--   0 irv033     (502) staff       (20)       38 2024-05-20 05:40:46.723679 cmdline_provenance-1.1.0/setup.cfg
+-rw-r--r--   0 irv033     (502) staff       (20)      791 2024-05-20 05:37:33.000000 cmdline_provenance-1.1.0/setup.py
```

### Comparing `cmdline_provenance-1.0.0/LICENSE` & `cmdline_provenance-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdline_provenance-1.0.0/PKG-INFO` & `cmdline_provenance-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 Metadata-Version: 2.1
 Name: cmdline_provenance
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package for keeping track of your data processing steps
 Home-page: https://github.com/DamienIrving/cmdline_provenance
 Author: Damien Irving
 Author-email: irving.damien@gmail.com
 License: MIT License
-Description: [![PyPI version](https://badge.fury.io/py/cmdline-provenance.svg)](https://badge.fury.io/py/cmdline-provenance)
-        [![Documentation Status](https://readthedocs.org/projects/cmdline-provenance/badge/?version=latest)](https://cmdline-provenance.readthedocs.io/en/latest/?badge=latest)
-        [![Downloads](https://pepy.tech/badge/cmdline-provenance/week)](https://pepy.tech/project/cmdline-provenance/week)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        # Command line provenance
-        
-        `cmdline_provenance` is a Python package for keeping track of your data processing steps.
-        
-        It was inspired by the popular [NCO](http://nco.sourceforge.net/)
-        and [CDO](https://code.mpimet.mpg.de/projects/cdo) command line tools,
-        which automatically generate a record of what was executed at the command line,
-        append that record to the history attribute from the input (netCDF) data file,
-        and then set the new extended record as the history attribute of the output (netCDF) data file.
-        
-        For example, after selecting the 2001-2005 time period from a rainfall data file
-        and then deleting the `long_name` file attribute,
-        the command log would look as follows:
-        ```
-        Fri Dec 08 10:05:47 2017: ncatted -O -a long_name,pr,d,, rainfall_data_2001-2005.nc
-        Fri Dec 01 07:59:16 2017: cdo seldate,2001-01-01,2005-12-31 rainfall_data_1850-2005.nc rainfall_data_2001-2005.nc
-        ```
-        Following this simple approach to data provenance,
-        it is possible maintain a record of all data processing steps
-        from intial download/creation of your data files to the end result (e.g. a .png image).
-        
-        `cmdline_provenance` contains a series of functions for generating history records in the NCO/CDO format,
-        and for combining the current record with previous records to maintain a complete command log.
-        
-        ## Documentation
-        
-        http://cmdline-provenance.readthedocs.io/en/latest/
-        
-        ## Installation
-        
-        ```
-        pip install cmdline-provenance
-        ```
-        or
-        ```
-        conda install cmdline_provenance
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipynbname
+Requires-Dist: numpy
+
+[![PyPI version](https://badge.fury.io/py/cmdline-provenance.svg)](https://badge.fury.io/py/cmdline-provenance)
+[![Documentation Status](https://readthedocs.org/projects/cmdline-provenance/badge/?version=latest)](https://cmdline-provenance.readthedocs.io/en/latest/?badge=latest)
+[![Downloads](https://pepy.tech/badge/cmdline-provenance/week)](https://pepy.tech/project/cmdline-provenance/week)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+# Command line provenance
+
+`cmdline_provenance` is a Python package for keeping track of your data processing steps.
+
+It was inspired by the popular [NCO](http://nco.sourceforge.net/)
+and [CDO](https://code.mpimet.mpg.de/projects/cdo) command line tools,
+which automatically generate a record of what was executed at the command line,
+append that record to the history attribute from the input (netCDF) data file,
+and then set the new extended record as the history attribute of the output (netCDF) data file.
+
+For example, after selecting the 2001-2005 time period from a rainfall data file
+and then deleting the `long_name` file attribute,
+the command log would look as follows:
+```
+Fri Dec 08 10:05:47 2017: ncatted -O -a long_name,pr,d,, rainfall_data_2001-2005.nc
+Fri Dec 01 07:59:16 2017: cdo seldate,2001-01-01,2005-12-31 rainfall_data_1850-2005.nc rainfall_data_2001-2005.nc
+```
+Following this simple approach to data provenance,
+it is possible maintain a record of all data processing steps
+from intial download/creation of your data files to the end result (e.g. a .png image).
+
+`cmdline_provenance` contains a series of functions for generating history records in the NCO/CDO format,
+and for combining the current record with previous records to maintain a complete command log.
+
+## Documentation
+
+http://cmdline-provenance.readthedocs.io/en/latest/
+
+## Installation
+
+```
+pip install cmdline-provenance
+```
+or
+```
+conda install cmdline_provenance
+```
```

### Comparing `cmdline_provenance-1.0.0/README.md` & `cmdline_provenance-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cmdline_provenance-1.0.0/cmdline_provenance/test_script.py` & `cmdline_provenance-1.1.0/cmdline_provenance/test_script.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,22 +9,28 @@
 
 
 def main(args):
     """Run the program."""
 
 #    dset1 = xr.open_dataset(args.infile1)
 #    dset2 = xr.open_dataset(args.infile2)
-    new_log = cmdprov.new_log(infile_logs={'file.nc': 'file history...'},
-                              code_url='https://github.com/',
-                              extra_notes=['note1', 'note2'])
+    new_log = cmdprov.new_log(
+        infile_logs={'file.nc': 'file history...'},
+        code_url='https://github.com/',
+        extra_notes=['note1', 'note2'],
+        wildcard_prefixes=[
+            '/g/data/ob53/BARRA2/output/reanalysis/AUS-11/BOM/ERA5/historical/hres/BARRA-R2/v1/day/pr/v20231001/',
+            '/g/data/ob53/BARRA2/output/reanalysis/AUS-11/BOM/ERA5/ssp370/hres/BARRA-R2/v1/day/pr/v20231001/',
+        ]
+    )
     print(new_log)
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description=__doc__)
     
-    parser.add_argument("infile1", type=str, help="Input file name")
-    parser.add_argument("infile2", type=str, help="Input file name")
+    parser.add_argument("infiles", type=str, nargs='*', help="Input file names")
     parser.add_argument("outfile", type=str, help="Output file name")
+    parser.add_argument("--more_files", type=str, nargs='*', help="More input file names")
 
     args = parser.parse_args()            
     main(args)
```

### Comparing `cmdline_provenance-1.0.0/cmdline_provenance.egg-info/PKG-INFO` & `cmdline_provenance-1.1.0/cmdline_provenance.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 Metadata-Version: 2.1
-Name: cmdline-provenance
-Version: 1.0.0
+Name: cmdline_provenance
+Version: 1.1.0
 Summary: A Python package for keeping track of your data processing steps
 Home-page: https://github.com/DamienIrving/cmdline_provenance
 Author: Damien Irving
 Author-email: irving.damien@gmail.com
 License: MIT License
-Description: [![PyPI version](https://badge.fury.io/py/cmdline-provenance.svg)](https://badge.fury.io/py/cmdline-provenance)
-        [![Documentation Status](https://readthedocs.org/projects/cmdline-provenance/badge/?version=latest)](https://cmdline-provenance.readthedocs.io/en/latest/?badge=latest)
-        [![Downloads](https://pepy.tech/badge/cmdline-provenance/week)](https://pepy.tech/project/cmdline-provenance/week)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        # Command line provenance
-        
-        `cmdline_provenance` is a Python package for keeping track of your data processing steps.
-        
-        It was inspired by the popular [NCO](http://nco.sourceforge.net/)
-        and [CDO](https://code.mpimet.mpg.de/projects/cdo) command line tools,
-        which automatically generate a record of what was executed at the command line,
-        append that record to the history attribute from the input (netCDF) data file,
-        and then set the new extended record as the history attribute of the output (netCDF) data file.
-        
-        For example, after selecting the 2001-2005 time period from a rainfall data file
-        and then deleting the `long_name` file attribute,
-        the command log would look as follows:
-        ```
-        Fri Dec 08 10:05:47 2017: ncatted -O -a long_name,pr,d,, rainfall_data_2001-2005.nc
-        Fri Dec 01 07:59:16 2017: cdo seldate,2001-01-01,2005-12-31 rainfall_data_1850-2005.nc rainfall_data_2001-2005.nc
-        ```
-        Following this simple approach to data provenance,
-        it is possible maintain a record of all data processing steps
-        from intial download/creation of your data files to the end result (e.g. a .png image).
-        
-        `cmdline_provenance` contains a series of functions for generating history records in the NCO/CDO format,
-        and for combining the current record with previous records to maintain a complete command log.
-        
-        ## Documentation
-        
-        http://cmdline-provenance.readthedocs.io/en/latest/
-        
-        ## Installation
-        
-        ```
-        pip install cmdline-provenance
-        ```
-        or
-        ```
-        conda install cmdline_provenance
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipynbname
+Requires-Dist: numpy
+
+[![PyPI version](https://badge.fury.io/py/cmdline-provenance.svg)](https://badge.fury.io/py/cmdline-provenance)
+[![Documentation Status](https://readthedocs.org/projects/cmdline-provenance/badge/?version=latest)](https://cmdline-provenance.readthedocs.io/en/latest/?badge=latest)
+[![Downloads](https://pepy.tech/badge/cmdline-provenance/week)](https://pepy.tech/project/cmdline-provenance/week)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+# Command line provenance
+
+`cmdline_provenance` is a Python package for keeping track of your data processing steps.
+
+It was inspired by the popular [NCO](http://nco.sourceforge.net/)
+and [CDO](https://code.mpimet.mpg.de/projects/cdo) command line tools,
+which automatically generate a record of what was executed at the command line,
+append that record to the history attribute from the input (netCDF) data file,
+and then set the new extended record as the history attribute of the output (netCDF) data file.
+
+For example, after selecting the 2001-2005 time period from a rainfall data file
+and then deleting the `long_name` file attribute,
+the command log would look as follows:
+```
+Fri Dec 08 10:05:47 2017: ncatted -O -a long_name,pr,d,, rainfall_data_2001-2005.nc
+Fri Dec 01 07:59:16 2017: cdo seldate,2001-01-01,2005-12-31 rainfall_data_1850-2005.nc rainfall_data_2001-2005.nc
+```
+Following this simple approach to data provenance,
+it is possible maintain a record of all data processing steps
+from intial download/creation of your data files to the end result (e.g. a .png image).
+
+`cmdline_provenance` contains a series of functions for generating history records in the NCO/CDO format,
+and for combining the current record with previous records to maintain a complete command log.
+
+## Documentation
+
+http://cmdline-provenance.readthedocs.io/en/latest/
+
+## Installation
+
+```
+pip install cmdline-provenance
+```
+or
+```
+conda install cmdline_provenance
+```
```

### Comparing `cmdline_provenance-1.0.0/setup.py` & `cmdline_provenance-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='cmdline_provenance',
-    version='1.0.0',
+    version='1.1.0',
     description='A Python package for keeping track of your data processing steps',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Damien Irving',
     author_email='irving.damien@gmail.com',
     url='https://github.com/DamienIrving/cmdline_provenance',
     packages=['cmdline_provenance'],
     zip_safe=False,
-    install_requires=['ipynbname'],
+    install_requires=['ipynbname', 'numpy'],
     license='MIT License',
     include_package_data=True,
     classifiers=(
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',)
 )
```

