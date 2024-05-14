# Comparing `tmp/amazon-ads-api-connector-0.1.4.tar.gz` & `tmp/amazon_ads_api_connector-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-ads-api-connector-0.1.4.tar", last modified: Mon Apr  8 11:52:03 2024, max compression
+gzip compressed data, was "amazon_ads_api_connector-0.1.5.tar", last modified: Tue May 14 10:08:27 2024, max compression
```

## Comparing `amazon-ads-api-connector-0.1.4.tar` & `amazon_ads_api_connector-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 muw        (501) staff       (20)        0 2024-04-08 11:52:03.972426 amazon-ads-api-connector-0.1.4/
--rw-r--r--   0 muw        (501) staff       (20)     1080 2024-03-09 23:03:48.000000 amazon-ads-api-connector-0.1.4/LICENSE.txt 
--rw-r--r--   0 muw        (501) staff       (20)     5325 2024-04-08 11:52:03.972188 amazon-ads-api-connector-0.1.4/PKG-INFO
--rw-r--r--   0 muw        (501) staff       (20)     5067 2024-04-08 11:18:54.000000 amazon-ads-api-connector-0.1.4/README.md
-drwxr-xr-x   0 muw        (501) staff       (20)        0 2024-04-08 11:52:03.970371 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/
--rw-r--r--   0 muw        (501) staff       (20)      225 2024-03-08 21:13:55.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/__init__.py
--rw-r--r--   0 muw        (501) staff       (20)    32588 2024-03-11 20:49:48.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/amazon_ads_api_connector.py
--rw-r--r--   0 muw        (501) staff       (20)    13422 2024-03-08 21:11:14.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/report_types.py
-drwxr-xr-x   0 muw        (501) staff       (20)        0 2024-04-08 11:52:03.971725 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/
--rw-r--r--   0 muw        (501) staff       (20)     5325 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/PKG-INFO
--rw-r--r--   0 muw        (501) staff       (20)      401 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/SOURCES.txt
--rw-r--r--   0 muw        (501) staff       (20)        1 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/dependency_links.txt
--rw-r--r--   0 muw        (501) staff       (20)       24 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/requires.txt
--rw-r--r--   0 muw        (501) staff       (20)       25 2024-04-08 11:52:03.000000 amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/top_level.txt
--rw-r--r--   0 muw        (501) staff       (20)       38 2024-04-08 11:52:03.972483 amazon-ads-api-connector-0.1.4/setup.cfg
--rw-r--r--   0 muw        (501) staff       (20)      448 2024-04-08 11:51:49.000000 amazon-ads-api-connector-0.1.4/setup.py
+drwxr-xr-x   0 markusulrichwahl   (501) staff       (20)        0 2024-05-14 10:08:27.103877 amazon_ads_api_connector-0.1.5/
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)     1080 2024-03-09 23:03:48.000000 amazon_ads_api_connector-0.1.5/LICENSE.txt 
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)     5703 2024-05-14 10:08:27.103588 amazon_ads_api_connector-0.1.5/PKG-INFO
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)     5478 2024-05-14 09:55:12.000000 amazon_ads_api_connector-0.1.5/README.md
+drwxr-xr-x   0 markusulrichwahl   (501) staff       (20)        0 2024-05-14 10:08:27.101826 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)      263 2024-05-14 10:04:54.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/__init__.py
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)    32231 2024-05-14 09:43:39.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_ads_api_connector.py
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)      471 2024-05-14 09:38:15.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_regions.py
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)    13422 2024-03-08 21:11:14.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_reports.py
+drwxr-xr-x   0 markusulrichwahl   (501) staff       (20)        0 2024-05-14 10:08:27.103174 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)     5703 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/PKG-INFO
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)      446 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)        1 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)        6 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/requires.txt
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)       25 2024-05-14 10:08:27.000000 amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/top_level.txt
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)       38 2024-05-14 10:08:27.103928 amazon_ads_api_connector-0.1.5/setup.cfg
+-rw-r--r--   0 markusulrichwahl   (501) staff       (20)      419 2024-05-14 10:06:11.000000 amazon_ads_api_connector-0.1.5/setup.py
```

### Comparing `amazon-ads-api-connector-0.1.4/LICENSE.txt ` & `amazon_ads_api_connector-0.1.5/LICENSE.txt `

 * *Files identical despite different names*

### Comparing `amazon-ads-api-connector-0.1.4/PKG-INFO` & `amazon_ads_api_connector-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: amazon-ads-api-connector
-Version: 0.1.4
+Version: 0.1.5
 Summary: API wrapper for the Amazon Ads API
 Author: Markus U. Wahl
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt 
-Requires-Dist: requests
-Requires-Dist: types-requests
+Requires-Dist: httpx
 
 # Amazon Ads API Connector
 
 A simple Python wrapper for the <a href="https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod">latest version of the Amazon Ads API for Sponsored Products campaign management</a>.
 
 This module covers the key endpoints for managing Sponsored Products campaigns. This includes methods for authentication, pagination and report generation. It features keyword and negative keyword targeting, as well as product ASIN targeting and auto campaigns. 
 
@@ -43,30 +42,36 @@
 - `refresh_token`
 - `client_id`
 - `client_secret`
 - `profile_id`
 
 Upon initialization, the AmazonAdsAPIConnector object will create a new access token. This access token will be valid for 60 minutes, however, the object automatically requests a new access token in case it has expired when trying to make a new request.
 
+You furthermore need to specify the region of your Amazon Ads account. The region is specified by the `Region` enum, which is part of the `amazon_ads_api_connector` module. The Amazon Ads API supports the following regions:
+- North America: `Region.NA`
+- Europe: `Region.EU`
+- Far East: `Region.FE`
+
 For more information about the Amazon Ads API, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/get-started/how-to-use-api).
 
 ## Examples
 ### Import the library
 ```python
-from amazon_ads_api_connector import AmazonAdsAPIConnector
+from amazon_ads_api_connector import AmazonAdsAPIConnector, Region
 ```
 ### Create an instance
 ```python
 api = AmazonAdsAPIConnector(
     {
         "refresh_token": "your_refresh_token",
         "client_id": "your_client_id",
         "client_secret": "your_client_secret",
         "profile_id": "your_profile_id",
-    }
+    },
+    Region.EU,
 )
 ```
 ### List campaigns
 ```python
 campaigns = api.list_campaigns()
 ```
 ### Create campaigns
@@ -112,12 +117,12 @@
 res = api.create_report(report_configuration)
 report = api.get_report(res)
 ```
 Please note that report gerneration is asynchronous. The `create_report` method returns a dictionary containing the report ID. The `get_report` takes this dictionary as an argument and returns the report once it is completed and available. The completion of a report usually takes a few minutes and can take up to 3 hours.
 
 ## Dependencies
 
-This module depends on the `requests` library, which is not included in the Python standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
+This module depends on the `httpx` library, which is not included in the Python standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
 
 ## Disclaimer
 
-This module is not affiliated with Amazon in any way. It is an independent project that aims to provide a simple and easy-to-use interface to the Amazon Ads API for Sponsored Products campaign management.
+I am not affiliated with Amazon in any way. This module is an independent project that aims to provide a simple and easy-to-use interface to the Amazon Ads API for Sponsored Products campaign management. I do not guarantee the correctness or completeness of the module. Use it at your own risk.
```

#### html2text {}

```diff
@@ -1,66 +1,71 @@
-Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.5 Summary:
 API wrapper for the Amazon Ads API Author: Markus U. Wahl Description-Content-
-Type: text/markdown License-File: LICENSE.txt Requires-Dist: requests Requires-
-Dist: types-requests # Amazon Ads API Connector A simple Python wrapper for the
-_l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f_ _t_h_e_ _A_m_a_z_o_n_ _A_d_s_ _A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n
-_m_a_n_a_g_e_m_e_n_t. This module covers the key endpoints for managing Sponsored
-Products campaigns. This includes methods for authentication, pagination and
-report generation. It features keyword and negative keyword targeting, as well
-as product ASIN targeting and auto campaigns. Please note that this module does
-not yet support Sponsored Brands and Sponsored Display campaigns. ##
-Installation Amazon Ads API Connector is available on PyPI: ```bash pip install
-amazon-ads-api-connector ``` ## Getting started The primary class of the module
-is `AmazonAdsAPIConnector`. This class provides methods to create, list, update
-and delete - campaigns, - ad groups, - product ads, - keywords, - negative
-keywords, and - targeting clauses (ASIN targeting). It furthermore provides
-methods to get `keyword recommendations`, which include bid recommendations for
-keyword targets, as well as `bid recommendations for ad groups`, which include
-bid recommendations for auto campaigns. And lastly, it provides also methods to
-request and retrieve reports via the API. To create an instance of the
-`AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials as a
-dictionary. The dictionary must contain the following keys: - `refresh_token` -
-`client_id` - `client_secret` - `profile_id` Upon initialization, the
-AmazonAdsAPIConnector object will create a new access token. This access token
-will be valid for 60 minutes, however, the object automatically requests a new
-access token in case it has expired when trying to make a new request. For more
-information about the Amazon Ads API, please visit the [official documentation]
-(https://advertising.amazon.com/API/docs/en-us/get-started/how-to-use-api). ##
-Examples ### Import the library ```python from amazon_ads_api_connector import
-AmazonAdsAPIConnector ``` ### Create an instance ```python api =
-AmazonAdsAPIConnector( { "refresh_token": "your_refresh_token", "client_id":
-"your_client_id", "client_secret": "your_client_secret", "profile_id":
-"your_profile_id", } ) ``` ### List campaigns ```python campaigns =
-api.list_campaigns() ``` ### Create campaigns ```python api.create_campaign
-( campaigns=[ { "name": "My Campaign", "targetingType": "MANUAL", "state":
-"ENABLED", "dynamicBidding": { "strategy": "LEGACY_FOR_SALES", }, "bugdget":
-{ "budgetType": "DAILY", "budget": 0, }, }, ] ) ``` Please note that all create
-and update methods expect a list of dictionaries as their only argument. This
-reflects the fact that the Amazon Ads API allows to create or update multiple
-objects at once. To ensure the greatest possible flexibility, the structure of
-the list and the dictionaries corresponds to the structure specified by the API
-and described in the API documentation. For more information about the
-structure of the lists and dictionaries, as well for information on data limits
-per request, please visit the [official documentation](https://
-advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod). ###
-Request and retrieve a report The module contains classes which represent basic
-configurations of the available report types: - `CampaignsReport` -
-`TargetingReport` - `SearchTermReport` - `AdvertisedProductReports` -
-`PurchasedProductReport` For more information about the report types, please
-visit the [official documentation](https://advertising.amazon.com/API/docs/en-
-us/guides/reporting/v3/report-types). To request a report you need to pass an
-instance of one of these classes to the `create_report` method of the
-`AmazonAdsAPIConnector` class. To customize the report, change the properties
-of the class instance before passing it to the `create_report` method.
-```python from amazon_ads_api_connector import SearchTermReport
-report_configuration = SearchTermReport("2023-10-01", â"2023-10-07") res =
-api.create_report(report_configuration) report = api.get_report(res) ``` Please
-note that report gerneration is asynchronous. The `create_report` method
-returns a dictionary containing the report ID. The `get_report` takes this
-dictionary as an argument and returns the report once it is completed and
-available. The completion of a report usually takes a few minutes and can take
-up to 3 hours. ## Dependencies This module depends on the `requests` library,
-which is not included in the Python standard library, but will be installed
-automatically when you install the `amazon-ads-api-connector` package. ##
-Disclaimer This module is not affiliated with Amazon in any way. It is an
-independent project that aims to provide a simple and easy-to-use interface to
-the Amazon Ads API for Sponsored Products campaign management.
+Type: text/markdown License-File: LICENSE.txt Requires-Dist: httpx # Amazon Ads
+API Connector A simple Python wrapper for the _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f_ _t_h_e_ _A_m_a_z_o_n_ _A_d_s
+_A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n_ _m_a_n_a_g_e_m_e_n_t. This module covers the key
+endpoints for managing Sponsored Products campaigns. This includes methods for
+authentication, pagination and report generation. It features keyword and
+negative keyword targeting, as well as product ASIN targeting and auto
+campaigns. Please note that this module does not yet support Sponsored Brands
+and Sponsored Display campaigns. ## Installation Amazon Ads API Connector is
+available on PyPI: ```bash pip install amazon-ads-api-connector ``` ## Getting
+started The primary class of the module is `AmazonAdsAPIConnector`. This class
+provides methods to create, list, update and delete - campaigns, - ad groups, -
+product ads, - keywords, - negative keywords, and - targeting clauses (ASIN
+targeting). It furthermore provides methods to get `keyword recommendations`,
+which include bid recommendations for keyword targets, as well as `bid
+recommendations for ad groups`, which include bid recommendations for auto
+campaigns. And lastly, it provides also methods to request and retrieve reports
+via the API. To create an instance of the `AmazonAdsAPIConnector`, you need to
+pass your Amazon Ads API credentials as a dictionary. The dictionary must
+contain the following keys: - `refresh_token` - `client_id` - `client_secret` -
+`profile_id` Upon initialization, the AmazonAdsAPIConnector object will create
+a new access token. This access token will be valid for 60 minutes, however,
+the object automatically requests a new access token in case it has expired
+when trying to make a new request. You furthermore need to specify the region
+of your Amazon Ads account. The region is specified by the `Region` enum, which
+is part of the `amazon_ads_api_connector` module. The Amazon Ads API supports
+the following regions: - North America: `Region.NA` - Europe: `Region.EU` - Far
+East: `Region.FE` For more information about the Amazon Ads API, please visit
+the [official documentation](https://advertising.amazon.com/API/docs/en-us/get-
+started/how-to-use-api). ## Examples ### Import the library ```python from
+amazon_ads_api_connector import AmazonAdsAPIConnector, Region ``` ### Create an
+instance ```python api = AmazonAdsAPIConnector( { "refresh_token":
+"your_refresh_token", "client_id": "your_client_id", "client_secret":
+"your_client_secret", "profile_id": "your_profile_id", }, Region.EU, ) ``` ###
+List campaigns ```python campaigns = api.list_campaigns() ``` ### Create
+campaigns ```python api.create_campaign( campaigns=[ { "name": "My Campaign",
+"targetingType": "MANUAL", "state": "ENABLED", "dynamicBidding": { "strategy":
+"LEGACY_FOR_SALES", }, "bugdget": { "budgetType": "DAILY", "budget": 0, }, }, ]
+) ``` Please note that all create and update methods expect a list of
+dictionaries as their only argument. This reflects the fact that the Amazon Ads
+API allows to create or update multiple objects at once. To ensure the greatest
+possible flexibility, the structure of the list and the dictionaries
+corresponds to the structure specified by the API and described in the API
+documentation. For more information about the structure of the lists and
+dictionaries, as well for information on data limits per request, please visit
+the [official documentation](https://advertising.amazon.com/API/docs/en-us/
+sponsored-products/3-0/openapi/prod). ### Request and retrieve a report The
+module contains classes which represent basic configurations of the available
+report types: - `CampaignsReport` - `TargetingReport` - `SearchTermReport` -
+`AdvertisedProductReports` - `PurchasedProductReport` For more information
+about the report types, please visit the [official documentation](https://
+advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To
+request a report you need to pass an instance of one of these classes to the
+`create_report` method of the `AmazonAdsAPIConnector` class. To customize the
+report, change the properties of the class instance before passing it to the
+`create_report` method. ```python from amazon_ads_api_connector import
+SearchTermReport report_configuration = SearchTermReport("2023-10-01",
+â"2023-10-07") res = api.create_report(report_configuration) report =
+api.get_report(res) ``` Please note that report gerneration is asynchronous.
+The `create_report` method returns a dictionary containing the report ID. The
+`get_report` takes this dictionary as an argument and returns the report once
+it is completed and available. The completion of a report usually takes a few
+minutes and can take up to 3 hours. ## Dependencies This module depends on the
+`httpx` library, which is not included in the Python standard library, but will
+be installed automatically when you install the `amazon-ads-api-connector`
+package. ## Disclaimer I am not affiliated with Amazon in any way. This module
+is an independent project that aims to provide a simple and easy-to-use
+interface to the Amazon Ads API for Sponsored Products campaign management. I
+do not guarantee the correctness or completeness of the module. Use it at your
+own risk.
```

### Comparing `amazon-ads-api-connector-0.1.4/README.md` & `amazon_ads_api_connector-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,30 +33,36 @@
 - `refresh_token`
 - `client_id`
 - `client_secret`
 - `profile_id`
 
 Upon initialization, the AmazonAdsAPIConnector object will create a new access token. This access token will be valid for 60 minutes, however, the object automatically requests a new access token in case it has expired when trying to make a new request.
 
+You furthermore need to specify the region of your Amazon Ads account. The region is specified by the `Region` enum, which is part of the `amazon_ads_api_connector` module. The Amazon Ads API supports the following regions:
+- North America: `Region.NA`
+- Europe: `Region.EU`
+- Far East: `Region.FE`
+
 For more information about the Amazon Ads API, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/get-started/how-to-use-api).
 
 ## Examples
 ### Import the library
 ```python
-from amazon_ads_api_connector import AmazonAdsAPIConnector
+from amazon_ads_api_connector import AmazonAdsAPIConnector, Region
 ```
 ### Create an instance
 ```python
 api = AmazonAdsAPIConnector(
     {
         "refresh_token": "your_refresh_token",
         "client_id": "your_client_id",
         "client_secret": "your_client_secret",
         "profile_id": "your_profile_id",
-    }
+    },
+    Region.EU,
 )
 ```
 ### List campaigns
 ```python
 campaigns = api.list_campaigns()
 ```
 ### Create campaigns
@@ -102,12 +108,12 @@
 res = api.create_report(report_configuration)
 report = api.get_report(res)
 ```
 Please note that report gerneration is asynchronous. The `create_report` method returns a dictionary containing the report ID. The `get_report` takes this dictionary as an argument and returns the report once it is completed and available. The completion of a report usually takes a few minutes and can take up to 3 hours.
 
 ## Dependencies
 
-This module depends on the `requests` library, which is not included in the Python standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
+This module depends on the `httpx` library, which is not included in the Python standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
 
 ## Disclaimer
 
-This module is not affiliated with Amazon in any way. It is an independent project that aims to provide a simple and easy-to-use interface to the Amazon Ads API for Sponsored Products campaign management.
+I am not affiliated with Amazon in any way. This module is an independent project that aims to provide a simple and easy-to-use interface to the Amazon Ads API for Sponsored Products campaign management. I do not guarantee the correctness or completeness of the module. Use it at your own risk.
```

#### html2text {}

```diff
@@ -15,49 +15,55 @@
 bid recommendations for auto campaigns. And lastly, it provides also methods to
 request and retrieve reports via the API. To create an instance of the
 `AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials as a
 dictionary. The dictionary must contain the following keys: - `refresh_token` -
 `client_id` - `client_secret` - `profile_id` Upon initialization, the
 AmazonAdsAPIConnector object will create a new access token. This access token
 will be valid for 60 minutes, however, the object automatically requests a new
-access token in case it has expired when trying to make a new request. For more
-information about the Amazon Ads API, please visit the [official documentation]
-(https://advertising.amazon.com/API/docs/en-us/get-started/how-to-use-api). ##
-Examples ### Import the library ```python from amazon_ads_api_connector import
-AmazonAdsAPIConnector ``` ### Create an instance ```python api =
-AmazonAdsAPIConnector( { "refresh_token": "your_refresh_token", "client_id":
-"your_client_id", "client_secret": "your_client_secret", "profile_id":
-"your_profile_id", } ) ``` ### List campaigns ```python campaigns =
-api.list_campaigns() ``` ### Create campaigns ```python api.create_campaign
-( campaigns=[ { "name": "My Campaign", "targetingType": "MANUAL", "state":
-"ENABLED", "dynamicBidding": { "strategy": "LEGACY_FOR_SALES", }, "bugdget":
-{ "budgetType": "DAILY", "budget": 0, }, }, ] ) ``` Please note that all create
-and update methods expect a list of dictionaries as their only argument. This
-reflects the fact that the Amazon Ads API allows to create or update multiple
-objects at once. To ensure the greatest possible flexibility, the structure of
-the list and the dictionaries corresponds to the structure specified by the API
-and described in the API documentation. For more information about the
-structure of the lists and dictionaries, as well for information on data limits
-per request, please visit the [official documentation](https://
-advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod). ###
-Request and retrieve a report The module contains classes which represent basic
-configurations of the available report types: - `CampaignsReport` -
-`TargetingReport` - `SearchTermReport` - `AdvertisedProductReports` -
-`PurchasedProductReport` For more information about the report types, please
-visit the [official documentation](https://advertising.amazon.com/API/docs/en-
-us/guides/reporting/v3/report-types). To request a report you need to pass an
-instance of one of these classes to the `create_report` method of the
-`AmazonAdsAPIConnector` class. To customize the report, change the properties
-of the class instance before passing it to the `create_report` method.
-```python from amazon_ads_api_connector import SearchTermReport
-report_configuration = SearchTermReport("2023-10-01", â"2023-10-07") res =
-api.create_report(report_configuration) report = api.get_report(res) ``` Please
-note that report gerneration is asynchronous. The `create_report` method
-returns a dictionary containing the report ID. The `get_report` takes this
-dictionary as an argument and returns the report once it is completed and
-available. The completion of a report usually takes a few minutes and can take
-up to 3 hours. ## Dependencies This module depends on the `requests` library,
-which is not included in the Python standard library, but will be installed
-automatically when you install the `amazon-ads-api-connector` package. ##
-Disclaimer This module is not affiliated with Amazon in any way. It is an
-independent project that aims to provide a simple and easy-to-use interface to
-the Amazon Ads API for Sponsored Products campaign management.
+access token in case it has expired when trying to make a new request. You
+furthermore need to specify the region of your Amazon Ads account. The region
+is specified by the `Region` enum, which is part of the
+`amazon_ads_api_connector` module. The Amazon Ads API supports the following
+regions: - North America: `Region.NA` - Europe: `Region.EU` - Far East:
+`Region.FE` For more information about the Amazon Ads API, please visit the
+[official documentation](https://advertising.amazon.com/API/docs/en-us/get-
+started/how-to-use-api). ## Examples ### Import the library ```python from
+amazon_ads_api_connector import AmazonAdsAPIConnector, Region ``` ### Create an
+instance ```python api = AmazonAdsAPIConnector( { "refresh_token":
+"your_refresh_token", "client_id": "your_client_id", "client_secret":
+"your_client_secret", "profile_id": "your_profile_id", }, Region.EU, ) ``` ###
+List campaigns ```python campaigns = api.list_campaigns() ``` ### Create
+campaigns ```python api.create_campaign( campaigns=[ { "name": "My Campaign",
+"targetingType": "MANUAL", "state": "ENABLED", "dynamicBidding": { "strategy":
+"LEGACY_FOR_SALES", }, "bugdget": { "budgetType": "DAILY", "budget": 0, }, }, ]
+) ``` Please note that all create and update methods expect a list of
+dictionaries as their only argument. This reflects the fact that the Amazon Ads
+API allows to create or update multiple objects at once. To ensure the greatest
+possible flexibility, the structure of the list and the dictionaries
+corresponds to the structure specified by the API and described in the API
+documentation. For more information about the structure of the lists and
+dictionaries, as well for information on data limits per request, please visit
+the [official documentation](https://advertising.amazon.com/API/docs/en-us/
+sponsored-products/3-0/openapi/prod). ### Request and retrieve a report The
+module contains classes which represent basic configurations of the available
+report types: - `CampaignsReport` - `TargetingReport` - `SearchTermReport` -
+`AdvertisedProductReports` - `PurchasedProductReport` For more information
+about the report types, please visit the [official documentation](https://
+advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To
+request a report you need to pass an instance of one of these classes to the
+`create_report` method of the `AmazonAdsAPIConnector` class. To customize the
+report, change the properties of the class instance before passing it to the
+`create_report` method. ```python from amazon_ads_api_connector import
+SearchTermReport report_configuration = SearchTermReport("2023-10-01",
+â"2023-10-07") res = api.create_report(report_configuration) report =
+api.get_report(res) ``` Please note that report gerneration is asynchronous.
+The `create_report` method returns a dictionary containing the report ID. The
+`get_report` takes this dictionary as an argument and returns the report once
+it is completed and available. The completion of a report usually takes a few
+minutes and can take up to 3 hours. ## Dependencies This module depends on the
+`httpx` library, which is not included in the Python standard library, but will
+be installed automatically when you install the `amazon-ads-api-connector`
+package. ## Disclaimer I am not affiliated with Amazon in any way. This module
+is an independent project that aims to provide a simple and easy-to-use
+interface to the Amazon Ads API for Sponsored Products campaign management. I
+do not guarantee the correctness or completeness of the module. Use it at your
+own risk.
```

### Comparing `amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/amazon_ads_api_connector.py` & `amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_ads_api_connector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 import json
 import gzip
-import requests
+import httpx
 from time import sleep
-from .report_types import Report
+from .amazon_reports import Report
+from .amazon_regions import Region
 
 
 class AmazonAdsAPIConnector:
     """
     AmazonAdsAPIConnector is a wrapper for the Amazon Advertising API.
     It covers the most important endpoints to manage sponsored products campaigns.
     It also provides methods for authentication, pagination and report creation.
     """
 
     def __init__(
         self,
         creds: dict,
+        region: Region,
     ) -> None:
         """
         Args:
             creds (dict): A dictionary containing the credentials for the API including the client_id, client_secret, refresh_token and profile_id.
+            region (Region): The region of your Amazon account. Possible values are Region.NA, Region.EU and Region.FE.
         """
         self.creds = creds
+        self.base_url = region.value["url"]
+        self.authorization_url = region.value["authorization_url"]
         self.refresh_access_token()
 
     def refresh_access_token(
         self,
     ) -> dict:
         """
         Refreshes the access token and the refresh token.
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://api.amazon.co.uk/auth/o2/token"
+        url = self.authorization_url
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
         payload = f"grant_type=refresh_token&refresh_token={self.creds['refresh_token']}&client_id={self.creds['client_id']}&client_secret={self.creds['client_secret']}"
-        response = requests.request(
+        response = httpx.request(
             "POST",
             url,
             headers=headers,
             data=payload,
         )
         result = json.loads(response.text)
         self.creds["access_token"] = result["access_token"]
@@ -82,24 +87,24 @@
             url (str): The url of the request.
             headers (dict): The headers of the request.
             payload (dict): The payload of the request.
 
         Returns:
             dict | list: The response from the API.
         """
-        response = requests.request(
+        response = httpx.request(
             method,
             url,
             headers=headers,
             data=json.dumps(payload),
         )
         if response.status_code == 401:
             self.refresh_access_token()
             headers = self._get_headers(headers["Content-Type"])
-            response = requests.request(
+            response = httpx.request(
                 method,
                 url,
                 headers=headers,
                 data=json.dumps(payload),
             )
         if response.status_code in [200, 207]:
             return json.loads(response.text)
@@ -160,15 +165,15 @@
             states (list, optional): The states of the campaigns to be listed. Defaults to ["ENABLED", "PAUSED", "ARCHIVED"].
             include_extended_data_fields (bool, optional): Whether to include extended data fields. Defaults to False.
             name_contains (list, optional): The strings the campaign names should contain. Defaults to [""].
 
         Returns:
             list: The list of campaigns.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/campaigns/list"
+        url = f"{self.base_url}/sp/campaigns/list"
         payload = {
             "includeExtendedDataFields": include_extended_data_fields,
             "stateFilter": {"include": states},
             "nameFilter": {
                 "queryTermMatchType": "BROAD_MATCH",
                 "include": name_contains,
             },
@@ -187,15 +192,15 @@
             campaigns (list): The campaigns to be created.
             For more information on the structure of the campaigns, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/Campaigns/operation/CreateSponsoredProductsCampaigns
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/campaigns"
+        url = f"{self.base_url}/sp/campaigns"
         payload = {
             "campaigns": campaigns,
         }
         headers = self._get_headers("application/vnd.spCampaign.v3+json")
         response = self._request_api(
             "POST",
             url,
@@ -215,15 +220,15 @@
             campaigns (list): The campaigns to be updated.
             For more information on the structure of the campaigns, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/Campaigns/operation/UpdateSponsoredProductsCampaigns
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/campaigns"
+        url = f"{self.base_url}/sp/campaigns"
         payload = {
             "campaigns": campaigns,
         }
         headers = self._get_headers("application/vnd.spCampaign.v3+json")
         response = self._request_api(
             "PUT",
             url,
@@ -241,15 +246,15 @@
 
         Args:
             campaign_ids (list): The ids of the campaigns to be deleted.
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/campaigns/delete"
+        url = f"{self.base_url}/sp/campaigns/delete"
         payload = {
             "campaignIdFilter": {
                 "include": campaign_ids,
             }
         }
         headers = self._get_headers("application/vnd.spCampaign.v3+json")
         return self._request_api(
@@ -278,15 +283,15 @@
             states (list, optional): The states of the ad groups to be listed. Defaults to ["ENABLED", "PAUSED", "ARCHIVED"].
             include_extended_data_fields (bool, optional): Whether to include extended data fields. Defaults to False.
             name_contains (list, optional): The strings the ad group names should contain. Defaults to [""].
 
         Returns:
             list: The list of ad groups.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/adGroups/list"
+        url = f"{self.base_url}/sp/adGroups/list"
         payload = {
             "campaignIdFilter": {"include": campaign_ids},
             "stateFilter": {"include": states},
             "includeExtendedDataFields": include_extended_data_fields,
             "nameFilter": {
                 "queryTermMatchType": "BROAD_MATCH",
                 "include": name_contains,
@@ -306,15 +311,15 @@
             ad_groups (list): The ad groups to be created.
             For more information on the structure of the ad groups, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/AdGroups/operation/CreateSponsoredProductsAdGroups
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/adGroups"
+        url = f"{self.base_url}/sp/adGroups"
         payload = {
             "adGroups": ad_groups,
         }
         headers = self._get_headers("application/vnd.spAdGroup.v3+json")
         return self._request_api(
             "POST",
             url,
@@ -333,15 +338,15 @@
             ad_groups (list): The ad groups to be updated.
             For more information on the structure of the ad groups, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/AdGroups/operation/UpdateSponsoredProductsAdGroups
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/adGroups"
+        url = f"{self.base_url}/sp/adGroups"
         payload = {
             "adGroups": ad_groups,
         }
         headers = self._get_headers("application/vnd.spAdGroup.v3+json")
         return self._request_api(
             "PUT",
             url,
@@ -358,15 +363,15 @@
 
         Args:
             ad_group_ids (list): The ids of the ad groups to be deleted.
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/adGroups/delete"
+        url = f"{self.base_url}/sp/adGroups/delete"
         payload = {
             "adGroupIdFilter": {
                 "include": ad_group_ids,
             }
         }
         headers = self._get_headers("application/vnd.spAdGroup.v3+json")
         return self._request_api(
@@ -392,15 +397,15 @@
 
         Args:
             campaign_ids (list, optional): The ids of the campaigns the product ads belong to. Defaults to [].
             ad_group_ids (list, optional): The ids of the ad groups the product ads belong to. Defaults to [].
             states (list, optional): The states of the product ads to be listed. Defaults to ["ENABLED", "PAUSED", "ARCHIVED"].
             include_extended_data_fields (bool, optional): Whether to include extended data fields. Defaults to False.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/productAds/list"
+        url = f"{self.base_url}/sp/productAds/list"
         payload = {
             "campaignIdFilter": {"include": campaign_ids},
             "adGroupIdFilter": {"include": ad_group_ids},
             "stateFilter": {"include": states},
             "includeExtendedDataFields": include_extended_data_fields,
         }
         headers = self._get_headers("application/vnd.spProductAd.v3+json")
@@ -417,15 +422,15 @@
             product_ads (list): The product ads to be created.
             For more information on the structure of the product ads, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/ProductAds/operation/CreateSponsoredProductsProductAds
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/productAds"
+        url = f"{self.base_url}/sp/productAds"
         payload = {
             "productAds": product_ads,
         }
         headers = self._get_headers("application/vnd.spProductAd.v3+json")
         return self._request_api(
             "POST",
             url,
@@ -444,15 +449,15 @@
             product_ads (list): The product ads to be updated.
             For more information on the structure of the product ads, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/ProductAds/operation/UpdateSponsoredProductsProductAds
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/productAds"
+        url = f"{self.base_url}/sp/productAds"
         payload = {
             "productAds": product_ads,
         }
         headers = self._get_headers("application/vnd.spProductAd.v3+json")
         return self._request_api(
             "PUT",
             url,
@@ -469,15 +474,15 @@
 
         Args:
             product_ad_ids (list): The ids of the product ads to be deleted.
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/productAds/delete"
+        url = f"{self.base_url}/sp/productAds/delete"
         payload = {
             "adIdFilter": {
                 "include": product_ad_ids,
             }
         }
         headers = self._get_headers("application/vnd.spProductAd.v3+json")
         return self._request_api(
@@ -508,15 +513,15 @@
             states (list, optional): The states of the keywords to be listed. Defaults to ["ENABLED", "PAUSED", "ARCHIVED"].
             match_types (list, optional): The match types of the keywords to be listed. Defaults to ["BROAD", "EXACT", "PHRASE"].
             include_extended_data_fields (bool, optional): Whether to include extended data fields. Defaults to False.
 
         Returns:
             list: The list of keywords.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/keywords/list"
+        url = f"{self.base_url}/sp/keywords/list"
         payload = {
             "campaignIdFilter": {"include": campaign_ids},
             "adGroupIdFilter": {"include": ad_group_ids},
             "stateFilter": {"include": states},
             "matchTypeFilter": match_types,
             "includeExtendedDataFields": include_extended_data_fields,
         }
@@ -534,15 +539,15 @@
             keywords (list): The keywords to be created.
             For more information on the structure of the keywords, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/Keywords/operation/CreateSponsoredProductsKeywords
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/keywords"
+        url = f"{self.base_url}/sp/keywords"
         payload = {
             "keywords": keywords,
         }
         headers = self._get_headers("application/vnd.spKeyword.v3+json")
         return self._request_api(
             "POST",
             url,
@@ -561,15 +566,15 @@
             keywords (list): The keywords to be updated.
             For more information on the structure of the keywords, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/Keywords/operation/UpdateSponsoredProductsKeywords
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/keywords"
+        url = f"{self.base_url}/sp/keywords"
         payload = {
             "keywords": keywords,
         }
         headers = self._get_headers("application/vnd.spKeyword.v3+json")
         return self._request_api(
             "PUT",
             url,
@@ -586,15 +591,15 @@
 
         Args:
             keyword_ids (list): The ids of the keywords to be deleted.
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/keywords/delete"
+        url = f"{self.base_url}/sp/keywords/delete"
         payload = {
             "keywordIdFilter": {
                 "include": keyword_ids,
             }
         }
         headers = self._get_headers("application/vnd.spKeyword.v3+json")
         return self._request_api(
@@ -623,15 +628,15 @@
             ad_group_ids (list, optional): The ids of the ad groups the negative keywords belong to. Defaults to [].
             states (list, optional): The states of the negative keywords to be listed. Defaults to ["ENABLED", "PAUSED", "ARCHIVED"].
             include_extended_data_fields (bool, optional): Whether to include extended data fields. Defaults to False.
 
         Returns:
             list: The list of negative keywords.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/negativeKeywords/list"
+        url = f"{self.base_url}/sp/negativeKeywords/list"
         payload = {
             "campaignIdFilter": {"include": campaign_ids},
             "adGroupIdFilter": {"include": ad_group_ids},
             "stateFilter": {"include": states},
             "includeExtendedDataFields": include_extended_data_fields,
         }
         headers = self._get_headers("application/vnd.spNegativeKeyword.v3+json")
@@ -648,15 +653,15 @@
             negative_keywords (list): The negative keywords to be created.
             For more information on the structure of the negative keywords, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/NegativeKeywords/operation/CreateSponsoredProductsNegativeKeywords
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/negativeKeywords"
+        url = f"{self.base_url}/sp/negativeKeywords"
         payload = {
             "negativeKeywords": negative_keywords,
         }
         headers = self._get_headers("application/vnd.spNegativeKeyword.v3+json")
         return self._request_api(
             "POST",
             url,
@@ -675,15 +680,15 @@
             negative_keywords (list): The negative keywords to be updated.
             For more information on the structure of the negative keywords, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/NegativeKeywords/operation/UpdateSponsoredProductsNegativeKeywords
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/negativeKeywords"
+        url = f"{self.base_url}/sp/negativeKeywords"
         payload = {
             "negativeKeywords": negative_keywords,
         }
         headers = self._get_headers("application/vnd.spNegativeKeyword.v3+json")
         return self._request_api(
             "PUT",
             url,
@@ -700,15 +705,15 @@
 
         Args:
             negative_keyword_ids (list): The ids of the negative keywords to be deleted.
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/negativeKeywords/delete"
+        url = f"{self.base_url}/sp/negativeKeywords/delete"
         payload = {
             "keywordIdFilter": {
                 "include": negative_keyword_ids,
             }
         }
         headers = self._get_headers("application/vnd.spNegativeKeyword.v3+json")
         return self._request_api(
@@ -737,15 +742,15 @@
             ad_group_ids (list, optional): The ids of the ad groups the targeting clauses belong to. Defaults to [].
             states (list, optional): The states of the targeting clauses to be listed. Defaults to ["ENABLED", "PAUSED", "ARCHIVED"].
             include_extended_data_fields (bool, optional): Whether to include extended data fields. Defaults to False.
 
         Returns:
             list: The list of targeting clauses.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/targets/list"
+        url = f"{self.base_url}/sp/targets/list"
         payload = {
             "campaignIdFilter": {"include": campaign_ids},
             "adGroupIdFilter": {"include": ad_group_ids},
             "stateFilter": {"include": states},
             "includeExtendedDataFields": include_extended_data_fields,
         }
         headers = self._get_headers("application/vnd.spTargetingClause.v3+json")
@@ -762,15 +767,15 @@
             targeting_clauses (list): The targeting clauses to be created.
             For more information on the structure of the targeting clauses, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/TargetingClauses/operation/CreateSponsoredProductsTargetingClauses
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/targets"
+        url = f"{self.base_url}/sp/targets"
         payload = {
             "targetingClauses": targeting_clauses,
         }
         headers = self._get_headers("application/vnd.spTargetingClause.v3+json")
         return self._request_api(
             "POST",
             url,
@@ -789,15 +794,15 @@
             targeting_clauses (list): The targeting clauses to be updated.
             For more information on the structure of the targeting clauses, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/CampaignNegativeTargetingClauses/operation/UpdateSponsoredProductsCampaignNegativeTargetingClauses
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/targets"
+        url = f"{self.base_url}/sp/targets"
         payload = {
             "targetingClauses": targeting_clauses,
         }
         headers = self._get_headers("application/vnd.spTargetingClause.v3+json")
         return self._request_api(
             "PUT",
             url,
@@ -814,15 +819,15 @@
 
         Args:
             targeting_clause_ids (list): The ids of the targeting clauses to be deleted.
 
         Returns:
             dict: The response from the API.
         """
-        url = "https://advertising-api-eu.amazon.com/sp/targets/delete"
+        url = f"{self.base_url}/sp/targets/delete"
         payload = {
             "targetIdFilter": {
                 "include": targeting_clause_ids,
             }
         }
         headers = self._get_headers("application/vnd.spTargetingClause.v3+json")
         return self._request_api(
@@ -847,17 +852,15 @@
             targets (list): The targets for which to get keyword recommendations.
             For more information on the structure of the targets, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/Keyword-Recommendations/operation/getRankedKeywordRecommendation
 
         Returns:
             dict: The response from the API.
         """
-        url = (
-            "https://advertising-api-eu.amazon.com/sp/targets/keywords/recommendations"
-        )
+        url = f"{self.base_url}/sp/targets/keywords/recommendations"
         payload = {
             "recommendationType": "KEYWORDS_FOR_ADGROUP",
             "campaignId": campaign_id,
             "adGroupId": ad_group_id,
             "targets": targets,
             "maxRecommendations": 0,
         }
@@ -887,15 +890,15 @@
         Args:
             campaign_id (str): The id of the campaign.
             ad_group_ids (list): The ids of the ad groups.
             targeting_expressions (list, optional): The targeting expressions for which to get bid recommendations. Defaults to [{"type": "CLOSE_MATCH"}, {"type": "LOOSE_MATCH"}, {"type": "SUBSTITUTES"}, {"type": "COMPLEMENTS"}].
             For more information on the structure of the targeting expressions, see
             https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod#tag/Theme-based-bid-recommendations/operation/GetThemeBasedBidRecommendationForAdGroup_v1
         """
-        url = "https://advertising-api-eu.amazon.com/sp/targets/bid/recommendations"
+        url = f"{self.base_url}/sp/targets/bid/recommendations"
         payload = {
             "targetingExpressions": targeting_expressions,
             "campaignId": campaign_id,
             "recommendationType": "BIDS_FOR_EXISTING_AD_GROUP",
             "adGroupId": ad_group_ids,
         }
         headers = self._get_headers(
@@ -921,15 +924,15 @@
             https://advertising.amazon.com/API/docs/en-us/offline-report-prod-3p
             and
             https://advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types#tag/Asynchronous-Reports/operation/createAsyncReport
 
         Returns:
             dict: The response from the API. It contains the report id.
         """
-        url = "https://advertising-api-eu.amazon.com/reporting/reports"
+        url = f"{self.base_url}/reporting/reports"
         payload = {
             "name": "Report",
             "startDate": report.start_date,
             "endDate": report.end_date,
             "configuration": {
                 "adProduct": "SPONSORED_PRODUCTS",
                 "groupBy": report.group_by,
@@ -956,15 +959,15 @@
 
         Args:
             report_request (dict): The report request containing the report id.
 
         Returns:
             dict: The report.
         """
-        url = f"https://advertising-api-eu.amazon.com/reporting/reports/{report_request['reportId']}"
+        url = f"{self.base_url}/reporting/reports/{report_request['reportId']}"
         headers = self._get_headers("application/vnd.advertisingReport+json")
         while True:
-            response = json.loads(requests.request("GET", url, headers=headers).text)
+            response = json.loads(httpx.request("GET", url, headers=headers).text)
             if response["status"] == "COMPLETED":
-                report = requests.request("GET", response["url"]).content
+                report = httpx.request("GET", response["url"]).content
                 return json.loads(gzip.decompress(report))
             sleep(5)
```

### Comparing `amazon-ads-api-connector-0.1.4/amazon_ads_api_connector/report_types.py` & `amazon_ads_api_connector-0.1.5/amazon_ads_api_connector/amazon_reports.py`

 * *Files identical despite different names*

### Comparing `amazon-ads-api-connector-0.1.4/amazon_ads_api_connector.egg-info/PKG-INFO` & `amazon_ads_api_connector-0.1.5/amazon_ads_api_connector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: amazon-ads-api-connector
-Version: 0.1.4
+Version: 0.1.5
 Summary: API wrapper for the Amazon Ads API
 Author: Markus U. Wahl
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt 
-Requires-Dist: requests
-Requires-Dist: types-requests
+Requires-Dist: httpx
 
 # Amazon Ads API Connector
 
 A simple Python wrapper for the <a href="https://advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod">latest version of the Amazon Ads API for Sponsored Products campaign management</a>.
 
 This module covers the key endpoints for managing Sponsored Products campaigns. This includes methods for authentication, pagination and report generation. It features keyword and negative keyword targeting, as well as product ASIN targeting and auto campaigns. 
 
@@ -43,30 +42,36 @@
 - `refresh_token`
 - `client_id`
 - `client_secret`
 - `profile_id`
 
 Upon initialization, the AmazonAdsAPIConnector object will create a new access token. This access token will be valid for 60 minutes, however, the object automatically requests a new access token in case it has expired when trying to make a new request.
 
+You furthermore need to specify the region of your Amazon Ads account. The region is specified by the `Region` enum, which is part of the `amazon_ads_api_connector` module. The Amazon Ads API supports the following regions:
+- North America: `Region.NA`
+- Europe: `Region.EU`
+- Far East: `Region.FE`
+
 For more information about the Amazon Ads API, please visit the [official documentation](https://advertising.amazon.com/API/docs/en-us/get-started/how-to-use-api).
 
 ## Examples
 ### Import the library
 ```python
-from amazon_ads_api_connector import AmazonAdsAPIConnector
+from amazon_ads_api_connector import AmazonAdsAPIConnector, Region
 ```
 ### Create an instance
 ```python
 api = AmazonAdsAPIConnector(
     {
         "refresh_token": "your_refresh_token",
         "client_id": "your_client_id",
         "client_secret": "your_client_secret",
         "profile_id": "your_profile_id",
-    }
+    },
+    Region.EU,
 )
 ```
 ### List campaigns
 ```python
 campaigns = api.list_campaigns()
 ```
 ### Create campaigns
@@ -112,12 +117,12 @@
 res = api.create_report(report_configuration)
 report = api.get_report(res)
 ```
 Please note that report gerneration is asynchronous. The `create_report` method returns a dictionary containing the report ID. The `get_report` takes this dictionary as an argument and returns the report once it is completed and available. The completion of a report usually takes a few minutes and can take up to 3 hours.
 
 ## Dependencies
 
-This module depends on the `requests` library, which is not included in the Python standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
+This module depends on the `httpx` library, which is not included in the Python standard library, but will be installed automatically when you install the `amazon-ads-api-connector` package.
 
 ## Disclaimer
 
-This module is not affiliated with Amazon in any way. It is an independent project that aims to provide a simple and easy-to-use interface to the Amazon Ads API for Sponsored Products campaign management.
+I am not affiliated with Amazon in any way. This module is an independent project that aims to provide a simple and easy-to-use interface to the Amazon Ads API for Sponsored Products campaign management. I do not guarantee the correctness or completeness of the module. Use it at your own risk.
```

#### html2text {}

```diff
@@ -1,66 +1,71 @@
-Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: amazon-ads-api-connector Version: 0.1.5 Summary:
 API wrapper for the Amazon Ads API Author: Markus U. Wahl Description-Content-
-Type: text/markdown License-File: LICENSE.txt Requires-Dist: requests Requires-
-Dist: types-requests # Amazon Ads API Connector A simple Python wrapper for the
-_l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f_ _t_h_e_ _A_m_a_z_o_n_ _A_d_s_ _A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n
-_m_a_n_a_g_e_m_e_n_t. This module covers the key endpoints for managing Sponsored
-Products campaigns. This includes methods for authentication, pagination and
-report generation. It features keyword and negative keyword targeting, as well
-as product ASIN targeting and auto campaigns. Please note that this module does
-not yet support Sponsored Brands and Sponsored Display campaigns. ##
-Installation Amazon Ads API Connector is available on PyPI: ```bash pip install
-amazon-ads-api-connector ``` ## Getting started The primary class of the module
-is `AmazonAdsAPIConnector`. This class provides methods to create, list, update
-and delete - campaigns, - ad groups, - product ads, - keywords, - negative
-keywords, and - targeting clauses (ASIN targeting). It furthermore provides
-methods to get `keyword recommendations`, which include bid recommendations for
-keyword targets, as well as `bid recommendations for ad groups`, which include
-bid recommendations for auto campaigns. And lastly, it provides also methods to
-request and retrieve reports via the API. To create an instance of the
-`AmazonAdsAPIConnector`, you need to pass your Amazon Ads API credentials as a
-dictionary. The dictionary must contain the following keys: - `refresh_token` -
-`client_id` - `client_secret` - `profile_id` Upon initialization, the
-AmazonAdsAPIConnector object will create a new access token. This access token
-will be valid for 60 minutes, however, the object automatically requests a new
-access token in case it has expired when trying to make a new request. For more
-information about the Amazon Ads API, please visit the [official documentation]
-(https://advertising.amazon.com/API/docs/en-us/get-started/how-to-use-api). ##
-Examples ### Import the library ```python from amazon_ads_api_connector import
-AmazonAdsAPIConnector ``` ### Create an instance ```python api =
-AmazonAdsAPIConnector( { "refresh_token": "your_refresh_token", "client_id":
-"your_client_id", "client_secret": "your_client_secret", "profile_id":
-"your_profile_id", } ) ``` ### List campaigns ```python campaigns =
-api.list_campaigns() ``` ### Create campaigns ```python api.create_campaign
-( campaigns=[ { "name": "My Campaign", "targetingType": "MANUAL", "state":
-"ENABLED", "dynamicBidding": { "strategy": "LEGACY_FOR_SALES", }, "bugdget":
-{ "budgetType": "DAILY", "budget": 0, }, }, ] ) ``` Please note that all create
-and update methods expect a list of dictionaries as their only argument. This
-reflects the fact that the Amazon Ads API allows to create or update multiple
-objects at once. To ensure the greatest possible flexibility, the structure of
-the list and the dictionaries corresponds to the structure specified by the API
-and described in the API documentation. For more information about the
-structure of the lists and dictionaries, as well for information on data limits
-per request, please visit the [official documentation](https://
-advertising.amazon.com/API/docs/en-us/sponsored-products/3-0/openapi/prod). ###
-Request and retrieve a report The module contains classes which represent basic
-configurations of the available report types: - `CampaignsReport` -
-`TargetingReport` - `SearchTermReport` - `AdvertisedProductReports` -
-`PurchasedProductReport` For more information about the report types, please
-visit the [official documentation](https://advertising.amazon.com/API/docs/en-
-us/guides/reporting/v3/report-types). To request a report you need to pass an
-instance of one of these classes to the `create_report` method of the
-`AmazonAdsAPIConnector` class. To customize the report, change the properties
-of the class instance before passing it to the `create_report` method.
-```python from amazon_ads_api_connector import SearchTermReport
-report_configuration = SearchTermReport("2023-10-01", â"2023-10-07") res =
-api.create_report(report_configuration) report = api.get_report(res) ``` Please
-note that report gerneration is asynchronous. The `create_report` method
-returns a dictionary containing the report ID. The `get_report` takes this
-dictionary as an argument and returns the report once it is completed and
-available. The completion of a report usually takes a few minutes and can take
-up to 3 hours. ## Dependencies This module depends on the `requests` library,
-which is not included in the Python standard library, but will be installed
-automatically when you install the `amazon-ads-api-connector` package. ##
-Disclaimer This module is not affiliated with Amazon in any way. It is an
-independent project that aims to provide a simple and easy-to-use interface to
-the Amazon Ads API for Sponsored Products campaign management.
+Type: text/markdown License-File: LICENSE.txt Requires-Dist: httpx # Amazon Ads
+API Connector A simple Python wrapper for the _l_a_t_e_s_t_ _v_e_r_s_i_o_n_ _o_f_ _t_h_e_ _A_m_a_z_o_n_ _A_d_s
+_A_P_I_ _f_o_r_ _S_p_o_n_s_o_r_e_d_ _P_r_o_d_u_c_t_s_ _c_a_m_p_a_i_g_n_ _m_a_n_a_g_e_m_e_n_t. This module covers the key
+endpoints for managing Sponsored Products campaigns. This includes methods for
+authentication, pagination and report generation. It features keyword and
+negative keyword targeting, as well as product ASIN targeting and auto
+campaigns. Please note that this module does not yet support Sponsored Brands
+and Sponsored Display campaigns. ## Installation Amazon Ads API Connector is
+available on PyPI: ```bash pip install amazon-ads-api-connector ``` ## Getting
+started The primary class of the module is `AmazonAdsAPIConnector`. This class
+provides methods to create, list, update and delete - campaigns, - ad groups, -
+product ads, - keywords, - negative keywords, and - targeting clauses (ASIN
+targeting). It furthermore provides methods to get `keyword recommendations`,
+which include bid recommendations for keyword targets, as well as `bid
+recommendations for ad groups`, which include bid recommendations for auto
+campaigns. And lastly, it provides also methods to request and retrieve reports
+via the API. To create an instance of the `AmazonAdsAPIConnector`, you need to
+pass your Amazon Ads API credentials as a dictionary. The dictionary must
+contain the following keys: - `refresh_token` - `client_id` - `client_secret` -
+`profile_id` Upon initialization, the AmazonAdsAPIConnector object will create
+a new access token. This access token will be valid for 60 minutes, however,
+the object automatically requests a new access token in case it has expired
+when trying to make a new request. You furthermore need to specify the region
+of your Amazon Ads account. The region is specified by the `Region` enum, which
+is part of the `amazon_ads_api_connector` module. The Amazon Ads API supports
+the following regions: - North America: `Region.NA` - Europe: `Region.EU` - Far
+East: `Region.FE` For more information about the Amazon Ads API, please visit
+the [official documentation](https://advertising.amazon.com/API/docs/en-us/get-
+started/how-to-use-api). ## Examples ### Import the library ```python from
+amazon_ads_api_connector import AmazonAdsAPIConnector, Region ``` ### Create an
+instance ```python api = AmazonAdsAPIConnector( { "refresh_token":
+"your_refresh_token", "client_id": "your_client_id", "client_secret":
+"your_client_secret", "profile_id": "your_profile_id", }, Region.EU, ) ``` ###
+List campaigns ```python campaigns = api.list_campaigns() ``` ### Create
+campaigns ```python api.create_campaign( campaigns=[ { "name": "My Campaign",
+"targetingType": "MANUAL", "state": "ENABLED", "dynamicBidding": { "strategy":
+"LEGACY_FOR_SALES", }, "bugdget": { "budgetType": "DAILY", "budget": 0, }, }, ]
+) ``` Please note that all create and update methods expect a list of
+dictionaries as their only argument. This reflects the fact that the Amazon Ads
+API allows to create or update multiple objects at once. To ensure the greatest
+possible flexibility, the structure of the list and the dictionaries
+corresponds to the structure specified by the API and described in the API
+documentation. For more information about the structure of the lists and
+dictionaries, as well for information on data limits per request, please visit
+the [official documentation](https://advertising.amazon.com/API/docs/en-us/
+sponsored-products/3-0/openapi/prod). ### Request and retrieve a report The
+module contains classes which represent basic configurations of the available
+report types: - `CampaignsReport` - `TargetingReport` - `SearchTermReport` -
+`AdvertisedProductReports` - `PurchasedProductReport` For more information
+about the report types, please visit the [official documentation](https://
+advertising.amazon.com/API/docs/en-us/guides/reporting/v3/report-types). To
+request a report you need to pass an instance of one of these classes to the
+`create_report` method of the `AmazonAdsAPIConnector` class. To customize the
+report, change the properties of the class instance before passing it to the
+`create_report` method. ```python from amazon_ads_api_connector import
+SearchTermReport report_configuration = SearchTermReport("2023-10-01",
+â"2023-10-07") res = api.create_report(report_configuration) report =
+api.get_report(res) ``` Please note that report gerneration is asynchronous.
+The `create_report` method returns a dictionary containing the report ID. The
+`get_report` takes this dictionary as an argument and returns the report once
+it is completed and available. The completion of a report usually takes a few
+minutes and can take up to 3 hours. ## Dependencies This module depends on the
+`httpx` library, which is not included in the Python standard library, but will
+be installed automatically when you install the `amazon-ads-api-connector`
+package. ## Disclaimer I am not affiliated with Amazon in any way. This module
+is an independent project that aims to provide a simple and easy-to-use
+interface to the Amazon Ads API for Sponsored Products campaign management. I
+do not guarantee the correctness or completeness of the module. Use it at your
+own risk.
```

