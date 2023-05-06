# Comparing `tmp/midlife-0.0.4.tar.gz` & `tmp/midlife-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midlife-0.0.4.tar", last modified: Sat May  6 03:23:48 2023, max compression
+gzip compressed data, was "midlife-0.0.5.tar", last modified: Sat May  6 06:45:07 2023, max compression
```

## Comparing `midlife-0.0.4.tar` & `midlife-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 03:23:48.900654 midlife-0.0.4/
--rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 03:23:48.899697 midlife-0.0.4/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      729 2023-05-06 02:04:11.000000 midlife-0.0.4/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-05-06 03:23:48.900654 midlife-0.0.4/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      932 2023-05-06 03:23:26.000000 midlife-0.0.4/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 03:23:48.891521 midlife-0.0.4/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 03:23:48.898824 midlife-0.0.4/src/midlife.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      211 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       42 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        8 2023-05-06 03:23:48.000000 midlife-0.0.4/src/midlife.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2639 2023-05-06 03:23:12.000000 midlife-0.0.4/src/midlife.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 06:45:07.486847 midlife-0.0.5/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 06:45:07.486177 midlife-0.0.5/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      729 2023-05-06 02:04:11.000000 midlife-0.0.5/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-05-06 06:45:07.487847 midlife-0.0.5/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      932 2023-05-06 06:44:38.000000 midlife-0.0.5/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 06:45:07.468227 midlife-0.0.5/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-05-06 06:45:07.485181 midlife-0.0.5/src/midlife.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1244 2023-05-06 06:45:07.000000 midlife-0.0.5/src/midlife.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      211 2023-05-06 06:45:07.000000 midlife-0.0.5/src/midlife.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-05-06 06:45:07.000000 midlife-0.0.5/src/midlife.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       42 2023-05-06 06:45:07.000000 midlife-0.0.5/src/midlife.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        8 2023-05-06 06:45:07.000000 midlife-0.0.5/src/midlife.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     2703 2023-05-06 05:18:54.000000 midlife-0.0.5/src/midlife.py
```

### Comparing `midlife-0.0.4/PKG-INFO` & `midlife-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midlife
-Version: 0.0.4
+Version: 0.0.5
 Summary: impact of COVID-19 on mortality of midlife
 Home-page: https://github.com/ytakefuji/vuv
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/midlife
 Platform: UNKNOWN
```

### Comparing `midlife-0.0.4/README.md` & `midlife-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `midlife-0.0.4/setup.py` & `midlife-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="midlife",
-    version="0.0.4",
+    version="0.0.5",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="impact of COVID-19 on mortality of midlife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/vuv",
     project_urls={
```

### Comparing `midlife-0.0.4/src/midlife.egg-info/PKG-INFO` & `midlife-0.0.5/src/midlife.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midlife
-Version: 0.0.4
+Version: 0.0.5
 Summary: impact of COVID-19 on mortality of midlife
 Home-page: https://github.com/ytakefuji/vuv
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/midlife
 Platform: UNKNOWN
```

### Comparing `midlife-0.0.4/src/midlife.py` & `midlife-0.0.5/src/midlife.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,40 +34,49 @@
  a=d.loc[(d.Year==i) &
   (d['Sex']==sex) & (d['Age Group']=='55-59 years'),'Total Deaths']
  a4.append(int(a))
  a=d.loc[(d.Year==i) &
   (d['Sex']==sex) & (d['Age Group']=='60-64 years'),'Total Deaths']
  a5.append(int(a))
 
-model=np.poly1d(np.polyfit(years[0:-2],a1[0:-2],degree))
-print('40-44 years:',round((a1[-1]-int(model(2020)))/int(model(2020)),3))
-error=r2(model(years[0:-2]),a1[0:-2])
+X=range(6)
+model=np.poly1d(np.polyfit(X[0:5],a1[0:5],degree))
+print('40-44 years:',round((a1[5]-int(model(5)))/int(model(5)),3))
+error=r2(model(X[0:5]),a1[0:5])
 print('r2=',round(error,3),'\n')
-#print(a1)
-#print(int(model(2020)),'\n')
+print(a1)
+print(int(model(5)),'\n')
 
-model=np.poly1d(np.polyfit(years[0:-2],a2[0:-2],degree))
-print('45:49 years:',round((a2[-1]-int(model(2020)))/int(model(2020)),3))
-error=r2(model(years[0:-2]),a2[0:-2])
+model=np.poly1d(np.polyfit(X[0:5],a2[0:5],degree))
+print('45:49 years:',round((a2[5]-int(model(5)))/int(model(5)),3))
+error=r2(model(X[0:5]),a2[0:5])
 print('r2=',round(error,3),'\n')
+print(a2)
+print(int(model(5)),'\n')
 
-model=np.poly1d(np.polyfit(years[0:-2],a3[0:-2],degree))
-print('50-54 years:',round((a3[-1]-int(model(2020)))/int(model(2020)),3))
-error=r2(model(years[0:-2]),a3[0:-2])
+model=np.poly1d(np.polyfit(X[0:5],a3[0:5],degree))
+print('50-54 years:',round((a3[5]-int(model(5)))/int(model(5)),3))
+error=r2(model(X[0:5]),a3[0:5])
 print('r2=',round(error,3),'\n')
+print(a3)
+print(int(model(5)),'\n')
 
-model=np.poly1d(np.polyfit(years[0:-2],a4[0:-2],degree))
-print('55-59 years:',round((a4[-1]-int(model(2020)))/int(model(2020)),3))
-error=r2(model(years[0:-2]),a4[0:-2])
+model=np.poly1d(np.polyfit(X[0:5],a4[0:5],degree))
+print('55-59 years:',round((a4[5]-int(model(5)))/int(model(5)),3))
+error=r2(model(X[0:5]),a4[0:5])
 print('r2=',round(error,3),'\n')
+print(a4)
+print(int(model(5)),'\n')
 
-model=np.poly1d(np.polyfit(years[0:-2],a5[0:-2],degree))
-print('60-65 years:',round((a5[-1]-int(model(2020)))/int(model(2020)),3))
-error=r2(model(years[0:-2]),a5[0:-2])
+model=np.poly1d(np.polyfit(X[0:5],a5[0:5],degree))
+print('60-65 years:',round((a5[5]-int(model(5)))/int(model(5)),3))
+error=r2(model(X[0:5]),a5[0:5])
 print('r2=',round(error,3),'\n')
+print(a5)
+print(int(model(5)),'\n')
 
 def main():
  plt.ylim([0,170000])
  plt.plot(years,a1,':k')
  plt.plot(years,a2,'-k')
  plt.plot(years,a3,'--k')
  plt.plot(years,a4,'-.k')
```

