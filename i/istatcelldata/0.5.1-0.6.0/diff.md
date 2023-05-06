# Comparing `tmp/istatcelldata-0.5.1.tar.gz` & `tmp/istatcelldata-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istatcelldata-0.5.1.tar", max compression
+gzip compressed data, was "istatcelldata-0.6.0.tar", max compression
```

## Comparing `istatcelldata-0.5.1.tar` & `istatcelldata-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1076 2023-04-12 18:25:21.536175 istatcelldata-0.5.1/LICENSE
--rwxr-xr-x   0        0        0      978 2023-04-12 18:25:21.536175 istatcelldata-0.5.1/README.md
--rwxr-xr-x   0        0        0       99 2023-04-14 10:41:50.115834 istatcelldata-0.5.1/istatcelldata/__init__.py
--rwxr-xr-x   0        0        0     6607 2023-04-14 10:48:45.206530 istatcelldata-0.5.1/istatcelldata/config.py
--rwxr-xr-x   0        0        0        0 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/data/__init__.py
--rwxr-xr-x   0        0        0     8447 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/data/census_1991_2001.py
--rwxr-xr-x   0        0        0     3004 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/data/manage_data.py
--rwxr-xr-x   0        0        0     6547 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/download.py
--rwxr-xr-x   0        0        0     4989 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/generic.py
--rwxr-xr-x   0        0        0        0 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/geodata/__init__.py
--rwxr-xr-x   0        0        0     5404 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/geodata/manage_geodata.py
--rw-r--r--   0        0        0     3758 2023-04-14 09:55:28.125042 istatcelldata-0.5.1/istatcelldata/processes.py
--rw-r--r--   0        0        0      869 2023-04-14 10:53:32.404374 istatcelldata-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 istatcelldata-0.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1076 2023-05-06 15:41:41.103342 istatcelldata-0.6.0/LICENSE
+-rwxr-xr-x   0        0        0     1025 2023-05-06 15:41:41.103595 istatcelldata-0.6.0/README.md
+-rwxr-xr-x   0        0        0       99 2023-05-06 15:41:41.105349 istatcelldata-0.6.0/istatcelldata/__init__.py
+-rwxr-xr-x   0        0        0     6522 2023-05-06 15:51:40.441104 istatcelldata-0.6.0/istatcelldata/config.py
+-rwxr-xr-x   0        0        0        0 2023-05-06 15:41:41.105745 istatcelldata-0.6.0/istatcelldata/data/__init__.py
+-rwxr-xr-x   0        0        0     8609 2023-05-06 17:54:29.963588 istatcelldata-0.6.0/istatcelldata/data/census_1991_2001.py
+-rwxr-xr-x   0        0        0     3148 2023-05-06 18:09:13.309829 istatcelldata-0.6.0/istatcelldata/data/manage_data.py
+-rwxr-xr-x   0        0        0     6828 2023-05-06 17:53:57.311237 istatcelldata-0.6.0/istatcelldata/download.py
+-rwxr-xr-x   0        0        0     4989 2023-05-06 15:41:41.106665 istatcelldata-0.6.0/istatcelldata/generic.py
+-rwxr-xr-x   0        0        0        0 2023-05-06 15:41:41.106955 istatcelldata-0.6.0/istatcelldata/geodata/__init__.py
+-rwxr-xr-x   0        0        0     5404 2023-05-06 15:41:41.107178 istatcelldata-0.6.0/istatcelldata/geodata/manage_geodata.py
+-rwxr-xr-x   0        0        0     4545 2023-05-06 18:09:13.319364 istatcelldata-0.6.0/istatcelldata/processes.py
+-rwxr-xr-x   0        0        0      869 2023-05-06 18:13:28.314309 istatcelldata-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1927 1970-01-01 00:00:00.000000 istatcelldata-0.6.0/PKG-INFO
```

### Comparing `istatcelldata-0.5.1/LICENSE` & `istatcelldata-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.1/README.md` & `istatcelldata-0.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # ISTAT Cell Data
 
 Con **ISTAT Cell Data** puoi ottenere facilmente il set di dati riferiti ai censimenti ISTAT in cui sono stati rilasciati anche i dati delle celle censuarie.
 
+## Installazione
+
+`pip install istatcelldata`
+
 ## Note
 Ad oggi i dati censuari ufficiali sono riferiti agli anni 1991, 2001 e 2011.
 Il 2 febbraio 2023 ISTAT ha pubblicato una [nota](https://www.istat.it/it/archivio/280254) in cui indica che i dati del censimento 2021 verranno pubblicati entro il primo semestre 2023.
 
 I dati dei censimenti della popolazione a cadenza decennale si differiscono da quelli del censimento permanente. I dati del censimento permanente sono riferiti ad un campione della popolazione italiana, mentre quelli del censimento decennale sono a carattere puntuale.
 
 Per la descrizione dei dati dal 1991 al 2011 si è fatto riferimento alla [documentazione](https://www.istat.it/it/files/2013/11/2015.04.28-Descrizione-dati-Pubblicazione.pdf) ufficiale.
```

### Comparing `istatcelldata-0.5.1/istatcelldata/config.py` & `istatcelldata-0.6.0/istatcelldata/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import logging
-from pathlib import Path
 # from multiprocessing import cpu_count
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 log_format = '%(asctime)s | %(process)d - %(message)s'
 console_handler = logging.StreamHandler()
 console_handler.setFormatter(logging.Formatter(log_format))
 logger.addHandler(console_handler)
 
 # N_CORES = cpu_count()
 
 # PROJECT
 MAIN_LINK = "https://www.istat.it/storage/cartografia"
 GLOBAL_CRS = 32632
-MAIN_PATH = Path("/home/max/Desktop/test")  # FOR TEST ONLY
 TARGET_YEARS = [1991, 2001, 2011]
 
 # PROJECT FOLDERS
 DATA_FOLDER = 'data'
 GEODATA_FOLDER = 'geodata'
 PREPROCESSING_FOLDER = 'preprocessing'
 CENSUS_DATA_FOLDER = 'Sezioni di Censimento'
```

### Comparing `istatcelldata-0.5.1/istatcelldata/data/census_1991_2001.py` & `istatcelldata-0.6.0/istatcelldata/data/census_1991_2001.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 from pathlib import Path
-from typing import Union
+from typing import Union, List
 
 import pandas as pd
 import xlrd
 from pandas import DataFrame
 from tqdm import tqdm
 
 from istatcelldata.config import logger, console_handler, PREPROCESSING_FOLDER, BOUNDARIES_DATA_FOLDER
@@ -205,22 +205,24 @@
 
 
 def merge_data_1991_2001(
         csv_path: Path,
         year: int,
         separator: str = ';',
         output_path: Path = None,
+        region_list: List = []
 ) -> Union[Path, DataFrame]:
     """Generazione di un unico file con tutti i dati censuari dell'anno selezionato.
 
     Args:
         csv_path: Path
         year: int
         separator: str
         output_path: Path
+        region_list: List
 
     Returns:
         Union[Path, DataFrame]
     """
     administrative_boundaries = csv_path.parent.parent.joinpath(BOUNDARIES_DATA_FOLDER)
 
     if year == 1991:
@@ -253,14 +255,17 @@
         left=census_data,
         right=municipality_data,
         on='pro_com'
     )
     join_data.rename(columns={'cod_com': 'codcom', 'pro_com': 'procom'}, inplace=True)
     join_data.drop(columns={'cod_pro', 'sezione'}, inplace=True)
 
+    if len(region_list) > 0:
+        join_data = join_data[join_data["codreg"].isin(region_list)]
+
     if output_path is None:
         # Pandas DataFrame to Dask DataFrame
         return join_data.from_pandas()
 
     else:
         output_data = output_path.joinpath(f'data{year}.csv')
         logging.info(f'Save data to {output_data}')
```

### Comparing `istatcelldata-0.5.1/istatcelldata/data/manage_data.py` & `istatcelldata-0.6.0/istatcelldata/data/manage_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pathlib import Path, PosixPath
-from typing import Union
+from typing import Union, List
 
 import pandas as pd
 # TODO Multithread processing with Dask #15
 # import dask.dataframe as dd
 # from dask.dataframe import DataFrame
 # from dask.distributed import Client, LocalCluster
 from pandas import DataFrame
@@ -47,23 +47,25 @@
 
 
 def merge_data(
         csv_path: Union[Path, PosixPath],
         year: int,
         separator: str = ';',
         output_path: Union[Path, PosixPath] = None,
+        region_list: List = []
 ) -> Union[Path, PosixPath, DataFrame]:
     """Unione di tutti i dati censuari per l'anno selezionato
     in un unico DataFrame.
 
     Args:
         csv_path: Union[Path, PosixPath]
         year: int
         separator: str
         output_path: Union[Path, PosixPath]
+        region_list: List
 
     Returns:
         Union[Path, PosixPath, DataFrame]
     """
     # List all csv paths
     files_path = list(csv_path.rglob("*.csv"))
 
@@ -77,14 +79,17 @@
     logging.info('Make DataFrame')
     # TODO Multithread processing with Dask #15
     # logging.info('Make Dask DataFrame')
     # ddf = dd.concat(data_list)
     ddf = pd.concat(data_list)
     ddf = ddf.sort_values(f'sez{year}')
 
+    if len(region_list) > 0:
+        ddf = ddf[ddf["codreg"].isin(region_list)]
+
     if output_path is None:
         return ddf
 
     else:
         output_data = output_path.joinpath(f'data{year}.csv')
         logging.info(f'Save data to {output_data}')
         # TODO Multithread processing with Dask #15
```

### Comparing `istatcelldata-0.5.1/istatcelldata/download.py` & `istatcelldata-0.6.0/istatcelldata/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 from pathlib import Path
+from typing import List
 
 from tqdm.auto import tqdm
 
 from istatcelldata.config import logger, console_handler, MAIN_LINK, CENSUS_DATA_FOLDER, GEODATA_FOLDER, \
     BOUNDARIES_DATA_FOLDER, PREPROCESSING_FOLDER
 from istatcelldata.data.census_1991_2001 import census_trace, remove_xls
 from istatcelldata.generic import census_folder, unzip_data, get_legacy_session
@@ -65,35 +66,40 @@
             output_path=data_folder_1991_2001,
         )
     logging.info("Download census data completed")
 
 
 def download_census_geodata(
         output_data_folder: Path,
-        year: int = 2011
+        year: int = 2011,
+        region_list: List = []
 ) -> Path:
     """Download dei geodati censuari.
 
     Args:
         output_data_folder: Path
         year: Integer. Default 2011.
+        region_list: List
 
     Returns:
         Path
     """
     # Make folder for yearly census data
     destination_folder = census_folder(output_data_folder=output_data_folder, year=year)
     Path(destination_folder).mkdir(parents=True, exist_ok=True)
 
     # Make data folder
     data_folder = destination_folder.joinpath(GEODATA_FOLDER)
     Path(data_folder).mkdir(parents=True, exist_ok=True)
 
     year_folder = str(year)[2:]
-    regions = tqdm(range(1, 21, 1))
+    if len(region_list) == 0:
+        regions = tqdm(range(1, 21, 1))
+    else:
+        regions = region_list
 
     logging.info("Download census geodata")
     for region in regions:
         region = str(region).zfill(2)
         data_link = f"{MAIN_LINK}/basi_territoriali/WGS_84_UTM/{year}/R{region}_{year_folder}_WGS84.zip"
 
         data_file_name = data_link.split('/')[-1]
@@ -142,34 +148,38 @@
         destination_folder=destination_folder
     )
     logging.info("Download administrative boundaries completed")
 
 
 def download_all_census_data(
         output_data_folder: Path,
-        year: int = 2011
+        year: int = 2011,
+        region_list: List = []
 ) -> None:
-    """Download di tutti i dati censuari per l'anno selezionato.
+    """Download di tutti i dati censuari per l'anno selezionato. E' possibile
+    effettuare il download per singola Regione ma anche per specifiche Regioni.
+    Quando il campo `region_list` resta vuoto vengono scaricati i dati di tutte le Regioni.
 
     Args:
         output_data_folder: Path
         year: int
+        region_list: List
     """
     # Make data folder
     data_folder = output_data_folder.joinpath(PREPROCESSING_FOLDER)
     Path(data_folder).mkdir(parents=True, exist_ok=True)
 
     # Download data
     download_census_data(
         output_data_folder=data_folder, year=year
     )
 
     # Download geodata
     download_census_geodata(
-        output_data_folder=data_folder, year=year
+        output_data_folder=data_folder, year=year, region_list=region_list
     )
 
     # Download administrative boundaries
     download_administrative_boundaries(
         output_data_folder=data_folder, year=year
     )
 
@@ -186,34 +196,32 @@
         data_link: Path
         data_file_path_destination: Path
         data_folder: Path
         destination_folder: Path
 
     Returns:
         Path
+
+    Raises:
+        Link {data_link} return status code {data.status_code}.
     """
-    try:
-        # Download data
-        logging.info(f"Download census data | {data_link}")
-        data = get_legacy_session().get(data_link)
-
-        if data.status_code == 200:
-            data_size = int(data.headers.get('Content-Length'))
-            # Progress bar via tqdm
-            with tqdm.wrapattr(data.raw, "read", total=data_size, desc="Downloading..."):
-                open(data_file_path_destination, 'wb').write(data.content)
-            logging.info("Download completed")
-        else:
-            raise Exception(f'Link {data_link} return status code {data.status_code}.')
-
-        logging.info("Unzip file")
-        unzip_data(data_file_path_destination, data_folder)
-
-        logging.info(f"Deleting zip file | {data_file_path_destination}")
-        os.remove(data_file_path_destination)
-        logging.info("File deleted")
-
-        return destination_folder
-
-    except:
-        logging.info("Something went wrong!!!")
-        #logging.info(f'Link {data_link} return status code {data.status_code}.')
+    # Download data
+    logging.info(f"Download census data | {data_link}")
+    data = get_legacy_session().get(data_link)
+
+    if data.status_code == 200:
+        data_size = int(data.headers.get('Content-Length'))
+        # Progress bar via tqdm
+        with tqdm.wrapattr(data.raw, "read", total=data_size, desc="Downloading..."):
+            open(data_file_path_destination, 'wb').write(data.content)
+        logging.info("Download completed")
+    else:
+        raise Exception(f'Link {data_link} return status code {data.status_code}.')
+
+    logging.info("Unzip file")
+    unzip_data(data_file_path_destination, data_folder)
+
+    logging.info(f"Deleting zip file | {data_file_path_destination}")
+    os.remove(data_file_path_destination)
+    logging.info("File deleted")
+
+    return destination_folder
```

### Comparing `istatcelldata-0.5.1/istatcelldata/generic.py` & `istatcelldata-0.6.0/istatcelldata/generic.py`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.1/istatcelldata/geodata/manage_geodata.py` & `istatcelldata-0.6.0/istatcelldata/geodata/manage_geodata.py`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.1/pyproject.toml` & `istatcelldata-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "istatcelldata"
-version = "0.5.1"
+version = "0.6.0"
 description = "\"Con ISTAT Cell Data puoi ottenere facilmente il set di dati riferiti ai censimenti ISTAT in cui sono stati rilasciati anche i dati delle celle censuarie.\""
 authors = ["Massimiliano Moraca <info@massimilianomoraca.it>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `istatcelldata-0.5.1/PKG-INFO` & `istatcelldata-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istatcelldata
-Version: 0.5.1
+Version: 0.6.0
 Summary: "Con ISTAT Cell Data puoi ottenere facilmente il set di dati riferiti ai censimenti ISTAT in cui sono stati rilasciati anche i dati delle celle censuarie."
 License: MIT
 Author: Massimiliano Moraca
 Author-email: info@massimilianomoraca.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,18 @@
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ISTAT Cell Data
 
 Con **ISTAT Cell Data** puoi ottenere facilmente il set di dati riferiti ai censimenti ISTAT in cui sono stati rilasciati anche i dati delle celle censuarie.
 
+## Installazione
+
+`pip install istatcelldata`
+
 ## Note
 Ad oggi i dati censuari ufficiali sono riferiti agli anni 1991, 2001 e 2011.
 Il 2 febbraio 2023 ISTAT ha pubblicato una [nota](https://www.istat.it/it/archivio/280254) in cui indica che i dati del censimento 2021 verranno pubblicati entro il primo semestre 2023.
 
 I dati dei censimenti della popolazione a cadenza decennale si differiscono da quelli del censimento permanente. I dati del censimento permanente sono riferiti ad un campione della popolazione italiana, mentre quelli del censimento decennale sono a carattere puntuale.
 
 Per la descrizione dei dati dal 1991 al 2011 si è fatto riferimento alla [documentazione](https://www.istat.it/it/files/2013/11/2015.04.28-Descrizione-dati-Pubblicazione.pdf) ufficiale.
```

