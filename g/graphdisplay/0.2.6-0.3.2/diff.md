# Comparing `tmp/graphdisplay-0.2.6.tar.gz` & `tmp/graphdisplay-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.2.6.tar", last modified: Fri May  5 19:07:53 2023, max compression
+gzip compressed data, was "graphdisplay-0.3.2.tar", last modified: Sat May  6 17:32:44 2023, max compression
```

## Comparing `graphdisplay-0.2.6.tar` & `graphdisplay-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:07:53.932468 graphdisplay-0.2.6/
--rw-rw-rw-   0        0        0     1051 2023-05-05 19:07:53.931471 graphdisplay-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-05-02 18:43:09.000000 graphdisplay-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 19:07:53.920520 graphdisplay-0.2.6/graphdisplay/
--rw-rw-rw-   0        0        0       60 2023-05-03 20:40:03.000000 graphdisplay-0.2.6/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0    12228 2023-05-05 19:07:33.000000 graphdisplay-0.2.6/graphdisplay/graph.py
--rw-rw-rw-   0        0        0    16032 2023-05-05 19:05:58.000000 graphdisplay-0.2.6/graphdisplay/graphdisplay.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:07:53.930475 graphdisplay-0.2.6/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     1051 2023-05-05 19:07:53.000000 graphdisplay-0.2.6/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-05 19:07:53.000000 graphdisplay-0.2.6/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:07:53.000000 graphdisplay-0.2.6/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 19:07:53.000000 graphdisplay-0.2.6/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 19:07:53.932468 graphdisplay-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1322 2023-05-05 19:07:49.000000 graphdisplay-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:32:44.443505 graphdisplay-0.3.2/
+-rw-rw-rw-   0        0        0     5408 2023-05-06 17:32:44.442554 graphdisplay-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4753 2023-05-06 17:15:34.000000 graphdisplay-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 17:32:44.428066 graphdisplay-0.3.2/graphdisplay/
+-rw-rw-rw-   0        0        0       60 2023-05-03 20:40:03.000000 graphdisplay-0.3.2/graphdisplay/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-05-06 17:02:49.000000 graphdisplay-0.3.2/graphdisplay/general_config.py
+-rw-rw-rw-   0        0        0     3483 2023-05-06 17:26:05.000000 graphdisplay-0.3.2/graphdisplay/graph.py
+-rw-rw-rw-   0        0        0    15740 2023-05-06 17:31:26.000000 graphdisplay-0.3.2/graphdisplay/graphdisplay.py
+-rw-rw-rw-   0        0        0     4904 2023-05-06 17:29:34.000000 graphdisplay-0.3.2/graphdisplay/json_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:32:44.441003 graphdisplay-0.3.2/graphdisplay/store/
+-rw-rw-rw-   0        0        0        0 2023-05-06 17:02:49.000000 graphdisplay-0.3.2/graphdisplay/store/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:32:44.440006 graphdisplay-0.3.2/graphdisplay.egg-info/
+-rw-rw-rw-   0        0        0     5408 2023-05-06 17:32:44.000000 graphdisplay-0.3.2/graphdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-06 17:32:44.000000 graphdisplay-0.3.2/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 17:32:44.000000 graphdisplay-0.3.2/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 17:32:44.000000 graphdisplay-0.3.2/graphdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:32:44.443505 graphdisplay-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1322 2023-05-06 17:32:42.000000 graphdisplay-0.3.2/setup.py
```

### Comparing `graphdisplay-0.2.6/graphdisplay/graphdisplay.py` & `graphdisplay-0.3.2/graphdisplay/graphdisplay.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tkinter as tk
-import json
 import math
-import os
+from .json_manager import JsonManager
+from .general_config import *
 
 class GraphGUI:
 
     instance = 0
 
     def __new__(cls, graph, node_radius: int = 40, scr_width: int = 600, scr_height: int = 600):
         GraphGUI.instance += 1
@@ -36,81 +36,81 @@
                 raise ValueError("The parameter node_radius must be a value between 10 and 100")
             if scr_width < 200 or scr_height < 200:
                 raise ValueError("The parameters scr_width and scr_height must be values greater than 200")
             if scr_width > 1000 or scr_height > 1000:
                 raise ValueError("The parameters scr_width and scr_height must be values less than 1000")
 
             self.__ACTUAL_INSTANCE = instance
-            self.__JSON_SAVE_DIR = os.path.join(os.path.dirname(__file__), 'save'+str(self.__ACTUAL_INSTANCE)+'.json')
             self.__graph = graph
             self.__node_radius = node_radius
             self.__scr_width = scr_width
             self.__scr_height = scr_height
             self.__XMARGIN = 7
             self.__YMARGIN = 7
             self.nodes = []
             self.edges = []
 
             # create the main window and start the GUI
             self.root = tk.Tk()
             self.root.title('GraphGUI')
             self.root.resizable(False, False)
-            self.root.configure(bg="#87715f", border=0, width=self.__scr_width, height=self.__scr_height)
+            self.root.configure(bg=FRAME_COLOR, border=0, width=self.__scr_width, height=self.__scr_height)
+
+            self.json_manager = JsonManager(self.root, self)
 
             # Closing protocol
             self.root.protocol("WM_DELETE_WINDOW", self.__on_closing)
 
-            # Data recovery
-            data = self.__get_data()
-
-            # Create the canvas
-            #self.canvas = tk.Canvas(self.root, width=scr_width, height=scr_height, bg="#c7b9a5")
-            #self.canvas.pack(fill=tk.BOTH, expand=True, padx=7, pady=7)
-
-            self.canvas = tk.Canvas(self.root, bg="#c7b9a5")
+            self.canvas = tk.Canvas(self.root, bg=BACKGROUND_CANVAS_COLOR)
             self.canvas.place(x=self.__XMARGIN,
                               y=self.__YMARGIN,
                               width=self.__scr_width - self.__XMARGIN * 2,
                               height=self.__scr_height - self.__YMARGIN * 2 - 30)
 
             # Reset button
-            self.reset_button = tk.Button(self.root, text="Reset", bg="#ede4cc", command=self.__display_reset)
+            self.reset_button = tk.Button(self.root, text="Reset", bg=BUTTON_COLOR, command=self.display_reset)
             self.reset_button.place(x=self.__XMARGIN, y=self.__scr_height-self.__YMARGIN//2-30, width=60, height=30)
 
-            """options = ["Dijkstra", "Prim", "Kruskal"]
-            self.__selection = tk.StringVar(self.root)
-            self.__selection.set(options[0])
-
             # Load button
-            self.load_button = tk.Button(self.root, text="Load", bg="#ede4cc")
+            self.load_button = tk.Button(self.root, text="Load", bg=BUTTON_COLOR, command=self.__call_manager_load)
             self.load_button.place(x=self.__XMARGIN + 60 + 7, y=self.__scr_height - self.__YMARGIN // 2 - 30, width=60,
                                     height=30)
-            self.load_button_options = tk.OptionMenu(self.root, self.__selection, *options)
 
             # Save button
-            self.save_button = tk.Button(self.root, text="Save", bg="#ede4cc")
+            self.save_button = tk.Button(self.root, text="Save", bg=BUTTON_COLOR, command=self.__call_manager_save)
             self.save_button.place(x=self.__XMARGIN + 60 + 60 + 7 + 7, y=self.__scr_height - self.__YMARGIN // 2 - 30, width=60,
                                     height=30)
-            self.save_button_options = tk.OptionMenu(self.root, self.__selection, *options)"""
 
             # Main display
+            data = self.json_manager.get_data('save'+str(self.__ACTUAL_INSTANCE))
             self.__display(data)
 
             self.canvas.tag_bind("movil", "<ButtonPress-1>", self.on_press)
             self.canvas.tag_bind("movil", "<Button1-Motion>", self.move)
             self.selected_node = None
 
             self.root.mainloop()
 
-        def __display_reset(self):
+        def __call_manager_load(self):
+            new_position = self.json_manager.generate_load_window()
+            if new_position:
+                self.display_reset(new_position)
+
+        def __call_manager_save(self):
+            curr_pos = {}
+            for node in self.nodes:
+                curr_pos[node.id] = (node.pos_x, node.pos_y)
+            self.json_manager.generate_save_window(curr_pos)
+
+        def display_reset(self, new_data: dict = None):
             for node in self.nodes:
                 node.terminate()
             for edge in self.edges:
                 edge.terminate()
-            self.__display()
+            self.__display(new_data)
 
         def __display(self, data: dict = None):
             # Preparation for the nodes display
             scr_center = (self.__scr_width // 2, self.__scr_height // 2)
             display_radius = min(self.__scr_width, self.__scr_height) // 2 - self.__node_radius - 10
             arch_angle = 360 / len(self.__graph._vertices)
             first_node_pos = (scr_center[0] - self.__node_radius, scr_center[1] - self.__node_radius)
@@ -152,16 +152,16 @@
 
             # Create the edges
             i = 0
             self.edges = []
             for vertex in self.__graph._vertices:
                 for adj in self.__graph._vertices[vertex]:
                     for node in self.nodes:
-                        if node.id == adj.vertex:
-                            self.edges.append(Edge(self.canvas, self.nodes[i], node, adj.weight))
+                        if node.id == adj._vertex:
+                            self.edges.append(Edge(self.canvas, self.nodes[i], node, adj._weight if adj._weight else 1))
                             node.asociated_edges_IN.append(self.edges[-1])
                             self.nodes[i].asociated_edges_OUT.append(self.edges[-1])
                 i += 1
 
             # Display the edges
             if self.__graph._directed:
                 for edge in self.edges:
@@ -177,33 +177,24 @@
                     if not found:
                         edge.show()
             else:
                 for edge in self.edges:
                     edge.show()
 
             # Display author
-            self.canvas.create_text(self.__scr_width // 2, self.__YMARGIN + 3, text="by @seniorbeto", fill="#695210",
+            self.canvas.create_text(self.__scr_width // 2, self.__YMARGIN + 3, text="by @seniorbeto", fill=FRAME_COLOR,
                                     font=("Courier", 10))
 
         def __on_closing(self):
             data = {}
             for node in self.nodes:
                 data[node.id] = (node.pos_x, node.pos_y)
-            with open(self.__JSON_SAVE_DIR, "w", encoding="utf-8", newline="") as file:
-                json.dump(data, file, indent=2)
+            self.json_manager.save_data('save'+str(self.__ACTUAL_INSTANCE), data)
             self.root.destroy()
 
-        def __get_data(self):
-            try:
-                with open(self.__JSON_SAVE_DIR, "r", encoding="utf-8", newline="") as file:
-                    data = json.load(file)
-            except FileNotFoundError:
-                data = None
-            return data
-
         def on_press(self, event):
             node = self.canvas.find_withtag(tk.CURRENT)
             self.selected_node = (node, event.x, event.y)
 
         def move(self, event):
             x, y = event.x, event.y
             node, x0, y0 = self.selected_node
@@ -222,15 +213,15 @@
                         self.canvas.delete(edge.window)
                         del edge
                         edge = Edge(self.canvas, edge_start, i, weight, overlaped=overlaped)
                         edge.show()
                         i.asociated_edges_IN.append(edge)
                     for adj in self.__graph._vertices[i.id]:
                         for nd in self.nodes:
-                            if nd.id == adj.vertex:
+                            if nd.id == adj._vertex:
                                 for edge in nd.asociated_edges_IN:
                                     if edge.start_node == i:
                                         edge_end = edge.end_node
                                         weight = edge.weight
                                         overlaped = edge.overlaped
                                         nd.asociated_edges_IN.remove(edge)
                                         self.canvas.delete(edge.line)
@@ -240,15 +231,15 @@
                                         edge.show()
                                         nd.asociated_edges_IN.append(edge)
 
 
             self.selected_node = (node, x, y)
 
 class Node:
-    def __init__(self, canvas: tk.Canvas, radius:int, posx: int, posy: int, text: str, bg: str = "#e3d7c5"):
+    def __init__(self, canvas: tk.Canvas, radius:int, posx: int, posy: int, text: str, bg: str = VERTEX_COLOR):
         self.asociated_edges_IN = []
         self.asociated_edges_OUT = []
         self.canvas = canvas
         self.id = text
         self.radius = radius
         self.pos_x = posx
         self.pos_y = posy
@@ -278,19 +269,19 @@
         self.canvas.delete(self.line)
         self.canvas.delete(self.window)
 
     def show(self):
         self.line = self.canvas.create_line(self.start[0], self.start[1], self.end[0], self.end[1], arrow=tk.LAST, width=1.5)
         if not self.overlaped:
             self.window = self.canvas.create_window((self.start[0] + self.end[0]) // 2, (self.start[1] + self.end[1]) // 2,
-                                               window=tk.Label(self.canvas,bg="#c7b9a5" ,text=str(self.weight)))
+                                               window=tk.Label(self.canvas,bg=BACKGROUND_CANVAS_COLOR ,text=str(self.weight)))
         else:
             self.window = self.canvas.create_window((self.start[0] * 0.2 + self.end[0] * 0.8),
                                                (self.start[1] * 0.2 + self.end[1] * 0.8),
-                                               window=tk.Label(self.canvas, bg="#c7b9a5", text=str(self.weight)))
+                                               window=tk.Label(self.canvas, bg=BACKGROUND_CANVAS_COLOR, text=str(self.weight)))
 
     def __calculate_start(self, start: Node, end: Node) -> tuple:
         """
         It calculates the initial position of the arrow that connects the nodes "start" and "end"
         :param start: Node
         :param end: Node
         :return: tuple with the initial position of the arrow
```

### Comparing `graphdisplay-0.2.6/setup.py` & `graphdisplay-0.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.2.6'
+VERSION = '0.3.2'
 PACKAGE_NAME = 'graphdisplay'
 AUTHOR = 'Alberto Penas Díaz'
 AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com'
 URL = 'https://github.com/seniorbeto'
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para representar visualmente grafos de tipo diccionario'
```

