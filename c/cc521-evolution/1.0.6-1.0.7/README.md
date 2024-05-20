# Comparing `tmp/cc521_evolution-1.0.6.tar.gz` & `tmp/cc521_evolution-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc521_evolution-1.0.6.tar", max compression
+gzip compressed data, was "cc521_evolution-1.0.7.tar", max compression
```

## Comparing `cc521_evolution-1.0.6.tar` & `cc521_evolution-1.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0        0 2024-04-20 16:48:16.722884 cc521_evolution-1.0.6/README.md
--rw-r--r--   0        0        0      435 2024-05-20 02:27:32.119768 cc521_evolution-1.0.6/pyproject.toml
--rw-r--r--   0        0        0       80 2024-05-01 15:27:09.336087 cc521_evolution-1.0.6/src/evolution/__init__.py
--rw-r--r--   0        0        0      354 2024-05-01 10:53:16.697215 cc521_evolution-1.0.6/src/evolution/encoding/__init__.py
--rw-r--r--   0        0        0     3161 2024-05-20 02:07:24.049320 cc521_evolution-1.0.6/src/evolution/encoding/base.py
--rw-r--r--   0        0        0     2723 2024-05-20 02:14:33.021360 cc521_evolution-1.0.6/src/evolution/encoding/binary.py
--rw-r--r--   0        0        0     2034 2024-05-01 12:32:18.671279 cc521_evolution-1.0.6/src/evolution/encoding/gray.py
--rw-r--r--   0        0        0     1506 2024-04-20 12:41:59.068191 cc521_evolution-1.0.6/src/evolution/encoding/gray_code.py
--rw-r--r--   0        0        0     4266 2024-05-20 02:16:56.378323 cc521_evolution-1.0.6/src/evolution/encoding/interval.py
--rw-r--r--   0        0        0     9010 2024-05-20 02:27:09.999104 cc521_evolution-1.0.6/src/evolution/evolution.py
--rw-r--r--   0        0        0      498 2024-05-15 12:10:21.455530 cc521_evolution-1.0.6/src/evolution/fitness.py
--rw-r--r--   0        0        0        0 2024-05-15 15:40:53.771300 cc521_evolution-1.0.6/src/evolution/history/__init__.py
--rw-r--r--   0        0        0      647 2024-05-15 15:51:00.283651 cc521_evolution-1.0.6/src/evolution/history/base.py
--rw-r--r--   0        0        0      683 2024-05-15 12:32:31.896803 cc521_evolution-1.0.6/src/evolution/individual.py
--rw-r--r--   0        0        0       69 2024-05-15 12:25:02.449380 cc521_evolution-1.0.6/src/evolution/metrics/__init__.py
--rw-r--r--   0        0        0      270 2024-05-15 12:08:33.983499 cc521_evolution-1.0.6/src/evolution/metrics/base.py
--rw-r--r--   0        0        0     1145 2024-05-15 12:36:13.235607 cc521_evolution-1.0.6/src/evolution/metrics/fitness.py
--rw-r--r--   0        0        0     1363 2024-05-15 14:23:53.737905 cc521_evolution-1.0.6/src/evolution/population.py
--rw-r--r--   0        0        0      179 2024-05-01 23:44:32.151131 cc521_evolution-1.0.6/src/evolution/selection/__init__.py
--rw-r--r--   0        0        0      487 2024-05-01 15:28:52.057254 cc521_evolution-1.0.6/src/evolution/selection/base.py
--rw-r--r--   0        0        0       53 2024-05-15 12:10:14.122058 cc521_evolution-1.0.6/src/evolution/selection/misc.py
--rw-r--r--   0        0        0      762 2024-05-01 19:07:59.046499 cc521_evolution-1.0.6/src/evolution/selection/proportional2fitness.py
--rw-r--r--   0        0        0      802 2024-05-01 23:43:39.304984 cc521_evolution-1.0.6/src/evolution/selection/proportional2inversefitness.py
--rw-r--r--   0        0        0     1657 2024-04-28 06:27:18.505872 cc521_evolution-1.0.6/src/evolution/selection/rank_based_exponential_classification.py
--rw-r--r--   0        0        0     1547 2024-04-28 06:28:09.901230 cc521_evolution-1.0.6/src/evolution/selection/rank_based_linear_classification.py
--rw-r--r--   0        0        0     2011 2024-04-28 06:51:23.729483 cc521_evolution-1.0.6/src/evolution/selection/roulette.py
--rw-r--r--   0        0        0     2409 2024-04-28 06:45:40.145945 cc521_evolution-1.0.6/src/evolution/selection/tournament.py
--rw-r--r--   0        0        0      862 2024-04-28 06:49:12.924329 cc521_evolution-1.0.6/src/evolution/selection/uniform.py
--rw-r--r--   0        0        0        0 2024-05-01 14:45:46.565897 cc521_evolution-1.0.6/src/evolution/variation/__init__.py
--rw-r--r--   0        0        0      159 2024-05-01 14:47:11.100554 cc521_evolution-1.0.6/src/evolution/variation/crossover/__init__.py
--rw-r--r--   0        0        0      313 2024-05-19 11:27:55.394824 cc521_evolution-1.0.6/src/evolution/variation/crossover/base.py
--rw-r--r--   0        0        0     1478 2024-05-01 19:59:49.362851 cc521_evolution-1.0.6/src/evolution/variation/crossover/bit.py
--rw-r--r--   0        0        0      553 2024-04-20 13:27:30.081869 cc521_evolution-1.0.6/src/evolution/variation/crossover/cross_gen.py
--rw-r--r--   0        0        0      157 2024-05-01 14:49:17.034398 cc521_evolution-1.0.6/src/evolution/variation/mutation/__init__.py
--rw-r--r--   0        0        0      538 2024-05-15 12:33:08.896494 cc521_evolution-1.0.6/src/evolution/variation/mutation/base.py
--rw-r--r--   0        0        0      895 2024-05-15 11:51:29.633436 cc521_evolution-1.0.6/src/evolution/variation/mutation/bit.py
--rw-r--r--   0        0        0     1165 2024-05-15 13:58:00.293361 cc521_evolution-1.0.6/src/evolution/variation/probability.py
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 cc521_evolution-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 16:48:16.722884 cc521_evolution-1.0.7/README.md
+-rw-r--r--   0        0        0      435 2024-05-20 02:45:18.199954 cc521_evolution-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-05-01 15:27:09.336087 cc521_evolution-1.0.7/src/evolution/__init__.py
+-rw-r--r--   0        0        0      354 2024-05-01 10:53:16.697215 cc521_evolution-1.0.7/src/evolution/encoding/__init__.py
+-rw-r--r--   0        0        0     3161 2024-05-20 02:07:24.049320 cc521_evolution-1.0.7/src/evolution/encoding/base.py
+-rw-r--r--   0        0        0     2723 2024-05-20 02:14:33.021360 cc521_evolution-1.0.7/src/evolution/encoding/binary.py
+-rw-r--r--   0        0        0     2034 2024-05-01 12:32:18.671279 cc521_evolution-1.0.7/src/evolution/encoding/gray.py
+-rw-r--r--   0        0        0     1506 2024-04-20 12:41:59.068191 cc521_evolution-1.0.7/src/evolution/encoding/gray_code.py
+-rw-r--r--   0        0        0     4266 2024-05-20 02:16:56.378323 cc521_evolution-1.0.7/src/evolution/encoding/interval.py
+-rw-r--r--   0        0        0     9010 2024-05-20 02:27:09.999104 cc521_evolution-1.0.7/src/evolution/evolution.py
+-rw-r--r--   0        0        0      498 2024-05-15 12:10:21.455530 cc521_evolution-1.0.7/src/evolution/fitness.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:40:53.771300 cc521_evolution-1.0.7/src/evolution/history/__init__.py
+-rw-r--r--   0        0        0      647 2024-05-15 15:51:00.283651 cc521_evolution-1.0.7/src/evolution/history/base.py
+-rw-r--r--   0        0        0      683 2024-05-15 12:32:31.896803 cc521_evolution-1.0.7/src/evolution/individual.py
+-rw-r--r--   0        0        0       69 2024-05-15 12:25:02.449380 cc521_evolution-1.0.7/src/evolution/metrics/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-15 12:08:33.983499 cc521_evolution-1.0.7/src/evolution/metrics/base.py
+-rw-r--r--   0        0        0     1145 2024-05-15 12:36:13.235607 cc521_evolution-1.0.7/src/evolution/metrics/fitness.py
+-rw-r--r--   0        0        0     1438 2024-05-20 02:45:37.065432 cc521_evolution-1.0.7/src/evolution/population.py
+-rw-r--r--   0        0        0      179 2024-05-01 23:44:32.151131 cc521_evolution-1.0.7/src/evolution/selection/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-01 15:28:52.057254 cc521_evolution-1.0.7/src/evolution/selection/base.py
+-rw-r--r--   0        0        0       53 2024-05-15 12:10:14.122058 cc521_evolution-1.0.7/src/evolution/selection/misc.py
+-rw-r--r--   0        0        0      762 2024-05-01 19:07:59.046499 cc521_evolution-1.0.7/src/evolution/selection/proportional2fitness.py
+-rw-r--r--   0        0        0      802 2024-05-01 23:43:39.304984 cc521_evolution-1.0.7/src/evolution/selection/proportional2inversefitness.py
+-rw-r--r--   0        0        0     1657 2024-04-28 06:27:18.505872 cc521_evolution-1.0.7/src/evolution/selection/rank_based_exponential_classification.py
+-rw-r--r--   0        0        0     1547 2024-04-28 06:28:09.901230 cc521_evolution-1.0.7/src/evolution/selection/rank_based_linear_classification.py
+-rw-r--r--   0        0        0     2011 2024-04-28 06:51:23.729483 cc521_evolution-1.0.7/src/evolution/selection/roulette.py
+-rw-r--r--   0        0        0     2409 2024-04-28 06:45:40.145945 cc521_evolution-1.0.7/src/evolution/selection/tournament.py
+-rw-r--r--   0        0        0      862 2024-04-28 06:49:12.924329 cc521_evolution-1.0.7/src/evolution/selection/uniform.py
+-rw-r--r--   0        0        0        0 2024-05-01 14:45:46.565897 cc521_evolution-1.0.7/src/evolution/variation/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-01 14:47:11.100554 cc521_evolution-1.0.7/src/evolution/variation/crossover/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-19 11:27:55.394824 cc521_evolution-1.0.7/src/evolution/variation/crossover/base.py
+-rw-r--r--   0        0        0     1478 2024-05-01 19:59:49.362851 cc521_evolution-1.0.7/src/evolution/variation/crossover/bit.py
+-rw-r--r--   0        0        0      553 2024-04-20 13:27:30.081869 cc521_evolution-1.0.7/src/evolution/variation/crossover/cross_gen.py
+-rw-r--r--   0        0        0      157 2024-05-01 14:49:17.034398 cc521_evolution-1.0.7/src/evolution/variation/mutation/__init__.py
+-rw-r--r--   0        0        0      538 2024-05-15 12:33:08.896494 cc521_evolution-1.0.7/src/evolution/variation/mutation/base.py
+-rw-r--r--   0        0        0      895 2024-05-15 11:51:29.633436 cc521_evolution-1.0.7/src/evolution/variation/mutation/bit.py
+-rw-r--r--   0        0        0     1165 2024-05-15 13:58:00.293361 cc521_evolution-1.0.7/src/evolution/variation/probability.py
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 cc521_evolution-1.0.7/PKG-INFO
```

### Comparing `cc521_evolution-1.0.6/src/evolution/encoding/base.py` & `cc521_evolution-1.0.7/src/evolution/encoding/base.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/encoding/binary.py` & `cc521_evolution-1.0.7/src/evolution/encoding/binary.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/encoding/gray.py` & `cc521_evolution-1.0.7/src/evolution/encoding/gray.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/encoding/gray_code.py` & `cc521_evolution-1.0.7/src/evolution/encoding/gray_code.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/encoding/interval.py` & `cc521_evolution-1.0.7/src/evolution/encoding/interval.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/evolution.py` & `cc521_evolution-1.0.7/src/evolution/evolution.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/history/base.py` & `cc521_evolution-1.0.7/src/evolution/history/base.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/individual.py` & `cc521_evolution-1.0.7/src/evolution/individual.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/metrics/fitness.py` & `cc521_evolution-1.0.7/src/evolution/metrics/fitness.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/population.py` & `cc521_evolution-1.0.7/src/evolution/population.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #!/usr/bin/env python3
 #
 # Population class - Just a group of individuals generated by an specific domain encoder
 
-from typing import List
+from typing import List, Type
 from abc import ABC, abstractmethod
 from .individual import Individual
 from .encoding.base import DomainEncoder
 
 class Population:
     """Just a group of individuals"""
     # initial_individuals attribute is added to support micro-AG evolution schema (transfer best individuals from a micro-AG to other AG to continue the evolution)
-    def __init__(self, domain_encoder: DomainEncoder, population: int = 10, initial_individuals: List[Individual] = None):
+    def __init__(self, domain_encoder: DomainEncoder, population: int = 10, 
+                 individual_cls: Type[Individual] = Individual, initial_individuals: List[Individual] = None):
         """
         IMPORTANT: If initial_individuals field is passed, them must have the same domain encoder with which is being creating this population"""
 
         n = population # random individuals to be created
         initial_individuals = [] if initial_individuals is None else initial_individuals
         if (init:=len(initial_individuals)) > n:
             self.individuals = initial_individuals[:population]
         else:
             n -= init
             self.individuals = initial_individuals + \
-                [Individual(domain_encoder.random(), domain_encoder) for _ in range(n)]
+                [individual_cls(domain_encoder.random(), domain_encoder) for _ in range(n)]
 
     @property
     def size(self):
         return len(self.individuals)
 
     def __iter__(self):
         for individual in self.individuals:
```

### Comparing `cc521_evolution-1.0.6/src/evolution/selection/proportional2fitness.py` & `cc521_evolution-1.0.7/src/evolution/selection/proportional2fitness.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/selection/proportional2inversefitness.py` & `cc521_evolution-1.0.7/src/evolution/selection/proportional2inversefitness.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/selection/rank_based_exponential_classification.py` & `cc521_evolution-1.0.7/src/evolution/selection/rank_based_exponential_classification.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/selection/rank_based_linear_classification.py` & `cc521_evolution-1.0.7/src/evolution/selection/rank_based_linear_classification.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/selection/roulette.py` & `cc521_evolution-1.0.7/src/evolution/selection/roulette.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/selection/tournament.py` & `cc521_evolution-1.0.7/src/evolution/selection/tournament.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/selection/uniform.py` & `cc521_evolution-1.0.7/src/evolution/selection/uniform.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/variation/crossover/bit.py` & `cc521_evolution-1.0.7/src/evolution/variation/crossover/bit.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/variation/crossover/cross_gen.py` & `cc521_evolution-1.0.7/src/evolution/variation/crossover/cross_gen.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/variation/mutation/base.py` & `cc521_evolution-1.0.7/src/evolution/variation/mutation/base.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/variation/mutation/bit.py` & `cc521_evolution-1.0.7/src/evolution/variation/mutation/bit.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/src/evolution/variation/probability.py` & `cc521_evolution-1.0.7/src/evolution/variation/probability.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.6/PKG-INFO` & `cc521_evolution-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc521-evolution
-Version: 1.0.6
+Version: 1.0.7
 Summary: Collection of utilities to develop evolutionary algorithms
 Author: Gustavo Lozano
 Author-email: glozanoac@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

