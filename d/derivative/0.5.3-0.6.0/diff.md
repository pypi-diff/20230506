# Comparing `tmp/derivative-0.5.3.tar.gz` & `tmp/derivative-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "derivative-0.5.3.tar", max compression
+gzip compressed data, was "derivative-0.6.0.tar", max compression
```

## Comparing `derivative-0.5.3.tar` & `derivative-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1229 2020-10-07 19:44:41.036098 derivative-0.5.3/LICENSE.rst
--rw-r--r--   0        0        0     4840 2022-11-08 04:44:38.286464 derivative-0.5.3/README.rst
--rw-r--r--   0        0        0      204 2022-11-08 04:44:38.298464 derivative-0.5.3/derivative/__init__.py
--rw-r--r--   0        0        0       27 2022-11-08 05:03:01.266639 derivative-0.5.3/derivative/__version__.py
--rw-r--r--   0        0        0     8598 2022-11-08 04:44:38.298464 derivative-0.5.3/derivative/dglobal.py
--rw-r--r--   0        0        0     9399 2022-11-08 04:44:38.298464 derivative-0.5.3/derivative/differentiation.py
--rw-r--r--   0        0        0     5657 2020-09-30 20:29:42.803394 derivative-0.5.3/derivative/dlocal.py
--rw-r--r--   0        0        0     4230 2022-11-08 04:44:38.302464 derivative-0.5.3/derivative/utils.py
--rw-r--r--   0        0        0     1162 2022-11-08 05:02:28.141510 derivative-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     5923 2022-11-08 05:08:46.442934 derivative-0.5.3/setup.py
--rw-r--r--   0        0        0     6143 2022-11-08 05:08:46.443291 derivative-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1229 2023-05-06 17:44:02.681192 derivative-0.6.0/LICENSE.rst
+-rw-r--r--   0        0        0     5447 2023-05-06 17:44:02.681192 derivative-0.6.0/README.rst
+-rw-r--r--   0        0        0      212 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/__version__.py
+-rw-r--r--   0        0        0    11189 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/dglobal.py
+-rw-r--r--   0        0        0     9399 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/differentiation.py
+-rw-r--r--   0        0        0     5657 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/dlocal.py
+-rw-r--r--   0        0        0     4230 2023-05-06 17:44:02.681192 derivative-0.6.0/derivative/utils.py
+-rw-r--r--   0        0        0     1206 2023-05-06 17:44:02.685191 derivative-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 derivative-0.6.0/setup.py
+-rw-r--r--   0        0        0     6666 1970-01-01 00:00:00.000000 derivative-0.6.0/PKG-INFO
```

### Comparing `derivative-0.5.3/LICENSE.rst` & `derivative-0.6.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `derivative-0.5.3/README.rst` & `derivative-0.6.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-|RTD| |PyPI| |Zenodo| |LIC|
+|RTD| |PyPI| |Zenodo| |GithubCI| |LIC|
 
 Numerical differentiation of noisy time series data in python
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 **derivative** is a Python package for differentiating noisy data. The package showcases a variety of improvements that can be made over finite differences when data is not clean.
 
 Want to see an example of how **derivative** can help? This package is part of **PySINDy** (`github.com/dynamicslab/pysindy <https://github.com/dynamicslab/pysindy/>`_), a sparse-regression framework for discovering nonlinear dynamical systems from data.
@@ -18,14 +18,16 @@
 
 4. Spline derivatives of any order.
 
 5. Polynomial-trend-filtered derivatives generalizing methods like total variational derivatives.
 
 6. Kalman derivatives find the maximum likelihood estimator for a derivative described by a Brownian motion.
 
+7. Kernel derivatives smooth a random process defined by its kernel (covariance).
+
 .. code-block:: python
 
     from derivative import dxdt
     import numpy as np
 
     t = np.linspace(0,2*np.pi,50)
     x = np.sin(x)
@@ -43,34 +45,38 @@
     result4 = dxdt(x, t, kind="spline", s=1e-2)
 
     # 5. Total variational derivative with regularization set to 0.01
     result5 = dxdt(x, t, kind="trend_filtered", order=0, alpha=1e-2)
 
     # 6. Kalman derivative with smoothing set to 1
     result6 = dxdt(x, t, kind="kalman", alpha=1)
-
+    
+    # 7. Kernel derivative with smoothing set to 1
+    result7 = dxdt(x, t, kind="kernel", sigma=1, lmbd=.1, kernel="rbf")
 
 Contributors:
 -------------
 Thanks to the members of the community who have contributed!
 
 +-----------------------------------------------------------------+----------------------------------------------------------------------------------+
-|  `Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_  | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_ |  
+|  `Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_  | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_,|
+|								  | Kernel derivatives `#30 <https://github.com/andgoldschmidt/derivative/pull/30>`_ |  
 +-----------------------------------------------------------------+----------------------------------------------------------------------------------+
 
 
 References:
 -----------
 
 [1] Numerical differentiation of experimental data: local versus global methods- K. Ahnert and M. Abel
 
 [2] Numerical Differentiation of Noisy, Nonsmooth Data- Rick Chartrand
 
 [3] The Solution Path of the Generalized LASSO- R.J. Tibshirani and J. Taylor
 
+[4] A Kernel Approach for PDE Discovery and Operator Learning - D. Long et al.
 
 
 Citing derivative:
 ------------------
 The **derivative** package is a contribution to `PySINDy <https://github.com/dynamicslab/pysindy/>`_; this work has been published in the Journal of Open Source Software (JOSS). If you use **derivative** in your work, please cite it using the following reference:
 
 Kaptanoglu et al., (2022). PySINDy: A comprehensive Python package for robust sparse system identification. Journal of Open Source Software, 7(69), 3994, https://doi.org/10.21105/joss.03994
@@ -100,7 +106,11 @@
    :alt: MIT License
 
 .. |PyPI| image:: https://badge.fury.io/py/derivative.svg
     :target: https://pypi.org/project/derivative/
 
 .. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6617446.svg
    :target: https://doi.org/10.5281/zenodo.6617446
+
+.. |GithubCI| image:: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml/badge.svg
+    :target: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml
+
```

### Comparing `derivative-0.5.3/derivative/dglobal.py` & `derivative-0.6.0/derivative/dglobal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import partialmethod
 from .differentiation import Derivative, register
 from .utils import deriv, integ, _memoize_arrays
 
 import numpy as np
 from numpy.linalg import inv
 from scipy import interpolate, sparse
 from scipy.special import legendre
@@ -112,15 +113,14 @@
         self.dorder = order + 1
         self.alpha = alpha
         self.kwargs = kwargs
 
         self._t = None
         self._x = None
         self._model = None
-        self._res = None
 
     @staticmethod
     def _nullsp(order, diffop):
         #  Analytic solutions to the null space are Legendre polynomials.
         n = diffop.shape[1]
         x = np.linspace(-1,1,n)
         dx = x[1]-x[0]
@@ -129,14 +129,15 @@
             lp = legendre(i,monic=True)(x)
             norm = np.sqrt(2/(2*i+1)/dx)
             lp = lp/norm
             nullsp.append(lp)
         nullsp = np.vstack(nullsp)
         return nullsp
 
+    @_memoize_arrays(1)
     def _global(self, t, x):
         self._t = t
         self._x = x
 
         # I: Integrals and derivatives
         n = len(self._t)
         dt = self._t[1] - self._t[0]
@@ -148,38 +149,49 @@
         Dtilde = np.vstack([arrD, self._nullsp(self.dorder, arrD)])
 
         # III: Compute workers X1 and X2
         invDtilde = inv(Dtilde)
         XDtilde = arrI.dot(invDtilde)
         X1, X2 = XDtilde[:, :-1], XDtilde[:, -1:]
 
-        # IV: Compute projectors
+        # IV: Compute projectors for range and nullspace of X2
         # Note: regarding inv, X2.T@X2 is always small
         X2_proj = inv(X2.T.dot(X2)).dot(X2.T)
         proj = np.identity(n) - X2.dot(X2_proj)
 
         # V: LASSO parameters; fit
         A = proj.dot(X1)
         b = proj.dot(self._x - self._x[0])
         self._model = Lasso(alpha=self.alpha / n, fit_intercept=False, **self.kwargs)
         self._model.fit(A, b)
 
         # VI: Restore desired variables
         theta1_hat = self._model.coef_
         theta2_hat = X2_proj.dot(self._x - self._x[0] - X1.dot(theta1_hat))
-        self._res = invDtilde.dot(np.hstack([theta1_hat, theta2_hat]))
+        x_dot_hat = invDtilde.dot(np.hstack([theta1_hat, theta2_hat]))
+        x_hat = arrI @ x_dot_hat + x[0]
+        return x_hat, x_dot_hat
 
     def compute(self, t, x, i):
-        self._global(t, x)
-        return self._res[i]
+        x_dot_hat = self._global(t, x)[1]
+        return x_dot_hat[i]
 
     def compute_for(self, t, x, indices):
-        self._global(t, x)
+        x_dot_hat = self._global(t, x)[1]
         for i in indices:
-            yield self._res[i]
+            yield x_dot_hat[i]
+
+    def compute_x(self, t, x, i):
+        x_hat = self._global(t, x)[0]
+        return x_hat[i]
+
+    def compute_x_for(self, t, x, indices):
+        x_hat = self._global(t, x)[0]
+        for i in indices:
+            yield x_hat[i]
 
 
 @register("kalman")
 class Kalman(Derivative):
     def __init__(self, alpha = 1):
         """ Fit the derivative assuming that given data are noisy measurements
 
@@ -237,7 +249,71 @@
         x_hat = self._global(t, x, self.alpha)[0]
         return x_hat[i]
 
     def compute_x_for(self, t, x, indices):
         x_hat = self._global(t, x, self.alpha)[0]
         for i in indices:
             yield x_hat[i]
+
+
+@register("kernel")
+class Kernel(Derivative):
+    def __init__(self, sigma: float=1, lmbd: float=0, kernel: str="gaussian"):
+        """ Fit the derivative assuming a gaussian process specified by kernels
+
+        Args:
+            sigma: parameter of kernel function
+            lmbd: noise variance
+            kernel: name of kernel function
+        """
+        self.sigma = sigma
+        self.lmbd = lmbd
+        self.kernel = kernel
+
+    @staticmethod
+    def _gauss_kernel(t1, t2, sigma):
+        r2 = (t2-t1)
+        return np.exp(-r2 ** 2 / (2 * sigma ** 2))
+
+    @staticmethod
+    def _gauss_kernel_dt(t1, t2, sigma):
+        r2 = (t2-t1)
+        return - (r2 / sigma **2) * np.exp(-r2 ** 2 / (2 * sigma ** 2))
+
+    @staticmethod
+    def _create_gram(kernel_func, t):
+        v_kernel_func = np.vectorize(kernel_func)
+        rows, cols = np.meshgrid(t,t)
+        return v_kernel_func(rows, cols)
+
+    @_memoize_arrays(1)
+    def _global(self, t, z, sigma, lmbd, kernel):
+        if kernel in ("gaussian", "rbf"):
+            k_fun = lambda t1, t2: self._gauss_kernel(t1, t2, sigma=sigma)
+            k_fun_dt = lambda t1, t2: self._gauss_kernel_dt(t1, t2, sigma=sigma)
+        else:
+            raise ValueError("Must choose either gaussian or rbf kernel")
+        kernel = self._create_gram(k_fun, t)
+        kernel_dt = self._create_gram(k_fun_dt, t)
+        noisy_kernel = kernel + lmbd * np.eye(len(t))
+        alpha = np.linalg.solve(noisy_kernel, z)
+        x_hat = kernel @ alpha
+        x_dot_hat = kernel_dt @ alpha
+        return x_hat, x_dot_hat
+
+    def compute(self, t, x, i):
+        x_dot_hat = self._global(t, x, self.sigma, self.lmbd, self.kernel)[1]
+        return x_dot_hat[i]
+
+    def compute_for(self, t, x, indices):
+        x_dot_hat = self._global(t, x, self.sigma, self.lmbd, self.kernel)[1]
+        for i in indices:
+            yield x_dot_hat[i]
+
+    def compute_x(self, t, x, i):
+        x_hat = self._global(t, x, self.sigma, self.lmbd, self.kernel)[0]
+        return x_hat[i]
+
+    def compute_x_for(self, t, x, indices):
+        x_hat = self._global(t, x, self.sigma, self.lmbd, self.kernel)[0]
+        for i in indices:
+            yield x_hat[i]
```

### Comparing `derivative-0.5.3/derivative/differentiation.py` & `derivative-0.6.0/derivative/differentiation.py`

 * *Files identical despite different names*

### Comparing `derivative-0.5.3/derivative/dlocal.py` & `derivative-0.6.0/derivative/dlocal.py`

 * *Files identical despite different names*

### Comparing `derivative-0.5.3/derivative/utils.py` & `derivative-0.6.0/derivative/utils.py`

 * *Files identical despite different names*

### Comparing `derivative-0.5.3/pyproject.toml` & `derivative-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 [tool.poetry]
 name = "derivative"
-version = "0.5.3"
+version = "0.6.0"
 description = "Numerical differentiation in python."
 repository = "https://github.com/andgoldschmidt/derivative"
 documentation = "https://derivative.readthedocs.io/"
 keywords = ["differentiation", "derivative", "gradient", "prime"]
-authors = ["Andy Goldschmidt <andygold@uw.edu>", "Markus Quade <info@markusqua.de>"]
+authors = [
+    "Andy Goldschmidt <andygold@uchicago.edu>",
+    "Markus Quade <info@markusqua.de>",
+    "Jacob Stevens-Haas <jmsh@uw.edu>"
+]
 license = "MIT"
 readme = "README.rst"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 numpy = "^1.18.3"
 scipy = "^1.4.1"
-scikit-learn = "~1.0.0"
+scikit-learn = "^1"
 
 # docs
-sphinx = {version = "^4.0.2", optional = true}
+sphinx = {version = "^4.5", optional = true}
 nbsphinx = {version = "^0.6.1", optional = true}
 ipykernel = {version = "^5.2.1", optional = true}
 jupyter_client = {version = "^6.1.3", optional = true}
-sphinx_rtd_theme = {version = "^0.4.3", optional = true}
+sphinx_rtd_theme = {version = "^1", optional = true}
 matplotlib = {version = "^3.2.1", optional = true}
-pandoc = {version = "^2.2", optional = true}
+#pandoc = {version = "^2.2", optional = true}
 
 # dev
-pytest = {version = "^3.6.4", optional = true}
+pytest = {version = "^7", optional = true}
 
 [tool.poetry.extras]
 docs = ["sphinx", "nbsphinx", "ipykernel", "jupyter_client", "sphinx_rtd_theme", "matplotlib", "pandoc"]
 dev = ["pytest"]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.1.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `derivative-0.5.3/setup.py` & `derivative-0.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 packages = \
 ['derivative']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.18.3,<2.0.0', 'scikit-learn>=1.0.0,<1.1.0', 'scipy>=1.4.1,<2.0.0']
+['numpy>=1.18.3,<2.0.0', 'scikit-learn>=1,<2', 'scipy>=1.4.1,<2.0.0']
 
 extras_require = \
-{'dev': ['pytest>=3.6.4,<4.0.0'],
- 'docs': ['sphinx>=4.0.2,<5.0.0',
+{'dev': ['pytest>=7,<8'],
+ 'docs': ['sphinx>=4.5,<5.0',
           'nbsphinx>=0.6.1,<0.7.0',
           'ipykernel>=5.2.1,<6.0.0',
           'jupyter_client>=6.1.3,<7.0.0',
-          'sphinx_rtd_theme>=0.4.3,<0.5.0',
-          'matplotlib>=3.2.1,<4.0.0',
-          'pandoc>=2.2,<3.0']}
+          'sphinx_rtd_theme>=1,<2',
+          'matplotlib>=3.2.1,<4.0.0']}
 
 setup_kwargs = {
     'name': 'derivative',
-    'version': '0.5.3',
+    'version': '0.6.0',
     'description': 'Numerical differentiation in python.',
-    'long_description': '|RTD| |PyPI| |Zenodo| |LIC|\n\nNumerical differentiation of noisy time series data in python\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\n**derivative** is a Python package for differentiating noisy data. The package showcases a variety of improvements that can be made over finite differences when data is not clean.\n\nWant to see an example of how **derivative** can help? This package is part of **PySINDy** (`github.com/dynamicslab/pysindy <https://github.com/dynamicslab/pysindy/>`_), a sparse-regression framework for discovering nonlinear dynamical systems from data.\n\nThis package binds common differentiation methods to a single easily implemented differentiation interface to encourage user adaptation.\nNumerical differentiation methods for noisy time series data in python includes:\n\n1. Symmetric finite difference schemes using arbitrary window size.\n\n2. Savitzky-Galoy derivatives (aka polynomial-filtered derivatives) of any polynomial order with independent left and right window parameters.\n\n3. Spectral derivatives with optional filter.\n\n4. Spline derivatives of any order.\n\n5. Polynomial-trend-filtered derivatives generalizing methods like total variational derivatives.\n\n6. Kalman derivatives find the maximum likelihood estimator for a derivative described by a Brownian motion.\n\n.. code-block:: python\n\n    from derivative import dxdt\n    import numpy as np\n\n    t = np.linspace(0,2*np.pi,50)\n    x = np.sin(x)\n\n    # 1. Finite differences with central differencing using 3 points.\n    result1 = dxdt(x, t, kind="finite_difference", k=1)\n\n    # 2. Savitzky-Golay using cubic polynomials to fit in a centered window of length 1\n    result2 = dxdt(x, t, kind="savitzky_golay", left=.5, right=.5, order=3)\n\n    # 3. Spectral derivative\n    result3 = dxdt(x, t, kind="spectral")\n\n    # 4. Spline derivative with smoothing set to 0.01\n    result4 = dxdt(x, t, kind="spline", s=1e-2)\n\n    # 5. Total variational derivative with regularization set to 0.01\n    result5 = dxdt(x, t, kind="trend_filtered", order=0, alpha=1e-2)\n\n    # 6. Kalman derivative with smoothing set to 1\n    result6 = dxdt(x, t, kind="kalman", alpha=1)\n\n\nContributors:\n-------------\nThanks to the members of the community who have contributed!\n\n+-----------------------------------------------------------------+----------------------------------------------------------------------------------+\n|  `Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_  | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_ |  \n+-----------------------------------------------------------------+----------------------------------------------------------------------------------+\n\n\nReferences:\n-----------\n\n[1] Numerical differentiation of experimental data: local versus global methods- K. Ahnert and M. Abel\n\n[2] Numerical Differentiation of Noisy, Nonsmooth Data- Rick Chartrand\n\n[3] The Solution Path of the Generalized LASSO- R.J. Tibshirani and J. Taylor\n\n\n\nCiting derivative:\n------------------\nThe **derivative** package is a contribution to `PySINDy <https://github.com/dynamicslab/pysindy/>`_; this work has been published in the Journal of Open Source Software (JOSS). If you use **derivative** in your work, please cite it using the following reference:\n\nKaptanoglu et al., (2022). PySINDy: A comprehensive Python package for robust sparse system identification. Journal of Open Source Software, 7(69), 3994, https://doi.org/10.21105/joss.03994\n\n.. code-block:: text\n\n      @article{kaptanoglu2022pysindy,\n  \tdoi = {10.21105/joss.03994},\n  \turl = {https://doi.org/10.21105/joss.03994},\n  \tyear = {2022},\n  \tpublisher = {The Open Journal},\n  \tvolume = {7},\n  \tnumber = {69},\n  \tpages = {3994},\n  \tauthor = {Alan A. Kaptanoglu and Brian M. de Silva and Urban Fasel and Kadierdan Kaheman and Andy J. Goldschmidt and Jared Callaham and Charles B. Delahunt and Zachary G. Nicolaou and Kathleen Champion and Jean-Christophe Loiseau and J. Nathan Kutz and Steven L. Brunton},\n  \ttitle = {PySINDy: A comprehensive Python package for robust sparse system identification},\n  \tjournal = {Journal of Open Source Software}\n\t}\n    \n\n.. |RTD| image:: https://readthedocs.org/projects/derivative/badge/?version=latest\n   :target: https://derivative.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n  \n.. |LIC| image:: https://img.shields.io/badge/License-MIT-blue.svg\n   :target: https://derivative.readthedocs.io/en/latest/license.html\n   :alt: MIT License\n\n.. |PyPI| image:: https://badge.fury.io/py/derivative.svg\n    :target: https://pypi.org/project/derivative/\n\n.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6617446.svg\n   :target: https://doi.org/10.5281/zenodo.6617446\n',
+    'long_description': '|RTD| |PyPI| |Zenodo| |GithubCI| |LIC|\n\nNumerical differentiation of noisy time series data in python\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\n**derivative** is a Python package for differentiating noisy data. The package showcases a variety of improvements that can be made over finite differences when data is not clean.\n\nWant to see an example of how **derivative** can help? This package is part of **PySINDy** (`github.com/dynamicslab/pysindy <https://github.com/dynamicslab/pysindy/>`_), a sparse-regression framework for discovering nonlinear dynamical systems from data.\n\nThis package binds common differentiation methods to a single easily implemented differentiation interface to encourage user adaptation.\nNumerical differentiation methods for noisy time series data in python includes:\n\n1. Symmetric finite difference schemes using arbitrary window size.\n\n2. Savitzky-Galoy derivatives (aka polynomial-filtered derivatives) of any polynomial order with independent left and right window parameters.\n\n3. Spectral derivatives with optional filter.\n\n4. Spline derivatives of any order.\n\n5. Polynomial-trend-filtered derivatives generalizing methods like total variational derivatives.\n\n6. Kalman derivatives find the maximum likelihood estimator for a derivative described by a Brownian motion.\n\n7. Kernel derivatives smooth a random process defined by its kernel (covariance).\n\n.. code-block:: python\n\n    from derivative import dxdt\n    import numpy as np\n\n    t = np.linspace(0,2*np.pi,50)\n    x = np.sin(x)\n\n    # 1. Finite differences with central differencing using 3 points.\n    result1 = dxdt(x, t, kind="finite_difference", k=1)\n\n    # 2. Savitzky-Golay using cubic polynomials to fit in a centered window of length 1\n    result2 = dxdt(x, t, kind="savitzky_golay", left=.5, right=.5, order=3)\n\n    # 3. Spectral derivative\n    result3 = dxdt(x, t, kind="spectral")\n\n    # 4. Spline derivative with smoothing set to 0.01\n    result4 = dxdt(x, t, kind="spline", s=1e-2)\n\n    # 5. Total variational derivative with regularization set to 0.01\n    result5 = dxdt(x, t, kind="trend_filtered", order=0, alpha=1e-2)\n\n    # 6. Kalman derivative with smoothing set to 1\n    result6 = dxdt(x, t, kind="kalman", alpha=1)\n    \n    # 7. Kernel derivative with smoothing set to 1\n    result7 = dxdt(x, t, kind="kernel", sigma=1, lmbd=.1, kernel="rbf")\n\nContributors:\n-------------\nThanks to the members of the community who have contributed!\n\n+-----------------------------------------------------------------+----------------------------------------------------------------------------------+\n|  `Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_  | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_,|\n|\t\t\t\t\t\t\t\t  | Kernel derivatives `#30 <https://github.com/andgoldschmidt/derivative/pull/30>`_ |  \n+-----------------------------------------------------------------+----------------------------------------------------------------------------------+\n\n\nReferences:\n-----------\n\n[1] Numerical differentiation of experimental data: local versus global methods- K. Ahnert and M. Abel\n\n[2] Numerical Differentiation of Noisy, Nonsmooth Data- Rick Chartrand\n\n[3] The Solution Path of the Generalized LASSO- R.J. Tibshirani and J. Taylor\n\n[4] A Kernel Approach for PDE Discovery and Operator Learning - D. Long et al.\n\n\nCiting derivative:\n------------------\nThe **derivative** package is a contribution to `PySINDy <https://github.com/dynamicslab/pysindy/>`_; this work has been published in the Journal of Open Source Software (JOSS). If you use **derivative** in your work, please cite it using the following reference:\n\nKaptanoglu et al., (2022). PySINDy: A comprehensive Python package for robust sparse system identification. Journal of Open Source Software, 7(69), 3994, https://doi.org/10.21105/joss.03994\n\n.. code-block:: text\n\n      @article{kaptanoglu2022pysindy,\n  \tdoi = {10.21105/joss.03994},\n  \turl = {https://doi.org/10.21105/joss.03994},\n  \tyear = {2022},\n  \tpublisher = {The Open Journal},\n  \tvolume = {7},\n  \tnumber = {69},\n  \tpages = {3994},\n  \tauthor = {Alan A. Kaptanoglu and Brian M. de Silva and Urban Fasel and Kadierdan Kaheman and Andy J. Goldschmidt and Jared Callaham and Charles B. Delahunt and Zachary G. Nicolaou and Kathleen Champion and Jean-Christophe Loiseau and J. Nathan Kutz and Steven L. Brunton},\n  \ttitle = {PySINDy: A comprehensive Python package for robust sparse system identification},\n  \tjournal = {Journal of Open Source Software}\n\t}\n    \n\n.. |RTD| image:: https://readthedocs.org/projects/derivative/badge/?version=latest\n   :target: https://derivative.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n  \n.. |LIC| image:: https://img.shields.io/badge/License-MIT-blue.svg\n   :target: https://derivative.readthedocs.io/en/latest/license.html\n   :alt: MIT License\n\n.. |PyPI| image:: https://badge.fury.io/py/derivative.svg\n    :target: https://pypi.org/project/derivative/\n\n.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6617446.svg\n   :target: https://doi.org/10.5281/zenodo.6617446\n\n.. |GithubCI| image:: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml/badge.svg\n    :target: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml\n\n',
     'author': 'Andy Goldschmidt',
-    'author_email': 'andygold@uw.edu',
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'andygold@uchicago.edu',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/andgoldschmidt/derivative',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `derivative-0.5.3/PKG-INFO` & `derivative-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: derivative
-Version: 0.5.3
+Version: 0.6.0
 Summary: Numerical differentiation in python.
 Home-page: https://github.com/andgoldschmidt/derivative
 License: MIT
 Keywords: differentiation,derivative,gradient,prime
 Author: Andy Goldschmidt
-Author-email: andygold@uw.edu
+Author-email: andygold@uchicago.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: dev
 Provides-Extra: docs
 Requires-Dist: ipykernel (>=5.2.1,<6.0.0); extra == "docs"
 Requires-Dist: jupyter_client (>=6.1.3,<7.0.0); extra == "docs"
 Requires-Dist: matplotlib (>=3.2.1,<4.0.0); extra == "docs"
 Requires-Dist: nbsphinx (>=0.6.1,<0.7.0); extra == "docs"
 Requires-Dist: numpy (>=1.18.3,<2.0.0)
-Requires-Dist: pandoc (>=2.2,<3.0); extra == "docs"
-Requires-Dist: pytest (>=3.6.4,<4.0.0); extra == "dev"
-Requires-Dist: scikit-learn (>=1.0.0,<1.1.0)
+Requires-Dist: pytest (>=7,<8); extra == "dev"
+Requires-Dist: scikit-learn (>=1,<2)
 Requires-Dist: scipy (>=1.4.1,<2.0.0)
-Requires-Dist: sphinx (>=4.0.2,<5.0.0); extra == "docs"
-Requires-Dist: sphinx_rtd_theme (>=0.4.3,<0.5.0); extra == "docs"
+Requires-Dist: sphinx (>=4.5,<5.0); extra == "docs"
+Requires-Dist: sphinx_rtd_theme (>=1,<2); extra == "docs"
 Project-URL: Documentation, https://derivative.readthedocs.io/
 Project-URL: Repository, https://github.com/andgoldschmidt/derivative
 Description-Content-Type: text/x-rst
 
-|RTD| |PyPI| |Zenodo| |LIC|
+|RTD| |PyPI| |Zenodo| |GithubCI| |LIC|
 
 Numerical differentiation of noisy time series data in python
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 **derivative** is a Python package for differentiating noisy data. The package showcases a variety of improvements that can be made over finite differences when data is not clean.
 
 Want to see an example of how **derivative** can help? This package is part of **PySINDy** (`github.com/dynamicslab/pysindy <https://github.com/dynamicslab/pysindy/>`_), a sparse-regression framework for discovering nonlinear dynamical systems from data.
@@ -51,14 +50,16 @@
 
 4. Spline derivatives of any order.
 
 5. Polynomial-trend-filtered derivatives generalizing methods like total variational derivatives.
 
 6. Kalman derivatives find the maximum likelihood estimator for a derivative described by a Brownian motion.
 
+7. Kernel derivatives smooth a random process defined by its kernel (covariance).
+
 .. code-block:: python
 
     from derivative import dxdt
     import numpy as np
 
     t = np.linspace(0,2*np.pi,50)
     x = np.sin(x)
@@ -76,34 +77,38 @@
     result4 = dxdt(x, t, kind="spline", s=1e-2)
 
     # 5. Total variational derivative with regularization set to 0.01
     result5 = dxdt(x, t, kind="trend_filtered", order=0, alpha=1e-2)
 
     # 6. Kalman derivative with smoothing set to 1
     result6 = dxdt(x, t, kind="kalman", alpha=1)
-
+    
+    # 7. Kernel derivative with smoothing set to 1
+    result7 = dxdt(x, t, kind="kernel", sigma=1, lmbd=.1, kernel="rbf")
 
 Contributors:
 -------------
 Thanks to the members of the community who have contributed!
 
 +-----------------------------------------------------------------+----------------------------------------------------------------------------------+
-|  `Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_  | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_ |  
+|  `Jacob Stevens-Haas <https://github.com/Jacob-Stevens-Haas>`_  | Kalman derivatives `#12 <https://github.com/andgoldschmidt/derivative/pull/12>`_,|
+|								  | Kernel derivatives `#30 <https://github.com/andgoldschmidt/derivative/pull/30>`_ |  
 +-----------------------------------------------------------------+----------------------------------------------------------------------------------+
 
 
 References:
 -----------
 
 [1] Numerical differentiation of experimental data: local versus global methods- K. Ahnert and M. Abel
 
 [2] Numerical Differentiation of Noisy, Nonsmooth Data- Rick Chartrand
 
 [3] The Solution Path of the Generalized LASSO- R.J. Tibshirani and J. Taylor
 
+[4] A Kernel Approach for PDE Discovery and Operator Learning - D. Long et al.
 
 
 Citing derivative:
 ------------------
 The **derivative** package is a contribution to `PySINDy <https://github.com/dynamicslab/pysindy/>`_; this work has been published in the Journal of Open Source Software (JOSS). If you use **derivative** in your work, please cite it using the following reference:
 
 Kaptanoglu et al., (2022). PySINDy: A comprehensive Python package for robust sparse system identification. Journal of Open Source Software, 7(69), 3994, https://doi.org/10.21105/joss.03994
@@ -134,7 +139,11 @@
 
 .. |PyPI| image:: https://badge.fury.io/py/derivative.svg
     :target: https://pypi.org/project/derivative/
 
 .. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6617446.svg
    :target: https://doi.org/10.5281/zenodo.6617446
 
+.. |GithubCI| image:: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml/badge.svg
+    :target: https://github.com/andgoldschmidt/derivative/actions/workflows/push-test.yml
+
+
```

