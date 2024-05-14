# Comparing `tmp/compas_ifc-0.3.0.tar.gz` & `tmp/compas_ifc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_ifc-0.3.0.tar", last modified: Thu Feb  1 21:24:34 2024, max compression
+gzip compressed data, was "compas_ifc-0.4.0.tar", last modified: Tue May 14 10:30:56 2024, max compression
```

## Comparing `compas_ifc-0.3.0.tar` & `compas_ifc-0.4.0.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-02-01 21:24:34.157028 compas_ifc-0.3.0/
--rw-rw-rw-   0        0        0      167 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/AUTHORS.md
--rw-rw-rw-   0        0        0      953 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1069 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      442 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3478 2024-02-01 21:24:34.157028 compas_ifc-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/README.md
--rw-rw-rw-   0        0        0      703 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       12 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0      227 2024-02-01 21:24:34.157028 compas_ifc-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2056 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-01 21:24:34.140734 compas_ifc-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-01 21:24:34.140734 compas_ifc-0.3.0/src/compas_ifc/
--rw-rw-rw-   0        0        0      943 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/__init__.py
--rw-rw-rw-   0        0        0       38 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/__main__.py
--rw-rw-rw-   0        0        0     3096 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/attributes.py
-drwxrwxrwx   0        0        0        0 2024-02-01 21:24:34.157028 compas_ifc-0.3.0/src/compas_ifc/entities/
--rw-rw-rw-   0        0        0     6697 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/__init__.py
--rw-rw-rw-   0        0        0     2997 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/building.py
--rw-rw-rw-   0        0        0     3373 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/buildingelements.py
--rw-rw-rw-   0        0        0     3152 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/buildingstorey.py
--rw-rw-rw-   0        0        0     1109 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/element.py
--rw-rw-rw-   0        0        0     7843 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/entity.py
--rw-rw-rw-   0        0        0      169 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/geographicelement.py
--rw-rw-rw-   0        0        0     3967 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/objectdefinition.py
--rw-rw-rw-   0        0        0     5012 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/product.py
--rw-rw-rw-   0        0        0     5605 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/project.py
--rw-rw-rw-   0        0        0      791 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/root.py
--rw-rw-rw-   0        0        0     1764 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/site.py
--rw-rw-rw-   0        0        0      789 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/space.py
--rw-rw-rw-   0        0        0      748 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/entities/spatialelement.py
--rw-rw-rw-   0        0        0     1799 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/helpers.py
--rw-rw-rw-   0        0        0     8991 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/model.py
--rw-rw-rw-   0        0        0     5053 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/reader.py
--rw-rw-rw-   0        0        0     7829 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/representation.py
-drwxrwxrwx   0        0        0        0 2024-02-01 21:24:34.157028 compas_ifc-0.3.0/src/compas_ifc/resources/
--rw-rw-rw-   0        0        0     4055 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/resources/__init__.py
--rw-rw-rw-   0        0        0    10375 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/resources/brep.py
--rw-rw-rw-   0        0        0     1444 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/resources/geometricconstraint.py
--rw-rw-rw-   0        0        0     7348 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/resources/geometricmodel.py
--rw-rw-rw-   0        0        0     5330 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/resources/geometry.py
--rw-rw-rw-   0        0        0      883 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/resources/mesh.py
--rw-rw-rw-   0        0        0     1091 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/resources/primities.py
--rw-rw-rw-   0        0        0     1999 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/resources/representation.py
--rw-rw-rw-   0        0        0     3197 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/resources/shapes.py
-drwxrwxrwx   0        0        0        0 2024-02-01 21:24:34.157028 compas_ifc-0.3.0/src/compas_ifc/viewer/
--rw-rw-rw-   0        0        0      387 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/viewer/__init__.py
--rw-rw-rw-   0        0        0     9349 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/viewer/app.py
--rw-rw-rw-   0        0        0     4177 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/viewer/config.json
-drwxrwxrwx   0        0        0        0 2024-02-01 21:24:34.157028 compas_ifc-0.3.0/src/compas_ifc/viewer/objects/
--rw-rw-rw-   0        0        0      305 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/viewer/objects/__init__.py
--rw-rw-rw-   0        0        0      624 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/viewer/objects/entityobject.py
--rw-rw-rw-   0        0        0      240 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/viewer/objects/projectobject.py
--rw-rw-rw-   0        0        0    10728 2024-02-01 21:24:06.000000 compas_ifc-0.3.0/src/compas_ifc/writer.py
-drwxrwxrwx   0        0        0        0 2024-02-01 21:24:34.140734 compas_ifc-0.3.0/src/compas_ifc.egg-info/
--rw-rw-rw-   0        0        0     3478 2024-02-01 21:24:34.000000 compas_ifc-0.3.0/src/compas_ifc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1650 2024-02-01 21:24:34.000000 compas_ifc-0.3.0/src/compas_ifc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-01 21:24:34.000000 compas_ifc-0.3.0/src/compas_ifc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-01 21:24:34.000000 compas_ifc-0.3.0/src/compas_ifc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2024-02-01 21:24:34.000000 compas_ifc-0.3.0/src/compas_ifc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-01 21:24:34.000000 compas_ifc-0.3.0/src/compas_ifc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/
+-rw-rw-rw-   0        0        0      167 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     1265 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1069 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      442 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5418 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/README.md
+-rw-rw-rw-   0        0        0     3919 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      126 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       18 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.744194 compas_ifc-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.759827 compas_ifc-0.4.0/src/compas_ifc/
+-rw-rw-rw-   0        0        0      993 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/__init__.py
+-rw-rw-rw-   0        0        0       38 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/__main__.py
+-rw-rw-rw-   0        0        0     3096 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/attributes.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.759827 compas_ifc-0.4.0/src/compas_ifc/brep/
+-rw-rw-rw-   0        0        0      445 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/brep/__init__.py
+-rw-rw-rw-   0        0        0      787 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/brep/tessellatedbrep.py
+-rw-rw-rw-   0        0        0     1789 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/brep/tessellatedbrepobject.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.759827 compas_ifc-0.4.0/src/compas_ifc/entities/
+-rw-rw-rw-   0        0        0     6698 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/__init__.py
+-rw-rw-rw-   0        0        0     2997 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/building.py
+-rw-rw-rw-   0        0        0     3341 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/buildingelements.py
+-rw-rw-rw-   0        0        0     3152 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/buildingstorey.py
+-rw-rw-rw-   0        0        0     1109 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/element.py
+-rw-rw-rw-   0        0        0     7962 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/entity.py
+-rw-rw-rw-   0        0        0      169 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/geographicelement.py
+-rw-rw-rw-   0        0        0     3943 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/objectdefinition.py
+-rw-rw-rw-   0        0        0     6956 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/product.py
+-rw-rw-rw-   0        0        0     5607 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/project.py
+-rw-rw-rw-   0        0        0      791 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/root.py
+-rw-rw-rw-   0        0        0     1764 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/site.py
+-rw-rw-rw-   0        0        0      789 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/space.py
+-rw-rw-rw-   0        0        0      748 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/entities/spatialelement.py
+-rw-rw-rw-   0        0        0     1799 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/helpers.py
+-rw-rw-rw-   0        0        0     9510 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/model.py
+-rw-rw-rw-   0        0        0     8305 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/reader.py
+-rw-rw-rw-   0        0        0     9693 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/representation.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/src/compas_ifc/resources/
+-rw-rw-rw-   0        0        0     4270 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/__init__.py
+-rw-rw-rw-   0        0        0    10041 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/brep.py
+-rw-rw-rw-   0        0        0     2099 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/geometricconstraint.py
+-rw-rw-rw-   0        0        0     7697 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/geometricmodel.py
+-rw-rw-rw-   0        0        0     5366 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/geometry.py
+-rw-rw-rw-   0        0        0     1729 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/mesh.py
+-rw-rw-rw-   0        0        0     1049 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/primities.py
+-rw-rw-rw-   0        0        0     2401 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/representation.py
+-rw-rw-rw-   0        0        0     3342 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/resources/shapes.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/src/compas_ifc/viewer/
+-rw-rw-rw-   0        0        0      387 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/__init__.py
+-rw-rw-rw-   0        0        0     9349 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/app.py
+-rw-rw-rw-   0        0        0     4177 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/config.json
+drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/src/compas_ifc/viewer/objects/
+-rw-rw-rw-   0        0        0      305 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/objects/__init__.py
+-rw-rw-rw-   0        0        0      624 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/objects/entityobject.py
+-rw-rw-rw-   0        0        0      240 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/viewer/objects/projectobject.py
+-rw-rw-rw-   0        0        0    13747 2024-05-14 10:30:27.000000 compas_ifc-0.4.0/src/compas_ifc/writer.py
+drwxrwxrwx   0        0        0        0 2024-05-14 10:30:56.775451 compas_ifc-0.4.0/src/compas_ifc.egg-info/
+-rw-rw-rw-   0        0        0     5418 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      139 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 10:30:56.000000 compas_ifc-0.4.0/src/compas_ifc.egg-info/top_level.txt
```

### Comparing `compas_ifc-0.3.0/CHANGELOG.md` & `compas_ifc-0.4.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0] 2024-05-14
+
+### Added
+
+* Added support to export to `IFC2x3`.
+* Added support pre-load geometries using `multi-processing`.
+
+### Changed
+
+* Updated workflow to not use `conda` anymore.
+* Updated `Reader` to re-enable lazy loading.
+* Update repo to use `pyproject.toml`.
+
+### Removed
+
+
 ## [0.3.0] 2024-02-01
 
 ### Added
 
 * Added `entity_opening_geometry`.
 * Added `entity_body_with_opening_geometry`.
 * Added `opening` attribute to `Product`.
```

### Comparing `compas_ifc-0.3.0/LICENSE` & `compas_ifc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/README.md` & `compas_ifc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/attributes.py` & `compas_ifc-0.4.0/src/compas_ifc/attributes.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/__init__.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 * a service that combine the above features.
 
 These "associations" are called "classifications".
 
 .. code-block:: python
 
     for association in entity.HasAssociations:
-        if association.is_a('IfcRelAssociatesClassification'):
+        if association.is_a("IfcRelAssociatesClassification"):
             ...
 
 Material Associations
 ---------------------
 
 See also :ifc:`material-association`.
 
@@ -62,22 +62,23 @@
 Materials can have representations for fill styles indicating colors, tiles, and hatch patterns for 2D rendering.
 Materials can have properties such as density, elasticity, thermal resistance, and others as defined in this specification.
 Materials can also be classified according to a referenced industry standard.
 
 .. code-block:: python
 
     for association in entity.HasAssociations:
-        if association.is_a('IfcRelAssociatesMaterial'):
+        if association.is_a("IfcRelAssociatesMaterial"):
             ...
 
 Object Composition
 ==================
 
 Objects may be composed into parts to indicate levels of detail, such as a building having multiple storeys, a framed wall having studs, or a task having subtasks.
-Composition may form a hierarchy of multiple levels, where an object must have single parent, or if a top-level object then declared within the single project or a project library.
+Composition may form a hierarchy of multiple levels, where an object must have single parent,
+or if a top-level object then declared within the single project or a project library.
 
 Element Composition
 -------------------
 
 See also :ifc:`element-composition`.
 
 Provision of an aggregation structure where the element is part of another element representing the composite.
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/building.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/building.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/buildingelements.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/buildingelements.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,15 @@
         return self._composite_opening
 
     @property
     def composite_body_with_opening(self):
         from compas_ifc.representation import entity_body_with_opening_geometry
 
         if not self._composite_body_with_opening:
-            self._composite_body_with_opening = entity_body_with_opening_geometry(
-                entity=self, bodies=self.composite_body, voids=self.composite_opening
-            )
+            self._composite_body_with_opening = entity_body_with_opening_geometry(entity=self, bodies=self.composite_body, voids=self.composite_opening)
         return self._composite_body_with_opening
 
     @composite_body_with_opening.setter
     def composite_body_with_opening(self, value):
         self._composite_body_with_opening = value
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/buildingstorey.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/buildingstorey.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/element.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/element.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/entity.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict
 from typing import Union
 
 # from typing import Optional
-
 import ifcopenshell
 import ifcopenshell.util.element
 import ifcopenshell.util.pset
 
 
 class Entity:
     """
@@ -49,14 +48,20 @@
     @property
     def declaration(self):
         if not self._declaration and self.model.schema:
             self._declaration = self.model.schema.declaration_by_name(self.ifc_type)
         return self._declaration
 
     @property
+    def id(self):
+        if self._entity:
+            return self._entity.id()
+        return None
+
+    @property
     def ifc_type(self):
         if self._entity:
             self._ifc_type = self._entity.is_a()
         else:
             self._ifc_type = "Ifc" + type(self).__name__
         return self._ifc_type
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/objectdefinition.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/objectdefinition.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,15 @@
 
     def is_decomposed_by(self):
         """Return the relation that this element is decomposed by."""
         return [self.model.reader.get_entity(rel) for rel in self._entity.IsDecomposedBy]
 
     @property
     def children(self):
-        children = [
-            entity for entity in self.model.get_entities_by_type("IfcObjectDefinition") if entity.parent == self
-        ]
+        children = [entity for entity in self.model.get_entities_by_type("IfcObjectDefinition") if entity.parent == self]
         for entity in self.model._new_entities:
             if entity.parent == self and entity not in children:
                 children.append(entity)
         return children
 
     def traverse(self, recursive: bool = True):
         """Traverse children of this element.
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/product.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/product.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,24 +13,38 @@
     ----------
     axis : List[:class:`compas.geometry.Line`]
         The axis representation of the product. Converted to list of COMPAS lines.
     box : :class:`compas.geometry.Box`
         The box representation of the product. Converted to COMPAS box.
     body : List[:class:`compas_occ.geometry.Shape`]
         The body representation of the product. Converted to list of OCC shapes (BRep).
+    body_with_opening : List[:class:`compas_occ.geometry.Shape`]
+        The body representation of the product including openings. Converted to list of OCC shapes (BRep).
+    opening : List[:class:`compas_occ`]
+        The opening representation of the product. Converted to list of OCC shapes (BRep).
+    transformation : :class:`compas.geometry.Transformation`
+        The transformation of the product, Calculated from the stack of transformations of the product's parent entities. Read-only.
+    style : dict
+        The style of the product. Converted to dictionary.
+    frame : :class:`compas.geometry.Frame`
+        The frame of the product. Converted to COMPAS frame.
+
 
     """
 
     def __init__(self, entity, model) -> None:
         super().__init__(entity, model)
         self._axis = None
         self._box = None
         self._body = None
         self._opening = None
         self._body_with_opening = None
+        self._transformation = None
+        self._style = None
+        self._frame = None
 
     def classifications(self) -> List[Dict[str, str]]:
         """
         External sources of information associated with this product.
         The source of information can be:
 
         * a classification system;
@@ -113,37 +127,71 @@
         return self._box
 
     @property
     def body(self):
         from compas_ifc.representation import entity_body_geometry
 
         if not self._body:
-            self._body = entity_body_geometry(self)
+            self._body = entity_body_geometry(self, use_occ=self.model.reader.use_occ)
         return self._body
 
     @body.setter
     def body(self, value):
         self._body = value
 
     @property
     def opening(self):
         from compas_ifc.representation import entity_opening_geometry
 
         if not self._opening:
-            self._opening = entity_opening_geometry(self)
+            self._opening = entity_opening_geometry(self, use_occ=self.model.reader.use_occ)
         return self._opening
 
     @opening.setter
     def opening(self, value):
         self._opening = value
 
     @property
     def body_with_opening(self):
         from compas_ifc.representation import entity_body_with_opening_geometry
 
         if not self._body_with_opening:
-            self._body_with_opening = entity_body_with_opening_geometry(self, self.body, self.opening)
+            cached_geometry = self.model.reader.get_preloaded_geometry(self)
+            if cached_geometry:
+                self._body_with_opening = cached_geometry
+            else:
+                # TODO: double check if this is still triggered with preloaded geometry
+                # raise
+                self._body_with_opening = entity_body_with_opening_geometry(self, use_occ=self.model.reader.use_occ)
+
         return self._body_with_opening
 
     @body_with_opening.setter
     def body_with_opening(self, value):
         self._body_with_opening = value
+
+    @property
+    def transformation(self):
+        from compas_ifc.representation import entity_transformation
+
+        if not self._transformation:
+            self._transformation = entity_transformation(self)
+        return self._transformation
+
+    @property
+    def frame(self):
+        from compas_ifc.representation import entity_frame
+
+        if not self._frame and self._entity:
+            self._frame = entity_frame(self)
+        return self._frame
+
+    @frame.setter
+    def frame(self, value):
+        self._frame = value
+
+    @property
+    def style(self):
+        if not self._style:
+            self._style = self.model.reader.get_preloaded_style(self)
+        # TODO: handle non-preloaded situation
+        return self._style
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/project.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # from typing import Iterator
 from typing import Dict
 from typing import List
 
 from compas.geometry import Frame
 from compas.geometry import Vector
+
 from compas_ifc.entities.objectdefinition import ObjectDefinition
 from compas_ifc.entities.site import Building
 from compas_ifc.entities.site import Site
 from compas_ifc.resources import IfcAxis2Placement3D_to_frame
 
 
 class Project(ObjectDefinition):
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/root.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/root.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/site.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/site.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/space.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/space.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/entities/spatialelement.py` & `compas_ifc-0.4.0/src/compas_ifc/entities/spatialelement.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/helpers.py` & `compas_ifc-0.4.0/src/compas_ifc/helpers.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/model.py` & `compas_ifc-0.4.0/src/compas_ifc/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import List
 
-from compas_ifc.entities.element import Element
+import ifcopenshell
+
 from compas_ifc.entities.building import Building
 from compas_ifc.entities.buildingelements import BuildingElement
-from compas_ifc.entities.geographicelement import GeographicElement
 from compas_ifc.entities.buildingelements import BuildingElementProxy
 from compas_ifc.entities.buildingstorey import BuildingStorey
-from compas_ifc.entities.objectdefinition import ObjectDefinition
+from compas_ifc.entities.element import Element
 from compas_ifc.entities.entity import Entity
+from compas_ifc.entities.geographicelement import GeographicElement
+from compas_ifc.entities.objectdefinition import ObjectDefinition
+from compas_ifc.entities.product import Product
 from compas_ifc.entities.project import Project
 from compas_ifc.entities.site import Site
 
 from .reader import IFCReader
 from .writer import IFCWriter
 
 
@@ -54,30 +57,34 @@
         All the building elements contained in the model.
         In a correctly formed hierarchical model, building elements are part of a building, building storey, or space.
         If that is not the case, they are also accessible here.
 
 
     """
 
-    def __init__(self, filepath: str = None, entity_types: dict = None) -> None:
-        self.reader = IFCReader(model=self, entity_types=entity_types)
+    def __init__(self, filepath: str = None, entity_types: dict = None, use_occ=False, schema=None, load_geometries=True) -> None:
+        self.reader = IFCReader(model=self, entity_types=entity_types, use_occ=use_occ)
         self.writer = IFCWriter(model=self)
         self._new_entities = set()
         self._projects = None
         self._sites = None
         self._buildings = None
         self._building_storeys = None
         self._elements = None
         self._building_elements = None
         self._geographic_elements = None
+        self._schema = None
+        if schema:
+            self._schema = ifcopenshell.ifcopenshell_wrapper.schema_by_name(schema)
+
         if filepath:
-            self.open(filepath)
+            self.open(filepath, load_geometries=load_geometries)
 
-    def open(self, filepath: str) -> None:
-        self.reader.open(filepath)
+    def open(self, filepath: str, load_geometries=True) -> None:
+        self.reader.open(filepath, load_geometries=load_geometries)
 
     def save(self, filepath: str) -> None:
         self.writer.save(filepath)
 
     def export(self, entities, filepath: str) -> None:
         self.writer.export(entities, filepath)
 
@@ -120,15 +127,15 @@
         print("Number of sites: {}".format(len(self.sites)))
         print("Number of buildings: {}".format(len(self.buildings)))
         print("Number of building elements: {}".format(len(self.building_elements)))
         print("=" * 80)
 
     @property
     def schema(self) -> str:
-        return self.reader._schema
+        return self._schema or self.reader._schema
 
     @property
     def project(self) -> Project:
         if self.projects:
             return self.projects[0]
 
     @property
@@ -169,15 +176,15 @@
 
     @property
     def geographic_elements(self) -> List[GeographicElement]:
         if self._geographic_elements is None:
             self._geographic_elements = self.get_entities_by_type("IfcGeographicElement")
         return self._geographic_elements
 
-    def create(self, cls, attributes, parent=None):
+    def create(self, cls, attributes, parent=None, frame=None):
         """Create an entity and add it to the model.
 
         Parameters
         ----------
         cls : :class:`compas_ifc.entities.Entity`
             The type of entity to create.
         attributes : dict
@@ -188,28 +195,30 @@
         Returns
         -------
         :class:`compas_ifc.entities.Entity`
             The created entity.
         """
         entity = cls(None, self)
         entity.set_attributes(attributes)
+        if isinstance(entity, Product) and frame:
+            entity.frame = frame
         if parent:
             if isinstance(entity, ObjectDefinition):
                 entity.parent = parent
             else:
                 print(hasattr(entity, "parent"))
                 raise ValueError(f"{entity} cannot be assigned a parent.")
         self._new_entities.add(entity)
 
         if cls == Project:
             self._projects = [entity]
 
         return entity
 
-    def insert(self, geometry, parent=None, name=None, description=None, cls=None) -> BuildingElementProxy:
+    def insert(self, geometry, parent=None, name=None, description=None, cls=None, frame=None) -> BuildingElementProxy:
         """Insert a geometry into the model. The geometry will be wrapped in a building element proxy.
 
         Parameters
         ----------
         geometry : :class:`compas.geometry.Geometry` or :class:`compas.datastructures.Mesh`
             The geometry to be inserted.
         parent : :class:`compas_ifc.entities.Entity`
@@ -225,11 +234,12 @@
             The building element proxy wrapping the geometry.
         """
         if cls is None:
             cls = BuildingElementProxy
         element = cls(None, self)
         element.body = geometry
         element.parent = parent
+        element.frame = frame
         element["Name"] = name
         element["Description"] = description
         self._new_entities.add(element)
         return element
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/representation.py` & `compas_ifc-0.4.0/src/compas_ifc/representation.py`

 * *Files 19% similar despite different names*

```diff
@@ -37,28 +37,31 @@
 
 """
 
 from functools import reduce
 from operator import mul
 from typing import List
 
+from compas.geometry import Box
+from compas.geometry import Scale
+from compas.geometry import Transformation
 from compas_occ.brep import OCCBrep
 from OCC.Core.BRep import BRep_Builder
 from OCC.Core.TopoDS import TopoDS_Compound
 
-from compas.geometry import Box
-from compas.geometry import Scale
-from compas.geometry import Transformation
+from compas_ifc.brep import TessellatedBrep
 from compas_ifc.entities.entity import Entity
 from compas_ifc.resources import IfcAxis2Placement3D_to_frame
 from compas_ifc.resources import IfcBoundingBox_to_box
 from compas_ifc.resources import IfcCartesianTransformationOperator3D_to_frame
 from compas_ifc.resources import IfcIndexedPolyCurve_to_lines
+from compas_ifc.resources import IfcLocalPlacement_to_frame
 from compas_ifc.resources import IfcLocalPlacement_to_transformation
 from compas_ifc.resources import IfcShape_to_brep
+from compas_ifc.resources import IfcShape_to_tessellatedbrep
 
 
 # this does not belong here
 # but rather in the representations module
 def IfcMappedItem_to_transformation(item) -> Transformation:
     """
     Convert an IFC MappedItem to a COMPAS transformation.
@@ -72,15 +75,38 @@
     stack.append(source_frame)
     stack.append(target_frame)
 
     matrices = [Transformation.from_frame(f) for f in stack]
     return reduce(mul, matrices[::-1])
 
 
-def entity_body_geometry(entity: Entity, context="Model"):
+def entity_transformation(entity: Entity):
+    """
+    Construct the transformation of an entity.
+    """
+    return _entity_transformation(entity._entity, scale=entity.model.project.length_scale)
+
+
+def _entity_transformation(_entity, scale=1.0):
+    if _entity.ObjectPlacement:
+        scaled_placement = IfcLocalPlacement_to_transformation(_entity.ObjectPlacement, scale=scale)
+    else:
+        scaled_placement = Scale.from_factors([scale, scale, scale])
+
+    return scaled_placement
+
+
+def entity_frame(entity: Entity):
+    """
+    Construct the frame of an entity.
+    """
+    return IfcLocalPlacement_to_frame(entity._entity.ObjectPlacement)
+
+
+def entity_body_geometry(entity: Entity, context="Model", use_occ=False, apply_transformation=True):
     """
     Construct the body geometry representations of an entity.
 
     References
     ----------
     .. [1] :ifc:`body-geometry`
 
@@ -93,82 +119,104 @@
             if temp.RepresentationIdentifier == "Body":
                 representation = temp
                 break
 
     if not representation:
         return bodies
 
-    scale = entity.model.project.length_scale
-    if entity._entity.ObjectPlacement:
-        scaled_placement = IfcLocalPlacement_to_transformation(entity._entity.ObjectPlacement, scale=scale)
-    else:
-        scaled_placement = Transformation()
     if representation.ContextOfItems.ContextType == context:
         for item in representation.Items:
-            brep = IfcShape_to_brep(item)
-            brep.transform(scaled_placement)
-            bodies.append(brep)
+            if use_occ:
+                brep = IfcShape_to_brep(item)
+                bodies.append(brep)
+            else:
+                tessellatedbrep = IfcShape_to_tessellatedbrep(item)
+                bodies.append(tessellatedbrep)
+
+    if apply_transformation:
+        transformation = entity_transformation(entity)
+        for body in bodies:
+            body.transform(transformation)
 
     return bodies
 
 
-def entity_opening_geometry(entity: Entity):
+def entity_opening_geometry(entity: Entity, use_occ=False, apply_transformation=True):
     """
     Construct the opening geometry representations of an entity.
     """
 
     voids = []
     if hasattr(entity._entity, "HasOpenings"):
-        scale = entity.model.project.length_scale
         for opening in entity._entity.HasOpenings:
             element = opening.RelatedOpeningElement
-            if element.ObjectPlacement:
-                scaled_placement = IfcLocalPlacement_to_transformation(element.ObjectPlacement, scale=scale)
-            else:
-                scaled_placement = Transformation()
+
+            if apply_transformation:
+                transformation = _entity_transformation(element, entity.model.project.length_scale)
+
             for representation in element.Representation.Representations:
                 for item in representation.Items:
-                    brep = IfcShape_to_brep(item)
-                    brep.transform(scaled_placement)
-                    voids.append(brep)
+                    if use_occ:
+                        brep = IfcShape_to_brep(item)
+                        if apply_transformation:
+                            brep.transform(transformation)
+                        voids.append(brep)
+                    else:
+                        tessellatedbrep = IfcShape_to_tessellatedbrep(item)
+                        if apply_transformation:
+                            tessellatedbrep.transform(transformation)
+                        voids.append(tessellatedbrep)
 
     return voids
 
 
-def entity_body_with_opening_geometry(entity: Entity = None, bodies=None, voids=None, context="Model"):
+def entity_body_with_opening_geometry(entity: Entity = None, bodies=None, voids=None, context="Model", use_occ=False):
     """
     Construct the body geometry representations of an entity.
 
     References
     ----------
     .. [1] :ifc:`body-geometry`
 
     """
-    bodies = bodies or entity_body_geometry(entity, context=context)
-    voids = voids or entity_opening_geometry(entity)
+    bodies = bodies or entity_body_geometry(entity, context=context, use_occ=use_occ, apply_transformation=True)
+    voids = voids or entity_opening_geometry(entity, use_occ=use_occ, apply_transformation=True)
 
     if not voids:
         return bodies
 
-    compound = TopoDS_Compound()
-    builder = BRep_Builder()
-    builder.MakeCompound(compound)
-    for brep in voids:
-        builder.Add(compound, brep.occ_shape)
-    B = OCCBrep.from_shape(compound)
-
-    shapes = []
-    for A in bodies:
-        try:
-            C: OCCBrep = A - B
-            C.make_solid()
+    if use_occ:
+        print("Using OCC for boolean operations.")
+        compound = TopoDS_Compound()
+        builder = BRep_Builder()
+        builder.MakeCompound(compound)
+        for brep in voids:
+            builder.Add(compound, brep.occ_shape)
+        B = OCCBrep.from_shape(compound)
+
+        shapes = []
+        for A in bodies:
+            try:
+                C: OCCBrep = A - B
+                C.make_solid()
+                shapes.append(C)
+            except Exception:
+                shapes.append(A)
+                print("Warning: Failed to subtract voids from body.")
+    else:
+        print("Using CGAL for boolean operations.")
+        from compas_cgal.booleans import boolean_difference
+
+        shapes = []
+        for A in bodies:
+            C = A
+            for B in voids:
+                vertices, faces = boolean_difference(C.to_vertices_and_faces(), B.to_vertices_and_faces())
+                C = TessellatedBrep(vertices=vertices, faces=faces)
             shapes.append(C)
-        except Exception:
-            shapes.append(A)
-            print("Warning: Failed to subtract voids from body.")
 
     return shapes
 
 
 def entity_box_geometry(entity, context="Model") -> List[Box]:
     """
     Construct the box geometry representations of an entity.
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/resources/__init__.py` & `compas_ifc-0.4.0/src/compas_ifc/resources/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 from .geometry import IfcLine_to_line  # noqa: F401
 from .geometry import IfcPlane_to_plane  # noqa: F401
 from .geometry import IfcAxis2Placement3D_to_frame  # noqa: F401
 from .geometry import IfcCartesianTransformationOperator3D_to_frame  # noqa: F401
 
 from .geometricconstraint import IfcGridPlacement_to_transformation  # noqa: F401
 from .geometricconstraint import IfcLocalPlacement_to_transformation  # noqa: F401
+from .geometricconstraint import IfcLocalPlacement_to_frame  # noqa: F401
 
 from .geometricmodel import IfcAdvancedBrep_to_brep  # noqa: F401
 from .geometricmodel import IfcAdvancedBrepWithVoids_to_brep  # noqa: F401
 from .geometricmodel import IfcBlock_to_box  # noqa: F401
 from .geometricmodel import IfcBooleanClippingResult_to_brep  # noqa: F401
 from .geometricmodel import IfcBoundingBox_to_box  # noqa: F401
 from .geometricmodel import IfcIndexedPolyCurve_to_lines  # noqa: F401
@@ -106,10 +107,13 @@
 from .geometricmodel import IfcFacetedBrepWithVoids_to_brep  # noqa: F401
 from .geometricmodel import IfcIndexedPolygonalFaceSet_to_brep  # noqa: F401
 from .geometricmodel import IfcPolygonalBoundedHalfSpace_to_brep  # noqa: F401
 from .geometricmodel import IfcPolygonalFaceSet_to_brep  # noqa: F401
 from .geometricmodel import IfcTessellatedFaceSet_to_brep  # noqa: F401
 from .geometricmodel import IfcTriangulatedFaceSet_to_brep  # noqa: F401
 from .geometricmodel import IfcShape_to_brep  # noqa: F401
+from .geometricmodel import IfcShape_to_tessellatedbrep  # noqa: F401
+
+from .shapes import frame_to_ifc_axis2_placement_3d  # noqa: F401
 
 # from .geometricmodel import IfcBoxedHalfSpace
 # from .geometricmodel import IfcCartesianPointList
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/resources/brep.py` & `compas_ifc-0.4.0/src/compas_ifc/resources/brep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
+from typing import List
+
 import ifcopenshell
 import numpy as np
+from compas.tolerance import TOL
 
-from compas.utilities import geometric_key
-from compas_occ.brep import OCCBrep
-from typing import List
-
-from .primities import point_to_ifc_cartesian_point
-from .primities import occ_plane_to_frame
 from .primities import frame_to_ifc_plane
-
+from .primities import occ_plane_to_frame
+from .primities import point_to_ifc_cartesian_point
 from .shapes import occ_cylinder_to_ifc_cylindrical_surface
 
 
 def calculate_knots_and_multiplicities(knot_sequence):
     knots = [knot_sequence[0]]
     multiplicities = [1]
 
@@ -22,32 +20,32 @@
             multiplicities.append(1)
         else:
             multiplicities[-1] += 1
 
     return knots, multiplicities
 
 
-def brep_to_ifc_advanced_brep(file: ifcopenshell.file, brep: OCCBrep) -> List[ifcopenshell.entity_instance]:
+def brep_to_ifc_advanced_brep(file: ifcopenshell.file, brep) -> List[ifcopenshell.entity_instance]:
     brep.fix()
     brep.sew()
     brep.make_solid()
 
     points = {}
     curves = {}
     lines = {}
 
     def get_ifc_point(point):
-        key = geometric_key(point)
+        key = TOL.geometric_key(point)
         if key in points:
             return points[key]
         points[key] = point_to_ifc_cartesian_point(file, point)
         return points[key]
 
     def get_ifc_line(edge):
-        line_key = geometric_key(edge.first_vertex.point) + "-" + geometric_key(edge.last_vertex.point)
+        line_key = TOL.geometric_key(edge.first_vertex.point) + "-" + TOL.geometric_key(edge.last_vertex.point)
         return lines.get(line_key)
 
     def get_ifc_curve(edge):
         curve = edge.nurbscurve
         for occ_curve in curves:
             if occ_curve.IsEqual(curve.occ_curve, 1e-6):
                 return curves[occ_curve]
@@ -117,15 +115,15 @@
                 "IfcEdgeCurve",
                 EdgeStart=start_vertex,
                 EdgeEnd=end_vertex,
                 EdgeGeometry=IfcPolyLine,
                 SameSense=True,
             )
 
-            line_key = geometric_key(edge.first_vertex.point) + "-" + geometric_key(edge.last_vertex.point)
+            line_key = TOL.geometric_key(edge.first_vertex.point) + "-" + TOL.geometric_key(edge.last_vertex.point)
             lines[line_key] = IfcEdgeCurve
 
         else:
             raise NotImplementedError("Only BSpline and Line edges are supported")
 
     for solid in brep.solids:
         for shell in solid.shells:
@@ -146,17 +144,15 @@
                             IfcEdgeCurve = get_ifc_line(edge)
                         else:
                             raise NotImplementedError("Only BSpline and Line edges are supported")
 
                         if not IfcEdgeCurve:
                             raise ValueError("Edge not found")
 
-                        ifc_oriented_edge = file.create_entity(
-                            "IFCORIENTEDEDGE", EdgeElement=IfcEdgeCurve, Orientation=oriented
-                        )
+                        ifc_oriented_edge = file.create_entity("IFCORIENTEDEDGE", EdgeElement=IfcEdgeCurve, Orientation=oriented)
                         ifc_oriented_edges.append(ifc_oriented_edge)
 
                     edge_loop = file.create_entity("IfcEdgeLoop", ifc_oriented_edges)
                     if is_outer:
                         ifc_face_bound = file.create_entity("IfcFaceOuterBound", edge_loop, True)
                         is_outer = False
                     else:
@@ -164,87 +160,77 @@
                     face_bounds.append(ifc_face_bound)
 
                 same_sense = face.orientation == 0
                 if face.is_plane:
                     occ_plane = face.occ_adaptor.Plane()
                     frame = occ_plane_to_frame(occ_plane)
                     ifc_plane = frame_to_ifc_plane(file, frame)
-                    IfcAdvancedFace = file.create_entity(
-                        "IfcAdvancedFace", face_bounds, ifc_plane, SameSense=same_sense
-                    )
+                    IfcAdvancedFace = file.create_entity("IfcAdvancedFace", face_bounds, ifc_plane, SameSense=same_sense)
                 elif face.is_cylinder:
                     cylinder = face.occ_adaptor.Cylinder()
                     IfcCylindricalSurface = occ_cylinder_to_ifc_cylindrical_surface(file, cylinder)
-                    IfcAdvancedFace = file.create_entity(
-                        "IfcAdvancedFace", face_bounds, IfcCylindricalSurface, SameSense=same_sense
-                    )
+                    IfcAdvancedFace = file.create_entity("IfcAdvancedFace", face_bounds, IfcCylindricalSurface, SameSense=same_sense)
                 else:
                     control_points = np.array(face.nurbssurface.points.points, dtype=float)
                     control_points = control_points.swapaxes(0, 1)
                     ifc_control_points = []
 
-                    u_knots, u_mults = calculate_knots_and_multiplicities(
-                        list(face.nurbssurface.occ_surface.UKnotSequence())
-                    )
-                    v_knots, v_mults = calculate_knots_and_multiplicities(
-                        list(face.nurbssurface.occ_surface.VKnotSequence())
-                    )
+                    u_knots, u_mults = calculate_knots_and_multiplicities(list(face.nurbssurface.occ_surface.UKnotSequence()))
+                    v_knots, v_mults = calculate_knots_and_multiplicities(list(face.nurbssurface.occ_surface.VKnotSequence()))
 
                     for row in control_points:
                         ifc_row = []
                         for point in row:
                             ifc_row.append(get_ifc_point(point))
                         ifc_control_points.append(ifc_row)
 
-                    if face.nurbssurface.is_u_periodic:
+                    if face.nurbssurface.is_periodic_u:
                         new_row = []
                         for point in control_points[0]:
                             new_row.append(get_ifc_point(point))
                         ifc_control_points.append(new_row)
 
-                    if face.nurbssurface.is_v_periodic:
+                    if face.nurbssurface.is_periodic_v:
                         for i, row in enumerate(ifc_control_points):
                             row.append(get_ifc_point(control_points[i % len(control_points)][0]))
 
                     weights = face.nurbssurface.weights
                     weights = np.array(weights, dtype=float)
                     weights = weights.swapaxes(0, 1)
 
                     ifc_weights = []
                     for row in weights:
                         ifc_row = []
                         for weight in row:
                             ifc_row.append(float(weight))
                         ifc_weights.append(ifc_row)
 
-                    if face.nurbssurface.is_u_periodic:
+                    if face.nurbssurface.is_periodic_u:
                         ifc_weights.append(ifc_weights[0])
-                    if face.nurbssurface.is_v_periodic:
+                    if face.nurbssurface.is_periodic_v:
                         for i, row in enumerate(ifc_weights):
                             row.append(row[0])
 
                     IfcBSplineSurfaceWithKnots = file.create_entity(
                         "IfcRationalBSplineSurfaceWithKnots",
-                        UDegree=face.nurbssurface.u_degree,
-                        VDegree=face.nurbssurface.v_degree,
+                        UDegree=face.nurbssurface.degree_u,
+                        VDegree=face.nurbssurface.degree_v,
                         ControlPointsList=ifc_control_points,
                         SurfaceForm="UNSPECIFIED",
-                        UClosed=face.nurbssurface.is_u_periodic,
-                        VClosed=face.nurbssurface.is_v_periodic,
+                        UClosed=face.nurbssurface.is_periodic_u,
+                        VClosed=face.nurbssurface.is_periodic_v,
                         SelfIntersect=False,  # Seems no way to get this from OCC
                         UMultiplicities=u_mults,
                         VMultiplicities=v_mults,
                         UKnots=u_knots,
                         VKnots=v_knots,
                         WeightsData=ifc_weights,
                     )
 
-                    IfcAdvancedFace = file.create_entity(
-                        "IfcAdvancedFace", face_bounds, IfcBSplineSurfaceWithKnots, SameSense=same_sense
-                    )
+                    IfcAdvancedFace = file.create_entity("IfcAdvancedFace", face_bounds, IfcBSplineSurfaceWithKnots, SameSense=same_sense)
 
                 ifc_faces.append(IfcAdvancedFace)
 
             ifc_shell = file.create_entity("IFCCLOSEDSHELL", ifc_faces)
 
         ifc_brep = file.create_entity("IFCADVANCEDBREP", ifc_shell)
         ifc_breps.append(ifc_brep)
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/resources/geometricconstraint.py` & `compas_ifc-0.4.0/src/compas_ifc/resources/geometricconstraint.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,9 +37,31 @@
 
         placement = placement.PlacementRelTo
 
     matrices = [Transformation.from_frame(f) for f in stack]
     return reduce(mul, matrices[::-1])
 
 
+def IfcLocalPlacement_to_frame(placement) -> Frame:
+    """
+    Convert an IFC LocalPlacement to a COMPAS frame.
+    """
+
+    Location = placement.RelativePlacement.Location
+    Axis = placement.RelativePlacement.Axis
+    RefDirection = placement.RelativePlacement.RefDirection
+
+    if Axis and RefDirection:
+        zaxis = Vector(*Axis.DirectionRatios)
+        xaxis = Vector(*RefDirection.DirectionRatios)
+        yaxis = zaxis.cross(xaxis)
+        xaxis = yaxis.cross(zaxis)
+    else:
+        xaxis = Vector.Xaxis()
+        yaxis = Vector.Yaxis()
+
+    point = Point(*Location.Coordinates)
+    return Frame(point, xaxis, yaxis)
+
+
 def IfcGridPlacement_to_transformation(placement) -> Transformation:
     pass
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/resources/geometricmodel.py` & `compas_ifc-0.4.0/src/compas_ifc/resources/geometricmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from typing import List
 
-from compas_occ.brep import OCCBrep
+import ifcopenshell
 
 # from compas.geometry import Polyline
 from compas.geometry import Box
 from compas.geometry import Line
 from compas.geometry import Point
 from compas.geometry import Transformation
+
 from compas_ifc.resources.geometry import IfcAxis2Placement3D_to_frame
 from compas_ifc.resources.geometry import IfcDirection_to_vector
 from compas_ifc.resources.geometry import IfcProfileDef_to_curve
 
-from ifcopenshell import geom
-
 
-def IfcAdvancedBrep_to_brep(advanced_brep) -> OCCBrep:
+def IfcAdvancedBrep_to_brep(advanced_brep):
     """
     Convert an IFC AdvancedBrep [advancedbrep]_ to a COMPAS brep.
 
     """
     pass
 
 
-def IfcAdvancedBrepWithVoids_to_brep(advanced_brep_with_voids) -> OCCBrep:
+def IfcAdvancedBrepWithVoids_to_brep(advanced_brep_with_voids):
     """
     Convert an IFC AdvancedBrepWithVoids [advancedbrepwithvoids]_ to a COMPAS brep.
 
     """
     pass
 
 
@@ -34,27 +33,29 @@
     """
     Convert an IFC Block [block]_ to a COMPAS box.
 
     """
     pass
 
 
-def IfcBooleanClippingResult_to_brep(boolean_clipping_result) -> OCCBrep:
+def IfcBooleanClippingResult_to_brep(boolean_clipping_result):
     """
     Convert an IFC BooleanClippingResult [booleanclippingresult]_ to a COMPAS brep.
 
     """
     return IfcBooleanResult_to_brep(boolean_clipping_result)
 
 
-def IfcBooleanResult_to_brep(boolean_result) -> OCCBrep:
+def IfcBooleanResult_to_brep(boolean_result):
     """
     Convert an IFC BooleanResult [booleanresult]_ to a COMPAS brep.
 
     """
+    from compas_occ.brep import OCCBrep
+
     br = boolean_result
 
     # First Operand
     if br.FirstOperand.is_a("IfcBooleanResult"):
         A = IfcBooleanResult_to_brep(br.FirstOperand)
     elif br.FirstOperand.is_a("IfcExtrudedAreaSolid"):
         A = IfcExtrudedAreaSolid_to_brep(br.FirstOperand)
@@ -109,26 +110,28 @@
     """
     a = Point(*bounding_box.Corner.Coordinates)
     b = a + [bounding_box.XDim, bounding_box.YDim, 0]
     box = Box.from_corner_corner_height(a, b, bounding_box.ZDim)
     return box
 
 
-def IfcBoxedHalfSpace(boxed_half_space) -> OCCBrep:
+def IfcBoxedHalfSpace(boxed_half_space):
     bhs = boxed_half_space
     print(bhs.BaseSurface)
     print(bhs.Enclosure)
     print(bhs.AgreementFlag)
 
 
 def IfcCartesianPointList(cartesian_point_list) -> List[Point]:
     return [Point(*p) for p in cartesian_point_list.CoordList]
 
 
-def IfcExtrudedAreaSolid_to_brep(extruded_area_solid) -> OCCBrep:
+def IfcExtrudedAreaSolid_to_brep(extruded_area_solid):
+    from compas_occ.brep import OCCBrep
+
     eas = extruded_area_solid
     profile = IfcProfileDef_to_curve(eas.SweptArea)
 
     position = IfcAxis2Placement3D_to_frame(eas.Position)
     transformation = Transformation.from_frame(position)
 
     def _extrude(profile, eas):
@@ -150,35 +153,37 @@
         union.fix()
         union.make_solid()
         return union
     else:
         return _extrude(profile, eas)
 
 
-def IfcFacetedBrep_to_brep(faceted_brep) -> OCCBrep:
+def IfcFacetedBrep_to_brep(faceted_brep):
     pass
 
 
-def IfcFacetedBrepWithVoids_to_brep(faceted_brep_with_voids) -> OCCBrep:
+def IfcFacetedBrepWithVoids_to_brep(faceted_brep_with_voids):
     # fbwv = faceted_brep_with_voids
     pass
 
 
-def IfcIndexedPolygonalFaceSet_to_brep() -> OCCBrep:
+def IfcIndexedPolygonalFaceSet_to_brep():
     pass
 
 
 def IfcPolygonalBoundedHalfSpace_to_brep(polygonal_bounded_half_space):
     pbhs = polygonal_bounded_half_space
     print(pbhs.Position)
     print(pbhs.PolygonalBoundary)
     print(pbhs.BaseSurface)
 
 
-def IfcPolygonalFaceSet_to_brep(polygonal_face_set) -> OCCBrep:
+def IfcPolygonalFaceSet_to_brep(polygonal_face_set):
+    from compas_occ.brep import OCCBrep
+
     pfs = polygonal_face_set
 
     xyz = pfs.Coordinates.CoordList
     vertices = [[float(x), float(y), float(z)] for x, y, z in xyz]
     faces = [[i - 1 for i in face.CoordIndex] for face in pfs.Faces]
     polygons = [[vertices[index] for index in face] for face in faces]
     brep = OCCBrep.from_polygons(polygons)
@@ -186,27 +191,29 @@
     brep.sew()
     brep.fix()
     brep.make_solid()
 
     return brep
 
 
-def IfcTessellatedFaceSet_to_brep(tessellated_face_set) -> OCCBrep:
+def IfcTessellatedFaceSet_to_brep(tessellated_face_set):
     tfs = tessellated_face_set
 
     if tfs.is_a("IfcTriangulatedFaceSet"):
         return IfcTriangulatedFaceSet_to_brep(tfs)
 
     if tfs.is_a("IfcPolygonalFaceSet"):
         return IfcPolygonalFaceSet_to_brep(tfs)
 
     raise NotImplementedError(tfs.is_a())
 
 
-def IfcTriangulatedFaceSet_to_brep(triangulated_face_set) -> OCCBrep:
+def IfcTriangulatedFaceSet_to_brep(triangulated_face_set):
+    from compas_occ.brep import OCCBrep
+
     tfs = triangulated_face_set
 
     xyz = tfs.Coordinates.CoordList
     vertices = [[float(x), float(y), float(z)] for x, y, z in xyz]
     faces = [[a - 1, b - 1, c - 1] for a, b, c in tfs.CoordIndex]
     triangles = [[vertices[index] for index in face] for face in faces]
     brep = OCCBrep.from_polygons(triangles)
@@ -214,27 +221,37 @@
     brep.sew()
     brep.fix()
     brep.make_solid()
 
     return brep
 
 
-def IfcShape_to_brep(ifc_shape) -> OCCBrep:
-    settings = geom.settings()
+def IfcShape_to_brep(ifc_shape):
+    from compas_occ.brep import OCCBrep
+
+    settings = ifcopenshell.geom.settings()
     settings.set(settings.USE_PYTHON_OPENCASCADE, True)
-    shape = geom.create_shape(settings, ifc_shape)
+    shape = ifcopenshell.geom.create_shape(settings, ifc_shape)
 
     brep = OCCBrep.from_shape(shape)
     brep.sew()
     brep.fix()
     brep.make_solid()
 
     return brep
 
 
+def IfcShape_to_tessellatedbrep(ifc_shape):
+    from compas_ifc.brep import TessellatedBrep
+
+    settings = ifcopenshell.geom.settings()
+    shape = ifcopenshell.geom.create_shape(settings, ifc_shape)
+    return TessellatedBrep(vertices=shape.verts, edges=shape.edges, faces=shape.faces)
+
+
 # # IfcTessellationItem_to_mesh
 # def tessellation_to_mesh(item) -> Mesh:
 #     """
 #     Convert a tessellation item to a Mesh.
 
 #     """
 #     mesh = Mesh()
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/resources/geometry.py` & `compas_ifc-0.4.0/src/compas_ifc/resources/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # from compas_occ.geometry import OCCNurbsCurve
-from compas_occ.brep import OCCBrepFace
-
 from compas.geometry import Frame
 from compas.geometry import Line
 from compas.geometry import Plane
 from compas.geometry import Point
 from compas.geometry import Vector
 
 # from compas.geometry import Transformation
@@ -114,15 +112,17 @@
     xaxis = Vector.Xaxis() if not Axis1 else IfcDirection_to_vector(Axis1)
     yaxis = Vector.Yaxis() if not Axis2 else IfcDirection_to_vector(Axis2)
     # zaxis = Vector.Zaxis() if not Axis3 else IfcDirection_to_vector(Axis3)
     point = IfcCartesianPoint_to_point(LocalOrigin)
     return Frame(point, xaxis, yaxis)
 
 
-def IfcProfileDef_to_curve(profile_def) -> OCCBrepFace:
+def IfcProfileDef_to_curve(profile_def):
+    from compas_occ.brep import OCCBrepFace
+
     pd = profile_def
 
     if pd.is_a("IfcParameterizedProfileDef"):
         if pd.is_a("IfcRectangleProfileDef"):
             frame = IfcAxis2Placement2D_to_frame(pd.Position)
             points = [
                 frame.point + frame.xaxis * +0.5 * pd.XDim + frame.yaxis * -0.5 * pd.YDim,
@@ -145,14 +145,16 @@
                 raise NotImplementedError(profile)
         return faces
     else:
         raise NotImplementedError(pd)
 
 
 def IfcCurve_to_face(curve):
+    from compas_occ.brep import OCCBrepFace
+
     if curve.is_a("IfcIndexedPolyCurve"):
         points = [(x, y, 0) for x, y in curve.Points[0]]
         return OCCBrepFace.from_polygon(points)
     elif curve.is_a("IfcPolyline"):
         points = [IfcCartesianPoint_to_point(pt) for pt in curve.Points]
         return OCCBrepFace.from_polygon(points)
     else:
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/resources/mesh.py` & `compas_ifc-0.4.0/src/compas_ifc/resources/mesh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import ifcopenshell
-
 from compas.datastructures import Mesh
 
 
 def mesh_to_IfcPolygonalFaceSet(file: ifcopenshell.file, mesh: Mesh) -> ifcopenshell.entity_instance:
     """
     Convert a COMPAS mesh to an IFC PolygonalFaceSet.
     """
@@ -21,7 +20,28 @@
         faces.append(file.createIfcIndexedPolygonalFace(indexes))
 
     return file.create_entity(
         "IfcPolygonalFaceSet",
         Coordinates=file.createIfcCartesianPointList3D(vertices),
         Faces=faces,
     )
+
+
+def mesh_to_IfcShellBasedSurfaceModel(file: ifcopenshell.file, mesh: Mesh) -> ifcopenshell.entity_instance:
+    """
+    Convert a COMPAS mesh to an IFC PolygonalFaceSet.
+    """
+    vertices = {}
+    for key, attr in mesh.vertices(True):
+        vertex = file.createIfcCartesianPoint((float(attr["x"]), float(attr["y"]), float(attr["z"])))
+        vertices[key] = vertex
+
+    faces = []
+    for fkey in mesh.faces():
+        indexes = [vertices[key] for key in mesh.face_vertices(fkey)]
+        polyloop = file.create_entity("IfcPolyLoop", indexes)
+        bound = file.create_entity("IfcFaceOuterBound", polyloop, True)
+        face = file.create_entity("IfcFace", [bound])
+        faces.append(face)
+
+    shell = file.create_entity("IfcOpenShell", faces)
+    return file.create_entity("IfcShellBasedSurfaceModel", [shell])
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/resources/primities.py` & `compas_ifc-0.4.0/src/compas_ifc/resources/primities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import ifcopenshell
-
-from OCC.Core.gp import gp_Pln
-
 from compas.geometry import Frame
 from compas.geometry import Point
+
 from .shapes import create_IfcAxis2Placement3D
 
 
 def point_to_ifc_cartesian_point(file: ifcopenshell.file, point: Point) -> ifcopenshell.entity_instance:
     """
     Convert a COMPAS point to an IFC Cartesian Point.
     """
     point = [float(i) for i in point]
     return file.create_entity("IFCCARTESIANPOINT", (*point,))
 
 
-def occ_plane_to_frame(occ_plane: gp_Pln) -> Frame:
+def occ_plane_to_frame(occ_plane) -> Frame:
     """
     Convert an OCC plane to a COMPAS frame.
     """
     location = occ_plane.Location().Coord()
     xdir = occ_plane.XAxis().Direction().Coord()
     ydir = occ_plane.YAxis().Direction().Coord()
     return Frame(location, xdir, ydir)
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/resources/representation.py` & `compas_ifc-0.4.0/src/compas_ifc/resources/representation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from ifcopenshell.api import run
-
 from compas.datastructures import Mesh
 from compas.geometry import Box
 from compas.geometry import Cone
 from compas.geometry import Cylinder
 from compas.geometry import Sphere
-from compas_occ.brep import OCCBrep
+from ifcopenshell.api import run
 
 from .brep import brep_to_ifc_advanced_brep
 from .mesh import mesh_to_IfcPolygonalFaceSet
+from .mesh import mesh_to_IfcShellBasedSurfaceModel
 from .shapes import box_to_IfcBlock
 from .shapes import cone_to_IfcRightCircularCone
 from .shapes import cylinder_to_IfcRightCircularCylinder
 from .shapes import sphere_to_IfcSphere
 
 
 def write_body_representation(file, body, ifc_entity, context):
+    from compas_occ.brep import OCCBrep
+
     def _body_to_shape(body):
         if isinstance(body, Box):
             shape = box_to_IfcBlock(file, body)
         elif isinstance(body, Sphere):
             shape = sphere_to_IfcSphere(file, body)
         elif isinstance(body, Cone):
             shape = cone_to_IfcRightCircularCone(file, body)
         elif isinstance(body, Cylinder):
             shape = cylinder_to_IfcRightCircularCylinder(file, body)
         elif isinstance(body, Mesh):
-            shape = mesh_to_IfcPolygonalFaceSet(file, body)
+            if file.schema == "IFC4" or file.schema == "IFC4x3":
+                shape = mesh_to_IfcPolygonalFaceSet(file, body)
+            else:
+                shape = mesh_to_IfcShellBasedSurfaceModel(file, body)
         elif isinstance(body, OCCBrep):
             shape = brep_to_ifc_advanced_brep(file, body)
         else:
             raise Exception("Unsupported body type.")
         return shape
 
     if isinstance(body, list):
@@ -42,16 +46,23 @@
             else:
                 shape.extend(s)
     else:
         shape = _body_to_shape(body)
         if not isinstance(shape, list):
             shape = [shape]
 
+    RepresentationType = "SolidModel"
+
+    if shape and shape[0].is_a("IfcShellBasedSurfaceModel"):
+        RepresentationType = "SurfaceModel"
+
     representation = file.create_entity(
         "IfcShapeRepresentation",
         ContextOfItems=context,
         RepresentationIdentifier="Body",
-        RepresentationType="SolidModel",
+        RepresentationType=RepresentationType,
         Items=shape,
     )
 
     run("geometry.assign_representation", file, product=ifc_entity, representation=representation)
+
+    return representation
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/resources/shapes.py` & `compas_ifc-0.4.0/src/compas_ifc/resources/shapes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import ifcopenshell
-
 from compas.geometry import Box
 from compas.geometry import Cone
 from compas.geometry import Cylinder
 from compas.geometry import Sphere
 
 
+def frame_to_ifc_axis2_placement_3d(file, frame):
+    return create_IfcAxis2Placement3D(file, point=frame.point, dir1=frame.zaxis, dir2=frame.xaxis)
+
+
 def create_IfcAxis2Placement3D(file, point=None, dir1=None, dir2=None):
     """
     Create an IFC Axis2Placement3D from a point, a direction and a second direction.
     """
     point = file.createIfcCartesianPoint(point or (0.0, 0.0, 0.0))
     dir1 = file.createIfcDirection(dir1 or (0.0, 0.0, 1.0))
     dir2 = file.createIfcDirection(dir2 or (1.0, 0.0, 0.0))
     axis2placement = file.createIfcAxis2Placement3D(point, dir1, dir2)
     return axis2placement
 
 
-def create_IfcShapeRepresentation(
-    file: ifcopenshell.file, item: ifcopenshell.entity_instance, context: ifcopenshell.entity_instance
-) -> ifcopenshell.entity_instance:
+def create_IfcShapeRepresentation(file: ifcopenshell.file, item: ifcopenshell.entity_instance, context: ifcopenshell.entity_instance) -> ifcopenshell.entity_instance:
     """
     Create an IFC Shape Representation from an IFC item and a context.
     """
     return file.create_entity(
         "IfcShapeRepresentation",
         ContextOfItems=context,
         RepresentationIdentifier="Body",
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc/viewer/app.py` & `compas_ifc-0.4.0/src/compas_ifc/viewer/app.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/viewer/config.json` & `compas_ifc-0.4.0/src/compas_ifc/viewer/config.json`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/viewer/objects/entityobject.py` & `compas_ifc-0.4.0/src/compas_ifc/viewer/objects/entityobject.py`

 * *Files identical despite different names*

### Comparing `compas_ifc-0.3.0/src/compas_ifc/writer.py` & `compas_ifc-0.4.0/src/compas_ifc/writer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import time
+
 import ifcopenshell
 from ifcopenshell.api import run
 
-from .entities.objectdefinition import ObjectDefinition
 from .entities.element import Element
 from .entities.entity import Entity
+from .entities.objectdefinition import ObjectDefinition
 from .entities.product import Product
 from .entities.project import Project
+from .entities.root import Root
 from .resources.representation import write_body_representation
+from .resources.shapes import frame_to_ifc_axis2_placement_3d
 
 
 class IFCWriter(object):
     """
     A class for writing IFC files.
 
     Parameters
@@ -39,20 +43,22 @@
 
     """
 
     def __init__(self, model):
         self.file = None
         self.model = model
         self._entitymap = {}
+        self._representationmap = {}
         self._default_context = None
         self._default_body_context = None
         self._default_project = None
         self._default_site = None
         self._default_building = None
         self._default_building_storey = None
+        self._default_owner_history = None
 
     @property
     def default_context(self):
         # TODO: allow loading of existing contexts
         if not self._default_context:
             self._default_context = run("context.add_context", self.file, context_type="Model")
         return self._default_context
@@ -71,74 +77,98 @@
             )
         return self._default_body_context
 
     @property
     def default_project(self):
         if not self._default_project:
             if not self.model.projects:
-                self._default_project = run(
-                    "root.create_entity", self.file, ifc_class="IfcProject", name="Default Project"
-                )
+                self._default_project = self.file.create_entity("IfcProject", GlobalId=self.create_guid(), Name="Default Project")
                 run("unit.assign_unit", self.file)
             else:
                 self._default_project = self.write_entity(self.model.projects[0])
         return self._default_project
 
     @property
     def default_site(self):
         if not self._default_site:
             if not self.model.sites:
-                self._default_site = run("root.create_entity", self.file, ifc_class="IfcSite", name="Default Site")
-                run(
-                    "aggregate.assign_object",
-                    self.file,
-                    product=self._default_site,
-                    relating_object=self.default_project,
+                self._default_site = self.file.create_entity("IfcSite", Name="Default Site", GlobalId=self.create_guid())
+                self.file.create_entity(
+                    "IfcRelAggregates",
+                    GlobalId=self.create_guid(),
+                    RelatingObject=self.default_project,
+                    RelatedObjects=[self._default_site],
                 )
             else:
                 self._default_site = self.write_entity(self.model.sites[0])
         return self._default_site
 
     @property
     def default_building(self):
         if not self._default_building:
             if not self.model.buildings:
-                self._default_building = run(
-                    "root.create_entity", self.file, ifc_class="IfcBuilding", name="Default Building"
-                )
-                run(
-                    "aggregate.assign_object",
-                    self.file,
-                    product=self._default_building,
-                    relating_object=self.default_site,
+                self._default_building = self.file.create_entity("IfcBuilding", GlobalId=self.create_guid(), Name="Default Building")
+                self.file.create_entity(
+                    "IfcRelAggregates",
+                    GlobalId=self.create_guid(),
+                    RelatingObject=self.default_site,
+                    RelatedObjects=[self._default_building],
                 )
             else:
                 self._default_building = self.write_entity(self.model.buildings[0])
         return self._default_building
 
     @property
     def default_building_storey(self):
         if not self._default_building_storey:
             if not self.model.building_storeys:
-                self._default_building_storey = run(
-                    "root.create_entity", self.file, ifc_class="IfcBuildingStorey", name="Default Storey"
-                )
-                run(
-                    "aggregate.assign_object",
-                    self.file,
-                    product=self._default_building_storey,
-                    relating_object=self.default_building,
+                self._default_building_storey = self.file.create_entity("IfcBuildingStorey", GlobalId=self.create_guid(), Name="Default Storey")
+                self.file.create_entity(
+                    "IfcRelAggregates",
+                    GlobalId=self.create_guid(),
+                    RelatingObject=self.default_building,
+                    RelatedObjects=[self._default_building_storey],
                 )
             else:
                 self._default_building_storey = self.write_entity(self.model.building_storeys[0])
         return self._default_building_storey
 
+    @property
+    def default_owner_history(self):
+        if not self._default_owner_history:
+            import compas_ifc
+
+            person = self.file.create_entity("IfcPerson")
+            organization = self.file.create_entity("IfcOrganization", Name="compas.dev")
+            person_and_org = self.file.create_entity("IfcPersonAndOrganization", ThePerson=person, TheOrganization=organization)
+            application = self.file.create_entity(
+                "IfcApplication",
+                ApplicationDeveloper=organization,
+                Version=compas_ifc.__version__,
+                ApplicationFullName="compas_ifc",
+                ApplicationIdentifier="compas_ifc v" + compas_ifc.__version__,
+            )
+
+            owner_history = self.file.create_entity(
+                "IfcOwnerHistory",
+                OwningUser=person_and_org,
+                OwningApplication=application,
+                ChangeAction="ADDED",
+                CreationDate=int(time.time()),
+            )
+
+            self._default_owner_history = owner_history
+        return self._default_owner_history
+
+    def create_guid(self):
+        return ifcopenshell.guid.new()
+
     def reset(self):
         """Resets the writer to start with a new ifc file."""
-        self.file = ifcopenshell.file()
+        self.file = ifcopenshell.file(schema=self.model.schema.name())
         self._entitymap = {}
         self._default_context = None
         self._default_body_context = None
         self._default_project = None
         self._default_site = None
         self._default_building = None
         self._default_building_storey = None
@@ -228,46 +258,79 @@
         else:
             # If no parent is given, use the default building storey.
             parent = self.default_building_storey
 
         child = self._entitymap[entity]
 
         if isinstance(entity, Element):
-            run("spatial.assign_container", self.file, relating_structure=parent, product=child)
+            self.file.create_entity(
+                "IfcRelContainedInSpatialStructure",
+                GlobalId=self.create_guid(),
+                RelatingStructure=parent,
+                RelatedElements=[child],
+            )
         else:
-            run("aggregate.assign_object", self.file, relating_object=parent, product=child)
+            self.file.create_entity("IfcRelAggregates", GlobalId=self.create_guid(), RelatingObject=parent, RelatedObjects=[child])
 
     def write_entity(self, entity: Entity) -> None:
         """Writes the given entity recursively with all its referencing attributes to the ifc file."""
         if entity in self._entitymap:
             return self._entitymap[entity]
 
         attributes = {}
+        if isinstance(entity, Root):
+            attributes["OwnerHistory"] = self.default_owner_history
+
         for key, value in entity.attributes.items():
             if isinstance(value, Entity):
                 attributes[key] = self.write_entity(value)
             elif isinstance(value, list) and value and isinstance(value[0], Entity):
                 attributes[key] = [self.write_entity(v) for v in value]
             else:
                 attributes[key] = value
 
-        ifc_entity = self.file.create_entity(entity.ifc_type, **attributes)
+        # ifc_entity = self.file.create_entity(entity.ifc_type, **attributes)
+        ifc_entity = self.file.create_entity(entity.ifc_type)
+        for key, value in attributes.items():
+            if value is not None:
+                setattr(ifc_entity, key, value)
+
         self._entitymap[entity] = ifc_entity
 
         if not entity._entity:
             # Entity created in memory
             self.write_entity_representation(entity)
+            self.write_entity_placement(entity)
+
+        if isinstance(entity, Project):
+            print("Writing project: " + str(entity))
+            run("unit.assign_unit", self.file)
 
         return ifc_entity
 
     def write_entity_pset(self, entity: Entity):
         raise NotImplementedError()
 
     def write_entity_representation(self, entity: Entity):
         """Writes the representations of the given entity to the ifc file."""
         if isinstance(entity, Product):
-            try:
-                write_body_representation(self.file, entity.body, self._entitymap[entity], self.default_body_context)
-            except Exception as e:
-                print("Error writing body representation of entity: " + str(entity))
-                print(e)
-                pass
+            if entity.body:
+                if id(entity.body) not in self._representationmap:
+                    representation = write_body_representation(self.file, entity.body, self._entitymap[entity], self.default_body_context)
+                    self._representationmap[id(entity.body)] = representation
+                else:
+                    representation = self._representationmap[id(entity.body)]
+                    run(
+                        "geometry.assign_representation",
+                        self.file,
+                        product=self._entitymap[entity],
+                        representation=representation,
+                    )
+
+    def write_entity_placement(self, entity: Entity):
+        """Writes the placement of the given entity to the ifc file."""
+        if isinstance(entity, Product):
+            if entity.frame:
+                # TODO: consider parent frame
+                loacal_placement = frame_to_ifc_axis2_placement_3d(self.file, entity.frame)
+                placement = self.file.create_entity("IfcLocalPlacement", RelativePlacement=loacal_placement)
+                self._entitymap[entity].ObjectPlacement = placement
```

### Comparing `compas_ifc-0.3.0/src/compas_ifc.egg-info/SOURCES.txt` & `compas_ifc-0.4.0/src/compas_ifc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+requirements-dev.txt
 requirements.txt
-setup.cfg
-setup.py
 src/compas_ifc/__init__.py
 src/compas_ifc/__main__.py
 src/compas_ifc/attributes.py
 src/compas_ifc/helpers.py
 src/compas_ifc/model.py
 src/compas_ifc/reader.py
 src/compas_ifc/representation.py
 src/compas_ifc/writer.py
 src/compas_ifc.egg-info/PKG-INFO
 src/compas_ifc.egg-info/SOURCES.txt
 src/compas_ifc.egg-info/dependency_links.txt
 src/compas_ifc.egg-info/not-zip-safe
 src/compas_ifc.egg-info/requires.txt
 src/compas_ifc.egg-info/top_level.txt
+src/compas_ifc/brep/__init__.py
+src/compas_ifc/brep/tessellatedbrep.py
+src/compas_ifc/brep/tessellatedbrepobject.py
 src/compas_ifc/entities/__init__.py
 src/compas_ifc/entities/building.py
 src/compas_ifc/entities/buildingelements.py
 src/compas_ifc/entities/buildingstorey.py
 src/compas_ifc/entities/element.py
 src/compas_ifc/entities/entity.py
 src/compas_ifc/entities/geographicelement.py
```

