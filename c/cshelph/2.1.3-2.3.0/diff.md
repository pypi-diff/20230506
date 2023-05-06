# Comparing `tmp/cshelph-2.1.3.tar.gz` & `tmp/cshelph-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshelph-2.1.3.tar", last modified: Sat May  6 03:07:05 2023, max compression
+gzip compressed data, was "cshelph-2.3.0.tar", last modified: Sat May  6 17:24:59 2023, max compression
```

## Comparing `cshelph-2.1.3.tar` & `cshelph-2.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 03:07:05.983249 cshelph-2.1.3/
--rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.1.3/LICENSE.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 03:07:05.983093 cshelph-2.1.3/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1165 2023-05-02 19:47:21.000000 cshelph-2.1.3/README.md
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 03:07:05.982888 cshelph-2.1.3/cshelph.egg-info/
--rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 03:07:05.000000 cshelph-2.1.3/cshelph.egg-info/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-06 03:07:05.000000 cshelph-2.1.3/cshelph.egg-info/SOURCES.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-06 03:07:05.000000 cshelph-2.1.3/cshelph.egg-info/dependency_links.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-06 03:07:05.000000 cshelph-2.1.3/cshelph.egg-info/top_level.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)    19075 2023-05-04 16:18:29.000000 cshelph-2.1.3/cshelph.py
--rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-06 03:07:05.983294 cshelph-2.1.3/setup.cfg
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1571 2023-05-06 03:05:47.000000 cshelph-2.1.3/setup.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 17:24:59.455164 cshelph-2.3.0/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.3.0/LICENSE.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 17:24:59.455044 cshelph-2.3.0/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1165 2023-05-02 19:47:21.000000 cshelph-2.3.0/README.md
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 17:24:59.454393 cshelph-2.3.0/cshelph/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    18618 2023-05-06 15:38:00.000000 cshelph-2.3.0/cshelph/bathy.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-06 17:24:59.454889 cshelph-2.3.0/cshelph.egg-info/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      467 2023-05-06 17:24:59.000000 cshelph-2.3.0/cshelph.egg-info/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      171 2023-05-06 17:24:59.000000 cshelph-2.3.0/cshelph.egg-info/SOURCES.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-06 17:24:59.000000 cshelph-2.3.0/cshelph.egg-info/dependency_links.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-06 17:24:59.000000 cshelph-2.3.0/cshelph.egg-info/top_level.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-06 17:24:59.455203 cshelph-2.3.0/setup.cfg
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1577 2023-05-06 17:24:26.000000 cshelph-2.3.0/setup.py
```

### Comparing `cshelph-2.1.3/LICENSE.txt` & `cshelph-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cshelph-2.1.3/README.md` & `cshelph-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cshelph-2.1.3/cshelph.py` & `cshelph-2.3.0/cshelph/bathy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 '''
-THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.'''
+THE SOFTWARE IS pROVIDED \"AS IS\", WITHOUT WARRANTY OF An_y KIND, EXpRESS OR IMpLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,FITNESS FOR A pARTICULAR pURpOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COpYRIGHT HOLDERS BE LIABLE FOR An_y CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.'''
 
 #####
-# This group of functions processes ICESAT2 data and creates a bathymetric model. 
+# This group of functions processes ICESAT2 data and creates a bathymetric model.
 # To do this, it follows a number of steps in the form of functions, including:
 # 1. Reading data (ReadATL03())
 # 2. Orthometrically correcting the dataset (OrthometricCorrection())
-# 3. Pulling down the data segment ID (getAtl03SegID())
+# 3. pulling down the data segment ID (getAtl03SegID())
 # 4. Bin the data along latitudinal and height gradients (bin_data())
 # 5. Calculate sea height (get_sea_height())
 # 6. Get water temperature (get_water_temp())
 # 7. Correct bathymetry surface for refraction (RefractionCorrection())
 # 8. Calculate bathymetry height (get_bath_height())
-# 9. Produce figures (produce_figures())
+# 9. produce figures (produce_figures())
 #####
 
 import numpy as np
 import h5py as h5
-from matplotlib.widgets import LassoSelector
-from matplotlib.path import Path
 import matplotlib.pyplot as plt
 import pyproj
 from pyproj import Proj
 from pyproj import Transformer
 import pandas as pd
 import argparse
 import os
-import subprocess
 import time
 import utm
 import math
 import fiona
 import geopandas
 #import netCDF4
 from datetime import datetime
 import utm
 import xarray as xr
 import fsspec
+# need s3fs installed
 
-def ReadATL03(h5_file, laser_num):
+def read_atl03(h5_file, laser_num):
     # Read File
     f = h5.File(h5_file,'r')
     
     # Select a laser
     orientation = f['/orbit_info/sc_orient'][0]
     
     # selects the strong beams only [we can include weak beams later on]
@@ -76,27 +74,27 @@
 	elif letter < 'N':
 		epsg = 'epsg:327' + str(num)
 	else:
 		print('Error Finding UTM')
 		
 	return epsg
 
-def OrthometricCorrection(lat, lon, Z, epsg):
+def orthometric_correction(lat, lon, Z, epsg):
     # transform ellipsod (WGS84) height to orthometric height
     transformerh = Transformer.from_crs("epsg:4326", "epsg:3855", always_xy=True)
     X_egm08, Y_egm08, Z_egm08 = transformerh.transform(lon, lat, Z)
     
     # transform WGS84 proj to local UTM
-    myProj = Proj(epsg)
-    X_utm, Y_utm = myProj(lon, lat)
+    myproj = Proj(epsg)
+    X_utm, Y_utm = myproj(lon, lat)
     
     return Y_utm, X_utm, Z_egm08
 
     
-def count_ph_per_seg(ph_index_beg, photon_h): # DEPRECATED
+def count_ph_per_seg(ph_index_beg, photon_h): # DEpRECATED
     
     ph_index_beg = ph_index_beg[ph_index_beg!=0]
     
     # add an extra val at the end of array for upper bounds
     ph_index_beg = np.hstack((ph_index_beg, len(photon_h)+1))-1
     
     photon_id = []
@@ -198,15 +196,15 @@
     sd = np.nanstd(sea_height, axis=0)
     sea_height_1 = np.where((sea_height > (mean + 2*sd)) | (sea_height < (mean - 2*sd)), np.nan, sea_height).tolist()
     
     return sea_height_1
 
 def get_water_temp_redacted(data_path, latitude, longitude):
     '''
-    Pull down surface water temperature along the track from the JPL GHRSST opendap website.
+    pull down surface water temperature along the track from the JpL GHRSST opendap website.
     
     The GHRSST data are gridded tiles with dimension 17998 x 35999. 
     To get the specific grid tile of the SST, you must convert from lat, lon coordinates
     to the gridded tile ratio of the SST data product using the coordinates of the IS2 data.
     '''
     # Get date from data filename
     file_date = data_path[-33:-25]
@@ -233,29 +231,29 @@
     lon_max = 180
     scaled_lon_min = 0
     scaled_lon_max = 35999
 
     new_lon_ratio = round(((lon_avg - lon_min) / (lon_max - lon_min)) *
                     (scaled_lon_max - scaled_lon_min) + lon_min)
 
-    # Access the SST data using the JPL OpenDap interface
-    url = 'https://opendap.jpl.nasa.gov/opendap/OceanTemperature/ghrsst/data/GDS2/L4/GLOB/JPL/MUR/v4.1/'\
+    # Access the SST data using the JpL OpenDap interface
+    url = 'https://opendap.jpl.nasa.gov/opendap/OceanTemperature/ghrsst/data/GDS2/L4/GLOB/JpL/MUR/v4.1/'\
         + str(year) + '/' + str(julian_day) + '/' + str(file_date) \
-        + '090000-JPL-L4_GHRSST-SSTfnd-MUR-GLOB-v02.0-fv04.1.nc'
+        + '090000-JpL-L4_GHRSST-SSTfnd-MUR-GLOB-v02.0-fv04.1.nc'
     
     dataset = netCDF4.Dataset(url)
     
     # Access the data and convert the temperature from K to C
     sea_temp = dataset['analysed_sst'][0,new_lat_ratio, new_lon_ratio] - 273.15
     return sea_temp
 
 def get_water_temp(data_path, latitude, longitude):
     '''
-    Pull down surface water temperature along the track from the MUR SST:
-    https://aws.amazon.com/marketplace/pp/prodview-kvgy4vkuhavsc?sr=0-3&ref_=beagle&applicationId=AWSMPContessa#overview.
+    pull down surface water temperature along the track from the MUR SST:
+    https://aws.amazon.com/marketplace/pp/prodview-kvgy4vkuhavsc?sr=0-3&ref_=beagle&applicationId=AWSMpContessa#overview.
     '''
     # Get date from data filename
     file_date = data_path[-33:-25]
     
     start_date = str(datetime.strptime(file_date + ' 00:00:00', '%Y%m%d %H:%M:%S'))
     end_date = str(datetime.strptime(file_date + ' 23:59:59', '%Y%m%d %H:%M:%S'))
 
@@ -269,57 +267,54 @@
     
     sea_temp = sea_temp_xr['analysed_sst'].sel(time=slice(start_date,end_date))
     
     sst = round(sea_temp.sel(lat=lat_med,lon=lon_med,method='nearest').load().values[0] - 273,2)
     
     return sst
 
-def RefractionCorrection(WTemp, WSmodel, Wavelength, Photon_ref_elev, Ph_ref_azimuth, PhotonZ, PhotonX, PhotonY, Ph_Conf, satellite_altitude):
+def refraction_correction(water_temp, water_surface, wavelength, photon_ref_elev, ph_ref_azimuth, photon_z, photon_x, photon_y, ph_conf, satellite_altitude):
     
     '''
-    WTemp; there is python library that pulls water temp data 
-    WSmodel is the value surface height
+    WTemp; there is python library that pulls water temp data
+    water_surface is the value surface height
     Wavelength is fixed
     '''
     
     # Only process photons below water surface model
-    PhotonX = PhotonX[PhotonZ<=WSmodel]
-    PhotonY = PhotonY[PhotonZ<=WSmodel]
-    Photon_ref_elev = Photon_ref_elev[PhotonZ<=WSmodel]
-    satellite_altitude = satellite_altitude[PhotonZ<=WSmodel]
-    Ph_ref_azimuth = Ph_ref_azimuth[PhotonZ<=WSmodel]
-    Ph_Conf = Ph_Conf[PhotonZ<=WSmodel]
-    PhotonZ = PhotonZ[PhotonZ<=WSmodel]
-    
-    # water temp for refraction correction
-    WaterTemp= WTemp
+    photon_x = photon_x[photon_z<=water_surface]
+    photon_y = photon_y[photon_z<=water_surface]
+    photon_ref_elev = photon_ref_elev[photon_z<=water_surface]
+    satellite_altitude = satellite_altitude[photon_z<=water_surface]
+    ph_ref_azimuth = ph_ref_azimuth[photon_z<=water_surface]
+    ph_conf = ph_conf[photon_z<=water_surface]
+    photon_z = photon_z[photon_z<=water_surface]
     
     # Refraction coefficient #
     a = -0.000001501562500
     b = 0.000000107084865
     c = -0.000042759374989
     d = -0.000160475520686
     e = 1.398067112092424
-    wl = Wavelength
+    wl = wavelength
     
     # refractive index of air
     n1 = 1.00029
     
     # refractive index of water
-    n2 = (a*WaterTemp**2) + (b*wl**2) + (c*WaterTemp) + (d*wl) + e
+    n2 = (a*water_temp**2) + (b*wl**2) + (c*water_temp) + (d*wl) + e
     
     # assumption is 0.25416
     # This example is refractionCoef = 0.25449
     # 1.00029 is refraction of air constant
-    CorrectionCoef = (1-(n1/n2))
+    #correction_coef = (1-(n1/n2))
     #########################
     
     # read photon ref_elev to get theta1
     # Does not account for curvature of Earth
-    theta1 = np.pi/2 - Photon_ref_elev
+    theta1 = np.pi/2 - photon_ref_elev
     
     # H = orbital altitude of IS2 (496km as mean)
     # H = 496km. we pass in the mean of the orbit from /geolocation/altitude_sc/
     # Diff from min to max of 100m over an orbit is 0.02% at 496km
     # More error probably introduced from Re (mean Earth radius) than intra-orbit changes in altitude
     # H = 496
     H = satellite_altitude/1000
@@ -331,78 +326,66 @@
     
     # eq 1. Theta2
     theta2 = np.arcsin(((n1*np.sin(theta1))/n2))
     
     # eq 3. S
     # Approximate water Surface = 1.5
     # D  = raw uncorrected depth
-    D = WSmodel - PhotonZ
+    D = water_surface - photon_z
     
     # For Triangle DTS
     S = D/np.cos(theta1)
     
     # eq 2. R
     R = (S*n1)/n2
     Gamma = (np.pi/2)-theta1
     
-    # For triangle RPS
+    # For triangle RpS
     # phi is an angle needed
     phi = theta1-theta2
     
-    # P is the difference between raw and corrected YZ location
-    P = np.sqrt(R**2 + S**2 - 2*R*S*np.cos(phi))
+    # p is the difference between raw and corrected YZ location
+    p = np.sqrt(R**2 + S**2 - 2*R*S*np.cos(phi))
     
     # alpha is an angle needed
-    alpha = np.arcsin((R*np.sin(phi))/P)
+    alpha = np.arcsin((R*np.sin(phi))/p)
     
     # Beta angle needed for Delta Y an d Delta Z
     Beta = Gamma - alpha
     
     # Delta Y
-    DY = P*np.cos(Beta)
+    DY = p*np.cos(Beta)
     
     # Delta Z
-    DZ = P*np.sin(Beta)
+    DZ = p*np.sin(Beta)
     
     # Delta Easting
-    DE = DY*np.sin(Ph_ref_azimuth)
+    DE = DY*np.sin(ph_ref_azimuth)
     
     # Delta Northing
-    DN = DY*np.cos(Ph_ref_azimuth)
+    DN = DY*np.cos(ph_ref_azimuth)
     
-    outX = PhotonX + DE
-    outY = PhotonY + DN
-    outZ = PhotonZ + DZ
-    '''
-        print('\nFor selected Bathy photon:')
-        print('lat = ', PhotonY[9000])
-        print('long = ', PhotonX[9000])
-        print('Raw Depth = ', PhotonZ[9000])
-        print('D = ', D[9000])
-        
-        print('ref_elev = ', Photon_ref_elev[9000])
-        
-        print('Delta Easting = ', DE[9000])
-        print('Delta Northing = ', DN[9000])
-        print('Delta Z = ', DZ[9000])
-        '''
-    return(outX, outY, outZ, Ph_Conf, PhotonX, PhotonY, PhotonZ, Ph_ref_azimuth, Photon_ref_elev) # We are most interested in outx, outy, outz
+    out_x = photon_x + DE
+    out_y = photon_y + DN
+    out_z = photon_z + DZ
+
+    return(out_x, out_y, out_z, ph_conf, photon_x, photon_y, photon_z, ph_ref_azimuth, photon_ref_elev) # We are most interested in out_x, out_y, out_z
 
 def get_bath_height(binned_data, percentile, WSHeight, height_resolution):
     '''Calculate bathymetry level per bin based on horizontal resolution'''
     # Create sea height list
     bath_height = []
     
     geo_photon_height = []
     geo_longitude = []
     geo_latitude = []
     
     # Group data by latitude
     # Filter out surface data that are two bins below median surface value calculated above
-    binned_data_bath = binned_data[(binned_data['photon_height'] < WSHeight - (height_resolution * 2))] 
+    binned_data_bath = binned_data[(binned_data['photon_height'] < WSHeight - (height_resolution * 2))]
     grouped_data = binned_data_bath.groupby(['lat_bins'], group_keys=True)
     data_groups = dict(list(grouped_data))
     
     # Create a percentile threshold of photon counts in each grid, grouped by both x and y axes.
     count_threshold = np.percentile(binned_data.groupby(['lat_bins', 'height_bins']).size().reset_index().groupby('lat_bins')[[0]].max(), percentile)
     
     # Loop through groups and return average bathy height
@@ -450,52 +433,52 @@
     # Create uniform sea surface based on median sea surface values and filter out surface breaching
     sea_surf = [np.nanmedian(sea_height) if i == i else np.nan for i in sea_height]
     sea_median_df = pd.DataFrame({'x':x_bins, 'y':sea_surf})
 
     # Define figure size
     fig = plt.rcParams["figure.figsize"] = (40,5)
     
-    # Plot raw points
+    # plot raw points
     plt.scatter(x=binned_data.latitude, y = binned_data.photon_height, marker='o', lw=0, s=1, alpha = 0.8, c = 'yellow', label ='Raw photon height')
     plt.scatter(RefY, RefZ, s=0.2, alpha=0.1, c='black')
-    plt.scatter(geo_df.latitude, geo_df.photon_height, s=0.5, alpha=0.1, c='red', label = 'Classified Photons')
+    plt.scatter(geo_df.latitude, geo_df.photon_height, s=0.5, alpha=0.1, c='red', label = 'Classified photons')
     
     #plt.scatter(x=geo_df.latitude, y = geo_df.photon_height, marker='o', lw=0, s=0.8, alpha = 0.8, c = 'black', label = 'Corrected photon bin')
 
-    # Plot median values
+    # plot median values
     #plt.scatter(bath_median_df.x, bath_median_df.y, marker = 'o', c='r', alpha = 0.8, s = 5, label = 'Median bathymetry')
     plt.scatter(sea_median_df.x, sea_median_df.y, marker = 'o', c='b', alpha = 1, s = 0.5, label = 'Median sea surface')
     
     # Insert titles and sub-titles
     plt.title('Icesat2 Bathymetry\n' + file)
     plt.xlabel('Latitude', fontsize=25)
-    plt.ylabel('Photon Height (m)', fontsize=25)
+    plt.ylabel('photon Height (m)', fontsize=25)
     plt.xticks(fontsize=16)
     plt.yticks(fontsize=16)
 
     plt.legend(loc="upper left",prop={'size': 20})
 
     # Limit the x and y axes using parameters
     plt.xlim(left=binned_data.latitude.min(), right=binned_data.latitude.max())
     plt.ylim(top = y_limit_top, bottom = y_limit_bottom)
     
     timestr = time.strftime("%Y%m%d_%H%M%S")
     file = file.replace('.h5','')
     # Define where to save file
     plt.tight_layout()
-    plt.savefig(file + '_gt' + str(laser) + '_' + str(percentile) + '_EPSG' + str(epsg_num) + '_' + timestr + ".png")
+    plt.savefig(file + '_gt' + str(laser) + '_' + str(percentile) + '_EpSG' + str(epsg_num) + '_' + timestr + ".png")
     #plt.show()
     #plt.close()
         
         # convert corrected locations back to wgs84 (useful to contain)
-    transformer = Transformer.from_crs("EPSG:"+str(epsg_num), "EPSG:4326", always_xy=True)
+    transformer = Transformer.from_crs("EpSG:"+str(epsg_num), "EpSG:4326", always_xy=True)
     #print(transformer)
     lon_wgs84, lat_wgs84 = transformer.transform(geo_df.longitude.values, geo_df.latitude.values)
 
     geo_df['lon_wgs84'] = lon_wgs84
     geo_df['lat_wgs84'] = lat_wgs84
     
     geodf = geopandas.GeoDataFrame(geo_df, geometry=geopandas.points_from_xy(geo_df.lon_wgs84,geo_df.lat_wgs84))
     
     geodf.set_crs(epsg=4326, inplace=True)
     
-    geodf.to_file(file + '_gt' + str(laser) + '_' + str(percentile) + '_EPSG' + str(epsg_num) + '_' + timestr + ".gpkg", driver="GPKG")
+    geodf.to_file(file + '_gt' + str(laser) + '_' + str(percentile) + '_EpSG' + str(epsg_num) + '_' + timestr + ".gpkg", driver="GPKG")
```

### Comparing `cshelph-2.1.3/setup.py` & `cshelph-2.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 #
 #
 # Purpose:  Installation of the C-SHELPh software
 #
 # Author: Nathan Thomas
 # Email: nmthomas28@gmail.com
 # Date: 05/05/2023
-# Version: 2.1.1
+# Version: 2.2.0
 #
 # History:
 # Version 2.1.2
 
 from distutils.core import setup
 import os
 
 setup(name='cshelph',
-    version='2.1.3',
+    version='2.3.0',
     description='Classification of Sub-aquatic Height Extracted Photons',
     author='Nathan Thomas and Brian Lee',
     author_email='nmthomas28@gmail.com',
-    scripts=['cshelph.py'],
+    scripts=['cshelph/bathy.py'],
     package_dir={},
     data_files=[],
     license='LICENSE.txt',
     url='https://github.com/nmt28/C-SHELPh',
     classifiers=['Intended Audience :: Developers',
                  'Intended Audience :: Science/Research',
                  'Operating System :: OS Independent',
```

