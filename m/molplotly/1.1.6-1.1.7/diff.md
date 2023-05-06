# Comparing `tmp/molplotly-1.1.6.tar.gz` & `tmp/molplotly-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molplotly-1.1.6.tar", last modified: Tue Mar 14 21:08:35 2023, max compression
+gzip compressed data, was "molplotly-1.1.7.tar", last modified: Sun Mar 19 18:39:43 2023, max compression
```

## Comparing `molplotly-1.1.6.tar` & `molplotly-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 williammccorkindale   (501) staff       (20)        0 2023-03-14 21:08:35.889642 molplotly-1.1.6/
--rw-r--r--   0 williammccorkindale   (501) staff       (20)    11350 2022-02-10 13:55:17.000000 molplotly-1.1.6/LICENSE
--rw-r--r--   0 williammccorkindale   (501) staff       (20)    10825 2023-03-14 21:08:35.889870 molplotly-1.1.6/PKG-INFO
--rw-r--r--   0 williammccorkindale   (501) staff       (20)    10005 2023-03-14 21:07:26.000000 molplotly-1.1.6/README.md
-drwxr-xr-x   0 williammccorkindale   (501) staff       (20)        0 2023-03-14 21:08:35.885620 molplotly-1.1.6/molplotly/
--rw-r--r--   0 williammccorkindale   (501) staff       (20)       19 2022-02-10 13:55:17.000000 molplotly-1.1.6/molplotly/__init__.py
--rw-r--r--   0 williammccorkindale   (501) staff       (20)    17384 2023-03-14 21:03:09.000000 molplotly-1.1.6/molplotly/main.py
-drwxr-xr-x   0 williammccorkindale   (501) staff       (20)        0 2023-03-14 21:08:35.887748 molplotly-1.1.6/molplotly.egg-info/
--rw-r--r--   0 williammccorkindale   (501) staff       (20)    10825 2023-03-14 21:08:35.000000 molplotly-1.1.6/molplotly.egg-info/PKG-INFO
--rw-r--r--   0 williammccorkindale   (501) staff       (20)      299 2023-03-14 21:08:35.000000 molplotly-1.1.6/molplotly.egg-info/SOURCES.txt
--rw-r--r--   0 williammccorkindale   (501) staff       (20)        1 2023-03-14 21:08:35.000000 molplotly-1.1.6/molplotly.egg-info/dependency_links.txt
--rw-r--r--   0 williammccorkindale   (501) staff       (20)      109 2023-03-14 21:08:35.000000 molplotly-1.1.6/molplotly.egg-info/requires.txt
--rw-r--r--   0 williammccorkindale   (501) staff       (20)       10 2023-03-14 21:08:35.000000 molplotly-1.1.6/molplotly.egg-info/top_level.txt
--rw-r--r--   0 williammccorkindale   (501) staff       (20)       79 2023-03-14 21:08:35.890503 molplotly-1.1.6/setup.cfg
--rw-r--r--   0 williammccorkindale   (501) staff       (20)     1062 2023-03-14 21:03:09.000000 molplotly-1.1.6/setup.py
--rw-r--r--   0 williammccorkindale   (501) staff       (20)     1380 2023-03-14 21:03:09.000000 molplotly-1.1.6/setup_pip.py
-drwxr-xr-x   0 williammccorkindale   (501) staff       (20)        0 2023-03-14 21:08:35.888920 molplotly-1.1.6/tests/
--rw-r--r--   0 williammccorkindale   (501) staff       (20)       63 2022-11-24 14:52:29.000000 molplotly-1.1.6/tests/__init__.py
--rw-r--r--   0 williammccorkindale   (501) staff       (20)      925 2022-06-01 13:28:15.000000 molplotly-1.1.6/tests/test_add_molecules.py
+drwxr-xr-x   0 williammccorkindale   (501) staff       (20)        0 2023-03-19 18:39:43.454836 molplotly-1.1.7/
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)    11350 2022-02-10 13:55:17.000000 molplotly-1.1.7/LICENSE
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)    10822 2023-03-19 18:39:43.455023 molplotly-1.1.7/PKG-INFO
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)    10002 2023-03-19 18:37:00.000000 molplotly-1.1.7/README.md
+drwxr-xr-x   0 williammccorkindale   (501) staff       (20)        0 2023-03-19 18:39:43.447569 molplotly-1.1.7/molplotly/
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)       19 2022-02-10 13:55:17.000000 molplotly-1.1.7/molplotly/__init__.py
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)    18855 2023-03-19 18:37:45.000000 molplotly-1.1.7/molplotly/main.py
+drwxr-xr-x   0 williammccorkindale   (501) staff       (20)        0 2023-03-19 18:39:43.453001 molplotly-1.1.7/molplotly.egg-info/
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)    10822 2023-03-19 18:39:42.000000 molplotly-1.1.7/molplotly.egg-info/PKG-INFO
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)      299 2023-03-19 18:39:43.000000 molplotly-1.1.7/molplotly.egg-info/SOURCES.txt
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)        1 2023-03-19 18:39:42.000000 molplotly-1.1.7/molplotly.egg-info/dependency_links.txt
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)      109 2023-03-19 18:39:43.000000 molplotly-1.1.7/molplotly.egg-info/requires.txt
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)       10 2023-03-19 18:39:43.000000 molplotly-1.1.7/molplotly.egg-info/top_level.txt
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)       79 2023-03-19 18:39:43.455762 molplotly-1.1.7/setup.cfg
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)     1032 2023-03-19 18:39:05.000000 molplotly-1.1.7/setup.py
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)     1380 2023-03-19 18:39:11.000000 molplotly-1.1.7/setup_pip.py
+drwxr-xr-x   0 williammccorkindale   (501) staff       (20)        0 2023-03-19 18:39:43.454150 molplotly-1.1.7/tests/
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)       63 2022-11-24 14:52:29.000000 molplotly-1.1.7/tests/__init__.py
+-rw-r--r--   0 williammccorkindale   (501) staff       (20)      925 2022-06-01 13:28:15.000000 molplotly-1.1.7/tests/test_add_molecules.py
```

### Comparing `molplotly-1.1.6/LICENSE` & `molplotly-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `molplotly-1.1.6/PKG-INFO` & `molplotly-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: molplotly
-Version: 1.1.6
+Version: 1.1.7
 Summary: molplotly is an add-on to plotly built on RDKit which allows 2D images of molecules to be shown in scatterplots when hovering over the datapoints.
 Home-page: https://github.com/wjm41/molplotly
-Download-URL: https://github.com/wjm41/molplotly/archive/refs/tags/v1.1.6.tar.gz
+Download-URL: https://github.com/wjm41/molplotly/archive/refs/tags/v1.1.7.tar.gz
 Author: William McCorkindale
 Author-email: wjm41@cam.ac.uk
 License: Apache License, Version 2.0
 Keywords: science,chemistry,cheminformatics
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -78,26 +78,26 @@
 | `alpha`             | `float`     | `0.7`      | the transparency of the hoverbox, 0 for full transparency 1 for full opaqueness                                                                                       |
 | `mol_alpha`         | `float`     | `0.7`      | the transparency of the SVG molecule image, 0 for full transparency 1 for full opaqueness                                                                             |
 | `title_col`         | `str`       | `None`     | name of the column in df to be used as the title entry in the hover box                                                                                               |
 | `show_coords`       | `bool`      | `True`     | whether or not to show the coordinates of the data point in the hover box                                                                                             |
 | `caption_cols`      | `list`      | `None`     | list of column names in df to be included in the hover box                                                                                                            |
 | `caption_transform` | `dict`      | `{}`       | Functions applied to captions for formatting. The dict must follow a key: function structure where the key must correspond to one of the columns in subset or tooltip |
 | `color_col`         | `str`       | `None`     | name of the column in df that is used to color the datapoints in `df` - necessary when there is discrete conditional coloring                                         |
-| `marker_col`        | `str`       | `None`     | name of the column in df that is used to determine the marker shape of the datapoints in `df`                                                                         |
+| `symbol_col`        | `str`       | `None`     | name of the column in df that is used to determine the marker shape of the datapoints in `df`                                                                         |
 | `wrap`              | `bool`      | `True`     | whether or not to wrap the title text to multiple lines if the length of the text is too long                                                                         |
 | `wraplen`           | `int`       | `20`       | the threshold length of the title text before wrapping begins - adjust when changing the width of the hover box                                                       |
 | `width`             | `int`       | `150`      | the width in pixels of the hover box                                                                                                                                  |
 | `fontfamily`        | `str`       | `'Arial'`  | the font family used in the hover box                                                                                                                                 |
 | `fontsize`          | `int`       | `12`       | the font size used in the hover box - the font of the title line is `fontsize`+2                                                                                      |
 
 #### Output parameters
 
 by default a JupyterDash `app` is returned which can be run inline in a jupyter notebook or deployed on a server via `app.run_server()`
 
-- The recommended `height` of the app is `50+(height of t   he plotly figure)`.
+- The recommended `height` of the app is `50+(height of the plotly figure)`.
 - For the `port` of the app, make sure you don't pick the same `port` as another `molplotly` plot otherwise the tooltips will clash with each other. Also, apparently on windows port numbers below `8700` are used by other processes so for safety processes keep to numbers above that.
 
 ## Can I run this in colab?
 
 JupyterDash is supposed to have support for Google Colab but at some point that seems to have broken.. Keep an eye on the raised issue [here](https://github.com/plotly/jupyter-dash/issues/10)!
 Update (1st March 2022): The plots seem to be running again but the hoverboxes are not showing so I don't think it has been fully fixed - I will keep an eye on it in the meantime.
```

### Comparing `molplotly-1.1.6/README.md` & `molplotly-1.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,26 +59,26 @@
 | `alpha`             | `float`     | `0.7`      | the transparency of the hoverbox, 0 for full transparency 1 for full opaqueness                                                                                       |
 | `mol_alpha`         | `float`     | `0.7`      | the transparency of the SVG molecule image, 0 for full transparency 1 for full opaqueness                                                                             |
 | `title_col`         | `str`       | `None`     | name of the column in df to be used as the title entry in the hover box                                                                                               |
 | `show_coords`       | `bool`      | `True`     | whether or not to show the coordinates of the data point in the hover box                                                                                             |
 | `caption_cols`      | `list`      | `None`     | list of column names in df to be included in the hover box                                                                                                            |
 | `caption_transform` | `dict`      | `{}`       | Functions applied to captions for formatting. The dict must follow a key: function structure where the key must correspond to one of the columns in subset or tooltip |
 | `color_col`         | `str`       | `None`     | name of the column in df that is used to color the datapoints in `df` - necessary when there is discrete conditional coloring                                         |
-| `marker_col`        | `str`       | `None`     | name of the column in df that is used to determine the marker shape of the datapoints in `df`                                                                         |
+| `symbol_col`        | `str`       | `None`     | name of the column in df that is used to determine the marker shape of the datapoints in `df`                                                                         |
 | `wrap`              | `bool`      | `True`     | whether or not to wrap the title text to multiple lines if the length of the text is too long                                                                         |
 | `wraplen`           | `int`       | `20`       | the threshold length of the title text before wrapping begins - adjust when changing the width of the hover box                                                       |
 | `width`             | `int`       | `150`      | the width in pixels of the hover box                                                                                                                                  |
 | `fontfamily`        | `str`       | `'Arial'`  | the font family used in the hover box                                                                                                                                 |
 | `fontsize`          | `int`       | `12`       | the font size used in the hover box - the font of the title line is `fontsize`+2                                                                                      |
 
 #### Output parameters
 
 by default a JupyterDash `app` is returned which can be run inline in a jupyter notebook or deployed on a server via `app.run_server()`
 
-- The recommended `height` of the app is `50+(height of t   he plotly figure)`.
+- The recommended `height` of the app is `50+(height of the plotly figure)`.
 - For the `port` of the app, make sure you don't pick the same `port` as another `molplotly` plot otherwise the tooltips will clash with each other. Also, apparently on windows port numbers below `8700` are used by other processes so for safety processes keep to numbers above that.
 
 ## Can I run this in colab?
 
 JupyterDash is supposed to have support for Google Colab but at some point that seems to have broken.. Keep an eye on the raised issue [here](https://github.com/plotly/jupyter-dash/issues/10)!
 Update (1st March 2022): The plots seem to be running again but the hoverboxes are not showing so I don't think it has been fully fixed - I will keep an eye on it in the meantime.
```

### Comparing `molplotly-1.1.6/molplotly/main.py` & `molplotly-1.1.7/molplotly/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,26 +46,36 @@
             if len(data.y) == len(str_groups[data.name]):
                 continue
         else:
             return False
     return True
 
 
+def find_correct_column_order(cols, col_names):
+
+    correctly_ordered_cols = []
+    for col in col_names:
+        if col in cols:
+            correctly_ordered_cols.append(col)
+    return correctly_ordered_cols
+
+
 def find_grouping(
     fig: Figure, df_data: pd.DataFrame, cols: list[str]
 ) -> tuple[DataFrameGroupBy, dict]:
 
     if fig.data[0].hovertemplate is not None:
         col_names = re.findall(r"(.*?)=.*?<.*?>", fig.data[0].hovertemplate)
         col_names = [re.sub(r"(.*)>", "", col_name) for col_name in col_names]
         if set(cols).issubset(set(col_names)) is False:
             raise ValueError(
-                f"marker_col/color_col/facet_col is misspecified because the specified dataframe grouping names {cols} don't match the names in the plotly figure {col_names}.",
+                f"symbol_col/color_col/facet_col is misspecified because the specified dataframe grouping names {cols} don't match the names in the plotly figure {col_names}.",
             )
 
+        cols = find_correct_column_order(cols, col_names)
         df_grouped = df_data.groupby(cols)
 
         str_groups = {}
         for name, group in df_grouped:
             if isinstance(name, tuple):
                 str_groups[", ".join(str(x) for x in name)] = group
             else:
@@ -73,24 +83,32 @@
 
         curve_dict = {}
         for index, data in enumerate(fig.data):
             curve_name = re.findall(r".*?=(.*?)<.*?>", data.hovertemplate)
             curve_name = ", ".join(str(x) for x in curve_name)
             if "%{x}" in curve_name:
                 unique_x_values = np.unique(data.x)
-                if len(unique_x_values) == 1:
+                if len(unique_x_values) == 1 and len(data.x) != 1:
                     curve_name = curve_name.replace("%{x}", str(unique_x_values[0]))
                 else:
                     curve_name = curve_name.replace(", %{x}", "")
             if "%{y}" in curve_name:
                 unique_y_values = np.unique(data.y)
-                if len(unique_y_values) == 1:
+                if len(unique_y_values) == 1 and len(data.y) != 1:
                     curve_name = curve_name.replace("%{y}", str(unique_y_values[0]))
                 else:
                     curve_name = curve_name.replace(", %{y}", "")
+            if "%{marker.size}" in curve_name:
+                unique_size_values = np.unique(data.marker.size)
+                if len(unique_size_values) == 1 and len(data.marker.size) != 1:
+                    curve_name = curve_name.replace(
+                        "%{marker.size}", str(unique_size_values[0])
+                    )
+                else:
+                    curve_name = curve_name.replace(", %{marker.size}", "")
             curve_dict[index] = str_groups[curve_name]
 
         return df_grouped, curve_dict
 
     else:
         grouping_found = False
         for combo in itertools.permutations(cols):
@@ -111,15 +129,15 @@
                 return df_grouped, curve_dict
 
             else:
                 continue
 
         if not grouping_found:
             raise ValueError(
-                "marker_col/color_col/facet_cik is misspecified because the dataframe grouping names don't match the names in the plotly figure."
+                "symbol_col/color_col/facet_col is misspecified because the dataframe grouping names don't match the names in the plotly figure."
             )
 
 
 def add_molecules(
     fig: Figure,
     df: pd.DataFrame,
     smiles_col: str | list[str] = "SMILES",
@@ -129,15 +147,15 @@
     alpha: float = 0.75,
     mol_alpha: float = 0.7,
     title_col: str = None,
     show_coords: bool = True,
     caption_cols: list[str] = None,
     caption_transform: dict[str, Callable] = {},
     color_col: str = None,
-    marker_col: str = None,
+    symbol_col: str = None,
     facet_col: str = None,
     wrap: bool = True,
     wraplen: int = 20,
     width: int = 150,
     fontfamily: str = "Arial",
     fontsize: int = 12,
 ) -> JupyterDash:
@@ -175,16 +193,16 @@
     caption_cols : list[str], optional
         list of column names in df to be included in the hover box (default None).
     caption_transform : dict[str, callable], optional
         Functions applied to specific items in all cells. The dict must follow a key: function structure where
         the key must correspond to one of the columns in subset or tooltip (default {}).
     color_col : str, optional
         name of the column in df that is used to color the datapoints in df - necessary when there is discrete conditional coloring (default None).
-    marker_col : str, optional
-        name of the column in df that is used to determine the marker shape of the datapoints in df (default None).
+    symbol_col : str, optional
+        name of the column in df that is used to determine the symbols of the datapoints in df (default None).
     facet_col : str, optional
         name of the column in df that is used to facet the data to multiple plots (default None).
     wrap : bool, optional
         whether or not to wrap the title text to multiple lines if the length of the text is too long (default True).
     wraplen : int, optional
         the threshold length of the title text before wrapping begins - adjust when changing the width of the hover box (default 20).
     width : int, optional
@@ -193,61 +211,87 @@
         the font family used in the hover box (default 'Arial').
     fontsize : int, optional
         the font size used in the hover box - the font of the title line is fontsize+2 (default 12).
     """
     df_data = df.copy()
     if color_col is not None:
         df_data[color_col] = df_data[color_col].astype(str)
-    if marker_col is not None:
-        df_data[marker_col] = df_data[marker_col].astype(str)
+    if symbol_col is not None:
+        df_data[symbol_col] = df_data[symbol_col].astype(str)
     if facet_col is not None:
         df_data[facet_col] = df_data[facet_col].astype(str)
 
     if len(fig.data) != 1:
         colors = {index: x.marker["color"] for index, x in enumerate(fig.data)}
 
         cols = []
 
         if color_col is not None:
             cols.append(color_col)
-        if marker_col is not None:
-            cols.append(marker_col)
+        if symbol_col is not None:
+            cols.append(symbol_col)
         if facet_col is not None:
             cols.append(facet_col)
+        cols = list(set(cols))
         _, curve_dict = find_grouping(fig, df_data, cols)
     else:
         colors = {0: "black"}
 
     app = JupyterDash(__name__)
     if smiles_col is None and mol_col is None:
         raise ValueError("Either smiles_col or mol_col has to be specified!")
 
     if isinstance(smiles_col, str):
         smiles_col = [smiles_col]
     if isinstance(mol_col, str):
         mol_col = [mol_col]
 
-    if mol_col is not None and len(mol_col) > 1:
+    if mol_col is not None:
+        if len(mol_col) > 1:
+            menu = dcc.Dropdown(
+                options=[{"label": x, "value": x} for x in mol_col],
+                value=mol_col[0],
+                multi=True,
+                id="smiles-menu",
+                placeholder="Select a mol column to display",
+            )
+        else:
+            menu = dcc.Dropdown(
+                options=[{"label": mol_col, "value": mol_col}],
+                value=mol_col,
+                multi=False,
+                id="smiles-menu",
+                disabled=True,
+            )
+    elif smiles_col is not None:
+        if len(smiles_col) > 1:
+            menu = dcc.Dropdown(
+                options=[{"label": x, "value": x} for x in smiles_col],
+                value=smiles_col[0],
+                multi=True,
+                id="smiles-menu",
+                placeholder="Select a SMILES column to display",
+                searchable=True,
+            )
+        else:
+            menu = dcc.Dropdown(
+                options=[{"label": smiles_col, "value": smiles_col}],
+                value=smiles_col,
+                multi=False,
+                id="smiles-menu",
+                disabled=True,
+            )
+    else:
         menu = dcc.Dropdown(
-            options=[{"label": x, "smiles_value": x} for x in mol_col],
-            value=mol_col[0],
-            multi=True,
+            options=None,
+            value=None,
             id="smiles-menu",
             placeholder="Select a mol column to display",
+            disabled=True,
         )
-    elif smiles_col is not None and len(smiles_col) > 1:
-        menu = dcc.Dropdown(
-            options=[{"label": x, "smiles_value": x} for x in smiles_col],
-            value=smiles_col[0],
-            multi=True,
-            id="smiles-menu",
-            placeholder="Select a SMILES column to display",
-        )
-    else:
-        menu = dcc.Store(id="smiles-menu", data=0)
 
     fig_copy = go.Figure(fig)
     fig_copy.update_traces(hoverinfo="none", hovertemplate=None)
 
     app.layout = html.Div(
         [
             menu,
@@ -262,30 +306,30 @@
         output=[
             Output("graph-tooltip", "show"),
             Output("graph-tooltip", "bbox"),
             Output("graph-tooltip", "children"),
         ],
         inputs=[
             Input("graph-basic-2", "hoverData"),
-            Input("smiles-menu", "smiles_value"),
+            Input("smiles-menu", "value"),
         ],
     )
-    def display_hover(hoverData, smiles_value):
+    def display_hover(hoverData, value):
         if hoverData is None:
             return False, no_update, no_update
 
-        if smiles_value is None:
+        if value is None:
             if mol_col is not None:
-                smiles_value = mol_col
+                value = mol_col
             elif smiles_col is not None:
-                smiles_value = smiles_col
-        if isinstance(smiles_value, str):
-            chosen_smiles = [smiles_value]
+                value = smiles_col
+        if isinstance(value, str):
+            chosen_smiles = [value]
         else:
-            chosen_smiles = smiles_value
+            chosen_smiles = value
 
         pt = hoverData["points"][0]
         bbox = pt["bbox"]
         num = pt["pointNumber"]
         curve_num = pt["curveNumber"]
 
         if len(fig.data) != 1:
```

### Comparing `molplotly-1.1.6/molplotly.egg-info/PKG-INFO` & `molplotly-1.1.7/molplotly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: molplotly
-Version: 1.1.6
+Version: 1.1.7
 Summary: molplotly is an add-on to plotly built on RDKit which allows 2D images of molecules to be shown in scatterplots when hovering over the datapoints.
 Home-page: https://github.com/wjm41/molplotly
-Download-URL: https://github.com/wjm41/molplotly/archive/refs/tags/v1.1.6.tar.gz
+Download-URL: https://github.com/wjm41/molplotly/archive/refs/tags/v1.1.7.tar.gz
 Author: William McCorkindale
 Author-email: wjm41@cam.ac.uk
 License: Apache License, Version 2.0
 Keywords: science,chemistry,cheminformatics
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -78,26 +78,26 @@
 | `alpha`             | `float`     | `0.7`      | the transparency of the hoverbox, 0 for full transparency 1 for full opaqueness                                                                                       |
 | `mol_alpha`         | `float`     | `0.7`      | the transparency of the SVG molecule image, 0 for full transparency 1 for full opaqueness                                                                             |
 | `title_col`         | `str`       | `None`     | name of the column in df to be used as the title entry in the hover box                                                                                               |
 | `show_coords`       | `bool`      | `True`     | whether or not to show the coordinates of the data point in the hover box                                                                                             |
 | `caption_cols`      | `list`      | `None`     | list of column names in df to be included in the hover box                                                                                                            |
 | `caption_transform` | `dict`      | `{}`       | Functions applied to captions for formatting. The dict must follow a key: function structure where the key must correspond to one of the columns in subset or tooltip |
 | `color_col`         | `str`       | `None`     | name of the column in df that is used to color the datapoints in `df` - necessary when there is discrete conditional coloring                                         |
-| `marker_col`        | `str`       | `None`     | name of the column in df that is used to determine the marker shape of the datapoints in `df`                                                                         |
+| `symbol_col`        | `str`       | `None`     | name of the column in df that is used to determine the marker shape of the datapoints in `df`                                                                         |
 | `wrap`              | `bool`      | `True`     | whether or not to wrap the title text to multiple lines if the length of the text is too long                                                                         |
 | `wraplen`           | `int`       | `20`       | the threshold length of the title text before wrapping begins - adjust when changing the width of the hover box                                                       |
 | `width`             | `int`       | `150`      | the width in pixels of the hover box                                                                                                                                  |
 | `fontfamily`        | `str`       | `'Arial'`  | the font family used in the hover box                                                                                                                                 |
 | `fontsize`          | `int`       | `12`       | the font size used in the hover box - the font of the title line is `fontsize`+2                                                                                      |
 
 #### Output parameters
 
 by default a JupyterDash `app` is returned which can be run inline in a jupyter notebook or deployed on a server via `app.run_server()`
 
-- The recommended `height` of the app is `50+(height of t   he plotly figure)`.
+- The recommended `height` of the app is `50+(height of the plotly figure)`.
 - For the `port` of the app, make sure you don't pick the same `port` as another `molplotly` plot otherwise the tooltips will clash with each other. Also, apparently on windows port numbers below `8700` are used by other processes so for safety processes keep to numbers above that.
 
 ## Can I run this in colab?
 
 JupyterDash is supposed to have support for Google Colab but at some point that seems to have broken.. Keep an eye on the raised issue [here](https://github.com/plotly/jupyter-dash/issues/10)!
 Update (1st March 2022): The plots seem to be running again but the hoverboxes are not showing so I don't think it has been fully fixed - I will keep an eye on it in the meantime.
```

### Comparing `molplotly-1.1.6/setup.py` & `molplotly-1.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="molplotly",
-    version="1.1.6",
+    version="1.1.7",
     description="plotly add-on to render molecule images on mouseover",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/wjm41/molplotly",
     author="William McCorkindale",
     license="Apache License 2.0",
     packages=find_packages(),
@@ -25,10 +25,8 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Chemistry",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
     ],
-)
-
-# TODO - change link in blog
+)
```

### Comparing `molplotly-1.1.6/setup_pip.py` & `molplotly-1.1.7/setup_pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="molplotly",
     packages=["molplotly"],
-    version="1.1.6",
+    version="1.1.7",
     license="Apache License, Version 2.0",
     description="molplotly is an add-on to plotly built on RDKit which allows 2D images of molecules to be shown in scatterplots when hovering over the datapoints.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="William McCorkindale",
     author_email="wjm41@cam.ac.uk",
     url="https://github.com/wjm41/molplotly",
-    download_url="https://github.com/wjm41/molplotly/archive/refs/tags/v1.1.6.tar.gz",
+    download_url="https://github.com/wjm41/molplotly/archive/refs/tags/v1.1.7.tar.gz",
     install_requires=[
         "dash>=2.0.0",
         "werkzeug>=2.0.0",
         "jupyter-dash>=0.4.2",
         "plotly>=5.0.0",
         "rdkit-pypi>=2021.9.4",
         "pandas",
```

### Comparing `molplotly-1.1.6/tests/test_add_molecules.py` & `molplotly-1.1.7/tests/test_add_molecules.py`

 * *Files identical despite different names*

