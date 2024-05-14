# Comparing `tmp/odoo_addons_oca_wms-16.0.20240503.1-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_wms-16.0.20240513.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1638 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3142 b- defN 24-May-04 06:43 odoo_addons_oca_wms-16.0.20240503.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-04 06:43 odoo_addons_oca_wms-16.0.20240503.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-04 06:43 odoo_addons_oca_wms-16.0.20240503.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-May-04 06:43 odoo_addons_oca_wms-16.0.20240503.1.dist-info/RECORD
-4 files, 3620 bytes uncompressed, 880 bytes compressed:  75.7%
+Zip file size: 1674 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3428 b- defN 24-May-14 07:05 odoo_addons_oca_wms-16.0.20240513.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 07:05 odoo_addons_oca_wms-16.0.20240513.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-14 07:05 odoo_addons_oca_wms-16.0.20240513.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-May-14 07:05 odoo_addons_oca_wms-16.0.20240513.3.dist-info/RECORD
+4 files, 3906 bytes uncompressed, 916 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_wms-16.0.20240503.1.dist-info/METADATA
+Filename: odoo_addons_oca_wms-16.0.20240513.3.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240503.1.dist-info/WHEEL
+Filename: odoo_addons_oca_wms-16.0.20240513.3.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240503.1.dist-info/top_level.txt
+Filename: odoo_addons_oca_wms-16.0.20240513.3.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20240503.1.dist-info/RECORD
+Filename: odoo_addons_oca_wms-16.0.20240513.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_wms-16.0.20240503.1.dist-info/METADATA` & `odoo_addons_oca_wms-16.0.20240513.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-wms
-Version: 16.0.20240503.1
+Version: 16.0.20240513.3
 Summary: Meta package for oca-wms Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-delivery-carrier-warehouse <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-stock-available-to-promise-release <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-stock-available-to-promise-release-block <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-shopfloor <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-shopfloor-base <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-shopfloor-batch-automatic-creation <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-shopfloor-mobile <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-shopfloor-mobile-base <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-shopfloor-mobile-base-auth-api-key <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-shopfloor-rest-log <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-shopfloor-workstation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-shopfloor-workstation-mobile <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-available-to-promise-release <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-available-to-promise-release-block <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-available-to-promise-release-exclude-location <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-dynamic-routing <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-picking-batch-creation <16.1dev,>=16.0dev
```

