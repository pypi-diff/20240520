# Comparing `tmp/checksec_py-0.7.1.tar.gz` & `tmp/checksec_py-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checksec_py-0.7.1.tar", max compression
+gzip compressed data, was "checksec_py-0.7.2.tar", max compression
```

## Comparing `checksec_py-0.7.1.tar` & `checksec_py-0.7.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-12 07:14:30.795878 checksec_py-0.7.1/LICENSE
--rw-r--r--   0        0        0     8657 2023-05-12 07:14:30.795878 checksec_py-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/__init__.py
--rw-r--r--   0        0        0     5901 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/__main__.py
--rw-r--r--   0        0        0      616 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/binary.py
--rw-r--r--   0        0        0     7384 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/elf.py
--rw-r--r--   0        0        0      218 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/errors.py
--rw-r--r--   0        0        0    13391 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/output.py
--rw-r--r--   0        0        0     4397 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/pe.py
--rw-r--r--   0        0        0     4809 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/utils.py
--rw-r--r--   0        0        0     1383 2023-05-12 07:14:30.795878 checksec_py-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     9527 1970-01-01 00:00:00.000000 checksec_py-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-20 02:56:59.107905 checksec_py-0.7.2/LICENSE
+-rw-r--r--   0        0        0     8657 2024-05-20 02:56:59.107905 checksec_py-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/__init__.py
+-rw-r--r--   0        0        0     5901 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/__main__.py
+-rw-r--r--   0        0        0      616 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/binary.py
+-rw-r--r--   0        0        0     7384 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/elf.py
+-rw-r--r--   0        0        0      218 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/errors.py
+-rw-r--r--   0        0        0    13391 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/output.py
+-rw-r--r--   0        0        0     4397 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/pe.py
+-rw-r--r--   0        0        0     4852 2024-05-20 02:56:59.107905 checksec_py-0.7.2/checksec/utils.py
+-rw-r--r--   0        0        0     1385 2024-05-20 02:56:59.107905 checksec_py-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     9479 1970-01-01 00:00:00.000000 checksec_py-0.7.2/PKG-INFO
```

### Comparing `checksec_py-0.7.1/LICENSE` & `checksec_py-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.1/README.md` & `checksec_py-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.1/checksec/__main__.py` & `checksec_py-0.7.2/checksec/__main__.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.1/checksec/binary.py` & `checksec_py-0.7.2/checksec/binary.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.1/checksec/elf.py` & `checksec_py-0.7.2/checksec/elf.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.1/checksec/output.py` & `checksec_py-0.7.2/checksec/output.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.1/checksec/pe.py` & `checksec_py-0.7.2/checksec/pe.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7.1/checksec/utils.py` & `checksec_py-0.7.2/checksec/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,25 +114,25 @@
         "s390x-64": "libc6,64bit",
         "ia64-64": "libc6,IA-64",
         "arm-32": "libc6(,hard-float)?",
     }
     abi_type = mach_map.get(machine, "libc6")
     # Note, we search libXXX.so.XXX, not just libXXX.so (!)
     expr = re.compile(r"^\s+lib%s\.so.[^\s]+\s+\(%s.*=>\s+(.*)$" % (re.escape(name), abi_type))
-    p = subprocess.Popen(["ldconfig", "-N", "-p"], stdout=subprocess.PIPE)
     result = None
-    for line in p.stdout:
-        res = expr.match(line.decode())
-        if res is None:
-            continue
-        if result is not None:
-            raise RuntimeError("Duplicate library found for %s" % name)
-        result = res.group(1)
-    if p.wait():
-        raise RuntimeError('"ldconfig -p" failed')
+    with subprocess.Popen(["ldconfig", "-N", "-p"], stdout=subprocess.PIPE) as p:
+        for line in p.stdout:
+            res = expr.match(line.decode())
+            if res is None:
+                continue
+            if result is not None:
+                raise RuntimeError("Duplicate library found for %s" % name)
+            result = res.group(1)
+        if p.wait():
+            raise RuntimeError('"ldconfig -p" failed')
     if result is None:
         raise RuntimeError("Library %s not found" % name)
     return result
 
 
 def lief_set_logging(lvl: int):
     """Configures LIEF logging level
```

### Comparing `checksec_py-0.7.1/pyproject.toml` & `checksec_py-0.7.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "checksec-py"
-version = "0.7.1"
+version = "0.7.2"
 description = "Checksec tool implemented in Python"
 authors = ["Mathieu Tarral <mathieu.tarral@protonmail.com>"]
 readme = "README.md"
 packages = [{include = "checksec"}]
 license = "GPL-3.0-only"
 repository = "https://github.com/Wenzel/checksec.py"
 keywords = ["checksec", "security", "ELF", "PE", "binary"]
 
 [tool.poetry.scripts]
 checksec = 'checksec.__main__:entrypoint'
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.12"
+python = ">=3.10,<3.13"
 lief = "0.13.0"
 docopt = "0.6.2"
 rich = "13.3.5"
 pylddwrap = "1.0.1"
 
 [tool.poetry.dev-dependencies]
 flake8 = "5.0.4"
 flake8-bugbear = "20.1.4"
 isort = "5.10.1"
-black = "22.8.0"
+black = "24.3.0"
 mypy = "1.2.0"
 pytest = "7.2.0"
 coverage = { version = "5.3", extras = ["toml"] }
 poethepoet = "0.20.0"
-pyinstaller = "5.10.1"
+pyinstaller = "5.13.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `checksec_py-0.7.1/PKG-INFO` & `checksec_py-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: checksec-py
-Version: 0.7.1
+Version: 0.7.2
 Summary: Checksec tool implemented in Python
 Home-page: https://github.com/Wenzel/checksec.py
 License: GPL-3.0-only
 Keywords: checksec,security,ELF,PE,binary
 Author: Mathieu Tarral
 Author-email: mathieu.tarral@protonmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: docopt (==0.6.2)
 Requires-Dist: lief (==0.13.0)
 Requires-Dist: pylddwrap (==1.0.1)
 Requires-Dist: rich (==13.3.5)
 Project-URL: Repository, https://github.com/Wenzel/checksec.py
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: checksec-py Version: 0.7.1 Summary: Checksec tool
+Metadata-Version: 2.1 Name: checksec-py Version: 0.7.2 Summary: Checksec tool
 implemented in Python Home-page: https://github.com/Wenzel/checksec.py License:
 GPL-3.0-only Keywords: checksec,security,ELF,PE,binary Author: Mathieu Tarral
-Author-email: mathieu.tarral@protonmail.com Requires-Python: >=3.8,<3.12
+Author-email: mathieu.tarral@protonmail.com Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: docopt (==0.6.2) Requires-Dist: lief
-(==0.13.0) Requires-Dist: pylddwrap (==1.0.1) Requires-Dist: rich (==13.3.5)
-Project-URL: Repository, https://github.com/Wenzel/checksec.py Description-
-Content-Type: text/markdown
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Requires-Dist: docopt
+(==0.6.2) Requires-Dist: lief (==0.13.0) Requires-Dist: pylddwrap (==1.0.1)
+Requires-Dist: rich (==13.3.5) Project-URL: Repository, https://github.com/
+Wenzel/checksec.py Description-Content-Type: text/markdown
                                     ************
                               cchheecckksseecc..ppyy ************
          ******** CChheecckksseecc ttooooll iinn PPyytthhoonn,, RRiicchh oouuttppuutt,, bbaasseedd oonn LLIIEEFF ********
                                      _DD_ee_mm_oo
 _[_C_I_ _b_a_d_g_e_]_[_P_y_P_I_ _p_a_c_k_a_g_e_ _b_a_d_g_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_ _b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_s_._g_i_t_t_e_r_._i_m_/
                           _c_h_e_c_k_s_e_c_-_p_y_/_c_o_m_m_u_n_i_t_y_._s_v_g_]
      _[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_c_h_e_c_k_s_e_c_-_p_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
```

