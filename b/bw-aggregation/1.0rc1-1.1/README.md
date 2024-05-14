# Comparing `tmp/bw_aggregation-1.0rc1.tar.gz` & `tmp/bw_aggregation-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_aggregation-1.0rc1.tar", last modified: Sat May 11 20:25:26 2024, max compression
+gzip compressed data, was "bw_aggregation-1.1.tar", last modified: Tue May 14 01:26:21 2024, max compression
```

## Comparing `bw_aggregation-1.0rc1.tar` & `bw_aggregation-1.1.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-11 20:25:26.256236 bw_aggregation-1.0rc1/
--rw-r--r--   0 cmutel     (501) staff       (20)     1070 2024-05-09 15:12:25.000000 bw_aggregation-1.0rc1/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2024-05-09 15:12:25.000000 bw_aggregation-1.0rc1/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     8403 2024-05-11 20:25:26.256014 bw_aggregation-1.0rc1/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     6712 2024-05-11 11:08:34.000000 bw_aggregation-1.0rc1/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-11 20:25:26.253610 bw_aggregation-1.0rc1/bw_aggregation/
--rw-r--r--   0 cmutel     (501) staff       (20)      582 2024-05-11 20:25:19.000000 bw_aggregation-1.0rc1/bw_aggregation/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4597 2024-05-11 11:29:50.000000 bw_aggregation-1.0rc1/bw_aggregation/calculator.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1827 2024-05-11 12:21:39.000000 bw_aggregation-1.0rc1/bw_aggregation/estimator.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7930 2024-05-11 12:19:09.000000 bw_aggregation-1.0rc1/bw_aggregation/main.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1625 2024-05-09 16:51:23.000000 bw_aggregation-1.0rc1/bw_aggregation/override.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-11 20:25:26.255386 bw_aggregation-1.0rc1/bw_aggregation.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     8403 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      434 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      214 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       15 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/top_level.txt
--rw-r--r--   0 cmutel     (501) staff       (20)     2581 2024-05-11 09:44:51.000000 bw_aggregation-1.0rc1/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2024-05-11 20:25:26.256291 bw_aggregation-1.0rc1/setup.cfg
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-11 20:25:26.255094 bw_aggregation-1.0rc1/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)      238 2024-05-11 12:23:14.000000 bw_aggregation-1.0rc1/tests/test_estimation.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7628 2024-05-11 11:30:42.000000 bw_aggregation-1.0rc1/tests/test_main.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1983 2024-05-09 16:58:44.000000 bw_aggregation-1.0rc1/tests/test_override.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-14 01:26:21.354922 bw_aggregation-1.1/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1070 2024-05-09 15:12:25.000000 bw_aggregation-1.1/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2024-05-09 15:12:25.000000 bw_aggregation-1.1/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     9140 2024-05-14 01:26:21.354561 bw_aggregation-1.1/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     7430 2024-05-13 15:07:17.000000 bw_aggregation-1.1/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-14 01:26:21.351379 bw_aggregation-1.1/bw_aggregation/
+-rw-r--r--   0 cmutel     (501) staff       (20)      578 2024-05-14 00:46:05.000000 bw_aggregation-1.1/bw_aggregation/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4691 2024-05-13 12:25:08.000000 bw_aggregation-1.1/bw_aggregation/calculator.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      288 2024-05-13 12:05:27.000000 bw_aggregation-1.1/bw_aggregation/errors.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3212 2024-05-14 00:45:15.000000 bw_aggregation-1.1/bw_aggregation/estimator.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8280 2024-05-14 00:45:15.000000 bw_aggregation-1.1/bw_aggregation/main.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1625 2024-05-09 16:51:23.000000 bw_aggregation-1.1/bw_aggregation/override.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      975 2024-05-14 00:43:49.000000 bw_aggregation-1.1/bw_aggregation/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-14 01:26:21.353925 bw_aggregation-1.1/bw_aggregation.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     9140 2024-05-14 01:26:21.000000 bw_aggregation-1.1/bw_aggregation.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      503 2024-05-14 01:26:21.000000 bw_aggregation-1.1/bw_aggregation.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-14 01:26:21.000000 bw_aggregation-1.1/bw_aggregation.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      236 2024-05-14 01:26:21.000000 bw_aggregation-1.1/bw_aggregation.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       15 2024-05-14 01:26:21.000000 bw_aggregation-1.1/bw_aggregation.egg-info/top_level.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)     2603 2024-05-12 10:13:46.000000 bw_aggregation-1.1/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)       38 2024-05-14 01:26:21.354974 bw_aggregation-1.1/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-14 01:26:21.353552 bw_aggregation-1.1/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)      298 2024-05-13 15:10:56.000000 bw_aggregation-1.1/tests/test_estimation.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     7960 2024-05-14 00:29:59.000000 bw_aggregation-1.1/tests/test_main.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1983 2024-05-09 16:58:44.000000 bw_aggregation-1.1/tests/test_override.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      515 2024-05-14 00:43:07.000000 bw_aggregation-1.1/tests/test_utils.py
```

### Comparing `bw_aggregation-1.0rc1/LICENSE` & `bw_aggregation-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_aggregation-1.0rc1/PKG-INFO` & `bw_aggregation-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_aggregation
-Version: 1.0rc1
+Version: 1.1
 Summary: Use aggregated processes for quicker calculations
 Author-email: bw_aggregation <cmutel@gmail.com>
 Maintainer-email: bw_aggregation <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_aggregation
 Project-URL: homepage, https://github.com/brightway-lca/bw_aggregation
 Project-URL: tracker, https://github.com/brightway-lca/bw_aggregation/issues
 Classifier: Development Status :: 4 - Beta
@@ -17,20 +17,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bw2calc>1.99
-Requires-Dist: bw2data>3.99
-Requires-Dist: bw_graph_tools
-Requires-Dist: bw_processing
+Requires-Dist: bw2data>=4.0.dev36
+Requires-Dist: bw_graph_tools>=0.3.1
+Requires-Dist: bw_processing>=0.9.3
 Requires-Dist: fs
 Requires-Dist: matrix_utils
-Requires-Dist: numpy
+Requires-Dist: numpy<2
 Provides-Extra: testing
 Requires-Dist: bw_aggregation; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
@@ -93,25 +93,37 @@
 ```python
 import bw_aggregated as bwa
 bwa.AggregatedDatabase.estimate_speedup("<database label>")
 ```
 
 That will return something like:
 
-TBD
+```python
+Speedup(
+    database_name='USEEIO-2.0',
+    time_with_aggregation=0.06253910064697266,
+    time_without_aggregation=0.026948928833007812,
+    time_difference_absolute=0.035590171813964844,
+    time_difference_relative=2.3206525585674855
+)
+```
+
+The times reported include `LCA` object creation, data loading, matrix construcion, and inventory calculations.
+
+As you can see, creating aggregated activities to avoid solving linear systems will not always lead to faster calculations, as the linear algebra libraries we use are pretty fast, and loading lots of data into the biosphere can take a lot of time. Please check on potential speedups before deciding to aggregate background databases.
 
 If you want to convert that database, you can with:
 
 ```python
 bwa.AggregatedDatabase.convert_existing("<database label>")
 ```
 
 From now on, calling `bw2data.Database("<database label>")` will return an instance of `AggregatedDatabase`. You can do everything you normally would with this database, including making changes.
 
-> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` object references.
+> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` class instances.
 
 The conversion command will also set the default to use the aggregated values during calculations. You can change the default back to using unit process data with:
 
 ```python
 import bw2data as bd
 bd.Database("<database label>").use_aggregated(False)
 ```
@@ -161,17 +173,17 @@
 ## Implementation
 
 This library gets the possibility of using both aggregated and unit process data by overriding the `.datapackage` method, and loading one or two different datapackages depending on the current context. This approach is compatiable with both manual loading of datapackages, and with the `bw2data` function `prepare_lca_inputs`. The `.datapackage` method of an `AggregatedDatabase` is roughly:
 
 ```
 if global_context is True:
     load_aggregated()
-elif local_context(me) is True:
+elif local_context(this_database) is True:
     load_aggregated()
-elif me.perfer_aggregated is True:
+elif this_database.prefer_aggregated is True:
     load_aggregated()
 else:
     load_unit_process()
 ```
 
 ## Contributing
```

### Comparing `bw_aggregation-1.0rc1/README.md` & `bw_aggregation-1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -50,25 +50,37 @@
 ```python
 import bw_aggregated as bwa
 bwa.AggregatedDatabase.estimate_speedup("<database label>")
 ```
 
 That will return something like:
 
-TBD
+```python
+Speedup(
+    database_name='USEEIO-2.0',
+    time_with_aggregation=0.06253910064697266,
+    time_without_aggregation=0.026948928833007812,
+    time_difference_absolute=0.035590171813964844,
+    time_difference_relative=2.3206525585674855
+)
+```
+
+The times reported include `LCA` object creation, data loading, matrix construcion, and inventory calculations.
+
+As you can see, creating aggregated activities to avoid solving linear systems will not always lead to faster calculations, as the linear algebra libraries we use are pretty fast, and loading lots of data into the biosphere can take a lot of time. Please check on potential speedups before deciding to aggregate background databases.
 
 If you want to convert that database, you can with:
 
 ```python
 bwa.AggregatedDatabase.convert_existing("<database label>")
 ```
 
 From now on, calling `bw2data.Database("<database label>")` will return an instance of `AggregatedDatabase`. You can do everything you normally would with this database, including making changes.
 
-> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` object references.
+> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` class instances.
 
 The conversion command will also set the default to use the aggregated values during calculations. You can change the default back to using unit process data with:
 
 ```python
 import bw2data as bd
 bd.Database("<database label>").use_aggregated(False)
 ```
@@ -118,17 +130,17 @@
 ## Implementation
 
 This library gets the possibility of using both aggregated and unit process data by overriding the `.datapackage` method, and loading one or two different datapackages depending on the current context. This approach is compatiable with both manual loading of datapackages, and with the `bw2data` function `prepare_lca_inputs`. The `.datapackage` method of an `AggregatedDatabase` is roughly:
 
 ```
 if global_context is True:
     load_aggregated()
-elif local_context(me) is True:
+elif local_context(this_database) is True:
     load_aggregated()
-elif me.perfer_aggregated is True:
+elif this_database.prefer_aggregated is True:
     load_aggregated()
 else:
     load_unit_process()
 ```
 
 ## Contributing
```

### Comparing `bw_aggregation-1.0rc1/bw_aggregation/__init__.py` & `bw_aggregation-1.1/bw_aggregation/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     "__version__",
     "AggregatedDatabase",
     "AggregationContext",
     "ObsoleteAggregatedDatapackage",
     "Speedup",
 )
 
-__version__ = "1.0.RC1"
+__version__ = "1.1"
 
 
 from bw2data.backends import Activity
 from bw2data.subclass_mapping import (
     DATABASE_BACKEND_MAPPING,
     NODE_PROCESS_CLASS_MAPPING,
 )
 
+from .estimator import Speedup
 from .main import AggregatedDatabase, ObsoleteAggregatedDatapackage
 from .override import AggregationContext
-from .estimator import Speedup
 
 DATABASE_BACKEND_MAPPING["aggregated"] = AggregatedDatabase
 NODE_PROCESS_CLASS_MAPPING["aggregated"] = Activity
```

### Comparing `bw_aggregation-1.0rc1/bw_aggregation/calculator.py` & `bw_aggregation-1.1/bw_aggregation/calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from time import time
 
 import numpy as np
-from bw2calc import LCA, PYPARDISO, spsolve
+from bw2calc import LCA, spsolve
 from bw2data import databases, prepare_lca_inputs
 from bw2data.database import DatabaseChooser
 from bw_graph_tools import guess_production_exchanges
 from matrix_utils import ArrayMapper
 from scipy.sparse import csr_matrix
 
 from .override import AggregationContext
@@ -30,15 +30,19 @@
 
         # Only need to solve for the products from the processes in *this* database
         # Correspondence between processes and their reference products is not fixed.
         # We use `guess_production_exchanges` instead of assuming values on a diagonal
         prod_rows, prod_cols = guess_production_exchanges(self.lca.technosphere_mm)
         # Not very efficient; could be SQL query but that would break IOTable
         matrix_db_process_ids = np.array(
-            [self.lca.dicts.activity[obj.id] for obj in self.db]
+            [
+                self.lca.dicts.activity[obj.id]
+                for obj in self.db
+                if obj.get("type", "process") == "process"
+            ]
         )
 
         # Get boolean mask for the column indices of the processes in the database
         # we are looking at
         mask = np.isin(prod_cols, matrix_db_process_ids)
 
         # Construct demand array with dimensions (all processes, filtered processes)
```

### Comparing `bw_aggregation-1.0rc1/bw_aggregation/main.py` & `bw_aggregation-1.1/bw_aggregation/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,25 @@
-import warnings
 from datetime import datetime as dt
 
-import tqdm
-from bw2calc import LCA, PYPARDISO
 from bw2data import databases
 from bw2data.backends import SQLiteBackend
 from bw_processing import (
     Datapackage,
     clean_datapackage_name,
     create_datapackage,
     load_datapackage,
     safe_filename,
 )
 from fs.zipfs import ZipFS
 
 from .calculator import AggregationCalculator
+from .errors import IncompatibleDatabase, ObsoleteAggregatedDatapackage
+from .estimator import CalculationDifferenceEstimator, Speedup
 from .override import AggregationContext, aggregation_override
-from .estimator import CalculationDifferenceEstimator
-
-
-class ObsoleteAggregatedDatapackage(Exception):
-    """The results from this aggregated datapackage are obsolete"""
-
-    pass
+from .utils import check_processes_in_data, check_processes_in_database
 
 
 class AggregatedDatabase(SQLiteBackend):
     """A class which maintains two processed datapackages, and can use the aggregated datapackage
     for quicker calculations.
 
     An aggregated database only stores the *cumulative biosphere flows* of each unit process
@@ -74,29 +67,33 @@
         )
         return (
             dt.fromisoformat(self.metadata["aggregation_calculation_timestamp"])
             >= latest_change
         )
 
     @staticmethod
-    def estimate_speedup(database_name: str) -> float:
+    def estimate_speedup(database_name: str) -> Speedup:
         """Estimate how much quicker calculations could be when using aggregated emissions.
 
         Prints to `stdout` and return a float, the ratio of calculation speed with aggregation
         to speed without aggregation."""
         return CalculationDifferenceEstimator(database_name).difference()
 
     @staticmethod
     def convert_existing(database_name: str) -> None:
         """Convert a unit process database to an aggregated database."""
         if database_name not in databases:
             raise ValueError(f"Database '{database_name}' doesn't exist")
         if databases[database_name]["backend"] == "aggregated":
             print(f"Database '{database_name}' is already aggregated")
             return
+        if not check_processes_in_database(database_name):
+            raise IncompatibleDatabase(
+                "This database only has biosphere flows, and can't be aggregated."
+            )
 
         db = AggregatedDatabase(database_name)
         db.process_aggregated()
         databases[database_name]["backend"] = "aggregated"
         db.use_aggregated(True)
 
     def use_aggregated(self, default: bool = True) -> None:
@@ -159,14 +156,19 @@
             and not AggregatedDatabase(name).aggregation_datapackage_valid()
         ]
         with AggregationContext(False):
             for db_name in outdated_databases:
                 AggregatedDatabase(db_name).refresh()
 
     def write(self, data, process=True, searchable=True) -> None:
+        if not check_processes_in_data(data.values()):
+            raise IncompatibleDatabase(
+                "This data only has biosphere flows, and can't be aggregated."
+            )
+
         super().write(data=data, process=process, searchable=searchable)
 
         if process:
             self.process_aggregated()
 
     def process_aggregated(self, in_memory: bool = False) -> Datapackage:
         """Create structured arrays for the aggregated biosphere emissions, and for unitary production."""
@@ -196,8 +198,8 @@
         dp.add_persistent_vector_from_iterator(
             matrix="technosphere_matrix",
             name=clean_datapackage_name(self.name + " technosphere matrix"),
             dict_iterator=calculator.technosphere_iterator,
         )
         if not in_memory:
             dp.finalize_serialization()
-        return dp
+        return dp
```

### Comparing `bw_aggregation-1.0rc1/bw_aggregation/override.py` & `bw_aggregation-1.1/bw_aggregation/override.py`

 * *Files identical despite different names*

### Comparing `bw_aggregation-1.0rc1/bw_aggregation.egg-info/PKG-INFO` & `bw_aggregation-1.1/bw_aggregation.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_aggregation
-Version: 1.0rc1
+Version: 1.1
 Summary: Use aggregated processes for quicker calculations
 Author-email: bw_aggregation <cmutel@gmail.com>
 Maintainer-email: bw_aggregation <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_aggregation
 Project-URL: homepage, https://github.com/brightway-lca/bw_aggregation
 Project-URL: tracker, https://github.com/brightway-lca/bw_aggregation/issues
 Classifier: Development Status :: 4 - Beta
@@ -17,20 +17,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bw2calc>1.99
-Requires-Dist: bw2data>3.99
-Requires-Dist: bw_graph_tools
-Requires-Dist: bw_processing
+Requires-Dist: bw2data>=4.0.dev36
+Requires-Dist: bw_graph_tools>=0.3.1
+Requires-Dist: bw_processing>=0.9.3
 Requires-Dist: fs
 Requires-Dist: matrix_utils
-Requires-Dist: numpy
+Requires-Dist: numpy<2
 Provides-Extra: testing
 Requires-Dist: bw_aggregation; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
@@ -93,25 +93,37 @@
 ```python
 import bw_aggregated as bwa
 bwa.AggregatedDatabase.estimate_speedup("<database label>")
 ```
 
 That will return something like:
 
-TBD
+```python
+Speedup(
+    database_name='USEEIO-2.0',
+    time_with_aggregation=0.06253910064697266,
+    time_without_aggregation=0.026948928833007812,
+    time_difference_absolute=0.035590171813964844,
+    time_difference_relative=2.3206525585674855
+)
+```
+
+The times reported include `LCA` object creation, data loading, matrix construcion, and inventory calculations.
+
+As you can see, creating aggregated activities to avoid solving linear systems will not always lead to faster calculations, as the linear algebra libraries we use are pretty fast, and loading lots of data into the biosphere can take a lot of time. Please check on potential speedups before deciding to aggregate background databases.
 
 If you want to convert that database, you can with:
 
 ```python
 bwa.AggregatedDatabase.convert_existing("<database label>")
 ```
 
 From now on, calling `bw2data.Database("<database label>")` will return an instance of `AggregatedDatabase`. You can do everything you normally would with this database, including making changes.
 
-> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` object references.
+> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` class instances.
 
 The conversion command will also set the default to use the aggregated values during calculations. You can change the default back to using unit process data with:
 
 ```python
 import bw2data as bd
 bd.Database("<database label>").use_aggregated(False)
 ```
@@ -161,17 +173,17 @@
 ## Implementation
 
 This library gets the possibility of using both aggregated and unit process data by overriding the `.datapackage` method, and loading one or two different datapackages depending on the current context. This approach is compatiable with both manual loading of datapackages, and with the `bw2data` function `prepare_lca_inputs`. The `.datapackage` method of an `AggregatedDatabase` is roughly:
 
 ```
 if global_context is True:
     load_aggregated()
-elif local_context(me) is True:
+elif local_context(this_database) is True:
     load_aggregated()
-elif me.perfer_aggregated is True:
+elif this_database.prefer_aggregated is True:
     load_aggregated()
 else:
     load_unit_process()
 ```
 
 ## Contributing
```

### Comparing `bw_aggregation-1.0rc1/pyproject.toml` & `bw_aggregation-1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     "Topic :: Scientific/Engineering"
 ]
 requires-python = ">=3.9"
 dependencies = [
     # dependencies as strings with quotes, e.g. "foo"
     # You can add version requirements like "foo>2.0"
     "bw2calc>1.99",
-    "bw2data>3.99",
-    "bw_graph_tools",
-    "bw_processing",
+    "bw2data>=4.0.dev36",
+    "bw_graph_tools>=0.3.1",
+    "bw_processing>=0.9.3",
     "fs",
     "matrix_utils",
-    "numpy",
+    "numpy<2",
 ]
 
 [project.urls]
 source = "https://github.com/brightway-lca/bw_aggregation"
 homepage = "https://github.com/brightway-lca/bw_aggregation"
 tracker = "https://github.com/brightway-lca/bw_aggregation/issues"
```

### Comparing `bw_aggregation-1.0rc1/tests/test_main.py` & `bw_aggregation-1.1/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import sys
+
 import numpy as np
 import pytest
 from bw2calc import LCA
 from bw2data import Database, databases, get_node
 from bw2data.backends import SQLiteBackend
 
 from bw_aggregation import AggregatedDatabase, ObsoleteAggregatedDatapackage
+from bw_aggregation.errors import IncompatibleDatabase
 
 
 def check_a_database_matrices_unaggregated(lca: LCA):
     node = get_node(database="a", code="2")
     rows, _ = lca.technosphere_matrix[:, lca.dicts.activity[node.id]].nonzero()
     assert rows.shape == (2,)
     assert lca.technosphere_matrix[:, lca.dicts.activity[node.id]].sum() == 2.5
@@ -49,14 +52,17 @@
     assert lca.technosphere_matrix[:, lca.dicts.activity[node.id]].sum() == 1
 
     rows, _ = lca.biosphere_matrix[:, lca.dicts.activity[node.id]].nonzero()
     assert rows.shape == (2,)
     assert lca.biosphere_matrix[:, lca.dicts.activity[node.id]].sum() != 7
 
 
+@pytest.mark.skipif(
+    sys.platform.startswith("win"), reason="Error on cleanup deleting tmpdir"
+)
 def test_convert_existing(background):
     AggregatedDatabase.convert_existing("a")
     assert databases["a"]["backend"] == "aggregated"
     assert databases["a"]["aggregation_calculation_time"]
     assert databases["a"]["aggregation_calculation_timestamp"]
     assert databases["a"]["aggregation_use_in_calculation"]
 
@@ -257,7 +263,12 @@
     assert not Database("a").aggregation_datapackage_valid()
     assert not Database("b").aggregation_datapackage_valid()
 
     AggregatedDatabase.refresh_all()
 
     assert Database("a").aggregation_datapackage_valid()
     assert Database("b").aggregation_datapackage_valid()
+
+
+def test_incompatible_database_only_biosphere_flows(background):
+    with pytest.raises(IncompatibleDatabase):
+        AggregatedDatabase.convert_existing("bio")
```

### Comparing `bw_aggregation-1.0rc1/tests/test_override.py` & `bw_aggregation-1.1/tests/test_override.py`

 * *Files identical despite different names*

