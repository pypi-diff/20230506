# Comparing `tmp/noisepy_seis-0.7.1.tar.gz` & `tmp/noisepy_seis-0.8.0.tar.gz`

## Comparing `noisepy_seis-0.7.1.tar` & `noisepy_seis-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    12728 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   112952 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35394 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/LICENSE
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/README.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     8722 2020-02-02 00:00:00.000000 noisepy_seis-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    12728 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   112952 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35394 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/README.md
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/PKG-INFO
```

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.8.0/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.8.0/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.8.0/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.8.0/src/noisepy/seis/S2_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/__init__.py` & `noisepy_seis-0.8.0/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.8.0/src/noisepy/seis/asdfstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.8.0/src/noisepy/seis/channelcatalog.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
-import os
 from abc import ABC, abstractmethod
 from functools import lru_cache
 
 import diskcache as dc
 import obspy
 import pandas as pd
 from datetimerange import DateTimeRange
 from obspy import UTCDateTime, read_inventory
 from obspy.clients.fdsn import Client
 
 from .datatypes import Channel, Station
+from .utils import fs_join, get_filesystem
 
 logger = logging.getLogger(__name__)
 
 
 class ChannelCatalog(ABC):
     """
     An abstract catalog for getting full channel information (lat, lon, elev, resp)
@@ -50,33 +50,35 @@
     @abstractmethod
     def get_inventory(self, timespan: DateTimeRange, station: Station) -> obspy.Inventory:
         pass
 
 
 class XMLStationChannelCatalog(ChannelCatalog):
     """
-    A channel catalog that reads <station>.XML files from a directory
+    A channel catalog that reads <station>.XML files from a directory or an s3://... bucket url path.
     """
 
-    def __init__(self, xmldir: str) -> None:
+    def __init__(self, xmlpath: str) -> None:
         super().__init__()
-        self.xmldir = xmldir
-        if not os.path.exists(self.xmldir):
-            raise Exception(f"The XML Station file directory '{xmldir}' doesn't exist")
+        self.xmlpath = xmlpath
+        self.fs = get_filesystem(xmlpath)
+        if not self.fs.exists(self.xmlpath):
+            raise Exception(f"The XML Station file directory '{xmlpath}' doesn't exist")
 
     def get_inventory(self, timespan: DateTimeRange, station: Station) -> obspy.Inventory:
-        xmlfile = os.path.join(self.xmldir, f"{station.network}_{station.name}.xml")
+        xmlfile = fs_join(self.xmlpath, f"{station.network}_{station.name}.xml")
         return self._get_inventory_from_file(xmlfile)
 
     @lru_cache
     def _get_inventory_from_file(self, xmlfile):
-        if not os.path.exists(xmlfile):
+        if not self.fs.exists(xmlfile):
             logger.warning(f"Could not find StationXML file {xmlfile}. Returning empty Inventory()")
             return obspy.Inventory()
-        return read_inventory(xmlfile)
+        with self.fs.open(xmlfile) as f:
+            return read_inventory(f)
 
 
 class FDSNChannelCatalog(ChannelCatalog):
     """
     A channel catalog that queries the FDSN service
     FDSN ~ International Federation of Digital Seismograph Network
     """
```

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.8.0/src/noisepy/seis/datatypes.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/main.py` & `noisepy_seis-0.8.0/src/noisepy/seis/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import argparse
 import os
 import typing
 from enum import Enum
-from glob import glob
 from typing import Any, Callable, List
 
 import obspy
 
 from .asdfstore import ASDFCCStore, ASDFRawDataStore
 from .channelcatalog import CSVChannelCatalog, XMLStationChannelCatalog
 from .constants import DATE_FORMAT_HELP, STATION_FILE
 from .datatypes import Channel, ConfigParameters
 from .S0A_download_ASDF_MPI import download
 from .S1_fft_cc_MPI import cross_correlate
 from .S2_stacking import stack
 from .scedc_s3store import SCEDCS3DataStore
+from .utils import fs_join, get_filesystem
 
 # Utility running the different steps from the command line. Defines the arguments for each step
 
 default_start_date = "2016_07_01_0_0_0"  # start date of download
 default_end_date = "2016_07_02_0_0_0"  # end date of download
 default_data_path = "Documents/SCAL"
 
@@ -33,15 +33,15 @@
 def valid_date(d: str) -> str:
     _ = obspy.UTCDateTime(d)
     return d
 
 
 def initialize_fft_params(raw_dir: str) -> ConfigParameters:
     params = ConfigParameters()
-    dfile = os.path.join(raw_dir, "download_info.txt")
+    dfile = fs_join(raw_dir, "download_info.txt")
     if os.path.isfile(dfile):
         down_info = eval(open(dfile).read())  # TODO: do proper json/yaml serialization
         params.samp_freq = down_info["samp_freq"]
         params.freqmin = down_info["freqmin"]
         params.freqmax = down_info["freqmax"]
         params.start_date = down_info["start_date"]
         params.end_date = down_info["end_date"]
@@ -55,16 +55,18 @@
         return lambda ch: True
     else:
         stations = set(sta_list)
         return lambda ch: ch.station.name in stations
 
 
 def create_raw_store(raw_dir: str, sta_list: List[str], xml_path: str):
+    fs = get_filesystem(raw_dir)
+
     def count(pat):
-        return len(glob(os.path.join(raw_dir, pat)))
+        return len(fs.glob(fs_join(raw_dir, pat)))
 
     # Use heuristics around which store to use by the files present
     if count("*.h5") > 0:
         return ASDFRawDataStore(raw_dir)
     else:
         assert count("*.ms") > 0 or count("*.sac") > 0, f"Can not find any .h5, .ms or .sac files in {raw_dir}"
         if xml_path is not None:
```

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.8.0/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.8.0/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.8.0/src/noisepy/seis/scedc_s3store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import glob
 import logging
 import os
 import re
 from datetime import datetime, timedelta, timezone
 from typing import Callable, List
 
 import obspy
 from datetimerange import DateTimeRange
 
 from noisepy.seis.channelcatalog import ChannelCatalog
 from noisepy.seis.stores import RawDataStore
 
 from .datatypes import Channel, ChannelData, ChannelType, Station
+from .utils import fs_join, get_filesystem
 
 logger = logging.getLogger(__name__)
 
 
 class SCEDCS3DataStore(RawDataStore):
     """
     A data store implementation to read from a directory of miniSEED (.ms) files from the SCEDC S3 bucket.
@@ -23,28 +23,30 @@
     """
 
     # TODO: Support reading directly from the S3 bucket
 
     # for checking the filename has the form: CIGMR__LHN___2022002.ms
     file_re = re.compile(r".*[0-9]{7}\.ms$", re.IGNORECASE)
 
-    def __init__(self, directory: str, chan_catalog: ChannelCatalog, channel_filter: Callable[[Channel], bool] = None):
+    def __init__(self, path: str, chan_catalog: ChannelCatalog, channel_filter: Callable[[Channel], bool] = None):
         """
         Parameters:
-            directory: directory to look for ms files
+            path: path to look for ms files. Can be a local file directory or an s3://... url path
             chan_catalog: ChannelCatalog to retrieve inventory information for the channels
             channel_filter: Function to decide whether a channel should be used or not,
                             if None, all channels are used
         """
         super().__init__()
-        self.directory = directory
+        self.fs = get_filesystem(path)
+        self.path = path
         self.channel_catalog = chan_catalog
         if channel_filter is None:
             channel_filter = lambda s: True  # noqa: E731
-        msfiles = [f for f in glob.glob(os.path.join(directory, "*.ms")) if self.file_re.match(f) is not None]
+
+        msfiles = [f for f in self.fs.glob(fs_join(path, "*.ms")) if self.file_re.match(f) is not None]
         # store a dict of {timerange: list of channels}
         self.channels = {}
         timespans = []
         for f in msfiles:
             timespan = SCEDCS3DataStore._parse_timespan(f)
             channel = SCEDCS3DataStore._parse_channel(os.path.basename(f))
             if not channel_filter(channel):
@@ -68,20 +70,21 @@
 
     def read_data(self, timespan: DateTimeRange, chan: Channel) -> ChannelData:
         # reconstruct the file name from the channel parameters
         chan_str = (
             f"{chan.station.network}{chan.station.name.ljust(5, '_')}{chan.type.name}"
             f"{chan.station.location.ljust(3, '_')}"
         )
-        filename = os.path.join(self.directory, f"{chan_str}{timespan.start_datetime.strftime('%Y%j')}.ms")
-        if not os.path.exists(filename):
+        filename = fs_join(self.path, f"{chan_str}{timespan.start_datetime.strftime('%Y%j')}.ms")
+        if not self.fs.exists(filename):
             logger.warning(f"Could not find file {filename}")
             return ChannelData.empty()
 
-        stream = obspy.read(filename)
+        with self.fs.open(filename) as f:
+            stream = obspy.read(f)
         return ChannelData(stream)
 
     def get_inventory(self, timespan: DateTimeRange, station: Station) -> obspy.Inventory:
         return self.channel_catalog.get_inventory(timespan, station)
 
     def _parse_timespan(filename: str) -> DateTimeRange:
         # The SCEDC S3 bucket stores files in the form: CIGMR__LHN___2022002.ms
```

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/stores.py` & `noisepy_seis-0.8.0/src/noisepy/seis/stores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.8.0/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.8.0/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.8.0/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.8.0/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/.gitignore` & `noisepy_seis-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/LICENSE` & `noisepy_seis-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.7.1/README.md` & `noisepy_seis-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,16 @@
 * download continous noise data based on obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
 * save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
 * offers high flexibility to handle messy SAC/miniSEED data stored on your local machine and convert them into ASDF format data that could easily be pluged into NoisePy
 * performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
 * includes a series of monitoring functions to measure dv/v on the resulted cross-correlation functions using some recently developed new methods (see our papers for more details<sup>**</sup>)
 
 # Short tutorial
-A short tutorial on how to use NoisePy-seis can be found in the following Jupyter Notebook: https://github.com/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb
+A short tutorial on how to use NoisePy-seis can be is available as a [Jupyter notebook](https://github.com/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb) and can be
+[run directly in Colab](https://colab.research.google.com/github/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb).
 
 
 This tutorial presents one simple example of how NoisePy might work! We strongly encourage you to download the NoisePy package and play it on your own! If you have any  comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
 
 Chengxin Jiang (chengxinjiang@gmail.com)
 Marine Denolle (mdenolle@uw.edu).
```

### Comparing `noisepy_seis-0.7.1/pyproject.toml` & `noisepy_seis-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     "mpi4py>=3.1.4",
     "numba>=0.57.0",
     "numpy>=1.22.0",
     "pandas>=1.5.3",
     "pyasdf>=0.7.5",
     "pycwt>=0.3.0a22",
     "diskcache>=5.5",
+    "fsspec>=2023.4.0",
+    "s3fs>=2023.4.0",
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/mdenolle/NoisePy"
 
 [tool.hatch.version]
```

### Comparing `noisepy_seis-0.7.1/PKG-INFO` & `noisepy_seis-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.7.1
+Version: 0.8.0
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -31,21 +31,23 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Requires-Dist: datetimerange==2.0.0
 Requires-Dist: diskcache>=5.5
+Requires-Dist: fsspec>=2023.4.0
 Requires-Dist: h5py>=3.8.0
 Requires-Dist: mpi4py>=3.1.4
 Requires-Dist: numba>=0.57.0
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: pyasdf>=0.7.5
 Requires-Dist: pycwt>=0.3.0a22
+Requires-Dist: s3fs>=2023.4.0
 Provides-Extra: dev
 Requires-Dist: memory-profiler>=0.61; extra == 'dev'
 Requires-Dist: pre-commit>=3.2; extra == 'dev'
 Requires-Dist: pytest>=7.2.2; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # About NoisePy
@@ -104,15 +106,16 @@
 * download continous noise data based on obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
 * save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
 * offers high flexibility to handle messy SAC/miniSEED data stored on your local machine and convert them into ASDF format data that could easily be pluged into NoisePy
 * performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
 * includes a series of monitoring functions to measure dv/v on the resulted cross-correlation functions using some recently developed new methods (see our papers for more details<sup>**</sup>)
 
 # Short tutorial
-A short tutorial on how to use NoisePy-seis can be found in the following Jupyter Notebook: https://github.com/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb
+A short tutorial on how to use NoisePy-seis can be is available as a [Jupyter notebook](https://github.com/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb) and can be
+[run directly in Colab](https://colab.research.google.com/github/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb).
 
 
 This tutorial presents one simple example of how NoisePy might work! We strongly encourage you to download the NoisePy package and play it on your own! If you have any  comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
 
 Chengxin Jiang (chengxinjiang@gmail.com)
 Marine Denolle (mdenolle@uw.edu).
```

