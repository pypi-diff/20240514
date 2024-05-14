# Comparing `tmp/crewai_tools-0.2.5.tar.gz` & `tmp/crewai_tools-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai_tools-0.2.5.tar", max compression
+gzip compressed data, was "crewai_tools-0.2.6.tar", max compression
```

## Comparing `crewai_tools-0.2.5.tar` & `crewai_tools-0.2.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.2.5/LICENSE
--rw-r--r--   0        0        0     3478 2024-05-02 06:04:48.741505 crewai_tools-0.2.5/README.md
--rw-r--r--   0        0        0      509 2024-05-02 05:49:21.488653 crewai_tools-0.2.5/crewai_tools/__init__.py
--rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.2.5/crewai_tools/adapters/embedchain_adapter.py
--rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.2.5/crewai_tools/adapters/lancedb_adapter.py
--rw-r--r--   0        0        0     1541 2024-05-02 06:53:53.439980 crewai_tools-0.2.5/crewai_tools/tools/__init__.py
--rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.2.5/crewai_tools/tools/base_tool.py
--rw-r--r--   0        0        0      931 2024-05-02 05:36:37.312858 crewai_tools-0.2.5/crewai_tools/tools/browserbase_load_tool/README.md
--rw-r--r--   0        0        0     1166 2024-05-02 06:55:55.945860 crewai_tools-0.2.5/crewai_tools/tools/browserbase_load_tool/browserbase_load_tool.py
--rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.2.5/crewai_tools/tools/code_docs_search_tool/README.md
--rw-r--r--   0        0        0     1723 2024-04-10 14:50:04.964839 crewai_tools-0.2.5/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
--rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.2.5/crewai_tools/tools/csv_search_tool/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.965121 crewai_tools-0.2.5/crewai_tools/tools/csv_search_tool/csv_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.2.5/crewai_tools/tools/directory_read_tool/README.md
--rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.2.5/crewai_tools/tools/directory_read_tool/directory_read_tool.py
--rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.2.5/crewai_tools/tools/directory_search_tool/README.md
--rw-r--r--   0        0        0     1780 2024-04-10 14:50:04.965389 crewai_tools-0.2.5/crewai_tools/tools/directory_search_tool/directory_search_tool.py
--rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.2.5/crewai_tools/tools/docx_search_tool/README.md
--rw-r--r--   0        0        0     1983 2024-05-09 12:10:27.910396 crewai_tools-0.2.5/crewai_tools/tools/docx_search_tool/docx_search_tool.py
--rw-r--r--   0        0        0     1472 2024-05-02 05:50:40.176058 crewai_tools-0.2.5/crewai_tools/tools/exa_tools/README.md
--rw-r--r--   0        0        0     1044 2024-05-02 07:12:25.534945 crewai_tools-0.2.5/crewai_tools/tools/exa_tools/exa_base_tool.py
--rw-r--r--   0        0        0      650 2024-05-03 01:31:40.048347 crewai_tools-0.2.5/crewai_tools/tools/exa_tools/exa_search_tool.py
--rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.2.5/crewai_tools/tools/file_read_tool/README.md
--rw-r--r--   0        0        0     1350 2024-05-02 05:36:37.313883 crewai_tools-0.2.5/crewai_tools/tools/file_read_tool/file_read_tool.py
--rw-r--r--   0        0        0     2934 2024-04-10 14:50:04.965947 crewai_tools-0.2.5/crewai_tools/tools/github_search_tool/README.md
--rw-r--r--   0        0        0     2455 2024-04-10 14:50:04.966204 crewai_tools-0.2.5/crewai_tools/tools/github_search_tool/github_search_tool.py
--rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.2.5/crewai_tools/tools/json_search_tool/README.md
--rw-r--r--   0        0        0     1677 2024-04-10 14:50:04.966622 crewai_tools-0.2.5/crewai_tools/tools/json_search_tool/json_search_tool.py
--rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.2.5/crewai_tools/tools/mdx_seach_tool/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.966794 crewai_tools-0.2.5/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
--rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.2.5/crewai_tools/tools/pdf_search_tool/README.md
--rw-r--r--   0        0        0     1462 2024-04-10 14:50:04.967262 crewai_tools-0.2.5/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
--rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.2.5/crewai_tools/tools/pg_seach_tool/README.md
--rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.2.5/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
--rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.2.5/crewai_tools/tools/rag/README.md
--rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.2.5/crewai_tools/tools/rag/__init__.py
--rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.2.5/crewai_tools/tools/rag/rag_tool.py
--rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.2.5/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
--rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.2.5/crewai_tools/tools/scrape_website_tool/README.md
--rw-r--r--   0        0        0     2135 2024-04-07 17:18:28.181398 crewai_tools-0.2.5/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
--rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.2.5/crewai_tools/tools/selenium_scraping_tool/README.md
--rw-r--r--   0        0        0     2504 2024-05-02 06:04:48.748764 crewai_tools-0.2.5/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
--rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.2.5/crewai_tools/tools/serper_dev_tool/README.md
--rw-r--r--   0        0        0     1447 2024-05-02 05:48:30.482467 crewai_tools-0.2.5/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
--rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.2.5/crewai_tools/tools/txt_search_tool/README.md
--rw-r--r--   0        0        0     1627 2024-04-10 14:50:04.967435 crewai_tools-0.2.5/crewai_tools/tools/txt_search_tool/txt_search_tool.py
--rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.2.5/crewai_tools/tools/website_search/README.md
--rw-r--r--   0        0        0     1713 2024-04-10 14:50:04.967608 crewai_tools-0.2.5/crewai_tools/tools/website_search/website_search_tool.py
--rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.2.5/crewai_tools/tools/xml_search_tool/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.967788 crewai_tools-0.2.5/crewai_tools/tools/xml_search_tool/xml_search_tool.py
--rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.2.5/crewai_tools/tools/youtube_channel_search_tool/README.md
--rw-r--r--   0        0        0     2071 2024-04-10 14:50:04.968144 crewai_tools-0.2.5/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
--rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.2.5/crewai_tools/tools/youtube_video_search_tool/README.md
--rw-r--r--   0        0        0     1845 2024-04-10 14:50:04.968320 crewai_tools-0.2.5/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
--rw-r--r--   0        0        0      748 2024-05-09 12:10:37.438284 crewai_tools-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 crewai_tools-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-01-14 14:53:52.377957 crewai_tools-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3478 2024-05-02 06:04:48.741505 crewai_tools-0.2.6/README.md
+-rw-r--r--   0        0        0      509 2024-05-02 05:49:21.488653 crewai_tools-0.2.6/crewai_tools/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-27 18:04:45.818361 crewai_tools-0.2.6/crewai_tools/adapters/embedchain_adapter.py
+-rw-r--r--   0        0        0     1698 2024-03-27 18:04:45.818963 crewai_tools-0.2.6/crewai_tools/adapters/lancedb_adapter.py
+-rw-r--r--   0        0        0     1541 2024-05-02 06:53:53.439980 crewai_tools-0.2.6/crewai_tools/tools/__init__.py
+-rw-r--r--   0        0        0     4638 2024-03-27 18:04:45.836995 crewai_tools-0.2.6/crewai_tools/tools/base_tool.py
+-rw-r--r--   0        0        0      931 2024-05-02 05:36:37.312858 crewai_tools-0.2.6/crewai_tools/tools/browserbase_load_tool/README.md
+-rw-r--r--   0        0        0     1166 2024-05-02 06:55:55.945860 crewai_tools-0.2.6/crewai_tools/tools/browserbase_load_tool/browserbase_load_tool.py
+-rw-r--r--   0        0        0     2316 2024-03-27 18:04:45.819894 crewai_tools-0.2.6/crewai_tools/tools/code_docs_search_tool/README.md
+-rw-r--r--   0        0        0     1723 2024-04-10 14:50:04.964839 crewai_tools-0.2.6/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py
+-rw-r--r--   0        0        0     1880 2024-03-27 18:04:45.820663 crewai_tools-0.2.6/crewai_tools/tools/csv_search_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.965121 crewai_tools-0.2.6/crewai_tools/tools/csv_search_tool/csv_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.821563 crewai_tools-0.2.6/crewai_tools/tools/directory_read_tool/README.md
+-rw-r--r--   0        0        0     1362 2024-02-29 06:10:11.673676 crewai_tools-0.2.6/crewai_tools/tools/directory_read_tool/directory_read_tool.py
+-rw-r--r--   0        0        0     2062 2024-03-27 18:04:45.822143 crewai_tools-0.2.6/crewai_tools/tools/directory_search_tool/README.md
+-rw-r--r--   0        0        0     1780 2024-04-10 14:50:04.965389 crewai_tools-0.2.6/crewai_tools/tools/directory_search_tool/directory_search_tool.py
+-rw-r--r--   0        0        0     2000 2024-03-27 18:04:45.823166 crewai_tools-0.2.6/crewai_tools/tools/docx_search_tool/README.md
+-rw-r--r--   0        0        0     1983 2024-05-09 12:10:27.910396 crewai_tools-0.2.6/crewai_tools/tools/docx_search_tool/docx_search_tool.py
+-rw-r--r--   0        0        0     1472 2024-05-02 05:50:40.176058 crewai_tools-0.2.6/crewai_tools/tools/exa_tools/README.md
+-rw-r--r--   0        0        0     1044 2024-05-02 07:12:25.534945 crewai_tools-0.2.6/crewai_tools/tools/exa_tools/exa_base_tool.py
+-rw-r--r--   0        0        0      675 2024-05-14 00:30:20.113726 crewai_tools-0.2.6/crewai_tools/tools/exa_tools/exa_search_tool.py
+-rw-r--r--   0        0        0     1264 2024-03-04 00:30:35.475774 crewai_tools-0.2.6/crewai_tools/tools/file_read_tool/README.md
+-rw-r--r--   0        0        0     1350 2024-05-02 05:36:37.313883 crewai_tools-0.2.6/crewai_tools/tools/file_read_tool/file_read_tool.py
+-rw-r--r--   0        0        0     2934 2024-04-10 14:50:04.965947 crewai_tools-0.2.6/crewai_tools/tools/github_search_tool/README.md
+-rw-r--r--   0        0        0     2455 2024-04-10 14:50:04.966204 crewai_tools-0.2.6/crewai_tools/tools/github_search_tool/github_search_tool.py
+-rw-r--r--   0        0        0     2151 2024-03-27 18:04:45.824313 crewai_tools-0.2.6/crewai_tools/tools/json_search_tool/README.md
+-rw-r--r--   0        0        0     1677 2024-04-10 14:50:04.966622 crewai_tools-0.2.6/crewai_tools/tools/json_search_tool/json_search_tool.py
+-rw-r--r--   0        0        0     1981 2024-03-27 18:04:45.824825 crewai_tools-0.2.6/crewai_tools/tools/mdx_seach_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.966794 crewai_tools-0.2.6/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py
+-rw-r--r--   0        0        0     1911 2024-03-27 18:04:45.825449 crewai_tools-0.2.6/crewai_tools/tools/pdf_search_tool/README.md
+-rw-r--r--   0        0        0     1462 2024-04-10 14:50:04.967262 crewai_tools-0.2.6/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py
+-rw-r--r--   0        0        0     2255 2024-03-27 18:04:45.827071 crewai_tools-0.2.6/crewai_tools/tools/pg_seach_tool/README.md
+-rw-r--r--   0        0        0     1387 2024-04-04 16:45:56.495555 crewai_tools-0.2.6/crewai_tools/tools/pg_seach_tool/pg_search_tool.py
+-rw-r--r--   0        0        0     1908 2024-03-27 18:04:45.827831 crewai_tools-0.2.6/crewai_tools/tools/rag/README.md
+-rw-r--r--   0        0        0        0 2024-02-15 16:59:19.054644 crewai_tools-0.2.6/crewai_tools/tools/rag/__init__.py
+-rw-r--r--   0        0        0     1915 2024-03-27 18:04:45.828213 crewai_tools-0.2.6/crewai_tools/tools/rag/rag_tool.py
+-rw-r--r--   0        0        0     2400 2024-02-29 06:10:11.675121 crewai_tools-0.2.6/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py
+-rw-r--r--   0        0        0      953 2024-03-04 00:42:02.929279 crewai_tools-0.2.6/crewai_tools/tools/scrape_website_tool/README.md
+-rw-r--r--   0        0        0     2135 2024-04-07 17:18:28.181398 crewai_tools-0.2.6/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py
+-rw-r--r--   0        0        0     1687 2024-03-04 00:46:01.635253 crewai_tools-0.2.6/crewai_tools/tools/selenium_scraping_tool/README.md
+-rw-r--r--   0        0        0     2504 2024-05-02 06:04:48.748764 crewai_tools-0.2.6/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py
+-rw-r--r--   0        0        0     1460 2024-03-04 01:00:13.261512 crewai_tools-0.2.6/crewai_tools/tools/serper_dev_tool/README.md
+-rw-r--r--   0        0        0     1447 2024-05-02 05:48:30.482467 crewai_tools-0.2.6/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py
+-rw-r--r--   0        0        0     2315 2024-03-27 18:04:45.828637 crewai_tools-0.2.6/crewai_tools/tools/txt_search_tool/README.md
+-rw-r--r--   0        0        0     1627 2024-04-10 14:50:04.967435 crewai_tools-0.2.6/crewai_tools/tools/txt_search_tool/txt_search_tool.py
+-rw-r--r--   0        0        0     2204 2024-03-27 18:04:45.829231 crewai_tools-0.2.6/crewai_tools/tools/website_search/README.md
+-rw-r--r--   0        0        0     1713 2024-04-10 14:50:04.967608 crewai_tools-0.2.6/crewai_tools/tools/website_search/website_search_tool.py
+-rw-r--r--   0        0        0     2259 2024-03-27 18:04:45.829685 crewai_tools-0.2.6/crewai_tools/tools/xml_search_tool/README.md
+-rw-r--r--   0        0        0     1621 2024-04-10 14:50:04.967788 crewai_tools-0.2.6/crewai_tools/tools/xml_search_tool/xml_search_tool.py
+-rw-r--r--   0        0        0     2361 2024-03-27 18:04:45.830409 crewai_tools-0.2.6/crewai_tools/tools/youtube_channel_search_tool/README.md
+-rw-r--r--   0        0        0     2071 2024-04-10 14:50:04.968144 crewai_tools-0.2.6/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py
+-rw-r--r--   0        0        0     2579 2024-03-27 18:04:45.830762 crewai_tools-0.2.6/crewai_tools/tools/youtube_video_search_tool/README.md
+-rw-r--r--   0        0        0     1845 2024-04-10 14:50:04.968320 crewai_tools-0.2.6/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py
+-rw-r--r--   0        0        0      748 2024-05-14 00:30:26.125714 crewai_tools-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 crewai_tools-0.2.6/PKG-INFO
```

### Comparing `crewai_tools-0.2.5/LICENSE` & `crewai_tools-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/README.md` & `crewai_tools-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/adapters/embedchain_adapter.py` & `crewai_tools-0.2.6/crewai_tools/adapters/embedchain_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/adapters/lancedb_adapter.py` & `crewai_tools-0.2.6/crewai_tools/adapters/lancedb_adapter.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/__init__.py` & `crewai_tools-0.2.6/crewai_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/base_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/browserbase_load_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/browserbase_load_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/browserbase_load_tool/browserbase_load_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/browserbase_load_tool/browserbase_load_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/code_docs_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/code_docs_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/code_docs_search_tool/code_docs_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/csv_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/csv_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/csv_search_tool/csv_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/csv_search_tool/csv_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/directory_read_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/directory_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/directory_read_tool/directory_read_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/directory_read_tool/directory_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/directory_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/directory_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/directory_search_tool/directory_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/directory_search_tool/directory_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/docx_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/docx_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/docx_search_tool/docx_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/docx_search_tool/docx_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/exa_tools/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/exa_tools/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/exa_tools/exa_base_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/exa_tools/exa_base_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/exa_tools/exa_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/exa_tools/exa_search_tool.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
   ) -> Any:
     search_query = kwargs.get('search_query')
     if search_query is None:
       search_query = kwargs.get('query')
 
     payload = {
         "query": search_query,
+        "type": "magic",
     }
 
     headers = self.headers.copy()
     headers["x-api-key"] = os.environ['EXA_API_KEY']
 
     response = requests.post(self.search_url, json=payload, headers=headers)
     results = response.json()
```

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/file_read_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/file_read_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/file_read_tool/file_read_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/file_read_tool/file_read_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/github_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/github_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/github_search_tool/github_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/github_search_tool/github_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/json_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/json_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/json_search_tool/json_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/json_search_tool/json_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/mdx_seach_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/mdx_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/mdx_seach_tool/mdx_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/pdf_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/pdf_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/pdf_search_tool/pdf_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/pg_seach_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/pg_seach_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/pg_seach_tool/pg_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/pg_seach_tool/pg_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/rag/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/rag/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/rag/rag_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/rag/rag_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py` & `crewai_tools-0.2.6/crewai_tools/tools/scrape_element_from_website/scrape_element_from_website.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/scrape_website_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/scrape_website_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/scrape_website_tool/scrape_website_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/selenium_scraping_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/selenium_scraping_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/selenium_scraping_tool/selenium_scraping_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/serper_dev_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/serper_dev_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/serper_dev_tool/serper_dev_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/txt_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/txt_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/txt_search_tool/txt_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/txt_search_tool/txt_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/website_search/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/website_search/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/website_search/website_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/website_search/website_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/xml_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/xml_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/xml_search_tool/xml_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/xml_search_tool/xml_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/youtube_channel_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/youtube_channel_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/youtube_channel_search_tool/youtube_channel_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/youtube_video_search_tool/README.md` & `crewai_tools-0.2.6/crewai_tools/tools/youtube_video_search_tool/README.md`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py` & `crewai_tools-0.2.6/crewai_tools/tools/youtube_video_search_tool/youtube_video_search_tool.py`

 * *Files identical despite different names*

### Comparing `crewai_tools-0.2.5/pyproject.toml` & `crewai_tools-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crewai-tools"
-version = "0.2.5"
+version = "0.2.6"
 description = "Set of tools for the crewAI framework"
 authors = ["João Moura <joaomdmoura@mgail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.13"
 pydantic = "^2.6.1"
```

### Comparing `crewai_tools-0.2.5/PKG-INFO` & `crewai_tools-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crewai-tools
-Version: 0.2.5
+Version: 0.2.6
 Summary: Set of tools for the crewAI framework
 Author: João Moura
 Author-email: joaomdmoura@mgail.com
 Requires-Python: >=3.10,<=3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

