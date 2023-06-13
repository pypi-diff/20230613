# Comparing `tmp/auxein-0.1.0.tar.gz` & `tmp/auxein-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auxein-0.1.0.tar", max compression
+gzip compressed data, was "auxein-0.1.1.tar", max compression
```

## Comparing `auxein-0.1.0.tar` & `auxein-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11346 2023-06-10 19:35:09.851119 auxein-0.1.0/LICENSE
--rw-r--r--   0        0        0      428 2023-06-10 19:35:09.851376 auxein-0.1.0/auxein/__init__.py
--rw-r--r--   0        0        0      216 2023-06-10 19:35:09.851485 auxein-0.1.0/auxein/fitness/__init__.py
--rw-r--r--   0        0        0      476 2023-06-10 19:35:09.851565 auxein-0.1.0/auxein/fitness/core.py
--rw-r--r--   0        0        0      672 2023-06-10 19:35:09.851633 auxein-0.1.0/auxein/fitness/kernel_based.py
--rw-r--r--   0        0        0     3411 2023-06-10 19:35:09.851706 auxein-0.1.0/auxein/fitness/observation_based.py
--rw-r--r--   0        0        0      166 2023-06-10 19:35:09.851807 auxein-0.1.0/auxein/fitness/utils/__init__.py
--rw-r--r--   0        0        0     1393 2023-06-10 19:35:09.851872 auxein-0.1.0/auxein/fitness/utils/utils.py
--rw-r--r--   0        0        0      140 2023-06-10 19:35:09.851986 auxein-0.1.0/auxein/mutations/__init__.py
--rw-r--r--   0        0        0     2703 2023-06-10 19:35:09.852067 auxein-0.1.0/auxein/mutations/core.py
--rw-r--r--   0        0        0      106 2023-06-10 19:35:09.852173 auxein-0.1.0/auxein/parents/__init__.py
--rw-r--r--   0        0        0      134 2023-06-10 19:35:09.852288 auxein-0.1.0/auxein/parents/distributions/__init__.py
--rw-r--r--   0        0        0     1924 2023-06-10 19:35:09.852364 auxein-0.1.0/auxein/parents/distributions/core.py
--rw-r--r--   0        0        0      142 2023-06-10 19:35:09.852473 auxein-0.1.0/auxein/parents/selections/__init__.py
--rw-r--r--   0        0        0     1460 2023-06-10 19:35:09.852545 auxein-0.1.0/auxein/parents/selections/core.py
--rw-r--r--   0        0        0       42 2023-06-10 19:35:09.852648 auxein-0.1.0/auxein/playgrounds/__init__.py
--rw-r--r--   0        0        0     5138 2023-06-10 19:35:09.852721 auxein-0.1.0/auxein/playgrounds/static.py
--rw-r--r--   0        0        0      305 2023-06-10 19:35:09.852815 auxein-0.1.0/auxein/population/__init__.py
--rw-r--r--   0        0        0     5244 2023-06-10 19:35:09.852888 auxein-0.1.0/auxein/population/core.py
--rw-r--r--   0        0        0     1488 2023-06-10 19:35:09.852958 auxein-0.1.0/auxein/population/dna_builders.py
--rw-r--r--   0        0        0      640 2023-06-10 19:35:09.853027 auxein-0.1.0/auxein/population/genotype.py
--rw-r--r--   0        0        0     1441 2023-06-10 19:35:09.853099 auxein-0.1.0/auxein/population/individual.py
--rw-r--r--   0        0        0      120 2023-06-10 19:35:09.853193 auxein-0.1.0/auxein/recombinations/__init__.py
--rw-r--r--   0        0        0     3180 2023-06-10 19:35:09.853265 auxein-0.1.0/auxein/recombinations/core.py
--rw-r--r--   0        0        0       76 2023-06-10 19:35:09.853360 auxein-0.1.0/auxein/replacements/__init__.py
--rw-r--r--   0        0        0     1624 2023-06-10 19:35:09.853448 auxein-0.1.0/auxein/replacements/core.py
--rw-r--r--   0        0        0      472 2023-06-10 20:41:10.670390 auxein-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 auxein-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-10 19:35:09.851119 auxein-0.1.1/LICENSE
+-rw-r--r--   0        0        0      428 2023-06-10 19:35:09.851376 auxein-0.1.1/auxein/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-10 19:35:09.851485 auxein-0.1.1/auxein/fitness/__init__.py
+-rw-r--r--   0        0        0      476 2023-06-10 19:35:09.851565 auxein-0.1.1/auxein/fitness/core.py
+-rw-r--r--   0        0        0      672 2023-06-12 12:28:18.428684 auxein-0.1.1/auxein/fitness/kernel_based.py
+-rw-r--r--   0        0        0     3873 2023-06-12 16:02:25.095800 auxein-0.1.1/auxein/fitness/observation_based.py
+-rw-r--r--   0        0        0      166 2023-06-10 19:35:09.851807 auxein-0.1.1/auxein/fitness/utils/__init__.py
+-rw-r--r--   0        0        0     1393 2023-06-10 19:35:09.851872 auxein-0.1.1/auxein/fitness/utils/utils.py
+-rw-r--r--   0        0        0      140 2023-06-10 19:35:09.851986 auxein-0.1.1/auxein/mutations/__init__.py
+-rw-r--r--   0        0        0     3122 2023-06-12 16:02:25.096253 auxein-0.1.1/auxein/mutations/core.py
+-rw-r--r--   0        0        0      106 2023-06-10 19:35:09.852173 auxein-0.1.1/auxein/parents/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-10 19:35:09.852288 auxein-0.1.1/auxein/parents/distributions/__init__.py
+-rw-r--r--   0        0        0     1924 2023-06-10 19:35:09.852364 auxein-0.1.1/auxein/parents/distributions/core.py
+-rw-r--r--   0        0        0      142 2023-06-10 19:35:09.852473 auxein-0.1.1/auxein/parents/selections/__init__.py
+-rw-r--r--   0        0        0     1462 2023-06-12 16:02:25.096958 auxein-0.1.1/auxein/parents/selections/core.py
+-rw-r--r--   0        0        0       42 2023-06-10 19:35:09.852648 auxein-0.1.1/auxein/playgrounds/__init__.py
+-rw-r--r--   0        0        0     5319 2023-06-12 16:02:25.097384 auxein-0.1.1/auxein/playgrounds/static.py
+-rw-r--r--   0        0        0      326 2023-06-12 19:19:45.297665 auxein-0.1.1/auxein/population/__init__.py
+-rw-r--r--   0        0        0     5690 2023-06-12 16:02:25.097845 auxein-0.1.1/auxein/population/core.py
+-rw-r--r--   0        0        0     2258 2023-06-12 19:19:45.298482 auxein-0.1.1/auxein/population/dna_builders.py
+-rw-r--r--   0        0        0      640 2023-06-10 19:35:09.853027 auxein-0.1.1/auxein/population/genotype.py
+-rw-r--r--   0        0        0     1441 2023-06-10 19:35:09.853099 auxein-0.1.1/auxein/population/individual.py
+-rw-r--r--   0        0        0      120 2023-06-10 19:35:09.853193 auxein-0.1.1/auxein/recombinations/__init__.py
+-rw-r--r--   0        0        0     3180 2023-06-10 19:35:09.853265 auxein-0.1.1/auxein/recombinations/core.py
+-rw-r--r--   0        0        0       76 2023-06-10 19:35:09.853360 auxein-0.1.1/auxein/replacements/__init__.py
+-rw-r--r--   0        0        0     1624 2023-06-10 19:35:09.853448 auxein-0.1.1/auxein/replacements/core.py
+-rw-r--r--   0        0        0      472 2023-06-12 19:20:52.745710 auxein-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 auxein-0.1.1/PKG-INFO
```

### Comparing `auxein-0.1.0/LICENSE` & `auxein-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auxein-0.1.0/auxein/fitness/kernel_based.py` & `auxein-0.1.1/auxein/fitness/kernel_based.py`

 * *Files identical despite different names*

### Comparing `auxein-0.1.0/auxein/fitness/observation_based.py` & `auxein-0.1.1/auxein/fitness/observation_based.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from .core import Fitness
 from .utils import linear_fit, polynomial_fit, least_squares, logit
 from auxein.population import build_individual, Individual
 
 
 class ObservationBasedFitness(Fitness):
+    """Abstract class for observation-based fitness function.
+    """
 
     @abstractmethod
     def fitness(self, individual: Individual) -> float:
         pass
 
     @abstractmethod
     def value(self, individual: Individual, x: np.ndarray) -> float:
@@ -33,26 +35,33 @@
         assert len(specs) == 2, 'Only 2-dimensional fitness landscapes are supported at the moment.'
         A = np.linspace(specs[0][0], specs[0][1], size)
         B = np.linspace(specs[1][0], specs[1][1], size)
         return self.__compute_f(A, B)
 
 
 class MultipleLinearRegression(ObservationBasedFitness):
+    """Multiple linear regression fitness function.
+    Given a set of observations (xi, yi), the fitness function will be computed as the
+    sum of the squared residuals of the linear regression model.
+    """
 
     def __init__(self, xs: np.ndarray, y: np.ndarray) -> None:
         super().__init__()
         assert xs.shape == (y.shape[0], xs.shape[1]), 'length of xs must be equal to length of y'
         self.xs = xs
         self.y = y
 
     def fitness(self, individual: Individual) -> float:
         dna = individual.genotype.dna
         return -1 * least_squares(self.xs, self.y, dna)
 
     def value(self, individual: Individual, x: np.ndarray) -> float:
+        """Compute the value of the linear regression model for a given x given an individual
+        representing the a and b coefficients of the linear model ax + b.
+        """
         dna = individual.genotype.dna
         return linear_fit(dna, x)
 
 
 class SimplePolynomialRegression(ObservationBasedFitness):
 
     def __init__(self, xs: np.ndarray, y: np.ndarray) -> None:
```

### Comparing `auxein-0.1.0/auxein/fitness/utils/utils.py` & `auxein-0.1.1/auxein/fitness/utils/utils.py`

 * *Files identical despite different names*

### Comparing `auxein-0.1.0/auxein/mutations/core.py` & `auxein-0.1.1/auxein/mutations/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 from auxein.population.genotype import Genotype
 
 import numpy as np
 
 
 class Mutation(ABC):
+    """Abstract class for mutations.
+    
+    Given an Individual, a Mutation is responsible for generating a new Individual with a mutated genotype.
+    """
 
     def __init__(self, extend_probability: float = 0.0):
         assert 0 <= extend_probability <= 1, 'extend_probability must be within [0, 1]'
         self.extend_probability = extend_probability
 
     def _extend(self, genotype: Genotype, new_gene: float) -> Genotype:
         if np.random.uniform(0, 1) <= self.extend_probability:
@@ -56,14 +60,19 @@
     def mutate(self, genotype: Genotype) -> Genotype:
         move = np.vectorize(lambda g: g + np.random.normal(0, self.sigma))
         new_gene = np.random.normal(0, self.sigma)
         return super()._extend(Genotype(move(genotype.dna), genotype.mask), new_gene)
 
 
 class SelfAdaptiveSingleStep(Mutation):
+    """Self-adaptive single step mutation as described in [back01].
+    
+    [back01]  T. Back, D.B. Fogel, and Z. Michalewicz, editors. 
+    "Evolutionary Computation 2:dvanced Algorithms and Operators. Institute of Physics Publishing", Bristol, 2000.
+    """
 
     def __init__(self, tau: float, extend_probability: float = 0.0) -> None:
         super().__init__(extend_probability=extend_probability)
         self.tau = tau
 
     def mutate(self, genotype: Genotype) -> Genotype:
         multiplier = np.exp(np.random.normal(0, self.tau))
```

### Comparing `auxein-0.1.0/auxein/parents/distributions/core.py` & `auxein-0.1.1/auxein/parents/distributions/core.py`

 * *Files identical despite different names*

### Comparing `auxein-0.1.0/auxein/parents/selections/core.py` & `auxein-0.1.1/auxein/parents/selections/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,9 +38,11 @@
         index = 0
         mating_pool: List[str] = []
         r = np.random.uniform(0, 1 / self.parents_to_select)
         while len(mating_pool) < self.parents_to_select:
             while r <= cumulative_probability_distribution(index, probabilities):
                 mating_pool.append(individual_ids[index])
                 r += 1 / self.parents_to_select
+
             index += 1
+
         return mating_pool
```

### Comparing `auxein-0.1.0/auxein/playgrounds/static.py` & `auxein-0.1.1/auxein/playgrounds/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 from auxein.parents.selections import Selection
 from auxein.replacements import Replacement
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 class Playground(ABC):
+    """Abstract class for playgrounds.
+    A playground is a class that implements the training and prediction methods and it 
+    represents the entire evolutionary cycle.
+    """
 
     def __init__(self, population: Population, fitness: Fitness) -> None:
         self.population = population
         self.fitness = fitness
 
     @abstractmethod
     def train(self, max_generations: int) -> Dict[str, Any]:
```

### Comparing `auxein-0.1.0/auxein/population/core.py` & `auxein-0.1.1/auxein/population/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,15 +133,27 @@
 
 def __add_to_population(population: Population, dimension: int, fitness_function: Fitness, dna_builder: DnaBuilder) -> None:
     individual = build_random_individual(dimension, dna_builder)
     fitness = fitness_function.fitness(individual)
     population.add(individual, fitness)
 
 
-def build_fixed_dimension_population(dimension: int, initial_size: int, fitness_function: Fitness, dna_builder: DnaBuilder) -> Population:
+def build_fixed_dimension_population(
+        dimension: int,
+        initial_size: int,
+        fitness_function: Fitness,
+        dna_builder: DnaBuilder
+) -> Population:
+    """Function to create a population of individuals with a fixed dimension.
+
+    :param int dimension: dimension of the individuals in the population.
+    :param int initial_size: Initial size of the population in terms of number of individuals.
+    :param Fitness fitness_function: Fitness function to evaluate the individuals.
+    :param DnaBuilder dna_builder: DnaBuilder to create the individuals.
+    """
     population = Population()
     for _ in range(0, initial_size):
         __add_to_population(population, dimension, fitness_function, dna_builder)
     return population
 
 
 def build_variable_dimension_population(initial_size: int, fitness_function: Fitness, dna_builder: DnaBuilder) -> Population:
```

### Comparing `auxein-0.1.0/auxein/population/dna_builders.py` & `auxein-0.1.1/auxein/population/dna_builders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Contains few classes to build random dna sequences.
 """
 from __future__ import absolute_import
 from abc import ABC, abstractmethod
-from typing import Tuple
+from typing import Tuple, List
 
 import numpy as np
 
 
 class DnaBuilder(ABC):
 
     @abstractmethod
@@ -53,7 +53,26 @@
     def get(self, dimension: int) -> np.ndarray:
         assert dimension > 0, 'dna dimension must be strictly positive.'
         return np.random.normal(
             self.mean,
             self.std,
             dimension
         )
+
+class CompositeDnaBuilder(RandomDnaBuilder):
+    """Composite dna builder. It builds various dna sequences with 
+    differnt underlyng distributons and concatenates them.
+    """
+
+    def __init__(self, builders: List[Tuple[DnaBuilder, int]]):
+        super().__init__(distribution='composite')
+        self.builders = builders
+
+    def get(self, dimension: int) -> np.ndarray:
+        assert dimension > 0, 'dna dimension must be strictly positive.'
+        assert dimension == sum(map(lambda item: item[1], self.builders)), 'dna dimension must be equal to the sum of the dimensions of the builders.'
+        
+        dna = []
+        for (builder, dimension) in self.builders:
+            dna.append(builder.get(dimension))
+
+        return np.concatenate(dna)
```

### Comparing `auxein-0.1.0/auxein/population/genotype.py` & `auxein-0.1.1/auxein/population/genotype.py`

 * *Files identical despite different names*

### Comparing `auxein-0.1.0/auxein/population/individual.py` & `auxein-0.1.1/auxein/population/individual.py`

 * *Files identical despite different names*

### Comparing `auxein-0.1.0/auxein/recombinations/core.py` & `auxein-0.1.1/auxein/recombinations/core.py`

 * *Files identical despite different names*

### Comparing `auxein-0.1.0/auxein/replacements/core.py` & `auxein-0.1.1/auxein/replacements/core.py`

 * *Files identical despite different names*

