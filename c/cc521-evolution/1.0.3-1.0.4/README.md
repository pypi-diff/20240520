# Comparing `tmp/cc521_evolution-1.0.3.tar.gz` & `tmp/cc521_evolution-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc521_evolution-1.0.3.tar", max compression
+gzip compressed data, was "cc521_evolution-1.0.4.tar", max compression
```

## Comparing `cc521_evolution-1.0.3.tar` & `cc521_evolution-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,38 @@
--rw-r--r--   0        0        0        0 2024-04-20 16:48:16.722884 cc521_evolution-1.0.3/README.md
--rw-r--r--   0        0        0      413 2024-05-02 02:37:56.454345 cc521_evolution-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       80 2024-05-01 15:27:09.336087 cc521_evolution-1.0.3/src/evolution/__init__.py
--rw-r--r--   0        0        0      354 2024-05-01 10:53:16.697215 cc521_evolution-1.0.3/src/evolution/encoding/__init__.py
--rw-r--r--   0        0        0     2775 2024-05-01 19:22:53.755082 cc521_evolution-1.0.3/src/evolution/encoding/base.py
--rw-r--r--   0        0        0     2421 2024-05-01 17:43:12.613572 cc521_evolution-1.0.3/src/evolution/encoding/binary.py
--rw-r--r--   0        0        0     2034 2024-05-01 12:32:18.671279 cc521_evolution-1.0.3/src/evolution/encoding/gray.py
--rw-r--r--   0        0        0     1506 2024-04-20 12:41:59.068191 cc521_evolution-1.0.3/src/evolution/encoding/gray_code.py
--rw-r--r--   0        0        0     4772 2024-05-01 19:04:10.318473 cc521_evolution-1.0.3/src/evolution/encoding/interval.py
--rw-r--r--   0        0        0     7873 2024-05-02 02:37:25.880839 cc521_evolution-1.0.3/src/evolution/evolution.py
--rw-r--r--   0        0        0      382 2024-04-28 05:36:30.660588 cc521_evolution-1.0.3/src/evolution/fitness.py
--rw-r--r--   0        0        0     1091 2024-05-01 20:01:00.912595 cc521_evolution-1.0.3/src/evolution/population.py
--rw-r--r--   0        0        0      179 2024-05-01 23:44:32.151131 cc521_evolution-1.0.3/src/evolution/selection/__init__.py
--rw-r--r--   0        0        0      487 2024-05-01 15:28:52.057254 cc521_evolution-1.0.3/src/evolution/selection/base.py
--rw-r--r--   0        0        0      168 2024-05-01 20:27:18.061307 cc521_evolution-1.0.3/src/evolution/selection/misc.py
--rw-r--r--   0        0        0      762 2024-05-01 19:07:59.046499 cc521_evolution-1.0.3/src/evolution/selection/proportional2fitness.py
--rw-r--r--   0        0        0      802 2024-05-01 23:43:39.304984 cc521_evolution-1.0.3/src/evolution/selection/proportional2inversefitness.py
--rw-r--r--   0        0        0     1657 2024-04-28 06:27:18.505872 cc521_evolution-1.0.3/src/evolution/selection/rank_based_exponential_classification.py
--rw-r--r--   0        0        0     1547 2024-04-28 06:28:09.901230 cc521_evolution-1.0.3/src/evolution/selection/rank_based_linear_classification.py
--rw-r--r--   0        0        0     2011 2024-04-28 06:51:23.729483 cc521_evolution-1.0.3/src/evolution/selection/roulette.py
--rw-r--r--   0        0        0     2409 2024-04-28 06:45:40.145945 cc521_evolution-1.0.3/src/evolution/selection/tournament.py
--rw-r--r--   0        0        0      862 2024-04-28 06:49:12.924329 cc521_evolution-1.0.3/src/evolution/selection/uniform.py
--rw-r--r--   0        0        0        0 2024-05-01 14:45:46.565897 cc521_evolution-1.0.3/src/evolution/variation/__init__.py
--rw-r--r--   0        0        0      159 2024-05-01 14:47:11.100554 cc521_evolution-1.0.3/src/evolution/variation/crossover/__init__.py
--rw-r--r--   0        0        0      315 2024-05-01 17:07:45.009487 cc521_evolution-1.0.3/src/evolution/variation/crossover/base.py
--rw-r--r--   0        0        0     1478 2024-05-01 19:59:49.362851 cc521_evolution-1.0.3/src/evolution/variation/crossover/bit.py
--rw-r--r--   0        0        0      553 2024-04-20 13:27:30.081869 cc521_evolution-1.0.3/src/evolution/variation/crossover/cross_gen.py
--rw-r--r--   0        0        0      157 2024-05-01 14:49:17.034398 cc521_evolution-1.0.3/src/evolution/variation/mutation/__init__.py
--rw-r--r--   0        0        0      255 2024-05-01 15:33:04.707998 cc521_evolution-1.0.3/src/evolution/variation/mutation/base.py
--rw-r--r--   0        0        0      864 2024-05-01 19:54:38.030414 cc521_evolution-1.0.3/src/evolution/variation/mutation/bit.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 cc521_evolution-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 16:48:16.722884 cc521_evolution-1.0.4/README.md
+-rw-r--r--   0        0        0      435 2024-05-19 11:31:10.598555 cc521_evolution-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-05-01 15:27:09.336087 cc521_evolution-1.0.4/src/evolution/__init__.py
+-rw-r--r--   0        0        0      354 2024-05-01 10:53:16.697215 cc521_evolution-1.0.4/src/evolution/encoding/__init__.py
+-rw-r--r--   0        0        0     3175 2024-05-19 11:08:43.520350 cc521_evolution-1.0.4/src/evolution/encoding/base.py
+-rw-r--r--   0        0        0     2421 2024-05-01 17:43:12.613572 cc521_evolution-1.0.4/src/evolution/encoding/binary.py
+-rw-r--r--   0        0        0     2034 2024-05-01 12:32:18.671279 cc521_evolution-1.0.4/src/evolution/encoding/gray.py
+-rw-r--r--   0        0        0     1506 2024-04-20 12:41:59.068191 cc521_evolution-1.0.4/src/evolution/encoding/gray_code.py
+-rw-r--r--   0        0        0     4772 2024-05-01 19:04:10.318473 cc521_evolution-1.0.4/src/evolution/encoding/interval.py
+-rw-r--r--   0        0        0     8629 2024-05-15 15:39:00.396113 cc521_evolution-1.0.4/src/evolution/evolution.py
+-rw-r--r--   0        0        0      498 2024-05-15 12:10:21.455530 cc521_evolution-1.0.4/src/evolution/fitness.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:40:53.771300 cc521_evolution-1.0.4/src/evolution/history/__init__.py
+-rw-r--r--   0        0        0      647 2024-05-15 15:51:00.283651 cc521_evolution-1.0.4/src/evolution/history/base.py
+-rw-r--r--   0        0        0      683 2024-05-15 12:32:31.896803 cc521_evolution-1.0.4/src/evolution/individual.py
+-rw-r--r--   0        0        0       69 2024-05-15 12:25:02.449380 cc521_evolution-1.0.4/src/evolution/metrics/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-15 12:08:33.983499 cc521_evolution-1.0.4/src/evolution/metrics/base.py
+-rw-r--r--   0        0        0     1145 2024-05-15 12:36:13.235607 cc521_evolution-1.0.4/src/evolution/metrics/fitness.py
+-rw-r--r--   0        0        0     1363 2024-05-15 14:23:53.737905 cc521_evolution-1.0.4/src/evolution/population.py
+-rw-r--r--   0        0        0      179 2024-05-01 23:44:32.151131 cc521_evolution-1.0.4/src/evolution/selection/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-01 15:28:52.057254 cc521_evolution-1.0.4/src/evolution/selection/base.py
+-rw-r--r--   0        0        0       53 2024-05-15 12:10:14.122058 cc521_evolution-1.0.4/src/evolution/selection/misc.py
+-rw-r--r--   0        0        0      762 2024-05-01 19:07:59.046499 cc521_evolution-1.0.4/src/evolution/selection/proportional2fitness.py
+-rw-r--r--   0        0        0      802 2024-05-01 23:43:39.304984 cc521_evolution-1.0.4/src/evolution/selection/proportional2inversefitness.py
+-rw-r--r--   0        0        0     1657 2024-04-28 06:27:18.505872 cc521_evolution-1.0.4/src/evolution/selection/rank_based_exponential_classification.py
+-rw-r--r--   0        0        0     1547 2024-04-28 06:28:09.901230 cc521_evolution-1.0.4/src/evolution/selection/rank_based_linear_classification.py
+-rw-r--r--   0        0        0     2011 2024-04-28 06:51:23.729483 cc521_evolution-1.0.4/src/evolution/selection/roulette.py
+-rw-r--r--   0        0        0     2409 2024-04-28 06:45:40.145945 cc521_evolution-1.0.4/src/evolution/selection/tournament.py
+-rw-r--r--   0        0        0      862 2024-04-28 06:49:12.924329 cc521_evolution-1.0.4/src/evolution/selection/uniform.py
+-rw-r--r--   0        0        0        0 2024-05-01 14:45:46.565897 cc521_evolution-1.0.4/src/evolution/variation/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-01 14:47:11.100554 cc521_evolution-1.0.4/src/evolution/variation/crossover/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-19 11:27:55.394824 cc521_evolution-1.0.4/src/evolution/variation/crossover/base.py
+-rw-r--r--   0        0        0     1478 2024-05-01 19:59:49.362851 cc521_evolution-1.0.4/src/evolution/variation/crossover/bit.py
+-rw-r--r--   0        0        0      553 2024-04-20 13:27:30.081869 cc521_evolution-1.0.4/src/evolution/variation/crossover/cross_gen.py
+-rw-r--r--   0        0        0      157 2024-05-01 14:49:17.034398 cc521_evolution-1.0.4/src/evolution/variation/mutation/__init__.py
+-rw-r--r--   0        0        0      538 2024-05-15 12:33:08.896494 cc521_evolution-1.0.4/src/evolution/variation/mutation/base.py
+-rw-r--r--   0        0        0      895 2024-05-15 11:51:29.633436 cc521_evolution-1.0.4/src/evolution/variation/mutation/bit.py
+-rw-r--r--   0        0        0     1165 2024-05-15 13:58:00.293361 cc521_evolution-1.0.4/src/evolution/variation/probability.py
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 cc521_evolution-1.0.4/PKG-INFO
```

### Comparing `cc521_evolution-1.0.3/src/evolution/encoding/base.py` & `cc521_evolution-1.0.4/src/evolution/encoding/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     def decode(self, x: Gen) -> object:
         pass
 
     @abstractmethod
     def encode(self, x: object) -> Gen:
         pass
 
+    @abstractmethod
+    def random(self) -> Gen:
+        pass
+
 class ChromosomeComponent:
     def __init__(self, gen: Gen, encoder: GenEncoder):
         self.gen = gen
         self.encoder = encoder
 
 class Chromosome:
     def __init__(self, components: List[ChromosomeComponent]):
@@ -83,13 +87,19 @@
     def __init__(self, gen_encoders: List[GenEncoder]):
         self.gen_encoders = gen_encoders
 
     def decode(self, chromosome: Chromosome) -> object:
         return [self.decode_component(component) for component in chromosome.chromosome_components]
 
     def decode_component(self, component: ChromosomeComponent) -> object:
-        pass
+        encoder, gen = component.encoder, component.gen
+        return encoder.decode(gen)
 
-    @abstractmethod
     def random(self) -> Chromosome:
-        pass
+         """Generate a random chromosome"""
+        components = []
+        for gen_encoder in self.gen_encoders:
+            component = ChromosomeComponent(gen_encoder.random(), encoder=gen_encoder)
+            components.append(component)
+
+        return Chromosome(components=components)
```

### Comparing `cc521_evolution-1.0.3/src/evolution/encoding/binary.py` & `cc521_evolution-1.0.4/src/evolution/encoding/binary.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/encoding/gray.py` & `cc521_evolution-1.0.4/src/evolution/encoding/gray.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/encoding/gray_code.py` & `cc521_evolution-1.0.4/src/evolution/encoding/gray_code.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/encoding/interval.py` & `cc521_evolution-1.0.4/src/evolution/encoding/interval.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/evolution.py` & `cc521_evolution-1.0.4/src/evolution/evolution.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,184 +1,193 @@
 #!/usr/bin/env python3
 #
 # Base Generatic Evolutionary Algorithm Class
 from __future__ import annotations
 
-from tqdm import tqdm
 import uuid
 import random
 import logging
 import json
+import matplotlib.pyplot as plt
+from matplotlib.figure import Figure
+from tqdm import tqdm
 from abc import abstractmethod
 from typing import Callable, Concatenate, List
+from collections.abc import Iterable
 
+from .fitness import FitnessEvaluation
 from .population import Population, Individual
-from .selection.misc import FitnessEvaluation
 from .selection.base import SelectionStrategy
 from .variation.crossover.base import CrossoverStrategy
 from .variation.mutation.base import MutationStrategy
+from .variation.probability import VariationProbability, ConstantVariationProbability
+
+from .metrics import EvolutionMetric, FitnessMetric
+
 
 class Evolution:
     def __init__(self, population: Population, *,
                  fitness: Callable[[object], float],
                  selection_strategy: SelectionStrategy,
                  # variation strategies
-                 crossover_strategy: CrossoverStrategy, 
-                 mutation_strategy: MutationStrategy, 
-                 crossover_prob: float = 0.7, mutation_prob: float = 0.2):
+                 crossover_strategy: CrossoverStrategy,
+                 mutation_strategy: MutationStrategy,
+                 crossover_prob: Union[float, Iterable] , mutation_prob: Union[float, Iterable],
+                 metrics: dict[str, EvolutionMetric] = None):
         self.fitness_func = fitness
         self.population = population
-        self.generation = 1
+        self.generation: int = 1
 
         self.best: Individual = None # invidividual with the largest fitness value on the last generation
         self.worse: Individual = None # invidividual with the smallest fitness value on the last generation
 
         self.selection_strategy = selection_strategy
-
         self.crossover_strategy = crossover_strategy
+
+        # variation(crossover and mutation) probabilities
         self.crossover_prob = crossover_prob
+        if not isinstance(crossover_prob, Iterable):
+            self.crossover_prob = ConstantVariationProbability(value=crossover_prob)
 
         self.mutation_strategy = mutation_strategy
         self.mutation_prob = mutation_prob
+        if not isinstance(mutation_prob, Iterable):
+            self.mutation_prob = ConstantVariationProbability(value=mutation_prob)
 
         self.logger: logging.Logger = logging.getLogger(type[self].__name__)
 
+        ## metrics
+        self.fitness_metric = FitnessMetric(fitness=fitness)
+
+        metrics = {} if metrics is None else metrics
+        self.metrics = dict({"fitness": self.fitness_metric}, **metrics)
+
     def select(self, k: int) -> List[Individual]:
         """ Select k individual from the current population using a selection strategy"""
         return self.selection(k, self.population.individuals)
 
     def selection(self, k: int, individuals: List[Individual], *args, **kwargs) -> List[Individual]:
         """ Select top k individual using an a selection strategy"""
         return self.selection_strategy.select(k, self.population.individuals)
 
     def variation(self, k: int, parents: List[Individual]) -> List[Individual]:
-        """Perform variation operators (reproduction mechanism) on a group of selected individual
-        to generate the k individuals"""
+        """Perform variation operators (crossover or mutation) on a group of selected individual (parents)
+        to generate k individuals"""
 
         count = 0
         generated_individuals = []
         while count < k:
             r = random.random()
-            if self.crossover_prob > r:
+            if next(self.crossover_prob) > r:
                 parent1 = random.choice(parents)
                 parent2 = random.choice(parents) # check that the two parent are different individuals
 
                 children = self.crossover_strategy.crossover(parent1, parent2)
                 generated_individuals += children
                 count += len(children)
 
-            if self.mutation_prob > r and count < k-1:
+            if next(self.mutation_prob) > r:
                 parent = random.choice(parents)
-                child = self.mutation_strategy.mutate(parent)
-                generated_individuals.append(child)
-                count += 1
+                children = self.mutation_strategy.mutate(parent)
+                generated_individuals += children
+                count += len(children)
 
-        return generated_individuals
+        # since the crossover and mutation can generate more than one individual, therefore can generate more than
+        # the required elements, we are only seleting the first k generated (But perhaps a more appropiated way of doing this
+        # is selecting the best k)
+        if count > k:
+            self.logger.info(f"Variation operation have been generated {count} individuals. Taking only {k} individuals")
+        return generated_individuals[:k]
 
 
     def converged(self) -> bool:
         """
         Function that determine if the current population of the evolution satisfice the required condition
         using an evaluation function
 
-        True means that the evoluation process has converged and the evolution must be stoped, 
-            otherwise the evoltion process will continue
+        True means that the evolution process has converged and the evolution must be stoped,
+            otherwise the evolution process will continue
         """
         return False # if the problen hasn't a well defined stop condition, just return False
 
     def evaluate(self, individuals: List[Individual]) -> dict:
-        n = len(individuals)
-        fitnessEvaluation = [FitnessEvaluation(x, self.fitness_func(x)) for x in individuals]
+        """Evaluate metric on evolved individuals (next-generation)"""
+        self.fitness_metric.evaluate(individuals)
 
-        avg_fitness = sum([x.fitness for x in fitnessEvaluation]) / float(n)
-        best = max(fitnessEvaluation, key=lambda t: t.fitness)
-        worse = min(fitnessEvaluation, key=lambda t: t.fitness)
+        self.best = self.fitness_metric.best.individual
+        self.worse = self.fitness_metric.worse.individual
 
-        self.best = best.individual
-        self.worse = worse.individual
+        #evaluate extra metrics
+        for name, metric in self.extra_metrics.items():
+            metric.evaluate(individuals)
 
-        return {'generation': self.generation, 
+        return {'generation': self.generation,
                 'fitness': {
-                    'average': avg_fitness, 'best': best.fitness, 'worse': worse.fitness
+                    'average': self.fitness_metric.avg_fitness,
+                    'best': self.fitness_metric.best.fitness,
+                    'worse': self.fitness_metric.worse.fitness
                     },
                 'individual': {
-                    'best': [gen.value for gen in best.individual.chromosome.genes],
-                    'worse': [gen.value for gen in worse.individual.chromosome.genes]
+                    'best': [gen.value for gen in self.best.chromosome.genes],
+                    'worse': [gen.value for gen in self.worse.chromosome.genes]
                     }
                 }
 
     def population_fitness(self) -> List[float]:
         """Compute the fitness of the current population"""
         return [self.fitness_func(individual) for individual in self.population]
 
-    def _evolve(self, max_generations: int, 
-                  selection: int, descendents: int, *args, **kwargs) -> Population:
+    def evolve(self, max_generations: int,
+                  selection: int, descendents: int, plot_metrics: bool = True *args, **kwargs) -> Population:
         """
         perform the evolution of initial population using multiple variation operations
         this method quits when max number of iteratons were done or the convergence condition was met
 
         Inputs
         =======
         max_generations: maximun number of iterations (or generations - evolutions)
         selection: number of parents selected fom current population (for generate next generation)
         descendents: number of descendents to generate using variation operation over selected individuals
 
         Output
         ======
         evolved population
         """
-        pass
-    
-
-    def evolve(self, max_generations: int, 
-                  selection: int, descendents: int, *args, **kwargs) -> Population:
-        """
-        perform the evolution of initial population using multiple variation operations
-        this method quits when max number of iteratons were done or the convergence condition was met
-
-        Inputs
-        =======
-        max_generations: maximun number of iterations (or generations - evolutions)
-        selection: number of parents selected fom current population (for generate next generation)
-        descendents: number of descendents to generate using variation operation over selected individuals
 
-        Output
-        ======
-        evolved population
-        """
-        
+        k = selection # number of individual to selecte in each generation for reproduction
         population_size = self.population.size # population size
 
-         
         with tqdm(total=max_generations) as pbar: # progress bar
             while self.generation < max_generations and not self.converged():
                 #import pdb; pdb.set_trace()
                 population = self.population.individuals # current generation
 
-                selected = self.select(selection) # select individuals from current generation for reproduction
+                selected = self.select(k) # select individuals from current generation for reproduction
 
                 generated = self.variation(descendents, selected + population) # reproduction (crossover + mutation)
-                population = self.selection(population_size, generated + population) # select individuals for next generation 
+                population = self.selection(population_size, generated + population) # select individuals for next generation
 
-                self.population.individuals = population # replace old generation with new on
+                self.population.individuals = population # replace old generation with a new one
                 self.generation += 1
-                
+
                 pbar.update(1)
                 # compute metric of current generation (next-generation)
                 evaluation = self.evaluate(self.population.individuals)
                 pbar.set_postfix({'generation': self.generation, **evaluation['fitness']})
 
         if self.converged():
-            print("The evolution process was converged")   
+            self.logger.info("The evolution process converged (generation: {self.generation})")
 
         # best is element with the largest fitness and worse is the element with the smallest fitness
-        # Therefore when is maximization problem our objective is find the individual that has the best fitness (the best)
-        #, but in minimization problems our objective is find the individual with the lowerst fitness (the worse)
+        # Therefore in a maximization problem our objective is find the individual that has the best fitness (the best),
+        # however in a minimization problem our objective is find the individual with the lowerst fitness (the worse)
         print("\n" + "="*20)
         print(f"Best: {self.best.phenotype}")
         print(f"Worse: {self.worse.phenotype}")
         print("="*20)
 
         file = f"evolution-{uuid.uuid4().hex}.json"
         print(f"Writing results to: {file}")
         with open(file, 'w') as f:
             json.dump(evaluation, f, indent=4)
+
+        return self.population
```

### Comparing `cc521_evolution-1.0.3/src/evolution/population.py` & `cc521_evolution-1.0.4/src/evolution/individual.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,23 @@
 #!/usr/bin/env python3
 #
-# Base Population class
-
-from abc import ABC, abstractmethod
-from .encoding.base import DomainEncoder, Gen, Chromosome
+# Individual class - Just an encapsulation of a cromosome and a domain encoder
 
+from .encoding.base import DomainEncoder, Chromosome
 
 class Individual:
     """Encapsulate a chromosome and the encoder that generated it"""
     def __init__(self, chromosome: Chromosome, encoder: DomainEncoder):
         self.encoder = encoder
         self._chromosome = chromosome
-    
+
     @property
     def phenotype(self) -> object:
         #import pdb; pdb.set_trace()
         return self.encoder.decode(self._chromosome)
-    
+
     @property
     def chromosome(self) -> object:
         return self._chromosome
 
     def __repr__(self) -> str:
         return self._chromosome.to_str()
-
-
-class Population:
-    """Just a group of individuals"""
-    def __init__(self, domain_encoder: DomainEncoder, population: int = 10):
-        self.individuals = [Individual(domain_encoder.random(), domain_encoder) for _ in range(population)]
-
-    @property
-    def size(self):
-        return len(self.individuals)
-
-    def __iter__(self):
-        for individual in self.individuals:
-            yield individual
```

### Comparing `cc521_evolution-1.0.3/src/evolution/selection/proportional2fitness.py` & `cc521_evolution-1.0.4/src/evolution/selection/proportional2fitness.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/selection/proportional2inversefitness.py` & `cc521_evolution-1.0.4/src/evolution/selection/proportional2inversefitness.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/selection/rank_based_exponential_classification.py` & `cc521_evolution-1.0.4/src/evolution/selection/rank_based_exponential_classification.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/selection/rank_based_linear_classification.py` & `cc521_evolution-1.0.4/src/evolution/selection/rank_based_linear_classification.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/selection/roulette.py` & `cc521_evolution-1.0.4/src/evolution/selection/roulette.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/selection/tournament.py` & `cc521_evolution-1.0.4/src/evolution/selection/tournament.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/selection/uniform.py` & `cc521_evolution-1.0.4/src/evolution/selection/uniform.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/variation/crossover/bit.py` & `cc521_evolution-1.0.4/src/evolution/variation/crossover/bit.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/variation/crossover/cross_gen.py` & `cc521_evolution-1.0.4/src/evolution/variation/crossover/cross_gen.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.3/src/evolution/variation/mutation/bit.py` & `cc521_evolution-1.0.4/src/evolution/variation/mutation/bit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 #
 # Mutation mechanism for gen encoded by BitGenEncoder class
 import copy
 import random
+from typing import List
 from .base import MutationStrategy
 from ...encoding.binary import BitStreamGen
 from ...population import Individual
 
 class BitFlipMutation(MutationStrategy):
     def __init__(self):
         super(BitFlipMutation, self).__init__()
 
-    def mutate(self, parent: Individual) -> Individual:
+    def mutate(self, parent: Individual) -> List[Individual]:
         chromosome = copy.deepcopy(parent.chromosome)
         for gen in chromosome.genes:
             #assert isinstance(gen, BitStreamGen) # CHECK: DomainEncoder is not creating BitStreamGen genes
             #i = random.randint(0, gen.size-1)
             i = random.randint(0, len(gen.value)-1)
             gen.value[i] = 1 ^ gen.value[i] # 1 xor X - invert value of X to its inverse  (X in [0, 1])
 
-        return Individual(chromosome, encoder=parent.encoder)
-
+        return [Individual(chromosome, encoder=parent.encoder)]
```

### Comparing `cc521_evolution-1.0.3/PKG-INFO` & `cc521_evolution-1.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: cc521-evolution
-Version: 1.0.3
+Version: 1.0.4
 Summary: Collection of utilities to develop evolutionary algorithms
 Author: Gustavo Lozano
 Author-email: glozanoac@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
```

