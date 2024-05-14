# Comparing `tmp/pytest_allure_id2history-0.1.1-py3-none-any.whl.zip` & `tmp/pytest_allure_id2history-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4972 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      788 b- defN 24-May-11 10:38 pytest_allure_id2history/listener.py
+Zip file size: 5199 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      859 b- defN 24-May-14 01:42 pytest_allure_id2history/listener.py
 -rw-rw-rw-  2.0 fat      418 b- defN 24-May-11 09:13 pytest_allure_id2history/plugin.py
--rw-rw-rw-  2.0 fat     1114 b- defN 24-May-11 10:44 pytest_allure_id2history-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4899 b- defN 24-May-11 10:44 pytest_allure_id2history-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 10:44 pytest_allure_id2history-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       63 b- defN 24-May-11 10:44 pytest_allure_id2history-0.1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       25 b- defN 24-May-11 10:44 pytest_allure_id2history-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      765 b- defN 24-May-11 10:44 pytest_allure_id2history-0.1.1.dist-info/RECORD
-8 files, 8164 bytes uncompressed, 3600 bytes compressed:  55.9%
+-rw-rw-rw-  2.0 fat     1114 b- defN 24-May-14 06:47 pytest_allure_id2history-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5288 b- defN 24-May-14 06:47 pytest_allure_id2history-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-14 06:47 pytest_allure_id2history-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       63 b- defN 24-May-14 06:47 pytest_allure_id2history-0.1.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       25 b- defN 24-May-14 06:47 pytest_allure_id2history-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      765 b- defN 24-May-14 06:47 pytest_allure_id2history-0.1.2.dist-info/RECORD
+8 files, 8624 bytes uncompressed, 3827 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: pytest_allure_id2history/listener.py
 Comment: 
 
 Filename: pytest_allure_id2history/plugin.py
 Comment: 
 
-Filename: pytest_allure_id2history-0.1.1.dist-info/LICENSE
+Filename: pytest_allure_id2history-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pytest_allure_id2history-0.1.1.dist-info/METADATA
+Filename: pytest_allure_id2history-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pytest_allure_id2history-0.1.1.dist-info/WHEEL
+Filename: pytest_allure_id2history-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_allure_id2history-0.1.1.dist-info/entry_points.txt
+Filename: pytest_allure_id2history-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_allure_id2history-0.1.1.dist-info/top_level.txt
+Filename: pytest_allure_id2history-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pytest_allure_id2history-0.1.1.dist-info/RECORD
+Filename: pytest_allure_id2history-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_allure_id2history/listener.py

```diff
@@ -1,9 +1,8 @@
 from typing import TYPE_CHECKING
-from allure_commons.utils import md5
 import pytest
 if TYPE_CHECKING:
     from allure_pytest.listener import AllureListener
 
 
 class AllureOverwriteListener:
     def __init__(self, config, allure_listener: 'AllureListener'):
@@ -14,8 +13,10 @@
     def pytest_runtest_teardown(self, item):
         yield
         if hasattr(item, 'callspec'):
             case_id = item.callspec.id
             # noinspection PyProtectedMember
             uuid = self._allure_listener._cache.get(item.nodeid)
             test_result = self._allure_listener.allure_logger.get_test(uuid)
-            test_result.historyId = md5(test_result.fullName, case_id)
+            if hasattr(test_result, 'historyId'):
+                from allure_commons.utils import md5
+                test_result.historyId = md5(test_result.fullName, case_id)
```

## Comparing `pytest_allure_id2history-0.1.1.dist-info/LICENSE` & `pytest_allure_id2history-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytest_allure_id2history-0.1.1.dist-info/METADATA` & `pytest_allure_id2history-0.1.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-allure-id2history
-Version: 0.1.1
+Version: 0.1.2
 Summary: Overwrite allure history id with testcase full name and testcase id if testcase has id, exclude parameters.
 Author-email: pytest-allure-id2history <ryaningli@foxmail.com>
 Maintainer-email: pytest-allure-id2history <ryaningli@foxmail.com>
 License: 
         The MIT License (MIT)
         
         Copyright (c) 2024 pytest-allure-id2history
@@ -43,14 +43,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pytest >=6.2.0
+Requires-Dist: allure-pytest >=2.4.0
 
 ========================
 pytest-allure-id2history
 ========================
 
 .. image:: https://img.shields.io/pypi/v/pytest-allure-id2history.svg
     :target: https://pypi.org/project/pytest-allure-id2history
@@ -64,41 +65,41 @@
     :target: https://github.com/Ryaningli/pytest-allure-id2history/actions/workflows/main.yml
     :alt: See Build Status on GitHub Actions
 
 Overwrite allure history id with testcase full name and testcase id if testcase has id, exclude parameters.
 
 ----
 
-This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
-
-
-Features
---------
-
-* TODO
-
-
-Requirements
-------------
-
-* TODO
+When the library is not installed,the ``historyId`` of the test cases generated by ``Allure`` is based on dynamic parameters within the test case, and each execution is not considered the same test case. After installing the library, when a test case id is configured, even with dynamic parameters, it will be recognized as the same test case.
 
 
 Installation
 ------------
 
 You can install "pytest-allure-id2history" via `pip`_ from `PyPI`_::
 
     $ pip install pytest-allure-id2history
 
 
 Usage
 -----
 
-* TODO
+::
+
+    import random
+    import pytest
+
+
+    @pytest.mark.parametrize('arg', [
+        random.randint(0, 9999)
+    ], ids=['some-id'])
+    def test_foo(arg):
+        print(f'Testing foo with {arg}')
+
+
 
 Contributing
 ------------
 Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
 License
```

## Comparing `pytest_allure_id2history-0.1.1.dist-info/RECORD` & `pytest_allure_id2history-0.1.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pytest_allure_id2history/listener.py,sha256=_nRlxaiajR2kHkizVKBRjMGtvLeA0J4UG-Vj3bYZCGw,788
+pytest_allure_id2history/listener.py,sha256=bBNVevqk4JKhgbSyq_1Ky2DgEdODGMqDSzjHLOYFLjg,859
 pytest_allure_id2history/plugin.py,sha256=UPZ9K1QYEfCZMuu9GElNe8-WEdDbhPg_cyB9kpuk0TQ,418
-pytest_allure_id2history-0.1.1.dist-info/LICENSE,sha256=uK6dHuXIXsMysbYjwvri76N9Aa9CQ41g7Q2OVZ9GeRM,1114
-pytest_allure_id2history-0.1.1.dist-info/METADATA,sha256=5KUcmfkbZbiCP3vED_Ok6tMTkibH--Ln2KlLnK712HU,4899
-pytest_allure_id2history-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pytest_allure_id2history-0.1.1.dist-info/entry_points.txt,sha256=BQ3JVuPzIPCa6eRDxMwxGgCrgc-2WjcwxMqSAa5HZM4,63
-pytest_allure_id2history-0.1.1.dist-info/top_level.txt,sha256=-H4IrGMjJsWtOeT9ucH7cCZf9JYairZTWd1isvhDe6k,25
-pytest_allure_id2history-0.1.1.dist-info/RECORD,,
+pytest_allure_id2history-0.1.2.dist-info/LICENSE,sha256=uK6dHuXIXsMysbYjwvri76N9Aa9CQ41g7Q2OVZ9GeRM,1114
+pytest_allure_id2history-0.1.2.dist-info/METADATA,sha256=rUW-PYD_fauZimOXBdiCCpBNHmwQWxIiWH0rSkQwvVo,5288
+pytest_allure_id2history-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pytest_allure_id2history-0.1.2.dist-info/entry_points.txt,sha256=BQ3JVuPzIPCa6eRDxMwxGgCrgc-2WjcwxMqSAa5HZM4,63
+pytest_allure_id2history-0.1.2.dist-info/top_level.txt,sha256=-H4IrGMjJsWtOeT9ucH7cCZf9JYairZTWd1isvhDe6k,25
+pytest_allure_id2history-0.1.2.dist-info/RECORD,,
```

