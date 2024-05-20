# Comparing `tmp/PySDDP-0.0.8.tar.gz` & `tmp/PySDDP-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PySDDP-0.0.8.tar", last modified: Sun May 24 23:23:26 2020, max compression
+gzip compressed data, was "dist/PySDDP-0.0.9.tar", last modified: Wed May 27 02:47:14 2020, max compression
```

## Comparing `PySDDP-0.0.8.tar` & `PySDDP-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-24 23:23:26.000000 PySDDP-0.0.8/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-24 23:23:26.000000 PySDDP-0.0.8/PySDDP.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      393 2020-05-24 23:23:26.000000 PySDDP-0.0.8/PySDDP.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2020-05-24 23:23:26.000000 PySDDP-0.0.8/PySDDP.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1574 2020-05-24 23:23:26.000000 PySDDP-0.0.8/PySDDP.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2020-05-24 23:23:26.000000 PySDDP-0.0.8/PySDDP.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-05-24 23:23:26.000000 PySDDP-0.0.8/PySDDP.egg-info/dependency_links.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-24 23:23:26.000000 PySDDP-0.0.8/PySDDP/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7224 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/resequiv.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/dadosgerais.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    50851 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/hidr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    40243 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/pmo.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    54459 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/PowerSystem.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/mixins.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      142 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/planerg.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8503 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/submercado.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/term.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1166 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/fcf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      429 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/interc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-05-24 23:23:16.000000 PySDDP-0.0.8/PySDDP/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1842 2020-05-24 23:23:16.000000 PySDDP-0.0.8/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-05-24 23:23:16.000000 PySDDP-0.0.8/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2020-05-24 23:23:16.000000 PySDDP-0.0.8/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1574 2020-05-24 23:23:26.000000 PySDDP-0.0.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2020-05-24 23:23:26.000000 PySDDP-0.0.8/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-27 02:47:14.000000 PySDDP-0.0.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1842 2020-05-27 02:47:03.000000 PySDDP-0.0.9/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-27 02:47:14.000000 PySDDP-0.0.9/PySDDP/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1166 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/fcf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    40243 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/pmo.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      528 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/dadosgerais.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      478 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    55133 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/PowerSystem.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      273 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/planerg.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7224 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/resequiv.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    50851 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/hidr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/term.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8503 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/submercado.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      429 2020-05-27 02:47:03.000000 PySDDP-0.0.9/PySDDP/interc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2020-05-27 02:47:14.000000 PySDDP-0.0.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1574 2020-05-27 02:47:14.000000 PySDDP-0.0.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-05-27 02:47:03.000000 PySDDP-0.0.9/MANIFEST.in
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-27 02:47:14.000000 PySDDP-0.0.9/PySDDP.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2020-05-27 02:47:14.000000 PySDDP-0.0.9/PySDDP.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1574 2020-05-27 02:47:14.000000 PySDDP-0.0.9/PySDDP.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-05-27 02:47:14.000000 PySDDP-0.0.9/PySDDP.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      393 2020-05-27 02:47:14.000000 PySDDP-0.0.9/PySDDP.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2020-05-27 02:47:14.000000 PySDDP-0.0.9/PySDDP.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2020-05-27 02:47:03.000000 PySDDP-0.0.9/README.rst
```

### Comparing `PySDDP-0.0.8/PySDDP.egg-info/PKG-INFO` & `PySDDP-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySDDP
-Version: 0.0.8
+Version: 0.0.9
 Summary: PySDDP package
 Home-page: https://github.com/AndreMarcato/PySDDP
 Author: Andre Marcato
 Author-email: andre.marcato@ufjf.edu.br
 License: MIT
 Description: PySDDP
         ###################
```

### Comparing `PySDDP-0.0.8/PySDDP/resequiv.py` & `PySDDP-0.0.9/PySDDP/resequiv.py`

 * *Files identical despite different names*

### Comparing `PySDDP-0.0.8/PySDDP/dadosgerais.py` & `PySDDP-0.0.9/PySDDP/dadosgerais.py`

 * *Files identical despite different names*

### Comparing `PySDDP-0.0.8/PySDDP/hidr.py` & `PySDDP-0.0.9/PySDDP/hidr.py`

 * *Files identical despite different names*

### Comparing `PySDDP-0.0.8/PySDDP/pmo.py` & `PySDDP-0.0.9/PySDDP/pmo.py`

 * *Files identical despite different names*

### Comparing `PySDDP-0.0.8/PySDDP/PowerSystem.py` & `PySDDP-0.0.9/PySDDP/PowerSystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # coding=utf-8
 
 import os
+
+import cvxopt
 import numpy as np
 from matplotlib import pyplot as plt
 from cvxopt.modeling import variable, solvers, op, matrix
 from PySDDP.pmo import pmo
 from PySDDP.dadosgerais import dadosgerais
 from PySDDP.fcf import fcf
 from itertools import product, tee
 import time
 from timeit import default_timer as timer
 from functools import partial
 from multiprocessing import Pool
 from matplotlib import cm
 
 
-class importa_pmo(object):
+class ImportaPmo(object):
     # Classe contendo informacoes sobre os arquivos de entrada e saida
     caso = None
     dger = None
     npmc = 1
 
     # Define listas
     cadr_uh = []  # Lista com usinas hidraulicas do cadastro (HIDR.DAT)
@@ -602,101 +604,108 @@
         ax.set_ylabel('Energia Armazenada Maxima (MWmes)', fontsize=14)
         ax.legend(fontsize=12)
 
         plt.show()
 
 
 class Classroom(object):
-    lista_uhe = []
 
-    usina = {
-        "Nome": "UHE DO MARCATO",  # Nome da Usina
-        "Vmax": 100.,  # Volume Máximo em hm^3
-        "Vmin": 20.,  # Volume Mínimo em hm^3
-        "VI": 65.,
-        "Prod": 0.95,  # Produtibilidade em MWmed/hm^3
-        "Engol": 60.,  # Engolimento Máximo em hm^3
-        "Afl": [  # Cenários de Afluências (linha: Estágio, coluna: cenário)
-            [23, 16],
-            [19, 14],
-            [15, 11]
-        ]
-    }
-
-    lista_uhe.append(usina)
-
-    #
-    # Retirar os comentários abaixo para considerar 2 UHEs
-    #
-    # usina = {
-    #    "Nome": "UHE DO VASCAO",
-    #    "Vmax": 200.,
-    #    "Vmin": 40.,
-    #    "VI": 80,
-    #    "Prod": 0.85,
-    #    "Engol": 100.,
-    #    "Afl": [
-    #            [ 46, 32],
-    #            [ 38, 28],
-    #            [ 30, 22]
-    #    ]
-    # }
-    # lista_uhe.append(usina)
-
-    usina = {
-        "Nome": "GT_1",  # Nome da Usina Térmica 1
-        "Capac": 15.,  # Capacidade Máxima de Geração MWMed
-        "Custo": 10.  # Custo de Operação $/MWMed
-    }
-
-    lista_ute = []
-
-    lista_ute.append(usina)
-
-    usina = {
-        "Nome": "GT_2",  # Nome da Usina Térmica 2
-        "Capac": 10.,  # Capacidade Máxima de Geração MWmed
-        "Custo": 25.  # Custo de Operação $/MWMed
-    }
-
-    lista_ute.append(usina)
-
-    #
-    # d_gerais para o caso 1 UHE
-    #
-    d_gerais = {
-        "CDef": 500.,  # Custo de Déficit $/MWMed
-        "Carga": [50, 50., 50],  # Lista com carga a ser atendida por estágio
-        "Nr_Disc": 3,  # Número de Discretizações
-        "Nr_Est": 3,  # Número de Estágios
-        "Nr_Cen": 2  # Número de Cenários de Afluências
-    }
-
-    #
-    # d_gerais para o caso 2 UHE (Comentar o bloco acima e descomentar o bloco abaixo)
-    #
-    # d_gerais = {
-    #    "CDef": 500.,
-    #    "Carga": [ 100, 100., 100],
-    #    "Nr_Disc": 5,
-    #    "Nr_Est": 3,
-    #    "Nr_Cen": 2
-    # }
-
-    #
-    # Cria dicionário de dados com todas as informações do sistema em estudo
-    #
-    sistema = {
-        "DGer": d_gerais,
-        "UHE": lista_uhe,
-        "UTE": lista_ute
-    }
+    sistema = None
+
+    def __init__(self):
+        lista_uhe = []
+
+        usina = {
+            "Nome": "UHE DO MARCATO",  # Nome da Usina
+            "Vmax": 100.,  # Volume Máximo em hm^3
+            "Vmin": 20.,  # Volume Mínimo em hm^3
+            "VI": 65.,
+            "Prod": 0.95,  # Produtibilidade em MWmed/hm^3
+            "Engol": 60.,  # Engolimento Máximo em hm^3
+            "Afl": [  # Cenários de Afluências (linha: Estágio, coluna: cenário)
+                [23, 16],
+                [19, 14],
+                [15, 11]
+            ]
+        }
+
+        lista_uhe.append(usina)
+
+        #
+        # Retirar os comentários abaixo para considerar 2 UHEs
+        #
+        # usina = {
+        #    "Nome": "UHE DO VASCAO",
+        #    "Vmax": 200.,
+        #    "Vmin": 40.,
+        #    "VI": 80,
+        #    "Prod": 0.85,
+        #    "Engol": 100.,
+        #    "Afl": [
+        #            [ 46, 32],
+        #            [ 38, 28],
+        #            [ 30, 22]
+        #    ]
+        # }
+        # lista_uhe.append(usina)
+
+        usina = {
+            "Nome": "GT_1",  # Nome da Usina Térmica 1
+            "Capac": 15.,  # Capacidade Máxima de Geração MWMed
+            "Custo": 10.  # Custo de Operação $/MWMed
+        }
+
+        lista_ute = []
+
+        lista_ute.append(usina)
+
+        usina = {
+            "Nome": "GT_2",  # Nome da Usina Térmica 2
+            "Capac": 10.,  # Capacidade Máxima de Geração MWmed
+            "Custo": 25.  # Custo de Operação $/MWMed
+        }
+
+        lista_ute.append(usina)
+
+        #
+        # d_gerais para o caso 1 UHE
+        #
+        d_gerais = {
+            "CDef": 500.,  # Custo de Déficit $/MWMed
+            "Carga": [50, 50., 50],  # Lista com carga a ser atendida por estágio
+            "Nr_Disc": 3,  # Número de Discretizações
+            "Nr_Est": 3,  # Número de Estágios
+            "Nr_Cen": 2  # Número de Cenários de Afluências
+        }
+
+        #
+        # d_gerais para o caso 2 UHE (Comentar o bloco acima e descomentar o bloco abaixo)
+        #
+        # d_gerais = {
+        #    "CDef": 500.,
+        #    "Carga": [ 100, 100., 100],
+        #    "Nr_Disc": 5,
+        #    "Nr_Est": 3,
+        #    "Nr_Cen": 2
+        # }
+
+        #
+        # Cria dicionário de dados com todas as informações do sistema em estudo
+        #
+        self.sistema = {
+            "DGer": d_gerais,
+            "UHE": lista_uhe,
+            "UTE": lista_ute
+        }
 
     def despacho_pdd(self, VI, VF, AFL, custofuturo, iest, imprime):
 
+        solvers.options['show_progress'] = True
+        solvers.options['glpk'] = dict(msg_lev='GLP_MSG_OFF')
+
         Num_UHE = len(self.sistema["UHE"])
 
         Num_UTE = len(self.sistema["UTE"])
 
         #
         # Cria Variáveis de Decisão
         #
@@ -812,15 +821,15 @@
             "UTE": lista_ute
         }
 
         #
         # Imprime resultados em tela
         #
 
-        if imprime and (problema.status == 'optmal'):
+        if imprime and (problema.status == 'optimal'):
             print("Custo Total:", fob.value())
 
             for i, usi in enumerate(self.sistema["UHE"]):
                 print(vt.name, i, "é", vt[i].value(), "hm3")
                 print(vv.name, i, "é", vv[i].value(), "hm3")
 
             for i, usi in enumerate(self.sistema["UTE"]):
@@ -915,15 +924,15 @@
                     for folha in arvore:
                         if (folha["VI"] == VF) and (folha["Est"] == iest):
                             CustoFuturo = folha["Dger"]["CustoTotal"]
 
                     #
                     # Chama função de despacho hidrotérmico
                     #
-                    resultado = self.despacho_pdd(VI, VF, AFL, CustoFuturo, iest - 1, imprime=False)
+                    resultado = self.despacho_pdd(VI, VF, AFL, CustoFuturo, iest - 1, imprime)
                     todos.append([iest - 1, VI, VF, resultado])
                     if (resultado["DGer"]["CustoTotal"] < menor):
                         menor = resultado["DGer"]["CustoTotal"]
                         posicao_menor = posicao
                     posicao += 1
                 melhor = {
                     "Est": todos[posicao_menor][0],
@@ -1044,14 +1053,17 @@
             "UTE": lista_ute
         }
 
         return resultado
 
     def pl_unico(self, cenario, imprime):
 
+        solvers.options['show_progress'] = True
+        solvers.options['glpk'] = dict(msg_lev='GLP_MSG_OFF')
+
         #
         # Cria função de despacho hidrotérmico
         #
 
         Num_UHE = len(self.sistema["UHE"])
 
         Num_UTE = len(self.sistema["UTE"])
@@ -1236,14 +1248,17 @@
 
             print("----- x ------ ")
 
         return resultado
 
     def despacho_pddd(self, VI, AFL, pote_de_corte, iest, imprime):
 
+        solvers.options['show_progress'] = True
+        solvers.options['glpk'] = dict(msg_lev='GLP_MSG_OFF')
+
         Num_UHE = len(self.sistema["UHE"])
 
         Num_UTE = len(self.sistema["UTE"])
 
         #
         # Cria Variáveis de Decisão
         #
@@ -1437,17 +1452,17 @@
                         VI.append(iusi["vf"])
                 AFL = []
                 for i, iusi in enumerate(self.sistema["UHE"]):
                     AFL.append(iusi["Afl"][iest][cenario])
                 #
                 # Chama função de despacho hidrotérmico
                 #
-                resultado = self.despacho_pddd(VI, AFL, pote_de_corte, iest + 1, imprime=False)
-                if iteracao == 1:
-                    print(iest, resultado)
+                resultado = self.despacho_pddd(VI, AFL, pote_de_corte, iest + 1, imprime)
+                #if iteracao == 1:
+                #    print(iest, resultado)
                 ZSUP[iteracao] += resultado["DGer"]["CustoTotal"] - resultado["DGer"]["CustoFuturo"]
                 if iest == 0:
                     ZINF[iteracao] = resultado["DGer"]["CustoTotal"]
                 memoria.append(resultado)
 
             if np.abs(ZSUP[iteracao] - ZINF[iteracao]) <= tol:
                 break
@@ -1467,15 +1482,15 @@
                         VI.append(iusi["vf"])
                 AFL = []
                 for i, iusi in enumerate(self.sistema["UHE"]):
                     AFL.append(iusi["Afl"][iest][cenario])
                 #
                 # Chama função de despacho hidrotérmico
                 #
-                resultado = self.despacho_pddd(VI, AFL, pote_de_corte, iest + 1, imprime=False)
+                resultado = self.despacho_pddd(VI, AFL, pote_de_corte, iest + 1, imprime)
                 term_indep = resultado["DGer"]["CustoTotal"]
                 coefs = []
                 for i, iusi in enumerate(resultado["UHE"]):
                     coefs.append(-iusi["cma"])
                     term_indep -= VI[i] * coefs[i]
                 #
                 # Calcula o corte (inequação) correspondente a uma discretização
```

### Comparing `PySDDP-0.0.8/PySDDP/submercado.py` & `PySDDP-0.0.9/PySDDP/submercado.py`

 * *Files identical despite different names*

### Comparing `PySDDP-0.0.8/PySDDP/term.py` & `PySDDP-0.0.9/PySDDP/term.py`

 * *Files identical despite different names*

### Comparing `PySDDP-0.0.8/PySDDP/fcf.py` & `PySDDP-0.0.9/PySDDP/fcf.py`

 * *Files identical despite different names*

### Comparing `PySDDP-0.0.8/setup.py` & `PySDDP-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from setuptools import setup
 from setuptools.command.install import install
 
 # current version
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 
 def readme():
     """print long description"""
     with open('README.rst') as f:
         return f.read()
```

### Comparing `PySDDP-0.0.8/README.rst` & `PySDDP-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `PySDDP-0.0.8/PKG-INFO` & `PySDDP-0.0.9/PySDDP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySDDP
-Version: 0.0.8
+Version: 0.0.9
 Summary: PySDDP package
 Home-page: https://github.com/AndreMarcato/PySDDP
 Author: Andre Marcato
 Author-email: andre.marcato@ufjf.edu.br
 License: MIT
 Description: PySDDP
         ###################
```

