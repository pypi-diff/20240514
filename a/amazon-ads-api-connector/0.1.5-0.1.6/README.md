# Comparing `tmp/amazon_ads_api_connector-0.1.5.tar.gz` & `tmp/amazon_ads_api_connector-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_ads_api_connector-0.1.5.tar", last modified: Tue May 14 10:08:27 2024, max compression
+gzip compressed data, was "amazon_ads_api_connector-0.1.6.tar", last modified: Tue May 14 10:46:12 2024, max compression
```

## Comparing `amazon_ads_api_connector-0.1.5.tar` & `amazon_ads_api_connector-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 markusulrichwahl   (501) staff       (20)        0 2024-05-14 10:08:27.103877 amazon_ads_api_connector-0.1.5/
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)     1080 2024-03-09 23:03:48.000000 amazon_ads_api_connector-0.1.5/LICENSE.txt 
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)     5703 2024-05-14 10:08:27.103588 amazon_ads_api_connector-0.1.5/PKG-INFO
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)     5478 2024-05-14 09:55:12.000000 amazon_ads_api_connector-0.1.5/README.md
-drwxr-xr-x   0 markusulrichwahl   (501) staff       (20)        0 2024-05-14 10:08:27.101826 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)      263 2024-05-14 10:04:54.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/__init__.py
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)    32231 2024-05-14 09:43:39.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_ads_api_connector.py
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)      471 2024-05-14 09:38:15.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_regions.py
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)    13422 2024-03-08 21:11:14.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_reports.py
-drwxr-xr-x   0 markusulrichwahl   (501) staff       (20)        0 2024-05-14 10:08:27.103174 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)     5703 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/PKG-INFO
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)      446 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/SOURCES.txt
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)        1 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/dependency_links.txt
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)        6 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/requires.txt
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)       25 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/top_level.txt
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)       38 2024-05-14 10:08:27.103928 amazon_ads_api_connector-0.1.5/setup.cfg
--rw-r--r--   0 markusulrichwahl   (501) staff       (20)      419 2024-05-14 10:06:11.000000 amazon_ads_api_connector-0.1.5/setup.py
+drwxr-xr-x   0 markusulrichwahl   (501) staff       (20)        0 2024-05-14 10:46:12.731302 amazon_ads_api_connector-0.1.6/
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)     1080 2024-03-09 23:03:48.000000 amazon_ads_api_connector-0.1.6/LICENSE.txt 
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)     5700 2024-05-14 10:46:12.731077 amazon_ads_api_connector-0.1.6/PKG-INFO
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)     5475 2024-05-14 10:43:30.000000 amazon_ads_api_connector-0.1.6/README.md
+drwxr-xr-x   0 markusulrichwahl   (501) staff       (20)        0 2024-05-14 10:46:12.729648 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector/
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)      263 2024-05-14 10:04:54.000000 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector/__init__.py
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)    32231 2024-05-14 09:43:39.000000 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector/amazon_ads_api_connector.py
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)      471 2024-05-14 09:38:15.000000 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector/amazon_regions.py
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)    13422 2024-03-08 21:11:14.000000 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector/amazon_reports.py
+drwxr-xr-x   0 markusulrichwahl   (501) staff       (20)        0 2024-05-14 10:46:12.730777 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector.egg-info/
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)     5700 2024-05-14 10:46:12.000000 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector.egg-info/PKG-INFO
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)      446 2024-05-14 10:46:12.000000 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)        1 2024-05-14 10:46:12.000000 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)        6 2024-05-14 10:46:12.000000 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector.egg-info/requires.txt
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)       25 2024-05-14 10:46:12.000000 amazon_ads_api_connector-0.1.6/amazon_ads_api_connector.egg-info/top_level.txt
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)       38 2024-05-14 10:46:12.731353 amazon_ads_api_connector-0.1.6/setup.cfg
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)      419 2024-05-14 10:44:23.000000 amazon_ads_api_connector-0.1.6/setup.py
```

### Comparing `amazon_ads_api_connector-0.1.5/LICENSE.txt ` & `amazon_ads_api_connector-0.1.6/LICENSE.txt `

 * *Files identical despite different names*

### Comparing `amazon_ads_api_connector-0.1.5/PKG-INFO` & `amazon_ads_api_connector-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-ads-api-connector
-Version: 0.1.5
+Version: 0.1.6
 Summary: API wrapper for the Amazon Ads API
 Author: Markus U. Wahl
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt 
 Requires-Dist: httpx
 
 # Amazon Ads API Connector
@@ -108,15 +108,15 @@
 For more information about the report types, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types).
 
 To request a report you need to pass an instance of one of these classes to the `create_report` method of the `AmazonAdsAPIConnector` class. To customize the report, change the properties of the class instance before passing it to the `create_report` method.
 
 ```python
 from amazon_ads_api_connector import SearchTermReport
 
-report_configuration = SearchTermReport("2023-10-01", ◊"2023-10-07")
+report_configuration = SearchTermReport("2023-10-01", "2023-10-07")
 
 res = api.create_report(report_configuration)
 report = api.get_report(res)
 ```
 Please note that report gerneration is asynchronous. The `create_report` method returns a dictionary containing the report ID. The `get_report` takes this dictionary as an argument and returns the report once it is completed and available. The completion of a report usually takes a few minutes and can take up to 3 hours.
 
 ## Dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.6 Summary:
 API wrapper for the Amazon Ads API Author: Markus U. Wahl Description-Content-
 Type: text/markdown License-File: LICENSE.txt Requires-Dist: httpx # Amazon Ads
 API Connector A simple Python wrapper for the _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f_ _t_h_e_ _A_m_a_z_o_n_ _A_d_s
 _A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n_ _m_a_n_a_g_e_m_e_n_t. This module covers the key
 endpoints for managing Sponsored Products campaigns. This includes methods for
 authentication, pagination and report generation. It features keyword and
 negative keyword targeting, as well as product ASIN targeting and auto
@@ -51,18 +51,18 @@
 `AdvertisedProductReports` - `PurchasedProductReport` For more information
 about the report types, please visit the [official documentation](https://
 advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To
 request a report you need to pass an instance of one of these classes to the
 `create_report` method of the `AmazonAdsAPIConnector` class. To customize the
 report, change the properties of the class instance before passing it to the
 `create_report` method. ```python from amazon_ads_api_connector import
-SearchTermReport report_configuration = SearchTermReport("2023-10-01",
-â"2023-10-07") res = api.create_report(report_configuration) report =
-api.get_report(res) ``` Please note that report gerneration is asynchronous.
-The `create_report` method returns a dictionary containing the report ID. The
+SearchTermReport report_configuration = SearchTermReport("2023-10-01", "2023-
+10-07") res = api.create_report(report_configuration) report = api.get_report
+(res) ``` Please note that report gerneration is asynchronous. The
+`create_report` method returns a dictionary containing the report ID. The
 `get_report` takes this dictionary as an argument and returns the report once
 it is completed and available. The completion of a report usually takes a few
 minutes and can take up to 3 hours. ## Dependencies This module depends on the
 `httpx` library, which is not included in the Python standard library, but will
 be installed automatically when you install the `amazon-ads-api-connector`
 package. ## Disclaimer I am not affiliated with Amazon in any way. This module
 is an independent project that aims to provide a simple and easy-to-use
```

### Comparing `amazon_ads_api_connector-0.1.5/README.md` & `amazon_ads_api_connector-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 For more information about the report types, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types).
 
 To request a report you need to pass an instance of one of these classes to the `create_report` method of the `AmazonAdsAPIConnector` class. To customize the report, change the properties of the class instance before passing it to the `create_report` method.
 
 ```python
 from amazon_ads_api_connector import SearchTermReport
 
-report_configuration = SearchTermReport("2023-10-01", ◊"2023-10-07")
+report_configuration = SearchTermReport("2023-10-01", "2023-10-07")
 
 res = api.create_report(report_configuration)
 report = api.get_report(res)
 ```
 Please note that report gerneration is asynchronous. The `create_report` method returns a dictionary containing the report ID. The `get_report` takes this dictionary as an argument and returns the report once it is completed and available. The completion of a report usually takes a few minutes and can take up to 3 hours.
 
 ## Dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -49,18 +49,18 @@
 `AdvertisedProductReports` - `PurchasedProductReport` For more information
 about the report types, please visit the [official documentation](https://
 advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To
 request a report you need to pass an instance of one of these classes to the
 `create_report` method of the `AmazonAdsAPIConnector` class. To customize the
 report, change the properties of the class instance before passing it to the
 `create_report` method. ```python from amazon_ads_api_connector import
-SearchTermReport report_configuration = SearchTermReport("2023-10-01",
-â"2023-10-07") res = api.create_report(report_configuration) report =
-api.get_report(res) ``` Please note that report gerneration is asynchronous.
-The `create_report` method returns a dictionary containing the report ID. The
+SearchTermReport report_configuration = SearchTermReport("2023-10-01", "2023-
+10-07") res = api.create_report(report_configuration) report = api.get_report
+(res) ``` Please note that report gerneration is asynchronous. The
+`create_report` method returns a dictionary containing the report ID. The
 `get_report` takes this dictionary as an argument and returns the report once
 it is completed and available. The completion of a report usually takes a few
 minutes and can take up to 3 hours. ## Dependencies This module depends on the
 `httpx` library, which is not included in the Python standard library, but will
 be installed automatically when you install the `amazon-ads-api-connector`
 package. ## Disclaimer I am not affiliated with Amazon in any way. This module
 is an independent project that aims to provide a simple and easy-to-use
```

### Comparing `amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_ads_api_connector.py` & `amazon_ads_api_connector-0.1.6/amazon_ads_api_connector/amazon_ads_api_connector.py`

 * *Files identical despite different names*

### Comparing `amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_reports.py` & `amazon_ads_api_connector-0.1.6/amazon_ads_api_connector/amazon_reports.py`

 * *Files identical despite different names*

### Comparing `amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/PKG-INFO` & `amazon_ads_api_connector-0.1.6/amazon_ads_api_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-ads-api-connector
-Version: 0.1.5
+Version: 0.1.6
 Summary: API wrapper for the Amazon Ads API
 Author: Markus U. Wahl
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt 
 Requires-Dist: httpx
 
 # Amazon Ads API Connector
@@ -108,15 +108,15 @@
 For more information about the report types, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types).
 
 To request a report you need to pass an instance of one of these classes to the `create_report` method of the `AmazonAdsAPIConnector` class. To customize the report, change the properties of the class instance before passing it to the `create_report` method.
 
 ```python
 from amazon_ads_api_connector import SearchTermReport
 
-report_configuration = SearchTermReport("2023-10-01", ◊"2023-10-07")
+report_configuration = SearchTermReport("2023-10-01", "2023-10-07")
 
 res = api.create_report(report_configuration)
 report = api.get_report(res)
 ```
 Please note that report gerneration is asynchronous. The `create_report` method returns a dictionary containing the report ID. The `get_report` takes this dictionary as an argument and returns the report once it is completed and available. The completion of a report usually takes a few minutes and can take up to 3 hours.
 
 ## Dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.6 Summary:
 API wrapper for the Amazon Ads API Author: Markus U. Wahl Description-Content-
 Type: text/markdown License-File: LICENSE.txt Requires-Dist: httpx # Amazon Ads
 API Connector A simple Python wrapper for the _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f_ _t_h_e_ _A_m_a_z_o_n_ _A_d_s
 _A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n_ _m_a_n_a_g_e_m_e_n_t. This module covers the key
 endpoints for managing Sponsored Products campaigns. This includes methods for
 authentication, pagination and report generation. It features keyword and
 negative keyword targeting, as well as product ASIN targeting and auto
@@ -51,18 +51,18 @@
 `AdvertisedProductReports` - `PurchasedProductReport` For more information
 about the report types, please visit the [official documentation](https://
 advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To
 request a report you need to pass an instance of one of these classes to the
 `create_report` method of the `AmazonAdsAPIConnector` class. To customize the
 report, change the properties of the class instance before passing it to the
 `create_report` method. ```python from amazon_ads_api_connector import
-SearchTermReport report_configuration = SearchTermReport("2023-10-01",
-â"2023-10-07") res = api.create_report(report_configuration) report =
-api.get_report(res) ``` Please note that report gerneration is asynchronous.
-The `create_report` method returns a dictionary containing the report ID. The
+SearchTermReport report_configuration = SearchTermReport("2023-10-01", "2023-
+10-07") res = api.create_report(report_configuration) report = api.get_report
+(res) ``` Please note that report gerneration is asynchronous. The
+`create_report` method returns a dictionary containing the report ID. The
 `get_report` takes this dictionary as an argument and returns the report once
 it is completed and available. The completion of a report usually takes a few
 minutes and can take up to 3 hours. ## Dependencies This module depends on the
 `httpx` library, which is not included in the Python standard library, but will
 be installed automatically when you install the `amazon-ads-api-connector`
 package. ## Disclaimer I am not affiliated with Amazon in any way. This module
 is an independent project that aims to provide a simple and easy-to-use
```

