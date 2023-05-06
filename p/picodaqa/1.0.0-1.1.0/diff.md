# Comparing `tmp/picodaqa-1.0.0.tar.gz` & `tmp/picodaqa-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodaqa-1.0.0.tar", last modified: Sun Oct  9 14:02:27 2022, max compression
+gzip compressed data, was "dist/picodaqa-1.1.0.tar", last modified: Sat May  6 15:28:21 2023, max compression
```

## Comparing `picodaqa-1.0.0.tar` & `picodaqa-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 quast     (1000) quast     (1000)        0 2022-10-09 14:02:27.906469 picodaqa-1.0.0/
--rw-rw-r--   0 quast     (1000) quast     (1000)    10116 2022-10-09 14:02:27.906469 picodaqa-1.0.0/PKG-INFO
--rw-rw-r--   0 quast     (1000) quast     (1000)     8349 2022-10-09 13:59:32.000000 picodaqa-1.0.0/README.md
-drwxrwxr-x   0 quast     (1000) quast     (1000)        0 2022-10-09 14:02:27.906469 picodaqa-1.0.0/picodaqa/
--rw-rw-r--   0 quast     (1000) quast     (1000)     2990 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/BarDisplay.py
--rw-rw-r--   0 quast     (1000) quast     (1000)    21247 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/BufferMan.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     7301 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/DataGraphs.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     2912 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/DataLogger.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     5791 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/Oscilloscope.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     2531 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/RMeter.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     6287 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/VoltMeter.py
--rw-rw-r--   0 quast     (1000) quast     (1000)      882 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/__init__.py
--rw-rw-r--   0 quast     (1000) quast     (1000)      412 2022-10-09 13:29:37.000000 picodaqa-1.0.0/picodaqa/_version_info.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     4607 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/animHists.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     2502 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/mpBDisplay.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     4294 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/mpBufManCntrl.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     4379 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/mpDataGraphs.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     4561 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/mpDataLogger.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     1914 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/mpHists.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     2250 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/mpOsci.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     3048 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/mpRMeter.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     2219 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/mpVMeter.py
--rw-rw-r--   0 quast     (1000) quast     (1000)    11331 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/picoConfig.py
--rw-rw-r--   0 quast     (1000) quast     (1000)     2820 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/plotBufManInfo.py
--rw-rw-r--   0 quast     (1000) quast     (1000)      917 2020-08-02 08:16:05.000000 picodaqa-1.0.0/picodaqa/read_config.py
-drwxrwxr-x   0 quast     (1000) quast     (1000)        0 2022-10-09 14:02:27.906469 picodaqa-1.0.0/picodaqa.egg-info/
--rw-rw-r--   0 quast     (1000) quast     (1000)    10116 2022-10-09 14:02:27.000000 picodaqa-1.0.0/picodaqa.egg-info/PKG-INFO
--rw-rw-r--   0 quast     (1000) quast     (1000)      626 2022-10-09 14:02:27.000000 picodaqa-1.0.0/picodaqa.egg-info/SOURCES.txt
--rw-rw-r--   0 quast     (1000) quast     (1000)        1 2022-10-09 14:02:27.000000 picodaqa-1.0.0/picodaqa.egg-info/dependency_links.txt
--rw-rw-r--   0 quast     (1000) quast     (1000)        9 2022-10-09 14:02:27.000000 picodaqa-1.0.0/picodaqa.egg-info/top_level.txt
--rw-rw-r--   0 quast     (1000) quast     (1000)       38 2022-10-09 14:02:27.906469 picodaqa-1.0.0/setup.cfg
--rw-rw-r--   0 quast     (1000) quast     (1000)     1508 2022-10-09 13:50:37.000000 picodaqa-1.0.0/setup.py
+drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-05-06 15:28:21.000000 picodaqa-1.1.0/
+-rw-r--r--   0 quast     (1000) users      (100)    10116 2023-05-06 15:28:21.000000 picodaqa-1.1.0/PKG-INFO
+-rw-r--r--   0 quast     (1000) users      (100)     8349 2022-10-10 18:35:00.000000 picodaqa-1.1.0/README.md
+drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa/
+-rw-r--r--   0 quast     (1000) users      (100)     2990 2019-09-08 19:19:42.000000 picodaqa-1.1.0/picodaqa/BarDisplay.py
+-rw-r--r--   0 quast     (1000) users      (100)    21247 2021-12-04 17:30:18.000000 picodaqa-1.1.0/picodaqa/BufferMan.py
+-rw-r--r--   0 quast     (1000) users      (100)     7301 2018-07-08 15:33:17.000000 picodaqa-1.1.0/picodaqa/DataGraphs.py
+-rw-r--r--   0 quast     (1000) users      (100)     2912 2018-07-08 12:48:15.000000 picodaqa-1.1.0/picodaqa/DataLogger.py
+-rw-r--r--   0 quast     (1000) users      (100)     5791 2019-09-08 19:19:42.000000 picodaqa-1.1.0/picodaqa/Oscilloscope.py
+-rw-r--r--   0 quast     (1000) users      (100)     2531 2019-10-02 16:56:42.000000 picodaqa-1.1.0/picodaqa/RMeter.py
+-rw-r--r--   0 quast     (1000) users      (100)     6287 2018-07-08 12:55:27.000000 picodaqa-1.1.0/picodaqa/VoltMeter.py
+-rw-r--r--   0 quast     (1000) users      (100)      882 2019-10-02 16:56:42.000000 picodaqa-1.1.0/picodaqa/__init__.py
+-rw-r--r--   0 quast     (1000) users      (100)      412 2023-05-06 15:28:17.000000 picodaqa-1.1.0/picodaqa/_version_info.py
+-rw-r--r--   0 quast     (1000) users      (100)     4689 2023-05-06 15:23:04.000000 picodaqa-1.1.0/picodaqa/animHists.py
+-rw-r--r--   0 quast     (1000) users      (100)     2502 2019-09-08 19:19:42.000000 picodaqa-1.1.0/picodaqa/mpBDisplay.py
+-rw-r--r--   0 quast     (1000) users      (100)     4294 2018-04-10 16:28:40.000000 picodaqa-1.1.0/picodaqa/mpBufManCntrl.py
+-rw-r--r--   0 quast     (1000) users      (100)     4379 2018-07-08 13:07:03.000000 picodaqa-1.1.0/picodaqa/mpDataGraphs.py
+-rw-r--r--   0 quast     (1000) users      (100)     4561 2018-07-07 06:17:08.000000 picodaqa-1.1.0/picodaqa/mpDataLogger.py
+-rw-r--r--   0 quast     (1000) users      (100)     1914 2018-03-10 19:32:27.000000 picodaqa-1.1.0/picodaqa/mpHists.py
+-rw-r--r--   0 quast     (1000) users      (100)     2250 2018-04-10 16:29:11.000000 picodaqa-1.1.0/picodaqa/mpOsci.py
+-rw-r--r--   0 quast     (1000) users      (100)     3048 2019-05-01 07:50:58.000000 picodaqa-1.1.0/picodaqa/mpRMeter.py
+-rw-r--r--   0 quast     (1000) users      (100)     2219 2018-05-15 16:03:19.000000 picodaqa-1.1.0/picodaqa/mpVMeter.py
+-rw-r--r--   0 quast     (1000) users      (100)    11336 2023-05-05 17:43:58.000000 picodaqa-1.1.0/picodaqa/picoConfig.py
+-rw-r--r--   0 quast     (1000) users      (100)     2820 2018-03-11 09:01:11.000000 picodaqa-1.1.0/picodaqa/plotBufManInfo.py
+-rw-r--r--   0 quast     (1000) users      (100)      917 2018-02-04 12:05:17.000000 picodaqa-1.1.0/picodaqa/read_config.py
+drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/
+-rw-r--r--   0 quast     (1000) users      (100)    10116 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/PKG-INFO
+-rw-r--r--   0 quast     (1000) users      (100)      626 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/SOURCES.txt
+-rw-r--r--   0 quast     (1000) users      (100)        1 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/dependency_links.txt
+-rw-r--r--   0 quast     (1000) users      (100)        9 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/top_level.txt
+-rw-r--r--   0 quast     (1000) users      (100)       38 2023-05-06 15:28:21.000000 picodaqa-1.1.0/setup.cfg
+-rw-r--r--   0 quast     (1000) users      (100)     1508 2022-10-09 13:31:42.000000 picodaqa-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `picodaqa-1.0.0/PKG-INFO` & `picodaqa-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: picodaqa
-Version: 1.0.0
+Version: 1.1.0
 Summary: Data AcQuisition and analysis with PicoScope usb-oscilloscopes
 Home-page: https://www.etp.kit.edu/~quast/
 Author: Guenter Quast
 Author-email: Guenter.Quast@online.de
 License: GNU Public Licence
 Description: # picoDAQ
```

### Comparing `picodaqa-1.0.0/README.md` & `picodaqa-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/BarDisplay.py` & `picodaqa-1.1.0/picodaqa/BarDisplay.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/BufferMan.py` & `picodaqa-1.1.0/picodaqa/BufferMan.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/DataGraphs.py` & `picodaqa-1.1.0/picodaqa/DataGraphs.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/DataLogger.py` & `picodaqa-1.1.0/picodaqa/DataLogger.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/Oscilloscope.py` & `picodaqa-1.1.0/picodaqa/Oscilloscope.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/RMeter.py` & `picodaqa-1.1.0/picodaqa/RMeter.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/VoltMeter.py` & `picodaqa-1.1.0/picodaqa/VoltMeter.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/__init__.py` & `picodaqa-1.1.0/picodaqa/__init__.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/animHists.py` & `picodaqa-1.1.0/picodaqa/animHists.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
   # create figure
     ncols = int(np.sqrt(self.nHist))
     nrows = ncols
     if ncols * nrows < self.nHist: nrows +=1
     if ncols * nrows < self.nHist: ncols +=1
     self.fig, axarray = plt.subplots(nrows=nrows, ncols=ncols,
                                           figsize=(3.*ncols, 2.*nrows) )
-    self.fig.canvas.set_window_title(name)
+    #!   deprecated sind vers. 3.4 self.fig.canvas.set_window_title(name)
+    self.fig.canvas.manager.set_window_title(name)
     self.fig.subplots_adjust(left=0.25/ncols, bottom=0.25/nrows, right=0.975, top=0.95,
                              wspace=0.35, hspace=0.35)
 # sort axes in linear array
     self.axes = []
     if self.nHist == 1:
       self.axes = [axarray]
     elif self.nHist == 2:
```

### Comparing `picodaqa-1.0.0/picodaqa/mpBDisplay.py` & `picodaqa-1.1.0/picodaqa/mpBDisplay.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/mpBufManCntrl.py` & `picodaqa-1.1.0/picodaqa/mpBufManCntrl.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/mpDataGraphs.py` & `picodaqa-1.1.0/picodaqa/mpDataGraphs.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/mpDataLogger.py` & `picodaqa-1.1.0/picodaqa/mpDataLogger.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/mpHists.py` & `picodaqa-1.1.0/picodaqa/mpHists.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/mpOsci.py` & `picodaqa-1.1.0/picodaqa/mpOsci.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/mpRMeter.py` & `picodaqa-1.1.0/picodaqa/mpRMeter.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/mpVMeter.py` & `picodaqa-1.1.0/picodaqa/mpVMeter.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/picoConfig.py` & `picodaqa-1.1.0/picodaqa/picoConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         print(prompt+"picoIni: trigger inactive")
 
 # 4) enable Signal Generator 
     if self.frqSG !=0. :
       self.picoDevice.setSigGenBuiltInSimple(frequency=self.frqSG, 
          pkToPk=self.PkToPkSG, waveType=self.waveTypeSG, 
          offsetVoltage=self.offsetVoltageSG, sweepType=self.swpSG, 
-         dwellTime=self.dwellTimeSG, stopFreq=self.stopFreqSG)
+         dwellTime=self.dwellTimeSG, stopFrequency=self.stopFreqSG)
       if verbose>0:
         print(prompt+"signal generator enabled: %.3gHz, +/-%.3g V %s"\
             % (self.frqSG, self.PkToPkSG, self.waveTypeSG) )
         print(prompt+"sweep type %s, stop %.3gHz, Tdwell %.3gs"\
             %(self.swpSG, self.stopFreqSG, self.dwellTimeSG) )
 
     self.setSamplingPars(TSampling, NSamples, CRanges) # store in config class
```

### Comparing `picodaqa-1.0.0/picodaqa/plotBufManInfo.py` & `picodaqa-1.1.0/picodaqa/plotBufManInfo.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa/read_config.py` & `picodaqa-1.1.0/picodaqa/read_config.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/picodaqa.egg-info/PKG-INFO` & `picodaqa-1.1.0/picodaqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: picodaqa
-Version: 1.0.0
+Version: 1.1.0
 Summary: Data AcQuisition and analysis with PicoScope usb-oscilloscopes
 Home-page: https://www.etp.kit.edu/~quast/
 Author: Guenter Quast
 Author-email: Guenter.Quast@online.de
 License: GNU Public Licence
 Description: # picoDAQ
```

### Comparing `picodaqa-1.0.0/picodaqa.egg-info/SOURCES.txt` & `picodaqa-1.1.0/picodaqa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picodaqa-1.0.0/setup.py` & `picodaqa-1.1.0/setup.py`

 * *Files identical despite different names*

