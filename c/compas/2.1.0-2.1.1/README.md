# Comparing `tmp/COMPAS-2.1.0.tar.gz` & `tmp/compas-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "COMPAS-2.1.0.tar", last modified: Fri Mar  1 23:04:19 2024, max compression
+gzip compressed data, was "compas-2.1.1.tar", last modified: Mon May 13 23:45:06 2024, max compression
```

## Comparing `COMPAS-2.1.0.tar` & `compas-2.1.1.tar`

### file list

```diff
@@ -1,552 +1,531 @@
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.260955 COMPAS-2.1.0/
--rw-rw-rw-   0        0        0     2899 2024-03-01 23:01:37.000000 COMPAS-2.1.0/AUTHORS.md
--rw-rw-rw-   0        0        0   132591 2024-03-01 23:01:37.000000 COMPAS-2.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1101 2024-03-01 23:01:37.000000 COMPAS-2.1.0/LICENSE
--rw-rw-rw-   0        0        0      457 2024-03-01 23:01:37.000000 COMPAS-2.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4893 2024-03-01 23:04:19.260955 COMPAS-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3623 2024-03-01 23:01:37.000000 COMPAS-2.1.0/README.md
--rw-rw-rw-   0        0        0      856 2024-03-01 23:01:37.000000 COMPAS-2.1.0/conftest.py
--rw-rw-rw-   0        0        0      703 2024-03-01 23:01:37.000000 COMPAS-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      135 2024-03-01 23:01:37.000000 COMPAS-2.1.0/requirements.txt
--rw-rw-rw-   0        0        0      227 2024-03-01 23:04:19.260955 COMPAS-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2307 2024-03-01 23:01:37.000000 COMPAS-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.026501 COMPAS-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.042130 COMPAS-2.1.0/src/COMPAS.egg-info/
--rw-rw-rw-   0        0        0     4893 2024-03-01 23:04:18.000000 COMPAS-2.1.0/src/COMPAS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18805 2024-03-01 23:04:18.000000 COMPAS-2.1.0/src/COMPAS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-01 23:04:18.000000 COMPAS-2.1.0/src/COMPAS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-03-01 23:04:18.000000 COMPAS-2.1.0/src/COMPAS.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-01 23:02:03.000000 COMPAS-2.1.0/src/COMPAS.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      125 2024-03-01 23:04:18.000000 COMPAS-2.1.0/src/COMPAS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2024-03-01 23:04:18.000000 COMPAS-2.1.0/src/COMPAS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.042130 COMPAS-2.1.0/src/compas/
--rw-rw-rw-   0        0        0     8387 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/__init__.py
--rw-rw-rw-   0        0        0     1762 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/__main__.py
--rw-rw-rw-   0        0        0     2476 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/_iotools.py
--rw-rw-rw-   0        0        0    21015 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/_os.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.042130 COMPAS-2.1.0/src/compas/colors/
--rw-rw-rw-   0        0        0      397 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.073378 COMPAS-2.1.0/src/compas/colors/cmcrameri/
--rw-rw-rw-   0        0        0     1191 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/LICENSE
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/acton.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/actonS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/bam.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/bamO.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/bamako.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/bamakoS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/batlow.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/batlowK.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/batlowS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/batlowW.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/berlin.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/bilbao.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/bilbaoS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/broc.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/brocO.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/buda.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/budaS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/bukavu.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/cork.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/corkO.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/davos.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/davosS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/devon.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/devonS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/fes.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/grayC.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/grayCS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/hawaii.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/hawaiiS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/imola.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/imolaS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/lajolla.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/lajollaS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/lapaz.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/lapazS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/lisbon.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/nuuk.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/nuukS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/oleron.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/oslo.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/osloS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/roma.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/romaO.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/tofino.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/tokyo.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/tokyoS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/turku.txt
--rw-rw-rw-   0        0        0     2800 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/turkuS.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/vanimo.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/vik.txt
--rw-rw-rw-   0        0        0     7168 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/cmcrameri/vikO.txt
--rw-rw-rw-   0        0        0    28048 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/color.py
--rw-rw-rw-   0        0        0     2526 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/colordict.py
--rw-rw-rw-   0        0        0     9518 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/colormap.py
--rw-rw-rw-   0        0        0     5007 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/html_colors.py
--rw-rw-rw-   0        0        0    39084 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/colors/mpl_colormap.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.073378 COMPAS-2.1.0/src/compas/data/
--rw-rw-rw-   0        0        0      938 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/coercion.py
--rw-rw-rw-   0        0        0      325 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/conftest.py
--rw-rw-rw-   0        0        0     9861 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/data.py
--rw-rw-rw-   0        0        0     6839 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/encoders.py
--rw-rw-rw-   0        0        0      169 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/exceptions.py
--rw-rw-rw-   0        0        0     6504 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/json.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.089003 COMPAS-2.1.0/src/compas/data/samples/
--rw-rw-rw-   0        0        0     3063 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/boxes.obj
--rw-rw-rw-   0        0        0    65931 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/butt_model.obj
--rw-rw-rw-   0        0        0     3184 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/cone.stl
--rw-rw-rw-   0        0        0      135 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/cube.off
--rw-rw-rw-   0        0        0  1394975 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/cube_ascii.stl
--rw-rw-rw-   0        0        0      684 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/cube_binary.stl
--rw-rw-rw-   0        0        0      684 2024-03-01 23:03:24.000000 COMPAS-2.1.0/src/compas/data/samples/cube_binary_2.stl
--rw-rw-rw-   0        0        0  4063805 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/doosabin.json
--rw-rw-rw-   0        0        0      702 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/faces.obj
--rw-rw-rw-   0        0        0   301165 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/faces_big.obj
--rw-rw-rw-   0        0        0      702 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/faces_reversed.obj
--rw-rw-rw-   0        0        0     2000 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/fink.obj
--rw-rw-rw-   0        0        0     5921 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/grid_irregular.obj
--rw-rw-rw-   0        0        0     2442 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/hypar.obj
--rw-rw-rw-   0        0        0     1672 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/lines.json
--rw-rw-rw-   0        0        0     3666 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/lines.obj
--rw-rw-rw-   0        0        0   554153 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/lines_big.obj
--rw-rw-rw-   0        0        0  2295689 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/lines_bigger.obj
--rw-rw-rw-   0        0        0     5409 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/lines_noleaves.obj
--rw-rw-rw-   0        0        0    25178 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/mesh.obj
--rw-rw-rw-   0        0        0    42388 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/mesh_100_faces.json
--rw-rw-rw-   0        0        0    46729 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/mesh_110_faces.json
--rw-rw-rw-   0        0        0     5023 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/open_edges.obj
--rw-rw-rw-   0        0        0       60 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/point.json
--rw-rw-rw-   0        0        0     6725 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/quadmesh.obj
--rw-rw-rw-   0        0        0     3289 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/quadmesh_planar.obj
--rw-rw-rw-   0        0        0     3914 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/saddle.obj
--rw-rw-rw-   0        0        0     1331 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/spline.obj
--rw-rw-rw-   0        0        0    37882 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/tubemesh.json
--rw-rw-rw-   0        0        0     7287 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/tubemesh.obj
--rw-rw-rw-   0        0        0     7153 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/tubemesh.off
--rw-rw-rw-   0        0        0     8978 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/samples/tubemesh.ply
--rw-rw-rw-   0        0        0     3290 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/schema.py
--rw-rw-rw-   0        0        0     4780 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/data/validators.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.089003 COMPAS-2.1.0/src/compas/datastructures/
--rw-rw-rw-   0        0        0     2409 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/__init__.py
--rw-rw-rw-   0        0        0     4746 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/_mutablemapping.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.089003 COMPAS-2.1.0/src/compas/datastructures/assembly/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/assembly/__init__.py
--rw-rw-rw-   0        0        0     7219 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/assembly/assembly.py
--rw-rw-rw-   0        0        0       89 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/assembly/exceptions.py
--rw-rw-rw-   0        0        0     7337 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/assembly/part.py
--rw-rw-rw-   0        0        0     3023 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/attributes.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.089003 COMPAS-2.1.0/src/compas/datastructures/cell_network/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/cell_network/__init__.py
--rw-rw-rw-   0        0        0   131306 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/cell_network/cell_network.py
--rw-rw-rw-   0        0        0     7536 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/datastructure.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.104629 COMPAS-2.1.0/src/compas/datastructures/graph/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/graph/__init__.py
--rw-rw-rw-   0        0        0     5978 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/graph/duality.py
--rw-rw-rw-   0        0        0    74959 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/graph/graph.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.104629 COMPAS-2.1.0/src/compas/datastructures/graph/operations/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/graph/operations/__init__.py
--rw-rw-rw-   0        0        0     4141 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/graph/operations/join.py
--rw-rw-rw-   0        0        0     1507 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/graph/operations/split.py
--rw-rw-rw-   0        0        0     7780 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/graph/planarity.py
--rw-rw-rw-   0        0        0     1689 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/graph/smoothing.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.104629 COMPAS-2.1.0/src/compas/datastructures/mesh/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/__init__.py
--rw-rw-rw-   0        0        0    17309 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/conway.py
--rw-rw-rw-   0        0        0     3374 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/duality.py
--rw-rw-rw-   0        0        0   161525 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/mesh.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.104629 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/__init__.py
--rw-rw-rw-   0        0        0    10232 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/collapse.py
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/extrude.py
--rw-rw-rw-   0        0        0     3640 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/insert.py
--rw-rw-rw-   0        0        0     2412 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/merge.py
--rw-rw-rw-   0        0        0     6859 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/split.py
--rw-rw-rw-   0        0        0     1043 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/substitute.py
--rw-rw-rw-   0        0        0     1573 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/swap.py
--rw-rw-rw-   0        0        0     3507 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/operations/weld.py
--rw-rw-rw-   0        0        0     7207 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/remesh.py
--rw-rw-rw-   0        0        0     5674 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/slice.py
--rw-rw-rw-   0        0        0     5683 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/smoothing.py
--rw-rw-rw-   0        0        0    23968 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/mesh/subdivision.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.104629 COMPAS-2.1.0/src/compas/datastructures/tree/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/tree/__init__.py
--rw-rw-rw-   0        0        0    14490 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/tree/tree.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.104629 COMPAS-2.1.0/src/compas/datastructures/volmesh/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/volmesh/__init__.py
--rw-rw-rw-   0        0        0   130545 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/datastructures/volmesh/volmesh.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.104629 COMPAS-2.1.0/src/compas/files/
--rw-rw-rw-   0        0        0      953 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.120255 COMPAS-2.1.0/src/compas/files/_xml/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/_xml/__init__.py
--rw-rw-rw-   0        0        0     7509 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/_xml/xml_cli.py
--rw-rw-rw-   0        0        0      971 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/_xml/xml_cpython.py
--rw-rw-rw-   0        0        0     1753 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/_xml/xml_pre_38.py
--rw-rw-rw-   0        0        0     1254 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/_xml/xml_shared.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.120255 COMPAS-2.1.0/src/compas/files/gltf/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/__init__.py
--rw-rw-rw-   0        0        0     1262 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/constants.py
--rw-rw-rw-   0        0        0    24791 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/data_classes.py
--rw-rw-rw-   0        0        0    12212 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/extensions.py
--rw-rw-rw-   0        0        0     2724 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/gltf.py
--rw-rw-rw-   0        0        0     1720 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/gltf_children.py
--rw-rw-rw-   0        0        0    21631 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/gltf_content.py
--rw-rw-rw-   0        0        0    19546 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/gltf_exporter.py
--rw-rw-rw-   0        0        0     9062 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/gltf_mesh.py
--rw-rw-rw-   0        0        0    12340 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/gltf_node.py
--rw-rw-rw-   0        0        0     5275 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/gltf_parser.py
--rw-rw-rw-   0        0        0    11428 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/gltf_reader.py
--rw-rw-rw-   0        0        0     3686 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/gltf_scene.py
--rw-rw-rw-   0        0        0     2394 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/gltf/helpers.py
--rw-rw-rw-   0        0        0    21861 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/obj.py
--rw-rw-rw-   0        0        0     8555 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/off.py
--rw-rw-rw-   0        0        0    23437 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/ply.py
--rw-rw-rw-   0        0        0    13169 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/stl.py
--rw-rw-rw-   0        0        0     8440 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/files/xml.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.151584 COMPAS-2.1.0/src/compas/geometry/
--rw-rw-rw-   0        0        0    21424 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.151584 COMPAS-2.1.0/src/compas/geometry/_core/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/__init__.py
--rw-rw-rw-   0        0        0    75175 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/_algebra.py
--rw-rw-rw-   0        0        0    11508 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/angles.py
--rw-rw-rw-   0        0        0    15920 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/centroids.py
--rw-rw-rw-   0        0        0    26733 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/distance.py
--rw-rw-rw-   0        0        0     3629 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/normals.py
--rw-rw-rw-   0        0        0     9423 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/nurbs.py
--rw-rw-rw-   0        0        0    21373 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/predicates_2.py
--rw-rw-rw-   0        0        0    37253 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/predicates_3.py
--rw-rw-rw-   0        0        0     5025 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/quaternions.py
--rw-rw-rw-   0        0        0     5805 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/size.py
--rw-rw-rw-   0        0        0     1440 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/tangent.py
--rw-rw-rw-   0        0        0    33077 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/transformations.py
--rw-rw-rw-   0        0        0     8435 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/_core/transformations_numpy.py
--rw-rw-rw-   0        0        0     3677 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/bbox.py
--rw-rw-rw-   0        0        0     8840 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/bbox_numpy.py
--rw-rw-rw-   0        0        0     2269 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/bestfit.py
--rw-rw-rw-   0        0        0     7845 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/bestfit_numpy.py
--rw-rw-rw-   0        0        0    10411 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/booleans.py
--rw-rw-rw-   0        0        0     4475 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/booleans_shapely.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.161620 COMPAS-2.1.0/src/compas/geometry/brep/
--rw-rw-rw-   0        0        0     2386 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/brep/__init__.py
--rw-rw-rw-   0        0        0    28921 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/brep/brep.py
--rw-rw-rw-   0        0        0     7485 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/brep/edge.py
--rw-rw-rw-   0        0        0      492 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/brep/errors.py
--rw-rw-rw-   0        0        0     8919 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/brep/face.py
--rw-rw-rw-   0        0        0     2263 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/brep/loop.py
--rw-rw-rw-   0        0        0     1099 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/brep/trim.py
--rw-rw-rw-   0        0        0     1287 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/brep/vertex.py
--rw-rw-rw-   0        0        0      969 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/contours.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.167162 COMPAS-2.1.0/src/compas/geometry/curves/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/__init__.py
--rw-rw-rw-   0        0        0    14208 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/arc.py
--rw-rw-rw-   0        0        0     9657 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/bezier.py
--rw-rw-rw-   0        0        0    15605 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/circle.py
--rw-rw-rw-   0        0        0      488 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/conic.py
--rw-rw-rw-   0        0        0    17728 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/curve.py
--rw-rw-rw-   0        0        0    12853 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/ellipse.py
--rw-rw-rw-   0        0        0    10162 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/hyperbola.py
--rw-rw-rw-   0        0        0    10399 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/line.py
--rw-rw-rw-   0        0        0    11682 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/nurbs.py
--rw-rw-rw-   0        0        0     7600 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/parabola.py
--rw-rw-rw-   0        0        0    24207 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/curves/polyline.py
--rw-rw-rw-   0        0        0    23040 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/frame.py
--rw-rw-rw-   0        0        0     7040 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/geometry.py
--rw-rw-rw-   0        0        0     4718 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/hull.py
--rw-rw-rw-   0        0        0     1922 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/hull_numpy.py
--rw-rw-rw-   0        0        0     3123 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/icp_numpy.py
--rw-rw-rw-   0        0        0     1077 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/interpolation_barycentric.py
--rw-rw-rw-   0        0        0     3661 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/interpolation_coons.py
--rw-rw-rw-   0        0        0     2644 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/interpolation_tweening.py
--rw-rw-rw-   0        0        0     2776 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/intersection.py
--rw-rw-rw-   0        0        0    36346 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/intersections.py
--rw-rw-rw-   0        0        0     4838 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/kdtree.py
--rw-rw-rw-   0        0        0     6856 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/offset.py
--rw-rw-rw-   0        0        0     3228 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/pca_numpy.py
--rw-rw-rw-   0        0        0    19189 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/plane.py
--rw-rw-rw-   0        0        0    19041 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/point.py
--rw-rw-rw-   0        0        0    12338 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/pointcloud.py
--rw-rw-rw-   0        0        0    15383 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/polygon.py
--rw-rw-rw-   0        0        0    18848 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/polyhedron.py
--rw-rw-rw-   0        0        0     5381 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/projection.py
--rw-rw-rw-   0        0        0      784 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/quadmesh_planarize.py
--rw-rw-rw-   0        0        0     3729 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/quadmesh_planarize_none.py
--rw-rw-rw-   0        0        0    12959 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/quaternion.py
--rw-rw-rw-   0        0        0     3504 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/reflection.py
--rw-rw-rw-   0        0        0    12463 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/rotation.py
--rw-rw-rw-   0        0        0     3498 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/scale.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.167162 COMPAS-2.1.0/src/compas/geometry/shapes/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/shapes/__init__.py
--rw-rw-rw-   0        0        0    22238 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/shapes/box.py
--rw-rw-rw-   0        0        0    14585 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/shapes/capsule.py
--rw-rw-rw-   0        0        0     9833 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/shapes/cone.py
--rw-rw-rw-   0        0        0    11367 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/shapes/cylinder.py
--rw-rw-rw-   0        0        0     9181 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/shapes/shape.py
--rw-rw-rw-   0        0        0    11303 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/shapes/sphere.py
--rw-rw-rw-   0        0        0    10479 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/shapes/torus.py
--rw-rw-rw-   0        0        0     3977 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/shear.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.167162 COMPAS-2.1.0/src/compas/geometry/surfaces/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/__init__.py
--rw-rw-rw-   0        0        0     5063 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/conical.py
--rw-rw-rw-   0        0        0     7279 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/cylindrical.py
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/extrusion.py
--rw-rw-rw-   0        0        0    11532 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/nurbs.py
--rw-rw-rw-   0        0        0     7029 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/planar.py
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/revolution.py
--rw-rw-rw-   0        0        0     7497 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/spherical.py
--rw-rw-rw-   0        0        0    19317 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/surface.py
--rw-rw-rw-   0        0        0     6227 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/surfaces/toroidal.py
--rw-rw-rw-   0        0        0    18114 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/transformation.py
--rw-rw-rw-   0        0        0     3104 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/translation.py
--rw-rw-rw-   0        0        0     3042 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/triangulation_delaunay.py
--rw-rw-rw-   0        0        0     9718 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/triangulation_earclip.py
--rw-rw-rw-   0        0        0     3144 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_curvature.py
--rw-rw-rw-   0        0        0      659 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_descent_numpy.py
--rw-rw-rw-   0        0        0     1262 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_geodistance.py
--rw-rw-rw-   0        0        0     2533 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_gradient_numpy.py
--rw-rw-rw-   0        0        0     1089 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_isolines.py
--rw-rw-rw-   0        0        0      742 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_matrices.py
--rw-rw-rw-   0        0        0     5335 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_matrices_numpy.py
--rw-rw-rw-   0        0        0     1290 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_parametrisation.py
--rw-rw-rw-   0        0        0     7717 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_pull_points_numpy.py
--rw-rw-rw-   0        0        0     3148 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_remeshing.py
--rw-rw-rw-   0        0        0     4134 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_samplepoints_numpy.py
--rw-rw-rw-   0        0        0      779 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_slicing.py
--rw-rw-rw-   0        0        0      959 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/trimesh_smoothing_numpy.py
--rw-rw-rw-   0        0        0    23101 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/geometry/vector.py
--rw-rw-rw-   0        0        0    12606 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/itertools.py
--rw-rw-rw-   0        0        0    15306 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/linalg.py
--rw-rw-rw-   0        0        0     8964 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/matrices.py
--rw-rw-rw-   0        0        0    17324 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/plugins.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.167162 COMPAS-2.1.0/src/compas/rpc/
--rw-rw-rw-   0        0        0     1041 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/rpc/__init__.py
--rw-rw-rw-   0        0        0     2144 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/rpc/__main__.py
--rw-rw-rw-   0        0        0     5781 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/rpc/dispatcher.py
--rw-rw-rw-   0        0        0      310 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/rpc/errors.py
--rw-rw-rw-   0        0        0    15578 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/rpc/proxy.py
--rw-rw-rw-   0        0        0     2102 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/rpc/server.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.167162 COMPAS-2.1.0/src/compas/rpc/services/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/rpc/services/__init__.py
--rw-rw-rw-   0        0        0     2393 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/rpc/services/default.py
--rw-rw-rw-   0        0        0     1520 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/rpc/services/watcher.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.182832 COMPAS-2.1.0/src/compas/scene/
--rw-rw-rw-   0        0        0     1901 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/__init__.py
--rw-rw-rw-   0        0        0      112 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/assemblyobject.py
--rw-rw-rw-   0        0        0     4356 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/context.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.182832 COMPAS-2.1.0/src/compas/scene/descriptors/
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/descriptors/__init__.py
--rw-rw-rw-   0        0        0      911 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/descriptors/attribute.py
--rw-rw-rw-   0        0        0     2719 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/descriptors/color.py
--rw-rw-rw-   0        0        0     2963 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/descriptors/colordict.py
--rw-rw-rw-   0        0        0      440 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/descriptors/protocol.py
--rw-rw-rw-   0        0        0      259 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/exceptions.py
--rw-rw-rw-   0        0        0     2117 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/geometryobject.py
--rw-rw-rw-   0        0        0     5604 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/graphobject.py
--rw-rw-rw-   0        0        0     7651 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/meshobject.py
--rw-rw-rw-   0        0        0     9217 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/scene.py
--rw-rw-rw-   0        0        0     6498 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/sceneobject.py
--rw-rw-rw-   0        0        0     8976 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/scene/volmeshobject.py
--rw-rw-rw-   0        0        0    21283 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/tolerance.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.182832 COMPAS-2.1.0/src/compas/topology/
--rw-rw-rw-   0        0        0     1153 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/topology/__init__.py
--rw-rw-rw-   0        0        0     3639 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/topology/combinatorics.py
--rw-rw-rw-   0        0        0     2988 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/topology/connectivity.py
--rw-rw-rw-   0        0        0     6245 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/topology/orientation.py
--rw-rw-rw-   0        0        0    19368 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/topology/traversal.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.182832 COMPAS-2.1.0/src/compas/utilities/
--rw-rw-rw-   0        0        0     1040 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/utilities/__init__.py
--rw-rw-rw-   0        0        0     4645 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/utilities/azync.py
--rw-rw-rw-   0        0        0      708 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/utilities/datetime.py
--rw-rw-rw-   0        0        0     3091 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/utilities/decorators.py
--rw-rw-rw-   0        0        0     3660 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/utilities/maps.py
--rw-rw-rw-   0        0        0     1542 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/utilities/remote.py
--rw-rw-rw-   0        0        0     4360 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas/utilities/ssh.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.182832 COMPAS-2.1.0/src/compas_blender/
--rw-rw-rw-   0        0        0     8388 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/__init__.py
--rw-rw-rw-   0        0        0     3323 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/collections.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.198464 COMPAS-2.1.0/src/compas_blender/conversions/
--rw-rw-rw-   0        0        0     1528 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/conversions/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/conversions/breps.py
--rw-rw-rw-   0        0        0      594 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/conversions/colors.py
--rw-rw-rw-   0        0        0     3211 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/conversions/curves.py
--rw-rw-rw-   0        0        0     4464 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/conversions/geometry.py
--rw-rw-rw-   0        0        0     3721 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/conversions/meshes.py
--rw-rw-rw-   0        0        0     1552 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/conversions/surfaces.py
--rw-rw-rw-   0        0        0     1231 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/conversions/transformations.py
--rw-rw-rw-   0        0        0      749 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/data.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.198464 COMPAS-2.1.0/src/compas_blender/geometry/
--rw-rw-rw-   0        0        0      386 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/geometry/__init__.py
--rw-rw-rw-   0        0        0     3356 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/geometry/booleans.py
--rw-rw-rw-   0        0        0    12706 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/install.py
--rw-rw-rw-   0        0        0     8355 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/objects.py
--rw-rw-rw-   0        0        0      442 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/print_python_path.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.198464 COMPAS-2.1.0/src/compas_blender/scene/
--rw-rw-rw-   0        0        0     4114 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/__init__.py
--rw-rw-rw-   0        0        0     2066 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/boxobject.py
--rw-rw-rw-   0        0        0     2383 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/capsuleobject.py
--rw-rw-rw-   0        0        0     1627 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/circleobject.py
--rw-rw-rw-   0        0        0     2210 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/coneobject.py
--rw-rw-rw-   0        0        0     1722 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/curveobject.py
--rw-rw-rw-   0        0        0     2262 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/cylinderobject.py
--rw-rw-rw-   0        0        0     3315 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/frameobject.py
--rw-rw-rw-   0        0        0     9253 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/graphobject.py
--rw-rw-rw-   0        0        0     1785 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/lineobject.py
--rw-rw-rw-   0        0        0    18073 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/meshobject.py
--rw-rw-rw-   0        0        0     2725 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/planeobject.py
--rw-rw-rw-   0        0        0     2124 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/pointcloudobject.py
--rw-rw-rw-   0        0        0     2007 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/pointobject.py
--rw-rw-rw-   0        0        0     1731 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/polygonobject.py
--rw-rw-rw-   0        0        0     1964 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/polyhedronobject.py
--rw-rw-rw-   0        0        0     1662 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/polylineobject.py
--rw-rw-rw-   0        0        0     7673 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/sceneobject.py
--rw-rw-rw-   0        0        0     2338 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/sphereobject.py
--rw-rw-rw-   0        0        0     1654 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/surfaceobject.py
--rw-rw-rw-   0        0        0     2346 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/torusobject.py
--rw-rw-rw-   0        0        0     2119 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/vectorobject.py
--rw-rw-rw-   0        0        0    17657 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/scene/volmeshobject.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.198464 COMPAS-2.1.0/src/compas_blender/utilities/
--rw-rw-rw-   0        0        0      663 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/utilities/__init__.py
--rw-rw-rw-   0        0        0    27135 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_blender/utilities/drawing.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.214089 COMPAS-2.1.0/src/compas_ghpython/
--rw-rw-rw-   0        0        0     4022 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.214089 COMPAS-2.1.0/src/compas_ghpython/components/
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.214089 COMPAS-2.1.0/src/compas_ghpython/components/Compas_FromJson/
--rw-rw-rw-   0        0        0      387 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_FromJson/code.py
--rw-rw-rw-   0        0        0      988 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_FromJson/icon.png
--rw-rw-rw-   0        0        0      658 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_FromJson/metadata.json
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.214089 COMPAS-2.1.0/src/compas_ghpython/components/Compas_Info/
--rw-rw-rw-   0        0        0      451 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_Info/code.py
--rw-rw-rw-   0        0        0     1287 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_Info/icon.png
--rw-rw-rw-   0        0        0      495 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_Info/metadata.json
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.214089 COMPAS-2.1.0/src/compas_ghpython/components/Compas_RpcCall/
--rw-rw-rw-   0        0        0      839 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_RpcCall/code.py
--rw-rw-rw-   0        0        0     1306 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_RpcCall/icon.png
--rw-rw-rw-   0        0        0     1498 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_RpcCall/metadata.json
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.214089 COMPAS-2.1.0/src/compas_ghpython/components/Compas_ToJson/
--rw-rw-rw-   0        0        0      413 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_ToJson/code.py
--rw-rw-rw-   0        0        0      979 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_ToJson/icon.png
--rw-rw-rw-   0        0        0     1084 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_ToJson/metadata.json
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.214089 COMPAS-2.1.0/src/compas_ghpython/components/Compas_ToRhinoGeometry/
--rw-rw-rw-   0        0        0      323 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_ToRhinoGeometry/code.py
--rw-rw-rw-   0        0        0     1159 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_ToRhinoGeometry/icon.png
--rw-rw-rw-   0        0        0      614 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/Compas_ToRhinoGeometry/metadata.json
--rw-rw-rw-   0        0        0     2830 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.214089 COMPAS-2.1.0/src/compas_ghpython/components/ghuser/
--rw-rw-rw-   0        0        0     1929 2024-03-01 23:04:15.000000 COMPAS-2.1.0/src/compas_ghpython/components/ghuser/Compas_FromJson.ghuser
--rw-rw-rw-   0        0        0     2096 2024-03-01 23:04:15.000000 COMPAS-2.1.0/src/compas_ghpython/components/ghuser/Compas_Info.ghuser
--rw-rw-rw-   0        0        0     2843 2024-03-01 23:04:15.000000 COMPAS-2.1.0/src/compas_ghpython/components/ghuser/Compas_RpcCall.ghuser
--rw-rw-rw-   0        0        0     2161 2024-03-01 23:04:15.000000 COMPAS-2.1.0/src/compas_ghpython/components/ghuser/Compas_ToJson.ghuser
--rw-rw-rw-   0        0        0     2067 2024-03-01 23:04:15.000000 COMPAS-2.1.0/src/compas_ghpython/components/ghuser/Compas_ToRhinoGeometry.ghuser
--rw-rw-rw-   0        0        0      775 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/install.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.229714 COMPAS-2.1.0/src/compas_ghpython/scene/
--rw-rw-rw-   0        0        0     4129 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/__init__.py
--rw-rw-rw-   0        0        0     1074 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/boxobject.py
--rw-rw-rw-   0        0        0     1109 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/brepobject.py
--rw-rw-rw-   0        0        0     1160 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/capsuleobject.py
--rw-rw-rw-   0        0        0     1081 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/circleobject.py
--rw-rw-rw-   0        0        0     1096 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/coneobject.py
--rw-rw-rw-   0        0        0     1078 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/curveobject.py
--rw-rw-rw-   0        0        0     1104 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/cylinderobject.py
--rw-rw-rw-   0        0        0     1096 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/ellipseobject.py
--rw-rw-rw-   0        0        0     2264 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/frameobject.py
--rw-rw-rw-   0        0        0     2182 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/graphobject.py
--rw-rw-rw-   0        0        0     1022 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/lineobject.py
--rw-rw-rw-   0        0        0     4384 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/meshobject.py
--rw-rw-rw-   0        0        0     2041 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/planeobject.py
--rw-rw-rw-   0        0        0     1034 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/pointobject.py
--rw-rw-rw-   0        0        0     1448 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/polygonobject.py
--rw-rw-rw-   0        0        0     1498 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/polyhedronobject.py
--rw-rw-rw-   0        0        0     1080 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/polylineobject.py
--rw-rw-rw-   0        0        0      331 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/sceneobject.py
--rw-rw-rw-   0        0        0     1085 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/sphereobject.py
--rw-rw-rw-   0        0        0     1100 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/surfaceobject.py
--rw-rw-rw-   0        0        0     1064 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/torusobject.py
--rw-rw-rw-   0        0        0     1468 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/vectorobject.py
--rw-rw-rw-   0        0        0     4990 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/scene/volmeshobject.py
--rw-rw-rw-   0        0        0     2450 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/sets.py
--rw-rw-rw-   0        0        0     1042 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/timer.py
--rw-rw-rw-   0        0        0     1033 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/uninstall.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.229714 COMPAS-2.1.0/src/compas_ghpython/utilities/
--rw-rw-rw-   0        0        0      585 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/utilities/__init__.py
--rw-rw-rw-   0        0        0    11766 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_ghpython/utilities/drawing.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.229714 COMPAS-2.1.0/src/compas_rhino/
--rw-rw-rw-   0        0        0    21202 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.229714 COMPAS-2.1.0/src/compas_rhino/conduits/
--rw-rw-rw-   0        0        0      335 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conduits/__init__.py
--rw-rw-rw-   0        0        0     2955 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conduits/base.py
--rw-rw-rw-   0        0        0     2706 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conduits/faces.py
--rw-rw-rw-   0        0        0     3511 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conduits/labels.py
--rw-rw-rw-   0        0        0     3371 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conduits/lines.py
--rw-rw-rw-   0        0        0     3252 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conduits/points.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.245340 COMPAS-2.1.0/src/compas_rhino/conversions/
--rw-rw-rw-   0        0        0     3989 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/__init__.py
--rw-rw-rw-   0        0        0     3052 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/breps.py
--rw-rw-rw-   0        0        0    10921 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/curves.py
--rw-rw-rw-   0        0        0        0 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/docobjects.py
--rw-rw-rw-   0        0        0      204 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/exceptions.py
--rw-rw-rw-   0        0        0     2373 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/extrusions.py
--rw-rw-rw-   0        0        0     3927 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/geometry.py
--rw-rw-rw-   0        0        0     8405 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/meshes.py
--rw-rw-rw-   0        0        0     7123 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/shapes.py
--rw-rw-rw-   0        0        0    10724 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/surfaces.py
--rw-rw-rw-   0        0        0     1144 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/conversions/transformations.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.245340 COMPAS-2.1.0/src/compas_rhino/geometry/
--rw-rw-rw-   0        0        0     1274 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/__init__.py
--rw-rw-rw-   0        0        0     3733 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/booleans.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.245340 COMPAS-2.1.0/src/compas_rhino/geometry/brep/
--rw-rw-rw-   0        0        0     1067 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/brep/__init__.py
--rw-rw-rw-   0        0        0    17716 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/brep/brep.py
--rw-rw-rw-   0        0        0     5400 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/brep/builder.py
--rw-rw-rw-   0        0        0     7904 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/brep/edge.py
--rw-rw-rw-   0        0        0    11108 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/brep/face.py
--rw-rw-rw-   0        0        0     3864 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/brep/loop.py
--rw-rw-rw-   0        0        0     3426 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/brep/trim.py
--rw-rw-rw-   0        0        0     2333 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/brep/vertex.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.245340 COMPAS-2.1.0/src/compas_rhino/geometry/curves/
--rw-rw-rw-   0        0        0     1342 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/curves/__init__.py
--rw-rw-rw-   0        0        0    11742 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/curves/curve.py
--rw-rw-rw-   0        0        0    10221 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/curves/nurbs.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.245340 COMPAS-2.1.0/src/compas_rhino/geometry/surfaces/
--rw-rw-rw-   0        0        0     1641 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/surfaces/__init__.py
--rw-rw-rw-   0        0        0    12152 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/surfaces/nurbs.py
--rw-rw-rw-   0        0        0    13105 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/surfaces/surface.py
--rw-rw-rw-   0        0        0    11345 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/trimesh_curvature.py
--rw-rw-rw-   0        0        0     2107 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/geometry/trimesh_slicing.py
--rw-rw-rw-   0        0        0    14557 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/install.py
--rw-rw-rw-   0        0        0     5433 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/install_plugin.py
--rw-rw-rw-   0        0        0      457 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/install_with_pip.py
--rw-rw-rw-   0        0        0     9597 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/layers.py
--rw-rw-rw-   0        0        0    30213 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/objects.py
--rw-rw-rw-   0        0        0      439 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/print_python_path.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.260955 COMPAS-2.1.0/src/compas_rhino/scene/
--rw-rw-rw-   0        0        0     4531 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/__init__.py
--rw-rw-rw-   0        0        0     1258 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/boxobject.py
--rw-rw-rw-   0        0        0     1185 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/brepobject.py
--rw-rw-rw-   0        0        0     1373 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/capsuleobject.py
--rw-rw-rw-   0        0        0     1231 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/circleobject.py
--rw-rw-rw-   0        0        0     1245 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/coneobject.py
--rw-rw-rw-   0        0        0     1219 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/curveobject.py
--rw-rw-rw-   0        0        0     1296 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/cylinderobject.py
--rw-rw-rw-   0        0        0     1278 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/ellipseobject.py
--rw-rw-rw-   0        0        0     3315 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/frameobject.py
--rw-rw-rw-   0        0        0    11572 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/graphobject.py
--rw-rw-rw-   0        0        0      801 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/helpers.py
--rw-rw-rw-   0        0        0     1192 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/lineobject.py
--rw-rw-rw-   0        0        0    22499 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/meshobject.py
--rw-rw-rw-   0        0        0     2238 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/planeobject.py
--rw-rw-rw-   0        0        0     1219 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/pointobject.py
--rw-rw-rw-   0        0        0     1330 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/polygonobject.py
--rw-rw-rw-   0        0        0     1435 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/polyhedronobject.py
--rw-rw-rw-   0        0        0     1255 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/polylineobject.py
--rw-rw-rw-   0        0        0     3436 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/sceneobject.py
--rw-rw-rw-   0        0        0     1266 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/sphereobject.py
--rw-rw-rw-   0        0        0     1235 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/surfaceobject.py
--rw-rw-rw-   0        0        0     1251 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/torusobject.py
--rw-rw-rw-   0        0        0     1499 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/vectorobject.py
--rw-rw-rw-   0        0        0    17308 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/scene/volmeshobject.py
--rw-rw-rw-   0        0        0     3569 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/ui.py
--rw-rw-rw-   0        0        0     8136 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/uninstall.py
--rw-rw-rw-   0        0        0     2545 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/uninstall_plugin.py
-drwxrwxrwx   0        0        0        0 2024-03-01 23:04:19.260955 COMPAS-2.1.0/src/compas_rhino/utilities/
--rw-rw-rw-   0        0        0      667 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/utilities/__init__.py
--rw-rw-rw-   0        0        0     2539 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/utilities/constructors.py
--rw-rw-rw-   0        0        0    33958 2024-03-01 23:01:37.000000 COMPAS-2.1.0/src/compas_rhino/utilities/drawing.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.733696 compas-2.1.1/
+-rw-rw-rw-   0        0        0     2899 2024-05-13 23:42:08.000000 compas-2.1.1/AUTHORS.md
+-rw-rw-rw-   0        0        0     1101 2024-05-13 23:42:08.000000 compas-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7041 2024-05-13 23:45:06.733696 compas-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3910 2024-05-13 23:42:08.000000 compas-2.1.1/README.md
+-rw-rw-rw-   0        0        0     4531 2024-05-13 23:42:08.000000 compas-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      126 2024-05-13 23:42:08.000000 compas-2.1.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0      116 2024-05-13 23:42:08.000000 compas-2.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 23:45:06.749320 compas-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.483701 compas-2.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.483701 compas-2.1.1/src/compas/
+-rw-rw-rw-   0        0        0     8252 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/__init__.py
+-rw-rw-rw-   0        0        0     1762 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/__main__.py
+-rw-rw-rw-   0        0        0     2476 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/_iotools.py
+-rw-rw-rw-   0        0        0    21048 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/_os.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.499325 compas-2.1.1/src/compas/colors/
+-rw-rw-rw-   0        0        0      397 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.530576 compas-2.1.1/src/compas/colors/cmcrameri/
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/acton.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/actonS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/bam.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/bamO.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/bamako.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/bamakoS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/batlow.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/batlowK.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/batlowS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/batlowW.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/berlin.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/bilbao.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/bilbaoS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/broc.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/brocO.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/buda.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/budaS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/bukavu.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/cork.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/corkO.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/davos.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/davosS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/devon.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/devonS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/fes.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/grayC.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/grayCS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/hawaii.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/hawaiiS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/imola.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/imolaS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/lajolla.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/lajollaS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/lapaz.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/lapazS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/lisbon.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/nuuk.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/nuukS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/oleron.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/oslo.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/osloS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/roma.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/romaO.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/tofino.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/tokyo.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/tokyoS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/turku.txt
+-rw-rw-rw-   0        0        0     2800 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/turkuS.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/vanimo.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/vik.txt
+-rw-rw-rw-   0        0        0     7168 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/cmcrameri/vikO.txt
+-rw-rw-rw-   0        0        0    28415 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/color.py
+-rw-rw-rw-   0        0        0     2528 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/colordict.py
+-rw-rw-rw-   0        0        0     9500 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/colormap.py
+-rw-rw-rw-   0        0        0     5007 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/html_colors.py
+-rw-rw-rw-   0        0        0    39084 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/colors/mpl_colormap.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.530576 compas-2.1.1/src/compas/data/
+-rw-rw-rw-   0        0        0      938 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/__init__.py
+-rw-rw-rw-   0        0        0     1810 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/coercion.py
+-rw-rw-rw-   0        0        0      325 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/conftest.py
+-rw-rw-rw-   0        0        0     9859 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/data.py
+-rw-rw-rw-   0        0        0     6821 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/encoders.py
+-rw-rw-rw-   0        0        0      169 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/exceptions.py
+-rw-rw-rw-   0        0        0     6504 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/json.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.546198 compas-2.1.1/src/compas/data/samples/
+-rw-rw-rw-   0        0        0     3063 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/boxes.obj
+-rw-rw-rw-   0        0        0    65931 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/butt_model.obj
+-rw-rw-rw-   0        0        0     3184 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/cone.stl
+-rw-rw-rw-   0        0        0      135 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/cube.off
+-rw-rw-rw-   0        0        0  1394975 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/cube_ascii.stl
+-rw-rw-rw-   0        0        0      684 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/cube_binary.stl
+-rw-rw-rw-   0        0        0      684 2024-05-13 23:43:59.000000 compas-2.1.1/src/compas/data/samples/cube_binary_2.stl
+-rw-rw-rw-   0        0        0  4063805 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/doosabin.json
+-rw-rw-rw-   0        0        0      702 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/faces.obj
+-rw-rw-rw-   0        0        0   301165 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/faces_big.obj
+-rw-rw-rw-   0        0        0      702 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/faces_reversed.obj
+-rw-rw-rw-   0        0        0     2000 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/fink.obj
+-rw-rw-rw-   0        0        0     5921 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/grid_irregular.obj
+-rw-rw-rw-   0        0        0     2442 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/hypar.obj
+-rw-rw-rw-   0        0        0     1672 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/lines.json
+-rw-rw-rw-   0        0        0     3666 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/lines.obj
+-rw-rw-rw-   0        0        0   554153 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/lines_big.obj
+-rw-rw-rw-   0        0        0  2295689 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/lines_bigger.obj
+-rw-rw-rw-   0        0        0     5409 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/lines_noleaves.obj
+-rw-rw-rw-   0        0        0    25178 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/mesh.obj
+-rw-rw-rw-   0        0        0    42388 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/mesh_100_faces.json
+-rw-rw-rw-   0        0        0    46729 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/mesh_110_faces.json
+-rw-rw-rw-   0        0        0     5023 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/open_edges.obj
+-rw-rw-rw-   0        0        0       60 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/point.json
+-rw-rw-rw-   0        0        0     6725 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/quadmesh.obj
+-rw-rw-rw-   0        0        0     3289 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/quadmesh_planar.obj
+-rw-rw-rw-   0        0        0     3914 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/saddle.obj
+-rw-rw-rw-   0        0        0     1331 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/spline.obj
+-rw-rw-rw-   0        0        0    37882 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/tubemesh.json
+-rw-rw-rw-   0        0        0     7287 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/tubemesh.obj
+-rw-rw-rw-   0        0        0     7153 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/tubemesh.off
+-rw-rw-rw-   0        0        0     8978 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/samples/tubemesh.ply
+-rw-rw-rw-   0        0        0     3292 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/schema.py
+-rw-rw-rw-   0        0        0     4777 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/data/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.546198 compas-2.1.1/src/compas/datastructures/
+-rw-rw-rw-   0        0        0     2409 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/__init__.py
+-rw-rw-rw-   0        0        0     4746 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/_mutablemapping.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.561820 compas-2.1.1/src/compas/datastructures/assembly/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/assembly/__init__.py
+-rw-rw-rw-   0        0        0     7221 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/assembly/assembly.py
+-rw-rw-rw-   0        0        0       89 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/assembly/exceptions.py
+-rw-rw-rw-   0        0        0     7321 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/assembly/part.py
+-rw-rw-rw-   0        0        0     3023 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/attributes.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.561820 compas-2.1.1/src/compas/datastructures/cell_network/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/cell_network/__init__.py
+-rw-rw-rw-   0        0        0   131244 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/cell_network/cell_network.py
+-rw-rw-rw-   0        0        0     7536 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/datastructure.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.561820 compas-2.1.1/src/compas/datastructures/graph/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/graph/__init__.py
+-rw-rw-rw-   0        0        0     5976 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/graph/duality.py
+-rw-rw-rw-   0        0        0    74955 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/graph/graph.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.561820 compas-2.1.1/src/compas/datastructures/graph/operations/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/graph/operations/__init__.py
+-rw-rw-rw-   0        0        0     4045 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/graph/operations/join.py
+-rw-rw-rw-   0        0        0     1507 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/graph/operations/split.py
+-rw-rw-rw-   0        0        0     7776 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/graph/planarity.py
+-rw-rw-rw-   0        0        0     1689 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/graph/smoothing.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.561820 compas-2.1.1/src/compas/datastructures/mesh/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/__init__.py
+-rw-rw-rw-   0        0        0    17259 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/conway.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/duality.py
+-rw-rw-rw-   0        0        0   161117 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/mesh.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.577451 compas-2.1.1/src/compas/datastructures/mesh/operations/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/operations/__init__.py
+-rw-rw-rw-   0        0        0    10232 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/operations/collapse.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/operations/extrude.py
+-rw-rw-rw-   0        0        0     3640 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/operations/insert.py
+-rw-rw-rw-   0        0        0     2412 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/operations/merge.py
+-rw-rw-rw-   0        0        0     6859 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/operations/split.py
+-rw-rw-rw-   0        0        0     1043 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/operations/substitute.py
+-rw-rw-rw-   0        0        0     1573 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/operations/swap.py
+-rw-rw-rw-   0        0        0     3505 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/operations/weld.py
+-rw-rw-rw-   0        0        0     7207 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/remesh.py
+-rw-rw-rw-   0        0        0     5674 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/slice.py
+-rw-rw-rw-   0        0        0     5683 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/smoothing.py
+-rw-rw-rw-   0        0        0    23898 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/mesh/subdivision.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.577451 compas-2.1.1/src/compas/datastructures/tree/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/tree/__init__.py
+-rw-rw-rw-   0        0        0    14704 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/tree/tree.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.577451 compas-2.1.1/src/compas/datastructures/volmesh/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/volmesh/__init__.py
+-rw-rw-rw-   0        0        0   130448 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/datastructures/volmesh/volmesh.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.577451 compas-2.1.1/src/compas/files/
+-rw-rw-rw-   0        0        0      953 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.577451 compas-2.1.1/src/compas/files/_xml/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/_xml/__init__.py
+-rw-rw-rw-   0        0        0     7505 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/_xml/xml_cli.py
+-rw-rw-rw-   0        0        0      971 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/_xml/xml_cpython.py
+-rw-rw-rw-   0        0        0     1755 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/_xml/xml_pre_38.py
+-rw-rw-rw-   0        0        0     1254 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/_xml/xml_shared.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.593074 compas-2.1.1/src/compas/files/gltf/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/__init__.py
+-rw-rw-rw-   0        0        0     1262 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/constants.py
+-rw-rw-rw-   0        0        0    24730 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/data_classes.py
+-rw-rw-rw-   0        0        0    12212 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/extensions.py
+-rw-rw-rw-   0        0        0     2724 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/gltf.py
+-rw-rw-rw-   0        0        0     1720 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/gltf_children.py
+-rw-rw-rw-   0        0        0    21599 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/gltf_content.py
+-rw-rw-rw-   0        0        0    19333 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/gltf_exporter.py
+-rw-rw-rw-   0        0        0     9062 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/gltf_mesh.py
+-rw-rw-rw-   0        0        0    12274 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/gltf_node.py
+-rw-rw-rw-   0        0        0     5105 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/gltf_parser.py
+-rw-rw-rw-   0        0        0    11391 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/gltf_reader.py
+-rw-rw-rw-   0        0        0     3686 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/gltf_scene.py
+-rw-rw-rw-   0        0        0     2394 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/gltf/helpers.py
+-rw-rw-rw-   0        0        0    21842 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/obj.py
+-rw-rw-rw-   0        0        0     8529 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/off.py
+-rw-rw-rw-   0        0        0    23411 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/ply.py
+-rw-rw-rw-   0        0        0    13171 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/stl.py
+-rw-rw-rw-   0        0        0     8440 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/files/xml.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.608696 compas-2.1.1/src/compas/geometry/
+-rw-rw-rw-   0        0        0    21424 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.624325 compas-2.1.1/src/compas/geometry/_core/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/__init__.py
+-rw-rw-rw-   0        0        0    75155 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/_algebra.py
+-rw-rw-rw-   0        0        0    11442 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/angles.py
+-rw-rw-rw-   0        0        0    15920 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/centroids.py
+-rw-rw-rw-   0        0        0    26634 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/distance.py
+-rw-rw-rw-   0        0        0     3627 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/normals.py
+-rw-rw-rw-   0        0        0     9423 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/nurbs.py
+-rw-rw-rw-   0        0        0    21355 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/predicates_2.py
+-rw-rw-rw-   0        0        0    36763 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/predicates_3.py
+-rw-rw-rw-   0        0        0     5027 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/quaternions.py
+-rw-rw-rw-   0        0        0     5801 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/size.py
+-rw-rw-rw-   0        0        0     1426 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/tangent.py
+-rw-rw-rw-   0        0        0    32735 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/transformations.py
+-rw-rw-rw-   0        0        0     8312 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/_core/transformations_numpy.py
+-rw-rw-rw-   0        0        0     3679 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/bbox.py
+-rw-rw-rw-   0        0        0     8970 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/bbox_numpy.py
+-rw-rw-rw-   0        0        0     2269 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/bestfit.py
+-rw-rw-rw-   0        0        0     7845 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/bestfit_numpy.py
+-rw-rw-rw-   0        0        0    10230 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/booleans.py
+-rw-rw-rw-   0        0        0     4477 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/booleans_shapely.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.624325 compas-2.1.1/src/compas/geometry/brep/
+-rw-rw-rw-   0        0        0     2493 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/brep/__init__.py
+-rw-rw-rw-   0        0        0    29530 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/brep/brep.py
+-rw-rw-rw-   0        0        0     7485 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/brep/edge.py
+-rw-rw-rw-   0        0        0      492 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/brep/errors.py
+-rw-rw-rw-   0        0        0     8917 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/brep/face.py
+-rw-rw-rw-   0        0        0     2263 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/brep/loop.py
+-rw-rw-rw-   0        0        0     1099 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/brep/trim.py
+-rw-rw-rw-   0        0        0     1287 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/brep/vertex.py
+-rw-rw-rw-   0        0        0      969 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/contours.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.624325 compas-2.1.1/src/compas/geometry/curves/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/__init__.py
+-rw-rw-rw-   0        0        0    13996 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/arc.py
+-rw-rw-rw-   0        0        0     9657 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/bezier.py
+-rw-rw-rw-   0        0        0    15587 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/circle.py
+-rw-rw-rw-   0        0        0      488 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/conic.py
+-rw-rw-rw-   0        0        0    17728 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/curve.py
+-rw-rw-rw-   0        0        0    12854 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/ellipse.py
+-rw-rw-rw-   0        0        0    10220 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/hyperbola.py
+-rw-rw-rw-   0        0        0    13121 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/line.py
+-rw-rw-rw-   0        0        0    11682 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/nurbs.py
+-rw-rw-rw-   0        0        0     7552 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/parabola.py
+-rw-rw-rw-   0        0        0    24246 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/curves/polyline.py
+-rw-rw-rw-   0        0        0    25207 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/frame.py
+-rw-rw-rw-   0        0        0     7040 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/geometry.py
+-rw-rw-rw-   0        0        0     4718 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/hull.py
+-rw-rw-rw-   0        0        0     1922 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/hull_numpy.py
+-rw-rw-rw-   0        0        0     3123 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/icp_numpy.py
+-rw-rw-rw-   0        0        0     1077 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/interpolation_barycentric.py
+-rw-rw-rw-   0        0        0     3659 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/interpolation_coons.py
+-rw-rw-rw-   0        0        0     2644 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/interpolation_tweening.py
+-rw-rw-rw-   0        0        0     2776 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/intersection.py
+-rw-rw-rw-   0        0        0    35767 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/intersections.py
+-rw-rw-rw-   0        0        0     4836 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/kdtree.py
+-rw-rw-rw-   0        0        0     6852 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/offset.py
+-rw-rw-rw-   0        0        0     3204 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/pca_numpy.py
+-rw-rw-rw-   0        0        0    19189 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/plane.py
+-rw-rw-rw-   0        0        0    19039 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/point.py
+-rw-rw-rw-   0        0        0    12336 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/pointcloud.py
+-rw-rw-rw-   0        0        0    15386 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/polygon.py
+-rw-rw-rw-   0        0        0    18976 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/polyhedron.py
+-rw-rw-rw-   0        0        0     5384 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/projection.py
+-rw-rw-rw-   0        0        0      784 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/quadmesh_planarize.py
+-rw-rw-rw-   0        0        0     3727 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/quadmesh_planarize_none.py
+-rw-rw-rw-   0        0        0    15064 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/quaternion.py
+-rw-rw-rw-   0        0        0     3507 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/reflection.py
+-rw-rw-rw-   0        0        0    12478 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/rotation.py
+-rw-rw-rw-   0        0        0     3503 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/scale.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.639946 compas-2.1.1/src/compas/geometry/shapes/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/shapes/__init__.py
+-rw-rw-rw-   0        0        0    22067 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/shapes/box.py
+-rw-rw-rw-   0        0        0    14585 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/shapes/capsule.py
+-rw-rw-rw-   0        0        0     9833 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/shapes/cone.py
+-rw-rw-rw-   0        0        0    11367 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/shapes/cylinder.py
+-rw-rw-rw-   0        0        0     9181 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/shapes/shape.py
+-rw-rw-rw-   0        0        0    11305 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/shapes/sphere.py
+-rw-rw-rw-   0        0        0     9661 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/shapes/torus.py
+-rw-rw-rw-   0        0        0     3980 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/shear.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.639946 compas-2.1.1/src/compas/geometry/surfaces/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/__init__.py
+-rw-rw-rw-   0        0        0     5099 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/conical.py
+-rw-rw-rw-   0        0        0     7315 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/cylindrical.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/extrusion.py
+-rw-rw-rw-   0        0        0    11532 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/nurbs.py
+-rw-rw-rw-   0        0        0     7031 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/planar.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/revolution.py
+-rw-rw-rw-   0        0        0     7533 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/spherical.py
+-rw-rw-rw-   0        0        0    19317 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/surface.py
+-rw-rw-rw-   0        0        0     6211 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/surfaces/toroidal.py
+-rw-rw-rw-   0        0        0    18110 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/transformation.py
+-rw-rw-rw-   0        0        0     3107 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/translation.py
+-rw-rw-rw-   0        0        0     2928 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/triangulation_delaunay.py
+-rw-rw-rw-   0        0        0     9810 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/triangulation_earclip.py
+-rw-rw-rw-   0        0        0     3146 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_curvature.py
+-rw-rw-rw-   0        0        0      661 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_descent_numpy.py
+-rw-rw-rw-   0        0        0      978 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_geodistance.py
+-rw-rw-rw-   0        0        0     2533 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_gradient_numpy.py
+-rw-rw-rw-   0        0        0     1089 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_isolines.py
+-rw-rw-rw-   0        0        0      742 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_matrices.py
+-rw-rw-rw-   0        0        0     5335 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_matrices_numpy.py
+-rw-rw-rw-   0        0        0     1290 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_parametrisation.py
+-rw-rw-rw-   0        0        0     7699 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_pull_points_numpy.py
+-rw-rw-rw-   0        0        0     3034 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_remeshing.py
+-rw-rw-rw-   0        0        0     4138 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_samplepoints_numpy.py
+-rw-rw-rw-   0        0        0      779 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_slicing.py
+-rw-rw-rw-   0        0        0      973 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/trimesh_smoothing_numpy.py
+-rw-rw-rw-   0        0        0    23101 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/geometry/vector.py
+-rw-rw-rw-   0        0        0    12588 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/itertools.py
+-rw-rw-rw-   0        0        0    15780 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/linalg.py
+-rw-rw-rw-   0        0        0     8962 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/matrices.py
+-rw-rw-rw-   0        0        0    16971 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/plugins.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.639946 compas-2.1.1/src/compas/rpc/
+-rw-rw-rw-   0        0        0     1042 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/rpc/__init__.py
+-rw-rw-rw-   0        0        0     2144 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/rpc/__main__.py
+-rw-rw-rw-   0        0        0     5706 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/rpc/dispatcher.py
+-rw-rw-rw-   0        0        0      310 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/rpc/errors.py
+-rw-rw-rw-   0        0        0    15420 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/rpc/proxy.py
+-rw-rw-rw-   0        0        0     2100 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/rpc/server.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.639946 compas-2.1.1/src/compas/rpc/services/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/rpc/services/__init__.py
+-rw-rw-rw-   0        0        0     2393 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/rpc/services/default.py
+-rw-rw-rw-   0        0        0     1520 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/rpc/services/watcher.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.655568 compas-2.1.1/src/compas/scene/
+-rw-rw-rw-   0        0        0     1793 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/__init__.py
+-rw-rw-rw-   0        0        0      112 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/assemblyobject.py
+-rw-rw-rw-   0        0        0     4024 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/context.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.655568 compas-2.1.1/src/compas/scene/descriptors/
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/descriptors/__init__.py
+-rw-rw-rw-   0        0        0      911 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/descriptors/attribute.py
+-rw-rw-rw-   0        0        0     2719 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/descriptors/color.py
+-rw-rw-rw-   0        0        0     2963 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/descriptors/colordict.py
+-rw-rw-rw-   0        0        0      440 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/descriptors/protocol.py
+-rw-rw-rw-   0        0        0      259 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/exceptions.py
+-rw-rw-rw-   0        0        0     2117 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/geometryobject.py
+-rw-rw-rw-   0        0        0     5606 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/graphobject.py
+-rw-rw-rw-   0        0        0     7653 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/meshobject.py
+-rw-rw-rw-   0        0        0     4767 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/scene.py
+-rw-rw-rw-   0        0        0     9442 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/sceneobject.py
+-rw-rw-rw-   0        0        0     8978 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/scene/volmeshobject.py
+-rw-rw-rw-   0        0        0    25801 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/tolerance.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.655568 compas-2.1.1/src/compas/topology/
+-rw-rw-rw-   0        0        0     1153 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/topology/__init__.py
+-rw-rw-rw-   0        0        0     3641 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/topology/combinatorics.py
+-rw-rw-rw-   0        0        0     2988 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/topology/connectivity.py
+-rw-rw-rw-   0        0        0     6341 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/topology/orientation.py
+-rw-rw-rw-   0        0        0    19366 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/topology/traversal.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.655568 compas-2.1.1/src/compas/utilities/
+-rw-rw-rw-   0        0        0      515 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/utilities/__init__.py
+-rw-rw-rw-   0        0        0     4648 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/utilities/azync.py
+-rw-rw-rw-   0        0        0      708 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/utilities/datetime.py
+-rw-rw-rw-   0        0        0     3089 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/utilities/decorators.py
+-rw-rw-rw-   0        0        0     1542 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/utilities/remote.py
+-rw-rw-rw-   0        0        0     4360 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas/utilities/ssh.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.733696 compas-2.1.1/src/compas.egg-info/
+-rw-rw-rw-   0        0        0     7041 2024-05-13 23:45:06.000000 compas-2.1.1/src/compas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17815 2024-05-13 23:45:06.000000 compas-2.1.1/src/compas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 23:45:06.000000 compas-2.1.1/src/compas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-13 23:45:06.000000 compas-2.1.1/src/compas.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-13 23:42:36.000000 compas-2.1.1/src/compas.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      213 2024-05-13 23:45:06.000000 compas-2.1.1/src/compas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2024-05-13 23:45:06.000000 compas-2.1.1/src/compas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.655568 compas-2.1.1/src/compas_blender/
+-rw-rw-rw-   0        0        0     8388 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/__init__.py
+-rw-rw-rw-   0        0        0     3344 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/collections.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.671196 compas-2.1.1/src/compas_blender/conversions/
+-rw-rw-rw-   0        0        0     1528 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/conversions/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/conversions/breps.py
+-rw-rw-rw-   0        0        0      594 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/conversions/colors.py
+-rw-rw-rw-   0        0        0     3209 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/conversions/curves.py
+-rw-rw-rw-   0        0        0     4454 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/conversions/geometry.py
+-rw-rw-rw-   0        0        0     3721 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/conversions/meshes.py
+-rw-rw-rw-   0        0        0     1552 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/conversions/surfaces.py
+-rw-rw-rw-   0        0        0     1231 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/conversions/transformations.py
+-rw-rw-rw-   0        0        0      749 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/data.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.671196 compas-2.1.1/src/compas_blender/geometry/
+-rw-rw-rw-   0        0        0      386 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/geometry/__init__.py
+-rw-rw-rw-   0        0        0     3358 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/geometry/booleans.py
+-rw-rw-rw-   0        0        0    12667 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/install.py
+-rw-rw-rw-   0        0        0     8393 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/objects.py
+-rw-rw-rw-   0        0        0      440 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/print_python_path.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.686823 compas-2.1.1/src/compas_blender/scene/
+-rw-rw-rw-   0        0        0     4114 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/__init__.py
+-rw-rw-rw-   0        0        0     2064 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/boxobject.py
+-rw-rw-rw-   0        0        0     2351 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/capsuleobject.py
+-rw-rw-rw-   0        0        0     1627 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/circleobject.py
+-rw-rw-rw-   0        0        0     2208 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/coneobject.py
+-rw-rw-rw-   0        0        0     1722 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/curveobject.py
+-rw-rw-rw-   0        0        0     2260 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/cylinderobject.py
+-rw-rw-rw-   0        0        0     3313 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/frameobject.py
+-rw-rw-rw-   0        0        0     9219 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/graphobject.py
+-rw-rw-rw-   0        0        0     1783 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/lineobject.py
+-rw-rw-rw-   0        0        0    18055 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/meshobject.py
+-rw-rw-rw-   0        0        0     2723 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/planeobject.py
+-rw-rw-rw-   0        0        0     2122 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/pointcloudobject.py
+-rw-rw-rw-   0        0        0     2007 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/pointobject.py
+-rw-rw-rw-   0        0        0     1729 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/polygonobject.py
+-rw-rw-rw-   0        0        0     1948 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/polyhedronobject.py
+-rw-rw-rw-   0        0        0     1660 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/polylineobject.py
+-rw-rw-rw-   0        0        0     7639 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/sceneobject.py
+-rw-rw-rw-   0        0        0     2336 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/sphereobject.py
+-rw-rw-rw-   0        0        0     1652 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/surfaceobject.py
+-rw-rw-rw-   0        0        0     2344 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/torusobject.py
+-rw-rw-rw-   0        0        0     2117 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/vectorobject.py
+-rw-rw-rw-   0        0        0    17605 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/scene/volmeshobject.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.686823 compas-2.1.1/src/compas_blender/utilities/
+-rw-rw-rw-   0        0        0      663 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/utilities/__init__.py
+-rw-rw-rw-   0        0        0    27131 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_blender/utilities/drawing.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.686823 compas-2.1.1/src/compas_ghpython/
+-rw-rw-rw-   0        0        0     3998 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.686823 compas-2.1.1/src/compas_ghpython/components/
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.686823 compas-2.1.1/src/compas_ghpython/components/Compas_FromJson/
+-rw-rw-rw-   0        0        0      387 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/components/Compas_FromJson/code.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.686823 compas-2.1.1/src/compas_ghpython/components/Compas_Info/
+-rw-rw-rw-   0        0        0      451 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/components/Compas_Info/code.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.686823 compas-2.1.1/src/compas_ghpython/components/Compas_RpcCall/
+-rw-rw-rw-   0        0        0      839 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/components/Compas_RpcCall/code.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.686823 compas-2.1.1/src/compas_ghpython/components/Compas_ToJson/
+-rw-rw-rw-   0        0        0      413 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/components/Compas_ToJson/code.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.686823 compas-2.1.1/src/compas_ghpython/components/Compas_ToRhinoGeometry/
+-rw-rw-rw-   0        0        0      323 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/components/Compas_ToRhinoGeometry/code.py
+-rw-rw-rw-   0        0        0     2830 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/components/__init__.py
+-rw-rw-rw-   0        0        0      775 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/install.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.702449 compas-2.1.1/src/compas_ghpython/scene/
+-rw-rw-rw-   0        0        0     4129 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/__init__.py
+-rw-rw-rw-   0        0        0     1074 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/boxobject.py
+-rw-rw-rw-   0        0        0     1109 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/brepobject.py
+-rw-rw-rw-   0        0        0     1160 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/capsuleobject.py
+-rw-rw-rw-   0        0        0     1081 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/circleobject.py
+-rw-rw-rw-   0        0        0     1096 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/coneobject.py
+-rw-rw-rw-   0        0        0     1078 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/curveobject.py
+-rw-rw-rw-   0        0        0     1104 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/cylinderobject.py
+-rw-rw-rw-   0        0        0     1096 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/ellipseobject.py
+-rw-rw-rw-   0        0        0     2264 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/frameobject.py
+-rw-rw-rw-   0        0        0     2182 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/graphobject.py
+-rw-rw-rw-   0        0        0     1022 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/lineobject.py
+-rw-rw-rw-   0        0        0     4386 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/meshobject.py
+-rw-rw-rw-   0        0        0     2017 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/planeobject.py
+-rw-rw-rw-   0        0        0     1034 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/pointobject.py
+-rw-rw-rw-   0        0        0     1446 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/polygonobject.py
+-rw-rw-rw-   0        0        0     1496 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/polyhedronobject.py
+-rw-rw-rw-   0        0        0     1080 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/polylineobject.py
+-rw-rw-rw-   0        0        0      331 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/sceneobject.py
+-rw-rw-rw-   0        0        0     1085 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/sphereobject.py
+-rw-rw-rw-   0        0        0     1100 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/surfaceobject.py
+-rw-rw-rw-   0        0        0     1064 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/torusobject.py
+-rw-rw-rw-   0        0        0     1468 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/vectorobject.py
+-rw-rw-rw-   0        0        0     4990 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/scene/volmeshobject.py
+-rw-rw-rw-   0        0        0     2450 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/sets.py
+-rw-rw-rw-   0        0        0     1042 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/timer.py
+-rw-rw-rw-   0        0        0     1033 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/uninstall.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.702449 compas-2.1.1/src/compas_ghpython/utilities/
+-rw-rw-rw-   0        0        0      585 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11544 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_ghpython/utilities/drawing.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.702449 compas-2.1.1/src/compas_rhino/
+-rw-rw-rw-   0        0        0    21202 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.702449 compas-2.1.1/src/compas_rhino/conduits/
+-rw-rw-rw-   0        0        0      335 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conduits/__init__.py
+-rw-rw-rw-   0        0        0     2955 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conduits/base.py
+-rw-rw-rw-   0        0        0     2706 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conduits/faces.py
+-rw-rw-rw-   0        0        0     3476 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conduits/labels.py
+-rw-rw-rw-   0        0        0     3370 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conduits/lines.py
+-rw-rw-rw-   0        0        0     3252 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conduits/points.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.718070 compas-2.1.1/src/compas_rhino/conversions/
+-rw-rw-rw-   0        0        0     3989 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/__init__.py
+-rw-rw-rw-   0        0        0     3048 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/breps.py
+-rw-rw-rw-   0        0        0    10915 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/curves.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/docobjects.py
+-rw-rw-rw-   0        0        0      204 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/exceptions.py
+-rw-rw-rw-   0        0        0     2371 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/extrusions.py
+-rw-rw-rw-   0        0        0     4283 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/geometry.py
+-rw-rw-rw-   0        0        0     8414 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/meshes.py
+-rw-rw-rw-   0        0        0     7105 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/shapes.py
+-rw-rw-rw-   0        0        0    10709 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/surfaces.py
+-rw-rw-rw-   0        0        0     1144 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/conversions/transformations.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.718070 compas-2.1.1/src/compas_rhino/geometry/
+-rw-rw-rw-   0        0        0     1274 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/__init__.py
+-rw-rw-rw-   0        0        0     3733 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/booleans.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.718070 compas-2.1.1/src/compas_rhino/geometry/brep/
+-rw-rw-rw-   0        0        0     1067 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/brep/__init__.py
+-rw-rw-rw-   0        0        0    18602 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/brep/brep.py
+-rw-rw-rw-   0        0        0     5400 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/brep/builder.py
+-rw-rw-rw-   0        0        0     7902 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/brep/edge.py
+-rw-rw-rw-   0        0        0    11056 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/brep/face.py
+-rw-rw-rw-   0        0        0     3838 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/brep/loop.py
+-rw-rw-rw-   0        0        0     3426 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/brep/trim.py
+-rw-rw-rw-   0        0        0     2333 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/brep/vertex.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.718070 compas-2.1.1/src/compas_rhino/geometry/curves/
+-rw-rw-rw-   0        0        0     1342 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/curves/__init__.py
+-rw-rw-rw-   0        0        0    11740 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/curves/curve.py
+-rw-rw-rw-   0        0        0    10219 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/curves/nurbs.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.718070 compas-2.1.1/src/compas_rhino/geometry/surfaces/
+-rw-rw-rw-   0        0        0     1641 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/surfaces/__init__.py
+-rw-rw-rw-   0        0        0    12102 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/surfaces/nurbs.py
+-rw-rw-rw-   0        0        0    13077 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/surfaces/surface.py
+-rw-rw-rw-   0        0        0    11321 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/trimesh_curvature.py
+-rw-rw-rw-   0        0        0     2107 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/geometry/trimesh_slicing.py
+-rw-rw-rw-   0        0        0    14520 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/install.py
+-rw-rw-rw-   0        0        0     5431 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/install_plugin.py
+-rw-rw-rw-   0        0        0      459 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/install_with_pip.py
+-rw-rw-rw-   0        0        0     9638 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/layers.py
+-rw-rw-rw-   0        0        0    30141 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/objects.py
+-rw-rw-rw-   0        0        0      437 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/print_python_path.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.733696 compas-2.1.1/src/compas_rhino/scene/
+-rw-rw-rw-   0        0        0     4531 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/boxobject.py
+-rw-rw-rw-   0        0        0     1187 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/brepobject.py
+-rw-rw-rw-   0        0        0     1375 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/capsuleobject.py
+-rw-rw-rw-   0        0        0     1233 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/circleobject.py
+-rw-rw-rw-   0        0        0     1247 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/coneobject.py
+-rw-rw-rw-   0        0        0     1221 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/curveobject.py
+-rw-rw-rw-   0        0        0     1298 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/cylinderobject.py
+-rw-rw-rw-   0        0        0     1278 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/ellipseobject.py
+-rw-rw-rw-   0        0        0     3317 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/frameobject.py
+-rw-rw-rw-   0        0        0    11574 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/graphobject.py
+-rw-rw-rw-   0        0        0      801 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/helpers.py
+-rw-rw-rw-   0        0        0     1194 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/lineobject.py
+-rw-rw-rw-   0        0        0    22497 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/meshobject.py
+-rw-rw-rw-   0        0        0     2240 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/planeobject.py
+-rw-rw-rw-   0        0        0     1221 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/pointobject.py
+-rw-rw-rw-   0        0        0     1332 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/polygonobject.py
+-rw-rw-rw-   0        0        0     1437 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/polyhedronobject.py
+-rw-rw-rw-   0        0        0     1257 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/polylineobject.py
+-rw-rw-rw-   0        0        0     3438 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/sceneobject.py
+-rw-rw-rw-   0        0        0     1268 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/sphereobject.py
+-rw-rw-rw-   0        0        0     1237 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/surfaceobject.py
+-rw-rw-rw-   0        0        0     1253 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/torusobject.py
+-rw-rw-rw-   0        0        0     1501 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/vectorobject.py
+-rw-rw-rw-   0        0        0    17306 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/scene/volmeshobject.py
+-rw-rw-rw-   0        0        0     3571 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/ui.py
+-rw-rw-rw-   0        0        0     8140 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/uninstall.py
+-rw-rw-rw-   0        0        0     2543 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/uninstall_plugin.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:45:06.733696 compas-2.1.1/src/compas_rhino/utilities/
+-rw-rw-rw-   0        0        0      667 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2539 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/utilities/constructors.py
+-rw-rw-rw-   0        0        0    34453 2024-05-13 23:42:08.000000 compas-2.1.1/src/compas_rhino/utilities/drawing.py
```

### Comparing `COMPAS-2.1.0/AUTHORS.md` & `compas-2.1.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/LICENSE` & `compas-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/PKG-INFO` & `compas-2.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: COMPAS
-Version: 2.1.0
-Summary: The COMPAS framework
-Home-page: http://compas.dev
-Author: Tom Van Mele
-Author-email: van.mele@arch.ethz.ch
-License: MIT
-Project-URL: Documentation, http://compas.dev
-Project-URL: Forum, https://forum.compas-framework.org/
-Project-URL: Repository, https://github.com/compas-dev/compas
-Project-URL: Issues, https://github.com/compas-dev/compas/issues
-Keywords: architecture,engineering,fabrication,construction
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-Provides-Extra: numba
-License-File: LICENSE
-License-File: AUTHORS.md
-
 # The COMPAS framework
 
 ![build](https://github.com/compas-dev/compas/workflows/build/badge.svg)
 [![GitHub - License](https://img.shields.io/github/license/compas-dev/compas.svg)](https://github.com/compas-dev/compas)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/compas)](https://anaconda.org/conda-forge/compas)
 [![pip downloads](https://img.shields.io/pypi/dm/compas)](https://pypi.python.org/project/COMPAS)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/COMPAS.svg)](https://pypi.python.org/project/COMPAS)
@@ -49,51 +17,51 @@
 
 COMPAS has dedicated packages for working with Rhino, Grasshopper, and Blender, but it can be used in any environment that supports Python scripting. It is available on PyPI and conda-forge and can be easily installed using popular package managers on multiple platforms.
 
 ## COMPAS 2.0!
 
 We are working on a new major release of the framework, COMPAS 2.0!
 Therefore, be aware that the current version of the repository already contains some changes that are incompatible with the version 1 releases.
-The documentation of the latest stable version (COMPAS 1.17.6) [is available here](https://compas.dev/compas/1.17.6).
+The documentation of the latest stable version (COMPAS 1.17.9) [is available here](https://compas.dev/compas/1.17.9).
 
 ## Installation
 
 The recommended way to install **COMPAS** is to use [Anaconda/conda](https://conda.io/docs/):
 
 ```bash
 conda config --add channels conda-forge
-conda install COMPAS
+conda install compas
 ```
 
-For other installation options, see <https://compas.dev/compas/latest/installation.html>
+For other installation options, [see the user guide](https://compas.dev/compas/latest/userguide/installation.html)
 
 ## First Steps
 
-* <https://compas.dev/compas/latest/gettingstarted.html>
-* <https://compas.dev/compas/latest/tutorial.html>
-* <https://compas.dev/compas/latest/api.html>
+* [First steps](https://compas.dev/compas/latest/userguide/firststeps.html)
+* [Tutorials: geometry basics](https://compas.dev/compas/latest/userguide/basics.geometry.html)
+* [Tutorials: datastructures](https://compas.dev/compas/latest/userguide/basics.datastructures.html)
+* [API Reference](https://compas.dev/compas/latest/api/index.html)
 
 ## Questions and feedback
 
-The **COMPAS** framework has a forum: <https://forum.compas-framework.org/>
-for questions and discussions.
+The **COMPAS** framework has a [forum for questions and discussions](https://forum.compas-framework.org/).
 
 ## Issue tracker
 
 If you find a bug, please help us solve it by [filing a report](https://github.com/compas-dev/compas/issues).
 
 ## Contributing
 
-If you want to contribute, check out the [contribution guidelines](https://compas.dev/compas/latest/devguide.html).
+If you want to contribute, check out the [contribution guidelines](https://compas.dev/compas/latest/devguide/index.html).
 
 ## Changelog
 
-See changes between releases on the [changelog](https://compas.dev/compas/latest/changelog.html).
+See changes between releases on the [changelog](https://github.com/compas-dev/compas/blob/main/CHANGELOG.md).
 
 ## License
 
-The main library of **COMPAS** is [released under the MIT license](https://compas.dev/compas/latest/license.html).
+The main library of **COMPAS** is [released under the MIT license](https://compas.dev/compas/latest/userguide/license.html).
 
 ## Credits
 
 COMPAS is developed by a small team of core developers (`compas-dev`) and with the support of contributers from the open source community.
-See the [list of authors](AUTHORS.md) for a complete overview...
+See the [list of authors](https://github.com/compas-dev/compas/blob/main/AUTHORS.md) for a complete overview...
```

### Comparing `COMPAS-2.1.0/src/COMPAS.egg-info/SOURCES.txt` & `compas-2.1.1/src/compas.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 AUTHORS.md
-CHANGELOG.md
 LICENSE
-MANIFEST.in
 README.md
-conftest.py
 pyproject.toml
+requirements-dev.txt
 requirements.txt
-setup.cfg
-setup.py
-src/COMPAS.egg-info/PKG-INFO
-src/COMPAS.egg-info/SOURCES.txt
-src/COMPAS.egg-info/dependency_links.txt
-src/COMPAS.egg-info/entry_points.txt
-src/COMPAS.egg-info/not-zip-safe
-src/COMPAS.egg-info/requires.txt
-src/COMPAS.egg-info/top_level.txt
 src/compas/__init__.py
 src/compas/__main__.py
 src/compas/_iotools.py
 src/compas/_os.py
 src/compas/itertools.py
 src/compas/linalg.py
 src/compas/matrices.py
 src/compas/plugins.py
 src/compas/tolerance.py
+src/compas.egg-info/PKG-INFO
+src/compas.egg-info/SOURCES.txt
+src/compas.egg-info/dependency_links.txt
+src/compas.egg-info/entry_points.txt
+src/compas.egg-info/not-zip-safe
+src/compas.egg-info/requires.txt
+src/compas.egg-info/top_level.txt
 src/compas/colors/__init__.py
 src/compas/colors/color.py
 src/compas/colors/colordict.py
 src/compas/colors/colormap.py
 src/compas/colors/html_colors.py
 src/compas/colors/mpl_colormap.py
-src/compas/colors/cmcrameri/LICENSE
 src/compas/colors/cmcrameri/acton.txt
 src/compas/colors/cmcrameri/actonS.txt
 src/compas/colors/cmcrameri/bam.txt
 src/compas/colors/cmcrameri/bamO.txt
 src/compas/colors/cmcrameri/bamako.txt
 src/compas/colors/cmcrameri/bamakoS.txt
 src/compas/colors/cmcrameri/batlow.txt
@@ -320,15 +315,14 @@
 src/compas/topology/connectivity.py
 src/compas/topology/orientation.py
 src/compas/topology/traversal.py
 src/compas/utilities/__init__.py
 src/compas/utilities/azync.py
 src/compas/utilities/datetime.py
 src/compas/utilities/decorators.py
-src/compas/utilities/maps.py
 src/compas/utilities/remote.py
 src/compas/utilities/ssh.py
 src/compas_blender/__init__.py
 src/compas_blender/collections.py
 src/compas_blender/data.py
 src/compas_blender/install.py
 src/compas_blender/objects.py
@@ -371,33 +365,18 @@
 src/compas_ghpython/__init__.py
 src/compas_ghpython/install.py
 src/compas_ghpython/sets.py
 src/compas_ghpython/timer.py
 src/compas_ghpython/uninstall.py
 src/compas_ghpython/components/__init__.py
 src/compas_ghpython/components/Compas_FromJson/code.py
-src/compas_ghpython/components/Compas_FromJson/icon.png
-src/compas_ghpython/components/Compas_FromJson/metadata.json
 src/compas_ghpython/components/Compas_Info/code.py
-src/compas_ghpython/components/Compas_Info/icon.png
-src/compas_ghpython/components/Compas_Info/metadata.json
 src/compas_ghpython/components/Compas_RpcCall/code.py
-src/compas_ghpython/components/Compas_RpcCall/icon.png
-src/compas_ghpython/components/Compas_RpcCall/metadata.json
 src/compas_ghpython/components/Compas_ToJson/code.py
-src/compas_ghpython/components/Compas_ToJson/icon.png
-src/compas_ghpython/components/Compas_ToJson/metadata.json
 src/compas_ghpython/components/Compas_ToRhinoGeometry/code.py
-src/compas_ghpython/components/Compas_ToRhinoGeometry/icon.png
-src/compas_ghpython/components/Compas_ToRhinoGeometry/metadata.json
-src/compas_ghpython/components/ghuser/Compas_FromJson.ghuser
-src/compas_ghpython/components/ghuser/Compas_Info.ghuser
-src/compas_ghpython/components/ghuser/Compas_RpcCall.ghuser
-src/compas_ghpython/components/ghuser/Compas_ToJson.ghuser
-src/compas_ghpython/components/ghuser/Compas_ToRhinoGeometry.ghuser
 src/compas_ghpython/scene/__init__.py
 src/compas_ghpython/scene/boxobject.py
 src/compas_ghpython/scene/brepobject.py
 src/compas_ghpython/scene/capsuleobject.py
 src/compas_ghpython/scene/circleobject.py
 src/compas_ghpython/scene/coneobject.py
 src/compas_ghpython/scene/curveobject.py
```

### Comparing `COMPAS-2.1.0/src/compas/__init__.py` & `compas-2.1.1/src/compas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import print_function
 
 import os
-from distutils.version import LooseVersion
 
 import compas._os
 from compas._os import (
     is_windows,
     is_linux,
     is_osx,
     is_mono,
@@ -17,18 +16,16 @@
 from compas.data import json_dump, json_dumps, json_dumpz, json_load, json_loads, json_loadz
 
 
 __author__ = "Tom Van Mele and many others (see AUTHORS.md)"
 __copyright__ = "Copyright 2014-2022 - ETH Zurich, Copyright 2023 - COMPAS Association"
 __license__ = "MIT License"
 __email__ = "tom.v.mele@gmail.com"
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
-version = LooseVersion(compas.__version__)
-versionstring = version.vstring.split("-")[0]
 
 HERE = compas._os.realpath(os.path.dirname(__file__))
 """str: Path to the location of the compas package."""
 
 HOME = compas._os.absjoin(HERE, "../..")
 """str: Path to the root of the local installation."""
 
@@ -171,15 +168,15 @@
     constructors of the data structures.
 
     .. code-block:: python
 
         import compas
         from compas.datastructures import Mesh
 
-        mesh = Mesh.from_obj(compas.get('faces.obj'))
+        mesh = Mesh.from_obj(compas.get("faces.obj"))
 
     """
     filename = filename.strip("/")
 
     if filename.endswith("bunny.ply"):
         return get_bunny()
```

### Comparing `COMPAS-2.1.0/src/compas/__main__.py` & `compas-2.1.1/src/compas/__main__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/_iotools.py` & `compas-2.1.1/src/compas/_iotools.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """For the time being, these functions are only for internal use."""
 
-from contextlib import contextmanager
 import io
+from contextlib import contextmanager
 
 try:
     from urllib.request import urlopen
 except ImportError:
     from urllib2 import urlopen
```

### Comparing `COMPAS-2.1.0/src/compas/_os.py` & `compas-2.1.1/src/compas/_os.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 These are internal functions of the framework.
 Not intended to be used outside compas* packages.
 """
+
 import os
 import platform
 import re
 import shutil
 import subprocess
 import sys
 import tempfile
@@ -673,15 +674,16 @@
         r"Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders",
     )
     dir, type = _winreg.QueryValueEx(key, shell_folder_name)
     return dir
 
 
 def _get_win_folder_with_pywin32(csidl_name):
-    from win32com.shell import shellcon, shell
+    from win32com.shell import shell
+    from win32com.shell import shellcon
 
     dir = shell.SHGetFolderPath(0, getattr(shellcon, csidl_name), 0, 0)
     # Try to make this a unicode path because SHGetFolderPath does
     # not return unicode strings when there is unicode data in the
     # path.
     try:
         dir = str(dir) if PY3 else unicode(dir)  # noqa: F821
```

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/acton.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/acton.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/actonS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/actonS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/bam.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/bam.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/bamO.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/bamO.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/bamako.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/bamako.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/bamakoS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/bamakoS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/batlow.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/batlow.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/batlowK.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/batlowK.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/batlowS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/batlowS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/batlowW.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/batlowW.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/berlin.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/berlin.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/bilbao.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/bilbao.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/bilbaoS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/bilbaoS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/broc.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/broc.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/brocO.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/brocO.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/buda.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/buda.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/budaS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/budaS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/bukavu.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/bukavu.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/cork.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/cork.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/corkO.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/corkO.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/davos.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/davos.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/davosS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/davosS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/devon.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/devon.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/devonS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/devonS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/fes.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/fes.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/grayC.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/grayC.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/grayCS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/grayCS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/hawaii.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/hawaii.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/hawaiiS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/hawaiiS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/imola.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/imola.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/imolaS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/imolaS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/lajolla.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/lajolla.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/lajollaS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/lajollaS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/lapaz.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/lapaz.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/lapazS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/lapazS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/lisbon.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/lisbon.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/nuuk.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/nuuk.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/nuukS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/nuukS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/oleron.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/oleron.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/oslo.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/oslo.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/osloS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/osloS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/roma.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/roma.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/romaO.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/romaO.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/tofino.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/tofino.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/tokyo.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/tokyo.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/tokyoS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/tokyoS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/turku.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/turku.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/turkuS.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/turkuS.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/vanimo.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/vanimo.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/vik.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/vik.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/cmcrameri/vikO.txt` & `compas-2.1.1/src/compas/colors/cmcrameri/vikO.txt`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/color.py` & `compas-2.1.1/src/compas/colors/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,16 @@
         The amount of light that passes through, is emitted from, or is reflected from a particular area.
         Here, it expresses the preceived brightness of the color.
         Note that this is not the same as the "Lightness" of HLS or the "Value/Brightness" of HSV.
     saturation : float
         The perceived freedom of whiteness.
     is_light : bool
         If True, the color is considered light.
+    contrast : :class:`compas.colors.Color`
+        The contrasting color to the current color.
 
     Examples
     --------
     By default, this class will create a color with the RGB components in the range ``[0.0, 1.0]``.
 
     >>> Color(1, 0, 0)
     Color(1.0, 0.0, 0.0, alpha=1.0)
@@ -307,14 +309,18 @@
 
     @property
     def saturation(self):
         maxval = max(self.r, self.g, self.b)
         minval = min(self.r, self.g, self.b)
         return (maxval - minval) / maxval
 
+    @property
+    def contrast(self):
+        return self.darkened(25) if self.is_light else self.lightened(50)
+
     # --------------------------------------------------------------------------
     # Constructors
     # --------------------------------------------------------------------------
 
     @classmethod
     def from_rgb255(cls, r, g, b):  # type: (int, int, int) -> Color
         """Construct a color from RGB255 components.
@@ -902,16 +908,16 @@
 
         """
         if factor > 100 or factor < 0:
             raise ValueError("Percentage of increased lightness should be in the range 0-100.")
 
         factor = 1.0 + factor / 100
 
-        h, l, s = self.hls
-        r, g, b = colorsys.hls_to_rgb(h, min(1.0, l * factor), s)
+        hue, luminance, saturation = self.hls
+        r, g, b = colorsys.hls_to_rgb(hue, min(1.0, luminance * factor), saturation)
         self.r = r
         self.g = g
         self.b = b
 
     def lightened(self, factor=10):
         """Return a lightened copy of the color.
 
@@ -953,16 +959,16 @@
 
         """
         if factor > 100 or factor < 0:
             raise ValueError("Percentage of reduced lightness should be in the range 0-100.")
 
         factor = 1.0 - factor / 100
 
-        h, l, s = self.hls
-        r, g, b = colorsys.hls_to_rgb(h, max(0.0, l * factor), s)
+        hue, luminance, saturation = self.hls
+        r, g, b = colorsys.hls_to_rgb(hue, max(0.0, luminance * factor), saturation)
         self.r = r
         self.g = g
         self.b = b
 
     def darkened(self, factor=10):
         """Return a darkened copy of the color.
 
@@ -1028,16 +1034,16 @@
 
         """
         if factor > 100 or factor < 0:
             raise ValueError("Percentage of saturation should be in the range 0-100.")
 
         factor = 1.0 + factor / 100
 
-        h, l, s = self.hls
-        r, g, b = colorsys.hls_to_rgb(h, l, min(1.0, s * factor))
+        hue, luminance, saturation = self.hls
+        r, g, b = colorsys.hls_to_rgb(hue, luminance, min(1.0, saturation * factor))
         self.r = r
         self.g = g
         self.b = b
 
     def saturated(self, factor=10):
         """Return a saturated copy of the color.
 
@@ -1079,16 +1085,16 @@
 
         """
         if factor > 100 or factor < 0:
             raise ValueError("Percentage of desaturation should be in the range 0-100.")
 
         factor = 1.0 - factor / 100
 
-        h, l, s = self.hls
-        r, g, b = colorsys.hls_to_rgb(h, l, max(0.0, s * factor))
+        hue, luminance, saturation = self.hls
+        r, g, b = colorsys.hls_to_rgb(hue, luminance, max(0.0, saturation * factor))
         self.r = r
         self.g = g
         self.b = b
 
     def desaturated(self, factor=10):
         """Return a desaturated copy of the color.
```

### Comparing `COMPAS-2.1.0/src/compas/colors/colordict.py` & `compas-2.1.1/src/compas/colors/colordict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.data import Data
+
 from .color import Color
 
 
 class ColorDict(Data):
     """Class representing a dictionary of colors.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/colors/colormap.py` & `compas-2.1.1/src/compas/colors/colormap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import os
 
-from compas.utilities import linspace
+from compas.itertools import linspace
 
 from .color import Color
-from .mpl_colormap import _magma_data
 from .mpl_colormap import _inferno_data
+from .mpl_colormap import _magma_data
 from .mpl_colormap import _plasma_data
 from .mpl_colormap import _viridis_data
 
 mpl = {
     "magma": _magma_data,
     "inferno": _inferno_data,
     "plasma": _plasma_data,
@@ -38,24 +38,22 @@
     ------
     ValueError
         If the number of colors in the sequence is not 256.
 
     Examples
     --------
     >>> import random
-    >>> cmap = ColorMap.from_palette('bamako')
+    >>> cmap = ColorMap.from_palette("bamako")
     >>> for i in range(100):
     ...     color = cmap(random.random())
-    ...
 
-    >>> cmap = ColorMap.from_mpl('viridis')
+    >>> cmap = ColorMap.from_mpl("viridis")
     >>> n = 100
     >>> for i in range(n):
     ...     color = cmap(i, minval=0, maxval=n - 1)
-    ...
 
     See Also
     --------
     :class:`compas.colors.Color`
 
     """
```

### Comparing `COMPAS-2.1.0/src/compas/colors/html_colors.py` & `compas-2.1.1/src/compas/colors/html_colors.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/colors/mpl_colormap.py` & `compas-2.1.1/src/compas/colors/mpl_colormap.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/__init__.py` & `compas-2.1.1/src/compas/data/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/coercion.py` & `compas-2.1.1/src/compas/data/coercion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from .validators import is_item_iterable
 
 
 def coerce_sequence_of_tuple(sequence):
     """Make sure all items of a sequence are of type tuple.
 
@@ -18,15 +18,15 @@
     list[tuple]
         A list containing the items of the original sequence,
         with each iterable item converted to a tuple,
         and non-iterable items wrapped in a tuple.
 
     Examples
     --------
-    >>> items = coerce_sequence_of_tuple(['a', 1, (None, ), [2.0, 3.0]])
+    >>> items = coerce_sequence_of_tuple(["a", 1, (None,), [2.0, 3.0]])
     >>> is_sequence_of_tuple(items)
     True
 
     """
     items = []
     for item in sequence:
         if not isinstance(item, tuple):
@@ -51,15 +51,15 @@
     list[list]
         A list containing the items of the original sequence,
         with each iterable item converted to a list,
         and non-iterable items wrapped in a list.
 
     Examples
     --------
-    >>> items = coerce_sequence_of_list(['a', 1, (None, ), [2.0, 3.0]])
+    >>> items = coerce_sequence_of_list(["a", 1, (None,), [2.0, 3.0]])
     >>> is_sequence_of_list(items)
     True
 
     """
     items = []
     for item in sequence:
         if not isinstance(item, list):
```

### Comparing `COMPAS-2.1.0/src/compas/data/data.py` & `compas-2.1.1/src/compas/data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 try:
     from typing import TypeVar  # noqa: F401
 
     D = TypeVar("D", bound="Data")
 except ImportError:
     pass
 
 import hashlib
-from uuid import uuid4
-from uuid import UUID
 from copy import deepcopy
+from uuid import UUID
+from uuid import uuid4
 
 import compas
 
-
 # ==============================================================================
 # If you ever feel tempted to use ABCMeta in your code: don't, just DON'T.
 # Assigning __metaclass__ = ABCMeta to a class causes a severe memory leak/performance
 # degradation on IronPython 2.7.
 
 # See these issues for more details:
 # - https://github.com/compas-dev/compas/issues/562
@@ -299,18 +298,18 @@
         Returns
         -------
         bytes | str
 
         Examples
         --------
         >>> from compas.datastructures import Mesh
-        >>> mesh = Mesh.from_obj(compas.get('faces.obj'))
+        >>> mesh = Mesh.from_obj(compas.get("faces.obj"))
         >>> v1 = mesh.sha256()
         >>> v2 = mesh.sha256()
-        >>> mesh.vertex_attribute(mesh.vertex_sample(1)[0], 'z', 1)
+        >>> mesh.vertex_attribute(mesh.vertex_sample(1)[0], "z", 1)
         >>> v3 = mesh.sha256()
         >>> v1 == v2
         True
         >>> v2 == v3
         False
 
         """
```

### Comparing `COMPAS-2.1.0/src/compas/data/encoders.py` & `compas-2.1.1/src/compas/data/encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 try:
     from typing import Type  # noqa: F401
 except ImportError:
     pass
 
 import json
@@ -83,24 +83,23 @@
     --------
     Explicit use case.
 
     >>> import json
     >>> from compas.data import DataEncoder
     >>> from compas.geometry import Point
     >>> point = Point(0, 0, 0)
-    >>> with open('point.json', 'w') as f:
+    >>> with open("point.json", "w") as f:
     ...     json.dump(point, f, cls=DataEncoder)
-    ...
 
     Implicit use case.
 
     >>> from compas.data import json_dump
     >>> from compas.geometry import Point
     >>> point = Point(0, 0, 0)
-    >>> json_dump(point, 'point.json')
+    >>> json_dump(point, "point.json")
 
     """
 
     minimal = False
 
     def default(self, o):
         """Return an object in serialized form.
@@ -178,22 +177,21 @@
 
     Examples
     --------
     Explicit use case.
 
     >>> import json
     >>> from compas.data import DataDecoder
-    >>> with open('point.json', 'r') as f:
+    >>> with open("point.json", "r") as f:
     ...     point = json.load(f, cls=DataDecoder)
-    ...
 
     Implicit use case.
 
     >>> from compas.data import json_load
-    >>> point = json_load('point.json')
+    >>> point = json_load("point.json")
 
     """
 
     def __init__(self, *args, **kwargs):
         super(DataDecoder, self).__init__(object_hook=self.object_hook, *args, **kwargs)
 
     def object_hook(self, o):
```

### Comparing `COMPAS-2.1.0/src/compas/data/json.py` & `compas-2.1.1/src/compas/data/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     :class:`compas.data.json_loads`
 
     Examples
     --------
     >>> import compas
     >>> from compas.geometry import Point, Vector
     >>> data1 = [Point(0, 0, 0), Vector(0, 0, 0)]
-    >>> compas.json_dump(data1, 'data.json')
-    >>> data2 = compas.json_load('data.json')
+    >>> compas.json_dump(data1, "data.json")
+    >>> data2 = compas.json_load("data.json")
     >>> data1 == data2
     True
 
     """
     DataEncoder.minimal = minimal
 
     with _iotools.open_file(fp, "w") as f:
@@ -193,16 +193,16 @@
     :class:`compas.data.json_loads`
 
     Examples
     --------
     >>> import compas
     >>> from compas.geometry import Point, Vector
     >>> data1 = [Point(0, 0, 0), Vector(0, 0, 0)]
-    >>> compas.json_dump(data1, 'data.json')
-    >>> data2 = compas.json_load('data.json')
+    >>> compas.json_dump(data1, "data.json")
+    >>> data2 = compas.json_load("data.json")
     >>> data1 == data2
     True
 
     """
     with _iotools.open_file(fp, "r") as f:
         return json.load(f, cls=DataDecoder)
```

### Comparing `COMPAS-2.1.0/src/compas/data/samples/boxes.obj` & `compas-2.1.1/src/compas/data/samples/boxes.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/butt_model.obj` & `compas-2.1.1/src/compas/data/samples/butt_model.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/cone.stl` & `compas-2.1.1/src/compas/data/samples/cone.stl`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/cube_ascii.stl` & `compas-2.1.1/src/compas/data/samples/cube_ascii.stl`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/doosabin.json` & `compas-2.1.1/src/compas/data/samples/doosabin.json`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/faces.obj` & `compas-2.1.1/src/compas/data/samples/faces.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/faces_big.obj` & `compas-2.1.1/src/compas/data/samples/faces_big.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/faces_reversed.obj` & `compas-2.1.1/src/compas/data/samples/faces_reversed.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/fink.obj` & `compas-2.1.1/src/compas/data/samples/fink.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/grid_irregular.obj` & `compas-2.1.1/src/compas/data/samples/grid_irregular.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/hypar.obj` & `compas-2.1.1/src/compas/data/samples/hypar.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/lines.json` & `compas-2.1.1/src/compas/data/samples/lines.json`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/lines.obj` & `compas-2.1.1/src/compas/data/samples/lines.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/lines_big.obj` & `compas-2.1.1/src/compas/data/samples/lines_big.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/lines_bigger.obj` & `compas-2.1.1/src/compas/data/samples/lines_bigger.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/lines_noleaves.obj` & `compas-2.1.1/src/compas/data/samples/lines_noleaves.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/mesh.obj` & `compas-2.1.1/src/compas/data/samples/mesh.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/mesh_100_faces.json` & `compas-2.1.1/src/compas/data/samples/mesh_100_faces.json`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/mesh_110_faces.json` & `compas-2.1.1/src/compas/data/samples/mesh_110_faces.json`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/open_edges.obj` & `compas-2.1.1/src/compas/data/samples/open_edges.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/quadmesh.obj` & `compas-2.1.1/src/compas/data/samples/quadmesh.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/quadmesh_planar.obj` & `compas-2.1.1/src/compas/data/samples/quadmesh_planar.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/saddle.obj` & `compas-2.1.1/src/compas/data/samples/saddle.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/spline.obj` & `compas-2.1.1/src/compas/data/samples/spline.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/tubemesh.json` & `compas-2.1.1/src/compas/data/samples/tubemesh.json`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/tubemesh.obj` & `compas-2.1.1/src/compas/data/samples/tubemesh.obj`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/tubemesh.off` & `compas-2.1.1/src/compas/data/samples/tubemesh.off`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/samples/tubemesh.ply` & `compas-2.1.1/src/compas/data/samples/tubemesh.ply`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/data/schema.py` & `compas-2.1.1/src/compas/data/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-import os
 import json
+import os
 
 
 def dataclass_dataschema(cls):  # type: (...) -> dict
     """Generate a JSON schema for a COMPAS object class.
 
     Parameters
     ----------
@@ -115,18 +115,19 @@
 
     Returns
     -------
     list
 
     """
     from collections import deque
-    from compas.data import Data
+
     import compas.colors  # noqa: F401
     import compas.datastructures  # noqa: F401
     import compas.geometry  # noqa: F401
+    from compas.data import Data
 
     tovisit = deque([Data])
     dataclasses = []
 
     while tovisit:
         cls = tovisit.popleft()
         dataclasses.append(cls)
```

### Comparing `COMPAS-2.1.0/src/compas/data/validators.py` & `compas-2.1.1/src/compas/data/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 try:
     basestring  # type: ignore
 except NameError:
     basestring = str
 
 
@@ -157,15 +157,15 @@
     -------
     bool
         True if all items in the sequence are of type tuple.
         False otherwise.
 
     Examples
     --------
-    >>> is_sequence_of_tuple([(1, ), (1, ), (1, )])
+    >>> is_sequence_of_tuple([(1,), (1,), (1,)])
     True
 
     """
     return all(isinstance(item, tuple) for item in items)
 
 
 def is_sequence_of_dict(items):
@@ -180,15 +180,15 @@
     -------
     bool
         True if all items in the sequence are of type dict.
         False otherwise.
 
     Examples
     --------
-    >>> is_sequence_of_dict([{'a': 1}, {'b': 2}, {'c': 3}])
+    >>> is_sequence_of_dict([{"a": 1}, {"b": 2}, {"c": 3}])
     True
 
     """
     return all(isinstance(item, dict) for item in items)
 
 
 def is_item_iterable(item):
@@ -205,15 +205,15 @@
         True if the item is iterable.
         False otherwise.
 
     Examples
     --------
     >>> is_item_iterable(1.0)
     False
-    >>> is_item_iterable('abc')
+    >>> is_item_iterable("abc")
     True
 
     """
     try:
         _ = [_ for _ in item]
     except TypeError:
         return False
@@ -232,12 +232,12 @@
     -------
     bool
         True if all items in the sequence are iterable.
         False otherwise.
 
     Examples
     --------
-    >>> is_sequence_of_iterable(['abc', [1.0], (2, 'a', None)])
+    >>> is_sequence_of_iterable(["abc", [1.0], (2, "a", None)])
     True
 
     """
     return all(is_item_iterable(item) for item in items)
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/__init__.py` & `compas-2.1.1/src/compas/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/datastructures/_mutablemapping.py` & `compas-2.1.1/src/compas/datastructures/_mutablemapping.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/datastructures/assembly/assembly.py` & `compas-2.1.1/src/compas/datastructures/assembly/assembly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.datastructures import Datastructure
 from compas.datastructures import Graph
+
 from .exceptions import AssemblyError
 
 
 class Assembly(Datastructure):
     """A data structure for managing the connections between different parts of an assembly.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/assembly/part.py` & `compas-2.1.1/src/compas/datastructures/assembly/part.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.data import Data
+from compas.datastructures import Datastructure
+from compas.geometry import Brep
 from compas.geometry import Frame
 from compas.geometry import Polyhedron
-from compas.geometry import Brep
-from compas.datastructures import Datastructure
-from compas.data import Data
 
 
 class Feature(Data):
     """Base class for a feature which may be applied to a :class:`compas.datastructures.Part`."""
 
     def apply(self, part):
         """Apply this Feature to the given part.
@@ -31,18 +31,18 @@
 
     An implementation of this class may offer support for various geometry types by adding an entry to OPERATIONS
     mapping the geometry type to its corresponding operation.
 
     Examples
     --------
     >>>    def trim_brep_plane(brep, plane):
-    >>>         # trim brep with plane, return trimmed brep
+    >>> # trim brep with plane, return trimmed brep
     >>>
     >>>    def trim_mesh_plane(mesh, plane):
-    >>>         # trim mesh with plane, return trimmed mesh
+    >>> # trim mesh with plane, return trimmed mesh
     >>>
     >>>    class TrimmingFeature(GeometricFeature):
     >>>        OPERATIONS = {Brep: trim_brep_plane, Mesh: trim_mesh_plane}
     >>>
     >>>            def __init__(self, trimming_plane):
     >>>                super(TrimmingFeature, self).__init__()
     >>>                self._geometry = trimming_plane
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/attributes.py` & `compas-2.1.1/src/compas/datastructures/attributes.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/datastructures/cell_network/cell_network.py` & `compas-2.1.1/src/compas/datastructures/cell_network/cell_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 from random import sample
 
-from compas.datastructures import Mesh
 from compas.datastructures import Graph
-from compas.datastructures.datastructure import Datastructure
-from compas.datastructures.attributes import VertexAttributeView
+from compas.datastructures import Mesh
+from compas.datastructures.attributes import CellAttributeView
 from compas.datastructures.attributes import EdgeAttributeView
 from compas.datastructures.attributes import FaceAttributeView
-from compas.datastructures.attributes import CellAttributeView
-
+from compas.datastructures.attributes import VertexAttributeView
+from compas.datastructures.datastructure import Datastructure
 from compas.files import OBJ
-
 from compas.geometry import Line
 from compas.geometry import Point
 from compas.geometry import Polygon
 from compas.geometry import Polyhedron
 from compas.geometry import Vector
+from compas.geometry import add_vectors
+from compas.geometry import bestfit_plane
+from compas.geometry import bounding_box
 from compas.geometry import centroid_points
 from compas.geometry import centroid_polygon
 from compas.geometry import centroid_polyhedron
 from compas.geometry import distance_point_point
 from compas.geometry import length_vector
 from compas.geometry import normal_polygon
 from compas.geometry import normalize_vector
-from compas.geometry import volume_polyhedron
-from compas.geometry import add_vectors
-from compas.geometry import bestfit_plane
 from compas.geometry import project_point_plane
 from compas.geometry import scale_vector
 from compas.geometry import subtract_vectors
-from compas.geometry import bounding_box
-
-from compas.utilities import pairwise
-
+from compas.geometry import volume_polyhedron
+from compas.itertools import pairwise
 from compas.tolerance import TOL
 
 
 class CellNetwork(Datastructure):
     """Geometric implementation of a data structure for a collection of mixed topologic entities such as cells, faces, edges and nodes.
 
     Parameters
@@ -69,15 +65,15 @@
         Default values for cell attributes.
 
     Examples
     --------
     >>> from compas.datastructures import CellNetwork
     >>> cell_network = CellNetwork()
     >>> vertices = [(0, 0, 0), (0, 1, 0), (1, 1, 0), (1, 0, 0), (0, 0, 1), (1, 0, 1), (1, 1, 1), (0, 1, 1)]
-    >>> faces = [[0, 1, 2, 3], [0, 3, 5, 4],[3, 2, 6, 5], [2, 1, 7, 6],[1, 0, 4, 7],[4, 5, 6, 7]]
+    >>> faces = [[0, 1, 2, 3], [0, 3, 5, 4], [3, 2, 6, 5], [2, 1, 7, 6], [1, 0, 4, 7], [4, 5, 6, 7]]
     >>> cells = [[0, 1, 2, 3, 4, 5]]
     >>> [network.add_vertex(x=x, y=y, z=z) for x, y, z in vertices]
     >>> [cell_network.add_face(fverts) for fverts in faces]
     >>> [cell_network.add_cell(fkeys) for fkeys in cells]
     >>> cell_network
 
     """
@@ -223,23 +219,15 @@
 
         cell_network._max_vertex = data.get("max_vertex", cell_network._max_vertex)
         cell_network._max_face = data.get("max_face", cell_network._max_face)
         cell_network._max_cell = data.get("max_cell", cell_network._max_cell)
 
         return cell_network
 
-    def __init__(
-        self,
-        default_vertex_attributes=None,
-        default_edge_attributes=None,
-        default_face_attributes=None,
-        default_cell_attributes=None,
-        name=None,
-        **kwargs
-    ):
+    def __init__(self, default_vertex_attributes=None, default_edge_attributes=None, default_face_attributes=None, default_cell_attributes=None, name=None, **kwargs):  # fmt: skip
         super(CellNetwork, self).__init__(kwargs, name=name)
         self._max_vertex = -1
         self._max_face = -1
         self._max_cell = -1
         self._vertex = {}
         self._edge = {}
         self._face = {}
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/datastructure.py` & `compas-2.1.1/src/compas/datastructures/datastructure.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/datastructures/graph/duality.py` & `compas-2.1.1/src/compas/datastructures/graph/duality.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import pi
 
-from compas.utilities import pairwise
 from compas.geometry import angle_vectors
 from compas.geometry import is_ccw_xy
-
+from compas.itertools import pairwise
 
 PI2 = 2.0 * pi
 
 
 def graph_find_cycles(graph, breakpoints=None):
     """Find the faces of a graph.
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/graph/graph.py` & `compas-2.1.1/src/compas/datastructures/graph/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,58 +1,56 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from random import sample
 from ast import literal_eval
 from itertools import combinations
+from random import sample
 
 import compas
 
 if compas.PY2:
     from collections import Mapping
 else:
     from collections.abc import Mapping
 
-from compas.tolerance import TOL
+from compas.datastructures.attributes import EdgeAttributeView
+from compas.datastructures.attributes import NodeAttributeView
+from compas.datastructures.datastructure import Datastructure
 from compas.files import OBJ
+from compas.geometry import Box
+from compas.geometry import Line
 from compas.geometry import Point
 from compas.geometry import Vector
-from compas.geometry import Line
-from compas.geometry import Box
+from compas.geometry import add_vectors
+from compas.geometry import bounding_box
 from compas.geometry import centroid_points
-from compas.geometry import subtract_vectors
 from compas.geometry import distance_point_point
 from compas.geometry import midpoint_line
 from compas.geometry import normalize_vector
-from compas.geometry import add_vectors
+from compas.geometry import oriented_bounding_box
 from compas.geometry import scale_vector
+from compas.geometry import subtract_vectors
 from compas.geometry import transform_points
-from compas.geometry import bounding_box
-from compas.geometry import oriented_bounding_box
+from compas.tolerance import TOL
 from compas.topology import astar_shortest_path
 from compas.topology import breadth_first_traverse
 from compas.topology import connected_components
 
-from compas.datastructures.datastructure import Datastructure
-from compas.datastructures.attributes import NodeAttributeView
-from compas.datastructures.attributes import EdgeAttributeView
-
-from .operations.split import graph_split_edge
+from .duality import graph_find_cycles
 from .operations.join import graph_join_edges
-
+from .operations.split import graph_split_edge
+from .planarity import graph_count_crossings
+from .planarity import graph_embed_in_plane
+from .planarity import graph_find_crossings
 from .planarity import graph_is_crossed
 from .planarity import graph_is_planar
 from .planarity import graph_is_planar_embedding
 from .planarity import graph_is_xy
-from .planarity import graph_count_crossings
-from .planarity import graph_find_crossings
-from .planarity import graph_embed_in_plane
 from .smoothing import graph_smooth_centroid
-from .duality import graph_find_cycles
 
 
 class Graph(Datastructure):
     """Data structure for describing the relationships between nodes connected by edges.
 
     Parameters
     ----------
@@ -903,15 +901,15 @@
         -----
         A graph is connected if for every two vertices a path exists connecting them.
 
         Examples
         --------
         >>> import compas
         >>> from compas.datastructures import Graph
-        >>> graph = Graph.from_obj(compas.get('lines.obj'))
+        >>> graph = Graph.from_obj(compas.get("lines.obj"))
         >>> graph.is_connected()
         True
 
         """
         if self.number_of_nodes() == 0:
             return False
         nodes = breadth_first_traverse(self.adjacency, self.node_sample(size=1)[0])
@@ -2362,15 +2360,15 @@
         .. [1] Wolfram MathWorld. *Graph complement*.
             Available at: http://mathworld.wolfram.com/GraphComplement.html.
 
         Examples
         --------
         >>> import compas
         >>> from compas.datastructures import Graph
-        >>> graph = Graph.from_obj(compas.get('lines.obj'))
+        >>> graph = Graph.from_obj(compas.get("lines.obj"))
         >>> complement = graph.complement()
         >>> any(complement.has_edge(u, v, directed=False) for u, v in graph.edges())
         False
 
         """
         cls = type(self)
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/graph/operations/join.py` & `compas-2.1.1/src/compas/datastructures/graph/operations/join.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.itertools import pairwise
 from compas.tolerance import TOL
-from compas.utilities import pairwise
 
 
 def graph_join_edges(graph, key):
     """Join the edges incidental on the given node, if there are exactly two incident edges.
 
     Parameters
     ----------
@@ -73,20 +73,20 @@
     Examples
     --------
     Joining the lines (a, b), (b, c), (c, d), (c, e) and (e, f),
     where a ... f are different point coordinates.
     This will result in the following polylines (a, b, c), (c, d) and (c, e, f).
 
     >>> from compas.datastructures import Graph
-    >>> a = [0., 0., 0.]
-    >>> b = [1., 0., 0.]
-    >>> c = [2., 0., 0.]
-    >>> d = [2., 1., 0.]
-    >>> e = [3., 0., 0.]
-    >>> f = [4., 0., 0.]
+    >>> a = [0.0, 0.0, 0.0]
+    >>> b = [1.0, 0.0, 0.0]
+    >>> c = [2.0, 0.0, 0.0]
+    >>> d = [2.0, 1.0, 0.0]
+    >>> e = [3.0, 0.0, 0.0]
+    >>> f = [4.0, 0.0, 0.0]
     >>> lines = [(a, b), (b, c), (c, d), (c, e), (e, f)]
     >>> graph = Graph.from_lines(lines)
     >>> len(graph_polylines(graph)) == 3
     True
 
     """
     # geometric keys of split points
@@ -100,23 +100,17 @@
     # initiate a polyline from an unvisited edge
     while len(edges_to_visit) > 0:
         polyline = list(edges_to_visit.pop())
 
         # get adjacent edges until the polyline is closed...
         while polyline[0] != polyline[-1]:
             # ... or until both end are non-two-valent vertices
-            if (
-                len(graph.neighbors(polyline[-1])) != 2
-                or TOL.geometric_key(graph.node_coordinates(polyline[-1])) in stop_geom_keys
-            ):
+            if len(graph.neighbors(polyline[-1])) != 2 or TOL.geometric_key(graph.node_coordinates(polyline[-1])) in stop_geom_keys:
                 polyline = list(reversed(polyline))
-                if (
-                    len(graph.neighbors(polyline[-1])) != 2
-                    or TOL.geometric_key(graph.node_coordinates(polyline[-1])) in stop_geom_keys
-                ):
+                if len(graph.neighbors(polyline[-1])) != 2 or TOL.geometric_key(graph.node_coordinates(polyline[-1])) in stop_geom_keys:
                     break
 
             # add next edge
             polyline.append([nbr for nbr in graph.neighbors(polyline[-1]) if nbr != polyline[-2]][0])
 
         # delete polyline edges from the list of univisted edges
         for u, v in pairwise(polyline):
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/graph/operations/split.py` & `compas-2.1.1/src/compas/datastructures/graph/operations/split.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 
 def graph_split_edge(graph, edge, t=0.5):
     """Split and edge by inserting a node along its length.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/graph/planarity.py` & `compas-2.1.1/src/compas/datastructures/graph/planarity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from itertools import product
 from math import cos
-from math import sin
 from math import pi
-
-from itertools import product
+from math import sin
 
 from compas.geometry import angle_vectors_xy
 from compas.geometry import is_ccw_xy
 from compas.geometry import subtract_vectors_xy
-
 from compas.geometry._core.predicates_2 import is_intersection_segment_segment_xy
 
 
 def graph_embed_in_plane_proxy(data, fixed=None):
     from compas.datastructures import Graph
 
     graph = Graph.__from_data__(data)
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/graph/smoothing.py` & `compas-2.1.1/src/compas/datastructures/graph/smoothing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.geometry import centroid_points
 
 
 def graph_smooth_centroid(graph, fixed=None, kmax=100, damping=0.5, callback=None, callback_args=None):
     """Smooth a graph by moving every free node to the centroid of its neighbors.
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/conway.py` & `compas-2.1.1/src/compas/datastructures/mesh/conway.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 
 def mesh_conway_dual(mesh):
     """Generates the dual mesh from a seed mesh.
 
     Parameters
     ----------
@@ -181,19 +181,15 @@
     """
     cls = type(mesh)
     vertices = [mesh.vertex_coordinates(vkey) for vkey in mesh.vertices()]
     vertices += [mesh.face_centroid(fkey) for fkey in mesh.faces()]
     v = mesh.number_of_vertices()
     vkey_index = {vkey: i for i, vkey in enumerate(mesh.vertices())}
     fkey_index = {fkey: i + v for i, fkey in enumerate(mesh.faces())}
-    faces = [
-        [vkey_index[u], vkey_index[v], fkey_index[mesh.halfedge[u][v]]]
-        for fkey in mesh.faces()
-        for u, v in mesh.face_halfedges(fkey)
-    ]
+    faces = [[vkey_index[u], vkey_index[v], fkey_index[mesh.halfedge[u][v]]] for fkey in mesh.faces() for u, v in mesh.face_halfedges(fkey)]
     return cls.from_vertices_and_faces(vertices, faces)
 
 
 def mesh_conway_needle(mesh):
     """Generates the needle mesh from a seed mesh.
 
     Parameters
@@ -423,17 +419,15 @@
     vertices = [mesh.vertex_coordinates(vkey) for vkey in mesh.vertices()]
     vertices += [mesh.face_centroid(fkey) for fkey in mesh.faces()]
     vertices += [mesh.edge_point((u, v), t=0.33) for u in mesh.vertices() for v in mesh.halfedge[u]]
     V = mesh.number_of_vertices()
     F = mesh.number_of_faces()
     vkey_index = {vkey: i for i, vkey in enumerate(mesh.vertices())}
     fkey_index = {fkey: i + V for i, fkey in enumerate(mesh.faces())}
-    ekey_index = {
-        halfedge: i + V + F for i, halfedge in enumerate([(u, v) for u in mesh.vertices() for v in mesh.halfedge[u]])
-    }
+    ekey_index = {halfedge: i + V + F for i, halfedge in enumerate([(u, v) for u in mesh.vertices() for v in mesh.halfedge[u]])}
     faces = []
     for fkey in mesh.faces():
         for u, v in mesh.face_halfedges(fkey):
             faces.append(
                 [
                     ekey_index[u, v],
                     ekey_index[v, u],
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/duality.py` & `compas-2.1.1/src/compas/datastructures/mesh/duality.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import pi
-from compas.utilities import flatten
 
+from compas.itertools import flatten
 
 PI2 = 2.0 * pi
 
 
 def mesh_dual(mesh, cls=None, include_boundary=False):
     """Construct the dual of a mesh.
 
@@ -28,20 +28,20 @@
     :class:`compas.datastructures.Mesh`
         The dual mesh object.
 
     Examples
     --------
     >>> import compas
     >>> from compas.datastructures import Mesh
-    >>> mesh = Mesh.from_obj(compas.get('faces.obj'))
+    >>> mesh = Mesh.from_obj(compas.get("faces.obj"))
     >>> mesh.delete_face(11)
     >>> mesh.delete_face(6)
     >>> mesh.delete_face(7)
     >>> mesh.quads_to_triangles()
-    >>> mesh = mesh.subdivide('corner')
+    >>> mesh = mesh.subdivide("corner")
     >>> dual = mesh.dual(include_boundary=True)
 
     """
     if not cls:
         cls = type(mesh)
 
     dual = cls()
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/mesh.py` & `compas-2.1.1/src/compas/datastructures/mesh/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,87 +1,80 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-from math import pi
 from itertools import product
+from math import pi
 from random import sample
 
 import compas
 
 if compas.PY2:
     from collections import Mapping
 else:
     from collections.abc import Mapping
 
-from compas.tolerance import TOL
-
+from compas.datastructures.attributes import EdgeAttributeView
+from compas.datastructures.attributes import FaceAttributeView
+from compas.datastructures.attributes import VertexAttributeView
+from compas.datastructures.datastructure import Datastructure
 from compas.files import OBJ
 from compas.files import OFF
 from compas.files import PLY
 from compas.files import STL
-
-from compas.geometry import Point
-from compas.geometry import Vector
+from compas.geometry import Box
+from compas.geometry import Circle
+from compas.geometry import Frame
 from compas.geometry import Line
 from compas.geometry import Plane
+from compas.geometry import Point
 from compas.geometry import Polygon
-from compas.geometry import Circle
-from compas.geometry import Frame
 from compas.geometry import Polyhedron
-from compas.geometry import Box
+from compas.geometry import Vector
+from compas.geometry import add_vectors
 from compas.geometry import angle_points
 from compas.geometry import area_polygon
 from compas.geometry import bestfit_plane
+from compas.geometry import bounding_box
 from compas.geometry import centroid_points
 from compas.geometry import centroid_polygon
 from compas.geometry import cross_vectors
+from compas.geometry import distance_line_line
 from compas.geometry import distance_point_plane
 from compas.geometry import distance_point_point
-from compas.geometry import distance_line_line
 from compas.geometry import length_vector
+from compas.geometry import midpoint_line
 from compas.geometry import normal_polygon
 from compas.geometry import normalize_vector
+from compas.geometry import oriented_bounding_box
 from compas.geometry import scale_vector
-from compas.geometry import add_vectors
 from compas.geometry import subtract_vectors
 from compas.geometry import sum_vectors
-from compas.geometry import midpoint_line
-from compas.geometry import vector_average
-from compas.geometry import bounding_box
-from compas.geometry import oriented_bounding_box
 from compas.geometry import transform_points
-
-from compas.utilities import linspace
-from compas.utilities import pairwise
-from compas.utilities import window
-
+from compas.geometry import vector_average
+from compas.itertools import linspace
+from compas.itertools import pairwise
+from compas.itertools import window
+from compas.tolerance import TOL
 from compas.topology import breadth_first_traverse
-from compas.topology import face_adjacency
 from compas.topology import connected_components
+from compas.topology import unify_cycles
 
-from compas.datastructures.datastructure import Datastructure
-from compas.datastructures.attributes import VertexAttributeView
-from compas.datastructures.attributes import EdgeAttributeView
-from compas.datastructures.attributes import FaceAttributeView
-
+from .duality import mesh_dual
 from .operations.collapse import mesh_collapse_edge
 from .operations.merge import mesh_merge_faces
 from .operations.split import mesh_split_edge
 from .operations.split import mesh_split_face
 from .operations.split import mesh_split_strip
 from .operations.weld import mesh_unweld_edges
 from .operations.weld import mesh_unweld_vertices
-
-from .subdivision import mesh_subdivide
-from .duality import mesh_dual
 from .slice import mesh_slice_plane
-
-from .smoothing import mesh_smooth_centroid
 from .smoothing import mesh_smooth_area
+from .smoothing import mesh_smooth_centroid
+from .subdivision import mesh_subdivide
 
 
 class Mesh(Datastructure):
     """Data structure for representing open or closed surface meshes.
 
     Parameters
     ----------
@@ -231,22 +224,15 @@
 
         mesh.edgedata = edgedata
         mesh._max_vertex = data.get("max_vertex", mesh._max_vertex)
         mesh._max_face = data.get("max_face", mesh._max_face)
 
         return mesh
 
-    def __init__(
-        self,
-        default_vertex_attributes=None,
-        default_edge_attributes=None,
-        default_face_attributes=None,
-        name=None,
-        **kwargs
-    ):
+    def __init__(self, default_vertex_attributes=None, default_edge_attributes=None, default_face_attributes=None, name=None, **kwargs):  # fmt: skip
         super(Mesh, self).__init__(kwargs, name=name)
         self._max_vertex = -1
         self._max_face = -1
         self.vertex = {}
         self.halfedge = {}
         self.face = {}
         self.facedata = {}
@@ -2859,20 +2845,19 @@
         None
             The mesh is modified in-place.
 
         Examples
         --------
         >>> import compas
         >>> from compas.datastructures import Mesh
-        >>> mesh = Mesh.from_obj(compas.get('faces.obj'))
+        >>> mesh = Mesh.from_obj(compas.get("faces.obj"))
         >>> mesh.number_of_vertices()
         36
-        >>> for x, y, z in mesh.vertices_attributes('xyz', keys=list(mesh.vertices())[:5]):
+        >>> for x, y, z in mesh.vertices_attributes("xyz", keys=list(mesh.vertices())[:5]):
         ...     mesh.add_vertex(x=x, y=y, z=z)
-        ...
         38
         39
         40
         >>> mesh.number_of_vertices()
         41
         >>> mesh.remove_duplicate_vertices()
         >>> mesh.number_of_vertices()
@@ -2949,50 +2934,33 @@
 
         Returns
         -------
         None
             The mesh is modified in place.
 
         """
-
-        def unify(node, nbr):
-            # find the common edge
-            for u, v in self.face_halfedges(nbr):
-                if u in self.face[node] and v in self.face[node]:
-                    # node and nbr have edge u-v in common
-                    i = self.face[node].index(u)
-                    j = self.face[node].index(v)
-                    if i == j - 1 or (j == 0 and u == self.face[node][-1]):
-                        # if the traversal of a neighboring halfedge
-                        # is in the same direction
-                        # flip the neighbor
-                        self.face[nbr][:] = self.face[nbr][::-1]
-                        return
-
-        if root is None:
-            root = self.face_sample(size=1)[0]
-
+        vertex_index = {}
+        index_vertex = {}
+        for index, vertex in enumerate(self.vertices()):
+            vertex_index[vertex] = index
+            index_vertex[index] = vertex
         index_face = {index: face for index, face in enumerate(self.faces())}
-        points = self.vertices_attributes("xyz")
-        faces = [self.face_vertices(face) for face in self.faces()]
-
-        adj = face_adjacency(points, faces)
-        adjacency = {}
-        for face in adj:
-            adjacency[index_face[face]] = [index_face[nbr] for nbr in adj[face]]
 
-        visited = breadth_first_traverse(adjacency, root, unify)
+        vertices = self.vertices_attributes("xyz")
+        faces = [[vertex_index[vertex] for vertex in self.face_vertices(face)] for face in self.faces()]
 
-        if len(list(visited)) != self.number_of_faces():
-            raise Exception("Not all faces were visited.")
+        unify_cycles(vertices, faces)
 
         self.halfedge = {key: {} for key in self.vertices()}
-        for fkey in self.faces():
-            for u, v in self.face_halfedges(fkey):
-                self.halfedge[u][v] = fkey
+        for index, vertices in enumerate(faces):
+            face = index_face[index]
+            vertices = [index_vertex[vertex] for vertex in vertices]
+            self.face[face] = vertices
+            for u, v in pairwise(vertices + vertices[:1]):
+                self.halfedge[u][v] = face
                 if u not in self.halfedge[v]:
                     self.halfedge[v][u] = None
 
     # --------------------------------------------------------------------------
     # Components
     # --------------------------------------------------------------------------
 
@@ -4409,27 +4377,38 @@
             A maximum value for the allowed deviation from flatness.
 
         Returns
         -------
         float
             The flatness.
 
+        Raises
+        ------
+        Exception
+            If the face has more than 4 vertices.
+
         Notes
         -----
         Flatness is computed as the ratio of the distance between the diagonals
         of the face to the average edge length. A practical limit on this value
         realted to manufacturing is 0.02 (2%).
 
         Warnings
         --------
         This method only makes sense for quadrilateral faces.
 
         """
         vertices = self.face_vertices(fkey)
         f = len(vertices)
+
+        if f == 3:
+            return 0.0
+        if f > 4:
+            raise Exception("Computing face flatness for faces with more than 4 vertices is not supported.")
+
         points = self.vertices_attributes("xyz", keys=vertices) or []
         lengths = [distance_point_point(a, b) for a, b in pairwise(points + points[:1])]
         length = sum(lengths) / f
         d = distance_line_line((points[0], points[2]), (points[1], points[3]))
         return (d / length) / maxdev
 
     def face_aspect_ratio(self, fkey):
@@ -5071,25 +5050,26 @@
         <compas.datastructures.mesh.mesh.Mesh object at 0x109eaad60>
 
         """
         if thickness <= 0:
             raise ValueError("Thickness should be a positive number.")
 
         if both:
-            mesh_top = self.offset(+0.5 * thickness)
-            mesh_bottom = self.offset(-0.5 * thickness)
+            mesh_top = self.offset(+0.5 * thickness)  # type: Mesh
+            mesh_bottom = self.offset(-0.5 * thickness)  # type: Mesh
         else:
             mesh_top = self.offset(thickness)
             mesh_bottom = self.copy()
 
         # flip bottom part
         mesh_bottom.flip_cycles()
 
         # join parts
-        thickened_mesh = mesh_top.join(mesh_bottom)
+        thickened_mesh = mesh_top.copy()  # type: Mesh
+        thickened_mesh.join(mesh_bottom)
 
         # close boundaries
         n = thickened_mesh.number_of_vertices() / 2
 
         edges_on_boundary = [edge for boundary in list(thickened_mesh.edges_on_boundaries()) for edge in boundary]
 
         for u, v in edges_on_boundary:
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/operations/collapse.py` & `compas-2.1.1/src/compas/datastructures/mesh/operations/collapse.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 
 def is_collapse_legal(mesh, edge, allow_boundary=False):
     """Verify if the requested collapse is legal for a triangle mesh.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/operations/insert.py` & `compas-2.1.1/src/compas/datastructures/mesh/operations/insert.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 
 def mesh_add_vertex_to_face_edge(mesh, key, fkey, v):
     """Add an existing vertex of the mesh to an existing face.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/operations/merge.py` & `compas-2.1.1/src/compas/datastructures/mesh/operations/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 
 def mesh_merge_faces(mesh, faces):
     """Merge two faces of a mesh over their shared edge.
 
     Parameters
     ----------
@@ -17,15 +17,15 @@
     -------
     int
 
     Examples
     --------
     >>> from compas.datastructures import Mesh
     >>> mesh = Mesh.from_vertices_and_faces([[0, 0, 0], [1, 0, 0], [1, 1, 0], [0, 1, 0]], [[0, 1, 2, 3]])
-    >>> mesh = mesh.subdivide(scheme='quad')
+    >>> mesh = mesh.subdivide(scheme="quad")
     >>> mesh_merge_faces(mesh, [1, 2])
     5
     >>> mesh_merge_faces(mesh, [3, 5])
     6
     >>> mesh_merge_faces(mesh, [4, 6])
     7
     >>> mesh.face_vertices(7)
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/operations/split.py` & `compas-2.1.1/src/compas/datastructures/mesh/operations/split.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.utilities import pairwise
+from compas.itertools import pairwise
 
 
 def mesh_split_edge(mesh, edge, t=0.5, allow_boundary=False):
     """Split and edge by inserting a vertex along its length.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/operations/substitute.py` & `compas-2.1.1/src/compas/datastructures/mesh/operations/substitute.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 
 def mesh_substitute_vertex_in_faces(mesh, old_vkey, new_vkey, fkeys=None):
     """Substitute in a mesh a vertex by another one.
     In all faces by default or in a given set of faces.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/operations/swap.py` & `compas-2.1.1/src/compas/datastructures/mesh/operations/swap.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 
 def trimesh_swap_edge(mesh, edge, allow_boundary=True):
     """Replace an edge of the mesh by an edge connecting the opposite
     vertices of the adjacent faces.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/operations/weld.py` & `compas-2.1.1/src/compas/datastructures/mesh/operations/weld.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.topology import vertex_adjacency_from_edges
+from compas.itertools import pairwise
 from compas.topology import connected_components
-
-from compas.utilities import pairwise
+from compas.topology import vertex_adjacency_from_edges
 
 from .substitute import mesh_substitute_vertex_in_faces
 
 
 def mesh_unweld_vertices(mesh, fkey, where=None):
     """Unweld a face of the mesh.
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/remesh.py` & `compas-2.1.1/src/compas/datastructures/mesh/remesh.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from .smoothing import mesh_smooth_area
 from .operations.collapse import trimesh_collapse_edge
-from .operations.swap import trimesh_swap_edge
 from .operations.split import trimesh_split_edge
+from .operations.swap import trimesh_swap_edge
+from .smoothing import mesh_smooth_area
 
 
 def trimesh_remesh(
     mesh,
     target,
     kmax=100,
     tol=0.1,
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/slice.py` & `compas-2.1.1/src/compas/datastructures/mesh/slice.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from compas.geometry import dot_vectors
 from compas.geometry import intersection_segment_plane
 from compas.geometry import length_vector
 from compas.geometry import subtract_vectors
-from compas.geometry import dot_vectors
 
 
 def mesh_slice_plane(mesh, plane):
     """Slice a mesh with a plane and construct the resulting submeshes.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/smoothing.py` & `compas-2.1.1/src/compas/datastructures/mesh/smoothing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.geometry import centroid_points
 from compas.geometry import centroid_polygon
 
 
 def mesh_smooth_centroid(mesh, fixed=None, kmax=100, damping=0.5, callback=None, callback_args=None):
     """Smooth a mesh by moving every free vertex to the centroid of its neighbors.
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/mesh/subdivision.py` & `compas-2.1.1/src/compas/datastructures/mesh/subdivision.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from copy import deepcopy
 from math import cos
 from math import pi
-from copy import deepcopy
 
 from compas.geometry import centroid_points
 from compas.geometry import offset_polygon
-
-from compas.utilities import iterable_like
-from compas.utilities import pairwise
+from compas.itertools import iterable_like
+from compas.itertools import pairwise
 
 
 def subd_factory(cls):
     class SubdMesh(cls):
         _add_vertex = cls.add_vertex
         _add_face = cls.add_face
         _insert_vertex = cls.insert_vertex
@@ -176,15 +175,15 @@
     >>> mesh = Mesh.from_shape(box)
     >>> k = 2
     >>> subd = mesh_subdivide_quad(mesh, k=k)
     >>> mesh is subd
     False
     >>> type(mesh) is type(subd)
     True
-    >>> subd.number_of_faces() == mesh.number_of_faces() * 4 ** k
+    >>> subd.number_of_faces() == mesh.number_of_faces() * 4**k
     True
 
     """
     cls = type(mesh)
     subd = mesh_fast_copy(mesh)
     for face in subd.faces():
         subd.facedata[face]["path"] = [face]
@@ -290,15 +289,15 @@
     >>> mesh = Mesh.from_shape(box)
     >>> k = 2
     >>> subd = mesh_subdivide_catmullclark(mesh, k=k)
     >>> mesh is subd
     False
     >>> type(mesh) is type(subd)
     True
-    >>> subd.number_of_faces() == mesh.number_of_faces() * 4 ** k
+    >>> subd.number_of_faces() == mesh.number_of_faces() * 4**k
     True
 
     The algorithm supports "integer creasing" as described in
     Subdivision Surfaces in Character Animation [1]_.
     Creases are supported through the optional edge attribute "crease",
     which can be set to an integer value that defines how sharp the crease is wrt
     the number of subdivision steps.
@@ -306,17 +305,17 @@
     To add an infinitely sharp crease to an edge, set the "crease" attribute of the edge
     to a number higher than the number of subdivision steps.
 
     >>> from compas.geometry import Box, dot_vectors
     >>> from compas.datastructures import Mesh
 
     >>> cage = Mesh.from_shape(Box.from_width_height_depth(1, 1, 1))
-    >>> cage.update_default_edge_attributes({'crease': 0})
+    >>> cage.update_default_edge_attributes({"crease": 0})
     >>> top = sorted(cage.faces(), key=lambda face: dot_vectors(cage.face_normal(face), [0, 0, 1]))[-1]
-    >>> cage.edges_attribute('crease', 5, keys=list(cage.face_halfedges(top)))
+    >>> cage.edges_attribute("crease", 5, keys=list(cage.face_halfedges(top)))
 
     >>> subd = cage.subdivide(k=4)
 
     """
     cls = type(mesh)
 
     if not fixed:
@@ -393,17 +392,15 @@
             nbrs = mesh.vertex_neighbors(key)
             creases = mesh.edges_attribute("crease", keys=[(key, nbr) for nbr in nbrs])
 
             C = sum(1 if crease else 0 for crease in creases)
 
             if C < 2:
                 fnbrs = [mesh.face_centroid(fkey) for fkey in mesh.vertex_faces(key) if fkey is not None]
-                enbrs = [
-                    key_xyz[nbr] for nbr in subd.halfedge[key]
-                ]  # this should be the location of the original neighbour
+                enbrs = [key_xyz[nbr] for nbr in subd.halfedge[key]]  # this should be the location of the original neighbour
                 n = len(enbrs)
                 v = n - 3.0
                 F = centroid_points(fnbrs)
                 E = centroid_points(enbrs)
                 V = key_xyz[key]
                 x = (F[0] + 2.0 * E[0] + v * V[0]) / n
                 y = (F[1] + 2.0 * E[1] + v * V[1]) / n
@@ -669,17 +666,15 @@
     fixed = set(fixed)
 
     subd = mesh_fast_copy(mesh)
 
     for _ in range(k):
         key_xyz = {key: subd.vertex_coordinates(key) for key in subd.vertices()}
         fkey_vertices = {fkey: subd.face_vertices(fkey)[:] for fkey in subd.faces()}
-        uv_w = {
-            (u, v): subd.face_vertex_ancestor(fkey, u) for fkey in subd.faces() for u, v in subd.face_halfedges(fkey)
-        }
+        uv_w = {(u, v): subd.face_vertex_ancestor(fkey, u) for fkey in subd.faces() for u, v in subd.face_halfedges(fkey)}
         boundary = set(subd.vertices_on_boundary())
 
         for key in subd.vertices():
             nbrs = subd.vertex_neighbors(key)
 
             if key in boundary:
                 xyz = key_xyz[key]
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/tree/tree.py` & `compas-2.1.1/src/compas/datastructures/tree/tree.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.datastructures import Datastructure
 from compas.data import Data
+from compas.datastructures import Datastructure
 
 
 class TreeNode(Data):
     """A node of a tree data structure.
 
     Parameters
     ----------
@@ -56,26 +56,25 @@
             data["attributes"] = self.attributes
         if self.children:
             data["children"] = [child.__data__ for child in self.children]
         return data
 
     @classmethod
     def __from_data__(cls, data):
-
         name = data.get("name", None)
         attributes = data.get("attributes", {})
         children = data.get("children", [])
 
         node = cls(name=name, **attributes)
         for child in children:
             node.add(cls.__from_data__(child))
         return node
 
     def __init__(self, name=None, **kwargs):
-        super(TreeNode, self).__init__(name=name, **kwargs)
+        super(TreeNode, self).__init__(name=name)
         self.attributes = kwargs
         self._parent = None
         self._children = []
         self._tree = None
 
     def __repr__(self):
         if self._name:
@@ -231,29 +230,28 @@
     leaves : generator[:class:`compas.datastructures.TreeNode`]
         A generator of the leaves of the tree.
 
     Examples
     --------
     >>> from compas.datastructures import Tree, TreeNode
     >>> tree = Tree()
-    >>> root = TreeNode('root')
-    >>> branch = TreeNode('branch')
-    >>> leaf1 = TreeNode('leaf1')
-    >>> leaf2 = TreeNode('leaf2')
+    >>> root = TreeNode("root")
+    >>> branch = TreeNode("branch")
+    >>> leaf1 = TreeNode("leaf1")
+    >>> leaf2 = TreeNode("leaf2")
     >>> tree.add(root)
     >>> root.add(branch)
     >>> branch.add(leaf1)
     >>> branch.add(leaf2)
     >>> print(tree)
-    <Tree with 4 nodes, 1 branches, and 2 leaves>
-    >>> tree.print()
-    <TreeNode root>
-        <TreeNode branch>
-            <TreeNode leaf2>
-            <TreeNode leaf1>
+    <Tree with 4 nodes>
+    |--<TreeNode: root>
+        |-- <TreeNode: branch>
+            |-- <TreeNode: leaf1>
+            |-- <TreeNode: leaf2>
 
     """
 
     DATASCHEMA = {
         "type": "object",
         "properties": {
             "root": TreeNode.DATASCHEMA,
@@ -277,14 +275,17 @@
         tree.add(root)
         return tree
 
     def __init__(self, name=None, **kwargs):
         super(Tree, self).__init__(kwargs, name=name)
         self._root = None
 
+    def __str__(self):
+        return "<Tree with {} nodes>\n{}".format(len(list(self.nodes)), self.get_hierarchy_string(max_depth=3))
+
     @property
     def root(self):
         return self._root
 
     def add(self, node, parent=None):
         """
         Add a node to the tree.
@@ -431,45 +432,46 @@
         """
         nodes = []
         for node in self.nodes:
             if node.name == name:
                 nodes.append(node)
         return nodes
 
-    def __repr__(self):
-        return "<Tree with {} nodes>".format(len(list(self.nodes)))
-
-    def print_hierarchy(self, max_depth=None):
+    def get_hierarchy_string(self, max_depth=None):
         """
-        Print the spatial hierarchy of the tree.
+        Return string representation for the spatial hierarchy of the tree.
 
         Parameters
         ----------
         max_depth : int, optional
             The maximum depth of the hierarchy to print.
             Default is ``None``, in which case the entire hierarchy is printed.
 
         Returns
         -------
-        None
+        str
+            String representing the spatial hierarchy of the tree.
 
         """
 
-        def _print(node, prefix="", last=True, depth=0):
+        hierarchy = []
 
+        def traverse(node, hierarchy, prefix="", last=True, depth=0):
             if max_depth is not None and depth > max_depth:
                 return
 
             connector = "└── " if last else "├── "
-            print("{}{}{}".format(prefix, connector, node))
+            hierarchy.append("{}{}{}".format(prefix, connector, node))
             prefix += "    " if last else "│   "
             for i, child in enumerate(node.children):
-                _print(child, prefix, i == len(node.children) - 1, depth + 1)
+                traverse(child, hierarchy, prefix, i == len(node.children) - 1, depth + 1)
+
+        traverse(self.root, hierarchy)
 
-        _print(self.root)
+        return "\n".join(hierarchy)
 
     def to_graph(self, key_mapper=None):
         """Convert the tree to a graph.
 
         Parameters
         ----------
         key_mapper : callable, optional
```

### Comparing `COMPAS-2.1.0/src/compas/datastructures/volmesh/volmesh.py` & `compas-2.1.1/src/compas/datastructures/volmesh/volmesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 from itertools import product
 from random import sample
 
-from compas.datastructures.datastructure import Datastructure
-from compas.datastructures.attributes import VertexAttributeView
+from compas.datastructures import Mesh
+from compas.datastructures.attributes import CellAttributeView
 from compas.datastructures.attributes import EdgeAttributeView
 from compas.datastructures.attributes import FaceAttributeView
-from compas.datastructures.attributes import CellAttributeView
-from compas.datastructures import Mesh
-
+from compas.datastructures.attributes import VertexAttributeView
+from compas.datastructures.datastructure import Datastructure
 from compas.files import OBJ
-
-from compas.geometry import Point
-from compas.geometry import Vector
+from compas.geometry import Box
 from compas.geometry import Line
+from compas.geometry import Point
 from compas.geometry import Polygon
 from compas.geometry import Polyhedron
-from compas.geometry import Box
+from compas.geometry import Vector
 from compas.geometry import add_vectors
 from compas.geometry import bestfit_plane
+from compas.geometry import bounding_box
 from compas.geometry import centroid_points
 from compas.geometry import centroid_polygon
 from compas.geometry import centroid_polyhedron
 from compas.geometry import distance_point_point
 from compas.geometry import length_vector
 from compas.geometry import normal_polygon
 from compas.geometry import normalize_vector
+from compas.geometry import oriented_bounding_box
 from compas.geometry import project_point_plane
 from compas.geometry import scale_vector
 from compas.geometry import subtract_vectors
-from compas.geometry import bounding_box
 from compas.geometry import transform_points
-from compas.geometry import oriented_bounding_box
-
-from compas.utilities import linspace
-from compas.utilities import pairwise
-
+from compas.itertools import linspace
+from compas.itertools import pairwise
 from compas.tolerance import TOL
 
 
 def iter_edges_from_vertices(vertices):
     for i, u in enumerate(vertices):
         j = (i + 1) % len(vertices)
         yield u, vertices[j]
@@ -198,23 +194,15 @@
 
         volmesh._max_vertex = data.get("max_vertex", volmesh._max_vertex)
         volmesh._max_face = data.get("max_face", volmesh._max_face)
         volmesh._max_cell = data.get("max_cell", volmesh._max_cell)
 
         return volmesh
 
-    def __init__(
-        self,
-        default_vertex_attributes=None,
-        default_edge_attributes=None,
-        default_face_attributes=None,
-        default_cell_attributes=None,
-        name=None,
-        **kwargs
-    ):
+    def __init__(self, default_vertex_attributes=None, default_edge_attributes=None, default_face_attributes=None, default_cell_attributes=None, name=None, **kwargs):  # fmt: skip
         super(VolMesh, self).__init__(kwargs, name=name)
         self._max_vertex = -1
         self._max_face = -1
         self._max_cell = -1
         self._vertex = {}
         self._halfface = {}
         self._cell = {}
@@ -439,17 +427,15 @@
         :meth:`from_vertices_and_cells`
 
         """
         vertex_index = self.vertex_index()
         vertices = [self.vertex_coordinates(vertex) for vertex in self.vertices()]
         cells = []
         for cell in self.cells():
-            faces = [
-                [vertex_index[vertex] for vertex in self.halfface_vertices(face)] for face in self.cell_faces(cell)
-            ]
+            faces = [[vertex_index[vertex] for vertex in self.halfface_vertices(face)] for face in self.cell_faces(cell)]
             cells.append(faces)
         return vertices, cells
 
     def cell_to_mesh(self, cell):
         """Construct a mesh object from from a cell of a volmesh.
 
         Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/files/__init__.py` & `compas-2.1.1/src/compas/files/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/files/_xml/xml_cli.py` & `compas-2.1.1/src/compas/files/_xml/xml_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,17 @@
 from __future__ import division
 from __future__ import print_function
 
 import xml.etree.ElementTree as ET
 from urllib import addinfourl
 
 import compas
-
 from compas.files._xml.xml_shared import shared_xml_from_file
 from compas.files._xml.xml_shared import shared_xml_from_string
 
-
 if compas.IPY:
     import clr
 
     clr.AddReference("System.Xml")
 
     from System.IO import MemoryStream
     from System.IO import StreamReader
```

### Comparing `COMPAS-2.1.0/src/compas/files/_xml/xml_cpython.py` & `compas-2.1.1/src/compas/files/_xml/xml_cpython.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/files/_xml/xml_pre_38.py` & `compas-2.1.1/src/compas/files/_xml/xml_pre_38.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import xml.etree.ElementTree as ET
+
 from compas import _iotools
 from compas.files._xml.xml_cpython import prettify_string  # noqa: F401
 
 # doesn't need special handling for pre-3.8 so we just import
 
 
 def xml_from_file(source, tree_parser=None):
```

### Comparing `COMPAS-2.1.0/src/compas/files/_xml/xml_shared.py` & `compas-2.1.1/src/compas/files/_xml/xml_shared.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/constants.py` & `compas-2.1.1/src/compas/files/gltf/constants.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 COMPONENT_TYPE_BYTE = 5120
 COMPONENT_TYPE_UNSIGNED_BYTE = 5121
 COMPONENT_TYPE_SHORT = 5122
 COMPONENT_TYPE_UNSIGNED_SHORT = 5123
 COMPONENT_TYPE_UNSIGNED_INT = 5125
 COMPONENT_TYPE_FLOAT = 5126
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/data_classes.py` & `compas-2.1.1/src/compas/files/gltf/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 
 class AlphaMode(object):
     BLEND = "BLEND"
     MASK = "MASK"
     OPAQUE = "OPAQUE"
 
@@ -26,18 +26,15 @@
         if not self.extensions:
             self.extensions = {}
         self.extensions.update({extension.key: extension})
 
     def extensions_to_data(self, **kwargs):
         if not self.extensions:
             return None
-        return {
-            key: value.to_data(**kwargs) if hasattr(value, "to_data") else value
-            for key, value in self.extensions.items()
-        }
+        return {key: value.to_data(**kwargs) if hasattr(value, "to_data") else value for key, value in self.extensions.items()}
 
     @classmethod
     def extensions_from_data(cls, data):
         # i hate hate hate this local import, but i don't see a good way around it
         from compas.files.gltf.extensions import SUPPORTED_EXTENSIONS
 
         if not data:
@@ -484,17 +481,15 @@
         self.channels = channels
         self.samplers_dict = samplers_dict
         self.name = name
 
         self._sampler_index_by_key = None
 
     def to_data(self, samplers_list, node_index_by_key):
-        channels = [
-            channel_data.to_data(node_index_by_key, self._sampler_index_by_key) for channel_data in self.channels
-        ]
+        channels = [channel_data.to_data(node_index_by_key, self._sampler_index_by_key) for channel_data in self.channels]
         animation_dict = {
             "channels": channels,
             "samplers": samplers_list,
         }
         if self.name is not None:
             animation_dict["name"] = self.name
         if self.extras is not None:
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/extensions.py` & `compas-2.1.1/src/compas/files/gltf/extensions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .data_classes import BaseGLTFDataClass
-from .data_classes import TextureInfoData
 from .data_classes import NormalTextureInfoData
+from .data_classes import TextureInfoData
 
 
 def create_if_data(cls, data, attr):
     return cls.from_data(data.get(attr)) if attr in data and data[attr] is not None else None
 
 
 class KHR_materials_transmission(BaseGLTFDataClass):
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/gltf.py` & `compas-2.1.1/src/compas/files/gltf/gltf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 from compas.files.gltf.gltf_exporter import GLTFExporter
 from compas.files.gltf.gltf_parser import GLTFParser
 from compas.files.gltf.gltf_reader import GLTFReader
 
 
 class GLTF(object):
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/gltf_children.py` & `compas-2.1.1/src/compas/files/gltf/gltf_children.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 
 class GLTFChildren(object):
     def __init__(self, context, values):
         self._values = list(values)
         self._context = context
         for v in values:
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/gltf_content.py` & `compas-2.1.1/src/compas/files/gltf/gltf_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,17 +130,15 @@
         for animation_key, animation in self.animations.items():
             visited_sampler_keys = []
             for channel in animation.channels:
                 if not node_visit_log[channel.target.node]:
                     animation.channels.remove(channel)
                 else:
                     visited_sampler_keys.append(channel.sampler)
-            animation.samplers_dict = {
-                key: animation.samplers_dict[key] for key in animation.samplers_dict if key in visited_sampler_keys
-            }
+            animation.samplers_dict = {key: animation.samplers_dict[key] for key in animation.samplers_dict if key in visited_sampler_keys}
             if not animation.samplers_dict:
                 del self.animations[animation_key]
 
         # remove skins referencing no existing nodes
         for key, skin_data in self.skins.items():
             for joint_key in skin_data.joints:
                 if not node_visit_log[joint_key]:
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/gltf_exporter.py` & `compas-2.1.1/src/compas/files/gltf/gltf_exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 import array
 import base64
 import json
 import os
-import struct
 import shutil
+import struct
 
 from compas.files.gltf.constants import COMPONENT_TYPE_ENUM
 from compas.files.gltf.constants import COMPONENT_TYPE_FLOAT
 from compas.files.gltf.constants import COMPONENT_TYPE_UNSIGNED_INT
 from compas.files.gltf.constants import COMPONENT_TYPE_UNSIGNED_SHORT
 from compas.files.gltf.constants import NUM_COMPONENTS_BY_TYPE_ENUM
 from compas.files.gltf.constants import TYPE_MAT4
 from compas.files.gltf.constants import TYPE_SCALAR
 from compas.files.gltf.constants import TYPE_VEC2
 from compas.files.gltf.constants import TYPE_VEC3
 from compas.files.gltf.constants import TYPE_VEC4
 from compas.files.gltf.data_classes import BaseGLTFDataClass
 
-
 # This fails on IronPython 2.7.8 (eg. Rhino 6 on Windows)
 # but works on IronPython 2.7.9 (Rhino 6 on Mac)
 try:
     struct.pack_into("<I", bytearray(4), 0, 0)
     USE_BYTEARRAY_BUFFERS = True
 except TypeError:
     USE_BYTEARRAY_BUFFERS = False
@@ -175,17 +174,15 @@
         # get the extensions that are in the attributes
         for a in dir(item):
             if not a.startswith("__") and not callable(getattr(item, a)):
                 if isinstance(getattr(item, a), BaseGLTFDataClass):
                     self._add_extensions_recursively(getattr(item, a))
         if item.extensions is not None:
             for ek, e in item.extensions.items():
-                if (
-                    self._content.extensions_used is None
-                ):  # attention: self._content.extension exists if we have general extensions.
+                if self._content.extensions_used is None:  # attention: self._content.extension exists if we have general extensions.
                     self._content.extensions_used = []
                 if ek not in self._content.extensions_used:
                     self._content.extensions_used.append(ek)
                 self._add_extensions_recursively(e)
 
     def _add_images(self):
         if not self._content.images:
@@ -204,20 +201,15 @@
             images_list[self._image_index_by_key[key]] = image_data.to_data(uri, buffer_view)
             self._add_extensions_recursively(image_data)
         self._gltf_dict["images"] = images_list
 
     def _construct_image_data_uri(self, image_data):
         if image_data.data is None:
             return None
-        return (
-            "data:"
-            + (image_data.mime_type if image_data.mime_type else "")
-            + ";base64,"
-            + base64.b64encode(image_data.data).decode("ascii")
-        )
+        return "data:" + (image_data.mime_type if image_data.mime_type else "") + ";base64," + base64.b64encode(image_data.data).decode("ascii")
 
     def _add_extensions(self):
         if not self._content.extensions_used:
             return
         self._gltf_dict["extensionsRequired"] = self._content.extensions_used
         self._gltf_dict["extensionsUsed"] = self._content.extensions_used
 
@@ -230,17 +222,15 @@
         self._gltf_dict["samplers"] = samplers_list
 
     def _add_textures(self):
         if not self._content.textures:
             return
         textures_list = [None] * len(self._content.textures)
         for key, texture_data in self._content.textures.items():
-            textures_list[self._texture_index_by_key[key]] = texture_data.to_data(
-                self._sampler_index_by_key, self._image_index_by_key
-            )
+            textures_list[self._texture_index_by_key[key]] = texture_data.to_data(self._sampler_index_by_key, self._image_index_by_key)
             self._add_extensions_recursively(texture_data)
         self._gltf_dict["textures"] = textures_list
 
     def _add_materials(self):
         if not self._content.materials:
             return
         materials_list = [None] * len(self._content.materials)
@@ -350,29 +340,25 @@
                 self._skin_index_by_key,
             )
         self._gltf_dict["nodes"] = node_list
 
     def _construct_primitives(self, mesh_data):
         primitives = []
         for primitive_data in mesh_data.primitive_data_list:
-            indices_accessor = self._construct_accessor(
-                primitive_data.indices, COMPONENT_TYPE_UNSIGNED_SHORT, TYPE_SCALAR
-            )
+            indices_accessor = self._construct_accessor(primitive_data.indices, COMPONENT_TYPE_UNSIGNED_SHORT, TYPE_SCALAR)
 
             attributes = {}
             for attr in primitive_data.attributes:
                 component_type = COMPONENT_TYPE_UNSIGNED_INT if attr.startswith("JOINT") else COMPONENT_TYPE_FLOAT
                 type_ = TYPE_VEC3
                 if len(primitive_data.attributes[attr][0]) == 4:
                     type_ = TYPE_VEC4
                 if len(primitive_data.attributes[attr][0]) == 2:
                     type_ = TYPE_VEC2
-                attributes[attr] = self._construct_accessor(
-                    primitive_data.attributes[attr], component_type, type_, True
-                )
+                attributes[attr] = self._construct_accessor(primitive_data.attributes[attr], component_type, type_, True)
 
             targets = []
             for target in primitive_data.targets or []:
                 target_dict = {}
                 for attr in target:
                     component_type = COMPONENT_TYPE_FLOAT
                     type_ = TYPE_VEC3
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/gltf_mesh.py` & `compas-2.1.1/src/compas/files/gltf/gltf_mesh.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 import itertools
 
 from compas.files.gltf.constants import VERTEX_COUNT_BY_MODE
 from compas.files.gltf.data_classes import PrimitiveData
-from compas.files.gltf.helpers import get_weighted_mesh_vertices
-from compas.files.gltf.helpers import get_unweighted_primitive_vertices
 from compas.files.gltf.helpers import get_mode
+from compas.files.gltf.helpers import get_unweighted_primitive_vertices
+from compas.files.gltf.helpers import get_weighted_mesh_vertices
 
 
 class GLTFMesh(object):
     """Object containing mesh data in a format compatible with the glTF standard.
 
     Attributes
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/gltf_node.py` & `compas-2.1.1/src/compas/files/gltf/gltf_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 from math import fabs
 
 from compas.files.gltf.gltf_children import GLTFChildren
 from compas.files.gltf.helpers import get_matrix_from_col_major_list
 from compas.files.gltf.helpers import matrix_to_col_major_order
 from compas.geometry import identity_matrix
@@ -158,18 +158,15 @@
     def rotation(self, value):
         if value is None:
             self._rotation = value
             return
         if self._matrix:
             raise Exception("Cannot set rotation when matrix is set.")
         if not isinstance(value, list) or len(value) != 4 or fabs(sum([q**2 for q in value]) - 1) > 1e-03:
-            raise Exception(
-                "Invalid rotation.  Rotations are expected to be given as "
-                "unit quaternions of the form [q1, q2, q3, q4]"
-            )
+            raise Exception("Invalid rotation.  Rotations are expected to be given as " "unit quaternions of the form [q1, q2, q3, q4]")
         self._rotation = value
 
     @property
     def scale(self):
         return self._scale
 
     @scale.setter
@@ -198,16 +195,15 @@
             raise Exception("Cannot set matrix when translation, rotation or scale is set.")
         if not isinstance(value, list) or not value or not value[0] or not isinstance(value[0], list):
             raise Exception("Invalid matrix. A list of lists is expected.")
         if len(value) != 4 or len(value[0]) != 4:
             raise Exception("Invalid matrix. A 4x4 matrix is expected.")
         if value[3] != [0, 0, 0, 1]:
             raise Exception(
-                "Invalid matrix.  A matrix without shear or skew is expected.  It must be of "
-                "the form TRS, where T is a translation, R is a rotation and S is a scaling."
+                "Invalid matrix.  A matrix without shear or skew is expected.  It must be of " "the form TRS, where T is a translation, R is a rotation and S is a scaling."
             )
         self._matrix = value
 
     @property
     def mesh_data(self):
         return self.context.meshes.get(self.mesh_key)
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/gltf_parser.py` & `compas-2.1.1/src/compas/files/gltf/gltf_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 from compas.files.gltf.data_classes import AnimationData
 from compas.files.gltf.data_classes import AnimationSamplerData
 from compas.files.gltf.data_classes import CameraData
 from compas.files.gltf.data_classes import ChannelData
 from compas.files.gltf.data_classes import MaterialData
 from compas.files.gltf.data_classes import PrimitiveData
@@ -38,34 +38,20 @@
 
     def parse(self):
         self.content.default_scene_key = self._get_default_scene()
         self.content.extras = self._get_extras()
         self.content.extensions = self._get_extensions()
 
         self.content.images = {key: image_data for key, image_data in enumerate(self.reader.image_data)}
-        self.content.samplers = {
-            key: SamplerData.from_data(sampler) for key, sampler in enumerate(self.reader.json.get("samplers", []))
-        }
-        self.content.textures = {
-            key: TextureData.from_data(texture) for key, texture in enumerate(self.reader.json.get("textures", []))
-        }
-        self.content.materials = {
-            key: MaterialData.from_data(material) for key, material in enumerate(self.reader.json.get("materials", []))
-        }
-        self.content.cameras = {
-            key: CameraData.from_data(camera) for key, camera in enumerate(self.reader.json.get("cameras", []))
-        }
-        self.content.skins = {
-            key: SkinData.from_data(skin, self.reader.data[skin["inverseBindMatrices"]])
-            for key, skin in enumerate(self.reader.json.get("skins", []))
-        }
-        self.content.animations = {
-            key: self._get_animation_data(animation)
-            for key, animation in enumerate(self.reader.json.get("animations", []))
-        }
+        self.content.samplers = {key: SamplerData.from_data(sampler) for key, sampler in enumerate(self.reader.json.get("samplers", []))}
+        self.content.textures = {key: TextureData.from_data(texture) for key, texture in enumerate(self.reader.json.get("textures", []))}
+        self.content.materials = {key: MaterialData.from_data(material) for key, material in enumerate(self.reader.json.get("materials", []))}
+        self.content.cameras = {key: CameraData.from_data(camera) for key, camera in enumerate(self.reader.json.get("cameras", []))}
+        self.content.skins = {key: SkinData.from_data(skin, self.reader.data[skin["inverseBindMatrices"]]) for key, skin in enumerate(self.reader.json.get("skins", []))}
+        self.content.animations = {key: self._get_animation_data(animation) for key, animation in enumerate(self.reader.json.get("animations", []))}
 
         for mesh in self.reader.json.get("meshes", []):
             self._add_gltf_mesh(mesh)
         for node in self.reader.json.get("nodes", []):
             self._add_gltf_node(node)
         for scene in self.reader.json.get("scenes", []):
             self._add_gltf_scene(scene)
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/gltf_reader.py` & `compas-2.1.1/src/compas/files/gltf/gltf_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 import base64
 import json
 import os
 import re
 import struct
 
@@ -234,18 +234,15 @@
         byte_stride = buffer_view.get("byteStride", expected_length)
 
         unpack_from = struct.Struct(format_).unpack_from
 
         buffer_index = buffer_view["buffer"]
         buffer = self._get_buffer(buffer_index)
 
-        data = [
-            unpack_from(buffer[i : i + byte_stride].tobytes())
-            for i in range(offset, offset + count * byte_stride, byte_stride)
-        ]  # noqa E203
+        data = [unpack_from(buffer[i : i + byte_stride].tobytes()) for i in range(offset, offset + count * byte_stride, byte_stride)]  # noqa E203
 
         if num_components == 1:
             data = [item[0] for item in data]  # unwrap scalars from tuple
 
         return data
 
     def _get_buffer(self, buffer_index):
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/gltf_scene.py` & `compas-2.1.1/src/compas/files/gltf/gltf_scene.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 from compas.files.gltf.gltf_children import GLTFChildren
 
 
 class GLTFScene(object):
     """Object representing the COMPAS consumable part of a glTF scene.
```

### Comparing `COMPAS-2.1.0/src/compas/files/gltf/helpers.py` & `compas-2.1.1/src/compas/files/gltf/helpers.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 import itertools
 import math
 
 from compas.files.gltf.constants import MODE_BY_VERTEX_COUNT
```

### Comparing `COMPAS-2.1.0/src/compas/files/obj.py` & `compas-2.1.1/src/compas/files/obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
 
     >>> from compas.datastructures import Mesh
     >>> from compas.files import OBJ
 
     Write mesh data to a file.
 
     >>> mesh = Mesh.from_polyhedron(12)
-    >>> obj = OBJ('mesh.obj')
+    >>> obj = OBJ("mesh.obj")
     >>> obj.write(mesh)
 
     Read mesh data from a file.
 
-    >>> obj = OBJ('mesh.obj')
+    >>> obj = OBJ("mesh.obj")
     >>> obj.read()
     >>> mesh = Mesh.from_vertices_and_faces(obj.vertices, obj.faces)
 
     Reading and writing of multiple meshes as separate objects in a single OBJ file.
 
     >>> from compas.geometry import Pointcloud, Translation
     >>> from compas.datastructures import Mesh
@@ -70,28 +70,26 @@
     Write mesh data to a file.
 
     >>> meshes = []
     >>> for point in Pointcloud.from_bounds(10, 10, 10, 100):
     ...     mesh = Mesh.from_polyhedron(12)
     ...     mesh.transform(Translation.from_vector(point))
     ...     meshes.append(mesh)
-    ...
-    >>> obj = OBJ('meshes.obj')
+    >>> obj = OBJ("meshes.obj")
     >>> obj.write(meshes)
 
     Read mesh data from a file.
 
-    >>> obj = OBJ('meshes.obj')
+    >>> obj = OBJ("meshes.obj")
     >>> obj.read()
     >>> meshes = []
     >>> for name in obj.objects:
-    ...     mesh = Mesh.from_vertices_and_faces(* obj.objects[name])
+    ...     mesh = Mesh.from_vertices_and_faces(*obj.objects[name])
     ...     mesh.name = name
     ...     meshes.append(mesh)
-    ...
 
     """
 
     def __init__(self, filepath, precision=None):
         self.filepath = filepath
         self.precision = precision
         self._is_parsed = False
```

### Comparing `COMPAS-2.1.0/src/compas/files/off.py` & `compas-2.1.1/src/compas/files/off.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,17 +250,15 @@
     def __init__(self, filepath, mesh, author=None, email=None, date=None, precision=None):
         self.filepath = filepath
         self.mesh = mesh
         self.author = author
         self.email = email
         self.date = date
         self.precision = precision or compas.PRECISION
-        self.vertex_tpl = (
-            "{0:." + self.precision + "}" + " {1:." + self.precision + "}" + " {2:." + self.precision + "}\n"
-        )
+        self.vertex_tpl = "{0:." + self.precision + "}" + " {1:." + self.precision + "}" + " {2:." + self.precision + "}\n"
         self.v = mesh.number_of_vertices()
         self.f = mesh.number_of_faces()
         self.e = mesh.number_of_edges()
         self.file = None
 
     def write(self):
         """Write the meshes to the file.
```

### Comparing `COMPAS-2.1.0/src/compas/files/ply.py` & `compas-2.1.1/src/compas/files/ply.py`

 * *Files identical despite different names*

```diff
@@ -644,17 +644,15 @@
     def __init__(self, filepath, mesh, author=None, email=None, date=None, precision=None):
         self.filepath = filepath
         self.mesh = mesh
         self.author = author
         self.email = email
         self.date = date
         self.precision = precision or compas.PRECISION
-        self.vertex_tpl = (
-            "{0:." + self.precision + "}" + " {1:." + self.precision + "}" + " {2:." + self.precision + "}\n"
-        )
+        self.vertex_tpl = "{0:." + self.precision + "}" + " {1:." + self.precision + "}" + " {2:." + self.precision + "}\n"
         self.v = mesh.number_of_vertices()
         self.f = mesh.number_of_faces()
         self.e = mesh.number_of_edges()
         self.file = None
 
     def write(self):
         """Write the data to a file.
```

### Comparing `COMPAS-2.1.0/src/compas/files/stl.py` & `compas-2.1.1/src/compas/files/stl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import struct
+
 from compas import _iotools
 from compas.geometry import Translation
 from compas.tolerance import TOL
 
 
 class STL(object):
     """Class for working with STL files.
```

### Comparing `COMPAS-2.1.0/src/compas/files/xml.py` & `compas-2.1.1/src/compas/files/xml.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/geometry/__init__.py` & `compas-2.1.1/src/compas/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/_algebra.py` & `compas-2.1.1/src/compas/geometry/_core/_algebra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from copy import deepcopy
-from math import acos, atan2, asin, cos, fabs, pi, sin, sqrt, tan
-from compas.tolerance import TOL
+from math import acos
+from math import asin
+from math import atan2
+from math import cos
+from math import fabs
+from math import pi
+from math import sin
+from math import sqrt
+from math import tan
 
+from compas.tolerance import TOL
 
 _SPEC2TUPLE = {
     "sxyz": (0, 0, 0, 0),
     "sxyx": (0, 0, 1, 0),
     "sxzy": (0, 1, 0, 0),
     "sxzx": (0, 1, 1, 0),
     "syzx": (1, 0, 0, 0),
@@ -2029,18 +2037,15 @@
         The rotation angle in radians.
 
     """
     eps = 0.01  # margin to allow for rounding errors
     eps2 = 0.1  # margin to distinguish between 0 and 180 degrees
 
     if all(fabs(M[i][j] - M[j][i]) < eps for i, j in [(0, 1), (0, 2), (1, 2)]):
-        if (
-            all(fabs(M[i][j] - M[j][i]) < eps2 for i, j in [(0, 1), (0, 2), (1, 2)])
-            and fabs(M[0][0] + M[1][1] + M[2][2] - 3) < eps2
-        ):
+        if all(fabs(M[i][j] - M[j][i]) < eps2 for i, j in [(0, 1), (0, 2), (1, 2)]) and fabs(M[0][0] + M[1][1] + M[2][2] - 3) < eps2:
             return [0, 0, 0], 0
 
         angle = pi
         xx = (M[0][0] + 1) / 2
         yy = (M[1][1] + 1) / 2
         zz = (M[2][2] + 1) / 2
         xy = (M[0][1] + M[1][0]) / 4
@@ -2064,19 +2069,15 @@
                 axis = [root_half, root_half, 0]
             else:
                 z = sqrt(zz)
                 axis = [xz / z, yz / z, z]
 
         return axis, angle
 
-    s = sqrt(
-        (M[2][1] - M[1][2]) * (M[2][1] - M[1][2])
-        + (M[0][2] - M[2][0]) * (M[0][2] - M[2][0])
-        + (M[1][0] - M[0][1]) * (M[1][0] - M[0][1])
-    )
+    s = sqrt((M[2][1] - M[1][2]) * (M[2][1] - M[1][2]) + (M[0][2] - M[2][0]) * (M[0][2] - M[2][0]) + (M[1][0] - M[0][1]) * (M[1][0] - M[0][1]))
 
     # should this also be an eps?
     if fabs(s) < 0.001:
         s = 1
 
     angle = acos((M[0][0] + M[1][1] + M[2][2] - 1) / 2)
 
@@ -2342,15 +2343,15 @@
 
 
 def matrix_from_orthogonal_projection(plane):
     """Returns an orthogonal projection matrix to project onto a plane.
 
     Parameters
     ----------
-    plane : [point, normal] | :class:`compas.geometry.Plane`
+    plane : [point, normal]
         The plane to project onto.
 
     Returns
     -------
     list[list[float]]
         The 4x4 transformation matrix representing an orthogonal projection.
 
@@ -2375,15 +2376,15 @@
 
 
 def matrix_from_parallel_projection(plane, direction):
     """Returns an parallel projection matrix to project onto a plane.
 
     Parameters
     ----------
-    plane : [point, normal] | :class:`compas.geometry.Plane`
+    plane : [point, normal]
         The plane to project onto.
     direction : [float, float, float] | :class:`compas.geometry.Vector`
         Direction of the projection.
 
     Returns
     -------
     list[list[float]]
@@ -2412,15 +2413,15 @@
 
 
 def matrix_from_perspective_projection(plane, center_of_projection):
     """Returns a perspective projection matrix to project onto a plane along lines that emanate from a single point, called the center of projection.
 
     Parameters
     ----------
-    plane : [point, normal] | :class:`compas.geometry.Plane`
+    plane : [point, normal]
         The plane to project onto.
     center_of_projection : [float, float, float] | :class:`compas.geometry.Point`
         The camera view point.
 
     Returns
     -------
     list[list[float]]
@@ -2676,18 +2677,18 @@
     Returns
     -------
     [float, float, float, float]
         Quaternion as a list of four real values ``[qw, qx, qy, qz]``.
 
     Examples
     --------
-    >>> axis =  [1.0, 0.0, 0.0]
-    >>> angle = math.pi/2
+    >>> axis = [1.0, 0.0, 0.0]
+    >>> angle = math.pi / 2
     >>> q = quaternion_from_axis_angle(axis, angle)
-    >>> allclose(q, [math.sqrt(2)/2, math.sqrt(2)/2, 0, 0])
+    >>> allclose(q, [math.sqrt(2) / 2, math.sqrt(2) / 2, 0, 0])
     True
 
     """
     m = matrix_from_axis_and_angle(axis, angle, None)
     q = quaternion_from_matrix(m)
     return q
 
@@ -2705,19 +2706,19 @@
     axis : [float, float, float]
         XYZ coordinates of the rotation axis vector.
     angle : float
         Angle of rotation in radians.
 
     Examples
     --------
-    >>> q = [1., 1., 0., 0.]
+    >>> q = [1.0, 1.0, 0.0, 0.0]
     >>> axis, angle = axis_angle_from_quaternion(q)
-    >>> allclose(axis, [1., 0., 0.])
+    >>> allclose(axis, [1.0, 0.0, 0.0])
     True
-    >>> allclose([angle], [math.pi/2], 1e-6)
+    >>> allclose([angle], [math.pi / 2], 1e-6)
     True
 
     """
     m = matrix_from_quaternion(q)
     axis, angle = axis_and_angle_from_matrix(m)
     return axis, angle
 
@@ -2764,17 +2765,17 @@
 
     The tolerance value used by this function is an absolute tolerance.
     It is more accurate to use a combination of absolute and relative tolerance.
     Therefor, use :func:`TOL.is_close` instead.
 
     Examples
     --------
-    >>> close(1., 1.001)
+    >>> close(1.0, 1.001)
     False
-    >>> close(1., 1.001, tol=1e-2)
+    >>> close(1.0, 1.001, tol=1e-2)
     True
     """
     return TOL.is_close(value1, value2, rtol=0.0, atol=tol)
 
 
 def allclose(l1, l2, tol=None):
     """Returns True if two lists are element-wise equal within a tolerance.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/angles.py` & `compas-2.1.1/src/compas/geometry/_core/angles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from math import pi
-from math import degrees
 from math import acos
+from math import degrees
+from math import pi
 
 from compas.tolerance import TOL
 
-from ._algebra import subtract_vectors
-from ._algebra import subtract_vectors_xy
+from ._algebra import cross_vectors
 from ._algebra import dot_vectors
 from ._algebra import dot_vectors_xy
 from ._algebra import length_vector
 from ._algebra import length_vector_xy
-from ._algebra import cross_vectors
+from ._algebra import subtract_vectors
+from ._algebra import subtract_vectors_xy
 
 
 def angle_vectors(u, v, deg=False, tol=None):
     """Compute the smallest angle between two vectors.
 
     Parameters
     ----------
@@ -380,17 +380,17 @@
 
 
 def angle_planes(a, b, deg=False):
     """Compute the smallest angle between the two normal vectors of two planes.
 
     Parameters
     ----------
-    a : [point, vector] | :class:`compas.geometry.Plane`
+    a : [point, vector]
         The first plane.
-    b : [point, vector] | :class:`compas.geometry.Plane`
+    b : [point, vector]
         The second plane.
     deg : bool, optional
         If True, returns the angle in degrees.
 
     Returns
     -------
     float
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/centroids.py` & `compas-2.1.1/src/compas/geometry/_core/centroids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 from math import fabs
 
-from compas.utilities import pairwise
+from compas.itertools import pairwise
 
 from ._algebra import add_vectors
-from ._algebra import subtract_vectors
-from ._algebra import subtract_vectors_xy
-from ._algebra import length_vector
-from ._algebra import length_vector_xy
-from ._algebra import dot_vectors
 from ._algebra import cross_vectors
 from ._algebra import cross_vectors_xy
+from ._algebra import dot_vectors
+from ._algebra import length_vector
+from ._algebra import length_vector_xy
 from ._algebra import scale_vector
+from ._algebra import subtract_vectors
+from ._algebra import subtract_vectors_xy
 from ._algebra import sum_vectors
 
 
 def midpoint_point_point(a, b):
     """Compute the midpoint of two points.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/distance.py` & `compas-2.1.1/src/compas/geometry/_core/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import fabs
 from math import sqrt
 
-from compas.utilities import pairwise
+from compas.itertools import pairwise
 from compas.tolerance import TOL
 
 from ._algebra import add_vectors
 from ._algebra import add_vectors_xy
-from ._algebra import subtract_vectors
-from ._algebra import subtract_vectors_xy
-from ._algebra import scale_vector
-from ._algebra import normalize_vector
-from ._algebra import length_vector
-from ._algebra import length_vector_xy
-from ._algebra import length_vector_sqrd
-from ._algebra import length_vector_sqrd_xy
 from ._algebra import cross_vectors
 from ._algebra import cross_vectors_xy
 from ._algebra import dot_vectors
+from ._algebra import length_vector
+from ._algebra import length_vector_sqrd
+from ._algebra import length_vector_sqrd_xy
+from ._algebra import length_vector_xy
+from ._algebra import normalize_vector
+from ._algebra import scale_vector
+from ._algebra import subtract_vectors
+from ._algebra import subtract_vectors_xy
 from ._algebra import vector_component
 from ._algebra import vector_component_xy
 
 
 def distance_point_point(a, b):
     """Compute the distance bewteen a and b.
 
@@ -294,15 +294,15 @@
 def distance_point_plane(point, plane):
     r"""Compute the distance from a point to a plane defined by origin point and normal.
 
     Parameters
     ----------
     point : [float, float, float] | :class:`compas.geometry.Point`
         Point coordinates.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         A point and a vector defining a plane.
 
     Returns
     -------
     float
         Distance between point and plane.
 
@@ -349,15 +349,15 @@
 def distance_point_plane_signed(point, plane):
     r"""Compute the signed distance from a point to a plane defined by origin point and normal.
 
     Parameters
     ----------
     point : [float, float, float] | :class:`compas.geometry.Point`
         Point coordinates.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         A point and a vector defining a plane.
 
     Returns
     -------
     float
         Distance between point and plane.
 
@@ -588,17 +588,17 @@
     >>> points = [[0, 0, 0], [1, 0, 0], [1, 1, 0], [0, 1, 0]]
     >>> cloud = [[0, 0, 0], [1, 0, 0], [1, 1, 0], [0, 1, 0]]
     >>> cp = closest_points_in_cloud_numpy(points, cloud, distances=True)
     >>> allclose(cp[1], [[0, 1, 1.4142, 1], [1, 0, 1, 1.4142], [1.4142, 1, 0, 1], [1, 1.4142, 1, 0]])
     True
 
     """
-    from numpy import asarray
     from numpy import argmin
     from numpy import argpartition
+    from numpy import asarray
     from scipy.spatial import distance_matrix
 
     points = asarray(points).reshape((-1, 3))
     cloud = asarray(cloud).reshape((-1, 3))
     d_matrix = distance_matrix(points, cloud, threshold=threshold)
     if num_nbrs == 1:
         indices = argmin(d_matrix, axis=1)
@@ -834,15 +834,15 @@
 def closest_point_on_plane(point, plane):
     """Compute closest point on a plane to a given point.
 
     Parameters
     ----------
     point : [float, float, float] | :class:`compas.geometry.Point`
         XYZ coordinates of point.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         The base point and normal defining the plane.
 
     Returns
     -------
     [float, float, float]
         XYZ coordinates of the closest point.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/normals.py` & `compas-2.1.1/src/compas/geometry/_core/normals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from ._algebra import subtract_vectors
-from ._algebra import subtract_vectors_xy
 from ._algebra import cross_vectors
 from ._algebra import cross_vectors_xy
 from ._algebra import length_vector
 from ._algebra import normalize_vector
-
+from ._algebra import subtract_vectors
+from ._algebra import subtract_vectors_xy
 from .centroids import centroid_points
 
 
 def normal_polygon(polygon, unitized=True):
     """Compute the normal of a polygon defined by a sequence of points.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/nurbs.py` & `compas-2.1.1/src/compas/geometry/_core/nurbs.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/predicates_2.py` & `compas-2.1.1/src/compas/geometry/_core/predicates_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.tolerance import TOL
-
-from compas.geometry import distance_point_point_xy
-from compas.geometry import distance_point_line_xy
 from compas.geometry import closest_point_on_segment_xy
-
+from compas.geometry import distance_point_line_xy
+from compas.geometry import distance_point_point_xy
+from compas.tolerance import TOL
 
 # =============================================================================
 # =============================================================================
 # =============================================================================
 # =============================================================================
 # =============================================================================
 # =============================================================================
@@ -56,24 +54,24 @@
     For more info, see [1]_.
 
     .. [1] Marsh, C. *Computational Geometry in Python: From Theory to Application*.
            Available at: https://www.toptal.com/python/computational-geometry-in-python-from-theory-to-implementation
 
     Examples
     --------
-    >>> print(is_ccw_xy([0,0,0], [0,1,0], [-1, 0, 0]))
+    >>> print(is_ccw_xy([0, 0, 0], [0, 1, 0], [-1, 0, 0]))
     True
 
-    >>> print(is_ccw_xy([0,0,0], [0,1,0], [+1, 0, 0]))
+    >>> print(is_ccw_xy([0, 0, 0], [0, 1, 0], [+1, 0, 0]))
     False
 
-    >>> print(is_ccw_xy([0,0,0], [1,0,0], [2,0,0]))
+    >>> print(is_ccw_xy([0, 0, 0], [1, 0, 0], [2, 0, 0]))
     False
 
-    >>> print(is_ccw_xy([0,0,0], [1,0,0], [2,0,0], True))
+    >>> print(is_ccw_xy([0, 0, 0], [1, 0, 0], [2, 0, 0], True))
     True
 
     """
     ab_x = b[0] - a[0]
     ab_y = b[1] - a[1]
     ac_x = c[0] - a[0]
     ac_y = c[1] - a[1]
@@ -449,15 +447,15 @@
 def is_point_in_circle_xy(point, circle):
     """Determine if a point lies in a circle lying on the XY-plane.
 
     Parameters
     ----------
     point : [float, float, float] | :class:`compas.geometry.Point`
         XY(Z) coordinates of a point (Z will be ignored).
-    circle : [[point, vector], float] | :class:`compas.geometry.Circle`
+    circle : [[point, vector], float]
         Center and radius of the circle on the XY plane.
 
     Returns
     -------
     bool
         True if the point lies in the circle.
         False otherwise.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/predicates_3.py` & `compas-2.1.1/src/compas/geometry/_core/predicates_3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.tolerance import TOL
-
-from compas.utilities import window
-
-from compas.geometry import subtract_vectors
+from compas.geometry import area_triangle
+from compas.geometry import centroid_points
+from compas.geometry import closest_point_on_segment
 from compas.geometry import cross_vectors
+from compas.geometry import distance_point_line
+from compas.geometry import distance_point_plane
+from compas.geometry import distance_point_point
 from compas.geometry import dot_vectors
-from compas.geometry import centroid_points
-from compas.geometry import normal_polygon
-from compas.geometry import area_triangle
 from compas.geometry import length_vector
-
-from compas.geometry import distance_point_point
-from compas.geometry import distance_point_plane
-from compas.geometry import distance_point_line
-from compas.geometry import closest_point_on_segment
-
+from compas.geometry import normal_polygon
+from compas.geometry import subtract_vectors
+from compas.itertools import window
+from compas.tolerance import TOL
 
 # =============================================================================
 # =============================================================================
 # =============================================================================
 # =============================================================================
 # =============================================================================
 # =============================================================================
@@ -126,15 +122,15 @@
 
     """
     if len(points) < 4:
         return True
 
     temp = points[:]
 
-    while True:
+    while len(temp) >= 3:
         a = temp.pop(0)
         b = temp.pop(0)
         c = temp.pop(0)
         if not is_colinear(a, b, c, tol):
             break
         if not temp:
             return True
@@ -237,17 +233,17 @@
 
 
 def is_parallel_plane_plane(plane1, plane2, tol=None):
     """Determine if two planes are parallel.
 
     Parameters
     ----------
-    plane1 : [point, vector] | :class:`compas.geometry.Plane`
+    plane1 : [point, vector]
         Plane 1.
-    plane2 : [point, vector] | :class:`compas.geometry.Plane`
+    plane2 : [point, vector]
         Plane 2.
     tol : float, optional
         A tolerance for verifying parallelity of the plane normals.
 
     Returns
     -------
     bool
@@ -333,17 +329,17 @@
 
 
 def is_perpendicular_plane_plane(plane1, plane2, tol=None):
     """Determine if two planes are perpendicular.
 
     Parameters
     ----------
-    plane1 : [point, vector] | :class:`compas.geometry.Plane`
+    plane1 : [point, vector]
         Plane 1.
-    plane2 : [point, vector] | :class:`compas.geometry.Plane`
+    plane2 : [point, vector]
         Plane 2.
     tol : float, optional
         A tolerance for verifying perpendicularity of the plane normals.
 
     Returns
     -------
     bool
@@ -425,15 +421,15 @@
 
 
 def is_polyhedron_convex(polyhedron):
     """Determine if a polyhedron is convex.
 
     Parameters
     ----------
-    polyhedron : [sequence[point], sequence[sequence[int]]] | :class:`compas.geometry.Polyhedron`
+    polyhedron : [sequence[point], sequence[sequence[int]]]
         A polyhedron defined by a sequence of points
         and a sequence of faces, with each face defined as a sequence of indices into the sequence of points.
 
     Returns
     -------
     bool
         True if the polyhedron is convex.
@@ -480,15 +476,15 @@
 def is_point_on_plane(point, plane, tol=None):
     """Determine if a point lies on a plane.
 
     Parameters
     ----------
     point : [float, float, float] | :class:`compas.geometry.Point`
         A point.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         A plane.
     tol : float, optional
         Tolerance for comparing the distance between the point and the plane to zero.
         Default is :attr:`TOL.absolute`.
 
     Returns
     -------
@@ -720,19 +716,15 @@
         if dot_vectors(c1, c2) >= 0:
             return True
         return False
 
     a, b, c = triangle
 
     if is_point_on_plane(point, (a, normal_polygon(triangle)), tol=tol):
-        if (
-            is_on_same_side(point, a, (b, c))
-            and is_on_same_side(point, b, (a, c))
-            and is_on_same_side(point, c, (a, b))
-        ):
+        if is_on_same_side(point, a, (b, c)) and is_on_same_side(point, b, (a, c)) and is_on_same_side(point, c, (a, b)):
             return True
 
     return False
 
 
 def is_point_in_polygon(point, polygon, tol=None):
     """Determine if a point is in the interior of a polygon.
@@ -816,15 +808,15 @@
 def is_point_in_polyhedron(point, polyhedron, tol=None):
     """Determine if the point lies inside the given polyhedron.
 
     Parameters
     ----------
     point : [float, float, float] | :class:`compas.geometry.Point`
         The test point.
-    polyhedron : [sequence[point], sequence[sequence[int]]] | :class:`compas.geometry.Polyhedron`.
+    polyhedron : [sequence[point], sequence[sequence[int]]]
         The polyhedron defined by a sequence of points
         and a sequence of faces, with each face defined as a sequence of indices into the sequence of points.
 
     Returns
     -------
     bool
         True, if the point lies in the polyhedron.
@@ -840,15 +832,15 @@
 def is_point_infrontof_plane(point, plane, tol=None):
     """Determine if a point lies in front of a plane.
 
     Parameters
     ----------
     point : [float, float, float] | :class:`compas.geometry.Point`
         A point.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         A plane.
     tol : float, optional
         A tolerance for membership verification.
 
     Returns
     -------
     bool
@@ -862,15 +854,15 @@
 def is_point_behind_plane(point, plane, tol=None):
     """Determine if a point lies behind a plane.
 
     Parameters
     ----------
     point : [float, float, float] | :class:`compas.geometry.Point`
         A point.
-    plane : [point,  normal] | :class:`compas.geometry.Plane`
+    plane : [point,  normal]
         A plane.
     tol : float, optional
         A tolerance for membership verification.
 
     Returns
     -------
     bool
@@ -1029,15 +1021,15 @@
 # def is_intersection_line_plane(line, plane, tol=None):
 #     """Determine if a line (ray) intersects with a plane.
 
 #     Parameters
 #     ----------
 #     line : [point, point] | :class:`compas.geometry.Line`
 #         A line.
-#     plane : [point, vector] | :class:`compas.geometry.Plane`
+#     plane : [point, vector]
 #         A plane.
 #     tol : float, optional
 #         A tolerance for intersection verification.
 
 #     Returns
 #     -------
 #     bool
@@ -1060,15 +1052,15 @@
 # def is_intersection_segment_plane(segment, plane, tol=None):
 #     """Determine if a line segment intersects with a plane.
 
 #     Parameters
 #     ----------
 #     segment : [point, point] | :class:`compas.geometry.Line`
 #         A line segment.
-#     plane : [point, vector] | :class:`compas.geometry.Plane`
+#     plane : [point, vector]
 #         A plane.
 #     tol : float, optional
 #         A tolerance for intersection verification.
 
 #     Returns
 #     -------
 #     bool
@@ -1095,17 +1087,17 @@
 
 
 # def is_intersection_plane_plane(plane1, plane2, tol=None):
 #     """Verifies if two planes intersect.
 
 #     Parameters
 #     ----------
-#     plane1 : [point, vector] | :class:`compas.geometry.Plane`
+#     plane1 : [point, vector]
 #         A plane.
-#     plane2 : [point, vector] | :class:`compas.geometry.Plane`
+#     plane2 : [point, vector]
 #         A plane.
 #     tol : float, optional
 #         A tolerance for intersection verification.
 
 #     Returns
 #     -------
 #     bool
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/quaternions.py` & `compas-2.1.1/src/compas/geometry/_core/quaternions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+
 from compas.tolerance import TOL
 
 
 def quaternion_norm(q):
     """Calculates the length (euclidean norm) of a quaternion.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/size.py` & `compas-2.1.1/src/compas/geometry/_core/size.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import fabs
 
-from compas.utilities import pairwise
+from compas.itertools import pairwise
 
-from ._algebra import subtract_vectors
-from ._algebra import subtract_vectors_xy
-from ._algebra import length_vector
 from ._algebra import cross_vectors
 from ._algebra import cross_vectors_xy
 from ._algebra import dot_vectors
-
+from ._algebra import length_vector
+from ._algebra import subtract_vectors
+from ._algebra import subtract_vectors_xy
 from .centroids import centroid_points
 from .centroids import centroid_points_xy
-
 from .normals import normal_triangle
 from .normals import normal_triangle_xy
 
 
 def area_triangle(triangle):
     """Compute the area of a triangle defined by three points.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/tangent.py` & `compas-2.1.1/src/compas/geometry/_core/tangent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import sqrt
 
 
 def tangent_points_to_circle_xy(circle, point):
     """Calculates the tangent points on a circle in the XY plane.
 
     Parameters
     ----------
-    circle : [plane, float] | :class:`compas.geometry.Circle`
+    circle : [plane, float]
         Plane and radius of the circle.
     point : [float, float] or [float, float, float] | :class:`compas.geometry.Point`
         XY(Z) coordinates of a point in the xy plane.
 
     Returns
     -------
     tuple[[float, float, 0.0], [float, float, 0.0]]
         the tangent points on the circle.
 
     Examples
     --------
-    >>> from compas.geometry import allclose
+    >>> from compas.tolerance import TOL
     >>> circle = ((0, 0, 0), (0, 0, 1)), 1.0
     >>> point = (2, 4, 0)
     >>> t1, t2 = tangent_points_to_circle_xy(circle, point)
-    >>> allclose(t1, [-0.772, 0.636, 0.000], 1e-3)
+    >>> TOL.is_allclose(t1, [-0.772, 0.636, 0.000], atol=1e-3)
     True
-    >>> allclose(t2, [0.972, -0.236, 0.000], 1e-3)
+    >>> TOL.is_allclose(t2, [0.972, -0.236, 0.000], atol=1e-3)
     True
 
     """
     plane, R = circle
     center, _ = plane
 
     cx, cy = center[:2]
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/transformations.py` & `compas-2.1.1/src/compas/geometry/_core/transformations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import math
 
-from ._algebra import scale_vector
-from ._algebra import scale_vector_xy
-from ._algebra import normalize_vector
 from ._algebra import add_vectors
 from ._algebra import add_vectors_xy
+from ._algebra import cross_vectors
+from ._algebra import dot_vectors
+from ._algebra import matrix_from_axis_and_angle
+from ._algebra import matrix_from_change_of_basis
+from ._algebra import matrix_from_scale_factors
+from ._algebra import multiply_matrices
+from ._algebra import multiply_matrix_vector
+from ._algebra import norm_vector
+from ._algebra import normalize_vector
+from ._algebra import scale_vector
+from ._algebra import scale_vector_xy
 from ._algebra import subtract_vectors
 from ._algebra import subtract_vectors_xy
-from ._algebra import dot_vectors
-from ._algebra import cross_vectors
+from ._algebra import transpose_matrix
 from ._algebra import vector_component
 from ._algebra import vector_component_xy
-from ._algebra import multiply_matrix_vector
-from ._algebra import multiply_matrices
-from ._algebra import transpose_matrix
-from ._algebra import norm_vector
-from ._algebra import matrix_from_axis_and_angle
-from ._algebra import matrix_from_scale_factors
-from ._algebra import matrix_from_change_of_basis
-
 from .angles import angle_vectors
-from .distance import closest_point_on_plane
 from .distance import closest_point_on_line
 from .distance import closest_point_on_line_xy
+from .distance import closest_point_on_plane
 
 
 # this function will not always work
 # it is also a duplicate of stuff found in matrices and frame
 def local_axes(a, b, c):
     u = b - a
     v = c - a
@@ -59,21 +58,21 @@
     Raises
     ------
     ValueError
         If xaxis and yaxis cannot span a plane.
 
     Examples
     --------
-    >>> from compas.geometry import allclose
+    >>> from compas.tolerance import TOL
     >>> xaxis = [1, 4, 5]
     >>> yaxis = [1, 0, -2]
     >>> xaxis, yaxis = orthonormalize_axes(xaxis, yaxis)
-    >>> allclose(xaxis, [0.1543, 0.6172, 0.7715], tol=0.001)
+    >>> TOL.is_allclose(xaxis, [0.1543, 0.6172, 0.7715], atol=0.001)
     True
-    >>> allclose(yaxis, [0.6929, 0.4891, -0.5298], tol=0.001)
+    >>> TOL.is_allclose(yaxis, [0.6929, 0.4891, -0.5298], atol=0.001)
     True
 
     """
     xaxis = normalize_vector(xaxis)
     yaxis = normalize_vector(yaxis)
     zaxis = cross_vectors(xaxis, yaxis)
     if not norm_vector(zaxis):
@@ -136,15 +135,15 @@
 
 
 def homogenize_and_flatten_frames(frames):
     """Homogenize a list of frames and flatten the 3D list into a 2D list.
 
     Parameters
     ----------
-    frames : sequence[[point, vector, vector] | :class:`compas.geometry.Frame`]
+    frames : sequence[[point, vector, vector]]
 
     Returns
     -------
     list[[float, float, float, `w`]]
         A list with 3 entries per frame: a homogenized point, and two homogenized vectors.
 
     Examples
@@ -173,15 +172,15 @@
     Returns
     -------
     list[[point, vector, vector]]
         The dehmogenized frame data.
 
     Examples
     --------
-    >>> points_and_vectors = [(1., 1., 1., 1.), (0., 1., 0., 0.), (1., 0., 0., 0.)]
+    >>> points_and_vectors = [(1.0, 1.0, 1.0, 1.0), (0.0, 1.0, 0.0, 0.0), (1.0, 0.0, 0.0, 0.0)]
     >>> dehomogenize_and_unflatten_frames(points_and_vectors)
     [[[1.0, 1.0, 1.0], [0.0, 1.0, 0.0], [1.0, 0.0, 0.0]]]
 
     """
     frames = dehomogenize(points_and_vectors)
     return [frames[i : i + 3] for i in range(0, len(frames), 3)]
 
@@ -242,15 +241,15 @@
 
 
 def transform_frames(frames, T):
     """Transform multiple frames with one transformation matrix.
 
     Parameters
     ----------
-    frames : sequence[[point, vector, vector] | :class:`compas.geometry.Frame`]
+    frames : sequence[[point, vector, vector]]
         A list of frames to be transformed.
     T : list[list[float]] | :class:`compas.geometry.Transformation`
         The transformation to apply on the frames.
 
     Returns
     -------
     list[[point, vector, vector]]
@@ -269,15 +268,15 @@
 
 
 def world_to_local_coordinates(frame, xyz):
     """Convert global coordinates to local coordinates.
 
     Parameters
     ----------
-    frame : [point, vector, vector] | :class:`compas.geometry.Frame`
+    frame : [point, vector, vector]
         The local coordinate system.
     xyz : array-like[[float, float, float] | :class:`compas.geometry.Point`]
         The global coordinates of the points to convert.
 
     Returns
     -------
     list[[float, float, float]]
@@ -299,15 +298,15 @@
 
 
 def local_to_world_coordinates(frame, xyz):
     """Convert local coordinates to global coordinates.
 
     Parameters
     ----------
-    frame : [point, vector, vector] | :class:`compas.geometry.Frame`
+    frame : [point, vector, vector]
         The local coordinate system.
     xyz : array-like[[float, float, float] | :class:`compas.geometry.Point`]
         The global coordinates of the points to convert.
 
     Returns
     -------
     list[[float, float, float]]
@@ -711,15 +710,15 @@
 def mirror_point_plane(point, plane):
     """Mirror a point about a plane.
 
     Parameters
     ----------
     point : list[float]
         XYZ coordinates of mirror point.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         Base point and normal defining the mirror plane.
 
     Returns
     -------
     [float, float, float]
         XYZ coordinates of the mirrored point.
 
@@ -731,15 +730,15 @@
 def mirror_points_plane(points, plane):
     """Mirror a point about a plane.
 
     Parameters
     ----------
     points : sequence[[float, float, float] | :class:`compas.geometry.Point`]
         List of points to mirror.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         Base point and normal defining the mirror plane.
 
     Returns
     -------
     list[[float, float, float]]
         The mirrored points.
 
@@ -757,15 +756,15 @@
 def project_point_plane(point, plane):
     """Project a point onto a plane.
 
     Parameters
     ----------
     point : [float, float, float] | :class:`compas.geometry.Point`
         XYZ coordinates of the point.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         Base point and normal vector defining the projection plane.
 
     Returns
     -------
     [float, float, float]
         XYZ coordinates of the projected point.
 
@@ -799,15 +798,15 @@
 def project_points_plane(points, plane):
     """Project multiple points onto a plane.
 
     Parameters
     ----------
     points : sequence[[float, float, float] | :class:`compas.geometry.Point`]
         List of points.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         Base point and normal vector defining the projection plane.
 
     Returns
     -------
     list[[float, float, float]]
         The projected points.
 
@@ -948,15 +947,15 @@
 def reflect_line_plane(line, plane, tol=None):
     """Bounce a line of a reflection plane.
 
     Parameters
     ----------
     line : [point, point] | :class:`compas.geometry.Line`
         Two points defining the line.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         Base point and normal vector of the plane.
     tol : float, optional
         A tolerance for finding the intersection between the line and the plane.
         Default is :func:`TOL.absolute`.
 
     Returns
     -------
@@ -1063,19 +1062,19 @@
 
 
 def orient_points(points, reference_plane, target_plane):
     """Orient points from one plane to another.
 
     Parameters
     ----------
-    points : sequence[[float, float, float] | :class:`compas.geometry.Point`]s
+    points : sequence[[float, float, float] | :class:`compas.geometry.Point`]
         XYZ coordinates of the points.
-    reference_plane : [point, vector] | :class:`compas.geometry.Plane`
+    reference_plane : [point, vector]
         Base point and normal defining a reference plane.
-    target_plane : [point, vector] | :class:`compas.geometry.Plane`
+    target_plane : [point, vector]
         Base point and normal defining a target plane.
 
     Returns
     -------
     list[[float, float, float]]
         XYZ coordinates of the oriented points.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/_core/transformations_numpy.py` & `compas-2.1.1/src/compas/geometry/_core/transformations_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from numpy import asarray
 from numpy import hstack
 from numpy import ones
-from numpy import vectorize
 from numpy import tile
-
+from numpy import vectorize
 from scipy.linalg import solve  # type: ignore
 
 from ._algebra import cross_vectors
 
 
 def transform_points_numpy(points, T):
     """Transform multiple points with one Transformation using numpy.
@@ -66,43 +65,43 @@
 
 
 def transform_frames_numpy(frames, T):
     """Transform multiple frames with one Transformation usig numpy.
 
     Parameters
     ----------
-    frames : sequence[[point, vector, vector] | :class:`compas.geometry.Frame`]
+    frames : sequence[[point, vector, vector]]
         A list of frames to be transformed.
     T : :class:`compas.geometry.Transformation`
         The transformation to apply on the frames.
 
     Returns
     -------
     (N, 3, 3) ndarray
         The transformed frames.
 
     Examples
     --------
     >>> from compas.geometry import Frame, matrix_from_axis_and_angle
     >>> frames = [Frame([1, 0, 0], [1, 2, 4], [4, 7, 1]), Frame([0, 2, 0], [5, 2, 1], [0, 2, 1])]
-    >>> T =  matrix_from_axis_and_angle([0, 2, 0], math.radians(45), point=[4, 5, 6])
+    >>> T = matrix_from_axis_and_angle([0, 2, 0], math.radians(45), point=[4, 5, 6])
     >>> transformed_frames = transform_frames_numpy(frames, T)
 
     """
     T = asarray(T)
     points_and_vectors = homogenize_and_flatten_frames_numpy(frames)
     return dehomogenize_and_unflatten_frames_numpy(points_and_vectors.dot(T.T))
 
 
 def world_to_local_coordinates_numpy(frame, xyz):
     """Convert global coordinates to local coordinates.
 
     Parameters
     ----------
-    frame : [point, vector, vector] | :class:`compas.geometry.Frame`
+    frame : [point, vector, vector]
         The local coordinate system.
     xyz : array-like[[float, float, float] | :class:`compas.geometry.Point`]
         The global coordinates of the points to convert.
 
     Returns
     -------
     (N, 3) ndarray
@@ -127,15 +126,15 @@
 
 
 def local_to_world_coordinates_numpy(frame, rst):
     """Convert local coordinates to global (world) coordinates.
 
     Parameters
     ----------
-    frame : [point, vector, vector] | :class:`compas.geometry.Frame`
+    frame : [point, vector, vector]
         The local coordinate system.
     rst : array-like[[float, float, float] | :class:`compas.geometry.Point`]
         The coordinates of the points wrt the local coordinate system.
 
     Returns
     -------
     (N, 3) ndarray
@@ -228,15 +227,15 @@
 
 
 def homogenize_and_flatten_frames_numpy(frames):
     """Homogenize a list of frames and flatten the 3D list into a 2D list using numpy.
 
     Parameters
     ----------
-    frames : array_like[[point, vector, vector] | :class:`compas.geometry.Frame`]
+    frames : array_like[[point, vector, vector]]
         The input frames.
 
     Returns
     -------
     (N x 3, 4) ndarray
         An array of points and vectors.
 
@@ -266,15 +265,15 @@
     Returns
     -------
     (N / 3, 3, 3) ndarray
         The frames.
 
     Examples
     --------
-    >>> points_and_vectors = [(1., 1., 1., 1.), (0., 1., 0., 0.), (1., 0., 0., 0.)]
+    >>> points_and_vectors = [(1.0, 1.0, 1.0, 1.0), (0.0, 1.0, 0.0, 0.0), (1.0, 0.0, 0.0, 0.0)]
     >>> res = dehomogenize_and_unflatten_frames_numpy(points_and_vectors)
     >>> np.allclose(res, [[1.0, 1.0, 1.0], [0.0, 1.0, 0.0], [1.0, 0.0, 0.0]])
     True
 
     """
     frames = dehomogenize_numpy(points_and_vectors)
     return frames.reshape((int(frames.shape[0] / 3.0), 3, 3))
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/bbox.py` & `compas-2.1.1/src/compas/geometry/bbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from itertools import islice
+
 from compas.plugins import pluggable
 
 
 def bounding_box(points):
     """Computes the axis-aligned minimum bounding box of a list of points.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/bbox_numpy.py` & `compas-2.1.1/src/compas/geometry/bbox_numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from numpy import array
-from numpy import asarray
-from numpy import argmax
-from numpy import argmin
 from numpy import amax
 from numpy import amin
+from numpy import argmax
+from numpy import argmin
+from numpy import array
+from numpy import asarray
 from numpy import dot
 from numpy import sum
-from numpy import zeros
 from numpy import vstack
-
+from numpy import zeros
 from scipy.spatial import ConvexHull
 
-from compas.tolerance import TOL
-
-from compas.geometry import pca_numpy
+from compas.geometry import length_vector
 from compas.geometry import local_axes
-from compas.geometry import world_to_local_coordinates_numpy
 from compas.geometry import local_to_world_coordinates_numpy
+from compas.geometry import pca_numpy
+from compas.geometry import world_to_local_coordinates_numpy
+from compas.tolerance import TOL
 
 from .bbox import bounding_box
 
 
 def oriented_bounding_box_numpy(points, tol=None):
     r"""Compute the oriented minimum bounding box of a set of points in 3D space.
 
@@ -71,15 +70,15 @@
     Compute the volume of the oriented bounding box.
 
     >>> from compas.geometry import length_vector, subtract_vectors, close
     >>> bbox = oriented_bounding_box_numpy(points)
     >>> a = length_vector(subtract_vectors(bbox[1], bbox[0]))
     >>> b = length_vector(subtract_vectors(bbox[3], bbox[0]))
     >>> c = length_vector(subtract_vectors(bbox[4], bbox[0]))
-    >>> close(a * b * c, 30.)
+    >>> close(a * b * c, 30.0)
     True
 
     """
     points = asarray(points)
     n, dim = points.shape
 
     if dim != 3:
@@ -196,14 +195,16 @@
     hull = ConvexHull(points)
     xyz = points[hull.vertices]
     boxes = []
 
     for simplex in hull.simplices:
         a, b, c = points[simplex]
         uvw = local_axes(a, b, c)
+        if not length_vector(uvw[0]) or not length_vector(uvw[1]):
+            continue
         frame = [a, uvw[0], uvw[1]]
         rst = world_to_local_coordinates_numpy(frame, xyz)
         rmin, smin, tmin = amin(rst, axis=0)
         rmax, smax, tmax = amax(rst, axis=0)
         dr = rmax - rmin
         ds = smax - smin
         dt = tmax - tmin
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/bestfit.py` & `compas-2.1.1/src/compas/geometry/bestfit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.geometry import subtract_vectors
-from compas.geometry import normalize_vector
 from compas.geometry import centroid_points
+from compas.geometry import normalize_vector
+from compas.geometry import subtract_vectors
 
 
 def bestfit_plane(points):
     """Fit a plane to a list of (more than three) points.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/bestfit_numpy.py` & `compas-2.1.1/src/compas/geometry/bestfit_numpy.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from numpy import asarray
 from numpy import sqrt
 from numpy import zeros
 from numpy.linalg import lstsq
 from scipy.optimize import leastsq
 
+from compas.geometry import local_to_world_coordinates_numpy
 from compas.geometry import pca_numpy
 from compas.geometry import world_to_local_coordinates_numpy
-from compas.geometry import local_to_world_coordinates_numpy
 
 
 def bestfit_line_numpy(points):
     """Fit a line through a set of points.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/booleans.py` & `compas-2.1.1/src/compas/geometry/booleans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.plugins import pluggable
 from compas.plugins import PluginNotInstalledError
+from compas.plugins import pluggable
 
 
 @pluggable(category="booleans")
 def boolean_union_mesh_mesh(A, B):
     """Compute the boolean union of two triangle meshes.
 
     Parameters
@@ -33,37 +33,35 @@
     This means that it doesn't provide an implementation, but receives an implementation from a corresponding "plugin".
     To use the plugin implementation, you have to install it in the same environment as COMPAS.
     One such plugin is available in ``compas_cgal``.
 
     Examples
     --------
     >>> from compas.geometry import Box, Sphere
-    >>> from compas.geometry import boolean_union_mesh_mesh     # doctest: +SKIP
-    >>> from compas.geometry import trimesh_remesh              # doctest: +SKIP
+    >>> from compas.geometry import boolean_union_mesh_mesh  # doctest: +SKIP
+    >>> from compas.geometry import trimesh_remesh  # doctest: +SKIP
     >>> from compas.datastructures import Mesh
 
     >>> box = Box.from_width_height_depth(2, 2, 2)
     >>> box = Mesh.from_shape(box)
     >>> box.quads_to_triangles()
 
     >>> sphere = Sphere([1, 1, 1], 1)
     >>> sphere = Mesh.from_shape(sphere, u=30, v=30)
     >>> sphere.quads_to_triangles()
 
     >>> A = box.to_vertices_and_faces()
     >>> B = sphere.to_vertices_and_faces()
-    >>> B = trimesh_remesh(B, 0.3, 10)                          # doctest: +SKIP
+    >>> B = trimesh_remesh(B, 0.3, 10)  # doctest: +SKIP
 
-    >>> V, F = boolean_union_mesh_mesh(A, B)                    # doctest: +SKIP
-    >>> union = Mesh.from_vertices_and_faces(V, F)              # doctest: +SKIP
+    >>> V, F = boolean_union_mesh_mesh(A, B)  # doctest: +SKIP
+    >>> union = Mesh.from_vertices_and_faces(V, F)  # doctest: +SKIP
 
     """
-    raise PluginNotInstalledError(
-        "No plugin was found for the boolean_union_mesh_mesh pluggable. A plugin is available in compas_cgal..."
-    )
+    raise PluginNotInstalledError("No plugin was found for the boolean_union_mesh_mesh pluggable. A plugin is available in compas_cgal...")
 
 
 boolean_union_mesh_mesh.__pluggable__ = True
 
 
 @pluggable(category="booleans")
 def boolean_difference_mesh_mesh(A, B):
@@ -90,17 +88,15 @@
     -----
     This function is a "pluggable".
     This means that it doesn't provide an implementation, but receives an implementation from a corresponding "plugin".
     To use the plugin implementation, you have to install it in the same environment as COMPAS.
     One such plugin is available in ``compas_cgal``.
 
     """
-    raise PluginNotInstalledError(
-        "No plugin was found for the boolean_difference_mesh_mesh pluggable. A plugin is available in compas_cgal..."
-    )
+    raise PluginNotInstalledError("No plugin was found for the boolean_difference_mesh_mesh pluggable. A plugin is available in compas_cgal...")
 
 
 boolean_difference_mesh_mesh.__pluggable__ = True
 
 
 @pluggable(category="booleans")
 def boolean_intersection_mesh_mesh(A, B):
@@ -127,17 +123,15 @@
     -----
     This function is a "pluggable".
     This means that it doesn't provide an implementation, but receives an implementation from a corresponding "plugin".
     To use the plugin implementation, you have to install it in the same environment as COMPAS.
     One such plugin is available in ``compas_cgal``.
 
     """
-    raise PluginNotInstalledError(
-        "No plugin was found for the boolean_intersection_mesh_mesh pluggable. A plugin is available in compas_cgal..."
-    )
+    raise PluginNotInstalledError("No plugin was found for the boolean_intersection_mesh_mesh pluggable. A plugin is available in compas_cgal...")
 
 
 boolean_intersection_mesh_mesh.__pluggable__ = True
 
 
 @pluggable(category="booleans")
 def boolean_union_polygon_polygon(A, B):
@@ -170,17 +164,15 @@
     -----
     This function is a "pluggable".
     This means that it doesn't provide an implementation, but receives an implementation from a corresponding "plugin".
     To use the plugin implementation, you have to install it in the same environment as COMPAS.
     One such plugin is available through ``shapely``.
 
     """
-    raise PluginNotInstalledError(
-        "No plugin was found for the boolean_union_polygon_polygon pluggable. Installing Shapely should solve the problem."
-    )
+    raise PluginNotInstalledError("No plugin was found for the boolean_union_polygon_polygon pluggable. Installing Shapely should solve the problem.")
 
 
 boolean_union_polygon_polygon.__pluggable__ = True
 
 
 @pluggable(category="booleans")
 def boolean_difference_polygon_polygon(A, B):
@@ -213,17 +205,15 @@
     -----
     This function is a "pluggable".
     This means that it doesn't provide an implementation, but receives an implementation from a corresponding "plugin".
     To use the plugin implementation, you have to install it in the same environment as COMPAS.
     One such plugin is available through ``shapely``.
 
     """
-    raise PluginNotInstalledError(
-        "No plugin was found for the boolean_difference_polygon_polygon pluggable. Installing Shapely should solve the problem."
-    )
+    raise PluginNotInstalledError("No plugin was found for the boolean_difference_polygon_polygon pluggable. Installing Shapely should solve the problem.")
 
 
 boolean_difference_polygon_polygon.__pluggable__ = True
 
 
 @pluggable(category="booleans")
 def boolean_symmetric_difference_polygon_polygon(A, B):
@@ -256,17 +246,15 @@
     -----
     This function is a "pluggable".
     This means that it doesn't provide an implementation, but receives an implementation from a corresponding "plugin".
     To use the plugin implementation, you have to install it in the same environment as COMPAS.
     One such plugin is available through ``shapely``.
 
     """
-    raise PluginNotInstalledError(
-        "No plugin was found for the boolean_symmetric_difference_polygon_polygon pluggable. Installing Shapely should solve the problem."
-    )
+    raise PluginNotInstalledError("No plugin was found for the boolean_symmetric_difference_polygon_polygon pluggable. Installing Shapely should solve the problem.")
 
 
 boolean_symmetric_difference_polygon_polygon.__pluggable__ = True
 
 
 @pluggable(category="booleans")
 def boolean_intersection_polygon_polygon(A, B):
@@ -299,13 +287,11 @@
     -----
     This function is a "pluggable".
     This means that it doesn't provide an implementation, but receives an implementation from a corresponding "plugin".
     To use the plugin implementation, you have to install it in the same environment as COMPAS.
     One such plugin is available through ``shapely``.
 
     """
-    raise PluginNotInstalledError(
-        "No plugin was found for the boolean_intersection_polygon_polygon pluggable. Installing Shapely should solve the problem."
-    )
+    raise PluginNotInstalledError("No plugin was found for the boolean_intersection_polygon_polygon pluggable. Installing Shapely should solve the problem.")
 
 
 boolean_intersection_polygon_polygon.__pluggable__ = True
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/booleans_shapely.py` & `compas-2.1.1/src/compas/geometry/booleans_shapely.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from compas.plugins import plugin
 from shapely.geometry import Polygon
 
+from compas.plugins import plugin
+
 
 @plugin(category="booleans", requires=["shapely"])
 def boolean_union_polygon_polygon(A, B):
     """Compute the boolean union of two polygons.
 
     For this operation, the polygons are assumed to lie in the XY plane.
     Therefore, the Z components of the points defining the polygons are simply ignored.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/brep/__init__.py` & `compas-2.1.1/src/compas/geometry/brep/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,19 @@
 
 @pluggable(category="factories")
 def from_pipe(*args, **kwargs):
     raise PluginNotInstalledError
 
 
 @pluggable(category="factories")
+def from_plane(*args, **kwargs):
+    raise PluginNotInstalledError
+
+
+@pluggable(category="factories")
 def from_planes(*args, **kwargs):
     raise PluginNotInstalledError
 
 
 @pluggable(category="factories")
 def from_polygons(*args, **kwargs):
     raise PluginNotInstalledError
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/brep/brep.py` & `compas-2.1.1/src/compas/geometry/brep/brep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from compas.geometry import Geometry
 
-from . import new_brep
-from . import from_brepfaces
+from . import from_boolean_difference
+from . import from_boolean_intersection
+from . import from_boolean_union
 from . import from_box
-from . import from_cylinder
-from . import from_sphere
-from . import from_mesh
+from . import from_brepfaces
 from . import from_cone
-from . import from_torus
+from . import from_curves
+from . import from_cylinder
 from . import from_extrusion
 from . import from_iges
 from . import from_loft
-from . import from_boolean_difference
-from . import from_boolean_intersection
-from . import from_boolean_union
-from . import from_curves
+from . import from_mesh
+from . import from_native
 from . import from_pipe
+from . import from_plane
 from . import from_planes
 from . import from_polygons
+from . import from_sphere
 from . import from_step
 from . import from_sweep
-from . import from_native
-
-
-LINEAR_DEFLECTION = 1e-3
+from . import from_torus
+from . import new_brep
 
 
 class BrepType(object):
     """Possible types of a Brep
 
     Attributes
     ----------
@@ -486,14 +484,34 @@
         -------
         :class:`compas.geometry.Brep`
 
         """
         return from_pipe(curve, radius, thickness=thickness)
 
     @classmethod
+    def from_plane(cls, plane, domain_u=(-1, +1), domain_v=(-1, +1)):
+        """Construct a Brep from one plane and its u and v domains.
+
+        Parameters
+        ----------
+        plane : :class:`~compas.geometry.Plane`
+            A plane.
+        domain_u : tuple[float, float], optional
+            The surface domain in the u direction.
+        domain_v : tuple[float, float], optional
+            The surface domain in the v direction.
+
+        Returns
+        -------
+        :class:`compas.geometry.Brep`
+
+        """
+        return from_plane(plane, domain_u=domain_u, domain_v=domain_v)
+
+    @classmethod
     def from_planes(cls, planes):
         """Construct a Brep from a set of planes.
 
         Parameters
         ----------
         planes : list[:class:`~compas.geometry.Plane`]
             A list of planes.
@@ -764,15 +782,15 @@
         Returns
         -------
         None
 
         """
         raise NotImplementedError
 
-    def to_tesselation(self, linear_deflection=LINEAR_DEFLECTION):
+    def to_tesselation(self, linear_deflection=None):
         """Create a tesselation of the shape for visualisation.
 
         Parameters
         ----------
         linear_deflection : float, optional
             Allowable deviation between curved geometry and mesh discretisation.
 
@@ -1089,15 +1107,15 @@
         Returns
         -------
         list[:class:`compas.geometry.Brep`]
 
         """
         raise NotImplementedError
 
-    def overlap(self, other, deflection=LINEAR_DEFLECTION, tolerance=0.0):
+    def overlap(self, other, deflection=None, tolerance=0.0):
         """Compute the overlap between this BRep and another.
 
         Parameters
         ----------
         other : :class:`compas.geometry.Brep`
             The other Brep.
         deflection : float, optional
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/brep/edge.py` & `compas-2.1.1/src/compas/geometry/brep/edge.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/geometry/brep/face.py` & `compas-2.1.1/src/compas/geometry/brep/face.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from compas.data import Data
-
 from compas.geometry import Polygon
 
 
 class SurfaceType(object):
     """Enumaration of surface types."""
 
     PLANE = 0
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/brep/loop.py` & `compas-2.1.1/src/compas/geometry/brep/loop.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/geometry/brep/trim.py` & `compas-2.1.1/src/compas/geometry/brep/trim.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/geometry/brep/vertex.py` & `compas-2.1.1/src/compas/geometry/brep/vertex.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/geometry/contours.py` & `compas-2.1.1/src/compas/geometry/contours.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from compas.plugins import pluggable
 from compas.plugins import PluginNotInstalledError
+from compas.plugins import pluggable
 
 
 @pluggable(category="contours")
 def scalarfield_contours(xy, s, levels=50, density=100):
     r"""Compute the contour lines of a scalarfield.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/arc.py` & `compas-2.1.1/src/compas/geometry/curves/arc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from math import pi, cos, sin
+from math import cos
+from math import pi
+from math import sin
 
-from compas.geometry import close
+from compas.geometry import Circle
+from compas.geometry import Frame
 from compas.geometry import Point
 from compas.geometry import Vector
-from compas.geometry import Frame
-from compas.geometry import Circle
+from compas.tolerance import TOL
+
 from .curve import Curve
 
 PI2 = 2.0 * pi
 
 
 class Arc(Curve):
     """An arc is a segment of a circle, and is defined by a coordinate system, radius, and start and end angles.
@@ -93,27 +96,27 @@
     >>> frame = Frame([0.0, 1.0, 0.0], [0.0, 0.0, 1.0], [1.0, 0.0, 0.0])
     >>> arc = Arc(radius=1.0, start_angle=pi, end_angle=pi * 1.5, frame=frame)
     >>> arc.length == 1.0 * pi * 0.5
     True
 
     Visualize the arc using the viewer.
 
-    >>> from compas_view2.app import App   # doctest: +SKIP
-    >>> viewer = App()                     # doctest: +SKIP
-    >>> viewer.add(arc.to_polyline(n=20))  # doctest: +SKIP
-    >>> viewer.add(arc.frame)              # doctest: +SKIP
-    >>> viewer.run()                       # doctest: +SKIP
+    >>> from compas_viewer import Viewer  # doctest: +SKIP
+    >>> viewer = Viewer()  # doctest: +SKIP
+    >>> viewer.scene.add(arc.to_polyline(n=20))  # doctest: +SKIP
+    >>> viewer.scene.add(arc.frame)  # doctest: +SKIP
+    >>> viewer.show()  # doctest: +SKIP
 
     Visualize only part of the arc.
 
-    >>> from compas_view2.app import App                        # doctest: +SKIP
-    >>> viewer = App()                                          # doctest: +SKIP
-    >>> viewer.add(arc.to_polyline(n=20, domain=(0.25, 0.75)))  # doctest: +SKIP
-    >>> viewer.add(arc.frame)                                   # doctest: +SKIP
-    >>> viewer.run()                                            # doctest: +SKIP
+    >>> from compas_viewer import Viewer  # doctest: +SKIP
+    >>> viewer = Viewer()  # doctest: +SKIP
+    >>> viewer.scene.add(arc.to_polyline(n=20, domain=(0.25, 0.75)))  # doctest: +SKIP
+    >>> viewer.scene.add(arc.frame)  # doctest: +SKIP
+    >>> viewer.show()  # doctest: +SKIP
 
     """
 
     # overwriting the __new__ method is necessary
     # to avoid triggering the plugin mechanism of the base curve class
     def __new__(cls, *args, **kwargs):
         curve = object.__new__(cls)
@@ -167,20 +170,15 @@
             self.start_angle,
             self.end_angle,
             self.frame,
         )
 
     def __eq__(self, other):
         try:
-            return (
-                self.radius == other.radius
-                and self.start_angle == other.start
-                and self.end_angle == other.end
-                and self.frame == other.frame
-            )
+            return self.radius == other.radius and self.start_angle == other.start and self.end_angle == other.end and self.frame == other.frame
         except Exception:
             return False
 
     # =============================================================================
     # Properties
     # =============================================================================
 
@@ -242,15 +240,15 @@
 
     @property
     def circumference(self):
         return self.diameter * pi
 
     @property
     def is_circle(self):
-        return close(abs(abs(self.angle) - PI2), 0.0)
+        return TOL.is_close(abs(self.angle), PI2)
 
     @property
     def is_closed(self):
         return False
 
     @property
     def is_periodic(self):
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/bezier.py` & `compas-2.1.1/src/compas/geometry/curves/bezier.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import factorial
 
-from compas.geometry import Vector
-from compas.geometry import Point
 from compas.geometry import Frame
+from compas.geometry import Point
+from compas.geometry import Vector
 
 from .curve import Curve
 
 
 def binomial_coefficient(n, k):
     """Returns the binomial coefficient of the :math:`x^k` term in the
     polynomial expansion of the binomial power :math:`(1 + x)^n`.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/circle.py` & `compas-2.1.1/src/compas/geometry/curves/circle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from math import pi, cos, sin
+from math import cos
+from math import pi
+from math import sin
 
-from compas.geometry import Point
-from compas.geometry import Vector
 from compas.geometry import Frame
 from compas.geometry import Plane
+from compas.geometry import Point
+from compas.geometry import Vector
+
 from .conic import Conic
 
 PI2 = 2 * pi
 
 
 class Circle(Conic):
     """A circle is a curve defined by a coordinate system and a radius.
@@ -74,20 +77,20 @@
     >>> line = Line([0, 0, 0], [1, 1, 1])
     >>> plane = Plane(line.end, line.direction)
     >>> circle = Circle.from_plane_and_radius(plane, 5)
     >>> circle = Circle(radius=5, frame=Frame.from_plane(plane))
 
     Visualise the line, circle, and frame of the circle with the COMPAS viewer.
 
-    >>> from compas_view2.app import App  # doctest: +SKIP
-    >>> viewer = App()                    # doctest: +SKIP
-    >>> viewer.add(line)                  # doctest: +SKIP
-    >>> viewer.add(circle)                # doctest: +SKIP
-    >>> viewer.add(circle.frame)          # doctest: +SKIP
-    >>> viewer.run()                      # doctest: +SKIP
+    >>> from compas_viewer import Viewer  # doctest: +SKIP
+    >>> viewer = Viewer()  # doctest: +SKIP
+    >>> viewer.scene.add(line)  # doctest: +SKIP
+    >>> viewer.scene.add(circle)  # doctest: +SKIP
+    >>> viewer.scene.add(circle.frame)  # doctest: +SKIP
+    >>> viewer.show()  # doctest: +SKIP
 
     """
 
     DATASCHEMA = {
         "type": "object",
         "properties": {
             "radius": {"type": "number", "minimum": 0},
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/curve.py` & `compas-2.1.1/src/compas/geometry/curves/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.plugins import pluggable
+from compas.geometry import Frame
 from compas.geometry import Geometry
-from compas.geometry import Transformation
 from compas.geometry import Plane
-from compas.geometry import Frame
-from compas.utilities import linspace
+from compas.geometry import Transformation
+from compas.itertools import linspace
+from compas.plugins import pluggable
 
 
 @pluggable(category="factories")
 def new_curve(cls, *args, **kwargs):
     curve = object.__new__(cls)
     curve.__init__(*args, **kwargs)
     return curve
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/ellipse.py` & `compas-2.1.1/src/compas/geometry/curves/ellipse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from math import sqrt, pi, cos, sin
+from math import cos
+from math import pi
+from math import sin
+from math import sqrt
 
+from compas.geometry import Frame
 from compas.geometry import Point
 from compas.geometry import Vector
-from compas.geometry import Frame
+
 from .conic import Conic
 from .line import Line
 
 PI2 = 2 * pi
 
 
 class Ellipse(Conic):
@@ -95,20 +99,20 @@
     >>> line = Line([0, 0, 0], [1, 1, 1])
     >>> plane = Plane(line.end, line.direction)
     >>> ellipse = Ellipse.from_plane_major_minor(plane, 3, 2)
     >>> ellipse = Ellipse(major=3, minor=2, frame=Frame.from_plane(plane))
 
     Visualise the line, ellipse, and frame of the ellipse with the COMPAS viewer.
 
-    >>> from compas_view2.app import App  # doctest: +SKIP
-    >>> viewer = App()                    # doctest: +SKIP
-    >>> viewer.add(line)                  # doctest: +SKIP
-    >>> viewer.add(ellipse)               # doctest: +SKIP
-    >>> viewer.add(ellipse.frame)         # doctest: +SKIP
-    >>> viewer.run()                      # doctest: +SKIP
+    >>> from compas_viewer import Viewer  # doctest: +SKIP
+    >>> viewer = Viewer()  # doctest: +SKIP
+    >>> viewer.scene.add(line)  # doctest: +SKIP
+    >>> viewer.scene.add(ellipse)  # doctest: +SKIP
+    >>> viewer.scene.add(ellipse.frame)  # doctest: +SKIP
+    >>> viewer.show()  # doctest: +SKIP
 
     """
 
     DATASCHEMA = {
         "type": "object",
         "properties": {
             "major": {"type": "number", "minimum": 0},
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/hyperbola.py` & `compas-2.1.1/src/compas/geometry/curves/hyperbola.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from math import cos, sin, sqrt
+from math import cos
 from math import pi
+from math import sin
+from math import sqrt
 
-from compas.geometry import Point
 from compas.geometry import Frame
+from compas.geometry import Point
+
 from .conic import Conic
 
 PI2 = 2 * pi
 
 
 class Hyperbola(Conic):
     r"""
@@ -99,20 +102,20 @@
     >>> from compas.geometry import Line, Frame, Hyperbola
     >>> line = Line([0, 0, 0], [1, 1, 1])
     >>> plane = Plane(line.end, line.direction)
     >>> hyperbola = Hyperbola(major=3, minor=2, frame=Frame.from_plane(plane))
 
     Visualise the line, hyperbola, and frame of the hyperbola with the COMPAS viewer.
 
-    >>> from compas_view2.app import App  # doctest: +SKIP
-    >>> viewer = App()                    # doctest: +SKIP
-    >>> viewer.add(line)                  # doctest: +SKIP
-    >>> viewer.add(hyperbola)               # doctest: +SKIP
-    >>> viewer.add(hyperbola.frame)         # doctest: +SKIP
-    >>> viewer.run()                      # doctest: +SKIP
+    >>> from compas_viewer import Viewer  # doctest: +SKIP
+    >>> viewer = Viewer()                    # doctest: +SKIP
+    >>> viewer.scene.add(line)                  # doctest: +SKIP
+    >>> viewer.scene.add(hyperbola)               # doctest: +SKIP
+    >>> viewer.scene.add(hyperbola.frame)         # doctest: +SKIP
+    >>> viewer.show()                      # doctest: +SKIP
 
     """
 
     DATASCHEMA = {
         "type": "object",
         "properties": {
             "major": {"type": "number", "minimum": 0},
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/line.py` & `compas-2.1.1/src/compas/geometry/shapes/shape.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,350 +1,300 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.geometry import add_vectors
-from compas.geometry import Point
-from compas.geometry import Vector
 from compas.geometry import Frame
-from .curve import Curve
+from compas.geometry import Geometry
+from compas.geometry import Rotation
+from compas.geometry import Transformation
+
+
+class Shape(Geometry):
+    """Base class for geometric shapes.
 
+    Shapes are parametrically defined with repsect to a local coordinate system.
+    The local coordinate system of a shape is defined by a frame.
+    The default frame is the word coordinate system, i.e. the origin and the axes of the world XY plane.
 
-class Line(Curve):
-    """A line is a curve defined by two points.
+    Shapes are finite, closed objects, with a boundary that separates the interior from the exterior.
+    They have a well-defined surface area and volume.
 
-    The first point is the start point of the line.
-    The second point is the end point of the line.
-    The vector between the two points defines the direction of the line.
-    The length of the vector is the length of the line.
-    The direction vector is the unit vector of the vector between start and end.
-    The parameterisation of the line is such that the start point corresponds to ``t = 0`` and the end point to ``t = 1``.
+    An explicit representation of a shape is obtained by discretising its boundary into a set of vertices and faces with a chosen resolution (:meth:`to_vertices_and_faces`).
+    The vertices and faces can be used to construct a :class:`compas.geometry.Polyhedron` object (:meth:`to_polyhedron`).
+    A shape can also be converted to a :class:`compas.geometry.Brep` object (:meth:`to_brep`).
 
-    The coordinate system of a line is always the world coordinate system (WCS).
-    Transformation of a line is performed by transforming the start and end point.
+    Breps and polyhedrons support boolean operations.
 
     Parameters
     ----------
-    start : [float, float, float] | :class:`compas.geometry.Point`
-        The first point.
-    end : [float, float, float] | :class:`compas.geometry.Point`
-        The second point.
-    name : str, optional
-        The name of the line.
+    frame : :class:`compas.geometry.Frame`, optional
+        The local coordinate system of the shape.
+        Default is ``None``, in which case the world coordinate system is used.
 
     Attributes
     ----------
-    start : :class:`compas.geometry.Point`
-        The start point of the line.
-    end : :class:`compas.geometry.Point`
-        The end point of the line.
-    vector : :class:`compas.geometry.Vector`, read-only
-        A vector pointing from start to end.
-    length : float, read-only
-        The length of the vector from start to end.
-    direction : :class:`compas.geometry.Vector`, read-only
-        A unit vector parallel to the line vector.
-    midpoint : :class:`compas.geometry.Point`, read-only
-        The midpoint between start and end.
-    frame : :class:`compas.geometry.Frame`, read-only
-        The frame of the line.
-        This is alsways the world XY frame.
+    area : float, read-only
+        The surface area of the shape.
+    frame : :class:`compas.geometry.Frame`
+        The local coordinate system of the shape.
     transformation : :class:`compas.geometry.Transformation`, read-only
-        This is always the identity transformation.
-
-    Examples
-    --------
-    >>> line = Line([0, 0, 0], [1, 1, 1])
-    >>> line
-    Line(Point(0.000, 0.000, 0.000), Point(1.000, 1.000, 1.000))
-    >>> line.start
-    Point(0.000, 0.000, 0.000)
-    >>> line.midpoint
-    Point(0.500, 0.500, 0.500)
-    >>> line.length == math.sqrt(line.dx **2 + line.dy **2 + line.dz **2)
-    True
-    >>> line.direction
-    Vector(0.577, 0.577, 0.577)
+        The transformation of the shape to global coordinates.
+    volume : float, read-only
+        The volume of the shape.
 
     """
 
-    # overwriting the __new__ method is necessary
-    # to avoid triggering the plugin mechanism of the base curve class
-    def __new__(cls, *args, **kwargs):
-        curve = object.__new__(cls)
-        curve.__init__(*args, **kwargs)
-        return curve
-
-    DATASCHEMA = {
-        "type": "object",
-        "properties": {
-            "start": Point.DATASCHEMA,
-            "end": Point.DATASCHEMA,
-        },
-        "required": ["start", "end"],
-    }
-
-    @property
-    def __data__(self):
-        return {"start": self.start.__data__, "end": self.end.__data__}
-
-    def __init__(self, start, end, name=None):
-        super(Line, self).__init__(name=name)
-        self._point = None
-        self._vector = None
-        self._direction = None
-        self.start = start
-        self.end = end
-
-    def __repr__(self):
-        return "{0}({1!r}, {2!r})".format(
-            type(self).__name__,
-            self.start,
-            self.end,
-        )
-
-    def __getitem__(self, key):
-        if key == 0:
-            return self.start
-        if key == 1:
-            return self.end
-        raise KeyError
-
-    def __setitem__(self, key, value):
-        if key == 0:
-            self.start = value
-        elif key == 1:
-            self.end = value
-        else:
-            raise KeyError
-
-    def __iter__(self):
-        return iter([self.start, self.end])
-
-    def __len__(self):
-        return 2
-
-    def __eq__(self, other):
-        try:
-            return self.start == other[0] and self.end == other[1]
-        except Exception:
-            return False
-
-    # ==========================================================================
-    # properties
-    # ==========================================================================
+    def __init__(self, frame=None, name=None):
+        super(Shape, self).__init__(name=name)
+        self._frame = None
+        self._transformation = None
+        self.frame = frame
+
+    # =============================================================================
+    # Data
+    # =============================================================================
+
+    # =============================================================================
+    # Properties
+    # =============================================================================
 
     @property
     def frame(self):
-        return Frame.worldXY()
+        if not self._frame:
+            self._frame = Frame.worldXY()
+        return self._frame
 
     @frame.setter
     def frame(self, frame):
-        raise AttributeError("Setting the coordinate frame of a line is not supported.")
+        if not frame:
+            self._frame = None
+        else:
+            self._frame = Frame(frame[0], frame[1], frame[2])
+        self._transformation = None
 
     @property
-    def point(self):
-        if not self._point:
-            raise ValueError("The line has no base point.")
-        return self._point
-
-    @point.setter
-    def point(self, point):
-        self._point = Point(*point)
+    def transformation(self):
+        if not self._transformation:
+            self._transformation = Transformation.from_frame_to_frame(Frame.worldXY(), self.frame)
+        return self._transformation
 
     @property
-    def vector(self):
-        if not self._vector:
-            raise ValueError("The line has no direction vector.")
-        return self._vector
-
-    @vector.setter
-    def vector(self, vector):
-        self._vector = Vector(*vector)
-        self._direction = None
+    def area(self):
+        raise NotImplementedError
 
     @property
-    def length(self):
-        return self.vector.length
+    def volume(self):
+        raise NotImplementedError
 
-    @property
-    def direction(self):
-        if not self._direction:
-            self._direction = self.vector.unitized()
-        return self._direction
+    # =============================================================================
+    # Constructors
+    # =============================================================================
 
-    @property
-    def start(self):
-        return self.point
+    # =============================================================================
+    # Conversions
+    # =============================================================================
 
-    @start.setter
-    def start(self, point):
-        self.point = point
+    def to_vertices_and_faces(self, **kwargs):
+        """Convert the shape to a list of vertices and faces.
 
-    @property
-    def end(self):
-        return self.start + self.vector
+        Returns
+        -------
+        list of list of float
+            The vertices of the shape.
+        list of list of int
+            The faces of the shape.
 
-    @end.setter
-    def end(self, point):
-        self._vector = Vector.from_start_end(self.start, point)
-        self._direction = None
+        """
+        raise NotImplementedError
 
-    @property
-    def midpoint(self):
-        return self.point_at(0.5)
+    def to_polyhedron(self, triangulated=True, u=16, v=None):
+        """Convert the shape to a polyhedron.
 
-    # ==========================================================================
-    # Constructors
-    # ==========================================================================
+        Parameters
+        ----------
+        triangulated : bool, optional
+            If True, triangulate the faces.
+        u : int, optional
+            Number of faces in the "u" direction.
+        v : int, optional
+            Number of faces in the "v" direction.
+            If no value is provided, and the shape has two parameter directions, the value of ``u`` will be used.
+
+        Returns
+        -------
+        :class:`compas.geometry.Polyhedron`
+            The polyhedron representation of the shape.
+
+        Notes
+        -----
+        Parameters ``u`` and ``v`` define the resolution of the discretisation of curved geometry.
+        If the geometry is not curved in a particular direction, the corresponding parameter will be ignored.
+        For example, a cylinder has a resolution in the "u" direction, but not in the "v" direction.
+        A sphere has a resolution in both the "u" and the "v" direction.
+        A box has no resolution in either direction.
+
+        """
+        from compas.geometry import Polyhedron
+
+        v = v or u
+
+        vertices, faces = self.to_vertices_and_faces(u=u, v=v)
 
-    @classmethod
-    def from_point_and_vector(cls, point, vector):
-        """Construct a line from a point and a vector.
+        if triangulated:
+            triangles = []
+            for face in faces:
+                if len(face) == 4:
+                    triangles.append(face[0:3])
+                    triangles.append([face[0], face[2], face[3]])
+                else:
+                    triangles.append(face)
+            faces = triangles
+
+        return Polyhedron(vertices, faces)
+
+    def to_brep(self):
+        """Convert the shape to a Brep.
+
+        Returns
+        -------
+        :class:`compas.geometry.Brep`
+            The Brep representation of the shape.
+
+        """
+        raise NotImplementedError
+
+    # =============================================================================
+    # Transformation
+    # =============================================================================
+
+    def transform(self, transformation):
+        """Transform the shape.
+
+        Transformations of a shape are performed by applying the transformation to the frame of the shape.
+        Transformations of the shape with respect to its local coordinate system are not supported.
+        For this reason, only (combinations of) translations and rotations are supported.
+        To scale a shape, use the :meth:`Shape.scale` method.
 
         Parameters
         ----------
-        point : :class:`compas.geometry.Point`
-            The start point of the line.
-        vector : :class:`compas.geometry.Vector`
-            The vector of the line.
+        transformation : :class:`Transformation`
+            The transformation used to transform the shape.
 
         Returns
         -------
-        :class:`Line`
-            The constructed line.
+        None
 
         See Also
         --------
-        :meth:`Line.from_point_direction_length`
-
-        Examples
-        --------
-        >>> from compas.geometry import Point, Vector
-        >>> line = Line.from_point_and_vector(Point(0, 0, 0), Vector(1, 1, 1))
-        >>> line
-        Line(Point(0.000, 0.000, 0.000), Point(1.000, 1.000, 1.000))
+        translate
+        rotate
+        scale
 
         """
-        return cls(point, add_vectors(point, vector))
+        self.frame.transform(transformation)
 
-    @classmethod
-    def from_point_direction_length(cls, point, direction, length):
-        """Construct a line from a point, a direction and a length.
+    def translate(self, vector):
+        """Translate the shape.
 
         Parameters
         ----------
-        point : :class:`compas.geometry.Point`
-            The start point of the line.
-        direction : :class:`compas.geometry.Vector`
-            The direction of the line.
-        length : float
-            The length of the line.
+        vector : :class:`Vector`
+            The translation vector.
 
         Returns
         -------
-        :class:`Line`
-            The constructed line.
+        None
 
         See Also
         --------
-        :meth:`Line.from_point_and_vector`
-
-        Examples
-        --------
-        >>> from compas.geometry import Point, Vector
-        >>> line = Line.from_point_direction_length(Point(0, 0, 0), Vector(1, 1, 1), 1)
-        >>> line
-        Line(Point(0.000, 0.000, 0.000), Point(0.577, 0.577, 0.577))
+        rotate
+        scale
+        transform
 
         """
-        direction = Vector(*direction)
-        direction.unitize()
-        return cls(point, add_vectors(point, direction * length))
-
-    # ==========================================================================
-    # Transformations
-    # ==========================================================================
+        self.frame.point += vector
 
-    def transform(self, T):
-        """Transform this line.
+    def rotate(self, angle, axis=None, point=None):
+        """Rotate the shape.
 
         Parameters
         ----------
-        T : :class:`compas.geometry.Transformation`
-            The transformation.
+        vector : :class:`Vector`
+            The translation vector.
 
         Returns
         -------
         None
 
-        Examples
+        See Also
         --------
-        >>> from math import radians
-        >>> from compas.geometry import Rotation
-        >>> line = Line([0.0, 0.0, 0.0], [1.0, 0.0, 0.0])
-        >>> R = Rotation.from_axis_and_angle([0.0, 0.0, 1.0], radians(90))
-        >>> line.transform(R)
-        >>> line.end
-        Point(0.000, 1.000, 0.000)
+        translate
+        scale
+        transform
 
         """
-        self.point.transform(T)
-        self.vector.transform(T)
+        axis = axis or [0, 0, 1]
+        point = point or [0, 0, 0]
+        matrix = Rotation.from_axis_and_angle(axis=axis, angle=angle, point=point)
+        self.transform(matrix)
 
-    # ==========================================================================
-    # Methods
-    # ==========================================================================
+    def scale(self, scale):
+        """Scale the shape.
 
-    def point_at(self, t):
-        """Construct a point at a specific location along the line.
+        Scale transformations are applied to the parameters of a shape rahter than to its frame.
+        Only uniform scaling is supported.
 
         Parameters
         ----------
-        t : float
-            The location along the line.
+        scale : float
+            The scaling factor.
 
         Returns
         -------
-        :class:`compas.geometry.Point`
-            The point at the specified location.
+        None
 
         See Also
         --------
-        :meth:`tangent_at`
-
-        Examples
-        --------
-        >>> line = Line([0, 0, 0], [1, 1, 1])
-        >>> line.point_at(0.5)
-        Point(0.500, 0.500, 0.500)
+        translate
+        rotate
+        transform
 
         """
-        point = self.point + self.vector * t
-        return point
+        raise NotImplementedError
+
+    # =============================================================================
+    # Methods
+    # =============================================================================
 
-    def closest_point(self, point, return_parameter=False):
-        """Compute the closest point on the line to a given point.
+    def contains_point(self, point):
+        """Verify if a point is inside the shape.
 
         Parameters
         ----------
         point : :class:`compas.geometry.Point`
-            The point.
-        return_parameter : bool, optional
-            Return the parameter of the closest point on the line.
-            Default is ``False``.
+            The point to test.
+
+        Returns
+        -------
+        bool
+            True if the point is inside the shape.
+            False otherwise.
+
+        """
+        raise NotImplementedError
+
+    def contains_points(self, points):
+        """Verify if a list of points are inside the shape.
+
+        Parameters
+        ----------
+        points : list of :class:`compas.geometry.Point`
+            The points to test.
 
         Returns
         -------
-        :class:`compas.geometry.Point`
-            The closest point on the line.
-        float
-            The parameter of the closest point on the line.
-            Only if ``return_parameter`` is ``True``.
+        list of bool
+            True if the point is inside the shape.
+            False otherwise.
 
         """
-        vector = point - self.start
-        t = vector.dot(self.vector) / self.length**2
-        closest = self.start + self.vector * t
-        if return_parameter:
-            return closest, t
-        return closest
+        return [self.contains_point(point) for point in points]
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/nurbs.py` & `compas-2.1.1/src/compas/geometry/curves/nurbs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import sqrt
 
-from compas.plugins import pluggable
-from compas.plugins import PluginNotInstalledError
-from compas.geometry import Point
 from compas.geometry import Frame
+from compas.geometry import Point
+from compas.plugins import PluginNotInstalledError
+from compas.plugins import pluggable
 
 from .curve import Curve
 
 
 @pluggable(category="factories")
 def new_nurbscurve(cls, *args, **kwargs):
     curve = object.__new__(NurbsCurve)
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/parabola.py` & `compas-2.1.1/src/compas/geometry/curves/parabola.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.geometry import Vector
-from compas.geometry import Point
 from compas.geometry import Frame
-from .line import Line
+from compas.geometry import Point
+from compas.geometry import Vector
+
 from .conic import Conic
+from .line import Line
 
 
 class Parabola(Conic):
     """
     A parabola is defined by a plane and a major and minor axis.
     The origin of the coordinate frame is the center of the parabola.
 
@@ -68,20 +69,20 @@
     >>> line = Line([0, 0, 0], [1, 1, 1])
     >>> plane = Plane(line.end, line.direction)
     >>> frame = Frame.from_plane(plane)
     >>> parabola = Parabola(focal=3, frame=frame)
 
     Visualize the parabola with the COMPAS viewer.
 
-    >>> from compas_view2.app import App  # doctest: +SKIP
-    >>> viewer = App()                    # doctest: +SKIP
-    >>> viewer.add(line)                  # doctest: +SKIP
-    >>> viewer.add(parabola)              # doctest: +SKIP
-    >>> viewer.add(parabola.frame)        # doctest: +SKIP
-    >>> viewer.run()                      # doctest: +SKIP
+    >>> from compas_viewer import Viewer  # doctest: +SKIP
+    >>> viewer = Viewer()  # doctest: +SKIP
+    >>> viewer.scene.add(line)  # doctest: +SKIP
+    >>> viewer.scene.add(parabola)  # doctest: +SKIP
+    >>> viewer.scene.add(parabola.frame)  # doctest: +SKIP
+    >>> viewer.show()  # doctest: +SKIP
 
     """
 
     DATASCHEMA = {
         "type": "object",
         "properties": {
             "focal": {"type": "number", "minimum": 0},
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/curves/polyline.py` & `compas-2.1.1/src/compas/geometry/curves/polyline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.utilities import pairwise
-
-from compas.geometry import allclose
-from compas.geometry import transform_points
-from compas.geometry import is_point_on_line, is_point_on_polyline
-from compas.geometry import Point
-from compas.geometry import Line
 from compas.geometry import Frame
+from compas.geometry import Line
+from compas.geometry import Point
+from compas.geometry import is_point_on_line
+from compas.geometry import is_point_on_polyline
+from compas.geometry import transform_points
+from compas.itertools import pairwise
+from compas.tolerance import TOL
+
 from .curve import Curve
 
 
 class Polyline(Curve):
     """A polyline is a curve defined by a sequence of points connected by line segments.
 
     A Polyline can be open or closed.
@@ -50,15 +51,15 @@
     is_selfintersecting : bool, read-only
         True if the polyline is self-intersecting.
     is_closed : bool, read-only
         True if the polyline is closed.
 
     Examples
     --------
-    >>> polyline = Polyline([[0,0,0], [1,0,0], [2,0,0], [3,0,0]])
+    >>> polyline = Polyline([[0, 0, 0], [1, 0, 0], [2, 0, 0], [3, 0, 0]])
     >>> polyline.length
     3.0
 
     >>> type(polyline.points[0]) == Point
     True
     >>> polyline.points[0].x
     0.0
@@ -113,15 +114,15 @@
 
     def __len__(self):
         return len(self.points)
 
     def __eq__(self, other):
         if not hasattr(other, "__iter__") or not hasattr(other, "__len__") or len(self) != len(other):
             return False
-        return allclose(self, other)
+        return TOL.is_allclose(self, other)
 
     # ==========================================================================
     # properties
     # ==========================================================================
 
     @property
     def frame(self):
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/frame.py` & `compas-2.1.1/src/compas/geometry/frame.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.tolerance import TOL
-
+from compas.geometry import Geometry
+from compas.geometry import Transformation
 from compas.geometry import argmax
 from compas.geometry import axis_angle_vector_from_matrix
 from compas.geometry import basis_vectors_from_matrix
 from compas.geometry import cross_vectors
 from compas.geometry import decompose_matrix
 from compas.geometry import euler_angles_from_matrix
 from compas.geometry import matrix_from_axis_angle_vector
 from compas.geometry import matrix_from_basis_vectors
 from compas.geometry import matrix_from_euler_angles
 from compas.geometry import matrix_from_quaternion
 from compas.geometry import quaternion_from_matrix
 from compas.geometry import subtract_vectors
+from compas.itertools import linspace
+from compas.tolerance import TOL
 
-from compas.geometry import Geometry
-from compas.geometry import Transformation
-
-from .vector import Vector
 from .point import Point
 from .quaternion import Quaternion
+from .vector import Vector
 
 
 class Frame(Geometry):
     """A frame is defined by a base point and two orthonormal base vectors.
 
     Parameters
     ----------
@@ -419,15 +418,15 @@
         Notes
         -----
         Since the transformation matrix follows the row-major order, the
         translational components must be at the list's indices 3, 7, 11.
 
         Examples
         --------
-        >>> l = [-1.0,  0.0,  0.0, 8110, 0.0,  0.0, -1.0, 7020, 0.0, -1.0,  0.0, 1810]
+        >>> l = [-1.0, 0.0, 0.0, 8110, 0.0, 0.0, -1.0, 7020, 0.0, -1.0, 0.0, 1810]
         >>> f = Frame.from_list(l)
 
         """
         if len(values) == 12:
             values.extend([0.0, 0.0, 0.0, 1.0])
         if len(values) != 16:
             raise ValueError("Expected 12 or 16 floats but got %d" % len(values))
@@ -454,15 +453,15 @@
         -------
         :class:`compas.geometry.Frame`
             The constructed frame.
 
         Examples
         --------
         >>> q1 = [0.945, -0.021, -0.125, 0.303]
-        >>> f = Frame.from_quaternion(q1, point=[1., 1., 1.])
+        >>> f = Frame.from_quaternion(q1, point=[1.0, 1.0, 1.0])
         >>> q2 = f.quaternion
         >>> allclose(q1, q2)
         True
 
         """
         R = matrix_from_quaternion(quaternion)
         xaxis, yaxis = basis_vectors_from_matrix(R)
@@ -518,16 +517,16 @@
         -------
         :class:`compas.geometry.Frame`
             The constructed frame.
 
         Examples
         --------
         >>> ea1 = 1.4, 0.5, 2.3
-        >>> f = Frame.from_euler_angles(ea1, static=True, axes='xyz')
-        >>> ea2 = f.euler_angles(static=True, axes='xyz')
+        >>> f = Frame.from_euler_angles(ea1, static=True, axes="xyz")
+        >>> ea2 = f.euler_angles(static=True, axes="xyz")
         >>> allclose(ea1, ea2)
         True
 
         """
         R = matrix_from_euler_angles(euler_angles, static, axes)
         xaxis, yaxis = basis_vectors_from_matrix(R)
         return cls(point, xaxis, yaxis)
@@ -547,15 +546,15 @@
         -------
         :class:`compas.geometry.Frame`
             The constructed frame.
 
         Examples
         --------
         >>> from compas.geometry import Plane
-        >>> plane = Plane([0,0,0], [0,0,1])
+        >>> plane = Plane([0, 0, 0], [0, 0, 1])
         >>> frame = Frame.from_plane(plane)
         >>> allclose(frame.normal, plane.normal)
         True
 
         """
         point, normal = plane
         # To construct a frame we need to find a vector v that is perpendicular
@@ -588,14 +587,73 @@
         """
         return Transformation.from_frame(self)
 
     # ==========================================================================
     # Methods
     # ==========================================================================
 
+    def interpolate_frame(self, other, t):
+        """Interpolates between two frames at a given parameter t in the range [0, 1]
+
+        Parameters
+        ----------
+        other : :class:`compas.geometry.Frame`
+        t : float
+            A parameter in the range [0-1].
+
+        Returns
+        -------
+        :class:`compas.geometry.Frame`
+            A list of the interpolated :class:`compas.geometry.Frame` instances.
+
+        Examples
+        --------
+        >>> frame1 = Frame(Point(0, 0, 0), Vector(1, 0, 0), Vector(0, 1, 0))
+        >>> frame2 = Frame(Point(1, 1, 1), Vector(0, 0, 1), Vector(0, 1, 0))
+        >>> start_frame = frame1.interpolate_frame(frame2, 0)
+        >>> allclose(start_frame.point, frame1.point) and allclose(start_frame.quaternion, frame1.quaternion)
+        True
+        """
+        quat1 = Quaternion.from_frame(self)
+        quat2 = Quaternion.from_frame(other)
+
+        # Interpolate origin
+        origin_interpolated = (self.point * (1.0 - t)) + other.point * t
+
+        rot_interpolated = quat1.slerp(quat2, t)
+
+        # Create a new frame with the interpolated position and orientation
+        interpolated_frame = Frame.from_quaternion(rot_interpolated, point=origin_interpolated)
+
+        return interpolated_frame
+
+    def interpolate_frames(self, other, steps):
+        """Generates a specified number of interpolated frames between two given frames
+
+        Parameters
+        ----------
+        other : :class:`compas.geometry.Frame`
+        steps : int
+            The number of interpolated frames to return.
+
+        Returns
+        -------
+        list of :class:`compas.geometry.Frame`
+
+        Examples
+        --------
+        >>> frame1 = Frame(Point(0, 0, 0), Vector(1, 0, 0), Vector(0, 1, 0))
+        >>> frame2 = Frame(Point(1, 1, 1), Vector(0, 0, 1), Vector(0, 1, 0))
+        >>> steps = 5
+        >>> frames = frame1.interpolate_frames(frame2, steps)
+        >>> assert len(frames) == steps
+        True
+        """
+        return [self.interpolate_frame(other, t) for t in linspace(0, 1, steps)]
+
     def euler_angles(self, static=True, axes="xyz"):
         """The Euler angles from the rotation given by the frame.
 
         Parameters
         ----------
         static : bool, optional
             If True the rotations are applied to a static frame.
@@ -607,16 +665,16 @@
         -------
         list[float]
             Three numbers that represent the angles of rotations about the defined axes.
 
         Examples
         --------
         >>> ea1 = 1.4, 0.5, 2.3
-        >>> f = Frame.from_euler_angles(ea1, static=True, axes='xyz')
-        >>> ea2 = f.euler_angles(static=True, axes='xyz')
+        >>> f = Frame.from_euler_angles(ea1, static=True, axes="xyz")
+        >>> ea2 = f.euler_angles(static=True, axes="xyz")
         >>> allclose(ea1, ea2)
         True
 
         """
         R = matrix_from_basis_vectors(self.xaxis, self.yaxis)
         return euler_angles_from_matrix(R, static, axes)
 
@@ -637,16 +695,16 @@
         -----
         If you pass a list of floats, it is assumed to represent a point.
 
         Examples
         --------
         >>> from compas.geometry import Point
         >>> frame = Frame([1, 1, 1], [0.68, 0.68, 0.27], [-0.67, 0.73, -0.15])
-        >>> pw = Point(2, 2, 2) # point in wcf
-        >>> pl = frame.to_local_coordinates(pw) # point in frame
+        >>> pw = Point(2, 2, 2)  # point in wcf
+        >>> pl = frame.to_local_coordinates(pw)  # point in frame
         >>> frame.to_world_coordinates(pl)
         Point(2.000, 2.000, 2.000)
 
         """
         T = Transformation.from_change_of_basis(Frame.worldXY(), self)
         if isinstance(obj_in_wcf, (list, tuple)):
             return Point(*obj_in_wcf).transformed(T)
@@ -669,16 +727,16 @@
         -----
         If you pass a list of floats, it is assumed to represent a point.
 
         Examples
         --------
         >>> from compas.geometry import Point
         >>> frame = Frame([1, 1, 1], [0.68, 0.68, 0.27], [-0.67, 0.73, -0.15])
-        >>> pl = Point(1.632, -0.090, 0.573) # point in frame
-        >>> pw = frame.to_world_coordinates(pl) # point in wcf
+        >>> pl = Point(1.632, -0.090, 0.573)  # point in frame
+        >>> pw = frame.to_world_coordinates(pl)  # point in wcf
         >>> frame.to_local_coordinates(pw)
         Point(1.632, -0.090, 0.573)
 
         """
         T = Transformation.from_change_of_basis(self, Frame.worldXY())
         if isinstance(obj_in_lcf, list):
             return Point(*obj_in_lcf).transformed(T)
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/geometry.py` & `compas-2.1.1/src/compas/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/geometry/hull.py` & `compas-2.1.1/src/compas/geometry/hull.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.geometry import cross_vectors
-from compas.geometry import subtract_vectors
-from compas.geometry import dot_vectors
 from compas.geometry import cross_vectors_xy
+from compas.geometry import dot_vectors
+from compas.geometry import subtract_vectors
 
 
 def convex_hull(points):
     """Construct convex hull for a set of points.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/hull_numpy.py` & `compas-2.1.1/src/compas/geometry/hull_numpy.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/geometry/icp_numpy.py` & `compas-2.1.1/src/compas/geometry/icp_numpy.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
-from numpy import asarray
 from numpy import argmin
+from numpy import asarray
 from numpy.linalg import det
-from scipy.spatial.distance import cdist
-from scipy.linalg import svd
 from scipy.linalg import norm
+from scipy.linalg import svd
+from scipy.spatial.distance import cdist
 
-from compas.tolerance import TOL
 from compas.geometry import pca_numpy
 from compas.geometry import transform_points_numpy
 from compas.linalg import normrow
+from compas.tolerance import TOL
 
 
 def bestfit_transform(A, B):
     n, m = A.shape
     Am = np.mean(A, axis=0)
     Bm = np.mean(B, axis=0)
     AA = A - Am
@@ -69,16 +69,16 @@
     During this iterative process, we continuously update the correspondence
     between the point clouds by finding the closest point in the target to each
     of the source points.
 
     The algorithm terminates when the alignment error is below a specified tolerance.
 
     """
-    from compas.geometry import Transformation
     from compas.geometry import Frame
+    from compas.geometry import Transformation
 
     tol = tol or TOL.approximation
 
     A = asarray(source)
     B = asarray(target)
 
     origin, axes, _ = pca_numpy(A)
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/interpolation_barycentric.py` & `compas-2.1.1/src/compas/geometry/interpolation_barycentric.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.geometry import subtract_vectors
 from compas.geometry import dot_vectors
+from compas.geometry import subtract_vectors
 
 
 def barycentric_coordinates(point, triangle):
     """Compute the barycentric coordinates of a point wrt to a triangle.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/interpolation_coons.py` & `compas-2.1.1/src/compas/geometry/interpolation_coons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.geometry import add_vectors
 from compas.geometry import scale_vector
 from compas.geometry import subtract_vectors
 from compas.geometry import sum_vectors
-
-from compas.utilities import normalize_values
+from compas.itertools import normalize_values
 
 
 def discrete_coons_patch(ab, bc, dc, ad):
     """Creates a coons patch from a set of four or three boundary
     polylines (ab, bc, dc, ad).
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/interpolation_tweening.py` & `compas-2.1.1/src/compas/geometry/interpolation_tweening.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.geometry import add_vectors
-from compas.geometry import subtract_vectors
-from compas.geometry import scale_vector
 from compas.geometry import distance_point_point
+from compas.geometry import scale_vector
+from compas.geometry import subtract_vectors
 
 
 def tween_points(points1, points2, num):
     """Compute the interpolated points between two sets of points.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/intersection.py` & `compas-2.1.1/src/compas/geometry/intersection.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 # from compas.precision import Precision
 from compas.geometry import distance_point_point
 
 
 class Intersection(object):
     """A class for computing intersections between geometric objects.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/intersections.py` & `compas-2.1.1/src/compas/geometry/intersections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import fabs
 from math import sqrt
 
-from compas.tolerance import TOL
-
-from compas.utilities import pairwise
-from compas.plugins import pluggable
-from compas.plugins import PluginNotInstalledError
-
 from compas.geometry import add_vectors
-from compas.geometry import subtract_vectors
-from compas.geometry import scale_vector
 from compas.geometry import cross_vectors
-from compas.geometry import dot_vectors
-from compas.geometry import length_vector_xy
-from compas.geometry import subtract_vectors_xy
-from compas.geometry import normalize_vector
 from compas.geometry import distance_point_point
+from compas.geometry import dot_vectors
+from compas.geometry import is_point_in_triangle
 from compas.geometry import is_point_on_segment
 from compas.geometry import is_point_on_segment_xy
-from compas.geometry import is_point_in_triangle
+from compas.geometry import length_vector_xy
+from compas.geometry import normalize_vector
+from compas.geometry import scale_vector
+from compas.geometry import subtract_vectors
+from compas.geometry import subtract_vectors_xy
+from compas.itertools import pairwise
+from compas.plugins import PluginNotInstalledError
+from compas.plugins import pluggable
+from compas.tolerance import TOL
 
 
 def intersection_line_line(l1, l2, tol=None):
     """Computes the intersection of two lines.
 
     Parameters
     ----------
@@ -203,15 +201,15 @@
 def intersection_line_plane(line, plane, tol=None):
     """Computes the intersection point of a line and a plane
 
     Parameters
     ----------
     line : [point, point] | :class:`compas.geometry.Line`
         Two points defining the line.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         The base point and normal defining the plane.
     tol : float, optional
         Tolerance for evaluating that the dot product of the line direction and the plane normal is zero.
         Default is :attr:`TOL.absolute`.
 
     Returns
     -------
@@ -251,15 +249,15 @@
 def intersection_segment_plane(segment, plane, tol=None):
     """Computes the intersection point of a line segment and a plane
 
     Parameters
     ----------
     segment : [point, point] | :class:`compas.geometry.Line`
         Two points defining the line segment.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         The base point and normal defining the plane.
     tol : float, optional
         Tolerance for evaluating that the dot product of the line direction and the plane normal is zero.
         Default is :attr:`TOL.absolute`.
 
     Returns
     -------
@@ -303,15 +301,15 @@
 def intersection_polyline_plane(polyline, plane, expected_number_of_intersections=None, tol=None):
     """Calculate the intersection point of a plane with a polyline. Reduce expected_number_of_intersections to speed up.
 
     Parameters
     ----------
     polyline : sequence[point] | :class:`compas.geometry.Polyline`
         Polyline to test intersection.
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         Plane to compute intersection.
     expected_number_of_intersections : int, optional
         Number of useful or expected intersections.
         Default is the number of line segments of the polyline.
     tol : float, optional
         Tolerance for computing the intersection points between the individual segments of the polyline and the plane.
         Default is :attr:`TOL.absolute`.
@@ -374,17 +372,17 @@
 
 
 def intersection_plane_plane(plane1, plane2, tol=None):
     """Computes the intersection of two planes
 
     Parameters
     ----------
-    plane1 : [point, vector] | :class:`compas.geometry.Plane`
+    plane1 : [point, vector]
         The base point and normal (normalized) defining the 1st plane.
-    plane2 : [point, vector] | :class:`compas.geometry.Plane`
+    plane2 : [point, vector]
         The base point and normal (normalized) defining the 2nd plane.
     tol : float, optional
         Tolerance for evaluating if the dot product of the plane normals is one.
         Default is :attr:`TOL.absolute`.
 
     Returns
     -------
@@ -412,19 +410,19 @@
 
 
 def intersection_plane_plane_plane(plane1, plane2, plane3, tol=None):
     """Computes the intersection of three planes
 
     Parameters
     ----------
-    plane1 : [point, vector] | :class:`compas.geometry.Plane`
+    plane1 : [point, vector]
         The base point and normal (normalized) defining the 1st plane.
-    plane2 : [point, vector] | :class:`compas.geometry.Plane`
+    plane2 : [point, vector]
         The base point and normal (normalized) defining the 2nd plane.
-    plane3 : [point, vector] | :class:`compas.geometry.Plane`
+    plane3 : [point, vector]
         The base point and normal (normalized) defining the 3rd plane.
     tol : float, optional
         Tolerance for computing the intersection line between the first two planes, and between the intersection line and the third plane.
         Default is :attr:`TOL.absolute`.
 
     Returns
     -------
@@ -448,17 +446,17 @@
 
 
 def intersection_sphere_sphere(sphere1, sphere2):
     """Computes the intersection of 2 spheres.
 
     Parameters
     ----------
-    sphere1 : [point, float] | :class:`compas.geometry.Sphere`
+    sphere1 : [point, float]
         A sphere defined by a point and radius.
-    sphere2 : [point, float] | :class:`compas.geometry.Sphere`
+    sphere2 : [point, float]
         A sphere defined by a point and radius.
 
     Returns
     -------
     {'point', 'circle', or 'sphere'}
         The type of intersection.
     [float, float, float] | tuple[[float, float, float], float, [float, float, float]] | tuple[[float, float, float], float]
@@ -587,15 +585,15 @@
 
 
 def intersection_sphere_line(sphere, line):
     """Computes the intersection of a sphere and a line.
 
     Parameters
     ----------
-    sphere : [point, radius] | :class:`compas.geometry.Sphere`
+    sphere : [point, radius]
         A sphere defined by a point and a radius.
     line : [point, point] | :class:`compas.geometry.Line`
         A line defined by two points.
 
     Returns
     -------
     tuple[[float, float, float], [float, float, float]] | [float, float, float] | None
@@ -607,44 +605,33 @@
 
     1. they intersect in 2 points
     2. they intersect in 1 point (line tangent to sphere), or
     3. they do not intersect.
 
     Examples
     --------
-    >>> from compas.geometry import allclose
+    >>> from compas.tolerance import TOL
 
     >>> sphere = (3.0, 7.0, 4.0), 10.0
     >>> line = (1.0, 0, 0.5), (2.0, 1.0, 0.5)
     >>> x1, x2 = intersection_sphere_line(sphere, line)
 
-    >>> allclose(x1, [11.634, 10.634, 0.500], 1e-3)
+    >>> TOL.is_allclose(x1, [11.634, 10.634, 0.500], atol=1e-3)
     True
-    >>> allclose(x2, [-0.634, -1.634, 0.50], 1e-3)
+    >>> TOL.is_allclose(x2, [-0.634, -1.634, 0.50], atol=1e-3)
     True
 
     """
     l1, l2 = line
     sp, radius = sphere
 
     a = (l2[0] - l1[0]) ** 2 + (l2[1] - l1[1]) ** 2 + (l2[2] - l1[2]) ** 2
-    b = 2.0 * (
-        (l2[0] - l1[0]) * (l1[0] - sp[0]) + (l2[1] - l1[1]) * (l1[1] - sp[1]) + (l2[2] - l1[2]) * (l1[2] - sp[2])
-    )
-
-    c = (
-        sp[0] ** 2
-        + sp[1] ** 2
-        + sp[2] ** 2
-        + l1[0] ** 2
-        + l1[1] ** 2
-        + l1[2] ** 2
-        - 2.0 * (sp[0] * l1[0] + sp[1] * l1[1] + sp[2] * l1[2])
-        - radius**2
-    )
+    b = 2.0 * ((l2[0] - l1[0]) * (l1[0] - sp[0]) + (l2[1] - l1[1]) * (l1[1] - sp[1]) + (l2[2] - l1[2]) * (l1[2] - sp[2]))
+
+    c = sp[0] ** 2 + sp[1] ** 2 + sp[2] ** 2 + l1[0] ** 2 + l1[1] ** 2 + l1[2] ** 2 - 2.0 * (sp[0] * l1[0] + sp[1] * l1[1] + sp[2] * l1[2]) - radius**2
 
     i = b * b - 4.0 * a * c
 
     if i < 0.0:  # case 3: no intersection
         return None
     elif i == 0.0:  # case 2: one intersection
         mu = -b / (2.0 * a)
@@ -673,17 +660,17 @@
 
 
 def intersection_plane_circle(plane, circle):
     """Computes the intersection of a plane and a circle.
 
     Parameters
     ----------
-    plane : [point, vector] | :class:`compas.geometry.Plane`
+    plane : [point, vector]
         A plane defined by a point and normal vector.
-    circle : [plane, float] | :class:`compas.geometry.Circle`
+    circle : [plane, float]
         A circle defined by a plane and radius.
 
     Returns
     -------
     tuple[[float, float, float], [float, float, float]] | [float, float, float] | None
         Two points (secant intersection), one point (tangent intersection), or None (otherwise).
 
@@ -950,17 +937,17 @@
 
 
 def intersection_circle_circle_xy(circle1, circle2):
     """Calculates the intersection points of two circles in 2d lying in the XY plane.
 
     Parameters
     ----------
-    circle1 : [plane, float] | :class:`compas.geometry.Circle`
+    circle1 : [plane, float]
         Circle defined by a plane, with at least XY coordinates, and a radius.
-    circle2 : [plane, float] | :class:`compas.geometry.Circle`
+    circle2 : [plane, float]
         Circle defined by a plane, with at least XY coordinates, and a radius.
 
     Returns
     -------
     tuple[[float, float, float], [float, float, float]] | None
         The intersection points if there are any.
         If the circles are tangent to each other, the two intersection points are identical.
@@ -1064,17 +1051,17 @@
     Based on [1]_.
 
     .. [1] C# Helper. *Calculate where a line segment and an ellipse intersect in C#*.
            Available at: http://csharphelper.com/blog/2017/08/calculate-where-a-line-segment-and-an-ellipse-intersect-in-c/
 
     Examples
     --------
-    >>> ellipse = 6., 2.5
-    >>> p1 = (4.1, 2.8, 0.)
-    >>> p2 = (3.4, -3.1, 0.)
+    >>> ellipse = 6.0, 2.5
+    >>> p1 = (4.1, 2.8, 0.0)
+    >>> p2 = (3.4, -3.1, 0.0)
     >>> i1, i2 = intersection_ellipse_line_xy(ellipse, [p1, p2])
 
     """
     x1, y1 = line[0][0], line[0][1]
     x2, y2 = line[1][0], line[1][1]
 
     a, b = ellipse
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/kdtree.py` & `compas-2.1.1/src/compas/geometry/kdtree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import collections
 
 from ._core.distance import distance_point_point_sqrd
 
-
 Node = collections.namedtuple("Node", "point axis label left right")
 
 
 class KDTree(object):
     """A tree for nearest neighbor search in a k-dimensional space.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/offset.py` & `compas-2.1.1/src/compas/geometry/offset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.geometry import scale_vector
-from compas.geometry import normalize_vector
+from compas.data.validators import is_item_iterable
 from compas.geometry import add_vectors
-from compas.geometry import subtract_vectors
-from compas.geometry import cross_vectors
 from compas.geometry import centroid_points
+from compas.geometry import cross_vectors
 from compas.geometry import intersection_line_line
-from compas.geometry import normal_polygon
 from compas.geometry import is_colinear
-
-from compas.data.validators import is_item_iterable
-
-from compas.utilities import iterable_like
-from compas.utilities import pairwise
+from compas.geometry import normal_polygon
+from compas.geometry import normalize_vector
+from compas.geometry import scale_vector
+from compas.geometry import subtract_vectors
+from compas.itertools import iterable_like
+from compas.itertools import pairwise
 
 
 def intersect_lines(l1, l2, tol):
     x1, x2 = intersection_line_line(l1, l2, tol)
     if x1 and x2:
         return centroid_points([x1, x2])
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/pca_numpy.py` & `compas-2.1.1/src/compas/geometry/pca_numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,15 @@
     --------
     >>>
     """
     X = asarray(data)
     n, dim = X.shape
 
     if not n >= dim:
-        raise ValueError(
-            "The number of observations (n) should be higher than the number of measured variables (dimensions)."
-        )
+        raise ValueError("The number of observations (n) should be higher than the number of measured variables (dimensions).")
 
     # the average of the observations for each of the variables
     # for example, if the data are 2D point coordinates,
     # the average is the average of the x-coordinate across all observations
     # and the average of the y-coordinate across all observations
     mean = (X.sum(axis=0) / n).reshape((-1, dim))
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/plane.py` & `compas-2.1.1/src/compas/geometry/plane.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 from math import sqrt
 
+from compas.geometry import Geometry
+from compas.geometry import bestfit_plane
+from compas.geometry import cross_vectors
 from compas.tolerance import TOL
 
-from compas.geometry import cross_vectors
-from compas.geometry import bestfit_plane
-from compas.geometry import Geometry
-from .vector import Vector
 from .point import Point
+from .vector import Vector
 
 
 class Plane(Geometry):
     """A plane is defined by a base point and a normal vector.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/point.py` & `compas-2.1.1/src/compas/geometry/point.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     Point objects support basic arithmetic operations.
 
     >>> p1 + p2
     Point(5.000, 7.000, 9.000)
     >>> p1 * 2
     Point(2.000, 4.000, 6.000)
-    >>> p1 ** 2
+    >>> p1**2
     Point(1.000, 4.000, 9.000)
     >>> p1
     Point(1.000, 2.000, 3.000)
 
     Points and lists can be used interchangeably.
 
     >>> p1 + [4, 5, 6]
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/pointcloud.py` & `compas-2.1.1/src/compas/geometry/pointcloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from random import uniform
 
-from compas.tolerance import TOL
-
-from compas.geometry import KDTree
 from compas.geometry import Geometry
+from compas.geometry import KDTree
 from compas.geometry import Point
-from compas.geometry import transform_points
-from compas.geometry import centroid_points
 from compas.geometry import bounding_box
+from compas.geometry import centroid_points
 from compas.geometry import closest_point_in_cloud
+from compas.geometry import transform_points
+from compas.tolerance import TOL
 
 
 class Pointcloud(Geometry):
     """Class for working with pointclouds.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/polygon.py` & `compas-2.1.1/src/compas/geometry/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import math
 
-from compas.utilities import pairwise
-from compas.geometry import allclose
+from compas.geometry import Frame
+from compas.geometry import Geometry
+from compas.geometry import Line
+from compas.geometry import Plane
+from compas.geometry import Point
+from compas.geometry import Transformation
 from compas.geometry import area_polygon
+from compas.geometry import bounding_box
 from compas.geometry import centroid_polygon
+from compas.geometry import earclip_polygon
 from compas.geometry import is_coplanar
 from compas.geometry import is_polygon_convex
 from compas.geometry import transform_points
-from compas.geometry import earclip_polygon
-from compas.geometry import bounding_box
-from compas.geometry import Geometry
-from compas.geometry import Transformation
-from compas.geometry import Point
-from compas.geometry import Plane
-from compas.geometry import Frame
-from compas.geometry import Line
+from compas.itertools import pairwise
+from compas.tolerance import TOL
 
 
 class Polygon(Geometry):
     """A polygon is a geometric object defined by a sequence of points forming a closed loop.
 
     A polygon is defined by a sequence of points connected by line segments
     forming a closed boundary that separates its interior from the exterior.
@@ -115,15 +115,15 @@
 
     def __iter__(self):
         return iter(self.points)
 
     def __eq__(self, other):
         if not hasattr(other, "__iter__") or not hasattr(other, "__len__") or len(self) != len(other):
             return False
-        return allclose(self, other)
+        return TOL.is_allclose(self, other)
 
     # ==========================================================================
     # Properties
     # ==========================================================================
 
     @property
     def points(self):
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/polyhedron.py` & `compas-2.1.1/src/compas/geometry/polyhedron.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import sqrt
 
-from compas.utilities import pairwise
-from compas.geometry import transform_points
-from compas.geometry import Polygon
-from compas.geometry import Point
 from compas.geometry import Line
+from compas.geometry import Point
+from compas.geometry import Polygon
+from compas.geometry import transform_points
+from compas.itertools import pairwise
+
 from .geometry import Geometry
 
 
 def tetrahedron():
     faces = [[0, 1, 2], [0, 3, 1], [0, 2, 3], [1, 3, 2]]
     vertices = []
     L = 2.0
@@ -410,18 +411,23 @@
         >>> halfspaces = np.array([left.abcd, right.abcd, top.abcd, bottom.abcd, front.abcd, back.abcd], dtype=float)
         >>> interior = np.array([0, 0, 0], dtype=float)
 
         >>> p = Polyhedron.from_halfspaces(halfspaces, interior)
 
         """
         from itertools import combinations
+
         from numpy import asarray
-        from scipy.spatial import HalfspaceIntersection, ConvexHull  # type: ignore
+        from scipy.spatial import ConvexHull  # type: ignore
+        from scipy.spatial import HalfspaceIntersection  # type: ignore
+
         from compas.datastructures import Mesh
-        from compas.geometry import length_vector, dot_vectors, cross_vectors
+        from compas.geometry import cross_vectors
+        from compas.geometry import dot_vectors
+        from compas.geometry import length_vector
 
         halfspaces = asarray(halfspaces, dtype=float)
         interior_point = asarray(interior_point, dtype=float)
         hsi = HalfspaceIntersection(halfspaces, interior_point)
         hull = ConvexHull(hsi.intersections)
         mesh = Mesh.from_vertices_and_faces([hsi.intersections[i] for i in hull.vertices], hull.simplices)
         mesh.unify_cycles()
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/projection.py` & `compas-2.1.1/src/compas/geometry/projection.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     * http://code.activestate.com/recipes/578108-determinant-of-matrix-of-any-order/
     * http://blog.acipo.com/matrix-inversion-in-javascript/
 
 Many thanks to Christoph Gohlke, Martin John Baker, Sachin Joglekar and Andrew
 Ippoliti for providing code and documentation.
 """
 
-from compas.utilities import flatten
-from compas.geometry import allclose
+from compas.geometry import Transformation
 from compas.geometry import decompose_matrix
 from compas.geometry import matrix_from_orthogonal_projection
 from compas.geometry import matrix_from_parallel_projection
-from compas.geometry import matrix_from_perspective_projection
 from compas.geometry import matrix_from_perspective_entries
-from compas.geometry import Transformation
+from compas.geometry import matrix_from_perspective_projection
+from compas.itertools import flatten
+from compas.tolerance import TOL
 
 
 class Projection(Transformation):
     """Class representing a projection transformation.
 
     Parameters
     ----------
@@ -43,15 +43,15 @@
     >>>
 
     """
 
     def __init__(self, matrix=None, check=False, name=None):
         if matrix and check:
             _, _, _, _, perspective = decompose_matrix(matrix)
-            if not allclose(flatten(matrix), flatten(matrix_from_perspective_entries(perspective))):
+            if not TOL.is_allclose(flatten(matrix), flatten(matrix_from_perspective_entries(perspective))):
                 raise ValueError("This is not a proper projection matrix.")
         super(Projection, self).__init__(matrix=matrix, name=name)
 
     @classmethod
     def from_plane(cls, plane):
         """Construct an orthogonal projection transformation to project onto a plane.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/quadmesh_planarize.py` & `compas-2.1.1/src/compas/geometry/quadmesh_planarize.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.plugins import pluggable
 
 
 @pluggable(category="quadmesh")
 def quadmesh_planarize(M, kmax=500, maxdev=0.005):
     """Planarize the faces of a quad mesh.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/quadmesh_planarize_none.py` & `compas-2.1.1/src/compas/geometry/quadmesh_planarize_none.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.geometry import project_points_plane
+from compas.geometry import bestfit_plane
 from compas.geometry import centroid_points
-from compas.geometry import midpoint_point_point
-from compas.geometry import distance_point_point
 from compas.geometry import distance_line_line
-from compas.geometry import bestfit_plane
-
-from compas.utilities import window
-from compas.utilities import pairwise
+from compas.geometry import distance_point_point
+from compas.geometry import midpoint_point_point
+from compas.geometry import project_points_plane
+from compas.itertools import pairwise
+from compas.itertools import window
 
 
 def mesh_flatness(mesh, maxdev=1.0):
     """Compute mesh flatness per face.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/quaternion.py` & `compas-2.1.1/src/compas/geometry/quaternion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.tolerance import TOL
+import math
+from sys import float_info
 
-from compas.geometry import quaternion_multiply
-from compas.geometry import quaternion_conjugate
-from compas.geometry import quaternion_unitize
+from compas.geometry import Geometry
+from compas.geometry import Rotation
 from compas.geometry import quaternion_canonize
-from compas.geometry import quaternion_norm
-from compas.geometry import quaternion_is_unit
+from compas.geometry import quaternion_conjugate
 from compas.geometry import quaternion_from_matrix
-from compas.geometry import Geometry
+from compas.geometry import quaternion_is_unit
+from compas.geometry import quaternion_multiply
+from compas.geometry import quaternion_norm
+from compas.geometry import quaternion_unitize
+from compas.tolerance import TOL
 
 
 class Quaternion(Geometry):
     r"""A quaternion is defined by 4 components, X, Y, Z, and W.
 
     Parameters
     ----------
@@ -155,28 +158,30 @@
             return self.w
         if key == 1:
             return self.x
         if key == 2:
             return self.y
         if key == 3:
             return self.z
-        raise KeyError
+        raise KeyError(key)
 
     def __setitem__(self, key, value):
         if key == 0:
             self.w = value
             return
         if key == 1:
             self.x = value
             return
         if key == 2:
             self.y = value
+            return
         if key == 3:
             self.z = value
-        raise KeyError
+            return
+        raise KeyError(key)
 
     def __iter__(self):
         return iter(self.wxyz)
 
     def __len__(self):
         return 4
 
@@ -255,16 +260,16 @@
         provided that both R and Q are unit-length.
         The result is also unit-length.
         Multiplication of quaternions is not commutative!
 
         Examples
         --------
         >>> Q = Quaternion(1.0, 1.0, 1.0, 1.0).unitized()
-        >>> R = Quaternion(0.0,-0.1, 0.2,-0.3).unitized()
-        >>> P = R*Q
+        >>> R = Quaternion(0.0, -0.1, 0.2, -0.3).unitized()
+        >>> P = R * Q
         >>> P.is_unit
         True
 
         """
         p = quaternion_multiply(list(self), list(other))
         return Quaternion(*p)
 
@@ -283,20 +288,20 @@
         Returns
         -------
         :class:`compas.geometry.Quaternion`
             The new quaternion.
 
         Examples
         --------
-        >>> from compas.geometry import allclose
+        >>> from compas.tolerance import TOL
         >>> from compas.geometry import Frame
-        >>> q = [1., -2., 3., -4.]
+        >>> q = [1.0, -2.0, 3.0, -4.0]
         >>> F = Frame.from_quaternion(q)
         >>> Q = Quaternion.from_frame(F)
-        >>> allclose(Q.canonized(), quaternion_canonize(quaternion_unitize(q)))
+        >>> TOL.is_allclose(Q.canonized(), quaternion_canonize(quaternion_unitize(q)))
         True
 
         """
         w, x, y, z = frame.quaternion
         return cls(w, x, y, z)
 
     @classmethod
@@ -363,15 +368,15 @@
         >>> q.is_unit
         False
         >>> q.unitize()
         >>> q.is_unit
         True
 
         """
-        qu = quaternion_unitize(self)
+        qu = quaternion_unitize(list(self))
         self.w, self.x, self.y, self.z = qu
 
     def unitized(self):
         """Returns a quaternion with a unit-length.
 
         Returns
         -------
@@ -383,15 +388,15 @@
         >>> q.is_unit
         False
         >>> p = q.unitized()
         >>> p.is_unit
         True
 
         """
-        qu = quaternion_unitize(self)
+        qu = quaternion_unitize(list(self))
         return Quaternion(*qu)
 
     def canonize(self):
         """Makes the quaternion canonic.
 
         Returns
         -------
@@ -404,15 +409,15 @@
         >>> q
         Quaternion(-0.500, 0.500, 0.500, 0.500)
         >>> q.canonize()
         >>> q
         Quaternion(0.500, -0.500, -0.500, -0.500)
 
         """
-        qc = quaternion_canonize(self)
+        qc = quaternion_canonize(list(self))
         self.w, self.x, self.y, self.z = qc  # type: ignore
 
     def canonized(self):
         """Returns a quaternion in canonic form.
 
         Returns
         -------
@@ -426,15 +431,15 @@
         >>> q
         Quaternion(-0.500, 0.500, 0.500, 0.500)
         >>> p = q.canonized()
         >>> p
         Quaternion(0.500, -0.500, -0.500, -0.500)
 
         """
-        qc = quaternion_canonize(self)
+        qc = quaternion_canonize(list(self))
         return Quaternion(*qc)  # type: ignore
 
     def conjugate(self):
         """Conjugate the quaternion.
 
         Returns
         -------
@@ -444,15 +449,15 @@
         --------
         >>> q = Quaternion(1.0, 1.0, 1.0, 1.0)
         >>> q.conjugate()
         >>> q
         Quaternion(1.000, -1.000, -1.000, -1.000)
 
         """
-        qc = quaternion_conjugate(self)
+        qc = quaternion_conjugate(list(self))
         self.w, self.x, self.y, self.z = qc
 
     def conjugated(self):
         """Returns a conjugate quaternion.
 
         Returns
         -------
@@ -465,9 +470,75 @@
         >>> p = q.conjugated()
         >>> q
         Quaternion(1.000, 1.000, 1.000, 1.000)
         >>> p
         Quaternion(1.000, -1.000, -1.000, -1.000)
 
         """
-        qc = quaternion_conjugate(self)
+        qc = quaternion_conjugate(list(self))
         return Quaternion(*qc)
+
+    def dot(self, other):
+        """Computes the cosine of the angle between the two quaternions"""
+        return self.w * other.w + self.x * other.x + self.y * other.y + self.z * other.z
+
+    def slerp(self, other, t):
+        """Slerp: spherical interpolation of two quaternions.
+
+        Parameters
+        ----------
+        other : :class:`compas.geometry.Quaternion`
+            The other quaternion to interpolate between.
+        t : float
+            A parameter in the range [0-1].
+
+        Returns
+        -------
+        :class:`compas.geometry.Quaternion`
+
+        Examples
+        --------
+        >>> q1 = Quaternion(1, 0, 0, 0)
+        >>> q2 = Quaternion(0, 1, 0, 0)
+        >>> t = 0.5
+        >>> interpolated_quaternion = Quaternion.slerp(q1, q2, t)
+
+        """
+        epsilon = float_info.epsilon
+
+        q1 = self.unitized()
+        q2 = other.unitized()
+
+        cosom = q1.dot(q2)
+
+        interpolated = Rotation()
+        quat = list(interpolated.quaternion)
+
+        # rotate around the shortest angle
+        if cosom < 0.0:
+            cosom = -cosom
+            quat[0] = -q1[0]
+            quat[1] = -q1[1]
+            quat[2] = -q1[2]
+            quat[3] = -q1[3]
+
+        else:
+            quat[0] = q1[0]
+            quat[1] = q1[1]
+            quat[2] = q1[2]
+            quat[3] = q1[3]
+
+        if (1.0 - cosom) > epsilon:
+            omega = math.acos(cosom)
+            sinom = math.sin(omega)
+            sc1 = math.sin((1.0 - t) * omega) / sinom
+            sc2 = math.sin(t * omega) / sinom
+        else:
+            sc1 = 1.0 - t
+            sc2 = t
+
+        qw_interp = sc1 * quat[0] + sc2 * q2[0]
+        qx_interp = sc1 * quat[1] + sc2 * q2[1]
+        qy_interp = sc1 * quat[2] + sc2 * q2[2]
+        qz_interp = sc1 * quat[3] + sc2 * q2[3]
+
+        return Quaternion(qw_interp, qx_interp, qy_interp, qz_interp)
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/reflection.py` & `compas-2.1.1/src/compas/geometry/reflection.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,23 @@
     * http://code.activestate.com/recipes/578108-determinant-of-matrix-of-any-order/
     * http://blog.acipo.com/matrix-inversion-in-javascript/
 
 Many thanks to Christoph Gohlke, Martin John Baker, Sachin Joglekar and Andrew
 Ippoliti for providing code and documentation.
 """
 
-from compas.utilities import flatten
-from compas.geometry import allclose
-from compas.geometry import dot_vectors
+from compas.geometry import Transformation
 from compas.geometry import cross_vectors
-from compas.geometry import normalize_vector
 from compas.geometry import decompose_matrix
-from compas.geometry import matrix_from_perspective_entries
+from compas.geometry import dot_vectors
 from compas.geometry import identity_matrix
-from compas.geometry import Transformation
+from compas.geometry import matrix_from_perspective_entries
+from compas.geometry import normalize_vector
+from compas.itertools import flatten
+from compas.tolerance import TOL
 
 
 class Reflection(Transformation):
     """Class representing a reflection transformation.
 
     A reflection transformation mirrors points at a plane.
 
@@ -46,15 +46,15 @@
     True
 
     """
 
     def __init__(self, matrix=None, check=False, name=None):
         if matrix and check:
             _, _, _, _, perspective = decompose_matrix(matrix)
-            if not allclose(flatten(matrix), flatten(matrix_from_perspective_entries(perspective))):
+            if not TOL.is_allclose(flatten(matrix), flatten(matrix_from_perspective_entries(perspective))):
                 raise ValueError("This is not a proper reflection matrix.")
         super(Reflection, self).__init__(matrix=matrix, name=name)
 
     @classmethod
     def from_plane(cls, plane):
         """Construct a reflection transformation that mirrors wrt the given plane.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/rotation.py` & `compas-2.1.1/src/compas/geometry/rotation.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,28 @@
     * http://code.activestate.com/recipes/578108-determinant-of-matrix-of-any-order/
     * http://blog.acipo.com/matrix-inversion-in-javascript/
 
 Many thanks to Christoph Gohlke, Martin John Baker, Sachin Joglekar and Andrew
 Ippoliti for providing code and documentation.
 """
 
-from compas.utilities import flatten
-from compas.geometry import normalize_vector
+from compas.geometry import Transformation
+from compas.geometry import axis_and_angle_from_matrix
+from compas.geometry import basis_vectors_from_matrix
 from compas.geometry import cross_vectors
-from compas.geometry import length_vector
-from compas.geometry import allclose
 from compas.geometry import decompose_matrix
-from compas.geometry import matrix_from_euler_angles
 from compas.geometry import euler_angles_from_matrix
+from compas.geometry import length_vector
 from compas.geometry import matrix_from_axis_and_angle
-from compas.geometry import axis_and_angle_from_matrix
-from compas.geometry import matrix_from_quaternion
+from compas.geometry import matrix_from_euler_angles
 from compas.geometry import matrix_from_frame
-from compas.geometry import basis_vectors_from_matrix
-from compas.geometry import Transformation
+from compas.geometry import matrix_from_quaternion
+from compas.geometry import normalize_vector
+from compas.itertools import flatten
+from compas.tolerance import TOL
 
 
 class Rotation(Transformation):
     """Class representing a rotation transformation.
 
     The class contains methods for converting rotation matrices to axis-angle
     representations, Euler angles, quaternion and basis vectors.
@@ -59,30 +59,30 @@
         If ``check`` is ``True`` and the provided transformation matrix is not a rotation.
 
     Examples
     --------
     >>> from compas.geometry import Frame
     >>> f1 = Frame([0, 0, 0], [0.68, 0.68, 0.27], [-0.67, 0.73, -0.15])
     >>> R = Rotation.from_frame(f1)
-    >>> args = False, 'xyz'
+    >>> args = False, "xyz"
     >>> alpha, beta, gamma = R.euler_angles(*args)
     >>> xaxis, yaxis, zaxis = [1, 0, 0], [0, 1, 0], [0, 0, 1]
     >>> Rx = Rotation.from_axis_and_angle(xaxis, alpha)
     >>> Ry = Rotation.from_axis_and_angle(yaxis, beta)
     >>> Rz = Rotation.from_axis_and_angle(zaxis, gamma)
     >>> f2 = Frame.worldXY()
     >>> f1 == f2.transformed(Rx * Ry * Rz)
     True
 
     """
 
     def __init__(self, matrix=None, check=False, name=None):
         if matrix and check:
             _, _, angles, _, _ = decompose_matrix(matrix)
-            if not allclose(flatten(matrix), flatten(matrix_from_euler_angles(angles))):
+            if not TOL.is_allclose(flatten(matrix), flatten(matrix_from_euler_angles(angles))):
                 raise ValueError("This is not a proper rotation matrix.")
         super(Rotation, self).__init__(matrix=matrix, name=name)
 
     @property
     def quaternion(self):
         from compas.geometry import Quaternion
 
@@ -226,19 +226,19 @@
 
         Returns
         -------
         :class:`compas.geometry.Rotation`
 
         Examples
         --------
-        >>> from compas.geometry import allclose
+        >>> from compas.tolerance import TOL
         >>> q1 = [0.945, -0.021, -0.125, 0.303]
         >>> R = Rotation.from_quaternion(q1)
         >>> q2 = R.quaternion
-        >>> allclose(q1, q2)
+        >>> TOL.is_allclose(q1, q2)
         True
 
         """
         matrix = matrix_from_quaternion(quaternion)
         return cls(matrix)
 
     @classmethod
@@ -254,19 +254,19 @@
 
         Returns
         -------
         :class:`compas.geometry.Rotation`
 
         Examples
         --------
-        >>> from compas.geometry import allclose
+        >>> from compas.tolerance import TOL
         >>> aav1 = [-0.043, -0.254, 0.617]
         >>> R = Rotation.from_axis_angle_vector(aav1)
         >>> aav2 = R.axis_angle_vector
-        >>> allclose(aav1, aav2)
+        >>> TOL.is_allclose(aav1, aav2)
         True
 
         """
         angle = length_vector(axis_angle_vector)
         return cls.from_axis_and_angle(axis_angle_vector, angle, point)
 
     # why is this repeated here?
@@ -293,20 +293,20 @@
 
         Returns
         -------
         :class:`compas.geometry.Rotation`
 
         Examples
         --------
-        >>> from compas.geometry import allclose
+        >>> from compas.tolerance import TOL
         >>> ea1 = 1.4, 0.5, 2.3
-        >>> args = False, 'xyz'
+        >>> args = False, "xyz"
         >>> R1 = Rotation.from_euler_angles(ea1, *args)
         >>> ea2 = R1.euler_angles(*args)
-        >>> allclose(ea1, ea2)
+        >>> TOL.is_allclose(ea1, ea2)
         True
 
         >>> alpha, beta, gamma = ea1
         >>> xaxis, yaxis, zaxis = [1, 0, 0], [0, 1, 0], [0, 0, 1]
         >>> Rx = Rotation.from_axis_and_angle(xaxis, alpha)
         >>> Ry = Rotation.from_axis_and_angle(yaxis, beta)
         >>> Rz = Rotation.from_axis_and_angle(zaxis, gamma)
@@ -338,17 +338,17 @@
         Returns
         -------
         [float, float, float]
             The 3 Euler angles.
 
         Examples
         --------
-        >>> from compas.geometry import allclose
+        >>> from compas.tolerance import TOL
         >>> ea1 = 1.4, 0.5, 2.3
-        >>> args = False, 'xyz'
+        >>> args = False, "xyz"
         >>> R1 = Rotation.from_euler_angles(ea1, *args)
         >>> ea2 = R1.euler_angles(*args)
-        >>> allclose(ea1, ea2)
+        >>> TOL.is_allclose(ea1, ea2)
         True
 
         """
         return euler_angles_from_matrix(self.matrix, static, axes)
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/scale.py` & `compas-2.1.1/src/compas/geometry/scale.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     * http://code.activestate.com/recipes/578108-determinant-of-matrix-of-any-order/
     * http://blog.acipo.com/matrix-inversion-in-javascript/
 
 Many thanks to Christoph Gohlke, Martin John Baker, Sachin Joglekar and Andrew
 Ippoliti for providing code and documentation.
 """
 
-from compas.utilities import flatten
-from compas.geometry import allclose
-from compas.geometry import multiply_matrices
+from compas.geometry import Transformation
 from compas.geometry import decompose_matrix
-from compas.geometry import matrix_from_scale_factors
 from compas.geometry import matrix_from_frame
+from compas.geometry import matrix_from_scale_factors
 from compas.geometry import matrix_inverse
-from compas.geometry import Transformation
+from compas.geometry import multiply_matrices
+from compas.itertools import flatten
+from compas.tolerance import TOL
 
 
 class Scale(Transformation):
     """Class representing a scale transformation.
 
     Parameters
     ----------
@@ -48,24 +48,24 @@
     >>> S[2, 2] == 3
     True
 
     >>> from compas.geometry import Point, Frame
     >>> point = Point(2, 5, 0)
     >>> frame = Frame(point, (1, 0, 0), (0, 1, 0))
     >>> points = [point, Point(2, 10, 0)]
-    >>> S = Scale.from_factors([2.] * 3, frame)
+    >>> S = Scale.from_factors([2.0] * 3, frame)
     >>> [p.transformed(S) for p in points]
     [Point(2.000, 5.000, 0.000), Point(2.000, 15.000, 0.000)]
 
     """
 
     def __init__(self, matrix=None, check=False, name=None):
         if matrix and check:
             scale, _, _, _, _ = decompose_matrix(matrix)
-            if not allclose(flatten(matrix), flatten(matrix_from_scale_factors(scale))):
+            if not TOL.is_allclose(flatten(matrix), flatten(matrix_from_scale_factors(scale))):
                 raise ValueError("This is not a proper scale matrix.")
         super(Scale, self).__init__(matrix=matrix, name=name)
 
     @classmethod
     def from_factors(cls, factors, frame=None):
         """Construct a scale transformation from scale factors.
 
@@ -83,15 +83,15 @@
 
         Examples
         --------
         >>> from compas.geometry import Point, Frame
         >>> point = Point(2, 5, 0)
         >>> frame = Frame(point, (1, 0, 0), (0, 1, 0))
         >>> points = [point, Point(2, 10, 0)]
-        >>> S = Scale.from_factors([2.] * 3, frame)
+        >>> S = Scale.from_factors([2.0] * 3, frame)
         >>> [p.transformed(S) for p in points]
         [Point(2.000, 5.000, 0.000), Point(2.000, 15.000, 0.000)]
 
         """
         matrix = matrix_from_scale_factors(factors)
         if frame:
             Tw = matrix_from_frame(frame)
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/shapes/box.py` & `compas-2.1.1/src/compas/geometry/shapes/box.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-from compas.geometry import centroid_points
-from compas.geometry import transform_points
-from compas.geometry import Transformation
 from compas.geometry import Frame
-from compas.geometry import Vector
 from compas.geometry import Line
+from compas.geometry import Transformation
+from compas.geometry import Vector
+from compas.geometry import centroid_points
+from compas.geometry import transform_points
 
 from .shape import Shape
 
 
 class Box(Shape):
     """A box is defined by a frame and its dimensions along the frame's x-, y- and z-axes.
 
@@ -147,44 +147,14 @@
             type(self).__name__,
             self.xsize,
             self.ysize,
             self.zsize,
             self.frame,
         )
 
-    def __len__(self):
-        return 4
-
-    def __getitem__(self, key):
-        if key == 0:
-            return self.xsize
-        elif key == 1:
-            return self.ysize
-        elif key == 2:
-            return self.zsize
-        elif key == 3:
-            return self.frame
-        else:
-            raise KeyError
-
-    def __setitem__(self, key, value):
-        if key == 0:
-            self.xsize = value
-        elif key == 1:
-            self.ysize = value
-        elif key == 2:
-            self.zsize = value
-        elif key == 3:
-            self.frame = value
-        else:
-            raise KeyError
-
-    def __iter__(self):
-        return iter([self.xsize, self.ysize, self.zsize, self.frame])
-
     # ==========================================================================
     # Properties
     # ==========================================================================
 
     @property
     def xsize(self):
         if self._xsize is None:
@@ -255,26 +225,16 @@
 
     @property
     def height(self):
         return self.zsize
 
     @property
     def diagonal(self):
-        a = (
-            self.frame.point
-            + self.frame.xaxis * -0.5 * self.xsize
-            + self.frame.yaxis * -0.5 * self.ysize
-            + self.frame.zaxis * -0.5 * self.zsize
-        )
-        b = (
-            self.frame.point
-            + self.frame.xaxis * 0.5 * self.xsize
-            + self.frame.yaxis * 0.5 * self.ysize
-            + self.frame.zaxis * 0.5 * self.zsize
-        )
+        a = self.frame.point + self.frame.xaxis * -0.5 * self.xsize + self.frame.yaxis * -0.5 * self.ysize + self.frame.zaxis * -0.5 * self.zsize
+        b = self.frame.point + self.frame.xaxis * 0.5 * self.xsize + self.frame.yaxis * 0.5 * self.ysize + self.frame.zaxis * 0.5 * self.zsize
         return Line(a, b)
 
     @property
     def dimensions(self):
         return [self.xsize, self.ysize, self.zsize]
 
     @property
@@ -305,14 +265,36 @@
     def left(self):
         return [1, 0, 4, 7]
 
     @property
     def top(self):
         return [4, 5, 6, 7]
 
+    @property
+    def points(self):
+        point = self.frame.point
+        xaxis = self.frame.xaxis
+        yaxis = self.frame.yaxis
+        zaxis = self.frame.zaxis
+
+        dx = 0.5 * self.xsize
+        dy = 0.5 * self.ysize
+        dz = 0.5 * self.zsize
+
+        a = point + xaxis * -dx + yaxis * -dy + zaxis * -dz
+        b = point + xaxis * -dx + yaxis * +dy + zaxis * -dz
+        c = point + xaxis * +dx + yaxis * +dy + zaxis * -dz
+        d = point + xaxis * +dx + yaxis * -dy + zaxis * -dz
+        e = a + zaxis * self.zsize
+        f = d + zaxis * self.zsize
+        g = c + zaxis * self.zsize
+        h = b + zaxis * self.zsize
+
+        return [a, b, c, d, e, f, g, h]
+
     # ==========================================================================
     # Constructors
     # ==========================================================================
 
     @classmethod
     def from_width_height_depth(cls, width, height, depth):  # type: (...) -> Box
         """Construct a box from its width, height and depth.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/shapes/capsule.py` & `compas-2.1.1/src/compas/geometry/shapes/capsule.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from __future__ import division
 from __future__ import print_function
 
 from math import cos
 from math import pi
 from math import sin
 
-from compas.geometry import transform_points
+from compas.geometry import Circle
 from compas.geometry import Frame
-from compas.geometry import Plane
 from compas.geometry import Line
-from compas.geometry import Circle
+from compas.geometry import Plane
 from compas.geometry import Transformation
+from compas.geometry import transform_points
 
 from .shape import Shape
 
 
 class Capsule(Shape):
     """A capsule is defined by a frame, radius, and height.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/shapes/cone.py` & `compas-2.1.1/src/compas/geometry/shapes/cone.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from __future__ import print_function
 
 from math import cos
 from math import pi
 from math import sin
 from math import sqrt
 
-from compas.utilities import pairwise
-from compas.geometry import transform_points
 from compas.geometry import Circle
-from compas.geometry import Plane
-from compas.geometry import Line
 from compas.geometry import Frame
+from compas.geometry import Line
+from compas.geometry import Plane
+from compas.geometry import transform_points
+from compas.itertools import pairwise
 
 from .shape import Shape
 
 
 class Cone(Shape):
     """A cone is defined by a frame, radius, and height.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/shapes/cylinder.py` & `compas-2.1.1/src/compas/geometry/shapes/cylinder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from __future__ import division
 from __future__ import print_function
 
 from math import cos
 from math import pi
 from math import sin
 
-from compas.geometry import transform_points
 from compas.geometry import Circle
-from compas.geometry import Plane
 from compas.geometry import Frame
 from compas.geometry import Line
+from compas.geometry import Plane
+from compas.geometry import transform_points
 
 from .shape import Shape
 
 
 class Cylinder(Shape):
     """A cylinder is defined by a frame, radius, and height.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/shapes/shape.py` & `compas-2.1.1/src/compas/geometry/shapes/torus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,300 +1,294 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.geometry import Geometry
-from compas.geometry import Frame
-from compas.geometry import Transformation
-from compas.geometry import Rotation
-
-
-class Shape(Geometry):
-    """Base class for geometric shapes.
+from math import cos
+from math import pi
+from math import sin
 
-    Shapes are parametrically defined with repsect to a local coordinate system.
-    The local coordinate system of a shape is defined by a frame.
-    The default frame is the word coordinate system, i.e. the origin and the axes of the world XY plane.
+from compas.geometry import Frame
+from compas.geometry import Plane
+from compas.geometry import matrix_from_frame
+from compas.geometry import transform_points
 
-    Shapes are finite, closed objects, with a boundary that separates the interior from the exterior.
-    They have a well-defined surface area and volume.
+from .shape import Shape
 
-    An explicit representation of a shape is obtained by discretising its boundary into a set of vertices and faces with a chosen resolution (:meth:`to_vertices_and_faces`).
-    The vertices and faces can be used to construct a :class:`compas.geometry.Polyhedron` object (:meth:`to_polyhedron`).
-    A shape can also be converted to a :class:`compas.geometry.Brep` object (:meth:`to_brep`).
 
-    Breps and polyhedrons support boolean operations.
+class Torus(Shape):
+    """A torus is defined by a plane and two radii.
 
     Parameters
     ----------
+    radius_axis: float, optional
+        The radius of the axis.
+    radius_pipe: float, optional
+        The radius of the pipe.
     frame : :class:`compas.geometry.Frame`, optional
-        The local coordinate system of the shape.
-        Default is ``None``, in which case the world coordinate system is used.
+        The local coordinate system of the torus.
+        Default is ``None``, in which case the torus is constructed in the world XY plane.
+    name : str, optional
+        The name of the shape.
 
     Attributes
     ----------
-    area : float, read-only
-        The surface area of the shape.
     frame : :class:`compas.geometry.Frame`
-        The local coordinate system of the shape.
-    transformation : :class:`compas.geometry.Transformation`, read-only
-        The transformation of the shape to global coordinates.
+        The coordinate system of the torus.
+    transformation : :class:`compas.geometry.Transformation`
+        The transformation of the sphere to global coordinates.
+    radius_axis : float
+        The radius of the axis.
+    radius_pipe : float
+        The radius of the pipe.
+    axis : :class:`compas.geometry.Line`, read-only
+        The central axis of the torus.
+    base : :class:`compas.geometry.Point`, read-only
+        The base point of the torus.
+        The base point is at the origin of the local coordinate system.
+    plane : :class:`compas.geometry.Plane`, read-only
+        The plane of the torus.
+        The base point of the plane is at the origin of the local coordinate system.
+        The normal of the plane is in the direction of the z-axis of the local coordinate system.
+    circle : :class:`compas.geometry.Circle`, read-only
+        The base circle of the torus.
+        The center of the circle is at the origin of the local coordinate system.
+    area : float, read-only
+        The surface area of the torus.
     volume : float, read-only
-        The volume of the shape.
+        The volume of the torus.
+
+    Examples
+    --------
+    >>> from compas.geometry import Frame
+    >>> from compas.geometry import Torus
+    >>> torus = Torus(frame=Frame.worldXY(), radius_axis=5.0, radius_pipe=2.0)
+    >>> torus = Torus(radius_axis=5.0, radius_pipe=2.0)
 
     """
 
-    def __init__(self, frame=None, name=None):
-        super(Shape, self).__init__(name=name)
-        self._frame = None
-        self._transformation = None
-        self.frame = frame
-
-    # =============================================================================
-    # Data
-    # =============================================================================
+    DATASCHEMA = {
+        "type": "object",
+        "properties": {
+            "radius_axis": {"type": "number", "minimum": 0},
+            "radius_pipe": {"type": "number", "minimum": 0},
+            "frame": Frame.DATASCHEMA,
+        },
+        "required": ["radius_axis", "radius_pipe", "frame"],
+    }
+
+    @property
+    def __data__(self):
+        return {
+            "radius_axis": self.radius_axis,
+            "radius_pipe": self.radius_pipe,
+            "frame": self.frame.__data__,
+        }
+
+    @classmethod
+    def __from_data__(cls, data):
+        return cls(
+            radius_axis=data["radius_axis"],
+            radius_pipe=data["radius_pipe"],
+            frame=Frame.__from_data__(data["frame"]),
+        )
+
+    def __init__(self, radius_axis, radius_pipe, frame=None, name=None):
+        super(Torus, self).__init__(frame=frame, name=name)
+        self._radius_axis = None
+        self._radius_pipe = None
+        self.radius_axis = radius_axis
+        self.radius_pipe = radius_pipe
+
+    def __repr__(self):
+        return "Torus(frame={0!r}, radius_axis={1!r}, radius_pipe={2!r})".format(
+            self.frame,
+            self.radius_axis,
+            self.radius_pipe,
+        )
 
-    # =============================================================================
+    # ==========================================================================
     # Properties
-    # =============================================================================
+    # ==========================================================================
 
     @property
-    def frame(self):
-        if not self._frame:
-            self._frame = Frame.worldXY()
-        return self._frame
-
-    @frame.setter
-    def frame(self, frame):
-        if not frame:
-            self._frame = None
-        else:
-            self._frame = Frame(frame[0], frame[1], frame[2])
-        self._transformation = None
+    def plane(self):
+        return Plane(self.frame.point, self.frame.zaxis)
 
     @property
-    def transformation(self):
-        if not self._transformation:
-            self._transformation = Transformation.from_frame_to_frame(Frame.worldXY(), self.frame)
-        return self._transformation
+    def radius_axis(self):
+        if self._radius_axis is None:
+            raise ValueError("The torus has no axis radius.")
+        return self._radius_axis
+
+    @radius_axis.setter
+    def radius_axis(self, radius):
+        if radius < 0:
+            raise ValueError("The value for the axis radius should be radius >= 0.")
+        self._radius_axis = float(radius)
+
+    @property
+    def radius_pipe(self):
+        if self._radius_pipe is None:
+            raise ValueError("The torus has no pipe radius.")
+        return self._radius_pipe
+
+    @radius_pipe.setter
+    def radius_pipe(self, radius):
+        if radius < 0:
+            raise ValueError("The value for the pipe radius should be radius >= 0.")
+        self._radius_pipe = float(radius)
+
+    @property
+    def center(self):
+        return self.plane.point
 
     @property
     def area(self):
-        raise NotImplementedError
+        return (2 * pi * self.radius_pipe) * (2 * pi * self.radius_axis)
 
     @property
     def volume(self):
-        raise NotImplementedError
+        return (pi * self.radius_pipe**2) * (2 * pi * self.radius_axis)
 
-    # =============================================================================
+    # ==========================================================================
     # Constructors
-    # =============================================================================
+    # ==========================================================================
 
-    # =============================================================================
-    # Conversions
-    # =============================================================================
+    @classmethod
+    def from_plane_and_radii(cls, plane, radius_axis, radius_pipe):
+        """Construct a torus from a plane and two radii.
 
-    def to_vertices_and_faces(self, **kwargs):
-        """Convert the shape to a list of vertices and faces.
+        Parameters
+        ----------
+        plane : :class:`compas.geometry.Plane`
+            The plane of the torus.
+        radius_axis: float
+            The radius of the axis.
+        radius_pipe: float
+            The radius of the pipe.
 
         Returns
         -------
-        list of list of float
-            The vertices of the shape.
-        list of list of int
-            The faces of the shape.
+        :class:`compas.geometry.Torus`
+            The constructed torus.
+
+        Examples
+        --------
+        >>> from compas.geometry import Plane
+        >>> from compas.geometry import Torus
+        >>> plane = Plane.worldXY()
+        >>> torus = Torus.from_plane_and_radii(plane, 5.0, 2.0)
 
         """
-        raise NotImplementedError
+        frame = Frame.from_plane(plane)
+        return cls(radius_axis=radius_axis, radius_pipe=radius_pipe, frame=frame)
+
+    # ==========================================================================
+    # Conversions
+    # ==========================================================================
 
-    def to_polyhedron(self, triangulated=True, u=16, v=None):
-        """Convert the shape to a polyhedron.
+    def to_vertices_and_faces(self, u=16, v=16, triangulated=False):
+        """Returns a list of vertices and faces.
+
+        The vertices are defined in global coordinates.
 
         Parameters
         ----------
-        triangulated : bool, optional
-            If True, triangulate the faces.
         u : int, optional
             Number of faces in the "u" direction.
         v : int, optional
             Number of faces in the "v" direction.
-            If no value is provided, and the shape has two parameter directions, the value of ``u`` will be used.
+        triangulated: bool, optional
+            If True, triangulate the faces.
 
         Returns
         -------
-        :class:`compas.geometry.Polyhedron`
-            The polyhedron representation of the shape.
-
-        Notes
-        -----
-        Parameters ``u`` and ``v`` define the resolution of the discretisation of curved geometry.
-        If the geometry is not curved in a particular direction, the corresponding parameter will be ignored.
-        For example, a cylinder has a resolution in the "u" direction, but not in the "v" direction.
-        A sphere has a resolution in both the "u" and the "v" direction.
-        A box has no resolution in either direction.
+        list[list[float]], list[list[int]]
+            A list of vertex locations, and a list of faces,
+            with each face defined as a list of indices into the list of vertices.
 
         """
-        from compas.geometry import Polyhedron
-
-        v = v or u
-
-        vertices, faces = self.to_vertices_and_faces(u=u, v=v)
+        if u < 3:
+            raise ValueError("The value for u should be u > 3.")
+        if v < 3:
+            raise ValueError("The value for v should be v > 3.")
+
+        theta = pi * 2 / u
+        phi = pi * 2 / v
+        vertices = []
+        for i in range(u):
+            for j in range(v):
+                x = cos(i * theta) * (self.radius_axis + self.radius_pipe * cos(j * phi))
+                y = sin(i * theta) * (self.radius_axis + self.radius_pipe * cos(j * phi))
+                z = self.radius_pipe * sin(j * phi)
+                vertices.append([x, y, z])
+
+        # transform vertices to torus' plane
+        frame = Frame.from_plane(self.plane)
+        M = matrix_from_frame(frame)
+        vertices = transform_points(vertices, M)
+
+        faces = []
+        for i in range(u):
+            ii = (i + 1) % u
+            for j in range(v):
+                jj = (j + 1) % v
+                a = i * v + j
+                b = ii * v + j
+                c = ii * v + jj
+                d = i * v + jj
+                faces.append([a, b, c, d])
 
         if triangulated:
             triangles = []
             for face in faces:
                 if len(face) == 4:
                     triangles.append(face[0:3])
                     triangles.append([face[0], face[2], face[3]])
                 else:
                     triangles.append(face)
             faces = triangles
 
-        return Polyhedron(vertices, faces)
+        vertices = transform_points(vertices, self.transformation)
+
+        return vertices, faces
 
     def to_brep(self):
-        """Convert the shape to a Brep.
+        """Returns a BRep representation of the torus.
 
         Returns
         -------
-        :class:`compas.geometry.Brep`
-            The Brep representation of the shape.
+        :class:`compas.brep.Brep`
 
         """
-        raise NotImplementedError
+        from compas.geometry import Brep
 
-    # =============================================================================
-    # Transformation
-    # =============================================================================
+        return Brep.from_torus(self)
 
-    def transform(self, transformation):
-        """Transform the shape.
+    # ==========================================================================
+    # Transformations
+    # ==========================================================================
 
-        Transformations of a shape are performed by applying the transformation to the frame of the shape.
-        Transformations of the shape with respect to its local coordinate system are not supported.
-        For this reason, only (combinations of) translations and rotations are supported.
-        To scale a shape, use the :meth:`Shape.scale` method.
+    def transform(self, transformation):
+        """Transform the torus.
 
         Parameters
         ----------
-        transformation : :class:`Transformation`
-            The transformation used to transform the shape.
+        transformation : :class:`compas.geometry.Transformation`
+            The transformation used to transform the Torus.
 
         Returns
         -------
         None
 
-        See Also
+        Examples
         --------
-        translate
-        rotate
-        scale
+        >>> from compas.geometry import Frame
+        >>> from compas.geometry import Transformation
+        >>> from compas.geometry import Torus
+        >>> torus = Torus(Frame.worldXY(), 5, 2)
+        >>> frame = Frame([1, 1, 1], [0.68, 0.68, 0.27], [-0.67, 0.73, -0.15])
+        >>> T = Transformation.from_frame(frame)
+        >>> torus.transform(T)
 
         """
         self.frame.transform(transformation)
-
-    def translate(self, vector):
-        """Translate the shape.
-
-        Parameters
-        ----------
-        vector : :class:`Vector`
-            The translation vector.
-
-        Returns
-        -------
-        None
-
-        See Also
-        --------
-        rotate
-        scale
-        transform
-
-        """
-        self.frame.point += vector
-
-    def rotate(self, angle, axis=None, point=None):
-        """Rotate the shape.
-
-        Parameters
-        ----------
-        vector : :class:`Vector`
-            The translation vector.
-
-        Returns
-        -------
-        None
-
-        See Also
-        --------
-        translate
-        scale
-        transform
-
-        """
-        axis = axis or [0, 0, 1]
-        point = point or [0, 0, 0]
-        matrix = Rotation.from_axis_and_angle(axis=axis, angle=angle, point=point)
-        self.transform(matrix)
-
-    def scale(self, scale):
-        """Scale the shape.
-
-        Scale transformations are applied to the parameters of a shape rahter than to its frame.
-        Only uniform scaling is supported.
-
-        Parameters
-        ----------
-        scale : float
-            The scaling factor.
-
-        Returns
-        -------
-        None
-
-        See Also
-        --------
-        translate
-        rotate
-        transform
-
-        """
-        raise NotImplementedError
-
-    # =============================================================================
-    # Methods
-    # =============================================================================
-
-    def contains_point(self, point):
-        """Verify if a point is inside the shape.
-
-        Parameters
-        ----------
-        point : :class:`compas.geometry.Point`
-            The point to test.
-
-        Returns
-        -------
-        bool
-            True if the point is inside the shape.
-            False otherwise.
-
-        """
-        raise NotImplementedError
-
-    def contains_points(self, points):
-        """Verify if a list of points are inside the shape.
-
-        Parameters
-        ----------
-        points : list of :class:`compas.geometry.Point`
-            The points to test.
-
-        Returns
-        -------
-        list of bool
-            True if the point is inside the shape.
-            False otherwise.
-
-        """
-        return [self.contains_point(point) for point in points]
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/shapes/sphere.py` & `compas-2.1.1/src/compas/geometry/shapes/sphere.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from __future__ import division
 from __future__ import print_function
 
 from math import cos
 from math import pi
 from math import sin
 
-from compas.geometry import transform_points
+from compas.geometry import Circle
 from compas.geometry import Frame
 from compas.geometry import Line
-from compas.geometry import Circle
+from compas.geometry import transform_points
+
 from .shape import Shape
 
 
 class Sphere(Shape):
     """A sphere is defined by a point and a radius.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/shapes/torus.py` & `compas-2.1.1/src/compas_blender/scene/graphobject.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,322 +1,257 @@
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Optional
+from typing import Tuple
+from typing import Union
+
+import bpy  # type: ignore
+
+import compas_blender
+from compas.colors import Color
+from compas.datastructures import Graph
+from compas.geometry import Line
+from compas.scene import GraphObject as BaseSceneObject
+from compas_blender import conversions
 
-from math import cos
-from math import pi
-from math import sin
+from .sceneobject import BlenderSceneObject
 
-from compas.geometry import matrix_from_frame
-from compas.geometry import transform_points
-from compas.geometry import Frame
-from compas.geometry import Plane
 
-from .shape import Shape
-
-
-class Torus(Shape):
-    """A torus is defined by a plane and two radii.
+class GraphObject(BlenderSceneObject, BaseSceneObject):
+    """Scene object for drawing graph data structures in Blender.
 
     Parameters
     ----------
-    radius_axis: float, optional
-        The radius of the axis.
-    radius_pipe: float, optional
-        The radius of the pipe.
-    frame : :class:`compas.geometry.Frame`, optional
-        The local coordinate system of the torus.
-        Default is ``None``, in which case the torus is constructed in the world XY plane.
-    name : str, optional
-        The name of the shape.
-
-    Attributes
-    ----------
-    frame : :class:`compas.geometry.Frame`
-        The coordinate system of the torus.
-    transformation : :class:`compas.geometry.Transformation`
-        The transformation of the sphere to global coordinates.
-    radius_axis : float
-        The radius of the axis.
-    radius_pipe : float
-        The radius of the pipe.
-    axis : :class:`compas.geometry.Line`, read-only
-        The central axis of the torus.
-    base : :class:`compas.geometry.Point`, read-only
-        The base point of the torus.
-        The base point is at the origin of the local coordinate system.
-    plane : :class:`compas.geometry.Plane`, read-only
-        The plane of the torus.
-        The base point of the plane is at the origin of the local coordinate system.
-        The normal of the plane is in the direction of the z-axis of the local coordinate system.
-    circle : :class:`compas.geometry.Circle`, read-only
-        The base circle of the torus.
-        The center of the circle is at the origin of the local coordinate system.
-    area : float, read-only
-        The surface area of the torus.
-    volume : float, read-only
-        The volume of the torus.
-
-    Examples
-    --------
-    >>> from compas.geometry import Frame
-    >>> from compas.geometry import Torus
-    >>> torus = Torus(frame=Frame.worldXY(), radius_axis=5.0, radius_pipe=2.0)
-    >>> torus = Torus(radius_axis=5.0, radius_pipe=2.0)
+    graph : :class:`compas.datastructures.Graph`
+        A COMPAS graph.
 
     """
 
-    DATASCHEMA = {
-        "type": "object",
-        "properties": {
-            "radius_axis": {"type": "number", "minimum": 0},
-            "radius_pipe": {"type": "number", "minimum": 0},
-            "frame": Frame.DATASCHEMA,
-        },
-        "required": ["radius_axis", "radius_pipe", "frame"],
-    }
-
-    @property
-    def __data__(self):
-        return {
-            "radius_axis": self.radius_axis,
-            "radius_pipe": self.radius_pipe,
-            "frame": self.frame.__data__,
-        }
-
-    @classmethod
-    def __from_data__(cls, data):
-        return cls(
-            radius_axis=data["radius_axis"],
-            radius_pipe=data["radius_pipe"],
-            frame=Frame.__from_data__(data["frame"]),
-        )
-
-    def __init__(self, radius_axis, radius_pipe, frame=None, name=None):
-        super(Torus, self).__init__(frame=frame, name=name)
-        self._radius_axis = None
-        self._radius_pipe = None
-        self.radius_axis = radius_axis
-        self.radius_pipe = radius_pipe
+    def __init__(self, graph: Graph, **kwargs: Any):
+        super().__init__(graph=graph, **kwargs)
+        self.nodeobjects = []
+        self.edgeobjects = []
 
     # ==========================================================================
-    # Properties
+    # clear
     # ==========================================================================
 
-    @property
-    def plane(self):
-        return Plane(self.frame.point, self.frame.zaxis)
-
-    @property
-    def radius_axis(self):
-        if self._radius_axis is None:
-            raise ValueError("The torus has no axis radius.")
-        return self._radius_axis
-
-    @radius_axis.setter
-    def radius_axis(self, radius):
-        if radius < 0:
-            raise ValueError("The value for the axis radius should be radius >= 0.")
-        self._radius_axis = float(radius)
-
-    @property
-    def radius_pipe(self):
-        if self._radius_pipe is None:
-            raise ValueError("The torus has no pipe radius.")
-        return self._radius_pipe
-
-    @radius_pipe.setter
-    def radius_pipe(self, radius):
-        if radius < 0:
-            raise ValueError("The value for the pipe radius should be radius >= 0.")
-        self._radius_pipe = float(radius)
-
-    @property
-    def center(self):
-        return self.plane.point
-
-    @property
-    def area(self):
-        return (2 * pi * self.radius_pipe) * (2 * pi * self.radius_axis)
-
-    @property
-    def volume(self):
-        return (pi * self.radius_pipe**2) * (2 * pi * self.radius_axis)
+    def clear_nodes(self):
+        """Clear all objects contained in the node collection.
 
-    # ==========================================================================
-    # Customisation
-    # ==========================================================================
+        Returns
+        -------
+        None
 
-    def __repr__(self):
-        return "Torus(frame={0!r}, radius_axis={1!r}, radius_pipe={2!r})".format(
-            self.frame, self.radius_axis, self.radius_pipe
-        )
-
-    def __len__(self):
-        return 3
-
-    def __getitem__(self, key):
-        if key == 0:
-            return self.frame
-        elif key == 1:
-            return self.radius_axis
-        elif key == 2:
-            return self.radius_pipe
-        else:
-            raise KeyError
-
-    def __setitem__(self, key, value):
-        if key == 0:
-            self.frame = value
-        elif key == 1:
-            self.radius_axis = value
-        elif key == 2:
-            self.radius_pipe = value
-        else:
-            raise KeyError
+        """
+        compas_blender.delete_objects(self.nodeobjects)
 
-    def __iter__(self):
-        return iter([self.frame, self.radius_axis, self.radius_pipe])
+    def clear_edges(self):
+        """Clear all objects contained in the edge collection.
 
-    # ==========================================================================
-    # Constructors
-    # ==========================================================================
+        Returns
+        -------
+        None
 
-    @classmethod
-    def from_plane_and_radii(cls, plane, radius_axis, radius_pipe):
-        """Construct a torus from a plane and two radii.
+        """
+        compas_blender.delete_objects(self.edgeobjects)
 
-        Parameters
-        ----------
-        plane : :class:`compas.geometry.Plane`
-            The plane of the torus.
-        radius_axis: float
-            The radius of the axis.
-        radius_pipe: float
-            The radius of the pipe.
+    # def clear_nodelabels(self):
+    #     """Clear all objects contained in the nodelabel collection.
 
-        Returns
-        -------
-        :class:`compas.geometry.Torus`
-            The constructed torus.
+    #     Returns
+    #     -------
+    #     None
 
-        Examples
-        --------
-        >>> from compas.geometry import Plane
-        >>> from compas.geometry import Torus
-        >>> plane = Plane.worldXY()
-        >>> torus = Torus.from_plane_and_radii(plane, 5.0, 2.0)
+    #     """
+    #     compas_blender.delete_objects(self.nodelabelcollection.objects)
 
-        """
-        frame = Frame.from_plane(plane)
-        return cls(radius_axis=radius_axis, radius_pipe=radius_pipe, frame=frame)
+    # def clear_edgelabels(self):
+    #     """Clear all objects contained in the edgelabel collection.
+
+    #     Returns
+    #     -------
+    #     None
+
+    #     """
+    #     compas_blender.delete_objects(self.edgelabelcollection.objects)
 
     # ==========================================================================
-    # Conversions
+    # draw
     # ==========================================================================
 
-    def to_vertices_and_faces(self, u=16, v=16, triangulated=False):
-        """Returns a list of vertices and faces.
-
-        The vertices are defined in global coordinates.
+    def draw(
+        self,
+        nodes: Optional[List[int]] = None,
+        edges: Optional[Tuple[int, int]] = None,
+        nodecolor: Optional[Union[Color, Dict[int, Color]]] = None,
+        edgecolor: Optional[Union[Color, Dict[Tuple[int, int], Color]]] = None,
+    ) -> list[bpy.types.Object]:
+        """Draw the graph.
 
         Parameters
         ----------
-        u : int, optional
-            Number of faces in the "u" direction.
-        v : int, optional
-            Number of faces in the "v" direction.
-        triangulated: bool, optional
-            If True, triangulate the faces.
+        nodes : list[hashable], optional
+            A list of node identifiers.
+            Default is None, in which case all nodes are drawn.
+        edges : list[tuple[hashable, hashable]], optional
+            A list of edge keys (as uv pairs) identifying which edges to draw.
+            The default is None, in which case all edges are drawn.
+        nodecolor : :class:`compas.colors.Color` | dict[hashable, :class:`compas.colors.Color`], optional
+            The color specification for the nodes.
+        edgecolor : :class:`compas.colors.Color` | dict[tuple[hashable, hashable], :class:`compas.colors.Color`], optional
+            The color specification for the edges.
 
         Returns
         -------
-        list[list[float]], list[list[int]]
-            A list of vertex locations, and a list of faces,
-            with each face defined as a list of indices into the list of vertices.
+        list[:blender:`bpy.types.Object`]
+            The objects created in Blender.
 
         """
-        if u < 3:
-            raise ValueError("The value for u should be u > 3.")
-        if v < 3:
-            raise ValueError("The value for v should be v > 3.")
-
-        theta = pi * 2 / u
-        phi = pi * 2 / v
-        vertices = []
-        for i in range(u):
-            for j in range(v):
-                x = cos(i * theta) * (self.radius_axis + self.radius_pipe * cos(j * phi))
-                y = sin(i * theta) * (self.radius_axis + self.radius_pipe * cos(j * phi))
-                z = self.radius_pipe * sin(j * phi)
-                vertices.append([x, y, z])
-
-        # transform vertices to torus' plane
-        frame = Frame.from_plane(self.plane)
-        M = matrix_from_frame(frame)
-        vertices = transform_points(vertices, M)
-
-        faces = []
-        for i in range(u):
-            ii = (i + 1) % u
-            for j in range(v):
-                jj = (j + 1) % v
-                a = i * v + j
-                b = ii * v + j
-                c = ii * v + jj
-                d = i * v + jj
-                faces.append([a, b, c, d])
-
-        if triangulated:
-            triangles = []
-            for face in faces:
-                if len(face) == 4:
-                    triangles.append(face[0:3])
-                    triangles.append([face[0], face[2], face[3]])
-                else:
-                    triangles.append(face)
-            faces = triangles
+        self._guids = self.draw_nodes(nodes=nodes, color=nodecolor) + self.draw_edges(edges=edges, color=edgecolor)
+        return self.guids
 
-        vertices = transform_points(vertices, self.transformation)
+    def draw_nodes(
+        self,
+        nodes: Optional[List[int]] = None,
+        color: Optional[Union[Color, Dict[int, Color]]] = None,
+        collection: Optional[str] = None,
+        radius: float = 0.05,
+        u: int = 16,
+        v: int = 16,
+    ) -> List[bpy.types.Object]:
+        """Draw a selection of nodes.
 
-        return vertices, faces
-
-    def to_brep(self):
-        """Returns a BRep representation of the torus.
+        Parameters
+        ----------
+        nodes : list[hashable], optional
+            A list of node identifiers.
+            Default is None, in which case all nodes are drawn.
+        color : :class:`compas.colors.Color` | dict[hashable, :class:`compas.colors.Color`], optional
+            The color specification for the nodes.
+        collection : str, optional
+            The name of the Blender scene collection containing the created object(s).
 
         Returns
         -------
-        :class:`compas.brep.Brep`
+        list[:blender:`bpy.types.Object`]
 
         """
-        from compas.geometry import Brep
-
-        return Brep.from_torus(self)
+        objects = []
 
-    # ==========================================================================
-    # Transformations
-    # ==========================================================================
+        self.nodecolor = color
 
-    def transform(self, transformation):
-        """Transform the torus.
+        for node in nodes or self.graph.nodes():  # type: ignore
+            name = f"{self.graph.name}.node.{node}"  # type: ignore
+            color = self.nodecolor[node]  # type: ignore
+            point = self.graph.nodes_attributes("xyz")[node]  # type: ignore
+
+            # there is no such thing as a sphere data block
+            bpy.ops.mesh.primitive_uv_sphere_add(location=point, radius=radius, segments=u, ring_count=v)
+            obj = bpy.context.object
+            self.objects.append(obj)
+            self.update_object(obj, name=name, color=color, collection=collection)
+            objects.append(obj)
+
+        return objects
+
+    def draw_edges(
+        self,
+        edges: Optional[Tuple[int, int]] = None,
+        color: Optional[Union[Color, Dict[Tuple[int, int], Color]]] = None,
+        collection: Optional[str] = None,
+    ) -> List[bpy.types.Object]:
+        """Draw a selection of edges.
 
         Parameters
         ----------
-        transformation : :class:`compas.geometry.Transformation`
-            The transformation used to transform the Torus.
+        edges : list[tuple[hashable, hashable]], optional
+            A list of edge keys (as uv pairs) identifying which edges to draw.
+            The default is None, in which case all edges are drawn.
+        color : :class:`compas.colors.Color` | dict[tuple[hashable, hashable], :class:`compas.colors.Color`], optional
+            The color specification for the edges.
+        collection : str, optional
+            The name of the Blender scene collection containing the created object(s).
 
         Returns
         -------
-        None
-
-        Examples
-        --------
-        >>> from compas.geometry import Frame
-        >>> from compas.geometry import Transformation
-        >>> from compas.geometry import Torus
-        >>> torus = Torus(Frame.worldXY(), 5, 2)
-        >>> frame = Frame([1, 1, 1], [0.68, 0.68, 0.27], [-0.67, 0.73, -0.15])
-        >>> T = Transformation.from_frame(frame)
-        >>> torus.transform(T)
+        list[:blender:`bpy.types.Object`]
 
         """
-        self.frame.transform(transformation)
+        objects = []
+
+        self.edgecolor = color
+
+        for u, v in edges or self.graph.edges():  # type: ignore
+            name = f"{self.graph.name}.edge.{u}-{v}"  # type: ignore
+            color = self.edgecolor[u, v]  # type: ignore
+            curve = conversions.line_to_blender_curve(Line(self.graph.nodes_attributes("xyz")[u], self.graph.nodes_attributes("xyz")[v]))
+
+            obj = self.create_object(curve, name=name)
+            self.update_object(obj, color=color, collection=collection)
+            objects.append(obj)
+
+        return objects
+
+    # =============================================================================
+    # draw labels
+    # =============================================================================
+
+    # def draw_nodelabels(self, text: Optional[Dict[int, str]] = None) -> List[bpy.types.Object]:
+    #     """Draw labels for a selection nodes.
+
+    #     Parameters
+    #     ----------
+    #     text : dict[hashable, str], optional
+    #         A dictionary of vertex labels as vertex-text pairs.
+    #         The default value is None, in which case every vertex will be labeled with its key.
+
+    #     Returns
+    #     -------
+    #     list[:blender:`bpy.types.Object`]
+
+    #     """
+    #     self.node_text = text
+    #     labels = []
+    #     for node in self.node_text:
+    #         labels.append(
+    #             {
+    #                 "pos": self.graph.nodes_attributes("xyz")[node],
+    #                 "name": f"{self.graph.name}.nodelabel.{node}",
+    #                 "text": self.node_text[node],
+    #                 "color": self.nodecolor[node],
+    #             }
+    #         )
+    #     return compas_blender.draw_texts(labels, collection=self.nodelabelcollection)
+
+    # def draw_edgelabels(self, text: Optional[Dict[Tuple[int, int], str]] = None) -> List[bpy.types.Object]:
+    #     """Draw labels for a selection of edges.
+
+    #     Parameters
+    #     ----------
+    #     text : dict[tuple[hashable, hashable], str], optional
+    #         A dictionary of edge labels as edge-text pairs.
+    #         The default value is None, in which case every edge will be labeled with its key.
+
+    #     Returns
+    #     -------
+    #     list[:blender:`bpy.types.Object`]
+
+    #     """
+    #     self.edge_text = text
+    #     labels = []
+    #     for edge in self.edge_text:
+    #         u, v = edge
+    #         labels.append(
+    #             {
+    #                 "pos": centroid_points([self.graph.nodes_attributes("xyz")[u], self.graph.nodes_attributes("xyz")[v]]),
+    #                 "name": f"{self.graph.name}.edgelabel.{u}-{v}",
+    #                 "text": self.edge_text[edge],
+    #                 "color": self.edgecolor[edge],
+    #             }
+    #         )
+    #     return compas_blender.draw_texts(labels, collection=self.edgelabelcollection)
+
+    # =============================================================================
+    # draw miscellaneous
+    # =============================================================================
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/shear.py` & `compas-2.1.1/src/compas/geometry/shear.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     * http://code.activestate.com/recipes/578108-determinant-of-matrix-of-any-order/
     * http://blog.acipo.com/matrix-inversion-in-javascript/
 
 Many thanks to Christoph Gohlke, Martin John Baker, Sachin Joglekar and Andrew
 Ippoliti for providing code and documentation.
 """
 
-from compas.utilities import flatten
-from compas.geometry import allclose
-from compas.geometry import matrix_from_shear_entries
-from compas.geometry import matrix_from_shear
-from compas.geometry import decompose_matrix
 from compas.geometry import Transformation
+from compas.geometry import decompose_matrix
+from compas.geometry import matrix_from_shear
+from compas.geometry import matrix_from_shear_entries
+from compas.itertools import flatten
+from compas.tolerance import TOL
 
 
 class Shear(Transformation):
     """Class representing a shear transformation.
 
     A point P is transformed by the shear matrix into P" such that
     the vector P-P" is parallel to the direction vector and its extent is
@@ -46,15 +46,15 @@
     >>>
 
     """
 
     def __init__(self, matrix=None, check=False, name=None):
         if matrix and check:
             _, shear, _, _, _ = decompose_matrix(matrix)
-            if not allclose(flatten(matrix), flatten(matrix_from_shear_entries(shear))):
+            if not TOL.is_allclose(flatten(matrix), flatten(matrix_from_shear_entries(shear))):
                 raise ValueError("This is not a proper shear matrix.")
         super(Shear, self).__init__(matrix=matrix, name=name)
 
     @classmethod
     def from_angle_direction_plane(cls, angle, direction, plane):
         """Construct a shear transformation from an angle, direction and plane.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/surfaces/conical.py` & `compas-2.1.1/src/compas/geometry/surfaces/conical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from math import pi, cos, sin
+from math import cos
+from math import pi
+from math import sin
 
-from compas.geometry import Point
 from compas.geometry import Frame
+from compas.geometry import Point
+
 from .surface import Surface
 
 PI2 = 2 * pi
 
 
 class ConicalSurface(Surface):
     """A cylindrical surface is defined by a radius and a local coordinate system.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/surfaces/cylindrical.py` & `compas-2.1.1/src/compas/geometry/surfaces/cylindrical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from math import pi, cos, sin
+from math import cos
+from math import pi
+from math import sin
 
+from compas.geometry import Circle
+from compas.geometry import Frame
 from compas.geometry import Point
 from compas.geometry import Vector
-from compas.geometry import Frame
-from compas.geometry import Circle
+
 from .surface import Surface
 
 PI2 = 2 * pi
 
 
 class CylindricalSurface(Surface):
     """A cylindrical surface is defined by a radius and a local coordinate system.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/surfaces/nurbs.py` & `compas-2.1.1/src/compas/geometry/surfaces/nurbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.plugins import pluggable
-from compas.plugins import PluginNotInstalledError
 from compas.geometry import Point
-from compas.utilities import linspace
-from compas.utilities import meshgrid
+from compas.itertools import linspace
+from compas.itertools import meshgrid
+from compas.plugins import PluginNotInstalledError
+from compas.plugins import pluggable
 
 from .surface import Surface
 
 
 @pluggable(category="factories")
 def new_nurbssurface(cls, *args, **kwargs):
     raise PluginNotInstalledError
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/surfaces/planar.py` & `compas-2.1.1/src/compas/geometry/surfaces/planar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-from compas.geometry import Point
-from compas.geometry import Vector
 from compas.geometry import Frame
 from compas.geometry import Plane
+from compas.geometry import Point
+from compas.geometry import Vector
+
 from .surface import Surface
 
 
 class PlanarSurface(Surface):
     """A planar surface is defined by a local coordinate system and a size.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/surfaces/spherical.py` & `compas-2.1.1/src/compas/geometry/surfaces/spherical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from math import cos, sin, pi
+from math import cos
+from math import pi
+from math import sin
 
+from compas.geometry import Circle
+from compas.geometry import Frame
 from compas.geometry import Point
 from compas.geometry import Vector
-from compas.geometry import Frame
-from compas.geometry import Circle
+
 from .surface import Surface
 
 PI2 = 2 * pi
 
 
 class SphericalSurface(Surface):
     """A spherical surface is defined by a radius and a frame.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/surfaces/surface.py` & `compas-2.1.1/src/compas/geometry/surfaces/surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from itertools import product
 
-from compas.geometry import Geometry
 from compas.geometry import Frame
-from compas.geometry import Transformation
+from compas.geometry import Geometry
 from compas.geometry import Point
+from compas.geometry import Transformation
+from compas.itertools import linspace
 from compas.plugins import pluggable
-from compas.utilities import linspace
 
 
 @pluggable(category="factories")
 def new_surface(cls, *args, **kwargs):
     surface = object.__new__(cls)
     surface.__init__(*args, **kwargs)
     return surface
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/surfaces/toroidal.py` & `compas-2.1.1/src/compas/geometry/surfaces/toroidal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from math import cos, sin, pi
+from math import cos
+from math import pi
+from math import sin
 
-from compas.geometry import Point
 from compas.geometry import Frame
+from compas.geometry import Point
+
 from .surface import Surface
 
 PI2 = 2 * pi
 
 
 class ToroidalSurface(Surface):
     """A spherical surface is defined by a radius and a frame.
@@ -83,19 +86,15 @@
     def __eq__(self, other):
         try:
             other_frame = other.frame
             other_radius_axis = other.radius_axis
             other_radius_pipe = other.radius_pipe
         except Exception:
             return False
-        return (
-            self.radius_axis == other_radius_axis
-            and self.radius_pipe == other_radius_pipe
-            and self.frame == other_frame
-        )
+        return self.radius_axis == other_radius_axis and self.radius_pipe == other_radius_pipe and self.frame == other_frame
 
     # =============================================================================
     # Properties
     # =============================================================================
 
     @property
     def center(self):
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/transformation.py` & `compas-2.1.1/src/compas/geometry/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,28 +8,26 @@
     * http://blog.acipo.com/matrix-inversion-in-javascript/
 
 Many thanks to Christoph Gohlke, Martin John Baker, Sachin Joglekar and Andrew
 Ippoliti for providing code and documentation.
 """
 
 from compas.data import Data
-
-from compas.tolerance import TOL
-
-from compas.geometry import multiply_matrices
-from compas.geometry import transpose_matrix
 from compas.geometry import basis_vectors_from_matrix
 from compas.geometry import decompose_matrix
 from compas.geometry import identity_matrix
 from compas.geometry import matrix_determinant
 from compas.geometry import matrix_from_euler_angles
 from compas.geometry import matrix_from_frame
 from compas.geometry import matrix_from_translation
 from compas.geometry import matrix_inverse
+from compas.geometry import multiply_matrices
 from compas.geometry import translation_from_matrix
+from compas.geometry import transpose_matrix
+from compas.tolerance import TOL
 
 
 class Transformation(Data):
     """Class representing a general 4x4 transformation matrix.
 
     It is the base class for transformations like :class:`Rotation`,
     :class:`Translation`, :class:`Scale`, :class:`Reflection`,
@@ -494,19 +492,19 @@
         True
         >>> R1 == R
         True
         >>> T1 == T
         True
 
         """
+        from compas.geometry import Projection
+        from compas.geometry import Rotation  # noqa: F811
         from compas.geometry import Scale  # noqa: F811
         from compas.geometry import Shear
-        from compas.geometry import Rotation  # noqa: F811
         from compas.geometry import Translation  # noqa: F811
-        from compas.geometry import Projection
 
         s, h, a, t, p = decompose_matrix(self.matrix)
         S = Scale.from_factors(s)
         H = Shear.from_entries(h)
         R = Rotation.from_euler_angles(a, static=True, axes="xyz")
         T = Translation.from_vector(t)
         P = Projection.from_entries(p)
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/translation.py` & `compas-2.1.1/src/compas/geometry/translation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     * http://code.activestate.com/recipes/578108-determinant-of-matrix-of-any-order/
     * http://blog.acipo.com/matrix-inversion-in-javascript/
 
 Many thanks to Christoph Gohlke, Martin John Baker, Sachin Joglekar and Andrew
 Ippoliti for providing code and documentation.
 """
 
-from compas.utilities import flatten
-from compas.geometry import allclose
+from compas.geometry import Transformation
 from compas.geometry import matrix_from_translation
 from compas.geometry import translation_from_matrix
-from compas.geometry import Transformation
+from compas.itertools import flatten
+from compas.tolerance import TOL
 
 
 class Translation(Transformation):
     """Class representing a translation transformation.
 
     Parameters
     ----------
@@ -68,15 +68,15 @@
     True
 
     """
 
     def __init__(self, matrix=None, check=False, name=None):
         if matrix and check:
             translation = translation_from_matrix(matrix)
-            if not allclose(flatten(matrix), flatten(matrix_from_translation(translation))):
+            if not TOL.is_allclose(flatten(matrix), flatten(matrix_from_translation(translation))):
                 raise ValueError("This is not a proper translation matrix.")
         super(Translation, self).__init__(matrix=matrix, name=name)
 
     @property
     def translation_vector(self):
         from compas.geometry import Vector
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/triangulation_delaunay.py` & `compas-2.1.1/src/compas/geometry/triangulation_delaunay.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from compas.plugins import pluggable
 
 
 @pluggable(category="triangulation")
 def delaunay_triangulation(points):
     """Construct a Delaunay triangulation of set of vertices.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/triangulation_earclip.py` & `compas-2.1.1/src/compas/geometry/triangulation_earclip.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,15 @@
         Returns
         -------
         bool
             True if the Ear triangle is valid, False otherwise.
 
         """
 
-        not_ear_points = [
-            points[i] for i in indexes if points[i] != self.coords and points[i] not in self.neighbour_coords
-        ]
+        not_ear_points = [points[i] for i in indexes if points[i] != self.coords and points[i] not in self.neighbour_coords]
         insides = [self.is_inside(p) for p in not_ear_points]
         if self.is_convex() and True not in insides:
             for e in ears:
                 if e.is_ear_point(self.coords):
                     return False
             return True
         return False
@@ -270,15 +268,17 @@
         If no ears were found for triangulation.
     IndexError
         If no more ears were found for triangulation.
 
     """
 
     # Orient the copy of polygon points to XY plane.
-    from compas.geometry import Plane, Frame, Transformation  # Avoid circular import.
+    from compas.geometry import Frame  # Avoid circular import.
+    from compas.geometry import Plane  # Avoid circular import.
+    from compas.geometry import Transformation  # Avoid circular import.
 
     frame = Frame.from_plane(Plane(polygon.points[0], polygon.normal))
     xform = Transformation.from_frame_to_frame(frame, Frame.worldXY())
     points = [point.transformed(xform) for point in polygon.points]
 
     # Check polygon winding by signed area of all current and next points pairs.
     sum_val = 0.0
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_curvature.py` & `compas-2.1.1/src/compas/geometry/trimesh_curvature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from math import pi
-from compas.plugins import pluggable
+
 from compas.geometry import angle_points
-from compas.utilities import window
+from compas.itertools import window
+from compas.plugins import pluggable
 
 
 @pluggable(category="trimesh")
 def trimesh_gaussian_curvature(M):
     r"""Compute the discrete gaussian curvature of a triangle mesh.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_descent_numpy.py` & `compas-2.1.1/src/compas/geometry/trimesh_descent_numpy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from numpy import asarray
+
 from .trimesh_gradient_numpy import trimesh_gradient_numpy
 
 
 def trimesh_descent_numpy(M):
     """Compute the descent directions of a triangular mesh as the gradient of the vertex heights.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_geodistance.py` & `compas-2.1.1/src/compas/geometry/trimesh_parametrisation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,55 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.plugins import pluggable
 
 
 @pluggable(category="trimesh")
-def trimesh_geodistance(M, source, method="exact"):
-    """Compute the geodesic distance from every vertex of the mesh to a source vertex.
+def trimesh_harmonic(M):
+    """Compute the harmonic parametrisation of a triangle mesh within a fixed circular boundary.
 
     Parameters
     ----------
     M : tuple[sequence[[float, float, float] | :class:`compas.geometry.Point`], sequence[[int, int, int]]]
         A mesh represented by a list of vertices and a list of faces.
-    source : int
-        The index of the vertex from where the geodesic distances should be calculated.
-    method : Literal['exact', 'heat'], optional
-        The method for calculating the distances.
 
     Returns
     -------
-    list[float]
-        A list of geodesic distances from the source vertex.
-
-    Raises
-    ------
-    NotImplementedError
-        If `method` is not one of ``{'exact', 'heat'}``.
+    list[[int, int]]
+        The u, v parameters per vertex.
 
     Examples
     --------
     >>>
 
     """
-    from .trimesh_geodistance_numpy import trimesh_geodesic_distances_numpy
+    raise NotImplementedError
+
+
+trimesh_harmonic.__pluggable__ = True
+
+
+@pluggable(category="trimesh")
+def trimesh_lscm(M):
+    """Compute the least squares conformal map of a triangle mesh.
+
+    Parameters
+    ----------
+    M : tuple[sequence[[float, float, float] | :class:`compas.geometry.Point`], sequence[[int, int, int]]]
+        A mesh represented by a list of vertices and a list of faces.
+
+    Returns
+    -------
+    list[[int, int]]
+        The u, v parameters per vertex.
 
-    if method == "exact":
-        raise NotImplementedError
+    Examples
+    --------
+    >>>
 
-    return trimesh_geodesic_distances_numpy(M, [source])
+    """
+    raise NotImplementedError
 
 
-trimesh_geodistance.__pluggable__ = True
+trimesh_lscm.__pluggable__ = True
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_gradient_numpy.py` & `compas-2.1.1/src/compas/geometry/trimesh_gradient_numpy.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from scipy.sparse import coo_matrix  # type: ignore
 
-from compas.linalg import normrow
 from compas.linalg import normalizerow
+from compas.linalg import normrow
 from compas.linalg import rot90
 
 
 def trimesh_gradient_numpy(M, rtype="array"):
     """Construct the gradient operator of a trianglular mesh.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_isolines.py` & `compas-2.1.1/src/compas/geometry/trimesh_isolines.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.plugins import pluggable
 
 
 @pluggable(category="trimesh")
 def trimesh_isolines(M, S, N=50):
     """Compute isolines on a triangle mesh using a scalarfield of data points
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_matrices.py` & `compas-2.1.1/src/compas/geometry/trimesh_matrices.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.plugins import pluggable
 
 
 @pluggable(category="trimesh")
 def trimesh_massmatrix(M):
     """Compute massmatrix on a triangle mesh using a scalarfield of data points
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_matrices_numpy.py` & `compas-2.1.1/src/compas/geometry/trimesh_matrices_numpy.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from numpy import asarray
-from numpy import zeros
-from numpy import cross
 from numpy import bincount
+from numpy import cross
+from numpy import zeros
 from scipy.sparse import coo_matrix
 from scipy.sparse import spdiags
 
+from compas.geometry import cross_vectors
 from compas.geometry import dot_vectors
 from compas.geometry import length_vector
-from compas.geometry import cross_vectors
 from compas.linalg import normrow
 
 
 def trimesh_edge_cotangent(mesh, edge):
     """Compute the cotangent of the angle opposite a halfedge of the triangle mesh.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_pull_points_numpy.py` & `compas-2.1.1/src/compas/geometry/trimesh_pull_points_numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,15 @@
 # ==============================================================================
 # helpers
 # ==============================================================================
 
 
 def _is_point_in_edgezone(p, p0, p1):
     n = cross_vectors(p1 - p0, [0, 0, 1.0])
-    return (
-        is_ccw_xy(p0 - p0, n, p - p0) and not is_ccw_xy(p0 - p0, p1 - p0, p - p0) and not is_ccw_xy(p1 - p1, n, p - p1)
-    )
+    return is_ccw_xy(p0 - p0, n, p - p0) and not is_ccw_xy(p0 - p0, p1 - p0, p - p0) and not is_ccw_xy(p1 - p1, n, p - p1)
 
 
 def _compute_point_on_segment(p, p0, p1):
     a = p1[1] - p0[1]
     b = p0[0] - p1[0]
     c = p1[0] * p0[1] - p1[1] * p0[0]
     r = (b * (b * p[0] - a * p[1]) - a * c) / (a**2 + b**2)
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_remeshing.py` & `compas-2.1.1/src/compas/geometry/trimesh_remeshing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import print_function
-from __future__ import absolute_import
-from __future__ import division
-
 from compas.plugins import pluggable
 
 
 @pluggable(category="trimesh")
 def trimesh_remesh(mesh, target_edge_length, number_of_iterations=10, do_project=True):
     """Remeshing of a triangle mesh.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_samplepoints_numpy.py` & `compas-2.1.1/src/compas/geometry/trimesh_samplepoints_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from numpy import array
-from numpy.random import choice
-from numpy.random import rand
-from numpy import sqrt
-from numpy import float64
-from numpy import cross
-from numpy.linalg import norm
 from numpy import clip
+from numpy import cross
 from numpy import finfo
+from numpy import float64
+from numpy import sqrt
+from numpy.linalg import norm
+from numpy.random import choice
+from numpy.random import rand
 
 
 def trimesh_samplepoints_numpy(M, num_points=1000, return_normals=False):
     """Compute sample points on a triangle mesh surface.
 
     Parameters
     ----------
@@ -33,26 +33,26 @@
     .. [2] Efficient barycentric point sampling on meshes, arXiv:1708.07559
 
     Examples
     --------
     Make a triangle mesh.
 
     >>> from compas.datastructures import Mesh
-    >>> hypar = Mesh.from_obj(compas.get('hypar.obj'))
+    >>> hypar = Mesh.from_obj(compas.get("hypar.obj"))
     >>> hypar.is_trimesh()
     False
     >>> hypar.quads_to_triangles()
 
     Compute sample points.
 
     >>> samples_pts, pts_normals = trimesh_samplepoints_numpy(hypar.to_vertices_and_faces(), 1000, True)
     >>> # the x,y,z of sample points would be the following
-    >>> x, y, z = samples_pts[:,0], samples_pts[:,1], samples_pts[:,2]
+    >>> x, y, z = samples_pts[:, 0], samples_pts[:, 1], samples_pts[:, 2]
     >>> # the sample points added normal vector would be the following
-    >>> X, Y, Z = x + pts_normals[:,0] , y + pts_normals[:,1] , z + pts_normals[:,2]
+    >>> X, Y, Z = x + pts_normals[:, 0], y + pts_normals[:, 1], z + pts_normals[:, 2]
 
     """
     # if mesh.is_empty():
     #     raise ValueError("Mesh is empty.")
     # if not mesh.is_trimesh():
     #     raise ValueError("Mesh is not trimesh.")
     # if not mesh.is_valid():
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_slicing.py` & `compas-2.1.1/src/compas/geometry/trimesh_slicing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.plugins import pluggable
 
 
 @pluggable(category="trimesh")
 def trimesh_slice(mesh, planes):
     """Slice a mesh by a list of planes.
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/trimesh_smoothing_numpy.py` & `compas-2.1.1/src/compas/geometry/trimesh_smoothing_numpy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from numpy import array
 
-from ._algebra import trimesh_cotangent_laplacian_matrix
+from .trimesh_matrices_numpy import trimesh_cotangent_laplacian_matrix
 
 
 def trimesh_smooth_laplacian_cotangent(trimesh, fixed, kmax=10):
     """Smooth a triangle mesh using a laplacian matrix with cotangent weights.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/geometry/vector.py` & `compas-2.1.1/src/compas/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/itertools.py` & `compas-2.1.1/src/compas/itertools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # recipes with itertools
 # see: https://docs.python.org/3.6/library/itertools.html
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from itertools import islice
+from functools import reduce
 from itertools import chain
+from itertools import islice
 from itertools import repeat
 from itertools import tee
-from functools import reduce
 from operator import mul
 
 try:
     from itertools import zip_longest
 except ImportError:
     from itertools import izip_longest as zip_longest
 
@@ -119,25 +119,25 @@
     This function mimicks the functionality of ``numpy.meshgrid`` [1]_, but in a simpler form.
 
     .. [1] `numpy.meshgrid`.
            Available at https://numpy.org/doc/stable/reference/generated/numpy.meshgrid.html
 
     Examples
     --------
-    >>> from compas.utilities import linspace, meshgrid
+    >>> from compas.itertools import linspace, meshgrid
     >>> x = list(linspace(0, 1, 3))
     >>> y = list(linspace(0, 1, 2))
 
     >>> X, Y = meshgrid(x, y)
     >>> X
     [[0.0, 0.5, 1.0], [0.0, 0.5, 1.0]]
     >>> Y
     [[0.0, 0.0, 0.0], [1.0, 1.0, 1.0]]
 
-    >>> X, Y = meshgrid(x, y, 'ij')
+    >>> X, Y = meshgrid(x, y, "ij")
     >>> X
     [[0.0, 0.0], [0.5, 0.5], [1.0, 1.0]]
     >>> Y
     [[0.0, 1.0], [0.0, 1.0], [0.0, 1.0]]
 
     """
     x = list(x)
@@ -177,15 +177,15 @@
     ----------
     This function mimicks the functionality of ``numpy.linspace`` [1]_, but in a simpler form.
 
     .. [1] ``numpy.linspace`` Available at https://numpy.org/doc/stable/reference/generated/numpy.linspace.html
 
     Examples
     --------
-    >>> from compas.utilities import linspace
+    >>> from compas.itertools import linspace
     >>> list(linspace(0, 1, 3))
     [0.0, 0.5, 1.0]
 
     """
     if num < 2:
         raise ValueError("ValueError: number of elements must be at least 2, got {:d}".format(num))
 
@@ -272,15 +272,14 @@
     tuple
         Two items per iteration, if there are at least two items in the iterable.
 
     Examples
     --------
     >>> for a, b in pairwise(range(5)):
     ...     print(a, b)
-    ...
     0 1
     1 2
     2 3
     3 4
 
     """
     a, b = tee(iterable)
@@ -304,15 +303,14 @@
         A tuple of size `n` at every iteration,
         if there are at least `n` items in the sequence.
 
     Examples
     --------
     >>> for view in window(range(10), 3):
     ...     print(view)
-    ...
     (0, 1, 2)
     (1, 2, 3)
     (2, 3, 4)
     (3, 4, 5)
     (4, 5, 6)
     (5, 6, 7)
     (6, 7, 8)
```

### Comparing `COMPAS-2.1.0/src/compas/linalg.py` & `compas-2.1.1/src/compas/linalg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import sys
 from functools import wraps
+
+from numpy import absolute
 from numpy import array
 from numpy import asarray
 from numpy import atleast_2d
+from numpy import cross
 from numpy import nan_to_num
 from numpy import nonzero
 from numpy import sum
-from numpy import absolute
-from numpy import cross
 from numpy.linalg import cond
 from scipy.linalg import cho_factor  # type: ignore
 from scipy.linalg import cho_solve  # type: ignore
 from scipy.linalg import lstsq  # type: ignore
 from scipy.linalg import qr  # type: ignore
 from scipy.linalg import svd  # type: ignore
 from scipy.sparse.linalg import factorized  # type: ignore
 from scipy.sparse.linalg import spsolve  # type: ignore
 
-
 # ==============================================================================
 # Fundamentals
 # ==============================================================================
 
 
 def nullspace(A, tol=0.001):
     r"""Calculates the nullspace of the input matrix A.
@@ -401,15 +401,15 @@
         Vectors of co-ordinate differences in x, y and z (m x 3).
     array
         Lengths of members (m x 1).
 
     Examples
     --------
     >>> from compas.matrices import connectivity_matrix
-    >>> C = connectivity_matrix([[0, 1], [1, 2]], 'csr')
+    >>> C = connectivity_matrix([[0, 1], [1, 2]], "csr")
     >>> X = array([[0, 0, 0], [1, 1, 0], [0, 0, 1]])
     >>> uvw_lengths(C, X)
     (array([[ 1.,  1.,  0.],
            [-1., -1.,  1.]]), array([[1.41421356],
            [1.73205081]]))
 
     """
@@ -434,15 +434,27 @@
     -----
     The calculation is the Euclidean 2-norm, i.e. the square root of the sum
     of the squares of the elements in each row, this equates to the "length" of
     the m row vectors.
 
     Examples
     --------
-    >>> normrow(array([[2, -1, 3,], [1, 0, 1], [0, 2, -1]]))
+    >>> normrow(
+    ...     array(
+    ...         [
+    ...             [
+    ...                 2,
+    ...                 -1,
+    ...                 3,
+    ...             ],
+    ...             [1, 0, 1],
+    ...             [0, 2, -1],
+    ...         ]
+    ...     )
+    ... )
     array([[3.74165739],
            [1.41421356],
            [2.23606798]])
 
     """
     A = atleast_2d(asarray(A, dtype=float))
     return (sum(A**2, axis=1) ** 0.5).reshape((-1, 1))
@@ -468,15 +480,27 @@
     Normalises the row vectors of A by the normrows, i.e. creates an array of
     vectors where the row vectors have length of unity.
 
     Tiling is not necessary, because of NumPy's broadcasting behaviour.
 
     Examples
     --------
-    >>> normalizerow(array([[2, -1, 3,], [1, 0, 1], [0, 2, -1]]))
+    >>> normalizerow(
+    ...     array(
+    ...         [
+    ...             [
+    ...                 2,
+    ...                 -1,
+    ...                 3,
+    ...             ],
+    ...             [1, 0, 1],
+    ...             [0, 2, -1],
+    ...         ]
+    ...     )
+    ... )
     array([[ 0.53452248, -0.26726124,  0.80178373],
            [ 0.70710678,  0.        ,  0.70710678],
            [ 0.        ,  0.89442719, -0.4472136 ]])
 
     """
     if do_nan_to_num:
         return nan_to_num(A / normrow(A))
```

### Comparing `COMPAS-2.1.0/src/compas/matrices.py` & `compas-2.1.1/src/compas/matrices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from numpy import abs
 from numpy import array
 from numpy import asarray
 from numpy import tile
-
 from scipy.sparse import coo_matrix  # type: ignore
 from scipy.sparse import csr_matrix  # type: ignore
 from scipy.sparse import diags  # type: ignore
 from scipy.sparse import vstack as svstack  # type: ignore
 
 
 def _return_matrix(M, rtype):
@@ -137,15 +136,15 @@
         }
 
     A connectivity matrix is generally sparse and will perform superior
     in numerical calculations as a sparse matrix.
 
     Examples
     --------
-    >>> connectivity_matrix([[0, 1], [0, 2], [0, 3]], rtype='array')
+    >>> connectivity_matrix([[0, 1], [0, 2], [0, 3]], rtype="array")
     array([[-1.,  1.,  0.,  0.],
            [-1.,  0.,  1.,  0.],
            [-1.,  0.,  0.,  1.]])
 
     """
     m = len(edges)
     data = array([-1] * m + [1] * m)
@@ -185,15 +184,15 @@
 
         \mathbf{L} = \mathbf{C} ^ \mathrm{T} \mathbf{C}
 
     The current implementation only supports umbrella weights.
 
     Examples
     --------
-    >>> laplacian_matrix([[0, 1], [0, 2], [0, 3]], rtype='array')
+    >>> laplacian_matrix([[0, 1], [0, 2], [0, 3]], rtype="array")
     array([[ 3., -1., -1., -1.],
            [-1.,  1.,  0.,  0.],
            [-1.,  0.,  1.,  0.],
            [-1.,  0.,  0.,  1.]])
 
     """
     C = connectivity_matrix(edges, rtype="csr")
@@ -249,15 +248,15 @@
     The matrix of vertex coordinates is vectorised to speed up the
     calculations.
 
     Examples
     --------
     >>> C = connectivity_matrix([[0, 1], [0, 2], [0, 3]])
     >>> xyz = [[0, 0, 1], [0, 1, 0], [-1, -1, 0], [1, -1, 0]]
-    >>> equilibrium_matrix(C, xyz, [0], rtype='array')
+    >>> equilibrium_matrix(C, xyz, [0], rtype="array")
     array([[ 0.,  1., -1.],
            [-1.,  1.,  1.]])
 
     """
     xyz = asarray(xyz, dtype=float)
     C = csr_matrix(C)
     xy = xyz[:, :2]
```

### Comparing `COMPAS-2.1.0/src/compas/plugins.py` & `compas-2.1.1/src/compas/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,19 +146,15 @@
 
         """
         # Since we modify global state,
         # let's lock around this.
         with self._discovery_lock:
             count = 0
 
-            modules = [
-                module_name
-                for _importer, module_name, is_pkg in pkgutil.iter_modules()
-                if is_pkg and module_name.startswith("compas")
-            ]
+            modules = [module_name for _importer, module_name, is_pkg in pkgutil.iter_modules() if is_pkg and module_name.startswith("compas")]
 
             modules_to_inspect = dict()
 
             for module_name in modules:
                 module = self.importer.try_import(module_name)
                 if module:
                     modules_to_inspect[module_name] = module
@@ -209,19 +205,15 @@
             if plugin_opts is not None:
                 plugin_impl = PluginImpl(plugin_module, plugin_method, plugin_opts)
                 plugins_list = self._registry.setdefault(plugin_opts["extension_point_url"], [])
                 plugins_list.append(plugin_impl)
                 plugins_list.sort(key=lambda p: p.key)
 
                 if self.DEBUG:
-                    print(
-                        'Registered plugin with ID "{}" for extension point: {}'.format(
-                            plugin_impl.id, plugin_opts["extension_point_url"]
-                        )
-                    )
+                    print('Registered plugin with ID "{}" for extension point: {}'.format(plugin_impl.id, plugin_opts["extension_point_url"]))
                 count += 1
 
         return count
 
     def _parse_plugin_opts(self, plugin_method):
         if not inspect.isroutine(plugin_method):
             return
@@ -264,17 +256,17 @@
     domain : str, optional
         Domain name that "owns" the pluggable extension point.
         This is useful to avoid name collisions between extension points
         of different packages.
 
     Examples
     --------
-    >>> @pluggable(category='triangulation')
+    >>> @pluggable(category="triangulation")
     ... def triangulate_mesh(mesh):
-    ...    pass
+    ...     pass
 
     """
 
     def pluggable_decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             extension_point_url = _get_extension_point_url_from_method(domain, category, func)
@@ -282,24 +274,18 @@
             # Select first matching plugin
             if selector == "first_match":
                 plugin_impl = _select_plugin(extension_point_url)
                 if plugin_impl is None:
                     try:
                         return func(*args, **kwargs)
                     except NotImplementedError:
-                        raise PluginNotInstalledError(
-                            "Plugin not found and no default implementation for extension point URL: {}".format(
-                                extension_point_url
-                            )
-                        )
+                        raise PluginNotInstalledError("Plugin not found and no default implementation for extension point URL: {}".format(extension_point_url))
                     except ImportError:
                         raise PluginDefaultNotAvailableError(
-                            "Plugin not found and the default implementation is not available in your environment for extension point URL: {}".format(
-                                extension_point_url
-                            )
+                            "Plugin not found and the default implementation is not available in your environment for extension point URL: {}".format(extension_point_url)
                         )
 
                 # Invoke plugin
                 return plugin_impl.method(*args, **kwargs)
 
             # Collect all matching plugins
             elif selector == "collect_all":
```

### Comparing `COMPAS-2.1.0/src/compas/rpc/__main__.py` & `compas-2.1.1/src/compas/rpc/__main__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/rpc/dispatcher.py` & `compas-2.1.1/src/compas/rpc/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,18 +118,15 @@
             except AttributeError:
                 odict["error"] = "This function is not part of the API: {0}".format(functionname)
 
             else:
                 try:
                     idict = json.loads(args[0], cls=DataDecoder)
                 except (IndexError, TypeError):
-                    odict["error"] = (
-                        "API methods require a single JSON encoded dictionary as input.\n"
-                        "For example: input = json.dumps({'param_1': 1, 'param_2': [2, 3]})"
-                    )
+                    odict["error"] = "API methods require a single JSON encoded dictionary as input.\n" "For example: input = json.dumps({'param_1': 1, 'param_2': [2, 3]})"
 
                 else:
                     self._call(function, idict, odict)
 
         return json.dumps(odict, cls=DataEncoder)
 
     def _call(self, function, idict, odict):
```

### Comparing `COMPAS-2.1.0/src/compas/rpc/proxy.py` & `compas-2.1.1/src/compas/rpc/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from __future__ import print_function
 
 import json
 import time
 
 import compas
 import compas._os
-from compas.rpc import RPCServerError
 from compas.data import DataDecoder
 from compas.data import DataEncoder
+from compas.rpc import RPCServerError
 
 try:
     from xmlrpclib import ServerProxy
 except ImportError:
     from xmlrpc.client import ServerProxy
 
 try:
-    from subprocess import Popen
     from subprocess import PIPE
+    from subprocess import Popen
 except ImportError:
     from System.Diagnostics import Process
 
 
 class Proxy(object):
     """Create a proxy object as intermediary between client code and remote functionality.
 
@@ -91,18 +91,18 @@
     If possible, the proxy will try to reconnect to an already existing service
 
     Examples
     --------
     Minimal example showing connection to the proxy server, and ensuring the
     server is disposed after using it:
 
-    >>> from compas.rpc import Proxy                        # doctest: +SKIP
-    >>> with Proxy('compas.numerical') as numerical:        # doctest: +SKIP
-    ...     pass                                            # doctest: +SKIP
-    ...                                                     # doctest: +SKIP
+    >>> from compas.rpc import Proxy  # doctest: +SKIP
+    >>> with Proxy("compas.numerical") as numerical:  # doctest: +SKIP
+    ...     pass  # doctest: +SKIP
+    ...     # doctest: +SKIP
     Starting a new proxy server...                          # doctest: +SKIP
     New proxy server started.                               # doctest: +SKIP
     Stopping the server proxy.                              # doctest: +SKIP
     """
 
     def __init__(
         self,
@@ -280,17 +280,15 @@
                     self._process.StartInfo.EnvironmentVariables[name] = env[name]
                 else:
                     self._process.StartInfo.EnvironmentVariables.Add(name, env[name])
             self._process.StartInfo.UseShellExecute = False
             self._process.StartInfo.RedirectStandardOutput = self.capture_output
             self._process.StartInfo.RedirectStandardError = self.capture_output
             self._process.StartInfo.FileName = self.python
-            self._process.StartInfo.Arguments = "-m {0} --port {1} --{2}autoreload".format(
-                self.service, self._port, "" if self.autoreload else "no-"
-            )
+            self._process.StartInfo.Arguments = "-m {0} --port {1} --{2}autoreload".format(self.service, self._port, "" if self.autoreload else "no-")
             self._process.Start()
         else:
             args = [
                 self.python,
                 "-m",
                 self.service,
                 "--port",
@@ -394,17 +392,17 @@
         Returns
         -------
         object
             The 'data' part of the result dict returned by the remote function.
             The result dict has the following structure ::
 
                 {
-                    'error'   : ...,  # A traceback of the error raised on the server, if any.
-                    'profile' : ...,  # A profile of the code executed on the server, if there was no error.
-                    'data'    : ...,  # The result returned by the target function, if there was no error.
+                    "error": ...,  # A traceback of the error raised on the server, if any.
+                    "profile": ...,  # A profile of the code executed on the server, if there was no error.
+                    "data": ...,  # The result returned by the target function, if there was no error.
                 }
 
         Warnings
         --------
         The `args` and `kwargs` have to be JSON-serializable.
         This means that, currently, only COMPAS data objects (geometry, robots, data structures) and native Python objects are supported.
         The returned results will also always be in the form of COMPAS data objects and built-in Python objects.
```

### Comparing `COMPAS-2.1.0/src/compas/rpc/server.py` & `compas-2.1.1/src/compas/rpc/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import threading
 
 try:
     from SimpleXMLRPCServer import SimpleXMLRPCServer
 except ImportError:
     from xmlrpc.server import SimpleXMLRPCServer
@@ -28,16 +28,15 @@
         from compas.rpc import Dispatcher
 
 
         class DefaultService(Dispatcher):
             pass
 
 
-        if __name__ == '__main__':
-
+        if __name__ == "__main__":
             server = Server(("localhost", 8888))
 
             server.register_function(server.ping)
             server.register_function(server.remote_shutdown)
             server.register_instance(DefaultService())
             server.serve_forever()
```

### Comparing `COMPAS-2.1.0/src/compas/rpc/services/default.py` & `compas-2.1.1/src/compas/rpc/services/default.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """This script starts a XMLRPC server and registers the default service.
 
 The server binds to all network interfaces (i.e. ``0.0.0.0``) and
 it listens to requests on port ``1753``.
 
 """
 
-from compas.rpc import Server
 from compas.rpc import Dispatcher
+from compas.rpc import Server
 
 from .watcher import FileWatcherService
 
 
 class DefaultService(Dispatcher):
     def __init__(self):
         super(DefaultService, self).__init__()
```

### Comparing `COMPAS-2.1.0/src/compas/rpc/services/watcher.py` & `compas-2.1.1/src/compas/rpc/services/watcher.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/scene/__init__.py` & `compas-2.1.1/src/compas/scene/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 from .context import before_draw
 from .context import after_draw
 from .context import register_scene_objects
 from .context import get_sceneobject_cls
 from .context import register
 
 from .scene import Scene
-from .scene import SceneObjectNode
-from .scene import SceneTree
 
 from compas.plugins import plugin
 from compas.geometry import Geometry
 from compas.datastructures import Mesh
 from compas.datastructures import Graph
 from compas.datastructures import VolMesh
 
@@ -45,16 +43,14 @@
     "SceneObjectNotRegisteredError",
     "SceneObject",
     "MeshObject",
     "GraphObject",
     "GeometryObject",
     "VolMeshObject",
     "Scene",
-    "SceneObjectNode",
-    "SceneTree",
     "clear",
     "before_draw",
     "after_draw",
     "register_scene_objects",
     "get_sceneobject_cls",
     "register",
 ]
```

### Comparing `COMPAS-2.1.0/src/compas/scene/context.py` & `compas-2.1.1/src/compas/scene/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,43 +88,28 @@
     -------
     None
 
     """
     ITEM_SCENEOBJECT[context][item_type] = sceneobject_type
 
 
-def is_viewer_open():
-    """Returns True if an instance of the compas_view2 App is available.
-
-    Returns
-    -------
-    bool
-
-    """
-    from compas.scene import Scene
-
-    return Scene.viewerinstance is not None
-
-
 def detect_current_context():
     """Chooses an appropriate context depending on available contexts and open instances. with the following priority:
     1. Viewer
     2. Plotter
     3. Rhino / GH - checked explicitly since SceneObjects for both get registered when code is run from either.
     4. Other
 
     Returns
     -------
     str
         Name of an available context, used as key in :attr:`SceneObject.ITEM_SCENEOBJECT`
 
     """
 
-    if is_viewer_open():
-        return "Viewer"
     if compas.is_grasshopper():
         return "Grasshopper"
     if compas.is_rhino():
         return "Rhino"
     if compas.is_blender():
         return "Blender"
     other_contexts = [v for v in ITEM_SCENEOBJECT.keys()]
@@ -148,26 +133,22 @@
 
         for type_ in inspect.getmro(dtype):
             cls = context.get(type_, None)
             if cls is not None:
                 break
 
     if cls is None:
-        raise SceneObjectNotRegisteredError(
-            "No scene object is registered for this data type: {} in this context: {}".format(dtype, context_name)
-        )
+        raise SceneObjectNotRegisteredError("No scene object is registered for this data type: {} in this context: {}".format(dtype, context_name))
 
     return cls
 
 
 def get_sceneobject_cls(item, **kwargs):
     if not ITEM_SCENEOBJECT:
         register_scene_objects()
 
     if item is None:
-        raise ValueError(
-            "Cannot create a scene object for None. Please ensure you pass a instance of a supported class."
-        )
+        raise ValueError("Cannot create a scene object for None. Please ensure you pass a instance of a supported class.")
 
     cls = _get_sceneobject_cls(item, **kwargs)
     PluginValidator.ensure_implementations(cls)
     return cls
```

### Comparing `COMPAS-2.1.0/src/compas/scene/descriptors/attribute.py` & `compas-2.1.1/src/compas/scene/descriptors/attribute.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/scene/descriptors/color.py` & `compas-2.1.1/src/compas/scene/descriptors/color.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/scene/descriptors/colordict.py` & `compas-2.1.1/src/compas/scene/descriptors/colordict.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/scene/geometryobject.py` & `compas-2.1.1/src/compas/scene/geometryobject.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from .sceneobject import SceneObject
 from .descriptors.color import ColorAttribute
+from .sceneobject import SceneObject
 
 
 class GeometryObject(SceneObject):
     """Base class for scene objects for geometry objects.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/scene/graphobject.py` & `compas-2.1.1/src/compas/scene/graphobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.geometry import transform_points
-from .sceneobject import SceneObject
+
 from .descriptors.colordict import ColorDictAttribute
+from .sceneobject import SceneObject
 
 
 class GraphObject(SceneObject):
     """Scene object for drawing graph data structures.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/scene/meshobject.py` & `compas-2.1.1/src/compas/scene/meshobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.geometry import transform_points
-from .sceneobject import SceneObject
+
 from .descriptors.colordict import ColorDictAttribute
+from .sceneobject import SceneObject
 
 
 class MeshObject(SceneObject):
     """Base class for all mesh scene objects.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/scene/volmeshobject.py` & `compas-2.1.1/src/compas/scene/volmeshobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.geometry import transform_points
-from .sceneobject import SceneObject
+
 from .descriptors.colordict import ColorDictAttribute
+from .sceneobject import SceneObject
 
 
 class VolMeshObject(SceneObject):
     """Scene object for drawing volmesh data structures.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/tolerance.py` & `compas-2.1.1/src/compas/tolerance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 The tolerance module provides functionality to deal with tolerances consistently across all other COMPAS packages.
 """
 
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.data import Data
 from decimal import Decimal
 
 import compas
+from compas.data import Data
 
 __all__ = ["Tolerance", "TOL"]
 
 
 class Tolerance(Data):
     """Tolerance settings for geometric operations.
 
@@ -49,28 +49,41 @@
     -----
     The absolute tolerance is used to determine when a number is small enough to be considered zero.
     The relative tolerance determines the allowable deviation between two values for the values to be considered equal.
     The relative tolerance is defined as a fraction of one of the two values.
     This value is called the "true value".
     By convention, the second value is considered the "true value" by the comparison functions of this class.
 
+    The :class:`compas.tolerance.Tolerance` class is implemented using a "singleton" pattern and can therefore have only 1 (one) instance per context.
+    Usage of :attr:`compas.tolerance.TOL` outside of :mod:`compas` internals is therefore deprecated.
+
     Examples
     --------
     >>> tol = Tolerance()
     >>> tol.unit
     'M'
     >>> tol.absolute
     1e-09
     >>> tol.relative
     1e-06
     >>> tol.angular
     1e-06
 
     """
 
+    _instance = None
+    _is_inited = False
+
+    SUPPORTED_UNITS = ["M", "MM"]
+    """{"M", "MM"}: Default tolerances are defined in relation to length units.
+
+    Currently, only meters ("M") and millimeters ("MM") are supported.
+
+    """
+
     ABSOLUTE = 1e-9
     """float: Determines when a number is small enough to be considered zero.
     """
 
     RELATIVE = 1e-6
     """float: Determines the accuracy of comparing a "computed value" to a "true value", as a fraction of the "true value".
     """
@@ -90,97 +103,142 @@
     Positive numbers correspond to the number of digits after the decimal point.
     Negative numbers correspond to the number of digits before the decimal point.
     Zero precision is not allowed.
 
     """
 
     LINEARDEFLECTION = 1e-3
-    """float: The maximum distance between a curve or surface and its polygonal approximation.
+    """float: The maximum "distance" deviation between a curve or surface and its polygonal approximation.
+
+    This is used by the viewer to determine the mesh and polyline resolution of curves and surfaces for visualisation.
+
+    """
+
+    ANGULARDEFLECTION = 1e-1
+    """float: The maximum "curvature" deviation between a curve or surface and its polygonal approximation.
 
     This is used by the viewer to determine the mesh and polyline resolution of curves and surfaces for visualisation.
 
     """
 
     def __new__(cls, *args, **kwargs):
-        if not hasattr(cls, "_instance"):
-            cls._instance = super(Tolerance, cls).__new__(cls)
+        if not cls._instance:
+            cls._instance = object.__new__(cls, *args, **kwargs)
+            cls._is_inited = False
         return cls._instance
 
     @property
     def __data__(self):
         return {
             "unit": self.unit,
             "absolute": self.absolute,
             "relative": self.relative,
             "angular": self.angular,
             "approximation": self.approximation,
             "precision": self.precision,
             "lineardeflection": self.lineardeflection,
+            "angulardeflection": self.angulardeflection,
         }
 
     @classmethod
     def __from_data__(cls, data):
         tol = cls()
         tol.unit = data["unit"]
         tol.absolute = data["absolute"]
         tol.relative = data["relative"]
         tol.angular = data["angular"]
         tol.approximation = data["approximation"]
         tol.precision = data["precision"]
         tol.lineardeflection = data["lineardeflection"]
+        tol.angulardeflection = data["angulardeflection"]
         return tol
 
     def __init__(
         self,
         unit="M",
         absolute=None,
         relative=None,
         angular=None,
         approximation=None,
         precision=None,
         lineardflection=None,
+        angulardflection=None,
         name=None,
     ):
         super(Tolerance, self).__init__(name=name)
-        self._unit = None
-        self._absolute = None
-        self._relative = None
-        self._angular = None
-        self._approximation = None
-        self._precision = None
-        self._lineardeflection = None
-        self.unit = unit
-        self.absolute = absolute
-        self.relative = relative
-        self.angular = angular
-        self.approximation = approximation
-        self.precision = precision
-        self.lineardeflection = lineardflection
+        if not self._is_inited:
+            self._unit = None
+            self._absolute = None
+            self._relative = None
+            self._angular = None
+            self._approximation = None
+            self._precision = None
+            self._lineardeflection = None
+            self._angulardeflection = None
+
+        self._is_inited = True
+
+        if unit is not None:
+            self.unit = unit
+        if absolute is not None:
+            self.absolute = absolute
+        if relative is not None:
+            self.relative = relative
+        if angular is not None:
+            self.angular = angular
+        if approximation is not None:
+            self.approximation = approximation
+        if precision is not None:
+            self.precision = precision
+        if lineardflection is not None:
+            self.lineardeflection = lineardflection
+        if angulardflection is not None:
+            self.angulardeflection = angulardflection
 
     # this can be autogenerated if we use slots
     # __repr__: return f"{__class__.__name__}({', '.join(f'{k}={v!r}' for k, v in self.__dict__.items())})}"
+
     def __repr__(self):
-        return "Tolerance(unit='{}', absolute={}, relative={}, angular={}, approximation={}, precision={}, lineardeflection={})".format(
+        return "Tolerance(unit='{}', absolute={}, relative={}, angular={}, approximation={}, precision={}, lineardeflection={}, angulardeflection={})".format(
             self.unit,
             self.absolute,
             self.relative,
             self.angular,
             self.approximation,
             self.precision,
             self.lineardeflection,
+            self.angulardeflection,
         )
 
     def reset(self):
         """Reset all precision settings to their default values."""
         self._absolute = None
         self._relative = None
         self._angular = None
         self._approximation = None
         self._precision = None
         self._lineardeflection = None
+        self._angulardeflection = None
+
+    def update_from_dict(self, tolerance):
+        """Update the tolerance singleton from the key-value pairs found in a dict.
+
+        Parameters
+        ----------
+        tolerance : dict
+            A dictionary containing named tolerance values.
+
+        Returns
+        -------
+        None
+
+        """
+        for name in tolerance:
+            if hasattr(self, name):
+                setattr(self, name, tolerance[name])
 
     @property
     def units(self):
         return self._unit
 
     @units.setter
     def units(self, value):
@@ -246,14 +304,24 @@
             return self.LINEARDEFLECTION
         return self._lineardeflection
 
     @lineardeflection.setter
     def lineardeflection(self, value):
         self._lineardeflection = value
 
+    @property
+    def angulardeflection(self):
+        if not self._angulardeflection:
+            return self.ANGULARDEFLECTION
+        return self._angulardeflection
+
+    @angulardeflection.setter
+    def angulardeflection(self, value):
+        self._angulardeflection = value
+
     def tolerance(self, truevalue, rtol, atol):
         """Compute the tolerance for a comparison.
 
         Parameters
         ----------
         truevalue : float
             The true value of the comparison.
@@ -508,18 +576,15 @@
         True
         >>> tol.is_allclose([0.0, 0.0], [1e-6, 1e-5])
         False
 
         """
         rtol = rtol or self.relative
         atol = atol or self.absolute
-        return all(
-            self.is_allclose(a, b, rtol, atol) if hasattr(a, "__iter__") else self.compare(a, b, rtol, atol)
-            for a, b in zip(A, B)
-        )
+        return all(self.is_allclose(a, b, rtol, atol) if hasattr(a, "__iter__") else self.compare(a, b, rtol, atol) for a, b in zip(A, B))
 
     def is_angle_zero(self, a, tol=None):
         """Check if an angle is close enough to zero to be considered zero.
 
         Parameters
         ----------
         a : float
@@ -649,14 +714,89 @@
             if "{0:.{1}f}".format(y, precision) == minzero:
                 y = 0.0
             if "{0:.{1}f}".format(z, precision) == minzero:
                 z = 0.0
 
         return "{0:.{3}f},{1:.{3}f},{2:.{3}f}".format(x, y, z, precision)
 
+    def geometric_key_xy(self, xy, precision=None, sanitize=True):
+        """Compute the geometric key of a point in the XY plane.
+
+        Parameters
+        ----------
+        xy : list of float
+            The XY coordinates of the point.
+        precision : int, optional
+            The precision used when converting numbers to strings.
+            Default is ``None``, in which case ``self.precision`` is used.
+        sanitize : bool, optional
+            If ``True``, minus signs ("-") will be removed from values that are equal to zero up to the given precision.
+
+        Returns
+        -------
+        str
+            The geometric key in XY.
+
+        Raises
+        ------
+        ValueError
+            If the precision is zero.
+
+        Examples
+        --------
+        >>> tol = Tolerance()
+        >>> tol.geometric_key_xy([1.0, 2.0])
+        '1.000,2.000'
+
+        >>> tol = Tolerance()
+        >>> tol.geometric_key_xy([1.05725, 2.0195], precision=3)
+        '1.057,2.019'
+
+        >>> tol = Tolerance()
+        >>> tol.geometric_key_xy([1.0, 2.0], precision=-1)
+        '1,2'
+
+        >>> tol = Tolerance()
+        >>> tol.geometric_key_xy([1.0, 2.0], precision=-3)
+        '0,0'
+
+        >>> tol = Tolerance()
+        >>> tol.geometric_key_xy([1103, 205], precision=-3)
+        '1100,200'
+
+        """
+        x = xy[0]
+        y = xy[1]
+
+        if not precision:
+            precision = self.precision
+
+        if precision == 0:
+            raise ValueError("Precision cannot be zero.")
+
+        if precision == -1:
+            return "{:d},{:d}".format(int(x), int(y))
+
+        if precision < -1:
+            precision = -precision - 1
+            factor = 10**precision
+            return "{:d},{:d}".format(
+                int(round(x / factor) * factor),
+                int(round(y / factor) * factor),
+            )
+
+        if sanitize:
+            minzero = "-{0:.{1}f}".format(0.0, precision)
+            if "{0:.{1}f}".format(x, precision) == minzero:
+                x = 0.0
+            if "{0:.{1}f}".format(y, precision) == minzero:
+                y = 0.0
+
+        return "{0:.{2}f},{1:.{2}f}".format(x, y, precision)
+
     def format_number(self, number, precision=None):
         """Format a number as a string.
 
         Parameters
         ----------
         number : float
             The number.
```

### Comparing `COMPAS-2.1.0/src/compas/topology/__init__.py` & `compas-2.1.1/src/compas/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas/topology/combinatorics.py` & `compas-2.1.1/src/compas/topology/combinatorics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from collections import deque
+
 from compas.topology.traversal import breadth_first_traverse
 
 
 def vertex_coloring(adjacency):
     """Color the vertices of a graph such that no two colors are adjacent.
 
     Parameters
@@ -40,15 +41,15 @@
     --------
     This is a greedy algorithm, so it might be slow for large graphs.
 
     Examples
     --------
     >>> import compas
     >>> from compas.datastructures import Graph
-    >>> graph = Graph.from_obj(compas.get('lines.obj'))
+    >>> graph = Graph.from_obj(compas.get("lines.obj"))
     >>> key_color = vertex_coloring(graph.adjacency)
     >>> key = graph.get_any_node()
     >>> color = key_color[key]
     >>> any(key_color[nbr] == color for nbr in graph.neighbors(key))
     False
 
     """
```

### Comparing `COMPAS-2.1.0/src/compas/topology/connectivity.py` & `compas-2.1.1/src/compas/topology/connectivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from compas.utilities import pairwise
+from compas.itertools import pairwise
 
 
 def vertex_adjacency_from_edges(edges):
     """Construct an adjacency dictionary from a set of edges.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas/topology/orientation.py` & `compas-2.1.1/src/compas/topology/orientation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import random
-from compas.topology import breadth_first_traverse
+
 from compas.geometry import centroid_points
-from compas.utilities import pairwise
+from compas.itertools import pairwise
+from compas.topology import breadth_first_traverse
 
 
 def _closest_faces(vertices, faces, nmax=10, radius=10.0):
     points = [centroid_points([vertices[index] for index in face]) for face in faces]
 
     k = min(len(faces), nmax)
 
@@ -20,17 +21,17 @@
     # [2] the distance between the test point and the face centroid
 
     try:
         from scipy.spatial import cKDTree
 
     except Exception:
         try:
+            from Rhino.Geometry import Point3d  # type: ignore
             from Rhino.Geometry import RTree  # type: ignore
             from Rhino.Geometry import Sphere  # type: ignore
-            from Rhino.Geometry import Point3d  # type: ignore
 
         except Exception:
             from compas.geometry import KDTree
 
             tree = KDTree(points)
             closest = [tree.nearest_neighbors(point, k) for point in points]
             closest = [[index for xyz, index, d in nnbrs] for nnbrs in closest]
@@ -84,26 +85,28 @@
 
                 for a, b in pairwise(faces[nbr] + faces[nbr][0:1]):
                     if u == a and v == b:
                         nbrs.append(nbr)
                         found.add(nbr)
                         break
 
-        adjacency[face] = nbrs
+        adjacency[index] = nbrs
 
     return adjacency
 
 
 def face_adjacency(points, faces):
     """Build a face adjacency dict.
 
     Parameters
     ----------
-    mesh : :class:`compas.datastructures.Mesh`
-        A mesh object.
+    points : list[point]
+        The vertex locations of the faces.
+    faces : list[list[int]]
+        The faces defined as list of indices in the points list.
 
     Returns
     -------
     dict[int, list[int]]
         A dictionary mapping face identifiers (keys) to lists of neighboring faces.
 
     Notes
```

### Comparing `COMPAS-2.1.0/src/compas/topology/traversal.py` & `compas-2.1.1/src/compas/topology/traversal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 try:
     from queue import PriorityQueue
 except ImportError:
     from Queue import PriorityQueue  # type: ignore
 
 from collections import deque
 
 from compas.geometry import distance_point_point
 
-
 # ==============================================================================
 # DFS
 # ==============================================================================
 
 
 def depth_first_ordering(adjacency, root):
     """Compute a depth-first ordering of the nodes of a graph, starting from a root node.
```

### Comparing `COMPAS-2.1.0/src/compas/utilities/azync.py` & `compas-2.1.1/src/compas/utilities/azync.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,23 +73,25 @@
     The following example shows how to await an async function (``do_async_stuff`` in
     the example), using this utility:
 
     .. code-block:: python
 
         from compas.utilities import await_callback
 
+
         def do_async_stuff(callback):
             from threading import Thread
 
             def runner(cb):
-                print('doing async stuff')
+                print("doing async stuff")
                 # ..
-                cb('done')
+                cb("done")
+
+            Thread(target=runner, args=(callback,)).start()
 
-            Thread(target=runner, args=(callback, )).start()
 
         result = await_callback(do_async_stuff)
 
     """
     wait_event = threading.Event()
     call_results = {}
```

### Comparing `COMPAS-2.1.0/src/compas/utilities/datetime.py` & `compas-2.1.1/src/compas/utilities/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-import time
 import datetime
+import time
 
 
 def timestamp():
     """Generate a timestamp using the current date and time.
 
     Returns
     -------
     str
         The timestamp.
 
     Examples
     --------
-    >>> type(timestamp()) == type('')
+    >>> type(timestamp()) == type("")
     True
 
     """
     return datetime.datetime.fromtimestamp(time.time()).strftime("%Y%m%d%H%M%S")
 
 
 def now():
@@ -29,12 +29,12 @@
     Returns
     -------
     str
         The timestamp.
 
     Examples
     --------
-    >>> type(now()) == type('')
+    >>> type(now()) == type("")
     True
 
     """
     return timestamp()
```

### Comparing `COMPAS-2.1.0/src/compas/utilities/decorators.py` & `compas-2.1.1/src/compas/utilities/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import functools
 import pstats
-
 from functools import wraps
 
 try:
     from cStringIO import StringIO
 except ImportError:
     try:
         from StringIO import StringIO
```

### Comparing `COMPAS-2.1.0/src/compas/utilities/remote.py` & `compas-2.1.1/src/compas/utilities/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import os
 
 try:
     from urllib.request import urlretrieve
 except ImportError:
     from urllib import urlretrieve
@@ -26,16 +26,16 @@
     --------
     .. code-block:: python
 
         import os
         import compas
         from compas.utilities.remote import download_file_from_remote
 
-        source = 'https://raw.githubusercontent.com/compas-dev/compas/main/data/faces.obj'
-        target = os.path.join(compas.APPDATA, 'data', 'faces.obj')
+        source = "https://raw.githubusercontent.com/compas-dev/compas/main/data/faces.obj"
+        target = os.path.join(compas.APPDATA, "data", "faces.obj")
 
         download_file_from_remote(source, target)
 
     """
     parent = os.path.abspath(os.path.dirname(target))
 
     if not os.path.exists(parent):
```

### Comparing `COMPAS-2.1.0/src/compas/utilities/ssh.py` & `compas-2.1.1/src/compas/utilities/ssh.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_blender/__init__.py` & `compas-2.1.1/src/compas_blender/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     import bpy
     import compas_blender.data
 
 except ImportError:
     pass
 
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 
 INSTALLABLE_PACKAGES = ["compas", "compas_blender"]
 SUPPORTED_VERSIONS = ["3.3", "3.6", "4.0"]
 DEFAULT_VERSION = "4.0"
 
 INSTALLATION_ARGUMENTS = None
```

### Comparing `COMPAS-2.1.0/src/compas_blender/collections.py` & `compas-2.1.1/src/compas_blender/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from typing import List
+from typing import Text
+
 import bpy  # type: ignore
-from typing import List, Text
 
 from compas_blender.objects import delete_objects
 
 
 def collection_path(collection, names=[]):
     for parent in bpy.data.collections:
         if collection.name in parent.children:
```

### Comparing `COMPAS-2.1.0/src/compas_blender/conversions/__init__.py` & `compas-2.1.1/src/compas_blender/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_blender/conversions/colors.py` & `compas-2.1.1/src/compas_blender/conversions/colors.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_blender/conversions/curves.py` & `compas-2.1.1/src/compas_blender/conversions/curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Optional
 
 import bpy  # type: ignore
 
 from compas.geometry import Circle
 from compas.geometry import Line
-from compas.geometry import Polyline
 from compas.geometry import NurbsCurve
-
+from compas.geometry import Polyline
 
 # =============================================================================
 # To Blender
 # =============================================================================
 
 
 def line_to_blender_curve(line: Line) -> bpy.types.Curve:
```

### Comparing `COMPAS-2.1.0/src/compas_blender/conversions/geometry.py` & `compas-2.1.1/src/compas_blender/conversions/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Optional
 
 import bpy  # type: ignore
 
+from compas.geometry import Cylinder
+
 # import bmesh  # type: ignore
 # import mathutils  # type: ignore
-
 from compas.geometry import Point
 from compas.geometry import Pointcloud
 from compas.geometry import Sphere
-from compas.geometry import Cylinder
-
 
 # =============================================================================
 # To Blender
 # =============================================================================
 
 
 def point_to_blender_sphere(point: Point) -> bpy.types.Object:
@@ -29,17 +28,15 @@
     :blender:`bpy.types.Object`
         A Blender sphere object.
 
     """
     raise NotImplementedError
 
 
-def pointcloud_to_blender(
-    pointcloud: Pointcloud, radius: float = 0.05, u: int = 16, v: int = 16, name: Optional[str] = None
-) -> bpy.types.Object:
+def pointcloud_to_blender(pointcloud: Pointcloud, radius: float = 0.05, u: int = 16, v: int = 16, name: Optional[str] = None) -> bpy.types.Object:
     """Convert a COMPAS pointcloud to a Blender pointcloud.
 
     Parameters
     ----------
     pointcloud : list of :class:`compas.geometry.Point`
         A COMPAS pointcloud.
     radius : float, optional
```

### Comparing `COMPAS-2.1.0/src/compas_blender/conversions/meshes.py` & `compas-2.1.1/src/compas_blender/conversions/meshes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
-import bpy  # type: ignore
 import bmesh  # type: ignore
+import bpy  # type: ignore
 
-from compas.geometry import Translation
 from compas.datastructures import Mesh
+from compas.geometry import Translation
 
 # To Do
 # -----
 # - [ ] Write COMPAS Mesh attributes to Blender
 # - [ ] Read Mesh attributes from Blender to COMPAS
 # - [ ] Include results of modifiers in VOMPAS Mesh
```

### Comparing `COMPAS-2.1.0/src/compas_blender/conversions/surfaces.py` & `compas-2.1.1/src/compas_blender/conversions/surfaces.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import bpy  # type: ignore
-from compas.geometry import NurbsSurface
 
+from compas.geometry import NurbsSurface
 
 # =============================================================================
 # To Blender
 # =============================================================================
 
 
 def nurbssurface_to_blender_surface(nurbssurface: NurbsSurface, u=32, v=32) -> bpy.types.Curve:
```

### Comparing `COMPAS-2.1.0/src/compas_blender/conversions/transformations.py` & `compas-2.1.1/src/compas_blender/conversions/transformations.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import mathutils  # type: ignore
-from compas.geometry import Transformation
 
+from compas.geometry import Transformation
 
 # =============================================================================
 # To Blender
 # =============================================================================
 
 
 def transformation_to_blender(transformation):
```

### Comparing `COMPAS-2.1.0/src/compas_blender/data.py` & `compas-2.1.1/src/compas_blender/data.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_blender/geometry/booleans.py` & `compas-2.1.1/src/compas_blender/geometry/booleans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import bpy  # type: ignore
+
 from compas.plugins import plugin
 
 
 @plugin(category="booleans", requires=["bpy"])
 def boolean_union_mesh_mesh(A, B, remesh=False):
     """Compute the boolean union of two triangle meshes.
 
@@ -74,17 +75,17 @@
     return _boolean_operation(A, B, "INTERSECT")
 
 
 boolean_intersection_mesh_mesh.__plugin__ = True
 
 
 def _boolean_operation(A, B, method):
-    from compas_blender.utilities import draw_mesh
     from compas_blender.utilities import delete_object
     from compas_blender.utilities import delete_unused_data
+    from compas_blender.utilities import draw_mesh
 
     A = draw_mesh(*A)
     B = draw_mesh(*B)
     boolean = A.modifiers.new(type="BOOLEAN", name=f"A {method} B")
     boolean.object = B
     boolean.operation = method
     bpy.ops.object.modifier_apply({"object": A}, modifier=boolean.name)
```

### Comparing `COMPAS-2.1.0/src/compas_blender/install.py` & `compas-2.1.1/src/compas_blender/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import importlib
 import itertools
 import os
 import sys
 
-import compas_blender
-
 import compas._os
 import compas.plugins
-
+import compas_blender
 
 INSTALLED_VERSION = None
 
 
 def install(version=None, packages=None, clean=False):
     """Install COMPAS for Blender.
 
@@ -29,14 +27,15 @@
         also existing symlinks that are not importable in the current environment.
 
     Examples
     --------
     .. code-block:: python
 
         import compas_blender.install
+
         compas_blender.install.install()
 
     .. code-block:: bash
 
         python -m compas_blender.install
 
     """
@@ -209,17 +208,15 @@
             try:
                 package, message, success = item
                 status = "OK" if success else "ERROR"
                 if not success:
                     all_steps_succeeded = False
                 print("   {} {}: {}".format(package.ljust(20), status, message))
             except ValueError:
-                post_execution_errors.append(
-                    ValueError("Step ran without errors but result is wrongly formatted: {}".format(str(item)))
-                )
+                post_execution_errors.append(ValueError("Step ran without errors but result is wrongly formatted: {}".format(str(item))))
 
     if post_execution_errors:
         print("\nOne or more errors occurred:\n")
         for error in post_execution_errors:
             print("   - {}".format(repr(error)))
 
         all_steps_succeeded = False
@@ -243,17 +240,17 @@
     can implement this pluggable interface to automatically
     have their packages made available inside Blender when
     COMPAS is installed into it.
 
     Examples
     --------
     >>> import compas.plugins
-    >>> @compas.plugins.plugin(category='install')
+    >>> @compas.plugins.plugin(category="install")
     ... def installable_blender_packages():
-    ...    return ['compas_fab']
+    ...     return ["compas_fab"]
 
     Returns
     -------
     :obj:`list` of :obj:`str`
         List of package names to make available inside Blender.
     """
     pass
@@ -272,18 +269,18 @@
     ----------
     installed_packages : :obj:`list` of :obj:`str`
         List of packages that have been installed successfully.
 
     Examples
     --------
     >>> import compas.plugins
-    >>> @compas.plugins.plugin(category='install')
+    >>> @compas.plugins.plugin(category="install")
     ... def after_blender_install(installed_packages):
-    ...    # Do something after package is installed to Blender, e.g. install the COMPAS UI, etc
-    ...    return [('compas_blender', 'COMPAS Blender UI installed', True)]
+    ...     # Do something after package is installed to Blender, e.g. install the COMPAS UI, etc
+    ...     return [("compas_blender", "COMPAS Blender UI installed", True)]
 
     Returns
     -------
     :obj:`list` of 3-tuple (str, str, bool)
         List containing a 3-tuple with component name, message and True/False success flag.
 
     """
```

### Comparing `COMPAS-2.1.0/src/compas_blender/objects.py` & `compas-2.1.1/src/compas_blender/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from typing import Iterable
+from typing import List
+from typing import Text
+
 import bpy  # type: ignore
-from typing import List, Iterable, Text
 
 from compas_blender.data import delete_unused_data
 
-
 # ==============================================================================
 # Delete
 # ==============================================================================
 
 
 def delete_all_objects(purge_data: bool = True):
     """Delete all mesh and curve scene objects, and the attached mesh and curve data blocks.
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/__init__.py` & `compas-2.1.1/src/compas_blender/scene/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/boxobject.py` & `compas-2.1.1/src/compas_blender/scene/boxobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Any
 from typing import Optional
 from typing import Union
 
 import bpy  # type: ignore
 
-from compas.geometry import Box
 from compas.colors import Color
-
+from compas.geometry import Box
+from compas.scene import GeometryObject
 from compas_blender import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import BlenderSceneObject
 
 
 class BoxObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing box shapes in Blender.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/capsuleobject.py` & `compas-2.1.1/src/compas_blender/scene/capsuleobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Capsule
 from compas.colors import Color
-
+from compas.geometry import Capsule
+from compas.scene import GeometryObject
 from compas_blender import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import BlenderSceneObject
 
 
 class CapsuleObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing capsule shapes in Blender.
 
     Parameters
@@ -61,15 +60,14 @@
         """
         name = self.geometry.name
         color = Color.coerce(color) or self.color
 
         vertices, faces = self.geometry.to_vertices_and_faces(u=u, v=v)
         mesh = conversions.vertices_and_faces_to_blender_mesh(vertices, faces, name=self.geometry.name)
         if shade_smooth:
-            print(dir(mesh))
             mesh.shade_smooth()
 
         obj = self.create_object(mesh, name=name)
         self.update_object(obj, color=color, collection=collection, show_wire=show_wire)
 
         self._guids = [obj]
         return self.guids
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/circleobject.py` & `compas-2.1.1/src/compas_blender/scene/circleobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Circle
 from compas.colors import Color
-
+from compas.geometry import Circle
 from compas.scene import GeometryObject
+
 from .sceneobject import BlenderSceneObject
 
 
 class CircleObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing circles in Blender.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/coneobject.py` & `compas-2.1.1/src/compas_blender/scene/coneobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Cone
 from compas.colors import Color
-
+from compas.geometry import Cone
+from compas.scene import GeometryObject
 from compas_blender import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import BlenderSceneObject
 
 
 class ConeObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing cone shapes in Blender.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/curveobject.py` & `compas-2.1.1/src/compas_blender/scene/curveobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Curve
 from compas.colors import Color
+from compas.geometry import Curve
+from compas.scene import GeometryObject
 from compas_blender import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import BlenderSceneObject
 
 
 class CurveObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing curves in Blender.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/cylinderobject.py` & `compas-2.1.1/src/compas_blender/scene/cylinderobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Cylinder
 from compas.colors import Color
-
+from compas.geometry import Cylinder
+from compas.scene import GeometryObject
 from compas_blender import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import BlenderSceneObject
 
 
 class CylinderObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing cylinder shapes in Blender.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/frameobject.py` & `compas-2.1.1/src/compas_blender/scene/frameobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
+from compas.colors import Color
 from compas.geometry import Frame
 from compas.geometry import Line
-from compas.colors import Color
-
 from compas.scene import GeometryObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class FrameObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing frames in Blender.
 
     Parameters
     ----------
     frame: :class:`compas.geometry.Frame`
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/lineobject.py` & `compas-2.1.1/src/compas_blender/scene/lineobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Line
 from compas.colors import Color
-
+from compas.geometry import Line
+from compas.scene import GeometryObject
 from compas_blender import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import BlenderSceneObject
 
 
 class LineObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing lines in Blender.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/meshobject.py` & `compas-2.1.1/src/compas_blender/scene/meshobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import bpy  # type: ignore
 
 import compas_blender
+from compas.colors import Color
 from compas.datastructures import Mesh
+from compas.geometry import Cylinder
 from compas.geometry import Line
 from compas.geometry import Sphere
-from compas.geometry import Cylinder
 from compas.geometry import add_vectors
 from compas.geometry import centroid_points
 from compas.geometry import scale_vector
-from compas.colors import Color
-
 from compas.scene import MeshObject as BaseMeshObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class MeshObject(BlenderSceneObject, BaseMeshObject):
     """Scene object for drawing mesh data structures in Blender.
 
     Parameters
     ----------
     mesh : :class:`compas.datastructures.Mesh`
@@ -76,17 +75,15 @@
         """
         compas_blender.delete_objects(self.faceobjects)
 
     # ==========================================================================
     # draw
     # ==========================================================================
 
-    def draw(
-        self, color: Optional[Color] = None, collection: Optional[str] = None, show_wire: bool = True
-    ) -> list[bpy.types.Object]:
+    def draw(self, color: Optional[Color] = None, collection: Optional[str] = None, show_wire: bool = True) -> list[bpy.types.Object]:
         """Draw the mesh.
 
         Parameters
         ----------
         color : :class:`compas.colors.Color`, optional
             The color of the mesh.
         collection : str, optional
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/planeobject.py` & `compas-2.1.1/src/compas_blender/scene/planeobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Plane
-from compas.geometry import Line
-from compas.geometry import Frame
 from compas.colors import Color
-
+from compas.geometry import Frame
+from compas.geometry import Line
+from compas.geometry import Plane
 from compas.scene import GeometryObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class PlaneObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing planes in Blender.
 
     Parameters
     ----------
     plane: :class:`compas.geometry.Plane`
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/pointcloudobject.py` & `compas-2.1.1/src/compas_blender/scene/pointcloudobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Point
 from compas.colors import Color
-
+from compas.geometry import Point
 from compas.scene import GeometryObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class PointcloudObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing pointclouds in Blender.
 
     Parameters
     ----------
     pointcloud : :class:`compas.geometry.Pointcloud`
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/pointobject.py` & `compas-2.1.1/src/compas_blender/scene/pointobject.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Point
 from compas.colors import Color
-
+from compas.geometry import Point
 from compas.scene import GeometryObject
+
 from .sceneobject import BlenderSceneObject
 
 
 class PointObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing points in Blender.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/polygonobject.py` & `compas-2.1.1/src/compas_blender/scene/polygonobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Polygon
 from compas.colors import Color
-
+from compas.geometry import Polygon
+from compas.scene import GeometryObject
 from compas_blender import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import BlenderSceneObject
 
 
 class PolygonObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing polygons in Blender.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/polyhedronobject.py` & `compas-2.1.1/src/compas_blender/scene/polyhedronobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
-from compas.geometry import Polyhedron
-from compas.colors import Color
 
+from compas.colors import Color
+from compas.geometry import Polyhedron
 from compas.scene import GeometryObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class PolyhedronObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing polyhedron shapes in Blender.
 
     Parameters
     ----------
     polyhedron : :class:`compas.geometry.Polyhedron`
@@ -22,17 +22,15 @@
         Additional keyword arguments.
 
     """
 
     def __init__(self, polyhedron: Polyhedron, **kwargs: Any):
         super().__init__(geometry=polyhedron, **kwargs)
 
-    def draw(
-        self, color: Optional[Color] = None, collection: Optional[str] = None, show_wire: bool = True
-    ) -> list[bpy.types.Object]:
+    def draw(self, color: Optional[Color] = None, collection: Optional[str] = None, show_wire: bool = True) -> list[bpy.types.Object]:
         """Draw the polyhedron associated with the scene object.
 
         Parameters
         ----------
         color : tuple[float, float, float] | tuple[int, int, int] | :class:`compas.colors.Color`, optional
             The RGB color of the polyhedron.
         collection : str, optional
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/polylineobject.py` & `compas-2.1.1/src/compas_blender/scene/polylineobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Polyline
 from compas.colors import Color
-
+from compas.geometry import Polyline
 from compas.scene import GeometryObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class PolylineObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing polylines in Blender.
 
     Parameters
     ----------
     polyline : :class:`compas.geometry.Polyline`
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/sceneobject.py` & `compas-2.1.1/src/compas_blender/scene/sceneobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Any
-from typing import Union
 from typing import Optional
+from typing import Union
 
 import bpy  # type: ignore
-import compas_blender
 
+import compas_blender
 from compas.colors import Color
-from compas.scene import SceneObject
 from compas.geometry import Transformation
-
+from compas.scene import SceneObject
 from compas_blender import conversions
 
 
 class BlenderSceneObject(SceneObject):
     """Base class for all Blender scene objects.
 
     Parameters
@@ -36,17 +35,15 @@
     # many of the methods below will be added to a general scene object in the future
     # to make them universaly accessible they are added here for now
 
     # =============================================================================
     # Objects
     # =============================================================================
 
-    def create_object(
-        self, geometry: Union[bpy.types.Mesh, bpy.types.Curve], name: Optional[str] = None
-    ) -> bpy.types.Object:
+    def create_object(self, geometry: Union[bpy.types.Mesh, bpy.types.Curve], name: Optional[str] = None) -> bpy.types.Object:
         """Add an object to the Blender scene.
 
         Parameters
         ----------
         geometry : :blender:`bpy.types.Mesh` | :blender:`bpy.types.Curve`
             The Blender object data.
         name : str, optional
@@ -101,17 +98,15 @@
 
         if color:
             self.set_object_color(obj, color)
 
         self.set_object_tranformation(obj, transformation)
         self.add_object_to_collection(obj, collection)
 
-    def add_object_to_collection(
-        self, obj: bpy.types.Object, name: Optional[str] = None, do_unlink: Optional[bool] = True
-    ) -> bpy.types.Collection:
+    def add_object_to_collection(self, obj: bpy.types.Object, name: Optional[str] = None, do_unlink: Optional[bool] = True) -> bpy.types.Collection:
         """Add an object to a collection.
 
         Parameters
         ----------
         obj : :blender:`bpy.types.Object`
             The Blender object.
         name : str, optional
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/sphereobject.py` & `compas-2.1.1/src/compas_blender/scene/sphereobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from typing import Optional
 from typing import Any
+from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Sphere
 from compas.colors import Color
-
+from compas.geometry import Sphere
 from compas.scene import GeometryObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class SphereObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing sphere shapes in Blender.
 
     Parameters
     ----------
     sphere : :class:`compas.geometry.Sphere`
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/surfaceobject.py` & `compas-2.1.1/src/compas_blender/scene/surfaceobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Surface
 from compas.colors import Color
-
+from compas.geometry import Surface
 from compas.scene import GeometryObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class SurfaceObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing surfaces in Blender.
 
     Parameters
     ----------
     surface : :class:`compas.geometry.Surface`
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/torusobject.py` & `compas-2.1.1/src/compas_blender/scene/torusobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from typing import Optional
 from typing import Any
+from typing import Optional
 
 import bpy  # type: ignore
 
-from compas.geometry import Torus
 from compas.colors import Color
-
+from compas.geometry import Torus
 from compas.scene import GeometryObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class TorusObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing torus shapes in Blender.
 
     Parameters
     ----------
     torus : :class:`compas.geometry.Torus`
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/vectorobject.py` & `compas-2.1.1/src/compas_blender/scene/vectorobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import Any
 from typing import Optional
 
 import bpy  # type: ignore
 
+from compas.colors import Color
+from compas.geometry import Line
 from compas.geometry import Point
 from compas.geometry import Vector
-from compas.geometry import Line
-from compas.colors import Color
-
 from compas.scene import GeometryObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class VectorObject(BlenderSceneObject, GeometryObject):
     """Scene object for drawing vectors in Blender.
 
     Parameters
     ----------
     primitive : :class:`compas.geometry.Vector`
```

### Comparing `COMPAS-2.1.0/src/compas_blender/scene/volmeshobject.py` & `compas-2.1.1/src/compas_blender/scene/volmeshobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from typing import Optional
-from typing import Union
 from typing import Any
-from typing import List
 from typing import Dict
+from typing import List
+from typing import Optional
 from typing import Tuple
+from typing import Union
 
 import bpy  # type: ignore
 
 import compas_blender
-
+from compas.colors import Color
+from compas.geometry import Line
 from compas.geometry import add_vectors
-from compas.geometry import scale_vector
 from compas.geometry import centroid_points
-from compas.geometry import Line
-from compas.colors import Color
-
+from compas.geometry import scale_vector
 from compas.scene import VolMeshObject as BaseVolMeshObject
-from .sceneobject import BlenderSceneObject
-
 from compas_blender import conversions
 
+from .sceneobject import BlenderSceneObject
+
 
 class VolMeshObject(BlenderSceneObject, BaseVolMeshObject):
     """A scene object for drawing volumetric mesh data structures in Blender.
 
     Parameters
     ----------
     volmesh : :class:`compas.datastructures.VolMesh`
@@ -87,17 +85,15 @@
         """
         compas_blender.delete_objects(self.cellobjects)
 
     # ==========================================================================
     # draw
     # ==========================================================================
 
-    def draw(
-        self, cells: Optional[List[int]] = None, color: Optional[Color] = None, collection: Optional[str] = None
-    ) -> list[bpy.types.Object]:
+    def draw(self, cells: Optional[List[int]] = None, color: Optional[Color] = None, collection: Optional[str] = None) -> list[bpy.types.Object]:
         """Draw a selection of cells.
 
         Parameters
         ----------
         cells : list[int], optional
             A list of cells to draw.
             The default is None, in which case all cells are drawn.
@@ -192,17 +188,15 @@
         objects = []
 
         self.edgecolor = color
 
         for u, v in edges or self.volmesh.edges():  # type: ignore
             name = f"{self.volmesh.name}.edge.{u}-{v}"  # type: ignore
             color = self.edgecolor[u, v]  # type: ignore
-            curve = conversions.line_to_blender_curve(
-                Line(self.volmesh.vertices_attributes("xyz")[u], self.volmesh.vertices_attributes("xyz")[v])
-            )
+            curve = conversions.line_to_blender_curve(Line(self.volmesh.vertices_attributes("xyz")[u], self.volmesh.vertices_attributes("xyz")[v]))
 
             obj = self.create_object(curve, name=name)
             self.update_object(obj, color=color, collection=collection)  # type: ignore
             objects.append(obj)
 
         return objects
```

### Comparing `COMPAS-2.1.0/src/compas_blender/utilities/__init__.py` & `compas-2.1.1/src/compas_blender/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_blender/utilities/drawing.py` & `compas-2.1.1/src/compas_blender/utilities/drawing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from typing import Dict
 from typing import List
-from typing import Union
-from typing import Tuple
 from typing import Text
+from typing import Tuple
+from typing import Union
 
 import bpy  # type: ignore
 
-from compas_blender.collections import create_collection
-
 from compas.geometry import centroid_points
 from compas.geometry import distance_point_point
 from compas.geometry import subtract_vectors
-
+from compas_blender.collections import create_collection
 
 RGBColor = Union[Tuple[int, int, int], Tuple[float, float, float]]
 
 
 def _link_object(obj, collection=None, layer=None):
     if not collection:
         collection = bpy.context.collection
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/__init__.py` & `compas-2.1.1/src/compas_ghpython/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import compas
 import compas_rhino
 
 from compas_rhino import unload_modules  # noqa: F401
 
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 if compas.is_rhino():
     from .utilities import *  # noqa: F401 F403
 
 __all__ = [
     "get_grasshopper_managedplugin_path",
     "get_grasshopper_library_path",
@@ -74,17 +74,15 @@
     elif compas.OSX:
         gh_managedplugin_path = os.path.join(managedplugins, "GrasshopperPlugin.rhp")
 
     else:
         raise NotImplementedError
 
     if not os.path.exists(gh_managedplugin_path):
-        raise Exception(
-            "The Grasshopper (managed) Plug-in folder does not exist in this location: {}".format(gh_managedplugin_path)
-        )
+        raise Exception("The Grasshopper (managed) Plug-in folder does not exist in this location: {}".format(gh_managedplugin_path))
 
     return gh_managedplugin_path
 
 
 # =============================================================================
 # GH Plugin Libraries path
 # =============================================================================
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/components/Compas_RpcCall/code.py` & `compas-2.1.1/src/compas_ghpython/components/Compas_RpcCall/code.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_ghpython/components/__init__.py` & `compas-2.1.1/src/compas_ghpython/components/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_ghpython/install.py` & `compas-2.1.1/src/compas_ghpython/install.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/__init__.py` & `compas-2.1.1/src/compas_ghpython/scene/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/boxobject.py` & `compas-2.1.1/src/compas_ghpython/scene/boxobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class BoxObject(GHSceneObject, GeometryObject):
     """Scene object for drawing box shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/brepobject.py` & `compas-2.1.1/src/compas_ghpython/scene/brepobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class BrepObject(GHSceneObject, GeometryObject):
     """A Scene object for drawing a brep in Grasshopper.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/capsuleobject.py` & `compas-2.1.1/src/compas_ghpython/scene/capsuleobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class CapsuleObject(GHSceneObject, GeometryObject):
     """Scene object for drawing capsule shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/circleobject.py` & `compas-2.1.1/src/compas_ghpython/scene/circleobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class CircleObject(GHSceneObject, GeometryObject):
     """Scene object for drawing circles.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/coneobject.py` & `compas-2.1.1/src/compas_ghpython/scene/coneobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class ConeObject(GHSceneObject, GeometryObject):
     """Scene object for drawing cone shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/curveobject.py` & `compas-2.1.1/src/compas_ghpython/scene/curveobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class CurveObject(GHSceneObject, GeometryObject):
     """Scene object for drawing curves.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/cylinderobject.py` & `compas-2.1.1/src/compas_ghpython/scene/cylinderobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class CylinderObject(GHSceneObject, GeometryObject):
     """Scene object for drawing cylinder shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/ellipseobject.py` & `compas-2.1.1/src/compas_ghpython/scene/ellipseobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class EllipseObject(GHSceneObject, GeometryObject):
     """Scene object for drawing ellipses.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/frameobject.py` & `compas-2.1.1/src/compas_ghpython/scene/frameobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class FrameObject(GHSceneObject, GeometryObject):
     """Scene object for drawing frames.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/graphobject.py` & `compas-2.1.1/src/compas_ghpython/scene/graphobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GraphObject as BaseGraphObject
 from compas_rhino import conversions
 
-from compas.scene import GraphObject as BaseGraphObject
 from .sceneobject import GHSceneObject
 
 
 class GraphObject(GHSceneObject, BaseGraphObject):
     """Scene object for drawing graph data structures.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/lineobject.py` & `compas-2.1.1/src/compas_ghpython/scene/lineobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class LineObject(GHSceneObject, GeometryObject):
     """Scene object for drawing lines.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/meshobject.py` & `compas-2.1.1/src/compas_ghpython/scene/meshobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-from compas.scene import MeshObject as BaseMeshObject
 from compas.colors import Color
+from compas.scene import MeshObject as BaseMeshObject
 from compas_rhino import conversions
 from compas_rhino.scene.helpers import ngon
+
 from .sceneobject import GHSceneObject
 
 
 class MeshObject(GHSceneObject, BaseMeshObject):
     """Scene object for drawing mesh data structures.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/planeobject.py` & `compas-2.1.1/src/compas_ghpython/scene/planeobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.geometry import Frame
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
-from compas.geometry import Frame
 
 
 class PlaneObject(GHSceneObject, GeometryObject):
     """Scene object for drawing planes.
 
     Parameters
     ----------
@@ -38,17 +38,15 @@
 
         Returns
         -------
         list[:rhino:`Rhino.Geometry.Line`, :rhino:`Rhino.Geometry.Mesh`]
             List of created Rhino geometries.
         """
         frame = Frame.from_plane(self._item)
-        normal = conversions.line_to_rhino(
-            [frame.to_world_coordinates([0, 0, 0]), frame.to_world_coordinates([0, 0, self.scale])]
-        )
+        normal = conversions.line_to_rhino([frame.to_world_coordinates([0, 0, 0]), frame.to_world_coordinates([0, 0, self.scale])])
 
         vertices = [
             frame.to_world_coordinates([-self.scale, -self.scale, 0]),
             frame.to_world_coordinates([self.scale, -self.scale, 0]),
             frame.to_world_coordinates([self.scale, self.scale, 0]),
             frame.to_world_coordinates([-self.scale, self.scale, 0]),
         ]
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/pointobject.py` & `compas-2.1.1/src/compas_ghpython/scene/pointobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class PointObject(GHSceneObject, GeometryObject):
     """Scene object for drawing points.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/polygonobject.py` & `compas-2.1.1/src/compas_ghpython/scene/polygonobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.colors import Color
-
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class PolygonObject(GHSceneObject, GeometryObject):
     """Scene object for drawing polygons.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/polyhedronobject.py` & `compas-2.1.1/src/compas_ghpython/scene/polyhedronobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.colors import Color
-
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class PolyhedronObject(GHSceneObject, GeometryObject):
     """Scene object for drawing polyhedron shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/polylineobject.py` & `compas-2.1.1/src/compas_ghpython/scene/polylineobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class PolylineObject(GHSceneObject, GeometryObject):
     """Scene object for drawing polylines.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/sphereobject.py` & `compas-2.1.1/src/compas_ghpython/scene/sphereobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class SphereObject(GHSceneObject, GeometryObject):
     """Scene object for drawing sphere shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/surfaceobject.py` & `compas-2.1.1/src/compas_ghpython/scene/surfaceobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class SurfaceObject(GHSceneObject, GeometryObject):
     """Scene object for drawing surfaces.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/torusobject.py` & `compas-2.1.1/src/compas_ghpython/scene/torusobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import GeometryObject
 from compas_rhino import conversions
 
-from compas.scene import GeometryObject
 from .sceneobject import GHSceneObject
 
 
 class TorusObject(GHSceneObject, GeometryObject):
     """Scene object for drawing torus shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/vectorobject.py` & `compas-2.1.1/src/compas_ghpython/scene/vectorobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-from compas_rhino import conversions
-
 from compas.geometry import Point
 from compas.scene import GeometryObject
+from compas_rhino import conversions
+
 from .sceneobject import GHSceneObject
 
 
 class VectorObject(GHSceneObject, GeometryObject):
     """Scene object for drawing vectors.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/scene/volmeshobject.py` & `compas-2.1.1/src/compas_ghpython/scene/volmeshobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
+from compas.scene import VolMeshObject as BaseVolMeshObject
 from compas_rhino import conversions
 from compas_rhino.scene.helpers import ngon
 
-from compas.scene import VolMeshObject as BaseVolMeshObject
 from .sceneobject import GHSceneObject
 
 
 class VolMeshObject(GHSceneObject, BaseVolMeshObject):
     """Scene object for drawing volmesh data structures.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/sets.py` & `compas-2.1.1/src/compas_ghpython/sets.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-import System  # type: ignore
 import Grasshopper  # type: ignore
+import System  # type: ignore
 
 
 def list_to_ghtree(items, none_and_holes=False, base_path=[0]):
     """Transforms nestings of lists or tuples to a Grasshopper DataTree.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas_ghpython/timer.py` & `compas-2.1.1/src/compas_ghpython/timer.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_ghpython/uninstall.py` & `compas-2.1.1/src/compas_ghpython/uninstall.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_ghpython/utilities/__init__.py` & `compas-2.1.1/src/compas_ghpython/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_ghpython/utilities/drawing.py` & `compas-2.1.1/src/compas_ghpython/utilities/drawing.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from Rhino.Geometry import Vector3d
 from Rhino.Geometry import Vector3f
 from System.Array import CreateInstance
 from System.Drawing import Color
 from System.Enum import ToObject
 
 from compas.geometry import centroid_points
-from compas.utilities import pairwise
+from compas.itertools import pairwise
 from compas_rhino.utilities.drawing import _face_to_max_quad
 
 try:
     from Rhino.Geometry import MeshNgon
 except ImportError:
     MeshNgon = False
 
@@ -145,17 +145,15 @@
     -------
     list[:rhino:`Rhino.Geometry.PolylineCurve`]
 
     Notes
     -----
     .. code-block:: python
 
-        Schema({
-            'points': lambda x: all(len(y) == 3 for y in x)
-        })
+        Schema({"points": lambda x: all(len(y) == 3 for y in x)})
 
     """
     rg_polylines = []
     # We need to use PolylineCurve because of this:
     # https://discourse.mcneel.com/t/polyline-output-wanted-but-got-a-list-of-points/77509
     for p in iter(polylines):
         points = p["points"]
@@ -176,18 +174,15 @@
     -------
     list[:rhino:`Rhino.Geometry.Mesh`]
 
     Notes
     -----
     .. code-block:: python
 
-        Schema({
-            'points': lambda x: all(len(y) == 3 for y in x),
-            Optional('vertexcolors', default=None): lambda x: all(len(y) == 3 for y in x)
-        })
+        Schema({"points": lambda x: all(len(y) == 3 for y in x), Optional("vertexcolors", default=None): lambda x: all(len(y) == 3 for y in x)})
 
     """
     meshes = []
     for face in iter(faces):
         points = face["points"][:]
         vertexcolors = face.get("vertexcolors")
         v = len(points)
@@ -230,19 +225,15 @@
     -------
     list[:rhino:`Rhino.Geometry.Cylinder`]
 
     Notes
     -----
     .. code-block:: python
 
-        Schema({
-            'start': lambda x: len(x) == 3,
-            'end': lambda x: len(x) == 3,
-            'radius': And(Or(int, float), lambda x: x > 0)
-        })
+        Schema({"start": lambda x: len(x) == 3, "end": lambda x: len(x) == 3, "radius": And(Or(int, float), lambda x: x > 0)})
 
     """
     rg_cylinders = []
     for c in iter(cylinders):
         start = c["start"]
         end = c["end"]
         radius = c["radius"]
@@ -280,18 +271,15 @@
     -------
     list[:rhino:`Rhino.Geometry.Brep`]
 
     Notes
     -----
     .. code-block:: python
 
-        Schema({
-            'points': lambda x: all(len(y) == 3 for y in x),
-            'radius': And(Or(int, float), lambda x: x > 0)
-        })
+        Schema({"points": lambda x: all(len(y) == 3 for y in x), "radius": And(Or(int, float), lambda x: x > 0)})
 
     """
     abs_tol = TOL
     ang_tol = sc.doc.ModelAngleToleranceRadians
     for p in pipes:
         points = p["points"]
         radius = p["radius"]
@@ -319,18 +307,15 @@
     -------
     list[:rhino:`Rhino.Geometry.Sphere`]
 
     Notes
     -----
     .. code-block:: python
 
-        Schema({
-            'pos': lambda x: len(x) == 3,
-            'radius': And(Or(int, float), lambda x: x > 0)
-        })
+        Schema({"pos": lambda x: len(x) == 3, "radius": And(Or(int, float), lambda x: x > 0)})
 
     """
     rg_sheres = []
     for s in iter(spheres):
         pos = s["pos"]
         radius = s["radius"]
         rg_sheres.append(Sphere(Point3d(*pos), radius))
@@ -441,18 +426,15 @@
     -------
     list[:rhino:`Rhino.Geometry.Circle`]
 
     Notes
     -----
     .. code-block:: python
 
-        Schema({
-            'plane': lambda x: len(x[0]) == 3 and len(x[1]) == 3,
-            'radius': And(Or(int, float), lambda x: x > 0)
-        })
+        Schema({"plane": lambda x: len(x[0]) == 3 and len(x[1]) == 3, "radius": And(Or(int, float), lambda x: x > 0)})
 
     """
     rg_circles = []
     for c in iter(circles):
         point, normal = c["plane"]
         radius = c["radius"]
         rg_circles.append(Circle(Plane(Point3d(*point), Vector3d(*normal)), radius))
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/__init__.py` & `compas-2.1.1/src/compas_rhino/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import io
 import os
 import sys
 
 import compas
 import compas._os
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 
 PURGE_ON_DELETE = True
 
 INSTALLABLE_PACKAGES = ["compas", "compas_rhino", "compas_ghpython"]
 SUPPORTED_VERSIONS = ["5.0", "6.0", "7.0", "8.0"]
 DEFAULT_VERSION = "8.0"
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conduits/base.py` & `compas-2.1.1/src/compas_rhino/conduits/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import time
 from contextlib import contextmanager
 
 import Rhino
 import scriptcontext as sc
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conduits/faces.py` & `compas-2.1.1/src/compas_rhino/conduits/faces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from System.Drawing.Color import FromArgb
 from Rhino.Geometry import Point3d
+from System.Drawing.Color import FromArgb
 
-from compas.utilities import iterable_like
+from compas.itertools import iterable_like
 from compas.utilities import is_sequence_of_iterable
 
 from .base import BaseConduit
 
 
 class FacesConduit(BaseConduit):
     """A Rhino display conduit for faces.
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conduits/labels.py` & `compas-2.1.1/src/compas_rhino/conduits/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from System.Drawing.Color import FromArgb
 from Rhino.Geometry import Point3d
+from System.Drawing.Color import FromArgb
 
-from compas.utilities import iterable_like
+from compas.itertools import iterable_like
 from compas.utilities import is_sequence_of_iterable
+
 from .base import BaseConduit
 
 
 class LabelsConduit(BaseConduit):
     """A Rhino display conduit for labels.
 
     Parameters
@@ -74,18 +75,15 @@
     def color(self, color):
         if not color:
             return
         if not is_sequence_of_iterable(color[0]):
             # the first item in the list should be a tuple of colors
             # if not, wrap the tuple
             color = [color]
-        color = [
-            (FromArgb(*bg), FromArgb(*text))
-            for bg, text in iterable_like(self.labels, color, (self.default_color, self.default_textcolor))
-        ]
+        color = [(FromArgb(*bg), FromArgb(*text)) for bg, text in iterable_like(self.labels, color, (self.default_color, self.default_textcolor))]
         self._color = color
 
     def DrawForeground(self, e):
         """Draw the labels as text dots.
 
         Parameters
         ----------
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conduits/lines.py` & `compas-2.1.1/src/compas_rhino/conduits/lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
-
-from System.Drawing.Color import FromArgb
+from __future__ import print_function
 
 from Rhino.Geometry import Point3d
+from System.Drawing.Color import FromArgb
 
+from compas.itertools import iterable_like
 from compas.utilities import is_sequence_of_iterable
-from compas.utilities import iterable_like
+
 from .base import BaseConduit
 
 
 class LinesConduit(BaseConduit):
     """A Rhino display conduit for lines.
 
     Parameters
@@ -42,15 +42,15 @@
     Examples
     --------
     .. code-block:: python
 
         from random import randint
 
         points = [(1.0 * randint(0, 30), 1.0 * randint(0, 30), 0.0) for _ in range(100)]
-        lines  = [(points[i], points[i + 1]) for i in range(99)]
+        lines = [(points[i], points[i + 1]) for i in range(99)]
         conduit = LinesConduit(lines)
 
         with conduit.enabled():
             for i in range(100):
                 points = [(1.0 * randint(0, 30), 1.0 * randint(0, 30), 0.0) for _ in range(100)]
                 conduit.lines = [(points[i], points[i + 1]) for i in range(99)]
                 conduit.redraw(pause=0.1)
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conduits/points.py` & `compas-2.1.1/src/compas_rhino/conduits/points.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from System.Drawing.Color import FromArgb
-
-from Rhino.Geometry import Point3d
 from Rhino.Display.PointStyle import Simple
+from Rhino.Geometry import Point3d
+from System.Drawing.Color import FromArgb
 
+from compas.itertools import iterable_like
 from compas.utilities import color_to_rgb
-from compas.utilities import iterable_like
 from compas.utilities.coercing import is_sequence_of_iterable
+
 from .base import BaseConduit
 
 
 class PointsConduit(BaseConduit):
     """A Rhino display conduit for points.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conversions/__init__.py` & `compas-2.1.1/src/compas_rhino/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/conversions/breps.py` & `compas-2.1.1/src/compas_rhino/conversions/breps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from .exceptions import ConversionError
-
 from .shapes import cone_to_compas
 from .shapes import cylinder_to_compas
 from .shapes import sphere_to_compas
 
-
 # =============================================================================
 # To Rhino
 # =============================================================================
 
 
 def brep_to_rhino(brep):
     """Convert a COMPAS brep to a Rhino brep.
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conversions/curves.py` & `compas-2.1.1/src/compas_rhino/conversions/curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-import scriptcontext as sc  # type: ignore
 import Rhino  # type: ignore
+import scriptcontext as sc  # type: ignore
 
-from compas.geometry import Line
+from compas.geometry import Arc
 from compas.geometry import Circle
 from compas.geometry import Ellipse
-from compas.geometry import Polyline
-from compas.geometry import Arc
+from compas.geometry import Line
 from compas.geometry import NurbsCurve
+from compas.geometry import Polyline
 
 from .exceptions import ConversionError
-
-from .geometry import point_to_rhino
-from .geometry import plane_to_rhino
 from .geometry import frame_to_rhino_plane
-
-from .geometry import point_to_compas
 from .geometry import plane_to_compas
 from .geometry import plane_to_compas_frame
-
+from .geometry import plane_to_rhino
+from .geometry import point_to_compas
+from .geometry import point_to_rhino
 
 # =============================================================================
 # To Rhino
 # =============================================================================
 
 
 def data_to_rhino_curve(data):
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conversions/extrusions.py` & `compas-2.1.1/src/compas_rhino/conversions/extrusions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-import scriptcontext as sc  # type: ignore
 import Rhino  # type: ignore
+import scriptcontext as sc  # type: ignore
 
 from .shapes import box_to_compas
 from .shapes import cylinder_to_compas
 from .shapes import torus_to_compas
 
-
 # =============================================================================
 # To Rhino
 # =============================================================================
 
 # =============================================================================
 # To COMPAS
 # =============================================================================
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conversions/geometry.py` & `compas-2.1.1/src/compas_rhino/conversions/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import Rhino  # type: ignore
+from System import MissingMemberException  # type: ignore
 
-from compas.geometry import Point
-from compas.geometry import Vector
-from compas.geometry import Plane
 from compas.geometry import Frame
+from compas.geometry import Plane
+from compas.geometry import Point
 from compas.geometry import Polygon
-
+from compas.geometry import Vector
 
 # =============================================================================
 # To Rhino
 # =============================================================================
 
 
 def point_to_rhino(point):
@@ -100,22 +100,28 @@
 
 
 def point_to_compas(point):
     """Convert a Rhino point to a COMPAS point.
 
     Parameters
     ----------
-    point : :rhino:`Rhino.Geometry.Point3d`
+    point : :rhino:`Rhino.Geometry.Point3d` | :rhino:`Rhino.Geometry.Point`
 
     Returns
     -------
     :class:`compas.geometry.Point`
 
     """
-    return Point(point.X, point.Y, point.Z)
+    try:
+        return Point(point.X, point.Y, point.Z)
+    except MissingMemberException:
+        try:
+            return Point(point.Location.X, point.Location.Y, point.Location.Z)
+        except MissingMemberException:
+            raise TypeError("Unexpected point type, got: {}".format(type(point)))
 
 
 def vector_to_compas(vector):
     """Convert a Rhino vector to a COMPAS vector.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conversions/meshes.py` & `compas-2.1.1/src/compas_rhino/conversions/meshes.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 
 import Rhino  # type: ignore
 import System  # type: ignore
 
 from compas.colors import Color
 from compas.datastructures import Mesh
 from compas.geometry import centroid_polygon
-from compas.utilities import pairwise
+from compas.itertools import pairwise
+
 from .geometry import vector_to_compas
 
 
 def average_color(colors):
     c = len(colors)
     r, g, b = zip(*colors)
     r = sum(r) / c
     g = sum(g) / c
     b = sum(b) / c
-    return int(r), int(g), int(b)
+    return Color(int(r), int(g), int(b))
 
 
 def connected_ngon(face, vertices, rmesh):
     points = [vertices[index] for index in face]
     centroid = centroid_polygon(points)
 
     c = rmesh.Vertices.Add(*centroid)
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conversions/shapes.py` & `compas-2.1.1/src/compas_rhino/conversions/shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-import scriptcontext as sc  # type: ignore
 import Rhino  # type: ignore
+import scriptcontext as sc  # type: ignore
 
-from compas.geometry import Plane
-from compas.geometry import Circle
 from compas.geometry import Box
-from compas.geometry import Sphere
+from compas.geometry import Circle
 from compas.geometry import Cone
 from compas.geometry import Cylinder
-from compas.geometry import Torus
 from compas.geometry import Frame
+from compas.geometry import Plane
+from compas.geometry import Sphere
+from compas.geometry import Torus
+
+from .curves import circle_to_rhino
+from .curves import line_to_rhino_curve
 
 # from .geometry import plane_to_rhino
 from .geometry import frame_to_rhino
-from .geometry import point_to_rhino
-from .geometry import plane_to_compas_frame
 from .geometry import plane_to_compas
+from .geometry import plane_to_compas_frame
 from .geometry import point_to_compas
+from .geometry import point_to_rhino
 from .geometry import vector_to_compas
-from .curves import line_to_rhino_curve
-
-from .curves import circle_to_rhino
-
 
 # =============================================================================
 # To Rhino
 # =============================================================================
 
 
 def box_to_rhino(box):
@@ -163,17 +162,15 @@
     abs_tol = sc.doc.ModelAbsoluteTolerance
     ang_tol = sc.doc.ModelAngleToleranceRadians
 
     radius = capsule.radius
     line = capsule.axis
     curve = line_to_rhino_curve(line)
 
-    return Rhino.Geometry.Brep.CreatePipe(
-        curve, radius, False, Rhino.Geometry.PipeCapMode.Round, False, abs_tol, ang_tol
-    )
+    return Rhino.Geometry.Brep.CreatePipe(curve, radius, False, Rhino.Geometry.PipeCapMode.Round, False, abs_tol, ang_tol)
 
 
 def torus_to_rhino(torus):
     """Convert a COMPAS torus to a Rhino torus.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conversions/surfaces.py` & `compas-2.1.1/src/compas_rhino/conversions/surfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import Rhino  # type: ignore
 
-from compas.tolerance import TOL
-
-from compas.geometry import Point
-from compas.geometry import NurbsSurface
 from compas.datastructures import Mesh
+from compas.geometry import NurbsSurface
+from compas.geometry import Point
+from compas.tolerance import TOL
 from compas.utilities import memoize
 
 from .exceptions import ConversionError
-
-from .geometry import point_to_rhino
 from .geometry import point_to_compas
-
+from .geometry import point_to_rhino
 
 # =============================================================================
 # To Rhino
 # =============================================================================
 
 
 def surface_to_rhino(surface):
@@ -202,15 +199,14 @@
 
     >>> def facefilter(face):
     ...     success, w, h = face.GetSurfaceSize()
     ...     if success:
     ...         if w > 10 and h > 10:
     ...             return True
     ...     return False
-    ...
 
     >>> guid = compas_rhino.select_surface()
     >>> surf = Rhino.Geometry.Surface.from_guid(guid)
     >>> mesh = surf.to_compas(facefilter=facefilter)
 
     >>> scene = Scene()
     >>> scene.add(mesh, layer="Blocks")
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/conversions/transformations.py` & `compas-2.1.1/src/compas_rhino/conversions/transformations.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/__init__.py` & `compas-2.1.1/src/compas_rhino/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/booleans.py` & `compas-2.1.1/src/compas_rhino/geometry/booleans.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/brep/__init__.py` & `compas-2.1.1/src/compas_rhino/geometry/brep/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/brep/brep.py` & `compas-2.1.1/src/compas_rhino/geometry/brep/brep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import Rhino  # type: ignore
 
-from compas.geometry import Frame
 from compas.geometry import Brep
-from compas.geometry import BrepTrimmingError
 from compas.geometry import BrepError
+from compas.geometry import BrepTrimmingError
+from compas.geometry import Frame
 from compas.geometry import Plane
 from compas.geometry import Point
-
+from compas.tolerance import TOL
 from compas_rhino.conversions import box_to_rhino
-from compas_rhino.conversions import transformation_to_rhino
-from compas_rhino.conversions import plane_to_rhino
+from compas_rhino.conversions import curve_to_compas
+from compas_rhino.conversions import curve_to_rhino
 from compas_rhino.conversions import cylinder_to_rhino
-from compas_rhino.conversions import sphere_to_rhino
 from compas_rhino.conversions import mesh_to_compas
 from compas_rhino.conversions import mesh_to_rhino
+from compas_rhino.conversions import plane_to_rhino
 from compas_rhino.conversions import point_to_rhino
-from compas_rhino.conversions import curve_to_compas
-from compas_rhino.conversions import curve_to_rhino
+from compas_rhino.conversions import sphere_to_rhino
+from compas_rhino.conversions import transformation_to_rhino
 from compas_rhino.conversions import vector_to_rhino
 
 from .builder import _RhinoBrepBuilder
-from .face import RhinoBrepFace
 from .edge import RhinoBrepEdge
-from .vertex import RhinoBrepVertex
+from .face import RhinoBrepFace
 from .loop import RhinoBrepLoop
-
-TOLERANCE = 1e-6
+from .vertex import RhinoBrepVertex
 
 
 class RhinoBrep(Brep):
     """Rhino Brep backend class.
 
     Wraps around and allows serialization and de-serialization of a :class:`Rhino.Geometry.Brep`.
 
@@ -238,15 +236,15 @@
 
         """
         extrusion = Rhino.Geometry.Surface.CreateExtrusion(curve_to_rhino(curve), vector_to_rhino(vector))
         if extrusion is None:
             raise BrepError("Failed to create extrusion from curve: {} and vector: {}".format(curve, vector))
         rhino_brep = extrusion.ToBrep()
         if cap_ends:
-            capped = rhino_brep.CapPlanarHoles(TOLERANCE)
+            capped = rhino_brep.CapPlanarHoles(TOL.absolute)
             if capped:
                 rhino_brep = capped
         return cls.from_native(rhino_brep)
 
     @classmethod
     def from_sphere(cls, sphere):
         """Create a RhinoBrep from a sphere.
@@ -323,15 +321,15 @@
             True if the object is contained in the Brep, False otherwise.
 
         """
         if not self.is_solid:
             raise BrepError("Cannot check for containment if brep is not manifold or is not closed")
 
         if isinstance(object, Point):
-            return self._brep.IsPointInside(point_to_rhino(object), TOLERANCE, False)
+            return self._brep.IsPointInside(point_to_rhino(object), TOL.absolute, False)
         else:
             raise NotImplementedError
 
     def to_meshes(self, u=16, v=16):
         """Convert the faces of this Brep shape to meshes.
 
         Parameters
@@ -361,63 +359,86 @@
         Returns
         -------
         None
 
         """
         self._brep.Transform(transformation_to_rhino(matrix))
 
-    def trim(self, plane, tolerance=TOLERANCE):
+    def trim(self, plane, tolerance=None):
         """Trim this brep by the given trimming plane.
 
         Parameters
         ----------
         plane : :class:`compas.geometry.Frame` or :class:`compas.geometry.Plane`
             The frame or plane to use when trimming. The discarded bit is in the direction of the frame's normal.
+        tolerance : float, optional
+            The precision to use for the trimming operation. Defaults to `TOL.absolute`.
 
-        tolerance : float
-            The precision to use for the trimming operation.
+        Notes
+        -----
+        Trimming operation may result in multiple results (breps). When trimming, only one is used.
+        The used bit is the one on the opposite side of the cutting plane's normal.
 
         Returns
         -------
         None
 
-        """
-        results = self.trimmed(plane, tolerance)
-        if not results:
-            raise BrepTrimmingError("Trim operation ended with no result")
+        Raises
+        ------
+        BrepTrimmingError
+            If the trimming operation ended with no result.
 
-        self._brep = results[0].native_brep
+        See Also
+        --------
+        :meth:`compas_rhino.geometry.RhinoBrep.trimmed`
+
+        """
+        result = self.trimmed(plane, tolerance)
+        self._brep = result.native_brep
 
-    def trimmed(self, plane, tolerance=TOLERANCE):
+    def trimmed(self, plane, tolerance=None):
         """Returns a trimmed copy of this brep by the given trimming plane.
 
         Parameters
         ----------
         plane : :class:`compas.geometry.Frame` or :class:`compas.geometry.Plane`
             The frame or plane to use when trimming. The discarded bit is in the direction of the plane's normal.
+        tolerance : float, optional
+            The precision to use for the trimming operation. Defaults to `TOL.absolute`.
 
-        tolerance : float
-            The precision to use for the trimming operation.
+        Notes
+        -----
+        Trimming operation may result in multiple results (breps). When trimming, only one is used.
+        The used bit is the one on the opposite side of the cutting plane's normal.
 
         Returns
         -------
         :class:`~compas_rhino.geometry.RhinoBrep`
 
+        Raises
+        ------
+        BrepTrimmingError
+            If the trimming operation ended with no result.
+
+        See Also
+        --------
+        :meth:`compas_rhino.geometry.RhinoBrep.trim`
+
         """
+        tolerance = tolerance or TOL.absolute
         if isinstance(plane, Frame):
             plane = Plane.from_frame(plane)
         results = self._brep.Trim(plane_to_rhino(plane), tolerance)
-
-        breps = []
-        for result in results:
-            capped = result.CapPlanarHoles(TOLERANCE)
-            if capped:
-                result = capped
-            breps.append(RhinoBrep.from_native(result))
-        return breps
+        if not results:
+            raise BrepTrimmingError("Trim operation ended with no result")
+        result = results[0]
+        capped = result.CapPlanarHoles(tolerance)
+        if capped:
+            result = capped
+        return RhinoBrep.from_native(result)
 
     @classmethod
     def from_boolean_difference(cls, breps_a, breps_b):
         """Construct a Brep from the boolean difference of two groups of Breps.
 
         Parameters
         ----------
@@ -435,15 +456,15 @@
         if not isinstance(breps_a, list):
             breps_a = [breps_a]
         if not isinstance(breps_b, list):
             breps_b = [breps_b]
         resulting_breps = Rhino.Geometry.Brep.CreateBooleanDifference(
             [b.native_brep for b in breps_a],
             [b.native_brep for b in breps_b],
-            TOLERANCE,
+            TOL.absolute,
         )
         return [RhinoBrep.from_native(brep) for brep in resulting_breps]
 
     @classmethod
     def from_boolean_union(cls, breps_a, breps_b):
         """Construct a Brep from the boolean union of two groups of Breps.
 
@@ -461,15 +482,15 @@
 
         """
         if not isinstance(breps_a, list):
             breps_a = [breps_a]
         if not isinstance(breps_b, list):
             breps_b = [breps_b]
 
-        resulting_breps = Rhino.Geometry.Brep.CreateBooleanUnion([b.native_brep for b in breps_a + breps_b], TOLERANCE)
+        resulting_breps = Rhino.Geometry.Brep.CreateBooleanUnion([b.native_brep for b in breps_a + breps_b], TOL.absolute)
         return [RhinoBrep.from_native(brep) for brep in resulting_breps]
 
     @classmethod
     def from_boolean_intersection(cls, breps_a, breps_b):
         """Construct a Brep from the boolean intersection of two groups of Breps.
 
         Parameters
@@ -488,15 +509,15 @@
         if not isinstance(breps_a, list):
             breps_a = [breps_a]
         if not isinstance(breps_b, list):
             breps_b = [breps_b]
         resulting_breps = Rhino.Geometry.Brep.CreateBooleanIntersection(
             [b.native_brep for b in breps_a],
             [b.native_brep for b in breps_b],
-            TOLERANCE,
+            TOL.absolute,
         )
         return [RhinoBrep.from_native(brep) for brep in resulting_breps]
 
     def slice(self, plane):
         """Slice through the Brep with a plane.
 
         Parameters
@@ -509,15 +530,14 @@
         list(:class:`~compas.geometry.Curve`)
             Zero or more curves which represent the intersection(s) between the brep and the plane.
 
         """
         if isinstance(plane, Frame):
             plane = Plane.from_frame(plane)
         curves = Rhino.Geometry.Brep.CreateContourCurves(self._brep, plane_to_rhino(plane))
-        print("curves:{}".format(curves))
         return [curve_to_compas(curve) for curve in curves]
 
     def split(self, cutter):
         """Splits a Brep into pieces using a Brep as a cutter.
 
         Parameters
         ----------
@@ -526,9 +546,9 @@
 
         Returns
         -------
         list(:class:`compas_rhino.geometry.RhinoBrep`)
             list of zero or more resulting Breps.
 
         """
-        resulting_breps = self._brep.Split(cutter.native_brep, TOLERANCE)
+        resulting_breps = self._brep.Split(cutter.native_brep, TOL.absolute)
         return [RhinoBrep.from_native(brep) for brep in resulting_breps]
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/brep/builder.py` & `compas-2.1.1/src/compas_rhino/geometry/brep/builder.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/brep/edge.py` & `compas-2.1.1/src/compas_rhino/geometry/brep/edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import Rhino  # type: ignore
 
+from compas.geometry import Arc
 from compas.geometry import BrepEdge
-from compas.geometry import Line
 from compas.geometry import Circle
 from compas.geometry import Ellipse
 from compas.geometry import Frame
-from compas.geometry import Arc
-
-from compas_rhino.geometry import RhinoNurbsCurve
-from compas_rhino.conversions import curve_to_compas_line
-from compas_rhino.conversions import plane_to_compas_frame
+from compas.geometry import Line
+from compas_rhino.conversions import arc_to_compas
+from compas_rhino.conversions import arc_to_rhino
 from compas_rhino.conversions import circle_to_compas
+from compas_rhino.conversions import circle_to_rhino
+from compas_rhino.conversions import curve_to_compas_line
 from compas_rhino.conversions import ellipse_to_compas
 from compas_rhino.conversions import ellipse_to_rhino
-from compas_rhino.conversions import circle_to_rhino
 from compas_rhino.conversions import frame_to_rhino_plane
 from compas_rhino.conversions import line_to_rhino
-from compas_rhino.conversions import arc_to_compas
-from compas_rhino.conversions import arc_to_rhino
+from compas_rhino.conversions import plane_to_compas_frame
 from compas_rhino.conversions import point_to_compas
+from compas_rhino.geometry import RhinoNurbsCurve
 
 from .vertex import RhinoBrepVertex
 
 
 class RhinoBrepEdge(BrepEdge):
     """A wrapper for Rhino.Geometry.BrepEdge.
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/brep/face.py` & `compas-2.1.1/src/compas_rhino/geometry/brep/face.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,29 @@
 from __future__ import division
 from __future__ import print_function
 
 import Rhino  # type: ignore
 
 from compas.geometry import Brep
 from compas.geometry import BrepFace
-from compas.geometry import Sphere
 from compas.geometry import Cylinder
 from compas.geometry import Frame
+from compas.geometry import Sphere
 from compas.geometry import SurfaceType
-
-
-from compas_rhino.geometry import RhinoNurbsSurface
-from compas_rhino.geometry.surfaces import RhinoSurface
-from compas_rhino.conversions import plane_to_compas_frame
-from compas_rhino.conversions import sphere_to_compas
 from compas_rhino.conversions import cylinder_to_compas
 from compas_rhino.conversions import cylinder_to_rhino
-from compas_rhino.conversions import sphere_to_rhino
 from compas_rhino.conversions import frame_to_rhino_plane
+from compas_rhino.conversions import plane_to_compas_frame
+from compas_rhino.conversions import sphere_to_compas
+from compas_rhino.conversions import sphere_to_rhino
+from compas_rhino.geometry import RhinoNurbsSurface
+from compas_rhino.geometry.surfaces import RhinoSurface
 
-from .loop import RhinoBrepLoop
 from .edge import RhinoBrepEdge
+from .loop import RhinoBrepLoop
 
 
 class RhinoBrepFace(BrepFace):
     """A wrapper for Rhino.Geometry.BrepFace
 
     Attributes
     ----------
@@ -85,17 +83,15 @@
         -------
         :class:`compas.data.Data`
             An instance of this object type if the data contained in the dict has the correct schema.
 
         """
 
         instance = cls()
-        instance._surface = instance._make_surface__from_data__(
-            data["surface_type"], data["surface"], data["uv_domain"], data["frame"]
-        )
+        instance._surface = instance._make_surface__from_data__(data["surface_type"], data["surface"], data["uv_domain"], data["frame"])
         face_builder = builder.add_face(instance._surface)
         for loop_data in data["loops"]:
             RhinoBrepLoop.__from_data__(loop_data, face_builder)
         instance.native_face = face_builder.result
         return instance
 
     # ==============================================================================
@@ -210,17 +206,15 @@
             success, cast_surface = surface.TryGetSphere()
             if success:
                 return "sphere", sphere_to_compas(cast_surface), uv_domain, cast_surface.EquatorialPlane
             success, cast_surface = surface.TryGetCylinder()
             if success:
                 return "cylinder", cylinder_to_compas(cast_surface), uv_domain, cast_surface.BasePlane
             success, cast_surface = surface.TryGetTorus()
-        raise NotImplementedError(
-            "Support for surface type: {} is not yet implemented.".format(surface.__class__.__name__)
-        )
+        raise NotImplementedError("Support for surface type: {} is not yet implemented.".format(surface.__class__.__name__))
 
     def _make_surface__from_data__(self, surface_type, surface_data, uv_domain, frame_data):
         u_domain, v_domain = uv_domain
         frame = Frame.__from_data__(frame_data)  # workaround until all shapes have a frame
         if surface_type == "plane":
             frame = Frame.__from_data__(surface_data)  # redundancy in shapes which already have a frame
             surface = RhinoSurface.from_frame(frame, u_domain, v_domain)
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/brep/loop.py` & `compas-2.1.1/src/compas_rhino/geometry/brep/loop.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from __future__ import division
 from __future__ import print_function
 
 import Rhino  # type: ignore
 
 from compas.geometry import BrepLoop
 
-from .trim import RhinoBrepTrim
 from .edge import RhinoBrepEdge
+from .trim import RhinoBrepTrim
 
 
 class LoopType(object):
     """Represents the type of a brep loop.
 
     Attributes
     ----------
@@ -83,17 +83,15 @@
         Returns
         -------
         :class:`compas.data.Data`
             An instance of this object type if the data contained in the dict has the correct schema.
 
         """
         instance = cls()
-        instance._type = (
-            Rhino.Geometry.BrepLoopType.Outer if data["type"] == "Outer" else Rhino.Geometry.BrepLoopType.Inner
-        )
+        instance._type = Rhino.Geometry.BrepLoopType.Outer if data["type"] == "Outer" else Rhino.Geometry.BrepLoopType.Inner
         loop_builder = builder.add_loop(instance._type)
         for trim_data in data["trims"]:
             RhinoBrepTrim.__from_data__(trim_data, loop_builder)
         instance.native_loop = loop_builder.result
         return instance
 
     # ==============================================================================
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/brep/trim.py` & `compas-2.1.1/src/compas_rhino/geometry/brep/trim.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/brep/vertex.py` & `compas-2.1.1/src/compas_rhino/geometry/brep/vertex.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-from compas.geometry import Point
 from compas.geometry import BrepVertex
+from compas.geometry import Point
 from compas_rhino.conversions import point_to_compas
 
 
 class RhinoBrepVertex(BrepVertex):
     """A wrapper for a Rhino Brep vertex.
 
     Attributes
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/curves/__init__.py` & `compas-2.1.1/src/compas_rhino/geometry/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/curves/curve.py` & `compas-2.1.1/src/compas_rhino/geometry/curves/curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from compas.geometry import Curve
 from compas.geometry import Plane
-
-from compas_rhino.conversions import point_to_rhino
-from compas_rhino.conversions import point_to_compas
-from compas_rhino.conversions import vector_to_compas
-from compas_rhino.conversions import transformation_to_rhino
+from compas_rhino.conversions import box_to_compas
 from compas_rhino.conversions import plane_to_compas_frame
 from compas_rhino.conversions import plane_to_rhino
-from compas_rhino.conversions import box_to_compas
+from compas_rhino.conversions import point_to_compas
+from compas_rhino.conversions import point_to_rhino
+from compas_rhino.conversions import transformation_to_rhino
+from compas_rhino.conversions import vector_to_compas
 
 
 class RhinoCurve(Curve):
     """Class representing a general curve object.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/curves/nurbs.py` & `compas-2.1.1/src/compas_rhino/geometry/curves/nurbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from itertools import groupby
 
 import Rhino.Geometry  # type: ignore
 
-from compas.geometry import Point
 from compas.geometry import NurbsCurve
-
-from compas_rhino.conversions import point_to_rhino
-from compas_rhino.conversions import point_to_compas
+from compas.geometry import Point
 from compas_rhino.conversions import line_to_rhino
+from compas_rhino.conversions import point_to_compas
+from compas_rhino.conversions import point_to_rhino
 
 from .curve import RhinoCurve
 
 
 def rhino_curve_from_parameters(points, weights, knots, multiplicities, degree):
     rhino_curve = Rhino.Geometry.NurbsCurve(3, True, degree + 1, len(points))
     for index, (point, weight) in enumerate(zip(points, weights)):
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/surfaces/__init__.py` & `compas-2.1.1/src/compas_rhino/geometry/surfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/surfaces/nurbs.py` & `compas-2.1.1/src/compas_rhino/geometry/surfaces/nurbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from itertools import groupby
 
 import Rhino.Geometry  # type: ignore
 
-from compas.geometry import Point
 from compas.geometry import NurbsSurface
+from compas.geometry import Point
 from compas.geometry import knots_and_mults_to_knotvector
-from compas.utilities import flatten
-
-from compas_rhino.conversions import point_to_rhino
+from compas.itertools import flatten
 from compas_rhino.conversions import point_to_compas
+from compas_rhino.conversions import point_to_rhino
 
 from .surface import RhinoSurface
 
 
 class ControlPoints(object):
     def __init__(self, surface):
         self.rhino_surface = surface
@@ -307,17 +306,15 @@
 
         Returns
         -------
         :class:`compas_rhino.geometry.RhinoNurbsSurface`
 
         """
         surface = cls()
-        surface.rhino_surface = rhino_surface_from_parameters(
-            points, weights, knots_u, knots_v, mults_u, mults_v, degree_u, degree_v
-        )
+        surface.rhino_surface = rhino_surface_from_parameters(points, weights, knots_u, knots_v, mults_u, mults_v, degree_u, degree_v)
         return surface
 
     @classmethod
     def from_points(cls, points, degree_u=3, degree_v=3):
         """Construct a NURBS surface from control points.
 
         Parameters
@@ -338,17 +335,15 @@
         # with the current convention this should not be needed.
         points = list(zip(*points))
 
         pointcount_u = len(points)
         pointcount_v = len(points[0])
         points[:] = [point_to_rhino(point) for row in points for point in row]
         surface = cls()
-        surface.rhino_surface = Rhino.Geometry.NurbsSurface.CreateFromPoints(
-            points, pointcount_u, pointcount_v, degree_u, degree_v
-        )
+        surface.rhino_surface = Rhino.Geometry.NurbsSurface.CreateFromPoints(points, pointcount_u, pointcount_v, degree_u, degree_v)
         return surface
 
     @classmethod
     def from_fill(cls, curve1, curve2):
         """Construct a NURBS surface from the infill between two NURBS curves.
 
         Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/surfaces/surface.py` & `compas-2.1.1/src/compas_rhino/geometry/surfaces/surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import Rhino.Geometry  # type: ignore
 
 from compas.geometry import Surface
-
-from compas_rhino.conversions import point_to_rhino
-from compas_rhino.conversions import point_to_compas
-from compas_rhino.conversions import vector_to_compas
-from compas_rhino.conversions import plane_to_compas_frame
+from compas_rhino.conversions import box_to_compas
+from compas_rhino.conversions import cylinder_to_rhino
 from compas_rhino.conversions import frame_to_rhino_plane
+from compas_rhino.conversions import plane_to_compas_frame
 from compas_rhino.conversions import plane_to_rhino
-from compas_rhino.conversions import box_to_compas
-from compas_rhino.conversions import transformation_to_rhino
+from compas_rhino.conversions import point_to_compas
+from compas_rhino.conversions import point_to_rhino
 from compas_rhino.conversions import sphere_to_rhino
-from compas_rhino.conversions import cylinder_to_rhino
-
+from compas_rhino.conversions import transformation_to_rhino
+from compas_rhino.conversions import vector_to_compas
 from compas_rhino.geometry.curves import RhinoCurve
 
 
 class RhinoSurface(Surface):
     """Class representing a general surface object.
 
     Attributes
@@ -396,16 +394,14 @@
         line : :class:`compas.geometry.Curve`
 
         Returns
         -------
         list[:class:`compas.geometry.Point`]
 
         """
-        intersections = Rhino.Geometry.Intersect.Intersection.CurveSurface(
-            curve.rhino_curve, self.rhino_surface, tolerance, overlap
-        )
+        intersections = Rhino.Geometry.Intersect.Intersection.CurveSurface(curve.rhino_curve, self.rhino_surface, tolerance, overlap)
         points = []
         for event in intersections:
             if event.IsPoint:
                 point = point_to_compas(event.PointA)
                 points.append(point)
         return points
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/trimesh_curvature.py` & `compas-2.1.1/src/compas_rhino/geometry/trimesh_curvature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-import Rhino  # type: ignore
-import System  # type: ignore
-import clr  # type: ignore
-import scriptcontext  # type: ignore
-
+from math import atan2
 from math import pi
 from math import sqrt
-from math import atan2
+
+import clr  # type: ignore
+import Rhino  # type: ignore
+import scriptcontext  # type: ignore
+import System  # type: ignore
 
 from compas.plugins import plugin
 
 
 @plugin(category="trimesh", requires=["Rhino"])
 def trimesh_gaussian_curvature(M):
     r"""Compute the discrete Gaussian curvature of a triangle mesh.
@@ -77,17 +77,15 @@
 
     # (2) Prepare ingredient and return list
     pi_2 = 2 * pi
     K = []
 
     # (3) Main - loop every vertex for angle defect
     for i in range(mesh.Vertices.Count):
-        vert_neighbors_topo = mesh.TopologyVertices.ConnectedTopologyVertices(
-            mesh.TopologyVertices.TopologyVertexIndex(i), True
-        )
+        vert_neighbors_topo = mesh.TopologyVertices.ConnectedTopologyVertices(mesh.TopologyVertices.TopologyVertexIndex(i), True)
         vert_neighbors = []
         if vert_neighbors_topo is None:
             K.append(None)
             continue
         for vert in vert_neighbors_topo:
             vert_neighbors.extend(mesh.TopologyVertices.MeshVertexIndices(vert))
         angles = []
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/geometry/trimesh_slicing.py` & `compas-2.1.1/src/compas_rhino/geometry/trimesh_slicing.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/install.py` & `compas-2.1.1/src/compas_rhino/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from __future__ import print_function
 
 import importlib
 import itertools
 import os
 import sys
 
-import compas_rhino
-
 import compas._os
 import compas.plugins
+import compas_rhino
 
 
 def install(version=None, packages=None, clean=False):
     """Install COMPAS for Rhino.
 
     Parameters
     ----------
@@ -30,14 +29,15 @@
         also existing symlinks that are not importable in the current environment.
 
     Examples
     --------
     .. code-block:: python
 
         import compas_rhino.install
+
         compas_rhino.install.install()
 
     .. code-block:: bash
 
         python -m compas_rhino.install
 
     """
@@ -238,17 +238,15 @@
             try:
                 package, message, success = item
                 status = "OK" if success else "ERROR"
                 if not success:
                     all_steps_succeeded = False
                 print("   {} {}: {}".format(package.ljust(20), status, message))
             except ValueError:
-                post_execution_errors.append(
-                    ValueError("Step ran without errors but result is wrongly formatted: {}".format(str(item)))
-                )
+                post_execution_errors.append(ValueError("Step ran without errors but result is wrongly formatted: {}".format(str(item))))
 
     if post_execution_errors:
         print("\nOne or more errors occurred:\n")
         for error in post_execution_errors:
             print("   - {}".format(repr(error)))
 
         all_steps_succeeded = False
@@ -272,17 +270,17 @@
     can implement this pluggable interface to automatically
     have their packages made available inside Rhino when
     COMPAS is installed into it.
 
     Examples
     --------
     >>> import compas.plugins
-    >>> @compas.plugins.plugin(category='install')
+    >>> @compas.plugins.plugin(category="install")
     ... def installable_rhino_packages():
-    ...    return ['compas_fab']
+    ...     return ["compas_fab"]
 
     Returns
     -------
     :obj:`list` of :obj:`str`
         List of package names to make available inside Rhino.
     """
     pass
@@ -301,18 +299,18 @@
     ----------
     installed_packages : :obj:`list` of :obj:`str`
         List of packages that have been installed successfully.
 
     Examples
     --------
     >>> import compas.plugins
-    >>> @compas.plugins.plugin(category='install')
+    >>> @compas.plugins.plugin(category="install")
     ... def after_rhino_install(installed_packages):
-    ...    # Do something after package is installed to Rhino, eg, copy components, etc
-    ...    return [('compas_ghpython', 'GH Components installed', True)]
+    ...     # Do something after package is installed to Rhino, eg, copy components, etc
+    ...     return [("compas_ghpython", "GH Components installed", True)]
 
     Returns
     -------
     :obj:`list` of 3-tuple (str, str, bool)
         List containing a 3-tuple with component name, message and True/False success flag.
     """
     pass
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/install_plugin.py` & `compas-2.1.1/src/compas_rhino/install_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import os
 import imp
+import os
 
 import compas_rhino
-
 from compas._os import create_symlinks
 from compas._os import remove_symlinks
+
 from .install import install as install_packages
 
 
 def install_plugin(plugin, version=None):
     """Install a Rhino Python Command Plugin.
 
     Parameters
@@ -147,15 +147,14 @@
 
 
 # ==============================================================================
 # Main
 # ==============================================================================
 
 if __name__ == "__main__":
-
     import argparse
 
     parser = argparse.ArgumentParser(description="COMPAS Rhino Plugin Installation command-line utility.")
 
     parser.add_argument("plugin", help="The path to the plugin directory.")
     parser.add_argument(
         "-v",
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/layers.py` & `compas-2.1.1/src/compas_rhino/layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from collections import deque
 
 import rhinoscriptsyntax as rs  # type: ignore
 import scriptcontext as sc  # type: ignore
 
 find_object = sc.doc.Objects.Find
@@ -121,20 +121,22 @@
         * Graph
       * Geometry
         * Point
         * Vector
 
     .. code-block:: python
 
-        create_layers_from_paths([
-            "COMPAS::Datastructures::Mesh",
-            "COMPAS::Datastructures::Graph",
-            "COMPAS::Geometry::Point",
-            "COMPAS::Geometry::Vector",
-        ])
+        create_layers_from_paths(
+            [
+                "COMPAS::Datastructures::Mesh",
+                "COMPAS::Datastructures::Graph",
+                "COMPAS::Geometry::Point",
+                "COMPAS::Geometry::Vector",
+            ]
+        )
 
     """
     for name in names:
         create_layers_from_path(name, separator=separator)
 
 
 def create_layers_from_dict(layers):
@@ -151,24 +153,23 @@
     -------
     None
 
     Examples
     --------
     .. code-block:: python
 
-        layers = {'COMPAS', {'layers': {
-            'Datastructures': {'color': (255, 0, 0), 'layers': {
-                'Mesh': {},
-                'Graph': {}
-            }},
-            'Geometry': {'color': (0, 0, 255),'layers': {
-                'Point': {},
-                'Vector': {}
-            }},
-        }}}
+        layers = {
+            "COMPAS",
+            {
+                "layers": {
+                    "Datastructures": {"color": (255, 0, 0), "layers": {"Mesh": {}, "Graph": {}}},
+                    "Geometry": {"color": (0, 0, 255), "layers": {"Point": {}, "Vector": {}}},
+                }
+            },
+        }
 
         create_layers_from_dict(layers)
 
     """
 
     def recurse(layers, parent=None):
         for name in layers:
@@ -303,20 +304,20 @@
     -------
     None
 
     Examples
     --------
     .. code-block:: python
 
-        layers = {'COMPAS': {'layers': {'Datastructures': {'layers': {'Mesh': {}, 'Graph': {}}}}}}
+        layers = {"COMPAS": {"layers": {"Datastructures": {"layers": {"Mesh": {}, "Graph": {}}}}}}
 
         create_layers(layers)
 
-        delete_layers(['COMPAS::Datastructures::Graph'])
-        delete_layers({'COMPAS': {'layers': {'Datastructures': {'layers': {'Mesh': {}}}}}})
+        delete_layers(["COMPAS::Datastructures::Graph"])
+        delete_layers({"COMPAS": {"layers": {"Datastructures": {"layers": {"Mesh": {}}}}}})
 
     """
     to_delete = []
 
     def recurse(layers, parent=None):
         for name in layers:
             if not name:
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/objects.py` & `compas-2.1.1/src/compas_rhino/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import json
 
-import compas_rhino
-
-import System  # type: ignore
 import Rhino  # type: ignore
 import rhinoscriptsyntax as rs  # type: ignore
 import scriptcontext as sc  # type: ignore
+import System  # type: ignore
+
+import compas_rhino
 
 find_object = sc.doc.Objects.Find
 
 try:
     purge_object = sc.doc.Objects.Purge
 except AttributeError:
     purge_object = None
@@ -46,15 +46,15 @@
     Examples
     --------
     .. code-block:: python
 
         import compas_rhino
 
         guids_all = compas_rhino.get_objects()
-        guids_compas = compas_rhino.get_objects(name='COMPAS.*')
+        guids_compas = compas_rhino.get_objects(name="COMPAS.*")
         guids_red = compas_rhino.get_objects(color=(255, 0, 0))
         guids_points = compas_rhino.get_objects(type=compas_rhino.rs.filter.point)
         guids_redpoints = compas_rhino.get_objects(color=(255, 0, 0), type=compas_rhino.rs.filter.point)
 
     .. code-block:: python
 
         guids_all = set(compas_rhino.get_objects())
@@ -294,19 +294,15 @@
     """
     o = find_object(guid)
     u = o.Attributes.UserDictionary
     for name, value in iter(attr.items()):
         try:
             u.Set(name, value)
         except Exception:
-            print(
-                "The following item cannot be stored in the user dictionary of this object: {0} => {1}".format(
-                    name, value
-                )
-            )
+            print("The following item cannot be stored in the user dictionary of this object: {0} => {1}".format(name, value))
 
 
 def get_object_attributes_from_name(guids, prefix=None):
     """Get attributes from JSON parsable object names.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/__init__.py` & `compas-2.1.1/src/compas_rhino/scene/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/boxobject.py` & `compas-2.1.1/src/compas_rhino/scene/boxobject.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import box_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoBoxObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing box shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/brepobject.py` & `compas-2.1.1/src/compas_rhino/scene/brepobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
+from compas.scene import GeometryObject
 from compas_rhino.conversions import brep_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
-from compas.scene import GeometryObject
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoBrepObject(RhinoSceneObject, GeometryObject):
     """A scene object for drawing a RhinoBrep.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/capsuleobject.py` & `compas-2.1.1/src/compas_rhino/scene/capsuleobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import capsule_to_rhino_brep
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoCapsuleObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing capsule shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/circleobject.py` & `compas-2.1.1/src/compas_rhino/scene/coneobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
-from compas_rhino.conversions import circle_to_rhino
+from compas_rhino.conversions import cone_to_rhino_brep
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
-class RhinoCircleObject(RhinoSceneObject, GeometryObject):
-    """Scene object for drawing circles.
+class RhinoConeObject(RhinoSceneObject, GeometryObject):
+    """Scene object for drawing cone shapes.
 
     Parameters
     ----------
-    circle : :class:`compas.geometry.Circle`
-        A COMPAS circle.
+    shape : :class:`compas.geometry.Cone`
+        A COMPAS cone.
     **kwargs : dict, optional
         Additional keyword arguments.
 
     """
 
-    def __init__(self, circle, **kwargs):
-        super(RhinoCircleObject, self).__init__(geometry=circle, **kwargs)
+    def __init__(self, cone, **kwargs):
+        super(RhinoConeObject, self).__init__(geometry=cone, **kwargs)
 
     def draw(self):
-        """Draw the circle.
+        """Draw the cone associated with the scene object.
 
         Returns
         -------
-        list[System.Guid]
-            List of GUIDs of the objects created in Rhino.
+        System.Guid
+            The GUID of the object created in Rhino.
 
         """
         attr = self.compile_attributes()
-        geometry = circle_to_rhino(self.geometry)
+        geometry = cone_to_rhino_brep(self.geometry)
         geometry.Transform(transformation_to_rhino(self.worldtransformation))
 
-        self._guids = [sc.doc.Objects.AddCircle(geometry, attr)]
+        self._guids = [sc.doc.Objects.AddBrep(geometry, attr)]
         return self.guids
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/coneobject.py` & `compas-2.1.1/src/compas_rhino/scene/sphereobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
-from compas_rhino.conversions import cone_to_rhino_brep
+from compas_rhino.conversions import sphere_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
-class RhinoConeObject(RhinoSceneObject, GeometryObject):
-    """Scene object for drawing cone shapes.
+class RhinoSphereObject(RhinoSceneObject, GeometryObject):
+    """Scene object for drawing sphere shapes.
 
     Parameters
     ----------
-    shape : :class:`compas.geometry.Cone`
-        A COMPAS cone.
+    sphere : :class:`compas.geometry.Sphere`
+        A COMPAS sphere.
     **kwargs : dict, optional
         Additional keyword arguments.
 
     """
 
-    def __init__(self, cone, **kwargs):
-        super(RhinoConeObject, self).__init__(geometry=cone, **kwargs)
+    def __init__(self, sphere, **kwargs):
+        super(RhinoSphereObject, self).__init__(geometry=sphere, **kwargs)
 
     def draw(self):
-        """Draw the cone associated with the scene object.
+        """Draw the sphere associated with the scene object.
 
         Returns
         -------
-        System.Guid
-            The GUID of the object created in Rhino.
+        list[System.Guid]
+            The GUIDs of the objects created in Rhino.
 
         """
         attr = self.compile_attributes()
-        geometry = cone_to_rhino_brep(self.geometry)
+        geometry = sphere_to_rhino(self.geometry)
         geometry.Transform(transformation_to_rhino(self.worldtransformation))
 
-        self._guids = [sc.doc.Objects.AddBrep(geometry, attr)]
+        self._guids = [sc.doc.Objects.AddSphere(geometry, attr)]
         return self.guids
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/curveobject.py` & `compas-2.1.1/src/compas_rhino/scene/curveobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import curve_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoCurveObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing curves.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/cylinderobject.py` & `compas-2.1.1/src/compas_rhino/scene/cylinderobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import cylinder_to_rhino_brep
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoCylinderObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing cylinder shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/ellipseobject.py` & `compas-2.1.1/src/compas_rhino/scene/ellipseobject.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import ellipse_to_rhino
-
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoEllipseObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing ellipses.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/frameobject.py` & `compas-2.1.1/src/compas_rhino/scene/frameobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
-from compas.scene import GeometryObject
 from compas.colors import Color
+from compas.scene import GeometryObject
 from compas_rhino.conversions import point_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoFrameObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing frames.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/graphobject.py` & `compas-2.1.1/src/compas_rhino/scene/graphobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import Rhino  # type: ignore
 import scriptcontext as sc  # type: ignore
 
 import compas_rhino
-from compas.geometry import Line
 from compas.geometry import Cylinder
+from compas.geometry import Line
 from compas.geometry import Sphere
 from compas.scene import GraphObject
-from compas_rhino.conversions import point_to_rhino
+from compas_rhino.conversions import cylinder_to_rhino_brep
 from compas_rhino.conversions import line_to_rhino
+from compas_rhino.conversions import point_to_rhino
 from compas_rhino.conversions import sphere_to_rhino
-from compas_rhino.conversions import cylinder_to_rhino_brep
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoGraphObject(RhinoSceneObject, GraphObject):
     """Scene object for drawing graph data structures.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/helpers.py` & `compas-2.1.1/src/compas_rhino/scene/helpers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import rhinoscriptsyntax as rs  # type: ignore
 import scriptcontext as sc  # type: ignore
 
 from compas_rhino.layers import create_layers_from_path
 
 try:
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/lineobject.py` & `compas-2.1.1/src/compas_rhino/scene/lineobject.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import line_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoLineObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing lines.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/meshobject.py` & `compas-2.1.1/src/compas_rhino/scene/meshobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-import scriptcontext as sc  # type: ignore
 import Rhino  # type: ignore
+import scriptcontext as sc  # type: ignore
 
-from compas.geometry import centroid_points
-from compas.geometry import Point
-from compas.geometry import Line
+import compas_rhino.objects
+from compas.colors import Color
 from compas.geometry import Cylinder
+from compas.geometry import Line
+from compas.geometry import Point
 from compas.geometry import Sphere
+from compas.geometry import centroid_points
 from compas.scene import MeshObject
-from compas.colors import Color
-
-import compas_rhino.objects
-from compas_rhino.conversions import vertices_and_faces_to_rhino
+from compas_rhino.conversions import cylinder_to_rhino_brep
+from compas_rhino.conversions import line_to_rhino
 from compas_rhino.conversions import mesh_to_rhino
 from compas_rhino.conversions import point_to_rhino
-from compas_rhino.conversions import line_to_rhino
-from compas_rhino.conversions import cylinder_to_rhino_brep
 from compas_rhino.conversions import sphere_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+from compas_rhino.conversions import vertices_and_faces_to_rhino
 
-from .sceneobject import RhinoSceneObject
 from .helpers import ngon
+from .sceneobject import RhinoSceneObject
 
 
 class RhinoMeshObject(RhinoSceneObject, MeshObject):
     """Scene object for drawing mesh data structures.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/planeobject.py` & `compas-2.1.1/src/compas_rhino/scene/planeobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
+from compas.geometry import Frame
 from compas.scene import GeometryObject
-from .sceneobject import RhinoSceneObject
 from compas_rhino.conversions import point_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
 from compas_rhino.conversions import vertices_and_faces_to_rhino
-from compas.geometry import Frame
+
+from .sceneobject import RhinoSceneObject
 
 
 class RhinoPlaneObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing planes.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/pointobject.py` & `compas-2.1.1/src/compas_rhino/scene/pointobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import point_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoPointObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing points.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/polygonobject.py` & `compas-2.1.1/src/compas_rhino/scene/polygonobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
-from compas_rhino.conversions import vertices_and_faces_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+from compas_rhino.conversions import vertices_and_faces_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoPolygonObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing polygons.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/polyhedronobject.py` & `compas-2.1.1/src/compas_rhino/scene/polyhedronobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
-from compas_rhino.conversions import vertices_and_faces_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+from compas_rhino.conversions import vertices_and_faces_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoPolyhedronObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing polyhedron shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/polylineobject.py` & `compas-2.1.1/src/compas_rhino/scene/polylineobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import polyline_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoPolylineObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing polylines.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/sceneobject.py` & `compas-2.1.1/src/compas_rhino/scene/sceneobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-import scriptcontext as sc  # type: ignore
 import Rhino  # type: ignore
+import scriptcontext as sc  # type: ignore
 import System  # type: ignore
 
 import compas_rhino.layers
 from compas.scene import SceneObject
+
 from .helpers import ensure_layer
 
 
 class RhinoSceneObject(SceneObject):
     """Base class for all Rhino scene objects.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/sphereobject.py` & `compas-2.1.1/src/compas_rhino/scene/vectorobject.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,49 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
+from compas.geometry import Point
 from compas.scene import GeometryObject
-from compas_rhino.conversions import sphere_to_rhino
+from compas_rhino.conversions import point_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
-class RhinoSphereObject(RhinoSceneObject, GeometryObject):
-    """Scene object for drawing sphere shapes.
+class RhinoVectorObject(RhinoSceneObject, GeometryObject):
+    """Scene object for drawing vectors.
 
     Parameters
     ----------
-    sphere : :class:`compas.geometry.Sphere`
-        A COMPAS sphere.
+    vector : :class:`compas.geometry.Vector`
+        A COMPAS vector.
     **kwargs : dict, optional
         Additional keyword arguments.
 
     """
 
-    def __init__(self, sphere, **kwargs):
-        super(RhinoSphereObject, self).__init__(geometry=sphere, **kwargs)
+    def __init__(self, vector, **kwargs):
+        super(RhinoVectorObject, self).__init__(geometry=vector, **kwargs)
 
     def draw(self):
-        """Draw the sphere associated with the scene object.
+        """Draw the vector.
 
         Returns
         -------
         list[System.Guid]
-            The GUIDs of the objects created in Rhino.
+            List of GUIDs of the objects created in Rhino.
 
         """
-        attr = self.compile_attributes()
-        geometry = sphere_to_rhino(self.geometry)
-        geometry.Transform(transformation_to_rhino(self.worldtransformation))
+        attr = self.compile_attributes(arrow="end")
+        start = Point(0, 0, 0)
+        end = start + self.geometry
+        start_geometry = point_to_rhino(start)
+        end_geometry = point_to_rhino(end)
+        transformation = transformation_to_rhino(self.worldtransformation)
+        start_geometry.Transform(transformation)
+        end_geometry.Transform(transformation)
 
-        self._guids = [sc.doc.Objects.AddSphere(geometry, attr)]
+        self._guids = [sc.doc.Objects.AddLine(start_geometry, end_geometry, attr)]
         return self.guids
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/surfaceobject.py` & `compas-2.1.1/src/compas_rhino/scene/surfaceobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import surface_to_rhino
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoSurfaceObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing surfaces.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/torusobject.py` & `compas-2.1.1/src/compas_rhino/scene/torusobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import scriptcontext as sc  # type: ignore
 
 from compas.scene import GeometryObject
 from compas_rhino.conversions import torus_to_rhino_brep
 from compas_rhino.conversions import transformation_to_rhino
+
 from .sceneobject import RhinoSceneObject
 
 
 class RhinoTorusObject(RhinoSceneObject, GeometryObject):
     """Scene object for drawing torus shapes.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/scene/volmeshobject.py` & `compas-2.1.1/src/compas_rhino/scene/volmeshobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
-from Rhino.Geometry import TextDot  # type: ignore
 import scriptcontext as sc  # type: ignore
+from Rhino.Geometry import TextDot  # type: ignore
 
-from compas.geometry import centroid_points
+import compas_rhino.objects
 from compas.geometry import Line
+from compas.geometry import centroid_points
 from compas.scene import VolMeshObject
-
-import compas_rhino.objects
-from compas_rhino.conversions import point_to_rhino
 from compas_rhino.conversions import line_to_rhino
+from compas_rhino.conversions import point_to_rhino
 from compas_rhino.conversions import vertices_and_faces_to_rhino
 
-from .sceneobject import RhinoSceneObject
 from .helpers import ngon
+from .sceneobject import RhinoSceneObject
 
 
 class RhinoVolMeshObject(RhinoSceneObject, VolMeshObject):
     """Scene object for drawing volmesh data structures.
 
     Parameters
     ----------
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/ui.py` & `compas-2.1.1/src/compas_rhino/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import os
+
 import rhinoscriptsyntax as rs  # type: ignore
 
 
 def toggle_toolbargroup(rui, group):
     if not os.path.exists(rui) or not os.path.isfile(rui):
         return
     collection = rs.IsToolbarCollection(rui)
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/uninstall.py` & `compas-2.1.1/src/compas_rhino/uninstall.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         Default is to uninstall all packages installed by the COMPAS installer.
 
     Examples
     --------
     .. code-block:: python
 
         import compas_rhino
+
         compas_rhino.uninstall()
 
     .. code-block:: bash
 
         python -m compas_rhino.uninstall
 
     """
@@ -201,18 +202,18 @@
     ----------
     uninstalled_packages : :obj:`list` of :obj:`str`
         List of packages that have been uninstalled.
 
     Examples
     --------
     >>> import compas.plugins
-    >>> @compas.plugins.plugin(category='install')
+    >>> @compas.plugins.plugin(category="install")
     ... def after_rhino_uninstall(uninstalled_packages):
-    ...    # Do something cleanup, eg remove copied files.
-    ...    return [('compas_ghpython', 'GH Components uninstalled', True)]
+    ...     # Do something cleanup, eg remove copied files.
+    ...     return [("compas_ghpython", "GH Components uninstalled", True)]
 
     Returns
     -------
     :obj:`list` of 3-tuple (str, str, bool)
         List containing a 3-tuple with component name, message and True/False success flag.
     """
     pass
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/uninstall_plugin.py` & `compas-2.1.1/src/compas_rhino/uninstall_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 import os
 
 import compas_rhino
-
 from compas._os import remove_symlink
 
 
 def uninstall_plugin(plugin, version=None):
     """Uninstall a Rhino Python Command Plugin.
 
     Parameters
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/utilities/__init__.py` & `compas-2.1.1/src/compas_rhino/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `COMPAS-2.1.0/src/compas_rhino/utilities/constructors.py` & `compas-2.1.1/src/compas_rhino/utilities/constructors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
-
-from compas.tolerance import TOL
+from __future__ import print_function
 
 import Rhino  # type: ignore
 import scriptcontext as sc  # type: ignore
 
+from compas.tolerance import TOL
+
 
 def volmesh_from_polysurfaces(cls, guids, precision=None):
     """Construct a volumetric mesh from given polysurfaces.
 
     Parameters
     ----------
     cls : :class:`compas.datastructures.VolMesh`
```

### Comparing `COMPAS-2.1.0/src/compas_rhino/utilities/drawing.py` & `compas-2.1.1/src/compas_rhino/utilities/drawing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
+from __future__ import print_function
 
 from functools import wraps
 
+import Rhino  # type: ignore
 import rhinoscriptsyntax as rs  # type: ignore
 import scriptcontext as sc  # type: ignore
 import System  # type: ignore
-import Rhino  # type: ignore
 
 import compas_rhino.objects
-from compas_rhino.layers import create_layers_from_path
-from compas_rhino.layers import clear_layer
-from compas_rhino.layers import clear_current_layer
-from compas_rhino.conversions import vertices_and_faces_to_rhino
-
 from compas.geometry import centroid_polygon
+from compas_rhino.conversions import vertices_and_faces_to_rhino
+from compas_rhino.layers import clear_current_layer
+from compas_rhino.layers import clear_layer
+from compas_rhino.layers import create_layers_from_path
 
 find_object = sc.doc.Objects.Find
 add_point = sc.doc.Objects.AddPoint
 add_line = sc.doc.Objects.AddLine
 add_dot = sc.doc.Objects.AddTextDot
 add_curve = sc.doc.Objects.AddCurve
 add_polyline = sc.doc.Objects.AddPolyline
@@ -81,23 +80,25 @@
 
     Notes
     -----
     A label dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'pos': And(list, lambda x: len(x) == 3),
-            'text': And(str, len),
-            Optional('name', default=''): str,
-            Optional('color', default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str,
-            Optional('fontsize', default=10): Or(int, float),
-            Optional('font', default="Arial Regular"): str
-        })
+        Schema(
+            {
+                "pos": And(list, lambda x: len(x) == 3),
+                "text": And(str, len),
+                Optional("name", default=""): str,
+                Optional("color", default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+                Optional("fontsize", default=10): Or(int, float),
+                Optional("font", default="Arial Regular"): str,
+            }
+        )
 
     """
     guids = []
     for label in iter(labels):
         pos = label["pos"]
         text = label["text"]
         name = label.get("name", "")
@@ -146,20 +147,22 @@
 
     Notes
     -----
     A point dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'pos': And(list, lambda x: len(x) == 3),
-            Optional('name', default=''): str,
-            Optional('color', default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str
-        })
+        Schema(
+            {
+                "pos": And(list, lambda x: len(x) == 3),
+                Optional("name", default=""): str,
+                Optional("color", default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+            }
+        )
 
     """
     guids = []
     for p in iter(points):
         pos = p["pos"]
         name = p.get("name", "")
         color = p.get("color")
@@ -203,23 +206,25 @@
 
     Notes
     -----
     A line dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'start': And(list, lambda x: len(x) == 3),
-            'end': And(list, lambda x: len(x) == 3),
-            Optional('name', default=''): str,
-            Optional('color', default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str,
-            Optional('arrow', default=None): str,
-            Optional('width', default=None): Or(int, float),
-        })
+        Schema(
+            {
+                "start": And(list, lambda x: len(x) == 3),
+                "end": And(list, lambda x: len(x) == 3),
+                Optional("name", default=""): str,
+                Optional("color", default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+                Optional("arrow", default=None): str,
+                Optional("width", default=None): Or(int, float),
+            }
+        )
 
     """
     guids = []
     for line in iter(lines):
         sp = line["start"]
         ep = line["end"]
         name = line.get("name", "")
@@ -273,23 +278,25 @@
 
     Notes
     -----
     A geodesic dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'start': And(list, lambda x: len(x) == 3),
-            'end': And(list, lambda x: len(x) == 3),
-            'srf': Or(str, System.Guid),
-            Optional('name', default=''): str,
-            Optional('color', default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str,
-            Optional('arrow', default=None): str,
-        })
+        Schema(
+            {
+                "start": And(list, lambda x: len(x) == 3),
+                "end": And(list, lambda x: len(x) == 3),
+                "srf": Or(str, System.Guid),
+                Optional("name", default=""): str,
+                Optional("color", default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+                Optional("arrow", default=None): str,
+            }
+        )
 
     """
     guids = []
     for g in iter(geodesics):
         sp = g["start"]
         ep = g["end"]
         srf = g["srf"]
@@ -431,16 +438,16 @@
     >>> from compas.geometry import Box, Frame
     >>> from compas_rhino.utilities import draw_breps
     >>> box = Box(Frame.worldXY(), 1.0, 2.0, 3.0)
     >>> mesh = Mesh.from_shape(box)
 
     Draw convert each mesh face to brep dict schema:
 
-    >>> vertices = mesh.vertices_attributes('xyz')
-    >>> breps = [{'points': mesh.face_coordinates(face)} for face in mesh.faces()]
+    >>> vertices = mesh.vertices_attributes("xyz")
+    >>> breps = [{"points": mesh.face_coordinates(face)} for face in mesh.faces()]
 
     Draw brep faces as one joined brep.
 
     >>> guids = draw_breps(breps, join=True)
 
     """
     breps = []
@@ -520,22 +527,24 @@
 
     Notes
     -----
     A cylinder dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'start': And(list, lambda x: len(x) == 3),
-            'end': And(list, lambda x: len(x) == 3),
-            'radius': And(Or(int, float), lambda x: x > 0.0),
-            Optional('name', default=''): str,
-            Optional('color', default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str,
-        })
+        Schema(
+            {
+                "start": And(list, lambda x: len(x) == 3),
+                "end": And(list, lambda x: len(x) == 3),
+                "radius": And(Or(int, float), lambda x: x > 0.0),
+                Optional("name", default=""): str,
+                Optional("color", default=None): (lambda x: len(x) == 3 and all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+            }
+        )
 
     """
     guids = []
     for c in iter(cylinders):
         start = c["start"]
         end = c["end"]
         radius = c["radius"]
@@ -599,21 +608,23 @@
 
     Notes
     -----
     A pipe dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'points': And(list, lambda x: all(len(y) == 3 for y in x)),
-            'radius': And(Or(int, float), lambda x: x > 0.0),
-            Optional('name', default=''): str,
-            Optional('color', default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str,
-        })
+        Schema(
+            {
+                "points": And(list, lambda x: all(len(y) == 3 for y in x)),
+                "radius": And(Or(int, float), lambda x: x > 0.0),
+                Optional("name", default=""): str,
+                Optional("color", default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+            }
+        )
 
     """
     guids = []
     abs_tol = TOL
     ang_tol = sc.doc.ModelAngleToleranceRadians
     for p in pipes:
         points = p["points"]
@@ -622,17 +633,15 @@
         color = p.get("color")
         layer = p.get("layer")
         params = [0.0, 1.0]
         cap = System.Enum.ToObject(Rhino.Geometry.PipeCapMode, cap)
         if type(radius) in (int, float):
             radius = [radius] * 2
         radius = [float(r) for r in radius]
-        rail = Rhino.Geometry.Curve.CreateControlPointRhino.Geometry.Curve(
-            [Rhino.Geometry.Point3d(*xyz) for xyz in points]
-        )
+        rail = Rhino.Geometry.Curve.CreateControlPointRhino.Geometry.Curve([Rhino.Geometry.Point3d(*xyz) for xyz in points])
         breps = Rhino.Geometry.Brep.CreatePipe(rail, params, radius, 1, cap, fit, abs_tol, ang_tol)
         temp = [add_brep(brep) for brep in breps]
         for guid in temp:
             if not guid:
                 continue
             obj = find_object(guid)
             if not obj:
@@ -670,21 +679,23 @@
 
     Notes
     -----
     A sphere dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'pos': And(list, lambda x: len(x) == 3),
-            'radius': And(Or(int, float), lambda x: x > 0.0),
-            Optional('name', default=''): str,
-            Optional('color', default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str,
-        })
+        Schema(
+            {
+                "pos": And(list, lambda x: len(x) == 3),
+                "radius": And(Or(int, float), lambda x: x > 0.0),
+                Optional("name", default=""): str,
+                Optional("color", default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+            }
+        )
 
     """
     guids = []
     for s in iter(spheres):
         pos = s["pos"]
         radius = s["radius"]
         name = s.get("name", "")
@@ -804,20 +815,22 @@
 
     Notes
     -----
     A face dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'points': And(len, lambda x: all(len(y) == 3 for y in x)),
-            Optional('name', default=''): str,
-            Optional('color', default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
-            Optional('vertexcolors', default=None): And(len, lambda x: all(0 <= y <= 255 for y in x)),
-        })
+        Schema(
+            {
+                "points": And(len, lambda x: all(len(y) == 3 for y in x)),
+                Optional("name", default=""): str,
+                Optional("color", default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
+                Optional("vertexcolors", default=None): And(len, lambda x: all(0 <= y <= 255 for y in x)),
+            }
+        )
 
     """
     guids = []
     for face in iter(faces):
         points = face["points"][:]
         name = face.get("name")
         color = face.get("color")
@@ -882,33 +895,33 @@
 
     Notes
     -----
     A circle dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'plane': lambda x: len(x[0]) == 3 and len(x[1]) == 3,
-            'radius': And(Or(int, float), lambda x: x > 0),
-            Optional('name', default=''): str,
-            Optional('color', default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str
-        })
+        Schema(
+            {
+                "plane": lambda x: len(x[0]) == 3 and len(x[1]) == 3,
+                "radius": And(Or(int, float), lambda x: x > 0),
+                Optional("name", default=""): str,
+                Optional("color", default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+            }
+        )
 
     """
     guids = []
     for data in iter(circles):
         point, normal = data["plane"]
         radius = data["radius"]
         name = data.get("name", "")
         color = data.get("color")
         layer = data.get("layer")
-        circle = Rhino.Geometry.Circle(
-            Rhino.Geometry.Plane(Rhino.Geometry.Point3d(*point), Rhino.Geometry.Vector3d(*normal)), radius
-        )
+        circle = Rhino.Geometry.Circle(Rhino.Geometry.Plane(Rhino.Geometry.Point3d(*point), Rhino.Geometry.Vector3d(*normal)), radius)
         guid = add_circle(circle)
         if not guid:
             continue
         obj = find_object(guid)
         if not obj:
             continue
         attr = obj.Attributes
@@ -944,20 +957,22 @@
 
     Notes
     -----
     A curve dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'curve': compas.geometry.Rhino.Geometry.Curve,
-            Optional('name', default=''): str,
-            Optional('color', default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str
-        })
+        Schema(
+            {
+                "curve": compas.geometry.Rhino.Geometry.Curve,
+                Optional("name", default=""): str,
+                Optional("color", default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+            }
+        )
 
     """
     guids = []
     for data in iter(curves):
         curve = data["curve"]
         name = data.get("name", "")
         color = data.get("color")
@@ -1000,20 +1015,22 @@
 
     Notes
     -----
     A surface dict has the following schema:
 
     .. code-block:: python
 
-        Schema({
-            'surface': compas.geometry.Surface,
-            Optional('name', default=''): str,
-            Optional('color', default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
-            Optional('layer', default=None): str
-        })
+        Schema(
+            {
+                "surface": compas.geometry.Surface,
+                Optional("name", default=""): str,
+                Optional("color", default=None): And(lambda x: len(x) == 3, all(0 <= y <= 255 for y in x)),
+                Optional("layer", default=None): str,
+            }
+        )
 
     """
     guids = []
     for data in iter(surfaces):
         surface = data["surface"]
         name = data.get("name", "")
         color = data.get("color")
```

