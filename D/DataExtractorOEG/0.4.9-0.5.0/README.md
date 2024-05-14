# Comparing `tmp/dataextractoroeg-0.4.9.tar.gz` & `tmp/dataextractoroeg-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.4.9.tar", last modified: Tue May  7 10:38:42 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.5.0.tar", last modified: Tue May 14 10:52:53 2024, max compression
```

## Comparing `dataextractoroeg-0.4.9.tar` & `dataextractoroeg-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 10:38:42.317805 dataextractoroeg-0.4.9/
--rw-rw-rw-   0        0        0      277 2024-05-07 10:05:11.000000 dataextractoroeg-0.4.9/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-07 10:38:42.312689 dataextractoroeg-0.4.9/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3078 2024-05-07 10:38:42.000000 dataextractoroeg-0.4.9/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2024-05-07 10:38:42.000000 dataextractoroeg-0.4.9/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 10:38:42.000000 dataextractoroeg-0.4.9/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-07 10:38:42.000000 dataextractoroeg-0.4.9/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-07 10:38:42.000000 dataextractoroeg-0.4.9/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-07 10:38:42.000000 dataextractoroeg-0.4.9/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.9/LICENSE.txt
--rw-rw-rw-   0        0        0     3078 2024-05-07 10:38:42.314799 dataextractoroeg-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 10:38:42.303266 dataextractoroeg-0.4.9/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-05-07 10:38:42.310610 dataextractoroeg-0.4.9/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.9/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.9/doiExtractor/ExistingPapers/name_doi_papers.csv
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.9/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8351 2024-05-07 09:58:32.000000 dataextractoroeg-0.4.9/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2454 2024-05-07 10:17:03.000000 dataextractoroeg-0.4.9/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4120 2024-05-07 09:59:13.000000 dataextractoroeg-0.4.9/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-05-07 10:38:42.318770 dataextractoroeg-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-05-07 10:38:30.000000 dataextractoroeg-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:52:53.746728 dataextractoroeg-0.5.0/
+-rw-rw-rw-   0        0        0      277 2024-05-07 10:05:11.000000 dataextractoroeg-0.5.0/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-14 10:52:53.738728 dataextractoroeg-0.5.0/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     4299 2024-05-14 10:52:53.000000 dataextractoroeg-0.5.0/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-14 10:52:53.000000 dataextractoroeg-0.5.0/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 10:52:53.000000 dataextractoroeg-0.5.0/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-14 10:52:53.000000 dataextractoroeg-0.5.0/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-14 10:52:53.000000 dataextractoroeg-0.5.0/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 10:52:53.000000 dataextractoroeg-0.5.0/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4299 2024-05-14 10:52:53.738728 dataextractoroeg-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4030 2024-05-14 08:44:15.000000 dataextractoroeg-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 10:52:53.710633 dataextractoroeg-0.5.0/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-14 10:52:53.738728 dataextractoroeg-0.5.0/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.5.0/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.5.0/doiExtractor/ExistingPapers/name_doi_papers.csv
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.5.0/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8443 2024-05-14 10:51:51.000000 dataextractoroeg-0.5.0/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2497 2024-05-14 10:51:29.000000 dataextractoroeg-0.5.0/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4116 2024-05-09 10:14:04.000000 dataextractoroeg-0.5.0/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 10:52:53.746728 dataextractoroeg-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-14 10:52:36.000000 dataextractoroeg-0.5.0/setup.py
```

### Comparing `dataextractoroeg-0.4.9/LICENSE.txt` & `dataextractoroeg-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.9/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.5.0/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.9/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.5.0/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.4.9/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.5.0/doiExtractor/doiExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pkg_resources
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from bs4 import BeautifulSoup
 import pandas as pd
 import urllib.parse
@@ -43,15 +44,15 @@
                     doi = next_sibling.strip()
                     if doi.startswith('https://doi.org/'):
                         doi = doi[len('https://doi.org/'):]  # Remove "https://doi.org/" from the beginning if present
                     # Write the resulting DOI to the CSV file
                     csv_file.writerow([title, doi])
                     doi_found = True
                 else:
-                    csv_file.writerow([title, "None"])
+                    csv_file.writerow([title, ""])
                     doi_found = False
                     
         return doi_found  # Return if DOI is found or not
     else:
         print("Error loading the webpage:", response.status_code)
         return False
 
@@ -191,11 +192,12 @@
 
 def csv_to_json(csv_file, json_file):
     df = pd.read_csv(csv_file)
     df.to_json(json_file, orient='records', indent=4)
 
 
 def find_file_by_name(path, name):
-    for root, dirs, files in os.walk(path):
+    package_path = pkg_resources.resource_filename(__name__, '')
+    for root, dirs, files in os.walk(package_path):
         if name in files:
             print(f"Found existing papers")
             return os.path.join(root, name)
```

### Comparing `dataextractoroeg-0.4.9/doiExtractor/main.py` & `dataextractoroeg-0.5.0/doiExtractor/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,19 @@
         txt_filename = args.output + "/dois.txt"
         csv_filename = args.output + "/results.csv"
         json_filename = args.output + "/results.json"
 
         os.makedirs(args.output, exist_ok=True)
 
         # ExistingPapers
-        papers = find_file_by_name(os.getcwd(),"name_doi_papers.csv")
+        papers = find_file_by_name("name_doi_papers.csv")
 
         logging.info("DOI Extractor Tool started")
         logging.info(f"Search in: {url}, Output csv: {csv_filename}, Output txt: {txt_filename}")
+        logging.info(f"Existing papers in: {papers}")
 
         # Delete contents of the files if already created
         if os.path.exists(csv_filename):
             open(csv_filename, 'w').close()
         if os.path.exists(txt_filename):
             open(txt_filename, 'w').close()
         if os.path.exists(json_filename):
```

### Comparing `dataextractoroeg-0.4.9/doiExtractor/openAlex.py` & `dataextractoroeg-0.5.0/doiExtractor/openAlex.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         else:
             page_url = get_primary_location_by_doi(name, doi)
         
         if page_url[0] is not None:
             row["primary_location"] = page_url[0]
             print(f"Searching in OpenAlex for {name} \nFounded link:{page_url[0]}")
         else:
-            row["primary_location"] = "None"
+            row["primary_location"] = ""
             print(f"Searching in OpenAlex for {name}: No primary location")
         print("-----------------------------------------------------------------")
 
     new_columns = list(rows[0].keys())  
     if "primary_location" not in new_columns: 
         new_columns.append("primary_location")
```

### Comparing `dataextractoroeg-0.4.9/setup.py` & `dataextractoroeg-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.4.9",
+    version="0.5.0",
     author =  "Pablo Torija Martínez",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
```

