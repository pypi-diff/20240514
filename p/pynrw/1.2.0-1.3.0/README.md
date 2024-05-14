# Comparing `tmp/pynrw-1.2.0.tar.gz` & `tmp/pynrw-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrw-1.2.0.tar", last modified: Sat May 11 01:11:39 2024, max compression
+gzip compressed data, was "pynrw-1.3.0.tar", last modified: Tue May 14 21:37:29 2024, max compression
```

## Comparing `pynrw-1.2.0.tar` & `pynrw-1.3.0.tar`

### file list

```diff
@@ -1,35 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.141213 pynrw-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-11 01:11:29.000000 pynrw-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-11 01:11:39.137213 pynrw-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-11 01:11:29.000000 pynrw-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.133213 pynrw-1.2.0/nrw/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.133213 pynrw-1.2.0/nrw/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/_searching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/_traversal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.137213 pynrw-1.2.0/nrw/datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_comparable_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.137213 pynrw-1.2.0/pynrw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-11 01:11:29.000000 pynrw-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:11:39.141213 pynrw-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.260302 pynrw-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-14 21:37:19.000000 pynrw-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-14 21:37:29.260302 pynrw-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-05-14 21:37:19.000000 pynrw-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.256302 pynrw-1.3.0/nrw/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.256302 pynrw-1.3.0/nrw/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/_searching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/algorithms/_traversal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.260302 pynrw-1.3.0/nrw/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/_query_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/msaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/msaccess.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/mysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/database/sqlite.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.260302 pynrw-1.3.0/nrw/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_comparable_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/datastructures/_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:19.000000 pynrw-1.3.0/nrw/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:37:29.260302 pynrw-1.3.0/pynrw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 21:37:29.000000 pynrw-1.3.0/pynrw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-14 21:37:19.000000 pynrw-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 21:37:19.000000 pynrw-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:37:29.260302 pynrw-1.3.0/setup.cfg
```

### Comparing `pynrw-1.2.0/LICENSE` & `pynrw-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/PKG-INFO` & `pynrw-1.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.2.0
+Version: 1.3.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -15,27 +15,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: bandit; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: covdefaults; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pylint-pytest; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: tox; extra == "dev"
+Requires-Dist: mysql-connector-python
+Requires-Dist: pyodbc; platform_python_implementation == "CPython"
+Requires-Dist: pypyodbc; platform_python_implementation == "PyPy"
 
 # pynrw
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/realshouzy/pynrw/main.svg)](https://results.pre-commit.ci/latest/github/realshouzy/pynrw/main)
 [![pylint status](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml)
 [![test status](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml)
 [![CodeQL](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml)
@@ -44,20 +34,56 @@
 [![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/pynrw/releases)
 [![PyPI - Format](https://img.shields.io/pypi/format/pynrw)](https://pypi.org/project/pynrw/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/realshouzy/pynrw/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-This package implements the datastructures given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
+This package implements the datastructures and database classes given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
 
 **Dieses Package dient alleine zu Bildungszwecken und sollte nicht in Produktion genutzt werden!**
 
+## Installation
+
+```bash
+pip install pynrw
+```
+
+Alternativ:
+
+```bash
+pip install git+https://github.com/realshouzy/pynrw
+```
+
+## Beispiel
+
+```python
+from nrw.algorithms import quick_sort
+from nrw.datastructures import List
+
+lst: List[int] = List()
+
+for i in range(0, 10, -1):
+  lst.append(i)
+
+print(lst.content)  # None
+lst.to_first()
+print(lst.content)  # 9
+print(lst)  # List(9 -> 8 -> 7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1 -> 0)
+
+sorted_lst: List[int] = quick_sort(lst)
+sorted_lst.to_first()
+print(sorted_lst.content)  # 0
+print(sorted_lst)  # List(0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9)
+```
+
 ## Dokumentation
 
+### Datenstrukturen
+
 Dieses Package implementiert die Datenstrukturen nach den Vorgaben des Landes NRW in Python, zu finden in [`nrw.datastructures`](/nrw/datastructures/), d.s.:
 
 - [`List`](/nrw/datastructures/_list.py)
 - [`Stack`](/nrw/datastructures/_stack.py)
 - [`Queue`](/nrw/datastructures/_queue.py)
 - [`BinaryTree`](/nrw/datastructures/_binary_tree.py)
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
@@ -93,73 +119,62 @@
 
 Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
 
+### Algorithmen
+
 Zusätzlich enthält dieses Package nützliche Funktionen zum Sortieren, Suchen und Traversiern, zu finden in [`nrw.algorithms`](/nrw/algorithms/):
 
-- [`linear_search`](/nrw/algorithms/_searching.py)
-- [`depth_first_search`](/nrw/algorithms/_searching.py)
-- [`breadth_first_search`](/nrw/algorithms/_searching.py)
-- [`bubble_sort`](/nrw/algorithms/_sorting.py)
-- [`selection_sort`](/nrw/algorithms/_sorting.py)
-- [`insertion_sort`](/nrw/algorithms/_sorting.py)
-- [`merge_sort`](/nrw/algorithms/_sorting.py)
-- [`quick_sort`](/nrw/algorithms/_sorting.py)
-- [`preorder`](/nrw/algorithms/_traversal.py)
-- [`inorder`](/nrw/algorithms/_traversal.py)
-- [`reverse_inorder`](/nrw/algorithms/_traversal.py)
-- [`postorder`](/nrw/algorithms/_traversal.py)
-- [`levelorder`](/nrw/algorithms/_traversal.py)
+- [`linear_search`](/nrw/algorithms/_searching.py#L23)
+- [`depth_first_search`](/nrw/algorithms/_searching.py#L55)
+- [`breadth_first_search`](/nrw/algorithms/_searching.py#L64)
+- [`bubble_sort`](/nrw/algorithms/_sorting.py#L21)
+- [`selection_sort`](/nrw/algorithms/_sorting.py#L37)
+- [`insertion_sort`](/nrw/algorithms/_sorting.py#L67)
+- [`merge_sort`](/nrw/algorithms/_sorting.py#L86)
+- [`quick_sort`](/nrw/algorithms/_sorting.py#L141)
+- [`preorder`](/nrw/algorithms/_traversal.py#L19)
+- [`inorder`](/nrw/algorithms/_traversal.py#L41)
+- [`postorder`](/nrw/algorithms/_traversal.py#L63)
+- [`levelorder`](/nrw/algorithms/_traversal.py#L85)
+
+Die verschiedenen Traversierungen unterstützen auch Umkehrung.
+Allerdings muss annotiert werden, dass aufgrund der Vorgaben des Landes die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte kommen. Welche dies sind, wird dem Leser als Übung überlassen.
+
+### Datenbankklassen
+
+Analog zu den Datenstrukturen sind auch Datenbankklassen größtenteils semantisch identisch zur den Vorgaben des Landes.
+Die jeweiligen Klassen sind in [`nrw.database`](/nrw/database/) definiert:
+
+- [`sqlite.DatabaseConnector`](/nrw/database/sqlite.py)
+- [`mysql.DatabaseConnector`](/nrw/database/mysql.py)
+- [`msaccess.DatabaseConnector`](/nrw/database/msaccess.py)
+- [`QueryResult`](/nrw/database/_query_result.py)
+
+Hierbei ist zu beachten, dass der `DatabaseConnector` für MSAccess den Microsoft Access Driver benötigt und passwortgeschützte Datenbanken nicht unterstüzt.
+Des weiteren gilt für `QueryResult`, dass die Daten und die Spaltentypen nicht unbedingt als String wiedergegeben werden. Die Daten werden als Python-Äquivalenten Datentypen wiedergegeben, und für die Spaltentypen gilt:
+
+- SQLite: immer `None`, da SQLite dynamisch typisiert ist
+- MySQL: die entsprechenden Datentypen von MySQL als String
+- MSAccess: die entsprechenden Datentypen (Klassen) von Python
 
-Allerdings muss annotiert werden, dass aufgrund der Vorgaben des Landes die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte kommen. Welche dies sind, wird dem Leser als Übung überlassen. Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.
+### Allgemein
 
-Für Hilfe zum jeweiligen Objekt (gilt für alle oben genannte Objekte), z.B.:
+Für mehr Information zu einem beliebigen Objekt kann `help` genutzt werden, z.B.:
 
 ```python
 from nrw.datastructures import List
 help(List)
 help(List.insert)
 ```
 
-## Installation
-
-```bash
-pip install pynrw
-```
-
-Alternativ:
-
-```bash
-pip install git+https://github.com/realshouzy/pynrw.git
-```
-
-## Beispiel
-
-```python
-from nrw.algorithms import quick_sort
-from nrw.datastructures import List
-
-lst: List[int] = List()
-
-for i in range(0, 10, -1):
-  lst.append(i)
-
-print(lst.content)  # None
-lst.to_first()
-print(lst.content)  # 9
-print(lst)  # List(9 -> 8 -> 7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1 -> 0)
-
-sorted_lst: List[int] = quick_sort(lst)
-sorted_lst.to_first()
-print(sorted_lst.content)  # 0
-print(sorted_lst)  # List(0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9)
-```
+**Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.**
 
 ## Motivation
 
 Vereinfacht: Java, als Programmiersprache in der Bildung, ist eine schlechte Wahl, da ...
 
 - Java veraltet ist.
 - das rein objekt-orientierte Paradigma schlechthin unbrauchbar ist.
```

### Comparing `pynrw-1.2.0/README.md` & `pynrw-1.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,20 +9,56 @@
 [![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/pynrw/releases)
 [![PyPI - Format](https://img.shields.io/pypi/format/pynrw)](https://pypi.org/project/pynrw/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/realshouzy/pynrw/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-This package implements the datastructures given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
+This package implements the datastructures and database classes given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
 
 **Dieses Package dient alleine zu Bildungszwecken und sollte nicht in Produktion genutzt werden!**
 
+## Installation
+
+```bash
+pip install pynrw
+```
+
+Alternativ:
+
+```bash
+pip install git+https://github.com/realshouzy/pynrw
+```
+
+## Beispiel
+
+```python
+from nrw.algorithms import quick_sort
+from nrw.datastructures import List
+
+lst: List[int] = List()
+
+for i in range(0, 10, -1):
+  lst.append(i)
+
+print(lst.content)  # None
+lst.to_first()
+print(lst.content)  # 9
+print(lst)  # List(9 -> 8 -> 7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1 -> 0)
+
+sorted_lst: List[int] = quick_sort(lst)
+sorted_lst.to_first()
+print(sorted_lst.content)  # 0
+print(sorted_lst)  # List(0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9)
+```
+
 ## Dokumentation
 
+### Datenstrukturen
+
 Dieses Package implementiert die Datenstrukturen nach den Vorgaben des Landes NRW in Python, zu finden in [`nrw.datastructures`](/nrw/datastructures/), d.s.:
 
 - [`List`](/nrw/datastructures/_list.py)
 - [`Stack`](/nrw/datastructures/_stack.py)
 - [`Queue`](/nrw/datastructures/_queue.py)
 - [`BinaryTree`](/nrw/datastructures/_binary_tree.py)
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
@@ -58,73 +94,62 @@
 
 Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
 
+### Algorithmen
+
 Zusätzlich enthält dieses Package nützliche Funktionen zum Sortieren, Suchen und Traversiern, zu finden in [`nrw.algorithms`](/nrw/algorithms/):
 
-- [`linear_search`](/nrw/algorithms/_searching.py)
-- [`depth_first_search`](/nrw/algorithms/_searching.py)
-- [`breadth_first_search`](/nrw/algorithms/_searching.py)
-- [`bubble_sort`](/nrw/algorithms/_sorting.py)
-- [`selection_sort`](/nrw/algorithms/_sorting.py)
-- [`insertion_sort`](/nrw/algorithms/_sorting.py)
-- [`merge_sort`](/nrw/algorithms/_sorting.py)
-- [`quick_sort`](/nrw/algorithms/_sorting.py)
-- [`preorder`](/nrw/algorithms/_traversal.py)
-- [`inorder`](/nrw/algorithms/_traversal.py)
-- [`reverse_inorder`](/nrw/algorithms/_traversal.py)
-- [`postorder`](/nrw/algorithms/_traversal.py)
-- [`levelorder`](/nrw/algorithms/_traversal.py)
+- [`linear_search`](/nrw/algorithms/_searching.py#L23)
+- [`depth_first_search`](/nrw/algorithms/_searching.py#L55)
+- [`breadth_first_search`](/nrw/algorithms/_searching.py#L64)
+- [`bubble_sort`](/nrw/algorithms/_sorting.py#L21)
+- [`selection_sort`](/nrw/algorithms/_sorting.py#L37)
+- [`insertion_sort`](/nrw/algorithms/_sorting.py#L67)
+- [`merge_sort`](/nrw/algorithms/_sorting.py#L86)
+- [`quick_sort`](/nrw/algorithms/_sorting.py#L141)
+- [`preorder`](/nrw/algorithms/_traversal.py#L19)
+- [`inorder`](/nrw/algorithms/_traversal.py#L41)
+- [`postorder`](/nrw/algorithms/_traversal.py#L63)
+- [`levelorder`](/nrw/algorithms/_traversal.py#L85)
+
+Die verschiedenen Traversierungen unterstützen auch Umkehrung.
+Allerdings muss annotiert werden, dass aufgrund der Vorgaben des Landes die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte kommen. Welche dies sind, wird dem Leser als Übung überlassen.
+
+### Datenbankklassen
+
+Analog zu den Datenstrukturen sind auch Datenbankklassen größtenteils semantisch identisch zur den Vorgaben des Landes.
+Die jeweiligen Klassen sind in [`nrw.database`](/nrw/database/) definiert:
+
+- [`sqlite.DatabaseConnector`](/nrw/database/sqlite.py)
+- [`mysql.DatabaseConnector`](/nrw/database/mysql.py)
+- [`msaccess.DatabaseConnector`](/nrw/database/msaccess.py)
+- [`QueryResult`](/nrw/database/_query_result.py)
+
+Hierbei ist zu beachten, dass der `DatabaseConnector` für MSAccess den Microsoft Access Driver benötigt und passwortgeschützte Datenbanken nicht unterstüzt.
+Des weiteren gilt für `QueryResult`, dass die Daten und die Spaltentypen nicht unbedingt als String wiedergegeben werden. Die Daten werden als Python-Äquivalenten Datentypen wiedergegeben, und für die Spaltentypen gilt:
+
+- SQLite: immer `None`, da SQLite dynamisch typisiert ist
+- MySQL: die entsprechenden Datentypen von MySQL als String
+- MSAccess: die entsprechenden Datentypen (Klassen) von Python
 
-Allerdings muss annotiert werden, dass aufgrund der Vorgaben des Landes die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte kommen. Welche dies sind, wird dem Leser als Übung überlassen. Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.
+### Allgemein
 
-Für Hilfe zum jeweiligen Objekt (gilt für alle oben genannte Objekte), z.B.:
+Für mehr Information zu einem beliebigen Objekt kann `help` genutzt werden, z.B.:
 
 ```python
 from nrw.datastructures import List
 help(List)
 help(List.insert)
 ```
 
-## Installation
-
-```bash
-pip install pynrw
-```
-
-Alternativ:
-
-```bash
-pip install git+https://github.com/realshouzy/pynrw.git
-```
-
-## Beispiel
-
-```python
-from nrw.algorithms import quick_sort
-from nrw.datastructures import List
-
-lst: List[int] = List()
-
-for i in range(0, 10, -1):
-  lst.append(i)
-
-print(lst.content)  # None
-lst.to_first()
-print(lst.content)  # 9
-print(lst)  # List(9 -> 8 -> 7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1 -> 0)
-
-sorted_lst: List[int] = quick_sort(lst)
-sorted_lst.to_first()
-print(sorted_lst.content)  # 0
-print(sorted_lst)  # List(0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9)
-```
+**Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.**
 
 ## Motivation
 
 Vereinfacht: Java, als Programmiersprache in der Bildung, ist eine schlechte Wahl, da ...
 
 - Java veraltet ist.
 - das rein objekt-orientierte Paradigma schlechthin unbrauchbar ist.
```

### Comparing `pynrw-1.2.0/nrw/algorithms/__init__.py` & `pynrw-1.3.0/nrw/algorithms/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     "bubble_sort",
     "selection_sort",
     "insertion_sort",
     "merge_sort",
     "quick_sort",
     "preorder",
     "inorder",
-    "reverse_inorder",
     "postorder",
     "levelorder",
+    "reverse_inorder",
 )
 
 from typing import Final
 
 from nrw.algorithms._searching import (
     breadth_first_search,
     depth_first_search,
```

### Comparing `pynrw-1.2.0/nrw/algorithms/__init__.pyi` & `pynrw-1.3.0/nrw/algorithms/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# pylint: skip-file
 __all__: Final[tuple[str, ...]] = (
     "linear_search",
     "depth_first_search",
     "breadth_first_search",
     "bubble_sort",
     "selection_sort",
     "insertion_sort",
     "merge_sort",
     "quick_sort",
     "preorder",
     "inorder",
-    "reverse_inorder",
     "postorder",
     "levelorder",
+    "reverse_inorder",
 )
 
 from typing import Final, TypeVar, overload
 
 from nrw.datastructures import (
     BinarySearchTree,
     BinaryTree,
@@ -32,36 +33,44 @@
 def breadth_first_search(graph: Graph, vertex: Vertex) -> List[Vertex]: ...
 def bubble_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
 def selection_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
 def insertion_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
 def merge_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
 def quick_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
 @overload
-def preorder(tree: BinaryTree[_T]) -> List[_T]: ...
+def preorder(tree: BinaryTree[_T], *, reverse: bool = False) -> List[_T]: ...
 @overload
 def preorder(
     tree: BinarySearchTree[ComparableContentT],
+    *,
+    reverse: bool = False,
 ) -> List[ComparableContentT]: ...
 @overload
-def inorder(tree: BinaryTree[_T]) -> List[_T]: ...
+def inorder(tree: BinaryTree[_T], *, reverse: bool = False) -> List[_T]: ...
 @overload
 def inorder(
     tree: BinarySearchTree[ComparableContentT],
+    *,
+    reverse: bool = False,
 ) -> List[ComparableContentT]: ...
 @overload
 def reverse_inorder(tree: BinaryTree[_T]) -> List[_T]: ...
 @overload
 def reverse_inorder(
     tree: BinarySearchTree[ComparableContentT],
 ) -> List[ComparableContentT]: ...
 @overload
-def postorder(tree: BinaryTree[_T]) -> List[_T]: ...
+def postorder(tree: BinaryTree[_T], *, reverse: bool = False) -> List[_T]: ...
 @overload
 def postorder(
     tree: BinarySearchTree[ComparableContentT],
+    *,
+    reverse: bool = False,
 ) -> List[ComparableContentT]: ...
 @overload
-def levelorder(tree: BinaryTree[_T]) -> List[_T]: ...
+def levelorder(tree: BinaryTree[_T], *, reverse: bool = False) -> List[_T]: ...
 @overload
 def levelorder(
     tree: BinarySearchTree[ComparableContentT],
+    *,
+    reverse: bool = False,
 ) -> List[ComparableContentT]: ...
```

### Comparing `pynrw-1.2.0/nrw/algorithms/_searching.py` & `pynrw-1.3.0/nrw/algorithms/_searching.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/algorithms/_sorting.py` & `pynrw-1.3.0/nrw/algorithms/_sorting.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/algorithms/_traversal.py` & `pynrw-1.3.0/nrw/algorithms/_traversal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,127 @@
 """Traversierung für Binär Bäume."""
 
 from __future__ import annotations
 
 __all__: Final[tuple[str, ...]] = (
     "preorder",
     "inorder",
-    "reverse_inorder",
     "postorder",
     "levelorder",
+    "reverse_inorder",
 )
 
 from typing import Final, TypeVar
+from warnings import warn
 
 from nrw.datastructures import BinarySearchTree, BinaryTree, ComparableContentT, List
 
 _T = TypeVar("_T")
 
 
 def preorder(
     tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
+    *,
+    reverse: bool = False,
 ) -> List[_T | ComparableContentT]:
     result: List[_T | ComparableContentT] = List()
 
     if tree.is_empty:
         return result
 
-    result.append(tree.content)
-    result.concat(preorder(tree.left_tree))
-    result.concat(preorder(tree.right_tree))
+    if not reverse:
+        result.append(tree.content)
+        result.concat(preorder(tree.left_tree))
+        result.concat(preorder(tree.right_tree))
+    else:
+        result.append(tree.content)
+        result.concat(preorder(tree.right_tree))
+        result.concat(preorder(tree.left_tree))
 
     return result
 
 
 def inorder(
     tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
+    *,
+    reverse: bool = False,
 ) -> List[_T | ComparableContentT]:
     result: List[_T | ComparableContentT] = List()
 
     if tree.is_empty:
         return result
 
-    result.concat(preorder(tree.left_tree))
-    result.append(tree.content)
-    result.concat(preorder(tree.right_tree))
+    if not reverse:
+        result.concat(preorder(tree.left_tree))
+        result.append(tree.content)
+        result.concat(preorder(tree.right_tree))
+    else:
+        result.concat(preorder(tree.right_tree))
+        result.append(tree.content)
+        result.concat(preorder(tree.left_tree))
 
     return result
 
 
 def reverse_inorder(
     tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
-) -> List[_T | ComparableContentT]:
-    result: List[_T | ComparableContentT] = List()
-
-    if tree.is_empty:
-        return result
-
-    result.concat(preorder(tree.right_tree))
-    result.append(tree.content)
-    result.concat(preorder(tree.left_tree))
-
-    return result
+) -> List[_T | ComparableContentT]:  # pragma: no cover
+    warn("Use 'inorder(..., reverse=True)'", DeprecationWarning, stacklevel=2)
+    return inorder(tree, reverse=True)
 
 
 def postorder(
     tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
+    *,
+    reverse: bool = False,
 ) -> List[_T | ComparableContentT]:
     result: List[_T | ComparableContentT] = List()
 
     if tree.is_empty:
         return result
 
-    result.concat(preorder(tree.left_tree))
-    result.concat(preorder(tree.right_tree))
-    result.append(tree.content)
+    if not reverse:
+        result.concat(preorder(tree.left_tree))
+        result.concat(preorder(tree.right_tree))
+        result.append(tree.content)
+    else:
+        result.concat(preorder(tree.right_tree))
+        result.concat(preorder(tree.left_tree))
+        result.append(tree.content)
 
     return result
 
 
 def levelorder(
     tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
+    *,
+    reverse: bool = False,
 ) -> List[_T | ComparableContentT]:
     if tree.is_empty:
         return List()
 
     trees: List[BinaryTree[_T] | BinarySearchTree[ComparableContentT]] = List()
     trees.append(tree)
     trees.to_first()
     while trees.has_access:
         current_tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT] | None = (
             trees.content
         )
         assert current_tree is not None
-        if not current_tree.left_tree.is_empty:
-            trees.append(current_tree.left_tree)
-        if not current_tree.right_tree.is_empty:
-            trees.append(current_tree.right_tree)
+
+        if not reverse:
+            if not current_tree.left_tree.is_empty:
+                trees.append(current_tree.left_tree)
+            if not current_tree.right_tree.is_empty:
+                trees.append(current_tree.right_tree)
+        else:
+            if not current_tree.right_tree.is_empty:
+                trees.append(current_tree.right_tree)
+            if not current_tree.left_tree.is_empty:
+                trees.append(current_tree.left_tree)
         trees.next()
 
     result: List[_T | ComparableContentT] = List()
     trees.to_first()
     while trees.has_access:
         result.append(trees.content.content)
         trees.next()
```

### Comparing `pynrw-1.2.0/nrw/datastructures/__init__.py` & `pynrw-1.3.0/nrw/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/datastructures/__init__.pyi` & `pynrw-1.3.0/nrw/datastructures/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: skip-file
 __all__: Final[tuple[str, ...]] = (
     "Stack",
     "Queue",
     "List",
     "BinaryTree",
     "ComparableContent",
     "ComparableContentT",
```

### Comparing `pynrw-1.2.0/nrw/datastructures/_binary_search_tree.py` & `pynrw-1.3.0/nrw/datastructures/_binary_search_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,15 @@
         """Der Konstruktor erzeugt einen leeren Suchbaum."""
         self._node: _BSTNode[ComparableContentT] | None = None
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(node={self._node!r})"
 
     def __str__(self) -> str:
-        if self.is_empty:
-            return ""
-        return str(self._node)
+        return str(self._node) if not self.is_empty else ""
 
     @property
     def is_empty(self) -> bool:
         """Diese Anfrage liefert den Wahrheitswert `True`, wenn der Suchbaum leer ist,
         sonst liefert sie den Wert `False`.
         """
         return self._node is None
@@ -174,19 +172,17 @@
         return None  # pragma: no cover
 
     def _ancestor_of_small_right(self) -> BinarySearchTree[ComparableContentT]:
         """Die Methode liefert denjenigen Baum, dessen linker Nachfolger keinen linken
         Nachfolger mehr hat. Es ist also später möglich, in einem Baum im
         rechten Nachfolger den Vorgänger des linkesten Nachfolgers zu finden.
         """
-        return (
-            self
-            if self._node_of_left_successor._left.is_empty
-            else self._node._left._ancestor_of_small_right()
-        )
+        if self._node_of_left_successor._left.is_empty:
+            return self
+        return self._node._left._ancestor_of_small_right()
 
     @property
     def _node_of_left_successor(self) -> _BSTNode[ComparableContentT] | None:
         return self._node._left._node
 
     @property
     def _node_of_right_successor(self) -> _BSTNode[ComparableContentT] | None:
```

### Comparing `pynrw-1.2.0/nrw/datastructures/_binary_tree.py` & `pynrw-1.3.0/nrw/datastructures/_binary_tree.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/datastructures/_comparable_content.py` & `pynrw-1.3.0/nrw/datastructures/_comparable_content.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/datastructures/_edge.py` & `pynrw-1.3.0/nrw/datastructures/_edge.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/datastructures/_graph.py` & `pynrw-1.3.0/nrw/datastructures/_graph.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/datastructures/_list.py` & `pynrw-1.3.0/nrw/datastructures/_list.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/datastructures/_queue.py` & `pynrw-1.3.0/nrw/datastructures/_queue.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/datastructures/_stack.py` & `pynrw-1.3.0/nrw/datastructures/_stack.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/datastructures/_utils.py` & `pynrw-1.3.0/nrw/datastructures/_utils.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/nrw/datastructures/_vertex.py` & `pynrw-1.3.0/nrw/datastructures/_vertex.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.2.0/pynrw.egg-info/PKG-INFO` & `pynrw-1.3.0/pynrw.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.2.0
+Version: 1.3.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -15,27 +15,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: bandit; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: covdefaults; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pylint-pytest; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: tox; extra == "dev"
+Requires-Dist: mysql-connector-python
+Requires-Dist: pyodbc; platform_python_implementation == "CPython"
+Requires-Dist: pypyodbc; platform_python_implementation == "PyPy"
 
 # pynrw
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/realshouzy/pynrw/main.svg)](https://results.pre-commit.ci/latest/github/realshouzy/pynrw/main)
 [![pylint status](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml)
 [![test status](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml)
 [![CodeQL](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml)
@@ -44,20 +34,56 @@
 [![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/pynrw/releases)
 [![PyPI - Format](https://img.shields.io/pypi/format/pynrw)](https://pypi.org/project/pynrw/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/realshouzy/pynrw/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-This package implements the datastructures given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
+This package implements the datastructures and database classes given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
 
 **Dieses Package dient alleine zu Bildungszwecken und sollte nicht in Produktion genutzt werden!**
 
+## Installation
+
+```bash
+pip install pynrw
+```
+
+Alternativ:
+
+```bash
+pip install git+https://github.com/realshouzy/pynrw
+```
+
+## Beispiel
+
+```python
+from nrw.algorithms import quick_sort
+from nrw.datastructures import List
+
+lst: List[int] = List()
+
+for i in range(0, 10, -1):
+  lst.append(i)
+
+print(lst.content)  # None
+lst.to_first()
+print(lst.content)  # 9
+print(lst)  # List(9 -> 8 -> 7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1 -> 0)
+
+sorted_lst: List[int] = quick_sort(lst)
+sorted_lst.to_first()
+print(sorted_lst.content)  # 0
+print(sorted_lst)  # List(0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9)
+```
+
 ## Dokumentation
 
+### Datenstrukturen
+
 Dieses Package implementiert die Datenstrukturen nach den Vorgaben des Landes NRW in Python, zu finden in [`nrw.datastructures`](/nrw/datastructures/), d.s.:
 
 - [`List`](/nrw/datastructures/_list.py)
 - [`Stack`](/nrw/datastructures/_stack.py)
 - [`Queue`](/nrw/datastructures/_queue.py)
 - [`BinaryTree`](/nrw/datastructures/_binary_tree.py)
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
@@ -93,73 +119,62 @@
 
 Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
 
+### Algorithmen
+
 Zusätzlich enthält dieses Package nützliche Funktionen zum Sortieren, Suchen und Traversiern, zu finden in [`nrw.algorithms`](/nrw/algorithms/):
 
-- [`linear_search`](/nrw/algorithms/_searching.py)
-- [`depth_first_search`](/nrw/algorithms/_searching.py)
-- [`breadth_first_search`](/nrw/algorithms/_searching.py)
-- [`bubble_sort`](/nrw/algorithms/_sorting.py)
-- [`selection_sort`](/nrw/algorithms/_sorting.py)
-- [`insertion_sort`](/nrw/algorithms/_sorting.py)
-- [`merge_sort`](/nrw/algorithms/_sorting.py)
-- [`quick_sort`](/nrw/algorithms/_sorting.py)
-- [`preorder`](/nrw/algorithms/_traversal.py)
-- [`inorder`](/nrw/algorithms/_traversal.py)
-- [`reverse_inorder`](/nrw/algorithms/_traversal.py)
-- [`postorder`](/nrw/algorithms/_traversal.py)
-- [`levelorder`](/nrw/algorithms/_traversal.py)
+- [`linear_search`](/nrw/algorithms/_searching.py#L23)
+- [`depth_first_search`](/nrw/algorithms/_searching.py#L55)
+- [`breadth_first_search`](/nrw/algorithms/_searching.py#L64)
+- [`bubble_sort`](/nrw/algorithms/_sorting.py#L21)
+- [`selection_sort`](/nrw/algorithms/_sorting.py#L37)
+- [`insertion_sort`](/nrw/algorithms/_sorting.py#L67)
+- [`merge_sort`](/nrw/algorithms/_sorting.py#L86)
+- [`quick_sort`](/nrw/algorithms/_sorting.py#L141)
+- [`preorder`](/nrw/algorithms/_traversal.py#L19)
+- [`inorder`](/nrw/algorithms/_traversal.py#L41)
+- [`postorder`](/nrw/algorithms/_traversal.py#L63)
+- [`levelorder`](/nrw/algorithms/_traversal.py#L85)
+
+Die verschiedenen Traversierungen unterstützen auch Umkehrung.
+Allerdings muss annotiert werden, dass aufgrund der Vorgaben des Landes die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte kommen. Welche dies sind, wird dem Leser als Übung überlassen.
+
+### Datenbankklassen
+
+Analog zu den Datenstrukturen sind auch Datenbankklassen größtenteils semantisch identisch zur den Vorgaben des Landes.
+Die jeweiligen Klassen sind in [`nrw.database`](/nrw/database/) definiert:
+
+- [`sqlite.DatabaseConnector`](/nrw/database/sqlite.py)
+- [`mysql.DatabaseConnector`](/nrw/database/mysql.py)
+- [`msaccess.DatabaseConnector`](/nrw/database/msaccess.py)
+- [`QueryResult`](/nrw/database/_query_result.py)
+
+Hierbei ist zu beachten, dass der `DatabaseConnector` für MSAccess den Microsoft Access Driver benötigt und passwortgeschützte Datenbanken nicht unterstüzt.
+Des weiteren gilt für `QueryResult`, dass die Daten und die Spaltentypen nicht unbedingt als String wiedergegeben werden. Die Daten werden als Python-Äquivalenten Datentypen wiedergegeben, und für die Spaltentypen gilt:
+
+- SQLite: immer `None`, da SQLite dynamisch typisiert ist
+- MySQL: die entsprechenden Datentypen von MySQL als String
+- MSAccess: die entsprechenden Datentypen (Klassen) von Python
 
-Allerdings muss annotiert werden, dass aufgrund der Vorgaben des Landes die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte kommen. Welche dies sind, wird dem Leser als Übung überlassen. Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.
+### Allgemein
 
-Für Hilfe zum jeweiligen Objekt (gilt für alle oben genannte Objekte), z.B.:
+Für mehr Information zu einem beliebigen Objekt kann `help` genutzt werden, z.B.:
 
 ```python
 from nrw.datastructures import List
 help(List)
 help(List.insert)
 ```
 
-## Installation
-
-```bash
-pip install pynrw
-```
-
-Alternativ:
-
-```bash
-pip install git+https://github.com/realshouzy/pynrw.git
-```
-
-## Beispiel
-
-```python
-from nrw.algorithms import quick_sort
-from nrw.datastructures import List
-
-lst: List[int] = List()
-
-for i in range(0, 10, -1):
-  lst.append(i)
-
-print(lst.content)  # None
-lst.to_first()
-print(lst.content)  # 9
-print(lst)  # List(9 -> 8 -> 7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1 -> 0)
-
-sorted_lst: List[int] = quick_sort(lst)
-sorted_lst.to_first()
-print(sorted_lst.content)  # 0
-print(sorted_lst)  # List(0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9)
-```
+**Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.**
 
 ## Motivation
 
 Vereinfacht: Java, als Programmiersprache in der Bildung, ist eine schlechte Wahl, da ...
 
 - Java veraltet ist.
 - das rein objekt-orientierte Paradigma schlechthin unbrauchbar ist.
```

### Comparing `pynrw-1.2.0/pynrw.egg-info/SOURCES.txt` & `pynrw-1.3.0/pynrw.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 nrw/__init__.py
 nrw/__init__.pyi
 nrw/py.typed
 nrw/algorithms/__init__.py
 nrw/algorithms/__init__.pyi
 nrw/algorithms/_searching.py
 nrw/algorithms/_sorting.py
 nrw/algorithms/_traversal.py
+nrw/database/__init__.py
+nrw/database/_query_result.py
+nrw/database/_query_result.pyi
+nrw/database/msaccess.py
+nrw/database/msaccess.pyi
+nrw/database/mysql.py
+nrw/database/mysql.pyi
+nrw/database/sqlite.py
+nrw/database/sqlite.pyi
 nrw/datastructures/__init__.py
 nrw/datastructures/__init__.pyi
 nrw/datastructures/_binary_search_tree.py
 nrw/datastructures/_binary_tree.py
 nrw/datastructures/_comparable_content.py
 nrw/datastructures/_edge.py
 nrw/datastructures/_graph.py
```

### Comparing `pynrw-1.2.0/pyproject.toml` & `pynrw-1.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -27,42 +27,26 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
-dynamic = ["version"]
-
-[project.optional-dependencies]
-# keep in sync with requirements-dev.txt
-dev = [
-  "bandit",
-  "black",
-  "covdefaults",
-  "coverage",
-  "isort",
-  "mypy",
-  "pre-commit",
-  "pylint",
-  "pylint-pytest",
-  "pytest",
-  "ruff",
-  "tox",
-]
+dynamic = ["version", "dependencies"]
 
 [tool.setuptools]
 license-files = ["LICENSE"]
 platforms = ["any"]
 
 [tool.setuptools.package-data]
 datastructures = ["py.typed", "*.pyi"]
 
 [tool.setuptools.dynamic]
 version = { attr = "nrw.__version__" }
+dependencies = { file = "requirements.txt" }
 
 [tool.black]
 target-version = ["py312", "py311", "py310", "py39", "py38"]
 line-length = 88
 
 [tool.isort]
 profile = "black"
@@ -113,31 +97,41 @@
 lint.fixable = ["ALL"]
 lint.unfixable = []
 show-fixes = true
 target-version = "py312"
 line-length = 88
 
 [tool.ruff.lint.extend-per-file-ignores]
-"./tests/*_test.py" = ["SLF001", "D100", "D103", "PLR2004"]
+"./tests/*_test.py" = ["SLF001", "D100", "D103", "PLR2004", "D102"]
 "./tests/*.py" = ["D104"]
+"./nrw/database/*.py" = ["BLE001", "PLR0913", "ARG002"]
+"./nrw/database/*.pyi" = ["PLR0913"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["nrw"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
 
 [tool.pylint]
-disable = ["C0116", "R0801", "W0212", "R0903", "C0114"]
+disable = ["C0116", "R0801", "W0212", "R0903", "C0114", "I1101", "C0301"]
 load-plugins = "pylint_pytest"
 
 [tool.bandit]
 skips = ["B101"]
 exclude_dirs = ["tests"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 python_files = ["*_test.py"]
 
 [tool.coverage.run]
+omit = ["./tests/*"]
 plugins = ["covdefaults"]
+
+[tool.coverage.report]
+exclude_also = [
+  "except Exception as exception:",
+  "if self._connection is None:",
+]
+fail_under = 95
```

