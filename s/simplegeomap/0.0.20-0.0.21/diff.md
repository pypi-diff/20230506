# Comparing `tmp/simplegeomap-0.0.20.tar.gz` & `tmp/simplegeomap-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplegeomap-0.0.20.tar", last modified: Sun Feb 12 16:50:51 2023, max compression
+gzip compressed data, was "dist/simplegeomap-0.0.21.tar", last modified: Sat May  6 06:28:12 2023, max compression
```

## Comparing `simplegeomap-0.0.20.tar` & `simplegeomap-0.0.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.20/README.md
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/simplegeomap.egg-info/
--rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/simplegeomap.egg-info/dependency_links.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/simplegeomap.egg-info/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/simplegeomap.egg-info/top_level.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)       51 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/simplegeomap.egg-info/requires.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/simplegeomap.egg-info/SOURCES.txt
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/simplegeomap/
--rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.20/simplegeomap/__init__.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     6737 2023-02-12 16:44:41.000000 simplegeomap-0.0.20/simplegeomap/simplegeomap.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     4594 2023-02-11 07:38:14.000000 simplegeomap-0.0.20/simplegeomap/util.py
--rw-rw-r--   0 burak     (1000) burak     (1000)      626 2023-02-11 07:38:58.000000 simplegeomap-0.0.20/setup.py
--rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-02-12 16:50:50.000000 simplegeomap-0.0.20/setup.cfg
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.21/README.md
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/simplegeomap.egg-info/
+-rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/simplegeomap.egg-info/dependency_links.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/simplegeomap.egg-info/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/simplegeomap.egg-info/top_level.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)       51 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/simplegeomap.egg-info/requires.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/simplegeomap.egg-info/SOURCES.txt
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/simplegeomap/
+-rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.21/simplegeomap/__init__.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     6832 2023-05-05 19:47:10.000000 simplegeomap-0.0.21/simplegeomap/simplegeomap.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     4594 2023-02-11 07:38:14.000000 simplegeomap-0.0.21/simplegeomap/util.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)      626 2023-05-06 06:24:36.000000 simplegeomap-0.0.21/setup.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-05-06 06:28:12.000000 simplegeomap-0.0.21/setup.cfg
```

### Comparing `simplegeomap-0.0.20/PKG-INFO` & `simplegeomap-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.20
+Version: 0.0.21
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.20/README.md` & `simplegeomap-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.20/simplegeomap.egg-info/PKG-INFO` & `simplegeomap-0.0.21/simplegeomap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.20
+Version: 0.0.21
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.20/simplegeomap/simplegeomap.py` & `simplegeomap-0.0.21/simplegeomap/simplegeomap.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,72 +3,71 @@
 import matplotlib.pyplot as plt, scipy.interpolate
 import numpy as np, json, shapefile
 from simplegeomap.util import gltiles
 from scipy.ndimage import gaussian_filter
 
 GWIDTH = 200
 
-def plot_water_df(df,clat,clon,zoom):
+def plot_water_df(df,clat,clon,zoom,ax):
     MAX = 60
     CENTER_DIST = (40000. / MAX)*(zoom+1)
     p1 = LatLon(clat,clon) 
     dist = df.apply(lambda x: p1.distanceTo(LatLon(x['lat'],x['lon']))/1000.0, axis=1)
     df2 = df[dist < CENTER_DIST]
-    print ('dist',CENTER_DIST)
-    print ('river lake df',len(df2))
     for idx,row in df2.iterrows():
         geo = np.array(json.loads(row['polygon']))
         if 'lake' in row['type']: 
-            plt.fill(geo[:,1],geo[:,0],'blue',alpha=0.4)
+            ax.fill(geo[:,1],geo[:,0],'blue',alpha=0.4)
         if 'river' in row['type']: 
-            plt.plot(geo[:,1],geo[:,0],'blue',alpha=0.4)
+            ax.plot(geo[:,1],geo[:,0],'blue',alpha=0.4)
     
-def plot_water(clat,clon,zoom):
+def plot_water(clat,clon,zoom,ax=None):
+    if not ax: fig, ax = plt.subplots()
     data_dir = os.path.dirname(__file__)    
     with zipfile.ZipFile(data_dir + '/lake_river.zip', 'r') as z:
         df =  pd.read_csv(z.open('lake_river.csv'))
-        plot_water_df(df,clat,clon,zoom)
+        plot_water_df(df,clat,clon,zoom=zoom,ax=ax)
 
     df =  pd.read_csv(data_dir + '/lake_river_addn.csv')
-    plot_water_df(df,clat,clon,zoom)
+    plot_water_df(df,clat,clon,zoom,ax=ax)
         
    
-def plot_countries(clat,clon,zoom=7,incolor='lightyellow',outcolor='lightblue',country_color={}):
-
+def plot_countries(clat,clon,zoom=7,incolor='lightyellow',outcolor='lightblue',country_color={},ax=None):
+    if not ax: fig, ax = plt.subplots()
     data_dir = os.path.dirname(__file__)
     MAX = 20    
     CENTER_DIST = (40000. / MAX)*(zoom+1)
     xlims = (clon+(-180./MAX)*zoom, clon+(180./MAX)*zoom)
     ylims = (clat+(-90./MAX)*zoom, clat+(90./MAX)*zoom)
     p1 = LatLon(clat, clon)
-    plt.axes().set_facecolor(color=outcolor)
+    ax.set_facecolor(color=outcolor)
     sf = shapefile.Reader(data_dir + "/TM_WORLD_BORDERS-0.3.shp", encoding = "ISO8859-1")
     r = sf.records()
     countries = sf.shapes()
     for idx in range(len(countries)):
         country = countries[idx]
         name = r[idx]
         iso3 = r[idx][2]
         lat,lon = name[10],name[9] # middle point of country
         p2 = LatLon(lat, lon)
         d = p1.distanceTo(p2)/1000.0
         if d > CENTER_DIST: continue # skip if a country is too far        
         bounds = list(country.parts) + [len(country.points)]        
-        plt.xlim(xlims)
-        plt.ylim(ylims)        
+        ax.set_xlim(xlims)
+        ax.set_ylim(ylims)        
         for previous, current in zip(bounds, bounds[1:]):    
             geo = [[x[0],x[1]] for x in country.points[previous:current]]
             if len(geo) < 1: continue
             geo = np.array(geo)
             if geo.shape[0] > 0:
                 if iso3 in country_color: 
-                    plt.fill(geo[:,0],geo[:,1],country_color[iso3],alpha=0.5)
+                    ax.fill(geo[:,0],geo[:,1],country_color[iso3],alpha=0.5)
                 else:
-                    plt.fill(geo[:,0],geo[:,1],incolor,alpha=0.5)
-                plt.plot(geo[:,0],geo[:,1],'b')
+                    ax.fill(geo[:,0],geo[:,1],incolor,alpha=0.5)
+                ax.plot(geo[:,0],geo[:,1],'b')
 
 def create_grid(clat,clon,dist):    
     p1 = LatLon(clat,clon)
     EARTH_RAD = 6371
     upright = p1.destination (dist, bearing=45, radius=EARTH_RAD)
     lowleft = p1.destination (dist, bearing=225, radius=EARTH_RAD)
 
@@ -85,16 +84,16 @@
     
     return lats,lons, np.unique(glatints), np.unique(glonints)
 
 def find_tile(lat,lon):
     res = [lat >= x[0] and lon < x[1] and lon >= x[2] and lon < x[3] for x in gltiles.values()]
     return res.index(True)
 
-def plot_elevation(clat,clon,zoom,levels=None):
-
+def plot_elevation(clat,clon,zoom,levels=None,ax=None):
+    if not ax: fig, ax = plt.subplots()    
     data_dir = os.path.dirname(__file__)
     npz_file = data_dir + "/gltiles.npz"
     tkeys = np.array(list(gltiles.keys()))
     CENTER_DIST = 2000 * zoom
 
     glat,glon,glatints,glonints = create_grid(clat,clon,CENTER_DIST)
     
@@ -136,19 +135,19 @@
     newz = gaussian_filter(newz, sigma=1.0)
     if not levels:
         CS=plt.contour(newx,newy,newz,cmap=plt.cm.binary,levels=[500,1000,1500,2000,3000])
     else:
         CS=plt.contour(newx,newy,newz,cmap=plt.cm.binary,levels=levels)
     plt.clabel(CS, fontsize=10, inline=1)
     
-def plot_line(regarr,color='black',linestyle='solid'):
-    plt.plot(regarr[:,1],regarr[:,0],color=color,linestyle=linestyle)
+def plot_line(regarr,ax,color='black',linestyle='solid'):
+    ax.plot(regarr[:,1],regarr[:,0],color=color,linestyle=linestyle)
        
-def plot_region(regarr,color='lightgray',alpha=0.5):
-    plt.fill(regarr[:,1],regarr[:,0],color=color,alpha=alpha)
+def plot_region(regarr,ax,color='lightgray',alpha=0.5):
+    ax.fill(regarr[:,1],regarr[:,0],color=color,alpha=alpha)
     
 def find_city(name,country):
     data_dir = os.path.dirname(__file__)
     zip_file    = zipfile.ZipFile(data_dir + '/cities.zip')
     items_file  = zip_file.open('cities.csv')
     items_file  = io.TextIOWrapper(items_file)
     rd = csv.reader(items_file)
```

### Comparing `simplegeomap-0.0.20/simplegeomap/util.py` & `simplegeomap-0.0.21/simplegeomap/util.py`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.20/setup.py` & `simplegeomap-0.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 readme=open("README.md").read()
 
 setuptools.setup(
     name='simplegeomap',    
-    version='0.0.20',
+    version='0.0.21',
     description="Simple offline map plot utility, for country borders, elevation, water",
     long_description=readme,
     long_description_content_type="text/markdown",    
     install_requires=['pandas','pygeodesy','matplotlib','numpy','pyshp','scipy','zarr'],
     include_package_data=True,
     url="https://github.com/burakbayramli/simplegeomap",
     author="Burak Bayramli",
```

