# Comparing `tmp/ng_data_pipelines_sdk-0.6.0.tar.gz` & `tmp/ng_data_pipelines_sdk-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.6.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.6.2.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.6.0.tar` & `ng_data_pipelines_sdk-0.6.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-02 22:26:22.376910 ng_data_pipelines_sdk-0.6.0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 22:26:22.401909 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    27485 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    15573 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5093 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     1453 2024-05-02 22:26:22.377910 ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      672 2024-05-02 22:26:22.378910 ng_data_pipelines_sdk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-14 17:47:38.473033 ng_data_pipelines_sdk-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 17:47:38.506033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-14 17:47:38.473033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-14 17:47:38.473033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    27137 2024-05-14 17:47:38.474033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    15575 2024-05-14 17:47:38.474033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5093 2024-05-14 17:47:38.474033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     1453 2024-05-14 17:47:38.474033 ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      695 2024-05-14 17:47:38.477033 ng_data_pipelines_sdk-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.6.2/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from pyspark.sql.functions import lit
 from pyspark.sql.types import StructType
 
 from ng_data_pipelines_sdk.aws_interface import AWSInterface
 from ng_data_pipelines_sdk.interfaces import (
     DATE_FORMATTER,
     DataFrameReadWriteParams,
-    DatePartition,
     FileType,
     FnKind,
     InputDataFrameParams,
     InputDataFrameParamsDict,
     OutputDataFrameParams,
     OutputDataFrameParamsDict,
     S3BucketParams,
@@ -251,26 +250,14 @@
                 object_data=pyspark_schema_json,
             )
         except Exception as e:
             raise ValueError(
                 f"Error writing schema to {bucket_name}/{path_to_schema}: {e}"
             )
 
-    def _add_date_partitions_columns(
-        self, df: DataFrame, date_partitions: DatePartition
-    ) -> DataFrame:
-        for date_part, value in date_partitions:
-            if value is not None:
-                df = df.withColumn(
-                    date_part,
-                    lit(DATE_FORMATTER[date_part](value)),
-                )
-
-        return df
-
     def _get_partitions(self, write_params: DataFrameReadWriteParams) -> List[str]:
         date_partition_columns: List[str] = []
         if write_params.processing_date_partitions:
             for date_partition in write_params.processing_date_partitions:
                 date_partition_columns.append(date_partition.value)
 
         # Choose the order of adding partitions based on the `date_partition_first` flag
@@ -332,15 +319,17 @@
         bucket_url = self._get_bucket_url(write_params.bucket_params)
         write_path_url = f"{bucket_url}/{write_params.path_to_dataframe_root}"
         logger.debug(f"Write root path: {write_path_url}")
 
         partitions = self._get_partitions(write_params)
         logger.debug(f"Using partitions: {partitions}")
 
-        path = f"{bucket_url}/{self._get_dataframe_path_with_date_partitions(write_params)}"
+
+        path = f"{self._get_dataframe_path_with_date_partitions(write_params)}"
+        full_path = f"{bucket_url}/{path}"
 
         # Add the date partitions columns to the DataFrame
         df_with_date_partitions = df
         if write_params.processing_date_partitions:
             for date_partition in write_params.processing_date_partitions:
                 formatted_date_part_value = DATE_FORMATTER[
                     date_partition.value.replace("part_", "")
@@ -348,15 +337,15 @@
 
                 df_with_date_partitions = df_with_date_partitions.withColumn(
                     date_partition.value, lit(formatted_date_part_value)
                 )
 
         if df_params.overwrite:
             logger.info(
-                f"Overwrite is set to True. Deleting existing objects under path {path}"
+                f"Overwrite is set to True. Deleting existing objects under path {full_path}"
             )
             try:
                 self.aws_interface.delete_objects_aws(
                     write_params.bucket_params.env,
                     write_params.bucket_params.bucket_name,
                     path,
                 )
```

### Comparing `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,15 @@
         path_to_dataframe_root (Optional[str]): The path to the root folder of the DataFrame within the bucket.
         file_type (FileType): The type of file to read or write.
         processing_date (Union[List[datetime], datetime, Literal["{{processing_date}}"], Literal["{{processing_date_previous}}"]]): The processing date or dates to use for partitioning.
         processing_date_partitions (Optional[List[DatePartition]]): The list of date partitions to use for filtering.
         processing_date_partitions_first (bool): Flag indicating whether to process date partitions first.
         column_partitions (Optional[List[str]]): The list of column partitions to use for filtering.
     """
+
     bucket_params: S3BucketParams
     specific_path: Optional[Union[List[str], str]] = None
     path_to_dataframe_root: Optional[str] = None
     file_type: FileType
     processing_date: Union[
         List[datetime],
         datetime,
@@ -262,15 +263,15 @@
             v (str): The input string.
 
         Returns:
             str: The input string with leading and trailing slashes stripped.
         """
         if v is not None:
             if isinstance(v, list):
-                return [x.strip("/") for x in v] # type: ignore
+                return [x.strip("/") for x in v]  # type: ignore
             else:
                 return v.strip("/")
 
     @field_validator("path_to_dataframe_root")
     def ensure_dataframe_root_parent_folder(cls, v: str) -> str:
         """
         Ensures that 'path_to_dataframe_root' has at least one parent folder inside the bucket.
```

### Comparing `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.6.0/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.6.2/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.6.0/pyproject.toml` & `ng_data_pipelines_sdk-0.6.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.6.0"
+version = "0.6.2"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pyspark = "^3.2.0"
 pydantic = "^2.5.3"
 boto3 = "^1.33.13"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 ruff = "^0.3.7"
+load-dotenv = "^0.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ng_data_pipelines_sdk-0.6.0/PKG-INFO` & `ng_data_pipelines_sdk-0.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.6.0
+Version: 0.6.2
 Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

