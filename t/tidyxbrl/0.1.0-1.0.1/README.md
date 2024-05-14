# Comparing `tmp/tidyxbrl-0.1.0.tar.gz` & `tmp/tidyxbrl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyxbrl-0.1.0.tar", last modified: Tue May 14 03:13:33 2024, max compression
+gzip compressed data, was "tidyxbrl-1.0.1.tar", last modified: Tue May 14 03:39:10 2024, max compression
```

## Comparing `tidyxbrl-0.1.0.tar` & `tidyxbrl-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 03:13:33.022775 tidyxbrl-0.1.0/
--rw-rw-rw-   0        0        0     1091 2021-11-14 19:09:57.000000 tidyxbrl-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4997 2024-05-14 03:13:33.020781 tidyxbrl-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4305 2021-11-19 03:57:45.000000 tidyxbrl-0.1.0/README.md
--rw-rw-rw-   0        0        0      110 2021-11-14 05:53:52.000000 tidyxbrl-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      807 2024-05-14 03:13:33.035740 tidyxbrl-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 03:13:32.773461 tidyxbrl-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 03:13:32.879159 tidyxbrl-0.1.0/src/tidyxbrl/
--rw-rw-rw-   0        0        0      165 2021-11-16 04:10:54.000000 tidyxbrl-0.1.0/src/tidyxbrl/__init__.py
--rw-rw-rw-   0        0        0     4893 2024-05-14 03:09:49.000000 tidyxbrl-0.1.0/src/tidyxbrl/edgar_cik.py
--rw-rw-rw-   0        0        0     3771 2024-05-14 03:09:49.000000 tidyxbrl-0.1.0/src/tidyxbrl/edgar_frames.py
--rw-rw-rw-   0        0        0     5315 2024-05-14 03:09:49.000000 tidyxbrl-0.1.0/src/tidyxbrl/edgar_query.py
--rw-rw-rw-   0        0        0     3618 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/src/tidyxbrl/xbrl_apikey.py
--rw-rw-rw-   0        0        0     5836 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/src/tidyxbrl/xbrl_parse.py
--rw-rw-rw-   0        0        0     3095 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/src/tidyxbrl/xbrl_query.py
-drwxrwxrwx   0        0        0        0 2024-05-14 03:13:33.016791 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/
--rw-rw-rw-   0        0        0     4997 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 03:13:33.004825 tidyxbrl-0.1.0/tests/
--rw-rw-rw-   0        0        0      118 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/tests/test_edgar_frames.py
--rw-rw-rw-   0        0        0      670 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/tests/test_edgar_query.py
--rw-rw-rw-   0        0        0      516 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/tests/test_xbrl_parse.py
--rw-rw-rw-   0        0        0     2174 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/tests/test_xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-1.0.1/LICENSE
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       25 2024-04-29 02:36:52.000000 tidyxbrl-1.0.1/MANIFEST.in
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4868 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4225 2022-12-27 22:39:13.000000 tidyxbrl-1.0.1/README.md
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      548 2024-05-14 03:38:54.000000 tidyxbrl-1.0.1/pyproject.toml
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      769 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/setup.cfg
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/src/
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/src/tidyxbrl/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-1.0.1/src/tidyxbrl/__init__.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4747 2024-05-05 22:08:02.000000 tidyxbrl-1.0.1/src/tidyxbrl/edgar_cik.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3687 2024-04-28 21:12:05.000000 tidyxbrl-1.0.1/src/tidyxbrl/edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5195 2024-05-05 22:08:04.000000 tidyxbrl-1.0.1/src/tidyxbrl/edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3523 2024-04-28 21:12:08.000000 tidyxbrl-1.0.1/src/tidyxbrl/xbrl_apikey.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     5703 2024-04-28 22:24:56.000000 tidyxbrl-1.0.1/src/tidyxbrl/xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3021 2024-04-28 21:24:46.000000 tidyxbrl-1.0.1/src/tidyxbrl/xbrl_query.py
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4868 2024-05-14 03:39:10.000000 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/PKG-INFO
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      491 2024-05-14 03:39:10.000000 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/SOURCES.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2024-05-14 03:39:10.000000 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/dependency_links.txt
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        9 2024-05-14 03:39:10.000000 tidyxbrl-1.0.1/src/tidyxbrl.egg-info/top_level.txt
+drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2024-05-14 03:39:10.172809 tidyxbrl-1.0.1/tests/
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      113 2024-04-28 22:26:49.000000 tidyxbrl-1.0.1/tests/test_edgar_frames.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      666 2024-04-29 03:42:25.000000 tidyxbrl-1.0.1/tests/test_edgar_query.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      503 2024-04-28 22:25:53.000000 tidyxbrl-1.0.1/tests/test_xbrl_parse.py
+-rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2143 2024-04-28 23:47:03.000000 tidyxbrl-1.0.1/tests/test_xbrl_query.py
```

### Comparing `tidyxbrl-0.1.0/LICENSE` & `tidyxbrl-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `tidyxbrl-0.1.0/PKG-INFO` & `tidyxbrl-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,100 +1,80 @@
-Metadata-Version: 2.1
-Name: tidyxbrl
-Version: 0.1.0
-Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
-Home-page: https://github.com/cowboycodeman/tidyxbrl/
-Author: Ryan McDonald
-Author-email: ryancmcdonald@gmail.com
-Project-URL: Bug Tracker, https://github.com/cowboycodeman/tidyxbrl/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: requests
-Requires-Dist: bs4
-Requires-Dist: tqdm
-
-<div align="center">
-  <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
-</div>
-
------------------
-
-# tidyxbrl: The tidy XBRL Interface
-
-## What is it?
-
-**tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
-
-## The XBRL Standard
-eXtensible Business Reporting Language (XBRL) is a standardized financial reporting framework to structure financial reporting in a way that enables automation and machine processing. This package aims to enable its users to realize the full capabilities of the XBRL standard through parsing files and interfacing with the applicable APIs.
-
-Applicable documentation can be found below:
-### XBRL
-  - [**XBRL API Overview**][xbrl-api-url]
-  - [**XBRL API Documentation**][xbrl-documentation-url]
-  - [**XBRL API Examples**][xbrl-example-url]
-
-### EDGAR
-  - [**SEC Edgar Information**][sec-edgar-data-url]
-  - [**SEC API Documentation**][sec-api-documentation-url]
-  - [**SEC Flat Files**][sec-flatfiles-url]
-  
-  [xbrl-api-url]: https://xbrl.us/home/use/xbrl-api/
-  [xbrl-documentation-url]: http://files.xbrl.us/documents/XBRL-API-V1.4.pdf
-  [xbrl-example-url]: https://xbrlus.github.io/xbrl-api/#/document/getDocumentInfo
-  [sec-edgar-data-url]: https://www.sec.gov/os/accessing-edgar-data
-  [sec-api-documentation-url]: https://www.sec.gov/edgar/sec-api-documentation
-  [sec-flatfiles-url]: https://www.sec.gov/Archives/edgar/full-index/
-
-## Where to get it
-The source code is currently hosted on GitHub at:
-https://github.com/cowboycodeman/tidyxbrl/
-
-The tidyxbrl package is publically available for download at:
-https://pypi.org/project/tidyxbrl/
-
-```sh
-# PyPI
-pip install tidyxbrl
-```
-## Examples
-**xbrl_parse** - Parse xbrl files or website urls
-```
-tidyxbrl.xbrl_parse("https://www.sec.gov/Archives/edgar/data/320193/000032019321000010/aapl-20201226_htm.xml")
-```
-
-**xbrl_query** - Query the XBRL API
-```
-response = tidyxbrl.xbrl_apikey(username=username, password=password, client_id=client_id, client_secret=client_secret, platform='pc', grant_type='password', refresh_token='')
-dataresponse = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
-               baseapiurl='https://api.xbrl.us/api/v1/report/search?',
-               queryparameters = {'report.entity-name': "APPLE INC.",
-                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
-                                  'report.document-type': "10-K"
-                        })
-```
-
-**edgar_query** - Query SEC data using the Central Index Key (CIK)
-```
-companycik = tidyxbrl.edgar_cik()
-desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
-tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
-tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent')
-tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
-```
-
-**edgar_frames** - Aggregates one fact for each reporting entity
-```
-tidyxbrl.edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I')
-```
-
-## Dependencies
-- [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
-- [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
-- [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
-- [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
+<div align="center">
+  <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
+</div>
+
+-----------------
+
+# tidyxbrl: The tidy XBRL Interface
+
+## What is it?
+
+**tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
+
+## The XBRL Standard
+eXtensible Business Reporting Language (XBRL) is a standardized financial reporting framework to structure financial reporting in a way that enables automation and machine processing. This package aims to enable its users to realize the full capabilities of the XBRL standard through parsing files and interfacing with the applicable APIs.
+
+Applicable documentation can be found below:
+### XBRL
+  - [**XBRL API Overview**][xbrl-api-url]
+  - [**XBRL API Documentation**][xbrl-documentation-url]
+  - [**XBRL API Examples**][xbrl-example-url]
+
+### EDGAR
+  - [**SEC Edgar Information**][sec-edgar-data-url]
+  - [**SEC API Documentation**][sec-api-documentation-url]
+  - [**SEC Flat Files**][sec-flatfiles-url]
+  
+  [xbrl-api-url]: https://xbrl.us/home/use/xbrl-api/
+  [xbrl-documentation-url]: http://files.xbrl.us/documents/XBRL-API-V1.4.pdf
+  [xbrl-example-url]: https://xbrlus.github.io/xbrl-api/#/document/getDocumentInfo
+  [sec-edgar-data-url]: https://www.sec.gov/os/accessing-edgar-data
+  [sec-api-documentation-url]: https://www.sec.gov/edgar/sec-api-documentation
+  [sec-flatfiles-url]: https://www.sec.gov/Archives/edgar/full-index/
+
+## Where to get it
+The source code is currently hosted on GitHub at:
+https://github.com/cowboycodeman/tidyxbrl/
+
+The tidyxbrl package is publically available for download at:
+https://pypi.org/project/tidyxbrl/
+
+```sh
+# PyPI
+pip install tidyxbrl
+```
+## Examples
+**xbrl_parse** - Parse xbrl files or website urls
+```
+tidyxbrl.xbrl_parse("https://www.sec.gov/Archives/edgar/data/320193/000032019321000010/aapl-20201226_htm.xml")
+```
+
+**xbrl_query** - Query the XBRL API
+```
+response = tidyxbrl.xbrl_apikey(username=username, password=password, client_id=client_id, client_secret=client_secret, platform='pc', grant_type='password', refresh_token='')
+dataresponse = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
+               baseapiurl='https://api.xbrl.us/api/v1/report/search?',
+               queryparameters = {'report.entity-name': "APPLE INC.",
+                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
+                                  'report.document-type': "10-K"
+                        })
+```
+
+**edgar_query** - Query SEC data using the Central Index Key (CIK)
+```
+companycik = tidyxbrl.edgar_cik()
+desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
+tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
+tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent')
+tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
+```
+
+**edgar_frames** - Aggregates one fact for each reporting entity
+```
+tidyxbrl.edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I')
+```
+
+## Dependencies
+- [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
+- [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
+- [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
+- [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
```

### Comparing `tidyxbrl-0.1.0/README.md` & `tidyxbrl-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,96 @@
-<div align="center">
-  <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
-</div>
-
------------------
-
-# tidyxbrl: The tidy XBRL Interface
-
-## What is it?
-
-**tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
-
-## The XBRL Standard
-eXtensible Business Reporting Language (XBRL) is a standardized financial reporting framework to structure financial reporting in a way that enables automation and machine processing. This package aims to enable its users to realize the full capabilities of the XBRL standard through parsing files and interfacing with the applicable APIs.
-
-Applicable documentation can be found below:
-### XBRL
-  - [**XBRL API Overview**][xbrl-api-url]
-  - [**XBRL API Documentation**][xbrl-documentation-url]
-  - [**XBRL API Examples**][xbrl-example-url]
-
-### EDGAR
-  - [**SEC Edgar Information**][sec-edgar-data-url]
-  - [**SEC API Documentation**][sec-api-documentation-url]
-  - [**SEC Flat Files**][sec-flatfiles-url]
-  
-  [xbrl-api-url]: https://xbrl.us/home/use/xbrl-api/
-  [xbrl-documentation-url]: http://files.xbrl.us/documents/XBRL-API-V1.4.pdf
-  [xbrl-example-url]: https://xbrlus.github.io/xbrl-api/#/document/getDocumentInfo
-  [sec-edgar-data-url]: https://www.sec.gov/os/accessing-edgar-data
-  [sec-api-documentation-url]: https://www.sec.gov/edgar/sec-api-documentation
-  [sec-flatfiles-url]: https://www.sec.gov/Archives/edgar/full-index/
-
-## Where to get it
-The source code is currently hosted on GitHub at:
-https://github.com/cowboycodeman/tidyxbrl/
-
-The tidyxbrl package is publically available for download at:
-https://pypi.org/project/tidyxbrl/
-
-```sh
-# PyPI
-pip install tidyxbrl
-```
-## Examples
-**xbrl_parse** - Parse xbrl files or website urls
-```
-tidyxbrl.xbrl_parse("https://www.sec.gov/Archives/edgar/data/320193/000032019321000010/aapl-20201226_htm.xml")
-```
-
-**xbrl_query** - Query the XBRL API
-```
-response = tidyxbrl.xbrl_apikey(username=username, password=password, client_id=client_id, client_secret=client_secret, platform='pc', grant_type='password', refresh_token='')
-dataresponse = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
-               baseapiurl='https://api.xbrl.us/api/v1/report/search?',
-               queryparameters = {'report.entity-name': "APPLE INC.",
-                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
-                                  'report.document-type': "10-K"
-                        })
-```
-
-**edgar_query** - Query SEC data using the Central Index Key (CIK)
-```
-companycik = tidyxbrl.edgar_cik()
-desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
-tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
-tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent')
-tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
-```
-
-**edgar_frames** - Aggregates one fact for each reporting entity
-```
-tidyxbrl.edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I')
-```
-
-## Dependencies
-- [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
-- [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
-- [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
-- [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
+Metadata-Version: 2.1
+Name: tidyxbrl
+Version: 1.0.1
+Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
+Home-page: https://github.com/cowboycodeman/tidyxbrl/
+Author: Ryan McDonald
+Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
+Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
+Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+  <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
+</div>
+
+-----------------
+
+# tidyxbrl: The tidy XBRL Interface
+
+## What is it?
+
+**tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
+
+## The XBRL Standard
+eXtensible Business Reporting Language (XBRL) is a standardized financial reporting framework to structure financial reporting in a way that enables automation and machine processing. This package aims to enable its users to realize the full capabilities of the XBRL standard through parsing files and interfacing with the applicable APIs.
+
+Applicable documentation can be found below:
+### XBRL
+  - [**XBRL API Overview**][xbrl-api-url]
+  - [**XBRL API Documentation**][xbrl-documentation-url]
+  - [**XBRL API Examples**][xbrl-example-url]
+
+### EDGAR
+  - [**SEC Edgar Information**][sec-edgar-data-url]
+  - [**SEC API Documentation**][sec-api-documentation-url]
+  - [**SEC Flat Files**][sec-flatfiles-url]
+  
+  [xbrl-api-url]: https://xbrl.us/home/use/xbrl-api/
+  [xbrl-documentation-url]: http://files.xbrl.us/documents/XBRL-API-V1.4.pdf
+  [xbrl-example-url]: https://xbrlus.github.io/xbrl-api/#/document/getDocumentInfo
+  [sec-edgar-data-url]: https://www.sec.gov/os/accessing-edgar-data
+  [sec-api-documentation-url]: https://www.sec.gov/edgar/sec-api-documentation
+  [sec-flatfiles-url]: https://www.sec.gov/Archives/edgar/full-index/
+
+## Where to get it
+The source code is currently hosted on GitHub at:
+https://github.com/cowboycodeman/tidyxbrl/
+
+The tidyxbrl package is publically available for download at:
+https://pypi.org/project/tidyxbrl/
+
+```sh
+# PyPI
+pip install tidyxbrl
+```
+## Examples
+**xbrl_parse** - Parse xbrl files or website urls
+```
+tidyxbrl.xbrl_parse("https://www.sec.gov/Archives/edgar/data/320193/000032019321000010/aapl-20201226_htm.xml")
+```
+
+**xbrl_query** - Query the XBRL API
+```
+response = tidyxbrl.xbrl_apikey(username=username, password=password, client_id=client_id, client_secret=client_secret, platform='pc', grant_type='password', refresh_token='')
+dataresponse = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
+               baseapiurl='https://api.xbrl.us/api/v1/report/search?',
+               queryparameters = {'report.entity-name': "APPLE INC.",
+                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
+                                  'report.document-type': "10-K"
+                        })
+```
+
+**edgar_query** - Query SEC data using the Central Index Key (CIK)
+```
+companycik = tidyxbrl.edgar_cik()
+desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
+tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
+tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent')
+tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
+```
+
+**edgar_frames** - Aggregates one fact for each reporting entity
+```
+tidyxbrl.edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I')
+```
+
+## Dependencies
+- [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
+- [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
+- [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
+- [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
```

### Comparing `tidyxbrl-0.1.0/setup.cfg` & `tidyxbrl-1.0.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2074 6964 7978 6272 6c0d 0a76 6572   = tidyxbrl..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e30 300d 0a61  sion = 0.1.00..a
-00000030: 7574 686f 7220 3d20 5279 616e 204d 6344  uthor = Ryan McD
-00000040: 6f6e 616c 640d 0a61 7574 686f 725f 656d  onald..author_em
-00000050: 6169 6c20 3d20 7279 616e 636d 6364 6f6e  ail = ryancmcdon
-00000060: 616c 6440 676d 6169 6c2e 636f 6d0d 0a64  ald@gmail.com..d
-00000070: 6573 6372 6970 7469 6f6e 203d 2041 2070  escription = A p
-00000080: 6163 6b61 6765 2074 6f20 7061 7273 6520  ackage to parse 
-00000090: 7468 6520 5842 524c 2066 696c 6520 666f  the XBRL file fo
-000000a0: 726d 6174 2026 2069 6e74 6572 6661 6365  rmat & interface
-000000b0: 2077 6974 6820 5842 524c 2041 5049 7320   with XBRL APIs 
-000000c0: 696e 2061 2074 6964 7920 666f 726d 6174  in a tidy format
-000000d0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000e0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000f0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
-00000100: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00000110: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-00000120: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
-00000130: 3a2f 2f67 6974 6875 622e 636f 6d2f 636f  ://github.com/co
-00000140: 7762 6f79 636f 6465 6d61 6e2f 7469 6479  wboycodeman/tidy
-00000150: 7862 726c 2f0d 0a70 726f 6a65 6374 5f75  xbrl/..project_u
-00000160: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-00000170: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000180: 6974 6875 622e 636f 6d2f 636f 7762 6f79  ithub.com/cowboy
-00000190: 636f 6465 6d61 6e2f 7469 6479 7862 726c  codeman/tidyxbrl
-000001a0: 2f69 7373 7565 730d 0a63 6c61 7373 6966  /issues..classif
-000001b0: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-000001c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001d0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-000001e0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000001f0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-00000200: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
-00000210: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000220: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
-00000230: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000240: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
-00000250: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000260: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-00000270: 7265 7320 3d20 3e3d 332e 360d 0a69 6e73  res = >=3.6..ins
-00000280: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000290: 0d0a 0970 616e 6461 730d 0a09 6e75 6d70  ...pandas...nump
-000002a0: 790d 0a09 7265 7175 6573 7473 0d0a 0962  y...requests...b
-000002b0: 7334 0d0a 0974 7164 6d0d 0a0d 0a5b 6f70  s4...tqdm....[op
-000002c0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000002d0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-000002e0: 630d 0a69 6e63 6c75 6465 203d 200d 0a09  c..include = ...
-000002f0: 7469 6479 7862 726c 2a0d 0a0d 0a5b 6567  tidyxbrl*....[eg
-00000300: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000310: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000320: 3d20 300d 0a0d 0a                        = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7469 6479 7862 726c 0a76 6572 7369  = tidyxbrl.versi
+00000020: 6f6e 203d 2031 2e30 2e31 0a61 7574 686f  on = 1.0.1.autho
+00000030: 7220 3d20 5279 616e 204d 6344 6f6e 616c  r = Ryan McDonal
+00000040: 640a 6175 7468 6f72 5f65 6d61 696c 203d  d.author_email =
+00000050: 2072 7961 6e63 6d63 646f 6e61 6c64 4067   ryancmcdonald@g
+00000060: 6d61 696c 2e63 6f6d 0a64 6573 6372 6970  mail.com.descrip
+00000070: 7469 6f6e 203d 2041 2070 6163 6b61 6765  tion = A package
+00000080: 2074 6f20 7061 7273 6520 7468 6520 5842   to parse the XB
+00000090: 524c 2066 696c 6520 666f 726d 6174 2026  RL file format &
+000000a0: 2069 6e74 6572 6661 6365 2077 6974 6820   interface with 
+000000b0: 5842 524c 2041 5049 7320 696e 2061 2074  XBRL APIs in a t
+000000c0: 6964 7920 666f 726d 6174 0a6c 6f6e 675f  idy format.long_
+000000d0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000e0: 6c65 3a20 5245 4144 4d45 2e6d 640a 6c6f  le: README.md.lo
+000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+00000100: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000110: 7874 2f6d 6172 6b64 6f77 6e0a 7572 6c20  xt/markdown.url 
+00000120: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000130: 2e63 6f6d 2f63 6f77 626f 7963 6f64 656d  .com/cowboycodem
+00000140: 616e 2f74 6964 7978 6272 6c2f 0a70 726f  an/tidyxbrl/.pro
+00000150: 6a65 6374 5f75 726c 7320 3d20 0a09 4275  ject_urls = ..Bu
+00000160: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
+00000170: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000180: 6f77 626f 7963 6f64 656d 616e 2f74 6964  owboycodeman/tid
+00000190: 7978 6272 6c2f 6973 7375 6573 0a63 6c61  yxbrl/issues.cla
+000001a0: 7373 6966 6965 7273 203d 200a 0950 726f  ssifiers = ..Pro
+000001b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001d0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+000001e0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000001f0: 204c 6963 656e 7365 0a09 4f70 6572 6174   License..Operat
+00000200: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000210: 2049 6e64 6570 656e 6465 6e74 0a0a 5b6f   Independent..[o
+00000220: 7074 696f 6e73 5d0a 7061 636b 6167 655f  ptions].package_
+00000230: 6469 7220 3d20 0a09 3d20 7372 630a 7061  dir = ..= src.pa
+00000240: 636b 6167 6573 203d 2066 696e 643a 0a70  ckages = find:.p
+00000250: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000260: 203e 3d33 2e36 0a69 6e73 7461 6c6c 5f72   >=3.6.install_r
+00000270: 6571 7569 7265 7320 3d20 0a09 7061 6e64  equires = ..pand
+00000280: 6173 0a09 6e75 6d70 790a 0972 6571 7565  as..numpy..reque
+00000290: 7374 730a 0962 7334 0a09 7471 646d 0a0a  sts..bs4..tqdm..
+000002a0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000002b0: 732e 6669 6e64 5d0a 7768 6572 6520 3d20  s.find].where = 
+000002c0: 7372 630a 696e 636c 7564 6520 3d20 0a09  src.include = ..
+000002d0: 7469 6479 7862 726c 2a0a 0a5b 6567 675f  tidyxbrl*..[egg_
+000002e0: 696e 666f 5d0a 7461 675f 6275 696c 6420  info].tag_build 
+000002f0: 3d20 0a74 6167 5f64 6174 6520 3d20 300a  = .tag_date = 0.
+00000300: 0a                                       .
```

### Comparing `tidyxbrl-0.1.0/src/tidyxbrl/edgar_cik.py` & `tidyxbrl-1.0.1/src/tidyxbrl/edgar_cik.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-"""
-The Central Index Key (CIK) is a unique identifier assigned by
-the U.S. Securities and Exchange Commission (SEC) to reporting companies.
-It is used to track and identify these companies in various SEC filings and databases.
-The CIK is a 10-digit number, and this function converts the CIKs of reporting companies
-into 10-digit format with leading zeros.
-"""
-
-# https://www.sec.gov/edgar/searchedgar/companysearch
-# https://www.edgarcompany.sec.gov/servlet/CompanyDBSearch?page=main
-
-import re
-import requests
-from bs4 import element
-from bs4 import BeautifulSoup
-import pandas as pd
-
-# %%
-
-
-def edgar_cik(
-    query,
-    comprehensive=False,
-    start_row=0,
-    timeout_sec=15,
-    last_company_df=pd.DataFrame(),
-    max_start_row=25000,
-):
-    """
-    The edgar_cik function is used to pull Central Index Key (CIK) for reporting companies
-
-    Args:
-        query: The company name or ticker symbol to search for
-        comprehensive: Whether to retrieve all available results or just the first 100
-        start_row: The starting index for retrieving results
-        timeout_sec: The time in seconds to wait for the server to respond
-        last_company_df: (comprehensive = True) The previous DataFrame to compare with current
-        max_start_row: The maximum starting index for retrieving results
-
-    Returns:
-        company_df: Pandas DataFrame of company names, CIK, and state
-
-    Examples:
-        -  edgar_cik(
-            query = 'App',
-            comprehensive=True,     
-            start_row=0,
-            timeout_sec=15,
-            last_company_df=pd.DataFrame(),
-            max_start_row=25000,)
-    """
-
-    # Read the company JSON from the SEC
-    headers = {
-        "User-Agent": "Mozilla",
-        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
-        "Accept-Language": "en-US,en;q=0.5",
-        "DNT": "1",  # Do Not Track Request Header
-        "Connection": "keep-alive",
-        "Upgrade-Insecure-Requests": "1",
-    }
-
-    url = "https://www.sec.gov/cgi-bin/browse-edgar"  # Replace with your desired CIK
-
-    payload = {
-        "company": query,
-        "match": "starts-with",
-        "count": 100,
-        "start": start_row,
-    }
-
-    response = requests.post(url, headers=headers, data=payload, timeout=timeout_sec)
-
-    # Parse the HTML content
-    soup = BeautifulSoup(response.content, "html.parser")
-
-    # Find the table in the HTML
-    table = soup.find("table", {"class": "tableFile2"})
-
-    if soup.find(class_='companyName') is not None:
-        company_names = str(soup.find(class_='companyName').text).split('CIK#: ', maxsplit=1)[0]
-        cik_codes = str(re
-                          .findall("\d+",
-                                   str(soup.find(class_="companyName").text)
-                                   .split("CIK#: ")[1]
-                                   .strip())[0])
-        states = (
-            soup.find(class_="identInfo")
-            .text.split("State location: ")[1]
-            .split("|")[0]
-            .strip()
-        )
-        company_df = pd.DataFrame(
-            {
-                "cik": pd.to_numeric(cik_codes),
-                "cik_str": [cik_codes],
-                "company": [company_names],
-                "state": [states],
-            }
-        )
-        return company_df
-
-    # Extract the table rows
-    if isinstance(table, element.Tag):
-        rows = table.find_all("tr")
-
-        # Extract the CIK Codes, Company Names and States
-        cik_codes = []
-        company_names = []
-        states = []
-        for row in rows[1:]:  # Ignore the header row
-            cols = row.find_all("td")
-            cik_code = cols[0].text
-            company_name = cols[1].text
-            state = cols[2].text
-            cik_codes.append(cik_code)
-            company_names.append(company_name)
-            states.append(state)
-
-        # Create a pandas DataFrame
-        company_df = pd.DataFrame(
-            {"cik": pd.to_numeric(cik_codes), "cik_str": cik_codes ,"company": company_names, "state": states}
-        )
-        print(f"Start Row: {start_row} - {company_df.iloc[0]['company']}")
-
-        if (
-            (comprehensive is True)
-            & (len(company_df) == 100)
-            & (last_company_df.equals(company_df) is False)
-            & (start_row < max_start_row)
-        ):
-            new_company_df = edgar_cik(
-                query,
-                comprehensive=comprehensive,
-                start_row=start_row + 100,
-                last_company_df=company_df,
-            )
-
-            company_df = pd.concat([company_df, new_company_df]).reset_index(drop=True)
-
-        return company_df
-
-    print(f"Final Row Reached At {start_row}")
-    return pd.DataFrame()
-
-# %%
+"""
+The Central Index Key (CIK) is a unique identifier assigned by
+the U.S. Securities and Exchange Commission (SEC) to reporting companies.
+It is used to track and identify these companies in various SEC filings and databases.
+The CIK is a 10-digit number, and this function converts the CIKs of reporting companies
+into 10-digit format with leading zeros.
+"""
+
+# https://www.sec.gov/edgar/searchedgar/companysearch
+# https://www.edgarcompany.sec.gov/servlet/CompanyDBSearch?page=main
+
+import re
+import requests
+from bs4 import element
+from bs4 import BeautifulSoup
+import pandas as pd
+
+# %%
+
+
+def edgar_cik(
+    query,
+    comprehensive=False,
+    start_row=0,
+    timeout_sec=15,
+    last_company_df=pd.DataFrame(),
+    max_start_row=25000,
+):
+    """
+    The edgar_cik function is used to pull Central Index Key (CIK) for reporting companies
+
+    Args:
+        query: The company name or ticker symbol to search for
+        comprehensive: Whether to retrieve all available results or just the first 100
+        start_row: The starting index for retrieving results
+        timeout_sec: The time in seconds to wait for the server to respond
+        last_company_df: (comprehensive = True) The previous DataFrame to compare with current
+        max_start_row: The maximum starting index for retrieving results
+
+    Returns:
+        company_df: Pandas DataFrame of company names, CIK, and state
+
+    Examples:
+        -  edgar_cik(
+            query = 'App',
+            comprehensive=True,     
+            start_row=0,
+            timeout_sec=15,
+            last_company_df=pd.DataFrame(),
+            max_start_row=25000,)
+    """
+
+    # Read the company JSON from the SEC
+    headers = {
+        "User-Agent": "Mozilla",
+        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
+        "Accept-Language": "en-US,en;q=0.5",
+        "DNT": "1",  # Do Not Track Request Header
+        "Connection": "keep-alive",
+        "Upgrade-Insecure-Requests": "1",
+    }
+
+    url = "https://www.sec.gov/cgi-bin/browse-edgar"  # Replace with your desired CIK
+
+    payload = {
+        "company": query,
+        "match": "starts-with",
+        "count": 100,
+        "start": start_row,
+    }
+
+    response = requests.post(url, headers=headers, data=payload, timeout=timeout_sec)
+
+    # Parse the HTML content
+    soup = BeautifulSoup(response.content, "html.parser")
+
+    # Find the table in the HTML
+    table = soup.find("table", {"class": "tableFile2"})
+
+    if soup.find(class_='companyName') is not None:
+        company_names = str(soup.find(class_='companyName').text).split('CIK#: ', maxsplit=1)[0]
+        cik_codes = str(re
+                          .findall("\d+",
+                                   str(soup.find(class_="companyName").text)
+                                   .split("CIK#: ")[1]
+                                   .strip())[0])
+        states = (
+            soup.find(class_="identInfo")
+            .text.split("State location: ")[1]
+            .split("|")[0]
+            .strip()
+        )
+        company_df = pd.DataFrame(
+            {
+                "cik": pd.to_numeric(cik_codes),
+                "cik_str": [cik_codes],
+                "company": [company_names],
+                "state": [states],
+            }
+        )
+        return company_df
+
+    # Extract the table rows
+    if isinstance(table, element.Tag):
+        rows = table.find_all("tr")
+
+        # Extract the CIK Codes, Company Names and States
+        cik_codes = []
+        company_names = []
+        states = []
+        for row in rows[1:]:  # Ignore the header row
+            cols = row.find_all("td")
+            cik_code = cols[0].text
+            company_name = cols[1].text
+            state = cols[2].text
+            cik_codes.append(cik_code)
+            company_names.append(company_name)
+            states.append(state)
+
+        # Create a pandas DataFrame
+        company_df = pd.DataFrame(
+            {"cik": pd.to_numeric(cik_codes), "cik_str": cik_codes ,"company": company_names, "state": states}
+        )
+        print(f"Start Row: {start_row} - {company_df.iloc[0]['company']}")
+
+        if (
+            (comprehensive is True)
+            & (len(company_df) == 100)
+            & (last_company_df.equals(company_df) is False)
+            & (start_row < max_start_row)
+        ):
+            new_company_df = edgar_cik(
+                query,
+                comprehensive=comprehensive,
+                start_row=start_row + 100,
+                last_company_df=company_df,
+            )
+
+            company_df = pd.concat([company_df, new_company_df]).reset_index(drop=True)
+
+        return company_df
+
+    print(f"Final Row Reached At {start_row}")
+    return pd.DataFrame()
+
+# %%
```

### Comparing `tidyxbrl-0.1.0/src/tidyxbrl/edgar_frames.py` & `tidyxbrl-1.0.1/src/tidyxbrl/edgar_frames.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-"""
-https://www.sec.gov/edgar/sec-api-documentation
-
-data.sec.gov/api/xbrl/frames/
-The xbrl/frames API aggregates one fact for each reporting entity that is last filed
-that most closely fits the calendrical period requested. This API supports for annual,
-quarterly and instantaneous data:
-
-https://data.sec.gov/api/xbrl/frames/us-gaap/AccountsPayableCurrent/USD/CY2019Q1I.json
-Where the units of measure specified in the XBRL contains a numerator and a denominator,
-these are separated by “-per-” such as “USD-per-shares”. Note that the default unit in
-XBRL is “pure”.
-
-The period format is CY#### for annual data (duration 365 days +/- 30 days), CY####Q# for
-quarterly data (duration 91 days +/- 30 days), and CY####Q#I for instantaneous data.
-Because company financial calendars can start and end on any month or day and even change
-in length from quarter to quarter to according to the day of the week, the frame data is
-assembled by the dates that best align with a calendar quarter or year. Data users should
-be mindful different reporting start and end dates for facts contained in a frame.
-"""
-
-import pandas
-import requests
-from tqdm import tqdm
-
-
-def edgar_frames(urldescriptor="", timeout_sec = 15):
-    """
-    The edgar_frames function aggregates one fact for each reporting entity
-    that is last filed that most closely fits the calendrical period requested.
-    This API supports for annual, quarterly and instantaneous data
-
-    Args:
-        urldescriptor: URL description of the frame query
-        (everything after https://data.sec.gov/api/xbrl/frames/***)
-        The data is structured as "finstandard/reporttype/denomination/dateholder"
-        
-            - finstandard: The financial reporting standard
-                * us-gaap
-                * ifrs-full
-                * dei
-                * srt
-            - reporttype: Type of report. See datacode in xbrl_parse (i.e. NonoperatingIncomeExpense)
-            - denomination: Report currency (i.e. USD)
-            - dateholder: Date of evaluation (i.e. CY2019Q1I)
-        timeout_sec: The time in seconds to wait for the server to respond
-
-    Outputs:
-        return companies: Return a pandas DataFrame of reporting companies and their associated CIK
-
-    Examples:
-        - edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I.json')
-    """
-
-    # Specify the query url and parameters
-    dataquery = (
-        "https://data.sec.gov/api/xbrl/frames/"
-        + str(urldescriptor).replace(".json", "")
-        + ".json"
-    )
-    soupheaders = {"User-Agent": "Mozilla"}
-    # Pull the data, check the response, and convert to a long format
-    dataresponse = requests.get(url=dataquery, headers=soupheaders, timeout=timeout_sec)
-    if dataresponse.status_code == 200:
-        try:
-            result = pandas.DataFrame(pandas.json_normalize(dataresponse.json()))
-            longdata = pandas.melt(result, id_vars=["taxonomy"])
-        except Exception as exc:
-            raise ValueError(f"Error in parsing JSON response: {str(dataresponse.json())}") from exc
-    else:
-        xbrl_queryoutput = dataresponse.status_code
-        print(dataresponse.text)
-        raise ValueError(str(xbrl_queryoutput) + ": Error in Response")
-
-    # If the data is in a list form, then convert into a nested dataframe
-    for valueholder in tqdm(range(1, len(longdata))):
-        loadvalue = longdata.iloc[valueholder].value
-        if str(type(loadvalue)) == "<class 'list'>" and len(loadvalue) > 1:
-            try:
-                longdata.at[valueholder, "value"] = pandas.json_normalize(loadvalue)
-            except ValueError:
-                pass
-
-    return longdata
+"""
+https://www.sec.gov/edgar/sec-api-documentation
+
+data.sec.gov/api/xbrl/frames/
+The xbrl/frames API aggregates one fact for each reporting entity that is last filed
+that most closely fits the calendrical period requested. This API supports for annual,
+quarterly and instantaneous data:
+
+https://data.sec.gov/api/xbrl/frames/us-gaap/AccountsPayableCurrent/USD/CY2019Q1I.json
+Where the units of measure specified in the XBRL contains a numerator and a denominator,
+these are separated by “-per-” such as “USD-per-shares”. Note that the default unit in
+XBRL is “pure”.
+
+The period format is CY#### for annual data (duration 365 days +/- 30 days), CY####Q# for
+quarterly data (duration 91 days +/- 30 days), and CY####Q#I for instantaneous data.
+Because company financial calendars can start and end on any month or day and even change
+in length from quarter to quarter to according to the day of the week, the frame data is
+assembled by the dates that best align with a calendar quarter or year. Data users should
+be mindful different reporting start and end dates for facts contained in a frame.
+"""
+
+import pandas
+import requests
+from tqdm import tqdm
+
+
+def edgar_frames(urldescriptor="", timeout_sec = 15):
+    """
+    The edgar_frames function aggregates one fact for each reporting entity
+    that is last filed that most closely fits the calendrical period requested.
+    This API supports for annual, quarterly and instantaneous data
+
+    Args:
+        urldescriptor: URL description of the frame query
+        (everything after https://data.sec.gov/api/xbrl/frames/***)
+        The data is structured as "finstandard/reporttype/denomination/dateholder"
+        
+            - finstandard: The financial reporting standard
+                * us-gaap
+                * ifrs-full
+                * dei
+                * srt
+            - reporttype: Type of report. See datacode in xbrl_parse (i.e. NonoperatingIncomeExpense)
+            - denomination: Report currency (i.e. USD)
+            - dateholder: Date of evaluation (i.e. CY2019Q1I)
+        timeout_sec: The time in seconds to wait for the server to respond
+
+    Outputs:
+        return companies: Return a pandas DataFrame of reporting companies and their associated CIK
+
+    Examples:
+        - edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I.json')
+    """
+
+    # Specify the query url and parameters
+    dataquery = (
+        "https://data.sec.gov/api/xbrl/frames/"
+        + str(urldescriptor).replace(".json", "")
+        + ".json"
+    )
+    soupheaders = {"User-Agent": "Mozilla"}
+    # Pull the data, check the response, and convert to a long format
+    dataresponse = requests.get(url=dataquery, headers=soupheaders, timeout=timeout_sec)
+    if dataresponse.status_code == 200:
+        try:
+            result = pandas.DataFrame(pandas.json_normalize(dataresponse.json()))
+            longdata = pandas.melt(result, id_vars=["taxonomy"])
+        except Exception as exc:
+            raise ValueError(f"Error in parsing JSON response: {str(dataresponse.json())}") from exc
+    else:
+        xbrl_queryoutput = dataresponse.status_code
+        print(dataresponse.text)
+        raise ValueError(str(xbrl_queryoutput) + ": Error in Response")
+
+    # If the data is in a list form, then convert into a nested dataframe
+    for valueholder in tqdm(range(1, len(longdata))):
+        loadvalue = longdata.iloc[valueholder].value
+        if str(type(loadvalue)) == "<class 'list'>" and len(loadvalue) > 1:
+            try:
+                longdata.at[valueholder, "value"] = pandas.json_normalize(loadvalue)
+            except ValueError:
+                pass
+
+    return longdata
```

### Comparing `tidyxbrl-0.1.0/src/tidyxbrl/edgar_query.py` & `tidyxbrl-1.0.1/src/tidyxbrl/edgar_query.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-"""
-https://www.sec.gov/edgar/sec-api-documentation
-
-data.sec.gov/submissions/
-Each entity’s current filing history is available at the following URL:
-https://data.sec.gov/submissions/CIK##########.json
-Where the ########## is the entity’s 10-digit Central Index Key (CIK), including leading
-zeros.
-
-This JSON data structure contains metadata such as current name, former name, and stock
-exchanges and ticker symbols of publicly-traded companies. The object’s property path
-contains at least one year’s of filing or to 1,000 (whichever is more) of the most recent
-filings in a compact columnar data array. If the entity has additional filings, files will
-contain an array of additional JSON files and the date range for the filings each one
-contains.
-
-------
-
-data.sec.gov/api/xbrl/companyconcept/
-The company-concept API returns all the XBRL disclosures from a single company (CIK) and
-concept (a taxonomy and tag) into a single JSON file, with a separate array of facts for
-each units on measure that the company has chosen to disclose (e.g. net profits reported
-in U.S. dollars and in Canadian dollars).
-
-https://data.sec.gov/api/xbrl/companyconcept/CIK##########/us-gaap/AccountsPayableCurrent.json
-
------
-
-data.sec.gov/api/xbrl/companyfacts/
-This API returns all the company concepts data for a company into a single API call:
-
-https://data.sec.gov/api/xbrl/companyfacts/CIK##########.json
-"""
-
-import pandas
-import requests
-from tqdm import tqdm
-import numpy
-
-
-def edgar_query(companycik, query_type, queryextension="", parse_pandas = True, timeout_sec = 15):
-    """
-    Query SEC data using the Central Index Key (CIK).
-
-    The edgar_query function is used to query SEC data using the Central Index Key (CIK)
-    determined in the edgar_cik function.
-
-    Args:
-        companycik (str): Unique company CIK value pulled in edgar_cik. Note that the CIK is
-        converted to 10 digits with leading 0s.
-        query_type (str): The type of API query. Can be 'submissions', 'companyconcept', or
-        'companyfacts'.
-        queryextension (str, optional): Extension required for the "companyconcept"
-        query_type to specify the report type. Defaults to "".
-        parse_pandas (bool, optional): If True, the data is converted to a pandas DataFrame.
-        timeout_sec: The time in seconds to wait for the server to respond
-
-    Returns:
-        pandas.DataFrame: Tidy dataframe housing the report data.
-
-    Raises:
-        ValueError: If query_type is not one of 'submissions', 'companyconcept', or
-        'companyfacts'.
-
-    Examples:
-        edgar_query('0000789019', query_type = 'submissions')
-        edgar_query('0000789019', query_type = 'companyconcept',
-        queryextension = '/us-gaap/AccountsPayableCurrent.json')
-        edgar_query('0000789019', query_type = 'companyfacts')
-    """
-
-    # Pull one of the urls associated with the query types
-    querydict = {
-        "submissions": "https://data.sec.gov/submissions/CIK",
-        "companyconcept": "https://data.sec.gov/api/xbrl/companyconcept/CIK",
-        "companyfacts": "https://data.sec.gov/api/xbrl/companyfacts/CIK",
-    }
-    # Raise error if the data does not exist
-    if query_type not in querydict:
-        raise ValueError("parse_type must be in: " + str(querydict))
-    # Specify the query url and parameters
-    urlquery = querydict[query_type]
-    dataquery = (
-        urlquery + str(companycik) + str(queryextension).replace(".json", "") + ".json"
-    )
-    headers = {
-        "User-Agent": "Mozilla",
-        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
-        "Accept-Language": "en-US,en;q=0.5",
-        "DNT": "1",  # Do Not Track Request Header
-        "Connection": "keep-alive",
-        "Upgrade-Insecure-Requests": "1",
-    }
-    # Pull the data, check the response, and convert to a long format
-    dataresponse = requests.get(url=dataquery, headers=headers, timeout=timeout_sec)
-    if dataresponse.status_code == 200:
-        try:
-            result = pandas.DataFrame(pandas.json_normalize(dataresponse.json()))
-            longdata = pandas.melt(result, id_vars=["cik"])
-        except Exception as exc:
-            raise ValueError(str(dataresponse.json())) from exc
-    else:
-        xbrl_queryoutput = dataresponse.status_code
-        # print(dataresponse.text)
-        raise ValueError(str(xbrl_queryoutput) + ": " + str(dataresponse.content))
-
-    # If the data is in a list form, then convert it into a nested dataframe
-    if parse_pandas:
-        for valueholder in tqdm(range(1, len(longdata.value))):
-            loadvalue = longdata.iloc[valueholder].value
-            if isinstance(loadvalue, list):
-                try:
-                    loadvalue_df = pandas.DataFrame(loadvalue)
-                    if len(loadvalue_df) > 1:
-                        loadvalue_df = loadvalue_df.transpose().explode("value")
-                    longdata.at[valueholder, "value"] = loadvalue_df
-                except Exception:
-                    longdata.at[valueholder, "value"] = pandas.DataFrame(loadvalue)
-    longdata = longdata.assign(cik = lambda x: pandas.to_numeric(x.cik, errors='coerce'))
-    return longdata
+"""
+https://www.sec.gov/edgar/sec-api-documentation
+
+data.sec.gov/submissions/
+Each entity’s current filing history is available at the following URL:
+https://data.sec.gov/submissions/CIK##########.json
+Where the ########## is the entity’s 10-digit Central Index Key (CIK), including leading
+zeros.
+
+This JSON data structure contains metadata such as current name, former name, and stock
+exchanges and ticker symbols of publicly-traded companies. The object’s property path
+contains at least one year’s of filing or to 1,000 (whichever is more) of the most recent
+filings in a compact columnar data array. If the entity has additional filings, files will
+contain an array of additional JSON files and the date range for the filings each one
+contains.
+
+------
+
+data.sec.gov/api/xbrl/companyconcept/
+The company-concept API returns all the XBRL disclosures from a single company (CIK) and
+concept (a taxonomy and tag) into a single JSON file, with a separate array of facts for
+each units on measure that the company has chosen to disclose (e.g. net profits reported
+in U.S. dollars and in Canadian dollars).
+
+https://data.sec.gov/api/xbrl/companyconcept/CIK##########/us-gaap/AccountsPayableCurrent.json
+
+-----
+
+data.sec.gov/api/xbrl/companyfacts/
+This API returns all the company concepts data for a company into a single API call:
+
+https://data.sec.gov/api/xbrl/companyfacts/CIK##########.json
+"""
+
+import pandas
+import requests
+from tqdm import tqdm
+import numpy
+
+
+def edgar_query(companycik, query_type, queryextension="", parse_pandas = True, timeout_sec = 15):
+    """
+    Query SEC data using the Central Index Key (CIK).
+
+    The edgar_query function is used to query SEC data using the Central Index Key (CIK)
+    determined in the edgar_cik function.
+
+    Args:
+        companycik (str): Unique company CIK value pulled in edgar_cik. Note that the CIK is
+        converted to 10 digits with leading 0s.
+        query_type (str): The type of API query. Can be 'submissions', 'companyconcept', or
+        'companyfacts'.
+        queryextension (str, optional): Extension required for the "companyconcept"
+        query_type to specify the report type. Defaults to "".
+        parse_pandas (bool, optional): If True, the data is converted to a pandas DataFrame.
+        timeout_sec: The time in seconds to wait for the server to respond
+
+    Returns:
+        pandas.DataFrame: Tidy dataframe housing the report data.
+
+    Raises:
+        ValueError: If query_type is not one of 'submissions', 'companyconcept', or
+        'companyfacts'.
+
+    Examples:
+        edgar_query('0000789019', query_type = 'submissions')
+        edgar_query('0000789019', query_type = 'companyconcept',
+        queryextension = '/us-gaap/AccountsPayableCurrent.json')
+        edgar_query('0000789019', query_type = 'companyfacts')
+    """
+
+    # Pull one of the urls associated with the query types
+    querydict = {
+        "submissions": "https://data.sec.gov/submissions/CIK",
+        "companyconcept": "https://data.sec.gov/api/xbrl/companyconcept/CIK",
+        "companyfacts": "https://data.sec.gov/api/xbrl/companyfacts/CIK",
+    }
+    # Raise error if the data does not exist
+    if query_type not in querydict:
+        raise ValueError("parse_type must be in: " + str(querydict))
+    # Specify the query url and parameters
+    urlquery = querydict[query_type]
+    dataquery = (
+        urlquery + str(companycik) + str(queryextension).replace(".json", "") + ".json"
+    )
+    headers = {
+        "User-Agent": "Mozilla",
+        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
+        "Accept-Language": "en-US,en;q=0.5",
+        "DNT": "1",  # Do Not Track Request Header
+        "Connection": "keep-alive",
+        "Upgrade-Insecure-Requests": "1",
+    }
+    # Pull the data, check the response, and convert to a long format
+    dataresponse = requests.get(url=dataquery, headers=headers, timeout=timeout_sec)
+    if dataresponse.status_code == 200:
+        try:
+            result = pandas.DataFrame(pandas.json_normalize(dataresponse.json()))
+            longdata = pandas.melt(result, id_vars=["cik"])
+        except Exception as exc:
+            raise ValueError(str(dataresponse.json())) from exc
+    else:
+        xbrl_queryoutput = dataresponse.status_code
+        # print(dataresponse.text)
+        raise ValueError(str(xbrl_queryoutput) + ": " + str(dataresponse.content))
+
+    # If the data is in a list form, then convert it into a nested dataframe
+    if parse_pandas:
+        for valueholder in tqdm(range(1, len(longdata.value))):
+            loadvalue = longdata.iloc[valueholder].value
+            if isinstance(loadvalue, list):
+                try:
+                    loadvalue_df = pandas.DataFrame(loadvalue)
+                    if len(loadvalue_df) > 1:
+                        loadvalue_df = loadvalue_df.transpose().explode("value")
+                    longdata.at[valueholder, "value"] = loadvalue_df
+                except Exception:
+                    longdata.at[valueholder, "value"] = pandas.DataFrame(loadvalue)
+    longdata = longdata.assign(cik = lambda x: pandas.to_numeric(x.cik, errors='coerce'))
+    return longdata
```

### Comparing `tidyxbrl-0.1.0/src/tidyxbrl/xbrl_apikey.py` & `tidyxbrl-1.0.1/src/tidyxbrl/xbrl_apikey.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-"""
-https://xbrl.us/home/use/xbrl-api/access-token/
-
-API key generation to pull data from the XBRL US API.
-
-"""
-
-import pandas
-import requests
-
-
-def xbrl_apikey(
-    username,
-    password,
-    client_id,
-    client_secret,
-    platform="pc",
-    grant_type="password",
-    refresh_token="",
-    timeout_sec = 15
-):
-    """
-    The xbrl_apikey function generates or refreshes a temporary token for the xbrl_apiquery
-    function.
-
-    Args:
-        username (str): Email address corresponding to the xbrl.us api website.
-        password (str): Password corresponding to the xbrl.us api website.
-        client_id (str): Active public Client ID.
-        client_secret (str): Secret ID corresponding to the client_id.
-        platform (str): Keyword to distinguish if the user is authenticating from different
-        applications.
-        grant_type (str): Either 'password' to generate a new key, or 'refresh_token' to
-        refresh an existing key.
-        refresh_token (str, optional): Optional refresh token provided in a previous
-        xbrl_apikey request.
-        timeout_sec: The time in seconds to wait for the server to respond
-
-    Returns:
-        pandas.DataFrame: DataFrame output of the XBRL api key.
-            - platform: Keyword to distinguish if the user is authenticating from different
-            applications.
-            - access_token: Access token to be passed to the xbrl_apiquery function.
-            - refresh_token: Refresh token to refresh the 'access_token'.
-            - expires_in: Seconds until expiry.
-            - refresh_token_expires_in token_type: Seconds until refresh token expiry.
-            - token_type: type of token. Always "bearer".
-
-    Examples:
-        xbrl_apikeyoutput = xbrl_apikey(username='username', password='password',
-        client_id='client_id', client_secret='client_secret', platform='pc',
-        grant_type='password', refresh_token='optional_refresh_token')
-    """
-
-    # Submit the request based on the grant_type
-    # If password, generate a new tolken
-    if grant_type == "password":
-        xbrl_apikeyoutput = requests.post(
-            url="https://api.xbrl.us/oauth2/token",
-            data={
-                "grant_type": grant_type,
-                "client_id": client_id,
-                "client_secret": client_secret,
-                "username": username,
-                "password": password,
-                "platform": platform,
-            },
-            timeout=timeout_sec
-        )
-    # If refresh_token, refresh an existing token
-    elif grant_type == "refresh_token":
-        xbrl_apikeyoutput = requests.post(
-            url="https://api.xbrl.us/oauth2/token",
-            data={
-                "grant_type": grant_type,
-                "client_id": client_id,
-                "client_secret": client_secret,
-                "refresh_token": refresh_token,
-                "platform": platform,
-            },
-            timeout=timeout_sec
-        )
-    else:
-        raise ValueError("grant_type must be either 'password' or 'refresh_token'")
-    # Check the Response Code. 200 is a success
-    if xbrl_apikeyoutput.status_code == 200:
-        try:
-            result = pandas.DataFrame(pandas.json_normalize(xbrl_apikeyoutput.json()))
-        except Exception as exc:
-            raise ValueError(str(xbrl_apikeyoutput.json())) from exc
-    else:
-        result = xbrl_apikeyoutput.status_code
-        print(xbrl_apikeyoutput.text)
-        raise ValueError(str(result) + ": Error in Response")
-    return result
+"""
+https://xbrl.us/home/use/xbrl-api/access-token/
+
+API key generation to pull data from the XBRL US API.
+
+"""
+
+import pandas
+import requests
+
+
+def xbrl_apikey(
+    username,
+    password,
+    client_id,
+    client_secret,
+    platform="pc",
+    grant_type="password",
+    refresh_token="",
+    timeout_sec = 15
+):
+    """
+    The xbrl_apikey function generates or refreshes a temporary token for the xbrl_apiquery
+    function.
+
+    Args:
+        username (str): Email address corresponding to the xbrl.us api website.
+        password (str): Password corresponding to the xbrl.us api website.
+        client_id (str): Active public Client ID.
+        client_secret (str): Secret ID corresponding to the client_id.
+        platform (str): Keyword to distinguish if the user is authenticating from different
+        applications.
+        grant_type (str): Either 'password' to generate a new key, or 'refresh_token' to
+        refresh an existing key.
+        refresh_token (str, optional): Optional refresh token provided in a previous
+        xbrl_apikey request.
+        timeout_sec: The time in seconds to wait for the server to respond
+
+    Returns:
+        pandas.DataFrame: DataFrame output of the XBRL api key.
+            - platform: Keyword to distinguish if the user is authenticating from different
+            applications.
+            - access_token: Access token to be passed to the xbrl_apiquery function.
+            - refresh_token: Refresh token to refresh the 'access_token'.
+            - expires_in: Seconds until expiry.
+            - refresh_token_expires_in token_type: Seconds until refresh token expiry.
+            - token_type: type of token. Always "bearer".
+
+    Examples:
+        xbrl_apikeyoutput = xbrl_apikey(username='username', password='password',
+        client_id='client_id', client_secret='client_secret', platform='pc',
+        grant_type='password', refresh_token='optional_refresh_token')
+    """
+
+    # Submit the request based on the grant_type
+    # If password, generate a new tolken
+    if grant_type == "password":
+        xbrl_apikeyoutput = requests.post(
+            url="https://api.xbrl.us/oauth2/token",
+            data={
+                "grant_type": grant_type,
+                "client_id": client_id,
+                "client_secret": client_secret,
+                "username": username,
+                "password": password,
+                "platform": platform,
+            },
+            timeout=timeout_sec
+        )
+    # If refresh_token, refresh an existing token
+    elif grant_type == "refresh_token":
+        xbrl_apikeyoutput = requests.post(
+            url="https://api.xbrl.us/oauth2/token",
+            data={
+                "grant_type": grant_type,
+                "client_id": client_id,
+                "client_secret": client_secret,
+                "refresh_token": refresh_token,
+                "platform": platform,
+            },
+            timeout=timeout_sec
+        )
+    else:
+        raise ValueError("grant_type must be either 'password' or 'refresh_token'")
+    # Check the Response Code. 200 is a success
+    if xbrl_apikeyoutput.status_code == 200:
+        try:
+            result = pandas.DataFrame(pandas.json_normalize(xbrl_apikeyoutput.json()))
+        except Exception as exc:
+            raise ValueError(str(xbrl_apikeyoutput.json())) from exc
+    else:
+        result = xbrl_apikeyoutput.status_code
+        print(xbrl_apikeyoutput.text)
+        raise ValueError(str(result) + ": Error in Response")
+    return result
```

### Comparing `tidyxbrl-0.1.0/src/tidyxbrl/xbrl_query.py` & `tidyxbrl-1.0.1/src/tidyxbrl/xbrl_query.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-"""
-
-https://xbrlus.github.io/xbrl-api/
-
-Query functions for the XBRL API
-"""
-
-import pandas
-import requests
-
-
-def xbrl_query(
-    access_token,
-    queryparameters,
-    baseapiurl="https://api.xbrl.us/api/v1/report/search?",
-    timeout_sec = 15
-):
-    """
-    https://xbrl.us/home/use/xbrl-api/
-    http://files.xbrl.us/documents/XBRL-API-V1.4.pdf
-
-    The xbrl_query function is used to query the xbrl api using the token generated in the
-    xbrl_apikey function.
-
-    Args:
-        access_token: Access token string generated in the xbrl_apikey function. Found in the
-        access_token column of the response dataframe.
-        baseapiurl: API request URL corresponding to the type of request prior to passing any
-        parameters. This is everything up-to and including the "?" in the API request
-            - 'https://api.xbrl.us/api/v1/report/search?'
-            - 'https://api.xbrl.us/api/v1/fact/search?'
-        queryparameters: Dictionary structure to specify each aspect of the api request (See the
-        Examples section below)
-
-    Outputs:
-        xbrl_queryoutput: Pandas Dataframe object corresponding to the fields specified in the
-        request
-
-    Examples:
-        - xbrl_query(access_token=xbrl_apikeyoutput.access_token.values[0],
-                    baseapiurl='https://api.xbrl.us/api/v1/report/search?',
-                    queryparameters = {'report.entity-name': "APPLE INC.",
-                                        'fields': "report.id,report.entity-name,report.filing-date,
-                                        report.base-taxonomy,report.document-type,report.accession,
-                                        entity.ticker,report.sic-code,entity.cik,report.entry-type,
-                                        report.period-end,report.sec-url,report.checks-run,
-    """
-
-    # Modify the queryparameter keys to create a web request string in dataquery
-    # Add the "=" sign between keys and values
-    for keyholder in list(queryparameters.keys()):
-        queryparameters[keyholder + "="] = queryparameters[keyholder]
-        del queryparameters[keyholder]
-    # Add the "&" sign between keys
-    queryurl = "".join(
-        [f"{key}{value}&" for key, value in queryparameters.items()]
-    )[:-1]
-    # Add the baseurl and modified request values
-    dataquery = str(baseapiurl + queryurl)
-    # Generate the authentication bearer tolken
-    headers = {"Authorization": "Bearer " + access_token}
-    # Generate the response
-    dataresponse = requests.get(url=dataquery, headers=headers, timeout=timeout_sec)
-    # Check the Response Code
-    if dataresponse.status_code == 200:
-        try:
-            xbrl_queryoutput = pandas.DataFrame.from_dict(dataresponse.json()["data"])
-        except Exception as exc:
-            raise ValueError(str(dataresponse.json())) from exc
-    else:
-        xbrl_queryoutput = dataresponse.status_code
-        print(dataresponse.text)
-        raise ValueError(str(xbrl_queryoutput) + ": Error in Response")
-    return xbrl_queryoutput
+"""
+
+https://xbrlus.github.io/xbrl-api/
+
+Query functions for the XBRL API
+"""
+
+import pandas
+import requests
+
+
+def xbrl_query(
+    access_token,
+    queryparameters,
+    baseapiurl="https://api.xbrl.us/api/v1/report/search?",
+    timeout_sec = 15
+):
+    """
+    https://xbrl.us/home/use/xbrl-api/
+    http://files.xbrl.us/documents/XBRL-API-V1.4.pdf
+
+    The xbrl_query function is used to query the xbrl api using the token generated in the
+    xbrl_apikey function.
+
+    Args:
+        access_token: Access token string generated in the xbrl_apikey function. Found in the
+        access_token column of the response dataframe.
+        baseapiurl: API request URL corresponding to the type of request prior to passing any
+        parameters. This is everything up-to and including the "?" in the API request
+            - 'https://api.xbrl.us/api/v1/report/search?'
+            - 'https://api.xbrl.us/api/v1/fact/search?'
+        queryparameters: Dictionary structure to specify each aspect of the api request (See the
+        Examples section below)
+
+    Outputs:
+        xbrl_queryoutput: Pandas Dataframe object corresponding to the fields specified in the
+        request
+
+    Examples:
+        - xbrl_query(access_token=xbrl_apikeyoutput.access_token.values[0],
+                    baseapiurl='https://api.xbrl.us/api/v1/report/search?',
+                    queryparameters = {'report.entity-name': "APPLE INC.",
+                                        'fields': "report.id,report.entity-name,report.filing-date,
+                                        report.base-taxonomy,report.document-type,report.accession,
+                                        entity.ticker,report.sic-code,entity.cik,report.entry-type,
+                                        report.period-end,report.sec-url,report.checks-run,
+    """
+
+    # Modify the queryparameter keys to create a web request string in dataquery
+    # Add the "=" sign between keys and values
+    for keyholder in list(queryparameters.keys()):
+        queryparameters[keyholder + "="] = queryparameters[keyholder]
+        del queryparameters[keyholder]
+    # Add the "&" sign between keys
+    queryurl = "".join(
+        [f"{key}{value}&" for key, value in queryparameters.items()]
+    )[:-1]
+    # Add the baseurl and modified request values
+    dataquery = str(baseapiurl + queryurl)
+    # Generate the authentication bearer tolken
+    headers = {"Authorization": "Bearer " + access_token}
+    # Generate the response
+    dataresponse = requests.get(url=dataquery, headers=headers, timeout=timeout_sec)
+    # Check the Response Code
+    if dataresponse.status_code == 200:
+        try:
+            xbrl_queryoutput = pandas.DataFrame.from_dict(dataresponse.json()["data"])
+        except Exception as exc:
+            raise ValueError(str(dataresponse.json())) from exc
+    else:
+        xbrl_queryoutput = dataresponse.status_code
+        print(dataresponse.text)
+        raise ValueError(str(xbrl_queryoutput) + ": Error in Response")
+    return xbrl_queryoutput
```

### Comparing `tidyxbrl-0.1.0/src/tidyxbrl.egg-info/PKG-INFO` & `tidyxbrl-1.0.1/src/tidyxbrl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,96 @@
-Metadata-Version: 2.1
-Name: tidyxbrl
-Version: 0.1.0
-Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
-Home-page: https://github.com/cowboycodeman/tidyxbrl/
-Author: Ryan McDonald
-Author-email: ryancmcdonald@gmail.com
-Project-URL: Bug Tracker, https://github.com/cowboycodeman/tidyxbrl/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: requests
-Requires-Dist: bs4
-Requires-Dist: tqdm
-
-<div align="center">
-  <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
-</div>
-
------------------
-
-# tidyxbrl: The tidy XBRL Interface
-
-## What is it?
-
-**tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
-
-## The XBRL Standard
-eXtensible Business Reporting Language (XBRL) is a standardized financial reporting framework to structure financial reporting in a way that enables automation and machine processing. This package aims to enable its users to realize the full capabilities of the XBRL standard through parsing files and interfacing with the applicable APIs.
-
-Applicable documentation can be found below:
-### XBRL
-  - [**XBRL API Overview**][xbrl-api-url]
-  - [**XBRL API Documentation**][xbrl-documentation-url]
-  - [**XBRL API Examples**][xbrl-example-url]
-
-### EDGAR
-  - [**SEC Edgar Information**][sec-edgar-data-url]
-  - [**SEC API Documentation**][sec-api-documentation-url]
-  - [**SEC Flat Files**][sec-flatfiles-url]
-  
-  [xbrl-api-url]: https://xbrl.us/home/use/xbrl-api/
-  [xbrl-documentation-url]: http://files.xbrl.us/documents/XBRL-API-V1.4.pdf
-  [xbrl-example-url]: https://xbrlus.github.io/xbrl-api/#/document/getDocumentInfo
-  [sec-edgar-data-url]: https://www.sec.gov/os/accessing-edgar-data
-  [sec-api-documentation-url]: https://www.sec.gov/edgar/sec-api-documentation
-  [sec-flatfiles-url]: https://www.sec.gov/Archives/edgar/full-index/
-
-## Where to get it
-The source code is currently hosted on GitHub at:
-https://github.com/cowboycodeman/tidyxbrl/
-
-The tidyxbrl package is publically available for download at:
-https://pypi.org/project/tidyxbrl/
-
-```sh
-# PyPI
-pip install tidyxbrl
-```
-## Examples
-**xbrl_parse** - Parse xbrl files or website urls
-```
-tidyxbrl.xbrl_parse("https://www.sec.gov/Archives/edgar/data/320193/000032019321000010/aapl-20201226_htm.xml")
-```
-
-**xbrl_query** - Query the XBRL API
-```
-response = tidyxbrl.xbrl_apikey(username=username, password=password, client_id=client_id, client_secret=client_secret, platform='pc', grant_type='password', refresh_token='')
-dataresponse = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
-               baseapiurl='https://api.xbrl.us/api/v1/report/search?',
-               queryparameters = {'report.entity-name': "APPLE INC.",
-                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
-                                  'report.document-type': "10-K"
-                        })
-```
-
-**edgar_query** - Query SEC data using the Central Index Key (CIK)
-```
-companycik = tidyxbrl.edgar_cik()
-desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
-tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
-tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent')
-tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
-```
-
-**edgar_frames** - Aggregates one fact for each reporting entity
-```
-tidyxbrl.edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I')
-```
-
-## Dependencies
-- [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
-- [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
-- [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
-- [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
+Metadata-Version: 2.1
+Name: tidyxbrl
+Version: 1.0.1
+Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
+Home-page: https://github.com/cowboycodeman/tidyxbrl/
+Author: Ryan McDonald
+Author-email: Ryan McDonald <ryancmcdonald@gmail.com>
+Project-URL: Homepage, https://github.com/cowboycodeman/tidyxbrl/
+Project-URL: Issues, https://github.com/cowboycodeman/tidyxbrl/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+  <img src="https://www.xbrl.org/wp-content/themes/xbrl/images/logoHeader.png"><br>
+</div>
+
+-----------------
+
+# tidyxbrl: The tidy XBRL Interface
+
+## What is it?
+
+**tidyxbrl** is a Python package that parses XBRL data files and returns dynamic structures that succinctly store the underlying data. This package additionally can interface with the XBRL API and SEC EDGAR interfaces, with further expansion to other XBRL data providers planned for the near future. This package aims to the be the simplest and most effective method to parse XBRL data in Python.
+
+## The XBRL Standard
+eXtensible Business Reporting Language (XBRL) is a standardized financial reporting framework to structure financial reporting in a way that enables automation and machine processing. This package aims to enable its users to realize the full capabilities of the XBRL standard through parsing files and interfacing with the applicable APIs.
+
+Applicable documentation can be found below:
+### XBRL
+  - [**XBRL API Overview**][xbrl-api-url]
+  - [**XBRL API Documentation**][xbrl-documentation-url]
+  - [**XBRL API Examples**][xbrl-example-url]
+
+### EDGAR
+  - [**SEC Edgar Information**][sec-edgar-data-url]
+  - [**SEC API Documentation**][sec-api-documentation-url]
+  - [**SEC Flat Files**][sec-flatfiles-url]
+  
+  [xbrl-api-url]: https://xbrl.us/home/use/xbrl-api/
+  [xbrl-documentation-url]: http://files.xbrl.us/documents/XBRL-API-V1.4.pdf
+  [xbrl-example-url]: https://xbrlus.github.io/xbrl-api/#/document/getDocumentInfo
+  [sec-edgar-data-url]: https://www.sec.gov/os/accessing-edgar-data
+  [sec-api-documentation-url]: https://www.sec.gov/edgar/sec-api-documentation
+  [sec-flatfiles-url]: https://www.sec.gov/Archives/edgar/full-index/
+
+## Where to get it
+The source code is currently hosted on GitHub at:
+https://github.com/cowboycodeman/tidyxbrl/
+
+The tidyxbrl package is publically available for download at:
+https://pypi.org/project/tidyxbrl/
+
+```sh
+# PyPI
+pip install tidyxbrl
+```
+## Examples
+**xbrl_parse** - Parse xbrl files or website urls
+```
+tidyxbrl.xbrl_parse("https://www.sec.gov/Archives/edgar/data/320193/000032019321000010/aapl-20201226_htm.xml")
+```
+
+**xbrl_query** - Query the XBRL API
+```
+response = tidyxbrl.xbrl_apikey(username=username, password=password, client_id=client_id, client_secret=client_secret, platform='pc', grant_type='password', refresh_token='')
+dataresponse = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
+               baseapiurl='https://api.xbrl.us/api/v1/report/search?',
+               queryparameters = {'report.entity-name': "APPLE INC.",
+                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
+                                  'report.document-type': "10-K"
+                        })
+```
+
+**edgar_query** - Query SEC data using the Central Index Key (CIK)
+```
+companycik = tidyxbrl.edgar_cik()
+desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
+tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
+tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent')
+tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
+```
+
+**edgar_frames** - Aggregates one fact for each reporting entity
+```
+tidyxbrl.edgar_frames(urldescriptor = 'us-gaap/NonoperatingIncomeExpense/USD/CY2019Q1I')
+```
+
+## Dependencies
+- [pandas - A fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.](https://pandas.pydata.org/)
+- [NumPy - The fundamental package for scientific computing with Python](https://www.numpy.org)
+- [requests - An elegant and simple HTTP library for Python, built for human beings.](https://docs.python-requests.org/en/master/)
+- [bs4 - For pulling data out of HTML and XML files](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
```

### Comparing `tidyxbrl-0.1.0/tests/test_edgar_query.py` & `tidyxbrl-1.0.1/tests/test_edgar_query.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# %%
-import tidyxbrl
-
-tidyxbrl.edgar_query('0000789019', query_type = 'submissions')
-tidyxbrl.edgar_query('0000789019', query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent.json')
-tidyxbrl.edgar_query('0000789019', query_type = 'companyfacts')
-
-companycik = tidyxbrl.edgar_cik()
-desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
-tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
-tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent.json')
-tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
+
+# %%
+import tidyxbrl
+
+tidyxbrl.edgar_query('0000789019', query_type = 'submissions')
+tidyxbrl.edgar_query('0000789019', query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent.json')
+tidyxbrl.edgar_query('0000789019', query_type = 'companyfacts')
+
+companycik = tidyxbrl.edgar_cik()
+desiredcorp = str(companycik[companycik.title.str.contains("ZILLOW GROUP, INC.")]['cik_str'].unique()[0])
+tidyxbrl.edgar_query(desiredcorp, query_type = 'submissions')
+tidyxbrl.edgar_query(desiredcorp, query_type = 'companyconcept', queryextension = '/us-gaap/AccountsPayableCurrent.json')
+tidyxbrl.edgar_query(desiredcorp, query_type = 'companyfacts')
+# %%
```

