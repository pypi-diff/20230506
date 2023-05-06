# Comparing `tmp/sviewgui-1.0.1.tar.gz` & `tmp/sviewgui-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sviewgui-1.0.1.tar", last modified: Fri Jun 10 14:37:47 2022, max compression
+gzip compressed data, was "sviewgui-1.1.2.tar", last modified: Sat May  6 06:03:13 2023, max compression
```

## Comparing `sviewgui-1.0.1.tar` & `sviewgui-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fukudasoujirou   (501) staff       (20)        0 2022-06-10 14:37:47.000000 sviewgui-1.0.1/
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)       52 2020-04-16 05:40:37.000000 sviewgui-1.0.1/MANIFEST.in
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)     2036 2022-06-10 14:37:47.000000 sviewgui-1.0.1/PKG-INFO
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)     1281 2022-05-21 23:59:56.000000 sviewgui-1.0.1/README.md
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)       38 2022-06-10 14:37:47.000000 sviewgui-1.0.1/setup.cfg
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)     1728 2022-06-10 14:37:41.000000 sviewgui-1.0.1/setup.py
-drwxr-xr-x   0 fukudasoujirou   (501) staff       (20)        0 2022-06-10 14:37:47.000000 sviewgui-1.0.1/sviewgui/
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)        1 2020-04-16 05:40:37.000000 sviewgui-1.0.1/sviewgui/__init__.py
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)    20670 2022-05-21 23:38:34.000000 sviewgui-1.0.1/sviewgui/sgui.py
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)    79074 2022-06-10 14:27:10.000000 sviewgui-1.0.1/sviewgui/sview.py
-drwxr-xr-x   0 fukudasoujirou   (501) staff       (20)        0 2022-06-10 14:37:47.000000 sviewgui-1.0.1/sviewgui.egg-info/
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)     2036 2022-06-10 14:37:46.000000 sviewgui-1.0.1/sviewgui.egg-info/PKG-INFO
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)      280 2022-06-10 14:37:47.000000 sviewgui-1.0.1/sviewgui.egg-info/SOURCES.txt
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)        1 2022-06-10 14:37:46.000000 sviewgui-1.0.1/sviewgui.egg-info/dependency_links.txt
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)      110 2022-06-10 14:37:46.000000 sviewgui-1.0.1/sviewgui.egg-info/entry_points.txt
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)      133 2022-06-10 14:37:46.000000 sviewgui-1.0.1/sviewgui.egg-info/requires.txt
--rw-r--r--   0 fukudasoujirou   (501) staff       (20)        9 2022-06-10 14:37:46.000000 sviewgui-1.0.1/sviewgui.egg-info/top_level.txt
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-05-06 06:03:13.350096 sviewgui-1.1.2/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       52 2023-05-05 11:34:25.000000 sviewgui-1.1.2/MANIFEST.in
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     2404 2023-05-06 06:03:13.350096 sviewgui-1.1.2/PKG-INFO
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1849 2023-05-06 06:00:12.000000 sviewgui-1.1.2/README.md
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)       38 2023-05-06 06:03:13.350096 sviewgui-1.1.2/setup.cfg
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     1748 2023-05-06 06:02:06.000000 sviewgui-1.1.2/setup.py
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-05-06 06:03:13.346096 sviewgui-1.1.2/sviewgui/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)        1 2023-05-05 11:34:25.000000 sviewgui-1.1.2/sviewgui/__init__.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    20675 2023-05-06 06:00:12.000000 sviewgui-1.1.2/sviewgui/sgui.py
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)    79086 2023-05-06 06:00:12.000000 sviewgui-1.1.2/sviewgui/sview.py
+drwxrwxr-x   0 sojiro    (1000) sojiro    (1000)        0 2023-05-06 06:03:13.350096 sviewgui-1.1.2/sviewgui.egg-info/
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)     2404 2023-05-06 06:03:13.000000 sviewgui-1.1.2/sviewgui.egg-info/PKG-INFO
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      280 2023-05-06 06:03:13.000000 sviewgui-1.1.2/sviewgui.egg-info/SOURCES.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)        1 2023-05-06 06:03:13.000000 sviewgui-1.1.2/sviewgui.egg-info/dependency_links.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      110 2023-05-06 06:03:13.000000 sviewgui-1.1.2/sviewgui.egg-info/entry_points.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)      133 2023-05-06 06:03:13.000000 sviewgui-1.1.2/sviewgui.egg-info/requires.txt
+-rw-rw-r--   0 sojiro    (1000) sojiro    (1000)        9 2023-05-06 06:03:13.000000 sviewgui-1.1.2/sviewgui.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sviewgui-1.0.1/PKG-INFO` & `sviewgui-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,74 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sviewgui
-Version: 1.0.1
+Version: 1.1.2
 Summary: Package Dependency: Validates package requirements
 Home-page: https://github.com/SojiroFukuda/sview-gui
 Author: SojiroFukuda
 Author-email: S.Fukuda-2018@hull.ac.uk
 Maintainer: SojiroFukuda
 Maintainer-email: S.Fukuda-2018@hull.ac.uk
 License: SojiroFukuda
-Description: # sview-gui
-        
-        PyQt5 GUI for data visualisation based on matplotlib and seaborn.
-        Have you ever felt that you are wasting a lot of time writing the code for a simple figure?
-        If so, this GUI will help you out to save your time. You can plot and save your figure by just pushing a couple of buttons on Sviewgui. Not only that, you can also get the source code of your plot so that you can copy and paste it to your environment to adjust minor settings.
-        Main features are
-        + Scatter, line, kdeplot, histgram, and box plot
-        + Detail setting for the style of plot, marker size, line width, number of bins of histgram, colormap, colorbar, etc.
-        + Subdevide your data based on the columns of DataFrame and use different colors for each subset in your plot.
-        + Save figure as editable PDF
-        + Source code of the graph you plotted are recorded in the log window
-        
-        # Usage
-        
-        This package has only one method: buildGUI(). 
-        You can use the file path of your csv file as an argument.
-        Also, you can use pandas' DataFrame object for the argument.
-        
-        # Recent updata
-        
-        + Fixed minor bugs.
-        + log scale for negative columns, colorbar, histgram
-        + Adjustable style
-        + kdeplot with scatter plot.
-        
-        # About license
-        © 2019 Sojiro Fukuda All Rightss Reserved.
-        Free to modify and redistribute by your own responsibility.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Framework :: Matplotlib
+Description-Content-Type: markdown
+
+# sview-gui
+
+PyQt5 GUI for data visualisation based on matplotlib and seaborn.
+Have you ever felt that you are wasting a lot of time writing the code for a simple figure?
+If so, this GUI will help you out to save your time. 
+You can plot and save your figure by just pushing a couple of buttons on Sviewgui.
+All figures you made are recorded in the log window as their source code. 
+You can reproduce and further modify your figures, copying and pasting the code from the log into your own editor.
+
+Main features are
++ Scatter, line, kdeplot, histgram, and box plot
++ Detail setting for the style of plot, marker size, line width, number of bins of histgram, colormap, colorbar, etc.
++ Subdevide your data based on the columns of DataFrame and use different colours for each subset in your plot.
++ Save figure as editable PDF
++ Source code of the graph you plotted are recorded in the log window
+
+# Usage
+
+This package has only one method: buildGUI(). 
+```python
+import sviewgui.sview as sv
+
+sv.buildGUI()
+```
+Then, GUI window will pop up, then you can choose your csv file via GUI.
+Alternatively, you can also pass the path of your csv file,
+```python
+import sviewgui.sview as sv
+
+csvpath = 'usr/mydata.csv'
+sv.buildGUI(csvpath)
+```
+or pandas DataFrame object
+```python
+import sviewgui.sview as sv
+from sklearn.datasets import load_iris
+import pandas as pd
+
+data = load_iris() # load iris data 
+df = pd.DataFrame(data=data.data, columns=data.feature_names) # convert sklearn data into DataFrame object
+sv.buildGUI(df)
+```
+Now, you are good to go. Have fun with Sview.
+
+
+# Recent update
+
++ Fixed minor bugs.
++ log scale for negative columns, colorbar, histgram
++ Adjustable style (seaborn, ggplot, etc.)
++ kdeplot with scatter plot.
+
+# About licence
+© 2019 Sojiro Fukuda All Rights Reserved.
+Free to modify and redistribute by your responsibility.
+
+
```

### Comparing `sviewgui-1.0.1/setup.py` & `sviewgui-1.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 
 # version
 here = os.path.dirname(os.path.abspath(__file__))
 version = next((line.split('=')[1].strip().replace("'", '')
                 for line in open(os.path.join(here,
                                               'sviewgui',
                                               '__init__.py'))
-                if line.startswith('__version__ = ')),'1.0.1')
+                if line.startswith('__version__ = ')),'1.1.2')
 
 setup(
     name="sviewgui",
     version=version,
     url='https://github.com/SojiroFukuda/sview-gui',
     author='SojiroFukuda',
     author_email='S.Fukuda-2018@hull.ac.uk',
     maintainer='SojiroFukuda',
     maintainer_email='S.Fukuda-2018@hull.ac.uk',
     description='Package Dependency: Validates package requirements',
     long_description=readme,
+    long_description_content_type='markdown',
     packages=find_packages(),
     install_requires=[
-#         "sys >= 3.7.3",
         "PyQt5 >= 5.7.0",
         "numpy >= 1.16.0",
         "pandas >= 0.24.0",
         "matplotlib >= 3.0.0",
         "Pathlib2 >= 2.3.0",
         "scipy >= 1.2.0",
         "cmocean >= 2.0",
```

### Comparing `sviewgui-1.0.1/sviewgui/sgui.py` & `sviewgui-1.1.2/sviewgui/sgui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file 'SView.ui'
+# Form implementation generated from reading ui file 'sgui.ui'
 #
-# Created by: PyQt5 UI code generator 5.15.6
+# Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
@@ -17,19 +17,19 @@
         MainWindow.resize(946, 806)
         self.centralwidget = QtWidgets.QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.gridLayout_2 = QtWidgets.QGridLayout(self.centralwidget)
         self.gridLayout_2.setObjectName("gridLayout_2")
         self.scrollArea = QtWidgets.QScrollArea(self.centralwidget)
         self.scrollArea.setMinimumSize(QtCore.QSize(240, 0))
-        self.scrollArea.setMaximumSize(QtCore.QSize(300, 16777215))
+        self.scrollArea.setMaximumSize(QtCore.QSize(350, 16777215))
         self.scrollArea.setWidgetResizable(True)
         self.scrollArea.setObjectName("scrollArea")
         self.scrollAreaWidgetContents = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 302, 735))
+        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 331, 845))
         self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
         self.gridLayout_5 = QtWidgets.QGridLayout(self.scrollAreaWidgetContents)
         self.gridLayout_5.setObjectName("gridLayout_5")
         self.frame_graph = QtWidgets.QFrame(self.scrollAreaWidgetContents)
         self.frame_graph.setEnabled(False)
         self.frame_graph.setFrameShape(QtWidgets.QFrame.StyledPanel)
         self.frame_graph.setFrameShadow(QtWidgets.QFrame.Raised)
@@ -257,37 +257,37 @@
         self.tn_graph.setObjectName("tn_graph")
         self.gridLayout_11 = QtWidgets.QGridLayout(self.tn_graph)
         self.gridLayout_11.setObjectName("gridLayout_11")
         self.canvas = QtWidgets.QScrollArea(self.tn_graph)
         self.canvas.setWidgetResizable(True)
         self.canvas.setObjectName("canvas")
         self.scrollAreaWidgetContents_3 = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents_3.setGeometry(QtCore.QRect(0, 0, 558, 680))
+        self.scrollAreaWidgetContents_3.setGeometry(QtCore.QRect(0, 0, 98, 28))
         self.scrollAreaWidgetContents_3.setObjectName("scrollAreaWidgetContents_3")
         self.canvas.setWidget(self.scrollAreaWidgetContents_3)
         self.gridLayout_11.addWidget(self.canvas, 0, 0, 1, 1)
         self.tab_pca.addTab(self.tn_graph, "")
         self.gridLayout_2.addWidget(self.tab_pca, 0, 1, 1, 1)
         MainWindow.setCentralWidget(self.centralwidget)
         self.menubar = QtWidgets.QMenuBar(MainWindow)
-        self.menubar.setGeometry(QtCore.QRect(0, 0, 946, 24))
+        self.menubar.setGeometry(QtCore.QRect(0, 0, 946, 27))
         self.menubar.setObjectName("menubar")
         self.menuMenu = QtWidgets.QMenu(self.menubar)
         self.menuMenu.setObjectName("menuMenu")
         MainWindow.setMenuBar(self.menubar)
         self.statusbar = QtWidgets.QStatusBar(MainWindow)
         self.statusbar.setObjectName("statusbar")
         MainWindow.setStatusBar(self.statusbar)
         self.actionPreference = QtWidgets.QAction(MainWindow)
         self.actionPreference.setObjectName("actionPreference")
         self.menuMenu.addAction(self.actionPreference)
         self.menubar.addAction(self.menuMenu.menuAction())
 
         self.retranslateUi(MainWindow)
-        self.tab_pca.setCurrentIndex(2)
+        self.tab_pca.setCurrentIndex(0)
         self.button_csvPath.clicked.connect(MainWindow.readcsv) # type: ignore
         self.cmb_x.currentIndexChanged['int'].connect(MainWindow.setXaxis) # type: ignore
         self.cmb_y.currentIndexChanged['int'].connect(MainWindow.setYaxis) # type: ignore
         self.cmb_color.currentIndexChanged['int'].connect(MainWindow.setColor) # type: ignore
         self.cmb_sort.currentIndexChanged['int'].connect(MainWindow.setSort) # type: ignore
         self.cmb_subcolor.currentIndexChanged['int'].connect(MainWindow.setSubColor) # type: ignore
         self.cmb_subsort.currentIndexChanged['int'].connect(MainWindow.setSubSort) # type: ignore
@@ -339,13 +339,13 @@
         self.button_csvPath.setText(_translate("MainWindow", "Select"))
         self.label_16.setText(_translate("MainWindow", "Sorted Data"))
         self.label_15.setText(_translate("MainWindow", "Imput CSV"))
         self.tab_pca.setTabText(self.tab_pca.indexOf(self.tn_summary), _translate("MainWindow", "CSV"))
         self.logbox.setHtml(_translate("MainWindow", "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
 "<html><head><meta name=\"qrichtext\" content=\"1\" /><style type=\"text/css\">\n"
 "p, li { white-space: pre-wrap; }\n"
-"</style></head><body style=\" font-family:\'.AppleSystemUIFont\'; font-size:13pt; font-weight:400; font-style:normal;\">\n"
-"<p style=\"-qt-paragraph-type:empty; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px; font-family:\'.SF NS Text\';\"><br /></p></body></html>"))
+"</style></head><body style=\" font-family:\'Sans Serif\'; font-size:9pt; font-weight:400; font-style:normal;\">\n"
+"<p style=\"-qt-paragraph-type:empty; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px; font-family:\'.SF NS Text\'; font-size:13pt;\"><br /></p></body></html>"))
         self.tab_pca.setTabText(self.tab_pca.indexOf(self.tab_4), _translate("MainWindow", "Log"))
         self.tab_pca.setTabText(self.tab_pca.indexOf(self.tn_graph), _translate("MainWindow", "Graph"))
         self.menuMenu.setTitle(_translate("MainWindow", "Menu"))
-        self.actionPreference.setText(_translate("MainWindow", "Preference"))
+        self.actionPreference.setText(_translate("MainWindow", "Preference"))
```

### Comparing `sviewgui-1.0.1/sviewgui/sview.py` & `sviewgui-1.1.2/sviewgui/sview.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 matplotlib.use("Qt5Agg")
 import os
 import re
 import glob
 import numpy as np
 import pandas as pd
 import random
-from . import sgui as gui
-# import sgui as gui
+from . import sgui as gui # switch
+# import sgui as gui   # 
 import matplotlib.cm
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.figure import Figure
 from matplotlib.colors import LinearSegmentedColormap
 import matplotlib.colors as mcolors # default colour pallete 
 from matplotlib import style
 from matplotlib.font_manager import FontProperties
 
 from matplotlib.lines import Line2D # default markars 
 from pathlib import Path
-from PyQt5.Qt import PYQT_VERSION_STR
+# from PyQt5.Qt import PYQT_VERSION_STR
 from datetime import datetime
 
 import scipy.stats as st
 
 import cmocean
 import cmocean.cm
 import seaborn as sns
@@ -966,15 +966,15 @@
                 log_str +=   '    ' + 'c_index = i%len(colors)' + '\n'
                 log_str +=   '    ' + 'ax.plot( group["'+ str(x_var) +'"].replace([np.inf, -np.inf], np.nan), group["'+ str(y_var) +'"].replace([np.inf, -np.inf], np.nan), color = colors[c_index], alpha = '+str(keyDict['alpha'])+', linewidth = '+str(keyDict['msize'])+', label = value )' + '\n'
         return log_str
     
     
     
     def get_pallete(self):
-        return (plt.rcParams['axes.prop_cycle'].by_key()['color'], list(Line2D.filled_markers), list(matplotlib.cm.cmap_d.keys()) )
+        return (plt.rcParams['axes.prop_cycle'].by_key()['color'], list(Line2D.filled_markers), list(cmocean.cm.cmap_d.keys()) )
     
     
     
     
     def get_setting(self):
         # ( 
         #   name of selected cmap
@@ -1473,8 +1473,7 @@
     wmain = Csviwer()
     wmain.show()
     if type(data) == pd.core.frame.DataFrame:
         wmain.loadData(data)
     elif isinstance(data,str) and data != 'None':
         wmain.loadData(data)
     sys.exit(app.exec_())
-
```

### Comparing `sviewgui-1.0.1/sviewgui.egg-info/PKG-INFO` & `sviewgui-1.1.2/sviewgui.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,74 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sviewgui
-Version: 1.0.1
+Version: 1.1.2
 Summary: Package Dependency: Validates package requirements
 Home-page: https://github.com/SojiroFukuda/sview-gui
 Author: SojiroFukuda
 Author-email: S.Fukuda-2018@hull.ac.uk
 Maintainer: SojiroFukuda
 Maintainer-email: S.Fukuda-2018@hull.ac.uk
 License: SojiroFukuda
-Description: # sview-gui
-        
-        PyQt5 GUI for data visualisation based on matplotlib and seaborn.
-        Have you ever felt that you are wasting a lot of time writing the code for a simple figure?
-        If so, this GUI will help you out to save your time. You can plot and save your figure by just pushing a couple of buttons on Sviewgui. Not only that, you can also get the source code of your plot so that you can copy and paste it to your environment to adjust minor settings.
-        Main features are
-        + Scatter, line, kdeplot, histgram, and box plot
-        + Detail setting for the style of plot, marker size, line width, number of bins of histgram, colormap, colorbar, etc.
-        + Subdevide your data based on the columns of DataFrame and use different colors for each subset in your plot.
-        + Save figure as editable PDF
-        + Source code of the graph you plotted are recorded in the log window
-        
-        # Usage
-        
-        This package has only one method: buildGUI(). 
-        You can use the file path of your csv file as an argument.
-        Also, you can use pandas' DataFrame object for the argument.
-        
-        # Recent updata
-        
-        + Fixed minor bugs.
-        + log scale for negative columns, colorbar, histgram
-        + Adjustable style
-        + kdeplot with scatter plot.
-        
-        # About license
-        © 2019 Sojiro Fukuda All Rightss Reserved.
-        Free to modify and redistribute by your own responsibility.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Framework :: Matplotlib
+Description-Content-Type: markdown
+
+# sview-gui
+
+PyQt5 GUI for data visualisation based on matplotlib and seaborn.
+Have you ever felt that you are wasting a lot of time writing the code for a simple figure?
+If so, this GUI will help you out to save your time. 
+You can plot and save your figure by just pushing a couple of buttons on Sviewgui.
+All figures you made are recorded in the log window as their source code. 
+You can reproduce and further modify your figures, copying and pasting the code from the log into your own editor.
+
+Main features are
++ Scatter, line, kdeplot, histgram, and box plot
++ Detail setting for the style of plot, marker size, line width, number of bins of histgram, colormap, colorbar, etc.
++ Subdevide your data based on the columns of DataFrame and use different colours for each subset in your plot.
++ Save figure as editable PDF
++ Source code of the graph you plotted are recorded in the log window
+
+# Usage
+
+This package has only one method: buildGUI(). 
+```python
+import sviewgui.sview as sv
+
+sv.buildGUI()
+```
+Then, GUI window will pop up, then you can choose your csv file via GUI.
+Alternatively, you can also pass the path of your csv file,
+```python
+import sviewgui.sview as sv
+
+csvpath = 'usr/mydata.csv'
+sv.buildGUI(csvpath)
+```
+or pandas DataFrame object
+```python
+import sviewgui.sview as sv
+from sklearn.datasets import load_iris
+import pandas as pd
+
+data = load_iris() # load iris data 
+df = pd.DataFrame(data=data.data, columns=data.feature_names) # convert sklearn data into DataFrame object
+sv.buildGUI(df)
+```
+Now, you are good to go. Have fun with Sview.
+
+
+# Recent update
+
++ Fixed minor bugs.
++ log scale for negative columns, colorbar, histgram
++ Adjustable style (seaborn, ggplot, etc.)
++ kdeplot with scatter plot.
+
+# About licence
+© 2019 Sojiro Fukuda All Rights Reserved.
+Free to modify and redistribute by your responsibility.
+
+
```

