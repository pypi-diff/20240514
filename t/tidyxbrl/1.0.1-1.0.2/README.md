# Comparing `tmp/tidyxbrl-1.0.1.tar.gz` & `tmp/tidyxbrl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyxbrl-1.0.1.tar", last modified: Tue May 14 03:39:10 2024, max compression
+gzip compressed data, was "tidyxbrl-1.0.2.tar", last modified: Tue May 14 04:22:09 2024, max compression
```

## Comparing `tidyxbrl-1.0.1.tar` & `tidyxbrl-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.0.1/LICENSE
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-04-29 02:36:52.000000 tidyxbrl-1.0.1/MANIFEST.in
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4868 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4225 2022-12-27 22:39:13.000000 tidyxbrl-1.0.1/README.md
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      548 2024-05-14 03:38:54.000000 tidyxbrl-1.0.1/pyproject.toml
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      769 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/setup.cfg
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/src/
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/src/tidyxbrl/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.0.1/src/tidyxbrl/__init__.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.0.1/src/tidyxbrl/edgar_cik.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.0.1/src/tidyxbrl/edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.0.1/src/tidyxbrl/edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.0.1/src/tidyxbrl/xbrl_apikey.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5703 2024-04-28 22:24:56.000000 tidyxbrl-1.0.1/src/tidyxbrl/xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.0.1/src/tidyxbrl/xbrl_query.py
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4868 2024-05-14 03:39:10.000000 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      491 2024-05-14 03:39:10.000000 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/SOURCES.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 03:39:10.000000 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/dependency_links.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        9 2024-05-14 03:39:10.000000 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/top_level.txt
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/tests/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      113 2024-04-28 22:26:49.000000 tidyxbrl-1.0.1/tests/test_edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      666 2024-04-29 03:42:25.000000 tidyxbrl-1.0.1/tests/test_edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      503 2024-04-28 22:25:53.000000 tidyxbrl-1.0.1/tests/test_xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2143 2024-04-28 23:47:03.000000 tidyxbrl-1.0.1/tests/test_xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.0.2/LICENSE
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-05-14 03:53:29.000000 tidyxbrl-1.0.2/MANIFEST.in
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4868 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4225 2022-12-27 22:39:13.000000 tidyxbrl-1.0.2/README.md
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      548 2024-05-14 04:21:47.000000 tidyxbrl-1.0.2/pyproject.toml
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      769 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/setup.cfg
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/src/
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/src/tidyxbrl/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.0.2/src/tidyxbrl/__init__.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.0.2/src/tidyxbrl/edgar_cik.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.0.2/src/tidyxbrl/edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.0.2/src/tidyxbrl/edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.0.2/src/tidyxbrl/xbrl_apikey.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5709 2024-05-14 04:21:21.000000 tidyxbrl-1.0.2/src/tidyxbrl/xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.0.2/src/tidyxbrl/xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4868 2024-05-14 04:22:09.000000 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      491 2024-05-14 04:22:09.000000 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/SOURCES.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 04:22:09.000000 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/dependency_links.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        9 2024-05-14 04:22:09.000000 tidyxbrl-1.0.2/src/tidyxbrl.egg-info/top_level.txt
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 04:22:09.962108 tidyxbrl-1.0.2/tests/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      119 2024-05-14 03:59:03.000000 tidyxbrl-1.0.2/tests/test_edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      681 2024-05-14 03:59:11.000000 tidyxbrl-1.0.2/tests/test_edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      503 2024-04-28 22:25:53.000000 tidyxbrl-1.0.2/tests/test_xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2181 2024-05-14 04:14:20.000000 tidyxbrl-1.0.2/tests/test_xbrl_query.py
```

### Comparing `tidyxbrl-1.0.1/LICENSE` & `tidyxbrl-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.1/PKG-INFO` & `tidyxbrl-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidyxbrl
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
 Home-page: https://github.com/cowboycodeman/tidyxbrl/
 Author: Ryan McDonald
 Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
 Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
 Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidyxbrl-1.0.1/README.md` & `tidyxbrl-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.1/pyproject.toml` & `tidyxbrl-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tidyxbrl"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Ryan McDonald", email="ryancmcdonald@gmail.com" },
 ]
 description = "A package to parse the XBRL file format & interface with XBRL APIs in a tidy format"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tidyxbrl-1.0.1/setup.cfg` & `tidyxbrl-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tidyxbrl
-version = 1.0.1
+version = 1.0.2
 author = Ryan McDonald
 author_email = ryancmcdonald@gmail.com
 description = A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cowboycodeman/tidyxbrl/
 project_urls =
```

### Comparing `tidyxbrl-1.0.1/src/tidyxbrl/edgar_cik.py` & `tidyxbrl-1.0.2/src/tidyxbrl/edgar_cik.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.1/src/tidyxbrl/edgar_frames.py` & `tidyxbrl-1.0.2/src/tidyxbrl/edgar_frames.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.1/src/tidyxbrl/edgar_query.py` & `tidyxbrl-1.0.2/src/tidyxbrl/edgar_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.1/src/tidyxbrl/xbrl_apikey.py` & `tidyxbrl-1.0.2/src/tidyxbrl/xbrl_apikey.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.1/src/tidyxbrl/xbrl_parse.py` & `tidyxbrl-1.0.2/src/tidyxbrl/xbrl_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             print("Path Does Not Correspond to a Website or Valid File Path")
 
     # Pull a list of the descriptive columns to populate an empty dataframe
     tag_listall = soup.find_all(xbrlcolumnprefilter)
     empty_tag_list = soup.select("context")
     columnlist = []
     for temp_tag in tag_listall:
-        if temp_tag.name not in numpy.unique(columnlist):
+        if temp_tag.name not in list(numpy.unique(columnlist)):
             columnlist.append(temp_tag.name)
 
     columnlist = list(columnlist) + ["datacode", "datavalue"]
     print(columnlist)
 
     data = []
     for tag in tqdm(empty_tag_list, desc="Processing Unique Identifiers"):
```

### Comparing `tidyxbrl-1.0.1/src/tidyxbrl/xbrl_query.py` & `tidyxbrl-1.0.2/src/tidyxbrl/xbrl_query.py`

 * *Files identical despite different names*

### Comparing `tidyxbrl-1.0.1/src/tidyxbrl.egg-info/PKG-INFO` & `tidyxbrl-1.0.2/src/tidyxbrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidyxbrl
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
 Home-page: https://github.com/cowboycodeman/tidyxbrl/
 Author: Ryan McDonald
 Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
 Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
 Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidyxbrl-1.0.1/tests/test_edgar_query.py` & `tidyxbrl-1.0.2/tests/test_edgar_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-
 # %%
 import tidyxbrl
 
 tidyxbrl.edgar_query('0000789019', query_type = 'submissions')
 tidyxbrl.edgar_query('0000789019', query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent.json')
 tidyxbrl.edgar_query('0000789019', query_type = 'companyfacts')
 
-companycik = tidyxbrl.edgar_cik()
-desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
+companycik = tidyxbrl.edgar_cik("ZILLOW GROUP, INC.")
+desiredcorp = str(companycik[companycik.company.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
 tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
 tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent.json')
-tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
-# %%
+tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
```

### Comparing `tidyxbrl-1.0.1/tests/test_xbrl_query.py` & `tidyxbrl-1.0.2/tests/test_xbrl_query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # %%
 import yaml
 import tidyxbrl 
 
-credentials = yaml.safe_load(open("tests/test_credentials.yml", "r"))
-username = credentials['credentials']['username'][0]
-password = credentials['credentials']['password'][0]
-client_id = credentials['credentials']['client_id'][0]
-client_secret = credentials['credentials']['client_secret'][0]
-
-response = tidyxbrl.xbrl_apikey(username=username, password=password, client_id=client_id, client_secret=client_secret, platform='pc', grant_type='password', refresh_token='')
-
-dataresponse = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
-               baseapiurl='https://api.xbrl.us/api/v1/report/search?',
-               queryparameters = {'report.entity-name': "APPLE INC.",
-                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
-                                  'report.document-type': "10-K"
-                        })
-
-dataresponse2 = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
-               baseapiurl='https://api.xbrl.us/api/v1/fact/search?',
-               queryparameters = {'report.id': "315201",
-                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
-                                  'concept.local-name': "AccumulatedOtherComprehensiveIncomeLossNetOfTax"
-                        })
-
-
-dataresponse3 = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
-               baseapiurl='https://api.xbrl.us/api/v1/fact/141024005?',
-               queryparameters = {'fields': "fact.value,concept.local-name"
-                        })
+# credentials = yaml.safe_load(open("test_credentials.yml", "r"))
+# username = credentials['credentials']['username'][0]
+# password = credentials['credentials']['password'][0]
+# client_id = credentials['credentials']['client_id'][0]
+# client_secret = credentials['credentials']['client_secret'][0]
+
+# response = tidyxbrl.xbrl_apikey(username=username, password=password, client_id=client_id, client_secret=client_secret, platform='pc', grant_type='password', refresh_token='')
+
+# dataresponse = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
+#                baseapiurl='https://api.xbrl.us/api/v1/report/search?',
+#                queryparameters = {'report.entity-name': "APPLE INC.",
+#                                   'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
+#                                   'report.document-type': "10-K"
+#                         })
+
+# dataresponse2 = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
+#                baseapiurl='https://api.xbrl.us/api/v1/fact/search?',
+#                queryparameters = {'report.id': "315201",
+#                                   'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
+#                                   'concept.local-name': "AccumulatedOtherComprehensiveIncomeLossNetOfTax"
+#                         })
+
+
+# dataresponse3 = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
+#                baseapiurl='https://api.xbrl.us/api/v1/fact/141024005?',
+#                queryparameters = {'fields': "fact.value,concept.local-name"
+#                         })
```

