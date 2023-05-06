# Comparing `tmp/composipy-1.0.1.tar.gz` & `tmp/composipy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composipy-1.0.1.tar", last modified: Tue Feb  7 02:58:57 2023, max compression
+gzip compressed data, was "composipy-1.0.2.tar", last modified: Sat May  6 17:07:07 2023, max compression
```

## Comparing `composipy-1.0.1.tar` & `composipy-1.0.2.tar`

### file list

```diff
@@ -1,34 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 02:58:57.826226 composipy-1.0.1/
--rw-rw-rw-   0        0        0     1092 2023-02-05 20:53:41.000000 composipy-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2170 2023-02-07 02:58:57.826226 composipy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1640 2023-02-05 21:05:25.000000 composipy-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-07 02:58:57.793217 composipy-1.0.1/composipy/
--rw-rw-rw-   0        0        0      213 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-07 02:58:57.815223 composipy-1.0.1/composipy/core/
--rw-rw-rw-   0        0        0        0 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/core/__init__.py
--rw-rw-rw-   0        0        0     8651 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/core/material.py
--rw-rw-rw-   0        0        0     6961 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/core/property.py
--rw-rw-rw-   0        0        0    12164 2023-02-07 01:58:55.000000 composipy-1.0.1/composipy/core/structure.py
-drwxrwxrwx   0        0        0        0 2023-02-07 02:58:57.816223 composipy-1.0.1/composipy/nastranapi/
--rw-rw-rw-   0        0        0       58 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/nastranapi/__init__.py
--rw-rw-rw-   0        0        0     6325 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/nastranapi/pcomp_generator.py
-drwxrwxrwx   0        0        0        0 2023-02-07 02:58:57.824225 composipy-1.0.1/composipy/pre_integrated_component/
--rw-rw-rw-   0        0        0  2270468 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/pre_integrated_component/_S.py
--rw-rw-rw-   0        0        0        0 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/pre_integrated_component/__init__.py
--rw-rw-rw-   0        0        0   119327 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/pre_integrated_component/_ii_F.py
--rw-rw-rw-   0        0        0     6377 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/pre_integrated_component/build_k.py
--rw-rw-rw-   0        0        0     1203 2023-02-07 01:58:55.000000 composipy-1.0.1/composipy/pre_integrated_component/functions.py
--rw-rw-rw-   0        0        0     3552 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/pre_integrated_component/write_pre_integrated_terms.py
--rw-rw-rw-   0        0        0     2340 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/pre_integrated_component/write_shape_function.py
-drwxrwxrwx   0        0        0        0 2023-02-07 02:58:57.825225 composipy-1.0.1/composipy/utils/
--rw-rw-rw-   0        0        0       42 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/utils/__init__.py
--rw-rw-rw-   0        0        0     1283 2023-02-05 20:53:41.000000 composipy-1.0.1/composipy/utils/validators.py
--rw-rw-rw-   0        0        0       21 2023-02-07 02:18:13.000000 composipy-1.0.1/composipy/version.py
-drwxrwxrwx   0        0        0        0 2023-02-07 02:58:57.812222 composipy-1.0.1/composipy.egg-info/
--rw-rw-rw-   0        0        0     2170 2023-02-07 02:58:57.000000 composipy-1.0.1/composipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      823 2023-02-07 02:58:57.000000 composipy-1.0.1/composipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 02:58:57.000000 composipy-1.0.1/composipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-02-07 02:58:57.000000 composipy-1.0.1/composipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-07 02:58:57.000000 composipy-1.0.1/composipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-07 02:58:57.826226 composipy-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1012 2023-02-05 20:53:41.000000 composipy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.984605 composipy-1.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-05-05 22:53:36.000000 composipy-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4021 2023-05-06 17:07:07.984605 composipy-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3532 2023-05-05 22:53:36.000000 composipy-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.949596 composipy-1.0.2/composipy/
+-rw-rw-rw-   0        0        0      213 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.968600 composipy-1.0.2/composipy/core/
+-rw-rw-rw-   0        0        0        0 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/core/__init__.py
+-rw-rw-rw-   0        0        0     9276 2023-05-06 16:51:15.000000 composipy-1.0.2/composipy/core/material.py
+-rw-rw-rw-   0        0        0     9433 2023-05-06 16:55:57.000000 composipy-1.0.2/composipy/core/property.py
+-rw-rw-rw-   0        0        0    13254 2023-05-06 00:02:25.000000 composipy-1.0.2/composipy/core/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.969601 composipy-1.0.2/composipy/nastranapi/
+-rw-rw-rw-   0        0        0       58 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/nastranapi/__init__.py
+-rw-rw-rw-   0        0        0     6325 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/nastranapi/pcomp_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.978603 composipy-1.0.2/composipy/pre_integrated_component/
+-rw-rw-rw-   0        0        0  2270468 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/_S.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/__init__.py
+-rw-rw-rw-   0        0        0   119327 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/_ii_F.py
+-rw-rw-rw-   0        0        0     6377 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/build_k.py
+-rw-rw-rw-   0        0        0     1203 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/functions.py
+-rw-rw-rw-   0        0        0     3552 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/write_pre_integrated_terms.py
+-rw-rw-rw-   0        0        0     2340 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/pre_integrated_component/write_shape_function.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.979604 composipy-1.0.2/composipy/utils/
+-rw-rw-rw-   0        0        0       42 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1283 2023-05-05 22:53:36.000000 composipy-1.0.2/composipy/utils/validators.py
+-rw-rw-rw-   0        0        0       21 2023-05-06 12:05:21.000000 composipy-1.0.2/composipy/version.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.964600 composipy-1.0.2/composipy.egg-info/
+-rw-rw-rw-   0        0        0     4021 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 17:07:07.000000 composipy-1.0.2/composipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:07:07.985605 composipy-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2023-05-05 22:53:36.000000 composipy-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:07:07.983604 composipy-1.0.2/tests/
+-rw-rw-rw-   0        0        0     1870 2023-05-05 22:53:36.000000 composipy-1.0.2/tests/test_ABD.py
+-rw-rw-rw-   0        0        0      864 2023-05-05 22:53:36.000000 composipy-1.0.2/tests/test_Material_Q0.py
+-rw-rw-rw-   0        0        0     1185 2023-05-05 22:53:36.000000 composipy-1.0.2/tests/test_lamination_parameters.py
+-rw-rw-rw-   0        0        0     1614 2023-05-05 22:53:36.000000 composipy-1.0.2/tests/test_plate_buckling.py
+-rw-rw-rw-   0        0        0     1948 2023-05-06 16:45:59.000000 composipy-1.0.2/tests/test_plate_buckling_LP.py
```

### Comparing `composipy-1.0.1/LICENSE` & `composipy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `composipy-1.0.1/PKG-INFO` & `composipy-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 Metadata-Version: 2.1
 Name: composipy
-Version: 1.0.1
+Version: 1.0.2
 Summary: This package intends to perform composite material calculations
 Home-page: https://github.com/rafaelpsilva07/composipy
 Author: Rafael Pereira
 Author-email: rafaelpsilva07@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Downloads](https://static.pepy.tech/badge/composipy)](https://pepy.tech/project/composipy)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rafaelpsilva07/composipy/pypi.yml)
+![PyPI](https://img.shields.io/pypi/v/composipy)
+
 
 # Composipy
 
 ## What it is
 
 **composipy** is a python library to calculate composite plates using the classical laminate theory. This library is designed to be simple, userfriendly and helpfull.
 
+Composipy is able to perform buckling calculation considering different boundary conditions and in-plane load applications. See [Examples](https://rafaelpsilva07.github.io/composipy/notebooks/Examples_BCs.html).
+
+
+<img src="https://github.com/rafaelpsilva07/composipy/blob/main/doc/images/load_bcs_examples.PNG" width="700">
+
 
 
 ## How to install
 
 ### Directly From PYPI
 
 ```shell
@@ -36,52 +43,86 @@
 ```shell
 python setup.py install
 ```
 
 
 ## Documentation
 
-[Composipy documentation](https://rafaelpsilva07.github.io/composipy/)
+- [Composipy documentation](https://rafaelpsilva07.github.io/composipy/#contents)
+
+- [Examples](https://rafaelpsilva07.github.io/composipy/notebooks/index.html)
+
+- [Code References](https://rafaelpsilva07.github.io/composipy/reference/index.html)
+
 
 ## Quick start
 
-Create the material.
+### Create the Material Properties.
 
 ```python
 >>> from composipy import OrthotropicMaterial
 >>> 
 >>> E1 = 60800
 >>> E2 = 58250
 >>> v12 = 0.07
 >>> G12 = 4550
 >>> t = 0.21
 >>>
 >>> mat_1 = OrthotropicMaterial(E1, E2, v12, G12, t)
 ```
 
-Define the laminate.
+See [OrthotropicMaterial](https://rafaelpsilva07.github.io/composipy/reference/classes.html) for reference.
+
+
+### Define the Laminate.
 
 ```python
 >>> from composipy import LaminateProperty
 >>> stacking = [-45, 45, 90, 0, 0, 0, 0, 90, 45, -45]
 >>> laminate1 = LaminateProperty(stacking, mat_1)
+```
+
+See [LaminateProperty](https://rafaelpsilva07.github.io/composipy/reference/classes.html#laminateproperty) for reference.
+
+### Calculate Stiffnnes Matrix and Lamination Parameters
+
+```python
 >>> print(laminate1.ABD) # prints the ABD matrix as a np.ndarray
 >>> print(laminate1.xiA) # prints lamination parameters of extension as a np.ndarray
 >>> print(laminate1.xiD) # prints lamination parameters of bending as a np.ndarray
 ```
 
-Create a plate structure.
+### Create a Plate Structure.
 
 ```python
 >>> from composipy import PlateStructure
 >>> 
 >>> constraints = {    
 ---     'x0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
 ---     'xa' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
 ---     'y0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
 ---     'yb' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ']
 --- }
 >>> panel = PlateStructure(laminate1, 360, 360, m=10, n=10, Nxx=-1, constraints=constraints)
+```
+
+See [PlateStructure](https://rafaelpsilva07.github.io/composipy/reference/classes.html#platestructure) for reference.
+
+
+### Calculate Buckling
+```python
 >>> print(panel.buckling_analysis()) # solve the eigenvalue problem.
 ```
 
+### Plot Buckling shape mode
+```python
+>>> print(panel.plot_eigenvalue())
+```
+
+
+
+## Theoretical References
+
+The implementation of composipy is based on the following references
 
+- [Mechanics Of Composite Materials by Robert M. Jones](https://www.routledge.com/Mechanics-Of-Composite-Materials/Jones/p/book/9781560327127)
+- [Castro S.G.P., Donadon M.V. Assembly of semi-analytical models to address linear buckling and vibration of stiffened composite panels with debonding defect. Compos. Struct., 160 (2017), pp. 232-247,](https://www.sciencedirect.com/science/article/abs/pii/S026382231631008X)
```

### Comparing `composipy-1.0.1/composipy/core/material.py` & `composipy-1.0.2/composipy/core/material.py`

 * *Files 12% similar despite different names*

```diff
@@ -143,14 +143,39 @@
             Q22 = self.e2 / (1-self.v12*self.v21)
             Q66 = self.g12
             self.__Q_0 = np.array([[Q11, Q12, 0],
                                    [Q12, Q22, 0],
                                    [0, 0, Q66]])
         return self.__Q_0
 
+    def Invariants(self):
+        '''
+        Get the material invariants
+
+        Returns
+        -------
+        Invariants : numpy.ndarray
+           array([U1, U2, U3, U4, U5])
+        
+        '''
+
+        Q11 = self.Q_0[0, 0]
+        Q12 = self.Q_0[0, 1]
+        Q22 = self.Q_0[1, 1]
+        Q66 = self.Q_0[2, 2]
+
+        U1 = 1/8 * (3*Q11 + 3*Q22 + 2*Q12 + 4*Q66)
+        U2 = 1/2 * (Q11 - Q22)
+        U3 = 1/8 * (Q11 + Q22 - 2*Q12 - 4*Q66)
+        U4 = 1/8 * (Q11 + Q22 + 6*Q12 - 4*Q66)
+        U5 = 1/8 * (Q11 + Q22 - 2*Q12 + 4*Q66)
+        
+        return np.array([U1, U2, U3, U4, U5])
+
+
     def __repr__(self):
         return (
             f'Ply({self.name}, E1 = {self.e1}, E2 = {self.e2}, \n\
             v12 = {self.v12}, G12 = {self.g12}, thickness = {self.thickness}, \n\
             T1 = {self.t1}, C1 = {self.c1}, T2 = {self.t2}, C2 = {self.c2}, S = {self.s})')
     
 #Comparisons
```

### Comparing `composipy-1.0.1/composipy/core/property.py` & `composipy-1.0.2/composipy/core/property.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,53 +16,92 @@
     This class creates laminate object. It needs Material objects (to define plies) and the angle information.
     Some formulation characteristics are:
     Laminate formulations ares used (see References)
     Main reference is the chapter 4 of reference 2.
 
     Parameters
     ----------
-    stacking : list
-        An iterable containing the angles (in degrees) of layup.
+    stacking : list or dict
+        To define a angle stacking sequence
+            An iterable containing the angles (in degrees) of layup.
+        To define a stack based on lamination parameters.
+            {xiA: [xiA1, xiA2, xiA3, xiA4],
+            xiB: [xiB1, xiB2, xiB3, xiB4],
+            xiD: [xiD1, xiD2, xiD3, xiD4],
+            T: thickness}
     plies : Material or list
         A single Material or a list of OrthotropicMaterial object
 
 
     Example
     -------
     >>> from composipy import OrthotropicMaterial, LaminateProperty
     >>> ply_1 = OrthotropicMaterial(129500, 9370, 0.38, 5240, 0.2)
     >>> stacking = [90, 0, 90]
-    >>> laminate = Laminate(stacking, ply_1)
+    >>> laminate_1 = Laminate(stacking, ply_1)
     >>> laminate_1.ABD # retunrs an array containing bending stiffness matrix [D] of the laminate
     >>> laminate_1.xiA # lamination parameters of extension
     >>> laminate_1.xiA # lamination parameters of bending
 
+    Example
+    -------
+    >>> stacking = {'xiD': [0., 0., -1., 0.], 'T': 1.0} #using lamination parameters to define D
+    >>> laminate_2 = Laminate(stacking, ply_1)
+    >>> laminate_2.ABD # retunrs an array containing bending stiffness matrix [D] of the laminate
+    >>> laminate_2.xiA # lamination parameters of extension
+    >>> laminate_2.xiA # lamination parameters of bending
     '''
 
     def __init__(self, stacking, plies):
         # Checking layup
-        if isinstance(plies, Material):
-            n_plies = len(stacking)
-            plies = [plies for s in range(n_plies)]
-        elif len(plies) != len(stacking):
-            raise ValueError('Number of plies and number of stacking must match')
+        if not isinstance(stacking, dict): # implements angle stacking sequence
+            if isinstance(plies, Material):
+                n_plies = len(stacking)
+                plies = [plies for s in range(n_plies)]
+            elif len(plies) != len(stacking):
+                raise ValueError('Number of plies and number of stacking must match')
+            xiA = None
+            xiB = None
+            xiD = None
+            total_thickness = None
+            layup = list(zip(stacking, plies))
+        else:
+            try:
+                xiA = stacking['xiA']
+            except KeyError:
+                xiA = None
+            try:             
+                xiB = stacking['xiB']
+            except KeyError:
+                xiB = None
+            try: 
+                xiD = stacking['xiD']
+            except KeyError:
+                KeyError('xiD must be a key')
+            try:
+                total_thickness = stacking['T']
+            except KeyError:
+                KeyError('T must be a key')
+            layup = []
 
         self.stacking = stacking
         self.plies = plies
-        self.layup = list(zip(stacking, plies))
+        self.layup = layup
         self._z_position = None
         self._Q_layup = None
         self._T_layup = None
         self._A = None
         self._B = None
         self._D = None
         self._ABD = None
         self._ABD_p = None
-        self._xiA = None
-        self._xiB = None
+        self._xiA = xiA
+        self._xiB = xiB
+        self._xiD = xiD
+        self._total_thickness = total_thickness
 
 #Properties
     @property
     def z_position(self):
     
         total_thickness = 0
         for t in self.layup:
@@ -127,40 +166,63 @@
                 self._T_layup.append([T_real,T_engineering])
         return self._T_layup
 
     @property
     def A(self):
         '''[A] Matrix as numpy.ndarray '''
 
+        if not self._xiA is None:
+            raise NotImplementedError
         if self._A is None:
             self._A = np.zeros(9).reshape(3,3)
 
             for i in enumerate(self.Q_layup):
                 zk1 = self.z_position[i[0]+1]
                 zk0 = self.z_position[i[0]]
                 self._A += (zk1-zk0) * i[1]
         return self._A
     
     @property
     def B(self):
         '''[B] Matrix as numpy.ndarray '''
-
+        if not self._xiB is None:
+            raise NotImplementedError
         if self._B is None:
             self._B = np.zeros(9).reshape(3,3)
 
             for i in enumerate(self.Q_layup):
                 zk1 = self.z_position[i[0]+1]
                 zk0 = self.z_position[i[0]]
                 self._B += (1/2) * (zk1**2-zk0**2) * i[1]
         return self._B
     
     @property
     def D(self):
         '''[D] Matrix as numpy.ndarray '''
 
+        if not self._xiD is None:
+
+            U1, U2, U3, U4, U5 = self.plies.Invariants()
+            xi1, xi2, xi3, xi4 = self._xiD
+            T = self._total_thickness
+
+            D11 = T**3*(U1 + U2*xi1 + U3*xi3)/12
+            D12 = T**3*(-U3*xi3 + U4)/12
+            D13 = T**3*(U2*xi2/2 + U3*xi4)/12
+            D21 = T**3*(-U3*xi3 + U4)/12
+            D22 = T**3*(U1 - U2*xi1 + U3*xi3)/12
+            D23 = T**3*(U2*xi2/2 - U3*xi4)/12
+            D31 = T**3*(U2*xi2/2 + U3*xi4)/12
+            D32 = T**3*(U2*xi2/2 - U3*xi4)/12
+            D33 = T**3*(-U3*xi3 + U5)/12
+
+            self._D = np.array([[D11, D12, D13],
+                                [D21, D22, D23],
+                                [D31, D32, D33]])
+
         if self._D is None:
             self._D = np.zeros(9).reshape(3,3)
 
             for i in enumerate(self.Q_layup):
                 zk1 = self.z_position[i[0]+1]
                 zk0 = self.z_position[i[0]]
                 self._D += (1/3) * (zk1**3-zk0**3) * i[1]
@@ -185,15 +247,17 @@
             zk1 = self.z_position[i+1]
             zk0 = self.z_position[i]
 
             xiA[0] += (zk1-zk0) * np.cos(2*angle)
             xiA[1] += (zk1-zk0) * np.sin(2*angle)
             xiA[2] += (zk1-zk0) * np.cos(4*angle)
             xiA[3] += (zk1-zk0) * np.sin(4*angle)                        
-        return xiA / T
+        
+        self._xiA = xiA / T
+        return self._xiA
 
     @property
     def xiD(self):
         '''Lamination parameter xiD'''
         xiD = np.zeros(4)
         T = sum([ply.thickness for ply in self.plies])        
         for i, angle in enumerate(self.stacking):
```

### Comparing `composipy-1.0.1/composipy/core/structure.py` & `composipy-1.0.2/composipy/core/structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -227,17 +227,18 @@
         self.su_idx = list(product(um, un))
         self.sv_idx = list(product(vm, vn))
         self.sw_idx = list(product(wm, wn))
 
         return (uidx, vidx, widx)
     
     #TODO: parallel process, sparse matrix, cython
-    def calc_K_KG(self):
+    def calc_K_KG_ABD(self):
         '''
         Calculates the stiffness and geometrical stifness matrices.
+        Considers full ABD matrix.
 
         Returns
         -------
         K_KG : tuple
             A tuple of array containing (K, KG)
         '''
 
@@ -291,14 +292,48 @@
         np.hstack([k00, k00, k00]),
         np.hstack([k00, k00, k00]),
         np.hstack([k00, k00, k33g])
         ])
 
         return K, KG  
 
+    def calc_K_KG_D(self):
+        '''
+        Calculates the stiffness and geometrical stifness matrices.
+        Considers only the bending stiffness D matrix.
+
+        Returns
+        -------
+        K_KG : tuple
+            A tuple of array containing (K, KG)
+        '''
+
+        D11, D12, D16 = self.dproperty.D[0, ::]
+        D12, D22, D26 = self.dproperty.D[1, ::]
+        D16, D26, D66 = self.dproperty.D[2, ::]
+
+        k33 = []
+        k33g = []
+
+        uidx, vidx, widx = self._compute_constraints()
+
+        for i in range(self.m**2*self.n**2):
+                wi, wj, wk, wl = widx[i]
+
+                k33.append(calc_k33_ijkl(self.a, self.b, wi, wj, wk, wl, D11, D12, D22, D16, D26, D66))
+                k33g.append(calc_kG33_ijkl(self.a, self.b, wi, wj, wk, wl, self.Nxx, self.Nyy, self.Nxy))
+        
+        k33 = np.array(k33).reshape(self.m*self.n, self.m*self.n)
+        k33g = np.array(k33g).reshape(self.m*self.n, self.m*self.n)
+
+        K = k33
+        KG = k33g
+
+        return K, KG  
+
     def buckling_analysis(self, silent=True, num_eigvalues = 5):
         """
         Linear Buckling Analysis
 
         Parameters
         ----------
         silent : bool, optional
@@ -309,15 +344,15 @@
         Returns
         -------
         eigvals, eigvecs
         """
         if not silent:
             ti = time()       
             print('calculating K and KG')
-        K, KG = self.calc_K_KG()
+        K, KG = self.calc_K_KG_D()
         K, KG = csr_matrix(K), csr_matrix(KG)
         if not silent:
             print(f'K and KG calculated in {time()-ti} seconds')
         tol = 0
     
         if not silent:
             ti = time()
```

### Comparing `composipy-1.0.1/composipy/nastranapi/pcomp_generator.py` & `composipy-1.0.2/composipy/nastranapi/pcomp_generator.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.1/composipy/pre_integrated_component/_S.py` & `composipy-1.0.2/composipy/pre_integrated_component/_S.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.1/composipy/pre_integrated_component/_ii_F.py` & `composipy-1.0.2/composipy/pre_integrated_component/_ii_F.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.1/composipy/pre_integrated_component/build_k.py` & `composipy-1.0.2/composipy/pre_integrated_component/build_k.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.1/composipy/pre_integrated_component/functions.py` & `composipy-1.0.2/composipy/pre_integrated_component/functions.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.1/composipy/pre_integrated_component/write_pre_integrated_terms.py` & `composipy-1.0.2/composipy/pre_integrated_component/write_pre_integrated_terms.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.1/composipy/pre_integrated_component/write_shape_function.py` & `composipy-1.0.2/composipy/pre_integrated_component/write_shape_function.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.1/composipy/utils/validators.py` & `composipy-1.0.2/composipy/utils/validators.py`

 * *Files identical despite different names*

### Comparing `composipy-1.0.1/composipy.egg-info/PKG-INFO` & `composipy-1.0.2/composipy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 Metadata-Version: 2.1
 Name: composipy
-Version: 1.0.1
+Version: 1.0.2
 Summary: This package intends to perform composite material calculations
 Home-page: https://github.com/rafaelpsilva07/composipy
 Author: Rafael Pereira
 Author-email: rafaelpsilva07@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Downloads](https://static.pepy.tech/badge/composipy)](https://pepy.tech/project/composipy)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rafaelpsilva07/composipy/pypi.yml)
+![PyPI](https://img.shields.io/pypi/v/composipy)
+
 
 # Composipy
 
 ## What it is
 
 **composipy** is a python library to calculate composite plates using the classical laminate theory. This library is designed to be simple, userfriendly and helpfull.
 
+Composipy is able to perform buckling calculation considering different boundary conditions and in-plane load applications. See [Examples](https://rafaelpsilva07.github.io/composipy/notebooks/Examples_BCs.html).
+
+
+<img src="https://github.com/rafaelpsilva07/composipy/blob/main/doc/images/load_bcs_examples.PNG" width="700">
+
 
 
 ## How to install
 
 ### Directly From PYPI
 
 ```shell
@@ -36,52 +43,86 @@
 ```shell
 python setup.py install
 ```
 
 
 ## Documentation
 
-[Composipy documentation](https://rafaelpsilva07.github.io/composipy/)
+- [Composipy documentation](https://rafaelpsilva07.github.io/composipy/#contents)
+
+- [Examples](https://rafaelpsilva07.github.io/composipy/notebooks/index.html)
+
+- [Code References](https://rafaelpsilva07.github.io/composipy/reference/index.html)
+
 
 ## Quick start
 
-Create the material.
+### Create the Material Properties.
 
 ```python
 >>> from composipy import OrthotropicMaterial
 >>> 
 >>> E1 = 60800
 >>> E2 = 58250
 >>> v12 = 0.07
 >>> G12 = 4550
 >>> t = 0.21
 >>>
 >>> mat_1 = OrthotropicMaterial(E1, E2, v12, G12, t)
 ```
 
-Define the laminate.
+See [OrthotropicMaterial](https://rafaelpsilva07.github.io/composipy/reference/classes.html) for reference.
+
+
+### Define the Laminate.
 
 ```python
 >>> from composipy import LaminateProperty
 >>> stacking = [-45, 45, 90, 0, 0, 0, 0, 90, 45, -45]
 >>> laminate1 = LaminateProperty(stacking, mat_1)
+```
+
+See [LaminateProperty](https://rafaelpsilva07.github.io/composipy/reference/classes.html#laminateproperty) for reference.
+
+### Calculate Stiffnnes Matrix and Lamination Parameters
+
+```python
 >>> print(laminate1.ABD) # prints the ABD matrix as a np.ndarray
 >>> print(laminate1.xiA) # prints lamination parameters of extension as a np.ndarray
 >>> print(laminate1.xiD) # prints lamination parameters of bending as a np.ndarray
 ```
 
-Create a plate structure.
+### Create a Plate Structure.
 
 ```python
 >>> from composipy import PlateStructure
 >>> 
 >>> constraints = {    
 ---     'x0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
 ---     'xa' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
 ---     'y0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
 ---     'yb' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ']
 --- }
 >>> panel = PlateStructure(laminate1, 360, 360, m=10, n=10, Nxx=-1, constraints=constraints)
+```
+
+See [PlateStructure](https://rafaelpsilva07.github.io/composipy/reference/classes.html#platestructure) for reference.
+
+
+### Calculate Buckling
+```python
 >>> print(panel.buckling_analysis()) # solve the eigenvalue problem.
 ```
 
+### Plot Buckling shape mode
+```python
+>>> print(panel.plot_eigenvalue())
+```
+
+
+
+## Theoretical References
+
+The implementation of composipy is based on the following references
 
+- [Mechanics Of Composite Materials by Robert M. Jones](https://www.routledge.com/Mechanics-Of-Composite-Materials/Jones/p/book/9781560327127)
+- [Castro S.G.P., Donadon M.V. Assembly of semi-analytical models to address linear buckling and vibration of stiffened composite panels with debonding defect. Compos. Struct., 160 (2017), pp. 232-247,](https://www.sciencedirect.com/science/article/abs/pii/S026382231631008X)
```

### Comparing `composipy-1.0.1/composipy.egg-info/SOURCES.txt` & `composipy-1.0.2/composipy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -18,8 +18,13 @@
 composipy/pre_integrated_component/__init__.py
 composipy/pre_integrated_component/_ii_F.py
 composipy/pre_integrated_component/build_k.py
 composipy/pre_integrated_component/functions.py
 composipy/pre_integrated_component/write_pre_integrated_terms.py
 composipy/pre_integrated_component/write_shape_function.py
 composipy/utils/__init__.py
-composipy/utils/validators.py
+composipy/utils/validators.py
+tests/test_ABD.py
+tests/test_Material_Q0.py
+tests/test_lamination_parameters.py
+tests/test_plate_buckling.py
+tests/test_plate_buckling_LP.py
```

### Comparing `composipy-1.0.1/setup.py` & `composipy-1.0.2/setup.py`

 * *Files identical despite different names*

