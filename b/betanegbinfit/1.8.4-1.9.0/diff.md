# Comparing `tmp/betanegbinfit-1.8.4.tar.gz` & `tmp/betanegbinfit-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betanegbinfit-1.8.4.tar", last modified: Sun Apr 16 06:19:02 2023, max compression
+gzip compressed data, was "betanegbinfit-1.9.0.tar", last modified: Sat May  6 12:30:24 2023, max compression
```

## Comparing `betanegbinfit-1.8.4.tar` & `betanegbinfit-1.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-16 06:19:02.858565 betanegbinfit-1.8.4/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-16 06:19:02.858565 betanegbinfit-1.8.4/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.8.4/README.md
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-16 06:19:02.855232 betanegbinfit-1.8.4/betanegbinfit/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-04-16 06:18:37.000000 betanegbinfit-1.8.4/betanegbinfit/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/betacdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/betainc.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/bridge_mixalime.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/cdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/combine.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/create.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    32670 2023-04-04 13:54:13.000000 betanegbinfit-1.8.4/betanegbinfit/distributions.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/hyp.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-16 06:19:02.858565 betanegbinfit-1.8.4/betanegbinfit/models/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/models/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/models/model.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/models/model_line.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/models/model_line_lrt.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/models/model_mixture.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/models/model_mixtures.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/models/model_window.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/plot.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/stats.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/tests.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-03-30 18:19:57.000000 betanegbinfit-1.8.4/betanegbinfit/utils.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-16 06:19:02.855232 betanegbinfit-1.8.4/betanegbinfit.egg-info/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-16 06:19:02.000000 betanegbinfit-1.8.4/betanegbinfit.egg-info/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-04-16 06:19:02.000000 betanegbinfit-1.8.4/betanegbinfit.egg-info/SOURCES.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-04-16 06:19:02.000000 betanegbinfit-1.8.4/betanegbinfit.egg-info/dependency_links.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-04-16 06:19:02.000000 betanegbinfit-1.8.4/betanegbinfit.egg-info/requires.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-04-16 06:19:02.000000 betanegbinfit-1.8.4/betanegbinfit.egg-info/top_level.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-04-16 06:19:02.858565 betanegbinfit-1.8.4/setup.cfg
--rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-04-16 06:18:26.000000 betanegbinfit-1.8.4/setup.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 12:30:24.611404 betanegbinfit-1.9.0/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-06 12:30:24.611404 betanegbinfit-1.9.0/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.9.0/README.md
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 12:30:24.608071 betanegbinfit-1.9.0/betanegbinfit/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-05-06 11:44:59.000000 betanegbinfit-1.9.0/betanegbinfit/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/betacdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/betainc.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/bridge_mixalime.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/cdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/combine.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/create.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    38366 2023-05-06 11:44:38.000000 betanegbinfit-1.9.0/betanegbinfit/distributions.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/hyp.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 12:30:24.611404 betanegbinfit-1.9.0/betanegbinfit/models/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_line.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_line_lrt.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_mixture.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_mixtures.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_window.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/plot.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/stats.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/tests.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/utils.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 12:30:24.608071 betanegbinfit-1.9.0/betanegbinfit.egg-info/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/SOURCES.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/dependency_links.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/requires.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/top_level.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-05-06 12:30:24.611404 betanegbinfit-1.9.0/setup.cfg
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-04-16 06:18:26.000000 betanegbinfit-1.9.0/setup.py
```

### Comparing `betanegbinfit-1.8.4/PKG-INFO` & `betanegbinfit-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.8.4
+Version: 1.9.0
+Summary: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
@@ -72,7 +75,9 @@
 
 
 **Please note, that all functions have plenty of optional arguments and they all are documented, so please consider reading through `help(function of interest)`.**
 
 
 ### A note on performance
 As far as we are concerned, **BetaNegBinFit** should work within a manageable amounts of time. For insance, when `ModelLine` with `model='BetaNB'` ran against *chipseq.tsv* dataset, it finishes in 6 minutes when ran at Ryzen 5600U. It does so under 2 minutes with `model='NB'`.
+
+
```

### Comparing `betanegbinfit-1.8.4/README.md` & `betanegbinfit-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/__init__.py` & `betanegbinfit-1.9.0/betanegbinfit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.8.4'
+__version__ = '1.9.0'
 
 import warnings
 # This will omit annoying FutureWarnings by JAX and RutimeWarnings caused by
 # estimates being clipped at bounds.
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.simplefilter(action='ignore', category=RuntimeWarning)
```

### Comparing `betanegbinfit-1.8.4/betanegbinfit/betacdnb.py` & `betanegbinfit-1.9.0/betanegbinfit/betacdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/betainc.py` & `betanegbinfit-1.9.0/betanegbinfit/betainc.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/bridge_mixalime.py` & `betanegbinfit-1.9.0/betanegbinfit/bridge_mixalime.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/cdnb.py` & `betanegbinfit-1.9.0/betanegbinfit/cdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/combine.py` & `betanegbinfit-1.9.0/betanegbinfit/combine.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/create.py` & `betanegbinfit-1.9.0/betanegbinfit/create.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/distributions.py` & `betanegbinfit-1.9.0/betanegbinfit/distributions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """Custom pyro-compatiable distribution"""
 from jax.scipy.special import betaln, gammaln, logsumexp
 from .betainc import betainc, logbetainc
 from . import cdnb, betacdnb
 import jax.numpy as jnp
 from scipy import stats
+from scipy.stats import betabinom as scipy_betabinom
 from scipy.stats import nbinom as scipy_nb, beta
 from scipy.stats import binom as scipy_binom
 from abc import abstractmethod
 from math import ceil
 import numpy as np
 import gmpy2
 import mpmath
@@ -358,14 +359,96 @@
     @staticmethod
     def long_cdf(x, r, p, skip=-1, ret_dict=False, r_transform=None):
         return scipy_binom.cdf(x, r, p)
     
     @staticmethod
     def long_sf(x, r, p, r_transform=None):
         return scipy_binom.sf(x, r, p)
+
+class BetaBinom(Distribution):
+    @staticmethod
+    def sample(r, mu, concentration, size, r_transform=None):
+        a = mu * concentration
+        b = (1.0 - mu) * concentration
+        return scipy_betabinom.rvs(n=r, a=a, b=b, size=size)
+
+    @staticmethod
+    def logprob(x, r, mu, concentration, r_transform=None):
+        a = mu * concentration
+        b = (1.0 - mu) * concentration
+        return scipy_betabinom.logpmf(x, n=r, a=a, b=b)
+    
+    @staticmethod
+    def cdf(x, r, mu, concentration, r_transform=None):
+        a = mu * concentration
+        b = (1.0 - mu) * concentration
+        return scipy_betabinom.cdf(x, n=r, a=a, b=b)
+    
+    @staticmethod
+    def sf(x, r, mu, concentration, r_transform=None):
+        a = mu * concentration
+        b = (1.0 - mu) * concentration
+        return scipy_betabinom.sf(x, n=r, a=a, b=b)
+    
+    @staticmethod
+    def mean(r, mu, concentration, r_transform=None):
+        a = mu * concentration
+        b = (1.0 - mu) * concentration
+        return scipy_betabinom.mean(n=r, a=a, b=b)
+    
+    @staticmethod
+    def long_mean(r, p, return_long=False, r_transform=None):
+        raise NotImplementedError
+    
+    @staticmethod
+    def long_cdf(x, r, mu, concentration, skip=-1, ret_dict=False, r_transform=None):
+        mu = gmpy2.mpq(str(mu)); concentration = gmpy2.mpfr(str(concentration))
+        r = gmpy2.mpfr(str(r))
+        a = mu * concentration
+        b = (gmpy2.mpq('1') - mu) * concentration
+        if type(x) in (np.ndarray, list):
+            x = list(x)
+        else:
+            x = [x]
+        cdfs = dict()
+        m = max(x)
+        nums = list(range(ceil(m)))
+        nums.append(m)
+        nums = [gmpy2.mpz(int(n)) for n in nums]
+        base = gmpy2.mpfr(str(mpmath.gammaprod(list(map(str, [b + r, a + b])), 
+                                                list(map(str, [a + r + b, b])))))
+        if 0 > skip:
+            s = base
+        else:
+            s = 0
+        cdfs[0] = s
+        last_cdf = s
+        pmf = base
+        num = gmpy2.mpq('1')
+        denum = gmpy2.mpq('1')
+        order = 0
+        pow_2 = gmpy2.mpfr('2')
+        for v in nums[1:]:
+            order_num, num = gmpy2.frexp(num * (1 + r - v) * (a + v - 1))
+            order_denum, denum = gmpy2.frexp(denum * v * (b + r - v))
+            order += order_num - order_denum
+            pmf = (num / denum) * base * pow_2 ** order
+            if v > skip:
+                s += pmf
+            if s < 1:
+                last_cdf = s
+            cdfs[v] = last_cdf
+        if ret_dict:
+            return cdfs
+        return list(map(cdfs.get, x))
+    
+    @staticmethod
+    def long_sf(x, r, mu, concentration, r_transform=None):
+        o = gmpy2.mpfr('1')
+        return [o - t for t in BetaBinom.long_cdf(x, r, mu, concentration, r_transform=r_transform)]  
     
 
 class LeftTruncatedBinom(Binom):
     def __init__(self, r, probs, left=5, validate_args=None):
         self.left = left
         self.left_vals = jnp.arange(1, left)
         super().__init__(r, probs, validate_args=validate_args)
@@ -402,17 +485,17 @@
         return res
 
     @staticmethod
     def long_cdf(x, r, p, left, r_transform=None):
         s = super(LeftTruncatedBinom, LeftTruncatedBinom)
         if type(r) in (list, np.ndarray):
             sm = list(map(gmpy2.mpfr, s.long_sf(left, r, p)))
-            res = [gmpy2.mpfr(cdf) / denom for cdf, denom in zip(s.long_cdf(x, r, p, r_transform=r_transform), sm)]
+            res = [gmpy2.mpfr(cdf) / denom for cdf, denom in zip(s.long_cdf(x, r, p, r_transform=r_transform, skip=left), sm)]
         else:
-            sm = gmpy2.mpfr(s.long_sf(left, r, p, r_transform=r_transform))
+            sm = gmpy2.mpfr(s.long_sf(left, r, p, r_transform=r_transform, skip=left))
             res = [gmpy2.mpfr(c) / sm for c in s.long_cdf(x, r, p)]
         return res 
     
     @staticmethod
     def long_sf(x, r, p, left, r_transform=None):
         sf = super(LeftTruncatedBinom, LeftTruncatedBinom).long_sf
         return sf(x, r, p) / sf(left, r, p)
@@ -440,14 +523,78 @@
                    for i in range(x + 1))
 
     @staticmethod
     def sf(x, r, p, left, r_transform=None):
         return 1 - Binom.cdf(x, r, p, left)
 
 
+class LeftTruncatedBetaBinom(BetaBinom):
+
+    @staticmethod
+    def sample(r, p, left, size: int, r_transform=None):
+        raise NotImplementedError
+
+    @staticmethod
+    def logprob(x, r, mu, concentration, left, r_transform=None):
+        left = float(left)
+        logprob = BetaBinom.logprob
+        lp = jnp.where(x <= left, -jnp.inf, logprob(x, r, mu, concentration))
+        lp = logprob(x, r, mu, concentration) - jnp.log1p(-sum(jnp.exp(logprob(i, r, mu, concentration))
+                                               for i in range(int(left) + 1)))
+        return jnp.where(x <= left, -jnp.inf, lp)
+
+    @staticmethod
+    def long_logprob(x, r, mu, concentration, left, r_transform=None) -> list:
+        raise NotImplementedError
+
+    @staticmethod
+    def long_cdf(x, r, mu, concentration, left, r_transform=None):
+        s = super(LeftTruncatedBetaBinom, LeftTruncatedBetaBinom)
+        if type(r) in (list, np.ndarray):
+            sm = s.long_sf(left, r, mu, concentration)
+            res = [gmpy2.mpfr(cdf) / denom for cdf, denom in zip(s.long_cdf(x, r, mu, concentration, r_transform=r_transform,
+                                                                            skip=left), sm)]
+        else:
+            sm = s.long_sf(left, r, mu, concentration, r_transform=r_transform)[0]
+            res = [gmpy2.mpfr(c) / sm for c in s.long_cdf(x, r, mu, concentration,
+                                                          skip=left)]
+        return res 
+    
+    @staticmethod
+    def long_sf(x, r, mu, concentration, left, r_transform=None):
+        return [1 - t for t in LeftTruncatedBetaBinom.cdf(x, r, mu, concentration, left, r_transform)]
+
+    @staticmethod
+    def mean(r, mu, concentration, left, r_transform=None):
+        s = super(LeftTruncatedBetaBinom, LeftTruncatedBetaBinom)
+        m = s.mean(r, mu, concentration) 
+        m -= sum(i * jnp.exp(s.logprob(i, r, mu, concentration)) for i in range(1, left + 1)) 
+        return m / s.sf(left, r, mu, concentration)
+    
+    @staticmethod
+    def long_mean(r, mu, concentration, left, return_long=False, r_transform=None):
+        s = super(BetaBinom, BetaBinom)
+        m = s.long_mean(r, mu, concentration, return_long=True) 
+        m -= sum(i * gmpy2.exp(s.long_logprob(i, r, mu, concentration)[0]) for i in range(1, left + 1)) 
+        mean = m / (gmpy2.mpfr('1') - s.long_cdf(left, r, mu, concentration)[0])
+        if return_long:
+            return mean
+        return float(mean)
+
+    @staticmethod
+    def cdf(x, r, mu, concentration, left, r_transform=None):
+        return sum(jnp.exp(BetaBinom.logprob(i, r, mu, concentration, left))
+                   for i in range(x + 1))
+
+    @staticmethod
+    def sf(x, r, mu, concentration, left, r_transform=None):
+        raise NotImplementedError
+
+
+
     
 class LeftTruncatedNB(NB):
     def __init__(self, r, probs, left=5, validate_args=None):
         self.left = left
         self.left_vals = jnp.arange(1, left)
         super().__init__(r, probs, validate_args=validate_args)
```

### Comparing `betanegbinfit-1.8.4/betanegbinfit/hyp.py` & `betanegbinfit-1.9.0/betanegbinfit/hyp.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/models/model.py` & `betanegbinfit-1.9.0/betanegbinfit/models/model.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/models/model_line.py` & `betanegbinfit-1.9.0/betanegbinfit/models/model_line.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/models/model_line_lrt.py` & `betanegbinfit-1.9.0/betanegbinfit/models/model_line_lrt.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/models/model_mixture.py` & `betanegbinfit-1.9.0/betanegbinfit/models/model_mixture.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/models/model_mixtures.py` & `betanegbinfit-1.9.0/betanegbinfit/models/model_mixtures.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/models/model_window.py` & `betanegbinfit-1.9.0/betanegbinfit/models/model_window.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/plot.py` & `betanegbinfit-1.9.0/betanegbinfit/plot.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/stats.py` & `betanegbinfit-1.9.0/betanegbinfit/stats.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/tests.py` & `betanegbinfit-1.9.0/betanegbinfit/tests.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit/utils.py` & `betanegbinfit-1.9.0/betanegbinfit/utils.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/betanegbinfit.egg-info/PKG-INFO` & `betanegbinfit-1.9.0/betanegbinfit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.8.4
+Version: 1.9.0
+Summary: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
@@ -72,7 +75,9 @@
 
 
 **Please note, that all functions have plenty of optional arguments and they all are documented, so please consider reading through `help(function of interest)`.**
 
 
 ### A note on performance
 As far as we are concerned, **BetaNegBinFit** should work within a manageable amounts of time. For insance, when `ModelLine` with `model='BetaNB'` ran against *chipseq.tsv* dataset, it finishes in 6 minutes when ran at Ryzen 5600U. It does so under 2 minutes with `model='NB'`.
+
+
```

### Comparing `betanegbinfit-1.8.4/betanegbinfit.egg-info/SOURCES.txt` & `betanegbinfit-1.9.0/betanegbinfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.4/setup.py` & `betanegbinfit-1.9.0/setup.py`

 * *Files identical despite different names*

