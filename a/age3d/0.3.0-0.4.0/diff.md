# Comparing `tmp/age3d-0.3.0.tar.gz` & `tmp/age3d-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "age3d-0.3.0.tar", last modified: Mon May  1 04:38:56 2023, max compression
+gzip compressed data, was "age3d-0.4.0.tar", last modified: Sat May  6 06:14:19 2023, max compression
```

## Comparing `age3d-0.3.0.tar` & `age3d-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.463701 age3d-0.3.0/
--rw-rw-rw-   0        0        0      294 2023-05-01 04:33:59.000000 age3d-0.3.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0      493 2023-04-04 09:58:38.000000 age3d-0.3.0/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1114 2023-03-26 00:42:17.000000 age3d-0.3.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11357 2023-03-24 19:50:45.000000 age3d-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      644 2023-04-05 00:11:10.000000 age3d-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2570 2023-04-04 09:58:38.000000 age3d-0.3.0/Makefile
--rw-rw-rw-   0        0        0    17220 2023-05-01 04:38:56.462695 age3d-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3132 2023-04-04 09:58:38.000000 age3d-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.328187 age3d-0.3.0/age3d/
--rw-rw-rw-   0        0        0      339 2023-03-25 23:20:12.000000 age3d-0.3.0/age3d/__init__.py
--rw-rw-rw-   0        0        0     1215 2023-03-25 23:20:12.000000 age3d-0.3.0/age3d/__main__.py
--rw-rw-rw-   0        0        0       22 2023-05-01 04:33:59.000000 age3d-0.3.0/age3d/_version.py
--rw-rw-rw-   0        0        0    17283 2023-05-01 04:33:59.000000 age3d-0.3.0/age3d/age3d.py
--rw-rw-rw-   0        0        0    17586 2023-04-04 11:40:52.000000 age3d-0.3.0/age3d/examples.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.362158 age3d-0.3.0/age3d/models/
--rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.3.0/age3d/models/monkey.stl
--rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.3.0/age3d/models/monkey_cleaned.stl
-drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.369156 age3d-0.3.0/age3d/tests/
--rw-rw-rw-   0        0        0    11744 2023-03-25 23:20:12.000000 age3d-0.3.0/age3d/tests/monkey_triangles.npy
--rw-rw-rw-   0        0        0    68912 2023-03-25 23:20:12.000000 age3d-0.3.0/age3d/tests/monkey_vertices.npy
--rw-rw-rw-   0        0        0     7171 2023-05-01 04:33:59.000000 age3d-0.3.0/age3d/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.357153 age3d-0.3.0/age3d.egg-info/
--rw-rw-rw-   0        0        0    17220 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.431706 age3d-0.3.0/docs/
--rw-rw-rw-   0        0        0      683 2023-04-04 06:54:19.000000 age3d-0.3.0/docs/Makefile
--rw-rw-rw-   0        0        0     1209 2023-04-04 06:54:19.000000 age3d-0.3.0/docs/conf.py
--rw-rw-rw-   0        0        0       96 2023-04-04 06:54:19.000000 age3d-0.3.0/docs/documentation.rst
--rw-rw-rw-   0        0        0    14680 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/examples.rst
--rw-rw-rw-   0        0        0     1340 2023-04-29 06:53:06.000000 age3d-0.3.0/docs/getting_started.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.459707 age3d-0.3.0/docs/img/
--rw-rw-rw-   0        0        0    63875 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey.png
--rw-rw-rw-   0        0        0    69385 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_below_above_between.png
--rw-rw-rw-   0        0        0   100655 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_bound_height.png
--rw-rw-rw-   0        0        0    81498 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_erode.png
--rw-rw-rw-   0        0        0   127495 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_erode_wireframe.png
--rw-rw-rw-   0        0        0    64955 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_min_max.png
--rw-rw-rw-   0        0        0    58693 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_neighbors.png
--rw-rw-rw-   0        0        0    67341 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_pc.png
--rw-rw-rw-   0        0        0   125751 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_subdivision.png
--rw-rw-rw-   0        0        0    73476 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_wireframe.png
--rw-rw-rw-   0        0        0      454 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/index.rst
--rwxrwxrwx   0        0        0      765 2023-04-04 06:54:19.000000 age3d-0.3.0/docs/make.bat
--rw-rw-rw-   0        0        0     2214 2023-05-01 04:33:59.000000 age3d-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 04:38:56.463701 age3d-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-24 19:50:45.000000 age3d-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:14:19.805830 age3d-0.4.0/
+-rw-rw-rw-   0        0        0      294 2023-05-06 04:54:45.000000 age3d-0.4.0/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      493 2023-05-06 06:03:00.000000 age3d-0.4.0/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1114 2023-03-26 00:42:17.000000 age3d-0.4.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11357 2023-03-24 19:50:45.000000 age3d-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      644 2023-05-06 06:03:00.000000 age3d-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2570 2023-04-04 09:58:38.000000 age3d-0.4.0/Makefile
+-rw-rw-rw-   0        0        0    17220 2023-05-06 06:14:19.803828 age3d-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3132 2023-04-04 09:58:38.000000 age3d-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 06:14:19.718777 age3d-0.4.0/age3d/
+-rw-rw-rw-   0        0        0      360 2023-05-06 04:54:45.000000 age3d-0.4.0/age3d/__init__.py
+-rw-rw-rw-   0        0        0     1215 2023-03-25 23:20:12.000000 age3d-0.4.0/age3d/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-05-06 04:54:45.000000 age3d-0.4.0/age3d/_version.py
+-rw-rw-rw-   0        0        0    19415 2023-05-06 04:54:45.000000 age3d-0.4.0/age3d/age3d.py
+-rw-rw-rw-   0        0        0    22588 2023-05-06 04:54:45.000000 age3d-0.4.0/age3d/examples.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-06 06:14:19.755830 age3d-0.4.0/age3d/models/
+-rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.4.0/age3d/models/monkey.stl
+-rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.4.0/age3d/models/monkey_cleaned.stl
+drwxrwxrwx   0        0        0        0 2023-05-06 06:14:19.762833 age3d-0.4.0/age3d/tests/
+-rw-rw-rw-   0        0        0    11744 2023-03-25 23:20:12.000000 age3d-0.4.0/age3d/tests/monkey_triangles.npy
+-rw-rw-rw-   0        0        0    68912 2023-03-25 23:20:12.000000 age3d-0.4.0/age3d/tests/monkey_vertices.npy
+-rw-rw-rw-   0        0        0     7898 2023-05-06 04:54:45.000000 age3d-0.4.0/age3d/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:14:19.750828 age3d-0.4.0/age3d.egg-info/
+-rw-rw-rw-   0        0        0    17220 2023-05-06 06:14:19.000000 age3d-0.4.0/age3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-05-06 06:14:19.000000 age3d-0.4.0/age3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 06:14:19.000000 age3d-0.4.0/age3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-05-06 06:14:19.000000 age3d-0.4.0/age3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 06:14:19.000000 age3d-0.4.0/age3d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 06:14:19.775829 age3d-0.4.0/docs/
+-rw-rw-rw-   0        0        0      683 2023-04-04 06:54:19.000000 age3d-0.4.0/docs/Makefile
+-rw-rw-rw-   0        0        0     1209 2023-04-04 06:54:19.000000 age3d-0.4.0/docs/conf.py
+-rw-rw-rw-   0        0        0       96 2023-04-04 06:54:19.000000 age3d-0.4.0/docs/documentation.rst
+-rw-rw-rw-   0        0        0     9113 2023-05-06 04:52:55.000000 age3d-0.4.0/docs/examples.rst
+-rw-rw-rw-   0        0        0     1340 2023-04-29 06:53:06.000000 age3d-0.4.0/docs/getting_started.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 06:14:19.801829 age3d-0.4.0/docs/img/
+-rw-rw-rw-   0        0        0    63875 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey.png
+-rw-rw-rw-   0        0        0   133031 2023-05-06 04:54:45.000000 age3d-0.4.0/docs/img/monkey_accessible.png
+-rw-rw-rw-   0        0        0    69385 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey_below_above_between.png
+-rw-rw-rw-   0        0        0   100655 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey_bound_height.png
+-rw-rw-rw-   0        0        0    81498 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey_erode.png
+-rw-rw-rw-   0        0        0   102027 2023-05-06 04:54:45.000000 age3d-0.4.0/docs/img/monkey_erode_direction.png
+-rw-rw-rw-   0        0        0   127495 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey_erode_wireframe.png
+-rw-rw-rw-   0        0        0   138074 2023-05-06 04:54:45.000000 age3d-0.4.0/docs/img/monkey_erode_wireframe_direction.png
+-rw-rw-rw-   0        0        0    64955 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey_min_max.png
+-rw-rw-rw-   0        0        0    58693 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey_neighbors.png
+-rw-rw-rw-   0        0        0    67341 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey_pc.png
+-rw-rw-rw-   0        0        0   125751 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey_subdivision.png
+-rw-rw-rw-   0        0        0    73476 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/img/monkey_wireframe.png
+-rw-rw-rw-   0        0        0      454 2023-04-04 11:40:52.000000 age3d-0.4.0/docs/index.rst
+-rwxrwxrwx   0        0        0      765 2023-04-04 06:54:19.000000 age3d-0.4.0/docs/make.bat
+-rw-rw-rw-   0        0        0     2214 2023-05-06 05:04:37.000000 age3d-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 06:14:19.806830 age3d-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-24 19:50:45.000000 age3d-0.4.0/setup.py
```

### Comparing `age3d-0.3.0/CONTRIBUTING.md` & `age3d-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/LICENSE` & `age3d-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/MANIFEST.in` & `age3d-0.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/Makefile` & `age3d-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/PKG-INFO` & `age3d-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age3d
-Version: 0.3.0
+Version: 0.4.0
 Summary: Aging 3D models
 Author-email: Abhishek Chaudhary <ac5003@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `age3d-0.3.0/README.md` & `age3d-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/age3d/__main__.py` & `age3d-0.4.0/age3d/__main__.py`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/age3d/age3d.py` & `age3d-0.4.0/age3d/age3d.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 def export_mesh(file_path: str, mesh):
     """
     Export a mesh to a given file path using the open3d library.
 
     Args:
         file_path (str): The file path where the mesh will be saved.
+
         mesh: The mesh to be exported.
 
     Returns:
         None
     """
     o3d.io.write_triangle_mesh(file_path, mesh)
     return
@@ -53,25 +54,26 @@
     Retrieve details of a mesh in the form of numpy arrays for vertices and triangles.
 
     Args:
         mesh: The mesh for which the details are to be extracted.
 
     Returns:
         tuple: A tuple of two numpy arrays. The first array contains the vertices of the mesh
-               and the second array contains the triangles of the mesh.
+        and the second array contains the triangles of the mesh.
     """
     return (np.asarray(mesh.vertices), np.asarray(mesh.triangles))
 
 
 def visualize(entries, show_wireframe=False) -> None:
     """
     Visualize a single mesh or a list of meshes using the open3d library.
 
     Args:
         entries: The mesh/meshes to be visualized. It can be a single mesh or a list of meshes.
+
         show_wireframe (bool): A flag to show/hide the wireframe of the mesh/meshes.
 
     Returns:
         None
     """
     if type(entries) is not list:
         o3d.visualization.draw_geometries([entries], mesh_show_wireframe=show_wireframe)
@@ -82,14 +84,15 @@
 
 def get_mask(mesh, idx):
     """
     Create a mask array for a specific vertex of the mesh.
 
     Args:
         mesh: The mesh for which the mask is to be created.
+
         idx: The index of the vertex for which the mask is to be created.
 
     Returns:
         np.ndarray: A boolean mask array with True value for the given index and False for all
                     other vertices of the mesh.
     """
     mask = np.full(np.asarray(mesh.vertices).shape[0], False)
@@ -99,15 +102,17 @@
 
 def find_minimum(mesh, k: int = 1, idx_mask=[]):
     """
     Find the k number of vertices having minimum z-coordinate of a mesh.
 
     Args:
         mesh (open3d.geometry.TriangleMesh): The input mesh.
+
         k (int, optional):: The number of minimum vertices to be found.
+
         idx_mask (list, optional): A list of indices of vertices to be considered for finding minimum vertices.
 
     Returns:
         tuple: A tuple of two numpy arrays. The first array contains the indices of the minimum
                vertices and the second array contains the coordinates of the minimum vertices.
     """
     mesh_vertices_np = np.asarray(mesh.vertices)
@@ -129,15 +134,17 @@
 
 def find_maximum(mesh, k: int = 1, idx_mask=[]):
     """
     Finds the maximum value(s) and corresponding index(s) in the z-coordinate of the mesh's vertices.
 
     Args:
         mesh (open3d.geometry.TriangleMesh): The input mesh.
+
         k (int, optional): The number of maximum values to return. Defaults to 1.
+
         idx_mask (list, optional): List of vertex indices to consider for the maximum search. Defaults to empty list.
 
     Returns:
         tuple: Two numpy arrays, one containing the index(s) of the maximum value(s) and the other containing
         the maximum value(s) in the z-coordinate of the mesh's vertices.
     """
     mesh_vertices_np = np.asarray(mesh.vertices)
@@ -159,15 +166,17 @@
 
 def find_all_below(mesh, value: float, inclusive=False):
     """
     Finds all the vertices below the given value in the z-coordinate.
 
     Args:
         mesh (open3d.geometry.TriangleMesh): The input mesh.
+
         value (float): The value below which to find vertices.
+
         inclusive (bool, optional): Whether to include vertices with value equal to the given value. Defaults to False.
 
     Returns:
         tuple: Two numpy arrays, one containing the indices and the other containing the vertices that are below the
         given value in the z-coordinate.
     """
     mesh_vertices_np = np.asarray(mesh.vertices)
@@ -190,15 +199,17 @@
 
 def find_all_above(mesh, value: float, inclusive=False):
     """
     Finds all the vertices above the given value in the z-coordinate.
 
     Args:
         mesh (open3d.geometry.TriangleMesh): The input mesh.
+
         value (float): The value above which to find vertices.
+
         inclusive (bool, optional): Whether to include vertices with value equal to the given value. Defaults to False.
 
     Returns:
         tuple: Two numpy arrays, one containing the indices and the other containing the vertices that are above the
         given value in the z-coordinate.
     """
     mesh_vertices_np = np.asarray(mesh.vertices)
@@ -221,15 +232,17 @@
 
 def find_all_between(mesh, lower_value: float, higher_value: float) -> np.ndarray:
     """
     Returns a NumPy array of vertices whose z-coordinate is between the given lower and higher values.
 
     Args:
         mesh (open3d.geometry.TriangleMesh): A triangle mesh object.
+
         lower_value (float): The lower bound of the z-coordinate.
+
         higher_value (float): The higher bound of the z-coordinate.
 
     Returns:
         np.ndarray: A NumPy array of vertices whose z-coordinate is between the given lower and higher values.
     """
     mesh_vertices_np = np.asarray(mesh.vertices)
     # print(mesh_vertices_np, type(mesh.vertices))
@@ -243,14 +256,15 @@
 
 def make_point_cloud(vertices, color):
     """
     Creates a point cloud object with the given vertices and color.
 
     Args:
         vertices (np.ndarray): A NumPy array of vertices.
+
         color (tuple): A tuple of RGB values (0-255).
 
     Returns:
         open3d.geometry.PointCloud: A point cloud object.
     """
     pc = o3d.geometry.PointCloud()
     pc.points = o3d.utility.Vector3dVector(vertices)
@@ -260,14 +274,15 @@
 
 def find_neighbors(mesh, index: int):
     """
     Returns the indices and coordinates of the neighboring vertices of the given vertex index.
 
     Args:
         mesh (open3d.geometry.TriangleMesh): A triangle mesh object.
+
         index (int): The index of the vertex.
 
     Returns:
         Tuple[np.ndarray, np.ndarray]: A tuple of two NumPy arrays
         representing the neighboring vertex indices and coordinates.
     """
     mesh_triangles_np = np.asarray(mesh.triangles)
@@ -283,14 +298,15 @@
 
 def mesh_subdivision(mesh, iterations=1):
     """
     Returns a new triangle mesh object obtained by subdividing the given mesh.
 
     Args:
         mesh (open3d.geometry.TriangleMesh): A triangle mesh object.
+
         iterations (int): The number of times to subdivide the mesh.
 
     Returns:
         open3d.geometry.TriangleMesh: A new triangle mesh object obtained by subdividing the given mesh.
     """
     return mesh.subdivide_midpoint(number_of_iterations=iterations)
 
@@ -310,22 +326,76 @@
     max_x_vertex = mesh_vertices_np[np.argmin(mesh_vertices_np[:, 0])]
     min_y_vertex = mesh_vertices_np[np.argmin(mesh_vertices_np[:, 1])]
     max_y_vertex = mesh_vertices_np[np.argmin(mesh_vertices_np[:, 1])]
 
     return min(min_x_vertex[2], max_x_vertex[2], min_y_vertex[2], max_y_vertex[2])
 
 
-def erode(mesh: o3d.geometry.TriangleMesh, iterations: int = 2, erosion_lifetime: int = 10, verbose: list = []):
+def find_accessible(mesh, rain_direction):
+    """
+    Returns the indices and coordinates of the vertices accessible by a given angle of particles' direction.
+
+    Args:
+        mesh (open3d.geometry.TriangleMesh): The mesh to check.
+
+        rain_direction (numpy.ndarray): The direction angle of the rain as a numpy array of shape (3,).
+            If direction is [0,0,0], every vertex is chosen.
+
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: A tuple of two NumPy arrays
+        representing the neighboring vertex indices and coordinates.
+    """
+    rain_direction = np.asarray(rain_direction)
+    # if rain_direction[2] == 0:
+    #     return np.array([]), np.array([])
+    raycast_angle = rain_direction * -1
+    # print(raycast_angle, type(rain_direction))
+    mesh_vertices_np = np.asarray(mesh.vertices)
+
+    angle_np = np.full(mesh_vertices_np.shape, raycast_angle)
+    ray_np = np.append(mesh_vertices_np, angle_np, axis=1)
+
+    rays = o3d.core.Tensor(ray_np, dtype=o3d.core.Dtype.Float32)
+    # print('ray', rays)
+    rays[:, 0] += 1e-6 * np.sign(raycast_angle[0])
+    rays[:, 1] += 1e-6 * np.sign(raycast_angle[1])
+    rays[:, 2] += 1e-6 * np.sign(raycast_angle[2])
+
+    # print('ray added', rays)
+    raycasting_scene = o3d.t.geometry.RaycastingScene()
+    mesh_legacy = o3d.t.geometry.TriangleMesh.from_legacy(mesh)
+    _ = raycasting_scene.add_triangles(mesh_legacy)
+    collision = raycasting_scene.cast_rays(rays)
+
+    idx = []
+    res = []
+    collisions_hit = collision['t_hit'].numpy()
+    # print('hit', collisions_hit)
+
+    for v, vertex in enumerate(mesh_vertices_np):
+        if collisions_hit[v] == np.inf:
+            idx.append(v)
+            res.append(vertex)
+    return np.array(idx), np.array(res).reshape((-1, 3))
+
+
+def erode(mesh: o3d.geometry.TriangleMesh, iterations: int = 2, erosion_lifetime: int = 10, direction=None, verbose=[]):
     """
     Erodes the mesh using the particle deposition and erosion method.
 
     Args:
         mesh (open3d.geometry.TriangleMesh): The mesh to be eroded.
+
         iterations (int, optional): The number of iterations for the erosion process. Defaults to 2.
+
         erosion_lifetime (int, optional): The maximum number of times a vertex can be eroded. Defaults to 10.
+
+        direction (numpy.ndarray, optional): The direction of the rain as a numpy array of shape (3,).
+            If not provided, the vertex mask is calculated from the mesh's bounding box. Defaults to None.
+
         verbose (list[str], optional): A list of strings containing information to be printed.
             Possible strings include 'all', 'vertex_progression', 'vector_direction',
             'vector_angle', 'ray', 'ray_scene', 'mesh', and 'collision'.
             Defaults to an empty list.
 
     Returns:
         Tuple[np.ndarray, open3d.geometry.TriangleMesh]: A tuple containing the updated vertex
@@ -342,15 +412,18 @@
         - 'collision': Prints information about the collision detection.
     """
     # total_vertex_count = np.asarray(mesh.vertices).shape[0]
     verbose = set(verbose)
     if len(verbose) > 0:
         print('Printing with Settings:', verbose)
 
-    vertices_idx, vertices = find_all_above(mesh, calculate_bounds_height(mesh), True)
+    if direction is None:
+        vertices_idx, vertices = find_all_above(mesh, calculate_bounds_height(mesh), True)
+    else:
+        vertices_idx, vertices = find_accessible(mesh, rain_direction=direction)
 
     set_vertices_idx = set()
     for idx in vertices_idx:
         set_vertices_idx.add(idx)
     # print('set', set_vertices_idx)
 
     # Create New Mesh
@@ -373,15 +446,15 @@
         strength = 0.5
         v_idx_prev = None
 
         while lifetime < erosion_lifetime:
             neighbors_idx, _ = find_neighbors(new_mesh, v_idx_curr)
             v_idx_next = int(find_minimum(new_mesh, 1, neighbors_idx)[0])
 
-            if v_idx_next not in vertices_idx:
+            if v_idx_next not in vertices_idx and direction is None:
                 break
 
             if v_idx_prev:
                 if 'vertex_progression' in verbose or 'all' in verbose:
                     print(
                         'Vertex Triples:',
                         v_idx_prev,
```

### Comparing `age3d-0.3.0/age3d/models/monkey.stl` & `age3d-0.4.0/age3d/models/monkey.stl`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/age3d/models/monkey_cleaned.stl` & `age3d-0.4.0/age3d/models/monkey_cleaned.stl`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/age3d/tests/monkey_triangles.npy` & `age3d-0.4.0/age3d/tests/monkey_triangles.npy`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/age3d/tests/monkey_vertices.npy` & `age3d-0.4.0/age3d/tests/monkey_vertices.npy`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/age3d/tests/test_all.py` & `age3d-0.4.0/age3d/tests/test_all.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,16 +181,33 @@
     mesh.vertices = o3d.utility.Vector3dVector(vertices)
     mesh.triangles = o3d.utility.Vector3iVector(triangles)
     v_idx, vertices = age3d.find_neighbors(mesh, 0)
 
     assert all(v_idx == [1, 2])
 
 
+@pytest.mark.parametrize(('direction', 'output_len'), [(np.array([0, 0, 0]), 2866), (np.array([0, 0, -1]), 687)])
+def test_find_accessible(direction, output_len):
+    mesh = o3d.geometry.TriangleMesh()
+    vertices = np.load('age3d/tests/monkey_vertices.npy')
+    triangles = np.load('age3d/tests/monkey_triangles.npy')
+    mesh.vertices = o3d.utility.Vector3dVector(vertices)
+    mesh.triangles = o3d.utility.Vector3iVector(triangles)
+    v_idx, vertices = age3d.find_accessible(mesh, rain_direction=direction)
+    print('len', len(v_idx))
+    assert len(v_idx) == output_len
+
+
 @pytest.mark.parametrize(
-    ('file_path', 'verbose'), [("age3d/models/monkey.stl", ['all']), ("age3d/models/monkey.stl", [])]
+    ('file_path', 'verbose', 'direction'),
+    [
+        ("age3d/models/monkey.stl", ['all'], None),
+        ("age3d/models/monkey.stl", [], None),
+        ("age3d/models/monkey.stl", [], np.array([0, 0, -1])),
+    ],
 )
-def test_full_run(file_path, verbose):
+def test_full_run(file_path, verbose, direction):
     mesh = age3d.import_mesh(file_path)
     mesh = age3d.mesh_subdivision(mesh, 2)
-    _, new_mesh = age3d.erode(mesh, iterations=50, erosion_lifetime=10, verbose=verbose)
+    _, new_mesh = age3d.erode(mesh, iterations=20, erosion_lifetime=10, direction=direction, verbose=verbose)
 
     assert all(np.asarray(mesh.triangles).flatten() == np.asarray(new_mesh.triangles).flatten())
```

### Comparing `age3d-0.3.0/age3d.egg-info/PKG-INFO` & `age3d-0.4.0/age3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age3d
-Version: 0.3.0
+Version: 0.4.0
 Summary: Aging 3D models
 Author-email: Abhishek Chaudhary <ac5003@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `age3d-0.3.0/age3d.egg-info/SOURCES.txt` & `age3d-0.4.0/age3d.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -26,16 +26,19 @@
 docs/conf.py
 docs/documentation.rst
 docs/examples.rst
 docs/getting_started.rst
 docs/index.rst
 docs/make.bat
 docs/img/monkey.png
+docs/img/monkey_accessible.png
 docs/img/monkey_below_above_between.png
 docs/img/monkey_bound_height.png
 docs/img/monkey_erode.png
+docs/img/monkey_erode_direction.png
 docs/img/monkey_erode_wireframe.png
+docs/img/monkey_erode_wireframe_direction.png
 docs/img/monkey_min_max.png
 docs/img/monkey_neighbors.png
 docs/img/monkey_pc.png
 docs/img/monkey_subdivision.png
 docs/img/monkey_wireframe.png
```

### Comparing `age3d-0.3.0/docs/Makefile` & `age3d-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/conf.py` & `age3d-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/getting_started.rst` & `age3d-0.4.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey.png` & `age3d-0.4.0/docs/img/monkey.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey_below_above_between.png` & `age3d-0.4.0/docs/img/monkey_below_above_between.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey_bound_height.png` & `age3d-0.4.0/docs/img/monkey_bound_height.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey_erode.png` & `age3d-0.4.0/docs/img/monkey_erode.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey_erode_wireframe.png` & `age3d-0.4.0/docs/img/monkey_erode_wireframe.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey_min_max.png` & `age3d-0.4.0/docs/img/monkey_min_max.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey_neighbors.png` & `age3d-0.4.0/docs/img/monkey_neighbors.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey_pc.png` & `age3d-0.4.0/docs/img/monkey_pc.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey_subdivision.png` & `age3d-0.4.0/docs/img/monkey_subdivision.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/img/monkey_wireframe.png` & `age3d-0.4.0/docs/img/monkey_wireframe.png`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/docs/make.bat` & `age3d-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `age3d-0.3.0/pyproject.toml` & `age3d-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "age3d"
 authors = [{name = "Abhishek Chaudhary", email = "ac5003@columbia.edu"}]
 description="Aging 3D models"
 readme = "README.md"
-version = "0.3.0"
+version = "0.4.0"
 requires-python = ">=3.7"
 
 dependencies = [
     "open3d==0.16.0"
 ]
 
 classifiers = [
```

