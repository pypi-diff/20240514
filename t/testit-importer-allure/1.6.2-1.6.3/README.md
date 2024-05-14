# Comparing `tmp/testit_importer_allure-1.6.2.tar.gz` & `tmp/testit_importer_allure-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit_importer_allure-1.6.2.tar", last modified: Fri Apr 19 11:03:00 2024, max compression
+gzip compressed data, was "testit_importer_allure-1.6.3.tar", last modified: Tue May 14 10:08:17 2024, max compression
```

## Comparing `testit_importer_allure-1.6.2.tar` & `testit_importer_allure-1.6.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:03:00.706045 testit_importer_allure-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-19 11:03:00.702045 testit_importer_allure-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/connection_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:03:00.706045 testit_importer_allure-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:03:00.702045 testit_importer_allure-1.6.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/filedto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/filereader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/minioreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 11:02:56.000000 testit_importer_allure-1.6.2/src/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:03:00.702045 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 11:03:00.000000 testit_importer_allure-1.6.2/testit_importer_allure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/connection_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13509 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/filedto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/minioreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/top_level.txt
```

### Comparing `testit_importer_allure-1.6.2/PKG-INFO` & `testit_importer_allure-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-importer-allure
-Version: 1.6.2
+Version: 1.6.3
 Summary: Allure report importer for Test IT
 Home-page: https://pypi.org/project/testit-importer-allure/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit_importer_allure-1.6.2/README.md` & `testit_importer_allure-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.2/setup.py` & `testit_importer_allure-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='testit-importer-allure',
-    version='1.6.2',
+    version='1.6.3',
     description='Allure report importer for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://pypi.org/project/testit-importer-allure/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
```

### Comparing `testit_importer_allure-1.6.2/src/__main__.py` & `testit_importer_allure-1.6.3/src/__main__.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.2/src/apiclient.py` & `testit_importer_allure-1.6.3/src/apiclient.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.2/src/configurator.py` & `testit_importer_allure-1.6.3/src/configurator.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 CONFIG_SECTION = 'testit'
 CONFIG_URL = 'url'
 CONFIG_PRIVATE_TOKEN = 'privateToken'
 CONFIG_PROJECT_ID = 'projectID'
 CONFIG_CONFIGURATION_ID = 'configurationID'
 CONFIG_CERT_VALIDATION = 'certValidation'
 CONFIG_NAME = 'connection_config.ini'
+ALLURE_IGNORE_PACKAGE_NAME = 'ignorePackageName'
 
 RABBITMQ_CONFIG_SECTION = 'rabbitmq'
 RABBITMQ_CONFIG_URL = 'host'
 RABBITMQ_CONFIG_USER = 'user'
 RABBITMQ_CONFIG_PASSWORD = 'password'
 RABBITMQ_CONFIG_EXCHANGE = 'exchange'
 
 MINIO_CONFIG_SECTION = 'minio'
 MINIO_CONFIG_URL = 'host'
 MINIO_CONFIG_ACCESS_KEY = 'accessKey'
 MINIO_CONFIG_SECRET_KEY = 'secretKey'
 
 
+
 class Configurator:
     """Class representing a configurator"""
 
     path_to_results = None
     path_to_config = None
     specified_testrun = None
     specified_testrun_name = None
@@ -61,14 +63,18 @@
     def get_cert_validation(self):
         """Function returns cert validation."""
         if not self.config.has_option(CONFIG_SECTION, CONFIG_CERT_VALIDATION):
             return
 
         return self.config.get(CONFIG_SECTION, CONFIG_CERT_VALIDATION)
 
+    def get_ignore_package_name(self):
+        """Function returns ignore package name."""
+        return self.config.get(CONFIG_SECTION, ALLURE_IGNORE_PACKAGE_NAME)
+
     def get_rabbitmq_url(self):
         """Function returns rabbit mq url."""
         return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL)
 
     def get_rabbitmq_user(self):
         """Function returns rabbit mq user."""
         return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_USER)
@@ -162,14 +168,23 @@
             '-sh',
             '--show',
             action='store_true',
             dest="show_settings",
             help='Show the connection_config.ini file'
         )
         self.parser.add_argument(
+            '-ipn',
+            '--ignorepackagename',
+            action="store",
+            dest="ignore_package_name",
+            metavar="True or False",
+            default=False,
+            help='Use parentSuite as namespace'
+        )
+        self.parser.add_argument(
             '-rd',
             '--resultsdir',
             action="store",
             dest="alluredir",
             metavar="DIR",
             default=None,
             help='Import the Allure report in the specified directory if it exists'
@@ -316,14 +331,16 @@
 
         if args.set_testrun_name:
             self.specified_testrun_name = args.set_testrun_name
 
         if args.set_cert_validation:
             self.config.set(CONFIG_SECTION, CONFIG_CERT_VALIDATION, args.set_cert_validation.lower())
 
+        self.config.set(CONFIG_SECTION, ALLURE_IGNORE_PACKAGE_NAME, args.ignore_package_name)
+
         if args.alluredir:
             self.path_to_results = args.alluredir
 
         if args.set_rabbitmqhost:
             self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL, args.set_rabbitmqhost)
 
         if args.set_rabbitmquser:
```

### Comparing `testit_importer_allure-1.6.2/src/converter.py` & `testit_importer_allure-1.6.3/src/converter.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.2/src/filereader.py` & `testit_importer_allure-1.6.3/src/filereader.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.2/src/importer.py` & `testit_importer_allure-1.6.3/src/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     def __init__(self, parser: Parser, api_client: ApiClient, config: Configurator):
         self.__parser = parser
         self.__api_client = api_client
         self.__project_id = config.get_project_id()
         self.__testrun_id = config.specified_testrun
         self.__testrun_name = config.specified_testrun_name
         self.__configuration_id = config.get_configuration_id()
+        self.__ignore_namespace_name = config.get_ignore_package_name()
 
     def send_result(self):
         """Function imports result to TMS."""
         data_tests, data_fixtures = self.__parser.parse_results()
 
         self.__set_test_run()
 
@@ -160,15 +161,15 @@
                 if label[f'{prefix}name'] == 'testcase':
                     work_items_id.append(label[f'{prefix}value'])
                 else:
                     labels.append(
                         Converter.label_to_label_post_model(
                             f"{label[f'{prefix}name']}::{label[f'{prefix}value']}"))
 
-                if label[f'{prefix}name'] == 'package':
+                if label[f'{prefix}name'] == 'package' and not self.__ignore_namespace_name:
                     packages = label[f'{prefix}value'].split('.')
 
                     while packages and not packages[-1]:
                         del packages[-1]
 
                     if packages:
                         namespace = packages[-1]
```

### Comparing `testit_importer_allure-1.6.2/src/minioreader.py` & `testit_importer_allure-1.6.3/src/minioreader.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.2/src/parser.py` & `testit_importer_allure-1.6.3/src/parser.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.2/src/rabbitmq.py` & `testit_importer_allure-1.6.3/src/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.2/testit_importer_allure.egg-info/PKG-INFO` & `testit_importer_allure-1.6.3/testit_importer_allure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-importer-allure
-Version: 1.6.2
+Version: 1.6.3
 Summary: Allure report importer for Test IT
 Home-page: https://pypi.org/project/testit-importer-allure/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit_importer_allure-1.6.2/testit_importer_allure.egg-info/SOURCES.txt` & `testit_importer_allure-1.6.3/testit_importer_allure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

