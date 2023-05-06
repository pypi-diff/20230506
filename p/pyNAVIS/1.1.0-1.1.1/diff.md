# Comparing `tmp/pyNAVIS-1.1.0.tar.gz` & `tmp/pyNAVIS-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNAVIS-1.1.0.tar", last modified: Wed Jun 16 11:14:26 2021, max compression
+gzip compressed data, was "pyNAVIS-1.1.1.tar", last modified: Sat May  6 10:12:51 2023, max compression
```

## Comparing `pyNAVIS-1.1.0.tar` & `pyNAVIS-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2021-06-16 11:14:26.782433 pyNAVIS-1.1.0/
--rw-rw-rw-   0        0        0     4899 2021-06-16 11:14:26.782433 pyNAVIS-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-06-16 11:14:26.748523 pyNAVIS-1.1.0/pyNAVIS/
--rw-rw-rw-   0        0        0      331 2021-06-16 10:15:49.000000 pyNAVIS-1.1.0/pyNAVIS/__init__.py
--rw-rw-rw-   0        0        0     8395 2021-06-16 11:03:42.000000 pyNAVIS-1.1.0/pyNAVIS/dataset_gen.py
--rw-rw-rw-   0        0        0    23563 2021-06-16 11:08:57.000000 pyNAVIS-1.1.0/pyNAVIS/functions.py
--rw-rw-rw-   0        0        0     8366 2020-06-16 08:16:10.000000 pyNAVIS-1.1.0/pyNAVIS/generators.py
--rw-rw-rw-   0        0        0    22918 2021-06-16 10:15:53.000000 pyNAVIS-1.1.0/pyNAVIS/loaders.py
--rw-rw-rw-   0        0        0     5108 2021-06-16 10:15:49.000000 pyNAVIS-1.1.0/pyNAVIS/main_settings.py
--rw-rw-rw-   0        0        0    35072 2021-06-16 10:53:49.000000 pyNAVIS-1.1.0/pyNAVIS/plots.py
--rw-rw-rw-   0        0        0    10205 2021-06-16 10:15:53.000000 pyNAVIS-1.1.0/pyNAVIS/savers.py
--rw-rw-rw-   0        0        0     9219 2020-12-01 18:45:13.000000 pyNAVIS-1.1.0/pyNAVIS/splitters.py
--rw-rw-rw-   0        0        0     4061 2021-01-25 17:31:47.000000 pyNAVIS-1.1.0/pyNAVIS/utils.py
-drwxrwxrwx   0        0        0        0 2021-06-16 11:14:26.781434 pyNAVIS-1.1.0/pyNAVIS.egg-info/
--rw-rw-rw-   0        0        0     4899 2021-06-16 11:14:26.000000 pyNAVIS-1.1.0/pyNAVIS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2021-06-16 11:14:26.000000 pyNAVIS-1.1.0/pyNAVIS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-16 11:14:26.000000 pyNAVIS-1.1.0/pyNAVIS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2021-06-16 11:14:26.000000 pyNAVIS-1.1.0/pyNAVIS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-06-16 11:14:26.000000 pyNAVIS-1.1.0/pyNAVIS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-06-16 11:14:26.782433 pyNAVIS-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      983 2021-06-16 11:11:52.000000 pyNAVIS-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:12:51.962733 pyNAVIS-1.1.1/
+-rw-rw-rw-   0        0        0     5225 2023-05-06 10:12:51.962733 pyNAVIS-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 10:12:51.899722 pyNAVIS-1.1.1/pyNAVIS/
+-rw-rw-rw-   0        0        0      399 2023-05-06 10:02:02.000000 pyNAVIS-1.1.1/pyNAVIS/__init__.py
+-rw-rw-rw-   0        0        0     8409 2023-05-06 10:00:39.000000 pyNAVIS-1.1.1/pyNAVIS/dataset_gen.py
+-rw-rw-rw-   0        0        0    18548 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/functions.py
+-rw-rw-rw-   0        0        0     8149 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/generators.py
+-rw-rw-rw-   0        0        0    22338 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/loaders.py
+-rw-rw-rw-   0        0        0     5287 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/main_settings.py
+-rw-rw-rw-   0        0        0     2268 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/objects.py
+-rw-rw-rw-   0        0        0    35380 2023-05-06 10:06:46.000000 pyNAVIS-1.1.1/pyNAVIS/plots.py
+-rw-rw-rw-   0        0        0     7950 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/report_functions.py
+-rw-rw-rw-   0        0        0    10205 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/savers.py
+-rw-rw-rw-   0        0        0     9241 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/splitters.py
+-rw-rw-rw-   0        0        0     3974 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:12:51.946938 pyNAVIS-1.1.1/pyNAVIS.egg-info/
+-rw-rw-rw-   0        0        0     5225 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 10:12:51.962733 pyNAVIS-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-05-06 10:10:16.000000 pyNAVIS-1.1.1/setup.py
```

### Comparing `pyNAVIS-1.1.0/pyNAVIS/dataset_gen.py` & `pyNAVIS-1.1.1/pyNAVIS/dataset_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,22 @@
 #################################################################################
 
 import os
 import time
 import matplotlib
 import numpy as np
 
+"""
+
 from .functions import Functions
 from .loaders import Loaders
 from .plots import Plots
 from .savers import Savers
+"""
+
 
 class DatasetGenerators:
 
     @staticmethod
     def generate_sonogram_dataset(path_input_folder, path_output_folder, settings, allow_subdirectories = False, verbose = False):
         """
         Automatically generates and saves sonograms from a set of AEDAT files.
```

### Comparing `pyNAVIS-1.1.0/pyNAVIS/functions.py` & `pyNAVIS-1.1.1/pyNAVIS/functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,84 +15,84 @@
 ##    GNU General Public License for more details.                             ##
 ##                                                                             ##
 ##    You should have received a copy of the GNU General Public License        ##
 ##    along with pyNAVIS.  If not, see <http://www.gnu.org/licenses/>.         ##
 ##                                                                             ##
 #################################################################################
 
-import math
-import struct
-import time
 import copy
 import random
-import datetime
-import os
+import time
 
-import matplotlib.backends.backend_pdf
-import matplotlib.pyplot as plt
 import numpy as np
 
-from .loaders import SpikesFile
-from .loaders import LocalizationFile
-from .loaders import Loaders
+# from .objects import LocalizationFile
+from .objects import SpikesFile
 from .savers import Savers
 from .utils import Utils
-from .plots import Plots
+
 
 class Functions:
 
 	@staticmethod
 	def check_SpikesFile(spikes_file, settings):
 		"""
-		Checks if the spiking information contained in the SpikesFile is correct and prints "The loaded SpikesFile file has been checked and it's OK" if the file passes all the checks.
-		
-		Parameters:
-				spikes_file (SpikesFile): File to check.
-				settings (MainSettings): Configuration parameters for the file to check.
-
-		Returns:
-				None.
-		
-		Raises:
-				TimestampOrderError: If the SpikesFile contains at least one timestamp which value is less than 0.
-				TimestampOrderError: If the SpikesFile contains at least one timestamp that is lesser than its previous one.
-				AddressValueError: If the SpikesFile contains at least one address less than 0 or greater than the num_channels that you specified in the MainSettings.
-		Notes:   
-				If mono_stereo is set to 1 (stereo) in the MainSettings, then  addresses should be less than num_channels*2.
+        Checks if the spiking information contained in the SpikesFile is correct and prints "The loaded SpikesFile file has been checked and it's OK" if the file passes all the checks.
 
-				If on_off_both is set to 1 (both) in the MainSettings, then addresses should be less than num_channels*2.
-				
-				If mono_stereo is set to 1 and on_off_both is set to 1 in the MainSettings, then addresses should be less than num_channels*2*2.
-		"""
+        Parameters:
+                spikes_file (SpikesFile): File to check.
+                settings (MainSettings): Configuration parameters for the file to check.
+
+        Returns:
+                None.
+
+        Raises:
+                TimestampOrderError: If the SpikesFile contains at least one timestamp which value is less than 0.
+                TimestampOrderError: If the SpikesFile contains at least one timestamp that is lesser than its previous one.
+                AddressValueError: If the SpikesFile contains at least one address less than 0 or greater than the num_channels that you specified in the MainSettings.
+        Notes:
+                If mono_stereo is set to 1 (stereo) in the MainSettings, then  addresses should be less than num_channels*2.
+
+                If on_off_both is set to 1 (both) in the MainSettings, then addresses should be less than num_channels*2.
+
+                If mono_stereo is set to 1 and on_off_both is set to 1 in the MainSettings, then addresses should be less than num_channels*2*2.
+        """
+		# Convert to numpy arrays
+		addresses = np.array(spikes_file.addresses, copy=False)
+		timestamps = np.array(spikes_file.timestamps, copy=False)
 
-		if settings.on_off_both == 1:
-			number_of_addresses = settings.num_channels*2
-		else:
-			number_of_addresses = settings.num_channels
 		# Check if all timestamps are greater than zero
-		a = all(item >= 0  for item in spikes_file.timestamps)
+		any_negative = np.any(timestamps < 0)
 
-		if not a:
+		if any_negative:
 			print("[Functions.check_SpikesFile] > TimestampOrderError: The SpikesFile file that you loaded has at least one timestamp that is less than 0.")
 
 		# Check if each timestamp is greater than its previous one
-		b = not any(i > 0 and spikes_file.timestamps[i] < spikes_file.timestamps[i-1] for i in range(len(spikes_file.timestamps)))
+		increasing_order = np.all(timestamps[:-1] <= timestamps[1:])
 
-		if not b:
+		if not increasing_order:
 			print("[Functions.check_SpikesFile] > TimestampOrderError: The SpikesFile file that you loaded has at least one timestamp whose value is lesser than its previous one.")
 
+		# Calculate maximum number of addresses
+		number_of_addresses = settings.num_channels * (settings.on_off_both + 1) * (settings.mono_stereo + 1)
+
 		# Check if all addresses are between zero and the total number of addresses
-		c = all(item >= 0 and item < number_of_addresses*(settings.mono_stereo + 1) for item in spikes_file.addresses)
+		all_in_range = np.all((addresses >= 0) & (addresses < number_of_addresses))
 
-		if not c:
+		if not all_in_range:
 			print("[Functions.check_SpikesFile] > AddressValueError: The SpikesFile file that you loaded has at least one event whose address is either less than 0 or greater than the number of addresses that you specified.")
 
-		if a and b and c:
+		# Check if all is OK
+		all_ok = not any_negative and increasing_order and all_in_range
+
+		if all_ok:
 			print("[Functions.check_SpikesFile] > The loaded SpikesFile file has been checked and it's OK")
-				
+
+		return not any_negative, increasing_order, all_in_range
+
 	@staticmethod
 	def check_LocalizationFile(localization_file, settings, localization_settings):
 		"""
 		Checks if the spiking information contained in the LocalizationFile is correct and prints "The loaded LocalizationFile file has been checked and it's OK" if the file passes all the checks.
 		
 		Parameters:
 				localization_file (LocalizationFile): File to check.
@@ -134,33 +134,60 @@
 
 		if not d:
 			print("[Functions.check_LocalizationFile] > NeuronIDValueError: The LocalizationFile file that you loaded has at least one event whose neuron ID value is either less than zero or greater than mso_num_neurons_channel.")
 
 		if a and b and c and d:
 			print("[Functions.check_LocalizationFile] > The loaded LocalizationFile file has been checked and it's OK")
 
-	@staticmethod 
-	def adapt_timestamps(timestamps, settings):
+	@staticmethod
+	def adapt_timestamps(spikes_file, settings):
 		"""
 		Subtracts the smallest timestamp of the timestamps list to all of the timestamps contained in the list (in order to start from 0)
 		It also adapts timestamps based on the tick frequency (ts_tick in the MainSettings).
-		
+
 		Parameters:
-				timestamps (int[]): Timestamps of the file to adapt.
+		  		spikes_file:
 				settings (MainSettings): Configuration parameters for the file to adapt.
 
 		Returns:
 				adapted_timestamps:  Adapted timestamps list.
 		"""
-		minimum_ts = min(timestamps)
-		if settings.reset_timestamp:
-			adapted_timestamps = [(x - minimum_ts)*settings.ts_tick for x in timestamps]
+		if spikes_file.timestamps != []:
+			# Convert to numpy array
+			timestamps = np.array(spikes_file.timestamps, copy=False)
+
+			if settings.reset_timestamp:
+				# Substract the minimum to all timestamps
+				minimum_ts = spikes_file.min_ts
+				adapted_timestamps = (timestamps - minimum_ts) * settings.ts_tick
+
+				# Update the maximum and minimum values
+				spikes_file.max_ts = spikes_file.max_ts - minimum_ts
+				spikes_file.min_ts = 0
+			else:
+				adapted_timestamps = timestamps * settings.ts_tick
+
+				# Update the maximum and minimum values
+				spikes_file.max_ts = adapted_timestamps[spikes_file.max_ts_index]
+				spikes_file.min_ts = adapted_timestamps[spikes_file.min_ts_index]
+
+			# Update the timestamps
+			spikes_file.timestamps = adapted_timestamps.astype(dtype=np.dtype(">u" + str(settings.timestamp_size)))
 		else:
-			adapted_timestamps = [x*settings.ts_tick for x in timestamps]
-		return adapted_timestamps
+			print("[Functions.adapt_timestamps] > The SpikesFile timestamps are empty")
+
+
+	@staticmethod
+	def order_SpikesFile(spikes_file, settings):
+		# Indices that would sort the file
+		indexes = np.argsort(spikes_file.timestamps)
+
+		# Sort the arrays
+		spikes_file.addresses = spikes_file.addresses[indexes]
+		spikes_file.timestamps = spikes_file.timestamps[indexes]
 
 
 	@staticmethod
 	def phase_lock(spikes_file, settings, posNeg_both = 0):
 		"""
 		Performs the phase lock operation over a SpikesFile. This can only be performed to SpikeFiles with both ON and OFF addresses. The phaselock operation puts a spike in the output only when the spike train from a specific channel changes from ON (positive part of the signal) to OFF (negative part of the signal). This heavily reduces the number of spikes at the output.
 		
@@ -222,23 +249,23 @@
 		if settings.mono_stereo:
 			addr_ts = list(zip(spikes_file.addresses, spikes_file.timestamps))
 			addr_ts = [x for x in addr_ts if x[0] >= left_right*settings.num_channels*(settings.on_off_both + 1) and x[0] < (left_right+1)*settings.num_channels*(settings.on_off_both + 1)]
 
 			spikes_file_mono = Utils.extract_addr_and_ts(addr_ts)
 			if left_right:
 				spikes_file_mono.addresses = [x-left_right*settings.num_channels*(settings.on_off_both + 1) for x in spikes_file_mono.addresses]
-			
-			
+
+
 			if return_save_both == 0:
 				return spikes_file_mono
 			elif return_save_both == 1 or return_save_both == 2:
-				Savers.save_as_any(spikes_file_mono, path=path, output_format=output_format, settings=settings) 
+				Savers.save_as_any(spikes_file_mono, path=path, output_format=output_format, settings=settings)
 				if return_save_both == 2:
 					return spikes_file_mono
-			
+
 		else:
 			print("[Functions.stereo_to_mono] > SettingsError: this functionality cannot be performed over a mono aedat file.")
 
 
 	@staticmethod
 	def mono_to_stereo(spikes_file, delay, settings, return_save_both = 0, path = None, output_format = '.aedat'):
 		"""
@@ -275,20 +302,20 @@
 				spikes_file_new.timestamps = [x-delay for x in spikes_file_new.timestamps]
 
 			if return_save_both == 0:
 				return spikes_file_new
 			elif return_save_both == 1 or return_save_both == 2:
 				#settings_new = copy.deepcopy(settings)
 				#settings_new.mono_stereo = 1
-				Savers.save_as_any(spikes_file_new, path=path, output_format=output_format, settings=settings) 
+				Savers.save_as_any(spikes_file_new, path=path, output_format=output_format, settings=settings)
 				if return_save_both == 2:
 					return spikes_file_new
 
 		else:
-			print("[Functions.mono_to_stereo] > SettingsError: this functionality cannot be performed over a stereo aedat file.")        
+			print("[Functions.mono_to_stereo] > SettingsError: this functionality cannot be performed over a stereo aedat file.")
 
 
 	@staticmethod
 	def extract_channels_activities(spikes_file, addresses, reset_addresses = True, verbose = False):
 		"""
 		Extract information from a specific set of addresses from the SpikesFile.
 		
@@ -316,151 +343,27 @@
 			new_spikes_file.addresses = [addr - addresses[0] for addr in new_spikes_file.addresses]
 		new_spikes_file.timestamps = spikes_per_channels_ts
 		new_spikes_file = Utils.order_timestamps(new_spikes_file)
 		return new_spikes_file
 
 
 	@staticmethod
-	def PDF_report(spikes_file, settings, output_path, plots = ["Spikegram", "Sonogram", "Histogram", "Average activity", "Difference between L/R"], add_localization_report = False, localization_file = None, localization_settings = None, localization_plots = ["MSO spikegram", "MSO heatmap", "MSO histogram", "MSO localization"], vector = False, verbose = False):
-		"""
-		Generates a PDF report with the spikegram, sonogram, histogram, average activity and difference between L/R plots obtained from the input SpikesFile or path containing SpikeFiles.
-		
-		Parameters:
-				spikes_file (SpikesFile or string): File or path to use.
-				settings (MainSettings): Configuration parameters for the input file.
-				output_path (string): Destination path.
-				plots (string[]): List to select the plots to be included in the PDF report.
-				add_localization_report (boolean, optional): If True, the localization plots will be included in the PDF report.
-				localization_file (LocalizationFile, optional): If add_localization_report is set to True, this parameter is mandatory, and it should contain the localization information.
-				localization_settings (LocalizationSettings, optional): If add_localization_report is set to True, this parameter is mandatory, and it should contain the localization settings.
-				localization_plots (string[], optional): If add_localization_report is set to True, this parameter is mandatory, and it should contain the list of localization plots.
-				vector (boolean, optional): Set to True if you want the Spikegram plot vectorized. Note: this may make your PDF heavy.
-				verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
-
-		Returns:
-				None.
-		
-		Notes:   
-				If the path used as input is a folder instead of a spikes file, the PDF report is generated for every spikes file contained in the folder.
-		"""
-
-		if isinstance(spikes_file, str):
-    			
-			spikes_file_extension = os.path.splitext(spikes_file)
-
-			if spikes_file_extension == ".aedat":
-				if add_localization_report == False:
-					spikes_file = Loaders.loadAEDAT(spikes_file, settings)
-				elif add_localization_report != False and localization_file != None and localization_settings != None:
-					spikes_file, localization_file = Loaders.loadAEDATLocalization(spikes_file, settings, localization_settings)
-				else:
-					print("[Functions.PDF_report] > ParametersError: the input parameters are not correct.")
-					return None
-			elif spikes_file_extension == ".csv":
-				if add_localization_report == False:
-					spikes_file = Loaders.loadCSV(spikes_file, delimiter=',')
-				elif add_localization_report != False and localization_file != None and localization_settings != None:
-					spikes_file, localization_file = Loaders.loadCSVLocalization(spikes_file, delimiter=',')
-				else:
-					print("[Functions.PDF_report] > ParametersError: the input parameters are not correct.")
-					return None
-			elif spikes_file_extension == ".txt":
-				spikes_file, localization_file = Loaders.loadZynqGrabberData(spikes_file, settings, localization_settings)
-			else:
-				print("[Functions.PDF_report] > InputFileExtensionError: the extension of the input file is not valid.")
-				return None
-			spikes_file.timestamps = Functions.adapt_timestamps(spikes_file.timestamps, settings)
-			if add_localization_report == True:
-				localization_file.timestamps = Functions.adapt_timestamps(localization_file.timestamps, settings)
-
-		if isinstance(spikes_file, SpikesFile):
-    		
-			pdf = matplotlib.backends.backend_pdf.PdfPages(output_path)
-			
-			# Spikegram
-			if any("Spikegram" in s for s in plots):
-				spikegram = Plots.spikegram(spikes_file, settings, )
-				pdf.savefig(spikegram)
-				plt.draw()
-			# Sonogram
-			if any("Sonogram" in s for s in plots):
-				sonogram = Plots.sonogram(spikes_file, settings)		
-				pdf.savefig(sonogram)
-				plt.draw()
-			# Histogram
-			if any("Histogram" in s for s in plots):
-				Plots.histogram(spikes_file, settings,)		
-				pdf.savefig()
-				plt.draw()
-			# Average activity
-			if any("Average activity" in s for s in plots):
-				Plots.average_activity(spikes_file, settings,)		
-				pdf.savefig()
-				plt.draw()
-			# Difference between L/R
-			if settings.mono_stereo == 1 and any("Difference between L/R" in s for s in plots):		
-				Plots.difference_between_LR(spikes_file, settings,)		
-				pdf.savefig()
-				plt.draw()
-
-			if add_localization_report == True:
-				if isinstance(localization_file, LocalizationFile):
-					# MSO spikegram
-					if any("MSO spikegram" in s for s in localization_plots):
-						mso_spikegram = Plots.mso_spikegram(localization_file, settings, localization_settings)
-						pdf.savefig(mso_spikegram)
-						plt.draw()
-					# MSO heatmap
-					if any("MSO heatmap" in s for s in localization_plots):
-						mso_heatmap = Plots.mso_heatmap(localization_file, localization_settings)		
-						pdf.savefig(mso_heatmap)
-						plt.draw()
-					# MSO histogram
-					if any("MSO histogram" in s for s in localization_plots):
-						mso_histogram = Plots.mso_histogram(localization_file, settings, localization_settings)		
-						pdf.savefig(mso_histogram)
-						plt.draw()
-					# MSO localization
-					if any("MSO localization" in s for s in localization_plots):
-						mso_localization = Plots.mso_localization_plot(localization_file, settings, localization_settings)		
-						pdf.savefig(mso_localization)
-						plt.draw()
-				else:
-					print("[Functions.PDF_report] > InputFileError: the input LocalizationFile is not valid.")
-
-			d = pdf.infodict()
-			d['Title'] = 'pyNAVIS report'
-			d['Author'] = 'Juan P. Dominguez-Morales'
-			d['Subject'] = 'pyNAVIS report'
-			d['Keywords'] = 'pyNAVIS'
-			d['CreationDate'] = datetime.datetime.today()
-			d['ModDate'] = datetime.datetime.today()
-
-			pdf.close()
-			plt.close()
-			print("[Functions.PDF_report] > PDF report generated correctly")
-
-		else:
-			print("[Functions.PDF_report] > InputFileError: the input SpikesFile is not valid.")
-
-
-	@staticmethod
 	def ISI(spikes_file, verbose = False):
 		"""
 		Generates an array with the inter-spike intervals of the input SpikesFile.
 		
 		Parameters:
 				spikes_file (SpikesFile or string): File or path to use.
 				settings (MainSettings): Configuration parameters for the input file.
 				verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
 
 		Returns:
 				int[]: inter-spike interval array.
 		"""
 
 		if verbose == True: start_time = time.time()
-		
+
 		isi_array = np.diff(spikes_file.timestamps)
 
 		if verbose == True: print('ISI CALCULATION', time.time() - start_time)
 
 		return isi_array
```

### Comparing `pyNAVIS-1.1.0/pyNAVIS/generators.py` & `pyNAVIS-1.1.1/pyNAVIS/generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 ##                                                                             ##
 ##    You should have received a copy of the GNU General Public License        ##
 ##    along with pyNAVIS.  If not, see <http://www.gnu.org/licenses/>.         ##
 ##                                                                             ##
 #################################################################################
 
 import random
-
 import numpy as np
 
-from .loaders import SpikesFile
-from .savers import Savers
 from .main_settings import MainSettings
+from .objects import SpikesFile
+from .savers import Savers
+
 
 class Generators:
     
     @staticmethod
     def sweep(freq, cycles, num_ch, length, path = None, output_format = '.aedat', return_save_both = 0):
         """
         Generates a SpikesFile with spikes going from address 0 to address N and back, repeating it for a specific number of cycles.
@@ -43,15 +43,14 @@
                 output_format (string, optional): Output format of the file. Currently supports '.aedat', '.csv', ".txt" and ".txt_rel". See the Savers class for more information.
                 return_save_both (int, optional): Set it to 0 to return the SpikesFile, to 1 to save the SpikesFile in the output path, and to 2 to do both.
 
         Returns:
                 SpikesFile: SpikesFile containing the sweep. Returned only if return_save_both is either 0 or 2.
         """
 
-        spikes_file = SpikesFile([], [])
         time_per_cycle = float(length) // cycles
         spikes_per_cycle = freq * (num_ch * 2 - 1)
         time_between_spikes = float(time_per_cycle) // spikes_per_cycle
 
         addrs = [0] * int(spikes_per_cycle*cycles)
         timestamps = [0] * int(spikes_per_cycle*cycles)
         current_spike_id = 0    
@@ -60,16 +59,15 @@
             for i in range((num_ch*2)-1):
                 for j in range(freq):
                     addrs[current_spike_id] = i - (i//num_ch)*(((i%(num_ch))+1)*2)
                     timestamps[current_spike_id] = int(current_spike_id*time_between_spikes)
                     current_spike_id += 1
         settings = MainSettings(num_channels = num_ch, mono_stereo = 0)
 
-        spikes_file.timestamps = timestamps
-        spikes_file.addresses = addrs
+        spikes_file = SpikesFile(addrs, timestamps)
 
         if return_save_both == 0:
             return spikes_file
         elif return_save_both == 1 or return_save_both == 2:
             Savers.save_as_any(spikes_file, path=path, output_format=output_format, settings=settings) 
             if return_save_both == 2:
                 return spikes_file
@@ -87,30 +85,28 @@
                 output_format (string, optional): Output format of the file. Currently supports '.aedat', '.csv', ".txt" and ".txt_rel". See the Savers class for more information.
                 return_save_both (int, optional): Set it to 0 to return the SpikesFile, to 1 to save the SpikesFile in the output path, and to 2 to do both.
 
         Returns:
                 SpikesFile: SpikesFile containing the shift. Returned only if return_save_both is either 0 or 2.
         """
 
-        spikes_file = SpikesFile([], [])
         total_spikes_no = freq * num_ch
         addrs = [0] * int(total_spikes_no)
         timestamps = [0] * int(total_spikes_no)
         current_spike_id = 0
         
         time_between_spikes = float(length) // total_spikes_no
 
         for i in range(num_ch):
             for j in range(freq):
                 addrs[current_spike_id] = i
                 timestamps[current_spike_id] = int(current_spike_id*time_between_spikes)
                 current_spike_id += 1
         settings = MainSettings(num_channels = num_ch, mono_stereo = 0)
-        spikes_file.timestamps = timestamps
-        spikes_file.addresses = addrs
+        spikes_file = SpikesFile(addrs, timestamps)
         if return_save_both == 0:
             return spikes_file
         elif return_save_both == 1 or return_save_both == 2:
             Savers.save_as_any(spikes_file, path=path, output_format=output_format, settings=settings) 
             if return_save_both == 2:
                 return spikes_file
 
@@ -127,24 +123,23 @@
                 output_format (string, optional): Output format of the file. Currently supports '.aedat', '.csv', ".txt" and ".txt_rel". See the Savers class for more information.
                 return_save_both (int, optional): Set it to 0 to return the SpikesFile, to 1 to save the SpikesFile in the output path, and to 2 to do both.
 
         Returns:
                 SpikesFile: SpikesFile containing the spikes. Returned only if return_save_both is either 0 or 2.
         """
 
-        spikes_file = SpikesFile([], [])
         addrs = [0] * int(freq*length/1000000)
         timestamps = [0] * int(freq*length/1000000)
         random.seed(0)
         for i in range(int(freq*length/1000000)):
             addrs[i] = random.randint(0, num_ch-1)
             timestamps[i] = int(i*1000000/freq) #Multiplying by 1000000 to convert timestamps to microseconds
         
         settings = MainSettings(num_channels = num_ch, mono_stereo = 0)
-        spikes_file.timestamps = timestamps
-        spikes_file.addresses = addrs
+
+        spikes_file = SpikesFile(addrs, timestamps)
         if return_save_both == 0:
             return spikes_file
         elif return_save_both == 1 or return_save_both == 2:
             Savers.save_as_any(spikes_file, path=path, output_format=output_format, settings=settings) 
             if return_save_both == 2:
                 return spikes_file
```

### Comparing `pyNAVIS-1.1.0/pyNAVIS/loaders.py` & `pyNAVIS-1.1.1/pyNAVIS/loaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,123 +19,98 @@
 ##                                                                             ##
 #################################################################################
 
 
 import math
 import struct
 import csv
+import numpy as np
+from .functions import Functions
+from .objects import SpikesFile
+from .objects import LocalizationFile
 
 
-class SpikesFile:
-    """
-    Class that contains all the addresses and timestamps of a file.
-
-    Attributes:
-            timestamps (int[]): Timestamps of the file.
-            addresses (int[]): Addresses of the file.
-    Note:
-            Timestamps and addresses are matched, which means that timestamps[0] is the timestamp for the spike with address addresses[0].
-    """
-
-    def __init__(self, addresses = [], timestamps = []):
-        self.addresses = addresses
-        self.timestamps = timestamps
-
-class LocalizationFile:
-    """
-    Class that contains all the events ant timestamps from the sound source localization model of a file.
-
-    Attributes:
-            mso_neurons_ids (int[]): Neuron's IDs of the MSO population of the file.
-            mso_channels (int[]): Frequency channels associated to the MSO neuron's IDs of the file.
-            mso_timestamps (int[]): Timestamps of the MSO neuron's IDs of the file.
-            lso_neuron_ids (int[]): Neuron's IDs of the LSO population of the file.
-            lso_channels (int[]): Frequency channels associated to the LSO neuron's IDs of the file.
-            lso_timestamps (int[]): Timestamps of the LSO neuron's IDs of the file.
-    
-    Note:
-            Timestamps, addresses, and neurons' ID are matched, which means that mso_timestamps[0] is the timestamp for the spike with address mso_neuron_ids[0].
-    """
-
-    def __init__(self, mso_neuron_ids = [], mso_channels = [], mso_timestamps = [], lso_neuron_ids = [], lso_channels = [], lso_timestamps = []):
-        self.mso_neuron_ids = mso_neuron_ids
-        self.mso_channels = mso_channels
-        self.mso_timestamps = mso_timestamps
-        self.lso_neuron_ids = lso_neuron_ids
-        self.lso_channels = lso_channels
-        self.lso_timestamps = lso_timestamps
-
 class Loaders:
     """
     Functionalities for loading spiking information from different formats.
     """
 
     @staticmethod
     def loadAEDAT(path, settings):
         """
         Loads an AEDAT (.aedat) file.
-        
+
         Parameters:
                 path (string): Full path of the AEDAT file to be loaded, including name and extension.
                 settings (MainSettings): Configuration parameters for the file to load.
 
         Returns:
                 SpikesFile: SpikesFile containing all the addresses and timestamps of the file.
-        Raises:
-                SettingsError: If settings.address_size is different than 2 and 4.
-
         """
-        unpack_param = ">H"
-        
-        if settings.address_size == 2:
-            unpack_param = ">H"
-        elif settings.address_size == 4:
-            unpack_param = ">L"
+        # Read all the file
+        file = open(path, "rb")
+        file_data = file.read()
+
+        # Find last header line
+        end_string = "#End Of ASCII Header\r\n"
+        index = file_data.find(end_string.encode("utf-8"))
+        if index != -1:
+            index += len(end_string)
         else:
-            print("[Loaders.loadAEDAT] > SettingsError: Only address sizes implemented are 2 and 4 bytes")
+            index = 0
 
-        with open(path, 'rb') as f:
-            ## Check header ##
-            p = 0
-            lt = f.readline()
-            while lt and lt[0] == ord("#"):
-                p += len(lt)
-                lt = f.readline()
-            f.seek(p)
-
-            f.seek(0, 2)
-            eof = f.tell()
-
-            num_events = math.floor((eof-p)/(settings.address_size + 4))
-
-            f.seek(p)
+        # Raw data extraction
+        num_spikes = int(math.floor(len(file_data[index:]) / (settings.address_size + settings.timestamp_size)))
+        spikes_array = file_data[index:index + num_spikes * (settings.address_size + settings.timestamp_size)]
+
+        if settings.address_size != 3 and settings.timestamp_size != 3:
+            address_param = ">u" + str(settings.address_size)
+            timestamp_param = ">u" + str(settings.timestamp_size)
+            bytes_struct = np.dtype(address_param + ", " + timestamp_param)
+
+            spikes = np.frombuffer(spikes_array, bytes_struct)
+            addresses = spikes['f0']
+            timestamps = spikes['f1']
 
-            events = [0] * int(num_events)
-            timestamps = [0] * int(num_events)
-
-            ## Read file ##
-            i = 0
-            try:
-                while 1:
-                    buff = f.read(settings.address_size)
-                    x = struct.unpack(unpack_param, buff)[0]
-                    events[i] = x
-
-                    buff = f.read(4)
-                    x = struct.unpack('>L', buff)[0]
-                    timestamps[i] = x
+        else:
+            # Separate addresses and timestamps
+            spikes_struct = np.dtype([("addresses", ">u1", settings.address_size),
+                                      ("timestamps", ">u1", settings.timestamp_size)])
+            spikes = np.frombuffer(spikes_array, spikes_struct)
+
+            # Fill addresses and timestamps with zeros to reach 4-bytes per element
+            address_struct = np.dtype([("zeros", ">u1", (4 - settings.address_size,)),
+                                       ("addresses", ">u1", (settings.address_size,))])
+            timestamp_struct = np.dtype([("zeros", ">u1", (4 - settings.timestamp_size,)),
+                                         ("timestamps", ">u1", (settings.timestamp_size,))])
+            filled_addresses = np.zeros(len(spikes), dtype=address_struct)
+            filled_timestamps = np.zeros(len(spikes), dtype=timestamp_struct)
+            filled_addresses['addresses'] = spikes['addresses']
+            filled_timestamps['timestamps'] = spikes['timestamps']
+
+            # View these filled addresses and timestamps as 4-byte ints
+            addresses = filled_addresses.view(">u4")
+            timestamps = filled_timestamps.view(">u4")
+
+        spikes_file = SpikesFile(addresses, timestamps)
+
+        # Close the file
+        file.close()
+
+        # Check correct address values and increasing timestamp order in the loaded aedat file
+        _, order_is_ok, all_in_range = Functions.check_SpikesFile(spikes_file, settings)
+        if not all_in_range:
+            raise ValueError("Addresses are not in range. Could be due to bad decoding")
+        if not order_is_ok:
+            Functions.order_SpikesFile(spikes_file, settings)
 
-                    i += 1
-            except Exception as inst:
-                pass
-        spikes_file = SpikesFile([], [])
-        spikes_file.addresses = events
-        spikes_file.timestamps = timestamps
         return spikes_file
 
+    # TODO: Check the rest of loading functions
+
     @staticmethod
     def loadAEDATLocalization(path, settings, localization_settings):
         """
         Loads an AEDAT (.aedat) file which contains events from both the NAS model and the SOC model (sound source localization).
         
         Parameters:
                 path (string): Full path of the AEDAT file to be loaded, including name and extension.
@@ -145,55 +120,55 @@
                 SpikesFile: SpikesFile containing all the addresses and timestamps of the file.
                 LocalizationFile: LocalizationFile containing all the events from both the MSO and LSO models of the file.
         Raises:
                 SettingsError: If settings.address_size is different than 2 and 4.
 
         """
         unpack_param = ">H"
-        
+
         if settings.address_size == 2:
             unpack_param = ">H"
         elif settings.address_size == 4:
             unpack_param = ">L"
         else:
             print("[Loaders.loadAEDATLocalization] > SettingsError: Only address sizes implemented are 2 and 4 bytes")
-        
+
         # Check the localization_settings values
         localization_settings_error = False
 
         # MSO start frequency channel range
         if ((localization_settings.mso_start_channel < 0) or (localization_settings.mso_start_channel >= settings.num_channels)):
             print("[Loaders.loadAEDATLocalization] > LocalizationSettingsError: MSO start frequency channel range should be in the range [0, num_channels-1]")
             localization_settings_error = True
-        
+
         # MSO start frequency channel and end frequency channel
         if (localization_settings.mso_end_channel < localization_settings.mso_start_channel):
             print("[Loaders.loadAEDATLocalization] > LocalizationSettingsError: MSO start frequency channel should be lower than MSO end frequency channel")
             localization_settings_error = True
-        
+
         # MSO start frequency channel and end frequency channel
         if ((localization_settings.mso_num_neurons_channel < 1) or (localization_settings.mso_num_neurons_channel > 32)):
             print("[Loaders.loadAEDATLocalization] > LocalizationSettingsError: MSO number of neurons value should be in the range [1, 32]")
             localization_settings_error = True
 
         # LSO start frequency channel range
         if ((localization_settings.lso_start_channel < 0) or (localization_settings.lso_start_channel >= settings.num_channels)):
             print("[Loaders.loadAEDATLocalization] > LocalizationSettingsError: LSO start frequency channel range should be in the range [0, num_channels-1]")
             localization_settings_error = True
-        
+
         # LSO start frequency channel and end frequency channel
         if (localization_settings.lso_end_channel < localization_settings.lso_start_channel):
             print("[Loaders.loadAEDATLocalization] > LocalizationSettingsError: LSO start frequency channel should be lower than LSO end frequency channel")
             localization_settings_error = True
-        
+
         # LSO start frequency channel and end frequency channel
         if ((localization_settings.lso_num_neurons_channel < 1) or (localization_settings.lso_num_neurons_channel > 32)):
             print("[Loaders.loadAEDATLocalization] > LocalizationSettingsError: lSO number of neurons value should be in the range [1, 32]")
             localization_settings_error = True
-        
+
         if(localization_settings_error):
             return None
 
         with open(path, 'rb') as f:
             ## Check header ##
             p = 0
             lt = f.readline()
@@ -229,15 +204,15 @@
                     # Read a word and unpack the event data
                     buff = f.read(settings.address_size)
                     ev = struct.unpack(unpack_param, buff)[0]
                     total_number_events_counter = total_number_events_counter + 1
                     # Read a word and unpack the event timestamp
                     buff = f.read(4)
                     ts = struct.unpack('>L', buff)[0]
-                    
+
                     # Check if the event is a NAS event of SOC event
                     auditory_model = (ev & 0x8000) >> 15
 
                     if auditory_model == 0:
                         # NAS event
                         events_nas.append(ev)
                         timestamps_nas.append(ts)
@@ -310,15 +285,15 @@
 
         Note:
                 The CSV file should contain one line per event, and the information in each line should be: address, timestamp
 
         """
         addresses = []
         timestamps = []
-        
+
 
         with open(path) as csv_file:
             csv_reader = csv.reader(csv_file, delimiter=delimiter)
             for row in csv_reader:
                 addresses.append(int(row[0]))
                 timestamps.append(int(row[1]))
 
@@ -352,15 +327,15 @@
         neuron_ids_mso = []
         channels_mso =  []
         timestamps_mso = []
 
         neuron_ids_lso = []
         channels_lso =  []
         timestamps_lso = []
-        
+
 
         with open(path) as csv_file:
             csv_reader = csv.reader(csv_file, delimiter=delimiter)
             for row in csv_reader:
 
                 try:
                     auditory_model = int(row[2])
@@ -405,23 +380,23 @@
                 else:
                     # Other case
                     print("[Loaders.loadCSVLocalization] > DataError: Auditory model not recognized!")
 
         spikes_file = SpikesFile([], [])
         spikes_file.addresses = addresses_nas
         spikes_file.timestamps = timestamps_nas
-        
+
         localization_file = LocalizationFile([], [], [], [], [], [])
         localization_file.mso_neuron_ids = neuron_ids_mso
         localization_file.mso_channels = channels_mso
         localization_file.mso_timestamps = timestamps_mso
         localization_file.lso_neuron_ids = neuron_ids_lso
         localization_file.lso_channels = channels_lso
         localization_file.lso_timestamps = timestamps_lso
-        
+
         return spikes_file, localization_file
 
     @staticmethod
     def loadZynqGrabberData(path, settings, localization_settings):
         """
         Loads a text (.txt) file with EAR events collected by the zynqGrabber.
         
@@ -430,54 +405,54 @@
                 settings (MainSettings): Configuration parameters for the file to load.
                 localization_settings (LocalizationSettings): Configuration parameters of the localization module for the file to load.
 
         Returns:
                 spikes_file: SpikesFile containing all the addresses and timestamps of the file.
                 localization_file: LocalizationFile containing all the events from both the MSO and LSO models of the file.
         """
-        
+
         addresses = []
         timestamps = []
 
         neuron_ids_mso = []
         channels_mso =  []
         timestamps_mso = []
 
         neuron_ids_lso = []
         channels_lso =  []
         timestamps_lso = []
-        
-        txt_file = open(path, 'r') 
-        txt_lines = txt_file.readlines() 
-        
+
+        txt_file = open(path, 'r')
+        txt_lines = txt_file.readlines()
+
         count = 0
         for line in txt_lines:
             event = line.strip().split(',')
             decoded_events_timestamps      = float(event[0])
             decoded_events_auditory_models = int(event[1])           # 0 if the event comes from the NAS, 1 for the SOC model
             decoded_events_channels        = int(event[2])           # 0 left, 1 right
             decoded_events_xso_types       = int(event[3])           # 0 for MSO, 1 for LSO
             decoded_events_neuron_ids      = int(event[4])           # Between 0 and 15
             decoded_events_freq_ch_addrs   = int(event[5])           # Between 0 and 32
             decoded_events_polarities      = int(event[6])           # 0 pos, 1 neg
 
             # It could be either NAS (auditory_models = 0) or SOC events (auditory_models = 1)
-            if decoded_events_auditory_models == 0: 
+            if decoded_events_auditory_models == 0:
                 # NAS event
                 timestamps.append(int(decoded_events_timestamps))
                 addresses.append(int(decoded_events_freq_ch_addrs*(1+settings.on_off_both) + decoded_events_polarities +  settings.num_channels*decoded_events_channels*(1+settings.on_off_both)))
 
             elif decoded_events_auditory_models == 1:
                 # It could be either MSO (xso_type = 0) or LSO events (xso_type = 1)
                 if decoded_events_xso_types == 0:
                     # MSO event
                     timestamps_mso.append(int(decoded_events_timestamps))
                     channels_mso.append(int(decoded_events_freq_ch_addrs))
                     neuron_ids_mso.append(int(decoded_events_neuron_ids))
-                    
+
                 elif decoded_events_xso_types == 1:
                     # LSO event
                     timestamps_lso.append(int(decoded_events_timestamps))
                     channels_lso.append(int(decoded_events_freq_ch_addrs))
                     neuron_ids_lso.append(int(decoded_events_neuron_ids))
                 else:
                     # Other case
```

### Comparing `pyNAVIS-1.1.0/pyNAVIS/main_settings.py` & `pyNAVIS-1.1.1/pyNAVIS/main_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,32 +25,34 @@
 
     Attributes:
         mono_stereo (int): Set to 0 for mono files and 1 for stereo files.
         bin_size (int): Bin width (or window size) to use when processing the information.
         ts_tick (float): Timestamp tick. Correspondence factor between timestamp value in file and actual time.
         num_channels (int): Number of cochlea channels.
         address_size (int): Number of bytes that each address is using. Only needed when loading .aedat files
+        timestamp_size (int): Number of bytes that each timestamp is using. Only needed when loading .aedat files
         on_off_both (int): Select wether the addresses contained in the file are ON, OFF or if it is using both.
         reset_timestamp (boolean): Select wether to have timedtamps starting at 0 (True) or leave it as they are (False).
     
     Notes:
             Set ts_tick to 1 for .aedat files recorded with jAER, to 0.2 for files recorded with USBAERmini2, and to 80e-3 for files recorded with zynqGrabber.
 
             Set address_size to 2 for .eadat files recorded with USBAERmini2, or to 4 for files recorded with jAER.
             This parameter is only relevant for loading AEDAT (.aedat) files.
 
             Set on_off_both to 0 if addresses are only ON or OFF, or to 1 if using both ON and OFF.
 
             reset_timestamp subtracts the smallest timestamp in the file to each of the timestamps.
     """
 
-    def __init__(self, num_channels, mono_stereo = 0, address_size = 2, ts_tick = 1, bin_size = 20000, on_off_both = 1, reset_timestamp = True):
+    def __init__(self, num_channels, mono_stereo = 0, address_size = 2, timestamp_size=4, ts_tick = 1, bin_size = 20000, on_off_both = 1, reset_timestamp = True):
         self.num_channels = num_channels
         self.mono_stereo = mono_stereo
         self.address_size = address_size
+        self.timestamp_size = timestamp_size
         self.ts_tick = ts_tick
         self.bin_size = bin_size
         self.on_off_both = on_off_both
         self.reset_timestamp = reset_timestamp
 
 class LocalizationSettings:
     """
```

### Comparing `pyNAVIS-1.1.0/pyNAVIS/plots.py` & `pyNAVIS-1.1.1/pyNAVIS/plots.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,399 +17,437 @@
 ##    You should have received a copy of the GNU General Public License        ##
 ##    along with pyNAVIS.  If not, see <http://www.gnu.org/licenses/>.         ##
 ##                                                                             ##
 #################################################################################
 
 import math
 import random
+import time
 from bisect import bisect_left, bisect_right
-from matplotlib.colors import LinearSegmentedColormap
 
-import matplotlib
 import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
 import numpy as np
-import time
+from matplotlib.colors import LinearSegmentedColormap
+from pyNAVIS import Functions
 
-from .utils import Utils
 
 class Plots:
     @staticmethod
-    def spikegram(spikes_file, settings, dot_size = 0.2, dot_freq = 1, graph_title = 'Spikegram', start_at_zero = True, verbose = False):
+    def spikegram(spikes_file, settings, dot_size=0.2, dot_freq=1, graph_title='Spikegram', start_at_zero=True,
+                  verbose=False):
         """
         Plots the spikegram (also known as cochleogram or raster plot) of a SpikesFile.
-        
+
         This is, a graph where the X axis means time and the Y axis represents addresses (or cochlea channels), and where every spike is plotted as a dot.
 
         Parameters:
                 spikes_file (SpikesFile): File to plot.
                 settings (MainSettings): Configuration parameters for the file to plot.
                 dot_size (float): Size of the dots used in the spikegram plot.
                 dot_freq (int): Set the frequency of spikes that will be represented in the spikegram.
                 graph_title (string, optional): Text that will appear as title for the graph.
                 start_at_zero (boolean, optional): If set to True, the X axis will start at 0, instead of starting at the minimum timestamp.
                 verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
 
         Returns:
                 None.
 
-        Note: 
+        Note:
                 A value of 10 in dot_freq means that for every 10 spikes, only 1 will be plotted. This helps reducing lag when plotting heavy files.
         """
-
-        if verbose == True: start_time = time.time()
-        #REPRESENTATION
+        if verbose:
+            start_time = time.time()
+        # REPRESENTATION
         plt.style.use('seaborn-whitegrid')
         spk_fig = plt.figure()
         spk_fig.canvas.set_window_title(graph_title)
 
         random.seed(0)
 
+        mid_address = settings.num_channels * (settings.on_off_both + 1)
+
+        if start_at_zero and spikes_file.min_ts != 0:
+            Functions.adapt_timestamps(spikes_file, settings)
+
         if settings.mono_stereo == 0:
-            plt.scatter(spikes_file.timestamps[0::dot_freq], spikes_file.addresses[0::dot_freq], s=dot_size)
+            plt.scatter(spikes_file.timestamps[0::dot_freq], spikes_file.addresses[0::dot_freq],
+                        s=dot_size, rasterized=True)
         else:
-            aedat_addr_ts = list(zip(spikes_file.addresses, spikes_file.timestamps))
-            addr, ts = zip(*[(evt[0], evt[1]) for evt in aedat_addr_ts if evt[0] < settings.num_channels*(settings.on_off_both + 1)])
-            plt.scatter(ts[0::dot_freq], addr[0::dot_freq], s=dot_size, label='Left cochlea')
-            addr, ts = zip(*[(evt[0], evt[1]) for evt in aedat_addr_ts if evt[0] >= settings.num_channels*(settings.on_off_both + 1) and evt[0] < settings.num_channels*(settings.on_off_both + 1)*2])
-            plt.scatter(ts[0::dot_freq], addr[0::dot_freq], s=dot_size, label='Right cochlea')
-            plt.legend(fancybox=False, ncol=2, loc='upper center', markerscale=2/dot_size, frameon=True)
-            
-        if verbose == True: print('SPIKEGRAM CALCULATION', time.time() - start_time)
+            # Convert to numpy arrays
+            addresses = np.array(spikes_file.addresses, copy=False)
+            timestamps = np.array(spikes_file.timestamps, copy=False)
+
+            sup_indexes = np.argwhere(addresses >= mid_address)
+
+            sup_addresses = addresses[sup_indexes]
+            sup_addresses = sup_addresses[::dot_freq]
+            sup_timestamps = timestamps[sup_indexes]
+            sup_timestamps = sup_timestamps[::dot_freq]
+
+            inf_addresses = np.delete(addresses, sup_indexes)
+            inf_addresses = inf_addresses[::dot_freq]
+            inf_timestamps = np.delete(timestamps, sup_indexes)
+            inf_timestamps = inf_timestamps[::dot_freq]
+
+            plt.scatter(inf_timestamps, inf_addresses, s=dot_size, label="Left cochlea", rasterized=True)
+            plt.scatter(sup_timestamps, sup_addresses, s=dot_size, label="Right cochlea", rasterized=True)
+            plt.legend(fancybox=False, ncol=2, loc='upper center', markerscale=2 / dot_size, frameon=True)
+
+        if verbose:
+            print('SPIKEGRAM CALCULATION', time.time() - start_time)
 
         plt.title(graph_title, fontsize='x-large')
         plt.xlabel('Timestamp ($\mu$s)', fontsize='large')
+        plt.xlim([spikes_file.min_ts, spikes_file.max_ts])
         plt.ylabel('Address', fontsize='large')
-        plt.ylim([0, settings.num_channels*(settings.on_off_both + 1)*(settings.mono_stereo + 1)])
-
-        if start_at_zero:
-            plt.xlim([0, np.max(spikes_file.timestamps)])
+        plt.ylim([0, mid_address * (settings.mono_stereo + 1)])
 
         plt.tight_layout()
-        spk_fig.show()
+
+        return spk_fig
 
     @staticmethod
-    def sonogram(spikes_file, settings, return_data = False, graph_title = 'Sonogram', start_at_zero = True, verbose = False):
+    def sonogram(spikes_file, settings, return_data=False, graph_title='Sonogram', start_at_zero=True, verbose=False):
         """
         Plots the sonogram of a SpikesFile.
-        
+
         This is, a graph where the X axis means time and the Y axis represents addresses (or cochlea channels), and where the spiking activity is shown with color.
 
         Parameters:
                 spikes_file (SpikesFile): File to plot.
                 settings (MainSettings): Configuration parameters for the file to plot.
                 return_data (boolean, optional): When set to True, the sonogram matrix will be returned instead of plotted.
                 graph_title (string, optional): Text that will appear as title for the graph.
                 start_at_zero (boolean, optional): If set to True, the X axis will start at 0, instead of starting at the minimum timestamp.
                 verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
 
         Returns:
                 int[ , ]: Sonogram matrix. Only returned if return_data is set to True.
         """
-        if verbose == True: start_time = time.time()
-
-        if start_at_zero:
-            total_time = max(spikes_file.timestamps)
-            last_time = 0
-        else:
-            total_time = max(spikes_file.timestamps) - min(spikes_file.timestamps)
-            last_time = min(spikes_file.timestamps)
-        
-
-        sonogram = np.zeros((settings.num_channels*(settings.on_off_both + 1)*(settings.mono_stereo+1), int(math.ceil(total_time/settings.bin_size))))
-
-        its = int(math.ceil(total_time/settings.bin_size))
-        
-        #THIS IS NOT NEEDED IF TS ARE SORTED
-        aedat_addr_ts = zip(spikes_file.addresses, spikes_file.timestamps)
-        aedat_addr_ts = sorted(aedat_addr_ts, key=Utils.getKey)
-        spikes_file = Utils.extract_addr_and_ts(aedat_addr_ts)
-        
-        for i in range(its):
+        if verbose:
+            start_time = time.time()
 
-            a =  bisect_left(spikes_file.timestamps, last_time)
-            b =  bisect_right(spikes_file.timestamps, last_time + settings.bin_size)
+        # In range timestamps
+        if start_at_zero and spikes_file.min_ts != 0:
+            Functions.adapt_timestamps(spikes_file, settings)
+
+        total_time = spikes_file.max_ts - spikes_file.min_ts
+        last_time = spikes_file.min_ts
+
+        # Calculate number of addresses and number of windows
+        num_addresses = settings.num_channels * (settings.on_off_both + 1) * (settings.mono_stereo + 1)
+        num_windows = int(math.ceil(total_time / settings.bin_size))
+
+        # Define sonogram array
+        sonogram = np.zeros((num_addresses, num_windows))
+
+        # Bincount
+        for i in range(num_windows):
+            a = bisect_left(spikes_file.timestamps, last_time)
+            b = bisect_right(spikes_file.timestamps, last_time + settings.bin_size)
 
             blockAddr = spikes_file.addresses[a:b]
 
-            spikes = np.bincount(blockAddr, minlength=settings.num_channels*(settings.on_off_both + 1)*(settings.mono_stereo+1))        
+            spikes = np.bincount(blockAddr, minlength=num_addresses)
 
             last_time += settings.bin_size
             sonogram[:, i] = spikes
 
-        if verbose == True: print('SONOGRAM CALCULATION', time.time() - start_time)
-        
-        if return_data == False:
+        if verbose:
+            print('SONOGRAM CALCULATION', time.time() - start_time)
+
+        if not return_data:
             # REPRESENTATION
             plt.style.use('default')
             sng_fig = plt.figure()
-            sng_fig.canvas.set_window_title(graph_title)
+            sng_fig.canvas.manager.set_window_title(graph_title)
 
-            plt.imshow(sonogram, aspect="auto", cmap='hot') #, aspect="auto")
+            plt.imshow(sonogram, aspect="auto", cmap='hot', rasterized=True)  # , aspect="auto")
             plt.gca().invert_yaxis()
 
-            plt.xlabel('Bin ('+str(settings.bin_size) + '$\mu$s width)', fontsize='large')
+            plt.xlabel('Bin (' + str(settings.bin_size) + '$\mu$s width)', fontsize='large')
             plt.ylabel('Address', fontsize='large')
 
             plt.title(graph_title, fontsize='x-large')
 
             """
             plt.annotate('Right cochlea | Left cochlea',
             xy=(1.00, 0.5), xytext=(5, 0),
             xycoords=('axes fraction', 'figure fraction'),
             textcoords='offset points',
             size=11, ha='center', va='center', rotation=270)
             """
 
             if settings.mono_stereo == 1:
                 plt.annotate('Right cochlea',
-                xy=(1.00, 0.75), xytext=(5, 0),
-                xycoords=('axes fraction', 'axes fraction'),
-                textcoords='offset points',
-                size=11, ha='center', va='center', rotation=270)
+                             xy=(1.00, 0.75), xytext=(5, 0),
+                             xycoords=('axes fraction', 'axes fraction'),
+                             textcoords='offset points',
+                             size=11, ha='center', va='center', rotation=270)
 
                 plt.annotate('Left cochlea',
-                xy=(1.00, 0.25), xytext=(5, 0),
-                xycoords=('axes fraction', 'axes fraction'),
-                textcoords='offset points',
-                size=11, ha='center', va='center', rotation=270)
+                             xy=(1.00, 0.25), xytext=(5, 0),
+                             xycoords=('axes fraction', 'axes fraction'),
+                             textcoords='offset points',
+                             size=11, ha='center', va='center', rotation=270)
 
             colorbar = plt.colorbar()
-            colorbar.set_label('No. of spikes', rotation=270, fontsize='large', labelpad= 10)
+            colorbar.set_label('No. of spikes', rotation=270, fontsize='large', labelpad=10)
 
-            sng_fig.show()
+            return sng_fig
         else:
             return sonogram
 
     @staticmethod
-    def histogram(spikes_file, settings, bar_line = 1, graph_title = 'Histogram', verbose = False):
+    def histogram(spikes_file, settings, bar_line=1, graph_title='Histogram', verbose=False):
         """
         Plots the histogram of a SpikesFile.
-        
+
         This is, a graph where addresses (or cochlea channels) are represented in the X axis, and number of spikes in the Y axis.
 
         Parameters:
                 spikes_file (SpikesFile): File to plot.
                 settings (MainSettings): Configuration parameters for the file to plot.
                 bar_line (int, optional): Select wether to plot the histogram as bar plot (0) or as a line graph (1).
                 graph_title (string, optional): Text that will appear as title for the graph.
                 verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
 
         Returns:
                 int[]: Histogram array.
         """
 
         start_time = time.time()
-        
-        spikes_count = np.bincount(spikes_file.addresses, minlength=settings.num_channels * (settings.on_off_both + 1) * (settings.mono_stereo + 1))
 
-        if verbose == True: print('HISTOGRAM CALCULATION:', time.time() - start_time)
+        spikes_count = np.bincount(spikes_file.addresses,
+                                   minlength=settings.num_channels * (settings.on_off_both + 1) * (settings.mono_stereo + 1))
+
+        if verbose:
+            print('HISTOGRAM CALCULATION:', time.time() - start_time)
 
         plt.style.use('seaborn-whitegrid')
         hst_fig = plt.figure()
-        hst_fig.canvas.set_window_title(graph_title)
+        hst_fig.canvas.manager.set_window_title(graph_title)
         plt.title(graph_title, fontsize='x-large')
         plt.xlabel('Address', fontsize='large')
         plt.ylabel('No. of spikes', fontsize='large')
 
         if bar_line == 0:
             if settings.mono_stereo == 1:
-                plt.bar(np.arange(settings.num_channels * (settings.on_off_both + 1)), spikes_count[0:settings.num_channels*(settings.on_off_both + 1)])
-                plt.bar(np.arange(settings.num_channels * (settings.on_off_both + 1)), spikes_count[settings.num_channels*(settings.on_off_both + 1):settings.num_channels*2*(settings.on_off_both + 1)])
+                plt.bar(np.arange(settings.num_channels * (settings.on_off_both + 1)),
+                        spikes_count[0:settings.num_channels * (settings.on_off_both + 1)],
+                        rasterized=True)
+                plt.bar(np.arange(settings.num_channels * (settings.on_off_both + 1)),
+                        spikes_count[settings.num_channels * (settings.on_off_both + 1):settings.num_channels * 2 * (settings.on_off_both + 1)],
+                        rasterized=True)
             else:
-                plt.bar(np.arange(settings.num_channels * (settings.on_off_both + 1) * (settings.mono_stereo + 1)), spikes_count)
+                plt.bar(np.arange(settings.num_channels * (settings.on_off_both + 1) * (settings.mono_stereo + 1)),
+                        spikes_count, rasterized=True)
         else:
             if settings.mono_stereo == 1:
-                plt.plot(np.arange(settings.num_channels * (settings.on_off_both + 1)), spikes_count[0:settings.num_channels*(settings.on_off_both + 1)], label='Left cochlea')
-                plt.plot(np.arange(settings.num_channels * (settings.on_off_both + 1)), spikes_count[settings.num_channels*(settings.on_off_both + 1):settings.num_channels*2*(settings.on_off_both + 1)], label='Right cochlea')
+                plt.plot(np.arange(settings.num_channels * (settings.on_off_both + 1)),
+                         spikes_count[0:settings.num_channels * (settings.on_off_both + 1)],
+                         label='Left cochlea', rasterized=True)
+                plt.plot(np.arange(settings.num_channels * (settings.on_off_both + 1)),
+                         spikes_count[settings.num_channels * (settings.on_off_both + 1):settings.num_channels * 2 * (settings.on_off_both + 1)],
+                         label='Right cochlea', rasterized=True)
                 plt.legend(loc='best', frameon=True)
             else:
-                plt.plot(np.arange(settings.num_channels * (settings.on_off_both + 1) * (settings.mono_stereo + 1)), spikes_count)
+                plt.plot(np.arange(settings.num_channels * (settings.on_off_both + 1) * (settings.mono_stereo + 1)),
+                         spikes_count, rasterized=True)
 
         plt.tight_layout()
-        hst_fig.show()
-        return spikes_count
+
+        return spikes_count, hst_fig
 
     @staticmethod
-    def average_activity(spikes_file, settings, graph_title = 'Average activity', verbose=False):
+    def average_activity(spikes_file, settings, graph_title='Average activity', verbose=False):
         """
         Plots the average activity plot of a SpikesFile.
-        
+
         This is, a graph where time is represented in the X axis, and average number of spikes in the Y axis.
 
         Parameters:
                 spikes_file (SpikesFile): File to plot.
                 settings (MainSettings): Configuration parameters for the file to plot.
                 graph_title (string, optional): Text that will appear as title for the graph.
                 verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
 
         Returns:
                 int[ ] average_activity_L: Average activity array.
                 int[ ] average_activity_R: Average activity array. Only returned if the mono_stereo parameter in settings is set to 1
         """
-        aedat_addr_ts = zip(spikes_file.addresses, spikes_file.timestamps)
-        total_time = int(max(spikes_file.timestamps))
-        last_ts = 0
-        average_activity_L = np.zeros(int(math.ceil(total_time/settings.bin_size))+1)
-        if(settings.mono_stereo == 1):
-            average_activity_R = np.zeros(int(math.ceil(total_time/settings.bin_size))+1)
-
-        #THIS TWO ONLY IF CHECK DETECTS AEDAT NOT IN ORDER
-        aedat_addr_ts = sorted(aedat_addr_ts, key=Utils.getKey)
-        spikes_file = Utils.extract_addr_and_ts(aedat_addr_ts)
+        # Convert to numpy array
+        addresses = np.array(spikes_file.addresses, copy=False)
+        timestamps = np.array(spikes_file.timestamps, copy=False)
+
+        # Define plot variables
+        total_time = spikes_file.max_ts - spikes_file.min_ts
+        mid_address = settings.num_channels * (settings.on_off_both + 1)
+        num_bins = int(math.ceil(total_time / settings.bin_size))
+
+        average_activity_L = np.zeros(num_bins)
+        if settings.mono_stereo == 1:
+            average_activity_R = np.zeros(num_bins)
+
+        if verbose:
+            start_time = time.time()
+
+        # Array of bins
+        bins = np.arange(num_bins) * settings.bin_size
+
+        # Calculate the bin associated with each timestamp
+        bins_indexes = np.digitize(timestamps, bins)
+
+        # Cutting indexes (timestamps must be sorted)
+        cut_indexes = np.where(np.diff(bins_indexes) > 0)[0]
+
+        # Split timestamps by cutting indexes
+        spikes_per_bins = np.array_split(addresses, cut_indexes)
+
+        # Calculate the number of spikes in the bins
+        for i in range(len(spikes_per_bins)):
+            count_below = np.count_nonzero(spikes_per_bins[i] < mid_address)
+            average_activity_L[i] = count_below
+            if settings.mono_stereo == 1:
+                average_activity_R[i] = len(spikes_per_bins[i]) - count_below
 
-        if verbose == True: start_time = time.time()
-        if settings.mono_stereo == 1: 
-            for i in range(0, total_time, settings.bin_size):        
-                evtL = 0
-                evtR = 0
-
-                a =  bisect_left(spikes_file.timestamps, last_ts)
-                b =  bisect_right(spikes_file.timestamps, last_ts + settings.bin_size)
-
-                events_list = spikes_file.addresses[a:b]
-                
-                for j in events_list:
-                    if j < settings.num_channels*(1 + settings.on_off_both):
-                        evtL = evtL + 1
-                    elif j >= settings.num_channels*(1 + settings.on_off_both) and j < settings.num_channels*(1 + settings.on_off_both)*2:
-                        evtR = evtR + 1
-
-                average_activity_L[int(i/settings.bin_size)] = evtL
-                average_activity_R[int(i/settings.bin_size)] = evtR
-                last_ts = last_ts + settings.bin_size
-        elif settings.mono_stereo == 0:
-            for i in range(0, total_time, settings.bin_size):
-                evtL = 0
-
-                a =  bisect_left(spikes_file.timestamps, last_ts)
-                b =  bisect_right(spikes_file.timestamps, last_ts + settings.bin_size)
-                events_list = spikes_file.addresses[a:b]
-                
-                for j in events_list:
-                    evtL = evtL + 1
-
-                average_activity_L[i//settings.bin_size] = evtL
-                last_ts = last_ts + settings.bin_size
-        if verbose == True: print('AVERAGE ACTIVITY CALCULATION', time.time() - start_time)
+        if verbose:
+            print('AVERAGE ACTIVITY CALCULATION', time.time() - start_time)
 
         plt.style.use('seaborn-whitegrid')
         avg_fig = plt.figure()
-        avg_fig.canvas.set_window_title(graph_title)
+        avg_fig.canvas.manager.set_window_title(graph_title)
         plt.title(graph_title, fontsize='x-large')
-        plt.xlabel('Bin ('+str(settings.bin_size) + '$\mu$s width)', fontsize='large')
+        plt.xlabel('Bin (' + str(settings.bin_size) + '$\mu$s width)', fontsize='large')
         plt.ylabel('No. of spikes', fontsize='large')
 
-        plt.plot(np.arange(math.ceil(total_time/settings.bin_size)+1), average_activity_L, label='Left cochlea')
-        if(settings.mono_stereo == 1):
-            plt.plot(np.arange(math.ceil(total_time/settings.bin_size)+1), average_activity_R, label='Right cochlea')
-            plt.legend(loc='best',  ncol=2, frameon=True)
+        plt.plot(bins / settings.bin_size, average_activity_L, label='Left cochlea', rasterized=True)
+        if settings.mono_stereo == 1:
+            plt.plot(bins / settings.bin_size, average_activity_R, label='Right cochlea')
+            plt.legend(loc='best', ncol=2, frameon=True)
 
         plt.tight_layout()
-        avg_fig.show()
         if settings.mono_stereo == 0:
-            return average_activity_L
+            return average_activity_L, avg_fig
         else:
-            return average_activity_L, average_activity_R
+            return average_activity_L, average_activity_R, avg_fig
 
     @staticmethod
-    def difference_between_LR(spikes_file, settings, return_data = False, graph_title = 'Diff. between L and R cochlea', verbose = False):
+    def difference_between_LR(spikes_file, settings, return_data=False, graph_title='Diff. between L and R cochlea',
+                              verbose=False, start_at_zero=True):
         """
         Plots a plot showing the differente between the left and the right activity of a SpikesFile.
 
         Parameters:
                 spikes_file (SpikesFile): File to plot.
                 settings (MainSettings): Configuration parameters for the file to plot.
                 return_data (boolean, optional): When set to True, the sonogram matrix will be returned instead of plotted.
                 graph_title (string, optional): Text that will appear as title for the graph.
                 verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
+                start_at_zero (boolean, optional): If set to True, the X axis will start at 0, instead of starting at the minimum timestamp.
 
         Returns:
                 int[ , ]: Disparity matrix. Only returned if return_data is set to True.
 
         Raises:
                 SettingsError: if settings.mono_stereo == 0
 
         Note:
                 This function can only be called if the mono_stereo parameter in settings is set to 1.
         """
-        if settings.mono_stereo == 1:    
-            total_time = max(spikes_file.timestamps) - min(spikes_file.timestamps)
-            diff = np.zeros((settings.num_channels*(settings.on_off_both + 1), int(math.ceil(total_time/settings.bin_size))))
-
-            last_time = min(spikes_file.timestamps)
-
-            its = int(math.ceil(total_time/settings.bin_size))
-
-            #THIS IS NOT NEEDED IF TS ARE SORTED
-            aedat_addr_ts = list(zip(spikes_file.addresses, spikes_file.timestamps))
-            aedat_addr_ts = sorted(aedat_addr_ts, key=Utils.getKey)
-            spikes_file = Utils.extract_addr_and_ts(aedat_addr_ts)
-
-            if verbose == True: start_time = time.time()
-            for i in range(its):
-                a =  bisect_left(spikes_file.timestamps, last_time)
-                b =  bisect_right(spikes_file.timestamps, last_time + settings.bin_size)
+        if settings.mono_stereo == 1:
+            if verbose:
+                start_time = time.time()
+
+            # In range timestamps
+            if start_at_zero and spikes_file.min_ts != 0:
+                Functions.adapt_timestamps(spikes_file, settings)
+
+            total_time = spikes_file.max_ts - spikes_file.min_ts
+            last_time = spikes_file.min_ts
+
+            # Calculate number of addresses and number of windows
+            num_addresses = settings.num_channels * (settings.on_off_both + 1) * (settings.mono_stereo + 1)
+            mid_address = round(num_addresses / 2)
+            num_windows = int(math.ceil(total_time / settings.bin_size))
+
+            # Define diff array and partial arrays
+            diff = np.zeros((round(num_addresses / 2), num_windows))
+
+            if verbose:
+                start_time = time.time()
+
+            for i in range(num_windows):
+                a = bisect_left(spikes_file.timestamps, last_time)
+                b = bisect_right(spikes_file.timestamps, last_time + settings.bin_size)
 
                 blockAddr = spikes_file.addresses[a:b]
-                
-                spikes = np.bincount(blockAddr, minlength=settings.num_channels*(settings.on_off_both + 1)*(settings.mono_stereo+1))
-                
+
+                spikes = np.bincount(blockAddr, minlength=num_addresses)
+
+                diff[:, i] = spikes[0:mid_address] - spikes[mid_address:num_addresses]
+
                 last_time += settings.bin_size
 
-                diff[:, i] = [x1 - x2 for (x1, x2) in list(zip(spikes[0:settings.num_channels*(settings.on_off_both + 1)], spikes[settings.num_channels*(settings.on_off_both + 1):settings.num_channels*(settings.on_off_both + 1)*2]))]
-            if verbose == True: print('DIFF CALCULATION', time.time() - start_time)
-            
-            if max(abs(np.min(diff)), np.max(diff)) != 0: diff = diff*100/max(abs(np.min(diff)), np.max(diff))
+            if verbose:
+                print('DIFF CALCULATION', time.time() - start_time)
 
-            if return_data == False:
+            max_abs = np.max(abs(diff))
+            if max_abs != 0:
+                diff = diff * 100 / max_abs
+
+            if not return_data:
                 # REPRESENTATION
                 plt.style.use('default')
-                sng_fig = plt.figure()
-                sng_fig.canvas.set_window_title(graph_title)
-                
-                #cmap = 'RdBu'
-                colors = [(1, 0.49803921568627450980392156862745, 0.05490196078431372549019607843137), (1, 1, 1), (0.12156862745098039215686274509804, 0.46666666666666666666666666666667, 0.70588235294117647058823529411765)]  # R -> G -> B
+                dlr_fig = plt.figure()
+                dlr_fig.canvas.manager.set_window_title(graph_title)
+
+                # cmap = 'RdBu'
+                colors = [(1, 0.49803921568627450980392156862745, 0.05490196078431372549019607843137), (1, 1, 1), (
+                    0.12156862745098039215686274509804, 0.46666666666666666666666666666667,
+                    0.70588235294117647058823529411765)]  # R -> G -> B
                 n_bins = [3, 6, 10, 100]  # Discretizes the interpolation into bins
                 cmap_name = 'my_list'
                 cm = LinearSegmentedColormap.from_list(cmap_name, colors, N=100)
 
-                plt.imshow(diff, vmin=-100, vmax=100, aspect="auto", cmap=cm) #, aspect="auto")
+                plt.imshow(diff, vmin=-100, vmax=100, aspect="auto", cmap=cm, rasterized=True)  # , aspect="auto")
                 plt.gca().invert_yaxis()
 
-                plt.xlabel('Bin ('+str(settings.bin_size) + '$\mu$s width)', fontsize='large')
+                plt.xlabel('Bin (' + str(settings.bin_size) + '$\mu$s width)', fontsize='large')
                 plt.ylabel('Address', fontsize='large')
 
                 plt.title(graph_title, fontsize='x-large')
 
                 colorbar = plt.colorbar(ticks=[100, 50, 0, -50, -100], orientation='horizontal')
-                colorbar.set_label('Cochlea predominance', rotation=0, fontsize='large', labelpad= 10)
+                colorbar.set_label('Cochlea predominance', rotation=0, fontsize='large', labelpad=10)
                 colorbar.ax.set_xticklabels(['100% L\nCochlea', '50%', '0%\nL==R', '50%', '100% R\nCochlea'])
                 colorbar.ax.invert_xaxis()
-                sng_fig.show()
+
+                return dlr_fig
             else:
                 return diff
         else:
-            #print("This functionality is only available for stereo AEDAT files.")
+            # print("This functionality is only available for stereo AEDAT files.")
             print("[Plots.difference_between_LR] > SettingsError: This functionality is only available for stereo files.")
-        
+
     @staticmethod
-    def mso_heatmap(localization_file, localization_settings, graph_title = "MSO heatmap", enable_colorbar = True, verbose = False):
+    def mso_heatmap(localization_file, localization_settings, graph_title="MSO heatmap", enable_colorbar=True,
+                    verbose=False):
         """
         Plots the heatmap for the MSO activity extracted from a LocalizationFile.
 
         This is, a graph where the X axis means the neuron ID, the Y axis means the frequency channel to which the MSO neuron's population are connected, and the color means the activity.
 
         Parameters:
                 localization_file (LocalizationFile): Localization file to plot.
                 localization_settings (LocalizationSettings): Localization configuration parameters for the file to plot.
                 graph_title (string, optional): Text that will appear as title for the graph.
                 enable_colorbar (boolean, optional): Set to True if you want to show the color bar that indicates the activity range by colors.
                 verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
-        
+
         Returns:
                 None.
 
         Note:
                 None.
         """
 
@@ -419,71 +457,72 @@
         mso_number_freq_ch = localization_settings.mso_end_channel - localization_settings.mso_start_channel + 1
 
         # Create the activity matrix
         mso_activity = np.zeros((mso_number_freq_ch, localization_settings.mso_num_neurons_channel))
 
         num_mso_events = len(localization_file.mso_timestamps)
 
-        for i in range (0, num_mso_events):
+        for i in range(0, num_mso_events):
             # Move the frequency channel from the relative range to an absolute range starting at zero
             freq_channel = localization_file.mso_channels[i] - localization_settings.mso_start_channel
             neuron_id = localization_file.mso_neuron_ids[i]
             # Accumulate the activity for each neuron for each frequency channel according to the LocalizationFIle
             mso_activity[freq_channel][neuron_id] = mso_activity[freq_channel][neuron_id] + 1
-        
+
         if verbose == True: print('MSO HEATMAP CALCULATION', time.time() - start_time)
 
         # Generate the labels lists
         freq_channel_labels = []
         for i in range(localization_settings.mso_start_channel, localization_settings.mso_end_channel + 1):
             freq_channel_labels.append(str(i))
-        
+
         neuron_id_labels = []
         for i in range(0, localization_settings.mso_num_neurons_channel):
             neuron_id_labels.append(str(i))
 
         # REPRESENTATION
         plt.style.use('seaborn-ticks')
         htmap_fig, htmap_ax = plt.subplots()
-        htmap_fig.canvas.set_window_title(graph_title)
-        
+        htmap_fig.canvas.manager.set_window_title(graph_title)
+
         # Create the heatmap image
         htmap_im = plt.imshow(mso_activity, cmap='viridis')
 
-        if enable_colorbar == True :
+        if enable_colorbar == True:
             colorbar = plt.colorbar()
-            colorbar.set_label('No. of spikes', rotation=270, fontsize='large', labelpad= 10)
+            colorbar.set_label('No. of spikes', rotation=270, fontsize='large', labelpad=10)
 
         # Set the ticks
         htmap_ax.set_xticks(np.arange(len(neuron_id_labels)))
         htmap_ax.set_yticks(np.arange(len(freq_channel_labels)))
         # And set all the ticks' labels
         htmap_ax.set_xticklabels(neuron_id_labels)
         htmap_ax.set_yticklabels(freq_channel_labels)
 
         htmap_ax.set_xlabel('Neuron ID', fontsize='large')
         htmap_ax.set_ylabel('Freq. channel', fontsize='large')
 
         # Rotate the tick labels and set their alignment.
         plt.setp(htmap_ax.get_xticklabels(), rotation=45, ha="right",
-                rotation_mode="anchor")
+                 rotation_mode="anchor")
 
         # Loop over data dimensions and create text annotations.
         for i in range(len(freq_channel_labels)):
             for j in range(len(neuron_id_labels)):
                 text = htmap_ax.text(j, i, mso_activity[i, j],
-                            ha="center", va="center", color="w", fontsize='xx-small')
-        
+                                     ha="center", va="center", color="w", fontsize='xx-small')
+
         plt.title(graph_title, fontsize='x-large')
 
         plt.tight_layout()
         htmap_fig.show()
 
     @staticmethod
-    def mso_spikegram(localization_file, settings, localization_settings, dot_size = 0.2, graph_title = 'MSO spikegram', verbose = False):
+    def mso_spikegram(localization_file, settings, localization_settings, dot_size=0.2, graph_title='MSO spikegram',
+                      verbose=False):
         """
         Plots the 3D spikegram (also known as raster plot) of the MSO information contained in a LocalizationFile.
         This is, a graph where the X axis represents neuron IDs, the Y axis means time, and the Z axis represents the frequency channels of the cochlea, and where every spike is plotted as a dot.
 
         Parameters:
                 localization_file (LocalizationFile): Localization file to plot.
                 settings (MainSettings): Configuration parameters for the file to plot.
@@ -491,29 +530,30 @@
                 dot_size (float): Size of the dots used in the spikegram plot.
                 graph_title (string, optional): Text that will appear as title for the graph.
                 verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
 
         Returns:
                 None.
 
-        Note: 
+        Note:
                 None.
         """
 
         if verbose == True: start_time = time.time()
 
         # REPRESENTATION
         plt.style.use('seaborn-whitegrid')
         msospk_fig = plt.figure()
         ax = msospk_fig.add_subplot(111, projection='3d')
-        msospk_fig.canvas.set_window_title(graph_title)
+        msospk_fig.canvas.manager.set_window_title(graph_title)
 
         # Plot all the spikes stored in the localization_file
-        ax.scatter(localization_file.mso_neuron_ids, localization_file.mso_timestamps, localization_file.mso_channels, s=dot_size)
-            
+        ax.scatter(localization_file.mso_neuron_ids, localization_file.mso_timestamps, localization_file.mso_channels,
+                   s=dot_size)
+
         if verbose == True: print('MSO SPIKEGRAM CALCULATION', time.time() - start_time)
 
         plt.title(graph_title, fontsize='x-large')
 
         # Set the label of each axis
         ax.set_xlabel('Neuron ID', fontsize='large')
         ax.set_ylabel('Timestamp ($\mu$s)', fontsize='large')
@@ -524,28 +564,29 @@
         ax.set_ylim([0, localization_file.mso_timestamps[-1]])
         ax.set_zlim([0, settings.num_channels])
 
         plt.tight_layout()
         msospk_fig.show()
 
     @staticmethod
-    def mso_localization_plot(localization_file, settings, localization_settings, graph_title = "MSO localization estimation", start_at_zero = True, verbose = False):
+    def mso_localization_plot(localization_file, settings, localization_settings,
+                              graph_title="MSO localization estimation", start_at_zero=True, verbose=False):
         """
         Plots the result of the coincidence counters of the Jeffress model for the MSO according to the activity in the LocalizationFile.
 
         This is, the neuron that fired the most in a time bin, thus indicating the sound source position.
 
         Parameters:
                 localization_file (LocalizationFile): Localization file to plot.
                 settings (MainSettings): Configuration parameters for the file to plot.
                 localization_settings (LocalizationSettings): Localization configuration parameters for the file to plot.
                 graph_title (string, optional): Text that will appear as title for the graph.
                 start_at_zero (boolean, optional): If set to True, the X axis will start at 0, instead of starting at the minimum timestamp.
                 verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
-        
+
         Returns:
                 None.
 
         Note:
                 None.
         """
 
@@ -558,22 +599,22 @@
             total_time = max(localization_file.mso_timestamps)
             last_time = 0
         else:
             total_time = max(localization_file.mso_timestamps) - min(localization_file.mso_timestamps)
             last_time = min(localization_file.mso_timestamps)
 
         # Estimate the number of time bins
-        its = int(math.ceil(total_time/settings.bin_size))
+        its = int(math.ceil(total_time / settings.bin_size))
 
         # Create the activity array
         mso_activity = np.zeros((its, localization_settings.mso_num_neurons_channel))
         mso_max_activity = np.zeros(its)
 
         # For each time bin, calculate the activity of all the MSO neurons and get the winner
-        for i in range (0, its):
+        for i in range(0, its):
             a = bisect_left(localization_file.mso_timestamps, last_time)
             b = bisect_right(localization_file.mso_timestamps, last_time + settings.bin_size)
 
             blockNeuronIDs = localization_file.mso_neuron_ids[a:b]
 
             spikes = np.bincount(blockNeuronIDs, minlength=localization_settings.mso_num_neurons_channel)
 
@@ -586,85 +627,85 @@
             mso_max_activity[i] = index_max_activity
 
         if verbose == True: print('MSO_LOCALIZATION PLOT CALCULATION', time.time() - start_time)
 
         # Set the figure
         plt.style.use('seaborn-whitegrid')
         mso_loc_fig = plt.figure()
-        mso_loc_fig.canvas.set_window_title(graph_title)
+        mso_loc_fig.canvas.manager.set_window_title(graph_title)
         plt.title(graph_title, fontsize='x-large')
-        plt.xlabel('Bin ('+str(settings.bin_size) + '$\mu$s width)', fontsize='large')
+        plt.xlabel('Bin (' + str(settings.bin_size) + '$\mu$s width)', fontsize='large')
         plt.ylabel('Position (in degrees)', fontsize='large')
         plt.ylim([-1, localization_settings.mso_num_neurons_channel + 1])
-        
+
         yticklabels = []
         angle_slot = 180.0 / localization_settings.mso_num_neurons_channel
         for slot_index in range(0, localization_settings.mso_num_neurons_channel):
             middle_angle = (slot_index * angle_slot) - 90.0 + (angle_slot / 2.0)
             yticklabels.append(str(int(abs(middle_angle))))
 
         plt.yticks(ticks=np.arange(localization_settings.mso_num_neurons_channel), labels=yticklabels, fontsize='small')
 
-        plt.plot(np.arange(math.ceil(total_time/settings.bin_size)), mso_max_activity, label='Position estimation')
+        plt.plot(np.arange(math.ceil(total_time / settings.bin_size)), mso_max_activity, label='Position estimation')
 
         # Add some text to clarify the results
         plt.annotate('Left side',
-        xy=(1.00, 0.85), xytext=(5, 0),
-        xycoords=('axes fraction', 'axes fraction'),
-        textcoords='offset points',
-        size=11, ha='center', va='center', rotation=270)
+                     xy=(1.00, 0.85), xytext=(5, 0),
+                     xycoords=('axes fraction', 'axes fraction'),
+                     textcoords='offset points',
+                     size=11, ha='center', va='center', rotation=270)
 
         plt.annotate('Centre',
-        xy=(1.00, 0.50), xytext=(5, 0),
-        xycoords=('axes fraction', 'axes fraction'),
-        textcoords='offset points',
-        size=11, ha='center', va='center', rotation=270)
+                     xy=(1.00, 0.50), xytext=(5, 0),
+                     xycoords=('axes fraction', 'axes fraction'),
+                     textcoords='offset points',
+                     size=11, ha='center', va='center', rotation=270)
 
         plt.annotate('Right side',
-        xy=(1.00, 0.15), xytext=(5, 0),
-        xycoords=('axes fraction', 'axes fraction'),
-        textcoords='offset points',
-        size=11, ha='center', va='center', rotation=270)
+                     xy=(1.00, 0.15), xytext=(5, 0),
+                     xycoords=('axes fraction', 'axes fraction'),
+                     textcoords='offset points',
+                     size=11, ha='center', va='center', rotation=270)
 
         plt.tight_layout()
         mso_loc_fig.show()
-    
+
     @staticmethod
-    def mso_histogram(localization_file, settings, localization_settings, graph_title = 'MSO histogram', verbose = False):
+    def mso_histogram(localization_file, settings, localization_settings, graph_title='MSO histogram', verbose=False):
         """
         Plots the 3D histogram of the MSO information contained in a LocalizationFile.
-        
+
         This is, a graph where neuron IDs are represented in the X axis, frequency channels are represented in the Y axis, and number of spikes in the Z axis.
 
         Parameters:
                 localization_file (LocalizationFile): Localization file to plot.
                 settings (MainSettings): Configuration parameters for the file to plot.
                 localization_settings (LocalizationSettings): Localization configuration parameters for the file to plot.
                 graph_title (string, optional): Text that will appear as title for the graph.
                 verbose (boolean, optional): Set to True if you want the execution time of the function to be printed.
 
         Returns:
                 None.
-        
+
         Note:
                 None.
         """
 
         start_time = time.time()
-        
+
         # Set the total number of frequency channels
         mso_number_freq_ch = localization_settings.mso_end_channel - localization_settings.mso_start_channel + 1
 
         # Create the activity matrix
         mso_activity = np.zeros((mso_number_freq_ch, localization_settings.mso_num_neurons_channel))
 
         num_mso_events = len(localization_file.mso_timestamps)
 
         # Calculate the total number of events for each frequency channel and for each neuron ID
-        for i in range (0, num_mso_events):
+        for i in range(0, num_mso_events):
             freq_channel = localization_file.mso_channels[i] - localization_settings.mso_start_channel
             neuron_id = localization_file.mso_neuron_ids[i]
             # Accumulate the activity for each neuron for each frequency channel according to the LocalizationFIle
             mso_activity[freq_channel][neuron_id] = mso_activity[freq_channel][neuron_id] + 1
 
         if verbose == True: print('MSO HISTOGRAM CALCULATION:', time.time() - start_time)
 
@@ -684,30 +725,30 @@
         bottom = np.zeros_like(top)
         width = depth = 1
 
         ax.bar3d(x, y, bottom, width - 0.25, depth - 0.5, top, shade=True)
         ax.set_title('Shaded')
 
         # Set the axes' limits
-        ax.set_xlim3d(0,localization_settings.mso_num_neurons_channel)
-        ax.set_ylim3d(0,mso_number_freq_ch)
-        ax.set_zlim3d(0,np.amax(z))
+        ax.set_xlim3d(0, localization_settings.mso_num_neurons_channel)
+        ax.set_ylim3d(0, mso_number_freq_ch)
+        ax.set_zlim3d(0, np.amax(z))
 
         # Set the axes' labels
         ax.set_xlabel('Neuron ID', fontsize='large')
         ax.set_ylabel('Freq. channel', fontsize='large')
         ax.set_zlabel('No. of spikes', fontsize='large')
 
         # Generate the labels lists
         freq_channel_labels = []
         for i in range(localization_settings.mso_start_channel, localization_settings.mso_end_channel + 1):
             freq_channel_labels.append(str(i))
-        
+
         # Set all the ticks
         ax.set_yticks(np.arange(len(freq_channel_labels)))
         # And all the ticks' labels
         ax.set_yticklabels(freq_channel_labels)
 
-        mso_hst_fig.canvas.set_window_title(graph_title)
+        mso_hst_fig.canvas.manager.set_window_title(graph_title)
         plt.title(graph_title, fontsize='x-large')
 
         mso_hst_fig.show()
```

### Comparing `pyNAVIS-1.1.0/pyNAVIS/savers.py` & `pyNAVIS-1.1.1/pyNAVIS/savers.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.0/pyNAVIS/splitters.py` & `pyNAVIS-1.1.1/pyNAVIS/splitters.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 ##    You should have received a copy of the GNU General Public License        ##
 ##    along with pyNAVIS.  If not, see <http://www.gnu.org/licenses/>.         ##
 ##                                                                             ##
 #################################################################################
 
 
 import copy
-import random
+# import random
 import numpy as np
 import time
+import os
 from bisect import bisect_left, bisect_right
 
 from .functions import Functions
 from .savers import Savers
 from .utils import Utils
-from .loaders import SpikesFile
+from .objects import SpikesFile
 
 class Splitters:
 
     @staticmethod
     def manual_splitter(spikes_file, settings, init, end = -1, return_save_both = 0, output_format = '.aedat', path=None):
         """
         Extract a portion of the input SpikesFile file.
@@ -146,15 +147,15 @@
                 
         Returns:
                 None.
         """
         number_of_splits_generated = 0
         index_previous_split = 0
         new_spikes_file = SpikesFile([], [])
-        spikes_filtered =  segmenter_RT(spikes_file,noise_threshold, bin_width, return_save_both = 0)
+        spikes_filtered = Splitters.segmenter_RT(spikes_file,noise_threshold, bin_width, return_save_both = 0)
 
         for i in range(1, len(spikes_filtered.timestamps)):
             if spikes_filtered.timestamps[i] - spikes_filtered.timestamps[i-1] >= bin_width:
                 new_spikes_file.addresses = spikes_filtered.addresses[index_previous_split:i]
                 new_spikes_file.timestamps = spikes_filtered.timestamps[index_previous_split:i]
                 index_previous_split = i
                 number_of_splits_generated += 1
```

### Comparing `pyNAVIS-1.1.0/pyNAVIS/utils.py` & `pyNAVIS-1.1.1/pyNAVIS/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,18 @@
 ##    GNU General Public License for more details.                             ##
 ##                                                                             ##
 ##    You should have received a copy of the GNU General Public License        ##
 ##    along with pyNAVIS.  If not, see <http://www.gnu.org/licenses/>.         ##
 ##                                                                             ##
 #################################################################################
 
-import math
-import struct
 import time
 
-import matplotlib.pyplot as plt
-import numpy as np
+from .objects import SpikesFile
 
-from .loaders import SpikesFile
 
 class Utils:
 
 	@staticmethod
 	def extract_addr_and_ts(zipped_addr_ts):
 		"""
 		Converts a list of [address, timestamp] tuples into a SpikesFile.
@@ -38,15 +34,15 @@
 		Parameters:
 				aedat_addr_ts (list): A list of [address, timestamp] tuples.
 
 		Returns:
 				SpikesFile: A SpikesFile object with the addresses and timestamps obtained from zipped_addr_ts
 		"""
 
-		spikes_file = SpikesFile([], [])
+		spikes_file = SpikesFile()
 		spikes_file.addresses = [x[0] for x in zipped_addr_ts]
 		spikes_file.timestamps = [x[1] for x in zipped_addr_ts]
 		return spikes_file
 
 	@staticmethod
 	def execution_time(executing_function, function_params):
 		"""
```

### Comparing `pyNAVIS-1.1.0/setup.py` & `pyNAVIS-1.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     README = readme_file.read()
 """
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 """
 setup_args = dict(
     name='pyNAVIS',
-    version='1.1.0',
+    version='1.1.1',
     description='Useful tools to analyze and process spiking information from neuromorphic auditory sensors.',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GPL',
     packages=find_packages(),
     author='Juan P. Dominguez-Morales',
-    author_email='jpdominguez@atc.us.es',
+    author_email='jpdominguez@us.es',
     keywords=['pyNAVIS', 'NAVIS', 'neuromorphic engineering', "neuromorphic audio processing", "neuromorphic sensors"],
     url='https://github.com/jpdominguez/pyNAVIS',
     download_url='https://pypi.org/project/pyNAVIS/'
 )
 
 install_requires = [
 	'matplotlib',
```

