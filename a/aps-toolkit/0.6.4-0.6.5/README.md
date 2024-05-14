# Comparing `tmp/aps-toolkit-0.6.4.tar.gz` & `tmp/aps-toolkit-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps-toolkit-0.6.4.tar", last modified: Sat May 11 17:23:52 2024, max compression
+gzip compressed data, was "aps-toolkit-0.6.5.tar", last modified: Tue May 14 15:10:14 2024, max compression
```

## Comparing `aps-toolkit-0.6.4.tar` & `aps-toolkit-0.6.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-11 17:23:52.975605 aps-toolkit-0.6.4/
--rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-11 17:23:52.975374 aps-toolkit-0.6.4/PKG-INFO
--rw-r--r--   0 chuongmep   (501) staff       (20)       38 2024-05-11 17:23:52.975647 aps-toolkit-0.6.4/setup.cfg
--rw-r--r--   0 chuongmep   (501) staff       (20)      983 2024-05-11 17:23:24.000000 aps-toolkit-0.6.4/setup.py
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-11 17:23:52.966200 aps-toolkit-0.6.4/src/
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-11 17:23:52.971689 aps-toolkit-0.6.4/src/aps_toolkit/
--rw-r--r--   0 chuongmep   (501) staff       (20)    12678 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/Auth.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     5499 2024-05-06 15:43:49.000000 aps-toolkit-0.6.4/src/aps_toolkit/AuthGoogleColab.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    28974 2024-05-11 17:19:27.000000 aps-toolkit-0.6.4/src/aps_toolkit/BIM360.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     8884 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/Bucket.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2454 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/DbReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    12722 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/Derivative.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3891 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/Fragments.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2322 2024-03-27 12:03:33.000000 aps-toolkit-0.6.4/src/aps_toolkit/InputStream.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      880 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/aps_toolkit/ManifestItem.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1136 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/MaterialProperties.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1726 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/Materials.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3686 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/PackFileReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      953 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/PathInfo.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     4520 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/ProDbReaderCad.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3547 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/ProDbReaderNavis.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    21227 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/ProDbReaderRevit.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    15777 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/PropReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1376 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/Resource.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1067 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFContent.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3333 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFGeometries.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1160 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFImage.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1037 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFLines.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      830 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFManifestType.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      886 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFMaterialGroup.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      773 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFMaterialMap.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      834 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFMaterialMapScale.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     7567 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFMaterials.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     9759 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFMesh.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      859 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFMetadata.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      936 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFPoints.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     6690 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFReader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      822 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFTransform.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      799 2024-03-17 07:21:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/SVFUVMap.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1005 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/Token.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     4975 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/Webhooks.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      822 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/__init__.py
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-11 17:23:52.972683 aps-toolkit-0.6.4/src/aps_toolkit/units/
--rw-r--r--   0 chuongmep   (501) staff       (20)     1442 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/units/DisplayUnits.py
--rw-r--r--   0 chuongmep   (501) staff       (20)        0 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/units/__init__.py
--rw-r--r--   0 chuongmep   (501) staff       (20)    36914 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/aps_toolkit/units/units.json
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-11 17:23:52.972316 aps-toolkit-0.6.4/src/aps_toolkit.egg-info/
--rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-11 17:23:52.000000 aps-toolkit-0.6.4/src/aps_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 chuongmep   (501) staff       (20)     1944 2024-05-11 17:23:52.000000 aps-toolkit-0.6.4/src/aps_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 chuongmep   (501) staff       (20)        1 2024-05-11 17:23:52.000000 aps-toolkit-0.6.4/src/aps_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 chuongmep   (501) staff       (20)       16 2024-05-11 17:23:52.000000 aps-toolkit-0.6.4/src/aps_toolkit.egg-info/requires.txt
--rw-r--r--   0 chuongmep   (501) staff       (20)       17 2024-05-11 17:23:52.000000 aps-toolkit-0.6.4/src/aps_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-11 17:23:52.975119 aps-toolkit-0.6.4/src/test/
--rw-r--r--   0 chuongmep   (501) staff       (20)        0 2024-03-12 14:17:11.000000 aps-toolkit-0.6.4/src/test/__init__.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1062 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/test/context.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1341 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/test/test_Webhooks.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1953 2024-05-06 15:43:49.000000 aps-toolkit-0.6.4/src/test/test_auth.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1393 2024-05-06 15:43:49.000000 aps-toolkit-0.6.4/src/test/test_auth_colab.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     4844 2024-05-11 17:16:22.000000 aps-toolkit-0.6.4/src/test/test_bim360.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1962 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/test/test_bucket.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      836 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/test/test_db_reader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1874 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/test/test_derivative.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      997 2024-03-13 15:06:23.000000 aps-toolkit-0.6.4/src/test/test_fragment.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      858 2024-03-13 15:27:50.000000 aps-toolkit-0.6.4/src/test/test_geometries.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      766 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/test/test_image.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1233 2024-03-13 15:27:50.000000 aps-toolkit-0.6.4/src/test/test_material.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      691 2024-03-13 15:27:50.000000 aps-toolkit-0.6.4/src/test/test_mesh.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      494 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/test/test_metadata.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1840 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/test/test_prop_reader.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     1442 2024-03-21 13:54:46.000000 aps-toolkit-0.6.4/src/test/test_prop_reader_cad.py
--rw-r--r--   0 chuongmep   (501) staff       (20)      777 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/test/test_prop_reader_navis.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     3427 2024-05-08 11:06:07.000000 aps-toolkit-0.6.4/src/test/test_prop_reader_revit.py
--rw-r--r--   0 chuongmep   (501) staff       (20)     2915 2024-05-01 12:43:15.000000 aps-toolkit-0.6.4/src/test/test_svf_reader.py
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-14 15:10:14.081180 aps-toolkit-0.6.5/
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-14 15:10:14.080842 aps-toolkit-0.6.5/PKG-INFO
+-rw-r--r--   0 chuongmep   (501) staff       (20)       38 2024-05-14 15:10:14.081237 aps-toolkit-0.6.5/setup.cfg
+-rw-r--r--   0 chuongmep   (501) staff       (20)      983 2024-05-14 15:10:06.000000 aps-toolkit-0.6.5/setup.py
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-14 15:10:14.071112 aps-toolkit-0.6.5/src/
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-14 15:10:14.076514 aps-toolkit-0.6.5/src/aps_toolkit/
+-rw-r--r--   0 chuongmep   (501) staff       (20)    12697 2024-05-12 15:30:28.000000 aps-toolkit-0.6.5/src/aps_toolkit/Auth.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     5534 2024-05-12 15:31:17.000000 aps-toolkit-0.6.5/src/aps_toolkit/AuthGoogleColab.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)    32538 2024-05-14 14:59:37.000000 aps-toolkit-0.6.5/src/aps_toolkit/BIM360.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     8891 2024-05-12 15:32:59.000000 aps-toolkit-0.6.5/src/aps_toolkit/Bucket.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     2493 2024-05-12 15:33:21.000000 aps-toolkit-0.6.5/src/aps_toolkit/DbReader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)    12722 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/Derivative.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3891 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/Fragments.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     2322 2024-03-27 12:03:33.000000 aps-toolkit-0.6.5/src/aps_toolkit/InputStream.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      880 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/aps_toolkit/ManifestItem.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1136 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/MaterialProperties.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1726 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/Materials.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3686 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/PackFileReader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      953 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/PathInfo.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     4520 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/ProDbReaderCad.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3547 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/ProDbReaderNavis.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)    21227 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/ProDbReaderRevit.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)    15777 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/PropReader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1376 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/Resource.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1067 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFContent.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3333 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFGeometries.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1160 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFImage.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1037 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFLines.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      830 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFManifestType.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      886 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFMaterialGroup.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      773 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFMaterialMap.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      834 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFMaterialMapScale.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     7567 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFMaterials.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     9759 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFMesh.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      859 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFMetadata.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      936 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFPoints.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     6690 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFReader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      822 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFTransform.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      799 2024-03-17 07:21:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/SVFUVMap.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1005 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/Token.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     4975 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/Webhooks.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      822 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/__init__.py
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-14 15:10:14.077504 aps-toolkit-0.6.5/src/aps_toolkit/units/
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1442 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/units/DisplayUnits.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)        0 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/units/__init__.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)    36914 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/aps_toolkit/units/units.json
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-14 15:10:14.077141 aps-toolkit-0.6.5/src/aps_toolkit.egg-info/
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1908 2024-05-14 15:10:13.000000 aps-toolkit-0.6.5/src/aps_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1944 2024-05-14 15:10:13.000000 aps-toolkit-0.6.5/src/aps_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 chuongmep   (501) staff       (20)        1 2024-05-14 15:10:13.000000 aps-toolkit-0.6.5/src/aps_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 chuongmep   (501) staff       (20)       16 2024-05-14 15:10:13.000000 aps-toolkit-0.6.5/src/aps_toolkit.egg-info/requires.txt
+-rw-r--r--   0 chuongmep   (501) staff       (20)       17 2024-05-14 15:10:13.000000 aps-toolkit-0.6.5/src/aps_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 chuongmep   (501) staff       (20)        0 2024-05-14 15:10:14.080475 aps-toolkit-0.6.5/src/test/
+-rw-r--r--   0 chuongmep   (501) staff       (20)        0 2024-03-12 14:17:11.000000 aps-toolkit-0.6.5/src/test/__init__.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1062 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/test/context.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1341 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/test/test_Webhooks.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1953 2024-05-14 13:29:14.000000 aps-toolkit-0.6.5/src/test/test_auth.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1393 2024-05-06 15:43:49.000000 aps-toolkit-0.6.5/src/test/test_auth_colab.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     5370 2024-05-14 14:53:20.000000 aps-toolkit-0.6.5/src/test/test_bim360.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1962 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/test/test_bucket.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      836 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/test/test_db_reader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1874 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/test/test_derivative.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      997 2024-03-13 15:06:23.000000 aps-toolkit-0.6.5/src/test/test_fragment.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      858 2024-03-13 15:27:50.000000 aps-toolkit-0.6.5/src/test/test_geometries.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      766 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/test/test_image.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1233 2024-03-13 15:27:50.000000 aps-toolkit-0.6.5/src/test/test_material.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      691 2024-03-13 15:27:50.000000 aps-toolkit-0.6.5/src/test/test_mesh.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      494 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/test/test_metadata.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1840 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/test/test_prop_reader.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     1442 2024-03-21 13:54:46.000000 aps-toolkit-0.6.5/src/test/test_prop_reader_cad.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)      777 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/test/test_prop_reader_navis.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     3427 2024-05-08 11:06:07.000000 aps-toolkit-0.6.5/src/test/test_prop_reader_revit.py
+-rw-r--r--   0 chuongmep   (501) staff       (20)     2915 2024-05-01 12:43:15.000000 aps-toolkit-0.6.5/src/test/test_svf_reader.py
```

### Comparing `aps-toolkit-0.6.4/PKG-INFO` & `aps-toolkit-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.6.4/setup.py` & `aps-toolkit-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("Readme.md") as f:
     if f is not None:
         readme = f.read()
 
 setuptools.setup(
     name="aps-toolkit",
-    version="0.6.4",
+    version="0.6.5",
     author="chuong mep",
     author_email="chuongpqvn@gmail.com",
     description="A Toolkit Autodesk Platform Services for Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/chuongmep/aps-toolkit",
     project_urls={
```

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/Auth.py` & `aps-toolkit-0.6.5/src/aps_toolkit/Auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         content = response.json()
         self.access_token = content['access_token']
         self.expires_in = content['expires_in']
         self.token_type = content['token_type']
         result = Token(self.access_token, self.token_type, self.expires_in)
         return result
 
-    def auth3leg(self, callback_url=None, scopes=None) -> Token:
+    def auth3leg(self, callback_url: str = None, scopes: str = None) -> Token:
         """
         This method is used to authenticate a user using the 3-legged OAuth flow.
         https://aps.autodesk.com/en/docs/oauth/v2/tutorials/get-3-legged-token/
         :param callback_url: This is the URL-encoded callback URL you want the user redirected to after they grant consent. In this example, that URL is http://localhost:8080/oauth/callback/. Replace the value here with the appropriate URL for your web app. Note that it must match the pattern specified for the callback URL in your app’s registration in the APS developer portal.
         :param scopes: This requests the data:read scope. You can leave this value as it is for the purpose of this example, but in your own app, you should request one or more scopes you actually need. If you need to include multiple scopes, you can include them all as space-delimited items. For example: scope=data:create%20data:read%20data:write includes data:read, data:write, and data:create scopes.
         :return: :class:`Token`:  An instance of the Token class containing the access token, token type, expiration time, and refresh token (if available).
         """
@@ -215,15 +215,15 @@
 
     @staticmethod
     def generate_code_challenge(code_verifier):
         sha256 = hashlib.sha256(code_verifier.encode()).digest()
         code_challenge = base64.urlsafe_b64encode(sha256).rstrip(b'=')
         return code_challenge.decode()
 
-    def refresh_new_token(self, old_refresh_token) -> Token:
+    def refresh_new_token(self, old_refresh_token: str) -> Token:
         Host = "https://developer.api.autodesk.com"
         url = "/authentication/v2/token"
 
         # body
         body = {
             "client_id": self.client_id,
             "client_secret": self.client_secret,
```

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/AuthGoogleColab.py` & `aps-toolkit-0.6.5/src/aps_toolkit/AuthGoogleColab.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .Token import Token
 
 
 class AuthGoogleColab(Auth):
     def __init__(self, client_id: Optional[str] = None, client_secret: Optional[str] = None):
         super().__init__(client_id, client_secret)
 
-    def auth3leg(self, callback_url=None, scopes=None) -> Token:
+    def auth3leg(self, callback_url: str = None, scopes: str = None) -> Token:
         if not scopes:
             scopes = 'data:read data:write data:create data:search bucket:create bucket:read bucket:update bucket:delete code:all'
         if not callback_url:
             # Default callback url
             callback_url = "http://localhost:8080/api/auth/callback"
         auth_url = f"https://developer.api.autodesk.com/authentication/v2/authorize?response_type=code&client_id={self.client_id}&redirect_uri={callback_url}&scope={scopes}"
         auth_url = auth_url.replace(" ", "%20")
@@ -52,15 +52,15 @@
         return Token(
             access_token=response_json['access_token'],
             token_type=response_json['token_type'],
             expires_in=response_json['expires_in'],
             refresh_token=response_json.get('refresh_token')
         )
 
-    def auth3legPkce(self, clientId=None, callback_url=None, scopes=None) -> Token:
+    def auth3legPkce(self, clientId: str = None, callback_url: str = None, scopes: str = None) -> Token:
         """
         This method is used to authenticate a user using the 3-legged OAuth PKCE flow.
         https://aps.autodesk.com/blog/new-application-types
         Parameters:
         clientId (str, optional): The client ID of the application. If not provided, it will use the client ID from the environment variables.
         callback_url (str, optional): The callback URL where the user will be redirected after authentication. If not provided, it defaults to "http://localhost:8080/api/auth/callback".
         scopes (str, optional): The scopes for which the application is requesting access. If not provided, it defaults to 'data:read data:write data:create data:search bucket:create bucket:read bucket:update bucket:delete code:all'.
```

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/BIM360.py` & `aps-toolkit-0.6.5/src/aps_toolkit/BIM360.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,79 @@
     def get_top_folder_project_files(self, hub_id: str, project_id: str):
         data = self.get_top_folders(hub_id, project_id)
         for item in data['data']:
             if item['attributes']['name'] == "Project Files":
                 return item
         return None
 
+    def create_folder(self, project_id, parent_folder_id, folder_name):
+        """
+        Creates a folder in a project. Folders are used to organize items in a project.
+        :param project_id:  :class:`str` The unique identifier of a project.
+        :param parent_folder_id:  :class:`str` The unique identifier of a parent folder.
+        :param folder_name:  :class:`str` The name of the folder.
+        :return:  :class:`dict` all information of new folder
+        """
+        url = f"{self.host}/data/v1/projects/{project_id}/folders"
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        data = {
+            "jsonapi": {
+                "version": "1.0"
+            },
+            "data": {
+                "type": "folders",
+                "attributes": {
+                    "name": folder_name,
+                    "extension": {
+                        "type": "folders:autodesk.bim360:Folder",
+                        "version": "1.0"
+                    }
+                },
+                "relationships": {
+                    "parent": {
+                        "data": {
+                            "type": "folders",
+                            "id": parent_folder_id
+                        }
+                    }
+                }
+            }
+        }
+        response = requests.post(url, headers=headers, json=data)
+        if response.status_code != 201:
+            raise Exception(response.content)
+        return response.json()
+
+    def rename_folder(self, project_id: str, folder_id: str, folder_name: str):
+        """
+        rename a folder in a project. Folders are used to organize items in a project.
+        :param project_id:  :class:`str` The unique identifier of a project.
+        :param folder_id:  :class:`str` The unique identifier of a folder.
+        :return:  :class:`bytes` response content
+        """
+        url = f"{self.host}/data/v1/projects/{project_id}/folders/{folder_id}"
+        headers = {'Authorization': 'Bearer ' + self.token.access_token, 'Content-Type': 'application/vnd.api+json'}
+        data = {
+            "jsonapi": {
+                "version": "1.0"
+            },
+            "data": {
+                "type": "folders",
+                "id": folder_id,
+                "attributes": {
+                    "name": folder_name
+                }
+            }
+
+        }
+        response = requests.patch(url, headers=headers, json=data)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        return response.content
+
     def get_folder_contents(self, project_id: str, folder_id: str):
         """
         Returns a collection of items and folders within a folder. Items represent word documents, fusion design files, drawings, spreadsheets, etc.
         https://aps.autodesk.com/en/docs/data/v2/reference/http/projects-project_id-folders-folder_id-contents-GET/
         :param project_id: :class:`str` The unique identifier of a project.
         :param folder_id: :class:`str` The unique identifier of a folder.
         :return:
@@ -126,14 +191,29 @@
         headers = {'Authorization': 'Bearer ' + self.token.access_token}
         url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}"
         response = requests.get(url, headers=headers)
         if response.status_code != 200:
             raise Exception(response.content)
         return response.json()
 
+    def get_latest_derivative_urn(self, project_id: str, item_id: str):
+        """
+        Get the latest derivative urn of an item by project_id and item_id
+        :param project_id: :class:`str` the unique identifier of a project
+        :param item_id: :class:`str` the unique identifier of an item
+        :return: :class:`str` the latest derivative urn of an item
+        """
+        headers = {'Authorization': 'Bearer ' + self.token.access_token}
+        url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
+        response = requests.get(url, headers=headers)
+        if response.status_code != 200:
+            raise Exception(response.content)
+        item_versions = response.json()
+        return item_versions['data'][0]['relationships']['derivatives']['data']['id']
+
     def batch_report_projects(self, hub_id: str) -> pd.DataFrame:
         """
         Get batch all projects with general information by hub_id
         :param hub_id:  :class:`str` the unique identifier of a hub
         :return:  :class:`pandas.DataFrame` all projects with general information
         """
         df = pd.DataFrame(columns=['project_id', 'project_name', "project_type", 'top_folder_id'])
@@ -155,15 +235,16 @@
         return df
 
     def batch_report_item_versions(self, project_id: str, item_id: str) -> pd.DataFrame:
         """
         Get batch all item versions with general information by project_id and item_id
         :param project_id:  :class:`str` the unique identifier of a project
         :param item_id:  :class:`str` the unique identifier of an item
-        :return:  :class:`pandas.DataFrame` all item versions with general information
+        :return:  :class:`pandas.DataFrame` all item versions with general information containing :
+        item_id,version,derivative_urn,last_modified_time
         """
         # create a dataframe to save data report with columns : item_id,version,derivative_urn,last_modified_time
         df = pd.DataFrame(columns=['item_id', 'version', 'derivative_urn', 'last_modified_time'])
         headers = {'Authorization': 'Bearer ' + self.token.access_token}
         url = f"{self.host}/data/v1/projects/{project_id}/items/{item_id}/versions"
         response = requests.get(url, headers=headers)
         if response.status_code != 200:
@@ -199,15 +280,16 @@
                            is_sub_folder: bool = False) -> pd.DataFrame:
         """
         Get batch all items with general information by project_id and folder_id
         :param project_id:  :class:`str` the unique identifier of a project
         :param folder_id:  :class:`str` the unique identifier of a folder
         :param extension:  :class:`str` the extension of file. e.g: .rvt, .dwg, .pdf
         :param is_sub_folder:  :class:`bool` if True, get all items in sub folders by recursive
-        :return:
+        :return: :class:`pandas.DataFrame` all items with general information containing :
+        project_id, folder_id, item_name, item_id, last_version, derivative_urn, last_modified_time
         """
         df = pd.DataFrame(columns=['project_id', 'folder_id', 'item_name', 'item_id', 'last_version', 'derivative_urn',
                                    'last_modified_time'])
         headers = {'Authorization': 'Bearer ' + self.token.access_token}
         url = f"{self.host}/data/v1/projects/{project_id}/folders/{folder_id}/contents"
         response = requests.get(url, headers=headers)
         if response.status_code != 200:
@@ -545,15 +627,14 @@
         bucket_key = url.split("/").pop(0).split(":").pop()
         object_key = url.split("/").pop()
         s3_url = f"{self.host}/oss/v2/buckets/{bucket_key}/objects/{object_key}/signeds3download"
         response = requests.get(s3_url, headers=headers)
         if response.status_code != 200:
             raise Exception(response.content)
         download_url = response.json()['url']
-        print("Start Download File:", download_url)
         response = requests.get(download_url)
         with open(file_path, 'wb') as file:
             file.write(response.content)
         return file_path
 
     def restore_file_item(self, project_id, item_id, version=1):
         """
```

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/Bucket.py` & `aps-toolkit-0.6.5/src/aps_toolkit/Bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class PublicKey(Enum):
     transient = "transient"
     temporary = "temporary"
     persistent = "persistent"
 
 
 class Bucket:
-    def __init__(self, token: Token, region="US"):
+    def __init__(self, token: Token, region: str = "US"):
         self.token = token
         self.region = region
         self.host = "https://developer.api.autodesk.com/oss/v2/buckets"
 
     def get_all_buckets(self) -> pd.DataFrame:
         """
           Retrieves all the buckets from the Autodesk OSS API.
@@ -156,15 +156,15 @@
         }
         url = f"{self.host}/{bucket_name}/objects/{object_name}"
         response = requests.delete(url, headers=headers)
         if response.status_code != 200:
             raise Exception(response.content)
         return response.content
 
-    def download_object(self, bucket_name: str, object_name: str, file_path: str) -> None:
+    def download_object(self, bucket_name: str, object_name: str, file_path: str) -> bool:
         """
             Downloads an object from a specified bucket in the Autodesk OSS API.
 
             This method sends a GET request to the Autodesk OSS API. It includes an Authorization header with a bearer token for authentication. The bucket name and object name are passed in the URL of the request. If the response status code is not 200, it raises an exception with the response content.
 
             The downloaded content is written to a file at the specified file path.
 
@@ -182,8 +182,8 @@
         url = f"{self.host}/{bucket_name}/objects/{object_name}"
         response = requests.get(url, headers=headers)
         if response.status_code != 200:
             raise Exception(response.content)
         with open(file_path, "wb") as file:
             file.write(response.content)
             file.close()
-        return None
+        return True
```

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/DbReader.py` & `aps-toolkit-0.6.5/src/aps_toolkit/DbReader.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 import os
 import requests
 from .Auth import Auth
 import pandas as pd
 import sqlite3
+from .Token import Token
 
 
 class DbReader:
-    def __init__(self, urn, token=None):
+    def __init__(self, urn: str, token: Token = None):
         self.urn = urn
         if token is None:
             auth = Auth()
             self.token = auth.auth2leg()
         else:
             self.token = token
         self.host = "https://developer.api.autodesk.com"
```

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/Derivative.py` & `aps-toolkit-0.6.5/src/aps_toolkit/Derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/Fragments.py` & `aps-toolkit-0.6.5/src/aps_toolkit/Fragments.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/InputStream.py` & `aps-toolkit-0.6.5/src/aps_toolkit/InputStream.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/ManifestItem.py` & `aps-toolkit-0.6.5/src/aps_toolkit/ManifestItem.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/MaterialProperties.py` & `aps-toolkit-0.6.5/src/aps_toolkit/MaterialProperties.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/Materials.py` & `aps-toolkit-0.6.5/src/aps_toolkit/Materials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/PackFileReader.py` & `aps-toolkit-0.6.5/src/aps_toolkit/PackFileReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/PathInfo.py` & `aps-toolkit-0.6.5/src/aps_toolkit/PathInfo.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/ProDbReaderCad.py` & `aps-toolkit-0.6.5/src/aps_toolkit/ProDbReaderCad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/ProDbReaderNavis.py` & `aps-toolkit-0.6.5/src/aps_toolkit/ProDbReaderNavis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/ProDbReaderRevit.py` & `aps-toolkit-0.6.5/src/aps_toolkit/ProDbReaderRevit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/PropReader.py` & `aps-toolkit-0.6.5/src/aps_toolkit/PropReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/Resource.py` & `aps-toolkit-0.6.5/src/aps_toolkit/Resource.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFContent.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFContent.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFGeometries.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFGeometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFImage.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFImage.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFLines.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFLines.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFManifestType.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFManifestType.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFMaterialGroup.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFMaterialGroup.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFMaterialMap.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFMaterialMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFMaterialMapScale.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFMaterialMapScale.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFMaterials.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFMaterials.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFMesh.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFMesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFMetadata.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFMetadata.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFPoints.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFPoints.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFReader.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFReader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFTransform.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFTransform.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/SVFUVMap.py` & `aps-toolkit-0.6.5/src/aps_toolkit/SVFUVMap.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/Token.py` & `aps-toolkit-0.6.5/src/aps_toolkit/Token.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/Webhooks.py` & `aps-toolkit-0.6.5/src/aps_toolkit/Webhooks.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/__init__.py` & `aps-toolkit-0.6.5/src/aps_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/units/DisplayUnits.py` & `aps-toolkit-0.6.5/src/aps_toolkit/units/DisplayUnits.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit/units/units.json` & `aps-toolkit-0.6.5/src/aps_toolkit/units/units.json`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit.egg-info/PKG-INFO` & `aps-toolkit-0.6.5/src/aps_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aps-toolkit
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Toolkit Autodesk Platform Services for Python
 Home-page: https://github.com/chuongmep/aps-toolkit
 Author: chuong mep
 Author-email: chuongpqvn@gmail.com
 Project-URL: Bug Tracker, https://github.com/chuongmep/aps-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `aps-toolkit-0.6.4/src/aps_toolkit.egg-info/SOURCES.txt` & `aps-toolkit-0.6.5/src/aps_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/context.py` & `aps-toolkit-0.6.5/src/test/context.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_Webhooks.py` & `aps-toolkit-0.6.5/src/test/test_Webhooks.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_auth.py` & `aps-toolkit-0.6.5/src/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_auth_colab.py` & `aps-toolkit-0.6.5/src/test/test_auth_colab.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_bim360.py` & `aps-toolkit-0.6.5/src/test/test_bim360.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         project_files = self.bim360.get_top_folder_project_files(self.hub_id, self.project_id)
         self.assertNotEquals(project_files, 0)
 
     def test_get_item_info(self):
         item_info = self.bim360.get_item_info(self.project_id, self.item_id)
         self.assertNotEquals(item_info, 0)
 
+    def test_get_latest_derivative_urn(self):
+        urn = self.bim360.get_latest_derivative_urn(self.project_id, self.item_id)
+        self.assertNotEquals(urn, "")
+
     def test_get_item_versions(self):
         items = self.bim360.batch_report_items(self.project_id, self.folder_id)
         self.assertNotEquals(len(items), 0)
 
     def test_batch_report_item_versions(self):
         df = self.bim360.batch_report_item_versions(self.project_id, self.item_id)
         self.assertNotEquals(df.empty, True)
@@ -105,7 +109,16 @@
         size_result = os.path.getsize(file_path_result)
         self.assertEqual(size, size_result)
 
     def test_restore_file_item(self):
         item_id = "urn:adsk.wipprod:fs.file:vf.-wv2uodvSgaXmUZ4O0oYkw";
         result = self.bim360.restore_file_item(self.project_id, item_id, 2)
         self.assertNotEquals(result, 0)
+
+    def test_create_folder(self):
+        folder_name = "TestFolder"
+        result = self.bim360.create_folder(self.project_id, self.folder_id, folder_name)
+        self.assertNotEquals(result, 0)
+
+    def test_rename_folder(self):
+        result = self.bim360.rename_folder(self.project_id, self.folder_id, "Test")
+        self.assertNotEquals(result, 0)
```

### Comparing `aps-toolkit-0.6.4/src/test/test_bucket.py` & `aps-toolkit-0.6.5/src/test/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_db_reader.py` & `aps-toolkit-0.6.5/src/test/test_db_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_derivative.py` & `aps-toolkit-0.6.5/src/test/test_derivative.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_fragment.py` & `aps-toolkit-0.6.5/src/test/test_fragment.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_geometries.py` & `aps-toolkit-0.6.5/src/test/test_geometries.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_image.py` & `aps-toolkit-0.6.5/src/test/test_image.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_material.py` & `aps-toolkit-0.6.5/src/test/test_material.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_mesh.py` & `aps-toolkit-0.6.5/src/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_prop_reader.py` & `aps-toolkit-0.6.5/src/test/test_prop_reader.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_prop_reader_cad.py` & `aps-toolkit-0.6.5/src/test/test_prop_reader_cad.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_prop_reader_navis.py` & `aps-toolkit-0.6.5/src/test/test_prop_reader_navis.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_prop_reader_revit.py` & `aps-toolkit-0.6.5/src/test/test_prop_reader_revit.py`

 * *Files identical despite different names*

### Comparing `aps-toolkit-0.6.4/src/test/test_svf_reader.py` & `aps-toolkit-0.6.5/src/test/test_svf_reader.py`

 * *Files identical despite different names*

