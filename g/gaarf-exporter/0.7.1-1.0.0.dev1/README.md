# Comparing `tmp/gaarf-exporter-0.7.1.tar.gz` & `tmp/gaarf-exporter-1.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaarf-exporter-0.7.1.tar", last modified: Mon May 13 11:19:49 2024, max compression
+gzip compressed data, was "gaarf-exporter-1.0.0.dev1.tar", last modified: Tue May 14 07:25:05 2024, max compression
```

## Comparing `gaarf-exporter-0.7.1.tar` & `gaarf-exporter-1.0.0.dev1.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.139074 gaarf-exporter-0.7.1/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6912 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6443 2024-03-26 12:03:46.000000 gaarf-exporter-0.7.1/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/gaarf_exporter/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1287 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/alert.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/alert_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2395 2024-05-02 16:45:02.000000 gaarf-exporter-0.7.1/gaarf_exporter/bootstrap.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    35232 2024-05-13 11:14:49.000000 gaarf-exporter-0.7.1/gaarf_exporter/collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4093 2024-05-09 20:50:51.000000 gaarf-exporter-0.7.1/gaarf_exporter/config.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7971 2024-05-13 11:13:48.000000 gaarf-exporter-0.7.1/gaarf_exporter/main.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2825 2024-05-08 08:46:57.000000 gaarf-exporter-0.7.1/gaarf_exporter/query_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      908 2024-03-15 19:34:24.000000 gaarf-exporter-0.7.1/gaarf_exporter/search_collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    13737 2024-05-13 11:13:48.000000 gaarf-exporter-0.7.1/gaarf_exporter/target.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-03-19 10:33:47.000000 gaarf-exporter-0.7.1/gaarf_exporter/util.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6912 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      885 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       56 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-05-13 11:19:49.000000 gaarf-exporter-0.7.1/gaarf_exporter.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-05-13 11:19:49.139074 gaarf-exporter-0.7.1/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1552 2024-05-10 05:03:01.000000 gaarf-exporter-0.7.1/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:38:01.000000 gaarf-exporter-0.7.1/tests/__init__.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/tests/end-to-end/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/end-to-end/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      504 2024-05-13 11:14:49.000000 gaarf-exporter-0.7.1/tests/end-to-end/test_gaarf_exporter.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-13 11:19:49.135074 gaarf-exporter-0.7.1/tests/unit/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/unit/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/unit/test_alerts.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3854 2024-05-13 11:13:48.000000 gaarf-exporter-0.7.1/tests/unit/test_collectors.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3724 2024-05-08 13:54:33.000000 gaarf-exporter-0.7.1/tests/unit/test_config.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/unit/test_exporter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3525 2024-05-08 08:46:57.000000 gaarf-exporter-0.7.1/tests/unit/test_query_elements.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    20353 2024-05-09 20:50:51.000000 gaarf-exporter-0.7.1/tests/unit/test_target.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-05-02 15:51:30.000000 gaarf-exporter-0.7.1/tests/unit/test_util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6443 2024-03-26 12:03:46.000000 gaarf-exporter-1.0.0.dev1/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.103046 gaarf-exporter-1.0.0.dev1/gaarf_exporter/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-01-26 13:03:47.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1293 2024-05-13 21:01:08.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/alert.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1886 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/alert_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2395 2024-05-02 16:45:02.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/bootstrap.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      450 2024-05-13 15:50:58.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/conversion_action.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      672 2024-05-13 19:59:40.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/disapprovals.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      433 2024-05-13 15:50:58.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/mapping.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      340 2024-05-13 12:26:59.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collector_definitions/performance.yaml
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6541 2024-05-14 07:00:12.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11841 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     8246 2024-05-14 06:59:31.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/main.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2825 2024-05-08 08:46:57.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/query_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    16979 2024-05-13 21:10:46.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/target.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2192 2024-03-19 10:33:47.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter/util.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7178 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1017 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       60 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       56 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       21 2024-05-14 07:25:05.000000 gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       38 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1848 2024-05-14 06:43:50.000000 gaarf-exporter-1.0.0.dev1/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:38:01.000000 gaarf-exporter-1.0.0.dev1/tests/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/tests/end-to-end/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/end-to-end/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3308 2024-05-14 07:17:45.000000 gaarf-exporter-1.0.0.dev1/tests/end-to-end/test_gaarf_exporter.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2024-05-14 07:25:05.107046 gaarf-exporter-1.0.0.dev1/tests/unit/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/unit/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2490 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_alerts.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6493 2024-05-14 06:59:03.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_collectors.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4474 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_exporter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3525 2024-05-08 08:46:57.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_query_elements.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    19671 2024-05-13 20:58:11.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_target.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2565 2024-05-02 15:51:30.000000 gaarf-exporter-1.0.0.dev1/tests/unit/test_util.py
```

### Comparing `gaarf-exporter-0.7.1/PKG-INFO` & `gaarf-exporter-1.0.0.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: gaarf-exporter
-Version: 0.7.1
-Author: Google Inc. (gTech gPS CSE team)
-Author-email: no-reply@google.com
-License: Apache 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-
 # gaarf exporter
 
 Prometheus exporter for Google Ads metrics with customizable metrics collectors.
 
 ## Installation and usage
 
 ### Locally
```

### Comparing `gaarf-exporter-0.7.1/README.md` & `gaarf-exporter-1.0.0.dev1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: gaarf-exporter
+Version: 1.0.0.dev1
+Author: Google Inc. (gTech gPS CSE team)
+Author-email: no-reply@google.com
+License: Apache 2.0
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Description-Content-Type: text/markdown
+
 # gaarf exporter
 
 Prometheus exporter for Google Ads metrics with customizable metrics collectors.
 
 ## Installation and usage
 
 ### Locally
```

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter/alert.py` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter/alert.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 # limitations under the License.
 '''Module for building Prometheus alert.'''
 from __future__ import annotations
 
 import yaml
 
 from gaarf_exporter.alert_elements import AlertRule
-from gaarf_exporter.target import Target
+from gaarf_exporter.target import Collector
 
 
 class Alert:
 
   def __init__(self,
                name: str,
                alert_rule: AlertRule,
                labels: str | None = None,
                duration: str = '1h',
-               target: Target | None = None) -> None:
+               target: Collector | None = None) -> None:
     self.name = name
     self.alert_rule = str(alert_rule)
     self.labels = labels
     self.duration = duration
     self.target = target
 
   @property
```

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter/alert_elements.py` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter/alert_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter/bootstrap.py` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter/exporter.py` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter/main.py` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 import prometheus_client
 import smart_open
 import yaml
 from gaarf.cli import utils as gaarf_utils
 
 from gaarf_exporter import bootstrap
 from gaarf_exporter import collectors
-from gaarf_exporter import config as exporter_config
 from gaarf_exporter import exporter
 from gaarf_exporter import util
 
 
 def main() -> None:
   parser = argparse.ArgumentParser()
   parser.add_argument('--account', dest='account', default=None)
@@ -73,35 +72,33 @@
       loglevel=args.loglevel.upper(), logger_type=args.logger)
 
   params = gaarf_utils.ParamsParser([
       'macro',
       'sql',
       'template',
   ]).parse(args_bag[1])
-  collectors_registry = collectors.Registry()
+  collectors_registry = collectors.Registry.from_collector_definitions()
   macros = params.get('macro', {})
   if config_file := args.config:
     with smart_open.open(config_file, encoding='utf-8') as f:
       config = yaml.safe_load(f)
       queries = config.get('queries')
   else:
     if not (active_collectors := collectors_registry.find_collectors(
         args.collectors)):
       logger.warning('Failed to get "%s" collectors, using default ones',
                      args.collectors)
       active_collectors = collectors_registry.default_collectors
     if macros:
       active_collectors.customize(macros)
-    config = exporter_config.Config(active_collectors.targets)
-    queries = config.queries
-  for query_name, query in queries.items():
-    if relative_metrics := util.find_relative_metrics(query['query']):
+  for collector in active_collectors:
+    if relative_metrics := util.find_relative_metrics(collector.query):
       logger.warning(
           'In query %s, relative metrics: [%s] are found, which might '
-          'not be useful.', query_name, ', '.join(relative_metrics))
+          'not be useful.', collector.name, ', '.join(relative_metrics))
   runtime_options = {
       'exclude_queries':
           args.exclude_queries.split(',') if args.exclude_queries else None,
       'include_queries':
           args.include_queries.split(',') if args.include_queries else None,
   }
 
@@ -138,50 +135,56 @@
     if accounts and iterations_left == 0:
       accounts = report_fetcher.expand_mcc(args.account)
       iterations_left = args.iterations_left
     start_export_time = time()
     if not args.config:
       if macros:
         active_collectors.customize(macros)
-      config = exporter_config.Config(active_collectors.targets)
-      queries = config.queries
-    for name, content in queries.items():
-      if not (query_text := content.get('query')):
-        raise ValueError(f'Missing query text for query "{name}"')
+    for collector in active_collectors:
+      if not (query_text := collector.query):
+        raise ValueError(f'Missing query text for query "{collector.name}"')
       if include_queries := runtime_options.get('include_queries'):
-        if name not in include_queries:
+        if collector.name not in include_queries:
           continue
       if exclude_queries := runtime_options.get('exclude_queries'):
-        if name in exclude_queries:
+        if collector.name in exclude_queries:
           continue
-      suffix = content.get('suffix') or name
       logger.info('Beginning export')
       if not accounts:
+        logging.info('Starting fake export for query "[%s]"', collector.name)
         report = report_fetcher.fetch(query_text, accounts)
+        logging.info('Ending export for query "[%s]"', collector.name)
       else:
         with futures.ThreadPoolExecutor() as executor:
           future_to_account = {
-              executor.submit(report_fetcher.fetch, query_text, account):
+              executor.submit(report_fetcher.fetch, collector.query, account):
                   account for account in accounts
           }
           for future in futures.as_completed(future_to_account):
             account = future_to_account[future]
+            logging.info('Started fetching for query "[%s]" for account "[%s]"',
+                         collector.name, account)
             start = time()
             report = future.result()
             end = time()
+            logging.info('Ended fetching for query "[%s]" for account "[%s]"',
+                         collector.name, account)
             gaarf_exporter.report_fetcher_gauge.labels(
-                collector=name, account=account).set(end - start)
+                collector=collector.name, account=account).set(end - start)
             if dependencies.get('convert_fake_report'):
               report.is_fake = False
             logging.info('Started export for query "[%s]" for account "[%s]"',
-                         name, account)
+                         collector.name, account)
             gaarf_exporter.export(
-                report=report, suffix=suffix, collector=name, account=account)
+                report=report,
+                suffix=collector.suffix,
+                collector=collector.name,
+                account=account)
             logging.info('Ended export for query "[%s]" for account "[%s]"',
-                         name, account)
+                         collector.name, account)
     logger.info('Export completed')
     end_export_time = time()
     gaarf_exporter.total_export_time_gauge.set(end_export_time -
                                                start_export_time)
     gaarf_exporter.delay_gauge.set(args.delay * 60)
 
     if gaarf_exporter.pushgateway_url:
```

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter/query_elements.py` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter/query_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter/target.py` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter/target.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,46 +7,75 @@
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines Target class and corresponding helper methods.
+"""Defines Collector class and corresponding helper methods.
 
-Target serves an important roles of building Google Ads queries from set of
+Collector serves an important roles of building Google Ads queries from set of
 diverse elements: metrics, dimensions, filters, resource names, etc.
 
-Target can be:
+Collector can be:
   * similar (sharing the same metrics, dimensions and filters) which allows
     to perform similar target deduplication with the lowest common level.
   * equal (sharing the same attributes) - useful for checking target presence
     in the sets.
 
-Metrics, dimensions and filters of a Target can be dynamically changed thus
-allowing Target customization at the runtime.
+Metrics, dimensions and filters of a Collector can be dynamically changed thus
+allowing Collector customization at the runtime.
 """
 from __future__ import annotations
 
-import copy
 import dataclasses
 import enum
-import itertools
+from collections.abc import Mapping
+from collections.abc import MutableSequence
 from collections.abc import Sequence
+from datetime import datetime
+
+from gaarf.cli import utils as gaarf_utils
 
 from gaarf_exporter import query_elements
 from gaarf_exporter import util
 
+_DEFAULT_METRICS = [
+    query_elements.Field('clicks'),
+    query_elements.Field('impressions'),
+    query_elements.Field('conversions'),
+    query_elements.Field('cost_micros / 1e6', 'cost')
+]
+
+_DEFAULT_CONVERSION_SPLIT_METRICS = [
+    query_elements.Field('all_conversions'),
+    query_elements.Field('all_conversions_value'),
+]
+
+_DEFAULT_CONVERSION_SPLIT_DIMENSIONS = [
+    query_elements.Field('segments.conversion_action_category',
+                         'conversion_category'),
+    query_elements.Field('segments.conversion_action_name', 'conversion_name'),
+    query_elements.Field(
+        'segments.conversion_action', 'conversion_id',
+        query_elements.Customizer(query_elements.CustomizerTypeEnum.INDEX, '0'))
+]
+
+_DEFAULT_CONVERSION_SPLIT_FILTERS = [
+    'metrics.all_conversions > 0',
+    'segments.date DURING TODAY',
+]
+
 
-class TargetLevel(enum.IntEnum):
+class CollectorLevel(enum.IntEnum):
   """Represents minimal level of entity.
 
-  TargetLevel regulates which entity id (ad_id, ad_group_id, campaign_id, etc.)
+  CollectorLevel regulates which entity id (ad_id, ad_group_id, campaign_id, etc.)
   is associated with metrics and dimensions for a given target.
-  Target levels are ordered hierarchically to support comparison operations.
+  Collector levels are ordered hierarchically to support comparison operations.
   """
   UNKNOWN = 0
   AD_GROUP_AD_ASSET = 1
   AD_GROUP_AD = 2
   AD_GROUP = 3
   CAMPAIGN = 4
   CUSTOMER = 5
@@ -56,17 +85,17 @@
   def contains(cls, *keys: str) -> bool:
     """Checks whether supplied keys are valid enum names."""
     return all(key.upper() in cls.__members__ for key in keys)
 
 
 @dataclasses.dataclass
 class LevelInfo:
-  """Stores meta information for a particular TargetLevel.
+  """Stores meta information for a particular CollectorLevel.
 
-  This meta information is used to correctly build query in the Target.
+  This meta information is used to correctly build query in the Collector.
 
   Attributes:
     resource_name: Name of Google Ads reporting resource.
     id: Field name for entity id (i.e. ad_group.id, campaign.id) .
     id_alias: Alias for entity_id (i.e ad_group_id, campaign_id).
     name: Field name for entity content (i.e ad_group.name, campaign.name).
     name_alias: Alias for entity content (i.e ad_group_name, campaign_name).
@@ -84,41 +113,41 @@
     return f'{self.id} AS {self.id_alias}'
 
   def to_field(self) -> query_elements.Field:
     """Builds Field from level meta information."""
     return query_elements.Field(name=self.id, alias=self.id_alias)
 
 
-_LEVELS = {
-    TargetLevel.AD_GROUP_AD_ASSET:
+LEVELS = {
+    CollectorLevel.AD_GROUP_AD_ASSET:
         LevelInfo('ad_group_ad_asset_view', 'asset.id', 'asset_id',
                   'asset.name', 'asset',
                   'ad_group_ad_asset_view.enabled = TRUE'),
-    TargetLevel.AD_GROUP_AD:
+    CollectorLevel.AD_GROUP_AD:
         LevelInfo('ad_group_ad', 'ad_group_ad.ad.id', 'ad_id',
                   'ad_group_ad.ad.name', 'ad_name',
                   'ad_group_ad.status = ENABLED'),
-    TargetLevel.AD_GROUP:
+    CollectorLevel.AD_GROUP:
         LevelInfo('ad_group', 'ad_group.id', 'ad_group_id', 'ad_group.name',
                   'ad_group_name', 'ad_group.status = ENABLED'),
-    TargetLevel.CAMPAIGN:
+    CollectorLevel.CAMPAIGN:
         LevelInfo('campaign', 'campaign.id', 'campaign_id', 'campaign.name',
                   'campaign_name', 'campaign.status = ENABLED'),
-    TargetLevel.CUSTOMER:
+    CollectorLevel.CUSTOMER:
         LevelInfo('customer', 'customer.id', 'customer_id',
                   'customer.descriptive_name', 'account_name',
                   'customer.status = ENABLED'),
-    TargetLevel.MCC:
+    CollectorLevel.MCC:
         LevelInfo('customer', 'customer.id', 'customer_id',
                   'customer.descriptive_name', 'account_name',
                   'customer.status = ENABLED'),
 }
 
 
-class Target:
+class Collector:
   """Represents collection of query elements needed to build a Google Ads query.
 
   Attributes:
     name: Unique identifier of a target.
     level: Minimal entity level in the target (ad_group, campaign, customer).
     metrics: All metrics (started with `metrics.`) associated with the target.
     dimensions: All segments and resources associated with the target.
@@ -127,45 +156,75 @@
     query: Full text of the query to be sent to Google Ads API.
     suffix: Optional custom identifier to the target.
   """
 
   def __init__(self,
                name: str | None = None,
                metrics: str | list[query_elements.Field] | None = None,
-               level: TargetLevel | None = TargetLevel.AD_GROUP,
+               level: CollectorLevel | None = CollectorLevel.AD_GROUP,
                resource_name: str | None = None,
                dimensions: str | list[query_elements.Field] | None = None,
                filters: str | None = None,
-               suffix: str | None = None) -> None:
-    """Initializes Target.
+               suffix: str | None = None,
+               query: strr | None = None) -> None:
+    """Initializes Collector.
 
     Args:
       name: Unique identifier of a target.
       metrics: All metrics (started with `metrics.`) associated with the target.
       level: Minimal entity level in the target (ad_group, campaign, customer).
       resource_name: Name of resource to get data from (used in FROM statement).
       dimensions: All segments and resources associated with the target.
       filters: Text conditions for limiting the query.
       suffix: Optional custom identifier to the target.
+      query: Full query_text.
     """
     self.name = name
     self._level = level
     self._resource_name = resource_name
     self._filters = filters
     self._metrics = self._init_fields(metrics, 'metrics')
     self._dimensions = self._init_fields(dimensions)
     self.suffix = suffix if suffix else name
+    self._query = query
+
+  @classmethod
+  def from_definition(cls, definition: dict) -> Collector:
+    query_spec = definition.get('query_spec', {})
+    # query = definition.get('query')
+    if level_string := query_spec.get('level'):
+      level = CollectorLevel[level_string.upper()]
+    else:
+      level = CollectorLevel.AD_GROUP
+    return cls(
+        name=definition.get('name'),
+        suffix=definition.get('suffix'),
+        metrics=query_spec.get('metrics'),
+        dimensions=query_spec.get('dimensions'),
+        filters=query_spec.get('filters'),
+        resource_name=query_spec.get('resource_name'),
+        level=level)
+
+  def create_conv_collector(self) -> Collector:
+    return Collector(
+        name=f'{self.name}_conversion_split',
+        suffix=self.suffix,
+        level=self.level,
+        metrics=_DEFAULT_CONVERSION_SPLIT_METRICS,
+        dimensions=_DEFAULT_CONVERSION_SPLIT_DIMENSIONS,
+        resource_name=self.resource_name,
+        filters=_DEFAULT_CONVERSION_SPLIT_FILTERS)
 
   @property
-  def level(self) -> TargetLevel | None:
+  def level(self) -> CollectorLevel | None:
     """Represents entity level of a target."""
     return self._level
 
   @level.setter
-  def level(self, value: TargetLevel) -> None:
+  def level(self, value: CollectorLevel) -> None:
     """Changes saved level of a target."""
     self._level = value
 
   @property
   def metrics(self) -> set[query_elements.Field]:
     """Returns unique metrics."""
     return set(self._metrics)
@@ -209,18 +268,30 @@
 
     Raises:
       ValueError: If fields has non-aliased virtual column.
     """
     if not fields:
       return []
 
-    if fields and isinstance(fields, str):
+    if isinstance(fields, str):
       field_list = [
           query_elements.Field(name=field) for field in fields.split(',')
       ]
+    elif isinstance(fields, MutableSequence):
+      field_list = []
+      for field in fields:
+        if isinstance(field, query_elements.Field):
+          element = field
+        elif isinstance(field, Mapping):
+          for alias, values in field.items():
+            element = query_elements.Field(
+                name=values.get('field'), alias=alias)
+        else:
+          element = query_elements.Field(name=field)
+        field_list.append(element)
     else:
       field_list = fields
 
     if not prefix:
       return field_list
 
     for field in field_list:
@@ -240,171 +311,180 @@
       field.name = ' '.join(processed_tokens)
 
     return field_list
 
   @property
   def level_info(self) -> LevelInfo | None:
     """Returns meta information related to a target level."""
-    return _LEVELS.get(self.level)
+    return LEVELS.get(self.level)
 
   @property
-  def formatted_level(self) -> str:
+  def _formatted_level(self) -> str:
     """Returns formatted level as field name with alias."""
     if level_info := self.level_info:
       return f'{level_info.to_query_field()},\n'
     return ''
 
   @property
-  def formatted_metrics(self) -> str:
+  def _formatted_metrics(self) -> str:
     """Returns formatted metrics as field names with aliases."""
     if not self.metrics:
       return '\n'
     metrics_info = ',\n'.join(
         [field.to_query_field() for field in sorted(self.metrics)])
     return f'{metrics_info},\n'
 
   @property
-  def formatted_dimensions(self) -> str:
+  def _formatted_dimensions(self) -> str:
     """Returns formatted metrics as field names with aliases."""
     if not (dimensions := self.dimensions):
       return '\n'
     if level_info := self.level_info:
       dimensions = set(dimensions).difference(set([level_info.to_field()]))
     if not dimensions:
       return '\n'
     dimensions_info = ',\n'.join(
         [field.to_query_field() for field in sorted(dimensions)])
     return f'{dimensions_info},\n'
 
   @property
+  def _formatted_filters(self) -> str:
+    if not self._filters:
+      return 'segments.date DURING TODAY'
+    if isinstance(self._filters, MutableSequence):
+      return ' AND '.join(self._filters)
+    return self._filters
+
+  @property
   def resource_name(self) -> str:
     """Gets resource_name or infers it from target level."""
     if self._resource_name:
       return self._resource_name
     if level_info := self.level_info:
       return level_info.resource_name.lower()
     return self.level.name
 
   @property
   def query(self) -> str:
     """Formats query based on elements."""
-    return (f'SELECT {self.formatted_level}{self.formatted_metrics}'
-            f'{self.formatted_dimensions}'
+    if self._query:
+      return self._query
+    return (f'SELECT {self._formatted_level}{self._formatted_metrics}'
+            f'{self._formatted_dimensions}'
             f'FROM {self.resource_name}\n'
-            f'WHERE {self.filters}')
-
-  def is_similar(self, other: Target) -> bool:
-    """Compares similarity between two targets.
+            f'WHERE {self._formatted_filters}')
 
-    Similarity first checks whether two targets are coming from different
-    non TargetLevel specific resouce_names, if they are different then
-    targets are not similar.
-    Then is compares all  metrics, dimensions and filters between two targets.
+  def customize(self, kwargs: dict[str, str]) -> None:
+    if level := kwargs.get('level'):
+      self.level = CollectorLevel[level.upper()]
+    if (start_date := kwargs.get('start_date')) and (end_date :=
+                                                     kwargs.get('end_date')):
+      start_date = gaarf_utils.convert_date(start_date)
+      end_date = gaarf_utils.convert_date(end_date)
+      self.filters = self.filters.replace(
+          'DURING TODAY', f"BETWEEN '{start_date}' AND '{end_date}'")
+      n_days = (datetime.strptime(end_date, '%Y-%m-%d') -
+                datetime.strptime(start_date, '%Y-%m-%d')).days + 1
+      self.dimensions.add(query_elements.Field(str(n_days), 'n_days'))
+
+  def is_similar(self, other: Collector) -> bool:
+    """Compares similarity between two collectors.
+
+    Similarity first checks whether two collectors are coming from different
+    non CollectorLevel specific resource_names, if they are different then
+    collectors are not similar.
+    Then is compares all  metrics, dimensions and filters between two collectors.
 
     Returns:
-      Whether two targets are similar.
+      Whether two collectors are similar.
     """
-    if not other or not isinstance(other, Target):
+    if not other or not isinstance(other, Collector):
       return False
 
     if (self.resource_name != other.resource_name and
-        not (TargetLevel.contains(self.resource_name, other.resource_name))):
+        not (CollectorLevel.contains(self.resource_name, other.resource_name))):
       return False
     if (self.metrics, self.dimensions,
         self.filters) == (other.metrics, other.dimensions, other.filters):
       return True
     return False
 
-  def __eq__(self, other: Target) -> bool:
+  def generate_service_collector(self) -> ServiceCollector | None:
+    """Generates correct ServiceCollector based on provided level.
+
+     Based on level (AD_GROUP, CAMPAIGN, ACCOUNT, etc.) corresponding
+     ServiceCollector is created that contains all necessary mapping information
+     downstream. I.e. if 'level=AD_GROUP' then information on ad_group, campaign
+     and customer will be included in to the mapping.
+
+     Returns:
+      ServiceCollector called 'mapping' for an appropriate level.
+
+    """
+    if isinstance(self, ServiceCollector):
+      return None
+    if self.level == CollectorLevel.MCC:
+      level = CollectorLevel.CUSTOMER
+    else:
+      level = self.level
+    dimensions = []
+    filters = ''
+
+    for target_level in CollectorLevel:
+      if (target_level
+          not in (CollectorLevel.MCC, CollectorLevel.AD_GROUP_AD_ASSET) and
+          self.level <= target_level and
+          (level_info := LEVELS.get(target_level))):
+        dimensions.extend([
+            query_elements.Field(name=level_info.id, alias=level_info.id_alias),
+            query_elements.Field(
+                name=level_info.name, alias=level_info.name_alias),
+        ])
+        if filters:
+          filters = filters + ' AND ' + level_info.active_entities_filter
+        else:
+          filters = level_info.active_entities_filter
+
+    return ServiceCollector(
+        name='mapping',
+        dimensions=dimensions,
+        level=level,
+        filters=filters)
+
+  def __eq__(self, other: Collector) -> bool:
     """Compares two targets based on similarity, resource_name and level."""
     if not self.is_similar(other):
       return False
     if self.level != other.level:
       return False
     return True
 
-  def __lt__(self, other: Target) -> bool:
+  def __lt__(self, other: Collector) -> bool:
     """Compares targets by level values."""
     if self.level.value < other.level.value:
       return True
     return False
 
-  def __gt__(self, other: Target) -> bool:
+  def __gt__(self, other: Collector) -> bool:
     """Compares targets by level values."""
     if self.level.value > other.level.value:
       return True
     return False
 
   def __hash__(self):
     return hash(self.query)
 
 
-class ServiceTarget(Target):
+class ServiceCollector(Collector):
   """Helper class for targets without metrics."""
 
   @property
   def metrics(self) -> set[query_elements.Field]:
     """Returns default info metric."""
     return {
         query_elements.Field(name='1', alias='info'),
     }
 
   @metrics.setter
   def metrics(self, value: query_elements.Field) -> None:
     """Ensures that metrics cannot be overwritten."""
     raise ValueError('Cannot change value of "metrics"!')
-
-
-def create_default_service_target(level: TargetLevel) -> ServiceTarget:
-  """Generates correct ServiceTarget based on provided level.
-
-   Based on level (AD_GROUP, CAMPAIGN, ACCOUNT, etc.) corresponding
-   ServiceTarget is created that contains all necessary mapping information
-   downstream. I.e. if 'level=AD_GROUP' then information on ad_group, campaign
-   and customer will be included in to the mapping.
-
-   Returns:
-    ServiceTarget called 'mapping' for an appropriate level.
-
-  """
-  if level == TargetLevel.MCC:
-    level = TargetLevel.CUSTOMER
-  dimensions = []
-  filters = ''
-
-  for target_level in TargetLevel:
-    if (target_level not in (TargetLevel.MCC, TargetLevel.AD_GROUP_AD_ASSET) and
-        level <= target_level and (level_info := _LEVELS.get(target_level))):
-      dimensions.extend([
-          query_elements.Field(name=level_info.id, alias=level_info.id_alias),
-          query_elements.Field(
-              name=level_info.name, alias=level_info.name_alias),
-      ])
-      if filters:
-        filters = filters + ' AND ' + level_info.active_entities_filter
-      else:
-        filters = level_info.active_entities_filter
-
-  return ServiceTarget(
-      name='mapping', dimensions=dimensions, level=level, filters=filters)
-
-
-def targets_similarity_check(targets: list[Target]) -> list[Target]:
-  """Dedupicates targets.
-
-  If there are similar target in the list return only those with the lowest
-  level.
-
-  Args:
-    targets: Possible target values.
-
-  Returns:
-    Deduplicated targets.
-  """
-  cloned_targets = copy.deepcopy(targets)
-  combinations = itertools.combinations(targets, 2)
-  for target1, target2 in combinations:
-    if target1.is_similar(target2):
-      max_target = max(target1, target2)
-      if max_target in cloned_targets:
-        cloned_targets.remove(max_target)
-  return cloned_targets
```

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter/util.py` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter/util.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter.egg-info/PKG-INFO` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Metadata-Version: 2.1
 Name: gaarf-exporter
-Version: 0.7.1
+Version: 1.0.0.dev1
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 
 # gaarf exporter
```

### Comparing `gaarf-exporter-0.7.1/gaarf_exporter.egg-info/SOURCES.txt` & `gaarf-exporter-1.0.0.dev1/gaarf_exporter.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 README.md
 setup.py
 gaarf_exporter/__init__.py
 gaarf_exporter/alert.py
 gaarf_exporter/alert_elements.py
 gaarf_exporter/bootstrap.py
 gaarf_exporter/collectors.py
-gaarf_exporter/config.py
 gaarf_exporter/exporter.py
 gaarf_exporter/main.py
 gaarf_exporter/query_elements.py
-gaarf_exporter/search_collectors.py
 gaarf_exporter/target.py
 gaarf_exporter/util.py
 gaarf_exporter.egg-info/PKG-INFO
 gaarf_exporter.egg-info/SOURCES.txt
 gaarf_exporter.egg-info/dependency_links.txt
 gaarf_exporter.egg-info/entry_points.txt
 gaarf_exporter.egg-info/requires.txt
 gaarf_exporter.egg-info/top_level.txt
+gaarf_exporter/collector_definitions/conversion_action.yaml
+gaarf_exporter/collector_definitions/disapprovals.yaml
+gaarf_exporter/collector_definitions/mapping.yaml
+gaarf_exporter/collector_definitions/performance.yaml
 tests/__init__.py
 tests/end-to-end/__init__.py
 tests/end-to-end/test_gaarf_exporter.py
 tests/unit/__init__.py
 tests/unit/test_alerts.py
 tests/unit/test_collectors.py
-tests/unit/test_config.py
 tests/unit/test_exporter.py
 tests/unit/test_query_elements.py
 tests/unit/test_target.py
 tests/unit/test_util.py
```

### Comparing `gaarf-exporter-0.7.1/tests/unit/test_alerts.py` & `gaarf-exporter-1.0.0.dev1/tests/unit/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.1/tests/unit/test_exporter.py` & `gaarf-exporter-1.0.0.dev1/tests/unit/test_exporter.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.1/tests/unit/test_query_elements.py` & `gaarf-exporter-1.0.0.dev1/tests/unit/test_query_elements.py`

 * *Files identical despite different names*

### Comparing `gaarf-exporter-0.7.1/tests/unit/test_target.py` & `gaarf-exporter-1.0.0.dev1/tests/unit/test_target.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,36 +36,36 @@
     print('\n')
     print(sorted_actual_sql_tokens)
     print(sorted_expected_sql_tokens)
 
   assert sorted_actual_sql_tokens == sorted_expected_sql_tokens
 
 
-class TestTarget:
+class TestCollector:
 
-  class TestTargetQuery:
+  class TestCollectorQuery:
 
     def test_simple_target_creates_correct_query(self):
-      target = query_target.Target(
+      target = query_target.Collector(
           name='simple',
           metrics='impressions',
-          level=query_target.TargetLevel.AD_GROUP)
+          level=query_target.CollectorLevel.AD_GROUP)
       expected_sql = """
         SELECT
             ad_group.id AS ad_group_id,
             metrics.impressions AS impressions,
         FROM ad_group
         WHERE segments.date DURING TODAY
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
     def test_complex_target_creates_correct_query(self):
-      target = query_target.Target(
+      target = query_target.Collector(
           metrics='impressions,clicks',
-          level=query_target.TargetLevel.AD_GROUP,
+          level=query_target.CollectorLevel.AD_GROUP,
           dimensions=[
               query_elements.Field(
                   name='segments.conversion_action',
                   alias='conversion_id',
                   customizer=query_elements.Customizer(
                       query_elements.CustomizerTypeEnum.INDEX, '0')),
               query_elements.Field(
@@ -80,24 +80,24 @@
             search_terms_view.search_term AS search_term,
         FROM ad_group
         WHERE segments.date DURING TODAY
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
     def test_complex_target_with_virtual_column_creates_correct_query(self):
-      target = query_target.Target(
+      target = query_target.Collector(
           metrics=[
               query_elements.Field(name='impressions'),
               query_elements.Field(name='clicks'),
               query_elements.Field(name='cost_micros * 1e6', alias='cost'),
               query_elements.Field(name='clicks / impressions', alias='ctr'),
               query_elements.Field(
                   name='var1-var2/(1.05e3+var3)*100.5', alias='vc')
           ],
-          level=query_target.TargetLevel.AD_GROUP,
+          level=query_target.CollectorLevel.AD_GROUP,
           dimensions=[
               query_elements.Field(
                   name='segments.conversion_action',
                   alias='conversion_id',
                   customizer=query_elements.Customizer(
                       query_elements.CustomizerTypeEnum.INDEX, '0')),
               query_elements.Field(
@@ -116,15 +116,15 @@
             search_terms_view.search_term AS search_term,
         FROM ad_group
         WHERE segments.date DURING TODAY
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
     def test_service_target_creates_correct_query(self):
-      target = query_target.ServiceTarget(
+      target = query_target.ServiceCollector(
           name='mapping',
           dimensions=[
               query_elements.Field(name='ad_group.id', alias='ad_group_id'),
               query_elements.Field(name='ad_group.name', alias='ad_group_name'),
               query_elements.Field(name='campaign.id', alias='campaign_id'),
               query_elements.Field(name='campaign.name', alias='campaign_name'),
               query_elements.Field(name='customer.id', alias='customer_id'),
@@ -148,103 +148,103 @@
           WHERE ad_group.status = ENABLED
             AND campaign.status = ENABLED
             AND customer.status = ENABLED
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
     def test_service_target_cannot_change_metrics_value(self):
-      target = query_target.ServiceTarget(
+      target = query_target.ServiceCollector(
           name='mapping',
           dimensions=[
               query_elements.Field(name='ad_group.id', alias='ad_group_id'),
           ])
       with pytest.raises(ValueError):
         target.metrics = query_elements.Field('ad_group.id')
 
     def test_mcc_level_target_creates_correct_customer_level_query(self):
-      target = query_target.Target(
+      target = query_target.Collector(
           name='simple_mcc_level',
           metrics='impressions',
-          level=query_target.TargetLevel.MCC)
+          level=query_target.CollectorLevel.MCC)
       expected_sql = """
         SELECT
             customer.id AS customer_id,
             metrics.impressions AS impressions,
         FROM customer
         WHERE segments.date DURING TODAY
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
     def test_ad_group_ad_level_target_creates_correct_query(self):
-      target = query_target.Target(
+      target = query_target.Collector(
           name='simple_ad_group_ad_level',
           metrics='impressions',
-          level=query_target.TargetLevel.AD_GROUP_AD)
+          level=query_target.CollectorLevel.AD_GROUP_AD)
 
       expected_sql = """
         SELECT
             ad_group_ad.ad.id AS ad_id,
             metrics.impressions AS impressions,
         FROM ad_group_ad
         WHERE segments.date DURING TODAY
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
     def test_ad_group_level_target_with_resource_name_creates_correct_query(
         self):
-      target = query_target.Target(
+      target = query_target.Collector(
           name='simple_with_resource',
           metrics='impressions',
           resource_name='search_term_view',
-          level=query_target.TargetLevel.AD_GROUP)
+          level=query_target.CollectorLevel.AD_GROUP)
       assert f'FROM {target.resource_name}' in target.query
 
     def test_target_with_not_unique_files_creates_query_with_unique_fields(
         self):
-      target = query_target.Target(
+      target = query_target.Collector(
           name='simple',
           metrics='impressions',
           dimensions=[
               query_elements.Field('ad_group.id'),
           ],
-          level=query_target.TargetLevel.AD_GROUP)
+          level=query_target.CollectorLevel.AD_GROUP)
       expected_sql = """
         SELECT
             ad_group.id AS ad_group_id,
             metrics.impressions AS impressions,
         FROM ad_group
         WHERE segments.date DURING TODAY
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
     def test_target_with_nested_fieds_names_creates_correct_query(self):
-      target = query_target.Target(
+      target = query_target.Collector(
           name='bid_budget',
           metrics=[
               query_elements.Field('impressions'),
               query_elements.Field('campaign_budget.amount_micros', 'budget'),
               query_elements.Field('campaign.target_cpa.target_cpa_micros',
                                    'target_cpa'),
           ],
-          level=query_target.TargetLevel.CAMPAIGN)
+          level=query_target.CollectorLevel.CAMPAIGN)
       expected_sql = """
         SELECT
             campaign.id AS campaign_id,
             metrics.impressions AS impressions,
             campaign_budget.amount_micros AS budget,
             campaign.target_cpa.target_cpa_micros AS target_cpa,
         FROM campaign
         WHERE segments.date DURING TODAY
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
     def test_target_with_empty_metrics_creates_correct_query(self):
-      target = query_target.Target(
+      target = query_target.Collector(
           name='disapproval',
-          level=query_target.TargetLevel.AD_GROUP_AD,
+          level=query_target.CollectorLevel.AD_GROUP_AD,
           dimensions=[
               query_elements.Field('campaign.id', 'campaign_id'),
               query_elements.Field('ad_group_ad.policy_summary.approval_status',
                                    'approval_status'),
               query_elements.Field('ad_group_ad.policy_summary.review_status',
                                    'review_status')
           ],
@@ -263,16 +263,17 @@
         WHERE campaign.status = ENABLED
             AND ad_group.status = ENABLED
             AND ad_group_ad.status = ENABLED
             AND ad_group_ad.policy_summary.approval_status != APPROVED
         """
       assert_sql_functionally_equivalent(target.query, expected_sql)
 
+    @pytest.mark.skip('Obsolete')
     @pytest.mark.parametrize('test_level, expected_sql', [
-        (query_target.TargetLevel.AD_GROUP_AD, """
+        (query_target.CollectorLevel.AD_GROUP_AD, """
                 SELECT
                     1 AS info,
                     ad_group_ad.ad.id AS ad_id,
                     ad_group_ad.ad.name AS ad_name,
                     ad_group.id AS ad_group_id,
                     ad_group.name AS ad_group_name,
                     campaign.id AS campaign_id,
@@ -281,247 +282,221 @@
                     customer.descriptive_name AS account_name,
                 FROM ad_group_ad
                 WHERE ad_group_ad.status = ENABLED
                     AND ad_group.status = ENABLED
                     AND campaign.status = ENABLED
                     AND customer.status = ENABLED
             """),
-        (query_target.TargetLevel.AD_GROUP, """
+        (query_target.CollectorLevel.AD_GROUP, """
                 SELECT
                     1 AS info,
                     ad_group.id AS ad_group_id,
                     ad_group.name AS ad_group_name,
                     campaign.id AS campaign_id,
                     campaign.name AS campaign_name,
                     customer.id AS customer_id,
                     customer.descriptive_name AS account_name,
                 FROM ad_group
                 WHERE ad_group.status = ENABLED
                     AND campaign.status = ENABLED
                     AND customer.status = ENABLED
             """),
-        (query_target.TargetLevel.CAMPAIGN, """
+        (query_target.CollectorLevel.CAMPAIGN, """
                 SELECT
                     1 AS info,
                     campaign.id AS campaign_id,
                     campaign.name AS campaign_name,
                     customer.id AS customer_id,
                     customer.descriptive_name AS account_name,
                 FROM campaign
                 WHERE campaign.status = ENABLED
                     AND customer.status = ENABLED
             """),
-        (query_target.TargetLevel.CUSTOMER, """
+        (query_target.CollectorLevel.CUSTOMER, """
                 SELECT
                     1 AS info,
                     customer.id AS customer_id,
                     customer.descriptive_name AS account_name,
                 FROM customer
                 WHERE customer.status = ENABLED
             """),
-        (query_target.TargetLevel.MCC, """
+        (query_target.CollectorLevel.MCC, """
                 SELECT
                     1 AS info,
                     customer.id AS customer_id,
                     customer.descriptive_name AS account_name,
                 FROM customer
                 WHERE customer.status = ENABLED
             """),
     ])
     def test_create_default_service_target_returns_correct_service_target_query_for_level(  # pylint: disable=line-too-long
         self, test_level, expected_sql):
       actual_target = query_target.create_default_service_target(test_level)
       assert_sql_functionally_equivalent(actual_target.query, expected_sql)
 
-  class TestTargetProperties:
+  class TestCollectorProperties:
 
     def test_metrics_returns_correct_fields(self):
-      target = query_target.Target(metrics='clicks')
+      target = query_target.Collector(metrics='clicks')
       assert target.metrics == {
           query_elements.Field(name='metrics.clicks', alias='clicks'),
       }
 
     def test_dimensions_returns_correct_fields(self):
-      target = query_target.Target(dimensions='segments.date')
+      target = query_target.Collector(dimensions='segments.date')
       assert target.dimensions == {
           query_elements.Field(name='segments.date', alias=None),
       }
 
     @pytest.mark.parametrize('filters,expected_filter', [
         ('segments.date DURING YESTERDAY', 'segments.date DURING YESTERDAY'),
         (None, 'segments.date DURING TODAY'),
     ])
     def test_filters_returns_correct_expression(self, filters, expected_filter):
-      target = query_target.Target(filters=filters)
+      target = query_target.Collector(filters=filters)
 
       assert target.filters == expected_filter
 
     def test_resource_name_returns_correct_expression_for_explicit_resource_name(
         self):
       resource_name = 'search_term_view'
-      level = query_target.TargetLevel.AD_GROUP
+      level = query_target.CollectorLevel.AD_GROUP
       expected_resource_name = 'search_term_view'
 
-      target = query_target.Target(level=level, resource_name=resource_name)
+      target = query_target.Collector(level=level, resource_name=resource_name)
 
       assert target.resource_name == expected_resource_name
 
     def test_resource_name_returns_correct_expression_for_missing_resource_name(
         self):
-      level = query_target.TargetLevel.CAMPAIGN
+      level = query_target.CollectorLevel.CAMPAIGN
       expected_resource_name = 'campaign'
 
-      target = query_target.Target(level=level)
+      target = query_target.Collector(level=level)
 
       assert target.resource_name == expected_resource_name
 
     def test_resource_name_returns_correct_expression_for_missing_resource_name_and_level(  # pylint: disable=line-too-long
         self):
       expected_resource_name = 'ad_group'
 
-      target = query_target.Target()
+      target = query_target.Collector()
 
       assert target.resource_name == expected_resource_name
 
-  class TestTargetEquality:
+  class TestCollectorEquality:
 
     def test_target_with_the_same_metrics_are_equal(self):
-      target1 = query_target.Target(
+      target1 = query_target.Collector(
           name='target1', metrics='clicks,conversions')
-      target2 = query_target.Target(
+      target2 = query_target.Collector(
           name='target2', metrics='clicks,conversions')
 
       assert target1 == target2
 
     def test_targets_with_different_metrics_and_dimensions_are_not_equal(self):
-      target1 = query_target.Target(
+      target1 = query_target.Collector(
           name='target1', metrics='clicks,conversions')
-      target2 = query_target.Target(
+      target2 = query_target.Collector(
           name='target2', dimensions='clicks,conversions')
 
       assert target1 != target2
 
     def test_targets_with_same_metrics_but_different_instantiations_are_equal(
         self):
-      target1 = query_target.Target(metrics='clicks,conversions')
-      target2 = query_target.Target(metrics=[
+      target1 = query_target.Collector(metrics='clicks,conversions')
+      target2 = query_target.Collector(metrics=[
           query_elements.Field(name='clicks'),
           query_elements.Field(name='conversions'),
       ])
 
       assert target1 == target2
 
     def test_targets_with_different_order_of_metrics_are_equal(self):
-      target1 = query_target.Target(metrics=[
+      target1 = query_target.Collector(metrics=[
           query_elements.Field(name='conversions'),
           query_elements.Field(name='impressions', alias='imp'),
       ])
-      target2 = query_target.Target(
+      target2 = query_target.Collector(
           metrics=[
               query_elements.Field(name='impressions', alias='imp'),
               query_elements.Field(name='conversions')
           ],)
 
       assert target1 == target2
 
-  class TestTargetSimilarity:
+  class TestCollectorSimilarity:
 
     def test_targets_with_same_metrics_and_dimensions_are_similar(self):
-      target1 = query_target.Target(
+      target1 = query_target.Collector(
           name='target1',
           metrics='clicks,conversions',
           dimensions='segments.date',
           filters='segments.date DURING TODAY',
-          level=query_target.TargetLevel.AD_GROUP)
-      target2 = query_target.Target(
+          level=query_target.CollectorLevel.AD_GROUP)
+      target2 = query_target.Collector(
           name='target2',
           metrics='clicks,conversions',
           dimensions='segments.date',
           filters='segments.date DURING TODAY',
-          level=query_target.TargetLevel.AD_GROUP_AD)
+          level=query_target.CollectorLevel.AD_GROUP_AD)
       assert target1.is_similar(target2)
       assert target1 != target2
 
     def test_targets_with_different_metrics_and_same_dimensions_are_not_similar(
         self):
-      target1 = query_target.Target(
+      target1 = query_target.Collector(
           name='target1',
           metrics='clicks',
           dimensions='segments.date',
-          level=query_target.TargetLevel.AD_GROUP)
-      target2 = query_target.Target(
+          level=query_target.CollectorLevel.AD_GROUP)
+      target2 = query_target.Collector(
           name='target2',
           metrics='clicks,conversions',
           dimensions='segments.date',
-          level=query_target.TargetLevel.AD_GROUP_AD)
+          level=query_target.CollectorLevel.AD_GROUP_AD)
       assert not target1.is_similar(target2)
 
     def test_targets_with_same_metrics_and_different_dimensions_are_not_similar(
         self):
-      target1 = query_target.Target(
+      target1 = query_target.Collector(
           name='target1',
           metrics='clicks,conversions',
-          level=query_target.TargetLevel.AD_GROUP)
-      target2 = query_target.Target(
+          level=query_target.CollectorLevel.AD_GROUP)
+      target2 = query_target.Collector(
           name='target2',
           metrics='clicks,conversions',
           dimensions='segments.date',
-          level=query_target.TargetLevel.AD_GROUP_AD)
+          level=query_target.CollectorLevel.AD_GROUP_AD)
       assert not target1.is_similar(target2)
 
     def test_targets_with_different_filters_are_not_similar(self):
-      target1 = query_target.Target(
+      target1 = query_target.Collector(
           name='target1',
           metrics='clicks,conversions',
           dimensions='segments.date',
           filters='segments.date DURING TODAY',
-          level=query_target.TargetLevel.AD_GROUP)
-      target2 = query_target.Target(
+          level=query_target.CollectorLevel.AD_GROUP)
+      target2 = query_target.Collector(
           name='target2',
           metrics='clicks,conversions',
           dimensions='segments.date',
           filters='segments.date DURING YESTERDAY',
-          level=query_target.TargetLevel.AD_GROUP)
+          level=query_target.CollectorLevel.AD_GROUP)
       assert not target1.is_similar(target2)
 
     def test_targets_with_different_resource_names_are_not_similar(self):
-      target1 = query_target.Target(
+      target1 = query_target.Collector(
           name='target1',
           metrics='clicks,conversions',
           dimensions='segments.date',
           filters='segments.date DURING TODAY',
           resource_name='age_view',
-          level=query_target.TargetLevel.AD_GROUP)
-      target2 = query_target.Target(
+          level=query_target.CollectorLevel.AD_GROUP)
+      target2 = query_target.Collector(
           name='target2',
           metrics='clicks,conversions',
           dimensions='segments.date',
           resource_name='gender_view',
           filters='segments.date DURING TODAY',
-          level=query_target.TargetLevel.AD_GROUP_AD)
+          level=query_target.CollectorLevel.AD_GROUP_AD)
       assert not target1.is_similar(target2)
-
-
-@pytest.mark.parametrize('targets,expected', [
-    ([
-        query_target.Target(
-            name='target1',
-            metrics='clicks,conversions',
-            level=query_target.TargetLevel.CUSTOMER),
-        query_target.Target(
-            name='target2',
-            metrics='clicks,conversions',
-            level=query_target.TargetLevel.AD_GROUP),
-        query_target.Target(
-            name='target3',
-            metrics='clicks,conversions',
-            level=query_target.TargetLevel.AD_GROUP_AD),
-        query_target.Target(
-            name='target4',
-            metrics='clicks,conversions,impressions',
-            level=query_target.TargetLevel.MCC)
-    ], ['target3', 'target4']),
-])
-def test_targets_similarity_check_returns_deduplicated_targets(
-    targets, expected):
-  actual = query_target.targets_similarity_check(targets)
-  assert set([t.name for t in actual]) == set(expected)
```

### Comparing `gaarf-exporter-0.7.1/tests/unit/test_util.py` & `gaarf-exporter-1.0.0.dev1/tests/unit/test_util.py`

 * *Files identical despite different names*

