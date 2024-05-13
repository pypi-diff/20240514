# Comparing `tmp/apache_airflow_providers_anomalo-0.2.0.tar.gz` & `tmp/apache_airflow_providers_anomalo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_anomalo-0.2.0.tar", max compression
+gzip compressed data, was "apache_airflow_providers_anomalo-0.2.1.tar", max compression
```

## Comparing `apache_airflow_providers_anomalo-0.2.0.tar` & `apache_airflow_providers_anomalo-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11358 2023-12-07 00:17:41.516792 apache_airflow_providers_anomalo-0.2.0/LICENSE
--rw-r--r--   0        0        0     1921 2024-02-06 22:29:10.031729 apache_airflow_providers_anomalo-0.2.0/README.md
--rw-r--r--   0        0        0     1398 2024-02-06 22:29:10.032077 apache_airflow_providers_anomalo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      442 2023-12-07 00:17:41.519965 apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/__init__.py
--rw-r--r--   0        0        0        0 2023-12-07 00:17:41.520059 apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/example_dags/__init__.py
--rw-r--r--   0        0        0     1537 2024-01-31 21:36:10.457948 apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/example_dags/example_anomalo.py
--rw-r--r--   0        0        0        0 2023-12-07 00:17:41.520243 apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/hooks/__init__.py
--rw-r--r--   0        0        0     1551 2024-01-31 21:36:10.458210 apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/hooks/anomalo.py
--rw-r--r--   0        0        0        0 2023-12-07 00:17:41.520434 apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/operators/__init__.py
--rw-r--r--   0        0        0     5088 2024-02-06 22:28:11.309323 apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/operators/anomalo.py
--rw-r--r--   0        0        0        0 2023-12-07 00:17:41.520610 apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/sensors/__init__.py
--rw-r--r--   0        0        0     1961 2024-02-06 22:28:11.309502 apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/sensors/anomalo.py
--rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 apache_airflow_providers_anomalo-0.2.0/setup.py
--rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 apache_airflow_providers_anomalo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-12-07 00:17:41.516792 apache_airflow_providers_anomalo-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1921 2024-05-13 16:33:49.259199 apache_airflow_providers_anomalo-0.2.1/README.md
+-rw-r--r--   0        0        0     1398 2024-05-13 18:14:27.915069 apache_airflow_providers_anomalo-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      442 2023-12-07 00:17:41.519965 apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-07 00:17:41.520059 apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/example_dags/__init__.py
+-rw-r--r--   0        0        0     1584 2024-05-13 16:36:26.099593 apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/example_dags/example_anomalo.py
+-rw-r--r--   0        0        0        0 2023-12-07 00:17:41.520243 apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/hooks/__init__.py
+-rw-r--r--   0        0        0     1551 2024-01-31 21:36:10.458210 apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/hooks/anomalo.py
+-rw-r--r--   0        0        0        0 2023-12-07 00:17:41.520434 apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/operators/__init__.py
+-rw-r--r--   0        0        0     7193 2024-05-13 16:36:26.099832 apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/operators/anomalo.py
+-rw-r--r--   0        0        0        0 2023-12-07 00:17:41.520610 apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/sensors/__init__.py
+-rw-r--r--   0        0        0     1961 2024-02-06 22:28:11.309502 apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/sensors/anomalo.py
+-rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 apache_airflow_providers_anomalo-0.2.1/setup.py
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 apache_airflow_providers_anomalo-0.2.1/PKG-INFO
```

### Comparing `apache_airflow_providers_anomalo-0.2.0/LICENSE` & `apache_airflow_providers_anomalo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_anomalo-0.2.0/README.md` & `apache_airflow_providers_anomalo-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_anomalo-0.2.0/pyproject.toml` & `apache_airflow_providers_anomalo-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 requires-python = ">=3.8"
 
 [tool.poetry]
 name = "apache-airflow-providers-anomalo"
-version = "0.2.0"
+version = "0.2.1"
 description = "An Apache Airflow provider for Anomalo"
 license = "Apache-2.0"
 authors = ["Anomalo <opensource@anomalo.com>"]
 readme = "README.md"
 repository = "https://github.com/anomalo-hq/anomalo-airflow-provider"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/example_dags/example_anomalo.py` & `apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/example_dags/example_anomalo.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,30 +17,33 @@
     dag_id="AnomaloDAG",
     default_args=args,
     description="Simple Anomalo Airflow operator example",
     schedule_interval="@daily",
 ) as dag:
     ingest_transform_data = EmptyOperator(task_id="ingest_transform_data")
 
+    my_table_name = "public-bq.austin_bikeshare.bikeshare_stations"
+
     anomalo_run = AnomaloRunCheckOperator(
         task_id="AnomaloRunCheck",
-        table_name="public-bq.austin_bikeshare.bikeshare_stations",
+        table_name=my_table_name,
     )
 
     anomalo_sensor = AnomaloJobCompleteSensor(
         task_id="AnomaloJobCompleteSensor",
         xcom_job_id_task=anomalo_run.task_id,
         poke_interval=60,
         timeout=900,  # 15 minutes
         mode="poke",
     )
 
     anomalo_validate = AnomaloPassFailOperator(
         task_id="AnomaloPassFail",
-        table_name="public-bq.austin_bikeshare.bikeshare_stations",
+        table_name=my_table_name,
+        xcom_job_id_task=anomalo_run.task_id,
         must_pass=[
             "data_freshness",
             "data_volume",
             "metric",
             "rule",
             "missing_data",
             "anomaly",
```

### Comparing `apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/hooks/anomalo.py` & `apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/hooks/anomalo.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_anomalo-0.2.0/src/airflow/providers/anomalo/sensors/anomalo.py` & `apache_airflow_providers_anomalo-0.2.1/src/airflow/providers/anomalo/sensors/anomalo.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_anomalo-0.2.0/setup.py` & `apache_airflow_providers_anomalo-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'apache_airflow_provider': ['provider_info = '
                              'airflow.providers.anomalo.__init__:get_provider_info']}
 
 setup_kwargs = {
     'name': 'apache-airflow-providers-anomalo',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'An Apache Airflow provider for Anomalo',
     'long_description': '# Apache Airflow Provider for Anomalo\nA set of native Airflow operators for [Anomalo](https://www.anomalo.com/)\n\n### Compatibility\nThese operators were created and tested with\n* Python 3.8-3.10\n* Airflow 2.3+\n* Anomalo python client 0.0.7\n\n### Installation\n\n\n```\npip install apache-airflow-providers-anomalo\n```\nYou can validate that it is correctly installed by running `airflow providers list` on the command line and seeing if `apache-airflow-providers-anomalo` is a listed providers package.\n\n### Airflow Setup\n\nFrom the airflow UI, go to Admin > Connections and hit the `+` button at the top to add a new connection.\n\nFrom the "Connection Type" drop down, select "Anomalo".\n![connection](https://github.com/anomalo-hq/anomalo-airflow-provider/blob/main/docs/connection.png?raw=True)\nThen fill in the fields for "Connection Id" (`anomalo-default` is the default connection id), "Host", and "API Secret Token".\n\n## Usage\n\n1. Obtain Anomalo table name from GUI. For example\n   ![table](https://github.com/anomalo-hq/anomalo-airflow-provider/blob/main/docs/table.png?raw=True)\n   would be `public-bq.covid19_nyt.us_counties`\n\n2. This package includes 3 different operators. You can find documentation for them on the operator code itself.\n   1. Run checks Operator: `airflow.providers.anomalo.operators.anomalo.AnomaloRunCheckOperator`\n   2. Job Sensor `airflow.providers.anomalo.sensors.anomalo.AnomaloJobCompleteSensor`\n   3. Validate table checks: `airflow.providers.anomalo.operators.anomalo.AnomaloPassFailOperator`\n\n3. See `anomalo_dag_example.py` for usage example\n\n## Releasing to PyPi\n\nTo release a new version to PyPi, you will need to\n\n1. Configure your pypi token by running:\n   ```poetry config pypi-token.pypi [token here]```\n   The token can be found in the AWS secrets manager\n2. Bump the version number in pyproject.toml. Make sure that this change is committed.\n3. run\n   ```poetry publish --build```\n\n',
     'author': 'Anomalo',
     'author_email': 'opensource@anomalo.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/anomalo-hq/anomalo-airflow-provider',
```

### Comparing `apache_airflow_providers_anomalo-0.2.0/PKG-INFO` & `apache_airflow_providers_anomalo-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-anomalo
-Version: 0.2.0
+Version: 0.2.1
 Summary: An Apache Airflow provider for Anomalo
 Home-page: https://github.com/anomalo-hq/anomalo-airflow-provider
 License: Apache-2.0
 Author: Anomalo
 Author-email: opensource@anomalo.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
```

