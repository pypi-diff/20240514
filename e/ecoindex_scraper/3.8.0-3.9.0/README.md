# Comparing `tmp/ecoindex_scraper-3.8.0.tar.gz` & `tmp/ecoindex_scraper-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoindex_scraper-3.8.0.tar", max compression
+gzip compressed data, was "ecoindex_scraper-3.9.0.tar", max compression
```

## Comparing `ecoindex_scraper-3.8.0.tar` & `ecoindex_scraper-3.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     5220 2024-02-09 20:09:25.150870 ecoindex_scraper-3.8.0/README.md
--rw-r--r--   0        0        0        5 2023-12-02 16:59:07.814060 ecoindex_scraper-3.8.0/ecoindex/compute/VERSION
--rw-r--r--   0        0        0      373 2023-12-07 16:11:18.720893 ecoindex_scraper-3.8.0/ecoindex/compute/__init__.py
--rw-r--r--   0        0        0     1843 2023-12-02 16:59:07.818060 ecoindex_scraper-3.8.0/ecoindex/compute/ecoindex.py
--rw-r--r--   0        0        0     1004 2023-12-02 16:59:07.818060 ecoindex_scraper-3.8.0/ecoindex/data/__init__.py
--rw-r--r--   0        0        0       98 2023-12-02 16:59:07.818060 ecoindex_scraper-3.8.0/ecoindex/data/colors.py
--rw-r--r--   0        0        0       48 2023-12-02 16:59:07.818060 ecoindex_scraper-3.8.0/ecoindex/data/grades.py
--rw-r--r--   0        0        0       52 2023-12-02 16:59:07.818060 ecoindex_scraper-3.8.0/ecoindex/data/medians.py
--rw-r--r--   0        0        0      688 2023-12-02 16:59:07.818060 ecoindex_scraper-3.8.0/ecoindex/data/quantiles.py
--rw-r--r--   0        0        0       52 2023-12-02 16:59:07.818060 ecoindex_scraper-3.8.0/ecoindex/data/targets.py
--rw-r--r--   0        0        0        0 2023-12-02 16:59:07.822060 ecoindex_scraper-3.8.0/ecoindex/exceptions/__init__.py
--rw-r--r--   0        0        0      272 2023-12-07 19:17:39.206300 ecoindex_scraper-3.8.0/ecoindex/exceptions/scraper.py
--rw-r--r--   0        0        0      249 2023-12-02 16:59:07.822060 ecoindex_scraper-3.8.0/ecoindex/exceptions/worker.py
--rw-r--r--   0        0        0      871 2023-12-02 16:59:07.822060 ecoindex_scraper-3.8.0/ecoindex/models/__init__.py
--rw-r--r--   0        0        0     1018 2023-12-02 16:59:07.822060 ecoindex_scraper-3.8.0/ecoindex/models/api.py
--rw-r--r--   0        0        0     4524 2023-12-08 22:46:51.703116 ecoindex_scraper-3.8.0/ecoindex/models/compute.py
--rw-r--r--   0        0        0      551 2024-02-05 14:44:54.264186 ecoindex_scraper-3.8.0/ecoindex/models/enums.py
--rw-r--r--   0        0        0     3828 2023-12-02 16:59:07.822060 ecoindex_scraper-3.8.0/ecoindex/models/response_examples.py
--rw-r--r--   0        0        0     1089 2024-02-09 20:09:25.102870 ecoindex_scraper-3.8.0/ecoindex/models/scraper.py
--rw-r--r--   0        0        0      133 2023-12-02 16:59:07.826060 ecoindex_scraper-3.8.0/ecoindex/models/sort.py
--rw-r--r--   0        0        0     1868 2023-12-02 16:59:07.826060 ecoindex_scraper-3.8.0/ecoindex/models/tasks.py
--rw-r--r--   0        0        0        6 2024-02-09 20:11:29.102866 ecoindex_scraper-3.8.0/ecoindex/scraper/VERSION
--rw-r--r--   0        0        0       82 2023-12-02 16:59:07.826060 ecoindex_scraper-3.8.0/ecoindex/scraper/__init__.py
--rw-r--r--   0        0        0     5534 2024-02-09 20:09:25.146870 ecoindex_scraper-3.8.0/ecoindex/scraper/scrap.py
--rw-r--r--   0        0        0      167 2023-12-02 16:59:07.826060 ecoindex_scraper-3.8.0/ecoindex/utils/__init__.py
--rw-r--r--   0        0        0     3088 2023-12-02 16:59:07.830060 ecoindex_scraper-3.8.0/ecoindex/utils/cli_translations/en.yml
--rw-r--r--   0        0        0     3321 2023-12-02 16:59:07.830060 ecoindex_scraper-3.8.0/ecoindex/utils/cli_translations/fr.yml
--rw-r--r--   0        0        0     2242 2023-12-08 15:07:21.195825 ecoindex_scraper-3.8.0/ecoindex/utils/files.py
--rw-r--r--   0        0        0      679 2023-12-02 16:59:07.830060 ecoindex_scraper-3.8.0/ecoindex/utils/screenshots.py
--rw-r--r--   0        0        0      735 2024-02-09 20:11:32.322866 ecoindex_scraper-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     6186 1970-01-01 00:00:00.000000 ecoindex_scraper-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     5220 2024-02-15 13:57:41.540646 ecoindex_scraper-3.9.0/README.md
+-rw-r--r--   0        0        0        6 2024-02-15 13:57:41.528644 ecoindex_scraper-3.9.0/ecoindex/compute/VERSION
+-rw-r--r--   0        0        0      373 2024-02-15 13:57:41.528644 ecoindex_scraper-3.9.0/ecoindex/compute/__init__.py
+-rw-r--r--   0        0        0     1843 2024-02-15 13:57:41.528644 ecoindex_scraper-3.9.0/ecoindex/compute/ecoindex.py
+-rw-r--r--   0        0        0     1004 2024-02-15 13:57:41.528644 ecoindex_scraper-3.9.0/ecoindex/data/__init__.py
+-rw-r--r--   0        0        0       98 2024-02-15 13:57:41.528644 ecoindex_scraper-3.9.0/ecoindex/data/colors.py
+-rw-r--r--   0        0        0       48 2024-02-15 13:57:41.528644 ecoindex_scraper-3.9.0/ecoindex/data/grades.py
+-rw-r--r--   0        0        0       52 2024-02-15 13:57:41.528644 ecoindex_scraper-3.9.0/ecoindex/data/medians.py
+-rw-r--r--   0        0        0      688 2024-02-15 13:57:41.528644 ecoindex_scraper-3.9.0/ecoindex/data/quantiles.py
+-rw-r--r--   0        0        0       52 2024-02-15 13:57:41.528644 ecoindex_scraper-3.9.0/ecoindex/data/targets.py
+-rw-r--r--   0        0        0        0 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/exceptions/__init__.py
+-rw-r--r--   0        0        0      272 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/exceptions/scraper.py
+-rw-r--r--   0        0        0      249 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/exceptions/worker.py
+-rw-r--r--   0        0        0      871 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/models/__init__.py
+-rw-r--r--   0        0        0     1018 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/models/api.py
+-rw-r--r--   0        0        0     4524 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/models/compute.py
+-rw-r--r--   0        0        0      551 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/models/enums.py
+-rw-r--r--   0        0        0     3828 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/models/response_examples.py
+-rw-r--r--   0        0        0     1089 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/models/scraper.py
+-rw-r--r--   0        0        0      133 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/models/sort.py
+-rw-r--r--   0        0        0     1868 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/models/tasks.py
+-rw-r--r--   0        0        0        6 2024-02-15 13:57:56.564892 ecoindex_scraper-3.9.0/ecoindex/scraper/VERSION
+-rw-r--r--   0        0        0       82 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/scraper/__init__.py
+-rw-r--r--   0        0        0     5590 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/scraper/scrap.py
+-rw-r--r--   0        0        0      167 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/utils/__init__.py
+-rw-r--r--   0        0        0     3088 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/utils/cli_translations/en.yml
+-rw-r--r--   0        0        0     3321 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/utils/cli_translations/fr.yml
+-rw-r--r--   0        0        0     2242 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/utils/files.py
+-rw-r--r--   0        0        0      679 2024-02-15 13:57:41.532645 ecoindex_scraper-3.9.0/ecoindex/utils/screenshots.py
+-rw-r--r--   0        0        0      735 2024-02-15 13:57:59.372931 ecoindex_scraper-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6186 1970-01-01 00:00:00.000000 ecoindex_scraper-3.9.0/PKG-INFO
```

### Comparing `ecoindex_scraper-3.8.0/README.md` & `ecoindex_scraper-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/compute/ecoindex.py` & `ecoindex_scraper-3.9.0/ecoindex/compute/ecoindex.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/data/__init__.py` & `ecoindex_scraper-3.9.0/ecoindex/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/data/quantiles.py` & `ecoindex_scraper-3.9.0/ecoindex/data/quantiles.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/models/__init__.py` & `ecoindex_scraper-3.9.0/ecoindex/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/models/api.py` & `ecoindex_scraper-3.9.0/ecoindex/models/api.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/models/compute.py` & `ecoindex_scraper-3.9.0/ecoindex/models/compute.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/models/enums.py` & `ecoindex_scraper-3.9.0/ecoindex/models/enums.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/models/response_examples.py` & `ecoindex_scraper-3.9.0/ecoindex/models/response_examples.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/models/scraper.py` & `ecoindex_scraper-3.9.0/ecoindex/models/scraper.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/models/tasks.py` & `ecoindex_scraper-3.9.0/ecoindex/models/tasks.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/scraper/scrap.py` & `ecoindex_scraper-3.9.0/ecoindex/scraper/scrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
                     status=response.status,
                     message=response.status_text,
                 )
 
             await self.page.wait_for_load_state()
             sleep(self.wait_before_scroll)
             await self.generate_screenshot()
+            await self.page.keyboard.press('ArrowDown')
             await self.page.evaluate(
                 "window.scrollTo({ top: document.body.scrollHeight, behavior: 'smooth' })"
             )
             sleep(self.wait_after_scroll)
             total_nodes = await self.get_nodes_count()
 
             await self.page.close()
```

### Comparing `ecoindex_scraper-3.8.0/ecoindex/utils/cli_translations/en.yml` & `ecoindex_scraper-3.9.0/ecoindex/utils/cli_translations/en.yml`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/utils/cli_translations/fr.yml` & `ecoindex_scraper-3.9.0/ecoindex/utils/cli_translations/fr.yml`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/utils/files.py` & `ecoindex_scraper-3.9.0/ecoindex/utils/files.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/ecoindex/utils/screenshots.py` & `ecoindex_scraper-3.9.0/ecoindex/utils/screenshots.py`

 * *Files identical despite different names*

### Comparing `ecoindex_scraper-3.8.0/pyproject.toml` & `ecoindex_scraper-3.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecoindex_scraper"
-version = "3.8.0"
+version = "3.9.0"
 readme = "README.md"
 description = "Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser"
 authors = ['Vincent Vatelot <vincent.vatelot@ik.me>']
 license = "Creative Commons BY-NC-ND"
 homepage = "http://www.ecoindex.fr"
 repository = "https://github.com/cnumr/ecoindex_scrap_python"
 include = ["LICENSE"]
```

### Comparing `ecoindex_scraper-3.8.0/PKG-INFO` & `ecoindex_scraper-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoindex_scraper
-Version: 3.8.0
+Version: 3.9.0
 Summary: Ecoindex_scraper module provides a way to scrape data from given website while simulating a real web browser
 Home-page: http://www.ecoindex.fr
 License: Creative Commons BY-NC-ND
 Author: Vincent Vatelot
 Author-email: vincent.vatelot@ik.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

