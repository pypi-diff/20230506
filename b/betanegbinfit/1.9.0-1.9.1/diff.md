# Comparing `tmp/betanegbinfit-1.9.0.tar.gz` & `tmp/betanegbinfit-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betanegbinfit-1.9.0.tar", last modified: Sat May  6 12:30:24 2023, max compression
+gzip compressed data, was "betanegbinfit-1.9.1.tar", last modified: Sat May  6 13:26:08 2023, max compression
```

## Comparing `betanegbinfit-1.9.0.tar` & `betanegbinfit-1.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 12:30:24.611404 betanegbinfit-1.9.0/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-06 12:30:24.611404 betanegbinfit-1.9.0/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.9.0/README.md
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 12:30:24.608071 betanegbinfit-1.9.0/betanegbinfit/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-05-06 11:44:59.000000 betanegbinfit-1.9.0/betanegbinfit/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/betacdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/betainc.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/bridge_mixalime.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/cdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/combine.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/create.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    38366 2023-05-06 11:44:38.000000 betanegbinfit-1.9.0/betanegbinfit/distributions.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/hyp.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 12:30:24.611404 betanegbinfit-1.9.0/betanegbinfit/models/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_line.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_line_lrt.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_mixture.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_mixtures.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/models/model_window.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/plot.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/stats.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/tests.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-04-24 17:33:25.000000 betanegbinfit-1.9.0/betanegbinfit/utils.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 12:30:24.608071 betanegbinfit-1.9.0/betanegbinfit.egg-info/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/SOURCES.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/dependency_links.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/requires.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-05-06 12:30:24.000000 betanegbinfit-1.9.0/betanegbinfit.egg-info/top_level.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-05-06 12:30:24.611404 betanegbinfit-1.9.0/setup.cfg
--rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-04-16 06:18:26.000000 betanegbinfit-1.9.0/setup.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.9.1/README.md
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 13:26:08.416389 betanegbinfit-1.9.1/betanegbinfit/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-05-06 13:25:32.000000 betanegbinfit-1.9.1/betanegbinfit/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/betacdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/betainc.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/bridge_mixalime.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/cdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/combine.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/create.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    38370 2023-05-06 13:24:10.000000 betanegbinfit-1.9.1/betanegbinfit/distributions.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/hyp.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/betanegbinfit/models/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_line.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_line_lrt.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_mixture.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_mixtures.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_window.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/plot.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/stats.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/tests.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/utils.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/betanegbinfit.egg-info/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/SOURCES.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/dependency_links.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/requires.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/top_level.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/setup.cfg
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-04-16 06:18:26.000000 betanegbinfit-1.9.1/setup.py
```

### Comparing `betanegbinfit-1.9.0/PKG-INFO` & `betanegbinfit-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.9.0
+Version: 1.9.1
 Summary: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `betanegbinfit-1.9.0/README.md` & `betanegbinfit-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/__init__.py` & `betanegbinfit-1.9.1/betanegbinfit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.9.0'
+__version__ = '1.9.1'
 
 import warnings
 # This will omit annoying FutureWarnings by JAX and RutimeWarnings caused by
 # estimates being clipped at bounds.
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.simplefilter(action='ignore', category=RuntimeWarning)
```

### Comparing `betanegbinfit-1.9.0/betanegbinfit/betacdnb.py` & `betanegbinfit-1.9.1/betanegbinfit/betacdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/betainc.py` & `betanegbinfit-1.9.1/betanegbinfit/betainc.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/bridge_mixalime.py` & `betanegbinfit-1.9.1/betanegbinfit/bridge_mixalime.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/cdnb.py` & `betanegbinfit-1.9.1/betanegbinfit/cdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/combine.py` & `betanegbinfit-1.9.1/betanegbinfit/combine.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/create.py` & `betanegbinfit-1.9.1/betanegbinfit/create.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/distributions.py` & `betanegbinfit-1.9.1/betanegbinfit/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,15 +524,14 @@
 
     @staticmethod
     def sf(x, r, p, left, r_transform=None):
         return 1 - Binom.cdf(x, r, p, left)
 
 
 class LeftTruncatedBetaBinom(BetaBinom):
-
     @staticmethod
     def sample(r, p, left, size: int, r_transform=None):
         raise NotImplementedError
 
     @staticmethod
     def logprob(x, r, mu, concentration, left, r_transform=None):
         left = float(left)
@@ -557,15 +556,15 @@
             sm = s.long_sf(left, r, mu, concentration, r_transform=r_transform)[0]
             res = [gmpy2.mpfr(c) / sm for c in s.long_cdf(x, r, mu, concentration,
                                                           skip=left)]
         return res 
     
     @staticmethod
     def long_sf(x, r, mu, concentration, left, r_transform=None):
-        return [1 - t for t in LeftTruncatedBetaBinom.cdf(x, r, mu, concentration, left, r_transform)]
+        return [1 - t for t in LeftTruncatedBetaBinom.long_cdf(x, r, mu, concentration, left, r_transform)]
 
     @staticmethod
     def mean(r, mu, concentration, left, r_transform=None):
         s = super(LeftTruncatedBetaBinom, LeftTruncatedBetaBinom)
         m = s.mean(r, mu, concentration) 
         m -= sum(i * jnp.exp(s.logprob(i, r, mu, concentration)) for i in range(1, left + 1)) 
         return m / s.sf(left, r, mu, concentration)
```

### Comparing `betanegbinfit-1.9.0/betanegbinfit/hyp.py` & `betanegbinfit-1.9.1/betanegbinfit/hyp.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/models/model.py` & `betanegbinfit-1.9.1/betanegbinfit/models/model.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/models/model_line.py` & `betanegbinfit-1.9.1/betanegbinfit/models/model_line.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/models/model_line_lrt.py` & `betanegbinfit-1.9.1/betanegbinfit/models/model_line_lrt.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/models/model_mixture.py` & `betanegbinfit-1.9.1/betanegbinfit/models/model_mixture.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/models/model_mixtures.py` & `betanegbinfit-1.9.1/betanegbinfit/models/model_mixtures.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/models/model_window.py` & `betanegbinfit-1.9.1/betanegbinfit/models/model_window.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/plot.py` & `betanegbinfit-1.9.1/betanegbinfit/plot.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/stats.py` & `betanegbinfit-1.9.1/betanegbinfit/stats.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/tests.py` & `betanegbinfit-1.9.1/betanegbinfit/tests.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit/utils.py` & `betanegbinfit-1.9.1/betanegbinfit/utils.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/betanegbinfit.egg-info/PKG-INFO` & `betanegbinfit-1.9.1/betanegbinfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.9.0
+Version: 1.9.1
 Summary: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `betanegbinfit-1.9.0/betanegbinfit.egg-info/SOURCES.txt` & `betanegbinfit-1.9.1/betanegbinfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.0/setup.py` & `betanegbinfit-1.9.1/setup.py`

 * *Files identical despite different names*

