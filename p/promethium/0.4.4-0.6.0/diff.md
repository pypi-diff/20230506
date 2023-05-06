# Comparing `tmp/promethium-0.4.4.tar.gz` & `tmp/promethium-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promethium-0.4.4.tar", max compression
+gzip compressed data, was "promethium-0.6.0.tar", max compression
```

## Comparing `promethium-0.4.4.tar` & `promethium-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-05-05 23:27:59.243710 promethium-0.4.4/LICENSE
--rw-r--r--   0        0        0     7397 2023-05-05 23:27:59.243710 promethium-0.4.4/README.md
--rw-r--r--   0        0        0      524 2023-05-05 23:27:59.243710 promethium-0.4.4/promethium/__init__.py
--rw-r--r--   0        0        0     2124 2023-05-05 23:28:27.013712 promethium-0.4.4/promethium/distributions_binomial.py
--rw-r--r--   0        0        0     1702 2023-05-05 23:27:59.243710 promethium-0.4.4/promethium/distributions_geometric.py
--rw-r--r--   0        0        0     1825 2023-05-05 23:27:59.243710 promethium-0.4.4/promethium/distributions_normal.py
--rw-r--r--   0        0        0     1803 2023-05-05 23:28:27.013712 promethium-0.4.4/promethium/distributions_poisson.py
--rw-r--r--   0        0        0      561 2023-05-05 23:34:25.213698 promethium-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     7872 1970-01-01 00:00:00.000000 promethium-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-05 23:27:59.243710 promethium-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7254 2023-05-06 00:25:02.063597 promethium-0.6.0/README.md
+-rw-r--r--   0        0        0      666 2023-05-06 00:06:09.703635 promethium-0.6.0/promethium/__init__.py
+-rw-r--r--   0        0        0     2124 2023-05-06 00:03:13.003675 promethium-0.6.0/promethium/distributions/binomial.py
+-rw-r--r--   0        0        0      994 2023-05-06 00:05:50.173639 promethium-0.6.0/promethium/distributions/chi2.py
+-rw-r--r--   0        0        0     1702 2023-05-06 00:03:29.723645 promethium-0.6.0/promethium/distributions/geometric.py
+-rw-r--r--   0        0        0     1825 2023-05-06 00:03:41.353637 promethium-0.6.0/promethium/distributions/normal.py
+-rw-r--r--   0        0        0     1803 2023-05-06 00:03:54.403634 promethium-0.6.0/promethium/distributions/poisson.py
+-rw-r--r--   0        0        0    17382 2023-05-06 00:05:08.733638 promethium-0.6.0/promethium/special/gamma.py
+-rw-r--r--   0        0        0      538 2023-05-06 00:09:15.853633 promethium-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7706 1970-01-01 00:00:00.000000 promethium-0.6.0/PKG-INFO
```

### Comparing `promethium-0.4.4/LICENSE` & `promethium-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promethium-0.4.4/README.md` & `promethium-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,22 @@
-# Python Probabilities 🐍
-*Library for accurate statistical calculations using Python.*
+Metadata-Version: 2.1
+Name: promethium
+Version: 0.6.0
+Summary: Statistical Distributions in Python.
+Author: berkay-yalin
+Author-email: 66202981+berkay-yalin@users.noreply.github.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+# Promethium 🐍
+*Statistical Distributions in Python.*
 
 - [Binomial Distributions](#binomial-distributions)
   - [Probability mass function](#probability-mass-function)
   - [Cumulative distribution function](#cumulative-distribution-function)
   - [Inverse cumulative distribution function](#inverse-cumulative-distribution-function)
 - [Normal Distributions](#normal-distributions)
   - [Probability density function](#probability-density-function)
@@ -25,30 +38,30 @@
 ```
 For the random variable `X` with the binomial distribution `B(n, p)`, calculate the **probability mass function**.\
 Where `r` is the number of successes, `n` is the number of trials, and `p` is the probability of success.
 
 **Example**\
 To calculate `P(X=7)` for the binomial distribution `X~B(11, 0.33)`:
 ```python
->>> from python_probabilities import BinomialPD
+>>> from promethium import BinomialPD
 >>> BinomialPD(7, 11, 0.33)
 0.029656979029412885
 ```
 ---
 ### Cumulative distribution function
 ```python
 BinomialCD(r, n, p)
 ```
 For the random variable `X` with the binomial distribution `B(n, p)`, calculate the **cumulative distribution function**.\
 Where `r` is the number of successes, `n` is the number of trials, and `p` is the probability of success.
 
 **Example**\
 To calculate `P(X≤7)` for the binomial distribution `X~B(11, 0.33)`:
 ```python
->>> from python_probabilities import BinomialCD
+>>> from promethium import BinomialCD
 >>> BinomialCD(7, 11, 0.33)
 0.9912362670526581
 ```
 ---
 ### Inverse cumulative distribution function
 ```python
 InvBinomialCD(q, n, p)
@@ -57,15 +70,15 @@
 Where `q` is the cumulative probability, `n` is the number of trials, and `p` is the probability of success.
 
 `InvBinomialCD(q, n, p)` returns the smallest integer `x` such that `BinomialCD(x, n, p)` is greater than or equal to `q`.
 
 **Example**\
 To calculate the corresponding value for `r` (the number of successes) given the value for `q` (the cumulative probability):
 ```python
->>> from python_probabilities import BinomialCD, InvBinomialCD
+>>> from promethium import BinomialCD, InvBinomialCD
 >>> InvBinomialCD(0.9912362670526581, 11, 0.333)
 7
 >>> BinomialCD(7, 11, 0.333)
 0.9912362670526581
 ```
 
 ## Normal Distributions
@@ -84,15 +97,15 @@
 ```
 Cumulative distribution function for the normal distribution `X~N(µ, σ)`.\
 Where `µ` is the mean, and `σ` is the standard deviation.
 
 **Example**\
 To calculate `P(X≤0.891)` for the normal distribution `X~N(0.734, 0.114)`:
 ```python
->>> from python_probabilities import NormalCD
+>>> from promethium import NormalCD
 >>> NormalCD(0.891, 0.734, 0.114)
 0.9157737045522477
 ```
 
 ---
 
 ### Inverse cumulative distribution function
@@ -103,15 +116,15 @@
 Where `µ` is the mean, and `σ` is the standard deviation.
 
 `InvNormalCD(y, µ, σ)` returns the smallest integer `x` such that `NormalCD(x, µ, σ)` is greater than or equal to `y`.
 
 **Example**\
 To calculate the corresponding value for `x` given the value for `y`:
 ```python
->>> from python_probabilities import NormalCD, InvNormalCD
+>>> from promethium import NormalCD, InvNormalCD
 >>> InvNormalCD(0.9157737045522477, 0.734, 0.114)
 0.891
 >>> NormalCD(0.891, 0.734, 0.114)
 0.9157737045522477
 ```
 
 ## Poisson Distributions
@@ -121,30 +134,30 @@
 ```
 For the random variable `X` with the poisson distribution `Po(m)`, calculate the **probability mass function**.\
 Where `r` is the number of occurrences, and `m` is the mean rate of occurrence.
 
 **Example**\
 To calculate `P(X=7)` for the poisson distribution `X~Po(11.556)`:
 ```python
->>> from python_probabilities import PoissonPD
+>>> from promethium import PoissonPD
 >>> PoissonPD(11, 23.445)
 0.0019380401123575617
 ```
 ---
 ### Cumulative distribution function
 ```python
 PoissonCD(r, m)
 ```
 For the random variable `X` with the poisson distribution `Po(m)`, calculate the **cumulative distribution function**.\
 Where `r` is the number of occurrences, and `m` is the mean rate of occurrence.
 
 **Example**\
 To calculate `P(X≤7)` for the poisson distribution `X~Po(11.556)`:
 ```python
->>> from python_probabilities import PoissonCD
+>>> from promethium import PoissonCD
 >>> PoissonCD(11, 23.445)
 0.0034549033698374467
 ```
 ---
 ### Inverse cumulative distribution
 ```python
 InvPoissonCD(q, m)
@@ -153,15 +166,15 @@
 Where `q` is the cumulative probability, and `m` is the mean rate of occurrence.
 
 `InvPoissonCD(q, m)` returns the smallest integer `x` such that `PoissonCD(x, m)` is greater than or equal to `q`.
 
 **Example**\
 To calculate the corresponding value for `r` (number of occurrences) given the values for `q` (cumulative probability):
 ```python
->>> from python_probabilities import PoissonCD, InvPoissonCD
+>>> from promethium import PoissonCD, InvPoissonCD
 >>> InvPoissonCD(0.0034549033698374467, 23.445)
 11
 >>> PoissonCD(11, 23.445)
 0.0034549033698374467
 ```
 
 ## Geometric Distributions
@@ -171,15 +184,15 @@
 ```
 Probability mass function for the geometric distribution `X~G(p)`.\
 Where `x` is the number of trials before the first success, and `p` is the probability of success.
 
 **Example**\
 To calculate `P(X=3)` for the geometric distribution `X~G(0.491)`:
 ```python
->>> from python_probabilities import GeometricPD
+>>> from promethium import GeometricPD
 >>> GeometricPD(3, 0.491)
 0.127208771
 ```
 ---
 
 ### Cumulative distribution function
 ```python
@@ -187,15 +200,15 @@
 ```
 Cumulative distribution function for the geometric distribution `X~G(p)`.\
 Where `x` is the number of trials before the first success, and `p` is the probability of success.
 
 **Example**\
 To calculate `P(X≤3)` for the geometric distribution `X~G(0.491)`:
 ```python
->>> from python_probabilities import GeometricCD
+>>> from promethium import GeometricCD
 >>> GeometricCD(3, 0.491)
 0.868127771
 ```
 ---
 
 ### Inverse cumulative distribution function
 ```python
@@ -205,14 +218,15 @@
 Where `x` is the number of trials before the first success, and `p` is the probability of success.
 
 `InvGeometricCD(area, p)` returns the smallest integer `x` such that `GeometricCD(x, p)` is greater than or equal to `area`.
 
 **Example**\
 To calculate the corresponding value for `x` given the value for `area`:
 ```python
->>> from python_probabilities import GeometricCD, InvGeometricCD
+>>> from promethium import GeometricCD, InvGeometricCD
 >>> InvGeometricCD(0.868, 0.491)
 3
 >> GeometricCD(3, 0.491)
 0.868127771
 ```
 
+
```

### Comparing `promethium-0.4.4/promethium/__init__.py` & `promethium-0.6.0/promethium/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from .distributions_binomial import BinomialPD, BinomialCD, InvBinomialCD
-from .distributions_poisson import PoissonPD, PoissonCD, InvPoissonCD
-from .distributions_normal import NormalPD, NormalCD, InvNormalCD
-from .distributions_geometric import GeometricPD, GeometricCD, InvGeometricCD
+from .distributions.binomial import BinomialPD, BinomialCD, InvBinomialCD
+from .distributions.poisson import PoissonPD, PoissonCD, InvPoissonCD
+from .distributions.normal import NormalPD, NormalCD, InvNormalCD
+from .distributions.geometric import GeometricPD, GeometricCD, InvGeometricCD
+from .distributions.chi2 import ChiSquaredPD, ChiSquaredCD#, InvChiSquaredCD
 
 __all__ = (
     'BinomialPD',
     'BinomialCD',
     'InvBinomialCD',
     'PoissonPD',
     'PoissonCD',
     'InvPoissonCD',
     'NormalPD',
     'NormalCD',
     'InvNormalCD',
     'GeometricPD',
     'GeometricCD',
-    'InvGeometricCD'
+    'InvGeometricCD',
+    'ChiSquaredPD',
+    'ChiSquaredCD',
+    # 'InvChiSquaredCD'
 )
```

### Comparing `promethium-0.4.4/promethium/distributions_binomial.py` & `promethium-0.6.0/promethium/distributions/binomial.py`

 * *Files identical despite different names*

### Comparing `promethium-0.4.4/promethium/distributions_geometric.py` & `promethium-0.6.0/promethium/distributions/geometric.py`

 * *Files identical despite different names*

### Comparing `promethium-0.4.4/promethium/distributions_normal.py` & `promethium-0.6.0/promethium/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `promethium-0.4.4/promethium/distributions_poisson.py` & `promethium-0.6.0/promethium/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `promethium-0.4.4/pyproject.toml` & `promethium-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "promethium"
-version = "0.4.4"
-description = "Library for accurate statistical calculations using Python."
+version = "0.6.0"
+description = "Statistical Distributions in Python."
 authors = ["berkay-yalin <66202981+berkay-yalin@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "promethium"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `promethium-0.4.4/PKG-INFO` & `promethium-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,9 @@
-Metadata-Version: 2.1
-Name: promethium
-Version: 0.4.4
-Summary: Library for accurate statistical calculations using Python.
-Author: berkay-yalin
-Author-email: 66202981+berkay-yalin@users.noreply.github.com
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
-# Python Probabilities 🐍
-*Library for accurate statistical calculations using Python.*
+# Promethium 🐍
+*Statistical Distributions in Python.*
 
 - [Binomial Distributions](#binomial-distributions)
   - [Probability mass function](#probability-mass-function)
   - [Cumulative distribution function](#cumulative-distribution-function)
   - [Inverse cumulative distribution function](#inverse-cumulative-distribution-function)
 - [Normal Distributions](#normal-distributions)
   - [Probability density function](#probability-density-function)
@@ -38,30 +25,30 @@
 ```
 For the random variable `X` with the binomial distribution `B(n, p)`, calculate the **probability mass function**.\
 Where `r` is the number of successes, `n` is the number of trials, and `p` is the probability of success.
 
 **Example**\
 To calculate `P(X=7)` for the binomial distribution `X~B(11, 0.33)`:
 ```python
->>> from python_probabilities import BinomialPD
+>>> from promethium import BinomialPD
 >>> BinomialPD(7, 11, 0.33)
 0.029656979029412885
 ```
 ---
 ### Cumulative distribution function
 ```python
 BinomialCD(r, n, p)
 ```
 For the random variable `X` with the binomial distribution `B(n, p)`, calculate the **cumulative distribution function**.\
 Where `r` is the number of successes, `n` is the number of trials, and `p` is the probability of success.
 
 **Example**\
 To calculate `P(X≤7)` for the binomial distribution `X~B(11, 0.33)`:
 ```python
->>> from python_probabilities import BinomialCD
+>>> from promethium import BinomialCD
 >>> BinomialCD(7, 11, 0.33)
 0.9912362670526581
 ```
 ---
 ### Inverse cumulative distribution function
 ```python
 InvBinomialCD(q, n, p)
@@ -70,15 +57,15 @@
 Where `q` is the cumulative probability, `n` is the number of trials, and `p` is the probability of success.
 
 `InvBinomialCD(q, n, p)` returns the smallest integer `x` such that `BinomialCD(x, n, p)` is greater than or equal to `q`.
 
 **Example**\
 To calculate the corresponding value for `r` (the number of successes) given the value for `q` (the cumulative probability):
 ```python
->>> from python_probabilities import BinomialCD, InvBinomialCD
+>>> from promethium import BinomialCD, InvBinomialCD
 >>> InvBinomialCD(0.9912362670526581, 11, 0.333)
 7
 >>> BinomialCD(7, 11, 0.333)
 0.9912362670526581
 ```
 
 ## Normal Distributions
@@ -97,15 +84,15 @@
 ```
 Cumulative distribution function for the normal distribution `X~N(µ, σ)`.\
 Where `µ` is the mean, and `σ` is the standard deviation.
 
 **Example**\
 To calculate `P(X≤0.891)` for the normal distribution `X~N(0.734, 0.114)`:
 ```python
->>> from python_probabilities import NormalCD
+>>> from promethium import NormalCD
 >>> NormalCD(0.891, 0.734, 0.114)
 0.9157737045522477
 ```
 
 ---
 
 ### Inverse cumulative distribution function
@@ -116,15 +103,15 @@
 Where `µ` is the mean, and `σ` is the standard deviation.
 
 `InvNormalCD(y, µ, σ)` returns the smallest integer `x` such that `NormalCD(x, µ, σ)` is greater than or equal to `y`.
 
 **Example**\
 To calculate the corresponding value for `x` given the value for `y`:
 ```python
->>> from python_probabilities import NormalCD, InvNormalCD
+>>> from promethium import NormalCD, InvNormalCD
 >>> InvNormalCD(0.9157737045522477, 0.734, 0.114)
 0.891
 >>> NormalCD(0.891, 0.734, 0.114)
 0.9157737045522477
 ```
 
 ## Poisson Distributions
@@ -134,30 +121,30 @@
 ```
 For the random variable `X` with the poisson distribution `Po(m)`, calculate the **probability mass function**.\
 Where `r` is the number of occurrences, and `m` is the mean rate of occurrence.
 
 **Example**\
 To calculate `P(X=7)` for the poisson distribution `X~Po(11.556)`:
 ```python
->>> from python_probabilities import PoissonPD
+>>> from promethium import PoissonPD
 >>> PoissonPD(11, 23.445)
 0.0019380401123575617
 ```
 ---
 ### Cumulative distribution function
 ```python
 PoissonCD(r, m)
 ```
 For the random variable `X` with the poisson distribution `Po(m)`, calculate the **cumulative distribution function**.\
 Where `r` is the number of occurrences, and `m` is the mean rate of occurrence.
 
 **Example**\
 To calculate `P(X≤7)` for the poisson distribution `X~Po(11.556)`:
 ```python
->>> from python_probabilities import PoissonCD
+>>> from promethium import PoissonCD
 >>> PoissonCD(11, 23.445)
 0.0034549033698374467
 ```
 ---
 ### Inverse cumulative distribution
 ```python
 InvPoissonCD(q, m)
@@ -166,15 +153,15 @@
 Where `q` is the cumulative probability, and `m` is the mean rate of occurrence.
 
 `InvPoissonCD(q, m)` returns the smallest integer `x` such that `PoissonCD(x, m)` is greater than or equal to `q`.
 
 **Example**\
 To calculate the corresponding value for `r` (number of occurrences) given the values for `q` (cumulative probability):
 ```python
->>> from python_probabilities import PoissonCD, InvPoissonCD
+>>> from promethium import PoissonCD, InvPoissonCD
 >>> InvPoissonCD(0.0034549033698374467, 23.445)
 11
 >>> PoissonCD(11, 23.445)
 0.0034549033698374467
 ```
 
 ## Geometric Distributions
@@ -184,15 +171,15 @@
 ```
 Probability mass function for the geometric distribution `X~G(p)`.\
 Where `x` is the number of trials before the first success, and `p` is the probability of success.
 
 **Example**\
 To calculate `P(X=3)` for the geometric distribution `X~G(0.491)`:
 ```python
->>> from python_probabilities import GeometricPD
+>>> from promethium import GeometricPD
 >>> GeometricPD(3, 0.491)
 0.127208771
 ```
 ---
 
 ### Cumulative distribution function
 ```python
@@ -200,15 +187,15 @@
 ```
 Cumulative distribution function for the geometric distribution `X~G(p)`.\
 Where `x` is the number of trials before the first success, and `p` is the probability of success.
 
 **Example**\
 To calculate `P(X≤3)` for the geometric distribution `X~G(0.491)`:
 ```python
->>> from python_probabilities import GeometricCD
+>>> from promethium import GeometricCD
 >>> GeometricCD(3, 0.491)
 0.868127771
 ```
 ---
 
 ### Inverse cumulative distribution function
 ```python
@@ -218,15 +205,14 @@
 Where `x` is the number of trials before the first success, and `p` is the probability of success.
 
 `InvGeometricCD(area, p)` returns the smallest integer `x` such that `GeometricCD(x, p)` is greater than or equal to `area`.
 
 **Example**\
 To calculate the corresponding value for `x` given the value for `area`:
 ```python
->>> from python_probabilities import GeometricCD, InvGeometricCD
+>>> from promethium import GeometricCD, InvGeometricCD
 >>> InvGeometricCD(0.868, 0.491)
 3
 >> GeometricCD(3, 0.491)
 0.868127771
 ```
 
-
```

