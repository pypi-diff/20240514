# Comparing `tmp/prodmatic-2024.5.10.tar.gz` & `tmp/prodmatic-2024.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodmatic-2024.5.10.tar", last modified: Fri May 10 09:33:42 2024, max compression
+gzip compressed data, was "prodmatic-2024.5.14.tar", last modified: Tue May 14 12:54:22 2024, max compression
```

## Comparing `prodmatic-2024.5.10.tar` & `prodmatic-2024.5.14.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:33:42.747382 prodmatic-2024.5.10/
--rw-r--r--   0 gkoduri    (502) staff       (20)    34523 2024-05-10 09:30:22.000000 prodmatic-2024.5.10/LICENSE
--rw-r--r--   0 gkoduri    (502) staff       (20)     4488 2024-05-10 09:33:42.747178 prodmatic-2024.5.10/PKG-INFO
--rw-r--r--   0 gkoduri    (502) staff       (20)     3239 2024-05-10 09:29:12.000000 prodmatic-2024.5.10/README.md
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:33:42.739203 prodmatic-2024.5.10/prodmatic/
--rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/__init__.py
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:33:42.741069 prodmatic-2024.5.10/prodmatic/appstore/
--rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/appstore/__init__.py
--rw-r--r--   0 gkoduri    (502) staff       (20)     2048 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/appstore/api.py
--rw-r--r--   0 gkoduri    (502) staff       (20)     3493 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/appstore/pricing.py
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:33:42.742665 prodmatic-2024.5.10/prodmatic/base/
--rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/base/__init__.py
--rw-r--r--   0 gkoduri    (502) staff       (20)     1040 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/base/api.py
--rw-r--r--   0 gkoduri    (502) staff       (20)     3575 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/base/pricing.py
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:33:42.744618 prodmatic-2024.5.10/prodmatic/playstore/
--rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/playstore/__init__.py
--rw-r--r--   0 gkoduri    (502) staff       (20)    10496 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/playstore/api.py
--rw-r--r--   0 gkoduri    (502) staff       (20)     3761 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/playstore/pricing.py
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:33:42.746607 prodmatic-2024.5.10/prodmatic/resources/
--rw-r--r--   0 gkoduri    (502) staff       (20)     3503 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/resources/appstore_reference_prices.csv
--rw-r--r--   0 gkoduri    (502) staff       (20)      269 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/resources/data_sources.json
--rw-r--r--   0 gkoduri    (502) staff       (20)     1077 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/prodmatic/resources/playstore_reference_prices.csv
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:33:42.746820 prodmatic-2024.5.10/prodmatic.egg-info/
--rw-r--r--   0 gkoduri    (502) staff       (20)     4488 2024-05-10 09:33:42.000000 prodmatic-2024.5.10/prodmatic.egg-info/PKG-INFO
--rw-r--r--   0 gkoduri    (502) staff       (20)      603 2024-05-10 09:33:42.000000 prodmatic-2024.5.10/prodmatic.egg-info/SOURCES.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)        1 2024-05-10 09:33:42.000000 prodmatic-2024.5.10/prodmatic.egg-info/dependency_links.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       59 2024-05-10 09:33:42.000000 prodmatic-2024.5.10/prodmatic.egg-info/requires.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       10 2024-05-10 09:33:42.000000 prodmatic-2024.5.10/prodmatic.egg-info/top_level.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       38 2024-05-10 09:33:42.747439 prodmatic-2024.5.10/setup.cfg
--rw-r--r--   0 gkoduri    (502) staff       (20)     1586 2024-05-10 09:28:42.000000 prodmatic-2024.5.10/setup.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-14 12:54:22.862866 prodmatic-2024.5.14/
+-rw-r--r--   0 gkoduri    (502) staff       (20)    34523 2024-05-10 09:30:22.000000 prodmatic-2024.5.14/LICENSE
+-rw-r--r--   0 gkoduri    (502) staff       (20)     4488 2024-05-14 12:54:22.862648 prodmatic-2024.5.14/PKG-INFO
+-rw-r--r--   0 gkoduri    (502) staff       (20)     3239 2024-05-10 09:29:12.000000 prodmatic-2024.5.14/README.md
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-14 12:54:22.857123 prodmatic-2024.5.14/prodmatic/
+-rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/__init__.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-14 12:54:22.858166 prodmatic-2024.5.14/prodmatic/appstore/
+-rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/appstore/__init__.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)     2048 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/appstore/api.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)     3493 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/appstore/pricing.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-14 12:54:22.859735 prodmatic-2024.5.14/prodmatic/base/
+-rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/base/__init__.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)     1040 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/base/api.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)     2864 2024-05-14 06:22:46.000000 prodmatic-2024.5.14/prodmatic/base/pricing.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-14 12:54:22.860398 prodmatic-2024.5.14/prodmatic/playstore/
+-rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/playstore/__init__.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)    10496 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/playstore/api.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)     4026 2024-05-14 05:11:50.000000 prodmatic-2024.5.14/prodmatic/playstore/pricing.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-14 12:54:22.861142 prodmatic-2024.5.14/prodmatic/resources/
+-rw-r--r--   0 gkoduri    (502) staff       (20)     3503 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/resources/appstore_reference_prices.csv
+-rw-r--r--   0 gkoduri    (502) staff       (20)      269 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/resources/data_sources.json
+-rw-r--r--   0 gkoduri    (502) staff       (20)     1077 2024-05-10 09:28:42.000000 prodmatic-2024.5.14/prodmatic/resources/playstore_reference_prices.csv
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-14 12:54:22.862442 prodmatic-2024.5.14/prodmatic.egg-info/
+-rw-r--r--   0 gkoduri    (502) staff       (20)     4488 2024-05-14 12:54:22.000000 prodmatic-2024.5.14/prodmatic.egg-info/PKG-INFO
+-rw-r--r--   0 gkoduri    (502) staff       (20)      603 2024-05-14 12:54:22.000000 prodmatic-2024.5.14/prodmatic.egg-info/SOURCES.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)        1 2024-05-14 12:54:22.000000 prodmatic-2024.5.14/prodmatic.egg-info/dependency_links.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       59 2024-05-14 12:54:22.000000 prodmatic-2024.5.14/prodmatic.egg-info/requires.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       10 2024-05-14 12:54:22.000000 prodmatic-2024.5.14/prodmatic.egg-info/top_level.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       38 2024-05-14 12:54:22.862906 prodmatic-2024.5.14/setup.cfg
+-rw-r--r--   0 gkoduri    (502) staff       (20)     1586 2024-05-14 05:07:56.000000 prodmatic-2024.5.14/setup.py
```

### Comparing `prodmatic-2024.5.10/LICENSE` & `prodmatic-2024.5.14/LICENSE`

 * *Files identical despite different names*

### Comparing `prodmatic-2024.5.10/PKG-INFO` & `prodmatic-2024.5.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodmatic
-Version: 2024.5.10
+Version: 2024.5.14
 Summary: A Python package for seamless management and pricing of in-app products and subscriptions
 Home-page: https://github.com/musicmuni/prodmatic
 Author: Gopala Krishna Koduri
 Author-email: gopal@riyazapp.com
 Project-URL: Source Code, https://github.com/musicmuni/prodmatic
 Project-URL: Issue Tracker, https://github.com/musicmuni/prodmatic/issues
 Project-URL: Connect w/ Author, https://linkedin.com/in/gopalkoduri
```

### Comparing `prodmatic-2024.5.10/README.md` & `prodmatic-2024.5.14/README.md`

 * *Files identical despite different names*

### Comparing `prodmatic-2024.5.10/prodmatic/appstore/api.py` & `prodmatic-2024.5.14/prodmatic/appstore/api.py`

 * *Files identical despite different names*

### Comparing `prodmatic-2024.5.10/prodmatic/appstore/pricing.py` & `prodmatic-2024.5.14/prodmatic/appstore/pricing.py`

 * *Files identical despite different names*

### Comparing `prodmatic-2024.5.10/prodmatic/base/api.py` & `prodmatic-2024.5.14/prodmatic/base/api.py`

 * *Files identical despite different names*

### Comparing `prodmatic-2024.5.10/prodmatic/base/pricing.py` & `prodmatic-2024.5.14/prodmatic/base/pricing.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,45 +43,29 @@
         store_prices = []
         for mapping in ppp_price_mapping:
             iso2_code = mapping["ISO2"]
             local_price = mapping["ppp_adjusted_local_price"]
             country_info = self.countries_api.fetch_country_by_cca2(iso2_code)
             local_currencies = list(country_info.currencies.keys())
 
-            # Is the country featured in appstore list of countries? Chuck if not
-            if iso2_code not in self.map_country_to_reference_rounded_price:
-                continue
-
             # Convert local currency to store supported currency
             store_currency = "USD"
             if iso2_code in self.map_country_to_store_currency:
                 store_currency = self.map_country_to_store_currency[iso2_code]["store_currency"]
             store_price = self.forex_api.convert(
                 price=local_price, from_currency=local_currencies[0], to_currency=store_currency
             )
 
             # Some heavily devalued currencies might end up with very low usd values < 10
             # TODO needs a better fix
             if store_price < 10:
                 store_price = 10
 
             # Round off to a format that store recommends
-            store_price_format = self.map_country_to_reference_rounded_price[iso2_code]
+            store_price_format = self.map_country_to_reference_rounded_price.get(iso2_code, 0)
             rounded_price = self.formatter.apply_price_format(price=store_price, format=store_price_format)
 
             mapping["store_currency"] = store_currency
             mapping["store_price"] = rounded_price
             store_prices.append(mapping)
 
-        # Check for countries on store's reference list but not in final mapping (missing PPP data)
-        countries_missing_ppp = set(self.map_country_to_reference_rounded_price.keys()) - set(
-            [i["ISO2"] for i in store_prices]
-        )
-        for c in countries_missing_ppp:
-            mapping = {
-                "store_currency": "USD",
-                "store_price": source_price,
-                "ISO2": c,
-                "ppp_adjusted_local_price": None,
-            }
-            store_prices.append(mapping)
         return store_prices
```

### Comparing `prodmatic-2024.5.10/prodmatic/playstore/api.py` & `prodmatic-2024.5.14/prodmatic/playstore/api.py`

 * *Files identical despite different names*

### Comparing `prodmatic-2024.5.10/prodmatic/playstore/pricing.py` & `prodmatic-2024.5.14/prodmatic/playstore/pricing.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,19 +52,24 @@
                 if third_col_span and third_col_span.get("class"):
                     if "green-text" not in third_col_span.get("class"):
                         continue  # Exclude rows without check mark
 
                 # Create a list of column values
                 row_data = [col.get_text().strip() for i, col in enumerate(cols)]
 
-                # Extract only the capital letters from the fourth column
+                # Extract only the capital letters from the fourth column - currency
                 if len(row_data) > 3:
                     currency = "".join([c for c in row_data[3] if c.isupper()])
                     row_data[3] = currency
 
+                # Extract just alphabets from first column - country name
+                if len(row_data) >= 1:
+                    country_name = "".join([char for char in row_data[0] if char.isalpha()])
+                    row_data[0] = country_name
+
                 entry = dict(zip(headers, row_data))
                 country = self.countries_api.search_countries(entry["Location"])[0]
                 iso_code = country.cca2
 
                 entry_clean = {
                     "country": entry["Location"],
                     "iso2_code": iso_code,
```

### Comparing `prodmatic-2024.5.10/prodmatic/resources/appstore_reference_prices.csv` & `prodmatic-2024.5.14/prodmatic/resources/appstore_reference_prices.csv`

 * *Files identical despite different names*

### Comparing `prodmatic-2024.5.10/prodmatic/resources/playstore_reference_prices.csv` & `prodmatic-2024.5.14/prodmatic/resources/playstore_reference_prices.csv`

 * *Files identical despite different names*

### Comparing `prodmatic-2024.5.10/prodmatic.egg-info/PKG-INFO` & `prodmatic-2024.5.14/prodmatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodmatic
-Version: 2024.5.10
+Version: 2024.5.14
 Summary: A Python package for seamless management and pricing of in-app products and subscriptions
 Home-page: https://github.com/musicmuni/prodmatic
 Author: Gopala Krishna Koduri
 Author-email: gopal@riyazapp.com
 Project-URL: Source Code, https://github.com/musicmuni/prodmatic
 Project-URL: Issue Tracker, https://github.com/musicmuni/prodmatic/issues
 Project-URL: Connect w/ Author, https://linkedin.com/in/gopalkoduri
```

### Comparing `prodmatic-2024.5.10/prodmatic.egg-info/SOURCES.txt` & `prodmatic-2024.5.14/prodmatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prodmatic-2024.5.10/setup.py` & `prodmatic-2024.5.14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="prodmatic",
-    version="2024.05.10",
+    version="2024.05.14",
     description="A Python package for seamless management and pricing of in-app products and subscriptions",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Gopala Krishna Koduri",
     author_email="gopal@riyazapp.com",
     url="https://github.com/musicmuni/prodmatic",
     project_urls={
```

