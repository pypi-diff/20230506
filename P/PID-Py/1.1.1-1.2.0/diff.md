# Comparing `tmp/PID_Py-1.1.1.tar.gz` & `tmp/PID_Py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PID_Py-1.1.1.tar", last modified: Sat Mar 25 14:47:01 2023, max compression
+gzip compressed data, was "PID_Py-1.2.0.tar", last modified: Sat May  6 17:01:06 2023, max compression
```

## Comparing `PID_Py-1.1.1.tar` & `PID_Py-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-03-25 14:47:01.654356 PID_Py-1.1.1/
--rw-rw-r--   0 steven    (1000) steven    (1000)     1069 2023-03-15 17:57:43.000000 PID_Py-1.1.1/LICENSE
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-03-25 14:47:01.654356 PID_Py-1.1.1/PID_Py/
--rw-rw-r--   0 steven    (1000) steven    (1000)    29743 2023-03-25 13:47:54.000000 PID_Py-1.1.1/PID_Py/PID.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      671 2023-03-15 17:57:43.000000 PID_Py-1.1.1/PID_Py/Simulation.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      161 2023-03-15 17:57:43.000000 PID_Py-1.1.1/PID_Py/__init__.py
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-03-25 14:47:01.654356 PID_Py-1.1.1/PID_Py.egg-info/
--rw-rw-r--   0 steven    (1000) steven    (1000)    17052 2023-03-25 14:47:01.000000 PID_Py-1.1.1/PID_Py.egg-info/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)      206 2023-03-25 14:47:01.000000 PID_Py-1.1.1/PID_Py.egg-info/SOURCES.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        1 2023-03-25 14:47:01.000000 PID_Py-1.1.1/PID_Py.egg-info/dependency_links.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        7 2023-03-25 14:47:01.000000 PID_Py-1.1.1/PID_Py.egg-info/top_level.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)    17052 2023-03-25 14:47:01.654356 PID_Py-1.1.1/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)    14852 2023-03-25 14:44:46.000000 PID_Py-1.1.1/README.md
--rw-rw-r--   0 steven    (1000) steven    (1000)     1122 2023-03-25 14:31:04.000000 PID_Py-1.1.1/pyproject.toml
--rw-rw-r--   0 steven    (1000) steven    (1000)       38 2023-03-25 14:47:01.654356 PID_Py-1.1.1/setup.cfg
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-05-06 17:01:06.506507 PID_Py-1.2.0/
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1069 2023-03-15 17:57:43.000000 PID_Py-1.2.0/LICENSE
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-05-06 17:01:06.502508 PID_Py-1.2.0/PID_Py/
+-rw-rw-r--   0 steven    (1000) steven    (1000)    30083 2023-05-06 17:00:11.000000 PID_Py-1.2.0/PID_Py/PID.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)    48669 2023-05-06 17:00:11.000000 PID_Py-1.2.0/PID_Py/SetupTool.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)      671 2023-03-15 17:57:43.000000 PID_Py-1.2.0/PID_Py/Simulation.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)      161 2023-03-15 17:57:43.000000 PID_Py-1.2.0/PID_Py/__init__.py
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-05-06 17:01:06.506507 PID_Py-1.2.0/PID_Py.egg-info/
+-rw-rw-r--   0 steven    (1000) steven    (1000)    19159 2023-05-06 17:01:06.000000 PID_Py-1.2.0/PID_Py.egg-info/PKG-INFO
+-rw-rw-r--   0 steven    (1000) steven    (1000)      226 2023-05-06 17:01:06.000000 PID_Py-1.2.0/PID_Py.egg-info/SOURCES.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)        1 2023-05-06 17:01:06.000000 PID_Py-1.2.0/PID_Py.egg-info/dependency_links.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)        7 2023-05-06 17:01:06.000000 PID_Py-1.2.0/PID_Py.egg-info/top_level.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)    19159 2023-05-06 17:01:06.506507 PID_Py-1.2.0/PKG-INFO
+-rw-rw-r--   0 steven    (1000) steven    (1000)    16959 2023-05-06 17:00:11.000000 PID_Py-1.2.0/README.md
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1122 2023-05-06 17:00:11.000000 PID_Py-1.2.0/pyproject.toml
+-rw-rw-r--   0 steven    (1000) steven    (1000)       38 2023-05-06 17:01:06.506507 PID_Py-1.2.0/setup.cfg
```

### Comparing `PID_Py-1.1.1/LICENSE` & `PID_Py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PID_Py-1.1.1/PID_Py/PID.py` & `PID_Py-1.2.0/PID_Py/PID.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,17 @@
 
         self._p = 0.0
         self._i = 0.0
         self._d = 0.0
 
         self._setpoint = 0.0
 
+        self._setuptoolControl = False
+        self._setuptoolSetpoint = 0.0
+
         # Outputs
         self.output = 0.0
         self.processValueStabilized = False
         self.setpointReached = False
 
         # Logger
         self.logger = None
@@ -351,15 +354,19 @@
 
                 self.processValueStabilized = self._processValueCurrStableTime > self.processValueStableTime
             else:
                 self.processValueStabilized = False
                 self._processValueCurrStableTime = 0.0
 
             # ===== Setpoint ramp =====
-            setpointDiff = setpoint - self._setpoint
+            if not self._setuptoolControl:
+                setpointDiff = setpoint - self._setpoint
+                self._setuptoolSetpoint = setpoint
+            else:
+                setpointDiff = self._setuptoolSetpoint - self._setpoint
 
             if (self.setpointRamp is not None):
                 if (self.setpointRamp > 0.0):
                     if (setpointDiff > self.setpointRamp * deltaTime):
                         setpointDiff = self.setpointRamp * deltaTime
                     elif (setpointDiff < -self.setpointRamp * deltaTime):
                         setpointDiff = -self.setpointRamp * deltaTime
@@ -681,21 +688,21 @@
     
     def start(self) -> None:
         """
         Used to start the threaded PID. Overrided from `threading.Thread`
         See `threading.Thread` documentation for more information.
         """
         # Call PID execution to initialize time memory
-        self.compute(self.setpoint, self.processValue)
+        self.compute(self.setpoint, self.processValue if self.simulation is None else None)
         self.quit = False
         return Thread.start(self)
     
     def run(self):
         """
         Thread execution. Overrided from `threading.Thread`
         See `threading.Thread` documentation for more information
         """
         while self.quit is False:
             while time.time() < (self._lastTime + self.cycleTime):
                 time.sleep(self.cycleTime / 100.0)
 
-            self.compute(self.setpoint, self.processValue)
+            self.compute(self.setpoint, self.processValue if self.simulation is None else None)
```

### Comparing `PID_Py-1.1.1/PID_Py/Simulation.py` & `PID_Py-1.2.0/PID_Py/Simulation.py`

 * *Files identical despite different names*

### Comparing `PID_Py-1.1.1/PID_Py.egg-info/PKG-INFO` & `PID_Py-1.2.0/PID_Py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PID-Py
-Version: 1.1.1
+Version: 1.2.0
 Summary: Simple (but complete) PID controller in Python
 Author-email: ThunderTecke <thunder.tecke@gmail.com>
 Maintainer-email: ThunderTecke <thunder.tecke@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ThunderTecke
         
@@ -71,14 +71,18 @@
   - [Historian](#historian)
     - [Historian parameters list](#historian-parameters-list)
   - [Manual mode](#manual-mode)
   - [Logging](#logging)
   - [Time simulation](#time-simulation)
   - [Threaded PID](#threaded-pid)
   - [Simulation](#simulation)
+- [SetupTool](#setuptool)
+  - [Usage](#usage-1)
+  - [Read-only and read-write mode](#read-only-and-read-write-mode)
+  - [Control on PID](#control-on-pid)
 
 ## Installation
 ```
 python3 -m pip install PID_Py
 ```
 
 ## Usage
@@ -463,7 +467,65 @@
 simulation = Simulation(K = 1.0, tau = 0.1)
 pid = PID(kp = 2.0, ki = 5.0, kd = 0.0, simulation=simulation)
 
 ...
 
 command = pid(setpoint = targetValue)
 ```
+
+## SetupTool
+SetupTool is a tool to help you to configure the PID's parameters.
+A trend with the historian values is displayed to show the PID behaviour.
+
+### Usage
+To use SetupTool you need to import QApplication from PySide6.QtWidgets, then create an application and instantiate SetupTool.
+
+After the SetupTool is open, you can see real-time chart updated every second, and on the right all PID's parameters you can adjust in read-write mode.
+
+After having taken control on the setpoint, you can also send a new setpoint to the PID.
+
+```Python
+# PID imports
+from PID_Py.PID import PID, ThreadedPID, HistorianParams
+from PID_Py.SetupTool import SetupToolApp
+from PID_Py.Simulation import Simulation
+
+# PySide6 (PyQt) imports
+from PySide6.QtWidgets import QApplication
+
+import sys
+
+# Threaded PID creation
+pid = ThreadedPID(kp=1, ki=0, kd=0.0, 
+                  cycleTime=0.01, 
+                  historianParams=HistorianParams.SETPOINT | HistorianParams.PROCESS_VALUE, 
+                  simulation=Simulation(1, 1))
+pid.start()
+
+# PyQt application creation
+app = QApplication(sys.argv)
+
+# SetupTool instantiation
+setupToolApp = SetupToolApp(pid)
+setupToolApp.show()
+
+# Application execution
+app.exec()
+
+# Application ended, stop the PID
+pid.quit = True
+pid.join()
+```
+
+In the example above, a threaded PId is created and gave to SetupTool constructor.
+
+If have a not threaded PID, you can execute PyQt application in a parallel thread.
+
+### Read-only and read-write mode
+When SetupTool is instantiate the read-only mode is activated. This mode prevent any modification on the PID's parameters.
+
+If you want to modify PID's parameters you need to switch on read-write mode. Then all parameters are unlocked.
+
+### Control on PID
+When SetulTool is instantiate, you don't have the control on the setpoint.
+
+If you want to override setpoint, you need to take the control. Then the setpoint is unlocked. Write the new setpoint and then click on "apply".
```

### Comparing `PID_Py-1.1.1/PKG-INFO` & `PID_Py-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PID_Py
-Version: 1.1.1
+Version: 1.2.0
 Summary: Simple (but complete) PID controller in Python
 Author-email: ThunderTecke <thunder.tecke@gmail.com>
 Maintainer-email: ThunderTecke <thunder.tecke@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ThunderTecke
         
@@ -71,14 +71,18 @@
   - [Historian](#historian)
     - [Historian parameters list](#historian-parameters-list)
   - [Manual mode](#manual-mode)
   - [Logging](#logging)
   - [Time simulation](#time-simulation)
   - [Threaded PID](#threaded-pid)
   - [Simulation](#simulation)
+- [SetupTool](#setuptool)
+  - [Usage](#usage-1)
+  - [Read-only and read-write mode](#read-only-and-read-write-mode)
+  - [Control on PID](#control-on-pid)
 
 ## Installation
 ```
 python3 -m pip install PID_Py
 ```
 
 ## Usage
@@ -463,7 +467,65 @@
 simulation = Simulation(K = 1.0, tau = 0.1)
 pid = PID(kp = 2.0, ki = 5.0, kd = 0.0, simulation=simulation)
 
 ...
 
 command = pid(setpoint = targetValue)
 ```
+
+## SetupTool
+SetupTool is a tool to help you to configure the PID's parameters.
+A trend with the historian values is displayed to show the PID behaviour.
+
+### Usage
+To use SetupTool you need to import QApplication from PySide6.QtWidgets, then create an application and instantiate SetupTool.
+
+After the SetupTool is open, you can see real-time chart updated every second, and on the right all PID's parameters you can adjust in read-write mode.
+
+After having taken control on the setpoint, you can also send a new setpoint to the PID.
+
+```Python
+# PID imports
+from PID_Py.PID import PID, ThreadedPID, HistorianParams
+from PID_Py.SetupTool import SetupToolApp
+from PID_Py.Simulation import Simulation
+
+# PySide6 (PyQt) imports
+from PySide6.QtWidgets import QApplication
+
+import sys
+
+# Threaded PID creation
+pid = ThreadedPID(kp=1, ki=0, kd=0.0, 
+                  cycleTime=0.01, 
+                  historianParams=HistorianParams.SETPOINT | HistorianParams.PROCESS_VALUE, 
+                  simulation=Simulation(1, 1))
+pid.start()
+
+# PyQt application creation
+app = QApplication(sys.argv)
+
+# SetupTool instantiation
+setupToolApp = SetupToolApp(pid)
+setupToolApp.show()
+
+# Application execution
+app.exec()
+
+# Application ended, stop the PID
+pid.quit = True
+pid.join()
+```
+
+In the example above, a threaded PId is created and gave to SetupTool constructor.
+
+If have a not threaded PID, you can execute PyQt application in a parallel thread.
+
+### Read-only and read-write mode
+When SetupTool is instantiate the read-only mode is activated. This mode prevent any modification on the PID's parameters.
+
+If you want to modify PID's parameters you need to switch on read-write mode. Then all parameters are unlocked.
+
+### Control on PID
+When SetulTool is instantiate, you don't have the control on the setpoint.
+
+If you want to override setpoint, you need to take the control. Then the setpoint is unlocked. Write the new setpoint and then click on "apply".
```

### Comparing `PID_Py-1.1.1/README.md` & `PID_Py-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,18 @@
   - [Historian](#historian)
     - [Historian parameters list](#historian-parameters-list)
   - [Manual mode](#manual-mode)
   - [Logging](#logging)
   - [Time simulation](#time-simulation)
   - [Threaded PID](#threaded-pid)
   - [Simulation](#simulation)
+- [SetupTool](#setuptool)
+  - [Usage](#usage-1)
+  - [Read-only and read-write mode](#read-only-and-read-write-mode)
+  - [Control on PID](#control-on-pid)
 
 ## Installation
 ```
 python3 -m pip install PID_Py
 ```
 
 ## Usage
@@ -419,8 +423,66 @@
 # Initialization
 simulation = Simulation(K = 1.0, tau = 0.1)
 pid = PID(kp = 2.0, ki = 5.0, kd = 0.0, simulation=simulation)
 
 ...
 
 command = pid(setpoint = targetValue)
-```
+```
+
+## SetupTool
+SetupTool is a tool to help you to configure the PID's parameters.
+A trend with the historian values is displayed to show the PID behaviour.
+
+### Usage
+To use SetupTool you need to import QApplication from PySide6.QtWidgets, then create an application and instantiate SetupTool.
+
+After the SetupTool is open, you can see real-time chart updated every second, and on the right all PID's parameters you can adjust in read-write mode.
+
+After having taken control on the setpoint, you can also send a new setpoint to the PID.
+
+```Python
+# PID imports
+from PID_Py.PID import PID, ThreadedPID, HistorianParams
+from PID_Py.SetupTool import SetupToolApp
+from PID_Py.Simulation import Simulation
+
+# PySide6 (PyQt) imports
+from PySide6.QtWidgets import QApplication
+
+import sys
+
+# Threaded PID creation
+pid = ThreadedPID(kp=1, ki=0, kd=0.0, 
+                  cycleTime=0.01, 
+                  historianParams=HistorianParams.SETPOINT | HistorianParams.PROCESS_VALUE, 
+                  simulation=Simulation(1, 1))
+pid.start()
+
+# PyQt application creation
+app = QApplication(sys.argv)
+
+# SetupTool instantiation
+setupToolApp = SetupToolApp(pid)
+setupToolApp.show()
+
+# Application execution
+app.exec()
+
+# Application ended, stop the PID
+pid.quit = True
+pid.join()
+```
+
+In the example above, a threaded PId is created and gave to SetupTool constructor.
+
+If have a not threaded PID, you can execute PyQt application in a parallel thread.
+
+### Read-only and read-write mode
+When SetupTool is instantiate the read-only mode is activated. This mode prevent any modification on the PID's parameters.
+
+If you want to modify PID's parameters you need to switch on read-write mode. Then all parameters are unlocked.
+
+### Control on PID
+When SetulTool is instantiate, you don't have the control on the setpoint.
+
+If you want to override setpoint, you need to take the control. Then the setpoint is unlocked. Write the new setpoint and then click on "apply".
```

### Comparing `PID_Py-1.1.1/pyproject.toml` & `PID_Py-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["PID_Py"]
 
 [project]
 name = "PID_Py"
-version = "1.1.1"
+version = "1.2.0"
 authors = [{name = "ThunderTecke", email = "thunder.tecke@gmail.com"}]
 maintainers = [{name = "ThunderTecke", email = "thunder.tecke@gmail.com"}]
 keywords = ["pid", "controller", "pid-controller", "control", "pid-control", "python", "raspberry", "raspberrypi", "raspberry-pi"]
 description = "Simple (but complete) PID controller in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

