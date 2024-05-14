# Comparing `tmp/EasyFEA-1.0.1.tar.gz` & `tmp/EasyFEA-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyFEA-1.0.1.tar", last modified: Sat Apr 13 16:43:24 2024, max compression
+gzip compressed data, was "EasyFEA-1.0.2.tar", last modified: Tue May 14 08:00:25 2024, max compression
```

## Comparing `EasyFEA-1.0.1.tar` & `EasyFEA-1.0.2.tar`

### file list

```diff
@@ -1,130 +1,63 @@
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.596342 EasyFEA-1.0.1/
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.582571 EasyFEA-1.0.1/EasyFEA/
--rw-r--r--   0 matnoel    (501) staff       (20)    35934 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/Geoms.py
--rw-r--r--   0 matnoel    (501) staff       (20)      807 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/Materials.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1065 2024-04-13 15:37:09.000000 EasyFEA-1.0.1/EasyFEA/Simulations.py
--rw-r--r--   0 matnoel    (501) staff       (20)       21 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/__about__.py
--rw-r--r--   0 matnoel    (501) staff       (20)      942 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/__init__.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.584373 EasyFEA-1.0.1/EasyFEA/fem/
--rw-r--r--   0 matnoel    (501) staff       (20)      260 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)     6176 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/_boundary_conditions.py
--rw-r--r--   0 matnoel    (501) staff       (20)    11030 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/_gauss.py
--rw-r--r--   0 matnoel    (501) staff       (20)    65546 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/_gmsh_interface.py
--rw-r--r--   0 matnoel    (501) staff       (20)    68300 2024-04-13 14:42:08.000000 EasyFEA-1.0.1/EasyFEA/fem/_group_elems.py
--rw-r--r--   0 matnoel    (501) staff       (20)    37173 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/_mesh.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1592 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/_utils.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.585327 EasyFEA-1.0.1/EasyFEA/fem/elems/
--rw-r--r--   0 matnoel    (501) staff       (20)        0 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/elems/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)    23110 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/elems/_hexa.py
--rw-r--r--   0 matnoel    (501) staff       (20)      783 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/elems/_point.py
--rw-r--r--   0 matnoel    (501) staff       (20)    13576 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/elems/_prism.py
--rw-r--r--   0 matnoel    (501) staff       (20)     4833 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/elems/_quad.py
--rw-r--r--   0 matnoel    (501) staff       (20)    12816 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/elems/_seg.py
--rw-r--r--   0 matnoel    (501) staff       (20)     7200 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/elems/_tetra.py
--rw-r--r--   0 matnoel    (501) staff       (20)    11843 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/fem/elems/_tri.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.586152 EasyFEA-1.0.1/EasyFEA/materials/
--rw-r--r--   0 matnoel    (501) staff       (20)      293 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/materials/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)    10778 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/materials/_beam.py
--rw-r--r--   0 matnoel    (501) staff       (20)    24303 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/materials/_elastic.py
--rw-r--r--   0 matnoel    (501) staff       (20)    49708 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/materials/_phasefield.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2239 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/materials/_thermal.py
--rw-r--r--   0 matnoel    (501) staff       (20)    17138 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/materials/_utils.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.587341 EasyFEA-1.0.1/EasyFEA/simulations/
--rw-r--r--   0 matnoel    (501) staff       (20)    14044 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/simulations/Solvers.py
--rw-r--r--   0 matnoel    (501) staff       (20)        0 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/simulations/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)    30212 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/simulations/_beam.py
--rw-r--r--   0 matnoel    (501) staff       (20)    19526 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/simulations/_dic.py
--rw-r--r--   0 matnoel    (501) staff       (20)    19227 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/simulations/_elastic.py
--rw-r--r--   0 matnoel    (501) staff       (20)    30902 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/simulations/_phasefield.py
--rw-r--r--   0 matnoel    (501) staff       (20)    58113 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/simulations/_simu.py
--rw-r--r--   0 matnoel    (501) staff       (20)     6780 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/simulations/_thermal.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2471 2024-04-13 14:48:04.000000 EasyFEA-1.0.1/EasyFEA/simulations/_utils.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.588455 EasyFEA-1.0.1/EasyFEA/utilities/
--rw-r--r--   0 matnoel    (501) staff       (20)    46023 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/utilities/Display.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3151 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/utilities/Folder.py
--rw-r--r--   0 matnoel    (501) staff       (20)     7771 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/utilities/Numba_Interface.py
--rw-r--r--   0 matnoel    (501) staff       (20)     9432 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/utilities/Paraview_Interface.py
--rw-r--r--   0 matnoel    (501) staff       (20)    27270 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/utilities/PyVista_Interface.py
--rw-r--r--   0 matnoel    (501) staff       (20)       21 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/utilities/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1348 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/utilities/_observers.py
--rw-r--r--   0 matnoel    (501) staff       (20)     6856 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/EasyFEA/utilities/_tic.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.583212 EasyFEA-1.0.1/EasyFEA.egg-info/
--rw-r--r--   0 matnoel    (501) staff       (20)    47301 2024-04-13 16:43:24.000000 EasyFEA-1.0.1/EasyFEA.egg-info/PKG-INFO
--rw-r--r--   0 matnoel    (501) staff       (20)     3129 2024-04-13 16:43:24.000000 EasyFEA-1.0.1/EasyFEA.egg-info/SOURCES.txt
--rw-r--r--   0 matnoel    (501) staff       (20)        1 2024-04-13 16:43:24.000000 EasyFEA-1.0.1/EasyFEA.egg-info/dependency_links.txt
--rw-r--r--   0 matnoel    (501) staff       (20)      132 2024-04-13 16:43:24.000000 EasyFEA-1.0.1/EasyFEA.egg-info/requires.txt
--rw-r--r--   0 matnoel    (501) staff       (20)        8 2024-04-13 16:43:24.000000 EasyFEA-1.0.1/EasyFEA.egg-info/top_level.txt
--rw-r--r--   0 matnoel    (501) staff       (20)    35149 2024-04-10 14:50:23.000000 EasyFEA-1.0.1/LICENSE.txt
--rw-r--r--   0 matnoel    (501) staff       (20)    47301 2024-04-13 16:43:24.596177 EasyFEA-1.0.1/PKG-INFO
--rw-r--r--   0 matnoel    (501) staff       (20)     5778 2024-04-13 16:36:21.000000 EasyFEA-1.0.1/README.md
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.588719 EasyFEA-1.0.1/examples/
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.589307 EasyFEA-1.0.1/examples/Beam/
--rw-r--r--   0 matnoel    (501) staff       (20)     2825 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Beam/Beam1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3388 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Beam/Beam2.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3083 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Beam/Beam3.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2199 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Beam/Beam4.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3167 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Beam/Beam5.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.589714 EasyFEA-1.0.1/examples/Contact/
--rw-r--r--   0 matnoel    (501) staff       (20)     6027 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Contact/Contact1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     5964 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Contact/Contact2.py
--rw-r--r--   0 matnoel    (501) staff       (20)     4137 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Contact/Contact3.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.590190 EasyFEA-1.0.1/examples/Dynamic/
--rw-r--r--   0 matnoel    (501) staff       (20)     4119 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Dynamic/Dyna1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3307 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Dynamic/Dyna2.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2759 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Dynamic/Modal1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     5547 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Dynamic/Modal2.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.591080 EasyFEA-1.0.1/examples/Elastic/
--rw-r--r--   0 matnoel    (501) staff       (20)     2194 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Elastic/Elas1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2441 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Elastic/Elas2.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2252 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Elastic/Elas3.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3833 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Elastic/Elas4.py
--rw-r--r--   0 matnoel    (501) staff       (20)     4133 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Elastic/HyperElasticity.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2642 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Elastic/PlateWithHole.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3463 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Elastic/PressurizedTube.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1139 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/HelloWorld.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.592074 EasyFEA-1.0.1/examples/Identification/
--rw-r--r--   0 matnoel    (501) staff       (20)     9219 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Identification/FEMU1.py
--rw-r--r--   0 matnoel    (501) staff       (20)    12098 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Identification/FEMU2.py
--rw-r--r--   0 matnoel    (501) staff       (20)     5860 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Identification/Homog1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     9673 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Identification/Homog2.py
--rw-r--r--   0 matnoel    (501) staff       (20)     6388 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Identification/HomogFullField.py
--rw-r--r--   0 matnoel    (501) staff       (20)    25437 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Identification/VFM1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     5357 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Identification/VFM2.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.592195 EasyFEA-1.0.1/examples/Machine learning/
--rw-r--r--   0 matnoel    (501) staff       (20)     1257 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Machine learning/k_means.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.594283 EasyFEA-1.0.1/examples/Meshes/
--rw-r--r--   0 matnoel    (501) staff       (20)      664 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1287 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh10.py
--rw-r--r--   0 matnoel    (501) staff       (20)      575 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh11.py
--rw-r--r--   0 matnoel    (501) staff       (20)      731 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh2.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1223 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh3.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1321 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh4.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2571 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh5.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1092 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh6.py
--rw-r--r--   0 matnoel    (501) staff       (20)     2937 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh7.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3299 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh8.py
--rw-r--r--   0 matnoel    (501) staff       (20)     9918 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/Mesh9.py
--rw-r--r--   0 matnoel    (501) staff       (20)     7540 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/MeshConvergence.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3074 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/MeshOptim0.py
--rw-r--r--   0 matnoel    (501) staff       (20)     4779 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/MeshOptim1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     4735 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/MeshOptim2.py
--rw-r--r--   0 matnoel    (501) staff       (20)     5424 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Meshes/MeshOptim3.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.595192 EasyFEA-1.0.1/examples/Phasefield/
--rw-r--r--   0 matnoel    (501) staff       (20)     5970 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/L_Shape.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.595607 EasyFEA-1.0.1/examples/Phasefield/PlateWithHole/
--rw-r--r--   0 matnoel    (501) staff       (20)     4521 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/PlateWithHole/Dimension.py
--rw-r--r--   0 matnoel    (501) staff       (20)     9930 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/PlateWithHole/Energy.py
--rw-r--r--   0 matnoel    (501) staff       (20)     4135 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/PlateWithHole/Loading.py
--rw-r--r--   0 matnoel    (501) staff       (20)    10441 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/PlateWithHole.py
--rw-r--r--   0 matnoel    (501) staff       (20)     6450 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/PostProcess.py
--rw-r--r--   0 matnoel    (501) staff       (20)     9352 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/Shear.py
--rw-r--r--   0 matnoel    (501) staff       (20)    11176 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/Tension.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3601 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/Tension_Inclusions.py
--rw-r--r--   0 matnoel    (501) staff       (20)     5941 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Phasefield/Traction_Wood.py
-drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-04-13 16:43:24.595860 EasyFEA-1.0.1/examples/Thermal/
--rw-r--r--   0 matnoel    (501) staff       (20)     3424 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Thermal/Thermal1.py
--rw-r--r--   0 matnoel    (501) staff       (20)     3091 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/Thermal/Thermal2.py
--rw-r--r--   0 matnoel    (501) staff       (20)        0 2024-04-13 14:15:50.000000 EasyFEA-1.0.1/examples/__init__.py
--rw-r--r--   0 matnoel    (501) staff       (20)     1382 2024-04-13 16:41:37.000000 EasyFEA-1.0.1/pyproject.toml
--rw-r--r--   0 matnoel    (501) staff       (20)       38 2024-04-13 16:43:24.596399 EasyFEA-1.0.1/setup.cfg
--rw-r--r--   0 matnoel    (501) staff       (20)       61 2024-03-19 17:45:45.000000 EasyFEA-1.0.1/setup.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.106489 EasyFEA-1.0.2/
+-rw-r--r--   0 matnoel    (501) staff       (20)      307 2024-05-08 15:55:35.000000 EasyFEA-1.0.2/AUTHORS.md
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.099151 EasyFEA-1.0.2/EasyFEA/
+-rw-r--r--   0 matnoel    (501) staff       (20)    36204 2024-05-08 13:48:20.000000 EasyFEA-1.0.2/EasyFEA/Geoms.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1077 2024-05-08 13:26:51.000000 EasyFEA-1.0.2/EasyFEA/Materials.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1345 2024-05-08 13:26:54.000000 EasyFEA-1.0.2/EasyFEA/Simulations.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      556 2024-05-14 07:57:58.000000 EasyFEA-1.0.2/EasyFEA/__about__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1212 2024-05-08 13:26:46.000000 EasyFEA-1.0.2/EasyFEA/__init__.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.101208 EasyFEA-1.0.2/EasyFEA/fem/
+-rw-r--r--   0 matnoel    (501) staff       (20)      530 2024-05-08 13:24:58.000000 EasyFEA-1.0.2/EasyFEA/fem/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     6446 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/fem/_boundary_conditions.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    11489 2024-05-08 13:25:02.000000 EasyFEA-1.0.2/EasyFEA/fem/_gauss.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    65816 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/fem/_gmsh_interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    68220 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/fem/_group_elems.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    37442 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/fem/_mesh.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1918 2024-05-08 13:33:39.000000 EasyFEA-1.0.2/EasyFEA/fem/_utils.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.102406 EasyFEA-1.0.2/EasyFEA/fem/elems/
+-rw-r--r--   0 matnoel    (501) staff       (20)      268 2024-05-08 13:24:31.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    23380 2024-05-08 13:24:34.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_hexa.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1053 2024-05-08 13:24:38.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_point.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    13846 2024-05-08 13:24:41.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_prism.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     5103 2024-05-08 13:24:43.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_quad.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    13086 2024-05-08 13:24:50.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_seg.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     7470 2024-05-08 13:24:52.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_tetra.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    12113 2024-05-08 13:24:55.000000 EasyFEA-1.0.2/EasyFEA/fem/elems/_tri.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.103311 EasyFEA-1.0.2/EasyFEA/materials/
+-rw-r--r--   0 matnoel    (501) staff       (20)      563 2024-05-08 13:25:20.000000 EasyFEA-1.0.2/EasyFEA/materials/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    11048 2024-05-08 13:25:22.000000 EasyFEA-1.0.2/EasyFEA/materials/_beam.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    24573 2024-05-08 13:25:24.000000 EasyFEA-1.0.2/EasyFEA/materials/_elastic.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    50153 2024-05-08 13:35:30.000000 EasyFEA-1.0.2/EasyFEA/materials/_phasefield.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     2509 2024-05-08 13:25:28.000000 EasyFEA-1.0.2/EasyFEA/materials/_thermal.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    17464 2024-05-08 13:34:07.000000 EasyFEA-1.0.2/EasyFEA/materials/_utils.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.104585 EasyFEA-1.0.2/EasyFEA/simulations/
+-rw-r--r--   0 matnoel    (501) staff       (20)    14581 2024-05-08 13:36:06.000000 EasyFEA-1.0.2/EasyFEA/simulations/Solvers.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      268 2024-05-08 13:25:37.000000 EasyFEA-1.0.2/EasyFEA/simulations/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    30482 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/simulations/_beam.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    19587 2024-05-08 13:25:42.000000 EasyFEA-1.0.2/EasyFEA/simulations/_dic.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    19497 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/simulations/_elastic.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    31172 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/simulations/_phasefield.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    59684 2024-05-14 07:58:25.000000 EasyFEA-1.0.2/EasyFEA/simulations/_simu.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     7050 2024-05-08 13:25:58.000000 EasyFEA-1.0.2/EasyFEA/simulations/_thermal.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1868 2024-05-08 13:48:35.000000 EasyFEA-1.0.2/EasyFEA/simulations/_utils.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.105646 EasyFEA-1.0.2/EasyFEA/utilities/
+-rw-r--r--   0 matnoel    (501) staff       (20)    46290 2024-05-08 14:04:02.000000 EasyFEA-1.0.2/EasyFEA/utilities/Display.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     3421 2024-05-08 13:48:35.000000 EasyFEA-1.0.2/EasyFEA/utilities/Folder.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     8041 2024-05-08 13:26:30.000000 EasyFEA-1.0.2/EasyFEA/utilities/Numba_Interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     9702 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/utilities/Paraview_Interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)    27540 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/utilities/PyVista_Interface.py
+-rw-r--r--   0 matnoel    (501) staff       (20)      291 2024-05-08 13:26:11.000000 EasyFEA-1.0.2/EasyFEA/utilities/__init__.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     1618 2024-05-08 13:48:40.000000 EasyFEA-1.0.2/EasyFEA/utilities/_observers.py
+-rw-r--r--   0 matnoel    (501) staff       (20)     7126 2024-05-08 13:26:16.000000 EasyFEA-1.0.2/EasyFEA/utilities/_tic.py
+drwxr-xr-x   0 matnoel    (501) staff       (20)        0 2024-05-14 08:00:25.099821 EasyFEA-1.0.2/EasyFEA.egg-info/
+-rw-r--r--   0 matnoel    (501) staff       (20)    48948 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/PKG-INFO
+-rw-r--r--   0 matnoel    (501) staff       (20)     1433 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/SOURCES.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)        1 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/dependency_links.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)      132 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/requires.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)        8 2024-05-14 08:00:25.000000 EasyFEA-1.0.2/EasyFEA.egg-info/top_level.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)    35149 2024-04-26 09:17:40.000000 EasyFEA-1.0.2/LICENSE.txt
+-rw-r--r--   0 matnoel    (501) staff       (20)    48948 2024-05-14 08:00:25.106214 EasyFEA-1.0.2/PKG-INFO
+-rw-r--r--   0 matnoel    (501) staff       (20)     7021 2024-05-14 07:23:45.000000 EasyFEA-1.0.2/README.md
+-rw-r--r--   0 matnoel    (501) staff       (20)     1378 2024-05-14 07:54:14.000000 EasyFEA-1.0.2/pyproject.toml
+-rw-r--r--   0 matnoel    (501) staff       (20)       38 2024-05-14 08:00:25.106535 EasyFEA-1.0.2/setup.cfg
+-rw-r--r--   0 matnoel    (501) staff       (20)       61 2024-03-19 17:45:45.000000 EasyFEA-1.0.2/setup.py
```

### Comparing `EasyFEA-1.0.1/EasyFEA/Geoms.py` & `EasyFEA-1.0.2/EasyFEA/Geoms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Module containing the geometric classes used to build meshes."""
 
 from typing import Union
 import numpy as np
 import copy
 import matplotlib.pyplot as plt
 from scipy.optimize import minimize
@@ -260,15 +264,15 @@
         [point.Translate(*dec[p]) for p, point in enumerate(self.points)]
 
     def Plot(self, ax: plt.Axes=None, color:str="", name:str="", plotPoints=True) -> plt.Axes:
 
         from EasyFEA import Display
 
         if ax is None:
-            ax = Display.init_Axes(3)
+            ax = Display.Init_Axes(3)
             
         inDim = 3 if ax.name == '3d' else 2
 
         lines, points = self.Get_coord_for_plot()
         if color != "":
             ax.plot(*lines[:,:inDim].T, color=color, label=self.name)
         else:
```

### Comparing `EasyFEA-1.0.1/EasyFEA/__init__.py` & `EasyFEA-1.0.2/EasyFEA/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 # ----------------------------------------------
 # utilities
 # ----------------------------------------------
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/_boundary_conditions.py` & `EasyFEA-1.0.2/EasyFEA/fem/_boundary_conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Module containing classes used to create boundary conditions."""
 
 import numpy as np
 
 class BoundaryCondition:
 
     def __init__(self, problemType: str, nodes: np.ndarray, dofs: np.ndarray, directions: np.ndarray, dofsValues: np.ndarray, description: str):
@@ -143,15 +147,15 @@
         from EasyFEA import Display
 
         dofs_d = np.zeros((nodes.size, nDir), dtype=int)
 
         for d, direction in enumerate(directions):
 
             if direction not in availableDirections:
-                Display.myPrintError(f"direction ({direction}) must be in {availableDirections}.")
+                Display.MyPrintError(f"direction ({direction}) must be in {availableDirections}.")
                 continue
             
             idx = availableDirections.index(direction)
 
             dofs_d[:,d] = nodes * dim + idx
 
         return dofs_d.ravel()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/_gauss.py` & `EasyFEA-1.0.2/EasyFEA/fem/_gauss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Module containing the Gauss class used to determine the coordinates and weights of integration points."""
 
 import numpy as np
 
 # utils
 from ._utils import ElemType, MatrixType
 
@@ -14,15 +18,15 @@
         ----------
         elemType : str
             element type
         matrixType : str
             [MatrixType.rigi, MatrixType.mass, MatrixType.beam]
         """
 
-        coord, weights = Gauss.__gauss_factory(elemType, matrixType)
+        coord, weights = Gauss._Gauss_factory(elemType, matrixType)
 
         self.__coord = coord
         self.__weights = weights
 
     @property
     def coord(self) -> np.ndarray:
         """integration point coordinates"""
@@ -35,16 +39,17 @@
 
     @property
     def nPg(self) -> int:
         """number of integration points"""
         return self.__weights.size
 
     @staticmethod
-    def __Triangle(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
-        """available [1, 3, 6, 7, 12]"""
+    def _Triangle(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """available [1, 3, 6, 7, 12]\n
+        order = [1, 2, 3, 4, 5]"""
         if nPg == 1:
             ksis = 1/3
             etas = 1/3
 
             weights = 1/2
 
         elif nPg == 3:
@@ -88,16 +93,17 @@
             etas = [a, a, 1-2*a, b, b, 1-2*b, d, c, c, d, 1-c-d, 1-c-d]
 
             weights = [p1, p1, p1, p2, p2, p2, p3, p3, p3, p3, p3, p3]
 
         return ksis, etas, weights
 
     @staticmethod
-    def __Quadrangle(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
-        """available [4, 9]"""
+    def _Quadrangle(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """available [4, 9]\n
+        order = [1, 2]"""
         if nPg == 4:
             a = 1/np.sqrt(3)
             ksis = [-a, a, a, -a]
             etas = [-a, -a, a, a]
 
             weights = [1]*nPg
         elif nPg == 9:
@@ -106,16 +112,18 @@
             ksis = [-a, a, a, -a, 0, a, 0, -a, 0]
             etas = [-a, -a, a, a, -a, 0, a, 0, 0]
             weights = [25/81, 25/81, 25/81, 25/81, 40/81, 40/81, 40/81, 40/81, 64/81]
 
         return ksis, etas, weights
 
     @staticmethod
-    def __Tetrahedron(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
-        """available [1, 4, 5, 15]"""
+    def _Tetrahedron(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+        """available [1, 4, 5, 15]\n
+        order = [1, 2, 3, 5]"""
+        
         if nPg == 1:            
 
             x = 1/4
             y = 1/4
             z = 1/4
 
             weights = 1/6
@@ -161,16 +169,18 @@
             p4 = 5/567
 
             weights = [p1, p2, p2, p2, p2, p3, p3, p3, p3, p4, p4, p4, p4, p4, p4]
 
         return x, y, z, weights
     
     @staticmethod
-    def __Hexahedron(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
-        """available [8]"""
+    def _Hexahedron(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+        """available [8, 27]\n
+        order = [3, 5]"""
+        
         if nPg == 8:            
 
             a = 1/np.sqrt(3)
 
             x = [-a, -a, -a, -a, a, a, a, a]
             y = [-a, -a, a, a, -a, -a, a, a]
             z = [-a, a, -a, a, -a, a, -a, a]
@@ -194,16 +204,19 @@
             c22 = c1*c2**2
 
             weights = [c13,c12,c13, c12,c22,c12, c13,c12,c13, c12,c22,c12, c22,c23,c22, c12,c22,c12, c13,c12,c13, c12,c22,c12, c13,c12,c13]
 
         return x, y, z, weights
     
     @staticmethod
-    def __Prism(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
-        """available [6, 8]"""
+    def _Prism(nPg: int) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+        """available [6, 8]\n
+        orderX = [3, 3]\n
+        orderYZ = [2, 3]"""
+        
 
         # X, Y, Z -> base code aster
         # z, x, y -> gmsh        
         # Y -> x, Z -> y, X -> z  
 
         if nPg == 6:
             
@@ -228,15 +241,15 @@
         x = np.array(Y)
         y = np.array(Z)
         z = np.array(X)
 
         return x, y, z, weights
 
     @staticmethod
-    def __gauss_factory(elemType: str, matrixType: str) -> tuple[np.ndarray, np.ndarray]:
+    def _Gauss_factory(elemType: str, matrixType: str) -> tuple[np.ndarray, np.ndarray]:
         """Calculation of integration points according to element and matrix type
         """
 
         assert matrixType in MatrixType.Get_types()
 
         # TODO create a function to calculate the order directly?
 
@@ -280,96 +293,96 @@
 
         elif elemType == ElemType.TRI3:
             dim = 2            
             if matrixType == MatrixType.rigi:
                 nPg = 1
             elif matrixType == MatrixType.mass:
                 nPg = 3
-            xis, etas, weights = Gauss.__Triangle(nPg)
+            xis, etas, weights = Gauss._Triangle(nPg)
 
         elif elemType == ElemType.TRI6:
             dim = 2            
             if matrixType == MatrixType.rigi:
                 nPg = 3
             elif matrixType == MatrixType.mass:
                 nPg = 6
-            xis, etas, weights = Gauss.__Triangle(nPg)
+            xis, etas, weights = Gauss._Triangle(nPg)
 
         elif elemType == ElemType.TRI10:
             dim = 2            
             nPg = 6
-            xis, etas, weights = Gauss.__Triangle(nPg)
+            xis, etas, weights = Gauss._Triangle(nPg)
 
         # elif elemType == ElemType.TRI15:
         #     dim = 2            
         #     if matrixType == MatrixType.rigi:
         #         nPg = 6
         #     elif matrixType == MatrixType.masse:
         #         nPg = 12
         #     ksis, etas, weights = Gauss.__CoordoPoidsGaussTriangle(nPg)
 
         elif elemType == ElemType.QUAD4:
             dim = 2            
             nPg = 4
-            xis, etas, weights = Gauss.__Quadrangle(nPg)
+            xis, etas, weights = Gauss._Quadrangle(nPg)
             
         elif elemType == ElemType.QUAD8:
             dim = 2            
             if matrixType == MatrixType.rigi:
                 nPg = 4
             elif matrixType == MatrixType.mass:
                 nPg = 9
-            xis, etas, weights = Gauss.__Quadrangle(nPg)
+            xis, etas, weights = Gauss._Quadrangle(nPg)
                     
         elif elemType == ElemType.TETRA4:
             dim = 3            
             if matrixType == MatrixType.rigi:
                 nPg = 1
             elif matrixType == MatrixType.mass:
                 nPg = 4            
-            x, y, z, weights = Gauss.__Tetrahedron(nPg)
+            x, y, z, weights = Gauss._Tetrahedron(nPg)
 
         elif elemType == ElemType.TETRA10:
             dim = 3            
             nPg = 4
-            x, y, z, weights = Gauss.__Tetrahedron(nPg)
+            x, y, z, weights = Gauss._Tetrahedron(nPg)
 
         elif elemType == ElemType.HEXA8:
             dim = 3            
             if matrixType in [MatrixType.rigi, MatrixType.mass]:
                 nPg = 8
-                x, y, z, weights = Gauss.__Hexahedron(nPg)
+                x, y, z, weights = Gauss._Hexahedron(nPg)
 
         elif elemType == ElemType.HEXA20:
             dim = 3
             if matrixType in [MatrixType.rigi, MatrixType.mass]:
                 nPg = 8
                 # nPg = 27
-                x, y, z, weights = Gauss.__Hexahedron(nPg)
+                x, y, z, weights = Gauss._Hexahedron(nPg)
 
         elif elemType == ElemType.PRISM6:
             dim = 3            
             if matrixType in [MatrixType.rigi, MatrixType.mass]:
                 nPg = 6
 
-                x, y, z, weights = Gauss.__Prism(nPg)
+                x, y, z, weights = Gauss._Prism(nPg)
 
         elif elemType == ElemType.PRISM15:
             dim = 3            
             if matrixType in [MatrixType.rigi, MatrixType.mass]:
                 nPg = 6
 
-                x, y, z, weights = Gauss.__Prism(nPg)
+                x, y, z, weights = Gauss._Prism(nPg)
 
         else:
             raise Exception("Element not implemented")
 
         if dim == 1:
-            coord = np.array([x]).T.reshape((nPg,1))
+            coord = np.asarray([x]).T.reshape((nPg,1))
         elif dim == 2:
-            coord = np.array([xis, etas]).T.reshape((nPg,2))
+            coord = np.asarray([xis, etas]).T.reshape((nPg,2))
         elif dim == 3:
-            coord = np.array([x, y, z]).T.reshape((nPg,3))
+            coord = np.asarray([x, y, z]).T.reshape((nPg,3))
 
-        weights = np.array(weights).reshape(nPg)
+        weights = np.asarray(weights).reshape(nPg)
 
         return coord, weights
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/_gmsh_interface.py` & `EasyFEA-1.0.2/EasyFEA/fem/_gmsh_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Module providing an interface with Gmsh (https://gmsh.info/).\n
 This module facilitates the manipulation of _Geom objects to create meshes through Gmsh with ease."""
 
 import gmsh
 import sys
 import os
 import numpy as np
@@ -667,18 +671,18 @@
         # Allow other meshes -> this seems impossible - you have to create the mesh using gmsh to control the type of element.
 
         __doesNotWork = [ElemType.HEXA8.name, ElemType.HEXA20.name,
                          ElemType.PRISM6.name, ElemType.PRISM15.name] # keep .name to improve error display
         if elemType is None:
             elemType = ElemType.TRI3 if dim == 2 else ElemType.TETRA4
         elif elemType in __doesNotWork:
-            from ..utilities.Display import myPrintError
-            myPrintError(f"It is not possible to mesh an imported part with the following elements: {__doesNotWork}")
+            from ..utilities.Display import MyPrintError
+            MyPrintError(f"It is not possible to mesh an imported part with the following elements: {__doesNotWork}")
             elemType = ElemType.TETRA4 if elemType in [ElemType.HEXA8, ElemType.HEXA20] else ElemType.TETRA10
-            myPrintError(f"\nThe part will be meshed with {elemType} elements.")
+            MyPrintError(f"\nThe part will be meshed with {elemType} elements.")
 
         self._Init_gmsh() # Only work with occ !! Do not change
 
         assert meshSize >= 0.0, "Must be greater than or equal to 0."
         self.__CheckType(dim, elemType)
         
         tic = Tic()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/_group_elems.py` & `EasyFEA-1.0.2/EasyFEA/fem/_group_elems.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Element group creation module.
 A mesh uses several element groups.
 For instance, a TRI3 mesh uses the elements POINT, SEG2 and TRI3."""
 
 from abc import ABC, abstractmethod, abstractproperty
 
 from scipy.optimize import least_squares
@@ -139,21 +143,15 @@
         """This matrix contains the element group coordinates (Nn, 3)"""
         coord: np.ndarray = self.coordGlob[self.__nodes]
         return coord
 
     @property
     def coordGlob(self) -> np.ndarray:
         """This matrix contains all the mesh coordinates (mesh.Nn, 3)"""
-        try:
-            return self.__coordGlob.copy()
-        except AttributeError:
-            # This may trigger an error, as I changed __coordoGlob to __coordGlob on April 5, 2024.
-            # TODO: to be removed when I no longer need to load old phasefield simulations
-            self.__coordGlob = self.__coordoGlob.copy()            
-            return self.__coordGlob.copy()
+        return self.__coordGlob.copy()
     
     @coordGlob.setter
     def coordGlob(self, coord: np.ndarray) -> None:
         if coord.shape == self.__coordGlob.shape:
             self.__coordGlob = coord
             self._InitMatrix()
 
@@ -1170,17 +1168,17 @@
 
         try:
             arrayTest = np.asarray(func(xn, yn, zn))
             if arrayTest.dtype == bool:
                 idx = np.where(arrayTest)[0]
                 return self.__nodes[idx].copy()
             else:
-                Display.myPrintError("The function must return a Boolean.")
+                Display.MyPrintError("The function must return a Boolean.")
         except TypeError:
-            Display.myPrintError("Must provide a 3-parameter function of type lambda x,y,z: ...")
+            Display.MyPrintError("Must provide a 3-parameter function of type lambda x,y,z: ...")
     
     def Get_Nodes_Point(self, point: Point) -> np.ndarray:
         """Returns nodes on the point."""
 
         coordo = self.coord
 
         idx = np.where((coordo[:,0] == point.x) & (coordo[:,1] == point.y) & (coordo[:,2] == point.z))[0]
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/_mesh.py` & `EasyFEA-1.0.2/EasyFEA/fem/_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Module containing the mesh class.
 This class allows you to manipulate different groups of elements.
 These element groups are used to construct finite element matrices."""
 
 import numpy as np
 import scipy.sparse as sp
 import copy
@@ -56,23 +60,23 @@
         
         Nn = self.coordGlob.shape[0]
         usedNodes = set(self.connect.ravel())
         nodes = set(range(Nn))
         orphanNodes = list(nodes - usedNodes)
         self.__orphanNodes: list[int] = orphanNodes
         if len(orphanNodes) > 0 and verbosity:            
-            Display.myPrintError("WARNING: Orphan nodes have been detected (stored in mesh.orphanNodes).")
+            Display.MyPrintError("WARNING: Orphan nodes have been detected (stored in mesh.orphanNodes).")
 
     def _ResetMatrix(self) -> None:
         """Reset matrix for each groupElem"""
         [groupElem._InitMatrix() for groupElem in self.Get_list_groupElem()]
 
     def __str__(self) -> str:
         """Return a string representation of the mesh."""
-        text = f"\nElement type : {self.elemType}"
+        text = f"\nElement type: {self.elemType}"
         text += f"\nNe = {self.Ne}, Nn = {self.Nn}, dof = {self.Nn * self.__dim}"
         return text
 
     def Get_list_groupElem(self, dim=None) -> list[_GroupElem]:
         """Get the list of mesh element groups.
 
         Parameters
@@ -494,15 +498,15 @@
         # elements = self.groupElem.Get_Elements_Nodes(nodes=nodes, exclusively=exclusively)
         
         for i in range(neighborLayer):
             elements = self.groupElem.Get_Elements_Nodes(nodes=nodes, exclusively=exclusively)
             nodes = list(set(np.ravel(self.connect[elements])))
 
             if neighborLayer > 1 and elements.size == self.Ne:                
-                Display.myPrint("All the neighbors have been found.")
+                Display.MyPrint("All the neighbors have been found.")
                 break
 
         return elements
 
     def Nodes_Tags(self, tags: list[str]) -> np.ndarray:
         """Returns node associated with the tag."""
         nodes = []
@@ -512,15 +516,15 @@
 
         # get dictionnary linking tags to nodes
         dict_nodes = {}
         [dict_nodes.update(grp._dict_nodes_tags) for grp in self.dict_groupElem.values()]
         # add nodes belonging to the tags
 
         if len(dict_nodes) == 0:
-            Display.myPrintError("There is no tags available in the mesh, so don't forget to use the '_Set_PhysicalGroups()' function before meshing your geometry with '_Meshing()' in the gmsh interface 'Gmsh_Interface'.")
+            Display.MyPrintError("There is no tags available in the mesh, so don't forget to use the '_Set_PhysicalGroups()' function before meshing your geometry with '_Meshing()' in the gmsh interface 'Gmsh_Interface'.")
             return np.asarray([])
 
         [nodes.extend(dict_nodes[tag]) for tag in tags]
         # make sure that that the list is unique
         nodes = np.asarray(list(set(nodes)), dtype=int)
 
         return nodes
@@ -533,15 +537,15 @@
             tags = [tags]
 
         # get dictionnary linking tags to elements
         dict_elements = {}
         [dict_elements.update(grp._dict_elements_tags) for grp in self.dict_groupElem.values()]
 
         if len(dict_elements) == 0:            
-            Display.myPrintError("There is no tags available in the mesh, so don't forget to use the '_Set_PhysicalGroups()' function before meshing your geometry with '_Meshing()' in the gmsh interface 'Gmsh_Interface'.")
+            Display.MyPrintError("There is no tags available in the mesh, so don't forget to use the '_Set_PhysicalGroups()' function before meshing your geometry with '_Meshing()' in the gmsh interface 'Gmsh_Interface'.")
             return np.asarray([])
 
         # add elements belonging to the tags
         [elements.extend(dict_elements[tag]) for tag in tags]
         # make sure that that the list is unique
         elements = np.asarray(list(set(elements)), dtype=int)
 
@@ -783,15 +787,15 @@
 
                 angle_e_s[:,c] = np.abs(angle_e)
 
         if criteria == 'gamma':
             # only available for triangular elements
 
             if groupElem.elemType not in [ElemType.TRI3, ElemType.TRI6, ElemType.TRI10]:
-                Display.myPrintError("The gamma criterion is only available for triangular elements.")
+                Display.MyPrintError("The gamma criterion is only available for triangular elements.")
                 return None
 
             # inscribed circle
             # https://fr.wikipedia.org/wiki/Cercles_inscrit_et_exinscrits_d%27un_triangle
             rci_e = 2*area_e/p_e
             # circumscribed circle
             # https://fr.wikipedia.org/wiki/Cercle_circonscrit_%C3%A0_un_triangle
@@ -802,27 +806,27 @@
         elif criteria == "aspect":
             # hMin / hMax
             values_e = np.min(h_e_s, 1) / np.max(h_e_s, 1)
 
         elif criteria == "angular":
             # only available for 2d elements
             if groupElem.dim != 2:
-                Display.myPrintError("The angular criterion is only available for 2D elements.")
+                Display.MyPrintError("The angular criterion is only available for 2D elements.")
                 return None
 
             # min(angle) / max(angle)
             values_e = np.min(angle_e_s, 1) / np.max(angle_e_s, 1)
 
         elif criteria == "jacobian":
             # jMin / jMax
             jacobian_e_pg = groupElem.Get_jacobian_e_pg(MatrixType.mass)
             values_e = np.max(jacobian_e_pg, 1) / np.min(jacobian_e_pg, 1)
 
         else:
-            Display.myPrintError(f"The criterion ({criteria}) is not implemented")
+            Display.MyPrintError(f"The criterion ({criteria}) is not implemented")
 
         if nodeValues:
             return self.Get_Node_Values(values_e)
         else:
             return np.asarray(values_e)
 
     def Get_New_meshSize_n(self, error_e: np.ndarray, coef=1/2) -> np.ndarray:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/elems/_hexa.py` & `EasyFEA-1.0.2/EasyFEA/fem/elems/_hexa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Hexa element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
 
 class HEXA8(_GroupElem):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/elems/_prism.py` & `EasyFEA-1.0.2/EasyFEA/fem/elems/_prism.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Prism element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
 
 class PRISM6(_GroupElem):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/elems/_quad.py` & `EasyFEA-1.0.2/EasyFEA/fem/elems/_quad.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Quad element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
 
 class QUAD4(_GroupElem):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/elems/_seg.py` & `EasyFEA-1.0.2/EasyFEA/fem/elems/_seg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Seg element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
 
 class SEG2(_GroupElem):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/elems/_tetra.py` & `EasyFEA-1.0.2/EasyFEA/fem/elems/_tetra.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Tetra element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
 
 class TETRA4(_GroupElem):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/fem/elems/_tri.py` & `EasyFEA-1.0.2/EasyFEA/fem/elems/_tri.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Tri element module."""
 
 from ... import np, plt
 
 from .._group_elems import _GroupElem
 
 class TRI3(_GroupElem):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/materials/_beam.py` & `EasyFEA-1.0.2/EasyFEA/materials/_beam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from abc import ABC, abstractmethod, abstractproperty
 from typing import Union
 
 # utilities
 from .. import np
 # others
 from ..Geoms import Line, Normalize_vect, As_Coordinates
```

### Comparing `EasyFEA-1.0.1/EasyFEA/materials/_elastic.py` & `EasyFEA-1.0.2/EasyFEA/materials/_elastic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from abc import ABC, abstractmethod, abstractproperty
 from typing import Union
 
 # utilities
 from .. import np
 # others
 from ..Geoms import As_Coordinates
```

### Comparing `EasyFEA-1.0.1/EasyFEA/materials/_phasefield.py` & `EasyFEA-1.0.2/EasyFEA/materials/_phasefield.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from abc import ABC, abstractmethod, abstractproperty
 from typing import Union
 from enum import Enum
 
 from scipy.linalg import sqrtm
 
 # utilities
@@ -30,14 +34,17 @@
 class PhaseField(_IModel):
 
     class ReguType(str, Enum):
         """Available crack regularization"""
         AT1 = "AT1"
         AT2 = "AT2"
 
+        def __str__(self) -> str:
+            return self.name
+
     class SplitType(str, Enum):
         """Available splits"""
 
         # Isotropic
         Bourdin = "Bourdin" # [Bourdin 2000] DOI : 10.1016/S0022-5096(99)00028-9
         Amor = "Amor" # [Amor 2009] DOI : 10.1016/j.jmps.2009.04.011
         Miehe = "Miehe" # [Miehe 2010] DOI : 10.1016/j.cma.2010.04.011
@@ -55,26 +62,31 @@
 
         # spectral decomposition in stress
         AnisotStress = "AnisotStress"
         AnisotStress_PM = "AnisotStress_PM"
         AnisotStress_MP = "AnisotStress_MP"
         AnisotStress_NoCross = "AnisotStress_NoCross"
 
-    # Phase field
+        def __str__(self) -> str:
+            return self.name
+
     __SPLITS_ISOT = [SplitType.Amor, SplitType.Miehe, SplitType.Stress]
-    __SPLIT_ANISOT = [SplitType.Bourdin, SplitType.He, SplitType.Zhang,
+    __SPLITS_ANISOT = [SplitType.Bourdin, SplitType.He, SplitType.Zhang,
                     SplitType.AnisotStrain, SplitType.AnisotStrain_PM, SplitType.AnisotStrain_MP, SplitType.AnisotStrain_NoCross,
                     SplitType.AnisotStress, SplitType.AnisotStress_PM, SplitType.AnisotStress_MP, SplitType.AnisotStress_NoCross]
     
     class SolverType(str, Enum):
         """Solver used to manage crack irreversibility"""
         History = "History"
         HistoryDamage = "HistoryDamage"
         BoundConstrain = "BoundConstrain"
 
+        def __str__(self) -> str:
+            return self.name
+
     def __init__(self, material: _Elas, split: SplitType, regularization: ReguType, Gc: Union[float,np.ndarray], l0: float, solver=SolverType.History, A=None):
         """Creation of a gradient damage model
 
         Parameters
         ----------
         material : _Elas
             Elastic behavior (Elas_Isot, Elas_IsotTrans, Elas_Anisot)
@@ -122,15 +134,15 @@
     def thickness(self) -> float:
         return self.__material.thickness
     
     def __str__(self) -> str:
         text = str(self.__material)
         text += f'\n\n{type(self).__name__} :'
         text += f'\nsplit : {self.__split}'
-        text += f'\nregularisation : {self.__regularization}'
+        text += f'\nregularization : {self.__regularization}'
         text += f'\nGc : {self.__Gc:.4e}'
         text += f'\nl0 : {self.__l0:.4e}'
         return text
     
     @property
     def isHeterogeneous(self) -> bool:
         return isinstance(self.Gc, np.ndarray)
```

### Comparing `EasyFEA-1.0.1/EasyFEA/materials/_thermal.py` & `EasyFEA-1.0.2/EasyFEA/materials/_thermal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from typing import Union
 
 # utilities
 from .. import np
 
 from ._utils import _IModel, ModelType
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/materials/_utils.py` & `EasyFEA-1.0.2/EasyFEA/materials/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from abc import ABC, abstractmethod, abstractproperty
 from typing import Union
 from enum import Enum
 
 # utilities
 from ..utilities._observers import Observable
 from .. import np
@@ -14,14 +18,17 @@
     """Model types"""
 
     elastic = "elastic"
     damage = "damage"
     thermal = "thermal"
     beam = "beam"
 
+    def __str__(self) -> str:
+        return self.name
+
 class _IModel(ABC, Observable):
     """Model interface.
     """
 
     @abstractproperty
     def modelType(self) -> ModelType:
         """Model type"""
```

### Comparing `EasyFEA-1.0.1/EasyFEA/simulations/Solvers.py` & `EasyFEA-1.0.2/EasyFEA/simulations/Solvers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Interface module to various solvers available on python for solving linear systems of type [A](x) = (b)."""
 
 import sys
 from enum import Enum
 import numpy as np
 import scipy.sparse as sparse
 import scipy.optimize as optimize
@@ -53,22 +57,28 @@
     elliptic = "elliptic"
     """Solve K u = F"""
     parabolic = "parabolic"
     """Solve K u + C v = F"""
     hyperbolic = "hyperbolic"
     """Solve K u + C v + M a = F"""
 
+    def __str__(self) -> str:
+        return self.name
+
 class ResolType(str, Enum):
     r1 = "1"
     """ui = inv(Aii) * (bi - Aic * xc)"""
     r2 = "2"
     """Lagrange multiplier"""
     r3 = "3"
     """Penalty"""
 
+    def __str__(self) -> str:
+        return self.name
+
 def _Available_Solvers():
     """Available solvers."""
 
     solvers = ["scipy", "BoundConstrain", "cg", "bicg", "gmres", "lgmres"]
     
     if __canUsePypardiso: solvers.insert(0, "pypardiso")
     if __canUsePetsc: solvers.insert(1, "petsc")
@@ -114,39 +124,43 @@
     # check types
     simu = __Cast_Simu(simu)
     assert isinstance(A, sparse.csr_matrix)
     assert isinstance(b, sparse.csr_matrix)
 
     # Choose the solver
     if len(lb) > 0 and len(lb) > 0:        
-        solveur = "BoundConstrain"
+        solver = "BoundConstrain"
     else:
         if len(simu.Bc_Lagrange) > 0:
             # if lagrange multiplier are found we cannot use iterative solvers
-            solveur = "scipy"
+            solver = "scipy"
         else:
-            solveur = simu.solver
+            solver = simu.solver
 
     # import matplotlib.pyplot as plt
     # plt.figure()
     # plt.spy(A, marker='.')
-    testSymetric = sla.norm(A-A.transpose())/sla.norm(A)
-    A_isSymetric = testSymetric <= 1e-12
-    useCholesky = True if simu.problemType == 'elastic' else False
 
-    solveur = __Check_solveurLibrary(solveur)
-    
+    if not A.has_canonical_format:
+        # Using sla.norm(A) ensures that A has a cononic format. 
+        # Canonical Format means:
+        # - Within each row, indices are sorted by column.
+        # - There are no duplicate entries.
+        sla.norm(A)
+
+    solver = __Check_solverLibrary(solver)
+
     tic = Tic()
 
     sla.use_solver(useUmfpack=__canUseUmfpack)
     
-    if solveur == "pypardiso":
+    if solver == "pypardiso":
         x = pypardiso.spsolve(A, b.toarray())
 
-    elif solveur == "petsc":
+    elif solver == "petsc":
         global __pc_default
         # TODO find the best for damage problem
         kspType = 'cg'
         
         if simu.problemType == 'damage':
             if problemType == 'damage':
                 pcType = 'ilu'
@@ -164,60 +178,62 @@
         if not converg:
             print(f'\nWarning petsc did not converge with ksp:{kspType} and pc:{pcType} !')
             print(f'Try out with  ksp:{kspType} and pc:none.\n')
             __pc_default = 'none'
             x, option, converg = _PETSc(A, b, x0, kspType, 'none')
             assert converg, 'petsc didnt converge 2 times. check for kspType and pcType'
 
-        solveur += option
+        solver += option
     
-    elif solveur == "scipy":
+    elif solver == "scipy":
+        testSymetric = sla.norm(A-A.transpose())/sla.norm(A)
+        A_isSymetric = testSymetric <= 1e-12
         x = _ScipyLinearDirect(A, b, A_isSymetric)
     
-    elif solveur == "BoundConstrain":
+    elif solver == "BoundConstrain":
         x = _BoundConstrain(A, b , lb, ub)
 
-    elif solveur == "cg":
+    elif solver == "cg":
         x, output = sla.cg(A, b.toarray(), x0, maxiter=None)
 
-    elif solveur == "bicg":
+    elif solver == "bicg":
         x, output = sla.bicg(A, b.toarray(), x0, maxiter=None)
 
-    elif solveur == "gmres":
+    elif solver == "gmres":
         x, output = sla.gmres(A, b.toarray(), x0, maxiter=None)
 
-    elif solveur == "lgmres":
+    elif solver == "lgmres":
         x, output = sla.lgmres(A, b.toarray(), x0, maxiter=None)
         print(output)
 
-    elif solveur == "umfpack":
+    elif solver == "umfpack":
         # lu = umfpack.splu(A)
         # x = lu.solve(b).ravel()
         x = umfpackSpsolve(A, b)
 
-    elif solveur == "mumps":
+    elif solver == "mumps":
         # # TODO dont work yet
         # ctx = DMumpsContext()
         # if ctx.myid == 0:
         #     ctx.set_centralized_sparse(A)
         #     x = b.copy()
         #     ctx.set_rhs(x) # Modified in place
         # ctx.run(job=6) # Analysis + Factorization + Solve
         # ctx.destroy() # Cleanup
         x = mumps.spsolve(A,b)
             
-    tic.Tac("Solver",f"Solve {problemType} ({solveur})", simu._verbosity)
+    tic.Tac("Solver",f"Solve {problemType} ({solver})", simu._verbosity)
 
     # # A x - b = 0
     # residu = np.linalg.norm(A.dot(x)-b.toarray().ravel())
     # print(residu/np.linalg.norm(b.toarray().ravel()))
 
     return np.array(x)
 
-def __Check_solveurLibrary(solveur: str) -> str:
+def __Check_solverLibrary(solveur: str) -> str:
     """Checks whether the selected solver library is available
     If not, returns the solver usable in all cases (scipy)."""
     solveurDeBase="scipy"
     if solveur == "pypardiso":
         return solveur if __canUsePypardiso else solveurDeBase
     elif solveur == "umfpack":
         return solveur if __canUseUmfpack else solveurDeBase
@@ -393,18 +409,18 @@
     # nprocs = __comm.Get_size()
     # rank   = __comm.Get_rank()
     
     __comm = None
     petsc4py.init(sys.argv, comm=__comm)
 
     dimI = A.shape[0]
-    dimJ = A.shape[1]
+    dimJ = A.shape[1]    
 
     matrix = PETSc.Mat()
-    csr = (A.indptr, A.indices, A.data)    
+    csr = (A.indptr, A.indices, A.data)
     matrix.createAIJ([dimI, dimJ], comm=__comm, csr=csr)
 
     vectb = matrix.createVecLeft()
 
     lines, _, values = sparse.find(b)    
 
     vectb.array[lines] = values
@@ -421,15 +437,15 @@
     pc.setType(pcType)
 
     # pc.setFactorSolverType("superlu") #"mumps"
 
     ksp.solve(vectb, x)
     x = x.array
 
-    converg = ksp.converged and not ksp.diverged    
+    converg = ksp.is_converged
 
     # PETSc._finalize()
 
     option = f", {kspType}, {pcType}"
 
     return x, option, converg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/simulations/_beam.py` & `EasyFEA-1.0.2/EasyFEA/simulations/_beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from typing import Union
 import numpy as np
 from scipy import sparse
 
 # utilities
 from ..utilities import Display, Tic
 # fem
@@ -82,19 +86,19 @@
         """Displacement vector field.\n
         1D [uxi, ...]\n
         2D [uxi, uyi, rzi, ...]\n
         3D [uxi, uyi, uzi, rxi, ryi, rzi, ...]"""
         return self._Get_u_n(self.problemType)
 
     def add_surfLoad(self, nodes: np.ndarray, values: list, directions: list, problemType=None, description=""):
-        Display.myPrintError("It is impossible to apply a surface load in a beam problem.")
+        Display.MyPrintError("It is impossible to apply a surface load in a beam problem.")
         return        
 
     def add_volumeLoad(self, nodes: np.ndarray, values: list, directions: list, problemType=None, description=""):
-        Display.myPrintError("It is impossible to apply a volumetric load to a beam problem.")
+        Display.MyPrintError("It is impossible to apply a volumetric load to a beam problem.")
         return
 
     def add_connection_fixed(self, nodes: np.ndarray, description="Fixed"):
         """Adds a fixed connection.
 
         Parameters
         ----------
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/simulations/_dic.py` & `EasyFEA-1.0.2/EasyFEA/simulations/_dic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """DIC analysis module"""
 
 import numpy as np
 from scipy import interpolate, sparse
 from scipy.sparse.linalg import splu
-import matplotlib.pyplot as plt
 import pickle
 import cv2 # need opencv-python library
 
 # utilities
-from ..utilities import Folder, Tic
+from ..utilities import Tic, Folder
 # fem
 from ..fem import Mesh, BoundaryCondition
 
 class DIC:
 
     def __init__(self, mesh: Mesh, idxImgRef: int, imgRef: np.ndarray,
                  forces: np.ndarray=None, displacements: np.ndarray=None, lr=0.0, verbosity=False):
@@ -473,65 +476,49 @@
                 print(f"The displacement vector field is the wrong dimension. Must be of dimension {self.__nDof}")
                 return
 
             self._list_idx_exp.append(idx)
             self._list_u_exp.append(u_exp)
             self._list_img_exp.append(img)
 
-    def Save(self, pathname: str) -> None:
-        with open(pathname, 'wb') as file:
+    def Save(self, folder: str, filename: str="dic") -> None:
+        """Saves the dic analysis as 'filename.pickle'."""
+        path_dic = Folder.New_File(f"{filename}.pickle", folder)
+        with open(path_dic, 'wb') as file:
             self.__Op_LU = None
             self._M_LU = None
             pickle.dump(self, file)
 
-def Load(path: str) -> DIC:
-    """Loading procedure"""
-
-    if not Folder.Exists(path):
-        raise Exception(f"The analysis does not exist in {path}")
-
-    with open(path, 'rb') as file:
-        analyseDic = pickle.load(file)
-
-    assert isinstance(analyseDic, DIC)
-
-    return analyseDic
-
-def Calc_Energy(displacements: np.ndarray, forces: np.ndarray, ax=None) -> float:
-    """Function that calculates the energy under the curve."""
-
-    if isinstance(ax, plt.Axes):
-        ax.plot(displacements, forces)
-        canPlot = True
-    else:
-        canPlot = False
-
-    energie = 0
-
-    indexes = np.arange(displacements.shape[0]-1)
+# ----------------------------------------------
+# DIC Functions
+# ----------------------------------------------
 
-    for idx0 in indexes:
+def Load_DIC(folder: str, filename: str="dic") -> DIC:
+    """Load the dic analysis from the specified folder.
 
-        idx1 = idx0+1
-
-        idxs = [idx0, idx1]
-
-        ff = forces[idxs]
-
-        width = displacements[idx1]-displacements[idx0]
-        heightRectangle = np.min(ff)
-
-        heightTriangle = np.max(ff)-np.min(ff)
-
-        energie += width * (heightRectangle + heightTriangle/2)
+    Parameters
+    ----------
+    folder : str
+        The name of the folder where the simulation is saved.
+    filename : str, optional
+        The simualtion name, by default "dic".
+
+    Returns
+    -------
+    DIC
+        The loaded dic analysis."""
+    
+    path_dic = Folder.Join(folder, f"{filename}.pickle")
+    if not Folder.Exists(path_dic):
+        raise Exception(f"The dic analysis does not exist in {path_dic}")
 
-        if canPlot:
-            ax.fill_between(displacements[idxs], forces[idxs], color='red')
+    with open(path_dic, 'rb') as file:
+        dic: DIC = pickle.load(file)
 
-    return energie
+    return dic
 
 def Get_Circle(img:np.ndarray, threshold: float, boundary=None, radiusCoef=1.0) -> tuple[float, float, float]:
     """Recovers the circle in the image.
 
     Parameters
     ----------
     img : np.ndarray
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/simulations/_elastic.py` & `EasyFEA-1.0.2/EasyFEA/simulations/_elastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from typing import Union, Callable
 import numpy as np
 from scipy import sparse
 
 # utilities
 from ..utilities import Folder, Display, Tic
 # fem
@@ -325,15 +329,15 @@
                 raise Exception("Wrong option")
             
             res = result if result in ["Strain", "Stress"] else result[-2:]
             
             values = Result_in_Strain_or_Stress_field(val_e, res, coef)
 
         if not isinstance(values, np.ndarray):
-            Display.myPrintError("This result option is not implemented yet.")
+            Display.MyPrintError("This result option is not implemented yet.")
             return
 
         # end cases ----------------------------------------------------
         
         return self.Results_Reshape_values(values, nodeValues)
 
     def _Calc_Psi_Elas(self, returnScalar=True, smoothedStress=False, matrixType=MatrixType.rigi) -> float:
```

### Comparing `EasyFEA-1.0.1/EasyFEA/simulations/_phasefield.py` & `EasyFEA-1.0.2/EasyFEA/simulations/_phasefield.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from typing import Union
 import numpy as np
 from scipy import sparse
 import pandas as pd
 
 # utilities
 from ..utilities import Display, Tic
@@ -153,15 +157,15 @@
             if event == 'The model has been modified' and not self.needUpdate:
                 self.Need_Update()
         elif isinstance(observable, Mesh):
             if event == 'The mesh has been modified':
                 self._Check_dim_mesh_material()
                 self.Need_Update()
         else:
-            Display.myPrintError("Notification not yet implemented")
+            Display.MyPrintError("Notification not yet implemented")
 
     @property
     def needUpdate(self) -> bool:
         return not self.__updatedDamage or not self.__updatedDisplacement
 
     def Need_Update(self, value=True) -> None:        
         # the following functions help to avoid assembling matrices too many times
@@ -644,15 +648,15 @@
                 raise Exception("Wrong option")
             
             res = result if result in ["Strain", "Stress"] else result[-2:]
             
             values = Result_in_Strain_or_Stress_field(val_e, res, coef)
 
         if not isinstance(values, np.ndarray):
-            Display.myPrintError("This result option is not implemented yet.")
+            Display.MyPrintError("This result option is not implemented yet.")
             return
 
         # end cases ----------------------------------------------------
         
         return self.Results_Reshape_values(values, nodeValues)
 
     def __indexResult(self, resultat: str) -> int:
@@ -808,15 +812,15 @@
 
         if percentage > 0:
             timeLeft = (1/percentage-1)*timeIter*iter            
             timeCoef, unite = Tic.Get_time_unity(timeLeft)
             # Adds percentage and estimated time remaining
             summaryIter = summaryIter + f"{percentage*100:3.2f} % -> {timeCoef:3.2f} {unite}  "
 
-        Display.myPrint(summaryIter, end=end)
+        Display.MyPrint(summaryIter, end=end)
 
         self.__resumeIter = summaryIter
 
     def Results_Get_Iteration_Summary(self) -> str: 
         return self.__resumeIter
 
     def Results_dict_Energy(self) -> dict[str, float]:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/simulations/_simu.py` & `EasyFEA-1.0.2/EasyFEA/simulations/_simu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from abc import ABC, abstractmethod
 import pickle
 from datetime import datetime
 from typing import Union
 import numpy as np
 from scipy import sparse
 
@@ -360,38 +364,15 @@
             diff = np.linalg.norm(center - self.mesh.center)/np.linalg.norm(center)
             assert diff <= 1e-12
 
         return center
 
     # ----------------------------------------------
     # Solutions
-    # ----------------------------------------------
-
-    def Save(self, folder: str) -> None:
-        """Saves the simulation and its summary in the folder."""
-        # Empty matrices in element groups
-        self.mesh._ResetMatrix()
-
-        folder_EasyFEA = Folder.Get_Path(Folder.Get_Path()) # path the EasyFEA folder
-        # this path will be removed in print
-
-        # Save simulation
-        path_simu = Folder.New_File("simulation.pickle", folder)
-        with open(path_simu, "wb") as file:
-            pickle.dump(self, file)
-        Display.myPrint(f'Saved:\n{path_simu.replace(folder_EasyFEA,"")}\n', 'green')
-        
-        # Save simulation summary
-        path_summary = Folder.New_File("summary.txt", folder)
-        summary = f"Simulation completed on: {datetime.now()}"
-        summary += f"version: {__version__}"
-        summary += str(self)        
-        with open(path_summary, 'w', encoding='utf8') as file:
-            file.write(summary)
-        Display.myPrint(f'Saved:\n{path_summary.replace(folder_EasyFEA,"")}\n', 'green')
+    # ----------------------------------------------    
 
     # TODO Enable simulation creation from the variational formulation ?
 
     # Solutions
     @property
     def results(self) -> list[dict]:
         """Returns a copy of the dictionary list containing the results of each iteration."""
@@ -538,15 +519,15 @@
             if event == 'The model has been modified' and not self.needUpdate:
                 self.Need_Update()
         elif isinstance(observable, Mesh):
             if event == 'The mesh has been modified':
                 self._Check_dim_mesh_material()
                 self.Need_Update()
         else:
-            Display.myPrintError("Notification not yet implemented")
+            Display.MyPrintError("Notification not yet implemented")
 
     def Need_Update(self, value=True) -> None:
         """Set whether the simulation needs to reconstruct matrices K, C, M and F.
         """
         self.__needUpdate = value
 
     # ----------------------------------------------
@@ -571,15 +552,15 @@
 
         if self.problemType != "damage":
             solvers.remove("BoundConstrain")
 
         if value in solvers:
             self.__solver = value
         else:
-            Display.myPrintError(f"The solver {value} cannot be used. The solver must be in {solvers}")
+            Display.MyPrintError(f"The solver {value} cannot be used. The solver must be in {solvers}")
 
     def Solver_Set_Elliptic_Algorithm(self) -> None:
         """Set the algorithm's resolution properties for an elliptic problem.
 
         Used to solve K u = F.
         """
         self.__algo = AlgoType.elliptic
@@ -1199,19 +1180,19 @@
 
         if problemType is None:
             problemType = self.problemType
 
         self.__Check_problemTypes(problemType)
 
         if self.dim == 1:
-            Display.myPrintError("Cant apply pressure on 1D mesh.")
+            Display.MyPrintError("Cant apply pressure on 1D mesh.")
             return
 
         if len(self.Get_dofs(problemType)) == 0:
-            Display.myPrintError("Cant apply pressure on scalar problems.")
+            Display.MyPrintError("Cant apply pressure on scalar problems.")
             return
 
         dofsValues, dofs, nodes = self.__Bc_pressureload(problemType, nodes, magnitude)
 
         directions = self.Get_dofs(problemType)[:self.mesh.inDim]
 
         self.__Bc_Add_Neumann(problemType, nodes, dofsValues, dofs, directions, description)
@@ -1542,15 +1523,15 @@
 
     def _Results_Check_Available(self, result: str) -> bool:
         """Check that the result is available"""
         availableResults = self.Results_Available()
         if result in availableResults:
             return True
         else:
-            Display.myPrintError(f"\nFor a {self.problemType} problem result must be in : \n {availableResults}")
+            Display.MyPrintError(f"\nFor a {self.problemType} problem result must be in : \n {availableResults}")
             return False
 
     def Results_Set_Iteration_Summary(self) -> None:
         """Sets the iteration summary."""
         pass
 
     def Results_Get_Iteration_Summary(self) -> str:
@@ -1616,8 +1597,71 @@
                 # get values on every elements and nPe (Ne, nPe, i)
                 values_e_nPe = values_n[mesh.connect]
                 # get values on elements by averaging over the nodes per elements (nPe)
                 values_e: np.ndarray = np.mean(values_e_nPe, 1)
                 return values_e.reshape(shape)
 
         # We should never reach this line of code if no unexpected conditions occurs
-        raise Exception("Unexpected conditions occurred during the calculation.")
+        raise Exception("Unexpected conditions occurred during the calculation.")
+    
+    def Save(self, folder: str, filename: str="simulation", additionalInfos:str="") -> None:
+        """Saves the simulation and its summary in the folder. Saves the simulation as 'filename.pickle'."""
+        # Empty matrices in element groups
+        self.mesh._ResetMatrix()
+
+        folder_EasyFEA = Folder.Get_Path(Folder.Get_Path()) # path the EasyFEA folder
+        # this path will be removed in print
+
+        # Save simulation
+        path_simu = Folder.New_File(f"{filename}.pickle", folder)
+        with open(path_simu, "wb") as file:
+            pickle.dump(self, file)
+        Display.MyPrint(f'Saved:\n{path_simu.replace(folder_EasyFEA,"")}\n', 'green')
+        
+        # Save simulation summary
+        path_summary = Folder.New_File("summary.txt", folder)
+        summary = f"Simulation completed on: {datetime.now()}\n"
+        summary += f"version: {__version__}"
+        summary += str(self)
+        if str(additionalInfos) != "":
+            summary += Display.Section("Additional information", False)
+            summary += '\n' + str(additionalInfos)
+
+        with open(path_summary, 'w', encoding='utf8') as file:
+            file.write(summary)
+        Display.MyPrint(f'Saved:\n{path_summary.replace(folder_EasyFEA,"")}\n', 'green')
+
+# ----------------------------------------------
+# _Simu Functions
+# ----------------------------------------------
+
+def Load_Simu(folder: str, filename: str="simulation") -> _Simu:
+    """
+    Load the simulation from the specified folder.
+
+    Parameters
+    ----------
+    folder : str
+        The name of the folder where the simulation is saved.
+    filename : str, optional
+        The simualtion name, by default "simulation".
+
+    Returns
+    -------
+    _Simu
+        The loaded simulation.
+    """
+
+    folder_PythonEF = Folder.Get_Path(Folder.Get_Path())
+    path_simu = Folder.Join(folder, f"{filename}.pickle")
+    assert Folder.Exists(path_simu), f"The file {filename}.pickle cannot be found."
+
+    try:
+        with open(path_simu, 'rb') as file:
+            simu: _Simu = pickle.load(file)
+    except EOFError:
+        Display.MyPrintError(f"The file:\n{path_simu}\nis empty or corrupted.")
+        return None    
+    
+    Display.MyPrint(f'\nLoaded:\n{path_simu.replace(folder_PythonEF,"")}\n', 'green')
+
+    return simu
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/simulations/_thermal.py` & `EasyFEA-1.0.2/EasyFEA/simulations/_thermal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 from typing import Union
 import numpy as np
 from scipy import sparse
 
 # utilities
 from ..utilities import Tic
 # fem
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/utilities/Display.py` & `EasyFEA-1.0.2/EasyFEA/utilities/Display.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Module containing functions used to display simulations and meshes with matplotlib (https://matplotlib.org/)."""
 
 import platform
 from typing import Union, Callable
 import numpy as np
 import pandas as pd
 from enum import Enum
@@ -73,15 +77,15 @@
     -------
     Figure, Axis, colorbar
         fig, ax, cb
     """
     
     tic = Tic()
 
-    simu, mesh, coordo, inDim = _init_obj(obj, deformFactor)
+    simu, mesh, coordo, inDim = _Init_obj(obj, deformFactor)
     plotDim = mesh.dim # plot dimension
 
     # I dont know how to display nodal values on lines
     nodeValues = False if plotDim == 1 else nodeValues
 
     # When mesh use 3D elements, results are displayed only on 2D elements.
     # To display values on 2D elements, we first need to know the values at 3D nodes.
@@ -136,15 +140,15 @@
         inDim = 3 if ax.name == '3d' else inDim
 
     if inDim in [1,2]:
         # Mesh contained in a 2D plane
         # Only designed for one element group!
 
         if ax == None:
-            ax = init_Axes()
+            ax = Init_Axes()
             fig = ax.figure
             ax.set_xlabel(r"$x$")
             ax.set_ylabel(r"$y$")
 
         # construct coordinates for each elements
         faces = mesh.groupElem.faces
         connectFaces = mesh.connect[:,faces]
@@ -197,24 +201,24 @@
         # If the mesh is a 3D mesh, only the 2D elements of the mesh will be displayed.
         # A 3D mesh can contain several types of 2D element.
         # For example, when PRISM6 -> TRI3 and QUAD4 at the same time
 
         plotDim = 2 if plotDim == 3 else plotDim
 
         if ax == None:
-            ax = init_Axes(3)
+            ax = Init_Axes(3)
             fig = ax.figure
             ax.set_xlabel(r"$x$")
             ax.set_ylabel(r"$y$")
             ax.set_zlabel(r"$z$")
 
         # constructs the face connection matrix
         connectFaces = []
         groupElems = mesh.Get_list_groupElem(plotDim)
-        list_faces = _get_list_faces(mesh, plotDim)
+        list_faces = _Get_list_faces(mesh, plotDim)
         for groupElem, faces in zip(groupElems, list_faces):            
             connectFaces.extend(groupElem.connect[:,faces])
         connectFaces = np.asarray(connectFaces, dtype=int)
 
         elements_coordinates: np.ndarray = coordo[connectFaces, :3]
 
         if nodeValues:
@@ -324,29 +328,29 @@
     Returns
     -------
     plt.Axes
     """
     
     tic = Tic()
 
-    simu, mesh, coordo, inDim = _init_obj(obj, deformFactor)
+    simu, mesh, coordo, inDim = _Init_obj(obj, deformFactor)
 
     if ax != None:
         inDim = 3 if ax.name == '3d' else inDim
 
     deformFactor = 0 if simu == None else np.abs(deformFactor)
 
     # Dimensions of displayed elements
     dimElem = mesh.dim 
     # If the mesh is a 3D mesh, only the 2D elements of the mesh will be displayed.    
     if dimElem == 3: dimElem = 2
     
     # constructs the connection matrix for the faces
     list_groupElem = mesh.Get_list_groupElem(dimElem)
-    list_faces = _get_list_faces(mesh, dimElem)
+    list_faces = _Get_list_faces(mesh, dimElem)
     connectFaces = []
     for groupElem, faces in zip(list_groupElem, list_faces):
         connectFaces.extend(groupElem.connect[:,faces])
     connectFaces = np.asarray(connectFaces, dtype=int)
 
     # faces coordinates
     coordFacesDef: np.ndarray = coordo[connectFaces, :inDim]
@@ -356,15 +360,15 @@
         title = f"{mesh.elemType} : Ne = {mesh.Ne}, Nn = {mesh.Nn}"
     
         
     if inDim in [1,2]:
         # in 2d space
 
         if ax == None:
-            ax = init_Axes()
+            ax = Init_Axes()
             ax.set_xlabel(r"$x$")
             ax.set_ylabel(r"$y$")
             ax.set_title(title)
 
         if deformFactor > 0:            
             # Deformed mesh
             pc = LineCollection(coordFacesDef, edgecolor='red', lw=lw, antialiaseds=True, zorder=1)
@@ -391,15 +395,15 @@
         if ax.name != '3d':
             ax.axis('equal')
 
     elif inDim == 3:
         # in 3d space
 
         if ax == None:
-            ax = init_Axes(3)
+            ax = Init_Axes(3)
             ax.set_xlabel(r"$x$")
             ax.set_ylabel(r"$y$")
             ax.set_zlabel(r"$z$")
             ax.set_title(title)
 
         if deformFactor > 0:
             # Displays only 1D or 2D elements, depending on the mesh type
@@ -465,20 +469,20 @@
     Returns
     -------
     plt.Axes
     """
     
     tic = Tic()
     
-    mesh = _init_obj(mesh)[1]
+    mesh = _Init_obj(mesh)[1]
 
     inDim = mesh.inDim
 
     if ax == None:
-        ax = init_Axes(inDim)
+        ax = Init_Axes(inDim)
         ax.set_title("")
     else:        
         inDim = 3 if ax.name == '3d' else inDim
     
     if len(nodes) == 0:
         nodes = mesh.nodes
     else:
@@ -536,15 +540,15 @@
         dimElem = 2 if mesh.inDim == 3 else mesh.dim
 
     # list of element group associated with the dimension
     list_groupElem = mesh.Get_list_groupElem(dimElem)[:1]
     if len(list_groupElem) == 0: return
 
     if ax == None:
-        ax = init_Axes(inDim)
+        ax = Init_Axes(inDim)
     else:        
         inDim = 3 if ax.name == '3d' else inDim
 
     # for each group elem
     for groupElem in list_groupElem:
 
         # get the elements associated with the nodes
@@ -706,29 +710,29 @@
     Returns
     -------
     plt.Axes
     """
 
     tic = Tic()
 
-    simu, mesh, coordo, inDim = _init_obj(obj, 0.0)
+    simu, mesh, coordo, inDim = _Init_obj(obj, 0.0)
 
     # check if there is available tags in the mesh
     nTtags = [np.max([len(groupElem.nodeTags), len(groupElem.elementTags)]) for groupElem in mesh.dict_groupElem.values()]
     if np.max(nTtags) == 0:
-        myPrintError("There is no tags available in the mesh, so don't forget to use the '_Set_PhysicalGroups()' function before meshing your geometry with '_Meshing()' in the gmsh interface 'Gmsh_Interface'.")
+        MyPrintError("There is no tags available in the mesh, so don't forget to use the '_Set_PhysicalGroups()' function before meshing your geometry with '_Meshing()' in the gmsh interface 'Gmsh_Interface'.")
         return
 
     if ax == None:
         if mesh.inDim <= 2:
-            ax = init_Axes()
+            ax = Init_Axes()
             ax.set_xlabel(r"$x$")
             ax.set_ylabel(r"$y$")
         else:
-            ax = init_Axes(3)
+            ax = Init_Axes(3)
             ax.set_xlabel(r"$x$")
             ax.set_ylabel(r"$y$")
             ax.set_zlabel(r"$z$")
         fig = ax.figure
     else:
         fig = ax.figure
         inDim = 3 if ax.name == '3d' else inDim
@@ -893,15 +897,15 @@
         returns figure and ax
     """
 
     if isinstance(ax, plt.Axes):
         fig = ax.figure
         ax.clear()
     else:        
-        ax = init_Axes()
+        ax = Init_Axes()
         fig = ax.figure
 
     ax.plot(np.abs(displacement), np.abs(force), c='blue')
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     ax.grid()
 
@@ -990,15 +994,15 @@
         listX = iterations 
         xlabel = "iter"    
 
     # Transforms list_dict_Energie into a dataframe
     df = pd.DataFrame(list_dict_Energy)
 
     # Affiche les energies
-    row = next(iter_rows)
+    row: int = next(iter_rows)
     # For each energy, we plot the values
     for energie_str in df.columns:
         valeurs = df[energie_str].values
         axs[row].plot(listX, valeurs, label=energie_str)    
     axs[row].legend()
     axs[row].grid()
 
@@ -1049,15 +1053,15 @@
     
     selectionIndex = list(filter(lambda iterations: iterations >= iterMin and iterations <= iterMax, iterations))
 
     nbGraph = len(list_label_values)
 
     iterations = iterations[selectionIndex]
 
-    fig, axs = plt.subplots(nrows=nbGraph, sharex=True)
+    axs: list[plt.Axes] = plt.subplots(nrows=nbGraph, sharex=True)[1]
     
     for ax, label_values in zip(axs, list_label_values):
         ax.grid()
         ax.plot(iterations, label_values[1][iterations], color='blue')
         ax.set_ylabel(label_values[0])
 
     ax.set_xlabel("iterations")
@@ -1095,25 +1099,25 @@
         Plot the mesh, by default False
     edgecolor : str, optional
         Color used to plot the mesh, by default 'black'
     fps : int, optional
         frames per second, by default 30
     """
 
-    simu = _init_obj(simu)[0]
+    simu = _Init_obj(simu)[0]
 
     if simu is None:
-        myPrintError("Must give a simulation.")
+        MyPrintError("Must give a simulation.")
         return
 
     Niter = len(simu.results)
     step = np.max([1, Niter//N])
     iterations: np.ndarray = np.arange(0, Niter, step)
 
-    ax = init_Axes(simu.mesh.inDim)
+    ax = Init_Axes(simu.mesh.inDim)
     fig = ax.figure
 
     def DoAnim(fig: plt.Figure, i):
         simu.Set_Iter(iterations[i])
         ax = fig.axes[0]
         Plot_Result(simu, result, deformFactor, coef, nodeValues, plotMesh, edgecolor, ax=ax)
         ax.set_title(f"{result} {iterations[i]:d}/{Niter-1:d}")
@@ -1202,17 +1206,15 @@
     
     tic = Tic()
 
     plt.savefig(path, dpi=dpi, transparent=transparent, bbox_inches='tight')
 
     tic.Tac("Display","Save figure")
 
-# TODO TO Upper case
-
-def _init_obj(obj, deformFactor: float=0.0):
+def _Init_obj(obj, deformFactor: float=0.0):
     """Return (simu, mesh, coordo, inDim) from an ojbect that could be either a _Simu or a Mesh object.
     
     Parameters
     ----------
     obj : _Simu | Mesh | _GroupElem
         An object that contain the mesh
     deformFactor : float, optional
@@ -1242,15 +1244,15 @@
         coordo = mesh.coordGlob
         inDim = mesh.inDim
     else:
         raise Exception("Must be a simulation or a mesh")
     
     return simu, mesh, coordo, inDim
 
-def _get_list_faces(mesh: Mesh, dimElem:int) -> list[list[int]]:
+def _Get_list_faces(mesh: Mesh, dimElem:int) -> list[list[int]]:
     """Construct a list of faces for each element group of dimension dimElem.\n
     Faces is a list of index used to construct/plot a faces.\n
     You can go check their values for each groupElem in /fem/elems/"""
     
     assert isinstance(mesh, Mesh), "mesh must be a Mesh object"
 
     list_faces: list[list[int]] = [] # list of faces
@@ -1268,15 +1270,15 @@
         repeat = max_len-len(faces)
         if repeat > 0:
             faces.extend([faces[0]]*repeat)
             list_faces[f] = faces
 
     return list_faces
 
-def init_Axes(dim: int=2, elev=105, azim=-90) -> Union[plt.Axes, Axes3D]:
+def Init_Axes(dim: int=2, elev=105, azim=-90) -> Union[plt.Axes, Axes3D]:
     if dim == 1 or dim == 2:
         ax = plt.subplots()[1]
     elif dim == 3:
         fig = plt.figure()
         ax: Axes3D = fig.add_subplot(projection="3d")
         ax.view_init(elev=elev, azim=azim)
     return ax
@@ -1325,50 +1327,50 @@
 
 class __Sytles(str, Enum):
     BOLD = '\033[1m'
     ITALIC = '\033[3m'
     UNDERLINE = '\033[4m'
     RESET = '\33[0m'
 
-def myPrint(text: str, color='cyan', bold=False, italic=False, underLine=False, end:str=None) -> None:
+def MyPrint(text: str, color='cyan', bold=False, italic=False, underLine=False, end:str=None) -> None:
 
     dct = dict(map(lambda item: (item.name, item.value), __Colors))
 
     if color not in dct:
-        myPrint(f"Color must be in {dct.keys()}", 'red')
+        MyPrint(f"Color must be in {dct.keys()}", 'red')
     
     else:    
         formatedText = ""
 
         if bold: formatedText += __Sytles.BOLD
         if italic: formatedText += __Sytles.ITALIC
         if underLine: formatedText += __Sytles.UNDERLINE
         
         formatedText += dct[color] + str(text)
 
         formatedText += __Sytles.RESET
 
         print(formatedText, end=end)
     
-def myPrintError(text: str) -> str:
-    return myPrint(text, 'red')
+def MyPrintError(text: str) -> str:
+    return MyPrint(text, 'red')
 
 def Section(text: str, verbosity=True) -> None:
     """New section."""    
     edges = "======================="
 
     lengthText = len(text)
 
     lengthTot = 45
 
     edges = "="*int((lengthTot - lengthText)/2)
 
     section = f"\n\n{edges} {text} {edges}\n"
 
-    if verbosity: myPrint(section)
+    if verbosity: MyPrint(section)
 
     return section
 
 def Clear() -> None:
     """Clear the terminal."""
     syst = platform.system()
     if syst in ["Linux","Darwin"]:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/utilities/Folder.py` & `EasyFEA-1.0.2/EasyFEA/utilities/Folder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Module containing functions used to facilitate folder and file creation using (os)."""
 
 import os
 
 def Get_Path(filename="") -> str:
     """Returns the folder containing the file. Otherwise returns the EasyFEA folder."""
     
@@ -101,10 +105,10 @@
         workFolder = Join(folder, "Test", name)
     else:
         workFolder = Join(folder, name)
 
     path_PythonEf = Get_Path(Get_Path())
     
     from . import Display
-    Display.myPrint(workFolder.replace(path_PythonEf,""), 'green')
+    Display.MyPrint(workFolder.replace(path_PythonEf,""), 'green')
 
     return Join(path, workFolder)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/utilities/Numba_Interface.py` & `EasyFEA-1.0.2/EasyFEA/utilities/Numba_Interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Numba functions to speed up calculations."""
 
 import numpy as np
 from numba import njit, prange, jit
 
 __USE_CACHE = True
 __USE_PARALLEL = True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/utilities/Paraview_Interface.py` & `EasyFEA-1.0.2/EasyFEA/utilities/Paraview_Interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """This module allows you to save a simulation on Paraview (https://www.paraview.org/)."""
 
 import numpy as np
 
 # utilities
 from . import Display, Folder, Tic
 
@@ -26,15 +30,15 @@
     elementsField: list, optional
         Additional elementsField, by default []
     """
     print('\n')
 
     vtuFiles: list[str] = []
 
-    simu = Display._init_obj(simu)[0]
+    simu = Display._Init_obj(simu)[0]
 
     results = simu.results
 
     Niter = len(results)
     step = np.max([1, Niter//N])
     iterations: np.ndarray = np.arange(0, Niter, step)
 
@@ -53,30 +57,30 @@
 
     [nodesField.append(n) for n in additionalNodesField
      if simu._Results_Check_Available(n) and n not in nodesField]
     [elementsField.append(e) for e in additionalElementsField
      if simu._Results_Check_Available(e) and e not in elementsField]
 
     if len(nodesField) == 0 and len(elementsField) == 0:
-        Display.myPrintError("The simulation has no solution fields to display in paraview.")
+        Display.MyPrintError("The simulation has no solution fields to display in paraview.")
 
     for i, iter in enumerate(iterations):
 
         f = Folder.Join(folder,f'solution_{iter}.vtu')
 
         __Make_vtu(simu, iter, f, nodesField=nodesField, elementsField=elementsField)
         
         # vtuFiles.append(vtuFile)
         vtuFiles.append(f'solution_{iter}.vtu')
         
         times.append(tic.Tac("Paraview","Make vtu", False))
 
         rmTime = Tic.Get_Remaining_Time(i, iterations.size-1, times[-1])
 
-        Display.myPrint(f"SaveParaview {i}/{iterations.size-1} {rmTime}     ", end='\r')
+        Display.MyPrint(f"SaveParaview {i}/{iterations.size-1} {rmTime}     ", end='\r')
     
     print('\n')
 
     tic = Tic()
 
     filenamePvd = Folder.os.path.join(folder,"simulation")    
     __Make_pvd(filenamePvd, vtuFiles)
@@ -107,15 +111,15 @@
 # ----------------------------------------------
 # Functions
 # ----------------------------------------------
 def __Make_vtu(simu, iter: int, filename: str, nodesField: list[str], elementsField: list[str]):
     """Create the .vtu (as a binary files) which can be read on paraview
     """
 
-    simu = Display._init_obj(simu)[0]
+    simu = Display._Init_obj(simu)[0]
 
     options = nodesField+elementsField
    
     simu.Set_Iter(iter)
 
     # Checking the compatibility of the results list with the simulation
     for option in options:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/EasyFEA/utilities/PyVista_Interface.py` & `EasyFEA-1.0.2/EasyFEA/utilities/PyVista_Interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Module providing an interface with PyVista (https://docs.pyvista.org/version/stable/)."""
 
 from typing import Union, Callable
 from cycler import cycler
 from scipy.sparse import csr_matrix
 import pyvista as pv
 import numpy as np
 
 # utilities
-from .Display import myPrintError, _init_obj, myPrint
+from .Display import MyPrintError, _Init_obj, MyPrint
 from . import Folder, Tic
 # fem
 from ..fem import GroupElemFactory
 
 def Plot(obj, result: Union[str,np.ndarray]=None, deformFactor=0.0, coef=1.0, nodeValues=True, 
                 color=None, show_edges=False, edge_color='k', line_width=None,
                 show_vertices=False, point_size=None, opacity=1.0,
@@ -74,15 +78,15 @@
     # initiate the obj to construct the grid
     if isinstance(obj, (pv.MultiBlock, pv.PolyData, pv.UnstructuredGrid)):
         inDim = 3
         pvMesh = obj        
         result = result if result in pvMesh.array_names else None
     else:
         pvMesh = _pvGrid(obj, result, deformFactor, nodeValues)
-        inDim = _init_obj(obj)[-1]
+        inDim = _Init_obj(obj)[-1]
 
     if pvMesh is None:
         # something do not work during the grid creation≠
         return
     
     # apply coef to the array
     name = "array" if isinstance(result, np.ndarray) else result
@@ -175,32 +179,32 @@
 
     Returns
     -------
     pv.Plotter
         The pyvista plotter
     """
 
-    simu, mesh, coordo, inDim = _init_obj(obj, deformFactor)   
+    simu, mesh, coordo, inDim = _Init_obj(obj, deformFactor)   
 
     if nodes is None:
         nodes = mesh.nodes
         coordo = coordo[nodes]
     else:
         nodes = np.asarray(nodes)
 
         if nodes.ndim == 1:
             if nodes.size > mesh.Nn:
-                myPrintError("The list of nodes must be of size <= mesh.Nn")
+                MyPrintError("The list of nodes must be of size <= mesh.Nn")
                 return
             else:
                 coordo = coordo[nodes]
         elif nodes.ndim == 2 and nodes.shape[1] == 3:
             coordo = nodes
         else:
-            myPrintError("Nodes must be either a list of nodes or a matrix of 3D vectors of dimension (n, 3).")
+            MyPrintError("Nodes must be either a list of nodes or a matrix of 3D vectors of dimension (n, 3).")
             return
 
     if plotter == None:
         plotter = Plot(obj, deformFactor=deformFactor, style='wireframe', color='k')
 
     pvData = pv.PolyData(coordo)
 
@@ -241,24 +245,24 @@
 
     Returns
     -------
     pv.Plotter
         The pyvista plotter
     """
 
-    simu, mesh, coordo, inDim = _init_obj(obj, deformFactor)
+    simu, mesh, coordo, inDim = _Init_obj(obj, deformFactor)
     
     dimElem = mesh.dim if dimElem == None else dimElem
 
     if nodes is None:
         nodes = mesh.nodes
     else:
         nodes = np.asarray(nodes)
         if nodes.ndim != 1 or nodes.size > mesh.Nn:
-            myPrintError("Nodes must be a list of nodes of size <= mesh.Nn.")
+            MyPrintError("Nodes must be a list of nodes of size <= mesh.Nn.")
             return
 
     if plotter == None:
         plotter = Plot(obj, deformFactor=deformFactor, style='wireframe', color=edge_color, line_width=line_width)
 
     
     
@@ -305,18 +309,18 @@
     pv.Plotter
         The pyvista plotter
     """
 
     tic = Tic()
 
     
-    simu, mesh, coordo, inDim = _init_obj(simu, deformFactor)
+    simu, mesh, coordo, inDim = _Init_obj(simu, deformFactor)
 
     if simu is None:
-        myPrintError('simu must be a _Simu object')
+        MyPrintError('simu must be a _Simu object')
         return
 
     # get dirichlet and neumann boundary conditions
     dirchlets = simu.Bc_Dirichlet
     BoundaryConditions = dirchlets
     neumanns = simu.Bc_Neuman
     BoundaryConditions.extend(neumanns)
@@ -521,18 +525,18 @@
         Factor used to display the deformed solution (0 means no deformations), default 0.0
     coef : float, optional
         Coef to apply to the solution, by default 1.0
     nodeValues : bool, optional
         Displays result to nodes otherwise displays it to elements, by default True
     """
     
-    simu = _init_obj(simu)[0]
+    simu = _Init_obj(simu)[0]
 
     if simu is None:
-        myPrintError("Must give a simulation.")
+        MyPrintError("Must give a simulation.")
         return
 
     Niter = len(simu.results)
     step = np.max([1, Niter//N])
     iterations: np.ndarray = np.arange(0, Niter, step)
 
     def DoAnim(plotter, i):        
@@ -580,15 +584,15 @@
 
         plotter.write_frame()
 
         time = tic.Tac("PyVista_Interface",f"Movie_func", False)        
 
         rmTime = Tic.Get_Remaining_Time(i, N-1, time)
 
-        myPrint(f"Movie_func {i}/{N-1} {rmTime}    ", end='\r')
+        MyPrint(f"Movie_func {i}/{N-1} {rmTime}    ", end='\r')
 
     print()
     plotter.close()    
 
 # ----------------------------------------------
 # Functions
 # ----------------------------------------------
@@ -625,22 +629,22 @@
         plotter.camera.elevation += 25
         plotter.camera.azimuth += 10
         plotter.camera.reset_clipping_range()
 
 def _pvGrid(obj, result: Union[str, np.ndarray]=None, deformFactor=0.0, nodeValues=True) -> pv.UnstructuredGrid:
     """Construct the pyvista mesh from obj (_Simu, Mesh, _GroupElem and _Geoms object)"""
 
-    simu, mesh, coordo, inDim = _init_obj(obj, deformFactor)
+    simu, mesh, coordo, inDim = _Init_obj(obj, deformFactor)
 
     elemType = mesh.elemType
     Nn = mesh.Nn
     Ne = mesh.Ne
 
     if elemType not in __dictCellTypes.keys():
-        myPrintError(f"{elemType} is not implemented yet.")
+        MyPrintError(f"{elemType} is not implemented yet.")
         return
     
     cellType = __dictCellTypes[elemType]
     
     # reorganize the connectivity order 
     # because some elements in gmsh don't have the same numbering order as in vtk
     # pyvista -> https://docs.pyvista.org/version/stable/api/core/_autosummary/pyvista.UnstructuredGrid.celltypes.html
@@ -674,26 +678,26 @@
                 if size % Nn == 0:
                     values = np.reshape(values, (Nn, -1))
                 elif size % Ne == 0:
                     values = np.reshape(values, (Ne, -1))
                 pvMesh[result] = values
                 pvMesh.set_active_scalars(result)
             else:
-                myPrintError("Must return nodes or elements values")
+                MyPrintError("Must return nodes or elements values")
                 
         else:
-            myPrintError("obj must be a simulation object or result should be nodes or elements values.")
+            MyPrintError("obj must be a simulation object or result should be nodes or elements values.")
 
     elif isinstance(result, np.ndarray):
         values = result
         size = result.size
         name = 'array' # here result is an array
 
         if size % Nn == 1 or size % Ne == 1:
-            myPrintError("Must be nodes or elements values")
+            MyPrintError("Must be nodes or elements values")
         else:
             if size % Ne == 0 and nodeValues:
                 # elements values that we want to plot on nodes
                 values = mesh.Get_Node_Values(values)
                 
             elif size % Nn == 0 and not nodeValues:
                 # nodes values that we want to plot on elements
@@ -705,15 +709,15 @@
     return pvMesh
 
 def _pvGeom(geom) -> Union[pv.DataSet, list[pv.DataSet]]:
 
     import Geoms
 
     if not isinstance(geom, (Geoms.Point, Geoms._Geom)):
-        myPrintError("Must be a point or a geometric object.")
+        MyPrintError("Must be a point or a geometric object.")
         return None
     
     def __Line(line: Geoms.Line):
         return pv.Line(line.pt1.coord, line.pt2.coord)        
     
     def __CircleArc(circleArc: Geoms.CircleArc):
         dataSet = pv.CircularArc(circleArc.pt1.coord, circleArc.pt2.coord,
@@ -757,10 +761,10 @@
             geoms = geom.Get_Contour().geoms
             if geom.isOpen:
                 geoms = geoms[:-1]
         else:
             geoms = geom.geoms
         dataSet = __DoGeoms(geoms)
     else:
-        myPrintError("obj must be in [Point, Line, Domain, Circle, CircleArc, Contour, Points]")
+        MyPrintError("obj must be in [Point, Line, Domain, Circle, CircleArc, Contour, Points]")
 
     return dataSet
```

### Comparing `EasyFEA-1.0.1/EasyFEA/utilities/_tic.py` & `EasyFEA-1.0.2/EasyFEA/utilities/_tic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+# This file is part of the EasyFEA project.
+# EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+
 """Module containing the Tic class for timing tasks."""
 
 import time
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
```

### Comparing `EasyFEA-1.0.1/EasyFEA.egg-info/PKG-INFO` & `EasyFEA-1.0.2/EasyFEA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyFEA
-Version: 1.0.1
+Version: 1.0.2
 Summary: User-friendly Python library that simplifies finite element analysis.
 Author-email: Matthieu Noel <matthieu.noel7@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,29 +688,45 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+License-File: AUTHORS.md
+Requires-Dist: numpy
+Requires-Dist: gmsh>=4.12
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pyvista
+Requires-Dist: numba
+Requires-Dist: pandas
+Requires-Dist: imageio
+Requires-Dist: imageio[ffmpeg]
 Provides-Extra: fast
+Requires-Dist: pypardiso; extra == "fast"
+Requires-Dist: petsc; extra == "fast"
+Requires-Dist: petsc4py; extra == "fast"
 Provides-Extra: cv
-License-File: LICENSE.txt
+Requires-Dist: opencv-python; extra == "cv"
 
 # EasyFEA - Easy Finite Element Analysis
 
 ## Overview
 
 **EasyFEA** is a user-friendly Python library that simplifies finite element analysis. It is flexible and supports different types of simulation without requiring users to handle complex PDE formulations. The library currently supports four specific simulation types:
 
 1. **ElasticSimu** (static and dynamic): Examples in `/examples/Elastic`, `/examples/Dynamic` and `/examples/Contact`.
 2. **BeamSimu** (static Euler-Bernoulli): Examples in `/examples/Beam`.
 3. **ThermalSimu** (stationary and transient): Examples in `/examples/Thermal`.
 4. **PhaseFieldSimu:** (quasi-static phase field) Examples in `/examples/PhaseField`.
 
+All examples are available [here](https://github.com/matnoel/EasyFEA/tree/master/examples).
+
 For each simulation, users create a **mesh** and a **model**. Once the simulation has been set up, defining the boundary conditions, solving the problem and visualizing the results is straightforward.
 
 Numerous examples of mesh creation are available in the `examples/Meshes` folder.
 
 The simplest and quickest introduction is shown below and is available in `examples/HelloWorld.py`.
 
 ```python
@@ -753,16 +769,14 @@
 Display.Plot_BoundaryConditions(simu)
 Display.Plot_Result(simu, 'uy', plotMesh=True)
 Display.Plot_Result(simu, 'Svm', plotMesh=True, ncolors=11)
 
 Display.plt.show()
 ```
 
-All examples are available [here](https://github.com/matnoel/EasyFEA/tree/master/examples).
-
 ## Installation
 
 EasyFEA can be easily installed from [PyPI](https://pypi.org/project/EasyFEA/) using pip, compatible with Python versions 3.9 through 3.12:
 
 ```
 pip install EasyFEA
 ```
@@ -784,37 +798,57 @@
 
 ### Optional Dependencies
 
 EasyFEA includes a few optional dependencies for reducing resolution time or for performing DIC:
 
 + [`pypardiso`](https://pypi.org/project/pypardiso/) (Python > 3.8 & Intel oneAPI)  - Library for solving large systems of sparse linear equations.
 + [`petsc`](https://pypi.org/project/petsc/) and [`petsc4py`](https://pypi.org/project/petsc4py/) - Python bindings for PETSc.
-+ [opencv-python](https://pypi.org/project/opencv-python/) - Computer Vision package.
++ [`opencv-python`](https://pypi.org/project/opencv-python/) - Computer Vision package.
 
 # Naming conventions
 
 **EasyFEA** uses Object-Oriented Programming ([OOP](https://en.wikipedia.org/wiki/Object-oriented_programming)) with the following naming conventions:
 + `PascalCasing` for classes
 + `camelCasing` for properties
 + `Snake_Casing` or `Snake_casing` for functions/methods
 
 In this library, objects can contain both **public** and **private** properties or functions.
 
 **Private** parameters or functions are designated by a double underscore, such as `__privateParam`. In addition, parameters or functions beginning with an underscore, such as `_My_Function` are accessible to advanced users, but should be used with caution.
 
 # Contributing
 
-Contributors are welcome! To contribute please use the following commands.
+**EasyFEA** is an emerging project with a strong commitment to growth and improvement. Your input and ideas are invaluable to me. I welcome your comments and advice with open arms, encouraging a culture of respect and kindness in our collaborative journey towards improvement.
 
-```
-git clone https://github.com/matnoel/EasyFEA.git
-cd EasyFEA
-python -m pip install -e .
-```
+To learn more about contributing to EasyFEA, please consult the [Contributing Guide](https://github.com/matnoel/EasyFEA/blob/main/CONTRIBUTING.md).
 
-To develop a new feature, start by creating a new branch in the project using the command `git branch my_new_feature`. After implementing and testing your modifications (refer to EasyFEA/tests), proceed to create a pull request to merge your changes.
+# Citing EasyFEA
 
-**EasyFEA** is an emerging project with a strong commitment to growth and improvement. Your input and ideas are invaluable to me. I welcome your comments and advice with open arms, encouraging a culture of respect and kindness in our collaborative journey towards improvement.
+If you are using EasyFEA as part of your scientific research, please contribute to the scientific visibility of the project by citing it as follows.
+
+> Matthieu Noel. EasyFEA: a user-friendly Python library that simplifies finite element analysis. 2024, ⟨swh:1:dir:ffb0e56fe2ce8a344ed27df7baf8f5f1b58700b5;origin=https://github.com/matnoel/EasyFEA;visit=swh:1:snp:88527adbdb363d97ebaee858943a02d98fc5c23c;anchor=swh:1:rev:ee2a09258bfd7fd60886ad9334b0893f4989cf35⟩. ⟨hal-04571962⟩ 
+
+Bibtex:
+
+```
+@softwareversion{noel:hal-04571962v1,
+  TITLE = {{EasyFEA: a user-friendly Python library that simplifies finite element analysis}},
+  AUTHOR = {Noel, Matthieu},
+  URL = {https://hal.science/hal-04571962},
+  NOTE = {},
+  INSTITUTION = {{Universit{\'e} Gustave Eiffel}},
+  YEAR = {2024},
+  MONTH = Apr,
+  SWHID = {swh:1:dir:ffb0e56fe2ce8a344ed27df7baf8f5f1b58700b5;origin=https://github.com/matnoel/EasyFEA;visit=swh:1:snp:88527adbdb363d97ebaee858943a02d98fc5c23c;anchor=swh:1:rev:ee2a09258bfd7fd60886ad9334b0893f4989cf35},
+  REPOSITORY = {https://github.com/matnoel/EasyFEA},
+  LICENSE = {GNU General Public License v3.0 or later},
+  KEYWORDS = {Finite element analyses ; Computational Mechanics ; Numerical Simulation ; Phase field modeling of brittle fracture ; Linear elasticity ; Euler-Bernoulli beam ; DIC - Digital Image Correlation ; User friendly ; Object oriented programming ; Mesh Generation},
+  HAL_ID = {hal-04571962},
+  HAL_VERSION = {v1},
+}
+```
 
 # License
 
-EasyFEA is copyright (C) 2021-2024 M. Noel, and is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+
+EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/LICENSE.txt` & `EasyFEA-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EasyFEA-1.0.1/PKG-INFO` & `EasyFEA-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyFEA
-Version: 1.0.1
+Version: 1.0.2
 Summary: User-friendly Python library that simplifies finite element analysis.
 Author-email: Matthieu Noel <matthieu.noel7@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -688,29 +688,45 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+License-File: AUTHORS.md
+Requires-Dist: numpy
+Requires-Dist: gmsh>=4.12
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pyvista
+Requires-Dist: numba
+Requires-Dist: pandas
+Requires-Dist: imageio
+Requires-Dist: imageio[ffmpeg]
 Provides-Extra: fast
+Requires-Dist: pypardiso; extra == "fast"
+Requires-Dist: petsc; extra == "fast"
+Requires-Dist: petsc4py; extra == "fast"
 Provides-Extra: cv
-License-File: LICENSE.txt
+Requires-Dist: opencv-python; extra == "cv"
 
 # EasyFEA - Easy Finite Element Analysis
 
 ## Overview
 
 **EasyFEA** is a user-friendly Python library that simplifies finite element analysis. It is flexible and supports different types of simulation without requiring users to handle complex PDE formulations. The library currently supports four specific simulation types:
 
 1. **ElasticSimu** (static and dynamic): Examples in `/examples/Elastic`, `/examples/Dynamic` and `/examples/Contact`.
 2. **BeamSimu** (static Euler-Bernoulli): Examples in `/examples/Beam`.
 3. **ThermalSimu** (stationary and transient): Examples in `/examples/Thermal`.
 4. **PhaseFieldSimu:** (quasi-static phase field) Examples in `/examples/PhaseField`.
 
+All examples are available [here](https://github.com/matnoel/EasyFEA/tree/master/examples).
+
 For each simulation, users create a **mesh** and a **model**. Once the simulation has been set up, defining the boundary conditions, solving the problem and visualizing the results is straightforward.
 
 Numerous examples of mesh creation are available in the `examples/Meshes` folder.
 
 The simplest and quickest introduction is shown below and is available in `examples/HelloWorld.py`.
 
 ```python
@@ -753,16 +769,14 @@
 Display.Plot_BoundaryConditions(simu)
 Display.Plot_Result(simu, 'uy', plotMesh=True)
 Display.Plot_Result(simu, 'Svm', plotMesh=True, ncolors=11)
 
 Display.plt.show()
 ```
 
-All examples are available [here](https://github.com/matnoel/EasyFEA/tree/master/examples).
-
 ## Installation
 
 EasyFEA can be easily installed from [PyPI](https://pypi.org/project/EasyFEA/) using pip, compatible with Python versions 3.9 through 3.12:
 
 ```
 pip install EasyFEA
 ```
@@ -784,37 +798,57 @@
 
 ### Optional Dependencies
 
 EasyFEA includes a few optional dependencies for reducing resolution time or for performing DIC:
 
 + [`pypardiso`](https://pypi.org/project/pypardiso/) (Python > 3.8 & Intel oneAPI)  - Library for solving large systems of sparse linear equations.
 + [`petsc`](https://pypi.org/project/petsc/) and [`petsc4py`](https://pypi.org/project/petsc4py/) - Python bindings for PETSc.
-+ [opencv-python](https://pypi.org/project/opencv-python/) - Computer Vision package.
++ [`opencv-python`](https://pypi.org/project/opencv-python/) - Computer Vision package.
 
 # Naming conventions
 
 **EasyFEA** uses Object-Oriented Programming ([OOP](https://en.wikipedia.org/wiki/Object-oriented_programming)) with the following naming conventions:
 + `PascalCasing` for classes
 + `camelCasing` for properties
 + `Snake_Casing` or `Snake_casing` for functions/methods
 
 In this library, objects can contain both **public** and **private** properties or functions.
 
 **Private** parameters or functions are designated by a double underscore, such as `__privateParam`. In addition, parameters or functions beginning with an underscore, such as `_My_Function` are accessible to advanced users, but should be used with caution.
 
 # Contributing
 
-Contributors are welcome! To contribute please use the following commands.
+**EasyFEA** is an emerging project with a strong commitment to growth and improvement. Your input and ideas are invaluable to me. I welcome your comments and advice with open arms, encouraging a culture of respect and kindness in our collaborative journey towards improvement.
 
-```
-git clone https://github.com/matnoel/EasyFEA.git
-cd EasyFEA
-python -m pip install -e .
-```
+To learn more about contributing to EasyFEA, please consult the [Contributing Guide](https://github.com/matnoel/EasyFEA/blob/main/CONTRIBUTING.md).
 
-To develop a new feature, start by creating a new branch in the project using the command `git branch my_new_feature`. After implementing and testing your modifications (refer to EasyFEA/tests), proceed to create a pull request to merge your changes.
+# Citing EasyFEA
 
-**EasyFEA** is an emerging project with a strong commitment to growth and improvement. Your input and ideas are invaluable to me. I welcome your comments and advice with open arms, encouraging a culture of respect and kindness in our collaborative journey towards improvement.
+If you are using EasyFEA as part of your scientific research, please contribute to the scientific visibility of the project by citing it as follows.
+
+> Matthieu Noel. EasyFEA: a user-friendly Python library that simplifies finite element analysis. 2024, ⟨swh:1:dir:ffb0e56fe2ce8a344ed27df7baf8f5f1b58700b5;origin=https://github.com/matnoel/EasyFEA;visit=swh:1:snp:88527adbdb363d97ebaee858943a02d98fc5c23c;anchor=swh:1:rev:ee2a09258bfd7fd60886ad9334b0893f4989cf35⟩. ⟨hal-04571962⟩ 
+
+Bibtex:
+
+```
+@softwareversion{noel:hal-04571962v1,
+  TITLE = {{EasyFEA: a user-friendly Python library that simplifies finite element analysis}},
+  AUTHOR = {Noel, Matthieu},
+  URL = {https://hal.science/hal-04571962},
+  NOTE = {},
+  INSTITUTION = {{Universit{\'e} Gustave Eiffel}},
+  YEAR = {2024},
+  MONTH = Apr,
+  SWHID = {swh:1:dir:ffb0e56fe2ce8a344ed27df7baf8f5f1b58700b5;origin=https://github.com/matnoel/EasyFEA;visit=swh:1:snp:88527adbdb363d97ebaee858943a02d98fc5c23c;anchor=swh:1:rev:ee2a09258bfd7fd60886ad9334b0893f4989cf35},
+  REPOSITORY = {https://github.com/matnoel/EasyFEA},
+  LICENSE = {GNU General Public License v3.0 or later},
+  KEYWORDS = {Finite element analyses ; Computational Mechanics ; Numerical Simulation ; Phase field modeling of brittle fracture ; Linear elasticity ; Euler-Bernoulli beam ; DIC - Digital Image Correlation ; User friendly ; Object oriented programming ; Mesh Generation},
+  HAL_ID = {hal-04571962},
+  HAL_VERSION = {v1},
+}
+```
 
 # License
 
-EasyFEA is copyright (C) 2021-2024 M. Noel, and is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+
+EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/README.md` & `EasyFEA-1.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 **EasyFEA** is a user-friendly Python library that simplifies finite element analysis. It is flexible and supports different types of simulation without requiring users to handle complex PDE formulations. The library currently supports four specific simulation types:
 
 1. **ElasticSimu** (static and dynamic): Examples in `/examples/Elastic`, `/examples/Dynamic` and `/examples/Contact`.
 2. **BeamSimu** (static Euler-Bernoulli): Examples in `/examples/Beam`.
 3. **ThermalSimu** (stationary and transient): Examples in `/examples/Thermal`.
 4. **PhaseFieldSimu:** (quasi-static phase field) Examples in `/examples/PhaseField`.
 
+All examples are available [here](https://github.com/matnoel/EasyFEA/tree/master/examples).
+
 For each simulation, users create a **mesh** and a **model**. Once the simulation has been set up, defining the boundary conditions, solving the problem and visualizing the results is straightforward.
 
 Numerous examples of mesh creation are available in the `examples/Meshes` folder.
 
 The simplest and quickest introduction is shown below and is available in `examples/HelloWorld.py`.
 
 ```python
@@ -55,16 +57,14 @@
 Display.Plot_BoundaryConditions(simu)
 Display.Plot_Result(simu, 'uy', plotMesh=True)
 Display.Plot_Result(simu, 'Svm', plotMesh=True, ncolors=11)
 
 Display.plt.show()
 ```
 
-All examples are available [here](https://github.com/matnoel/EasyFEA/tree/master/examples).
-
 ## Installation
 
 EasyFEA can be easily installed from [PyPI](https://pypi.org/project/EasyFEA/) using pip, compatible with Python versions 3.9 through 3.12:
 
 ```
 pip install EasyFEA
 ```
@@ -86,37 +86,57 @@
 
 ### Optional Dependencies
 
 EasyFEA includes a few optional dependencies for reducing resolution time or for performing DIC:
 
 + [`pypardiso`](https://pypi.org/project/pypardiso/) (Python > 3.8 & Intel oneAPI)  - Library for solving large systems of sparse linear equations.
 + [`petsc`](https://pypi.org/project/petsc/) and [`petsc4py`](https://pypi.org/project/petsc4py/) - Python bindings for PETSc.
-+ [opencv-python](https://pypi.org/project/opencv-python/) - Computer Vision package.
++ [`opencv-python`](https://pypi.org/project/opencv-python/) - Computer Vision package.
 
 # Naming conventions
 
 **EasyFEA** uses Object-Oriented Programming ([OOP](https://en.wikipedia.org/wiki/Object-oriented_programming)) with the following naming conventions:
 + `PascalCasing` for classes
 + `camelCasing` for properties
 + `Snake_Casing` or `Snake_casing` for functions/methods
 
 In this library, objects can contain both **public** and **private** properties or functions.
 
 **Private** parameters or functions are designated by a double underscore, such as `__privateParam`. In addition, parameters or functions beginning with an underscore, such as `_My_Function` are accessible to advanced users, but should be used with caution.
 
 # Contributing
 
-Contributors are welcome! To contribute please use the following commands.
+**EasyFEA** is an emerging project with a strong commitment to growth and improvement. Your input and ideas are invaluable to me. I welcome your comments and advice with open arms, encouraging a culture of respect and kindness in our collaborative journey towards improvement.
 
-```
-git clone https://github.com/matnoel/EasyFEA.git
-cd EasyFEA
-python -m pip install -e .
-```
+To learn more about contributing to EasyFEA, please consult the [Contributing Guide](https://github.com/matnoel/EasyFEA/blob/main/CONTRIBUTING.md).
 
-To develop a new feature, start by creating a new branch in the project using the command `git branch my_new_feature`. After implementing and testing your modifications (refer to EasyFEA/tests), proceed to create a pull request to merge your changes.
+# Citing EasyFEA
 
-**EasyFEA** is an emerging project with a strong commitment to growth and improvement. Your input and ideas are invaluable to me. I welcome your comments and advice with open arms, encouraging a culture of respect and kindness in our collaborative journey towards improvement.
+If you are using EasyFEA as part of your scientific research, please contribute to the scientific visibility of the project by citing it as follows.
+
+> Matthieu Noel. EasyFEA: a user-friendly Python library that simplifies finite element analysis. 2024, ⟨swh:1:dir:ffb0e56fe2ce8a344ed27df7baf8f5f1b58700b5;origin=https://github.com/matnoel/EasyFEA;visit=swh:1:snp:88527adbdb363d97ebaee858943a02d98fc5c23c;anchor=swh:1:rev:ee2a09258bfd7fd60886ad9334b0893f4989cf35⟩. ⟨hal-04571962⟩ 
+
+Bibtex:
+
+```
+@softwareversion{noel:hal-04571962v1,
+  TITLE = {{EasyFEA: a user-friendly Python library that simplifies finite element analysis}},
+  AUTHOR = {Noel, Matthieu},
+  URL = {https://hal.science/hal-04571962},
+  NOTE = {},
+  INSTITUTION = {{Universit{\'e} Gustave Eiffel}},
+  YEAR = {2024},
+  MONTH = Apr,
+  SWHID = {swh:1:dir:ffb0e56fe2ce8a344ed27df7baf8f5f1b58700b5;origin=https://github.com/matnoel/EasyFEA;visit=swh:1:snp:88527adbdb363d97ebaee858943a02d98fc5c23c;anchor=swh:1:rev:ee2a09258bfd7fd60886ad9334b0893f4989cf35},
+  REPOSITORY = {https://github.com/matnoel/EasyFEA},
+  LICENSE = {GNU General Public License v3.0 or later},
+  KEYWORDS = {Finite element analyses ; Computational Mechanics ; Numerical Simulation ; Phase field modeling of brittle fracture ; Linear elasticity ; Euler-Bernoulli beam ; DIC - Digital Image Correlation ; User friendly ; Object oriented programming ; Mesh Generation},
+  HAL_ID = {hal-04571962},
+  HAL_VERSION = {v1},
+}
+```
 
 # License
 
-EasyFEA is copyright (C) 2021-2024 M. Noel, and is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
+Copyright (C) 2021-2024 Université Gustave Eiffel. All rights reserved.
+
+EasyFEA is distributed under the terms of the GNU General Public License, Version 3 or later, see LICENSE.txt and CREDITS.txt for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `EasyFEA-1.0.1/pyproject.toml` & `EasyFEA-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EasyFEA"
-version = "1.0.1"
+version = "1.0.2"
 description = "User-friendly Python library that simplifies finite element analysis."
 authors = [
     {name = "Matthieu Noel", email = "matthieu.noel7@gmail.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["finite-element-analysis", "phase-field", "python", "easy", "fem"]
 license = {file = "LICENSE.txt"}
-classifiers = [    
+classifiers = [
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.9",
```

