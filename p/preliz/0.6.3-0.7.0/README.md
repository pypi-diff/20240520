# Comparing `tmp/preliz-0.6.3.tar.gz` & `tmp/preliz-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preliz-0.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "preliz-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `preliz-0.6.3.tar` & `preliz-0.7.0.tar`

### file list

```diff
@@ -1,104 +1,106 @@
--rw-r--r--   0        0        0    11357 2024-05-15 19:06:31.789746 preliz-0.6.3/LICENSE
--rw-r--r--   0        0        0     4324 2024-05-15 19:06:31.789746 preliz-0.6.3/README.md
--rw-r--r--   0        0        0      649 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/__init__.py
--rw-r--r--   0        0        0     2830 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/__init__.py
--rw-r--r--   0        0        0     6649 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/asymmetric_laplace.py
--rw-r--r--   0        0        0     4977 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/bernoulli.py
--rw-r--r--   0        0        0     7804 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/beta.py
--rw-r--r--   0        0        0     6302 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/betabinomial.py
--rw-r--r--   0        0        0     7169 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/betascaled.py
--rw-r--r--   0        0        0     5368 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/binomial.py
--rw-r--r--   0        0        0     4730 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/categorical.py
--rw-r--r--   0        0        0     4302 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/cauchy.py
--rw-r--r--   0        0        0     7502 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/censored.py
--rw-r--r--   0        0        0     4135 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/chi_squared.py
--rw-r--r--   0        0        0    21635 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/continuous_multivariate.py
--rw-r--r--   0        0        0     5071 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/discrete_uniform.py
--rw-r--r--   0        0        0     4942 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/discrete_weibull.py
--rw-r--r--   0        0        0    25870 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/distributions.py
--rw-r--r--   0        0        0     6516 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/distributions_multivariate.py
--rw-r--r--   0        0        0     5700 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/exgaussian.py
--rw-r--r--   0        0        0     4397 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/exponential.py
--rw-r--r--   0        0        0     5941 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/gamma.py
--rw-r--r--   0        0        0     3987 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/geometric.py
--rw-r--r--   0        0        0     4489 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/gumbel.py
--rw-r--r--   0        0        0     3991 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/halfcauchy.py
--rw-r--r--   0        0        0     4920 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/halfnormal.py
--rw-r--r--   0        0        0     8033 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/halfstudentt.py
--rw-r--r--   0        0        0     5386 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/hurdle.py
--rw-r--r--   0        0        0     6040 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/hypergeometric.py
--rw-r--r--   0        0        0     6527 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/inversegamma.py
--rw-r--r--   0        0        0     4899 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/kumaraswamy.py
--rw-r--r--   0        0        0     4061 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/laplace.py
--rw-r--r--   0        0        0     3938 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/logistic.py
--rw-r--r--   0        0        0     5742 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/logitnormal.py
--rw-r--r--   0        0        0     5093 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/lognormal.py
--rw-r--r--   0        0        0     4710 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/moyal.py
--rw-r--r--   0        0        0     6104 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/negativebinomial.py
--rw-r--r--   0        0        0     5017 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/normal.py
--rw-r--r--   0        0        0     5070 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/pareto.py
--rw-r--r--   0        0        0     4265 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/poisson.py
--rw-r--r--   0        0        0     5851 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/rice.py
--rw-r--r--   0        0        0     9518 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/skew_studentt.py
--rw-r--r--   0        0        0     6598 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/skewnormal.py
--rw-r--r--   0        0        0     7610 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/studentt.py
--rw-r--r--   0        0        0     6953 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/triangular.py
--rw-r--r--   0        0        0     5694 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/truncated.py
--rw-r--r--   0        0        0    14787 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/truncatednormal.py
--rw-r--r--   0        0        0     4692 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/uniform.py
--rw-r--r--   0        0        0     4987 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/vonmises.py
--rw-r--r--   0        0        0     5712 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/wald.py
--rw-r--r--   0        0        0     5152 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/weibull.py
--rw-r--r--   0        0        0     5601 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/zi_binomial.py
--rw-r--r--   0        0        0     7262 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/zi_negativebinomial.py
--rw-r--r--   0        0        0     5707 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/zi_poisson.py
--rw-r--r--   0        0        0       64 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/__init__.py
--rw-r--r--   0        0        0     4667 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/distribution_helper.py
--rw-r--r--   0        0        0    13819 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/optimization.py
--rw-r--r--   0        0        0     5596 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/parser.py
--rw-r--r--   0        0        0    19087 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/plot_helper.py
--rw-r--r--   0        0        0     9785 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/plot_helper_multivariate.py
--rw-r--r--   0        0        0     2028 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/predictive_helper.py
--rw-r--r--   0        0        0    12204 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/special.py
--rw-r--r--   0        0        0     6565 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/ppls/pymc_io.py
--rw-r--r--   0        0        0      145 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/predictive/__init__.py
--rw-r--r--   0        0        0    14606 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/predictive/ppa.py
--rw-r--r--   0        0        0     2251 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/predictive/ppe.py
--rw-r--r--   0        0        0     2160 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/predictive/predictive_explorer.py
--rw-r--r--   0        0        0     1946 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/tests/check_inside_notebook.ipynb
--rw-r--r--   0        0        0     1787 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/tests/plot_interactive.ipynb
--rw-r--r--   0        0        0   477854 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/ppa.ipynb
--rw-r--r--   0        0        0     2787 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/predictive_explorer.ipynb
--rw-r--r--   0        0        0     1439 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/quartile_int.ipynb
--rw-r--r--   0        0        0     1472 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/roulette.ipynb
--rw-r--r--   0        0        0      661 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_beta_mode.py
--rw-r--r--   0        0        0     1967 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_censored.py
--rw-r--r--   0        0        0      757 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_dirichlet_mode.py
--rw-r--r--   0        0        0     1144 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_discrete_weibull.py
--rw-r--r--   0        0        0     7521 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_distributions.py
--rw-r--r--   0        0        0      346 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_distributions_helper.py
--rw-r--r--   0        0        0      626 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_helper.py
--rw-r--r--   0        0        0     2292 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_hurdle.py
--rw-r--r--   0        0        0      338 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_internals.py
--rw-r--r--   0        0        0     6842 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_maxent.py
--rw-r--r--   0        0        0     3387 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_mle.py
--rw-r--r--   0        0        0      987 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_optimization.py
--rw-r--r--   0        0        0     6153 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_plots.py
--rw-r--r--   0        0        0       85 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_ppa.py
--rw-r--r--   0        0        0      117 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_predictive_explorer.py
--rw-r--r--   0        0        0     3557 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_quartile.py
--rw-r--r--   0        0        0      103 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_quartile_int.py
--rw-r--r--   0        0        0      910 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_roulette.py
--rw-r--r--   0        0        0    11197 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_scipy.py
--rw-r--r--   0        0        0     2287 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_special.py
--rw-r--r--   0        0        0     2568 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_truncated.py
--rw-r--r--   0        0        0      325 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/__init__.py
--rw-r--r--   0        0        0     2244 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/beta_mode.py
--rw-r--r--   0        0        0     2341 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/dirichlet_mode.py
--rw-r--r--   0        0        0     4125 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/maxent.py
--rw-r--r--   0        0        0     1654 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/mle.py
--rw-r--r--   0        0        0     3259 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/quartile.py
--rw-r--r--   0        0        0     6136 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/quartile_int.py
--rw-r--r--   0        0        0    12994 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/roulette.py
--rw-r--r--   0        0        0     1559 2024-05-15 19:06:31.853747 preliz-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 preliz-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-20 19:01:32.593948 preliz-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4324 2024-05-20 19:01:32.593948 preliz-0.7.0/README.md
+-rw-r--r--   0        0        0      649 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/__init__.py
+-rw-r--r--   0        0        0     2884 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/__init__.py
+-rw-r--r--   0        0        0     6649 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/asymmetric_laplace.py
+-rw-r--r--   0        0        0     4977 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/bernoulli.py
+-rw-r--r--   0        0        0     7804 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/beta.py
+-rw-r--r--   0        0        0     6302 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/betabinomial.py
+-rw-r--r--   0        0        0     7169 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/betascaled.py
+-rw-r--r--   0        0        0     5368 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/binomial.py
+-rw-r--r--   0        0        0     4730 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/categorical.py
+-rw-r--r--   0        0        0     4302 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/cauchy.py
+-rw-r--r--   0        0        0     7502 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/censored.py
+-rw-r--r--   0        0        0     4135 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/chi_squared.py
+-rw-r--r--   0        0        0    21635 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/continuous_multivariate.py
+-rw-r--r--   0        0        0     5071 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/discrete_uniform.py
+-rw-r--r--   0        0        0     4942 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/discrete_weibull.py
+-rw-r--r--   0        0        0    25916 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/distributions.py
+-rw-r--r--   0        0        0     6516 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/distributions_multivariate.py
+-rw-r--r--   0        0        0     5700 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/exgaussian.py
+-rw-r--r--   0        0        0     4397 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/exponential.py
+-rw-r--r--   0        0        0     5941 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/gamma.py
+-rw-r--r--   0        0        0     3987 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/geometric.py
+-rw-r--r--   0        0        0     4489 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/gumbel.py
+-rw-r--r--   0        0        0     3991 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/halfcauchy.py
+-rw-r--r--   0        0        0     4920 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/halfnormal.py
+-rw-r--r--   0        0        0     8033 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/halfstudentt.py
+-rw-r--r--   0        0        0     5386 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/hurdle.py
+-rw-r--r--   0        0        0     6040 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/hypergeometric.py
+-rw-r--r--   0        0        0     6527 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/inversegamma.py
+-rw-r--r--   0        0        0     4899 2024-05-20 19:01:32.649948 preliz-0.7.0/preliz/distributions/kumaraswamy.py
+-rw-r--r--   0        0        0     4061 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/laplace.py
+-rw-r--r--   0        0        0     3938 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/logistic.py
+-rw-r--r--   0        0        0     5742 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/logitnormal.py
+-rw-r--r--   0        0        0     5511 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/loglogistic.py
+-rw-r--r--   0        0        0     5093 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/lognormal.py
+-rw-r--r--   0        0        0     4710 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/moyal.py
+-rw-r--r--   0        0        0     6104 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/negativebinomial.py
+-rw-r--r--   0        0        0     5017 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/normal.py
+-rw-r--r--   0        0        0     5070 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/pareto.py
+-rw-r--r--   0        0        0     4265 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/poisson.py
+-rw-r--r--   0        0        0     5851 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/rice.py
+-rw-r--r--   0        0        0     9518 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/skew_studentt.py
+-rw-r--r--   0        0        0     6598 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/skewnormal.py
+-rw-r--r--   0        0        0     7610 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/studentt.py
+-rw-r--r--   0        0        0     6953 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/triangular.py
+-rw-r--r--   0        0        0     5694 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/truncated.py
+-rw-r--r--   0        0        0    14787 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/truncatednormal.py
+-rw-r--r--   0        0        0     4692 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/uniform.py
+-rw-r--r--   0        0        0     4987 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/vonmises.py
+-rw-r--r--   0        0        0     5712 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/wald.py
+-rw-r--r--   0        0        0     5152 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/weibull.py
+-rw-r--r--   0        0        0     5601 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/zi_binomial.py
+-rw-r--r--   0        0        0     7262 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/zi_negativebinomial.py
+-rw-r--r--   0        0        0     5707 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/distributions/zi_poisson.py
+-rw-r--r--   0        0        0       64 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/internal/__init__.py
+-rw-r--r--   0        0        0     4711 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/internal/distribution_helper.py
+-rw-r--r--   0        0        0    14276 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/internal/optimization.py
+-rw-r--r--   0        0        0     5596 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/internal/parser.py
+-rw-r--r--   0        0        0    19087 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/internal/plot_helper.py
+-rw-r--r--   0        0        0     9785 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/internal/plot_helper_multivariate.py
+-rw-r--r--   0        0        0     2028 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/internal/predictive_helper.py
+-rw-r--r--   0        0        0    12204 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/internal/special.py
+-rw-r--r--   0        0        0     6565 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/ppls/pymc_io.py
+-rw-r--r--   0        0        0      145 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/predictive/__init__.py
+-rw-r--r--   0        0        0    14606 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/predictive/ppa.py
+-rw-r--r--   0        0        0     2548 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/predictive/ppe.py
+-rw-r--r--   0        0        0     2160 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/predictive/predictive_explorer.py
+-rw-r--r--   0        0        0     1946 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/tests/check_inside_notebook.ipynb
+-rw-r--r--   0        0        0     1787 2024-05-20 19:01:32.653948 preliz-0.7.0/preliz/tests/plot_interactive.ipynb
+-rw-r--r--   0        0        0   477854 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/ppa.ipynb
+-rw-r--r--   0        0        0     2787 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/predictive_explorer.ipynb
+-rw-r--r--   0        0        0     1439 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/quartile_int.ipynb
+-rw-r--r--   0        0        0     1472 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/roulette.ipynb
+-rw-r--r--   0        0        0      661 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_beta_mode.py
+-rw-r--r--   0        0        0     1967 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_censored.py
+-rw-r--r--   0        0        0      757 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_dirichlet_mode.py
+-rw-r--r--   0        0        0     1144 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_discrete_weibull.py
+-rw-r--r--   0        0        0     7569 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_distributions.py
+-rw-r--r--   0        0        0      346 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_distributions_helper.py
+-rw-r--r--   0        0        0      626 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_helper.py
+-rw-r--r--   0        0        0     2292 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_hurdle.py
+-rw-r--r--   0        0        0      338 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_internals.py
+-rw-r--r--   0        0        0     6925 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_maxent.py
+-rw-r--r--   0        0        0     3435 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_mle.py
+-rw-r--r--   0        0        0      987 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_optimization.py
+-rw-r--r--   0        0        0     6153 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_plots.py
+-rw-r--r--   0        0        0       85 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_ppa.py
+-rw-r--r--   0        0        0     3772 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_ppe.py
+-rw-r--r--   0        0        0      117 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_predictive_explorer.py
+-rw-r--r--   0        0        0     3626 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_quartile.py
+-rw-r--r--   0        0        0      103 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_quartile_int.py
+-rw-r--r--   0        0        0      910 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_roulette.py
+-rw-r--r--   0        0        0    11307 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_scipy.py
+-rw-r--r--   0        0        0     2287 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_special.py
+-rw-r--r--   0        0        0     2568 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/tests/test_truncated.py
+-rw-r--r--   0        0        0      325 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/unidimensional/__init__.py
+-rw-r--r--   0        0        0     2244 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/unidimensional/beta_mode.py
+-rw-r--r--   0        0        0     2341 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/unidimensional/dirichlet_mode.py
+-rw-r--r--   0        0        0     4125 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/unidimensional/maxent.py
+-rw-r--r--   0        0        0     1654 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/unidimensional/mle.py
+-rw-r--r--   0        0        0     3259 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/unidimensional/quartile.py
+-rw-r--r--   0        0        0     6136 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/unidimensional/quartile_int.py
+-rw-r--r--   0        0        0    12994 2024-05-20 19:01:32.657948 preliz-0.7.0/preliz/unidimensional/roulette.py
+-rw-r--r--   0        0        0     1559 2024-05-20 19:01:32.657948 preliz-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 preliz-0.7.0/PKG-INFO
```

### Comparing `preliz-0.6.3/LICENSE` & `preliz-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/README.md` & `preliz-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/__init__.py` & `preliz-0.7.0/preliz/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .distributions import *
 from .predictive import *
 from .unidimensional import *
 
 
 __all__ = ["maxent", "mle", "ppa", "roulette", "quartile"]
 
-__version__ = "0.6.3"
+__version__ = "0.7.0"
 
 _log = logging.getLogger("preliz")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
```

### Comparing `preliz-0.6.3/preliz/distributions/__init__.py` & `preliz-0.7.0/preliz/distributions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .halfcauchy import HalfCauchy
 from .halfnormal import HalfNormal
 from .halfstudentt import HalfStudentT
 from .inversegamma import InverseGamma
 from .kumaraswamy import Kumaraswamy
 from .laplace import Laplace
 from .logistic import Logistic
+from .loglogistic import LogLogistic
 from .logitnormal import LogitNormal
 from .lognormal import LogNormal
 from .moyal import Moyal
 from .normal import Normal
 from .pareto import Pareto
 from .skew_studentt import SkewStudentT
 from .skewnormal import SkewNormal
@@ -68,14 +69,15 @@
     HalfCauchy,
     HalfNormal,
     HalfStudentT,
     InverseGamma,
     Kumaraswamy,
     Laplace,
     Logistic,
+    LogLogistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
```

### Comparing `preliz-0.6.3/preliz/distributions/asymmetric_laplace.py` & `preliz-0.7.0/preliz/distributions/asymmetric_laplace.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/bernoulli.py` & `preliz-0.7.0/preliz/distributions/bernoulli.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/beta.py` & `preliz-0.7.0/preliz/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/betabinomial.py` & `preliz-0.7.0/preliz/distributions/betabinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/betascaled.py` & `preliz-0.7.0/preliz/distributions/betascaled.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/binomial.py` & `preliz-0.7.0/preliz/distributions/binomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/categorical.py` & `preliz-0.7.0/preliz/distributions/categorical.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/cauchy.py` & `preliz-0.7.0/preliz/distributions/cauchy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/censored.py` & `preliz-0.7.0/preliz/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/chi_squared.py` & `preliz-0.7.0/preliz/distributions/chi_squared.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/continuous_multivariate.py` & `preliz-0.7.0/preliz/distributions/continuous_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/discrete_uniform.py` & `preliz-0.7.0/preliz/distributions/discrete_uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/discrete_weibull.py` & `preliz-0.7.0/preliz/distributions/discrete_weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/distributions.py` & `preliz-0.7.0/preliz/distributions/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,29 +597,31 @@
         support : str
             Available options are `full` or `restricted`. If `full` the values will cover the entire
             support of the distribution, if finite, or the quantiles 0.0001 or 0.9999, if infinite.
             If `restricted` the values will cover the quantile 0.0001 to 0.9999.
         n_points : int
             Number of values to return.
         """
+        half_n_points = int(n_points / 2)
+
         if isinstance(support, tuple):
-            return self.ppf(np.linspace(*self.cdf(support), n_points))
+            even = np.linspace(*support, n_points)
+            uneven = self.ppf(np.linspace(*self.cdf(support), n_points))
         else:
             lower_ep, upper_ep = self.support
 
             if not np.isfinite(lower_ep) or support == "restricted":
                 lower_ep = 0.0001
             if not np.isfinite(upper_ep) or support == "restricted":
                 upper_ep = 0.9999
 
-            half_n_points = int(n_points / 2)
             even = np.linspace(*self.ppf([lower_ep, upper_ep]), half_n_points)
             uneven = self.ppf(np.linspace(lower_ep, upper_ep, half_n_points))
 
-            return np.sort(np.concatenate([even, uneven]))
+        return np.sort(np.concatenate([even, uneven]))
 
     def _fit_mle(self, sample, **kwargs):
         """
         Estimate the parameters of the distribution from a sample by maximizing the likelihood.
 
         Parameters
         ----------
```

### Comparing `preliz-0.6.3/preliz/distributions/distributions_multivariate.py` & `preliz-0.7.0/preliz/distributions/distributions_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/exgaussian.py` & `preliz-0.7.0/preliz/distributions/exgaussian.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/exponential.py` & `preliz-0.7.0/preliz/distributions/exponential.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/gamma.py` & `preliz-0.7.0/preliz/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/geometric.py` & `preliz-0.7.0/preliz/distributions/geometric.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/gumbel.py` & `preliz-0.7.0/preliz/distributions/gumbel.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/halfcauchy.py` & `preliz-0.7.0/preliz/distributions/halfcauchy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/halfnormal.py` & `preliz-0.7.0/preliz/distributions/halfnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/halfstudentt.py` & `preliz-0.7.0/preliz/distributions/halfstudentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/hurdle.py` & `preliz-0.7.0/preliz/distributions/hurdle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/hypergeometric.py` & `preliz-0.7.0/preliz/distributions/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/inversegamma.py` & `preliz-0.7.0/preliz/distributions/inversegamma.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/kumaraswamy.py` & `preliz-0.7.0/preliz/distributions/kumaraswamy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/laplace.py` & `preliz-0.7.0/preliz/distributions/laplace.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/logistic.py` & `preliz-0.7.0/preliz/distributions/logistic.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/logitnormal.py` & `preliz-0.7.0/preliz/distributions/logitnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/lognormal.py` & `preliz-0.7.0/preliz/distributions/lognormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/moyal.py` & `preliz-0.7.0/preliz/distributions/moyal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/negativebinomial.py` & `preliz-0.7.0/preliz/distributions/negativebinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/normal.py` & `preliz-0.7.0/preliz/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/pareto.py` & `preliz-0.7.0/preliz/distributions/pareto.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/poisson.py` & `preliz-0.7.0/preliz/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/rice.py` & `preliz-0.7.0/preliz/distributions/rice.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/skew_studentt.py` & `preliz-0.7.0/preliz/distributions/skew_studentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/skewnormal.py` & `preliz-0.7.0/preliz/distributions/skewnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/studentt.py` & `preliz-0.7.0/preliz/distributions/studentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/triangular.py` & `preliz-0.7.0/preliz/distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/truncated.py` & `preliz-0.7.0/preliz/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/truncatednormal.py` & `preliz-0.7.0/preliz/distributions/truncatednormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/uniform.py` & `preliz-0.7.0/preliz/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/vonmises.py` & `preliz-0.7.0/preliz/distributions/vonmises.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/wald.py` & `preliz-0.7.0/preliz/distributions/wald.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/weibull.py` & `preliz-0.7.0/preliz/distributions/weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/zi_binomial.py` & `preliz-0.7.0/preliz/distributions/zi_binomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/zi_negativebinomial.py` & `preliz-0.7.0/preliz/distributions/zi_negativebinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/distributions/zi_poisson.py` & `preliz-0.7.0/preliz/distributions/zi_poisson.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/internal/distribution_helper.py` & `preliz-0.7.0/preliz/internal/distribution_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     "Gumbel": {"mu": 2.0, "beta": 5.0},
     "HalfCauchy": {"beta": 1.0},
     "HalfNormal": {"sigma": 1.0},
     "HalfStudentT": {"nu": 7.0, "sigma": 1.0},
     "InverseGamma": {"alpha": 3.0, "beta": 5.0},
     "Kumaraswamy": {"a": 2.0, "b": 2.0},
     "Laplace": {"mu": 0.0, "b": 1.0},
+    "LogLogistic": {"alpha": 1, "beta": 5},
     "Logistic": {"mu": 0.0, "s": 1},
     "LogNormal": {"mu": 0.0, "sigma": 0.5},
     "LogitNormal": {"mu": 0.0, "sigma": 0.5},
     "Moyal": {"mu": 0.0, "sigma": 1.0},
     "Normal": {"mu": 0.0, "sigma": 1.0},
     "Pareto": {"alpha": 5, "m": 2.0},
     "Rice": {"nu": 2.0, "sigma": 1.0},
```

### Comparing `preliz-0.6.3/preliz/internal/optimization.py` & `preliz-0.7.0/preliz/internal/optimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,20 +223,25 @@
 
         if prob > mass:
             tau_not -= 0.5 * tau_not
         else:
             tau_not += 0.5 * tau_not
 
 
-def optimize_pymc_model(fmodel, target, draws, prior, initial_guess, bounds, var_info, p_model):
+def optimize_pymc_model(
+    fmodel, target, draws, prior, initial_guess, bounds, var_info, p_model, rng
+):
     for _ in range(400):
         # can we sample systematically from these and less random?
         # This should be more flexible and allow other targets than just
         # a preliz distribution
-        obs = target.rvs(draws)
+        if isinstance(target, list):
+            obs = get_weighted_rvs(target, draws, rng)
+        else:
+            obs = target.rvs(draws, random_state=rng)
         result = minimize(
             fmodel,
             initial_guess,
             tol=0.001,
             method="SLSQP",
             args=(obs, var_info, p_model),
             bounds=bounds,
@@ -448,7 +453,15 @@
         left, right = left * factor, left
 
     right = max(factor, left)
     while func(right, dist, q) < 0.0:
         left, right = right, right * factor
 
     return brentq(func, left, right, args=(dist, q))
+
+
+def get_weighted_rvs(target, size, rng):
+    targets = [t[0] for t in target]
+    weights = [t[1] for t in target]
+    target_rnd_choices = np.random.choice(len(targets), size=size, p=weights)
+    samples = [target.rvs(size, random_state=rng) for target in targets]
+    return np.choose(target_rnd_choices, samples)
```

### Comparing `preliz-0.6.3/preliz/internal/parser.py` & `preliz-0.7.0/preliz/internal/parser.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/internal/plot_helper.py` & `preliz-0.7.0/preliz/internal/plot_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/internal/plot_helper_multivariate.py` & `preliz-0.7.0/preliz/internal/plot_helper_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/internal/predictive_helper.py` & `preliz-0.7.0/preliz/internal/predictive_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/internal/special.py` & `preliz-0.7.0/preliz/internal/special.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/ppls/pymc_io.py` & `preliz-0.7.0/preliz/ppls/pymc_io.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/predictive/ppa.py` & `preliz-0.7.0/preliz/predictive/ppa.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/predictive/ppe.py` & `preliz-0.7.0/preliz/predictive/ppe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 """Projective predictive elicitation."""
 
 import logging
+import numpy as np
 
 from preliz.internal.optimization import optimize_pymc_model
 from preliz.ppls.pymc_io import (
     get_model_information,
     get_guess,
     compile_logp,
     backfitting,
     write_pymc_string,
 )
 
 
 _log = logging.getLogger("preliz")
 
 
-def ppe(model, target):
+def ppe(model, target, seed=0):
     """
     Projective Predictive Elicitation.
 
     This is an experimental method under development, use with caution.
     Most likely thing will break.
 
     Parameters
     ----------
     model : a probabilistic model
         Currently it only works with PyMC model. More PPls coming soon.
-    target : a Preliz distribution
-        This represent the prior predictive distribution **previously** elicited from the user,
+    target : a Preliz distribution or list
+        Instance of a PreliZ distribution or a list of tuples where each tuple contains a PreliZ
+        distribution and a weight.
+        This represents the prior predictive distribution **previously** elicited from the user,
         possibly using other Preliz's methods to obtain this distribution, such as maxent,
         roulette, quartile, etc.
         This should represent the domain-knowledge of the user and not any observed dataset.
-        Currently only works with a Preliz distributions. In the future we should support mixture of
-        distributions (mixture of "experts"), and maybe other options.
+    seed : int
+        A seed to initialize the Random Generator. Default is 0.
 
     Returns
     -------
     prior : a dictionary
         Prior samples approximating the prior distribution that will induce
         a prior predictive distribution close to ``target``.
+    new_priors : a dictionary
+        PreliZ Distributions approximating the prior distribution inducing a
+        prior predictive distribution close to ``target``.
     pymc_string : a string
         This is the PyMC model string with the new priors.
         Computed by taking the "prior samples" and fit it into the model's prior families
         using MLE.
     """
     _log.info(""""This is an experimental method under development, use with caution.""")
 
     # Get information from PyMC model
+    rng = np.random.default_rng(seed)
     bounds, prior, p_model, var_info, var_info2, draws, free_rvs = get_model_information(model)
     # Initial point for optimization
     guess = get_guess(model, free_rvs)
     # compile PyMC model
     fmodel = compile_logp(model)
     # find prior that induce a prior predictive distribution close to target
-    prior = optimize_pymc_model(fmodel, target, draws, prior, guess, bounds, var_info, p_model)
+    prior = optimize_pymc_model(fmodel, target, draws, prior, guess, bounds, var_info, p_model, rng)
     # Fit the prior into the model's prior
     # So we can write it as a PyMC model
     new_priors = backfitting(prior, p_model, var_info2)
 
-    return prior, write_pymc_string(new_priors, var_info2)
+    return prior, new_priors, write_pymc_string(new_priors, var_info2)
```

### Comparing `preliz-0.6.3/preliz/predictive/predictive_explorer.py` & `preliz-0.7.0/preliz/predictive/predictive_explorer.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/check_inside_notebook.ipynb` & `preliz-0.7.0/preliz/tests/check_inside_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/plot_interactive.ipynb` & `preliz-0.7.0/preliz/tests/plot_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/ppa.ipynb` & `preliz-0.7.0/preliz/tests/ppa.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/predictive_explorer.ipynb` & `preliz-0.7.0/preliz/tests/predictive_explorer.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/quartile_int.ipynb` & `preliz-0.7.0/preliz/tests/quartile_int.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/roulette.ipynb` & `preliz-0.7.0/preliz/tests/roulette.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_beta_mode.py` & `preliz-0.7.0/preliz/tests/test_beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_censored.py` & `preliz-0.7.0/preliz/tests/test_censored.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_dirichlet_mode.py` & `preliz-0.7.0/preliz/tests/test_dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_discrete_weibull.py` & `preliz-0.7.0/preliz/tests/test_discrete_weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_distributions.py` & `preliz-0.7.0/preliz/tests/test_distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     HalfCauchy,
     HalfNormal,
     HalfStudentT,
     InverseGamma,
     Kumaraswamy,
     Laplace,
     Logistic,
+    LogLogistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
@@ -73,14 +74,15 @@
         (Gumbel, (1, 2)),
         (HalfNormal, (1,)),
         (HalfStudentT, (100, 1)),
         (InverseGamma, (3, 1)),
         (Kumaraswamy, (5, 2)),
         (Laplace, (0, 1)),
         (Logistic, (1, 2)),
+        (LogLogistic, (1, 5)),
         (LogNormal, (0, 0.5)),
         (LogitNormal, (0, 0.5)),
         (Moyal, (1, 2)),
         (Normal, (0, 1)),
         (Pareto, (5, 1)),
         (Rice, (4, 1)),
         (SkewNormal, (0, 1, 0)),
```

### Comparing `preliz-0.6.3/preliz/tests/test_helper.py` & `preliz-0.7.0/preliz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_hurdle.py` & `preliz-0.7.0/preliz/tests/test_hurdle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_maxent.py` & `preliz-0.7.0/preliz/tests/test_maxent.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     HalfCauchy,
     HalfNormal,
     HalfStudentT,
     InverseGamma,
     Kumaraswamy,
     Laplace,
     Logistic,
+    LogLogistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
@@ -88,14 +89,15 @@
         (HalfStudentT(), 1, 10, 0.7, (0, np.inf), (99.997, 7.697)),
         (HalfStudentT(nu=7), 1, 10, 0.7, (0, np.inf), (2.541)),
         (InverseGamma(), 0, 1, 0.99, (0, np.inf), (8.889, 3.439)),
         (Kumaraswamy(), 0.1, 0.6, 0.9, (0, 1), (2.311, 7.495)),
         (Laplace(), -1, 1, 0.9, (-np.inf, np.inf), (0, 0.435)),
         (Laplace(mu=0.5), -1, 1, 0.9, (-np.inf, np.inf), (0.303)),
         (Logistic(), -1, 1, 0.5, (-np.inf, np.inf), (0, 0.91)),
+        (LogLogistic(), 2, 10, 0.9, (0, np.inf), (5.543, 4.047)),
         (LogNormal(), 1, 4, 0.5, (0, np.inf), (1.216, 0.859)),
         (LogNormal(mu=1), 1, 4, 0.5, (0, np.inf), (0.978)),
         (LogitNormal(), 0.3, 0.8, 0.9, (0, 1), (0.213, 0.676)),
         (LogitNormal(mu=0.7), 0.3, 0.8, 0.9, (0, 1), (0.531)),
         (Moyal(), 0, 10, 0.9, (-np.inf, np.inf), (2.935, 1.6)),
         (Moyal(mu=4), 0, 10, 0.9, (-np.inf, np.inf), (1.445)),
         (Normal(), -1, 1, 0.683, (-np.inf, np.inf), (0, 1)),
```

### Comparing `preliz-0.6.3/preliz/tests/test_mle.py` & `preliz-0.7.0/preliz/tests/test_mle.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     HalfCauchy,
     HalfNormal,
     HalfStudentT,
     InverseGamma,
     Kumaraswamy,
     Laplace,
     Logistic,
+    LogLogistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
@@ -67,14 +68,15 @@
         (HalfNormal, (1,)),
         (HalfStudentT, (5, 1)),
         (HalfNormal, (2,)),
         (InverseGamma, (3, 5)),
         (Kumaraswamy, (2, 3)),
         (Laplace, (0, 2)),
         (Logistic, (0, 1)),
+        (LogLogistic, (1, 5)),
         (LogNormal, (0, 1)),
         (LogitNormal, (0, 0.5)),
         (Moyal, (0, 2)),
         (Normal, (0, 1)),
         (Pareto, (5, 1)),
         (Rice, (0, 2)),
         (SkewNormal, (0, 1, -6)),
@@ -104,24 +106,24 @@
                 4.2,
             ),
         ),
     ],
 )
 def test_auto_recover(distribution, params):
     for _ in range(10):
-        sample = distribution(*params).rvs(10_000)
+        sample = distribution(*params).rvs(20_000)
         dist = distribution()
         try:
             if dist.__class__.__name__ in [
                 "BetaScaled",
                 "TruncatedNormal",
             ]:
                 tol = 1
             else:
-                tol = 0.1
+                tol = 0.5
             pz.mle([dist], sample)
             assert_allclose(dist.params, params, atol=tol)
             break
         except AssertionError:
             pass
     else:
         raise AssertionError(f"Test failed after 10 attempts.{dist.params}")
```

### Comparing `preliz-0.6.3/preliz/tests/test_optimization.py` & `preliz-0.7.0/preliz/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_plots.py` & `preliz-0.7.0/preliz/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_quartile.py` & `preliz-0.7.0/preliz/tests/test_quartile.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     HalfCauchy,
     HalfNormal,
     HalfStudentT,
     InverseGamma,
     Kumaraswamy,
     Laplace,
     Logistic,
+    LogLogistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewStudentT,
@@ -63,14 +64,15 @@
         (HalfCauchy(), 0.5, 1, 3, (1.105)),
         (HalfNormal(), 0.5, 1, 2, (1.613)),
         (HalfStudentT(), 0.5, 1, 2, (2.393, 1.311)),
         (InverseGamma(), 0.2, 0.3, 0.4, (3.881, 1.019)),
         (Kumaraswamy(), 0.2, 0.3, 0.4, (2.199, 9.598)),
         (Laplace(), -1, 0, 1, (0, 1.442)),
         (Logistic(), -1, 0, 1, (0, 0.910)),
+        (LogLogistic(), 1, 1.5, 2, (1.454, 3.143)),
         (LogNormal(), 0.5, 1, 2, (0, 1.027)),
         (LogitNormal(), 0.3, 0.45, 0.6, (-0.212, 0.929)),
         (Moyal(), 0.5, 1, 2, (0.620, 0.567)),
         (Normal(), -1, 0, 1, (0, 1.482)),
         (Pareto(), 0.5, 1, 4, (0.541, 0.289)),
         (Rice(), 2, 4, 6, (0, 3.395)),
         (SkewStudentT(), 2, 4, 6, (4, 2.648, 1.663, 1.663)),
```

### Comparing `preliz-0.6.3/preliz/tests/test_roulette.py` & `preliz-0.7.0/preliz/tests/test_roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_scipy.py` & `preliz-0.7.0/preliz/tests/test_scipy.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     HalfCauchy,
     HalfNormal,
     HalfStudentT,
     InverseGamma,
     Kumaraswamy,
     Laplace,
     Logistic,
+    LogLogistic,
     LogitNormal,
     LogNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
@@ -84,14 +85,15 @@
             stats.halfnorm,
             {"nu": 100, "sigma": 2},
             {"loc": 0, "scale": 2},
         ),  # not in scipy
         (InverseGamma, stats.invgamma, {"alpha": 5, "beta": 2}, {"a": 5, "scale": 2}),
         (Kumaraswamy, stats.beta, {"a": 1, "b": 5}, {"a": 1, "b": 5}),  # not in scipy
         (Laplace, stats.laplace, {"mu": 2.5, "b": 4}, {"loc": 2.5, "scale": 4}),
+        (LogLogistic, stats.fisk, {"alpha": 1, "beta": 8}, {"c": 8}),
         (Logistic, stats.logistic, {"mu": 2.5, "s": 4}, {"loc": 2.5, "scale": 4}),
         (LogNormal, stats.lognorm, {"mu": 0, "sigma": 2}, {"s": 2, "scale": 1}),
         (LogitNormal, stats.beta, {"mu": 0, "sigma": 0.2}, {"a": 50.5, "b": 50.5}),  # not in scipy
         (Moyal, stats.moyal, {"mu": 1, "sigma": 2}, {"loc": 1, "scale": 2}),
         (Normal, stats.norm, {"mu": 0, "sigma": 2}, {"loc": 0, "scale": 2}),
         (Pareto, stats.pareto, {"m": 1, "alpha": 4.5}, {"b": 4.5}),
         (
@@ -277,14 +279,15 @@
     elif preliz_name in ["TruncatedNormal"]:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf, decimal=6)
     else:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf)
 
     if preliz_dist.__class__.__name__ not in [
         "HalfStudentT",
+        "LogLogistic",
         "Rice",
         "VonMises",
         "ZeroInflatedBinomial",
         "ZeroInflatedNegativeBinomial",
         "ZeroInflatedPoisson",
     ]:
         actual_moments = preliz_dist.moments("mvsk")
```

### Comparing `preliz-0.6.3/preliz/tests/test_special.py` & `preliz-0.7.0/preliz/tests/test_special.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/tests/test_truncated.py` & `preliz-0.7.0/preliz/tests/test_truncated.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/unidimensional/beta_mode.py` & `preliz-0.7.0/preliz/unidimensional/beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/unidimensional/dirichlet_mode.py` & `preliz-0.7.0/preliz/unidimensional/dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/unidimensional/maxent.py` & `preliz-0.7.0/preliz/unidimensional/maxent.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/unidimensional/mle.py` & `preliz-0.7.0/preliz/unidimensional/mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/unidimensional/quartile.py` & `preliz-0.7.0/preliz/unidimensional/quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/unidimensional/quartile_int.py` & `preliz-0.7.0/preliz/unidimensional/quartile_int.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/preliz/unidimensional/roulette.py` & `preliz-0.7.0/preliz/unidimensional/roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/pyproject.toml` & `preliz-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `preliz-0.6.3/PKG-INFO` & `preliz-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preliz
-Version: 0.6.3
+Version: 0.7.0
 Summary: The place for all your prior elicitation needs.
 Author-email: ArviZ team <arviz.devs@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
```

