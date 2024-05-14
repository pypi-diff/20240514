# Comparing `tmp/OpenSRANE-0.0.4.1.tar.gz` & `tmp/opensrane-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenSRANE-0.0.4.1.tar", last modified: Thu Mar 21 10:37:24 2024, max compression
+gzip compressed data, was "opensrane-0.0.5.tar", last modified: Tue May 14 15:51:27 2024, max compression
```

## Comparing `OpenSRANE-0.0.4.1.tar` & `opensrane-0.0.5.tar`

### file list

```diff
@@ -1,142 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.204940 OpenSRANE-0.0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.204940 OpenSRANE-0.0.4.1/OpenSRANE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-21 10:37:24.000000 OpenSRANE-0.0.4.1/OpenSRANE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-21 10:37:24.000000 OpenSRANE-0.0.4.1/OpenSRANE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:37:24.000000 OpenSRANE-0.0.4.1/OpenSRANE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-21 10:37:24.000000 OpenSRANE-0.0.4.1/OpenSRANE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-21 10:37:24.000000 OpenSRANE-0.0.4.1/OpenSRANE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-21 10:37:24.204940 OpenSRANE-0.0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.180940 OpenSRANE-0.0.4.1/opensrane/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.184940 OpenSRANE-0.0.4.1/opensrane/All/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/All/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/All/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/All/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.184940 OpenSRANE-0.0.4.1/opensrane/Analyze/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/ScenarioAnalyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/_DispSprd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/_Frag_OutFlow.py
--rw-r--r--   0 runner    (1001) docker     (127)    17005 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/_NodesGroupsVulnerability.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/_PhysicalAssign.py
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/_PhysicalEffects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/_Prob_OutFlow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/_Sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/_ZeroLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Analyze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.184940 OpenSRANE-0.0.4.1/opensrane/Connectors/
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Connectors/DS_LOC.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Connectors/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Connectors/Out_Physic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Connectors/Pb_LOC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.184940 OpenSRANE-0.0.4.1/opensrane/DateAndTime/
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DateAndTime/DateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DateAndTime/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DateAndTime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.188940 OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/
--rw-r--r--   0 runner    (1001) docker     (127)    21663 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/BritterMcQuaid.py
--rw-r--r--   0 runner    (1001) docker     (127)    29223 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/GasGaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/LiquidSpread.py
--rw-r--r--   0 runner    (1001) docker     (127)    38856 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/LqdSprdGaussianGasDisp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.188940 OpenSRANE-0.0.4.1/opensrane/Fragilities/
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Fragilities/Fragility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Fragilities/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Fragilities/Probit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Fragilities/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Fragilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.188940 OpenSRANE-0.0.4.1/opensrane/Hazard/
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Hazard/ConstIM.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Hazard/Earthquake.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Hazard/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Hazard/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Hazard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.192940 OpenSRANE-0.0.4.1/opensrane/Misc/
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Misc/MiscFuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Misc/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Misc/WarningRecorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Misc/_NewClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.192940 OpenSRANE-0.0.4.1/opensrane/NodesGroups/
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/NodesGroups/Nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/NodesGroups/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/NodesGroups/RectangNodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/NodesGroups/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/NodesGroups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.192940 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/GasUnitHole.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/Liquid10min.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/NoOutFlow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/SimultaniousGas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/SimultaniousLiquid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/TankHole.py
--rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/TankHoleDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/TankHoleFixStep.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/TankHoleInitRate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/OutFlowModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.196940 OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/Rapid_N_Poolfire_point_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/SAFE.py
--rw-r--r--   0 runner    (1001) docker     (127)    21854 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/Simple_fire_point_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/VCE_TNT.py
--rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/fire_point_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.196940 OpenSRANE-0.0.4.1/opensrane/PlantUnits/
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PlantUnits/ONGStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PlantUnits/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PlantUnits/SphericalTank.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PlantUnits/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PlantUnits/_Position.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PlantUnits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.196940 OpenSRANE-0.0.4.1/opensrane/Plot/
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Plot/Matplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Plot/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    51234 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Plot/Plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.200940 OpenSRANE-0.0.4.1/opensrane/PostProcess/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PostProcess/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16740 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PostProcess/ObjsRecorderPP.py
--rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PostProcess/PlotPP.py
--rw-r--r--   0 runner    (1001) docker     (127)    20168 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PostProcess/RecorderPP.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/PostProcess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.200940 OpenSRANE-0.0.4.1/opensrane/Recorders/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Recorders/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Recorders/Objs_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Recorders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19280 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Recorders/recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.200940 OpenSRANE-0.0.4.1/opensrane/Safety/
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Safety/Dike.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Safety/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Safety/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Safety/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.200940 OpenSRANE-0.0.4.1/opensrane/Sites/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Sites/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Sites/Site.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Sites/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.200940 OpenSRANE-0.0.4.1/opensrane/Substance/
--rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Substance/DataBank.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Substance/Material.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Substance/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Substance/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/Substance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.200940 OpenSRANE-0.0.4.1/opensrane/WindData/
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/WindData/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/WindData/WindRose.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/WindData/_GlobalParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/WindData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:37:24.204940 OpenSRANE-0.0.4.1/opensrane/_New_module/
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/_New_module/New_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/_New_module/ObjManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/_New_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/opensrane/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:37:24.204940 OpenSRANE-0.0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-21 10:37:15.000000 OpenSRANE-0.0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.888543 opensrane-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.888543 opensrane-0.0.5/OpenSRANE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-14 15:51:27.000000 opensrane-0.0.5/OpenSRANE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-14 15:51:27.000000 opensrane-0.0.5/OpenSRANE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:51:27.000000 opensrane-0.0.5/OpenSRANE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 15:51:27.000000 opensrane-0.0.5/OpenSRANE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 15:51:27.000000 opensrane-0.0.5/OpenSRANE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-14 15:51:27.888543 opensrane-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 15:51:19.000000 opensrane-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.868542 opensrane-0.0.5/opensrane/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.872542 opensrane-0.0.5/opensrane/All/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/All/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/All/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/All/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.872542 opensrane-0.0.5/opensrane/Analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/ScenarioAnalyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/_DispSprd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/_Frag_OutFlow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17005 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/_NodesGroupsVulnerability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/_PhysicalAssign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/_PhysicalEffects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/_Prob_OutFlow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/_Sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/_ZeroLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Analyze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.872542 opensrane-0.0.5/opensrane/Connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Connectors/DS_LOC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Connectors/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Connectors/Out_Physic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Connectors/Pb_LOC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.872542 opensrane-0.0.5/opensrane/DateAndTime/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DateAndTime/DateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DateAndTime/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DateAndTime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.876542 opensrane-0.0.5/opensrane/DispersionSpreadModels/
+-rw-r--r--   0 runner    (1001) docker     (127)    21663 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DispersionSpreadModels/BritterMcQuaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29223 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DispersionSpreadModels/GasGaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DispersionSpreadModels/LiquidSpread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38856 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DispersionSpreadModels/LqdSprdGaussianGasDisp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DispersionSpreadModels/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DispersionSpreadModels/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/DispersionSpreadModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.876542 opensrane-0.0.5/opensrane/Fragilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Fragilities/Fragility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Fragilities/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Fragilities/Probit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Fragilities/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Fragilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.876542 opensrane-0.0.5/opensrane/Hazard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Hazard/ConstIM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Hazard/Earthquake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Hazard/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Hazard/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Hazard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.880543 opensrane-0.0.5/opensrane/Misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Misc/MiscFuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Misc/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Misc/WarningRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Misc/_NewClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.880543 opensrane-0.0.5/opensrane/NodesGroups/
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/NodesGroups/Nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/NodesGroups/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/NodesGroups/RectangNodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/NodesGroups/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/NodesGroups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.880543 opensrane-0.0.5/opensrane/OutFlowModel/
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/GasUnitHole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/Liquid10min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/NoOutFlow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/SimultaniousGas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/SimultaniousLiquid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/TankHole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/TankHoleDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/TankHoleFixStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/TankHoleInitRate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/OutFlowModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.884543 opensrane-0.0.5/opensrane/PhysicalEffect/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PhysicalEffect/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PhysicalEffect/Rapid_N_Poolfire_point_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PhysicalEffect/SAFE.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21854 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PhysicalEffect/Simple_fire_point_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PhysicalEffect/VCE_TNT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PhysicalEffect/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PhysicalEffect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PhysicalEffect/fire_point_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.884543 opensrane-0.0.5/opensrane/PlantUnits/
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PlantUnits/ONGStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PlantUnits/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PlantUnits/SphericalTank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PlantUnits/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PlantUnits/_Position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PlantUnits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.884543 opensrane-0.0.5/opensrane/Plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Plot/Matplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Plot/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51234 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Plot/Plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.884543 opensrane-0.0.5/opensrane/PostProcess/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PostProcess/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31839 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PostProcess/ObjsRecorderPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39303 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PostProcess/RecorderPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/PostProcess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.884543 opensrane-0.0.5/opensrane/Recorders/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Recorders/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24673 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Recorders/Objs_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Recorders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19390 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Recorders/recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.884543 opensrane-0.0.5/opensrane/Safety/
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Safety/Dike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Safety/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Safety/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Safety/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.888543 opensrane-0.0.5/opensrane/Sites/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Sites/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Sites/Site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Sites/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.888543 opensrane-0.0.5/opensrane/Substance/
+-rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Substance/DataBank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Substance/Material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Substance/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Substance/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/Substance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.888543 opensrane-0.0.5/opensrane/WindData/
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/WindData/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/WindData/WindRose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/WindData/_GlobalParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/WindData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:51:27.888543 opensrane-0.0.5/opensrane/_New_module/
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/_New_module/New_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/_New_module/ObjManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/_New_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-14 15:51:19.000000 opensrane-0.0.5/opensrane/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:51:27.888543 opensrane-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-14 15:51:19.000000 opensrane-0.0.5/setup.py
```

### Comparing `OpenSRANE-0.0.4.1/OpenSRANE.egg-info/PKG-INFO` & `opensrane-0.0.5/OpenSRANE.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: OpenSRANE
-Version: 0.0.4.1
-Summary: Open Software for Risk Assessment of Natech Events
+Version: 0.0.5
+Summary: Open System for Risk Assessment of Natech Events
 Home-page: https://github.com/OpenSRANE/OpenSRANE
 Author: Bijan Sayyafzadeh
 Author-email: <OpenSRANE@Gmail.com>
 Keywords: python,NaTech,Modeling,Risk
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,12 +18,12 @@
 Requires-Dist: pandas
 Requires-Dist: ipywidgets
 Requires-Dist: nbformat
 Requires-Dist: ipykernel
 
 ## OpenSRANE
 
-### Open Software for Risk Assessment of Natech Events
+### Open System for Risk Assessment of Natech Events
 
 Documentation: https://github.com/OpenSRANE/OpenSRANE_Documentation
```

### Comparing `OpenSRANE-0.0.4.1/OpenSRANE.egg-info/SOURCES.txt` & `opensrane-0.0.5/OpenSRANE.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 opensrane/PlantUnits/__init__.py
 opensrane/Plot/Matplot.py
 opensrane/Plot/ObjManager.py
 opensrane/Plot/Plotly.py
 opensrane/Plot/__init__.py
 opensrane/PostProcess/ObjManager.py
 opensrane/PostProcess/ObjsRecorderPP.py
-opensrane/PostProcess/PlotPP.py
 opensrane/PostProcess/RecorderPP.py
 opensrane/PostProcess/__init__.py
 opensrane/Recorders/ObjManager.py
 opensrane/Recorders/Objs_recorder.py
 opensrane/Recorders/__init__.py
 opensrane/Recorders/recorder.py
 opensrane/Safety/Dike.py
```

### Comparing `OpenSRANE-0.0.4.1/PKG-INFO` & `opensrane-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: OpenSRANE
-Version: 0.0.4.1
-Summary: Open Software for Risk Assessment of Natech Events
+Version: 0.0.5
+Summary: Open System for Risk Assessment of Natech Events
 Home-page: https://github.com/OpenSRANE/OpenSRANE
 Author: Bijan Sayyafzadeh
 Author-email: <OpenSRANE@Gmail.com>
 Keywords: python,NaTech,Modeling,Risk
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,12 +18,12 @@
 Requires-Dist: pandas
 Requires-Dist: ipywidgets
 Requires-Dist: nbformat
 Requires-Dist: ipykernel
 
 ## OpenSRANE
 
-### Open Software for Risk Assessment of Natech Events
+### Open System for Risk Assessment of Natech Events
 
 Documentation: https://github.com/OpenSRANE/OpenSRANE_Documentation
```

### Comparing `OpenSRANE-0.0.4.1/opensrane/All/ObjManager.py` & `opensrane-0.0.5/opensrane/All/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/All/__init__.py` & `opensrane-0.0.5/opensrane/All/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/All/empty.py` & `opensrane-0.0.5/opensrane/All/empty.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/ObjManager.py` & `opensrane-0.0.5/opensrane/Analyze/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/ScenarioAnalyze.py` & `opensrane-0.0.5/opensrane/Analyze/ScenarioAnalyze.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,20 +43,23 @@
 from tqdm import tqdm as _tqdm
 import multiprocessing as _mp
 
 class ScenarioAnalyze():
     
     anydamage=None                      #A parameter that shows does the analysis encounter with any damage or not
 
-    def UniAnalyze(SavetoFile=True,fileindex=0):
+    def UniAnalyze(SavetoFile=True,fileindex=0, MergeSavedFiles=False):
         
         '''
         SavetoFile: For recorder objects it is emphasize that record data to a file or not (For unianalysis it is yes but for multiple analysis it should be no till after finishing the analysis in one time data be stored) (For objs recorder it will be save and it doesn't have any effect on them)
 
-        fileindex: is an integer that will be add to the end of the filename to save in seperate file (For unianalysis it should be 0)
+        fileindex: is an integer that will be add to the end of the filename to save recorded scenarios in seperate file
+        
+        MergeSavedFiles: If set this option into True, When analysis finished all files will be merge into one file and for huge files it take so_
+                         much memory and time!
 
         '''
         
         #Clear previous analysis results
         _opr.Misc.wipeAnalysis()             
         
         #------------------------ First Part: Read Defined Objects -------------------------------------------#
@@ -116,93 +119,93 @@
             ScenarioAnalyze.anydamage=False
         #---------------------------- LastPart : Record Scenario -----------------------------------------------------------------#
         #Do the recordings for all Objs_recorder objects
         [obj.Record() for obj in _opr.Recorders.ObjManager.Objlst]
         
         #Save the recorded data just for recorder objects
         if SavetoFile==True:
-            [obj.SaveToFile(fileindex) for obj in _opr.Recorders.ObjManager.Objlst]
-            [obj._MergeAndClear() for obj in _opr.Recorders.ObjManager.Objlst]
+            [obj.SaveToFile(fileindex) for obj in _opr.Recorders.ObjManager.Objlst] #Save all Objects of subpackages that are recorded in recorders.
+            [obj.OtherSaveOnce() for obj in _opr.Recorders.ObjManager.Objlst] #Save Other subpackages that aren't defined for objs_recorder (It doesn't have any influence of affect for recordes and is only for objs_recorder.            
+            if MergeSavedFiles==True: [obj._MergeAndClear() for obj in _opr.Recorders.ObjManager.Objlst]
         
         
         
         
-    def MultiAnalysis(AnalysisNumber=100,isParallel=False,fileindex=0):
+    def MultiAnalysis(AnalysisNumber=100,isParallel=False,fileindex=0, MergeSavedFiles=None):
         
         '''
         This function implement multiple scenario analysis and record results
         AnalysisNumber: Number of analysis that user intend to do by this function
         ResetRecorder: Does the function clear the recorder file and record scenarios from zero or add new analysed scenarios to the end of the current file
         
         fileindex: is an integer that will be add to the end of the filename to save in seperate file
+
         '''
         
         #Do the analysis
         for i in _tqdm(range(AnalysisNumber)):
             _opr.Analyze.ScenarioAnalyze.UniAnalyze(SavetoFile=False)  #Do a unit scenario analysis and do not save for recorder objects and after the analysis in next lines the data will be store in the file (For objs recorder it will be save and it doesn't have any effect on them)
             # FR=[obj.DamageLevel for obj in _opr.PlantUnits.ObjManager.Objlst]
             # FR=[obj.DamageLevel for obj in _opr.PlantUnits.ObjManager.Objlst]
             # print(FR) #to see the damage level of objects in the ith analyzed scenario
             
-        [obj.SaveToFile(fileindex) for obj in _opr.Recorders.ObjManager.Objlst] #Save the recorded data just for recorder objects   
+        [obj.SaveToFile(fileindex) for obj in _opr.Recorders.ObjManager.Objlst] #Save the recorded data just for recorder objects  
         
         if isParallel==False:
-            #Merge all created files and remove them and just put the filnal file
-            [obj._MergeAndClear() for obj in _opr.Recorders.ObjManager.Objlst] 
+            #Run Merge all created files and remove them and just put the final file for objects that user set the mergesavedfiles equal to True
+            [obj._MergeAndClear() for obj in _opr.Recorders.ObjManager.Objlst]
+            
+            #Save Other subpackages that aren't defined for objs_recorder (It doesn't have any influence of affect for recordes and is only for objs_recorder.
+            [obj.OtherSaveOnce() for obj in _opr.Recorders.ObjManager.Objlst] 
 
-    def MultiParallel(AnalysisNumber=100, NumberOfProcessors=3, RecorderSaveStep=5000):
+    def MultiParallel(AnalysisNumber=100, NumberOfProcessors=3, RecordersSaveStep=5000, MergeSavedFiles=None):
         
         '''
         
         REMEMBER: The only way to use this command is to call it inside "if __name__='__main__': " 
         
-        RecorderSaveStep: if user didn't define Objs_recorder then the RecorderSaveStep will be use as save step But_
-                          if Objs_recorder were define its save step will be consider as savestep
+        RecordersSaveStep: RecordersSaveStep will be use as save step.
+
         '''
 
         #For Recorder objects if append is false the append should be True 
         # and file should be remove here manually to avoid multipe file removing
         for obj in _opr.Recorders.ObjManager.Objlst:
             if obj.__class__.__name__=='recorder':
                 if obj.fileAppend==False:
                     obj.fileAppend==True
                     obj._Deletefile()
 
             if obj.__class__.__name__=='Objs_recorder':
                 if obj.fileAppend==False:
                     obj.fileAppend==True
-                    obj._ResetRecorder()            
+                    obj._ResetRecorder()   
 
-
-        #Set SaveStep
-        SaveStep=None
-        for obj in _opr.Recorders.ObjManager.Objlst:
-            if obj.__class__.__name__=='Objs_recorder':
-                SaveStep=int(obj.SaveStep)
-                break
         
         #Check Number of CPUs        
         NOP=_mp.cpu_count()
         
         if NumberOfProcessors<NOP:
             NOP=NumberOfProcessors
         
         #Set the save step:
-        if SaveStep==None: SaveStep=int(RecorderSaveStep)
+        SaveStep=int(RecordersSaveStep)
 
         #Set Number of Analysis for each CPU
         AnalyzeList=AnalysisNumber/SaveStep if AnalysisNumber%SaveStep==0 else int(AnalysisNumber/SaveStep)+1
         AnalyzeList=[SaveStep for i in range(int(AnalyzeList))]
         
         #Set number of CPUs    
         pool = _mp.Pool(NOP)
         
         #Set Analyze
         print('Analysis Number of each core: ',AnalyzeList)
-        pool.starmap(_opr.Analyze.ScenarioAnalyze.MultiAnalysis, [(AnalyseNumber,True,fileindex) for fileindex,AnalyseNumber in enumerate(AnalyzeList)])
+        pool.starmap(_opr.Analyze.ScenarioAnalyze.MultiAnalysis, [(AnalyseNumber,True,fileindex+1) for fileindex,AnalyseNumber in enumerate(AnalyzeList)])
         
         pool.close()
 
-        #Merge all created files and remove them and just put the filnal file
-        [obj._MergeAndClear() for obj in _opr.Recorders.ObjManager.Objlst] 
-
+        #Run Merge all created files and remove them and just put the final file for objects that user set the mergesavedfiles equal to True
+        [obj._MergeAndClear() for obj in _opr.Recorders.ObjManager.Objlst]
+        
+        #Save Other subpackages that aren't defined for objs_recorder (It doesn't have any influence of affect for recordes and is only for objs_recorder.
+        [obj.OtherSaveOnce() for obj in _opr.Recorders.ObjManager.Objlst]
```

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/_DispSprd.py` & `opensrane-0.0.5/opensrane/Analyze/_DispSprd.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/_Frag_OutFlow.py` & `opensrane-0.0.5/opensrane/Analyze/_Frag_OutFlow.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/_NodesGroupsVulnerability.py` & `opensrane-0.0.5/opensrane/Analyze/_NodesGroupsVulnerability.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/_PhysicalAssign.py` & `opensrane-0.0.5/opensrane/Analyze/_PhysicalAssign.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/_PhysicalEffects.py` & `opensrane-0.0.5/opensrane/Analyze/_PhysicalEffects.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/_Prob_OutFlow.py` & `opensrane-0.0.5/opensrane/Analyze/_Prob_OutFlow.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/_Sampling.py` & `opensrane-0.0.5/opensrane/Analyze/_Sampling.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/_ZeroLevel.py` & `opensrane-0.0.5/opensrane/Analyze/_ZeroLevel.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Analyze/__init__.py` & `opensrane-0.0.5/opensrane/Analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Connectors/DS_LOC.py` & `opensrane-0.0.5/opensrane/Connectors/DS_LOC.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Connectors/ObjManager.py` & `opensrane-0.0.5/opensrane/Connectors/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Connectors/Out_Physic.py` & `opensrane-0.0.5/opensrane/Connectors/Out_Physic.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Connectors/Pb_LOC.py` & `opensrane-0.0.5/opensrane/Connectors/Pb_LOC.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Connectors/__init__.py` & `opensrane-0.0.5/opensrane/Connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DateAndTime/DateTime.py` & `opensrane-0.0.5/opensrane/DateAndTime/DateTime.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DateAndTime/ObjManager.py` & `opensrane-0.0.5/opensrane/DateAndTime/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DateAndTime/__init__.py` & `opensrane-0.0.5/opensrane/DateAndTime/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/BritterMcQuaid.py` & `opensrane-0.0.5/opensrane/DispersionSpreadModels/BritterMcQuaid.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/GasGaussian.py` & `opensrane-0.0.5/opensrane/DispersionSpreadModels/GasGaussian.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/LiquidSpread.py` & `opensrane-0.0.5/opensrane/DispersionSpreadModels/LiquidSpread.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/LqdSprdGaussianGasDisp.py` & `opensrane-0.0.5/opensrane/DispersionSpreadModels/LqdSprdGaussianGasDisp.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/ObjManager.py` & `opensrane-0.0.5/opensrane/DispersionSpreadModels/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/DispersionSpreadModels/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/DispersionSpreadModels/__init__.py` & `opensrane-0.0.5/opensrane/DispersionSpreadModels/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Fragilities/Fragility.py` & `opensrane-0.0.5/opensrane/Fragilities/Fragility.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Fragilities/ObjManager.py` & `opensrane-0.0.5/opensrane/Fragilities/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Fragilities/Probit.py` & `opensrane-0.0.5/opensrane/Fragilities/Probit.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Fragilities/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/Fragilities/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Fragilities/__init__.py` & `opensrane-0.0.5/opensrane/Fragilities/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Hazard/ConstIM.py` & `opensrane-0.0.5/opensrane/Hazard/ConstIM.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Hazard/Earthquake.py` & `opensrane-0.0.5/opensrane/Hazard/Earthquake.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Hazard/ObjManager.py` & `opensrane-0.0.5/opensrane/Hazard/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Hazard/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/Hazard/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Hazard/__init__.py` & `opensrane-0.0.5/opensrane/Hazard/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Misc/MiscFuncs.py` & `opensrane-0.0.5/opensrane/Misc/MiscFuncs.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Misc/ObjManager.py` & `opensrane-0.0.5/opensrane/Misc/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Misc/WarningRecorder.py` & `opensrane-0.0.5/opensrane/Misc/WarningRecorder.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Misc/_NewClass.py` & `opensrane-0.0.5/opensrane/Misc/_NewClass.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Misc/__init__.py` & `opensrane-0.0.5/opensrane/Misc/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/NodesGroups/Nodes.py` & `opensrane-0.0.5/opensrane/NodesGroups/Nodes.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/NodesGroups/ObjManager.py` & `opensrane-0.0.5/opensrane/NodesGroups/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/NodesGroups/RectangNodes.py` & `opensrane-0.0.5/opensrane/NodesGroups/RectangNodes.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/NodesGroups/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/NodesGroups/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/NodesGroups/__init__.py` & `opensrane-0.0.5/opensrane/NodesGroups/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/GasUnitHole.py` & `opensrane-0.0.5/opensrane/OutFlowModel/GasUnitHole.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,21 @@
 
         #Check if P0=0 or T0=0
         if  P0==0 or T0==0:
             warning(f'Pressure or Temprature for Unit with tag={UnitObject.tag} entered equal Zero and it cause a devision By Zero Error '+
                   f'So the code do not calculate any Gas Outflow (GasUnitHole Model) for this Plant Unit')
             return -1
         
+        #Check P0 and Pa
+        if  P0<=Pa:
+            warning(f'Pressure of Unit with tag={UnitObject.tag} is equal to {P0} and is equal or less than the ambient Pressure {Pa}! '+
+                  f'So the code do not calculate any Gas Outflow (GasUnitHole Model) for this Plant Unit')
+            return -1      
+            
+        
         Gamma=SubstanceObject.Specific_Heat_Ratio
         #Check if Gamma has not been assign to the material
         if Gamma==None:
             warning(f'Unit with tag={UnitObject.tag} With materialTag {SubstanceObject.tag} Has no Gamma (specific heat ratio) for its material'+
                   f'So the code do not calculate any Gas Outflow (GasUnitHole Model) for this Plant Unit')
             return -1
```

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/Liquid10min.py` & `opensrane-0.0.5/opensrane/OutFlowModel/Liquid10min.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/NoOutFlow.py` & `opensrane-0.0.5/opensrane/OutFlowModel/NoOutFlow.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/ObjManager.py` & `opensrane-0.0.5/opensrane/OutFlowModel/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/SimultaniousGas.py` & `opensrane-0.0.5/opensrane/OutFlowModel/SimultaniousGas.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/SimultaniousLiquid.py` & `opensrane-0.0.5/opensrane/OutFlowModel/SimultaniousLiquid.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/TankHole.py` & `opensrane-0.0.5/opensrane/OutFlowModel/TankHole.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/TankHoleDuration.py` & `opensrane-0.0.5/opensrane/OutFlowModel/TankHoleDuration.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/TankHoleFixStep.py` & `opensrane-0.0.5/opensrane/OutFlowModel/TankHoleFixStep.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/TankHoleInitRate.py` & `opensrane-0.0.5/opensrane/OutFlowModel/TankHoleInitRate.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/OutFlowModel/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/OutFlowModel/__init__.py` & `opensrane-0.0.5/opensrane/OutFlowModel/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/ObjManager.py` & `opensrane-0.0.5/opensrane/PhysicalEffect/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/Rapid_N_Poolfire_point_source.py` & `opensrane-0.0.5/opensrane/PhysicalEffect/Rapid_N_Poolfire_point_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,14 @@
         PoolRadius=UnitObject.DispersionSpreadModelObject.LiquidRadious
         PoolCenter=UnitObject.DispersionSpreadModelObject.LiquidCenter
         if PoolRadius==None or PoolCenter==None:
             warning(f'(Rapid-N PoolFire_Point_Source) for Plant unit {UnitObject.tag} because of pool radius or pool center is None so pool fire does not exist and no calculations has done!')
             return None
         Xcp,Ycp=PoolCenter[-1]
         Apool=PoolRadius[-1]**2*_math.pi
-        print('Apool=',Apool)
         
         SiteObject=_opr.Sites.ObjManager[UnitObject.SiteTag]
         if SiteObject==None:
             warning(f'(Rapid-N PoolFire_Point_Source) for Plant unit {UnitObject.tag} because of No site tag has been defined for metioned Plant unit Object')
             return None 
             
         Ta=SiteObject.Temperature #Site Temperature or air Temperature
```

### Comparing `OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/SAFE.py` & `opensrane-0.0.5/opensrane/PhysicalEffect/SAFE.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/Simple_fire_point_source.py` & `opensrane-0.0.5/opensrane/PhysicalEffect/Simple_fire_point_source.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/VCE_TNT.py` & `opensrane-0.0.5/opensrane/PhysicalEffect/VCE_TNT.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/PhysicalEffect/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/__init__.py` & `opensrane-0.0.5/opensrane/PhysicalEffect/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PhysicalEffect/fire_point_source.py` & `opensrane-0.0.5/opensrane/PhysicalEffect/fire_point_source.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PlantUnits/ONGStorage.py` & `opensrane-0.0.5/opensrane/PlantUnits/ONGStorage.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PlantUnits/ObjManager.py` & `opensrane-0.0.5/opensrane/PlantUnits/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PlantUnits/SphericalTank.py` & `opensrane-0.0.5/opensrane/PlantUnits/SphericalTank.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PlantUnits/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/PlantUnits/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PlantUnits/_Position.py` & `opensrane-0.0.5/opensrane/PlantUnits/_Position.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PlantUnits/__init__.py` & `opensrane-0.0.5/opensrane/PlantUnits/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Plot/Matplot.py` & `opensrane-0.0.5/opensrane/Plot/Matplot.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Plot/ObjManager.py` & `opensrane-0.0.5/opensrane/Plot/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Plot/Plotly.py` & `opensrane-0.0.5/opensrane/Plot/Plotly.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Plot/__init__.py` & `opensrane-0.0.5/opensrane/Plot/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PostProcess/ObjManager.py` & `opensrane-0.0.5/opensrane/PostProcess/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/PostProcess/RecorderPP.py` & `opensrane-0.0.5/opensrane/Recorders/recorder.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,361 +26,351 @@
  Created: 2022
  
  Revision: -
  By & Date: -
 '''
 
 
+from opensrane.Misc._NewClass import _NewClass
+from .ObjManager import *
 import opensrane as _opr
-import random as _rnd
-from tqdm import tqdm as _tqdm
-import multiprocessing as _mp
-import numpy as _np
+import json as _json
 import os as _os
 
-class RecorderPP():
+class recorder(_NewClass):
+    '''
+    Developer Attention: To add any new recorder :
+                                                    1st- Add target data to the "Record" method
+                                                    2nd- Remember to add two header row to the 
     
-    Results=None
+    This Object Specify a recorder object that records type of data to a variable or a file
+    filename: name of the file that user wants to store data in
+    fileAppend: specify that does the recorder add data to the current data in name or not
+    recordfield: Specifies the field of data that want to record. The selections are as the following
+        'DamageLevel' : record the damage level of each plant unit ( the level that the plant unit got damage)
+        'NodesGroupIsDamaged' : record the nodesgroup with tag equal NodesGroupTag is damaged or not (0 for not damaged and 1 for damaged or failed or dead)
+        'FragilityTag' : record the Happened Fragility tag of each plant unit
+        'LOC' : record the maximum released liquid (LOC : Loss of containment) of each plant unit
+        'HazardMag' : Record the sampled hazard magnitude
+        'NodesRadiationOverPressure' : Record NodesGroup Radiation,OverPressure 
+        'NodesRadiationProbit' :
+        'NodesOverPressureProbit' : 
 
-    def Analyze(Recorer_FilenamesList=[],Number_Of_LOC_Histogram_Bins=100):
+        
+        
+
+    NodesGroupTag : Specify the tag of interested nodesgroup to be recorded for 'NodesGroupIsDamaged'
+        
+    recorded results is a list that in each line first it gives the scenario number and in the following it gives requested data
+    
+    '''
+    
+    def __init__(self,tag,filename='Recorder',fileAppend=True, recordfield='DamageLevel', NodesGroupTag=1, MergeSavedFiles=False):
+         
+        #---- Fix Part for each class __init__ ----
+        ObjManager.Add(tag,self)
+        _NewClass.__init__(self,tag)
+        #------------------------------------------
+        
+        self.filename=filename
+        self.fileAppend=fileAppend
+        self.recordfield=recordfield
+        self.NodesGroupTag=NodesGroupTag
+        
+        self.results=""        #String Variable that the results are stored in
+        self.AnalyzeCounter=0  #Integer that counts the number of calling record method that shows the number of the analysis
 
-        #Define Variables
-        DamagedLevelList=[]             #list of the plant units Damage level list, each value is a Dictionary of Damage level of the plant units for each scenario
-        FragilityTagList=[]             #List of the plant units happend fragility tag Dictionaries, 
-        LOCList=[]                      #List of the PlantUnits tag and max Loss of Containment value Dictionary
-        NodesGroupDamageList=[]         #List of NodesGroup isDamaged list, each Dictionary is NodesGroupTag and corresponding Damagelist
-        NodesGroupTypeDict={}           #Dictionray of each NodesGroup object that keys are tag of nodes group and values are the type of the nodes group
-        NodesGroupDamProb={}            #Dictionray of each NodesGroup object that keys are tag of nodes group and values are the probability of their damage
-        NodesGroupRadiationAveDict={}  #Dictionary of NodesGroup Radiation Data, and keys is Nodes Group tag and value is the list of Radiation values Average 
-        NodesGroupOverPressureAveDict={}  #Dictionary of NodesGroup OverPressure Data, and keys is Nodes Group tag and value is the list of OverPressure values Average
-        NodesGroupOVPProbAveDict={}     #Dictionary of NodesGroup OverPressure corresponding Probit Data, and keys is Nodes Group tag and value is the list of Probit(OverPressure) values Average 
-        NodesGroupRadProbAveDict={}     #Dictionary of NodesGroup Radiation Probit Data, and keys is Nodes Group tag and value is the list of Probit(Radiation) values Average
-        ListOfLoc=[]                    #List of total LOC in each scenario
-        [bins,hist,probloc]=[[],[],[]]  #statistics parameters of LOC in scenarios (bins of LOC, histogram values, probability values)
-        DmglvlLOC={}
-        TotalScenario=None              #Total modeled scenario number
-        UnitsZeroDamageProb={}          #Probability of each PlantUnit zero level damage
-        ProbOfFragilities=[]            #Probablility of happening each fragility 
-        HazardMagnitude=[]              #List of the hazard tags and magnitudes (tag as key and magnitude as value)
-        ScenNameDamLvlDict={}            #Dictionary that its key is Scenario name and the value is its corresponding Damage level Dictionary
-
-
-        files=_os.listdir()
-        #Check files content one by one
-        for file in Recorer_FilenamesList:
-            
-            #Check if file exist
-            if file not in files:
-                print(f'{file} not found and not loaded!')
-                continue
-
-            #Text to show the loading file started
-            print('filename:',file,end=' ')
-            
-            with open(file, "r") as file:
-                filedata = file.readlines()
-
-            #File rows number -2 headers line is equal to the recorded scenarios number
-            TotalScenario=int(filedata[0].split('-')[0][1:])
+        #Set does the code merge all created files together or not
+        self.MergeSavedFiles=MergeSavedFiles
+        
+        #Remember for parallel analysis it cause multiple remove and in parallel do not set fileAppend==False
+        if fileAppend==False:
+            self._Deletefile()
+
+        #If file append be True then code should find the number of maximum existing saved file and create new files with number greater than the founded number
+        self.MaxExistSavedfileIndex=0
+        if fileAppend==True:
             
+            for file in _os.listdir():
+                if file[-6:]=='OPRrec' and file[:len(filename)]==filename and len(file)>=len(filename+'.OPRrec'):
+                    num=file[len(filename):-7]
+                    if num!='' and num.isnumeric()==True:
+                        if int(num)>self.MaxExistSavedfileIndex: self.MaxExistSavedfileIndex=int(num)            
+        
+    def Record(self):
 
-            #Read the type of recoder (Recorder field)
-            RecordField=filedata[0].split('=')[1].split("'")[1]
+        #By each time calling the Record command, 1 should be added to analyze counter 
+        self.AnalyzeCounter +=1
 
+        #If there is any damage then the data will be recorded
+        if _opr.Analyze.ScenarioAnalyze.anydamage==False: return
 
-            #Case Recorder is 'DamageLevel'-----------------------------------------------
-            if RecordField=='DamageLevel':
+        #-----------Case recordfield be 'DamageLevel'
+        if self.recordfield=='DamageLevel':
+            
+          
+            #Record data
+            record=""   #Dictionary that records the current scenario data
+            for tag,obj in _opr.PlantUnits.ObjManager.TagObjDict.items():
                 
-                #Export PlantUnits objects tag
-                Objstag=filedata[1].split('=')[1].split('[')[1].split(']')[0].split(',')
-                Objstag=[int(i) for i in Objstag]
-
-
-                # Export DamagedLevelList data
-                for linedata in filedata[2:]:   #data[2:] beccause two first lines are headers
-                    
-                    DamagedLevelList.append({tag:(int(dmlvl) if dmlvl!='None' else None)  for tag,dmlvl in zip(Objstag,linedata.split())})
-                    
-                #------ Probability of Units Zero Level Damage
-                UnitsZeroDamageProb={tag:0 for tag in Objstag}
-                for DamLevelDict in DamagedLevelList:
-                    for tag,DamLev in DamLevelDict.items() :
-                        if DamLev==0: UnitsZeroDamageProb[tag]=UnitsZeroDamageProb[tag]+1
-
-                #convert to probability
-                UnitsZeroDamageProb={tag:DamLev/TotalScenario for tag,DamLev in UnitsZeroDamageProb.items()}
-
-                #------ Probability of Damage levels and scenarios and subscenarios and Scenarios analyze number
-                Results={} #Store scenario and number of happening (ScenariosProbability)
-                ScenariosAnalyzeNumbers={} #Store scenario(key)  and number of alnazed scenarios list (Value)
-                DamlvlScenDict={}   #Dictionary of damage level (key) and corresponding Scenarios set (Value)
-                for ScenarioNum,damagelistrow in enumerate(DamagedLevelList):
-                    LevelList=RecorderPP._LevelList(damagelistrow)
-                    LevelList=['-'.join(LevelList[:i])  for i in range(1,len(LevelList)+1)]
-                    #fill DamlvlScenDict
-                    for lvl,name in enumerate(LevelList):
-                        if lvl not in DamlvlScenDict.keys():
-                            DamlvlScenDict[lvl]=set([name])
-                        else:
-                            DamlvlScenDict[lvl].update([name])
-
-                    #Fill Results for ScenariosProbability
-                    if LevelList!=[]: 
-                        
-                        for i in  LevelList:
-                            if i not in Results.keys():
-                                Results[i]=1
-                            else:
-                                Results[i]=Results[i]+1
-                    
-                    #Fill Results for ScenariosProbability
-                    if LevelList!=[]: 
-                        i=LevelList[-1]
-                        if i not in ScenariosAnalyzeNumbers.keys():
-                            ScenariosAnalyzeNumbers[i]=[ScenarioNum]
-                        else:
-                            ScenariosAnalyzeNumbers[i].append(ScenarioNum)                    
-
-                #Convert Results number to probability(value) (Scenario(key)) 
-                ScenariosProbability={tag:val/TotalScenario for tag,val in Results.items()}
-
-                #Scenarios(key) and its SubScenariosList(Value) Dictionary
-                dmlvl=lambda scenario: [key for key,val in DamlvlScenDict.items() if scenario in val][0] #Find scenario damage level
-                ScanariosSubScenario={Scenario:[] for Scenario in Results.keys()}
-                for Scenario in ScanariosSubScenario.keys():
-                    ScanariosSubScenario[Scenario]=[SubScen for SubScen in Results.keys() if (dmlvl(SubScen)==dmlvl(Scenario)+1 and Scenario in SubScen)]
-
-                #Create Damage Level and Corresponding Name Dictionary
-                for dmlvl in DamagedLevelList:
-                    ScenNameDamLvlDict["-".join(RecorderPP._LevelList(dmlvl))]=dmlvl
-
-
-            #Case Recorder is 'FragilityTagList'-----------------------------------------------
-            if RecordField=='FragilityTag':
-
-                #Export PlantUnits objects tag
-                Objstag=filedata[1].split('=')[1].split('[')[1].split(']')[0].split(',')
-                Objstag=[int(i) for i in Objstag]
-
-                # Export Fragility/Probit recorded data
-                for linedata in filedata[2:]:    #data[2:] beccause two first lines are headers
-                    
-                    FragilityTagList.append({tag:(int(Fragtag) if Fragtag!='None' else None)  for tag,Fragtag in zip(Objstag,linedata.split())})
+                #record damage level of the each plant unit
+                record=record+str(obj.DamageLevel)+' '                     
+        
+        #-----------Case recordfield be 'NodesGroupIsDamaged'
+        if self.recordfield=='NodesGroupIsDamaged':
+            
+               
+            #Record data
+            record=''   #Dictionary that records the current scenario data
+            if _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].isDamagedList==[]: #Means not analyzed because no damage
+                record='0 '*len(_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].xGlobalList)
+            else:            
+
+                #record damage level of the each plant unit
+                record=record.join([("0 " if i==False else "1 ") for i in _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].isDamagedList])      
 
+        #-----------Case recordfield be 'FragilityTag'
+        if self.recordfield=='FragilityTag':
+            
+          
+            #Record data
+            record=""   #Dictionary that records the current scenario data
+            for tag,obj in _opr.PlantUnits.ObjManager.TagObjDict.items():
                 
-                #------ Probability of happening Fragilities and probits
-                #find Fragilities tag (Fragtags)
-                Fragtags=[]
-                [Fragtags.extend([fragtag for fragtag in fragdict.values() if fragtag!=None]) for fragdict in FragilityTagList]
-                Fragtags=list(set(Fragtags))
+                #record damage level of the each plant unit
+                record=record+str(obj.DamageFragilityTag)+' '          
 
-                ProbOfFragilities={tag:0 for tag in Fragtags}
-                for FragDict in FragilityTagList:
-                    for Fragtag in FragDict.values() :
-                        if Fragtag!=None: ProbOfFragilities[Fragtag]=ProbOfFragilities[Fragtag]+1
+        #-----------Case recordfield be 'LOC'
+        if self.recordfield=='LOC':
+            
+          
+            #Record data
+            record=""   #Dictionary that records the current scenario data
+            for tag,obj in _opr.PlantUnits.ObjManager.TagObjDict.items():
+                
+                #record damage level of the each plant unit
+                record=record+str(max(obj.OutFlowModelObject.TotalMassLiquid_Release) if obj.OutFlowModelObject!=None else 0)+' '         
+                
+        #-----------Case recordfield be 'HazardMag'
+        if self.recordfield=='HazardMag':
+            
+          
+            #Record data
+            record=""   #Dictionary that records the current scenario data
+            for tag,obj in _opr.Hazard.ObjManager.TagObjDict.items():
+                
+                #record damage level of the each plant unit
+                record=record+str(obj.SampledMagnitude) +' '         
 
-                #convert to probability
-                ProbOfFragilities={tag:Num/TotalScenario for tag,Num in ProbOfFragilities.items()}
+        #-----------Case recordfield be 'NodesRadiationOverPressure'
+        if self.recordfield=='NodesRadiationOverPressure':
+            
+               
+            #Record data
+            record=''   #Dictionary that records the current scenario data
+            if _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].isDamagedList==[]: #Means not analyzed because no damage
+                record='0,0 '*len(_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].xGlobalList)
+            else:            
+
+                #record RadiationOverPressure for each node
+                record=record.join([f"{round(Radiation,4)},{round(OVPressure,4)} " for Radiation,OVPressure in zip(_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].Radiation_Intensity,
+                                                                                                                   _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].OverPressure_Intensity)])      
 
+        #-----------Case recordfield be 'NodesToxic'
+        if self.recordfield=='NodesToxic':
+            
+               
+            #Record data
+            record=''   #Dictionary that records the current scenario data
+            if _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].isDamagedList==[]: #Means not analyzed because no damage
+                record='None '*len(_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].xGlobalList)
+            else:            
 
+                #record damage level of the each plant unit
+                record=record.join([",".join([f"{mattag}:{dose}" for mattag,dose in recDict.items()])+" " for recDict in _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].Toxic_Intensity])      
 
-            #Case Recorder is 'LOCList'-----------------------------------------------
-            if RecordField=='LOC':
+        #-----------Case recordfield be 'NodesRadiationProbit'
+        if self.recordfield=='NodesRadiationProbit':
+            
+               
+            #Record data
+            record=''   #Dictionary that records the current scenario data
+            if _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].isDamagedList==[]: #Means not analyzed because no damage
+                record='0 '*len(_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].xGlobalList)
+            else:            
 
-                #Export PlantUnits objects tag
-                Objstag=filedata[1].split('=')[1].split('[')[1].split(']')[0].split(',')
-                Objstag=[int(i) for i in Objstag]
+                #record RadiationOverPressure for each node
+                record=record.join([f"{RadiationProbit} " for RadiationProbit in _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].Radiation_Probit])      
 
-                # Export LOC recorded data
-                for linedata in filedata[2:]:    #data[2:] beccause two first lines are headers
-                    
-                    LOCList.append({tag:float(Loci) for tag,Loci in zip(Objstag,linedata.split())})
+        #-----------Case recordfield be 'NodesOverPressureProbit'
+        if self.recordfield=='NodesOverPressureProbit':
+            
+               
+            #Record data
+            record=''   #Dictionary that records the current scenario data
+            if _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].isDamagedList==[]: #Means not analyzed because no damage
+                record='0 '*len(_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].xGlobalList)
+            else:            
 
+                #record RadiationOverPressure for each node
+                record=record.join([f"{OverPressureProbit} " for OverPressureProbit in _opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].OverPressure_Probit])      
 
-                #----Probability of Loss of Containment 
-                ListOfLoc=[sum(list(LOCDIC.values())) for LOCDIC in LOCList]
-                
-                minLoc=min([i for i in ListOfLoc if i!=0])
-                maxLoc=max([i for i in ListOfLoc if i!=0])
-                nbins=Number_Of_LOC_Histogram_Bins
-                hist, bins=_np.histogram(ListOfLoc,bins=[minLoc+(maxLoc-minLoc)/nbins*i for i in range(nbins+1)]) #length of the bins always should be one more than length of the hist
-                probloc=[i/TotalScenario for i in hist] 
-
-                #----Damagelevel and corresponding expected loss of containment
-                for dam,loc in zip(DamagedLevelList,LOCList):
-                    for tag,dmlvl in dam.items():
-                        if (dmlvl not in list(DmglvlLOC.keys()) and dmlvl!=None):
-                            DmglvlLOC[dmlvl]=0
-                        if (loc[tag]!=None and dmlvl!=None):
-                            DmglvlLOC[dmlvl]=DmglvlLOC[dmlvl]+loc[tag]
-                    
-                #convert to expected Value
-                for dmlvl,loc in DmglvlLOC.items():
-                    DmglvlLOC[dmlvl]=loc/TotalScenario
-
-
-            #Case Recorder is 'NodesGroupIsDamaged'-----------------------------------------------
-            if RecordField=='NodesGroupIsDamaged':
-
-                #Export NodesGroup Tag and type
-                NodesGroupTag=int(filedata[1].split()[3])
-                NodesGroupType=filedata[1].split('=')[-1]
+        #----- Final Part -----   (((Add recorded data to the results)))
+        self.results=f'{self.results}\n{record}'            #Format of entering scenario tag and other
+        
+        
+        
+    def SaveToFile(self,fileindex):
 
-                #NodesGroupTypeDict
-                NodesGroupTypeDict[NodesGroupTag]=NodesGroupType
-                
-                #Export Data
-                for linedata in filedata[2:]:    #data[2:] beccause two first lines are headers
-                    NodesGroupDamageList.append({NodesGroupTag:[int(isDam) for isDam in linedata.split()]})
+        #fileindex: is an integer that will be add to the end of the filename to save in seperate file
+        #fileindex are from 0 to number of files. If user wanna to append the existing files then the maximum index number of existing files should be added to input fileindex
+        cnt=fileindex+self.MaxExistSavedfileIndex
 
-                #----Probability of NodesGroup Damage
-                NGtag=NodesGroupTag
-                NodesGroupDamProb[NGtag]=[int(i) for i in filedata[2].split()]
 
-                for linedata in filedata[3:]:
-                    NodesGroupDamProb[NGtag]=[i+int(j) for i,j in zip(NodesGroupDamProb[NGtag],linedata.split())]
+        #--------------- First part: Define Header lines (Two First Rows) ---------------------------------------------------------------------
+        
+        #Fill two first header line
+        #-----------Case recordfield be 'DamageLevel'
+        if self.recordfield=='DamageLevel':
 
-                #convert to expected Value
-                NodesGroupDamProb[NGtag]=[i/TotalScenario for i in NodesGroupDamProb[NGtag]]
+            header="%"+str(self.AnalyzeCounter) + '-'+"recordfield='DamageLevel'" #First line specify Number of analysis and the recordfield name
+            header=f'{header}\n%PlantUnits tags = {[tag for tag in _opr.PlantUnits.ObjManager.TagObjDict.keys()]}' #Secondline specifiy the tags of the plant units
 
+        #-----------Case recordfield be 'NodesGroupIsDamaged'
+        if self.recordfield=='NodesGroupIsDamaged':
 
+            header="%"+str(self.AnalyzeCounter) + '-'+"recordfield='NodesGroupIsDamaged'" #First line specify Number of analysis and the recordfield name
+            header=f'{header}\n%NodesGroup with tags {self.NodesGroupTag} and with type={_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].Type}' #Secondline shows the tags and type of the nodesgroup
 
-            #Case Recorder is 'HazardMag'-----------------------------------------------
-            if RecordField=='HazardMag':
-                
-                #Export Hazard objects tag
-                Objstag=filedata[1].split('=')[1].split('[')[1].split(']')[0].split(',')
-                Objstag=[int(i) for i in Objstag]
+        #-----------Case recordfield be 'FragilityTag'
+        if self.recordfield=='FragilityTag':
 
+            header="%"+str(self.AnalyzeCounter) + '-'+"recordfield='FragilityTag'" #First line specify Number of analysis and the recordfield name
+            header=f'{header}\n%PlantUnits tags = {[tag for tag in _opr.PlantUnits.ObjManager.TagObjDict.keys()]}' #Secondline specifiy the tags of the plant units
 
-                # Export Hazard data
-                for linedata in filedata[2:]:   #data[2:] beccause two first lines are headers
-                    
-                    HazardMagnitude.append({tag:(float(mag) if dmlvl!='None' else None)  for tag,mag in zip(Objstag,linedata.split())})
+        #-----------Case recordfield be 'LOC'
+        if self.recordfield=='LOC':
 
-            #Case Recorder is 'NodesRadiationOverPressure'-----------------------------------------------
-            if RecordField=='NodesRadiationOverPressure':
-                
-                #import NodesGroup Tag and type
-                NodesGroupTag=int(filedata[1].split()[5])
-                NodesGroupType=filedata[1].split('=')[-1]
-
-                #NodesGroupTypeDict
-                NodesGroupTypeDict[NodesGroupTag]=NodesGroupType
-
-                # import NodesRadiationOverPressure data
-                for linedata in filedata[2:]:   #data[2:] beccause two first lines are headers
-
-                    if NodesGroupTag not in NodesGroupRadiationAveDict.keys():
-                        NodesGroupRadiationAveDict[NodesGroupTag]=[0 for i in [float(data.split(',')[0])  for data in linedata.split()]]
-                        NodesGroupOverPressureAveDict[NodesGroupTag]=[0 for i in [float(data.split(',')[0])  for data in linedata.split()]]
-                    
-                    NodesGroupRadiationAveDict[NodesGroupTag]=[i+j for i,j in zip(NodesGroupRadiationAveDict[NodesGroupTag],[float(data.split(',')[0])  for data in linedata.split()])]
-                    NodesGroupOverPressureAveDict[NodesGroupTag]=[i+j for i,j in zip(NodesGroupOverPressureAveDict[NodesGroupTag],[float(data.split(',')[1])  for data in linedata.split()])]
-
-                #Convert to average
-                NodesGroupRadiationAveDict[NodesGroupTag]=[i/TotalScenario for i in NodesGroupRadiationAveDict[NodesGroupTag]]
-                NodesGroupOverPressureAveDict[NodesGroupTag]=[i/TotalScenario for i in NodesGroupOverPressureAveDict[NodesGroupTag]]
-                
+            header="%"+str(self.AnalyzeCounter) + '-'+"recordfield='LOC'" #First line specify Number of analysis and the recordfield name
+            header=f'{header}\n%PlantUnits tags = {[tag for tag in _opr.PlantUnits.ObjManager.TagObjDict.keys()]}' #Secondline specifiy the tags of the plant units
 
-            #Case Recorder is 'NodesRadiationProbit'-----------------------------------------------
-            if RecordField=='NodesRadiationProbit':
-                
-                #import NodesGroup Tag and type
-                NodesGroupTag=int(filedata[1].split()[3])
-                NodesGroupType=filedata[1].split('=')[-1]
+        #-----------Case recordfield be 'HazardMag'
+        if self.recordfield=='HazardMag':
 
-                #NodesGroupTypeDict
-                NodesGroupTypeDict[NodesGroupTag]=NodesGroupType
+            header="%"+str(self.AnalyzeCounter) + '-'+"recordfield='HazardMag'" #First line specify Number of analysis and the recordfield name
+            header=f'{header}\n%Defined Hazards tags = {[tag for tag in _opr.Hazard.ObjManager.TagObjDict.keys()]}' #Secondline specifiy the tags of the plant units
 
+        #-----------Case recordfield be 'NodesRadiationOverPressure'
+        if self.recordfield=='NodesRadiationOverPressure':
 
-                # import NodesRadiationProbit data
-                for linedata in filedata[2:]:   #data[2:] beccause two first lines are headers
+            header="%"+str(self.AnalyzeCounter) + '-'+"recordfield='NodesRadiationOverPressure'" #First line specify Number of analysis and the recordfield name
+            header=f'{header}\n%(Radiation,OverPressure) for NodesGroup with tags {self.NodesGroupTag} and with type={_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].Type}' #Secondline shows the tags and type of the nodesgroup
 
-                    if NodesGroupTag not in NodesGroupRadProbAveDict.keys():
-                        NodesGroupRadProbAveDict[NodesGroupTag]=[0 for i in [float(data)  for data in linedata.split()]]
+        #-----------Case recordfield be 'NodesToxic'
+        if self.recordfield=='NodesToxic':
 
-                    NodesGroupRadProbAveDict[NodesGroupTag]=[i+j for i,j in zip(NodesGroupRadProbAveDict[NodesGroupTag],[float(data)  for data in linedata.split()])]
+            header="%"+str(self.AnalyzeCounter) + '-'+"recordfield='NodesToxic'" #First line specify Number of analysis and the recordfield name
+            header=f'{header}\n%(ProbitTag:Dose,...) [(0:0) for not for No toxic tag] NodesGroup with tags {self.NodesGroupTag} and with type={_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].Type}' #Secondline shows the tags and type of the nodesgroup
 
-                #Convert to average
-                NodesGroupRadProbAveDict[NodesGroupTag]=[i/TotalScenario for i in NodesGroupRadProbAveDict[NodesGroupTag]]
+        #-----------Case recordfield be 'NodesRadiationProbit'
+        if self.recordfield=='NodesRadiationProbit':
 
+            header="%"+str(self.AnalyzeCounter) + '-'+"recordfield='NodesRadiationProbit'" #First line specify Number of analysis and the recordfield name
+            header=f'{header}\n%NodesGroup with tags {self.NodesGroupTag} and with type={_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].Type}' #Secondline shows the tags and type of the nodesgroup
 
-            #Case Recorder is 'NodesOverPressureProbit'-----------------------------------------------
-            if RecordField=='NodesOverPressureProbit':
-                
-                #import NodesGroup Tag and type
-                NodesGroupTag=int(filedata[1].split()[3])
-                NodesGroupType=filedata[1].split('=')[-1]
+        #-----------Case recordfield be 'NodesOverPressureProbit'
+        if self.recordfield=='NodesOverPressureProbit':
+
+            header="%"+str(self.AnalyzeCounter) + '-'+"recordfield='NodesOverPressureProbit'" #First line specify Number of analysis and the recordfield name
+            header=f'{header}\n%NodesGroup with tags {self.NodesGroupTag} and with type={_opr.NodesGroups.ObjManager.TagObjDict[self.NodesGroupTag].Type}' #Secondline shows the tags and type of the nodesgroup
 
-                #NodesGroupTypeDict
-                NodesGroupTypeDict[NodesGroupTag]=NodesGroupType
 
+        #----- Final Part ----- Write to file/s 
+        #Add results to header
+        self.results=str(header)+str(self.results)
 
-                # import NodesOverPressureProbit data
-                for linedata in filedata[2:]:   #data[2:] beccause two first lines are headers
+        #(((Save recorded data to the file or files (Create new file and write to it))))
+        with open(self.filename+str(cnt)+'.OPRrec', 'w' ) as file:
+                file.write(str(self.results))        
+                self.results=""                 #Clear results after writing them in file
 
-                    if NodesGroupTag not in NodesGroupOVPProbAveDict.keys():
-                        NodesGroupOVPProbAveDict[NodesGroupTag]=[0 for i in [float(data)  for data in linedata.split()]]
+        #Set the Recorder Counter to zero
+        self.AnalyzeCounter=0
+    
+    def OtherSaveOnce(self):
+        #Just because such method exist for objs_recorder, so here also should exist to avoid error when calling all objects (For recorder it doesn't do anything
+        pass
+    
+    
+    def _Deletefile(self):
+        
+            
+        #Remove all OPR files
+        for file in _os.listdir():
+            if file[-6:]=='OPRrec' and file[:len(self.filename)]==self.filename:
+                _os.remove(file)
+
+    def _MergeAndClear(self):
+        '''
+        Merge multiple files to gether and clear the created files
 
-                    NodesGroupOVPProbAveDict[NodesGroupTag]=[i+j for i,j in zip(NodesGroupOVPProbAveDict[NodesGroupTag],[float(data)  for data in linedata.split()])]
+        '''
+        
+        #At the end of analysis _MergeAndClear method for any object will be called and for each object 
+        if self.MergeSavedFiles==True:
+        
+            AllData=''
+            AllAnalysisNumber=0
+            files=_os.listdir()
 
-                #Convert to average
-                NodesGroupOVPProbAveDict[NodesGroupTag]=[i/TotalScenario for i in NodesGroupOVPProbAveDict[NodesGroupTag]]
+            #Set files equal the files that their name is similar with 
+            Recfiles=[file for file in files if (file.startswith(self.filename) and file.endswith('OPRrec') and len(file)>len(self.filename+'.OPRrec'))]
 
+            #Get all files content
 
-            #Text to show the loading file ended
-            print('loaded.',end=' ')
-        
+            for file in Recfiles:
+                
+                #read file data
+                with open(file,'r') as f:
+                
+                    #Get and store the number of analysis
+                    data=f.readlines()
+                    FirstLine=data[0]  #Save firstline 
+                    Secondline=data[1] #Save second line data
+                    Number_of_analysis=data[0].split('-')[0][1:]
+                    AllAnalysisNumber=AllAnalysisNumber+int(Number_of_analysis)
+                    data=''.join(data[2:])  
+                    AllData=AllData +"\n"+data if data!='' else AllData
+                
+                #Remove file
+                _os.remove(file)
 
+                
+            #Create first two lines
+            header="%"+str(AllAnalysisNumber)+'-'+FirstLine.split('-')[1][:-1]+'\n'+Secondline[:-1]
 
-        RecorderPP.Results=dict(DamagedLevelList=DamagedLevelList,
-                                UnitsZeroDamageProb=UnitsZeroDamageProb,
-                                Total_Number_Of_Scenarios=TotalScenario,
-                                FragilityTagList=FragilityTagList,
-                                ProbOfFragilities=ProbOfFragilities,
-                                LOCList=LOCList,
-                                Damagelevel_eLOC=DmglvlLOC,
-                                TotalLOCList=ListOfLoc,
-                                LOC_bins_hist_probloc=[bins,hist,probloc],
-                                NodesGroupDamageList=NodesGroupDamageList,
-                                NodesGroupTypeDict=NodesGroupTypeDict,
-                                NodesGroupDamageProbability=NodesGroupDamProb,
-                                ScenariosAnalyzeNumbers=ScenariosAnalyzeNumbers,
-                                ScenariosProbability=ScenariosProbability,
-                                ScanariosSubScenario=ScanariosSubScenario,
-                                Damagelevel_Scenario_Dict=DamlvlScenDict,
-                                HazardMagnitude=HazardMagnitude,
-                                ScenarioName_DamageLevel_Dict=ScenNameDamLvlDict,
-                                NodesGroupRadiationDict=NodesGroupRadiationAveDict,
-                                NodesGroupOverPressureDict=NodesGroupOverPressureAveDict,
-                                NodesGroup_OVP_Probit_Dict=NodesGroupOVPProbAveDict,
-                                NodesGroup_Rad_Probit_Dict=NodesGroupRadProbAveDict,)
+            #add allData to the main file data
+            AllData=header+AllData
 
-        
-        return RecorderPP.Results
-    
+            with open(self.filename+'M.OPRrec', 'w' ) as file:
+                    file.write(AllData)  
 
 
-    def _LevelList(damagelistrow):
-        #This function returns damage levels and corresponding tags
-        #Format= (Damage Level):[tag of damaged units]
-
-        #if no damage happened return []
-        if 0 not in damagelistrow.values(): return []
-
-        #Export data
-        rslt={}
-        for tag,dmlvl in damagelistrow.items():
-            if dmlvl not in list(rslt.keys()) and dmlvl!=None:
-                rslt[dmlvl]=str(tag)
-            elif dmlvl!=None:
-                rslt[dmlvl]=rslt[dmlvl]+','+str(tag)
-        
-
-        #Arrange data from 0 to ... 
-        finalrslt=[]
-        for dmlvl in range(max(rslt.keys())+1):
-            text=f'({dmlvl}):[{rslt[dmlvl]}]'   #Convert to text format
-            finalrslt.append(text)
 
-        return finalrslt
+    def LoadRecorderfile(self,filename=''):
+        '''
+        This function return results of as a dictionary with keys equal to scenario tag and values equal to entered value
+        '''
+        if filename=='': filename=self.filename+'.OPRrec'
+        
+        with open(filename, "r") as file:
+            data = file.readlines()
+            
+        result={}   #Dictionary of the results
+        scenario=0
+        for dat in data[2:]:                        #data[2:] beccause two first lines are headers
+            scenario +=1         #First value that separated with : is the tag value    
+            rslt=[]
+            [rslt.extend([float(val) if val!='None' else None]) for val in dat.split()]
+            result[scenario]=rslt
+            
+        return result
```

### Comparing `OpenSRANE-0.0.4.1/opensrane/PostProcess/__init__.py` & `opensrane-0.0.5/opensrane/PostProcess/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Recorders/ObjManager.py` & `opensrane-0.0.5/opensrane/Recorders/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Recorders/__init__.py` & `opensrane-0.0.5/opensrane/Recorders/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Safety/Dike.py` & `opensrane-0.0.5/opensrane/Safety/Dike.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Safety/ObjManager.py` & `opensrane-0.0.5/opensrane/Safety/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Safety/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/Safety/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Safety/__init__.py` & `opensrane-0.0.5/opensrane/Safety/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Sites/ObjManager.py` & `opensrane-0.0.5/opensrane/Sites/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Sites/Site.py` & `opensrane-0.0.5/opensrane/Sites/Site.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Sites/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/Sites/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Sites/__init__.py` & `opensrane-0.0.5/opensrane/Sites/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Substance/DataBank.py` & `opensrane-0.0.5/opensrane/Substance/DataBank.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Substance/Material.py` & `opensrane-0.0.5/opensrane/Substance/Material.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Substance/ObjManager.py` & `opensrane-0.0.5/opensrane/Substance/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Substance/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/Substance/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/Substance/__init__.py` & `opensrane-0.0.5/opensrane/Substance/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/WindData/ObjManager.py` & `opensrane-0.0.5/opensrane/WindData/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/WindData/WindRose.py` & `opensrane-0.0.5/opensrane/WindData/WindRose.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/WindData/_GlobalParameters.py` & `opensrane-0.0.5/opensrane/WindData/_GlobalParameters.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/WindData/__init__.py` & `opensrane-0.0.5/opensrane/WindData/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/_New_module/New_class.py` & `opensrane-0.0.5/opensrane/_New_module/New_class.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/_New_module/ObjManager.py` & `opensrane-0.0.5/opensrane/_New_module/ObjManager.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/_New_module/__init__.py` & `opensrane-0.0.5/opensrane/_New_module/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/__init__.py` & `opensrane-0.0.5/opensrane/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/opensrane/version.py` & `opensrane-0.0.5/opensrane/version.py`

 * *Files identical despite different names*

### Comparing `OpenSRANE-0.0.4.1/setup.py` & `opensrane-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 setup(
     name="OpenSRANE",
     version=OpenSRANE_version,
     author="Bijan Sayyafzadeh",
     author_email="<OpenSRANE@Gmail.com>",
-    description="Open Software for Risk Assessment of Natech Events",
+    description="Open System for Risk Assessment of Natech Events",
     long_description_content_type="text/markdown",
     long_description=long_description ,
     package_data={
         # "":["*.jpg","*.at2","*.pyd"],
 
     },
     packages=find_packages(),
```

