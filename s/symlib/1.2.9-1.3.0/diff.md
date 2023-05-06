# Comparing `tmp/symlib-1.2.9.tar.gz` & `tmp/symlib-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.2.9.tar", last modified: Tue Apr 18 17:25:41 2023, max compression
+gzip compressed data, was "symlib-1.3.0.tar", last modified: Sat May  6 00:43:31 2023, max compression
```

## Comparing `symlib-1.2.9.tar` & `symlib-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-18 17:25:41.753183 symlib-1.2.9/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.2.9/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-04-18 17:25:41.753067 symlib-1.2.9/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.2.9/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.2.9/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-18 17:25:41.753219 symlib-1.2.9/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-04-18 17:25:39.000000 symlib-1.2.9/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-18 17:25:41.752300 symlib-1.2.9/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1629 2023-04-18 17:25:19.000000 symlib-1.2.9/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.2.9/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    44206 2023-04-18 17:25:19.000000 symlib-1.2.9/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)    35330 2023-04-11 22:48:38.000000 symlib-1.2.9/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     8469 2022-09-02 12:56:37.000000 symlib-1.2.9/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-18 17:25:41.752878 symlib-1.2.9/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      287 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-04-18 17:25:41.000000 symlib-1.2.9/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-06 00:43:31.923970 symlib-1.3.0/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-06 00:43:31.923856 symlib-1.3.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.0/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.0/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-05-06 00:43:31.924003 symlib-1.3.0/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-05-06 00:43:24.000000 symlib-1.3.0/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-06 00:43:31.923139 symlib-1.3.0/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1629 2023-04-18 17:25:19.000000 symlib-1.3.0/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.0/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    46482 2023-05-06 00:43:01.000000 symlib-1.3.0/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)    35330 2023-04-11 22:48:38.000000 symlib-1.3.0/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     8508 2023-05-06 00:43:01.000000 symlib-1.3.0/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-06 00:43:31.923700 symlib-1.3.0/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      287 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-05-06 00:43:31.000000 symlib-1.3.0/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.2.9/LICENSE` & `symlib-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.2.9/PKG-INFO` & `symlib-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.2.9
+Version: 1.3.0
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.2.9/setup.py` & `symlib-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.2.9"
+version = "1.3.0"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.2.9/symlib/__init__.py` & `symlib-1.3.0/symlib/__init__.py`

 * *Files identical despite different names*

### Comparing `symlib-1.2.9/symlib/file_management.py` & `symlib-1.3.0/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.2.9/symlib/lib.py` & `symlib-1.3.0/symlib/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import array
 import struct
 import numpy as np
 import os
 import os.path as path
 import scipy.interpolate as interpolate
 import numpy.random as random
+import scipy.optimize as optimize
 import glob
 from . import util
 
 """ SUBHALO_DTYPE is the numpy datatype used by the main return value of
 read_subhalos(). Positions and distances are in comvoing Mpc/h, velocities are
 physical peculiar velocities, and masses are in Msun/h.
 """
@@ -79,20 +80,30 @@
  - r50_bound: radius enclosing 50% of bound particles
  - r50_bound_rs: radius enclosing 50% of bound particles
  - r95_bound: radius enclosing 95% of bound particles
  - m_tidal: total mass within tidal radius
  - m_tidal_bound: total bound mass within tidal radius
  - m_bound: total bound mass
  - ok: true if the core is being tracked and false otherwise
+ - ok_rs: true if a rockstar halo exists and at least one core particle is
+   still inside Rockstar's r_50 (almost all cases where this fails are cases
+   where Rockstar has made an error)
+ - is_err: Rockstar and core-tracking disagree, but more core particles are
+   assoicated with Rockstar
+ - is_err_rs: Rockstar and core-tracking disagree, but more core particles are
+   with the particle-tracking subhalo.
+ - interp: true if the core in this snapshot is interpolated betwen two
+   nearby snapshots.
 """
 CORE_DTYPE = [("x", "f4", (3,)), ("v", "f4", (3,)), ("r_tidal", "f4"),
               ("r50_bound", "f4"), ("r50_bound_rs", "f4"), ("m_tidal", "f4"),
               ("m_tidal_bound", "f4"), ("m_bound", "f4"), ("vmax", "f4"),
               ("f_core", "f4"), ("f_core_rs", "f4"), ("d_core_mbp", "f4"),
-              ("ok", "?"), ("ok_rs", "?"), ("is_err", "?"), ("is_err_rs", "?")]
+              ("ok", "?"), ("ok_rs", "?"), ("is_err", "?"), ("is_err_rs", "?"),
+              ("interp", "?")]
 
 """ UM_DTYPE is a numpy datatype representing UniverseMachine predictions for
 galaxy properties.
 - m_star: the stellar mass of the galaxy in Msun
 - m_in_situ: the stellar mass of a galaxy that formed inside the galaxy (as
              opposed to coming in via mergers) in Msun
 - m_icl: the stellar mass of the galaxy's stellar halo
@@ -108,15 +119,22 @@
       false otherwise
 """
 UM_DTYPE = [("m_star", "f4"), ("m_in_situ", "f4"), ("m_icl", "f4"),
             ("sfr", "f4"), ("x", "f4", (3,)), ("v", "f4", (3,)),
             ("rank", "f4"), ("mvir", "f4"), ("vmax", "f4"),
             ("is_orphan", "?"), ("ok", "?")]
 
-""" TODO
+""" PARTICLE_DTYPE is a numpy datatype representing the properties of tracked 
+particles within a subhalo. Positions (x) and velocities (v) are given in
+physical units.
+- x: position in pkpc
+- v: velocity in km/s
+- snap: integer value for the desired snapshot
+ - ok: true if the particle is being tracked and false otherwise
+ - smooth: true if the particle smoothly accreted onto the subhalo and false otherwise.
 """
 PARTICLE_DTYPE = [
     ("x", "f4", (3,)), ("v", "f4", (3,)),
     ("snap", "i4"), ("id", "i4"),
     ("ok", "?"), ("smooth", "?")
 ]
 
@@ -301,16 +319,14 @@
         mvir = max(0, mvir)
 
     omega_L = 1 - omega_M
     Ez = np.sqrt(omega_M/a**3 + omega_L)
     rho_crit = 2.77519737e11*Ez**2
     omega_Mz = (omega_M/a**3)/Ez**2
 
-    rho_m = omega_Mz * rho_crit
-
     x = omega_Mz - 1
     delta_vir = 18*np.pi**2 + 82*x - 39.0*x**2
     rho_vir = rho_crit*delta_vir
 
     r_phys = (mvir/(rho_vir * (4*np.pi / 3)))**(1.0/3)
     r_cmov = r_phys/a
 
@@ -503,22 +519,24 @@
         h["mpeak_pre"][i] = mpeak_infall
         h["false_selection"][i] = mpeak_infall < 300*param["mp"]
 
     return h
 
 def read_cores(dir_name, include_false_selections=False, suffix="fid"):
     """ read_cores read the particle-tracked halo cores of the halo in the
-    given directory. The returned array is a structured array of type CORE_DTYPE
-    with shape (n_halos, n_snaps).
+    given directory. The returned array is a structured array of type
+    CORE_DTYPE with shape (n_halos, n_snaps).
     """
     if suffix == "":
         file_name = path.join(dir_name, "halos", "cores.dat")
     else:
         file_name = path.join(dir_name, "halos", "cores_%s.dat" % suffix)
 
+    param = simulation_parameters(dir_name)
+    mp = param["mp"]/param["h100"]
     h, hist = read_subhalos(dir_name, include_false_selections=True)
     with open(file_name, "rb") as fp:
         n_halo, n_snap = struct.unpack("qq", fp.read(16))
         n = n_halo*n_snap
         out = np.zeros(n, dtype=CORE_DTYPE)
 
         x = np.fromfile(fp, np.float32, 3*n)
@@ -532,19 +550,24 @@
         out["m_tidal"] = np.fromfile(fp, np.float32, n)
         out["m_tidal_bound"] = np.fromfile(fp, np.float32, n)
         out["m_bound"] = np.fromfile(fp, np.float32, n)
         out["vmax"] = np.fromfile(fp, np.float32, n)
         out["f_core"] = np.fromfile(fp, np.float32, n)
         out["f_core_rs"] = np.fromfile(fp, np.float32, n)
         out["d_core_mbp"] = np.fromfile(fp, np.float32, n)
-
-        out["ok"] = out["m_bound"] > 0
+        out["ok"] = np.fromfile(fp, np.bool, n)
+        out["ok_rs"] = np.fromfile(fp, np.bool, n)
+        out["is_err"] = np.fromfile(fp, np.bool, n)
+        out["is_err_rs"] = np.fromfile(fp, np.bool, n)
+        out["interp"] = np.fromfile(fp, np.bool, n)
+       
 
     out = out.reshape((n_halo, n_snap))
 
+    """
     r_core = np.sqrt(np.sum(out["x"]**2, axis=2))
     r_rs = np.sqrt(np.sum(h["x"]**2, axis=2))
     r_core_rs = np.sqrt(np.sum((h["x"] - out["x"])**2, axis=2))
 
     out["is_err"] = (out["f_core"] == 0) | (out["r50_bound"] > r_core)
     out["is_err_rs"] = (out["f_core_rs"] == 0)|(out["r50_bound_rs"] > r_rs)
 
@@ -564,14 +587,18 @@
     has_neighbor = np.zeros(out.shape, dtype=bool)
     has_neighbor[:,:-1] = out["ok"][:,1:]
     has_neighbor[:,1:] = has_neighbor[:,1:] | out["ok"][:,:-1]
     out["ok"] = out["ok"] & has_neighbor
     recent_infall = hist["first_infall_snap"] == out.shape[1]-1
     out["ok"][recent_infall, -1] = True
 
+    scale = scale_factors(dir_name)
+    interpolate_cores(scale, out, h, hist, mp)
+    """
+
     if not include_false_selections:
         h, hist = read_subhalos(dir_name, include_false_selections=True)
         out = out[~hist["false_selection"]]
 
     return out
 
 def read_um(dir_name):
@@ -756,22 +783,18 @@
     n_merger = struct.unpack("i", f.read(4))[0]
 
     idx = np.fromfile(f, np.int32, n_merger)    
     
 class ParticleHeader(object):
     def __init__(self, base_dir):
         file_name = path.join(base_dir, "particles", "particle_header.dat")
-        ## BH: first attempt
-        #        if not file_name.is_file():
-        #           raise FileNotFoundError("The particle data for {} has not been generated.".format(file_name))
         try:
             f = open(file_name, "rb")
-        except FileNotFoundError as e:
-            # TODO: raise error here
-            print("The particle data for this halo does not exist.", e.args)
+        except FileNotFoundError:
+            raise FileNotFoundError("The particle data for this halo does not exist.") from None
         # TODO: if not working, try os.path.exists() and os.path.isfile() after that
 
         self.n_file = struct.unpack("i", f.read(4))[0]
         self.n_halo = struct.unpack("i", f.read(4))[0]
         self.n_particle = struct.unpack("i", f.read(4))[0]
         
         self.file_lengths = np.fromfile(f, np.int32, self.n_file)
@@ -856,25 +879,41 @@
 
 def is_real_confirmed(part_info, h, i_sub):
     first_snap = np.where(h[i_sub]["ok"])[0][0]
     ok = read_particles(part_info, None, first_snap, "valid", owner=i_sub)
     return np.sum(ok) > 0
 
 class Particles(object):
+    """ A wrapper for accessing particle data associated with the desired halo suite."""
     def __init__(self, sim_dir):
-        # TODO: write docstring
         self.sim_dir = sim_dir
         self.part_info = ParticleInfo(sim_dir)
         self.params = simulation_parameters(sim_dir)
         self.scale = scale_factors(sim_dir)
         self.h_cmov, _ = read_subhalos(sim_dir, comoving=True)
 
     def read(self, snap, halo=-1, mode="current", comoving=False):
-        # TODO: write docstring
-        """ mode_args: ["all", "current", "smooth"]
+        """ read returns a list of 1D arrays containing frequently used variables 
+        stored in the particle data for a given subhalo. 
+
+        Parameters
+        ----------
+        snap: int, snapshot.
+        halo: int, index for subhalo of interest, default returns all subhalos.
+        comoving: boolean, default is False to return physical units.
+        mode: string 
+            "Current" is the default setting and returns variables for valid particles.
+            "All" returns variables for all particles, valid or invalid.
+            "Smooth" returns variables for smoothly accreted particles. 
+
+        Returns
+        -------
+        p: list containing 1D arrays of the following variables from stored particle data:
+            id, x, v, snap, ok, and smooth. See PARTICLE_DTYPE for more detail.
+
         """
 
         sim_dir = self.sim_dir
         part_info = self.part_info
         h0 = self.h_cmov[0,snap]
         a = self.scale[snap]
 
@@ -898,33 +937,37 @@
                 for i in range(len(x)):
                     ok = valid[i]
                     x[i], v[i], idp[i] = x[i][ok], v[i][ok], idp[i][ok]
                     snaps[i], smooth[i] = snaps[i][ok], smooth[i][ok]
                     valid[i] = valid[i][ok]
 
         if mode == "smooth":
-            for sh in range(len(h)):
+            idp = [None]*len(self.h_cmov)
+            x = [None]*len(self.h_cmov)
+            v = [None]*len(self.h_cmov)
+            snaps = [None]*len(self.h_cmov)
+            valid = [None]*len(self.h_cmov)
+            smooth = [None]*len(self.h_cmov)
+            for sh in range(len(self.h_cmov)):
                 # A single halo read is fast for smooth particles, so we only
                 # have to read the specified halo in this mode
                 if halo != -1 and sh != halo: continue
-                idp = read_particles(part_info, sim_dir, snap, "id", owner=sh)
-                x = read_particles(part_info, sim_dir, snap, "x", owner=sh)
-                v = read_particles(part_info, sim_dir, snap, "v", owner=sh)
+                idp[sh] = read_particles(part_info, sim_dir, snap, "id", owner=sh)
+                x[sh] = read_particles(part_info, sim_dir, snap, "x", owner=sh)
+                v[sh] = read_particles(part_info, sim_dir, snap, "v", owner=sh)
                 if not comoving:
-                    x[s] = util.set_units_x(x[s], h0, a, self.params)
-                    v[s] = util.set_units_v(v[s], h0, a, self.params)
+                    x[sh] = util.set_units_x(x[sh], h0, a, self.params)
+                    v[sh] = util.set_units_v(v[sh], h0, a, self.params)
             
-                snaps = read_particles(part_info, sim_dir, snap,
-                                       "snap", owner=sh)
-                valid = read_particles(part_info, sim_dir, snap,
-                                       "valid", owner=sh)
-                smooth = read_particles(part_info, sim_dir, snap,
-                                        "ownership", owner=sh)
-
-
+                snaps[sh] = read_particles(part_info, sim_dir, snap,
+                                           "snap", owner=sh)
+                valid[sh] = read_particles(part_info, sim_dir, snap,
+                                           "valid", owner=sh)
+                smooth[sh] = read_particles(part_info, sim_dir, snap,
+                                            "ownership", owner=sh)
         p = [None]*len(x)
         for i in range(len(x)):
             if halo == -1 or i == halo:
                 p[i] = np.zeros(len(x[i]), dtype=PARTICLE_DTYPE)
                 p[i]["id"] = idp[i]
                 p[i]["x"] = x[i]
                 p[i]["v"] = v[i]
@@ -933,16 +976,17 @@
                 p[i]["smooth"] = smooth[i] == 0
 
         if halo == -1:
             return p 
         else:
             return p[halo]
 
-
     def core_particles(self, snap, halo=-1, comoving=False):
+        """ TODO: write docstring
+        """
         pass
 
 def read_particles(part_info, base_dir, snap, var_name,
                    owner=None, include_false_selections=False):
     hd, tags = part_info.part_hd, part_info.tags
     
     h_idx = np.arange(len(part_info.hist_false), dtype=int)
```

### Comparing `symlib-1.2.9/symlib/star_tagging.py` & `symlib-1.3.0/symlib/star_tagging.py`

 * *Files identical despite different names*

### Comparing `symlib-1.2.9/symlib/util.py` & `symlib-1.3.0/symlib/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 def set_units_histories(hist, scale, param):
     """ set_units_histories takes an array of type HISTORY_DTYPE and returns a
     copy with units that have been converted from Rockstar's detail units to
     symlib's default units: Msun, physical kpc, and physical km/s.
     """
     hist = np.copy(hist)
     hist["mpeak"] /= param["h100"]
+    hist["mpeak_pre"] /= param["h100"]
     return hist
 
 def set_units_halos(h, scale, param):
     """ set_units_halos takes a array of type SUBHALO_DTYPE and returns a copy
     with units that have been converted from Rockstar's default units to
     symlib's default units, Msun, physical kpc centered on the host halo,
     and physical km/s centered on the host halo.
```

### Comparing `symlib-1.2.9/symlib.egg-info/PKG-INFO` & `symlib-1.3.0/symlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.2.9
+Version: 1.3.0
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

