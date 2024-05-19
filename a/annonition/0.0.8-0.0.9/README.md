# Comparing `tmp/annonition-0.0.8.tar.gz` & `tmp/annonition-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annonition-0.0.8.tar", last modified: Sat May 18 19:18:13 2024, max compression
+gzip compressed data, was "annonition-0.0.9.tar", last modified: Sun May 19 22:20:52 2024, max compression
```

## Comparing `annonition-0.0.8.tar` & `annonition-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 19:18:13.030000 annonition-0.0.8/
--rw-rw-rw-   0        0        0      452 2024-05-18 19:18:14.000000 annonition-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-05-07 21:46:06.000000 annonition-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 19:18:13.040000 annonition-0.0.8/annonition/
--rw-rw-rw-   0        0        0       77 2024-05-12 22:40:06.000000 annonition-0.0.8/annonition/__init__.py
--rw-rw-rw-   0        0        0     5068 2024-05-18 19:16:14.000000 annonition-0.0.8/annonition/logger.py
--rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.0.8/annonition/main.py
--rw-rw-rw-   0        0        0      930 2024-05-18 19:10:48.000000 annonition-0.0.8/annonition/t.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:18:13.060000 annonition-0.0.8/annonition.egg-info/
--rw-rw-rw-   0        0        0      452 2024-05-18 19:18:14.000000 annonition-0.0.8/annonition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-05-18 19:18:14.000000 annonition-0.0.8/annonition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 19:18:14.000000 annonition-0.0.8/annonition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-18 19:18:14.000000 annonition-0.0.8/annonition.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 19:18:14.000000 annonition-0.0.8/annonition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 19:18:14.000000 annonition-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      843 2024-05-18 19:18:04.000000 annonition-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:20:52.360000 annonition-0.0.9/
+-rw-rw-rw-   0        0        0      452 2024-05-19 22:20:54.000000 annonition-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-05-07 21:46:06.000000 annonition-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 22:20:52.390000 annonition-0.0.9/annonition/
+-rw-rw-rw-   0        0        0       77 2024-05-12 22:40:06.000000 annonition-0.0.9/annonition/__init__.py
+-rw-rw-rw-   0        0        0     5352 2024-05-19 22:20:16.000000 annonition-0.0.9/annonition/logger.py
+-rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.0.9/annonition/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 22:20:52.410000 annonition-0.0.9/annonition.egg-info/
+-rw-rw-rw-   0        0        0      452 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-19 22:20:54.000000 annonition-0.0.9/annonition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 22:20:54.000000 annonition-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      843 2024-05-19 22:20:32.000000 annonition-0.0.9/setup.py
```

### Comparing `annonition-0.0.8/annonition/logger.py` & `annonition-0.0.9/annonition/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,113 +205,131 @@
 00000cc0: 7175 6974 220d 0a20 2020 2020 2020 206c  quit"..        l
 00000cd0: 6f67 6765 7220 3d20 4375 7374 6f6d 4c6f  ogger = CustomLo
 00000ce0: 6767 6572 2869 676e 6f72 653d 5b22 2f68  gger(ignore=["/h
 00000cf0: 6561 6c74 6822 2c20 2250 7265 7373 2043  ealth", "Press C
 00000d00: 5452 4c2b 4320 746f 2071 7569 7422 5d29  TRL+C to quit"])
 00000d10: 0d0a 2020 2020 2222 220d 0a20 2020 2064  ..    """..    d
 00000d20: 6566 205f 5f6e 6577 5f5f 2863 6c73 2c20  ef __new__(cls, 
-00000d30: 6c65 7665 6c3a 204c 6576 656c 5479 7065  level: LevelType
-00000d40: 203d 2249 4e46 4f22 2c20 6e61 6d65 3d27   ="INFO", name='
-00000d50: 7765 726b 7a65 7567 272c 2069 676e 6f72  werkzeug', ignor
-00000d60: 653a 206c 6973 7420 7c20 4e6f 6e65 203d  e: list | None =
-00000d70: 204e 6f6e 652c 2069 6e63 6c75 6465 5f64   None, include_d
-00000d80: 6174 653a 2062 6f6f 6c20 3d54 7275 652c  ate: bool =True,
-00000d90: 2069 6e63 6c75 6465 5f6c 6576 656c 3a20   include_level: 
-00000da0: 626f 6f6c 203d 5472 7565 2c20 6461 7465  bool =True, date
-00000db0: 5f63 6f6c 6f72 3a20 436f 6c6f 7254 7970  _color: ColorTyp
-00000dc0: 6520 3d27 7965 6c6c 6f77 2729 3a0d 0a20  e ='yellow'):.. 
-00000dd0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00000de0: 2020 2020 4372 6561 7465 7320 616e 6420      Creates and 
-00000df0: 7265 7475 726e 7320 6120 6e65 7720 6c6f  returns a new lo
-00000e00: 6767 6572 2069 6e73 7461 6e63 6520 7769  gger instance wi
-00000e10: 7468 2073 7065 6369 6669 6564 2063 6f6e  th specified con
-00000e20: 6669 6775 7261 7469 6f6e 732e 0d0a 0d0a  figurations.....
-00000e30: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00000e40: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
-00000e50: 206e 616d 6520 2873 7472 293a 2054 6865   name (str): The
-00000e60: 206e 616d 6520 6f66 2074 6865 206c 6f67   name of the log
-00000e70: 6765 722e 2044 6566 6175 6c74 2069 7320  ger. Default is 
-00000e80: 2777 6572 6b7a 6575 6727 2e0d 0a20 2020  'werkzeug'...   
-00000e90: 2020 2020 2020 2020 2069 676e 6f72 6520           ignore 
-00000ea0: 286c 6973 7420 6f66 2073 7472 2c20 6f70  (list of str, op
-00000eb0: 7469 6f6e 616c 293a 2041 206c 6973 7420  tional): A list 
-00000ec0: 6f66 206d 6573 7361 6765 2073 7562 7374  of message subst
-00000ed0: 7269 6e67 7320 746f 2069 676e 6f72 6520  rings to ignore 
-00000ee0: 696e 2074 6865 206c 6f67 732e 0d0a 2020  in the logs...  
-00000ef0: 2020 2020 2020 2020 2020 696e 636c 7564            includ
-00000f00: 655f 6461 7465 2028 626f 6f6c 2c20 6f70  e_date (bool, op
-00000f10: 7469 6f6e 616c 293a 2057 6865 7468 6572  tional): Whether
-00000f20: 2074 6f20 696e 636c 7564 6520 7468 6520   to include the 
-00000f30: 6461 7465 2069 6e20 7468 6520 6c6f 6720  date in the log 
-00000f40: 6d65 7373 6167 6573 2e20 4465 6661 756c  messages. Defaul
-00000f50: 7420 6973 2054 7275 652e 0d0a 2020 2020  t is True...    
-00000f60: 2020 2020 2020 2020 696e 636c 7564 655f          include_
-00000f70: 6c65 7665 6c20 2862 6f6f 6c2c 206f 7074  level (bool, opt
-00000f80: 696f 6e61 6c29 3a20 5768 6574 6865 7220  ional): Whether 
-00000f90: 746f 2069 6e63 6c75 6465 2074 6865 206c  to include the l
-00000fa0: 6f67 206c 6576 656c 2069 6e20 7468 6520  og level in the 
-00000fb0: 6c6f 6720 6d65 7373 6167 6573 2e20 4465  log messages. De
-00000fc0: 6661 756c 7420 6973 2054 7275 652e 0d0a  fault is True...
-00000fd0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00000fe0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000ff0: 6c6f 6767 696e 672e 4c6f 6767 6572 3a20  logging.Logger: 
-00001000: 4120 636f 6e66 6967 7572 6564 206c 6f67  A configured log
-00001010: 6765 7220 696e 7374 616e 6365 2077 6974  ger instance wit
-00001020: 6820 636f 6c6f 7265 6420 6c6f 6773 2061  h colored logs a
-00001030: 6e64 2065 6e64 706f 696e 7420 6669 6c74  nd endpoint filt
-00001040: 6572 696e 672e 0d0a 2020 2020 2020 2020  ering...        
-00001050: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-00001060: 6967 6e6f 7265 2069 7320 4e6f 6e65 3a0d  ignore is None:.
-00001070: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
-00001080: 6f72 6520 3d20 5b5d 0d0a 2020 2020 2020  ore = []..      
-00001090: 2020 7665 7262 6f73 656c 6f67 732e 696e    verboselogs.in
-000010a0: 7374 616c 6c28 290d 0a20 2020 2020 2020  stall()..       
-000010b0: 206c 6f67 6769 6e67 2e56 4552 424f 5345   logging.VERBOSE
-000010c0: 203d 2076 6572 626f 7365 6c6f 6773 2e56   = verboselogs.V
-000010d0: 4552 424f 5345 0d0a 2020 2020 2020 2020  ERBOSE..        
-000010e0: 6c6f 6767 696e 672e 5350 414d 203d 2076  logging.SPAM = v
-000010f0: 6572 626f 7365 6c6f 6773 2e53 5041 4d0d  erboselogs.SPAM.
-00001100: 0a20 2020 2020 2020 206c 6f67 6769 6e67  .        logging
-00001110: 2e4e 4f54 4943 4520 3d20 7665 7262 6f73  .NOTICE = verbos
-00001120: 656c 6f67 732e 4e4f 5449 4345 0d0a 2020  elogs.NOTICE..  
-00001130: 2020 2020 2020 6c6f 6767 696e 672e 5355        logging.SU
-00001140: 4343 4553 5320 3d20 7665 7262 6f73 656c  CCESS = verbosel
-00001150: 6f67 732e 5355 4343 4553 530d 0a0d 0a20  ogs.SUCCESS.... 
-00001160: 2020 2020 2020 206c 6f67 6765 7220 3d20         logger = 
-00001170: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
-00001180: 7228 6e61 6d65 290d 0a20 2020 2020 2020  r(name)..       
-00001190: 206c 6f67 6765 722e 6164 6446 696c 7465   logger.addFilte
-000011a0: 7228 456e 6470 6f69 6e74 4669 6c74 6572  r(EndpointFilter
-000011b0: 2869 676e 6f72 6529 290d 0a0d 0a20 2020  (ignore))....   
-000011c0: 2020 2020 2066 6f72 6d61 745f 656c 656d       format_elem
-000011d0: 656e 7473 203d 205b 5d0d 0a20 2020 2020  ents = []..     
-000011e0: 2020 2069 6620 696e 636c 7564 655f 6461     if include_da
-000011f0: 7465 3a0d 0a20 2020 2020 2020 2020 2020  te:..           
-00001200: 2066 6f72 6d61 745f 656c 656d 656e 7473   format_elements
-00001210: 2e61 7070 656e 6428 2725 2861 7363 7469  .append('%(ascti
-00001220: 6d65 2973 2729 0d0a 2020 2020 2020 2020  me)s')..        
-00001230: 6966 2069 6e63 6c75 6465 5f6c 6576 656c  if include_level
-00001240: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00001250: 6f72 6d61 745f 656c 656d 656e 7473 2e61  ormat_elements.a
-00001260: 7070 656e 6428 2725 286c 6576 656c 6e61  ppend('%(levelna
-00001270: 6d65 2973 2729 0d0a 2020 2020 2020 2020  me)s')..        
-00001280: 666f 726d 6174 5f65 6c65 6d65 6e74 732e  format_elements.
-00001290: 6170 7065 6e64 2827 2528 6d65 7373 6167  append('%(messag
-000012a0: 6529 7327 290d 0a20 2020 2020 2020 206c  e)s')..        l
-000012b0: 6f67 5f66 6f72 6d61 7420 3d20 2720 272e  og_format = ' '.
-000012c0: 6a6f 696e 2866 6f72 6d61 745f 656c 656d  join(format_elem
-000012d0: 656e 7473 290d 0a20 2020 2020 2020 2066  ents)..        f
-000012e0: 6965 6c64 5f73 7479 6c65 7320 3d20 7b27  ield_styles = {'
-000012f0: 6173 6374 696d 6527 3a20 7b27 636f 6c6f  asctime': {'colo
-00001300: 7227 3a20 6461 7465 5f63 6f6c 6f72 2c20  r': date_color, 
-00001310: 2762 6f6c 6427 3a20 4661 6c73 657d 7d0d  'bold': False}}.
-00001320: 0a0d 0a20 2020 2020 2020 2063 6f6c 6f72  ...        color
-00001330: 6564 6c6f 6773 2e69 6e73 7461 6c6c 286c  edlogs.install(l
-00001340: 6f67 6765 723d 6c6f 6767 6572 2c20 6973  ogger=logger, is
-00001350: 6174 7479 3d54 7275 652c 2066 6d74 3d6c  atty=True, fmt=l
-00001360: 6f67 5f66 6f72 6d61 742c 206c 6576 656c  og_format, level
-00001370: 3d6c 6576 656c 2e75 7070 6572 2829 2c20  =level.upper(), 
-00001380: 6669 656c 645f 7374 796c 6573 3d66 6965  field_styles=fie
-00001390: 6c64 5f73 7479 6c65 7329 0d0a 2020 2020  ld_styles)..    
-000013a0: 2020 2020 7265 7475 726e 2041 7574 6f46      return AutoF
-000013b0: 6f72 6d61 7441 6461 7074 6572 286c 6f67  ormatAdapter(log
-000013c0: 6765 7229 0d0a 2020 2020 0d0a            ger)..    ..
+00000d30: 6c65 7665 6c3a 204f 7074 696f 6e61 6c5b  level: Optional[
+00000d40: 4c65 7665 6c54 7970 655d 203d 2249 4e46  LevelType] ="INF
+00000d50: 4f22 2c20 6e61 6d65 3d27 7765 726b 7a65  O", name='werkze
+00000d60: 7567 272c 2069 676e 6f72 653a 206c 6973  ug', ignore: lis
+00000d70: 7420 7c20 4e6f 6e65 203d 204e 6f6e 652c  t | None = None,
+00000d80: 2069 6e63 6c75 6465 5f64 6174 653a 2062   include_date: b
+00000d90: 6f6f 6c20 3d54 7275 652c 2069 6e63 6c75  ool =True, inclu
+00000da0: 6465 5f6c 6576 656c 3a20 626f 6f6c 203d  de_level: bool =
+00000db0: 5472 7565 2c20 6461 7465 5f63 6f6c 6f72  True, date_color
+00000dc0: 3a20 436f 6c6f 7254 7970 6520 3d27 7965  : ColorType ='ye
+00000dd0: 6c6c 6f77 2729 3a0d 0a20 2020 2020 2020  llow'):..       
+00000de0: 2022 2222 0d0a 2020 2020 2020 2020 4372   """..        Cr
+00000df0: 6561 7465 7320 616e 6420 7265 7475 726e  eates and return
+00000e00: 7320 6120 6e65 7720 6c6f 6767 6572 2069  s a new logger i
+00000e10: 6e73 7461 6e63 6520 7769 7468 2073 7065  nstance with spe
+00000e20: 6369 6669 6564 2063 6f6e 6669 6775 7261  cified configura
+00000e30: 7469 6f6e 732e 0d0a 0d0a 2020 2020 2020  tions.....      
+00000e40: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
+00000e50: 2020 2020 2020 2020 2020 206e 616d 6520             name 
+00000e60: 2873 7472 293a 2054 6865 206e 616d 6520  (str): The name 
+00000e70: 6f66 2074 6865 206c 6f67 6765 722e 2044  of the logger. D
+00000e80: 6566 6175 6c74 2069 7320 2777 6572 6b7a  efault is 'werkz
+00000e90: 6575 6727 2e0d 0a20 2020 2020 2020 2020  eug'...         
+00000ea0: 2020 2069 676e 6f72 6520 286c 6973 7420     ignore (list 
+00000eb0: 6f66 2073 7472 2c20 6f70 7469 6f6e 616c  of str, optional
+00000ec0: 293a 2041 206c 6973 7420 6f66 206d 6573  ): A list of mes
+00000ed0: 7361 6765 2073 7562 7374 7269 6e67 7320  sage substrings 
+00000ee0: 746f 2069 676e 6f72 6520 696e 2074 6865  to ignore in the
+00000ef0: 206c 6f67 732e 0d0a 2020 2020 2020 2020   logs...        
+00000f00: 2020 2020 696e 636c 7564 655f 6461 7465      include_date
+00000f10: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
+00000f20: 293a 2057 6865 7468 6572 2074 6f20 696e  ): Whether to in
+00000f30: 636c 7564 6520 7468 6520 6461 7465 2069  clude the date i
+00000f40: 6e20 7468 6520 6c6f 6720 6d65 7373 6167  n the log messag
+00000f50: 6573 2e20 4465 6661 756c 7420 6973 2054  es. Default is T
+00000f60: 7275 652e 0d0a 2020 2020 2020 2020 2020  rue...          
+00000f70: 2020 696e 636c 7564 655f 6c65 7665 6c20    include_level 
+00000f80: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
+00000f90: 3a20 5768 6574 6865 7220 746f 2069 6e63  : Whether to inc
+00000fa0: 6c75 6465 2074 6865 206c 6f67 206c 6576  lude the log lev
+00000fb0: 656c 2069 6e20 7468 6520 6c6f 6720 6d65  el in the log me
+00000fc0: 7373 6167 6573 2e20 4465 6661 756c 7420  ssages. Default 
+00000fd0: 6973 2054 7275 652e 0d0a 0d0a 2020 2020  is True.....    
+00000fe0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+00000ff0: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
+00001000: 672e 4c6f 6767 6572 3a20 4120 636f 6e66  g.Logger: A conf
+00001010: 6967 7572 6564 206c 6f67 6765 7220 696e  igured logger in
+00001020: 7374 616e 6365 2077 6974 6820 636f 6c6f  stance with colo
+00001030: 7265 6420 6c6f 6773 2061 6e64 2065 6e64  red logs and end
+00001040: 706f 696e 7420 6669 6c74 6572 696e 672e  point filtering.
+00001050: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00001060: 2020 2020 2020 2069 6620 6967 6e6f 7265         if ignore
+00001070: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00001080: 2020 2020 2020 2069 676e 6f72 6520 3d20         ignore = 
+00001090: 5b5d 0d0a 2020 2020 2020 2020 7665 7262  []..        verb
+000010a0: 6f73 656c 6f67 732e 696e 7374 616c 6c28  oselogs.install(
+000010b0: 290d 0a20 2020 2020 2020 206c 6f67 6769  )..        loggi
+000010c0: 6e67 2e56 4552 424f 5345 203d 2076 6572  ng.VERBOSE = ver
+000010d0: 626f 7365 6c6f 6773 2e56 4552 424f 5345  boselogs.VERBOSE
+000010e0: 0d0a 2020 2020 2020 2020 6c6f 6767 696e  ..        loggin
+000010f0: 672e 5350 414d 203d 2076 6572 626f 7365  g.SPAM = verbose
+00001100: 6c6f 6773 2e53 5041 4d0d 0a20 2020 2020  logs.SPAM..     
+00001110: 2020 206c 6f67 6769 6e67 2e4e 4f54 4943     logging.NOTIC
+00001120: 4520 3d20 7665 7262 6f73 656c 6f67 732e  E = verboselogs.
+00001130: 4e4f 5449 4345 0d0a 2020 2020 2020 2020  NOTICE..        
+00001140: 6c6f 6767 696e 672e 5355 4343 4553 5320  logging.SUCCESS 
+00001150: 3d20 7665 7262 6f73 656c 6f67 732e 5355  = verboselogs.SU
+00001160: 4343 4553 530d 0a0d 0a20 2020 2020 2020  CCESS....       
+00001170: 206c 6f67 6765 7220 3d20 6c6f 6767 696e   logger = loggin
+00001180: 672e 6765 744c 6f67 6765 7228 6e61 6d65  g.getLogger(name
+00001190: 290d 0a20 2020 2020 2020 206c 6f67 6765  )..        logge
+000011a0: 722e 6164 6446 696c 7465 7228 456e 6470  r.addFilter(Endp
+000011b0: 6f69 6e74 4669 6c74 6572 2869 676e 6f72  ointFilter(ignor
+000011c0: 6529 290d 0a0d 0a20 2020 2020 2020 2069  e))....        i
+000011d0: 6620 6c65 7665 6c20 6973 204e 6f6e 653a  f level is None:
+000011e0: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+000011f0: 6767 6572 2e64 6973 6162 6c65 6420 3d20  gger.disabled = 
+00001200: 5472 7565 0d0a 2020 2020 2020 2020 656c  True..        el
+00001210: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00001220: 2066 6f72 6d61 745f 656c 656d 656e 7473   format_elements
+00001230: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00001240: 2020 2069 6620 696e 636c 7564 655f 6461     if include_da
+00001250: 7465 3a0d 0a20 2020 2020 2020 2020 2020  te:..           
+00001260: 2020 2020 2066 6f72 6d61 745f 656c 656d       format_elem
+00001270: 656e 7473 2e61 7070 656e 6428 2725 2861  ents.append('%(a
+00001280: 7363 7469 6d65 2973 2729 0d0a 2020 2020  sctime)s')..    
+00001290: 2020 2020 2020 2020 6966 2069 6e63 6c75          if inclu
+000012a0: 6465 5f6c 6576 656c 3a0d 0a20 2020 2020  de_level:..     
+000012b0: 2020 2020 2020 2020 2020 2066 6f72 6d61             forma
+000012c0: 745f 656c 656d 656e 7473 2e61 7070 656e  t_elements.appen
+000012d0: 6428 2725 286c 6576 656c 6e61 6d65 2973  d('%(levelname)s
+000012e0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+000012f0: 666f 726d 6174 5f65 6c65 6d65 6e74 732e  format_elements.
+00001300: 6170 7065 6e64 2827 2528 6d65 7373 6167  append('%(messag
+00001310: 6529 7327 290d 0a20 2020 2020 2020 2020  e)s')..         
+00001320: 2020 206c 6f67 5f66 6f72 6d61 7420 3d20     log_format = 
+00001330: 2720 272e 6a6f 696e 2866 6f72 6d61 745f  ' '.join(format_
+00001340: 656c 656d 656e 7473 290d 0a20 2020 2020  elements)..     
+00001350: 2020 2020 2020 2066 6965 6c64 5f73 7479         field_sty
+00001360: 6c65 7320 3d20 7b27 6173 6374 696d 6527  les = {'asctime'
+00001370: 3a20 7b27 636f 6c6f 7227 3a20 6461 7465  : {'color': date
+00001380: 5f63 6f6c 6f72 2c20 2762 6f6c 6427 3a20  _color, 'bold': 
+00001390: 4661 6c73 657d 7d0d 0a0d 0a20 2020 2020  False}}....     
+000013a0: 2020 2020 2020 2063 6f6c 6f72 6564 6c6f         coloredlo
+000013b0: 6773 2e69 6e73 7461 6c6c 286c 6f67 6765  gs.install(logge
+000013c0: 723d 6c6f 6767 6572 2c20 6973 6174 7479  r=logger, isatty
+000013d0: 3d54 7275 652c 2066 6d74 3d6c 6f67 5f66  =True, fmt=log_f
+000013e0: 6f72 6d61 742c 206c 6576 656c 3d6c 6576  ormat, level=lev
+000013f0: 656c 2e75 7070 6572 2829 2c20 6669 656c  el.upper(), fiel
+00001400: 645f 7374 796c 6573 3d66 6965 6c64 5f73  d_styles=field_s
+00001410: 7479 6c65 7329 0d0a 2020 2020 2020 2020  tyles)..        
+00001420: 2020 2020 6c6f 6767 6572 2e64 6973 6162      logger.disab
+00001430: 6c65 6420 3d20 4661 6c73 650d 0a0d 0a20  led = False.... 
+00001440: 2020 2020 2020 2063 6f6c 6f72 6564 6c6f         coloredlo
+00001450: 6773 2e69 6e73 7461 6c6c 286c 6f67 6765  gs.install(logge
+00001460: 723d 6c6f 6767 6572 2c20 6973 6174 7479  r=logger, isatty
+00001470: 3d54 7275 652c 2066 6d74 3d6c 6f67 5f66  =True, fmt=log_f
+00001480: 6f72 6d61 742c 206c 6576 656c 3d6c 6576  ormat, level=lev
+00001490: 656c 2e75 7070 6572 2829 2c20 6669 656c  el.upper(), fiel
+000014a0: 645f 7374 796c 6573 3d66 6965 6c64 5f73  d_styles=field_s
+000014b0: 7479 6c65 7329 0d0a 2020 2020 2020 2020  tyles)..        
+000014c0: 7265 7475 726e 2041 7574 6f46 6f72 6d61  return AutoForma
+000014d0: 7441 6461 7074 6572 286c 6f67 6765 7229  tAdapter(logger)
+000014e0: 0d0a 2020 2020 0d0a                      ..    ..
```

### Comparing `annonition-0.0.8/setup.py` & `annonition-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(path.join(working_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="annonition",
-    version="0.0.8",
+    version="0.0.9",
     author="Abtin Turing",
     author_email="abtinturing@gmail.com",
     description="Beginning of a new era in annotation tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/abtinturing/anno",
     packages=find_packages(),
```

