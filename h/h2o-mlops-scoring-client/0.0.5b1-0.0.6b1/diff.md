# Comparing `tmp/h2o_mlops_scoring_client-0.0.5b1-py3-none-any.whl.zip` & `tmp/h2o_mlops_scoring_client-0.0.6b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 7357 bytes, number of entries: 6
--rw-r--r--  2.0 unx     8725 b- defN 23-Apr-15 02:34 h2o_mlops_scoring_client/__init__.py
--rw-r--r--  2.0 unx    11796 b- defN 23-Apr-15 02:35 h2o_mlops_scoring_client/_utils.py
--rw-r--r--  2.0 unx     2330 b- defN 23-Apr-15 03:47 h2o_mlops_scoring_client-0.0.5b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 03:47 h2o_mlops_scoring_client-0.0.5b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-15 03:47 h2o_mlops_scoring_client-0.0.5b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      559 b- defN 23-Apr-15 03:47 h2o_mlops_scoring_client-0.0.5b1.dist-info/RECORD
-6 files, 23527 bytes uncompressed, 6331 bytes compressed:  73.1%
+Zip file size: 8448 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        8 b- defN 23-May-06 00:00 h2o_mlops_scoring_client/VERSION
+-rw-r--r--  2.0 unx     9746 b- defN 23-May-05 23:26 h2o_mlops_scoring_client/__init__.py
+-rw-r--r--  2.0 unx    12413 b- defN 23-May-05 23:26 h2o_mlops_scoring_client/_utils.py
+-rw-r--r--  2.0 unx      228 b- defN 23-May-05 23:26 h2o_mlops_scoring_client/_version.py
+-rw-r--r--  2.0 unx     2993 b- defN 23-May-06 00:00 h2o_mlops_scoring_client-0.0.6b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 00:00 h2o_mlops_scoring_client-0.0.6b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-May-06 00:00 h2o_mlops_scoring_client-0.0.6b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      737 b- defN 23-May-06 00:00 h2o_mlops_scoring_client-0.0.6b1.dist-info/RECORD
+8 files, 26242 bytes uncompressed, 7134 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
+Filename: h2o_mlops_scoring_client/VERSION
+Comment: 
+
 Filename: h2o_mlops_scoring_client/__init__.py
 Comment: 
 
 Filename: h2o_mlops_scoring_client/_utils.py
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.5b1.dist-info/METADATA
+Filename: h2o_mlops_scoring_client/_version.py
+Comment: 
+
+Filename: h2o_mlops_scoring_client-0.0.6b1.dist-info/METADATA
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.5b1.dist-info/WHEEL
+Filename: h2o_mlops_scoring_client-0.0.6b1.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.5b1.dist-info/top_level.txt
+Filename: h2o_mlops_scoring_client-0.0.6b1.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.5b1.dist-info/RECORD
+Filename: h2o_mlops_scoring_client-0.0.6b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_mlops_scoring_client/__init__.py

```diff
@@ -4,62 +4,75 @@
 import typing as _typing
 
 import pandas as _pandas
 
 from h2o_mlops_scoring_client import _utils
 from h2o_mlops_scoring_client._utils import Format
 from h2o_mlops_scoring_client._utils import WriteMode
+from h2o_mlops_scoring_client._version import version as __version__  # noqa: F401
 
 
 _logging.basicConfig(
     format="%(asctime)s %(levelname)s %(name)s: %(message)s",
     datefmt="%y/%m/%d %H:%M:%S",
     level=_logging.INFO,
 )
 logger = _logging.getLogger(__name__)
 spark_conf_dir = _os.environ.get("SPARK_CONF_DIR")
 spark_master = _os.environ.get("MASTER", "local[*]")
+if spark_master.startswith("local"):
+    _os.environ.pop("SPARK_HOME", None)
 
 
-def get_capabilities(mlops_endpoint_url: str) -> _typing.List[str]:
+def get_capabilities(
+    mlops_endpoint_url: str, passphrase: _typing.Optional[str] = None
+) -> _typing.List[str]:
     """Capabilities of the scoring endpoint.
 
     Args:
         mlops_endpoint_url: MLOps deployment scoring endpoint URL
+        passphrase: passphrase for protected MLOps endpoint
     """
-    return _utils.MLOpsEndpoint(mlops_endpoint_url).capabilities
+    return _utils.MLOpsEndpoint(mlops_endpoint_url, passphrase).capabilities
 
 
-def get_experiment_id(mlops_endpoint_url: str) -> str:
+def get_experiment_id(
+    mlops_endpoint_url: str, passphrase: _typing.Optional[str] = None
+) -> str:
     """ID of experiment used for scoring by the scoring endpoint.
 
     Args:
         mlops_endpoint_url: MLOps deployment scoring endpoint URL
+        passphrase: passphrase for protected MLOps endpoint
     """
-    return _utils.MLOpsEndpoint(mlops_endpoint_url).experiment_id
+    return _utils.MLOpsEndpoint(mlops_endpoint_url, passphrase).experiment_id
 
 
-def get_schema(mlops_endpoint_url: str) -> _typing.Dict[str, _typing.Any]:
+def get_schema(
+    mlops_endpoint_url: str, passphrase: _typing.Optional[str] = None
+) -> _typing.Dict[str, _typing.Any]:
     """Column names and types expected by the scoring endpoint.
 
     Args:
         mlops_endpoint_url: MLOps deployment scoring endpoint URL
+        passphrase: passphrase for protected MLOps endpoints
     """
-    return _utils.MLOpsEndpoint(mlops_endpoint_url).schema
+    return _utils.MLOpsEndpoint(mlops_endpoint_url, passphrase).schema
 
 
 def score_source_sink(
     *,
     mlops_endpoint_url: str,
     id_column: str,
     source_data: str,
     source_format: Format,
     sink_location: str,
     sink_format: Format,
     sink_write_mode: WriteMode,
+    passphrase: _typing.Optional[str] = None,
     source_config: _typing.Optional[_typing.Dict[str, str]] = None,
     sink_config: _typing.Optional[_typing.Dict[str, str]] = None,
     preprocess_method: _typing.Optional[_typing.Callable] = None,
     postprocess_method: _typing.Optional[_typing.Callable] = None,
     mini_batch_size: int = 1000,
     spark_config_overrides: _typing.Optional[_typing.Dict[str, str]] = None,
 ) -> None:
@@ -70,14 +83,15 @@
         id_column: name of column in data to be scored
             - column should contain unique row identifiers
         source_data: path or query for data to be scored
         source_format: file type or table type data to be scored is stored in
         sink_location: path or query for scored data to be written to
         sink_format: file type or table type for scored data when written
         sink_write_mode: write behavior when data already exists in sink location
+        passphrase: passphrase for protected MLOps endpoint
         source_config: pass Spark data source options for the specified format
             (useful for JDBC_QUERY and JDBC_TABLE formats)
         sink_config: pass Spark data source options for the specified format
             (useful for JDBC_QUERY and JDBC_TABLE formats)
         preprocess_method: method that takes and returns a Spark dataframe
             before scoring
         postprocess_method: method that takes and returns a Spark dataframe
@@ -85,26 +99,27 @@
         mini_batch_size: number of rows per scorer call
         spark_config_overrides: pass Spark configuration options to the Spark context
     """
     try:
         start = _datetime.datetime.now().replace(microsecond=0)
 
         if spark_conf_dir:
+            _utils.preflight(spark_conf_dir)
             _os.environ["SPARK_CONF_DIR"] = _os.path.abspath(spark_conf_dir)
 
         logger.info("Starting Spark context")
         spark = _utils.get_spark_session(
             app_name="h2o_mlops_scoring_client",
             master=spark_master,
             mini_batch_size=mini_batch_size,
             spark_config=spark_config_overrides,
         )
 
         logger.info(f"Connecting to H2O.ai MLOps scorer at '{mlops_endpoint_url}'")
-        mlops_endpoint = _utils.MLOpsEndpoint(mlops_endpoint_url)
+        mlops_endpoint = _utils.MLOpsEndpoint(mlops_endpoint_url, passphrase)
 
         sdf = _utils.read_source(spark, source_data, source_format, source_config)
 
         if preprocess_method:
             logger.info("Applying preprocess method")
             sdf = preprocess_method(sdf)
 
@@ -137,53 +152,58 @@
 
 def score_data_frame(
     *,
     mlops_endpoint_url: str,
     id_column: str,
     data_frame: _pandas.DataFrame,
     mini_batch_size: int = 1000,
+    passphrase: _typing.Optional[str] = None,
     spark_config_overrides: _typing.Optional[_typing.Dict[str, str]] = None,
 ) -> _pandas.DataFrame:
     """Do scoring of a data frame against a MLOps deployment. Parallelized mini-batch
     scoring with Spark is done if the data frame row count is more than mini_batch_size.
 
     Args:
         mlops_endpoint_url: MLOps deployment scoring endpoint URL
         id_column: name of column in data to be scored
             - column should contain unique row identifiers
         data_frame: Pandas DataFrame
         mini_batch_size: number of rows per scorer call
+        passphrase: passphrase for protected MLOps endpoint
         spark_config_overrides: pass Spark configuration options to the Spark context
     """
     if data_frame.shape[0] > mini_batch_size:
         return _score_data_frame_spark(
             mlops_endpoint_url=mlops_endpoint_url,
+            passphrase=passphrase,
             id_column=id_column,
             data_frame=data_frame,
             mini_batch_size=mini_batch_size,
             spark_config_overrides=spark_config_overrides,
         )
     else:
         return _score_data_frame_direct(
             mlops_endpoint_url=mlops_endpoint_url,
+            passphrase=passphrase,
             id_column=id_column,
             data_frame=data_frame,
         )
 
 
 def _score_data_frame_direct(
     *,
     mlops_endpoint_url: str,
     id_column: str,
     data_frame: _pandas.DataFrame,
+    passphrase: _typing.Optional[str] = None,
 ) -> _pandas.DataFrame:
     start = _datetime.datetime.now().replace(microsecond=0)
 
     logger.info(f"Connecting to H2O.ai MLOps scorer at '{mlops_endpoint_url}'")
-    mlops_endpoint = _utils.MLOpsEndpoint(mlops_endpoint_url)
+    mlops_endpoint = _utils.MLOpsEndpoint(mlops_endpoint_url, passphrase)
 
     logger.info("Starting scoring data frame")
     start_scoring = _datetime.datetime.now().replace(microsecond=0)
     scored_df = mlops_endpoint.score_pandas_dataframe(data_frame, id_column=id_column)
 
     logger.info("Scoring complete")
     stop = _datetime.datetime.now().replace(microsecond=0)
@@ -196,32 +216,34 @@
 
 def _score_data_frame_spark(
     *,
     mlops_endpoint_url: str,
     id_column: str,
     data_frame: _pandas.DataFrame,
     mini_batch_size: int = 1000,
+    passphrase: _typing.Optional[str] = None,
     spark_config_overrides: _typing.Optional[_typing.Dict[str, str]] = None,
 ) -> _pandas.DataFrame:
     try:
         start = _datetime.datetime.now().replace(microsecond=0)
 
         if spark_conf_dir:
+            _utils.preflight(spark_conf_dir)
             _os.environ["SPARK_CONF_DIR"] = _os.path.abspath(spark_conf_dir)
 
         logger.info("Starting Spark context")
         spark = _utils.get_spark_session(
             app_name="h2o_mlops_scoring_client",
             master=spark_master,
             mini_batch_size=mini_batch_size,
             spark_config=spark_config_overrides,
         )
 
         logger.info(f"Connecting to H2O.ai MLOps scorer at '{mlops_endpoint_url}'")
-        mlops_endpoint = _utils.MLOpsEndpoint(mlops_endpoint_url)
+        mlops_endpoint = _utils.MLOpsEndpoint(mlops_endpoint_url, passphrase)
 
         sdf = spark.createDataFrame(data_frame)
 
         logger.info("Starting scoring data frame")
         start_scoring = _datetime.datetime.now().replace(microsecond=0)
         scored_sdf = mlops_endpoint.score_spark_dataframe(sdf, id_column=id_column)
         scored_df = scored_sdf.toPandas()
```

## h2o_mlops_scoring_client/_utils.py

```diff
@@ -1,9 +1,10 @@
 import copy as _copy
 import enum as _enum
+import pathlib as _pathlib
 from typing import Any as _Any
 from typing import Dict as _Dict
 from typing import Iterator as _Iterator
 from typing import List as _List
 from typing import Optional as _Optional
 
 import pandas as _pandas
@@ -54,15 +55,15 @@
 
 
 class MLOpsEndpoint:
     """Python wrapper giving convenient access to H2O.ai MLOps endpoint
     information and scoring.
     """
 
-    def __init__(self, url: str):
+    def __init__(self, url: str, passphrase: _Optional[str] = None):
         url = url.rstrip("/")
         if url.endswith("model"):
             self._endpoint_parent_url = url
         else:
             self._endpoint_parent_url = "/".join(url.split("/")[:-1])
         self._capabilities_url = f"{self._endpoint_parent_url}/capabilities"
         self._experiment_id_url = f"{self._endpoint_parent_url}/id"
@@ -80,25 +81,29 @@
             backoff_factor=0.1,
             status_forcelist=[403, 404],
         )
         adapter = _HTTPAdapter(max_retries=session_retry)
         self._session = _requests.Session()
         self._session.mount("http://", adapter)
         self._session.mount("https://", adapter)
+        if passphrase is not None:
+            self._session.headers = {"Authorization": f"Bearer {passphrase}"}
 
         # for post to score url
         session_retry = _Retry(
             total=10,
             status_forcelist=[404, 500, 502, 503, 504],
             backoff_factor=0.2,
             allowed_methods=["POST"],
         )
         adapter = _HTTPAdapter(max_retries=session_retry)
         self._score_session = _requests.Session()
         self._score_session.mount(self.score_url, adapter)
+        if passphrase is not None:
+            self._score_session.headers = {"Authorization": f"Bearer {passphrase}"}
 
         self._spark_type_map = {
             "bool": _pyspark_sql_types.BooleanType(),
             "int32": _pyspark_sql_types.IntegerType(),
             "int64": _pyspark_sql_types.LongType(),
             "float32": _pyspark_sql_types.FloatType(),
             "float64": _pyspark_sql_types.DoubleType(),
@@ -273,14 +278,23 @@
     conf.set("spark.sql.execution.arrow.pyspark.enabled", "true")
     conf.set("spark.sql.execution.arrow.maxRecordsPerBatch", str(mini_batch_size))
     conf.setAll([(k, str(v)) for k, v in spark_config.items()])
     spark = _pyspark_sql.SparkSession.builder.config(conf=conf).getOrCreate()
     return spark
 
 
+def preflight(spark_conf_dir: str) -> None:
+    spark_defaults_conf = "spark-defaults.conf"
+    if not _pathlib.Path(spark_conf_dir, spark_defaults_conf).is_file():
+        raise RuntimeError(
+            f"SPARK_CONF_DIR is set to '{spark_conf_dir}' "
+            f"but '{spark_defaults_conf}' was not found."
+        )
+
+
 def read_source(
     spark: _pyspark_sql.SparkSession,
     source_data: str,
     source_format: Format,
     source_config: _Optional[_Dict[str, str]] = None,
 ) -> _pyspark_sql.DataFrame:
     _source_config = _copy.copy(_format_config[source_format])
```

## Comparing `h2o_mlops_scoring_client-0.0.5b1.dist-info/METADATA` & `h2o_mlops_scoring_client-0.0.6b1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: h2o-mlops-scoring-client
-Version: 0.0.5b1
+Version: 0.0.6b1
 Summary: A Python client library to simplify robust mini-batch scoring against an H2O MLOps scoring endpoint.
 Author: H2O.ai
 Author-email: support@h2o.ai
 License: Proprietary License
+Project-URL: Documentation, https://docs.h2o.ai/mlops/mlops-scoring-client/overview
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Requires-Dist: pandas (<2,>=1.0.5)
 Requires-Dist: pyarrow (>=1)
 Requires-Dist: pyspark (<4,>=3)
 Requires-Dist: requests (<3,>=2)
+Requires-Dist: urllib3 (>=1.26)
 
 # H2O MLOps Scoring Client
 
 A Python client library to simplify robust mini-batch scoring against an H2O MLOps scoring endpoint. It can run on your local PC, a stand alone server, Databricks, or a Spark 3 cluster.
 
 Using it is as easy as:
 
@@ -46,29 +48,53 @@
 
 ### Requirements
 
 - Linux or Mac OS (Windows is not supported)
 - Java
 - Python 3.8 or greater
 
-### 
-
 ### Install from PyPI
 
 ```
 pip install h2o_mlops_scoring_client
 ```
 
-
 ## FAQ
 
 ### When should I use the MLOps Scoring Client?
 
 Use when batch scoring processing (authenticating and connecting to source or sink, file/data processing or conversions, etc.) can happen external to H2O AI Cloud but you want to stay within the H2O MLOps workflow (projects, scoring, registry, monitoring, etc.).
 
+### Where does scoring take place?
+
+As the batch scoring processing occurs, the data is sent to an H2O MLOps deployment for scoring. The scores are then returned for the batch scoring processing to complete.
+
+### What Source/Sinks are supported?
+
+The MLOps scoring client can support many source/sinks, including:
+
+- ADLS Gen 2
+- Databases with a JDBC driver
+- Local file system
+- GBQ
+- S3
+
 ### What file types are supported?
 
-The MLOps scoring client can read and write CSV, Parquet, ORC, BigQuery Tables, JDBC Tables, and JDBC queries. If there's a file type you would like to see supported, please let us know.
+The MLOps scoring client can read and write:
+
+- CSV
+- Parquet
+- ORC
+- BigQuery tables
+- JDBC tables
+- JDBC queries
+
+If there's a file type you would like to see supported, please let us know.
+
+### I want model monitoring for batch scoring, can I do that?
+
+Yes. The MLOps Scoring Client uses MLOps scoring endpoints which are automatically monitored.
 
 ### Is a Spark installation required?
 
 No. If you're running locally and scoring local files or data frames, then no extra Spark install or configuration is needed. If you want to connect to an external source or sink, you'll need to do a small amount of configuration.
```

## Comparing `h2o_mlops_scoring_client-0.0.5b1.dist-info/RECORD` & `h2o_mlops_scoring_client-0.0.6b1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,6 +1,8 @@
-h2o_mlops_scoring_client/__init__.py,sha256=I36cotxAWRG9YCIBYi45NbtzuXoqbQ-8hkiKBMsW0Is,8725
-h2o_mlops_scoring_client/_utils.py,sha256=EMeFvAO-lTIXzZoGfGJM_71BKqArbBro7jSVxDYQLgQ,11796
-h2o_mlops_scoring_client-0.0.5b1.dist-info/METADATA,sha256=yaSf1Jd9UPrLCJuVJt95CO76LLiExO79GlsW_25vI10,2330
-h2o_mlops_scoring_client-0.0.5b1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-h2o_mlops_scoring_client-0.0.5b1.dist-info/top_level.txt,sha256=QqsGjPwyloWBgEOjck-e-Bdmk2YW_AaAcX7YWz40UKg,25
-h2o_mlops_scoring_client-0.0.5b1.dist-info/RECORD,,
+h2o_mlops_scoring_client/VERSION,sha256=RanFHF0QS6lWeWp168HpEmwMRRP1VJ03SHTidWfhXH8,8
+h2o_mlops_scoring_client/__init__.py,sha256=Oo_QZvQp4sz6Pmp24viyAu3fk8Bab2jrJ9uG4Bk8aiI,9746
+h2o_mlops_scoring_client/_utils.py,sha256=IW8EULX4my42Knqoon062ehs3x49PqhlaTXT1O3nAl0,12413
+h2o_mlops_scoring_client/_version.py,sha256=1zDsuRRqsnIsxWZY4--3dDuaB3D82cfPyw541E-uOic,228
+h2o_mlops_scoring_client-0.0.6b1.dist-info/METADATA,sha256=Tz0KDbjOZORjoLXKM2xGV0ew0zklF3IevTCiGUijbnQ,2993
+h2o_mlops_scoring_client-0.0.6b1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+h2o_mlops_scoring_client-0.0.6b1.dist-info/top_level.txt,sha256=QqsGjPwyloWBgEOjck-e-Bdmk2YW_AaAcX7YWz40UKg,25
+h2o_mlops_scoring_client-0.0.6b1.dist-info/RECORD,,
```

