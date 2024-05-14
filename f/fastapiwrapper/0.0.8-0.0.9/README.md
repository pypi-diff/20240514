# Comparing `tmp/fastapiwrapper-0.0.8.tar.gz` & `tmp/fastapiwrapper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapiwrapper-0.0.8.tar", last modified: Mon May 13 11:31:54 2024, max compression
+gzip compressed data, was "fastapiwrapper-0.0.9.tar", last modified: Tue May 14 14:07:28 2024, max compression
```

## Comparing `fastapiwrapper-0.0.8.tar` & `fastapiwrapper-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 11:31:54.268325 fastapiwrapper-0.0.8/
--rw-rw-rw-   0        0        0      652 2024-05-13 11:31:54.268325 fastapiwrapper-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 11:31:54.264180 fastapiwrapper-0.0.8/fastapiwrapper/
--rw-rw-rw-   0        0        0       38 2024-05-13 11:28:12.000000 fastapiwrapper-0.0.8/fastapiwrapper/__init__.py
--rw-rw-rw-   0        0        0     8217 2024-04-25 12:25:14.000000 fastapiwrapper-0.0.8/fastapiwrapper/fastapiwrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-13 11:31:54.268325 fastapiwrapper-0.0.8/fastapiwrapper.egg-info/
--rw-rw-rw-   0        0        0      652 2024-05-13 11:31:54.000000 fastapiwrapper-0.0.8/fastapiwrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-13 11:31:54.000000 fastapiwrapper-0.0.8/fastapiwrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 11:31:54.000000 fastapiwrapper-0.0.8/fastapiwrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 11:31:54.000000 fastapiwrapper-0.0.8/fastapiwrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-13 11:31:54.000000 fastapiwrapper-0.0.8/fastapiwrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 11:31:54.268325 fastapiwrapper-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      988 2024-05-13 11:29:45.000000 fastapiwrapper-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:07:28.852943 fastapiwrapper-0.0.9/
+-rw-rw-rw-   0        0        0      652 2024-05-14 14:07:28.852943 fastapiwrapper-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 14:07:28.848937 fastapiwrapper-0.0.9/fastapiwrapper/
+-rw-rw-rw-   0        0        0       38 2024-05-13 11:28:12.000000 fastapiwrapper-0.0.9/fastapiwrapper/__init__.py
+-rw-rw-rw-   0        0        0     7559 2024-05-14 14:06:56.000000 fastapiwrapper-0.0.9/fastapiwrapper/fastapiwrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-14 14:07:28.851944 fastapiwrapper-0.0.9/fastapiwrapper.egg-info/
+-rw-rw-rw-   0        0        0      652 2024-05-14 14:07:28.000000 fastapiwrapper-0.0.9/fastapiwrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-14 14:07:28.000000 fastapiwrapper-0.0.9/fastapiwrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 14:07:28.000000 fastapiwrapper-0.0.9/fastapiwrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 14:07:28.000000 fastapiwrapper-0.0.9/fastapiwrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 14:07:28.000000 fastapiwrapper-0.0.9/fastapiwrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 14:07:28.852943 fastapiwrapper-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      988 2024-05-14 14:07:18.000000 fastapiwrapper-0.0.9/setup.py
```

### Comparing `fastapiwrapper-0.0.8/PKG-INFO` & `fastapiwrapper-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapiwrapper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrap an api that can fitch Deftable and timeseries table to make it more convenient. 
 Author: Ahmad Riad
 Author-email: meuralengine@outlook.com
 Keywords: python,Deftable,timeseries
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `fastapiwrapper-0.0.8/fastapiwrapper/fastapiwrapper.py` & `fastapiwrapper-0.0.9/fastapiwrapper/fastapiwrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,21 +21,22 @@
             'accept': 'application/json',
             'Content-Type': 'application/x-www-form-urlencoded'
         }
         payload = {
             'username': self.username,
             'password': self.password
         }
-        response = requests.post(self.url+"login/", headers=headers, data=payload)
+        response = requests.post(self.url+"login/", headers=headers, data=payload)#
         
         if response.status_code == 202:
             data = response.json()
             
             return data['access_token']
         else:
+            data = response.json()
             raise ValueError(f"Authentication failed: {data['detail']}", response.status_code)
 
 
     @lru_cache(maxsize=None)
     def DefTable(self,curveid = None):
         if curveid is None:
             url_1 = self.url+'get/DefTable'
@@ -48,14 +49,15 @@
                 logging.warning("The response is empty due to a server problem.")
 
             if response_1.status_code == 200:
                 data_1 = response_1.json()
                 df = pd.DataFrame(data_1)
                 return df
             else:
+                data_1 = response_1.json()
                 raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
             
             
         else:
             url_1 = self.url+ f'get/DefTable?cur={curveid}'
             headers_1 = {
                 'accept': 'application/json',
@@ -65,14 +67,15 @@
             
             if response_1.status_code == 200:
                 data_1 = response_1.json()
                 df = pd.DataFrame(data_1)
                 return df
             
             else:
+                data_1 = response_1.json()
                 raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
     
             
     
     @lru_cache(maxsize=None)
     def TimeSeries(self, curveid = None, startdate = None, enddate = None):
         if curveid is None:
@@ -86,14 +89,15 @@
                         
                 response_1 = requests.get(url_1, headers=headers_1)
                 if response_1.status_code == 200:
                     data_1 = response_1.json()
                     df = pd.DataFrame(data_1)
                     return df
                 else:
+                    data_1 = response_1.json()
                     raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
                     
                     
             elif startdate is not None and enddate == None:
                 url_1= self.url+f'get/TimeSeries?startdate={startdate}'
                 headers_1 = {
                     'accept': 'application/json',
@@ -102,14 +106,15 @@
                         
                 response_1 = requests.get(url_1, headers=headers_1)
                 if response_1.status_code == 200:
                     data_1 = response_1.json()
                     df = pd.DataFrame(data_1)
                     return df
                 else:
+                    data_1 = response_1.json()
                     raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
                     
             else:
                 url_1= self.url+'get/TimeSeries'
                 headers_1 = {
                     'accept': 'application/json',
                     'Authorization': f"Bearer {self.token}"
@@ -117,14 +122,15 @@
                         
                 response_1 = requests.get(url_1, headers=headers_1)
                 if response_1.status_code == 200:
                     data_1 = response_1.json()
                     df = pd.DataFrame(data_1)
                     return df
                 else:
+                    data_1 = response_1.json()
                     raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
             
                 
             
                 
         else:
             if startdate is not None and enddate is not None:
@@ -137,14 +143,15 @@
                         
                 response_1 = requests.get(url_1, headers=headers_1)
                 if response_1.status_code == 200:
                     data_1 = response_1.json()
                     df = pd.DataFrame(data_1)
                     return df
                 else:
+                    data_1 = response_1.json()
                     raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
                     
                     
             elif startdate is not None and enddate == None:
                 url_1= self.url+ f'get/TimeSeries?cur={curveid}&startdate={startdate}'
                 headers_1 = {
                     'accept': 'application/json',
@@ -153,14 +160,15 @@
                         
                 response_1 = requests.get(url_1, headers=headers_1)
                 if response_1.status_code == 200:
                     data_1 = response_1.json()
                     df = pd.DataFrame(data_1)
                     return df
                 else:
+                    data_1 = response_1.json()
                     raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
                     
             else:
                 url_1= self.url+ f'get/TimeSeries?cur={curveid}'
                 headers_1 = {
                     'accept': 'application/json',
                     'Authorization': f"Bearer {self.token}"
@@ -169,53 +177,18 @@
                 response_1 = requests.get(url_1, headers=headers_1)
                 
                 if response_1.status_code == 200:
                     data_1 = response_1.json()
                     df = pd.DataFrame(data_1)
                     return df
                 else:
+                    data_1 = response_1.json()
                     raise ValueError(f"Failed to get table: {data_1['detail']}", response_1.status_code)
             
             
-        # table['ValueDate']= pd.to_datetime(table['ValueDate'])
-        # startdate= pd.to_datetime(startdate)
-        # enddate= pd.to_datetime(enddate)
-        # if startdate is not None and enddate is not None:
-        #     sliced_by_date_range = table[(table['ValueDate'] >= startdate) & (table['ValueDate'] <= enddate)]
-        #     return sliced_by_date_range
-        
-        # elif startdate is not None and enddate == None:
-        #     sliced_by_date_range = table[(table['ValueDate'] >= startdate)]
-        #     return sliced_by_date_range
-        
-        # else:
-        #     return table
-  
-    
-#%%%%%%%%%%%   
-# from datetime import datetime
-   
-# curveid=2
-# analysis = Analysis('ahmadriad3@gmail.com', '12345678')
-
-# start = datetime.now()
-# table = analysis.DefTable()
-# end = datetime.now()
-# timing = end - start
-# print(timing)
-      
-      
-# start = datetime.now()
-# table_1= analysis.TimeSeries(startdate="2024-04-25")
-# end = datetime.now()
-# timing = end - start
-# print(timing)
-#%%%%%%%%%%%
-
-
```

### Comparing `fastapiwrapper-0.0.8/fastapiwrapper.egg-info/PKG-INFO` & `fastapiwrapper-0.0.9/fastapiwrapper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapiwrapper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrap an api that can fitch Deftable and timeseries table to make it more convenient. 
 Author: Ahmad Riad
 Author-email: meuralengine@outlook.com
 Keywords: python,Deftable,timeseries
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `fastapiwrapper-0.0.8/setup.py` & `fastapiwrapper-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Wrap an api that can fitch Deftable and timeseries table to make it more convenient. '
 LONG_DESCRIPTION = 'contain an api wrapper that helps to fetch gas cconsumption data.'
 
 # Setting up
 setup(
     name="fastapiwrapper",
     version=VERSION,
```

