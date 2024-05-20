# Comparing `tmp/cc521_evolution-1.0.4.tar.gz` & `tmp/cc521_evolution-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc521_evolution-1.0.4.tar", max compression
+gzip compressed data, was "cc521_evolution-1.0.6.tar", max compression
```

## Comparing `cc521_evolution-1.0.4.tar` & `cc521_evolution-1.0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0        0 2024-04-20 16:48:16.722884 cc521_evolution-1.0.4/README.md
--rw-r--r--   0        0        0      435 2024-05-19 11:31:10.598555 cc521_evolution-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       80 2024-05-01 15:27:09.336087 cc521_evolution-1.0.4/src/evolution/__init__.py
--rw-r--r--   0        0        0      354 2024-05-01 10:53:16.697215 cc521_evolution-1.0.4/src/evolution/encoding/__init__.py
--rw-r--r--   0        0        0     3175 2024-05-19 11:08:43.520350 cc521_evolution-1.0.4/src/evolution/encoding/base.py
--rw-r--r--   0        0        0     2421 2024-05-01 17:43:12.613572 cc521_evolution-1.0.4/src/evolution/encoding/binary.py
--rw-r--r--   0        0        0     2034 2024-05-01 12:32:18.671279 cc521_evolution-1.0.4/src/evolution/encoding/gray.py
--rw-r--r--   0        0        0     1506 2024-04-20 12:41:59.068191 cc521_evolution-1.0.4/src/evolution/encoding/gray_code.py
--rw-r--r--   0        0        0     4772 2024-05-01 19:04:10.318473 cc521_evolution-1.0.4/src/evolution/encoding/interval.py
--rw-r--r--   0        0        0     8629 2024-05-15 15:39:00.396113 cc521_evolution-1.0.4/src/evolution/evolution.py
--rw-r--r--   0        0        0      498 2024-05-15 12:10:21.455530 cc521_evolution-1.0.4/src/evolution/fitness.py
--rw-r--r--   0        0        0        0 2024-05-15 15:40:53.771300 cc521_evolution-1.0.4/src/evolution/history/__init__.py
--rw-r--r--   0        0        0      647 2024-05-15 15:51:00.283651 cc521_evolution-1.0.4/src/evolution/history/base.py
--rw-r--r--   0        0        0      683 2024-05-15 12:32:31.896803 cc521_evolution-1.0.4/src/evolution/individual.py
--rw-r--r--   0        0        0       69 2024-05-15 12:25:02.449380 cc521_evolution-1.0.4/src/evolution/metrics/__init__.py
--rw-r--r--   0        0        0      270 2024-05-15 12:08:33.983499 cc521_evolution-1.0.4/src/evolution/metrics/base.py
--rw-r--r--   0        0        0     1145 2024-05-15 12:36:13.235607 cc521_evolution-1.0.4/src/evolution/metrics/fitness.py
--rw-r--r--   0        0        0     1363 2024-05-15 14:23:53.737905 cc521_evolution-1.0.4/src/evolution/population.py
--rw-r--r--   0        0        0      179 2024-05-01 23:44:32.151131 cc521_evolution-1.0.4/src/evolution/selection/__init__.py
--rw-r--r--   0        0        0      487 2024-05-01 15:28:52.057254 cc521_evolution-1.0.4/src/evolution/selection/base.py
--rw-r--r--   0        0        0       53 2024-05-15 12:10:14.122058 cc521_evolution-1.0.4/src/evolution/selection/misc.py
--rw-r--r--   0        0        0      762 2024-05-01 19:07:59.046499 cc521_evolution-1.0.4/src/evolution/selection/proportional2fitness.py
--rw-r--r--   0        0        0      802 2024-05-01 23:43:39.304984 cc521_evolution-1.0.4/src/evolution/selection/proportional2inversefitness.py
--rw-r--r--   0        0        0     1657 2024-04-28 06:27:18.505872 cc521_evolution-1.0.4/src/evolution/selection/rank_based_exponential_classification.py
--rw-r--r--   0        0        0     1547 2024-04-28 06:28:09.901230 cc521_evolution-1.0.4/src/evolution/selection/rank_based_linear_classification.py
--rw-r--r--   0        0        0     2011 2024-04-28 06:51:23.729483 cc521_evolution-1.0.4/src/evolution/selection/roulette.py
--rw-r--r--   0        0        0     2409 2024-04-28 06:45:40.145945 cc521_evolution-1.0.4/src/evolution/selection/tournament.py
--rw-r--r--   0        0        0      862 2024-04-28 06:49:12.924329 cc521_evolution-1.0.4/src/evolution/selection/uniform.py
--rw-r--r--   0        0        0        0 2024-05-01 14:45:46.565897 cc521_evolution-1.0.4/src/evolution/variation/__init__.py
--rw-r--r--   0        0        0      159 2024-05-01 14:47:11.100554 cc521_evolution-1.0.4/src/evolution/variation/crossover/__init__.py
--rw-r--r--   0        0        0      313 2024-05-19 11:27:55.394824 cc521_evolution-1.0.4/src/evolution/variation/crossover/base.py
--rw-r--r--   0        0        0     1478 2024-05-01 19:59:49.362851 cc521_evolution-1.0.4/src/evolution/variation/crossover/bit.py
--rw-r--r--   0        0        0      553 2024-04-20 13:27:30.081869 cc521_evolution-1.0.4/src/evolution/variation/crossover/cross_gen.py
--rw-r--r--   0        0        0      157 2024-05-01 14:49:17.034398 cc521_evolution-1.0.4/src/evolution/variation/mutation/__init__.py
--rw-r--r--   0        0        0      538 2024-05-15 12:33:08.896494 cc521_evolution-1.0.4/src/evolution/variation/mutation/base.py
--rw-r--r--   0        0        0      895 2024-05-15 11:51:29.633436 cc521_evolution-1.0.4/src/evolution/variation/mutation/bit.py
--rw-r--r--   0        0        0     1165 2024-05-15 13:58:00.293361 cc521_evolution-1.0.4/src/evolution/variation/probability.py
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 cc521_evolution-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 16:48:16.722884 cc521_evolution-1.0.6/README.md
+-rw-r--r--   0        0        0      435 2024-05-20 02:27:32.119768 cc521_evolution-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-05-01 15:27:09.336087 cc521_evolution-1.0.6/src/evolution/__init__.py
+-rw-r--r--   0        0        0      354 2024-05-01 10:53:16.697215 cc521_evolution-1.0.6/src/evolution/encoding/__init__.py
+-rw-r--r--   0        0        0     3161 2024-05-20 02:07:24.049320 cc521_evolution-1.0.6/src/evolution/encoding/base.py
+-rw-r--r--   0        0        0     2723 2024-05-20 02:14:33.021360 cc521_evolution-1.0.6/src/evolution/encoding/binary.py
+-rw-r--r--   0        0        0     2034 2024-05-01 12:32:18.671279 cc521_evolution-1.0.6/src/evolution/encoding/gray.py
+-rw-r--r--   0        0        0     1506 2024-04-20 12:41:59.068191 cc521_evolution-1.0.6/src/evolution/encoding/gray_code.py
+-rw-r--r--   0        0        0     4266 2024-05-20 02:16:56.378323 cc521_evolution-1.0.6/src/evolution/encoding/interval.py
+-rw-r--r--   0        0        0     9010 2024-05-20 02:27:09.999104 cc521_evolution-1.0.6/src/evolution/evolution.py
+-rw-r--r--   0        0        0      498 2024-05-15 12:10:21.455530 cc521_evolution-1.0.6/src/evolution/fitness.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:40:53.771300 cc521_evolution-1.0.6/src/evolution/history/__init__.py
+-rw-r--r--   0        0        0      647 2024-05-15 15:51:00.283651 cc521_evolution-1.0.6/src/evolution/history/base.py
+-rw-r--r--   0        0        0      683 2024-05-15 12:32:31.896803 cc521_evolution-1.0.6/src/evolution/individual.py
+-rw-r--r--   0        0        0       69 2024-05-15 12:25:02.449380 cc521_evolution-1.0.6/src/evolution/metrics/__init__.py
+-rw-r--r--   0        0        0      270 2024-05-15 12:08:33.983499 cc521_evolution-1.0.6/src/evolution/metrics/base.py
+-rw-r--r--   0        0        0     1145 2024-05-15 12:36:13.235607 cc521_evolution-1.0.6/src/evolution/metrics/fitness.py
+-rw-r--r--   0        0        0     1363 2024-05-15 14:23:53.737905 cc521_evolution-1.0.6/src/evolution/population.py
+-rw-r--r--   0        0        0      179 2024-05-01 23:44:32.151131 cc521_evolution-1.0.6/src/evolution/selection/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-01 15:28:52.057254 cc521_evolution-1.0.6/src/evolution/selection/base.py
+-rw-r--r--   0        0        0       53 2024-05-15 12:10:14.122058 cc521_evolution-1.0.6/src/evolution/selection/misc.py
+-rw-r--r--   0        0        0      762 2024-05-01 19:07:59.046499 cc521_evolution-1.0.6/src/evolution/selection/proportional2fitness.py
+-rw-r--r--   0        0        0      802 2024-05-01 23:43:39.304984 cc521_evolution-1.0.6/src/evolution/selection/proportional2inversefitness.py
+-rw-r--r--   0        0        0     1657 2024-04-28 06:27:18.505872 cc521_evolution-1.0.6/src/evolution/selection/rank_based_exponential_classification.py
+-rw-r--r--   0        0        0     1547 2024-04-28 06:28:09.901230 cc521_evolution-1.0.6/src/evolution/selection/rank_based_linear_classification.py
+-rw-r--r--   0        0        0     2011 2024-04-28 06:51:23.729483 cc521_evolution-1.0.6/src/evolution/selection/roulette.py
+-rw-r--r--   0        0        0     2409 2024-04-28 06:45:40.145945 cc521_evolution-1.0.6/src/evolution/selection/tournament.py
+-rw-r--r--   0        0        0      862 2024-04-28 06:49:12.924329 cc521_evolution-1.0.6/src/evolution/selection/uniform.py
+-rw-r--r--   0        0        0        0 2024-05-01 14:45:46.565897 cc521_evolution-1.0.6/src/evolution/variation/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-01 14:47:11.100554 cc521_evolution-1.0.6/src/evolution/variation/crossover/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-19 11:27:55.394824 cc521_evolution-1.0.6/src/evolution/variation/crossover/base.py
+-rw-r--r--   0        0        0     1478 2024-05-01 19:59:49.362851 cc521_evolution-1.0.6/src/evolution/variation/crossover/bit.py
+-rw-r--r--   0        0        0      553 2024-04-20 13:27:30.081869 cc521_evolution-1.0.6/src/evolution/variation/crossover/cross_gen.py
+-rw-r--r--   0        0        0      157 2024-05-01 14:49:17.034398 cc521_evolution-1.0.6/src/evolution/variation/mutation/__init__.py
+-rw-r--r--   0        0        0      538 2024-05-15 12:33:08.896494 cc521_evolution-1.0.6/src/evolution/variation/mutation/base.py
+-rw-r--r--   0        0        0      895 2024-05-15 11:51:29.633436 cc521_evolution-1.0.6/src/evolution/variation/mutation/bit.py
+-rw-r--r--   0        0        0     1165 2024-05-15 13:58:00.293361 cc521_evolution-1.0.6/src/evolution/variation/probability.py
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 cc521_evolution-1.0.6/PKG-INFO
```

### Comparing `cc521_evolution-1.0.4/src/evolution/encoding/base.py` & `cc521_evolution-1.0.6/src/evolution/encoding/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 class Chromosome:
     def __init__(self, components: List[ChromosomeComponent]):
         self._components = components
 
     def chromosome_component(self, k: int) -> ChromosomeComponent:
         assert k < self.ngenes
         return self._components[k]
-        
+
     def component(self, k: int) -> Tuple[Gen, GenEncoder]:
         """Return component k of chromosome"""
         component = self.chromosome_component(k)
         return (component.gen, component.encoder)
 
     @property
     def chromosome_components(self):
@@ -91,15 +91,14 @@
         return [self.decode_component(component) for component in chromosome.chromosome_components]
 
     def decode_component(self, component: ChromosomeComponent) -> object:
         encoder, gen = component.encoder, component.gen
         return encoder.decode(gen)
 
     def random(self) -> Chromosome:
-         """Generate a random chromosome"""
+        """Generate a random chromosome"""
         components = []
         for gen_encoder in self.gen_encoders:
             component = ChromosomeComponent(gen_encoder.random(), encoder=gen_encoder)
             components.append(component)
 
         return Chromosome(components=components)
-
```

### Comparing `cc521_evolution-1.0.4/src/evolution/encoding/binary.py` & `cc521_evolution-1.0.6/src/evolution/encoding/binary.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """From binary to decimal"""
     return int(binary, 2)
 
 
 class BitStreamGen(Gen):
     def __init__(self, value: List[int]):
         for bit in value:
-            assert isintance(bit, int) and bit in [0, 1], f"Bit must be an integer and its value must be 0 or 1, not {bit} (gene: {value})"
+            assert isinstance(bit, int) and bit in [0, 1], f"Bit must be an integer and its value must be 0 or 1, not {bit} (gene: {value})"
         super(BitStreamGen, self).__init__(value)
 
     @property
     def size(self) -> int:
         return len(self.value)
 
     def __str__(self) -> str:
@@ -48,22 +48,36 @@
             return Gen(value = [int(bit) for bit in to_binary(x, self.nbits)])
         else:
             if (size := len(x)) > self.nbits:
                 logging.warning(f"Expecting a bitstream with at most {self.nbits} bits, but given one with {size} bits. Taking only {self.nbits} least significant bits")
                 x = x[-self.nbits:]
             else:
                 x = x.zfill(self.nbits)
-                
+
             bits = []
             for bit in x:
                 assert bit in ['0', '1'], f"Bit must be '0' or '1', and not {bit} (object being encoding: {x})"
                 bits.append(int(bit))
             return BitStreamGen(value=bits)
 
     def decode(self, gen: BitStreamGen) -> object:
         #assert isinstance(gen, BitStreamGen), f"gen is expected to be an instance of BitStreamGen class"
         bits = ''.join([str(x) for x in gen.value])
         #import pdb; pdb.set_trace()
         #for bit in gen.value:
         #    assert isinstance(bit, int) and bit in [0, 1] # this responsability was delegated to BitStreamGen (REMOVE)
         #    bits += str(bit)
         return from_binary(bits)
+
+
+    def random(self) -> Gen:
+        """
+        Generate a point on encoded interval
+
+        Returns
+        =======
+        chromosome
+        """
+        point = random.randint(0, 2**self.nbits-1)
+
+        value= [int(bit) for bit in to_binary(point, nbits=self.nbits)]
+        return BitStreamGen(value=value)
```

### Comparing `cc521_evolution-1.0.4/src/evolution/encoding/gray.py` & `cc521_evolution-1.0.6/src/evolution/encoding/gray.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/encoding/gray_code.py` & `cc521_evolution-1.0.6/src/evolution/encoding/gray_code.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/encoding/interval.py` & `cc521_evolution-1.0.6/src/evolution/encoding/interval.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         if b <= a:
             raise Exception(f"Expected a regular interval (low-bound: {a}, high-bound: {b})")
 
         self.lower_bound = a
         self.upper_bound = b
         self.nbits = math.ceil(math.log2((b-a)/delta)) # estimate numbers of bits to represent partition
         self.delta = (b-a)/(2**self.nbits-1)
-        
+
         assert issubclass(gen_encoder_cls, BitGenEncoder)
         super(IntervalEncoder, self).__init__(gen_encoders = [gen_encoder_cls(nbits=self.nbits)])
 
     def _phenotype(self, jumps: int) -> float:
         """
         Inputs
         ======
@@ -58,45 +58,28 @@
         phenotype = super().decode(chromosome)[0]
         return phenotype
 
     def decode_component(self, component: ChromosomeComponent) -> float:
         """decode chromosome component from encoded form to phenotype"""
         gen, encoder = component.gen, component.encoder
         #import pdb; pdb.set_trace()
-        jumps = encoder.decode(gen) # jumps from 0000 ... 000  chromosome to supplied chromosome 
+        jumps = encoder.decode(gen) # jumps from 0000 ... 000  chromosome to supplied chromosome
         return self._phenotype(jumps)
 
     @property
     def gen_encoder(self):
         return self.gen_encoders[0]
 
     @property
     def describe(self):
         x = self._partition
         x['delta'] = self.delta # updated delta
         x['bits'] = self.nbits
         return x
 
-    def random(self) -> Chromosome:
-        """
-        Generate a point on encoded interval
-
-        Returns
-        =======
-        chromosome
-        """
-        components = []
-        for gen_encoder in self.gen_encoders:
-            point = random.randint(0, 2**self.nbits-1)
-            gen = gen_encoder.encode(point)
-            component = ChromosomeComponent(gen, encoder=gen_encoder)
-            components.append(component)
-
-        return Chromosome(components=components)
-
 
 class MultipleIntervalEncoder(DomainEncoder):
     def __init__(self, partitions: List[IntervalPartition]):
         self.interval_encoders: List[IntervalEncoder] = [IntervalEncoder(partition=p) for p in partitions]
 
     def encoder(self, k: int) -> IntervalEncoder:
         assert k >= len(self.interval_encoder), f"Number of interval encoders: {len(self.interval_encoder)} - Trying to acces to {k}"
@@ -106,28 +89,28 @@
     def describe(self):
         return [encoder.describe for encoder in self.interval_encoders]
 
     def decode(self, chromosome: Chromosome) -> List[float]:
         assert len(self.interval_encoders) == chromosome.ngenes, f"Expecting a chromosome with {len(self.interval_encoders)} genes, not one with {chromosome.ngenes}."
 
         #import pdb; pdb.set_trace()
-        phenotype = [encoder.decode_component(component) 
+        phenotype = [encoder.decode_component(component)
                      for encoder, component in zip(self.interval_encoders, chromosome.chromosome_components)]
 
         return phenotype
 
     def random(self) -> Chromosome:
         """
         Generate a point on encoded interval
 
         Returns
         =======
         chromosome: Chromosome
         """
-        
+
         components = []
         for encoder in self.interval_encoders:
             chromosome = encoder.random() # generated interval chromosome has only 1 component
             component = chromosome.chromosome_component(0)
             components.append(component)
 
         return Chromosome(components=components)
```

### Comparing `cc521_evolution-1.0.4/src/evolution/evolution.py` & `cc521_evolution-1.0.6/src/evolution/evolution.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,31 +23,35 @@
 
 from .metrics import EvolutionMetric, FitnessMetric
 
 
 class Evolution:
     def __init__(self, population: Population, *,
                  fitness: Callable[[object], float],
-                 selection_strategy: SelectionStrategy,
+                 selection_strategy: SelectionStrategy, # selection strategy to select parents
                  # variation strategies
                  crossover_strategy: CrossoverStrategy,
                  mutation_strategy: MutationStrategy,
                  crossover_prob: Union[float, Iterable] , mutation_prob: Union[float, Iterable],
-                 metrics: dict[str, EvolutionMetric] = None):
+                 metrics: dict[str, EvolutionMetric] = None,
+                 next_generation_selection_strategy: SelectionStrategy = None):
         self.fitness_func = fitness
         self.population = population
         self.generation: int = 1
 
         self.best: Individual = None # invidividual with the largest fitness value on the last generation
         self.worse: Individual = None # invidividual with the smallest fitness value on the last generation
 
-        self.selection_strategy = selection_strategy
-        self.crossover_strategy = crossover_strategy
+        self.parent_selection_strategy = selection_strategy
+        self.next_generation_selection_strategy = selection_strategy
+        if next_generation_selection_strategy is not None:
+            self.next_generation_selection_strategy = next_generation_selection_strategy
 
-        # variation(crossover and mutation) probabilities
+        # variation(crossover and mutation)
+        self.crossover_strategy = crossover_strategy
         self.crossover_prob = crossover_prob
         if not isinstance(crossover_prob, Iterable):
             self.crossover_prob = ConstantVariationProbability(value=crossover_prob)
 
         self.mutation_strategy = mutation_strategy
         self.mutation_prob = mutation_prob
         if not isinstance(mutation_prob, Iterable):
@@ -57,21 +61,21 @@
 
         ## metrics
         self.fitness_metric = FitnessMetric(fitness=fitness)
 
         metrics = {} if metrics is None else metrics
         self.metrics = dict({"fitness": self.fitness_metric}, **metrics)
 
-    def select(self, k: int) -> List[Individual]:
+    def select_next_generation(self, k: int, individuals: List[Individual]) -> List[Individual]:
         """ Select k individual from the current population using a selection strategy"""
-        return self.selection(k, self.population.individuals)
+        return self.next_generation_selection_strategy.select(k, individuals)
 
-    def selection(self, k: int, individuals: List[Individual], *args, **kwargs) -> List[Individual]:
-        """ Select top k individual using an a selection strategy"""
-        return self.selection_strategy.select(k, self.population.individuals)
+    def select_parents(self, k: int, individuals: List[Individual], *args, **kwargs) -> List[Individual]:
+        """ Select individuals using a selection strategy"""
+        return self.parent_selection_strategy.select(k, individuals)
 
     def variation(self, k: int, parents: List[Individual]) -> List[Individual]:
         """Perform variation operators (crossover or mutation) on a group of selected individual (parents)
         to generate k individuals"""
 
         count = 0
         generated_individuals = []
@@ -113,16 +117,16 @@
         """Evaluate metric on evolved individuals (next-generation)"""
         self.fitness_metric.evaluate(individuals)
 
         self.best = self.fitness_metric.best.individual
         self.worse = self.fitness_metric.worse.individual
 
         #evaluate extra metrics
-        for name, metric in self.extra_metrics.items():
-            metric.evaluate(individuals)
+        # for name, metric in self.metrics.items():
+        #     metric.evaluate(individuals)
 
         return {'generation': self.generation,
                 'fitness': {
                     'average': self.fitness_metric.avg_fitness,
                     'best': self.fitness_metric.best.fitness,
                     'worse': self.fitness_metric.worse.fitness
                     },
@@ -132,16 +136,17 @@
                     }
                 }
 
     def population_fitness(self) -> List[float]:
         """Compute the fitness of the current population"""
         return [self.fitness_func(individual) for individual in self.population]
 
+
     def evolve(self, max_generations: int,
-                  selection: int, descendents: int, plot_metrics: bool = True *args, **kwargs) -> Population:
+               selection: int, descendents: int) -> Population:
         """
         perform the evolution of initial population using multiple variation operations
         this method quits when max number of iteratons were done or the convergence condition was met
 
         Inputs
         =======
         max_generations: maximun number of iterations (or generations - evolutions)
@@ -157,18 +162,19 @@
         population_size = self.population.size # population size
 
         with tqdm(total=max_generations) as pbar: # progress bar
             while self.generation < max_generations and not self.converged():
                 #import pdb; pdb.set_trace()
                 population = self.population.individuals # current generation
 
-                selected = self.select(k) # select individuals from current generation for reproduction
-
+                selected = self.select_parents(k, population) # select individuals from current generation for reproduction
                 generated = self.variation(descendents, selected + population) # reproduction (crossover + mutation)
-                population = self.selection(population_size, generated + population) # select individuals for next generation
+
+                # select individuals for next generation
+                population = self.select_next_generation(population_size, generated + population)
 
                 self.population.individuals = population # replace old generation with a new one
                 self.generation += 1
 
                 pbar.update(1)
                 # compute metric of current generation (next-generation)
                 evaluation = self.evaluate(self.population.individuals)
```

### Comparing `cc521_evolution-1.0.4/src/evolution/history/base.py` & `cc521_evolution-1.0.6/src/evolution/history/base.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/individual.py` & `cc521_evolution-1.0.6/src/evolution/individual.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/metrics/fitness.py` & `cc521_evolution-1.0.6/src/evolution/metrics/fitness.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/population.py` & `cc521_evolution-1.0.6/src/evolution/population.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/selection/proportional2fitness.py` & `cc521_evolution-1.0.6/src/evolution/selection/proportional2fitness.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/selection/proportional2inversefitness.py` & `cc521_evolution-1.0.6/src/evolution/selection/proportional2inversefitness.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/selection/rank_based_exponential_classification.py` & `cc521_evolution-1.0.6/src/evolution/selection/rank_based_exponential_classification.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/selection/rank_based_linear_classification.py` & `cc521_evolution-1.0.6/src/evolution/selection/rank_based_linear_classification.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/selection/roulette.py` & `cc521_evolution-1.0.6/src/evolution/selection/roulette.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/selection/tournament.py` & `cc521_evolution-1.0.6/src/evolution/selection/tournament.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/selection/uniform.py` & `cc521_evolution-1.0.6/src/evolution/selection/uniform.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/variation/crossover/bit.py` & `cc521_evolution-1.0.6/src/evolution/variation/crossover/bit.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/variation/crossover/cross_gen.py` & `cc521_evolution-1.0.6/src/evolution/variation/crossover/cross_gen.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/variation/mutation/base.py` & `cc521_evolution-1.0.6/src/evolution/variation/mutation/base.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/variation/mutation/bit.py` & `cc521_evolution-1.0.6/src/evolution/variation/mutation/bit.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/src/evolution/variation/probability.py` & `cc521_evolution-1.0.6/src/evolution/variation/probability.py`

 * *Files identical despite different names*

### Comparing `cc521_evolution-1.0.4/PKG-INFO` & `cc521_evolution-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc521-evolution
-Version: 1.0.4
+Version: 1.0.6
 Summary: Collection of utilities to develop evolutionary algorithms
 Author: Gustavo Lozano
 Author-email: glozanoac@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

