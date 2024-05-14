# Comparing `tmp/tidyxbrl-0.0.50.tar.gz` & `tmp/tidyxbrl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyxbrl-0.0.50.tar", last modified: Fri Feb 24 05:07:06 2023, max compression
+gzip compressed data, was "tidyxbrl-0.1.0.tar", last modified: Tue May 14 03:13:33 2024, max compression
```

## Comparing `tidyxbrl-0.0.50.tar` & `tidyxbrl-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2023-02-24 05:07:06.117357 tidyxbrl-0.0.50/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     1073 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/LICENSE
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4792 2023-02-24 05:07:06.117357 tidyxbrl-0.0.50/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4225 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/README.md
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      104 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/pyproject.toml
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      770 2023-02-24 05:07:06.117357 tidyxbrl-0.0.50/setup.cfg
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2023-02-24 05:07:06.117357 tidyxbrl-0.0.50/src/
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2023-02-24 05:07:06.117357 tidyxbrl-0.0.50/src/tidyxbrl/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      159 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/src/tidyxbrl/__init__.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      986 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/src/tidyxbrl/edgar_cik.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2433 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/src/tidyxbrl/edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3092 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/src/tidyxbrl/edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4077 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/src/tidyxbrl/xbrl_apikey.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     8687 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/src/tidyxbrl/xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     3767 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/src/tidyxbrl/xbrl_query.py
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2023-02-24 05:07:06.117357 tidyxbrl-0.0.50/src/tidyxbrl.egg-info/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     4792 2023-02-24 05:07:06.000000 tidyxbrl-0.0.50/src/tidyxbrl.egg-info/PKG-INFO
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      514 2023-02-24 05:07:06.000000 tidyxbrl-0.0.50/src/tidyxbrl.egg-info/SOURCES.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        1 2023-02-24 05:07:06.000000 tidyxbrl-0.0.50/src/tidyxbrl.egg-info/dependency_links.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)       31 2023-02-24 05:07:06.000000 tidyxbrl-0.0.50/src/tidyxbrl.egg-info/requires.txt
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)        9 2023-02-24 05:07:06.000000 tidyxbrl-0.0.50/src/tidyxbrl.egg-info/top_level.txt
-drwxr-xr-x   0 rmdonald  (1000) rmdonald  (1001)        0 2023-02-24 05:07:06.117357 tidyxbrl-0.0.50/tests/
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      105 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/tests/test_edgar_frames.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      654 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/tests/test_edgar_query.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)      491 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/tests/test_xbrl_parse.py
--rw-r--r--   0 rmdonald  (1000) rmdonald  (1001)     2138 2022-12-27 22:39:13.000000 tidyxbrl-0.0.50/tests/test_xbrl_query.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:13:33.022775 tidyxbrl-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2021-11-14 19:09:57.000000 tidyxbrl-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4997 2024-05-14 03:13:33.020781 tidyxbrl-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4305 2021-11-19 03:57:45.000000 tidyxbrl-0.1.0/README.md
+-rw-rw-rw-   0        0        0      110 2021-11-14 05:53:52.000000 tidyxbrl-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      807 2024-05-14 03:13:33.035740 tidyxbrl-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 03:13:32.773461 tidyxbrl-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 03:13:32.879159 tidyxbrl-0.1.0/src/tidyxbrl/
+-rw-rw-rw-   0        0        0      165 2021-11-16 04:10:54.000000 tidyxbrl-0.1.0/src/tidyxbrl/__init__.py
+-rw-rw-rw-   0        0        0     4893 2024-05-14 03:09:49.000000 tidyxbrl-0.1.0/src/tidyxbrl/edgar_cik.py
+-rw-rw-rw-   0        0        0     3771 2024-05-14 03:09:49.000000 tidyxbrl-0.1.0/src/tidyxbrl/edgar_frames.py
+-rw-rw-rw-   0        0        0     5315 2024-05-14 03:09:49.000000 tidyxbrl-0.1.0/src/tidyxbrl/edgar_query.py
+-rw-rw-rw-   0        0        0     3618 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/src/tidyxbrl/xbrl_apikey.py
+-rw-rw-rw-   0        0        0     5836 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/src/tidyxbrl/xbrl_parse.py
+-rw-rw-rw-   0        0        0     3095 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/src/tidyxbrl/xbrl_query.py
+drwxrwxrwx   0        0        0        0 2024-05-14 03:13:33.016791 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/
+-rw-rw-rw-   0        0        0     4997 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 03:13:32.000000 tidyxbrl-0.1.0/src/tidyxbrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 03:13:33.004825 tidyxbrl-0.1.0/tests/
+-rw-rw-rw-   0        0        0      118 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/tests/test_edgar_frames.py
+-rw-rw-rw-   0        0        0      670 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/tests/test_edgar_query.py
+-rw-rw-rw-   0        0        0      516 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/tests/test_xbrl_parse.py
+-rw-rw-rw-   0        0        0     2174 2024-05-14 03:09:50.000000 tidyxbrl-0.1.0/tests/test_xbrl_query.py
```

### Comparing `tidyxbrl-0.0.50/LICENSE` & `tidyxbrl-0.1.0/LICENSE`

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

### Comparing `tidyxbrl-0.0.50/PKG-INFO` & `tidyxbrl-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,100 @@
-Metadata-Version: 2.1
-Name: tidyxbrl
-Version: 0.0.50
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
+Version: 0.1.0
+Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
+Home-page: https://github.com/cowboycodeman/tidyxbrl/
+Author: Ryan McDonald
+Author-email: ryancmcdonald@gmail.com
+Project-URL: Bug Tracker, https://github.com/cowboycodeman/tidyxbrl/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: bs4
+Requires-Dist: tqdm
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

### Comparing `tidyxbrl-0.0.50/README.md` & `tidyxbrl-0.1.0/src/tidyxbrl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,100 @@
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
+Version: 0.1.0
+Summary: A package to parse the XBRL file format & interface with XBRL APIs in a tidy format
+Home-page: https://github.com/cowboycodeman/tidyxbrl/
+Author: Ryan McDonald
+Author-email: ryancmcdonald@gmail.com
+Project-URL: Bug Tracker, https://github.com/cowboycodeman/tidyxbrl/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: bs4
+Requires-Dist: tqdm
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

### Comparing `tidyxbrl-0.0.50/src/tidyxbrl/xbrl_apikey.py` & `tidyxbrl-0.1.0/src/tidyxbrl/xbrl_apikey.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,95 @@
-import pandas
-import requests
-
-
-def xbrl_apikey(username, password, client_id, client_secret, platform='pc', grant_type='password', refresh_token=''):
-    """
-    The xbrl_apikey function is used to generate or refresh a temporary tolken to be used with the xbrl_apiquery function
-    Inputs:
-        username: Email address corresponding to the xbrl.us api website
-        password: Password corresponding to the xbrl.us api website
-        client_id: Active public Client ID 
-        client_secret: Secret ID corresponding to the client_id above
-        platform: Keyword to distinguish if the user is authenticating from different applications
-        grant_type: Either 'password' to generate a new key, or 'refresh_token' to refresh an existing key (see refresh_token)
-        refresh_token: Optional refresh token provided in a previous xbrl_apikey request 
-
-    Outputs:
-        xbrl_apikeyoutput: Pandas DataFrame output of the XBRL api key
-            - platform: Keyword to distinguish if the user is authenticating from different applications (specified in the request)
-            - access_token: Access token to be passed to the xbrl_apiquery function
-            - refresh_token: Refresh token to refresh the 'access_token'. Can be passed back to the function with a 'refresh_token' grant_type
-            - expires_in: Seconds until expiry
-            - refresh_token_expires_in token_type: Seconds until refresh token expiry
-            - token_type: type of token. Always "bearer"
-
-    The apikey can be accessed in the abrl_apiquery function using: access_token=xbrl_apikeyoutput.access_token.values[0]
-
-    Examples:
-        xbrl_apikeyoutput = xbrl_apikey(username='username', password='password', client_id='client_id', client_secret='client_secret', platform='pc', grant_type='password', refresh_token='optional_refresh_token')
-    """
-
-    # Submit the request based on the grant_type
-    # If password, generate a new tolken
-    if grant_type == "password":
-        xbrl_apikeyoutput = requests.post(url='https://api.xbrl.us/oauth2/token', data={'grant_type': grant_type,
-                                                                                        'client_id': client_id,
-                                                                                        'client_secret': client_secret,
-                                                                                        'username': username,
-                                                                                        'password': password,
-                                                                                        'platform': platform
-                                                                                        })
-    # If refresh_token, refresh an existing token
-    elif grant_type == "refresh_token":
-        xbrl_apikeyoutput = requests.post(url='https://api.xbrl.us/oauth2/token', data={'grant_type': grant_type,
-                                                                                        'client_id': client_id,
-                                                                                        'client_secret': client_secret,
-                                                                                        'refresh_token': refresh_token,
-                                                                                        'platform': platform
-                                                                                        })
-    else:
-        raise ValueError(
-            "grant_type must be either 'password' or 'refresh_token'")
-    # Check the Response Code. 200 is a success
-    if xbrl_apikeyoutput.status_code == 200:
-        try:
-            result = pandas.DataFrame(
-                pandas.json_normalize(xbrl_apikeyoutput.json()))
-        except Exception:
-            raise ValueError(str(dataresponse.json()))
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

### Comparing `tidyxbrl-0.0.50/src/tidyxbrl/xbrl_query.py` & `tidyxbrl-0.1.0/src/tidyxbrl/xbrl_query.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,74 @@
-import pandas
-import requests
-
-
-def xbrl_query(access_token,
-               queryparameters,
-               baseapiurl='https://api.xbrl.us/api/v1/report/search?'):
-    """
-    https://xbrl.us/home/use/xbrl-api/
-    http://files.xbrl.us/documents/XBRL-API-V1.4.pdf
-
-    The xbrl_query function is used to query the xbrl api usingthe token generated in the xbrl_apikey function. 
-    Inputs:
-        access_token: Access token string generated in the xbrl_apikey function. Found in the access_token column of the response dataframe.
-        baseapiurl: API request URL corresponding to the type of request prior to passing any parameters. This is everything up-to and including the "?" in the API request
-            - 'https://api.xbrl.us/api/v1/report/search?'
-            - 'https://api.xbrl.us/api/v1/fact/search?'
-        queryparameters: Dictionary structure to specify each aspect of the api request (See the Examples section below)
-
-    Outputs:
-        xbrl_queryoutput: Pandas Dataframe object corresponding to the fields specified in the request
-
-    Examples:
-        - xbrl_query(access_token=xbrl_apikeyoutput.access_token.values[0], 
-                        baseapiurl='https://api.xbrl.us/api/v1/report/search?',
-                        queryparameters = {'report.entity-name': "APPLE INC.",
-                                        'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
-                                        'report.document-type': "10-K"
-                            })
-        - xbrl_query(access_token=xbrl_apikeyoutput.access_token.values[0], 
-                        baseapiurl='https://api.xbrl.us/api/v1/fact/search?',
-                        queryparameters = {'report.id': "315201",
-                                        'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
-                                        'concept.local-name': "AccumulatedOtherComprehensiveIncomeLossNetOfTax"
-                                })
-
-    """
-
-    # Modify the queryparameter keys to create a web request string in dataquery
-    # Add the "=" sign between keys and values
-    for keyholder in list(queryparameters.keys()):
-        queryparameters[keyholder + "="] = queryparameters[keyholder]
-        del queryparameters[keyholder]
-    # Add the "&" sign between keys
-    queryurl = ''.join(list(map(str.__add__, list(queryparameters.keys()), [
-                       "{}{}".format(i, '&') for i in list(queryparameters.values())])))[:-1]
-    # Add the baseurl and modified request values
-    dataquery = str(baseapiurl + queryurl)
-    # Generate the authentication bearer tolken
-    headers = {"Authorization": "Bearer " + access_token}
-    # Generate the response
-    dataresponse = requests.get(url=dataquery, headers=headers)
-    # Check the Response Code
-    if dataresponse.status_code == 200:
-        try:
-            xbrl_queryoutput = pandas.DataFrame.from_dict(
-                dataresponse.json()['data'])
-        except Exception:
-            raise ValueError(str(dataresponse.json()))
-    else:
-        xbrl_queryoutput = dataresponse.status_code
-        print(dataresponse.text)
-        raise ValueError(str(xbrl_queryoutput) + ": Error in Response")
-    return(xbrl_queryoutput)
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

### Comparing `tidyxbrl-0.0.50/src/tidyxbrl.egg-info/PKG-INFO` & `tidyxbrl-0.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,95 +1,80 @@
-Metadata-Version: 2.1
-Name: tidyxbrl
-Version: 0.0.50
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

### Comparing `tidyxbrl-0.0.50/src/tidyxbrl.egg-info/SOURCES.txt` & `tidyxbrl-0.1.0/src/tidyxbrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidyxbrl-0.0.50/tests/test_xbrl_query.py` & `tidyxbrl-0.1.0/tests/test_xbrl_query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-import yaml
-import tidyxbrl 
-
-credentials = yaml.safe_load(open("tests\test_credentials.yml", "r"))
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
+# %%
+import yaml
+import tidyxbrl 
+
+credentials = yaml.safe_load(open("tests/test_credentials.yml", "r"))
+username = credentials['credentials']['username'][0]
+password = credentials['credentials']['password'][0]
+client_id = credentials['credentials']['client_id'][0]
+client_secret = credentials['credentials']['client_secret'][0]
+
+response = tidyxbrl.xbrl_apikey(username=username, password=password, client_id=client_id, client_secret=client_secret, platform='pc', grant_type='password', refresh_token='')
+
+dataresponse = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
+               baseapiurl='https://api.xbrl.us/api/v1/report/search?',
+               queryparameters = {'report.entity-name': "APPLE INC.",
+                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
+                                  'report.document-type': "10-K"
+                        })
+
+dataresponse2 = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
+               baseapiurl='https://api.xbrl.us/api/v1/fact/search?',
+               queryparameters = {'report.id': "315201",
+                                  'fields': "report.id,report.entity-name,report.filing-date,report.base-taxonomy,report.document-type,report.accession,entity.ticker,report.sic-code,entity.cik,report.entry-type,report.period-end,report.sec-url,report.checks-run,report.accepted-timestamp.sort(DESC),report.limit(20),report.offset(0),dts.id,report.entry-url",
+                                  'concept.local-name': "AccumulatedOtherComprehensiveIncomeLossNetOfTax"
+                        })
+
+
+dataresponse3 = tidyxbrl.xbrl_query(access_token=response.access_token.values[0], 
+               baseapiurl='https://api.xbrl.us/api/v1/fact/141024005?',
+               queryparameters = {'fields': "fact.value,concept.local-name"
+                        })
```

