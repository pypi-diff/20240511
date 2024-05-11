# Comparing `tmp/CTG_Utils-1.0.0.tar.gz` & `tmp/CTG_Utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTG_Utils-1.0.0.tar", last modified: Thu May  9 08:21:25 2024, max compression
+gzip compressed data, was "CTG_Utils-1.1.0.tar", last modified: Sat May 11 06:52:48 2024, max compression
```

## Comparing `CTG_Utils-1.0.0.tar` & `CTG_Utils-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 08:21:25.784801 CTG_Utils-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-09 08:21:25.732195 CTG_Utils-1.0.0/CTG_Utils/
-drwxrwxrwx   0        0        0        0 2024-05-09 08:21:25.751672 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/
--rw-rw-rw-   0        0        0     6423 2024-05-08 13:04:56.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTGClasses.py
-drwxrwxrwx   0        0        0        0 2024-05-09 08:21:25.762859 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/
--rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
--rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
--rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
--rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
--rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
--rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
--rw-rw-rw-   0        0        0     1267 2024-04-16 10:18:07.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
--rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
--rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
--rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_config.py
--rw-rw-rw-   0        0        0    19763 2024-05-08 14:48:15.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_effectif.py
--rw-rw-rw-   0        0        0    13982 2024-05-09 07:14:17.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_plot.py
--rw-rw-rw-   0        0        0    14750 2024-05-09 07:14:17.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_synthese.py
--rw-rw-rw-   0        0        0     4575 2024-05-08 11:55:32.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_utility.py
--rw-rw-rw-   0        0        0      241 2024-04-06 06:50:36.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_Func/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 08:21:25.782809 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/
--rw-rw-rw-   0        0        0    15056 2024-05-08 13:51:42.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/GUI_Globals.py
--rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/PageEffectif.py
--rw-rw-rw-   0        0        0    11613 2024-05-07 11:49:29.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/PageSorties.py
--rw-rw-rw-   0        0        0    10759 2024-05-07 13:39:45.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/PageSynthese.py
--rw-rw-rw-   0        0        0     9011 2024-05-08 07:41:08.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/PageTendance.py
--rw-rw-rw-   0        0        0    29208 2024-05-09 07:10:13.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/Page_Classes.py
--rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/Useful_Classes.py
--rw-rw-rw-   0        0        0    13064 2024-05-06 10:12:44.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/Useful_Functions.py
--rw-rw-rw-   0        0        0      269 2024-04-26 09:09:37.000000 CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 08:21:25.744689 CTG_Utils-1.0.0/CTG_Utils.egg-info/
--rw-rw-rw-   0        0        0      681 2024-05-09 08:21:24.000000 CTG_Utils-1.0.0/CTG_Utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1183 2024-05-09 08:21:24.000000 CTG_Utils-1.0.0/CTG_Utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 08:21:24.000000 CTG_Utils-1.0.0/CTG_Utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-09 08:21:24.000000 CTG_Utils-1.0.0/CTG_Utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-05-09 08:21:24.000000 CTG_Utils-1.0.0/CTG_Utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      681 2024-05-09 08:21:25.784801 CTG_Utils-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-09 08:21:25.784801 CTG_Utils-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1398 2024-05-09 08:19:23.000000 CTG_Utils-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.081676 CTG_Utils-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.026275 CTG_Utils-1.1.0/CTG_Utils/
+drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.045225 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/
+-rw-rw-rw-   0        0        0     6571 2024-05-10 17:41:23.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTGClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.055200 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/
+-rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
+-rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
+-rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
+-rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
+-rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
+-rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
+-rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
+-rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
+-rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
+-rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_config.py
+-rw-rw-rw-   0        0        0    19835 2024-05-09 11:52:03.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_effectif.py
+-rw-rw-rw-   0        0        0    11586 2024-05-10 13:31:57.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_plot.py
+-rw-rw-rw-   0        0        0    15509 2024-05-10 17:36:41.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_synthese.py
+-rw-rw-rw-   0        0        0     4645 2024-05-10 17:35:42.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_utility.py
+-rw-rw-rw-   0        0        0      218 2024-05-10 17:42:50.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_Func/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.079650 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/
+-rw-rw-rw-   0        0        0    15700 2024-05-10 12:50:50.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/GUI_Globals.py
+-rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageDivers.py
+-rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageEffectif.py
+-rw-rw-rw-   0        0        0    11613 2024-05-07 11:49:29.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageSorties.py
+-rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageSynthese.py
+-rw-rw-rw-   0        0        0     9011 2024-05-08 07:41:08.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageTendance.py
+-rw-rw-rw-   0        0        0    30344 2024-05-10 07:03:45.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Page_Classes.py
+-rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Useful_Classes.py
+-rw-rw-rw-   0        0        0    11470 2024-05-10 06:56:47.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Useful_Functions.py
+-rw-rw-rw-   0        0        0      198 2024-05-10 17:28:54.000000 CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:52:48.038245 CTG_Utils-1.1.0/CTG_Utils.egg-info/
+-rw-rw-rw-   0        0        0      681 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-05-11 06:52:47.000000 CTG_Utils-1.1.0/CTG_Utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      681 2024-05-11 06:52:48.080648 CTG_Utils-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 06:52:48.081676 CTG_Utils-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1398 2024-05-09 18:13:06.000000 CTG_Utils-1.1.0/setup.py
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTGClasses.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTGClasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 
 class EffectifCtg():
     
     
     def __init__(self,year,ctg_path):
+        
+        # Standard library imports
         from pathlib import Path
 
+        # Third party imports
         import pandas as pd
 
+        # Internal imports
         from CTG_Utils.CTG_Func.CTG_config import _config_ctg
         from CTG_Utils.CTG_Func.CTG_plot import built_lat_long
-        
-        GLOBAL = _config_ctg()
 
-        
-
-        
         self.year = year
         self.ctg_path = ctg_path
-        #df = pd.read_excel(GLOBAL['ROOT'] / Path(str(year))/ Path('DATA')/Path(str(year)+'.xlsx'))
         df = pd.read_excel(self.ctg_path / Path(str(year))/ Path('DATA')/Path(str(year)+'.xlsx'))
         
         year_1 = int(year)-1
         df_1 = pd.read_excel(self.ctg_path / Path(str(year_1))/ Path('DATA')/Path(str(year_1)+'.xlsx'))
 
         df['Date de naissance'] = pd.to_datetime(df['Date de naissance'], format="%d/%m/%Y")
         df_1['Date de naissance'] = pd.to_datetime(df_1['Date de naissance'], format="%d/%m/%Y")
@@ -34,27 +32,35 @@
         df['distance'] = df.apply(lambda row: self.distance_(row, dh),axis=1)
         
         self.effectif = df
         self.effectif_1 = df_1
         
     @staticmethod
     def distance_(row,dh):
+    
+        # Standard library imports
         from math import asin, cos, radians, sin, sqrt
+        
+        # Third party imports        
         import numpy as np
         
         phi1, lon1 = dh.query("Ville=='GRENOBLE'")[['long','lat']].values.flatten()
         phi1, lon1 = radians(phi1), radians(lon1)
         phi2, lon2 = radians(row['long']), radians(row['lat'])
         rad = 6371
         dist = 2 * rad * asin(sqrt(sin((phi2 - phi1) / 2) ** 2
                                  + cos(phi1) * cos(phi2) * sin((lon2 - lon1) / 2) ** 2))
         return np.round(dist,1)
     
     def stat(self):
+    
+        # Standard library imports
         from tkinter import messagebox
+        
+        # Internal imports
         from CTG_Utils.CTG_Func.CTG_utility import read_correction_effectifs
 
         da = self.effectif.groupby('Sexe')['Age'].agg(['count','median','max','min'])
         res = self.effectif['Age'].agg(['count','median','max','min']).tolist()
         stat = []
         nbr_membres = round(res[0],0)
         stat.append(f"Nombre d'adhérents : {nbr_membres}")
@@ -108,14 +114,16 @@
         nbr_abonnements = len(self.effectif.query('Abonnements == "Oui"'))
         stat.append(f"Nombre d'abonnés à la revue FFCT : {nbr_abonnements} ({round(100*nbr_abonnements/nbr_membres)} %)")
         
         stat ='\n'.join(stat)
         messagebox.showinfo(f'Statistique {self.year}',stat)
         
     def plot_histo(self):
+    
+        # Third party imports
         import matplotlib.pyplot as plt
         import pandas as pd
         
         fig, ax = plt.subplots(figsize=(10,10))
         self.effectif['age group'] = pd.cut(self.effectif.Age, bins=range(0, 95, 5), right=False)
         result_hist = self.effectif.groupby('Sexe')['age group'].value_counts().unstack().T.plot.bar(width=1, stacked=False,ax=ax)
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_effectif.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_effectif.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,30 +102,30 @@
             if (row.name3 is None) and ( row.name2 is not None):
                 if len(row.name1)==1:
                     dr = df_effectif.query('Prénom1==@row.name1[0] and Nom==@row.name2')
                     if len(dr):
                         dic[idx] =dr.iloc[0].tolist()[:-1]+[sejour]
                     else:
                         print(f'no match,{row.name2},{row.name1} dans {sejour}')
-                        no_match.append((row.name2,row.name1))
+                        no_match.append((file,row.name2,row.name1))
                 elif len(row.name2)==1:
                     dr = df_effectif.query('Prénom1==@row.name2 and Nom==@row.name1')
                     if len(dr):
                          dic[idx] =dr.iloc[0].tolist()[:-1]+[sejour]
                     else:
                         print(f'no match,{row.name2},{row.name1} dans {sejour}')
-                        no_match.append((row.name2,row.name1))
+                        no_match.append((file,row.name2,row.name1))
                 else:
                     if len((dr:=df_effectif.query('Prénom==@row.name2 and Nom==@row.name1'))):
                          dic[idx] =dr.iloc[0].tolist()[:-1]+[sejour]
                     elif len((dr:=df_effectif.query('Prénom==@row.name1 and Nom==@row.name2'))):
                          dic[idx] =dr.iloc[0].tolist()[:-1]+[sejour]
                     else:
                         print(f'{sejour} : no match, prénom/prénom:{row.name2}, nom/prénom: {row.name1}')
-                        no_match.append((row.name2,row.name1))
+                        no_match.append((file,row.name2,row.name1))
             else:
                 print(f'WARNING: incorrect name {row.name1}, {row.name2}, {row.name3} in sejour {sejour}')
 
         dg = pd.DataFrame.from_dict(dic).T 
         if len(dg) !=0:
             dg.columns = ['N° Licencié','Nom','Prénom','Sexe','Pratique VAE','sejour',]
         else:
@@ -180,15 +180,15 @@
     df_effectif = read_effectif_corrected(dic_correction_licence, list_non_licencie, dic_part_club,year)
 
     no_match = []
     df_list = [] 
     sejours = [x for x in os.listdir( path / Path('CSV')) if x.endswith('.csv')]
     
     
-    nbr_inscrits_mean = 0
+    nbr_moyen_participants = 0
     counter = 1
     for sejour in sejours:
         dg = inscrit_sejour( path / Path('CSV') /Path(sejour),no_match,df_effectif)
         
         if re.findall(r'^\d{4}[-_]',sejour):
             date = sejour[2:10].replace('_','-')
         else:
@@ -205,22 +205,23 @@
             else:
                 dg['nbr_jours'] = 1
         else:
             dg['nbr_jours'] = 0
         if dg.reset_index().loc[0,'Nom'] is not None:
             nbr_inscrits = len(dg)
             if nbr_inscrits != 0:
-                nbr_inscrits_mean = nbr_inscrits_mean + (nbr_inscrits - nbr_inscrits_mean)/counter
+                nbr_moyen_participants = nbr_moyen_participants + (nbr_inscrits - nbr_moyen_participants)/counter
                 counter += 1
                 print(f"{os.path.split(path)[-1]} :{sejour}, Nombre d'inscrits : {nbr_inscrits}")
         df_list.append(dg)
         file_store = os.path.splitext(sejour)[0]+'.xlsx'
         dg.to_excel(path / Path('EXCEL') / Path(file_store))
         
-    print(f"Nombre d'évènenements : {counter-1}. Nombre moyen de participants : {nbr_inscrits_mean}")
+    print(f"Nombre d'évènenements : {counter-1}. Nombre moyen de participants : {nbr_moyen_participants}")
+    nbr_evenement = counter-1 
     if counter-1 > 0 :  #
         df_total = pd.concat(df_list,ignore_index=True)
     else:
         return (None, None, None)
 
 
     liste_licence = df_effectif['N° Licencié']
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_plot.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 __all_ = ["built_lat_long",
           "plot_club_38",
           "plot_ctg",
-          "plot_vignoble",
           "stat_sorties_club",]
           
 from CTG_Utils.CTG_Func.CTG_config import GLOBAL   
 
 def plot_club_38():
 
     # Standard library import
@@ -69,15 +68,15 @@
     from pathlib import Path
     
     # 3rd party imports
     import folium
     import numpy as np
     import pandas as pd
     
-    path_villes_de_france = Path(__file__).parent.parent / Path('CTG_RefFiles/villes_france_premium.csv')
+    path_villes_de_france = Path(__file__).parent.parent / Path('CTG_Func/CTG_RefFiles/villes_france_premium.csv')
     
     def normalize_ville(x):
         dic_ville = {'SAINT-HILAIRE-DU-TOUVET':"SAINT-HILAIRE-38",
                      'SAINT-HILAIRE':"SAINT-HILAIRE-38",
                      'LAVAL-EN-BELLEDONNE':'LAVAL-38',
                      'LAVAL':"LAVAL-38",
                      'CRETS-EN-BELLEDONNE':"SAINT-PIERRE-D'ALLEVARD"}
@@ -199,15 +198,20 @@
     else:
         flag_labels = False
     
     no_match,df_total,_ = count_participation(path_sorties_club,year,info_rando)
     if no_match is None:
         messagebox.showinfo('WARNING',"Aucun participant n'a participé à ce type de sortie" )
     else:
-        print(no_match)
+        text_message = ''
+        for tup in no_match:
+              text_message += f'Le nom {tup[1]}, {tup[2]} est inconnu dans le fichier : "{os.path.split(tup[0])[-1]}"'
+              text_message += '\n'
+           
+        if len(text_message) : messagebox.showinfo('WARNING',text_message )
     
     if year is None:
         currentDateTime = datetime.datetime.now()
         date = currentDateTime.date()
         year = date.strftime("%Y")
         
     list_non_licencie, dic_correction_licence, dic_part_club = correction_effectif(year)
@@ -227,15 +231,14 @@
     df_total['VAE'] = df_total['N° Licencié'].map(dic_vae)
     df_total['VAE'].fillna('Non',inplace=True)
     dic_sexe = dict(M="Homme",F="Femme")
     dic_vae = dict(Oui="VAE",Non="Musculaire")
     df_total = df_total.replace({"sexe": dic_sexe})
     df_total = df_total.replace({"VAE": dic_vae})
     if df_total['Nom'].isna().all():
-        print("Aucune sortie")
         return None
     dg = df_total.groupby(['sexe','VAE'])['sejour'].value_counts().unstack().T
    
     try:
         dg['irrelevant'] = dg['irrelevant'] - 1
     except KeyError as error:
         pass
@@ -274,74 +277,14 @@
     plt.tight_layout()
     plt.show()
     fig_file = os.path.split(path_sorties_club)[-1].replace(' ','_')+'.png'
     plt.savefig(Path(GLOBAL['ROOT']) / Path(str(year)) / Path('STATISTIQUES') / Path(fig_file),bbox_inches='tight')
     
     return df_total
 
-    
-def plot_vignoble():
-
-    # Standard library import
-    from pathlib import Path
-
-    # 3rd party imports
-    import folium
-    import numpy as np
-    import pandas as pd
-
-
-    df_club_38 = pd.read_excel(GLOBAL['ROOT'] / Path('club_38.xlsx'))
-    path_villes_de_france = Path(__file__).parent.parent /Path('CTG_Func') / Path('CTG_RefFiles/villes_france_premium.csv')
-    df_villes = pd.read_csv(path_villes_de_france,header=None,usecols=[2,19,20])
-    dic_long = dict(zip(df_villes[2] , df_villes[19]))
-    dic_lat = dict(zip(df_villes[2] , df_villes[20]))
-    df_vignobles = pd.read_excel(r'C:\Users\franc\CTG\RANDONNEES\vignobles\listing_participants.xlsx')
-    df = pd.merge(df_vignobles, df_club_38, on='N° FFCT', how='inner')
-    df['femmes'] = df['femmes'].fillna(0)
-    df['total'] =df['hommes']+df['femmes']
-
-    #df =pd.read_excel(root / Path(effectif))
-
-    df['Ville'] = df['Ville'].str.replace(' ','-')
-    df['Ville'] = df['Ville'].str.replace('ST-','SAINT-')
-    df['Ville'] = df['Ville'].str.replace('\-D\-+',"-D'",regex=True)
-    df['Ville'] = df['Ville'].str.replace('^LA-',"LA ",regex=True)
-    df['Ville'] = df['Ville'].str.replace('^LE-',"LE ",regex=True)
-    df['Ville'] = df['Ville'].str.replace('SAINT-HILAIRE-DU-TOUVET',"SAINT-HILAIRE",regex=False)
-    df['Ville'] = df['Ville'].str.replace('SAINT-HILAIRE',"SAINT-HILAIRE-38",regex=False)
-    df['Ville'] = df['Ville'].str.replace('LAVAL',"LAVAL-38",regex=False)
-    df['Ville'] = df['Ville'].str.replace('LES-ABRETS',"LES ABRETS",regex=False)
-    df['Ville'] = df['Ville'].str.lower()
-
-    df['long'] = df['Ville'].map(dic_long)
-    df['lat'] = df['Ville'].map(dic_lat)
-
-
-    kol = folium.Map(location=[45.2,5.7], tiles='openstreetmap', zoom_start=12)
-
-    for latitude,longitude,size, ville, num_ffct, club in zip(df['lat'],
-                                                        df['long'],
-                                                        df['total'],
-                                                        df['Ville'],
-                                                        df['N° FFCT'],
-                                                        df['total'] ):
-
-        long_ville, lat_ville =df.query("Ville==@ville")[['long','lat']].values[0]#.flatten()
-        color='blue'
-
-        folium.Circle(
-                        location=[latitude, longitude],
-                        radius=size*70,
-                        popup=f'{ville} ({size}), club:{club} ',
-                        color=color,
-                        fill=True,
-    ).add_to(kol)
-    return kol
-
 def _distance(ϕ1, λ1,ϕ2, λ2):
     from math import asin, cos, radians, sin, sqrt
     ϕ1, λ1 = radians(ϕ1), radians(λ1)
     ϕ2, λ2 = radians(ϕ2), radians(λ2)
     rad = 6371
     dist = 2 * rad * asin(
                             sqrt(
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_synthese.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_synthese.py`

 * *Files 12% similar despite different names*

```diff
@@ -497,426 +497,474 @@
 00001f00: 275d 2920 2f20 5061 7468 2873 7472 2879  ']) / Path(str(y
 00001f10: 6561 7229 2920 2f20 5061 7468 2827 5354  ear)) / Path('ST
 00001f20: 4154 4953 5449 5155 4553 2729 202f 2050  ATISTIQUES') / P
 00001f30: 6174 6828 6669 675f 6669 6c65 292c 6262  ath(fig_file),bb
 00001f40: 6f78 5f69 6e63 6865 733d 2774 6967 6874  ox_inches='tight
 00001f50: 2729 0d0a 2020 2020 0d0a 6465 6620 6e62  ')..    ..def nb
 00001f60: 725f 7365 6a6f 7572 735f 6164 6865 7265  r_sejours_adhere
-00001f70: 6e74 2879 6561 7229 3a0d 0a0d 0a20 2020  nt(year):....   
-00001f80: 2066 726f 6d20 636f 6c6c 6563 7469 6f6e   from collection
-00001f90: 7320 696d 706f 7274 2043 6f75 6e74 6572  s import Counter
-00001fa0: 0d0a 2020 2020 6672 6f6d 2070 6174 686c  ..    from pathl
-00001fb0: 6962 2069 6d70 6f72 7420 5061 7468 0d0a  ib import Path..
-00001fc0: 2020 2020 0d0a 2020 2020 696d 706f 7274      ..    import
-00001fd0: 206d 6174 706c 6f74 6c69 622e 7079 706c   matplotlib.pypl
-00001fe0: 6f74 2061 7320 706c 740d 0a20 2020 2069  ot as plt..    i
-00001ff0: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
-00002000: 7064 0d0a 2020 2020 0d0a 2020 2020 706c  pd..    ..    pl
-00002010: 742e 7374 796c 652e 7573 6528 2767 6770  t.style.use('ggp
-00002020: 6c6f 7427 290d 0a20 2020 200d 0a20 2020  lot')..    ..   
-00002030: 2023 2066 756e 6374 696f 6e20 746f 2061   # function to a
-00002040: 6464 2076 616c 7565 206c 6162 656c 730d  dd value labels.
-00002050: 0a20 2020 2064 6566 2061 6464 6c61 6265  .    def addlabe
-00002060: 6c73 2878 2c79 293a 0d0a 2020 2020 2020  ls(x,y):..      
-00002070: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00002080: 286c 656e 2878 2929 3a0d 0a20 2020 2020  (len(x)):..     
-00002090: 2020 2020 2020 2070 6c74 2e74 6578 7428         plt.text(
-000020a0: 785b 695d 2d30 2e32 2c79 5b69 5d2b 312c  x[i]-0.2,y[i]+1,
-000020b0: 795b 695d 2c73 697a 653d 3230 290d 0a20  y[i],size=20).. 
-000020c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000020d0: 2066 696c 655f 696e 203d 2050 6174 6828   file_in = Path(
-000020e0: 474c 4f42 414c 5b27 524f 4f54 275d 2920  GLOBAL['ROOT']) 
-000020f0: 2f20 5061 7468 2873 7472 2879 6561 7229  / Path(str(year)
-00002100: 2920 2f20 5061 7468 2827 5354 4154 4953  ) / Path('STATIS
-00002110: 5449 5155 4553 2729 202f 2050 6174 6828  TIQUES') / Path(
-00002120: 2773 796e 7468 6573 655f 6164 6865 7265  'synthese_adhere
-00002130: 6e74 2e78 6c73 7827 290d 0a20 2020 2064  nt.xlsx')..    d
-00002140: 665f 746f 7461 6c20 3d20 7064 2e72 6561  f_total = pd.rea
-00002150: 645f 6578 6365 6c28 6669 6c65 5f69 6e29  d_excel(file_in)
-00002160: 0d0a 2020 2020 0d0a 2020 2020 6320 3d20  ..    ..    c = 
-00002170: 436f 756e 7465 7228 290d 0a20 2020 2063  Counter()..    c
-00002180: 203d 2043 6f75 6e74 6572 2864 665f 746f   = Counter(df_to
-00002190: 7461 6c5b 274e 6272 5f53 454a 4f55 5253  tal['Nbr_SEJOURS
-000021a0: 275d 2e74 6f6c 6973 7428 2929 0d0a 2020  '].tolist())..  
-000021b0: 2020 6320 3d20 632e 6d6f 7374 5f63 6f6d    c = c.most_com
-000021c0: 6d6f 6e28 290d 0a0d 0a20 2020 2078 2c20  mon()....    x, 
-000021d0: 7920 3d20 7a69 7028 2a63 290d 0a20 2020  y = zip(*c)..   
-000021e0: 2078 203d 206c 6973 7428 7829 0d0a 2020   x = list(x)..  
-000021f0: 2020 7920 3d20 6c69 7374 2879 290d 0a20    y = list(y).. 
-00002200: 2020 200d 0a20 2020 2066 6967 2c20 6178     ..    fig, ax
-00002210: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
-00002220: 6669 6773 697a 653d 2835 2c35 2929 0d0a  figsize=(5,5))..
-00002230: 2020 2020 706c 742e 6261 7228 5b73 7472      plt.bar([str
-00002240: 2878 5f73 2920 666f 7220 785f 7320 696e  (x_s) for x_s in
-00002250: 2078 5d2c 7929 0d0a 2020 2020 706c 742e   x],y)..    plt.
-00002260: 786c 6162 656c 2827 4e6f 6d62 7265 2064  xlabel('Nombre d
-00002270: 6520 7061 7274 6963 6970 6174 696f 6e20  e participation 
-00002280: c3a0 2064 6573 2073 c3a9 6a6f 7572 7327  .. des s..jours'
-00002290: 290d 0a20 2020 2070 6c74 2e79 6c61 6265  )..    plt.ylabe
-000022a0: 6c28 274e 6f6d 6272 6520 6465 206c 6963  l('Nombre de lic
-000022b0: 656e 6369 6572 7327 290d 0a20 2020 2070  enciers')..    p
-000022c0: 6c74 2e74 6963 6b5f 7061 7261 6d73 2861  lt.tick_params(a
-000022d0: 7869 733d 2778 272c 206c 6162 656c 7369  xis='x', labelsi
-000022e0: 7a65 3d32 3029 0d0a 2020 2020 706c 742e  ze=20)..    plt.
-000022f0: 7469 636b 5f70 6172 616d 7328 6178 6973  tick_params(axis
-00002300: 3d27 7927 2c20 6c61 6265 6c73 697a 653d  ='y', labelsize=
-00002310: 3230 290d 0a20 2020 2070 6c74 2e74 6974  20)..    plt.tit
-00002320: 6c65 2873 7472 2879 6561 7229 2c70 6164  le(str(year),pad
-00002330: 3d32 302c 2066 6f6e 7473 697a 653d 3330  =20, fontsize=30
-00002340: 290d 0a20 2020 200d 0a20 2020 2061 782e  )..    ..    ax.
-00002350: 7365 745f 786c 6162 656c 2827 4e20 73c3  set_xlabel('N s.
-00002360: a96a 6f75 7273 272c 2066 6f6e 7473 697a  .jours', fontsiz
-00002370: 6520 3d20 3230 290d 0a20 2020 2061 782e  e = 20)..    ax.
-00002380: 7365 745f 796c 6162 656c 2827 4e6f 6d62  set_ylabel('Nomb
-00002390: 7265 2064 6520 4354 4720 6179 616e 7420  re de CTG ayant 
-000023a0: 5c6e 2070 6172 7469 6369 70c3 a920 c3a0  \n particip.. ..
-000023b0: 204e 2073 c3a9 6a6f 7572 7327 2c20 666f   N s..jours', fo
-000023c0: 6e74 7369 7a65 203d 2032 3029 0d0a 2020  ntsize = 20)..  
-000023d0: 2020 0d0a 2020 2020 782e 736f 7274 2829    ..    x.sort()
-000023e0: 0d0a 2020 2020 6164 646c 6162 656c 7328  ..    addlabels(
-000023f0: 782c 7929 0d0a 0d0a 2020 2020 6669 675f  x,y)....    fig_
-00002400: 6669 6c65 203d 2027 5345 4a4f 5552 535f  file = 'SEJOURS_
-00002410: 5354 4154 5f50 4152 5449 4349 5041 5449  STAT_PARTICIPATI
-00002420: 4f4e 2e70 6e67 270d 0a20 2020 2070 6c74  ON.png'..    plt
-00002430: 2e73 6176 6566 6967 2850 6174 6828 474c  .savefig(Path(GL
-00002440: 4f42 414c 5b27 524f 4f54 275d 2920 2f20  OBAL['ROOT']) / 
-00002450: 5061 7468 2873 7472 2879 6561 7229 2920  Path(str(year)) 
-00002460: 2f20 5061 7468 2827 5354 4154 4953 5449  / Path('STATISTI
-00002470: 5155 4553 2729 202f 2050 6174 6828 6669  QUES') / Path(fi
-00002480: 675f 6669 6c65 292c 6262 6f78 5f69 6e63  g_file),bbox_inc
-00002490: 6865 733d 2774 6967 6874 2729 0d0a 2020  hes='tight')..  
-000024a0: 2020 0d0a 6465 6620 7265 6164 5f6d 656d    ..def read_mem
-000024b0: 6f72 795f 736f 7274 6965 7328 293a 0d0a  ory_sorties():..
-000024c0: 0d0a 2020 2020 2320 5374 616e 6461 7264  ..    # Standard
-000024d0: 206c 6962 7261 7279 2069 6d70 6f72 7473   library imports
-000024e0: 0d0a 2020 2020 696d 706f 7274 206f 732e  ..    import os.
-000024f0: 7061 7468 0d0a 2020 2020 6672 6f6d 2070  path..    from p
-00002500: 6174 686c 6962 2069 6d70 6f72 7420 5061  athlib import Pa
-00002510: 7468 0d0a 0d0a 2020 2020 2320 3372 6420  th....    # 3rd 
-00002520: 7061 7274 7920 696d 706f 7274 730d 0a20  party imports.. 
-00002530: 2020 2069 6d70 6f72 7420 7961 6d6c 0d0a     import yaml..
-00002540: 2020 2020 0d0a 2020 2020 2320 5265 6164      ..    # Read
-00002550: 7320 7468 6520 6465 6661 756c 7420 5056  s the default PV
-00002560: 6368 6172 6163 7465 7269 7a61 7469 6f6e  characterization
-00002570: 2e79 616d 6c20 636f 6e66 6967 2066 696c  .yaml config fil
-00002580: 650d 0a20 2020 2070 6174 685f 636f 6e66  e..    path_conf
-00002590: 6967 5f66 696c 6520 3d20 5061 7468 285f  ig_file = Path(_
-000025a0: 5f66 696c 655f 5f29 2e70 6172 656e 742e  _file__).parent.
-000025b0: 7061 7265 6e74 202f 2050 6174 6828 2743  parent / Path('C
-000025c0: 5447 5f46 756e 6327 2920 2f20 5061 7468  TG_Func') / Path
-000025d0: 2827 4354 475f 5265 6646 696c 6573 2729  ('CTG_RefFiles')
-000025e0: 202f 2050 6174 6828 276d 656d 6f72 795f   / Path('memory_
-000025f0: 736f 7274 6965 732e 796d 6c27 290d 0a20  sorties.yml').. 
-00002600: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
-00002610: 685f 636f 6e66 6967 5f66 696c 6529 2061  h_config_file) a
-00002620: 7320 6669 6c65 3a0d 0a20 2020 2020 2020  s file:..       
-00002630: 206d 656d 6f72 7920 3d20 7961 6d6c 2e73   memory = yaml.s
-00002640: 6166 655f 6c6f 6164 2866 696c 6529 0d0a  afe_load(file)..
-00002650: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002660: 200d 0a20 2020 2072 6574 7572 6e20 6d65   ..    return me
-00002670: 6d6f 7279 0d0a 2020 2020 0d0a 6465 6620  mory..    ..def 
-00002680: 6576 6f6c 7574 696f 6e5f 736f 7274 6965  evolution_sortie
-00002690: 7328 7479 7065 2c63 7467 5f70 6174 6829  s(type,ctg_path)
-000026a0: 3a0d 0a0d 0a20 2020 2023 2053 7461 6e64  :....    # Stand
-000026b0: 6172 6420 6c69 6272 6172 7920 696d 706f  ard library impo
-000026c0: 7274 2020 2020 0d0a 2020 2020 696d 706f  rt    ..    impo
-000026d0: 7274 2064 6174 6574 696d 650d 0a20 2020  rt datetime..   
-000026e0: 2066 726f 6d20 7061 7468 6c69 6220 696d   from pathlib im
-000026f0: 706f 7274 2050 6174 680d 0a20 2020 2066  port Path..    f
-00002700: 726f 6d20 636f 6c6c 6563 7469 6f6e 7320  rom collections 
-00002710: 696d 706f 7274 206e 616d 6564 7475 706c  import namedtupl
-00002720: 650d 0a0d 0a20 2020 2023 2054 6869 7264  e....    # Third
-00002730: 2070 6172 7479 206c 6962 7261 7279 2069   party library i
-00002740: 6d70 6f72 7420 2020 2020 0d0a 2020 2020  mport     ..    
-00002750: 696d 706f 7274 206d 6174 706c 6f74 6c69  import matplotli
-00002760: 622e 7079 706c 6f74 2061 7320 706c 740d  b.pyplot as plt.
-00002770: 0a20 2020 2069 6d70 6f72 7420 7061 6e64  .    import pand
-00002780: 6173 2061 7320 7064 0d0a 2020 2020 2020  as as pd..      
-00002790: 0d0a 2020 2020 2320 496e 7465 726e 616c  ..    # Internal
-000027a0: 2069 6d70 6f72 740d 0a20 2020 2069 6d70   import..    imp
-000027b0: 6f72 7420 4354 475f 5574 696c 7320 6173  ort CTG_Utils as
-000027c0: 2063 7467 0d0a 2020 2020 6672 6f6d 2043   ctg..    from C
-000027d0: 5447 5f55 7469 6c73 2e43 5447 5f47 5549  TG_Utils.CTG_GUI
-000027e0: 2e47 5549 5f47 6c6f 6261 6c73 2069 6d70  .GUI_Globals imp
-000027f0: 6f72 7420 4143 5449 5649 5445 5f4c 4953  ort ACTIVITE_LIS
-00002800: 5420 0d0a 2020 2020 0d0a 2020 2020 6465  T ..    ..    de
-00002810: 6620 6164 645f 6d65 6d6f 7279 2873 7461  f add_memory(sta
-00002820: 745f 6469 632c 7965 6172 7329 3a0d 0a20  t_dic,years):.. 
-00002830: 2020 2020 2020 206d 656d 6f72 7920 3d20         memory = 
-00002840: 7265 6164 5f6d 656d 6f72 795f 736f 7274  read_memory_sort
-00002850: 6965 7328 290d 0a20 2020 200d 0a20 2020  ies()..    ..   
-00002860: 200d 0a20 2020 2020 2020 2066 6f72 2079   ..        for y
-00002870: 6561 722c 7620 696e 206d 656d 6f72 795b  ear,v in memory[
-00002880: 276d 656d 6f72 7927 5d2e 6974 656d 7328  'memory'].items(
-00002890: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000028c0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-000028d0: 745f 6469 635b 7374 7228 7965 6172 295d  t_dic[str(year)]
-000028e0: 203d 2073 7461 7479 6561 7228 765b 2753   = statyear(v['S
-000028f0: 454a 4f55 5227 5d2c 2020 2020 2020 2020  EJOUR'],        
-00002900: 2020 2020 2020 2020 2320 6e62 725f 7365          # nbr_se
-00002910: 6a6f 7572 730d 0a20 2020 2020 2020 2020  jours..         
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002940: 2020 302c 2020 2020 2020 2020 2020 2020    0,            
-00002950: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00002960: 6a6f 7572 735f 7365 6a6f 7572 0d0a 2020  jours_sejour..  
-00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 6e74 2879 6561 722c 2063 7467 5f70 6174  nt(year, ctg_pat
+00001f80: 6829 3a0d 0a0d 0a20 2020 2066 726f 6d20  h):....    from 
+00001f90: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
+00001fa0: 7274 2043 6f75 6e74 6572 0d0a 2020 2020  rt Counter..    
+00001fb0: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
+00001fc0: 6f72 7420 5061 7468 0d0a 2020 2020 0d0a  ort Path..    ..
+00001fd0: 2020 2020 696d 706f 7274 206d 6174 706c      import matpl
+00001fe0: 6f74 6c69 622e 7079 706c 6f74 2061 7320  otlib.pyplot as 
+00001ff0: 706c 740d 0a20 2020 2069 6d70 6f72 7420  plt..    import 
+00002000: 7061 6e64 6173 2061 7320 7064 0d0a 2020  pandas as pd..  
+00002010: 2020 0d0a 2020 2020 706c 742e 7374 796c    ..    plt.styl
+00002020: 652e 7573 6528 2767 6770 6c6f 7427 290d  e.use('ggplot').
+00002030: 0a20 2020 200d 0a20 2020 2023 2066 756e  .    ..    # fun
+00002040: 6374 696f 6e20 746f 2061 6464 2076 616c  ction to add val
+00002050: 7565 206c 6162 656c 730d 0a20 2020 2064  ue labels..    d
+00002060: 6566 2061 6464 6c61 6265 6c73 2878 2c79  ef addlabels(x,y
+00002070: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
+00002080: 6920 696e 2072 616e 6765 286c 656e 2878  i in range(len(x
+00002090: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+000020a0: 2070 6c74 2e74 6578 7428 785b 695d 2d30   plt.text(x[i]-0
+000020b0: 2e32 2c79 5b69 5d2b 312c 795b 695d 2c73  .2,y[i]+1,y[i],s
+000020c0: 697a 653d 6c61 6265 6c5f 7369 7a65 290d  ize=label_size).
+000020d0: 0a20 2020 206c 6162 656c 5f73 697a 6520  .    label_size 
+000020e0: 3d20 3135 0d0a 2020 2020 6669 6c65 5f69  = 15..    file_i
+000020f0: 6e20 3d20 6374 675f 7061 7468 202f 2050  n = ctg_path / P
+00002100: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
+00002110: 2050 6174 6828 2753 5441 5449 5354 4951   Path('STATISTIQ
+00002120: 5545 5327 2920 2f20 5061 7468 2827 7379  UES') / Path('sy
+00002130: 6e74 6865 7365 5f61 6468 6572 656e 742e  nthese_adherent.
+00002140: 786c 7378 2729 0d0a 2020 2020 6466 5f74  xlsx')..    df_t
+00002150: 6f74 616c 203d 2070 642e 7265 6164 5f65  otal = pd.read_e
+00002160: 7863 656c 2866 696c 655f 696e 290d 0a20  xcel(file_in).. 
+00002170: 2020 200d 0a20 2020 2063 203d 2043 6f75     ..    c = Cou
+00002180: 6e74 6572 2829 0d0a 2020 2020 6320 3d20  nter()..    c = 
+00002190: 436f 756e 7465 7228 6466 5f74 6f74 616c  Counter(df_total
+000021a0: 5b27 4e62 725f 5345 4a4f 5552 5327 5d2e  ['Nbr_SEJOURS'].
+000021b0: 746f 6c69 7374 2829 290d 0a20 2020 2063  tolist())..    c
+000021c0: 203d 2063 2e6d 6f73 745f 636f 6d6d 6f6e   = c.most_common
+000021d0: 2829 0d0a 0d0a 2020 2020 782c 2079 203d  ()....    x, y =
+000021e0: 207a 6970 282a 6329 0d0a 2020 2020 7820   zip(*c)..    x 
+000021f0: 3d20 6c69 7374 2878 290d 0a20 2020 2079  = list(x)..    y
+00002200: 203d 206c 6973 7428 7929 0d0a 2020 2020   = list(y)..    
+00002210: 0d0a 2020 2020 6669 672c 2061 7820 3d20  ..    fig, ax = 
+00002220: 706c 742e 7375 6270 6c6f 7473 2866 6967  plt.subplots(fig
+00002230: 7369 7a65 3d28 352c 3529 290d 0a20 2020  size=(5,5))..   
+00002240: 2070 6c74 2e62 6172 285b 7374 7228 785f   plt.bar([str(x_
+00002250: 7329 2066 6f72 2078 5f73 2069 6e20 785d  s) for x_s in x]
+00002260: 2c79 290d 0a20 2020 2070 6c74 2e78 6c61  ,y)..    plt.xla
+00002270: 6265 6c28 274e 6f6d 6272 6520 6465 2070  bel('Nombre de p
+00002280: 6172 7469 6369 7061 7469 6f6e 20c3 a020  articipation .. 
+00002290: 6465 7320 73c3 a96a 6f75 7273 2729 0d0a  des s..jours')..
+000022a0: 2020 2020 706c 742e 796c 6162 656c 2827      plt.ylabel('
+000022b0: 4e6f 6d62 7265 2064 6520 6c69 6365 6e63  Nombre de licenc
+000022c0: 6965 7273 2729 0d0a 2020 2020 706c 742e  iers')..    plt.
+000022d0: 7469 636b 5f70 6172 616d 7328 6178 6973  tick_params(axis
+000022e0: 3d27 7827 2c20 6c61 6265 6c73 697a 653d  ='x', labelsize=
+000022f0: 6c61 6265 6c5f 7369 7a65 290d 0a20 2020  label_size)..   
+00002300: 2070 6c74 2e74 6963 6b5f 7061 7261 6d73   plt.tick_params
+00002310: 2861 7869 733d 2779 272c 206c 6162 656c  (axis='y', label
+00002320: 7369 7a65 3d6c 6162 656c 5f73 697a 6529  size=label_size)
+00002330: 0d0a 2020 2020 706c 742e 7469 746c 6528  ..    plt.title(
+00002340: 7374 7228 7965 6172 292c 7061 643d 3230  str(year),pad=20
+00002350: 2c20 666f 6e74 7369 7a65 3d32 3029 0d0a  , fontsize=20)..
+00002360: 2020 2020 0d0a 2020 2020 6178 2e73 6574      ..    ax.set
+00002370: 5f78 6c61 6265 6c28 274e 2073 c3a9 6a6f  _xlabel('N s..jo
+00002380: 7572 7327 2c20 666f 6e74 7369 7a65 203d  urs', fontsize =
+00002390: 206c 6162 656c 5f73 697a 6529 0d0a 2020   label_size)..  
+000023a0: 2020 6178 2e73 6574 5f79 6c61 6265 6c28    ax.set_ylabel(
+000023b0: 274e 6f6d 6272 6520 6465 2043 5447 2061  'Nombre de CTG a
+000023c0: 7961 6e74 205c 6e20 7061 7274 6963 6970  yant \n particip
+000023d0: c3a9 20c3 a020 4e20 73c3 a96a 6f75 7273  .. .. N s..jours
+000023e0: 272c 2066 6f6e 7473 697a 6520 3d20 6c61  ', fontsize = la
+000023f0: 6265 6c5f 7369 7a65 290d 0a20 2020 200d  bel_size)..    .
+00002400: 0a20 2020 2078 2e73 6f72 7428 290d 0a20  .    x.sort().. 
+00002410: 2020 2061 6464 6c61 6265 6c73 2878 2c79     addlabels(x,y
+00002420: 290d 0a20 2020 2070 6c74 2e74 6967 6874  )..    plt.tight
+00002430: 5f6c 6179 6f75 7428 290d 0a20 2020 2070  _layout()..    p
+00002440: 6c74 2e73 686f 7728 290d 0a0d 0a20 2020  lt.show()....   
+00002450: 2066 6967 5f66 696c 6520 3d20 2753 454a   fig_file = 'SEJ
+00002460: 4f55 5253 5f53 5441 545f 5041 5254 4943  OURS_STAT_PARTIC
+00002470: 4950 4154 494f 4e2e 706e 6727 0d0a 2020  IPATION.png'..  
+00002480: 2020 706c 742e 7361 7665 6669 6728 5061    plt.savefig(Pa
+00002490: 7468 2847 4c4f 4241 4c5b 2752 4f4f 5427  th(GLOBAL['ROOT'
+000024a0: 5d29 202f 2050 6174 6828 7374 7228 7965  ]) / Path(str(ye
+000024b0: 6172 2929 202f 2050 6174 6828 2753 5441  ar)) / Path('STA
+000024c0: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
+000024d0: 7468 2866 6967 5f66 696c 6529 2c62 626f  th(fig_file),bbo
+000024e0: 785f 696e 6368 6573 3d27 7469 6768 7427  x_inches='tight'
+000024f0: 290d 0a20 2020 200d 0a64 6566 2072 6561  )..    ..def rea
+00002500: 645f 6d65 6d6f 7279 5f73 6f72 7469 6573  d_memory_sorties
+00002510: 2829 3a0d 0a0d 0a20 2020 2023 2053 7461  ():....    # Sta
+00002520: 6e64 6172 6420 6c69 6272 6172 7920 696d  ndard library im
+00002530: 706f 7274 730d 0a20 2020 2069 6d70 6f72  ports..    impor
+00002540: 7420 6f73 2e70 6174 680d 0a20 2020 2066  t os.path..    f
+00002550: 726f 6d20 7061 7468 6c69 6220 696d 706f  rom pathlib impo
+00002560: 7274 2050 6174 680d 0a0d 0a20 2020 2023  rt Path....    #
+00002570: 2033 7264 2070 6172 7479 2069 6d70 6f72   3rd party impor
+00002580: 7473 0d0a 2020 2020 696d 706f 7274 2079  ts..    import y
+00002590: 616d 6c0d 0a20 2020 200d 0a20 2020 2023  aml..    ..    #
+000025a0: 2052 6561 6473 2074 6865 2064 6566 6175   Reads the defau
+000025b0: 6c74 2050 5663 6861 7261 6374 6572 697a  lt PVcharacteriz
+000025c0: 6174 696f 6e2e 7961 6d6c 2063 6f6e 6669  ation.yaml confi
+000025d0: 6720 6669 6c65 0d0a 2020 2020 7061 7468  g file..    path
+000025e0: 5f63 6f6e 6669 675f 6669 6c65 203d 2050  _config_file = P
+000025f0: 6174 6828 5f5f 6669 6c65 5f5f 292e 7061  ath(__file__).pa
+00002600: 7265 6e74 2e70 6172 656e 7420 2f20 5061  rent.parent / Pa
+00002610: 7468 2827 4354 475f 4675 6e63 2729 202f  th('CTG_Func') /
+00002620: 2050 6174 6828 2743 5447 5f52 6566 4669   Path('CTG_RefFi
+00002630: 6c65 7327 2920 2f20 5061 7468 2827 6d65  les') / Path('me
+00002640: 6d6f 7279 5f73 6f72 7469 6573 2e79 6d6c  mory_sorties.yml
+00002650: 2729 0d0a 2020 2020 7769 7468 206f 7065  ')..    with ope
+00002660: 6e28 7061 7468 5f63 6f6e 6669 675f 6669  n(path_config_fi
+00002670: 6c65 2920 6173 2066 696c 653a 0d0a 2020  le) as file:..  
+00002680: 2020 2020 2020 6d65 6d6f 7279 203d 2079        memory = y
+00002690: 616d 6c2e 7361 6665 5f6c 6f61 6428 6669  aml.safe_load(fi
+000026a0: 6c65 290d 0a20 2020 2020 2020 200d 0a20  le)..        .. 
+000026b0: 2020 2020 2020 0d0a 2020 2020 7265 7475        ..    retu
+000026c0: 726e 206d 656d 6f72 790d 0a20 2020 200d  rn memory..    .
+000026d0: 0a64 6566 2065 766f 6c75 7469 6f6e 5f73  .def evolution_s
+000026e0: 6f72 7469 6573 2874 7970 652c 6374 675f  orties(type,ctg_
+000026f0: 7061 7468 293a 0d0a 0d0a 2020 2020 2320  path):....    # 
+00002700: 5374 616e 6461 7264 206c 6962 7261 7279  Standard library
+00002710: 2069 6d70 6f72 7420 2020 200d 0a20 2020   import    ..   
+00002720: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
+00002730: 0d0a 2020 2020 6672 6f6d 2070 6174 686c  ..    from pathl
+00002740: 6962 2069 6d70 6f72 7420 5061 7468 0d0a  ib import Path..
+00002750: 2020 2020 6672 6f6d 2063 6f6c 6c65 6374      from collect
+00002760: 696f 6e73 2069 6d70 6f72 7420 6e61 6d65  ions import name
+00002770: 6474 7570 6c65 0d0a 0d0a 2020 2020 2320  dtuple....    # 
+00002780: 5468 6972 6420 7061 7274 7920 6c69 6272  Third party libr
+00002790: 6172 7920 696d 706f 7274 2020 2020 200d  ary import     .
+000027a0: 0a20 2020 2069 6d70 6f72 7420 6d61 7470  .    import matp
+000027b0: 6c6f 746c 6962 2e70 7970 6c6f 7420 6173  lotlib.pyplot as
+000027c0: 2070 6c74 0d0a 2020 2020 696d 706f 7274   plt..    import
+000027d0: 2070 616e 6461 7320 6173 2070 640d 0a20   pandas as pd.. 
+000027e0: 2020 2020 200d 0a20 2020 2023 2049 6e74       ..    # Int
+000027f0: 6572 6e61 6c20 696d 706f 7274 0d0a 2020  ernal import..  
+00002800: 2020 696d 706f 7274 2043 5447 5f55 7469    import CTG_Uti
+00002810: 6c73 2061 7320 6374 670d 0a20 2020 2066  ls as ctg..    f
+00002820: 726f 6d20 4354 475f 5574 696c 732e 4354  rom CTG_Utils.CT
+00002830: 475f 4755 492e 4755 495f 476c 6f62 616c  G_GUI.GUI_Global
+00002840: 7320 696d 706f 7274 2041 4354 4956 4954  s import ACTIVIT
+00002850: 455f 4c49 5354 200d 0a20 2020 200d 0a20  E_LIST ..    .. 
+00002860: 2020 2064 6566 2061 6464 5f6d 656d 6f72     def add_memor
+00002870: 7928 7374 6174 5f64 6963 2c79 6561 7273  y(stat_dic,years
+00002880: 293a 0d0a 2020 2020 2020 2020 6d65 6d6f  ):..        memo
+00002890: 7279 203d 2072 6561 645f 6d65 6d6f 7279  ry = read_memory
+000028a0: 5f73 6f72 7469 6573 2829 0d0a 2020 2020  _sorties()..    
+000028b0: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
+000028c0: 666f 7220 7965 6172 2c76 2069 6e20 6d65  for year,v in me
+000028d0: 6d6f 7279 5b27 6d65 6d6f 7279 275d 2e69  mory['memory'].i
+000028e0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002910: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00002920: 2020 7374 6174 5f64 6963 5b73 7472 2879    stat_dic[str(y
+00002930: 6561 7229 5d20 3d20 7374 6174 7965 6172  ear)] = statyear
+00002940: 2876 5b27 5041 5254 4943 4950 4154 494f  (v['PARTICIPATIO
+00002950: 4e5f 5345 4a4f 5552 5327 5d2c 2020 2020  N_SEJOURS'],    
+00002960: 2020 2020 2020 2020 2020 2020 2320 6e62              # nb
+00002970: 725f 7365 6a6f 7572 730d 0a20 2020 2020  r_sejours..     
 00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 2020 2020 2020 2020 2076 5b27 534f 5254           v['SORT
-000029a0: 4945 535f 434c 5542 5f44 494d 414e 4348  IES_CLUB_DIMANCH
-000029b0: 4527 5d2c 2023 2073 6f72 7469 655f 6469  E'], # sortie_di
-000029c0: 6d61 6e63 6865 5f63 6c75 620d 0a20 2020  manche_club..   
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029a0: 2020 2020 2020 302c 2020 2020 2020 2020        0,        
+000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029c0: 2020 2320 6a6f 7572 735f 7365 6a6f 7572    # jours_sejour
+000029d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2020 2020 2020 765b 2753 4f52 5449          v['SORTI
-00002a00: 4553 5f43 4c55 425f 5341 4d45 4449 275d  ES_CLUB_SAMEDI']
-00002a10: 2c20 2020 2320 736f 7274 6965 5f73 616d  ,   # sortie_sam
-00002a20: 6564 695f 636c 7562 0d0a 2020 2020 2020  edi_club..      
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 2020 2020 2020 2020 2020 2020 2076 5b27               v['
+00002a00: 534f 5254 4945 535f 434c 5542 5f44 494d  SORTIES_CLUB_DIM
+00002a10: 414e 4348 4527 5d2c 2023 2073 6f72 7469  ANCHE'], # sorti
+00002a20: 655f 6469 6d61 6e63 6865 5f63 6c75 620d  e_dimanche_club.
+00002a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a50: 2020 2020 2076 5b27 534f 5254 4945 535f       v['SORTIES_
-00002a60: 4849 5645 5227 5d2c 2020 2020 2020 2020  HIVER'],        
-00002a70: 2023 2073 6f72 7469 655f 6869 7665 725f   # sortie_hiver_
-00002a80: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
+00002a50: 2020 2020 2020 2020 2020 2020 765b 2753              v['S
+00002a60: 4f52 5449 4553 5f43 4c55 425f 5341 4d45  ORTIES_CLUB_SAME
+00002a70: 4449 275d 2c20 2020 2320 736f 7274 6965  DI'],   # sortie
+00002a80: 5f73 616d 6564 695f 636c 7562 0d0a 2020  _samedi_club..  
 00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ab0: 2076 5b27 534f 5254 4945 535f 434c 5542   v['SORTIES_CLUB
-00002ac0: 5f4a 4555 4449 275d 2c20 2020 2023 2073  _JEUDI'],    # s
-00002ad0: 6f72 7469 655f 6a65 7564 695f 636c 7562  ortie_jeudi_club
-00002ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002ab0: 2020 2020 2020 2020 2076 5b27 534f 5254           v['SORT
+00002ac0: 4945 535f 4849 5645 5227 5d2c 2020 2020  IES_HIVER'],    
+00002ad0: 2020 2020 2023 2073 6f72 7469 655f 6869       # sortie_hi
+00002ae0: 7665 725f 636c 7562 0d0a 2020 2020 2020  ver_club..      
 00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2020 2020 2020 2020 2020 2020 2076 5b27               v['
-00002b10: 5241 4e44 4f4e 4e45 4553 275d 2c20 2020  RANDONNEES'],   
-00002b20: 2020 2020 2020 2020 2023 2072 616e 646f           # rando
-00002b30: 6e6e 6565 0d0a 2020 2020 2020 2020 2020  nnee..          
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b10: 2020 2020 2076 5b27 534f 5254 4945 535f       v['SORTIES_
+00002b20: 434c 5542 5f4a 4555 4449 275d 2c20 2020  CLUB_JEUDI'],   
+00002b30: 2023 2073 6f72 7469 655f 6a65 7564 695f   # sortie_jeudi_
+00002b40: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
 00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 2030 2c20 2020 2020 2020 2020 2020 2020   0,             
-00002b70: 2020 2020 2020 2020 2020 2020 2023 206e               # n
-00002b80: 6272 5f73 656a 6f75 7273 0d0a 2020 2020  br_sejours..    
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b70: 2076 5b27 5241 4e44 4f4e 4e45 4553 275d   v['RANDONNEES']
+00002b80: 2c20 2020 2020 2020 2020 2020 2023 2072  ,            # r
+00002b90: 616e 646f 6e6e 6565 0d0a 2020 2020 2020  andonnee..      
 00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 2020 2020 2020 2030 2c29 2020 2020 2020         0,)      
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bd0: 2020 2023 206e 6272 5f6a 6f75 7273 5f73     # nbr_jours_s
-00002be0: 656a 6f75 7273 0d0a 2020 2020 2020 2020  ejours..        
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 2020 2076 5b27 4e6f 6d62 7265 5f73       v['Nombre_s
+00002bd0: 656a 6f75 7273 275d 2c20 2020 2020 2020  ejours'],       
+00002be0: 2023 206e 6272 5f73 656a 6f75 7273 0d0a   # nbr_sejours..
 00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c20: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00002c30: 2020 7965 6172 732e 6170 7065 6e64 2873    years.append(s
-00002c40: 7472 2879 6561 7229 290d 0a20 2020 2020  tr(year))..     
+00002c10: 2020 2020 2020 2020 2020 2030 2c29 2020             0,)  
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 2020 2020 2023 206e 6272 5f6a 6f75         # nbr_jou
+00002c40: 7273 5f73 656a 6f75 7273 0d0a 2020 2020  rs_sejours..    
 00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00002c70: 2064 6566 2066 696c 6c5f 7374 6174 5f79   def fill_stat_y
-00002c80: 6561 7228 7965 6172 293a 0d0a 2020 2020  ear(year):..    
-00002c90: 2020 2020 6672 6f6d 2043 5447 5f55 7469      from CTG_Uti
-00002ca0: 6c73 2e43 5447 5f46 756e 632e 4354 475f  ls.CTG_Func.CTG_
-00002cb0: 7574 696c 6974 7920 696d 706f 7274 2067  utility import g
-00002cc0: 6574 5f73 656a 6f75 725f 696e 666f 0d0a  et_sejour_info..
-00002cd0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002ce0: 2020 7365 6a6f 7572 5f69 6e66 6f20 3d20    sejour_info = 
-00002cf0: 6765 745f 7365 6a6f 7572 5f69 6e66 6f28  get_sejour_info(
-00002d00: 6374 675f 7061 7468 2c79 6561 7229 0d0a  ctg_path,year)..
-00002d10: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002d20: 2020 0d0a 2020 2020 2020 2020 6669 6c65    ..        file
-00002d30: 5f69 6e20 3d20 6374 675f 7061 7468 202f  _in = ctg_path /
-00002d40: 2050 6174 6828 7374 7228 7965 6172 2929   Path(str(year))
-00002d50: 202f 2050 6174 6828 2753 5441 5449 5354   / Path('STATIST
-00002d60: 4951 5545 5327 2920 2f20 5061 7468 2827  IQUES') / Path('
-00002d70: 7379 6e74 6865 7365 5f61 6468 6572 656e  synthese_adheren
-00002d80: 742e 786c 7378 2729 0d0a 2020 2020 2020  t.xlsx')..      
-00002d90: 2020 0d0a 2020 2020 2020 2020 6466 203d    ..        df =
-00002da0: 2070 642e 7265 6164 5f65 7863 656c 2866   pd.read_excel(f
-00002db0: 696c 655f 696e 290d 0a20 2020 2020 2020  ile_in)..       
-00002dc0: 200d 0a20 2020 2020 2020 2073 7461 745f   ..        stat_
-00002dd0: 7965 6172 203d 2073 7461 7479 6561 7228  year = statyear(
-00002de0: 6466 5b27 4e62 725f 5345 4a4f 5552 5327  df['Nbr_SEJOURS'
-00002df0: 5d2e 7375 6d28 292c 2020 2020 2020 2020  ].sum(),        
-00002e00: 2020 2020 2023 206e 6272 5f6a 6f75 7273       # nbr_jours
-00002e10: 5f70 6172 7469 6369 7061 7469 6f6e 5f73  _participation_s
-00002e20: 656a 6f75 7273 0d0a 2020 2020 2020 2020  ejours..        
-00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e40: 2020 2020 2064 665b 2753 454a 4f55 522d       df['SEJOUR-
-00002e50: 4a4f 5552 275d 2e73 756d 2829 2c20 2020  JOUR'].sum(),   
-00002e60: 2020 2020 2020 2020 2020 2320 6e62 725f            # nbr_
-00002e70: 7061 7274 6963 6970 6174 696f 6e73 5f73  participations_s
-00002e80: 656a 6f75 720d 0a20 2020 2020 2020 2020  ejour..         
-00002e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ea0: 2020 2020 6466 5b27 534f 5254 4945 2044      df['SORTIE D
-00002eb0: 5520 4449 4d41 4e43 4845 2043 4c55 4227  U DIMANCHE CLUB'
-00002ec0: 5d2e 7375 6d28 292c 2023 2073 6f72 7469  ].sum(), # sorti
-00002ed0: 655f 6469 6d61 6e63 6865 5f63 6c75 620d  e_dimanche_club.
-00002ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ef0: 2020 2020 2020 2020 2020 2020 2020 6466                df
-00002f00: 5b27 534f 5254 4945 2044 5520 5341 4d45  ['SORTIE DU SAME
-00002f10: 4449 2043 4c55 4227 5d2e 7375 6d28 292c  DI CLUB'].sum(),
-00002f20: 2020 2023 2073 6f72 7469 655f 7361 6d65     # sortie_same
-00002f30: 6469 5f63 6c75 620d 0a20 2020 2020 2020  di_club..       
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2020 2020 2020 6466 5b27 534f 5254 4945        df['SORTIE
-00002f60: 2048 4956 4552 275d 2e73 756d 2829 2c20   HIVER'].sum(), 
-00002f70: 2020 2020 2020 2020 2020 2023 2073 6f72             # sor
-00002f80: 7469 655f 6869 7665 725f 636c 7562 0d0a  tie_hiver_club..
-00002f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fa0: 2020 2020 2020 2020 2020 2020 2064 665b               df[
-00002fb0: 2753 4f52 5449 4520 4455 204a 4555 4449  'SORTIE DU JEUDI
-00002fc0: 2043 4c55 4227 5d2e 7375 6d28 292c 2020   CLUB'].sum(),  
-00002fd0: 2020 2320 736f 7274 6965 5f6a 6575 6469    # sortie_jeudi
-00002fe0: 5f63 6c75 620d 0a20 2020 2020 2020 2020  _club..         
-00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003000: 2020 2020 6466 5b27 5241 4e44 4f4e 4e45      df['RANDONNE
-00003010: 4527 5d2e 7375 6d28 292c 2020 2020 2020  E'].sum(),      
-00003020: 2020 2020 2020 2020 2023 2072 616e 646f           # rando
-00003030: 6e6e 6565 0d0a 2020 2020 2020 2020 2020  nnee..          
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 2020 2073 656a 6f75 725f 696e 666f 2e6e     sejour_info.n
-00003060: 6272 5f73 656a 6f75 7273 2c20 2020 2020  br_sejours,     
-00003070: 2020 2020 2020 2020 2320 6e62 725f 7365          # nbr_se
-00003080: 6a6f 7572 7320 0d0a 2020 2020 2020 2020  jours ..        
-00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030a0: 2020 2020 2073 656a 6f75 725f 696e 666f       sejour_info
-000030b0: 2e6e 6272 5f6a 6f75 7273 2920 2020 2020  .nbr_jours)     
-000030c0: 2020 2020 2020 2020 2020 2320 6e62 725f            # nbr_
-000030d0: 6a6f 7572 735f 7365 6a6f 7572 7320 2020  jours_sejours   
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003110: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003120: 2020 2020 7265 7475 726e 2073 7461 745f      return stat_
-00003130: 7965 6172 0d0a 2020 2020 0d0a 2020 2020  year..    ..    
-00003140: 6465 6620 6164 646c 6162 656c 7328 782c  def addlabels(x,
-00003150: 792c 6f66 6673 6574 293a 0d0a 2020 2020  y,offset):..    
-00003160: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00003170: 6765 286c 656e 2878 2929 3a0d 0a20 2020  ge(len(x)):..   
-00003180: 2020 2020 2020 2020 2070 6c74 2e74 6578           plt.tex
-00003190: 7428 785b 695d 2c79 5b69 5d2b 6f66 6673  t(x[i],y[i]+offs
-000031a0: 6574 2c72 6f75 6e64 2879 5b69 5d2c 3129  et,round(y[i],1)
-000031b0: 2c73 697a 653d 3130 290d 0a20 2020 2020  ,size=10)..     
-000031c0: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-000031d0: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
-000031e0: 2c6e 625f 7061 7274 6963 6970 616e 7473  ,nb_participants
-000031f0: 2c74 6974 6c65 293a 0d0a 2020 2020 2020  ,title):..      
-00003200: 2020 706c 742e 7375 6270 6c6f 7428 312c    plt.subplot(1,
-00003210: 312c 3129 0d0a 2020 2020 2020 2020 636f  1,1)..        co
-00003220: 6c6f 7273 203d 205b 2723 6664 6161 3438  lors = ['#fdaa48
-00003230: 275d 200d 0a20 2020 2020 2020 2073 697a  '] ..        siz
-00003240: 655f 6c61 6265 6c20 3d20 3230 0d0a 2020  e_label = 20..  
-00003250: 2020 2020 2020 706c 742e 6261 7228 7965        plt.bar(ye
-00003260: 6172 732c 6e62 5f70 6172 7469 6369 7061  ars,nb_participa
-00003270: 6e74 732c 636f 6c6f 723d 636f 6c6f 7273  nts,color=colors
-00003280: 290d 0a20 2020 2020 2020 2070 6c74 2e79  )..        plt.y
-00003290: 6c61 6265 6c28 2223 2070 6172 7469 6369  label("# partici
-000032a0: 7061 6e74 7322 2c73 697a 653d 7369 7a65  pants",size=size
-000032b0: 5f6c 6162 656c 290d 0a20 2020 2020 2020  _label)..       
-000032c0: 2061 6464 6c61 6265 6c73 2879 6561 7273   addlabels(years
-000032d0: 2c6e 625f 7061 7274 6963 6970 616e 7473  ,nb_participants
-000032e0: 2c31 290d 0a20 2020 2020 2020 2070 6c74  ,1)..        plt
-000032f0: 2e78 7469 636b 7328 726f 7461 7469 6f6e  .xticks(rotation
-00003300: 3d39 3029 0d0a 2020 2020 2020 2020 706c  =90)..        pl
-00003310: 742e 7469 636b 5f70 6172 616d 7328 6178  t.tick_params(ax
-00003320: 6973 3d27 7827 2c20 6c61 6265 6c73 697a  is='x', labelsiz
-00003330: 653d 7369 7a65 5f6c 6162 656c 290d 0a20  e=size_label).. 
-00003340: 2020 2020 2020 2070 6c74 2e74 6963 6b5f         plt.tick_
-00003350: 7061 7261 6d73 2861 7869 733d 2779 272c  params(axis='y',
-00003360: 206c 6162 656c 7369 7a65 3d73 697a 655f   labelsize=size_
-00003370: 6c61 6265 6c29 0d0a 2020 2020 2020 2020  label)..        
-00003380: 706c 742e 7469 746c 6528 7469 746c 652c  plt.title(title,
-00003390: 666f 6e74 7369 7a65 3d31 3829 0d0a 2020  fontsize=18)..  
-000033a0: 2020 2020 2020 706c 742e 7469 6768 745f        plt.tight_
-000033b0: 6c61 796f 7574 2829 0d0a 2020 2020 2020  layout()..      
-000033c0: 2020 706c 742e 7368 6f77 2829 0d0a 2020    plt.show()..  
-000033d0: 2020 0d0a 2020 2020 7374 6174 7965 6172    ..    statyear
-000033e0: 203d 206e 616d 6564 7475 706c 6528 2761   = namedtuple('a
-000033f0: 6374 6976 6974 6527 2c20 4143 5449 5649  ctivite', ACTIVI
-00003400: 5445 5f4c 4953 5429 0d0a 200d 0a20 2020  TE_LIST).. ..   
-00003410: 2070 6c74 2e73 7479 6c65 2e75 7365 2827   plt.style.use('
-00003420: 6767 706c 6f74 2729 0d0a 2020 2020 7965  ggplot')..    ye
-00003430: 6172 7320 3d20 5b5d 0d0a 2020 2020 7374  ars = []..    st
-00003440: 6174 5f64 6963 203d 207b 7d0d 0a20 2020  at_dic = {}..   
-00003450: 2061 6464 5f6d 656d 6f72 7928 7374 6174   add_memory(stat
-00003460: 5f64 6963 2c79 6561 7273 290d 0a0d 0a20  _dic,years).... 
-00003470: 2020 2074 6f64 6179 203d 2064 6174 6574     today = datet
-00003480: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
-00003490: 2829 0d0a 2020 2020 7965 6172 735f 6e65  ()..    years_ne
-000034a0: 7720 3d20 5b73 7472 2879 6561 7229 2066  w = [str(year) f
-000034b0: 6f72 2079 6561 7220 696e 2072 616e 6765  or year in range
-000034c0: 2832 3032 322c 746f 6461 792e 7965 6172  (2022,today.year
-000034d0: 2b31 295d 0d0a 2020 2020 666f 7220 7965  +1)]..    for ye
-000034e0: 6172 2069 6e20 7965 6172 735f 6e65 773a  ar in years_new:
-000034f0: 0d0a 2020 2020 2020 2020 7374 6174 5f64  ..        stat_d
-00003500: 6963 5b79 6561 725d 203d 2066 696c 6c5f  ic[year] = fill_
-00003510: 7374 6174 5f79 6561 7228 7965 6172 290d  stat_year(year).
-00003520: 0a20 2020 2020 2020 200d 0a20 2020 2079  .        ..    y
-00003530: 6561 7273 203d 2079 6561 7273 202b 2079  ears = years + y
-00003540: 6561 7273 5f6e 6577 2020 200d 0a20 2020  ears_new   ..   
-00003550: 200d 0a20 2020 200d 0a20 2020 2069 6620   ..    ..    if 
-00003560: 7479 7065 203d 3d20 276e 6272 5f6a 6f75  type == 'nbr_jou
-00003570: 7273 5f70 6172 7469 6369 7061 7469 6f6e  rs_participation
-00003580: 5f73 656a 6f75 7273 273a 0d0a 2020 2020  _sejours':..    
-00003590: 2020 2020 706c 6f74 5f73 7461 7428 7965      plot_stat(ye
-000035a0: 6172 732c 5b73 7461 745f 6469 635b 7965  ars,[stat_dic[ye
-000035b0: 6172 5d2e 6e62 725f 6a6f 7572 735f 7061  ar].nbr_jours_pa
-000035c0: 7274 6963 6970 6174 696f 6e5f 7365 6a6f  rticipation_sejo
-000035d0: 7572 7320 666f 7220 7965 6172 2069 6e20  urs for year in 
-000035e0: 7965 6172 735d 2c74 7970 6529 0d0a 2020  years],type)..  
-000035f0: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
-00003600: 2773 6f72 7469 655f 6469 6d61 6e63 6865  'sortie_dimanche
-00003610: 5f63 6c75 6227 3a0d 0a20 2020 2020 2020  _club':..       
+00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00002c90: 2020 2020 2020 7965 6172 732e 6170 7065        years.appe
+00002ca0: 6e64 2873 7472 2879 6561 7229 290d 0a20  nd(str(year)).. 
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00002cd0: 0a20 2020 2064 6566 2066 696c 6c5f 7374  .    def fill_st
+00002ce0: 6174 5f79 6561 7228 7965 6172 293a 0d0a  at_year(year):..
+00002cf0: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
+00002d00: 496e 7465 726e 616c 206c 6962 7261 7279  Internal library
+00002d10: 2069 6d70 6f72 7473 0d0a 2020 2020 2020   imports..      
+00002d20: 2020 6672 6f6d 2043 5447 5f55 7469 6c73    from CTG_Utils
+00002d30: 2e43 5447 5f46 756e 632e 4354 475f 7574  .CTG_Func.CTG_ut
+00002d40: 696c 6974 7920 696d 706f 7274 2067 6574  ility import get
+00002d50: 5f73 656a 6f75 725f 696e 666f 0d0a 2020  _sejour_info..  
+00002d60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00002d70: 7365 6a6f 7572 5f69 6e66 6f20 3d20 6765  sejour_info = ge
+00002d80: 745f 7365 6a6f 7572 5f69 6e66 6f28 6374  t_sejour_info(ct
+00002d90: 675f 7061 7468 2c79 6561 7229 0d0a 2020  g_path,year)..  
+00002da0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00002db0: 0d0a 2020 2020 2020 2020 6669 6c65 5f69  ..        file_i
+00002dc0: 6e20 3d20 6374 675f 7061 7468 202f 2050  n = ctg_path / P
+00002dd0: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
+00002de0: 2050 6174 6828 2753 5441 5449 5354 4951   Path('STATISTIQ
+00002df0: 5545 5327 2920 2f20 5061 7468 2827 7379  UES') / Path('sy
+00002e00: 6e74 6865 7365 5f61 6468 6572 656e 742e  nthese_adherent.
+00002e10: 786c 7378 2729 0d0a 2020 2020 2020 2020  xlsx')..        
+00002e20: 0d0a 2020 2020 2020 2020 6466 203d 2070  ..        df = p
+00002e30: 642e 7265 6164 5f65 7863 656c 2866 696c  d.read_excel(fil
+00002e40: 655f 696e 290d 0a20 2020 2020 2020 200d  e_in)..        .
+00002e50: 0a20 2020 2020 2020 2073 7461 745f 7965  .        stat_ye
+00002e60: 6172 203d 2073 7461 7479 6561 7228 6466  ar = statyear(df
+00002e70: 5b27 4e62 725f 5345 4a4f 5552 5327 5d2e  ['Nbr_SEJOURS'].
+00002e80: 7375 6d28 292c 2020 2020 2020 2020 2020  sum(),          
+00002e90: 2020 2023 206e 6272 5f6a 6f75 7273 5f70     # nbr_jours_p
+00002ea0: 6172 7469 6369 7061 7469 6f6e 5f73 656a  articipation_sej
+00002eb0: 6f75 7273 0d0a 2020 2020 2020 2020 2020  ours..          
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ed0: 2020 2064 665b 2753 454a 4f55 522d 4a4f     df['SEJOUR-JO
+00002ee0: 5552 275d 2e73 756d 2829 2c20 2020 2020  UR'].sum(),     
+00002ef0: 2020 2020 2020 2020 2320 6e62 725f 7061          # nbr_pa
+00002f00: 7274 6963 6970 6174 696f 6e73 5f73 656a  rticipations_sej
+00002f10: 6f75 720d 0a20 2020 2020 2020 2020 2020  our..           
+00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f30: 2020 6466 5b27 534f 5254 4945 2044 5520    df['SORTIE DU 
+00002f40: 4449 4d41 4e43 4845 2043 4c55 4227 5d2e  DIMANCHE CLUB'].
+00002f50: 7375 6d28 292c 2023 2073 6f72 7469 655f  sum(), # sortie_
+00002f60: 6469 6d61 6e63 6865 5f63 6c75 620d 0a20  dimanche_club.. 
+00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f80: 2020 2020 2020 2020 2020 2020 6466 5b27              df['
+00002f90: 534f 5254 4945 2044 5520 5341 4d45 4449  SORTIE DU SAMEDI
+00002fa0: 2043 4c55 4227 5d2e 7375 6d28 292c 2020   CLUB'].sum(),  
+00002fb0: 2023 2073 6f72 7469 655f 7361 6d65 6469   # sortie_samedi
+00002fc0: 5f63 6c75 620d 0a20 2020 2020 2020 2020  _club..         
+00002fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fe0: 2020 2020 6466 5b27 534f 5254 4945 2048      df['SORTIE H
+00002ff0: 4956 4552 275d 2e73 756d 2829 2c20 2020  IVER'].sum(),   
+00003000: 2020 2020 2020 2020 2023 2073 6f72 7469           # sorti
+00003010: 655f 6869 7665 725f 636c 7562 0d0a 2020  e_hiver_club..  
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 2020 2020 2020 2020 2020 2064 665b 2753             df['S
+00003040: 4f52 5449 4520 4455 204a 4555 4449 2043  ORTIE DU JEUDI C
+00003050: 4c55 4227 5d2e 7375 6d28 292c 2020 2020  LUB'].sum(),    
+00003060: 2320 736f 7274 6965 5f6a 6575 6469 5f63  # sortie_jeudi_c
+00003070: 6c75 620d 0a20 2020 2020 2020 2020 2020  lub..           
+00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003090: 2020 6466 5b27 5241 4e44 4f4e 4e45 4527    df['RANDONNEE'
+000030a0: 5d2e 7375 6d28 292c 2020 2020 2020 2020  ].sum(),        
+000030b0: 2020 2020 2020 2023 2072 616e 646f 6e6e         # randonn
+000030c0: 6565 0d0a 2020 2020 2020 2020 2020 2020  ee..            
+000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030e0: 2073 656a 6f75 725f 696e 666f 2e6e 6272   sejour_info.nbr
+000030f0: 5f73 656a 6f75 7273 2c20 2020 2020 2020  _sejours,       
+00003100: 2020 2020 2020 2320 6e62 725f 7365 6a6f        # nbr_sejo
+00003110: 7572 7320 0d0a 2020 2020 2020 2020 2020  urs ..          
+00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003130: 2020 2073 656a 6f75 725f 696e 666f 2e6e     sejour_info.n
+00003140: 6272 5f6a 6f75 7273 2920 2020 2020 2020  br_jours)       
+00003150: 2020 2020 2020 2020 2320 6e62 725f 6a6f          # nbr_jo
+00003160: 7572 735f 7365 6a6f 7572 7320 2020 2020  urs_sejours     
+00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003180: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031a0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000031b0: 2020 7265 7475 726e 2073 7461 745f 7965    return stat_ye
+000031c0: 6172 0d0a 2020 2020 0d0a 2020 2020 6465  ar..    ..    de
+000031d0: 6620 6164 646c 6162 656c 7328 782c 792c  f addlabels(x,y,
+000031e0: 6f66 6673 6574 293a 0d0a 2020 2020 2020  offset):..      
+000031f0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00003200: 286c 656e 2878 2929 3a0d 0a20 2020 2020  (len(x)):..     
+00003210: 2020 2020 2020 2070 6c74 2e74 6578 7428         plt.text(
+00003220: 785b 695d 2c79 5b69 5d2b 6f66 6673 6574  x[i],y[i]+offset
+00003230: 2c72 6f75 6e64 2879 5b69 5d2c 3129 2c73  ,round(y[i],1),s
+00003240: 697a 653d 3130 290d 0a20 2020 2020 2020  ize=10)..       
+00003250: 2020 2020 200d 0a20 2020 2064 6566 2070       ..    def p
+00003260: 6c6f 745f 7374 6174 2879 6561 7273 2c6e  lot_stat(years,n
+00003270: 625f 7061 7274 6963 6970 616e 7473 2c74  b_participants,t
+00003280: 6974 6c65 2c6c 6162 656c 5f79 293a 0d0a  itle,label_y):..
+00003290: 2020 2020 2020 2020 706c 742e 7375 6270          plt.subp
+000032a0: 6c6f 7428 312c 312c 3129 0d0a 2020 2020  lot(1,1,1)..    
+000032b0: 2020 2020 636f 6c6f 7273 203d 205b 2723      colors = ['#
+000032c0: 6664 6161 3438 275d 200d 0a20 2020 2020  fdaa48'] ..     
+000032d0: 2020 2073 697a 655f 6c61 6265 6c20 3d20     size_label = 
+000032e0: 3230 0d0a 2020 2020 2020 2020 706c 742e  20..        plt.
+000032f0: 6261 7228 7965 6172 732c 6e62 5f70 6172  bar(years,nb_par
+00003300: 7469 6369 7061 6e74 732c 636f 6c6f 723d  ticipants,color=
+00003310: 636f 6c6f 7273 290d 0a20 2020 2020 2020  colors)..       
+00003320: 2070 6c74 2e79 6c61 6265 6c28 6c61 6265   plt.ylabel(labe
+00003330: 6c5f 792c 7369 7a65 3d73 697a 655f 6c61  l_y,size=size_la
+00003340: 6265 6c29 0d0a 2020 2020 2020 2020 6164  bel)..        ad
+00003350: 646c 6162 656c 7328 7965 6172 732c 6e62  dlabels(years,nb
+00003360: 5f70 6172 7469 6369 7061 6e74 732c 3129  _participants,1)
+00003370: 0d0a 2020 2020 2020 2020 706c 742e 7874  ..        plt.xt
+00003380: 6963 6b73 2872 6f74 6174 696f 6e3d 3930  icks(rotation=90
+00003390: 290d 0a20 2020 2020 2020 2070 6c74 2e74  )..        plt.t
+000033a0: 6963 6b5f 7061 7261 6d73 2861 7869 733d  ick_params(axis=
+000033b0: 2778 272c 206c 6162 656c 7369 7a65 3d73  'x', labelsize=s
+000033c0: 697a 655f 6c61 6265 6c29 0d0a 2020 2020  ize_label)..    
+000033d0: 2020 2020 706c 742e 7469 636b 5f70 6172      plt.tick_par
+000033e0: 616d 7328 6178 6973 3d27 7927 2c20 6c61  ams(axis='y', la
+000033f0: 6265 6c73 697a 653d 7369 7a65 5f6c 6162  belsize=size_lab
+00003400: 656c 290d 0a20 2020 2020 2020 2070 6c74  el)..        plt
+00003410: 2e74 6974 6c65 2874 6974 6c65 2c66 6f6e  .title(title,fon
+00003420: 7473 697a 653d 3138 290d 0a20 2020 2020  tsize=18)..     
+00003430: 2020 2070 6c74 2e74 6967 6874 5f6c 6179     plt.tight_lay
+00003440: 6f75 7428 290d 0a20 2020 2020 2020 2070  out()..        p
+00003450: 6c74 2e73 686f 7728 290d 0a20 2020 200d  lt.show()..    .
+00003460: 0a20 2020 2073 7461 7479 6561 7220 3d20  .    statyear = 
+00003470: 6e61 6d65 6474 7570 6c65 2827 6163 7469  namedtuple('acti
+00003480: 7669 7465 272c 2041 4354 4956 4954 455f  vite', ACTIVITE_
+00003490: 4c49 5354 290d 0a20 0d0a 2020 2020 706c  LIST).. ..    pl
+000034a0: 742e 7374 796c 652e 7573 6528 2767 6770  t.style.use('ggp
+000034b0: 6c6f 7427 290d 0a20 2020 2079 6561 7273  lot')..    years
+000034c0: 203d 205b 5d0d 0a20 2020 2073 7461 745f   = []..    stat_
+000034d0: 6469 6320 3d20 7b7d 0d0a 2020 2020 6164  dic = {}..    ad
+000034e0: 645f 6d65 6d6f 7279 2873 7461 745f 6469  d_memory(stat_di
+000034f0: 632c 7965 6172 7329 0d0a 0d0a 2020 2020  c,years)....    
+00003500: 746f 6461 7920 3d20 6461 7465 7469 6d65  today = datetime
+00003510: 2e64 6174 6574 696d 652e 6e6f 7728 290d  .datetime.now().
+00003520: 0a20 2020 2079 6561 7273 5f6e 6577 203d  .    years_new =
+00003530: 205b 7374 7228 7965 6172 2920 666f 7220   [str(year) for 
+00003540: 7965 6172 2069 6e20 7261 6e67 6528 3230  year in range(20
+00003550: 3232 2c74 6f64 6179 2e79 6561 722b 3129  22,today.year+1)
+00003560: 5d0d 0a20 2020 2066 6f72 2079 6561 7220  ]..    for year 
+00003570: 696e 2079 6561 7273 5f6e 6577 3a0d 0a20  in years_new:.. 
+00003580: 2020 2020 2020 2073 7461 745f 6469 635b         stat_dic[
+00003590: 7965 6172 5d20 3d20 6669 6c6c 5f73 7461  year] = fill_sta
+000035a0: 745f 7965 6172 2879 6561 7229 0d0a 2020  t_year(year)..  
+000035b0: 2020 2020 2020 0d0a 2020 2020 7965 6172        ..    year
+000035c0: 7320 3d20 7965 6172 7320 2b20 7965 6172  s = years + year
+000035d0: 735f 6e65 7720 2020 0d0a 2020 2020 0d0a  s_new   ..    ..
+000035e0: 2020 2020 0d0a 2020 2020 6966 2074 7970      ..    if typ
+000035f0: 6520 3d3d 2027 6e62 725f 6a6f 7572 735f  e == 'nbr_jours_
+00003600: 7061 7274 6963 6970 6174 696f 6e5f 7365  participation_se
+00003610: 6a6f 7572 7327 3a0d 0a20 2020 2020 2020  jours':..       
 00003620: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
-00003630: 2c5b 7374 6174 5f64 6963 5b79 6561 725d  ,[stat_dic[year]
-00003640: 2e73 6f72 7469 655f 6469 6d61 6e63 6865  .sortie_dimanche
-00003650: 5f63 6c75 6220 666f 7220 7965 6172 2069  _club for year i
-00003660: 6e20 7965 6172 735d 2c74 7970 6529 0d0a  n years],type)..
-00003670: 2020 2020 656c 6966 2020 7479 7065 203d      elif  type =
-00003680: 3d20 2773 6f72 7469 655f 7361 6d65 6469  = 'sortie_samedi
-00003690: 5f63 6c75 6227 3a0d 0a20 2020 2020 2020  _club':..       
-000036a0: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
-000036b0: 2c5b 7374 6174 5f64 6963 5b79 6561 725d  ,[stat_dic[year]
-000036c0: 2e73 6f72 7469 655f 7361 6d65 6469 5f63  .sortie_samedi_c
-000036d0: 6c75 6220 666f 7220 7965 6172 2069 6e20  lub for year in 
-000036e0: 7965 6172 735d 2c74 7970 6529 0d0a 2020  years],type)..  
-000036f0: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
-00003700: 2773 6f72 7469 655f 6a65 7564 695f 636c  'sortie_jeudi_cl
-00003710: 7562 273a 0d0a 2020 2020 2020 2020 706c  ub':..        pl
-00003720: 6f74 5f73 7461 7428 7965 6172 732c 5b73  ot_stat(years,[s
-00003730: 7461 745f 6469 635b 7965 6172 5d2e 736f  tat_dic[year].so
-00003740: 7274 6965 5f6a 6575 6469 5f63 6c75 6220  rtie_jeudi_club 
-00003750: 666f 7220 7965 6172 2069 6e20 7965 6172  for year in year
-00003760: 735d 2c74 7970 6529 2020 0d0a 2020 2020  s],type)  ..    
-00003770: 656c 6966 2020 7479 7065 203d 3d20 2772  elif  type == 'r
-00003780: 616e 646f 6e6e 6565 273a 0d0a 2020 2020  andonnee':..    
-00003790: 2020 2020 706c 6f74 5f73 7461 7428 7965      plot_stat(ye
-000037a0: 6172 732c 5b73 7461 745f 6469 635b 7965  ars,[stat_dic[ye
-000037b0: 6172 5d2e 7261 6e64 6f6e 6e65 6520 666f  ar].randonnee fo
-000037c0: 7220 7965 6172 2069 6e20 7965 6172 735d  r year in years]
-000037d0: 2c74 7970 6529 2020 0d0a 2020 2020 656c  ,type)  ..    el
-000037e0: 6966 2020 7479 7065 203d 3d20 276e 6272  if  type == 'nbr
-000037f0: 5f70 6172 7469 6369 7061 7469 6f6e 735f  _participations_
-00003800: 7365 6a6f 7572 7327 3a0d 0a20 2020 2020  sejours':..     
-00003810: 2020 2070 6c6f 745f 7374 6174 2879 6561     plot_stat(yea
-00003820: 7273 2c5b 7374 6174 5f64 6963 5b79 6561  rs,[stat_dic[yea
-00003830: 725d 2e6e 6272 5f70 6172 7469 6369 7061  r].nbr_participa
-00003840: 7469 6f6e 735f 7365 6a6f 7572 7320 666f  tions_sejours fo
-00003850: 7220 7965 6172 2069 6e20 7965 6172 735d  r year in years]
-00003860: 2c27 4e6f 6d62 7265 2064 6520 7061 7274  ,'Nombre de part
-00003870: 6963 6970 6174 696f 6e73 2061 7578 2073  icipations aux s
-00003880: c3a9 6a6f 7572 7327 2920 0d0a 2020 2020  ..jours') ..    
-00003890: 656c 6966 2020 7479 7065 203d 3d20 276e  elif  type == 'n
-000038a0: 6272 5f73 656a 6f75 7273 273a 0d0a 2020  br_sejours':..  
-000038b0: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
-000038c0: 7965 6172 732c 5b73 7461 745f 6469 635b  years,[stat_dic[
-000038d0: 7965 6172 5d2e 6e62 725f 7365 6a6f 7572  year].nbr_sejour
-000038e0: 7320 666f 7220 7965 6172 2069 6e20 7965  s for year in ye
-000038f0: 6172 735d 2c27 4e6f 6d62 7265 2064 6520  ars],'Nombre de 
-00003900: 73c3 a96a 6f75 7273 2729 0d0a 2020 2020  s..jours')..    
-00003910: 656c 6966 2020 7479 7065 203d 3d20 276e  elif  type == 'n
-00003920: 6272 5f6a 6f75 7273 5f73 656a 6f75 7273  br_jours_sejours
-00003930: 273a 0d0a 2020 2020 2020 2020 706c 6f74  ':..        plot
-00003940: 5f73 7461 7428 7965 6172 732c 5b73 7461  _stat(years,[sta
-00003950: 745f 6469 635b 7965 6172 5d2e 6e62 725f  t_dic[year].nbr_
-00003960: 6a6f 7572 735f 7365 6a6f 7572 7320 666f  jours_sejours fo
-00003970: 7220 7965 6172 2069 6e20 7965 6172 735d  r year in years]
-00003980: 2c27 4e6f 6d62 7265 2064 6520 73c3 a96a  ,'Nombre de s..j
-00003990: 6f75 7273 2729 2020 2020 2020 2020       ours')        
+00003630: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003640: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
+00003650: 6561 725d 2e6e 6272 5f6a 6f75 7273 5f70  ear].nbr_jours_p
+00003660: 6172 7469 6369 7061 7469 6f6e 5f73 656a  articipation_sej
+00003670: 6f75 7273 2066 6f72 2079 6561 7220 696e  ours for year in
+00003680: 2079 6561 7273 5d2c 0d0a 2020 2020 2020   years],..      
+00003690: 2020 2020 2020 2020 2020 2020 7479 7065              type
+000036a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000036b0: 2020 2020 2074 7970 6529 0d0a 2020 2020       type)..    
+000036c0: 656c 6966 2020 7479 7065 203d 3d20 2773  elif  type == 's
+000036d0: 6f72 7469 655f 6469 6d61 6e63 6865 5f63  ortie_dimanche_c
+000036e0: 6c75 6227 3a0d 0a20 2020 2020 2020 2070  lub':..        p
+000036f0: 6c6f 745f 7374 6174 2879 6561 7273 2c0d  lot_stat(years,.
+00003700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003710: 2020 205b 7374 6174 5f64 6963 5b79 6561     [stat_dic[yea
+00003720: 725d 2e73 6f72 7469 655f 6469 6d61 6e63  r].sortie_dimanc
+00003730: 6865 5f63 6c75 6220 666f 7220 7965 6172  he_club for year
+00003740: 2069 6e20 7965 6172 735d 2c0d 0a20 2020   in years],..   
+00003750: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00003760: 7970 652c 0d0a 2020 2020 2020 2020 2020  ype,..          
+00003770: 2020 2020 2020 2020 2723 7061 7274 6963          '#partic
+00003780: 6970 616e 7473 2729 0d0a 2020 2020 656c  ipants')..    el
+00003790: 6966 2020 7479 7065 203d 3d20 2773 6f72  if  type == 'sor
+000037a0: 7469 655f 7361 6d65 6469 5f63 6c75 6227  tie_samedi_club'
+000037b0: 3a0d 0a20 2020 2020 2020 2070 6c6f 745f  :..        plot_
+000037c0: 7374 6174 2879 6561 7273 2c0d 0a20 2020  stat(years,..   
+000037d0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000037e0: 7374 6174 5f64 6963 5b79 6561 725d 2e73  stat_dic[year].s
+000037f0: 6f72 7469 655f 7361 6d65 6469 5f63 6c75  ortie_samedi_clu
+00003800: 6220 666f 7220 7965 6172 2069 6e20 7965  b for year in ye
+00003810: 6172 735d 2c0d 0a20 2020 2020 2020 2020  ars],..         
+00003820: 2020 2020 2020 2020 2074 7970 652c 0d0a           type,..
+00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003840: 2020 2723 7061 7274 6963 6970 616e 7473    '#participants
+00003850: 2729 0d0a 2020 2020 656c 6966 2020 7479  ')..    elif  ty
+00003860: 7065 203d 3d20 2773 6f72 7469 655f 6a65  pe == 'sortie_je
+00003870: 7564 695f 636c 7562 273a 0d0a 2020 2020  udi_club':..    
+00003880: 2020 2020 706c 6f74 5f73 7461 7428 7965      plot_stat(ye
+00003890: 6172 732c 0d0a 2020 2020 2020 2020 2020  ars,..          
+000038a0: 2020 2020 2020 2020 5b73 7461 745f 6469          [stat_di
+000038b0: 635b 7965 6172 5d2e 736f 7274 6965 5f6a  c[year].sortie_j
+000038c0: 6575 6469 5f63 6c75 6220 666f 7220 7965  eudi_club for ye
+000038d0: 6172 2069 6e20 7965 6172 735d 2c0d 0a20  ar in years],.. 
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038f0: 2074 7970 652c 0d0a 2020 2020 2020 2020   type,..        
+00003900: 2020 2020 2020 2020 2020 2723 7061 7274            '#part
+00003910: 6963 6970 616e 7473 2729 2020 0d0a 2020  icipants')  ..  
+00003920: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
+00003930: 2772 616e 646f 6e6e 6565 273a 0d0a 2020  'randonnee':..  
+00003940: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
+00003950: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
+00003960: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
+00003970: 6469 635b 7965 6172 5d2e 7261 6e64 6f6e  dic[year].randon
+00003980: 6e65 6520 666f 7220 7965 6172 2069 6e20  nee for year in 
+00003990: 7965 6172 735d 2c0d 0a20 2020 2020 2020  years],..       
+000039a0: 2020 2020 2020 2020 2020 2074 7970 652c             type,
+000039b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000039c0: 2020 2020 2723 7061 7274 6963 6970 616e      '#participan
+000039d0: 7473 2729 2020 0d0a 2020 2020 656c 6966  ts')  ..    elif
+000039e0: 2020 7479 7065 203d 3d20 276e 6272 5f70    type == 'nbr_p
+000039f0: 6172 7469 6369 7061 7469 6f6e 735f 7365  articipations_se
+00003a00: 6a6f 7572 7327 3a0d 0a20 2020 2020 2020  jours':..       
+00003a10: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
+00003a20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003a30: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
+00003a40: 6561 725d 2e6e 6272 5f70 6172 7469 6369  ear].nbr_partici
+00003a50: 7061 7469 6f6e 735f 7365 6a6f 7572 7320  pations_sejours 
+00003a60: 666f 7220 7965 6172 2069 6e20 7965 6172  for year in year
+00003a70: 735d 2c0d 0a20 2020 2020 2020 2020 2020  s],..           
+00003a80: 2020 2020 2020 2027 4e6f 6d62 7265 2064         'Nombre d
+00003a90: 6520 7061 7274 6963 6970 6174 696f 6e73  e participations
+00003aa0: 2061 7578 2073 c3a9 6a6f 7572 7327 2c0d   aux s..jours',.
+00003ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ac0: 2020 2027 2320 7061 7274 6963 6970 6174     '# participat
+00003ad0: 696f 6e73 2061 7578 2073 c3a9 6a6f 7572  ions aux s..jour
+00003ae0: 7327 2920 0d0a 2020 2020 656c 6966 2020  s') ..    elif  
+00003af0: 7479 7065 203d 3d20 276e 6272 5f73 656a  type == 'nbr_sej
+00003b00: 6f75 7273 273a 0d0a 2020 2020 2020 2020  ours':..        
+00003b10: 706c 6f74 5f73 7461 7428 7965 6172 732c  plot_stat(years,
+00003b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003b30: 2020 2020 5b73 7461 745f 6469 635b 7965      [stat_dic[ye
+00003b40: 6172 5d2e 6e62 725f 7365 6a6f 7572 7320  ar].nbr_sejours 
+00003b50: 666f 7220 7965 6172 2069 6e20 7965 6172  for year in year
+00003b60: 735d 2c0d 0a20 2020 2020 2020 2020 2020  s],..           
+00003b70: 2020 2020 2020 2027 4e6f 6d62 7265 2064         'Nombre d
+00003b80: 6520 73c3 a96a 6f75 7273 272c 0d0a 2020  e s..jours',..  
+00003b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ba0: 2723 2073 c3a9 6a6f 7572 7327 290d 0a20  '# s..jours').. 
+00003bb0: 2020 2065 6c69 6620 2074 7970 6520 3d3d     elif  type ==
+00003bc0: 2027 6e62 725f 6a6f 7572 735f 7365 6a6f   'nbr_jours_sejo
+00003bd0: 7572 7327 3a0d 0a20 2020 2020 2020 2070  urs':..        p
+00003be0: 6c6f 745f 7374 6174 2879 6561 7273 2c0d  lot_stat(years,.
+00003bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003c00: 2020 205b 7374 6174 5f64 6963 5b79 6561     [stat_dic[yea
+00003c10: 725d 2e6e 6272 5f6a 6f75 7273 5f73 656a  r].nbr_jours_sej
+00003c20: 6f75 7273 2066 6f72 2079 6561 7220 696e  ours for year in
+00003c30: 2079 6561 7273 5d2c 0d0a 2020 2020 2020   years],..      
+00003c40: 2020 2020 2020 2020 2020 2020 274e 6f6d              'Nom
+00003c50: 6272 6520 6465 206a 6f75 7273 2073 c3a9  bre de jours s..
+00003c60: 6a6f 7572 7327 2c0d 0a20 2020 2020 2020  jours',..       
+00003c70: 2020 2020 2020 2020 2020 2027 2320 6a6f             '# jo
+00003c80: 7572 7320 73c3 a96a 6f75 7227 2920 2020  urs s..jour')   
+00003c90: 2020 2020 20
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_Func/CTG_utility.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_Func/CTG_utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 def parse_date(s,year):
-    
+
+    # Standard library imports
     import re
     from datetime import datetime 
 
     convert_to_date = lambda s: datetime.strptime(s,"%Y_%m_%d")
     s = re.sub(r"-","_",s)
     
     try:
@@ -14,17 +15,20 @@
         pattern = re.compile(r"(?P<month>\d{1,2}_)(?P<day>\d{1,2})")
         match = pattern.search(s)
         date = convert_to_date(str(year)+'_'+match.group("month")+match.group("day"))
     
     return date
 
 def day_of_the_date(day,month,year):
-    # Compute the day of the week of the date after "Elementary Number Theory David M. Burton Chap 6.4" [1]
+
+    # Standard library imports
     import itertools
     from calendar import monthrange
+    
+    # Compute the day of the week of the date after "Elementary Number Theory David M. Burton Chap 6.4" [1]
     days_dict = {0: 'dimanche',
                  1: 'Lundi',
                  2: 'mardi',
                  3: 'mercredi',
                  4: 'jeudi',
                  5: 'vendredi',
                  6: 'samedi'}
@@ -39,14 +43,15 @@
     m = month_dict[month]
     if m>10 : y = y-1
 
     return days_dict[(day + int(2.6*m - 0.2) - 2*c + y + int(c/4) + int(y/4))%7] # [1] thm 6.12
     
 def parse_date(s,year):
     
+    # Standard library imports
     import re
     from datetime import datetime 
 
     convert_to_date = lambda s: datetime.strptime(s,"%Y_%m_%d")
     s = re.sub(r"-","_",s)
     
     try:
@@ -125,20 +130,20 @@
     
     return df
     
 def get_sejour_info(ctg_path,year):
 
     # Standard library imports 
     from collections import namedtuple
+    from collections import Counter
     
     sejour_info = namedtuple('sejour_info', 'nbr_jours nbr_sejours histo')
     df =  yamlinfo_randos2df(ctg_path,year)
     info_sejour = [nbr_jours for nbr_jours in df['nbr_jours'] if nbr_jours>1]
-    from collections import Counter
+    
     c = Counter()
     c = Counter(info_sejour)
 
-    sejour_info.nbr_jours= sum(info_sejour)
-    sejour_info.nbr_sejours= len(info_sejour)
-    sejour_info.histo = c
     
-    return sejour_info
+    sejour_info_tup = sejour_info( sum(info_sejour),len(info_sejour),c)
+    
+    return sejour_info_tup
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/GUI_Globals.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/GUI_Globals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __all__ = ['ACTIVITE_LIST',
            'ADD_SPACE_MM',           
            'BM_GUI_DISP',
            'CONTAINER_BUTTON_HEIGHT_PX',
-           'CORPUSES_NUMBER',
+           'FIRST_YEAR',
            'DIR_SORTIES_LIST',
            'FONT_NAME',
            'HELP_EVOLUTION_EFFECTIF',
            'HELP_MEMBER_ANALYSIS',
            'HELP_RANDO',
            'HELP_SORTIES',
            'HELP_SYNTHESE_SORTIES',
@@ -84,25 +84,31 @@
            'TEXT_YEAR_PC',
            'TEXT_YEAR_PI',
            'TEXT_TENDANCE_SORTIES',
            'HELP_TENDANCE_SORTIES',
            'BUTT_TENDANCE_SORTIES',
            'TEXT_PRESENCE_EFFECTIF',
            'HELP_PRESENCE_EFFECTIF',
-           'BUTT_PRESENCE_EFFECTIF',           
-           ]
+           'BUTT_PRESENCE_EFFECTIF',
+           'TEXT_GEO_PI',
+           'TEXT_GEO',
+           'HELP_GEO',
+           'BUTT_GEO',           
+           'TEXT_NBR_SEJOURS',
+           'HELP_NBR_SEJOURS',
+           'BUTT_NBR_SEJOURS']
 
 
 ################################## General globals ##################################
 
 # Setting BiblioMeter version value (internal)
-VERSION ='4.0.0'
+VERSION ='5.0.0'
 
-# Setting the number of corpuses to analyse
-CORPUSES_NUMBER = 2021
+# Setting the first available year -1 for activity following
+FIRST_YEAR = 2021
 
 # Setting the title of the application main window (internal)
 APPLICATION_WINDOW_TITLE = f"CTG_Meter - Analyse des statistiques des effectifs et des sorties"
 
 ######################## Definition of display globals ###########################
 
 def _get_displays(in_to_mm): 
@@ -239,19 +245,20 @@
 REF_SORTIES_BUT_POS_X_MM   = 10      #10
 REF_SORTIES_BUT_POS_Y_MM   = 50      #26
 
 # Separation space in mm for check boxes
 REF_CHECK_BOXES_SEP_SPACE  = 25      #25
 
 # Setting label for each gui page
-PAGES_LABELS = {'PageEffectif'      : "Analyse des effectifs",
-                'PageSorties': "Analyse des sorties",
+PAGES_LABELS = {'PageEffectif': "Analyse des effectifs",
+                'PageSorties' : "Analyse des sorties",
                 'PageSynthese': "Synthèse des sorties et effectifs",
                 'PageTendance': "Analyse de l'évolution temporelle des pratiques ",
-                'PageTendance': "Analyse tendancielle"
+                'PageTendance': "Analyse tendancielle",
+                'PageDivers'  : "Autres analyses",
                }
 
 
 ########################## Cover Page (BiblioMeter launching Page) ##########################
 
 # Titre de la page
 TEXT_TITLE                  = "- CTG_Meter -\nInitialisation de l'analyse"
@@ -350,23 +357,30 @@
 BUTT_MEMBER_ANALYSIS    = "Construction du fichier EXCEL"
 
 ### - Page analyse tendancielle
 TEXT_ACTIVITE_PI = "Choix de l'activité"
 TEXT_TENDANCE_SORTIES     = "Analyse tendancielle des sorties"
 HELP_TENDANCE_SORTIES     = " La synthèse est effectuée à partir des fichiers"
 HELP_TENDANCE_SORTIES    += " d'émargement aux sorties, randonnées et séjours"
-BUTT_TENDANCE_SORTIES = "Lancer l'analyse"
-TEXT_PRESENCE_EFFECTIF     = "Analyse de la présence an club"
-HELP_PRESENCE_EFFECTIF     = " L'analyse de l'évolution de l'effectif est issue"
-HELP_PRESENCE_EFFECTIF    += " des archives disponnibles à partir de 2012."
+BUTT_TENDANCE_SORTIES     = "Lancer l'analyse"
+TEXT_PRESENCE_EFFECTIF    = "Analyse de la présence an club"
+HELP_PRESENCE_EFFECTIF    = " L'analyse de l'évolution de l'effectif est issue"
+HELP_PRESENCE_EFFECTIF   += " des archives disponnibles à partir de 2012."
 BUTT_PRESENCE_EFFECTIF = "Lancer l'analyse de l'évolution des effectifs"
-#TEXT_MEMBER_ANALYSIS    = "Analyse des sorties par adhérent"
-#HELP_MEMBER_ANALYSIS    = " Analyse de la participation aux sorties, randonnées et séjour "
-#HELP_MEMBER_ANALYSIS   += " par adhérent. Un fichier EXCEL est généré."
-#BUTT_MEMBER_ANALYSIS    = "Construction du fichier EXCEL"
+
+### - Page analyse tendancielle
+TEXT_GEO_PI               = "Choix de l'année"
+TEXT_GEO                  = "Analyse de la répartition géographique des adhérents"
+HELP_GEO                  = " La synthèse est effectuée à partir des fichiers"
+HELP_GEO                 += " EXCEL extraits de https://cyclo38ffct.fr/"
+BUTT_GEO                  = "Lancer la construction du fichier html"
+TEXT_NBR_SEJOURS          = "Histogramme de nombre de membres ayant participé à N séjours"
+HELP_NBR_SEJOURS    = " La construction de l'histogramme est issue"
+HELP_NBR_SEJOURS   += " de l'anlyse du fichier EXCEL : 'synthese_adherent.xl'."
+BUTT_NBR_SEJOURS = "Lancer la construction de l'histogramme"
 
 
 ################# Liste répertoires
 DIR_SORTIES_LIST = ['SEJOUR',
                     'SORTIES DE DERNIERE MINUTE',
                     'SORTIES DU DIMANCHE',
                     'SORTIES DU JEUDI',
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/PageEffectif.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageEffectif.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/PageSorties.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageSorties.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/PageSynthese.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageSynthese.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     
         # Getting year selection
         year_select =  variable_years.get()
         
         synthese_adherent(year_select,ctg_path)
         info_title = "- Information -"
         info_text  = f"L'analyse de la participation aux sorties par membre a été effectuée pour l'année {year_select} "
-        info_text += f"\n\nLe fichier EXCEL obtenu synthese_adherent.xlsx a été créé dans le dossier :"
+        info_text += f"\n\nLe fichier EXCEL obtenu : 'synthese_adherent.xlsx' a été créé dans le dossier :"
         info_text += f"\n\n{ctg_path}\{str(year_select)}\STATISTIQUES."
   
         messagebox.showinfo(info_title, info_text) 
     
     
     # Setting effective font sizes and positions (numbers are reference values)
     eff_etape_font_size      = font_size(gg.REF_ETAPE_FONT_SIZE,   AppMain.width_sf_min)           #14
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/PageTendance.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/PageTendance.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/Page_Classes.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Page_Classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,37 +15,53 @@
         # Standard library imports
         from pathlib import Path
         
         # 3rd party imports
         from screeninfo import get_monitors
         
         # Local imports
-        from CTG_Utils.CTG_GUI.Useful_Functions import general_properties
+        from CTG_Utils.CTG_GUI.Useful_Functions import window_properties
+        import CTG_Utils.CTG_GUI.GUI_Globals as gg
         
         # Setting the link with "tk.Tk"
         tk.Tk.__init__(master)
 
   
         # Identifying tk window of init class   
         _ = get_monitors() # OBLIGATOIRE        
         master.attributes("-topmost", True)
+        
+        # Setting the icon
+        master.iconbitmap( Path(__file__).parent.parent / Path('CTG_Func') / Path('CTG_RefFiles') / Path( 'logoctg4.ico') ) 
 
-        print(Path(__file__).parent.parent / Path('CTG_Func') /Path('CTG_RefFiles') / Path( 'logoctg4.ico'))
-        master.iconbitmap( Path(__file__).parent.parent / Path('CTG_Func') / Path('CTG_RefFiles') / Path( 'logoctg4.ico') )        
+        # Setting title window
+        master.title(gg.APPLICATION_WINDOW_TITLE)
+        
+        # Setting window size depending on scale factor
+        screen_width_px  = master.winfo_screenwidth()
+        screen_height_px = master.winfo_screenheight()
+        
+        sizes_tuple = window_properties(screen_width_px, screen_height_px)
+        
+        win_width_px  = sizes_tuple[0]
+        win_height_px = sizes_tuple[1]
+        
+        master.geometry(f"{win_width_px}x{win_height_px}")
+        master.resizable(False, False)           
         
         # Defining pages classes and pages list
-        AppMain.pages = ( PageTendance,
+        AppMain.pages = ( PageDivers,
+                          PageTendance,
                           PageSynthese,
                           PageEffectif,
                           PageSorties,                     
                          )
         AppMain.pages_ordered_list = [x.__name__ for x in AppMain.pages][::-1]
         
         # Getting useful screen sizes and scale factors depending on displays properties
-        sizes_tuple = general_properties(master)
         AppMain.win_width_px  = sizes_tuple[0]
         AppMain.win_height_px = sizes_tuple[1]
         AppMain.width_sf_px   = sizes_tuple[2] 
         AppMain.height_sf_px  = sizes_tuple[3]     # unused here
         AppMain.width_sf_mm   = sizes_tuple[4]
         AppMain.height_sf_mm  = sizes_tuple[5]
         AppMain.width_sf_min  = min(AppMain.width_sf_mm, AppMain.width_sf_px)
@@ -71,15 +87,14 @@
         from tkinter import font as tkFont
         from functools import partial
         from pathlib import Path
         
         # Local imports
         import CTG_Utils.CTG_GUI.GUI_Globals as gg 
         from CTG_Utils.CTG_GUI.Useful_Functions import font_size
-        from CTG_Utils.CTG_GUI.Useful_Functions import general_properties
         from CTG_Utils.CTG_GUI.Useful_Functions import last_available_years
         from CTG_Utils.CTG_GUI.Useful_Functions import mm_to_px 
         from CTG_Utils.CTG_GUI.Useful_Functions import place_after
         from CTG_Utils.CTG_GUI.Useful_Functions import str_size_mm
         from CTG_Utils.CTG_GUI.Useful_Functions import create_archi
         
         # Internal functions - start        
@@ -138,24 +153,24 @@
             bmf_val2.set((_display_path(inst_bmf))) 
         
         def _create_corpus(inst_bmf):
             corpi_val = _set_corpi_widgets_param(inst_bmf)
             bmf_path = Path(inst_bmf)
             try: 
                 # Setting new corpus year folder name
-                corpuses_list    = last_available_years(bmf_path, gg.CORPUSES_NUMBER)
+                corpuses_list    = last_available_years(bmf_path, gg.FIRST_YEAR)
                 last_corpus_year = corpuses_list[-1]
                 new_corpus_year_folder = str(int(last_corpus_year) + 1)
                 
                 # Creating required folders for new corpus year
                 message = create_archi(bmf_path, new_corpus_year_folder, verbose = False)
                 print("\n",message)
 
                 # Getting updated corpuses list
-                corpuses_list = last_available_years(bmf_path, gg.CORPUSES_NUMBER)
+                corpuses_list = last_available_years(bmf_path, gg.FIRST_YEAR)
                 
                 # Setting corpi_val value to corpuses list 
                 corpi_val.set(str(corpuses_list))
                 
             except FileNotFoundError:
                 warning_title = "!!! ATTENTION : Dossier de travail inaccessible !!!"
                 warning_text  = f"L'accès au dossier {bmf_path} est impossible."
@@ -195,15 +210,15 @@
             return corpi_val
             
         def _update_corpi(inst_bmf):
             corpi_val = _set_corpi_widgets_param(inst_bmf)
             bmf_path = Path(inst_bmf)
             try: 
                 # Getting updated corpuses list
-                corpuses_list = last_available_years(bmf_path, gg.CORPUSES_NUMBER)
+                corpuses_list = last_available_years(bmf_path, gg.FIRST_YEAR)
                 # Setting corpi_val value to corpuses list
                 corpi_val.set(str(corpuses_list))
                 
             except FileNotFoundError:
                 warning_title = "!!! ATTENTION : Dossier de travail inaccessible !!!"
                 warning_text  = f"L'accès au dossier {bmf_path} est impossible."
                 warning_text += f"\nChoisissez un autre dossier de travail."                       
@@ -221,15 +236,15 @@
             # Managing working folder (bmf stands for "BiblioMeter_Files") 
             _set_bmf_widget_param(institute_select, inst_default_bmf)
             
             # Managing corpus list
             corpi_val = _set_corpi_widgets_param(inst_default_bmf)            
                 # Setting and displating corpuses list initial values
             try:
-                init_corpuses_list = last_available_years(inst_default_bmf, gg.CORPUSES_NUMBER)
+                init_corpuses_list = last_available_years(inst_default_bmf, gg.FIRST_YEAR)
                 corpi_val.set(str(init_corpuses_list))
             except FileNotFoundError:
                 warning_title = "!!! ATTENTION : Dossier de travail inaccessible !!!"
                 warning_text  = f"L'accès au dossier {inst_default_bmf} est impossible."
                 warning_text += f"\nChoisissez un autre dossier de travail."                       
                 messagebox.showwarning(warning_title, warning_text)
                 # Setting corpuses list value to empty string
@@ -519,14 +534,34 @@
         
         setcontrollerbutton = SetControllerButton(master, container_button,page_name)
         
         settitleclass = SetTitltleClass(self,page_name,institute)
         
         quitapp = QuitApp(self, master, container_button)
         
+class PageDivers(tk.Frame):
+    '''PAGE 5 'Analyse des corpus'.
+    '''
+    def __init__(self, container_frame, master, container_button, institute, ctg_path):
+        # Local imports
+        from CTG_Utils.CTG_GUI.PageDivers import create_divers_analysis
+        
+        super().__init__(container_frame)
+
+        page_name  = self.__class__.__name__
+        
+        create_divers_analysis(self, master, page_name, institute, ctg_path)
+        
+        setcontrollerbutton = SetControllerButton(master, container_button,page_name)
+        
+        settitleclass = SetTitltleClass(self,page_name,institute)
+        
+        quitapp = QuitApp(self, master, container_button)
+        
+        
 class SetControllerButton(tk.Tk):
 
     def __init__(self, master, container_button,page_name):
         # Standard library imports
         from tkinter import font as tkFont
     
         # Local imports
@@ -609,13 +644,13 @@
                                 command = lambda: self._launch_exit(master)).place(x = exit_button_x_pos_px, 
                                                                                        y = exit_button_y_pos_px,
                                                                                        anchor = 'n')                                                                                              
  
         
     def _launch_exit(self,controller):
         from tkinter import messagebox
-        message =  "Vous allez fermer BiblioMeter. "
+        message =  "Vous allez fermer CTG_Meter. "
         message += "\nRien ne sera perdu et vous pourrez reprendre le traitement plus tard."
         message += "\n\nSouhaitez-vous faire une pause dans le traitement ?"
         answer_1 = messagebox.askokcancel('Information', message)
         if answer_1:
             controller.destroy()
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/Useful_Classes.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Useful_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/CTG_Utils/CTG_GUI/Useful_Functions.py` & `CTG_Utils-1.1.0/CTG_Utils/CTG_GUI/Useful_Functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 __all__ = ['encadre_RL', 
            'encadre_UD', 
            'font_size',
-           'general_properties',
            'get_available_sorties',
            'last_available_years',
            'mm_to_px',
            'place_after', 
            'place_bellow', 
            'place_bellow_LabelEntry',
            'str_size_mm',
            'show_frame',
-           'create_archi'
+           'create_archi',
+           'window_properties'
           ]
 
 def show_frame(self, page_name):        
     '''Show a frame for the given page name'''
     frame = self.frames[page_name]
     frame.tkraise()
     
@@ -154,15 +154,15 @@
     from CTG_Utils.CTG_GUI.GUI_Globals import IN_TO_MM
 
     size_px = math.ceil((size_mm * fact / IN_TO_MM) * ppi)
     
     return size_px
 
 
-def _window_properties(screen_width_px, screen_height_px):
+def window_properties(screen_width_px, screen_height_px):
     # Local imports
     import CTG_Utils.CTG_GUI.GUI_Globals as gg
     from CTG_Utils.CTG_GUI.Useful_Functions import mm_to_px
     
     # Getting number of pixels per inch screen resolution from imported global DISPLAYS
     ppi = gg.DISPLAYS[gg.BM_GUI_DISP]["ppi"]
     
@@ -194,55 +194,14 @@
     
     sizes_tuple = (win_width_px, win_height_px, 
                    scale_factor_width_px, scale_factor_height_px, 
                    scale_factor_width_mm, scale_factor_height_mm)
     
     return sizes_tuple
 
-def general_properties(self):
-    '''The function `general_properties` calculate the window sizes 
-    and useful scale factors for the application launch window.
-    For that, it uses reference values for the display sizes in pixels
-    and mm through the globals:
-    - "REF_SCREEN_WIDTH_PX" and "REF_SCREEN_HEIGHT_PX";
-    - "REF_SCREEN_WIDTH_MM" and "REF_SCREEN_HEIGHT_MM".
-    The secondary window sizes in mm are set through the globals: 
-    - "REF_WINDOW_WIDTH_MM" and "REF_WINDOW_HEIGHT_MM".
-    The window title is set through the global "APPLICATION_TITLE".
-    These globals are defined locally in the module "GUI_Globals.py" 
-    of the package "BiblioMeter_GUI".
-    
-    Args:
-        None.
-        
-    Returns:
-        (tuple): self, 2 window sizes in pixels, 2 scale factors for sizes in mm 
-                 and 2 scale factors for sizes in pixels.
-    '''
-    # Local imports
-    import CTG_Utils.CTG_GUI.GUI_Globals as gg
-    
-    # Getting screen effective sizes in pixels for window "root" (not woring for Darwin platform)
-    screen_width_px  = self.winfo_screenwidth()
-    screen_height_px = self.winfo_screenheight()
-    
-    sizes_tuple = _window_properties(screen_width_px, screen_height_px)
-    
-    win_width_px  = sizes_tuple[0]
-    win_height_px = sizes_tuple[1]
-    
-    # Setting window size depending on scale factor
-    self.geometry(f"{win_width_px}x{win_height_px}")
-    self.resizable(False, False)    
-    
-    # Setting title window
-    self.title(gg.APPLICATION_WINDOW_TITLE)
-        
-    return sizes_tuple
-
 def create_folder(root_path, folder, verbose = False):
     # Standard library imports
     import os
     from pathlib import Path
     
     folder_path = root_path / Path(folder)
     if not os.path.exists(folder_path):
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils.egg-info/PKG-INFO` & `CTG_Utils-1.1.0/CTG_Utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG-Utils
-Version: 1.0.0
+Version: 1.1.0
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.0.0/CTG_Utils.egg-info/SOURCES.txt` & `CTG_Utils-1.1.0/CTG_Utils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
 CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
 CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
 CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
 CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
 CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
 CTG_Utils/CTG_GUI/GUI_Globals.py
+CTG_Utils/CTG_GUI/PageDivers.py
 CTG_Utils/CTG_GUI/PageEffectif.py
 CTG_Utils/CTG_GUI/PageSorties.py
 CTG_Utils/CTG_GUI/PageSynthese.py
 CTG_Utils/CTG_GUI/PageTendance.py
 CTG_Utils/CTG_GUI/Page_Classes.py
 CTG_Utils/CTG_GUI/Useful_Classes.py
 CTG_Utils/CTG_GUI/Useful_Functions.py
```

### Comparing `CTG_Utils-1.0.0/LICENSE` & `CTG_Utils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.0.0/PKG-INFO` & `CTG_Utils-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG_Utils
-Version: 1.0.0
+Version: 1.1.0
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.0.0/setup.py` & `CTG_Utils-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = f.read()
 
 install_requires = open(path.join(this_directory, 'requirements.txt'), encoding='utf-8').read().strip().split('\n') 
 
 # This setup is suitable for "python setup.py develop".
 
 setup(name='CTG_Utils',
-      version='1.0.0',
+      version='1.1.0',
       description='A toolbox for ctg statistics analysis',
       long_description=long_description,
       long_description_content_type='text/markdown',
       include_package_data = True,
       license = 'MIT',
       classifiers = [
         'Development Status :: 4 - Beta',
```

