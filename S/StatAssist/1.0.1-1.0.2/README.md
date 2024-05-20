# Comparing `tmp/StatAssist-1.0.1.tar.gz` & `tmp/StatAssist-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StatAssist-1.0.1.tar", last modified: Fri May 17 02:37:19 2024, max compression
+gzip compressed data, was "StatAssist-1.0.2.tar", last modified: Sun May 19 20:03:46 2024, max compression
```

## Comparing `StatAssist-1.0.1.tar` & `StatAssist-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 02:37:19.003521 StatAssist-1.0.1/
--rw-rw-rw-   0        0        0     2223 2024-05-17 02:37:19.003521 StatAssist-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1747 2024-05-14 23:57:05.000000 StatAssist-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 02:37:19.003521 StatAssist-1.0.1/StatAssist/
--rw-rw-rw-   0        0        0      286 2024-05-17 02:36:44.000000 StatAssist-1.0.1/StatAssist/__init__.py
--rw-rw-rw-   0        0        0     1769 2024-05-17 00:28:15.000000 StatAssist-1.0.1/StatAssist/algebra.py
--rw-rw-rw-   0        0        0    10327 2024-05-17 02:24:46.000000 StatAssist-1.0.1/StatAssist/stats.py
--rw-rw-rw-   0        0        0     5809 2024-05-17 02:19:35.000000 StatAssist-1.0.1/StatAssist/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 02:37:19.003521 StatAssist-1.0.1/StatAssist.egg-info/
--rw-rw-rw-   0        0        0     2223 2024-05-17 02:37:18.000000 StatAssist-1.0.1/StatAssist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-17 02:37:18.000000 StatAssist-1.0.1/StatAssist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 02:37:18.000000 StatAssist-1.0.1/StatAssist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-17 02:37:18.000000 StatAssist-1.0.1/StatAssist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 02:37:18.000000 StatAssist-1.0.1/StatAssist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 02:37:19.003521 StatAssist-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      788 2024-05-17 02:36:59.000000 StatAssist-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 20:03:46.478384 StatAssist-1.0.2/
+-rw-rw-rw-   0        0        0     2221 2024-05-19 20:03:46.478384 StatAssist-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1745 2024-05-19 20:02:54.000000 StatAssist-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 20:03:46.447029 StatAssist-1.0.2/StatAssist/
+-rw-rw-rw-   0        0        0      285 2024-05-19 20:02:20.000000 StatAssist-1.0.2/StatAssist/__init__.py
+-rw-rw-rw-   0        0        0     2358 2024-05-19 19:35:48.000000 StatAssist-1.0.2/StatAssist/algebra.py
+-rw-rw-rw-   0        0        0    11081 2024-05-19 20:01:59.000000 StatAssist-1.0.2/StatAssist/stats.py
+-rw-rw-rw-   0        0        0     7153 2024-05-19 19:46:17.000000 StatAssist-1.0.2/StatAssist/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 20:03:46.478384 StatAssist-1.0.2/StatAssist.egg-info/
+-rw-rw-rw-   0        0        0     2221 2024-05-19 20:03:45.000000 StatAssist-1.0.2/StatAssist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-19 20:03:45.000000 StatAssist-1.0.2/StatAssist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 20:03:45.000000 StatAssist-1.0.2/StatAssist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-19 20:03:45.000000 StatAssist-1.0.2/StatAssist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-19 20:03:45.000000 StatAssist-1.0.2/StatAssist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 20:03:46.478384 StatAssist-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      788 2024-05-19 20:01:59.000000 StatAssist-1.0.2/setup.py
```

### Comparing `StatAssist-1.0.1/PKG-INFO` & `StatAssist-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StatAssist
-Version: 1.0.1
+Version: 1.0.2
 Summary: Math tools for private or personal use.
 Author: Damion J. Quintanilla
 Author-email: djq314159@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,22 +18,22 @@
 StatAssist is a python library that provides statistical and mathematical functions as well as built-in algorithms such
 as integration and linear regression.
 
 ## Installation
 
 You can install StatAssist using pip:
 
-pip install StatAssist
+pip install StatAssist==1.0.2
 
 ## Usage
 
 Example 1:
 
 ```python
-from StatAssist.stats import statistics as stats
+from StatAssist import statistics_ as stats
 import matplotlib.pyplot as plt
 
 # Define data
 x_data = [0, 1, 2, 3, 4, 5]
 y_data = [0, 2, 4, 6, 8, 10]
 
 # Get statistical information
@@ -54,18 +54,18 @@
 plt.plot(x_data, y_reg, color='r')
 
 plt.show()
 ```
 Example 2:
 
 ```python
-from StatAssist.utils import algorithms
+from StatAssist import algorithms_
 import matplotlib.pyplot as plt
 
-lin_reg = algorithms.linear_regression
+lin_reg = algorithms_.linear_regression
 
 # Define data
 x_data = [0, 1, 2, 3, 4, 5]
 y_data = [0, 2, 4, 6, 8, 10]
 
 # Linear regression of data
 m, b = lin_reg([x_data, y_data])
```

### Comparing `StatAssist-1.0.1/README.md` & `StatAssist-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 StatAssist is a python library that provides statistical and mathematical functions as well as built-in algorithms such
 as integration and linear regression.
 
 ## Installation
 
 You can install StatAssist using pip:
 
-pip install StatAssist
+pip install StatAssist==1.0.2
 
 ## Usage
 
 Example 1:
 
 ```python
-from StatAssist.stats import statistics as stats
+from StatAssist import statistics_ as stats
 import matplotlib.pyplot as plt
 
 # Define data
 x_data = [0, 1, 2, 3, 4, 5]
 y_data = [0, 2, 4, 6, 8, 10]
 
 # Get statistical information
@@ -39,18 +39,18 @@
 plt.plot(x_data, y_reg, color='r')
 
 plt.show()
 ```
 Example 2:
 
 ```python
-from StatAssist.utils import algorithms
+from StatAssist import algorithms_
 import matplotlib.pyplot as plt
 
-lin_reg = algorithms.linear_regression
+lin_reg = algorithms_.linear_regression
 
 # Define data
 x_data = [0, 1, 2, 3, 4, 5]
 y_data = [0, 2, 4, 6, 8, 10]
 
 # Linear regression of data
 m, b = lin_reg([x_data, y_data])
```

### Comparing `StatAssist-1.0.1/StatAssist/algebra.py` & `StatAssist-1.0.2/StatAssist/algebra.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,23 @@
     @staticmethod
     def polynomial(x: float, coefficients: list) -> float:
         """
         Returns an evaluation of a polynomial.
         :param x: float
         :param coefficients: list, by increasing degree.
         :return: float
+
+        Example:
+
+        >>> f_x = funcs_.polynomial
+
+        >>> y = f_x(4, [0, 0, 1)
+        >>> print(y)
+
+        Returns: 16
         """
         P = 0
         degree = len(coefficients)
         for i in range(degree):
             P += coefficients[i] * pow(x, i)
 
         return P
@@ -20,39 +29,66 @@
     @staticmethod
     def exponential_equation_1(x: float, Args: list = [1, 0]) -> float:
         """
         Returns an evaluation of a basic exponential equation with base e.
         :param x: float, exponent of e.
         :param Args: list, [coefficient of e, constant]; Default: [1, 0].
         :return: float
+
+        Example:
+
+        >>> f_x = funcs_.exponential_equation_1
+
+        >>> y = f_x(0, [1, 0])
+        >>> print(y)
+
+        Returns: 2.71...
         """
         A = Args[0]
         C = Args[1]
         return A * math.exp(x) + C
 
     @staticmethod
     def exponential_equation_2(x: float, Args: list = [1, 2, 0]) -> float:
         """
         Returns an evaluation of a basic general exponential equation.
         :param x: float, exponent of base.
         :param Args: list, [coefficient of base, base, constant]; Default: [1, 2, 0].
         :return: float
+
+        Example:
+
+        >>> f_x = funcs_.exponential_equation_2
+
+        >>> y = f_x(2, [1, 2])
+        >>> print(y)
+
+        Returns: 4
         """
         A = Args[0]
         B = Args[1]
         C = Args[2]
         return A * pow(B, x) + C
 
     @staticmethod
     def log_equation(x: float, Args: list = [1, 0, 10]) -> float:
         """
         Returns an evaluation of a basic logarithmic equation.
         :param x: float
         :param Args: list, [coefficient of log_n(x), constant, base]; Default: [1, 0, 10].
         :return: float
+
+        Example:
+
+        >>> f_x = funcs_.log_equation
+
+        >>> y = f_x(100, [1, 0, 10])
+        >>> print(y)
+
+        Returns: 2
         """
         A = Args[0]
         C = Args[1]
         base = Args[2]
 
         return A * math.log(x, base) + C
```

### Comparing `StatAssist-1.0.1/StatAssist/stats.py` & `StatAssist-1.0.2/StatAssist/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,25 @@
 class STATS:
     @staticmethod
     def get_mean(*Data: list) -> list:
         """
         Returns the mean for multiple sets of data
         :param Data: list, contains a list of datasets.
         :return: list, Measure of the average of a dataset.
+
+        Example:
+
+        >>> x = [2, 4, 6]
+        >>> y = [4, 8, 12]
+        >>> z = [...]
+
+        >>> averages = statistics_.get_mean(x, y, ...)
+        >>> print(averages)
+
+        Returns: [4, 8, ...]
         """
         means = []
         for dataset in Data:
             temp = 0
             n = len(dataset)
             for datapoint in dataset:
                 temp += datapoint / n
@@ -26,14 +37,26 @@
     @staticmethod
     def get_variance(datasets: list, means: list) -> list:
         """
         Returns the variance for multiple datasets.
         :param datasets: list, contains a list of datasets.
         :param means: list, means for each dataset.
         :return: list, Measure of the 'spread' of a dataset.
+
+        Example:
+
+        >>> x = [2, 4, 6]
+        >>> y = [4, 8, 12]
+        >>> z = [...]
+        >>> averages = statistics_.get_mean(x, y, ...)
+
+        >>> Variances = statistics_.get_variance([x, y, ...], averages)
+        >>> print(Variances)
+
+        Returns: [0, 0, ...]
         """
         variances = []
 
         if len(datasets) == len(means):
             for i in range(len(means)):
                 n = len(datasets[i])
                 temp = 0
@@ -46,18 +69,29 @@
             return variances
 
         return ["len(datasets) != len(means)"]
 
     @staticmethod
     def get_covariance(datasets: list, means: list) -> float:
         """
-        Obtains the covariance for two datasets, x and y.
+        Obtains the covariance between two datasets, x and y.
         :param datasets: list, [dataset 'x', dataset 'x'].
         :param means: list, ['x' mean, 'y' mean].
         :return: float, covariance for datasets x and y.
+
+        Example:
+
+        >>> x = [2, 4, 6]
+        >>> y = [4, 8, 12]
+        >>> averages = statistics_.get_mean(x, y)
+
+        >>> cov = statistics_.get_covariance(x, y, averages)
+        >>> print(cov)
+
+        Returns: 0
         """
         covariance = 0
         mu_x = means[0]
         mu_y = means[1]
         x = datasets[0]
         y = datasets[1]
         n = len(datasets[0])
```

### Comparing `StatAssist-1.0.1/StatAssist/utils.py` & `StatAssist-1.0.2/StatAssist/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,28 @@
     @staticmethod
     def linear_regression(data: list, EPOCH=500) -> (float, float):
         """
         Hybrid linear regression algorithm employing statistical analysis and machine learning.
         :param data: list, [x_data, y_data]
         :param EPOCH: int, Epochs for machine learning algorithm.
         :return: (float, float), slope / y-intercept
+
+        Example:
+
+        >>> lin_reg = algorithms_.linear_regression
+
+        >>> x = [1, 2, 3]
+        >>> y = [1, 2, 3]
+
+        >>> data = [x, y]
+
+        >>> m, b = lin_reg(data)
+        >>> print(m, b)
+
+        Returns: 1, 0
         """
         averages = []
         for dataset in data:
             temp = 0
             n = len(dataset)
             for datapoint in dataset:
                 temp += datapoint / n
@@ -75,14 +89,26 @@
 
     @staticmethod
     def correlation_coefficient_matrix(data: list) -> list:
         """
         Correlation coefficient matrix
         :param data: list
         :return: list
+
+        Example:
+
+        >>> f_x = algorithms_.correlation_coefficient_matrix
+        >>> V_1 = [1, 1, 1]
+        >>> V_2 = [1, 1, 1]
+
+        >>> V_3 = f_x(V_1, V_2)
+        >>> print(V_3)
+
+        Returns: [[1, 1]
+                  [1, 1]]
         """
         n_cols = len(data)
         n = len(data[0])
         row = [0 for i in range(n_cols)]
         matrix = [row for i in range(n_cols)]
 
         for i in range(n_cols):
@@ -124,17 +150,29 @@
         return matrix
 
     @staticmethod
     def integral(func, func_args: list, interval: list) -> float:
         """
         Returns the area under a defined continuous function on an interval.
         :param func: callable function with x as first param.
-        :param func_args: list, arguments for callable function.
+        :param func_args: list, arguments for callable function that returns float.
         :param interval: interval on which the geometric area is to be calculated.
         :return: float
+
+        Example:
+
+        >>> def f_x(X):
+        >>>     return 2
+
+        >>> I = algorithms_.integral
+
+        >>> Area = I(f_x, [2, 6])
+        >>> print(Area)
+
+        Returns: 8
         """
         dx = 0.0001
         area = 0
         x = interval[0]
         while x < interval[1]:
             area += func(x, func_args) * dx
             x += dx
@@ -147,14 +185,25 @@
     def vector_add(vector_1: list, vector_2: list, add: bool = True) -> list:
         """
         Returns the sum or difference between two vectors.
         :param vector_1: list
         :param vector_2: list
         :param add: bool, Default: True
         :return: list
+
+        Example:
+
+        >>> f_x = vector_.vector_cross
+        >>> V_1 = [1, 2, 3]
+        >>> V_2 = [1, 1, 1]
+
+        >>> V_3 = f_x(V_1, V_2)
+        >>> print(V_3)
+
+        Returns: [2, 3, 4]
         """
         new_vector = []
         for element_x, element_y in vector_1, vector_2:
             if add:
                 new_vector.append(element_x + element_y)
             if not add:
                 new_vector.append(element_x - element_y)
@@ -164,28 +213,50 @@
     @staticmethod
     def vector_dot(vector_1: list, vector_2: list) -> float:
         """
         Returns the dot product between two vectors.
         :param vector_1: list
         :param vector_2: list
         :return: float
+
+        Example:
+
+        >>> f_x = vector_.vector_cross
+        >>> V_1 = [1, 2, 3]
+        >>> V_2 = [3, 2, 1]
+
+        >>> scalar = f_x(V_1, V_2)
+        >>> print(scalar)
+
+        Returns: 10
         """
         dot_sum = 0
         for element_x, element_y in vector_1, vector_2:
             dot_sum += element_x * element_y
 
         return dot_sum
 
     @staticmethod
     def vector_cross(vector_1: list, vector_2: list) -> list:
         """
         Returns the cross product between two 3-dimensional vectors.
         :param vector_1: list
         :param vector_2: list
         :return: list
+
+        Example:
+
+        >>> f_x = vector_.vector_cross
+        >>> V_1 = [1, 0, 0]
+        >>> V_2 = [0, 1, 0]
+
+        >>> V_3 = f_x(V_1, V_2)
+        >>> print(V_3)
+
+        Returns: [0, 0, 1]
         """
         a = vector_1[1] * vector_2[2] - vector_1[2] * vector_2[1]
         b = vector_1[0] * vector_2[2] - vector_1[2] * vector_2[0]
         c = vector_1[0] * vector_2[1] - vector_1[1] * vector_2[0]
 
         return [a, b, c]
```

### Comparing `StatAssist-1.0.1/StatAssist.egg-info/PKG-INFO` & `StatAssist-1.0.2/StatAssist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StatAssist
-Version: 1.0.1
+Version: 1.0.2
 Summary: Math tools for private or personal use.
 Author: Damion J. Quintanilla
 Author-email: djq314159@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,22 +18,22 @@
 StatAssist is a python library that provides statistical and mathematical functions as well as built-in algorithms such
 as integration and linear regression.
 
 ## Installation
 
 You can install StatAssist using pip:
 
-pip install StatAssist
+pip install StatAssist==1.0.2
 
 ## Usage
 
 Example 1:
 
 ```python
-from StatAssist.stats import statistics as stats
+from StatAssist import statistics_ as stats
 import matplotlib.pyplot as plt
 
 # Define data
 x_data = [0, 1, 2, 3, 4, 5]
 y_data = [0, 2, 4, 6, 8, 10]
 
 # Get statistical information
@@ -54,18 +54,18 @@
 plt.plot(x_data, y_reg, color='r')
 
 plt.show()
 ```
 Example 2:
 
 ```python
-from StatAssist.utils import algorithms
+from StatAssist import algorithms_
 import matplotlib.pyplot as plt
 
-lin_reg = algorithms.linear_regression
+lin_reg = algorithms_.linear_regression
 
 # Define data
 x_data = [0, 1, 2, 3, 4, 5]
 y_data = [0, 2, 4, 6, 8, 10]
 
 # Linear regression of data
 m, b = lin_reg([x_data, y_data])
```

### Comparing `StatAssist-1.0.1/setup.py` & `StatAssist-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="StatAssist",
-    version="1.0.1",
+    version="1.0.2",
     license='MIT',
     author="Damion J. Quintanilla",
     author_email="djq314159@gmail.com",
     description="Math tools for private or personal use.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

