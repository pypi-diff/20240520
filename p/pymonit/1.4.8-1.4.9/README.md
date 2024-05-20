# Comparing `tmp/pymonit-1.4.8.tar.gz` & `tmp/pymonit-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.4.8.tar", last modified: Mon May 20 10:10:18 2024, max compression
+gzip compressed data, was "pymonit-1.4.9.tar", last modified: Mon May 20 10:16:30 2024, max compression
```

## Comparing `pymonit-1.4.8.tar` & `pymonit-1.4.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-20 10:10:18.589273 pymonit-1.4.8/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       86 2024-05-19 13:06:25.000000 pymonit-1.4.8/.gitignore
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.8/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1820 2024-05-20 10:10:18.589273 pymonit-1.4.8/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1185 2024-05-20 10:09:51.000000 pymonit-1.4.8/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-20 10:10:18.589273 pymonit-1.4.8/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.8/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.8/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.8/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2020 2024-05-19 13:04:31.000000 pymonit-1.4.8/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.8/monit/http.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.8/monit/init.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.8/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.8/monit/logger.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-20 10:10:18.589273 pymonit-1.4.8/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1820 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      359 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-20 10:10:18.000000 pymonit-1.4.8/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 01:06:10.000000 pymonit-1.4.8/requirements.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      542 2024-05-19 12:44:37.000000 pymonit-1.4.8/sample.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      320 2024-05-18 17:14:22.000000 pymonit-1.4.8/sample_static.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-20 10:10:18.592606 pymonit-1.4.8/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-20 10:10:15.000000 pymonit-1.4.8/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-20 10:16:30.169164 pymonit-1.4.9/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       86 2024-05-19 13:06:25.000000 pymonit-1.4.9/.gitignore
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.9/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1846 2024-05-20 10:16:30.169164 pymonit-1.4.9/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1211 2024-05-20 10:15:56.000000 pymonit-1.4.9/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-20 10:16:30.165830 pymonit-1.4.9/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.9/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.9/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.9/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2020 2024-05-19 13:04:31.000000 pymonit-1.4.9/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.9/monit/http.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.9/monit/init.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.9/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.9/monit/logger.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-20 10:16:30.165830 pymonit-1.4.9/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1846 2024-05-20 10:16:29.000000 pymonit-1.4.9/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      359 2024-05-20 10:16:30.000000 pymonit-1.4.9/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-20 10:16:29.000000 pymonit-1.4.9/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-20 10:16:29.000000 pymonit-1.4.9/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-20 10:16:29.000000 pymonit-1.4.9/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 01:06:10.000000 pymonit-1.4.9/requirements.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      542 2024-05-19 12:44:37.000000 pymonit-1.4.9/sample.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      320 2024-05-18 17:14:22.000000 pymonit-1.4.9/sample_static.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-20 10:16:30.169164 pymonit-1.4.9/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-20 10:16:15.000000 pymonit-1.4.9/setup.py
```

### Comparing `pymonit-1.4.8/LICENSE` & `pymonit-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.8/PKG-INFO` & `pymonit-1.4.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.8
+Version: 1.4.9
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -47,17 +47,17 @@
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
-        monit.notify_and_exit(e)
+        monit.notify_and_exit(e) # para o script
 
-    monit.end()
+    monit.end() # manda sinal de fim sem erros
 
 
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização avançada**
@@ -77,17 +77,16 @@
     try:
         log.info("Hello, World!")
 
         sleep(2)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
-        monit.notify(e)
-
-    monit.msg("O Script terminou com sucesso.") # whatsapp
+        monit.msg("Ocorreu um erro.") # Whatsapp
+        monit.notify(e) # não para o script
 
-    monit.end() # manda sinal de fim sem erros
+    monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.4.8/README.md` & `pymonit-1.4.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
-        monit.notify_and_exit(e)
+        monit.notify_and_exit(e) # para o script
 
-    monit.end()
+    monit.end() # manda sinal de fim sem erros
 
 
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização avançada**
@@ -58,17 +58,16 @@
     try:
         log.info("Hello, World!")
 
         sleep(2)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
-        monit.notify(e)
-
-    monit.msg("O Script terminou com sucesso.") # whatsapp
+        monit.msg("Ocorreu um erro.") # Whatsapp
+        monit.notify(e) # não para o script
 
-    monit.end() # manda sinal de fim sem erros
+    monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.4.8/monit/config.py` & `pymonit-1.4.9/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.8/monit/core.py` & `pymonit-1.4.9/monit/core.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.8/monit/func.py` & `pymonit-1.4.9/monit/func.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.8/monit/http.py` & `pymonit-1.4.9/monit/http.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.8/monit/log2file.py` & `pymonit-1.4.9/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.8/monit/logger.py` & `pymonit-1.4.9/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.8/pymonit.egg-info/PKG-INFO` & `pymonit-1.4.9/pymonit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.8
+Version: 1.4.9
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -47,17 +47,17 @@
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
-        monit.notify_and_exit(e)
+        monit.notify_and_exit(e) # para o script
 
-    monit.end()
+    monit.end() # manda sinal de fim sem erros
 
 
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização avançada**
@@ -77,17 +77,16 @@
     try:
         log.info("Hello, World!")
 
         sleep(2)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
-        monit.notify(e)
-
-    monit.msg("O Script terminou com sucesso.") # whatsapp
+        monit.msg("Ocorreu um erro.") # Whatsapp
+        monit.notify(e) # não para o script
 
-    monit.end() # manda sinal de fim sem erros
+    monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.4.8/sample.py` & `pymonit-1.4.9/sample.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.8/setup.py` & `pymonit-1.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.4.8',
+    version='1.4.9',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

