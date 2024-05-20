# Comparing `tmp/CTG_Utils-1.1.7.tar.gz` & `tmp/CTG_Utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTG_Utils-1.1.7.tar", last modified: Sat May 18 08:14:53 2024, max compression
+gzip compressed data, was "CTG_Utils-1.2.0.tar", last modified: Mon May 20 08:27:05 2024, max compression
```

## Comparing `CTG_Utils-1.1.7.tar` & `CTG_Utils-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 08:14:53.858442 CTG_Utils-1.1.7/
-drwxrwxrwx   0        0        0        0 2024-05-18 08:14:53.805616 CTG_Utils-1.1.7/CTG_Utils/
-drwxrwxrwx   0        0        0        0 2024-05-18 08:14:53.825015 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/
--rw-rw-rw-   0        0        0     9766 2024-05-17 09:17:02.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTGClasses.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:14:53.835503 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/
--rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
--rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
--rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
--rw-rw-rw-   0        0        0     1920 2024-05-15 10:17:54.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt
--rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
--rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
--rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
--rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
--rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
--rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
--rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
--rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_config.py
--rw-rw-rw-   0        0        0    18645 2024-05-17 13:14:08.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_effectif.py
--rw-rw-rw-   0        0        0    11562 2024-05-17 09:25:57.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_plot.py
--rw-rw-rw-   0        0        0    15508 2024-05-17 09:25:57.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_synthese.py
--rw-rw-rw-   0        0        0     3865 2024-05-17 09:08:39.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_utility.py
--rw-rw-rw-   0        0        0      214 2024-05-15 06:16:14.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_Func/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:14:53.856448 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/
--rw-rw-rw-   0        0        0    16064 2024-05-14 08:52:29.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/GUI_Globals.py
--rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageDivers.py
--rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageEffectif.py
--rw-rw-rw-   0        0        0    11622 2024-05-16 07:23:59.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageSorties.py
--rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageSynthese.py
--rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageTendance.py
--rw-rw-rw-   0        0        0    32252 2024-05-15 06:32:08.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/Page_Classes.py
--rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/Useful_Classes.py
--rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/Useful_Functions.py
--rw-rw-rw-   0        0        0      221 2024-05-15 06:17:11.000000 CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 08:14:53.818030 CTG_Utils-1.1.7/CTG_Utils.egg-info/
--rw-rw-rw-   0        0        0      670 2024-05-18 08:14:52.000000 CTG_Utils-1.1.7/CTG_Utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2024-05-18 08:14:52.000000 CTG_Utils-1.1.7/CTG_Utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 08:14:52.000000 CTG_Utils-1.1.7/CTG_Utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-18 08:14:52.000000 CTG_Utils-1.1.7/CTG_Utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-05-18 08:14:52.000000 CTG_Utils-1.1.7/CTG_Utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.7/LICENSE
--rw-rw-rw-   0        0        0       90 2024-05-18 08:06:39.000000 CTG_Utils-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      670 2024-05-18 08:14:53.857444 CTG_Utils-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-05-18 08:07:37.000000 CTG_Utils-1.1.7/README.md
--rwxrwxrwx   0        0        0     1041 2024-05-18 07:56:05.000000 CTG_Utils-1.1.7/make_exe.bat
--rwxrwxrwx   0        0        0      166 2024-05-18 07:46:20.000000 CTG_Utils-1.1.7/make_venv.bat
--rw-rw-rw-   0        0        0       42 2024-05-18 08:14:53.858442 CTG_Utils-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1367 2024-05-18 08:08:25.000000 CTG_Utils-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.914675 CTG_Utils-1.2.0/
+drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.841866 CTG_Utils-1.2.0/CTG_Utils/
+drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.864803 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/
+-rw-rw-rw-   0        0        0     9766 2024-05-17 09:17:02.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTGClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.879766 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/
+-rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
+-rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
+-rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
+-rw-rw-rw-   0        0        0     1920 2024-05-15 10:17:54.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt
+-rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
+-rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
+-rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
+-rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
+-rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
+-rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
+-rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
+-rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_config.py
+-rw-rw-rw-   0        0        0    18737 2024-05-20 06:33:57.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_effectif.py
+-rw-rw-rw-   0        0        0    11562 2024-05-17 09:25:57.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_plot.py
+-rw-rw-rw-   0        0        0    15836 2024-05-20 06:57:30.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_synthese.py
+-rw-rw-rw-   0        0        0     4661 2024-05-20 06:33:57.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_utility.py
+-rw-rw-rw-   0        0        0      214 2024-05-15 06:16:14.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_Func/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.912680 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/
+-rw-rw-rw-   0        0        0    16076 2024-05-20 07:00:54.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/GUI_Globals.py
+-rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageDivers.py
+-rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageEffectif.py
+-rw-rw-rw-   0        0        0    11820 2024-05-20 06:52:52.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageSorties.py
+-rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageSynthese.py
+-rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageTendance.py
+-rw-rw-rw-   0        0        0    32252 2024-05-15 06:32:08.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Page_Classes.py
+-rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Useful_Classes.py
+-rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Useful_Functions.py
+-rw-rw-rw-   0        0        0      221 2024-05-15 06:17:11.000000 CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 08:27:05.854830 CTG_Utils-1.2.0/CTG_Utils.egg-info/
+-rw-rw-rw-   0        0        0      670 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-05-20 08:27:04.000000 CTG_Utils-1.2.0/CTG_Utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       90 2024-05-18 08:06:39.000000 CTG_Utils-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      670 2024-05-20 08:27:05.914675 CTG_Utils-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-05-18 08:07:37.000000 CTG_Utils-1.2.0/README.md
+-rwxrwxrwx   0        0        0     1031 2024-05-20 08:04:44.000000 CTG_Utils-1.2.0/make_exe.bat
+-rwxrwxrwx   0        0        0      107 2024-05-20 07:59:16.000000 CTG_Utils-1.2.0/make_venv.bat
+-rw-rw-rw-   0        0        0       42 2024-05-20 08:27:05.914675 CTG_Utils-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2024-05-20 08:22:55.000000 CTG_Utils-1.2.0/setup.py
```

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTGClasses.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTGClasses.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_effectif.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_effectif.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
         
     effectif_df = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path(file_effectif))
     effectif_df = effectif_df[['N° Licencié', 'Nom','Prénom','Sexe','Pratique VAE']]
     
     correction_effectif = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path('correction_effectif.xlsx'))
     correction_effectif.index = correction_effectif['N° Licencié']
     membres_sympathisants_df = pd.read_excel(ctg_path / Path(str(year))/Path('DATA')/ Path('membres_sympatisants.xlsx'))
+    membres_sympathisants_df = membres_sympathisants_df[['N° Licencié', 'Nom','Prénom','Sexe','Pratique VAE']]
     
     for num_licence in correction_effectif.index:
         idx = effectif_df[effectif_df["N° Licencié"]==num_licence].index
         effectif_df.loc[idx,'Prénom'] = correction_effectif.loc[num_licence,'Prénom']
         effectif_df.loc[idx,'Nom'] = correction_effectif.loc[num_licence,'Nom']
     
     effectif_df = pd.concat([effectif_df, membres_sympathisants_df], ignore_index=True, axis=0)
-    
     effectif_df['Prénom1'] = effectif_df['Prénom'].str[0]
     effectif_df['Prénom'] = effectif_df['Prénom'].str.replace(' ','-')
     
     return effectif_df
 
 def inscrit_sejour(file,no_match,df_effectif):
 
@@ -59,24 +59,22 @@
 
 
     nfc = functools.partial(unicodedata.normalize,'NFD')
     convert_to_ascii = lambda text : nfc(text). \
                                      encode('ascii', 'ignore'). \
                                      decode('utf-8').\
                                      strip()
-
+                                     
     df = pd.read_csv(file) 
     sejour = os.path.splitext(os.path.basename(file))[0]
     
     if len(df) != 0:
         dg = df['Unnamed: 0'].str.upper()
         dg = dg.dropna()
         dg = dg.str.replace(' \t?','',regex=False)
-        dg = dg.str.replace('JO ','JOSEPH ')
-        dg = dg.str.replace('HERVÉ.P','PEREZ HERVE',regex=False)
         dg = dg.str.replace('.',' ',regex=False)
         dg = dg.str.replace(' - ','-',regex=False)
         dg = dg.apply(convert_to_ascii)
         dg = dg.drop_duplicates()
         dg = dg.str.split('\s{1,10}')
 
         dg = dg.apply(lambda row : row+[None] if len(row)==2 else row)
@@ -120,18 +118,20 @@
         dg = pd.DataFrame([[None,None,None,None,sejour,]], columns=['N° Licencié','Nom','Prénom','Sexe','sejour',])
     
     return dg
 
     
 def count_participation(path,ctg_path,year,info_rando):
     
+    # Standard library imports
     import os
     import re
     from pathlib import Path
-
+    
+    # Third party imports
     import pandas as pd
     
     flag_sejour = False
     if os.path.split(path)[-1] == 'SEJOUR' : 
         flag_sejour = True
 
     type_sortie_default = os.path.basename(path)
@@ -173,16 +173,16 @@
                 dg['nbr_jours'] = dh['nbr_jours'].tolist()[0]    
             
         if dg.reset_index().loc[0,'Nom'] is not None:
             nbr_inscrits = len(dg)
             if nbr_inscrits != 0:
                 nbr_moyen_participants = nbr_moyen_participants + (nbr_inscrits - nbr_moyen_participants)/counter
                 counter += 1
-                info_sejours.append(f"{os.path.split(path)[-1]} :{sejour}, Nombre d'inscrits : {nbr_inscrits}")
-               
+                info_sejours.append(f"{os.path.split(path)[-1]} :{sejour}, Nombre d'inscrits : {nbr_inscrits}")   
+        
         df_list.append(dg)
         file_store = os.path.splitext(sejour)[0]+'.xlsx'
         dg.to_excel(path / Path('EXCEL') / Path(file_store))
        
     info_sejours.append(f"Nombre d'évènenements : {counter-1}. Nombre moyen de participants : {nbr_moyen_participants}")
     info_sejours = '\n'.join(info_sejours)
     info_sejours_path = ctg_path / Path(str(year)) / Path('STATISTIQUES')/ Path(type_sortie_default+'.txt')
```

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_plot.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_plot.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_synthese.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_synthese.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,554 +417,574 @@
 00001a00: 202f 2050 6174 6828 2753 5441 5449 5354   / Path('STATIST
 00001a10: 4951 5545 5327 2920 2f20 5061 7468 2827  IQUES') / Path('
 00001a20: 7379 6e74 6865 7365 5f61 6468 6572 656e  synthese_adheren
 00001a30: 742e 786c 7378 2729 0d0a 2020 2020 6467  t.xlsx')..    dg
 00001a40: 2e74 6f5f 6578 6365 6c28 6669 6c65 5f6f  .to_excel(file_o
 00001a50: 7574 290d 0a20 2020 200d 0a64 6566 2073  ut)..    ..def s
 00001a60: 796e 7468 6573 655f 7261 6e64 6f6e 6e65  ynthese_randonne
-00001a70: 6528 7965 6172 2c63 7467 5f70 6174 6829  e(year,ctg_path)
-00001a80: 3a0d 0a0d 0a20 2020 2023 2053 7461 6e64  :....    # Stand
-00001a90: 6172 6420 6c69 6272 6172 7920 696d 706f  ard library impo
-00001aa0: 7274 730d 0a20 2020 2066 726f 6d20 7061  rts..    from pa
-00001ab0: 7468 6c69 6220 696d 706f 7274 2050 6174  thlib import Pat
-00001ac0: 680d 0a20 2020 200d 0a20 2020 2023 2054  h..    ..    # T
-00001ad0: 6869 7264 2070 6172 7479 2069 6d70 6f72  hird party impor
-00001ae0: 7473 0d0a 2020 2020 696d 706f 7274 206d  ts..    import m
-00001af0: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
-00001b00: 2061 7320 706c 740d 0a20 2020 2069 6d70   as plt..    imp
-00001b10: 6f72 7420 7061 6e64 6173 2061 7320 7064  ort pandas as pd
-00001b20: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00001b30: 6164 646c 6162 656c 7328 782c 792c 6f66  addlabels(x,y,of
-00001b40: 6673 6574 293a 0d0a 2020 2020 2020 2020  fset):..        
-00001b50: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00001b60: 656e 2878 2929 3a0d 0a20 2020 2020 2020  en(x)):..       
-00001b70: 2020 2020 2069 6620 795b 695d 2021 3d20       if y[i] != 
-00001b80: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00001b90: 2020 2020 706c 742e 7465 7874 2878 5b69      plt.text(x[i
-00001ba0: 5d2c 795b 695d 2b6f 6666 7365 742c 726f  ],y[i]+offset,ro
-00001bb0: 756e 6428 795b 695d 2c31 292c 7369 7a65  und(y[i],1),size
-00001bc0: 3d31 3029 0d0a 2020 2020 2020 2020 0d0a  =10)..        ..
-00001bd0: 2020 2020 0d0a 2020 2020 6669 6c65 5f69      ..    file_i
-00001be0: 6e20 3d20 5061 7468 2863 7467 5f70 6174  n = Path(ctg_pat
-00001bf0: 6829 202f 2050 6174 6828 7374 7228 7965  h) / Path(str(ye
-00001c00: 6172 2929 202f 2050 6174 6828 2753 5441  ar)) / Path('STA
-00001c10: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
-00001c20: 7468 2827 7379 6e74 6865 7365 2e78 6c73  th('synthese.xls
-00001c30: 7827 290d 0a20 2020 2064 665f 746f 7461  x')..    df_tota
-00001c40: 6c20 3d20 7064 2e72 6561 645f 6578 6365  l = pd.read_exce
-00001c50: 6c28 6669 6c65 5f69 6e29 0d0a 2020 2020  l(file_in)..    
-00001c60: 6466 5f74 6f74 616c 203d 2064 665f 746f  df_total = df_to
-00001c70: 7461 6c2e 6472 6f70 6e61 2873 7562 7365  tal.dropna(subse
-00001c80: 743d 5b27 4e6f 6d27 5d29 200d 0a20 2020  t=['Nom']) ..   
-00001c90: 2064 6720 3d20 6466 5f74 6f74 616c 2e71   dg = df_total.q
-00001ca0: 7565 7279 2827 5479 7065 3d3d 2252 414e  uery('Type=="RAN
-00001cb0: 444f 4e4e 4545 2227 292e 6772 6f75 7062  DONNEE"').groupb
-00001cc0: 7928 2773 656a 6f75 7227 292e 6167 6728  y('sejour').agg(
-00001cd0: 2763 6f75 6e74 2729 5b27 4ec2 b020 4c69  'count')['N.. Li
-00001ce0: 6365 6e63 69c3 a927 5d0d 0a20 2020 200d  cenci..']..    .
-00001cf0: 0a20 2020 2066 6967 203d 2070 6c74 2e66  .    fig = plt.f
-00001d00: 6967 7572 6528 290d 0a20 2020 2070 6c74  igure()..    plt
-00001d10: 2e62 6172 2872 616e 6765 286c 656e 2864  .bar(range(len(d
-00001d20: 6729 292c 6467 2e74 6f6c 6973 7428 2929  g)),dg.tolist())
-00001d30: 0d0a 2020 2020 6164 646c 6162 656c 7328  ..    addlabels(
-00001d40: 6c69 7374 2872 616e 6765 286c 656e 2864  list(range(len(d
-00001d50: 6729 2929 2c64 672e 746f 6c69 7374 2829  g))),dg.tolist()
-00001d60: 2c30 2e32 290d 0a20 2020 2070 6c74 2e78  ,0.2)..    plt.x
-00001d70: 7469 636b 7328 7261 6e67 6528 6c65 6e28  ticks(range(len(
-00001d80: 6467 2929 2c20 6467 2e69 6e64 6578 2c20  dg)), dg.index, 
-00001d90: 726f 7461 7469 6f6e 3d27 7665 7274 6963  rotation='vertic
-00001da0: 616c 2729 0d0a 2020 2020 706c 742e 7469  al')..    plt.ti
-00001db0: 636b 5f70 6172 616d 7328 6178 6973 3d27  ck_params(axis='
-00001dc0: 7827 2c20 726f 7461 7469 6f6e 3d39 302c  x', rotation=90,
-00001dd0: 206c 6162 656c 7369 7a65 3d31 3029 0d0a   labelsize=10)..
-00001de0: 2020 2020 706c 742e 7469 636b 5f70 6172      plt.tick_par
-00001df0: 616d 7328 6178 6973 3d27 7927 2c6c 6162  ams(axis='y',lab
-00001e00: 656c 7369 7a65 3d31 3029 0d0a 2020 2020  elsize=10)..    
-00001e10: 0d0a 2020 2020 5f20 3d20 706c 742e 7469  ..    _ = plt.ti
-00001e20: 746c 6528 6627 2320 7261 6e64 6f73 203a  tle(f'# randos :
-00001e30: 207b 6c65 6e28 6467 297d 202c 2023 2070   {len(dg)} , # p
-00001e40: 6172 7469 6369 7061 6e74 7320 3a20 7b73  articipants : {s
-00001e50: 756d 2864 6729 7d27 290d 0a20 2020 2070  um(dg)}')..    p
-00001e60: 6c74 2e74 6967 6874 5f6c 6179 6f75 7428  lt.tight_layout(
-00001e70: 290d 0a20 2020 2070 6c74 2e73 686f 7728  )..    plt.show(
-00001e80: 290d 0a20 2020 200d 0a20 2020 2066 6967  )..    ..    fig
-00001e90: 5f66 696c 6520 3d20 2753 594e 5448 4553  _file = 'SYNTHES
-00001ea0: 455f 5241 4e44 4f4e 4e45 4553 2e70 6e67  E_RANDONNEES.png
-00001eb0: 270d 0a20 2020 2070 6c74 2e73 6176 6566  '..    plt.savef
-00001ec0: 6967 2863 7467 5f70 6174 6820 2f20 5061  ig(ctg_path / Pa
-00001ed0: 7468 2873 7472 2879 6561 7229 2920 2f20  th(str(year)) / 
-00001ee0: 5061 7468 2827 5354 4154 4953 5449 5155  Path('STATISTIQU
-00001ef0: 4553 2729 202f 2050 6174 6828 6669 675f  ES') / Path(fig_
-00001f00: 6669 6c65 292c 6262 6f78 5f69 6e63 6865  file),bbox_inche
-00001f10: 733d 2774 6967 6874 2729 0d0a 2020 2020  s='tight')..    
-00001f20: 0d0a 6465 6620 6e62 725f 7365 6a6f 7572  ..def nbr_sejour
-00001f30: 735f 6164 6865 7265 6e74 2879 6561 722c  s_adherent(year,
-00001f40: 2063 7467 5f70 6174 6829 3a0d 0a0d 0a20   ctg_path):.... 
-00001f50: 2020 2023 2053 7461 6e64 6172 6420 6c69     # Standard li
-00001f60: 6272 6172 7920 696d 706f 7274 730d 0a20  brary imports.. 
-00001f70: 2020 2066 726f 6d20 636f 6c6c 6563 7469     from collecti
-00001f80: 6f6e 7320 696d 706f 7274 2043 6f75 6e74  ons import Count
-00001f90: 6572 0d0a 2020 2020 6672 6f6d 2070 6174  er..    from pat
-00001fa0: 686c 6962 2069 6d70 6f72 7420 5061 7468  hlib import Path
-00001fb0: 0d0a 2020 2020 0d0a 2020 2020 2320 5468  ..    ..    # Th
-00001fc0: 6972 6420 7061 7274 7920 696d 706f 7274  ird party import
-00001fd0: 730d 0a20 2020 2069 6d70 6f72 7420 6d61  s..    import ma
-00001fe0: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
-00001ff0: 6173 2070 6c74 0d0a 2020 2020 696d 706f  as plt..    impo
-00002000: 7274 2070 616e 6461 7320 6173 2070 640d  rt pandas as pd.
-00002010: 0a20 2020 200d 0a20 2020 2070 6c74 2e73  .    ..    plt.s
-00002020: 7479 6c65 2e75 7365 2827 6767 706c 6f74  tyle.use('ggplot
-00002030: 2729 0d0a 2020 2020 0d0a 2020 2020 2320  ')..    ..    # 
-00002040: 6675 6e63 7469 6f6e 2074 6f20 6164 6420  function to add 
-00002050: 7661 6c75 6520 6c61 6265 6c73 0d0a 2020  value labels..  
-00002060: 2020 6465 6620 6164 646c 6162 656c 7328    def addlabels(
-00002070: 782c 7929 3a0d 0a20 2020 2020 2020 2066  x,y):..        f
-00002080: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00002090: 6e28 7829 293a 0d0a 2020 2020 2020 2020  n(x)):..        
-000020a0: 2020 2020 706c 742e 7465 7874 2878 5b69      plt.text(x[i
-000020b0: 5d2d 302e 322c 795b 695d 2b31 2c79 5b69  ]-0.2,y[i]+1,y[i
-000020c0: 5d2c 7369 7a65 3d6c 6162 656c 5f73 697a  ],size=label_siz
-000020d0: 6529 0d0a 2020 2020 6c61 6265 6c5f 7369  e)..    label_si
-000020e0: 7a65 203d 2031 350d 0a20 2020 2066 696c  ze = 15..    fil
-000020f0: 655f 696e 203d 2063 7467 5f70 6174 6820  e_in = ctg_path 
-00002100: 2f20 5061 7468 2873 7472 2879 6561 7229  / Path(str(year)
-00002110: 2920 2f20 5061 7468 2827 5354 4154 4953  ) / Path('STATIS
-00002120: 5449 5155 4553 2729 202f 2050 6174 6828  TIQUES') / Path(
-00002130: 2773 796e 7468 6573 655f 6164 6865 7265  'synthese_adhere
-00002140: 6e74 2e78 6c73 7827 290d 0a20 2020 2064  nt.xlsx')..    d
-00002150: 665f 746f 7461 6c20 3d20 7064 2e72 6561  f_total = pd.rea
-00002160: 645f 6578 6365 6c28 6669 6c65 5f69 6e29  d_excel(file_in)
-00002170: 0d0a 2020 2020 0d0a 2020 2020 6320 3d20  ..    ..    c = 
-00002180: 436f 756e 7465 7228 290d 0a20 2020 2063  Counter()..    c
-00002190: 203d 2043 6f75 6e74 6572 2864 665f 746f   = Counter(df_to
-000021a0: 7461 6c5b 274e 6272 5f53 454a 4f55 5253  tal['Nbr_SEJOURS
-000021b0: 275d 2e74 6f6c 6973 7428 2929 0d0a 2020  '].tolist())..  
-000021c0: 2020 6320 3d20 632e 6d6f 7374 5f63 6f6d    c = c.most_com
-000021d0: 6d6f 6e28 290d 0a0d 0a20 2020 2078 2c20  mon()....    x, 
-000021e0: 7920 3d20 7a69 7028 2a63 290d 0a20 2020  y = zip(*c)..   
-000021f0: 2078 203d 206c 6973 7428 7829 0d0a 2020   x = list(x)..  
-00002200: 2020 7920 3d20 6c69 7374 2879 290d 0a20    y = list(y).. 
-00002210: 2020 200d 0a20 2020 2066 6967 2c20 6178     ..    fig, ax
-00002220: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
-00002230: 6669 6773 697a 653d 2835 2c35 2929 0d0a  figsize=(5,5))..
-00002240: 2020 2020 706c 742e 6261 7228 5b73 7472      plt.bar([str
-00002250: 2878 5f73 2920 666f 7220 785f 7320 696e  (x_s) for x_s in
-00002260: 2078 5d2c 7929 0d0a 2020 2020 706c 742e   x],y)..    plt.
-00002270: 786c 6162 656c 2827 4e6f 6d62 7265 2064  xlabel('Nombre d
-00002280: 6520 7061 7274 6963 6970 6174 696f 6e20  e participation 
-00002290: c3a0 2064 6573 2073 c3a9 6a6f 7572 7327  .. des s..jours'
-000022a0: 290d 0a20 2020 2070 6c74 2e79 6c61 6265  )..    plt.ylabe
-000022b0: 6c28 274e 6f6d 6272 6520 6465 206c 6963  l('Nombre de lic
-000022c0: 656e 6369 6572 7327 290d 0a20 2020 2070  enciers')..    p
-000022d0: 6c74 2e74 6963 6b5f 7061 7261 6d73 2861  lt.tick_params(a
-000022e0: 7869 733d 2778 272c 206c 6162 656c 7369  xis='x', labelsi
-000022f0: 7a65 3d6c 6162 656c 5f73 697a 6529 0d0a  ze=label_size)..
-00002300: 2020 2020 706c 742e 7469 636b 5f70 6172      plt.tick_par
-00002310: 616d 7328 6178 6973 3d27 7927 2c20 6c61  ams(axis='y', la
-00002320: 6265 6c73 697a 653d 6c61 6265 6c5f 7369  belsize=label_si
-00002330: 7a65 290d 0a20 2020 2070 6c74 2e74 6974  ze)..    plt.tit
-00002340: 6c65 2873 7472 2879 6561 7229 2c70 6164  le(str(year),pad
-00002350: 3d32 302c 2066 6f6e 7473 697a 653d 3230  =20, fontsize=20
-00002360: 290d 0a20 2020 200d 0a20 2020 2061 782e  )..    ..    ax.
-00002370: 7365 745f 786c 6162 656c 2827 4e20 73c3  set_xlabel('N s.
-00002380: a96a 6f75 7273 272c 2066 6f6e 7473 697a  .jours', fontsiz
-00002390: 6520 3d20 6c61 6265 6c5f 7369 7a65 290d  e = label_size).
-000023a0: 0a20 2020 2061 782e 7365 745f 796c 6162  .    ax.set_ylab
-000023b0: 656c 2827 4e6f 6d62 7265 2064 6520 4354  el('Nombre de CT
-000023c0: 4720 6179 616e 7420 5c6e 2070 6172 7469  G ayant \n parti
-000023d0: 6369 70c3 a920 c3a0 204e 2073 c3a9 6a6f  cip.. .. N s..jo
-000023e0: 7572 7327 2c20 666f 6e74 7369 7a65 203d  urs', fontsize =
-000023f0: 206c 6162 656c 5f73 697a 6529 0d0a 2020   label_size)..  
-00002400: 2020 0d0a 2020 2020 782e 736f 7274 2829    ..    x.sort()
-00002410: 0d0a 2020 2020 6164 646c 6162 656c 7328  ..    addlabels(
-00002420: 782c 7929 0d0a 2020 2020 706c 742e 7469  x,y)..    plt.ti
-00002430: 6768 745f 6c61 796f 7574 2829 0d0a 2020  ght_layout()..  
-00002440: 2020 706c 742e 7368 6f77 2829 0d0a 0d0a    plt.show()....
-00002450: 2020 2020 6669 675f 6669 6c65 203d 2027      fig_file = '
-00002460: 5345 4a4f 5552 535f 5354 4154 5f50 4152  SEJOURS_STAT_PAR
-00002470: 5449 4349 5041 5449 4f4e 2e70 6e67 270d  TICIPATION.png'.
-00002480: 0a20 2020 2070 6c74 2e73 6176 6566 6967  .    plt.savefig
-00002490: 2863 7467 5f70 6174 6820 2f20 5061 7468  (ctg_path / Path
-000024a0: 2873 7472 2879 6561 7229 2920 2f20 5061  (str(year)) / Pa
-000024b0: 7468 2827 5354 4154 4953 5449 5155 4553  th('STATISTIQUES
-000024c0: 2729 202f 2050 6174 6828 6669 675f 6669  ') / Path(fig_fi
-000024d0: 6c65 292c 6262 6f78 5f69 6e63 6865 733d  le),bbox_inches=
-000024e0: 2774 6967 6874 2729 0d0a 2020 2020 0d0a  'tight')..    ..
-000024f0: 6465 6620 7265 6164 5f6d 656d 6f72 795f  def read_memory_
-00002500: 736f 7274 6965 7328 293a 0d0a 0d0a 2020  sorties():....  
-00002510: 2020 2320 5374 616e 6461 7264 206c 6962    # Standard lib
-00002520: 7261 7279 2069 6d70 6f72 7473 0d0a 2020  rary imports..  
-00002530: 2020 696d 706f 7274 206f 732e 7061 7468    import os.path
-00002540: 0d0a 2020 2020 6672 6f6d 2070 6174 686c  ..    from pathl
-00002550: 6962 2069 6d70 6f72 7420 5061 7468 0d0a  ib import Path..
-00002560: 0d0a 2020 2020 2320 3372 6420 7061 7274  ..    # 3rd part
-00002570: 7920 696d 706f 7274 730d 0a20 2020 2069  y imports..    i
-00002580: 6d70 6f72 7420 7961 6d6c 0d0a 2020 2020  mport yaml..    
-00002590: 0d0a 2020 2020 2320 5265 6164 7320 7468  ..    # Reads th
-000025a0: 6520 6465 6661 756c 7420 5056 6368 6172  e default PVchar
-000025b0: 6163 7465 7269 7a61 7469 6f6e 2e79 616d  acterization.yam
-000025c0: 6c20 636f 6e66 6967 2066 696c 650d 0a20  l config file.. 
-000025d0: 2020 2070 6174 685f 636f 6e66 6967 5f66     path_config_f
-000025e0: 696c 6520 3d20 5061 7468 285f 5f66 696c  ile = Path(__fil
-000025f0: 655f 5f29 2e70 6172 656e 742e 7061 7265  e__).parent.pare
-00002600: 6e74 202f 2050 6174 6828 2743 5447 5f46  nt / Path('CTG_F
-00002610: 756e 6327 2920 2f20 5061 7468 2827 4354  unc') / Path('CT
-00002620: 475f 5265 6646 696c 6573 2729 202f 2050  G_RefFiles') / P
-00002630: 6174 6828 276d 656d 6f72 795f 736f 7274  ath('memory_sort
-00002640: 6965 732e 796d 6c27 290d 0a20 2020 2077  ies.yml')..    w
-00002650: 6974 6820 6f70 656e 2870 6174 685f 636f  ith open(path_co
-00002660: 6e66 6967 5f66 696c 6529 2061 7320 6669  nfig_file) as fi
-00002670: 6c65 3a0d 0a20 2020 2020 2020 206d 656d  le:..        mem
-00002680: 6f72 7920 3d20 7961 6d6c 2e73 6166 655f  ory = yaml.safe_
-00002690: 6c6f 6164 2866 696c 6529 0d0a 2020 2020  load(file)..    
-000026a0: 2020 2020 0d0a 2020 2020 2020 200d 0a20      ..       .. 
-000026b0: 2020 2072 6574 7572 6e20 6d65 6d6f 7279     return memory
-000026c0: 0d0a 2020 2020 0d0a 6465 6620 6576 6f6c  ..    ..def evol
-000026d0: 7574 696f 6e5f 736f 7274 6965 7328 7479  ution_sorties(ty
-000026e0: 7065 2c63 7467 5f70 6174 6829 3a0d 0a0d  pe,ctg_path):...
-000026f0: 0a20 2020 2023 2053 7461 6e64 6172 6420  .    # Standard 
-00002700: 6c69 6272 6172 7920 696d 706f 7274 2020  library import  
-00002710: 2020 0d0a 2020 2020 696d 706f 7274 2064    ..    import d
-00002720: 6174 6574 696d 650d 0a20 2020 2066 726f  atetime..    fro
-00002730: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
-00002740: 2050 6174 680d 0a20 2020 2066 726f 6d20   Path..    from 
-00002750: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
-00002760: 7274 206e 616d 6564 7475 706c 650d 0a0d  rt namedtuple...
-00002770: 0a20 2020 2023 2054 6869 7264 2070 6172  .    # Third par
-00002780: 7479 206c 6962 7261 7279 2069 6d70 6f72  ty library impor
-00002790: 7420 2020 2020 0d0a 2020 2020 696d 706f  t     ..    impo
-000027a0: 7274 206d 6174 706c 6f74 6c69 622e 7079  rt matplotlib.py
-000027b0: 706c 6f74 2061 7320 706c 740d 0a20 2020  plot as plt..   
-000027c0: 2069 6d70 6f72 7420 7061 6e64 6173 2061   import pandas a
-000027d0: 7320 7064 0d0a 2020 2020 2020 0d0a 2020  s pd..      ..  
-000027e0: 2020 2320 496e 7465 726e 616c 2069 6d70    # Internal imp
-000027f0: 6f72 740d 0a20 2020 2069 6d70 6f72 7420  ort..    import 
-00002800: 4354 475f 5574 696c 7320 6173 2063 7467  CTG_Utils as ctg
-00002810: 0d0a 2020 2020 6672 6f6d 2043 5447 5f55  ..    from CTG_U
-00002820: 7469 6c73 2e43 5447 5f47 5549 2e47 5549  tils.CTG_GUI.GUI
-00002830: 5f47 6c6f 6261 6c73 2069 6d70 6f72 7420  _Globals import 
-00002840: 4143 5449 5649 5445 5f4c 4953 5420 0d0a  ACTIVITE_LIST ..
-00002850: 2020 2020 0d0a 2020 2020 6465 6620 6164      ..    def ad
-00002860: 645f 6d65 6d6f 7279 2873 7461 745f 6469  d_memory(stat_di
-00002870: 632c 7965 6172 7329 3a0d 0a20 2020 2020  c,years):..     
-00002880: 2020 206d 656d 6f72 7920 3d20 7265 6164     memory = read
-00002890: 5f6d 656d 6f72 795f 736f 7274 6965 7328  _memory_sorties(
-000028a0: 290d 0a20 2020 200d 0a20 2020 200d 0a20  )..    ..    .. 
-000028b0: 2020 2020 2020 2066 6f72 2079 6561 722c         for year,
-000028c0: 7620 696e 206d 656d 6f72 795b 276d 656d  v in memory['mem
-000028d0: 6f72 7927 5d2e 6974 656d 7328 293a 0d0a  ory'].items():..
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00002910: 2020 2020 2020 2020 2073 7461 745f 6469           stat_di
-00002920: 635b 7374 7228 7965 6172 295d 203d 2073  c[str(year)] = s
-00002930: 7461 7479 6561 7228 765b 2750 4152 5449  tatyear(v['PARTI
-00002940: 4349 5041 5449 4f4e 5f53 454a 4f55 5253  CIPATION_SEJOURS
-00002950: 275d 2c20 2020 2020 2020 2020 2020 2020  '],             
-00002960: 2020 2023 206e 6272 5f73 656a 6f75 7273     # nbr_sejours
-00002970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 2020 2020 2020 2020 2020 2020 2030 2c20               0, 
-000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029b0: 2020 2020 2020 2020 2023 206a 6f75 7273           # jours
-000029c0: 5f73 656a 6f75 720d 0a20 2020 2020 2020  _sejour..       
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2020 765b 2753 4f52 5449 4553 5f43      v['SORTIES_C
-00002a00: 4c55 425f 4449 4d41 4e43 4845 275d 2c20  LUB_DIMANCHE'], 
-00002a10: 2320 736f 7274 6965 5f64 696d 616e 6368  # sortie_dimanch
-00002a20: 655f 636c 7562 0d0a 2020 2020 2020 2020  e_club..        
+00001a70: 6528 7965 6172 2c63 7467 5f70 6174 682c  e(year,ctg_path,
+00001a80: 7479 7065 5f73 656a 6f75 7229 3a0d 0a0d  type_sejour):...
+00001a90: 0a20 2020 2023 2053 7461 6e64 6172 6420  .    # Standard 
+00001aa0: 6c69 6272 6172 7920 696d 706f 7274 730d  library imports.
+00001ab0: 0a20 2020 2066 726f 6d20 7061 7468 6c69  .    from pathli
+00001ac0: 6220 696d 706f 7274 2050 6174 680d 0a20  b import Path.. 
+00001ad0: 2020 200d 0a20 2020 2023 2054 6869 7264     ..    # Third
+00001ae0: 2070 6172 7479 2069 6d70 6f72 7473 0d0a   party imports..
+00001af0: 2020 2020 696d 706f 7274 206d 6174 706c      import matpl
+00001b00: 6f74 6c69 622e 7079 706c 6f74 2061 7320  otlib.pyplot as 
+00001b10: 706c 740d 0a20 2020 2069 6d70 6f72 7420  plt..    import 
+00001b20: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
+00001b30: 2020 0d0a 2020 2020 2320 496e 7465 726e    ..    # Intern
+00001b40: 616c 2069 6d70 6f72 7473 0d0a 2020 2020  al imports..    
+00001b50: 6672 6f6d 2043 5447 5f55 7469 6c73 2e43  from CTG_Utils.C
+00001b60: 5447 5f46 756e 632e 4354 475f 7574 696c  TG_Func.CTG_util
+00001b70: 6974 7920 696d 706f 7274 2067 6574 5f63  ity import get_c
+00001b80: 6f75 745f 746f 7461 6c0d 0a20 2020 200d  out_total..    .
+00001b90: 0a20 2020 2064 6566 2061 6464 6c61 6265  .    def addlabe
+00001ba0: 6c73 2878 2c79 2c6f 6666 7365 7429 3a0d  ls(x,y,offset):.
+00001bb0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+00001bc0: 6e20 7261 6e67 6528 6c65 6e28 7829 293a  n range(len(x)):
+00001bd0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00001be0: 2079 5b69 5d20 213d 2030 3a0d 0a20 2020   y[i] != 0:..   
+00001bf0: 2020 2020 2020 2020 2020 2020 2070 6c74               plt
+00001c00: 2e74 6578 7428 785b 695d 2c79 5b69 5d2b  .text(x[i],y[i]+
+00001c10: 6f66 6673 6574 2c72 6f75 6e64 2879 5b69  offset,round(y[i
+00001c20: 5d2c 3129 2c73 697a 653d 3130 290d 0a20  ],1),size=10).. 
+00001c30: 2020 2020 2020 200d 0a20 2020 200d 0a20         ..    .. 
+00001c40: 2020 2066 696c 655f 696e 203d 2050 6174     file_in = Pat
+00001c50: 6828 6374 675f 7061 7468 2920 2f20 5061  h(ctg_path) / Pa
+00001c60: 7468 2873 7472 2879 6561 7229 2920 2f20  th(str(year)) / 
+00001c70: 5061 7468 2827 5354 4154 4953 5449 5155  Path('STATISTIQU
+00001c80: 4553 2729 202f 2050 6174 6828 2773 796e  ES') / Path('syn
+00001c90: 7468 6573 652e 786c 7378 2729 0d0a 2020  these.xlsx')..  
+00001ca0: 2020 6466 5f74 6f74 616c 203d 2070 642e    df_total = pd.
+00001cb0: 7265 6164 5f65 7863 656c 2866 696c 655f  read_excel(file_
+00001cc0: 696e 290d 0a20 2020 2064 665f 746f 7461  in)..    df_tota
+00001cd0: 6c20 3d20 6466 5f74 6f74 616c 2e64 726f  l = df_total.dro
+00001ce0: 706e 6128 7375 6273 6574 3d5b 274e 6f6d  pna(subset=['Nom
+00001cf0: 275d 2920 0d0a 2020 2020 6467 203d 2064  ']) ..    dg = d
+00001d00: 665f 746f 7461 6c2e 7175 6572 7928 2754  f_total.query('T
+00001d10: 7970 653d 3d40 7479 7065 5f73 656a 6f75  ype==@type_sejou
+00001d20: 7227 292e 6772 6f75 7062 7928 2773 656a  r').groupby('sej
+00001d30: 6f75 7227 292e 6167 6728 2763 6f75 6e74  our').agg('count
+00001d40: 2729 5b27 4ec2 b020 4c69 6365 6e63 69c3  ')['N.. Licenci.
+00001d50: a927 5d0d 0a20 2020 0d0a 2020 2020 6669  .']..   ..    fi
+00001d60: 6c65 5f69 6e66 6f20 3d20 5061 7468 2863  le_info = Path(c
+00001d70: 7467 5f70 6174 6829 202f 2050 6174 6828  tg_path) / Path(
+00001d80: 7374 7228 7965 6172 2929 202f 2050 6174  str(year)) / Pat
+00001d90: 6828 2744 4154 4127 2920 2f20 5061 7468  h('DATA') / Path
+00001da0: 2827 696e 666f 5f72 616e 646f 732e 786c  ('info_randos.xl
+00001db0: 7378 2729 0d0a 2020 2020 636f 7574 5f74  sx')..    cout_t
+00001dc0: 6f74 616c 5f72 616e 646f 203d 2067 6574  otal_rando = get
+00001dd0: 5f63 6f75 745f 746f 7461 6c28 7965 6172  _cout_total(year
+00001de0: 2c74 7970 655f 7365 6a6f 7572 2e6c 6f77  ,type_sejour.low
+00001df0: 6572 2829 2c64 672c 6374 675f 7061 7468  er(),dg,ctg_path
+00001e00: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00001e10: 2066 6967 203d 2070 6c74 2e66 6967 7572   fig = plt.figur
+00001e20: 6528 290d 0a20 2020 2070 6c74 2e62 6172  e()..    plt.bar
+00001e30: 2872 616e 6765 286c 656e 2864 6729 292c  (range(len(dg)),
+00001e40: 6467 2e74 6f6c 6973 7428 2929 0d0a 2020  dg.tolist())..  
+00001e50: 2020 6164 646c 6162 656c 7328 6c69 7374    addlabels(list
+00001e60: 2872 616e 6765 286c 656e 2864 6729 2929  (range(len(dg)))
+00001e70: 2c64 672e 746f 6c69 7374 2829 2c30 2e32  ,dg.tolist(),0.2
+00001e80: 290d 0a20 2020 2070 6c74 2e78 7469 636b  )..    plt.xtick
+00001e90: 7328 7261 6e67 6528 6c65 6e28 6467 2929  s(range(len(dg))
+00001ea0: 2c20 6467 2e69 6e64 6578 2c20 726f 7461  , dg.index, rota
+00001eb0: 7469 6f6e 3d27 7665 7274 6963 616c 2729  tion='vertical')
+00001ec0: 0d0a 2020 2020 706c 742e 7469 636b 5f70  ..    plt.tick_p
+00001ed0: 6172 616d 7328 6178 6973 3d27 7827 2c20  arams(axis='x', 
+00001ee0: 726f 7461 7469 6f6e 3d39 302c 206c 6162  rotation=90, lab
+00001ef0: 656c 7369 7a65 3d31 3029 0d0a 2020 2020  elsize=10)..    
+00001f00: 706c 742e 7469 636b 5f70 6172 616d 7328  plt.tick_params(
+00001f10: 6178 6973 3d27 7927 2c6c 6162 656c 7369  axis='y',labelsi
+00001f20: 7a65 3d31 3029 0d0a 2020 2020 0d0a 2020  ze=10)..    ..  
+00001f30: 2020 6966 2074 7970 655f 7365 6a6f 7572    if type_sejour
+00001f40: 203d 3d20 2752 414e 444f 4e4e 4545 273a   == 'RANDONNEE':
+00001f50: 0d0a 2020 2020 2020 2020 5f20 3d20 706c  ..        _ = pl
+00001f60: 742e 7469 746c 6528 6627 2320 7261 6e64  t.title(f'# rand
+00001f70: 6f73 203a 207b 6c65 6e28 6467 297d 202c  os : {len(dg)} ,
+00001f80: 2023 2070 6172 7469 6369 7061 6e74 7320   # participants 
+00001f90: 3a20 7b73 756d 2864 6729 7d2c 2043 6fc3  : {sum(dg)}, Co.
+00001fa0: bb74 203a 207b 636f 7574 5f74 6f74 616c  .t : {cout_total
+00001fb0: 5f72 616e 646f 7d20 e282 ac27 290d 0a20  _rando} ...').. 
+00001fc0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00001fd0: 2020 5f20 3d20 706c 742e 7469 746c 6528    _ = plt.title(
+00001fe0: 6627 2320 7365 6a6f 7572 7320 3a20 7b6c  f'# sejours : {l
+00001ff0: 656e 2864 6729 7d20 2c20 2320 7061 7274  en(dg)} , # part
+00002000: 6963 6970 616e 7473 203a 207b 7375 6d28  icipants : {sum(
+00002010: 6467 297d 2c20 436f c3bb 7420 3a20 7b63  dg)}, Co..t : {c
+00002020: 6f75 745f 746f 7461 6c5f 7261 6e64 6f7d  out_total_rando}
+00002030: 20e2 82ac 2729 2020 2020 0d0a 2020 2020   ...')    ..    
+00002040: 706c 742e 7469 6768 745f 6c61 796f 7574  plt.tight_layout
+00002050: 2829 0d0a 2020 2020 706c 742e 7368 6f77  ()..    plt.show
+00002060: 2829 0d0a 2020 2020 0d0a 6465 6620 6e62  ()..    ..def nb
+00002070: 725f 7365 6a6f 7572 735f 6164 6865 7265  r_sejours_adhere
+00002080: 6e74 2879 6561 722c 2063 7467 5f70 6174  nt(year, ctg_pat
+00002090: 6829 3a0d 0a0d 0a20 2020 2023 2053 7461  h):....    # Sta
+000020a0: 6e64 6172 6420 6c69 6272 6172 7920 696d  ndard library im
+000020b0: 706f 7274 730d 0a20 2020 2066 726f 6d20  ports..    from 
+000020c0: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
+000020d0: 7274 2043 6f75 6e74 6572 0d0a 2020 2020  rt Counter..    
+000020e0: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
+000020f0: 6f72 7420 5061 7468 0d0a 2020 2020 0d0a  ort Path..    ..
+00002100: 2020 2020 2320 5468 6972 6420 7061 7274      # Third part
+00002110: 7920 696d 706f 7274 730d 0a20 2020 2069  y imports..    i
+00002120: 6d70 6f72 7420 6d61 7470 6c6f 746c 6962  mport matplotlib
+00002130: 2e70 7970 6c6f 7420 6173 2070 6c74 0d0a  .pyplot as plt..
+00002140: 2020 2020 696d 706f 7274 2070 616e 6461      import panda
+00002150: 7320 6173 2070 640d 0a20 2020 200d 0a20  s as pd..    .. 
+00002160: 2020 2070 6c74 2e73 7479 6c65 2e75 7365     plt.style.use
+00002170: 2827 6767 706c 6f74 2729 0d0a 2020 2020  ('ggplot')..    
+00002180: 0d0a 2020 2020 2320 6675 6e63 7469 6f6e  ..    # function
+00002190: 2074 6f20 6164 6420 7661 6c75 6520 6c61   to add value la
+000021a0: 6265 6c73 0d0a 2020 2020 6465 6620 6164  bels..    def ad
+000021b0: 646c 6162 656c 7328 782c 7929 3a0d 0a20  dlabels(x,y):.. 
+000021c0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000021d0: 7261 6e67 6528 6c65 6e28 7829 293a 0d0a  range(len(x)):..
+000021e0: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+000021f0: 7465 7874 2878 5b69 5d2d 302e 322c 795b  text(x[i]-0.2,y[
+00002200: 695d 2b31 2c79 5b69 5d2c 7369 7a65 3d6c  i]+1,y[i],size=l
+00002210: 6162 656c 5f73 697a 6529 0d0a 2020 2020  abel_size)..    
+00002220: 6c61 6265 6c5f 7369 7a65 203d 2031 350d  label_size = 15.
+00002230: 0a20 2020 2066 696c 655f 696e 203d 2063  .    file_in = c
+00002240: 7467 5f70 6174 6820 2f20 5061 7468 2873  tg_path / Path(s
+00002250: 7472 2879 6561 7229 2920 2f20 5061 7468  tr(year)) / Path
+00002260: 2827 5354 4154 4953 5449 5155 4553 2729  ('STATISTIQUES')
+00002270: 202f 2050 6174 6828 2773 796e 7468 6573   / Path('synthes
+00002280: 655f 6164 6865 7265 6e74 2e78 6c73 7827  e_adherent.xlsx'
+00002290: 290d 0a20 2020 2064 665f 746f 7461 6c20  )..    df_total 
+000022a0: 3d20 7064 2e72 6561 645f 6578 6365 6c28  = pd.read_excel(
+000022b0: 6669 6c65 5f69 6e29 0d0a 2020 2020 0d0a  file_in)..    ..
+000022c0: 2020 2020 6320 3d20 436f 756e 7465 7228      c = Counter(
+000022d0: 290d 0a20 2020 2063 203d 2043 6f75 6e74  )..    c = Count
+000022e0: 6572 2864 665f 746f 7461 6c5b 274e 6272  er(df_total['Nbr
+000022f0: 5f53 454a 4f55 5253 275d 2e74 6f6c 6973  _SEJOURS'].tolis
+00002300: 7428 2929 0d0a 2020 2020 6320 3d20 632e  t())..    c = c.
+00002310: 6d6f 7374 5f63 6f6d 6d6f 6e28 290d 0a0d  most_common()...
+00002320: 0a20 2020 2078 2c20 7920 3d20 7a69 7028  .    x, y = zip(
+00002330: 2a63 290d 0a20 2020 2078 203d 206c 6973  *c)..    x = lis
+00002340: 7428 7829 0d0a 2020 2020 7920 3d20 6c69  t(x)..    y = li
+00002350: 7374 2879 290d 0a20 2020 200d 0a20 2020  st(y)..    ..   
+00002360: 2066 6967 2c20 6178 203d 2070 6c74 2e73   fig, ax = plt.s
+00002370: 7562 706c 6f74 7328 6669 6773 697a 653d  ubplots(figsize=
+00002380: 2835 2c35 2929 0d0a 2020 2020 706c 742e  (5,5))..    plt.
+00002390: 6261 7228 5b73 7472 2878 5f73 2920 666f  bar([str(x_s) fo
+000023a0: 7220 785f 7320 696e 2078 5d2c 7929 0d0a  r x_s in x],y)..
+000023b0: 2020 2020 706c 742e 786c 6162 656c 2827      plt.xlabel('
+000023c0: 4e6f 6d62 7265 2064 6520 7061 7274 6963  Nombre de partic
+000023d0: 6970 6174 696f 6e20 c3a0 2064 6573 2073  ipation .. des s
+000023e0: c3a9 6a6f 7572 7327 290d 0a20 2020 2070  ..jours')..    p
+000023f0: 6c74 2e79 6c61 6265 6c28 274e 6f6d 6272  lt.ylabel('Nombr
+00002400: 6520 6465 206c 6963 656e 6369 6572 7327  e de licenciers'
+00002410: 290d 0a20 2020 2070 6c74 2e74 6963 6b5f  )..    plt.tick_
+00002420: 7061 7261 6d73 2861 7869 733d 2778 272c  params(axis='x',
+00002430: 206c 6162 656c 7369 7a65 3d6c 6162 656c   labelsize=label
+00002440: 5f73 697a 6529 0d0a 2020 2020 706c 742e  _size)..    plt.
+00002450: 7469 636b 5f70 6172 616d 7328 6178 6973  tick_params(axis
+00002460: 3d27 7927 2c20 6c61 6265 6c73 697a 653d  ='y', labelsize=
+00002470: 6c61 6265 6c5f 7369 7a65 290d 0a20 2020  label_size)..   
+00002480: 2070 6c74 2e74 6974 6c65 2873 7472 2879   plt.title(str(y
+00002490: 6561 7229 2c70 6164 3d32 302c 2066 6f6e  ear),pad=20, fon
+000024a0: 7473 697a 653d 3230 290d 0a20 2020 200d  tsize=20)..    .
+000024b0: 0a20 2020 2061 782e 7365 745f 786c 6162  .    ax.set_xlab
+000024c0: 656c 2827 4e20 73c3 a96a 6f75 7273 272c  el('N s..jours',
+000024d0: 2066 6f6e 7473 697a 6520 3d20 6c61 6265   fontsize = labe
+000024e0: 6c5f 7369 7a65 290d 0a20 2020 2061 782e  l_size)..    ax.
+000024f0: 7365 745f 796c 6162 656c 2827 4e6f 6d62  set_ylabel('Nomb
+00002500: 7265 2064 6520 4354 4720 6179 616e 7420  re de CTG ayant 
+00002510: 5c6e 2070 6172 7469 6369 70c3 a920 c3a0  \n particip.. ..
+00002520: 204e 2073 c3a9 6a6f 7572 7327 2c20 666f   N s..jours', fo
+00002530: 6e74 7369 7a65 203d 206c 6162 656c 5f73  ntsize = label_s
+00002540: 697a 6529 0d0a 2020 2020 0d0a 2020 2020  ize)..    ..    
+00002550: 782e 736f 7274 2829 0d0a 2020 2020 6164  x.sort()..    ad
+00002560: 646c 6162 656c 7328 782c 7929 0d0a 2020  dlabels(x,y)..  
+00002570: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
+00002580: 7574 2829 0d0a 2020 2020 706c 742e 7368  ut()..    plt.sh
+00002590: 6f77 2829 0d0a 0d0a 2020 2020 6669 675f  ow()....    fig_
+000025a0: 6669 6c65 203d 2027 5345 4a4f 5552 535f  file = 'SEJOURS_
+000025b0: 5354 4154 5f50 4152 5449 4349 5041 5449  STAT_PARTICIPATI
+000025c0: 4f4e 2e70 6e67 270d 0a20 2020 2070 6c74  ON.png'..    plt
+000025d0: 2e73 6176 6566 6967 2863 7467 5f70 6174  .savefig(ctg_pat
+000025e0: 6820 2f20 5061 7468 2873 7472 2879 6561  h / Path(str(yea
+000025f0: 7229 2920 2f20 5061 7468 2827 5354 4154  r)) / Path('STAT
+00002600: 4953 5449 5155 4553 2729 202f 2050 6174  ISTIQUES') / Pat
+00002610: 6828 6669 675f 6669 6c65 292c 6262 6f78  h(fig_file),bbox
+00002620: 5f69 6e63 6865 733d 2774 6967 6874 2729  _inches='tight')
+00002630: 0d0a 2020 2020 0d0a 6465 6620 7265 6164  ..    ..def read
+00002640: 5f6d 656d 6f72 795f 736f 7274 6965 7328  _memory_sorties(
+00002650: 293a 0d0a 0d0a 2020 2020 2320 5374 616e  ):....    # Stan
+00002660: 6461 7264 206c 6962 7261 7279 2069 6d70  dard library imp
+00002670: 6f72 7473 0d0a 2020 2020 696d 706f 7274  orts..    import
+00002680: 206f 732e 7061 7468 0d0a 2020 2020 6672   os.path..    fr
+00002690: 6f6d 2070 6174 686c 6962 2069 6d70 6f72  om pathlib impor
+000026a0: 7420 5061 7468 0d0a 0d0a 2020 2020 2320  t Path....    # 
+000026b0: 3372 6420 7061 7274 7920 696d 706f 7274  3rd party import
+000026c0: 730d 0a20 2020 2069 6d70 6f72 7420 7961  s..    import ya
+000026d0: 6d6c 0d0a 2020 2020 0d0a 2020 2020 2320  ml..    ..    # 
+000026e0: 5265 6164 7320 7468 6520 6465 6661 756c  Reads the defaul
+000026f0: 7420 5056 6368 6172 6163 7465 7269 7a61  t PVcharacteriza
+00002700: 7469 6f6e 2e79 616d 6c20 636f 6e66 6967  tion.yaml config
+00002710: 2066 696c 650d 0a20 2020 2070 6174 685f   file..    path_
+00002720: 636f 6e66 6967 5f66 696c 6520 3d20 5061  config_file = Pa
+00002730: 7468 285f 5f66 696c 655f 5f29 2e70 6172  th(__file__).par
+00002740: 656e 742e 7061 7265 6e74 202f 2050 6174  ent.parent / Pat
+00002750: 6828 2743 5447 5f46 756e 6327 2920 2f20  h('CTG_Func') / 
+00002760: 5061 7468 2827 4354 475f 5265 6646 696c  Path('CTG_RefFil
+00002770: 6573 2729 202f 2050 6174 6828 276d 656d  es') / Path('mem
+00002780: 6f72 795f 736f 7274 6965 732e 796d 6c27  ory_sorties.yml'
+00002790: 290d 0a20 2020 2077 6974 6820 6f70 656e  )..    with open
+000027a0: 2870 6174 685f 636f 6e66 6967 5f66 696c  (path_config_fil
+000027b0: 6529 2061 7320 6669 6c65 3a0d 0a20 2020  e) as file:..   
+000027c0: 2020 2020 206d 656d 6f72 7920 3d20 7961       memory = ya
+000027d0: 6d6c 2e73 6166 655f 6c6f 6164 2866 696c  ml.safe_load(fil
+000027e0: 6529 0d0a 2020 2020 2020 2020 0d0a 2020  e)..        ..  
+000027f0: 2020 2020 200d 0a20 2020 2072 6574 7572       ..    retur
+00002800: 6e20 6d65 6d6f 7279 0d0a 2020 2020 0d0a  n memory..    ..
+00002810: 6465 6620 6576 6f6c 7574 696f 6e5f 736f  def evolution_so
+00002820: 7274 6965 7328 7479 7065 2c63 7467 5f70  rties(type,ctg_p
+00002830: 6174 6829 3a0d 0a0d 0a20 2020 2023 2053  ath):....    # S
+00002840: 7461 6e64 6172 6420 6c69 6272 6172 7920  tandard library 
+00002850: 696d 706f 7274 2020 2020 0d0a 2020 2020  import    ..    
+00002860: 696d 706f 7274 2064 6174 6574 696d 650d  import datetime.
+00002870: 0a20 2020 2066 726f 6d20 7061 7468 6c69  .    from pathli
+00002880: 6220 696d 706f 7274 2050 6174 680d 0a20  b import Path.. 
+00002890: 2020 2066 726f 6d20 636f 6c6c 6563 7469     from collecti
+000028a0: 6f6e 7320 696d 706f 7274 206e 616d 6564  ons import named
+000028b0: 7475 706c 650d 0a0d 0a20 2020 2023 2054  tuple....    # T
+000028c0: 6869 7264 2070 6172 7479 206c 6962 7261  hird party libra
+000028d0: 7279 2069 6d70 6f72 7420 2020 2020 0d0a  ry import     ..
+000028e0: 2020 2020 696d 706f 7274 206d 6174 706c      import matpl
+000028f0: 6f74 6c69 622e 7079 706c 6f74 2061 7320  otlib.pyplot as 
+00002900: 706c 740d 0a20 2020 2069 6d70 6f72 7420  plt..    import 
+00002910: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
+00002920: 2020 2020 0d0a 2020 2020 2320 496e 7465      ..    # Inte
+00002930: 726e 616c 2069 6d70 6f72 740d 0a20 2020  rnal import..   
+00002940: 2069 6d70 6f72 7420 4354 475f 5574 696c   import CTG_Util
+00002950: 7320 6173 2063 7467 0d0a 2020 2020 6672  s as ctg..    fr
+00002960: 6f6d 2043 5447 5f55 7469 6c73 2e43 5447  om CTG_Utils.CTG
+00002970: 5f47 5549 2e47 5549 5f47 6c6f 6261 6c73  _GUI.GUI_Globals
+00002980: 2069 6d70 6f72 7420 4143 5449 5649 5445   import ACTIVITE
+00002990: 5f4c 4953 5420 0d0a 2020 2020 0d0a 2020  _LIST ..    ..  
+000029a0: 2020 6465 6620 6164 645f 6d65 6d6f 7279    def add_memory
+000029b0: 2873 7461 745f 6469 632c 7965 6172 7329  (stat_dic,years)
+000029c0: 3a0d 0a20 2020 2020 2020 206d 656d 6f72  :..        memor
+000029d0: 7920 3d20 7265 6164 5f6d 656d 6f72 795f  y = read_memory_
+000029e0: 736f 7274 6965 7328 290d 0a20 2020 200d  sorties()..    .
+000029f0: 0a20 2020 200d 0a20 2020 2020 2020 2066  .    ..        f
+00002a00: 6f72 2079 6561 722c 7620 696e 206d 656d  or year,v in mem
+00002a10: 6f72 795b 276d 656d 6f72 7927 5d2e 6974  ory['memory'].it
+00002a20: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
 00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a50: 2020 2076 5b27 534f 5254 4945 535f 434c     v['SORTIES_CL
-00002a60: 5542 5f53 414d 4544 4927 5d2c 2020 2023  UB_SAMEDI'],   #
-00002a70: 2073 6f72 7469 655f 7361 6d65 6469 5f63   sortie_samedi_c
-00002a80: 6c75 620d 0a20 2020 2020 2020 2020 2020  lub..           
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ab0: 765b 2753 4f52 5449 4553 5f48 4956 4552  v['SORTIES_HIVER
-00002ac0: 275d 2c20 2020 2020 2020 2020 2320 736f  '],         # so
-00002ad0: 7274 6965 5f68 6976 6572 5f63 6c75 620d  rtie_hiver_club.
-00002ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00002a60: 2073 7461 745f 6469 635b 7374 7228 7965   stat_dic[str(ye
+00002a70: 6172 295d 203d 2073 7461 7479 6561 7228  ar)] = statyear(
+00002a80: 765b 2750 4152 5449 4349 5041 5449 4f4e  v['PARTICIPATION
+00002a90: 5f53 454a 4f55 5253 275d 2c20 2020 2020  _SEJOURS'],     
+00002aa0: 2020 2020 2020 2020 2020 2023 206e 6272             # nbr
+00002ab0: 5f73 656a 6f75 7273 0d0a 2020 2020 2020  _sejours..      
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ae0: 2020 2020 2030 2c20 2020 2020 2020 2020       0,         
 00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2020 2020 2020 2020 2020 2020 765b 2753              v['S
-00002b10: 4f52 5449 4553 5f43 4c55 425f 4a45 5544  ORTIES_CLUB_JEUD
-00002b20: 4927 5d2c 2020 2020 2320 736f 7274 6965  I'],    # sortie
-00002b30: 5f6a 6575 6469 5f63 6c75 620d 0a20 2020  _jeudi_club..   
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 2020 2020 2020 2020 765b 2752 414e 444f          v['RANDO
-00002b70: 4e4e 4545 5327 5d2c 2020 2020 2020 2020  NNEES'],        
-00002b80: 2020 2020 2320 7261 6e64 6f6e 6e65 650d      # randonnee.
-00002b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 2020 2020 2020 2020 2020 2020 765b 274e              v['N
-00002bc0: 6f6d 6272 655f 7365 6a6f 7572 7327 5d2c  ombre_sejours'],
-00002bd0: 2020 2020 2020 2020 2320 6e62 725f 7365          # nbr_se
-00002be0: 6a6f 7572 730d 0a20 2020 2020 2020 2020  jours..         
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 302c 2920 2020 2020 2020 2020 2020    0,)           
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00002c30: 6e62 725f 6a6f 7572 735f 7365 6a6f 7572  nbr_jours_sejour
-00002c40: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00002c80: 0a20 2020 2020 2020 2020 2020 2079 6561  .            yea
-00002c90: 7273 2e61 7070 656e 6428 7374 7228 7965  rs.append(str(ye
-00002ca0: 6172 2929 0d0a 2020 2020 2020 2020 2020  ar))..          
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-00002cd0: 6669 6c6c 5f73 7461 745f 7965 6172 2879  fill_stat_year(y
-00002ce0: 6561 7229 3a0d 0a20 2020 200d 0a20 2020  ear):..    ..   
-00002cf0: 2020 2020 2023 2049 6e74 6572 6e61 6c20       # Internal 
-00002d00: 6c69 6272 6172 7920 696d 706f 7274 730d  library imports.
-00002d10: 0a20 2020 2020 2020 2066 726f 6d20 4354  .        from CT
-00002d20: 475f 5574 696c 732e 4354 475f 4675 6e63  G_Utils.CTG_Func
-00002d30: 2e43 5447 5f75 7469 6c69 7479 2069 6d70  .CTG_utility imp
-00002d40: 6f72 7420 6765 745f 7365 6a6f 7572 5f69  ort get_sejour_i
-00002d50: 6e66 6f0d 0a20 2020 2020 2020 200d 0a20  nfo..        .. 
-00002d60: 2020 2020 2020 2073 656a 6f75 725f 696e         sejour_in
-00002d70: 666f 203d 2067 6574 5f73 656a 6f75 725f  fo = get_sejour_
-00002d80: 696e 666f 2863 7467 5f70 6174 682c 7965  info(ctg_path,ye
-00002d90: 6172 290d 0a20 2020 2020 2020 200d 0a20  ar)..        .. 
-00002da0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002db0: 2066 696c 655f 696e 203d 2063 7467 5f70   file_in = ctg_p
-00002dc0: 6174 6820 2f20 5061 7468 2873 7472 2879  ath / Path(str(y
-00002dd0: 6561 7229 2920 2f20 5061 7468 2827 5354  ear)) / Path('ST
-00002de0: 4154 4953 5449 5155 4553 2729 202f 2050  ATISTIQUES') / P
-00002df0: 6174 6828 2773 796e 7468 6573 655f 6164  ath('synthese_ad
-00002e00: 6865 7265 6e74 2e78 6c73 7827 290d 0a20  herent.xlsx').. 
-00002e10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002e20: 2064 6620 3d20 7064 2e72 6561 645f 6578   df = pd.read_ex
-00002e30: 6365 6c28 6669 6c65 5f69 6e29 0d0a 2020  cel(file_in)..  
-00002e40: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002e50: 7374 6174 5f79 6561 7220 3d20 7374 6174  stat_year = stat
-00002e60: 7965 6172 2864 665b 274e 6272 5f53 454a  year(df['Nbr_SEJ
-00002e70: 4f55 5253 275d 2e73 756d 2829 2c20 2020  OURS'].sum(),   
-00002e80: 2020 2020 2020 2020 2020 2320 6e62 725f            # nbr_
-00002e90: 6a6f 7572 735f 7061 7274 6963 6970 6174  jours_participat
-00002ea0: 696f 6e5f 7365 6a6f 7572 730d 0a20 2020  ion_sejours..   
-00002eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ec0: 2020 2020 2020 2020 2020 6466 5b27 5345            df['SE
-00002ed0: 4a4f 5552 2d4a 4f55 5227 5d2e 7375 6d28  JOUR-JOUR'].sum(
-00002ee0: 292c 2020 2020 2020 2020 2020 2020 2023  ),             #
-00002ef0: 206e 6272 5f70 6172 7469 6369 7061 7469   nbr_participati
-00002f00: 6f6e 735f 7365 6a6f 7572 0d0a 2020 2020  ons_sejour..    
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2020 2020 2020 2020 2064 665b 2753 4f52           df['SOR
-00002f30: 5449 4520 4455 2044 494d 414e 4348 4520  TIE DU DIMANCHE 
-00002f40: 434c 5542 275d 2e73 756d 2829 2c20 2320  CLUB'].sum(), # 
-00002f50: 736f 7274 6965 5f64 696d 616e 6368 655f  sortie_dimanche_
-00002f60: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
-00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f80: 2020 2064 665b 2753 4f52 5449 4520 4455     df['SORTIE DU
-00002f90: 2053 414d 4544 4920 434c 5542 275d 2e73   SAMEDI CLUB'].s
-00002fa0: 756d 2829 2c20 2020 2320 736f 7274 6965  um(),   # sortie
-00002fb0: 5f73 616d 6564 695f 636c 7562 0d0a 2020  _samedi_club..  
-00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fd0: 2020 2020 2020 2020 2020 2064 665b 2753             df['S
-00002fe0: 4f52 5449 4520 4849 5645 5227 5d2e 7375  ORTIE HIVER'].su
-00002ff0: 6d28 292c 2020 2020 2020 2020 2020 2020  m(),            
-00003000: 2320 736f 7274 6965 5f68 6976 6572 5f63  # sortie_hiver_c
-00003010: 6c75 620d 0a20 2020 2020 2020 2020 2020  lub..           
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 2020 6466 5b27 534f 5254 4945 2044 5520    df['SORTIE DU 
-00003040: 4a45 5544 4920 434c 5542 275d 2e73 756d  JEUDI CLUB'].sum
-00003050: 2829 2c20 2020 2023 2073 6f72 7469 655f  (),    # sortie_
-00003060: 6a65 7564 695f 636c 7562 0d0a 2020 2020  jeudi_club..    
-00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003080: 2020 2020 2020 2020 2064 665b 2752 414e           df['RAN
-00003090: 444f 4e4e 4545 275d 2e73 756d 2829 2c20  DONNEE'].sum(), 
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000030b0: 7261 6e64 6f6e 6e65 650d 0a20 2020 2020  randonnee..     
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 2020 2020 2020 2020 7365 6a6f 7572 5f69          sejour_i
-000030e0: 6e66 6f2e 6e62 725f 7365 6a6f 7572 732c  nfo.nbr_sejours,
-000030f0: 2020 2020 2020 2020 2020 2020 2023 206e               # n
-00003100: 6272 5f73 656a 6f75 7273 200d 0a20 2020  br_sejours ..   
+00002b00: 2023 206a 6f75 7273 5f73 656a 6f75 720d   # jours_sejour.
+00002b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b30: 2020 2020 2020 2020 2020 2020 765b 2753              v['S
+00002b40: 4f52 5449 4553 5f43 4c55 425f 4449 4d41  ORTIES_CLUB_DIMA
+00002b50: 4e43 4845 275d 2c20 2320 736f 7274 6965  NCHE'], # sortie
+00002b60: 5f64 696d 616e 6368 655f 636c 7562 0d0a  _dimanche_club..
+00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2020 2020 2020 2020 2076 5b27 534f             v['SO
+00002ba0: 5254 4945 535f 434c 5542 5f53 414d 4544  RTIES_CLUB_SAMED
+00002bb0: 4927 5d2c 2020 2023 2073 6f72 7469 655f  I'],   # sortie_
+00002bc0: 7361 6d65 6469 5f63 6c75 620d 0a20 2020  samedi_club..   
+00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2020 2020 2020 765b 2753 4f52 5449          v['SORTI
+00002c00: 4553 5f48 4956 4552 275d 2c20 2020 2020  ES_HIVER'],     
+00002c10: 2020 2020 2320 736f 7274 6965 5f68 6976      # sortie_hiv
+00002c20: 6572 5f63 6c75 620d 0a20 2020 2020 2020  er_club..       
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c50: 2020 2020 765b 2753 4f52 5449 4553 5f43      v['SORTIES_C
+00002c60: 4c55 425f 4a45 5544 4927 5d2c 2020 2020  LUB_JEUDI'],    
+00002c70: 2320 736f 7274 6965 5f6a 6575 6469 5f63  # sortie_jeudi_c
+00002c80: 6c75 620d 0a20 2020 2020 2020 2020 2020  lub..           
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cb0: 765b 2752 414e 444f 4e4e 4545 5327 5d2c  v['RANDONNEES'],
+00002cc0: 2020 2020 2020 2020 2020 2020 2320 7261              # ra
+00002cd0: 6e64 6f6e 6e65 650d 0a20 2020 2020 2020  ndonnee..       
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 2020 2020 765b 274e 6f6d 6272 655f 7365      v['Nombre_se
+00002d10: 6a6f 7572 7327 5d2c 2020 2020 2020 2020  jours'],        
+00002d20: 2320 6e62 725f 7365 6a6f 7572 730d 0a20  # nbr_sejours.. 
+00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d50: 2020 2020 2020 2020 2020 302c 2920 2020            0,)   
+00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d70: 2020 2020 2020 2320 6e62 725f 6a6f 7572        # nbr_jour
+00002d80: 735f 7365 6a6f 7572 730d 0a20 2020 2020  s_sejours..     
+00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002dd0: 2020 2020 2079 6561 7273 2e61 7070 656e       years.appen
+00002de0: 6428 7374 7228 7965 6172 2929 0d0a 2020  d(str(year))..  
+00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e00: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00002e10: 2020 2020 6465 6620 6669 6c6c 5f73 7461      def fill_sta
+00002e20: 745f 7965 6172 2879 6561 7229 3a0d 0a20  t_year(year):.. 
+00002e30: 2020 200d 0a20 2020 2020 2020 2023 2049     ..        # I
+00002e40: 6e74 6572 6e61 6c20 6c69 6272 6172 7920  nternal library 
+00002e50: 696d 706f 7274 730d 0a20 2020 2020 2020  imports..       
+00002e60: 2066 726f 6d20 4354 475f 5574 696c 732e   from CTG_Utils.
+00002e70: 4354 475f 4675 6e63 2e43 5447 5f75 7469  CTG_Func.CTG_uti
+00002e80: 6c69 7479 2069 6d70 6f72 7420 6765 745f  lity import get_
+00002e90: 7365 6a6f 7572 5f69 6e66 6f0d 0a20 2020  sejour_info..   
+00002ea0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+00002eb0: 656a 6f75 725f 696e 666f 203d 2067 6574  ejour_info = get
+00002ec0: 5f73 656a 6f75 725f 696e 666f 2863 7467  _sejour_info(ctg
+00002ed0: 5f70 6174 682c 7965 6172 290d 0a20 2020  _path,year)..   
+00002ee0: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
+00002ef0: 0a20 2020 2020 2020 2066 696c 655f 696e  .        file_in
+00002f00: 203d 2063 7467 5f70 6174 6820 2f20 5061   = ctg_path / Pa
+00002f10: 7468 2873 7472 2879 6561 7229 2920 2f20  th(str(year)) / 
+00002f20: 5061 7468 2827 5354 4154 4953 5449 5155  Path('STATISTIQU
+00002f30: 4553 2729 202f 2050 6174 6828 2773 796e  ES') / Path('syn
+00002f40: 7468 6573 655f 6164 6865 7265 6e74 2e78  these_adherent.x
+00002f50: 6c73 7827 290d 0a20 2020 2020 2020 200d  lsx')..        .
+00002f60: 0a20 2020 2020 2020 2064 6620 3d20 7064  .        df = pd
+00002f70: 2e72 6561 645f 6578 6365 6c28 6669 6c65  .read_excel(file
+00002f80: 5f69 6e29 0d0a 2020 2020 2020 2020 0d0a  _in)..        ..
+00002f90: 2020 2020 2020 2020 7374 6174 5f79 6561          stat_yea
+00002fa0: 7220 3d20 7374 6174 7965 6172 2864 665b  r = statyear(df[
+00002fb0: 274e 6272 5f53 454a 4f55 5253 275d 2e73  'Nbr_SEJOURS'].s
+00002fc0: 756d 2829 2c20 2020 2020 2020 2020 2020  um(),           
+00002fd0: 2020 2320 6e62 725f 6a6f 7572 735f 7061    # nbr_jours_pa
+00002fe0: 7274 6963 6970 6174 696f 6e5f 7365 6a6f  rticipation_sejo
+00002ff0: 7572 730d 0a20 2020 2020 2020 2020 2020  urs..           
+00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003010: 2020 6466 5b27 5345 4a4f 5552 2d4a 4f55    df['SEJOUR-JOU
+00003020: 5227 5d2e 7375 6d28 292c 2020 2020 2020  R'].sum(),      
+00003030: 2020 2020 2020 2023 206e 6272 5f70 6172         # nbr_par
+00003040: 7469 6369 7061 7469 6f6e 735f 7365 6a6f  ticipations_sejo
+00003050: 7572 0d0a 2020 2020 2020 2020 2020 2020  ur..            
+00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003070: 2064 665b 2753 4f52 5449 4520 4455 2044   df['SORTIE DU D
+00003080: 494d 414e 4348 4520 434c 5542 275d 2e73  IMANCHE CLUB'].s
+00003090: 756d 2829 2c20 2320 736f 7274 6965 5f64  um(), # sortie_d
+000030a0: 696d 616e 6368 655f 636c 7562 0d0a 2020  imanche_club..  
+000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030c0: 2020 2020 2020 2020 2020 2064 665b 2753             df['S
+000030d0: 4f52 5449 4520 4455 2053 414d 4544 4920  ORTIE DU SAMEDI 
+000030e0: 434c 5542 275d 2e73 756d 2829 2c20 2020  CLUB'].sum(),   
+000030f0: 2320 736f 7274 6965 5f73 616d 6564 695f  # sortie_samedi_
+00003100: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
 00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003120: 2020 2020 2020 2020 2020 7365 6a6f 7572            sejour
-00003130: 5f69 6e66 6f2e 6e62 725f 6a6f 7572 7329  _info.nbr_jours)
-00003140: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00003150: 206e 6272 5f6a 6f75 7273 5f73 656a 6f75   nbr_jours_sejou
-00003160: 7273 2020 2020 2020 2020 2020 2020 2020  rs              
-00003170: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00003180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003190: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000031a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000031b0: 7374 6174 5f79 6561 720d 0a20 2020 200d  stat_year..    .
-000031c0: 0a20 2020 2064 6566 2061 6464 6c61 6265  .    def addlabe
-000031d0: 6c73 2878 2c79 2c6f 6666 7365 7429 3a0d  ls(x,y,offset):.
-000031e0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-000031f0: 6e20 7261 6e67 6528 6c65 6e28 7829 293a  n range(len(x)):
-00003200: 0d0a 2020 2020 2020 2020 2020 2020 706c  ..            pl
-00003210: 742e 7465 7874 2878 5b69 5d2c 795b 695d  t.text(x[i],y[i]
-00003220: 2b6f 6666 7365 742c 726f 756e 6428 795b  +offset,round(y[
-00003230: 695d 2c31 292c 7369 7a65 3d31 3029 0d0a  i],1),size=10)..
-00003240: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00003250: 2020 6465 6620 706c 6f74 5f73 7461 7428    def plot_stat(
-00003260: 7965 6172 732c 6e62 5f70 6172 7469 6369  years,nb_partici
-00003270: 7061 6e74 732c 7469 746c 652c 6c61 6265  pants,title,labe
-00003280: 6c5f 7929 3a0d 0a20 2020 2020 2020 2070  l_y):..        p
-00003290: 6c74 2e66 6967 7572 6528 6669 6773 697a  lt.figure(figsiz
-000032a0: 653d 2838 2c20 3629 290d 0a20 2020 2020  e=(8, 6))..     
-000032b0: 2020 2063 6f6c 6f72 7320 3d20 5b27 2366     colors = ['#f
-000032c0: 6461 6134 3827 5d20 0d0a 2020 2020 2020  daa48'] ..      
-000032d0: 2020 7369 7a65 5f6c 6162 656c 203d 2032    size_label = 2
-000032e0: 300d 0a20 2020 2020 2020 2070 6c74 2e62  0..        plt.b
-000032f0: 6172 2879 6561 7273 2c6e 625f 7061 7274  ar(years,nb_part
-00003300: 6963 6970 616e 7473 2c63 6f6c 6f72 3d63  icipants,color=c
-00003310: 6f6c 6f72 7329 0d0a 2020 2020 2020 2020  olors)..        
-00003320: 706c 742e 796c 6162 656c 286c 6162 656c  plt.ylabel(label
-00003330: 5f79 2c73 697a 653d 7369 7a65 5f6c 6162  _y,size=size_lab
-00003340: 656c 290d 0a20 2020 2020 2020 2061 6464  el)..        add
-00003350: 6c61 6265 6c73 2879 6561 7273 2c6e 625f  labels(years,nb_
-00003360: 7061 7274 6963 6970 616e 7473 2c31 290d  participants,1).
-00003370: 0a20 2020 2020 2020 2070 6c74 2e78 7469  .        plt.xti
-00003380: 636b 7328 726f 7461 7469 6f6e 3d39 3029  cks(rotation=90)
-00003390: 0d0a 2020 2020 2020 2020 706c 742e 7469  ..        plt.ti
-000033a0: 636b 5f70 6172 616d 7328 6178 6973 3d27  ck_params(axis='
-000033b0: 7827 2c20 6c61 6265 6c73 697a 653d 7369  x', labelsize=si
-000033c0: 7a65 5f6c 6162 656c 290d 0a20 2020 2020  ze_label)..     
-000033d0: 2020 2070 6c74 2e74 6963 6b5f 7061 7261     plt.tick_para
-000033e0: 6d73 2861 7869 733d 2779 272c 206c 6162  ms(axis='y', lab
-000033f0: 656c 7369 7a65 3d73 697a 655f 6c61 6265  elsize=size_labe
-00003400: 6c29 0d0a 2020 2020 2020 2020 706c 742e  l)..        plt.
-00003410: 7469 746c 6528 7469 746c 652c 666f 6e74  title(title,font
-00003420: 7369 7a65 3d31 3829 0d0a 2020 2020 2020  size=18)..      
-00003430: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
-00003440: 7574 2829 0d0a 2020 2020 2020 2020 706c  ut()..        pl
-00003450: 742e 7368 6f77 2829 0d0a 2020 2020 0d0a  t.show()..    ..
-00003460: 2020 2020 7374 6174 7965 6172 203d 206e      statyear = n
-00003470: 616d 6564 7475 706c 6528 2761 6374 6976  amedtuple('activ
-00003480: 6974 6527 2c20 4143 5449 5649 5445 5f4c  ite', ACTIVITE_L
-00003490: 4953 5429 0d0a 200d 0a20 2020 2070 6c74  IST).. ..    plt
-000034a0: 2e73 7479 6c65 2e75 7365 2827 6767 706c  .style.use('ggpl
-000034b0: 6f74 2729 0d0a 2020 2020 7965 6172 7320  ot')..    years 
-000034c0: 3d20 5b5d 0d0a 2020 2020 7374 6174 5f64  = []..    stat_d
-000034d0: 6963 203d 207b 7d0d 0a20 2020 2061 6464  ic = {}..    add
-000034e0: 5f6d 656d 6f72 7928 7374 6174 5f64 6963  _memory(stat_dic
-000034f0: 2c79 6561 7273 290d 0a0d 0a20 2020 2074  ,years)....    t
-00003500: 6f64 6179 203d 2064 6174 6574 696d 652e  oday = datetime.
-00003510: 6461 7465 7469 6d65 2e6e 6f77 2829 0d0a  datetime.now()..
-00003520: 2020 2020 7965 6172 735f 6e65 7720 3d20      years_new = 
-00003530: 5b73 7472 2879 6561 7229 2066 6f72 2079  [str(year) for y
-00003540: 6561 7220 696e 2072 616e 6765 2832 3032  ear in range(202
-00003550: 322c 746f 6461 792e 7965 6172 2b31 295d  2,today.year+1)]
-00003560: 0d0a 2020 2020 666f 7220 7965 6172 2069  ..    for year i
-00003570: 6e20 7965 6172 735f 6e65 773a 0d0a 2020  n years_new:..  
-00003580: 2020 2020 2020 7374 6174 5f64 6963 5b79        stat_dic[y
-00003590: 6561 725d 203d 2066 696c 6c5f 7374 6174  ear] = fill_stat
-000035a0: 5f79 6561 7228 7965 6172 290d 0a20 2020  _year(year)..   
-000035b0: 2020 2020 200d 0a20 2020 2079 6561 7273       ..    years
-000035c0: 203d 2079 6561 7273 202b 2079 6561 7273   = years + years
-000035d0: 5f6e 6577 2020 200d 0a20 2020 200d 0a20  _new   ..    .. 
-000035e0: 2020 200d 0a20 2020 2069 6620 7479 7065     ..    if type
-000035f0: 203d 3d20 276e 6272 5f6a 6f75 7273 5f70   == 'nbr_jours_p
-00003600: 6172 7469 6369 7061 7469 6f6e 5f73 656a  articipation_sej
-00003610: 6f75 7273 273a 0d0a 2020 2020 2020 2020  ours':..        
-00003620: 706c 6f74 5f73 7461 7428 7965 6172 732c  plot_stat(years,
-00003630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003640: 2020 2020 5b73 7461 745f 6469 635b 7965      [stat_dic[ye
-00003650: 6172 5d2e 6e62 725f 6a6f 7572 735f 7061  ar].nbr_jours_pa
-00003660: 7274 6963 6970 6174 696f 6e5f 7365 6a6f  rticipation_sejo
-00003670: 7572 7320 666f 7220 7965 6172 2069 6e20  urs for year in 
-00003680: 7965 6172 735d 2c0d 0a20 2020 2020 2020  years],..       
-00003690: 2020 2020 2020 2020 2020 2074 7970 652c             type,
-000036a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000036b0: 2020 2020 7479 7065 290d 0a20 2020 2065      type)..    e
-000036c0: 6c69 6620 2074 7970 6520 3d3d 2027 736f  lif  type == 'so
-000036d0: 7274 6965 5f64 696d 616e 6368 655f 636c  rtie_dimanche_cl
-000036e0: 7562 273a 0d0a 2020 2020 2020 2020 706c  ub':..        pl
-000036f0: 6f74 5f73 7461 7428 7965 6172 732c 0d0a  ot_stat(years,..
-00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003710: 2020 5b73 7461 745f 6469 635b 7965 6172    [stat_dic[year
-00003720: 5d2e 736f 7274 6965 5f64 696d 616e 6368  ].sortie_dimanch
-00003730: 655f 636c 7562 2066 6f72 2079 6561 7220  e_club for year 
-00003740: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
-00003750: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-00003760: 7065 2c0d 0a20 2020 2020 2020 2020 2020  pe,..           
-00003770: 2020 2020 2020 2027 2370 6172 7469 6369         '#partici
-00003780: 7061 6e74 7327 290d 0a20 2020 2065 6c69  pants')..    eli
-00003790: 6620 2074 7970 6520 3d3d 2027 736f 7274  f  type == 'sort
-000037a0: 6965 5f73 616d 6564 695f 636c 7562 273a  ie_samedi_club':
-000037b0: 0d0a 2020 2020 2020 2020 706c 6f74 5f73  ..        plot_s
-000037c0: 7461 7428 7965 6172 732c 0d0a 2020 2020  tat(years,..    
-000037d0: 2020 2020 2020 2020 2020 2020 2020 5b73                [s
-000037e0: 7461 745f 6469 635b 7965 6172 5d2e 736f  tat_dic[year].so
-000037f0: 7274 6965 5f73 616d 6564 695f 636c 7562  rtie_samedi_club
-00003800: 2066 6f72 2079 6561 7220 696e 2079 6561   for year in yea
-00003810: 7273 5d2c 0d0a 2020 2020 2020 2020 2020  rs],..          
-00003820: 2020 2020 2020 2020 7479 7065 2c0d 0a20          type,.. 
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2027 2370 6172 7469 6369 7061 6e74 7327   '#participants'
-00003850: 290d 0a20 2020 2065 6c69 6620 2074 7970  )..    elif  typ
-00003860: 6520 3d3d 2027 736f 7274 6965 5f6a 6575  e == 'sortie_jeu
-00003870: 6469 5f63 6c75 6227 3a0d 0a20 2020 2020  di_club':..     
-00003880: 2020 2070 6c6f 745f 7374 6174 2879 6561     plot_stat(yea
-00003890: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
-000038a0: 2020 2020 2020 205b 7374 6174 5f64 6963         [stat_dic
-000038b0: 5b79 6561 725d 2e73 6f72 7469 655f 6a65  [year].sortie_je
-000038c0: 7564 695f 636c 7562 2066 6f72 2079 6561  udi_club for yea
-000038d0: 7220 696e 2079 6561 7273 5d2c 0d0a 2020  r in years],..  
-000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038f0: 7479 7065 2c0d 0a20 2020 2020 2020 2020  type,..         
-00003900: 2020 2020 2020 2020 2027 2370 6172 7469           '#parti
-00003910: 6369 7061 6e74 7327 2920 200d 0a20 2020  cipants')  ..   
-00003920: 2065 6c69 6620 2074 7970 6520 3d3d 2027   elif  type == '
-00003930: 7261 6e64 6f6e 6e65 6527 3a0d 0a20 2020  randonnee':..   
-00003940: 2020 2020 2070 6c6f 745f 7374 6174 2879       plot_stat(y
-00003950: 6561 7273 2c0d 0a20 2020 2020 2020 2020  ears,..         
-00003960: 2020 2020 2020 2020 205b 7374 6174 5f64           [stat_d
-00003970: 6963 5b79 6561 725d 2e72 616e 646f 6e6e  ic[year].randonn
-00003980: 6565 2066 6f72 2079 6561 7220 696e 2079  ee for year in y
-00003990: 6561 7273 5d2c 0d0a 2020 2020 2020 2020  ears],..        
-000039a0: 2020 2020 2020 2020 2020 7479 7065 2c0d            type,.
-000039b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000039c0: 2020 2027 2370 6172 7469 6369 7061 6e74     '#participant
-000039d0: 7327 2920 200d 0a20 2020 2065 6c69 6620  s')  ..    elif 
-000039e0: 2074 7970 6520 3d3d 2027 6e62 725f 7061   type == 'nbr_pa
-000039f0: 7274 6963 6970 6174 696f 6e73 5f73 656a  rticipations_sej
-00003a00: 6f75 7273 273a 0d0a 2020 2020 2020 2020  ours':..        
-00003a10: 706c 6f74 5f73 7461 7428 7965 6172 732c  plot_stat(years,
-00003a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003a30: 2020 2020 5b73 7461 745f 6469 635b 7965      [stat_dic[ye
-00003a40: 6172 5d2e 6e62 725f 7061 7274 6963 6970  ar].nbr_particip
-00003a50: 6174 696f 6e73 5f73 656a 6f75 7273 2066  ations_sejours f
-00003a60: 6f72 2079 6561 7220 696e 2079 6561 7273  or year in years
-00003a70: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00003a80: 2020 2020 2020 274e 6f6d 6272 6520 6465        'Nombre de
-00003a90: 2070 6172 7469 6369 7061 7469 6f6e 7320   participations 
-00003aa0: 6175 7820 73c3 a96a 6f75 7273 272c 0d0a  aux s..jours',..
-00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ac0: 2020 2723 2070 6172 7469 6369 7061 7469    '# participati
-00003ad0: 6f6e 7320 6175 7820 73c3 a96a 6f75 7273  ons aux s..jours
-00003ae0: 2729 200d 0a20 2020 2065 6c69 6620 2074  ') ..    elif  t
-00003af0: 7970 6520 3d3d 2027 6e62 725f 7365 6a6f  ype == 'nbr_sejo
-00003b00: 7572 7327 3a0d 0a20 2020 2020 2020 2070  urs':..        p
-00003b10: 6c6f 745f 7374 6174 2879 6561 7273 2c0d  lot_stat(years,.
-00003b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003b30: 2020 205b 7374 6174 5f64 6963 5b79 6561     [stat_dic[yea
-00003b40: 725d 2e6e 6272 5f73 656a 6f75 7273 2066  r].nbr_sejours f
-00003b50: 6f72 2079 6561 7220 696e 2079 6561 7273  or year in years
-00003b60: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00003b70: 2020 2020 2020 274e 6f6d 6272 6520 6465        'Nombre de
-00003b80: 2073 c3a9 6a6f 7572 7327 2c0d 0a20 2020   s..jours',..   
-00003b90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00003ba0: 2320 73c3 a96a 6f75 7273 2729 0d0a 2020  # s..jours')..  
-00003bb0: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
-00003bc0: 276e 6272 5f6a 6f75 7273 5f73 656a 6f75  'nbr_jours_sejou
-00003bd0: 7273 273a 0d0a 2020 2020 2020 2020 706c  rs':..        pl
-00003be0: 6f74 5f73 7461 7428 7965 6172 732c 0d0a  ot_stat(years,..
-00003bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c00: 2020 5b73 7461 745f 6469 635b 7965 6172    [stat_dic[year
-00003c10: 5d2e 6e62 725f 6a6f 7572 735f 7365 6a6f  ].nbr_jours_sejo
-00003c20: 7572 7320 666f 7220 7965 6172 2069 6e20  urs for year in 
-00003c30: 7965 6172 735d 2c0d 0a20 2020 2020 2020  years],..       
-00003c40: 2020 2020 2020 2020 2020 2027 4e6f 6d62             'Nomb
-00003c50: 7265 2064 6520 6a6f 7572 7320 73c3 a96a  re de jours s..j
-00003c60: 6f75 7273 272c 0d0a 2020 2020 2020 2020  ours',..        
-00003c70: 2020 2020 2020 2020 2020 2723 206a 6f75            '# jou
-00003c80: 7273 2073 c3a9 6a6f 7572 2729 2020 2020  rs s..jour')    
-00003c90: 2020 2020                                    
+00003120: 2020 2064 665b 2753 4f52 5449 4520 4849     df['SORTIE HI
+00003130: 5645 5227 5d2e 7375 6d28 292c 2020 2020  VER'].sum(),    
+00003140: 2020 2020 2020 2020 2320 736f 7274 6965          # sortie
+00003150: 5f68 6976 6572 5f63 6c75 620d 0a20 2020  _hiver_club..   
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 2020 2020 2020 2020 2020 6466 5b27 534f            df['SO
+00003180: 5254 4945 2044 5520 4a45 5544 4920 434c  RTIE DU JEUDI CL
+00003190: 5542 275d 2e73 756d 2829 2c20 2020 2023  UB'].sum(),    #
+000031a0: 2073 6f72 7469 655f 6a65 7564 695f 636c   sortie_jeudi_cl
+000031b0: 7562 0d0a 2020 2020 2020 2020 2020 2020  ub..            
+000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031d0: 2064 665b 2752 414e 444f 4e4e 4545 275d   df['RANDONNEE']
+000031e0: 2e73 756d 2829 2c20 2020 2020 2020 2020  .sum(),         
+000031f0: 2020 2020 2020 2320 7261 6e64 6f6e 6e65        # randonne
+00003200: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003220: 7365 6a6f 7572 5f69 6e66 6f2e 6e62 725f  sejour_info.nbr_
+00003230: 7365 6a6f 7572 732c 2020 2020 2020 2020  sejours,        
+00003240: 2020 2020 2023 206e 6272 5f73 656a 6f75       # nbr_sejou
+00003250: 7273 200d 0a20 2020 2020 2020 2020 2020  rs ..           
+00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003270: 2020 7365 6a6f 7572 5f69 6e66 6f2e 6e62    sejour_info.nb
+00003280: 725f 6a6f 7572 7329 2020 2020 2020 2020  r_jours)        
+00003290: 2020 2020 2020 2023 206e 6272 5f6a 6f75         # nbr_jou
+000032a0: 7273 5f73 656a 6f75 7273 2020 2020 2020  rs_sejours      
+000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000032f0: 2072 6574 7572 6e20 7374 6174 5f79 6561   return stat_yea
+00003300: 720d 0a20 2020 200d 0a20 2020 2064 6566  r..    ..    def
+00003310: 2061 6464 6c61 6265 6c73 2878 2c79 2c6f   addlabels(x,y,o
+00003320: 6666 7365 7429 3a0d 0a20 2020 2020 2020  ffset):..       
+00003330: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00003340: 6c65 6e28 7829 293a 0d0a 2020 2020 2020  len(x)):..      
+00003350: 2020 2020 2020 706c 742e 7465 7874 2878        plt.text(x
+00003360: 5b69 5d2c 795b 695d 2b6f 6666 7365 742c  [i],y[i]+offset,
+00003370: 726f 756e 6428 795b 695d 2c31 292c 7369  round(y[i],1),si
+00003380: 7a65 3d31 3029 0d0a 2020 2020 2020 2020  ze=10)..        
+00003390: 2020 2020 0d0a 2020 2020 6465 6620 706c      ..    def pl
+000033a0: 6f74 5f73 7461 7428 7965 6172 732c 6e62  ot_stat(years,nb
+000033b0: 5f70 6172 7469 6369 7061 6e74 732c 7469  _participants,ti
+000033c0: 746c 652c 6c61 6265 6c5f 7929 3a0d 0a20  tle,label_y):.. 
+000033d0: 2020 2020 2020 2070 6c74 2e66 6967 7572         plt.figur
+000033e0: 6528 6669 6773 697a 653d 2838 2c20 3629  e(figsize=(8, 6)
+000033f0: 290d 0a20 2020 2020 2020 2063 6f6c 6f72  )..        color
+00003400: 7320 3d20 5b27 2366 6461 6134 3827 5d20  s = ['#fdaa48'] 
+00003410: 0d0a 2020 2020 2020 2020 7369 7a65 5f6c  ..        size_l
+00003420: 6162 656c 203d 2032 300d 0a20 2020 2020  abel = 20..     
+00003430: 2020 2070 6c74 2e62 6172 2879 6561 7273     plt.bar(years
+00003440: 2c6e 625f 7061 7274 6963 6970 616e 7473  ,nb_participants
+00003450: 2c63 6f6c 6f72 3d63 6f6c 6f72 7329 0d0a  ,color=colors)..
+00003460: 2020 2020 2020 2020 706c 742e 796c 6162          plt.ylab
+00003470: 656c 286c 6162 656c 5f79 2c73 697a 653d  el(label_y,size=
+00003480: 7369 7a65 5f6c 6162 656c 290d 0a20 2020  size_label)..   
+00003490: 2020 2020 2061 6464 6c61 6265 6c73 2879       addlabels(y
+000034a0: 6561 7273 2c6e 625f 7061 7274 6963 6970  ears,nb_particip
+000034b0: 616e 7473 2c31 290d 0a20 2020 2020 2020  ants,1)..       
+000034c0: 2070 6c74 2e78 7469 636b 7328 726f 7461   plt.xticks(rota
+000034d0: 7469 6f6e 3d39 3029 0d0a 2020 2020 2020  tion=90)..      
+000034e0: 2020 706c 742e 7469 636b 5f70 6172 616d    plt.tick_param
+000034f0: 7328 6178 6973 3d27 7827 2c20 6c61 6265  s(axis='x', labe
+00003500: 6c73 697a 653d 7369 7a65 5f6c 6162 656c  lsize=size_label
+00003510: 290d 0a20 2020 2020 2020 2070 6c74 2e74  )..        plt.t
+00003520: 6963 6b5f 7061 7261 6d73 2861 7869 733d  ick_params(axis=
+00003530: 2779 272c 206c 6162 656c 7369 7a65 3d73  'y', labelsize=s
+00003540: 697a 655f 6c61 6265 6c29 0d0a 2020 2020  ize_label)..    
+00003550: 2020 2020 706c 742e 7469 746c 6528 7469      plt.title(ti
+00003560: 746c 652c 666f 6e74 7369 7a65 3d31 3829  tle,fontsize=18)
+00003570: 0d0a 2020 2020 2020 2020 706c 742e 7469  ..        plt.ti
+00003580: 6768 745f 6c61 796f 7574 2829 0d0a 2020  ght_layout()..  
+00003590: 2020 2020 2020 706c 742e 7368 6f77 2829        plt.show()
+000035a0: 0d0a 2020 2020 0d0a 2020 2020 7374 6174  ..    ..    stat
+000035b0: 7965 6172 203d 206e 616d 6564 7475 706c  year = namedtupl
+000035c0: 6528 2761 6374 6976 6974 6527 2c20 4143  e('activite', AC
+000035d0: 5449 5649 5445 5f4c 4953 5429 0d0a 200d  TIVITE_LIST).. .
+000035e0: 0a20 2020 2070 6c74 2e73 7479 6c65 2e75  .    plt.style.u
+000035f0: 7365 2827 6767 706c 6f74 2729 0d0a 2020  se('ggplot')..  
+00003600: 2020 7965 6172 7320 3d20 5b5d 0d0a 2020    years = []..  
+00003610: 2020 7374 6174 5f64 6963 203d 207b 7d0d    stat_dic = {}.
+00003620: 0a20 2020 2061 6464 5f6d 656d 6f72 7928  .    add_memory(
+00003630: 7374 6174 5f64 6963 2c79 6561 7273 290d  stat_dic,years).
+00003640: 0a0d 0a20 2020 2074 6f64 6179 203d 2064  ...    today = d
+00003650: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+00003660: 2e6e 6f77 2829 0d0a 2020 2020 7965 6172  .now()..    year
+00003670: 735f 6e65 7720 3d20 5b73 7472 2879 6561  s_new = [str(yea
+00003680: 7229 2066 6f72 2079 6561 7220 696e 2072  r) for year in r
+00003690: 616e 6765 2832 3032 322c 746f 6461 792e  ange(2022,today.
+000036a0: 7965 6172 2b31 295d 0d0a 2020 2020 666f  year+1)]..    fo
+000036b0: 7220 7965 6172 2069 6e20 7965 6172 735f  r year in years_
+000036c0: 6e65 773a 0d0a 2020 2020 2020 2020 7374  new:..        st
+000036d0: 6174 5f64 6963 5b79 6561 725d 203d 2066  at_dic[year] = f
+000036e0: 696c 6c5f 7374 6174 5f79 6561 7228 7965  ill_stat_year(ye
+000036f0: 6172 290d 0a20 2020 2020 2020 200d 0a20  ar)..        .. 
+00003700: 2020 2079 6561 7273 203d 2079 6561 7273     years = years
+00003710: 202b 2079 6561 7273 5f6e 6577 2020 200d   + years_new   .
+00003720: 0a20 2020 200d 0a20 2020 200d 0a20 2020  .    ..    ..   
+00003730: 2069 6620 7479 7065 203d 3d20 276e 6272   if type == 'nbr
+00003740: 5f6a 6f75 7273 5f70 6172 7469 6369 7061  _jours_participa
+00003750: 7469 6f6e 5f73 656a 6f75 7273 273a 0d0a  tion_sejours':..
+00003760: 2020 2020 2020 2020 706c 6f74 5f73 7461          plot_sta
+00003770: 7428 7965 6172 732c 0d0a 2020 2020 2020  t(years,..      
+00003780: 2020 2020 2020 2020 2020 2020 5b73 7461              [sta
+00003790: 745f 6469 635b 7965 6172 5d2e 6e62 725f  t_dic[year].nbr_
+000037a0: 6a6f 7572 735f 7061 7274 6963 6970 6174  jours_participat
+000037b0: 696f 6e5f 7365 6a6f 7572 7320 666f 7220  ion_sejours for 
+000037c0: 7965 6172 2069 6e20 7965 6172 735d 2c0d  year in years],.
+000037d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000037e0: 2020 2074 7970 652c 0d0a 2020 2020 2020     type,..      
+000037f0: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00003800: 290d 0a20 2020 2065 6c69 6620 2074 7970  )..    elif  typ
+00003810: 6520 3d3d 2027 736f 7274 6965 5f64 696d  e == 'sortie_dim
+00003820: 616e 6368 655f 636c 7562 273a 0d0a 2020  anche_club':..  
+00003830: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
+00003840: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
+00003850: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
+00003860: 6469 635b 7965 6172 5d2e 736f 7274 6965  dic[year].sortie
+00003870: 5f64 696d 616e 6368 655f 636c 7562 2066  _dimanche_club f
+00003880: 6f72 2079 6561 7220 696e 2079 6561 7273  or year in years
+00003890: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+000038a0: 2020 2020 2020 7479 7065 2c0d 0a20 2020        type,..   
+000038b0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000038c0: 2370 6172 7469 6369 7061 6e74 7327 290d  #participants').
+000038d0: 0a20 2020 2065 6c69 6620 2074 7970 6520  .    elif  type 
+000038e0: 3d3d 2027 736f 7274 6965 5f73 616d 6564  == 'sortie_samed
+000038f0: 695f 636c 7562 273a 0d0a 2020 2020 2020  i_club':..      
+00003900: 2020 706c 6f74 5f73 7461 7428 7965 6172    plot_stat(year
+00003910: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+00003920: 2020 2020 2020 5b73 7461 745f 6469 635b        [stat_dic[
+00003930: 7965 6172 5d2e 736f 7274 6965 5f73 616d  year].sortie_sam
+00003940: 6564 695f 636c 7562 2066 6f72 2079 6561  edi_club for yea
+00003950: 7220 696e 2079 6561 7273 5d2c 0d0a 2020  r in years],..  
+00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003970: 7479 7065 2c0d 0a20 2020 2020 2020 2020  type,..         
+00003980: 2020 2020 2020 2020 2027 2370 6172 7469           '#parti
+00003990: 6369 7061 6e74 7327 290d 0a20 2020 2065  cipants')..    e
+000039a0: 6c69 6620 2074 7970 6520 3d3d 2027 736f  lif  type == 'so
+000039b0: 7274 6965 5f6a 6575 6469 5f63 6c75 6227  rtie_jeudi_club'
+000039c0: 3a0d 0a20 2020 2020 2020 2070 6c6f 745f  :..        plot_
+000039d0: 7374 6174 2879 6561 7273 2c0d 0a20 2020  stat(years,..   
+000039e0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000039f0: 7374 6174 5f64 6963 5b79 6561 725d 2e73  stat_dic[year].s
+00003a00: 6f72 7469 655f 6a65 7564 695f 636c 7562  ortie_jeudi_club
+00003a10: 2066 6f72 2079 6561 7220 696e 2079 6561   for year in yea
+00003a20: 7273 5d2c 0d0a 2020 2020 2020 2020 2020  rs],..          
+00003a30: 2020 2020 2020 2020 7479 7065 2c0d 0a20          type,.. 
+00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a50: 2027 2370 6172 7469 6369 7061 6e74 7327   '#participants'
+00003a60: 2920 200d 0a20 2020 2065 6c69 6620 2074  )  ..    elif  t
+00003a70: 7970 6520 3d3d 2027 7261 6e64 6f6e 6e65  ype == 'randonne
+00003a80: 6527 3a0d 0a20 2020 2020 2020 2070 6c6f  e':..        plo
+00003a90: 745f 7374 6174 2879 6561 7273 2c0d 0a20  t_stat(years,.. 
+00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ab0: 205b 7374 6174 5f64 6963 5b79 6561 725d   [stat_dic[year]
+00003ac0: 2e72 616e 646f 6e6e 6565 2066 6f72 2079  .randonnee for y
+00003ad0: 6561 7220 696e 2079 6561 7273 5d2c 0d0a  ear in years],..
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 2020 7479 7065 2c0d 0a20 2020 2020 2020    type,..       
+00003b00: 2020 2020 2020 2020 2020 2027 2370 6172             '#par
+00003b10: 7469 6369 7061 6e74 7327 2920 200d 0a20  ticipants')  .. 
+00003b20: 2020 2065 6c69 6620 2074 7970 6520 3d3d     elif  type ==
+00003b30: 2027 6e62 725f 7061 7274 6963 6970 6174   'nbr_participat
+00003b40: 696f 6e73 5f73 656a 6f75 7273 273a 0d0a  ions_sejours':..
+00003b50: 2020 2020 2020 2020 706c 6f74 5f73 7461          plot_sta
+00003b60: 7428 7965 6172 732c 0d0a 2020 2020 2020  t(years,..      
+00003b70: 2020 2020 2020 2020 2020 2020 5b73 7461              [sta
+00003b80: 745f 6469 635b 7965 6172 5d2e 6e62 725f  t_dic[year].nbr_
+00003b90: 7061 7274 6963 6970 6174 696f 6e73 5f73  participations_s
+00003ba0: 656a 6f75 7273 2066 6f72 2079 6561 7220  ejours for year 
+00003bb0: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
+00003bc0: 2020 2020 2020 2020 2020 2020 2020 274e                'N
+00003bd0: 6f6d 6272 6520 6465 2070 6172 7469 6369  ombre de partici
+00003be0: 7061 7469 6f6e 7320 6175 7820 73c3 a96a  pations aux s..j
+00003bf0: 6f75 7273 272c 0d0a 2020 2020 2020 2020  ours',..        
+00003c00: 2020 2020 2020 2020 2020 2723 2070 6172            '# par
+00003c10: 7469 6369 7061 7469 6f6e 7320 6175 7820  ticipations aux 
+00003c20: 73c3 a96a 6f75 7273 2729 200d 0a20 2020  s..jours') ..   
+00003c30: 2065 6c69 6620 2074 7970 6520 3d3d 2027   elif  type == '
+00003c40: 6e62 725f 7365 6a6f 7572 7327 3a0d 0a20  nbr_sejours':.. 
+00003c50: 2020 2020 2020 2070 6c6f 745f 7374 6174         plot_stat
+00003c60: 2879 6561 7273 2c0d 0a20 2020 2020 2020  (years,..       
+00003c70: 2020 2020 2020 2020 2020 205b 7374 6174             [stat
+00003c80: 5f64 6963 5b79 6561 725d 2e6e 6272 5f73  _dic[year].nbr_s
+00003c90: 656a 6f75 7273 2066 6f72 2079 6561 7220  ejours for year 
+00003ca0: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
+00003cb0: 2020 2020 2020 2020 2020 2020 2020 274e                'N
+00003cc0: 6f6d 6272 6520 6465 2073 c3a9 6a6f 7572  ombre de s..jour
+00003cd0: 7327 2c0d 0a20 2020 2020 2020 2020 2020  s',..           
+00003ce0: 2020 2020 2020 2027 2320 73c3 a96a 6f75         '# s..jou
+00003cf0: 7273 2729 0d0a 2020 2020 656c 6966 2020  rs')..    elif  
+00003d00: 7479 7065 203d 3d20 276e 6272 5f6a 6f75  type == 'nbr_jou
+00003d10: 7273 5f73 656a 6f75 7273 273a 0d0a 2020  rs_sejours':..  
+00003d20: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
+00003d30: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
+00003d40: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
+00003d50: 6469 635b 7965 6172 5d2e 6e62 725f 6a6f  dic[year].nbr_jo
+00003d60: 7572 735f 7365 6a6f 7572 7320 666f 7220  urs_sejours for 
+00003d70: 7965 6172 2069 6e20 7965 6172 735d 2c0d  year in years],.
+00003d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d90: 2020 2027 4e6f 6d62 7265 2064 6520 6a6f     'Nombre de jo
+00003da0: 7572 7320 73c3 a96a 6f75 7273 272c 0d0a  urs s..jours',..
+00003db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dc0: 2020 2723 206a 6f75 7273 2073 c3a9 6a6f    '# jours s..jo
+00003dd0: 7572 2729 2020 2020 2020 2020            ur')
```

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_Func/CTG_utility.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_Func/CTG_utility.py`

 * *Files 18% similar despite different names*

```diff
@@ -117,8 +117,28 @@
     
     c = Counter()
     c = Counter(info_sejour)
 
     
     sejour_info_tup = sejour_info( sum(info_sejour),len(info_sejour),c)
     
-    return sejour_info_tup
+    return sejour_info_tup
+    
+def get_cout_total(year,type_sejour,dg,ctg_path):
+    ''' Calcul du coût total des randonnées (type='randonnee") ou des séjours (type="sejour") pour l'année year
+    '''
+    # Standard library imports
+    from pathlib import Path
+    
+    # Third party import
+    import pandas as pd
+    
+    file_info = Path(ctg_path) / Path(str(year)) / Path('DATA') / Path('info_randos.xlsx')
+    df_indo = pd.read_excel(file_info)
+    cout_total = 0
+    for evenement in dg.index:
+        date_rando = f"{str(year)[2:4]}-{evenement[0:5].replace('_','-')}"
+        cout_rando = df_indo.query('date==@date_rando and type==@type_sejour')['Cout'].tolist()[0]
+        nbr_participants = dg[evenement]
+        cout_total += cout_rando * nbr_participants
+        
+    return cout_total
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/GUI_Globals.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/GUI_Globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,18 +334,18 @@
 BUTT_AGE_ANALYSIS = "Lancer l'analyse de l'évolution de l'âge médian"
 
 ### - sorties
 TEXT_SORTIES     = "Analyse des sorties"
 HELP_SORTIES     = " L'analyse des sorties est effectuée à partir des fichiers"
 HELP_SORTIES    += " csv issues des Framadate"
 BUTT_SORTIES = "Lancer l'analyse des sorties"
-TEXT_RANDO       = "Analyse des randonnées"
-HELP_RANDO       = " L'analyse des sorties est effectuée à partir des fiches"
-HELP_RANDO      += " d'émargements des participants aux randonnées"
-BUTT_RANDO = "Lancer l'analyse des randonnées"
+TEXT_RANDO       = "Analyse des randonnées/séjours"
+HELP_RANDO       = " L'analyse des sorties/séjours est effectuée à partir des fichers"
+HELP_RANDO      += " d'émargements des participants aux randonnées/séjours"
+BUTT_RANDO = "Lancer l'analyse"
 
 ### - Page synthese
 TEXT_SYNTHESE_SORTIES     = "Synthèse des sorties"
 HELP_SYNTHESE_SORTIES     = " La synthèse est effectuée à partir des fichiers"
 HELP_SYNTHESE_SORTIES    += " d'émargement aux sorties, randonnées et séjours"
 BUTT_SYNTHESE_SORTIES = "Lancer la synthèse"
 TEXT_EVOLUTION_EFFECTIF     = "Analyse de l'évolution temporelle de l'effectif"
```

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageDivers.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageDivers.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageEffectif.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageEffectif.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageSorties.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageSorties.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,30 @@
     #info_text += f"\n\nLa base de donnée des indicateurs respective de l'Institut "
     #info_text += f"et de chaque département a été mise à jour "
     #info_text += f"avec les résultats de cette analyse et se trouve dans le dossier :" 
     #info_text += f"\n\n''."
     #messagebox.showinfo(info_title, info_text) 
     
 def _launch_rando_analysis(ctg_path, 
-                           year):
+                           year,
+                           type_sortie):
     """
     """
     
     # Standard library imports
     from pathlib import Path
     from tkinter import messagebox
     
     # Local imports
     from CTG_Utils.CTG_Func.CTG_synthese import synthese_randonnee
-        
-    synthese_randonnee(year,ctg_path)  
+    
+    if type_sortie == "SEJOUR":
+        synthese_randonnee(year,ctg_path,'SEJOUR')
+    else:    
+        synthese_randonnee(year,ctg_path,'RANDONNEE')  
 
 def create_sorties_analysis(self, master, page_name, institute, ctg_path):
     
     """
     Description : function working as a bridge between the BiblioMeter 
     App and the functionalities needed for the use of the app
     
@@ -95,15 +99,16 @@
         return
         
     def _launch_rando_analysis_try():        
         # Getting year selection
         year_select = variable_years.get()
         type_sortie = variable_sortie.get()
         _launch_rando_analysis(ctg_path, 
-                               year_select)
+                               year_select,
+                               type_sortie)
         return        
     
     
     # Setting effective font sizes and positions (numbers are reference values)
     eff_etape_font_size      = font_size(gg.REF_ETAPE_FONT_SIZE,   AppMain.width_sf_min)           #14
     eff_launch_font_size     = font_size(gg.REF_ETAPE_FONT_SIZE-1, AppMain.width_sf_min)
     eff_help_font_size       = font_size(gg.REF_ETAPE_FONT_SIZE-2, AppMain.width_sf_min)
```

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageSynthese.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageSynthese.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/PageTendance.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/PageTendance.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/Page_Classes.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Page_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/Useful_Classes.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Useful_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils/CTG_GUI/Useful_Functions.py` & `CTG_Utils-1.2.0/CTG_Utils/CTG_GUI/Useful_Functions.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/CTG_Utils.egg-info/PKG-INFO` & `CTG_Utils-1.2.0/CTG_Utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG-Utils
-Version: 1.1.7
+Version: 1.2.0
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.7/CTG_Utils.egg-info/SOURCES.txt` & `CTG_Utils-1.2.0/CTG_Utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/LICENSE` & `CTG_Utils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.7/PKG-INFO` & `CTG_Utils-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG_Utils
-Version: 1.1.7
+Version: 1.2.0
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.7/make_exe.bat` & `CTG_Utils-1.2.0/make_exe.bat`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Title create CTG_Meter.exe executable
 
 :: builds the CTG_METER python program
-set "PGM=%userprofile%\PyVenv\CTG_exe\CTG_METER.py"
+set "PGM=%userprofile%\Temp\CTG_exe\CTG_METER.py"
 echo from CTG_Utils.CTG_GUI import AppMain > %PGM%
 echo app_main = AppMain() >> %PGM%
 echo app_main.mainloop() >> %PGM%
 
 :: install packages
 
 pip install CTG_Utils
 pip install auto-py-to-exe
 
 :: remote the directories buib and dist
 :: set the directories buid and dist used when making the executable
 
-set "BUILD=%userprofile%\PyVenv\CTG_exe\build"
-set "DIST=%userprofile%\PyVenv\CTG_exe\dist"
+set "BUILD=%userprofile%\Temp\CTG_exe\build"
+set "DIST=%userprofile%\Temp\CTG_exe\dist"
 rmdir /s /q %BUILD%
 rmdir /s /q %DIST%
 
 :: set the default directories
 :: ICON contains the icon file with the format.ico
 :: PGM contain the application lauch python program
 
-set "ICON=%userprofile%/PyVenv/CTG_exe/venv/Lib/site-packages/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico"
-set "DATA=%userprofile%/PyVenv/CTG_exe/venv/Lib/site-packages/CTG_Utils;CTG_Utils/"
+set "ICON=%userprofile%/Temp/CTG_exe/venv/Lib/site-packages/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico"
+set "DATA=%userprofile%/Temp/CTG_exe/venv/Lib/site-packages/CTG_Utils;CTG_Utils/"
 
 :: make the executable 
 pyinstaller --noconfirm --onefile --console^
  --icon "%ICON%"^
  --add-data "%DATA%"^
  "%PGM%"
```

### Comparing `CTG_Utils-1.1.7/setup.py` & `CTG_Utils-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 install_requires = open(path.join(this_directory, 'requirements.txt'), encoding='utf-8').read().strip().split('\n') 
 
 # This setup is suitable for "python setup.py develop".
 
 setup(name='CTG_Utils',
-      version='1.1.7',
+      version='1.2.0',
       description='A toolbox for ctg statistics analysis',
       long_description=long_description,
       long_description_content_type='text/markdown',
       include_package_data = True,
       license = 'MIT',
       classifiers = [
         'Development Status :: 4 - Beta',
```

