# Comparing `tmp/steam-sdk-2024.5.3.tar.gz` & `tmp/steam-sdk-2024.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam-sdk-2024.5.3.tar", last modified: Mon May 13 10:25:49 2024, max compression
+gzip compressed data, was "steam-sdk-2024.5.4.tar", last modified: Tue May 14 13:15:47 2024, max compression
```

## Comparing `steam-sdk-2024.5.3.tar` & `steam-sdk-2024.5.4.tar`

### file list

```diff
@@ -1,216 +1,211 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:49.030924 steam-sdk-2024.5.3/
--rw-rw-rw-   0        0        0      264 2023-06-07 14:48:24.000000 steam-sdk-2024.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5753 2024-05-13 10:25:49.028925 steam-sdk-2024.5.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-13 10:25:49.030924 steam-sdk-2024.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1668 2024-05-13 10:22:21.000000 steam-sdk-2024.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.699924 steam-sdk-2024.5.3/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.747924 steam-sdk-2024.5.3/steam_sdk/analyses/
--rw-rw-rw-   0        0        0    37589 2024-04-19 11:58:44.000000 steam-sdk-2024.5.3/steam_sdk/analyses/AnalysisEvent.py
--rw-rw-rw-   0        0        0    30954 2024-04-26 11:34:23.000000 steam-sdk-2024.5.3/steam_sdk/analyses/AnalysisEventLHC.py
--rw-rw-rw-   0        0        0   135654 2024-05-13 10:08:33.000000 steam-sdk-2024.5.3/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.749936 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.751924 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23388 2024-01-12 14:29:22.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.762925 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16777 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2820 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6761 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95432 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2672 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2361 2024-01-12 14:29:35.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.765928 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22357 2024-03-11 05:39:28.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.772926 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4450 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2844 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.775925 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29436 2024-03-11 05:39:28.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.783923 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5330 2024-01-12 14:32:09.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4627 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4775 2024-01-12 14:32:10.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.787924 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-10 00:27:54.000000 steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.825924 steam-sdk-2024.5.3/steam_sdk/builders/
--rw-rw-rw-   0        0        0    13175 2024-03-13 09:34:54.000000 steam-sdk-2024.5.3/steam_sdk/builders/BuilderAPDL_CT.py
--rw-rw-rw-   0        0        0     4805 2024-03-22 08:53:57.000000 steam-sdk-2024.5.3/steam_sdk/builders/BuilderCosim.py
--rw-rw-rw-   0        0        0    17741 2024-02-07 15:54:14.000000 steam-sdk-2024.5.3/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   160440 2024-04-17 14:10:37.000000 steam-sdk-2024.5.3/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    53471 2024-05-08 10:36:11.000000 steam-sdk-2024.5.3/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2024-03-13 11:10:16.000000 steam-sdk-2024.5.3/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-08-22 11:29:04.000000 steam-sdk-2024.5.3/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12487 2024-04-11 22:26:08.000000 steam-sdk-2024.5.3/steam_sdk/builders/BuilderPySIGMA.py
--rw-rw-rw-   0        0        0    57747 2024-05-07 07:59:18.000000 steam-sdk-2024.5.3/steam_sdk/builders/BuilderTFM.py
--rw-rw-rw-   0        0        0    11689 2023-01-18 09:46:00.000000 steam-sdk-2024.5.3/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-06 11:41:34.000000 steam-sdk-2024.5.3/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-02 15:39:34.000000 steam-sdk-2024.5.3/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.827936 steam-sdk-2024.5.3/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.830924 steam-sdk-2024.5.3/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.832927 steam-sdk-2024.5.3/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     1426 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.835925 steam-sdk-2024.5.3/steam_sdk/cosims/
--rw-rw-rw-   0        0        0    26984 2024-04-29 06:28:52.000000 steam-sdk-2024.5.3/steam_sdk/cosims/CoSimPyCoSim.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.886924 steam-sdk-2024.5.3/steam_sdk/data/
--rw-rw-rw-   0        0        0     1684 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataAPDLCTOptions.py
--rw-rw-rw-   0        0        0    13080 2024-05-13 10:22:21.000000 steam-sdk-2024.5.3/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0      414 2024-03-06 09:01:34.000000 steam-sdk-2024.5.3/steam_sdk/data/DataCoSim.py
--rw-rw-rw-   0        0        0     9303 2024-04-08 06:18:59.000000 steam-sdk-2024.5.3/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0      308 2024-04-19 11:58:44.000000 steam-sdk-2024.5.3/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2987 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4636 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0    87484 2024-05-13 08:12:26.000000 steam-sdk-2024.5.3/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0     7309 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataFiQuSOptions.py
--rw-rw-rw-   0        0        0    16769 2024-04-08 06:18:59.000000 steam-sdk-2024.5.3/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     9528 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataLEDETOptions.py
--rw-rw-rw-   0        0        0     5377 2024-05-07 07:59:18.000000 steam-sdk-2024.5.3/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5216 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataModelCommon.py
--rw-rw-rw-   0        0        0     6621 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    12150 2024-04-29 06:28:52.000000 steam-sdk-2024.5.3/steam_sdk/data/DataModelCosim.py
--rw-rw-rw-   0        0        0     8020 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     6491 2024-04-19 11:58:44.000000 steam-sdk-2024.5.3/steam_sdk/data/DataModelParsimDakota.py
--rw-rw-rw-   0        0        0     3008 2024-04-08 08:00:24.000000 steam-sdk-2024.5.3/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0      625 2024-05-08 10:18:52.000000 steam-sdk-2024.5.3/steam_sdk/data/DataPlot.py
--rw-rw-rw-   0        0        0     2130 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2956 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataProteCCTOptions.py
--rw-rw-rw-   0        0        0     2595 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     1508 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataPyBBQOptions.py
--rw-rw-rw-   0        0        0      766 2024-04-17 14:10:37.000000 steam-sdk-2024.5.3/steam_sdk/data/DataPyCoSim.py
--rw-rw-rw-   0        0        0     6552 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataPySIGMA.py
--rw-rw-rw-   0        0        0     2228 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataPySIGMAOptions.py
--rw-rw-rw-   0        0        0      236 2024-02-01 12:22:22.000000 steam-sdk-2024.5.3/steam_sdk/data/DataRoxieParams.py
--rw-rw-rw-   0        0        0     9824 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0    12733 2024-05-06 07:29:15.000000 steam-sdk-2024.5.3/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3263 2024-03-21 12:23:41.000000 steam-sdk-2024.5.3/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0     6024 2024-05-07 07:59:18.000000 steam-sdk-2024.5.3/steam_sdk/data/DataTFM.py
--rw-rw-rw-   0        0        0    18457 2023-11-20 11:26:58.000000 steam-sdk-2024.5.3/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-08-23 08:56:30.000000 steam-sdk-2024.5.3/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 09:57:32.000000 steam-sdk-2024.5.3/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    30456 2024-04-08 06:18:59.000000 steam-sdk-2024.5.3/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-03-30 17:37:43.000000 steam-sdk-2024.5.3/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.900923 steam-sdk-2024.5.3/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3739 2024-01-31 11:21:01.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverANSYS.py
--rw-rw-rw-   0        0        0    13733 2024-04-26 11:34:23.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     7448 2024-04-15 08:30:14.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     4278 2024-05-06 07:29:15.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     4301 2024-05-13 10:25:12.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1894 2024-03-20 11:29:04.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2275 2024-04-19 11:54:24.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-06-02 08:33:55.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0      517 2024-02-21 14:45:24.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverPySIGMA.py
--rw-rw-rw-   0        0        0     1983 2024-03-13 14:05:47.000000 steam-sdk-2024.5.3/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/drivers/__init__.py
--rw-rw-rw-   0        0        0      723 2024-01-30 11:37:38.000000 steam-sdk-2024.5.3/steam_sdk/drivers/to_DELETE.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.936924 steam-sdk-2024.5.3/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-08-22 11:29:04.000000 steam-sdk-2024.5.3/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      315 2023-10-17 12:06:12.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0    14173 2024-04-17 08:17:01.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserCOSIM.py
--rw-rw-rw-   0        0        0     2290 2022-06-24 07:36:06.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1024 2023-10-17 12:06:12.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6302 2024-04-17 11:47:52.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     2729 2024-04-19 11:58:44.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     8536 2023-02-02 15:29:22.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2614 2024-03-19 10:59:46.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0     3760 2024-04-17 14:10:36.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserFile.py
--rw-rw-rw-   0        0        0    30071 2024-05-06 07:29:15.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    18391 2024-05-06 07:29:15.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    15085 2024-04-17 12:14:12.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    65009 2024-04-12 12:06:03.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4706 2023-10-17 12:06:12.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6765 2024-03-13 13:40:54.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     1758 2023-10-17 12:06:12.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserPyBBQ.py
--rw-rw-rw-   0        0        0     1663 2024-04-17 08:08:09.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserPyCoSim.py
--rw-rw-rw-   0        0        0     4061 2024-04-11 22:26:08.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserPySIGMA.py
--rw-rw-rw-   0        0        0   155447 2024-04-16 07:32:37.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11746 2024-04-12 13:06:00.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    58167 2024-05-06 07:29:15.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     7770 2024-04-18 11:38:14.000000 steam-sdk-2024.5.3/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0      929 2024-03-21 13:47:53.000000 steam-sdk-2024.5.3/steam_sdk/parsers/utils_ParserCircuits.py
--rw-rw-rw-   0        0        0     9687 2024-04-29 06:28:52.000000 steam-sdk-2024.5.3/steam_sdk/parsers/utils_ParserCosims.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.944930 steam-sdk-2024.5.3/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    66858 2024-04-16 07:32:37.000000 steam-sdk-2024.5.3/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0     4619 2024-04-15 08:30:14.000000 steam-sdk-2024.5.3/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    90102 2024-02-16 08:41:13.000000 steam-sdk-2024.5.3/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    48261 2024-03-18 14:18:48.000000 steam-sdk-2024.5.3/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.946924 steam-sdk-2024.5.3/steam_sdk/parsims/translation_dicts/
--rw-rw-rw-   0        0        0     2351 2024-04-08 08:04:39.000000 steam-sdk-2024.5.3/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
--rw-rw-rw-   0        0        0     2016 2023-05-09 19:16:09.000000 steam-sdk-2024.5.3/steam_sdk/parsims/translation_dicts/event_column_names.yaml
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.954924 steam-sdk-2024.5.3/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    29312 2023-07-13 14:20:54.000000 steam-sdk-2024.5.3/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0     8480 2024-05-08 10:18:52.000000 steam-sdk-2024.5.3/steam_sdk/plotters/PlotterGriddedData.py
--rw-rw-rw-   0        0        0    20627 2024-05-06 07:29:15.000000 steam-sdk-2024.5.3/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39519 2024-04-16 07:32:37.000000 steam-sdk-2024.5.3/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-06 11:41:34.000000 steam-sdk-2024.5.3/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0    13246 2024-03-25 10:52:36.000000 steam-sdk-2024.5.3/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:48.960928 steam-sdk-2024.5.3/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0    15676 2024-05-08 10:18:52.000000 steam-sdk-2024.5.3/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-14 13:30:58.000000 steam-sdk-2024.5.3/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:49.000923 steam-sdk-2024.5.3/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-13 09:01:17.000000 steam-sdk-2024.5.3/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0      204 2024-04-16 07:32:37.000000 steam-sdk-2024.5.3/steam_sdk/utils/MatrixOperations.py
--rw-rw-rw-   0        0        0    15002 2024-01-12 14:37:06.000000 steam-sdk-2024.5.3/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     3201 2024-04-08 06:18:59.000000 steam-sdk-2024.5.3/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2770 2024-04-08 06:18:59.000000 steam-sdk-2024.5.3/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-03-01 14:21:51.000000 steam-sdk-2024.5.3/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0     5730 2023-06-20 09:25:09.000000 steam-sdk-2024.5.3/steam_sdk/utils/ParserRoxieHelpers.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     5806 2024-03-27 10:23:11.000000 steam-sdk-2024.5.3/steam_sdk/utils/attribute_model.py
--rw-rw-rw-   0        0        0      686 2022-06-12 12:41:34.000000 steam-sdk-2024.5.3/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0    12832 2023-10-02 06:56:47.000000 steam-sdk-2024.5.3/steam_sdk/utils/compare_simulations.py
--rw-rw-rw-   0        0        0     3837 2023-02-03 13:26:48.000000 steam-sdk-2024.5.3/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0     1650 2024-04-11 23:08:34.000000 steam-sdk-2024.5.3/steam_sdk/utils/correct_RRR_NIST.py
--rw-rw-rw-   0        0        0      227 2024-01-10 14:12:29.000000 steam-sdk-2024.5.3/steam_sdk/utils/delete_if_existing.py
--rw-rw-rw-   0        0        0     1135 2024-04-17 08:22:42.000000 steam-sdk-2024.5.3/steam_sdk/utils/find_delete_files.py
--rw-rw-rw-   0        0        0     1204 2024-03-22 11:11:51.000000 steam-sdk-2024.5.3/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-06-11 12:54:31.000000 steam-sdk-2024.5.3/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      691 2024-04-11 22:26:08.000000 steam-sdk-2024.5.3/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0      928 2023-09-25 12:01:38.000000 steam-sdk-2024.5.3/steam_sdk/utils/make_json_schema.py
--rw-rw-rw-   0        0        0     4512 2022-05-02 08:49:48.000000 steam-sdk-2024.5.3/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1878 2023-11-21 15:44:37.000000 steam-sdk-2024.5.3/steam_sdk/utils/overwrite_files.py
--rw-rw-rw-   0        0        0    11408 2024-01-10 12:09:33.000000 steam-sdk-2024.5.3/steam_sdk/utils/overwrite_output_to_reference_files.py
--rw-rw-rw-   0        0        0     3555 2023-06-13 10:45:51.000000 steam-sdk-2024.5.3/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0     1596 2024-04-15 10:55:27.000000 steam-sdk-2024.5.3/steam_sdk/utils/read_settings_file.py
--rw-rw-rw-   0        0        0     3365 2023-12-06 09:10:21.000000 steam-sdk-2024.5.3/steam_sdk/utils/reformat_figure.py
--rw-rw-rw-   0        0        0      388 2022-04-11 18:20:26.000000 steam-sdk-2024.5.3/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-07 20:16:27.000000 steam-sdk-2024.5.3/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-04-11 18:20:26.000000 steam-sdk-2024.5.3/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-06-07 19:34:59.000000 steam-sdk-2024.5.3/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2023-05-12 14:38:34.000000 steam-sdk-2024.5.3/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:49.007927 steam-sdk-2024.5.3/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    39140 2024-02-23 08:10:26.000000 steam-sdk-2024.5.3/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:49.011925 steam-sdk-2024.5.3/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:49.013925 steam-sdk-2024.5.3/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:49.014925 steam-sdk-2024.5.3/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:49.016924 steam-sdk-2024.5.3/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam-sdk-2024.5.3/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1830 2024-01-10 12:13:04.000000 steam-sdk-2024.5.3/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:25:49.018925 steam-sdk-2024.5.3/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     5753 2024-05-13 10:25:48.000000 steam-sdk-2024.5.3/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7888 2024-05-13 10:25:48.000000 steam-sdk-2024.5.3/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 10:25:48.000000 steam-sdk-2024.5.3/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1745 2024-05-13 10:25:48.000000 steam-sdk-2024.5.3/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 10:25:48.000000 steam-sdk-2024.5.3/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.567932 steam-sdk-2024.5.4/
+-rw-rw-rw-   0        0        0      264 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5837 2024-05-14 13:15:47.565931 steam-sdk-2024.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-14 13:15:47.567932 steam-sdk-2024.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1668 2024-05-14 13:13:44.000000 steam-sdk-2024.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.141388 steam-sdk-2024.5.4/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.159387 steam-sdk-2024.5.4/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0    37589 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisEvent.py
+-rw-rw-rw-   0        0        0    30954 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisEventLHC.py
+-rw-rw-rw-   0        0        0   135856 2024-05-14 07:53:34.000000 steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.160387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.162387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23388 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.174388 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16777 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2820 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6761 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95432 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2672 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2361 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.177388 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22357 2024-04-11 12:40:24.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.185387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4450 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2844 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.188387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29436 2024-04-11 12:41:03.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.196387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4627 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4775 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.199387 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.223388 steam-sdk-2024.5.4/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    13175 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderAPDL_CT.py
+-rw-rw-rw-   0        0        0     4805 2024-03-22 11:40:47.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderCosim.py
+-rw-rw-rw-   0        0        0    17741 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   160548 2024-05-14 10:56:54.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    53474 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12487 2024-04-11 12:01:36.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderPySIGMA.py
+-rw-rw-rw-   0        0        0    66165 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/builders/BuilderTFM.py
+-rw-rw-rw-   0        0        0    11689 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.225387 steam-sdk-2024.5.4/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.229388 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.232388 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     1426 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.236388 steam-sdk-2024.5.4/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0    26984 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/cosims/CoSimPyCoSim.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.293389 steam-sdk-2024.5.4/steam_sdk/data/
+-rw-rw-rw-   0        0        0     1684 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataAPDLCTOptions.py
+-rw-rw-rw-   0        0        0    13080 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0      414 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DataCoSim.py
+-rw-rw-rw-   0        0        0     9303 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0      308 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2987 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4636 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    93048 2024-05-13 19:23:49.000000 steam-sdk-2024.5.4/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0     7309 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataFiQuSOptions.py
+-rw-rw-rw-   0        0        0    16769 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     9528 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataLEDETOptions.py
+-rw-rw-rw-   0        0        0     5330 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5216 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelCommon.py
+-rw-rw-rw-   0        0        0     6621 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    12150 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelCosim.py
+-rw-rw-rw-   0        0        0     8020 2024-04-30 14:26:16.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     6491 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/data/DataModelParsimDakota.py
+-rw-rw-rw-   0        0        0     3008 2024-04-08 08:37:58.000000 steam-sdk-2024.5.4/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0      625 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPlot.py
+-rw-rw-rw-   0        0        0     2130 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2956 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataProteCCTOptions.py
+-rw-rw-rw-   0        0        0     2595 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     1508 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPyBBQOptions.py
+-rw-rw-rw-   0        0        0      766 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPyCoSim.py
+-rw-rw-rw-   0        0        0     6552 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPySIGMA.py
+-rw-rw-rw-   0        0        0     2228 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataPySIGMAOptions.py
+-rw-rw-rw-   0        0        0      236 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DataRoxieParams.py
+-rw-rw-rw-   0        0        0     9824 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0    12733 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3263 2024-03-19 10:04:08.000000 steam-sdk-2024.5.4/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0     6207 2024-05-13 19:22:01.000000 steam-sdk-2024.5.4/steam_sdk/data/DataTFM.py
+-rw-rw-rw-   0        0        0    18457 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    30456 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.312388 steam-sdk-2024.5.4/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3739 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverANSYS.py
+-rw-rw-rw-   0        0        0    13733 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     7448 2024-04-14 11:58:12.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     4278 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3573 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1894 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2275 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0      517 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverPySIGMA.py
+-rw-rw-rw-   0        0        0     1983 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.399387 steam-sdk-2024.5.4/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      315 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0    14173 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCOSIM.py
+-rw-rw-rw-   0        0        0     2290 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1024 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6302 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     2729 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     8536 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2614 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0     3760 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserFile.py
+-rw-rw-rw-   0        0        0    30071 2024-04-30 14:35:01.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    18391 2024-04-30 14:35:01.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    15085 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    65086 2024-05-14 13:06:42.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4706 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6765 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     1758 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPyBBQ.py
+-rw-rw-rw-   0        0        0     1663 2024-04-22 06:54:43.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPyCoSim.py
+-rw-rw-rw-   0        0        0     4061 2024-04-11 12:27:48.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserPySIGMA.py
+-rw-rw-rw-   0        0        0   155447 2024-04-15 21:11:35.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0    11746 2024-04-12 18:35:10.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    58167 2024-04-30 14:26:16.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     7770 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0      929 2024-03-22 11:40:47.000000 steam-sdk-2024.5.4/steam_sdk/parsers/utils_ParserCircuits.py
+-rw-rw-rw-   0        0        0     9687 2024-04-30 05:16:26.000000 steam-sdk-2024.5.4/steam_sdk/parsers/utils_ParserCosims.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.410388 steam-sdk-2024.5.4/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    66858 2024-04-15 21:11:35.000000 steam-sdk-2024.5.4/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0     4619 2024-04-14 11:38:50.000000 steam-sdk-2024.5.4/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    90102 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    48261 2024-03-21 12:26:24.000000 steam-sdk-2024.5.4/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.418905 steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/
+-rw-rw-rw-   0        0        0     2351 2024-04-08 08:37:58.000000 steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+-rw-rw-rw-   0        0        0     2016 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/event_column_names.yaml
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.486417 steam-sdk-2024.5.4/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0    29312 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0     8480 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterGriddedData.py
+-rw-rw-rw-   0        0        0    20627 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39519 2024-04-15 21:11:35.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0    13246 2024-03-26 07:52:01.000000 steam-sdk-2024.5.4/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.491415 steam-sdk-2024.5.4/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0    15676 2024-05-08 10:41:57.000000 steam-sdk-2024.5.4/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.528417 steam-sdk-2024.5.4/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0      204 2024-04-15 21:11:35.000000 steam-sdk-2024.5.4/steam_sdk/utils/MatrixOperations.py
+-rw-rw-rw-   0        0        0    15002 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     3846 2024-05-13 21:24:50.000000 steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2770 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0     5730 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/ParserRoxieHelpers.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     5806 2024-04-05 07:58:47.000000 steam-sdk-2024.5.4/steam_sdk/utils/attribute_model.py
+-rw-rw-rw-   0        0        0      686 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0    12832 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/compare_simulations.py
+-rw-rw-rw-   0        0        0     3837 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0     1650 2024-04-12 18:35:10.000000 steam-sdk-2024.5.4/steam_sdk/utils/correct_RRR_NIST.py
+-rw-rw-rw-   0        0        0      227 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/delete_if_existing.py
+-rw-rw-rw-   0        0        0     1204 2024-03-22 11:42:52.000000 steam-sdk-2024.5.4/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      691 2024-04-11 06:51:22.000000 steam-sdk-2024.5.4/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     3555 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0     1596 2024-04-13 18:58:31.000000 steam-sdk-2024.5.4/steam_sdk/utils/read_settings_file.py
+-rw-rw-rw-   0        0        0     3365 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/reformat_figure.py
+-rw-rw-rw-   0        0        0      388 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.538931 steam-sdk-2024.5.4/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    39140 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.540931 steam-sdk-2024.5.4/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.540931 steam-sdk-2024.5.4/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.541932 steam-sdk-2024.5.4/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.542930 steam-sdk-2024.5.4/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1830 2024-03-19 09:48:27.000000 steam-sdk-2024.5.4/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2024-05-14 13:15:47.545932 steam-sdk-2024.5.4/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     5837 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7694 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1781 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 13:15:43.000000 steam-sdk-2024.5.4/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2024.5.3/PKG-INFO` & `steam-sdk-2024.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.5.3
+Version: 2024.5.4
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: STEAM,CERN,API,SDK
+Keywords: SDK,STEAM,API,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
@@ -30,14 +30,15 @@
 Requires-Dist: seaborn==0.13.2
 Requires-Dist: STEAM-materials==2024.4.2
 Requires-Dist: svglib==1.5.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: steam-pysigma==2024.3.2
 Requires-Dist: pyarrow==15.0.1
 Requires-Dist: tqdm==4.66.2
+Requires-Dist: mplcursors==0.5.3
 Provides-Extra: all
 Requires-Dist: gmsh==4.11.1; extra == "all"
 Requires-Dist: matplotlib==3.8.3; extra == "all"
 Requires-Dist: Jinja2==3.1.3; extra == "all"
 Requires-Dist: numpy==1.26.4; extra == "all"
 Requires-Dist: pandas==2.2.1; extra == "all"
 Requires-Dist: pydantic==2.6.4; extra == "all"
@@ -56,14 +57,15 @@
 Requires-Dist: seaborn==0.13.2; extra == "all"
 Requires-Dist: STEAM-materials==2024.4.2; extra == "all"
 Requires-Dist: svglib==1.5.1; extra == "all"
 Requires-Dist: PyYAML==6.0.1; extra == "all"
 Requires-Dist: steam-pysigma==2024.3.2; extra == "all"
 Requires-Dist: pyarrow==15.0.1; extra == "all"
 Requires-Dist: tqdm==4.66.2; extra == "all"
+Requires-Dist: mplcursors==0.5.3; extra == "all"
 Requires-Dist: Markdown==3.5.2; extra == "all"
 Requires-Dist: markdown-include==0.8.1; extra == "all"
 Requires-Dist: MarkupSafe==2.1.5; extra == "all"
 Requires-Dist: mkdocs==1.5.3; extra == "all"
 Requires-Dist: mkdocs-autorefs==1.0.1; extra == "all"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == "all"
 Requires-Dist: mkdocs-include-markdown-plugin==6.0.4; extra == "all"
```

### Comparing `steam-sdk-2024.5.3/setup.py` & `steam-sdk-2024.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 build_require = ["setuptools==69.2.0"]
 
 all_requirements = required + docs_require + tests_require + build_require
 
 setup(
     name="steam-sdk",
-    version="2024.5.3",
+    version="2024.5.4",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={"STEAM", "API", "SDK", "CERN"},
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/AnalysisEvent.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisEvent.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/AnalysisEventLHC.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisEventLHC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         self.list_sims = []  # this list will be populated with integers indicating simulations to run
         self.list_viewers = {}  # this dictionary will be populated with Viewer objects and their names
         self.list_metrics = {}  # this dictionary will be populated with calculated metrics
         self.verbose = verbose
         self.summary = None  # float representing the overall outcome of a simulation for parsims
         self.file_name_analysis = file_name_analysis
         self.simulation_numbers_source_tools_and_models = {}
+        self.input_parsim_sweep_df = pd.DataFrame()
         if file_name_analysis:
             self.path_analysis_file = str(Path(self.file_name_analysis).resolve())  # Find folder where the input file is located, which will be used as the "anchor" for all input files
         if isinstance(file_name_analysis, str) or isinstance(file_name_analysis, PurePath):
             self.data_analysis: DataAnalysis = yaml_to_data(file_name_analysis, DataAnalysis)  # Load yaml keys into DataAnalysis dataclass
             # Read analysis settings
             self._resolve_settings()
             # Read working folders and set them up
@@ -214,15 +215,16 @@
         # Run analysis (and re-print analysis steps)
         if verbose: print('Analysis started.')
         for s, seq_step in enumerate(self.data_analysis.AnalysisStepSequence):
             if verbose: print(f'Step {s + 1}/{len(self.data_analysis.AnalysisStepSequence)}: {seq_step}')
             step = step_definitions[seq_step]  # this is the object containing the information about the current step
             if step.type == 'MakeModel':
                 self.step_make_model(step, verbose=verbose)
-            elif step.type == 'ModifyModel':                self.step_modify_model(step, verbose=verbose)
+            elif step.type == 'ModifyModel':
+                self.step_modify_model(step, verbose=verbose)
             elif step.type == 'ModifyModelMultipleVariables':
                 self.step_modify_model_multiple_variables(step, verbose=verbose)
             elif step.type == 'RunSimulation':
                 self.step_run_simulation(step, verbose=verbose)
             elif step.type == 'PostProcessCompare':
                 self.step_postprocess_compare(step, verbose=verbose)
             elif step.type == 'SetUpFolder':  # DO NOT USE THESE STEPS ANYMORE - THEY WILL BE DELETED
@@ -680,15 +682,18 @@
                 #     raise Exception(f'Key {local_tool_folder} is not found in the analysis permanent settings.')
                 # if self.data_analysis.GeneralParameters.flag_permanent_settings:
                 #     abs_tool_path = self.data_analysis.PermanentSettings.__dict__[local_tool_folder]
                 # else:
                 #     abs_tool_path = self.settings.__dict__[local_tool_folder]
                 abs_tool_path = getattr(self.settings, local_tool_folder)
                 if local_tool_folder == 'local_library_path':
-                    abs_tool_path = os.path.join(abs_tool_path, f"{self.data_analysis.AnalysisStepDefinition['makeModel'].case_model}s")
+                    for step_data in self.data_analysis.AnalysisStepDefinition.values():
+                        if step_data.type == 'MakeModel':
+                            abs_tool_path = os.path.join(abs_tool_path, f"{step_data.case_model}s")
+                            break
                 paths_out.append(str(Path(os.path.join(abs_tool_path, simulation_name, remaining_path)).resolve()))
             return paths_out
 
         for full_path_file_to_copy, full_path_file_target in zip(get_full_path(step.copy_from), get_full_path(step.copy_to)):
             print(f'Copying from: {full_path_file_to_copy}')
             print(f'Copying to: {full_path_file_target}')
             # Make sure the target folder exists
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2024.5.4/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/BuilderAPDL_CT.py` & `steam-sdk-2024.5.4/steam_sdk/builders/BuilderAPDL_CT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/BuilderCosim.py` & `steam-sdk-2024.5.4/steam_sdk/builders/BuilderCosim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2024.5.4/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2024.5.4/steam_sdk/builders/BuilderLEDET.py`

 * *Files 0% similar despite different names*

```diff
@@ -1376,23 +1376,23 @@
             elif magnet_type in ['CCT_straight']:
                 # selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
                 #                                                f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
                 # df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows = 1, header = None)
                 # self.Auxiliary.overwrite_inductance_coil_sections = float(df.to_numpy().sum())  # [:-1] to remove last nan
                 HalfTurnToInductanceBlock = []  # set to empty as it is later overwritten for CCT_straight by method self.assignCCTValuesWindings()
             elif magnet_type in ['CWS']:
-                # selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
-                #                                                f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
-                # df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows=1, header=None)
-                # self.Auxiliary.overwrite_inductance_coil_sections = df.to_numpy()  # [:-1] to remove last nan
-                # fL_I_fL_L_file = Path.joinpath(self.path_input_file,
-                #                                f'{self.model_data.GeneralParameters.magnet_name}_fL_I_fL_L_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
-                # df_fL_I_fL_L = pd.read_csv(fL_I_fL_L_file, delimiter=',', engine='python')
-                # self.setAttribute(self.Inputs, 'fL_I', df_fL_I_fL_L['fL_I'].to_numpy())
-                # self.setAttribute(self.Inputs, 'fL_L', df_fL_I_fL_L['fL_L'].to_numpy())
+                selfMutualInductanceMatrix_csv = Path.joinpath(self.path_input_file,
+                                                               f'{self.model_data.GeneralParameters.magnet_name}_selfMutualInductanceMatrix_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
+                df = pd.read_csv(selfMutualInductanceMatrix_csv, delimiter=',', engine='python', skiprows=1, header=None)
+                self.Auxiliary.overwrite_inductance_coil_sections = df.to_numpy()  # [:-1] to remove last nan
+                fL_I_fL_L_file = Path.joinpath(self.path_input_file,
+                                               f'{self.model_data.GeneralParameters.magnet_name}_fL_I_fL_L_{str(self.model_data.Options_LEDET.input_generation_options.selfMutualInductanceFileNumber)}.csv')
+                df_fL_I_fL_L = pd.read_csv(fL_I_fL_L_file, delimiter=',', engine='python')
+                self.setAttribute(self.Inputs, 'fL_I', df_fL_I_fL_L['fL_I'].to_numpy())
+                self.setAttribute(self.Inputs, 'fL_L', df_fL_I_fL_L['fL_L'].to_numpy())
                 HalfTurnToInductanceBlock = []  # set to empty as it is later overwritten
             else:
                 raise Exception(f'Magnet type not recognized: {magnet_type}.')
 
         # Self-mutual inductances between coil sections, per unit length [H/m]
         self.setAttribute(self.Inputs, 'M_m', self.Auxiliary.overwrite_inductance_coil_sections)
         self.setAttribute(self.Inputs, 'HalfTurnToInductanceBlock', HalfTurnToInductanceBlock)
@@ -1545,15 +1545,15 @@
         list_of_attr_names = [
             'nT',
             'nStrands_inGroup',
             'GroupToCoilSection',
             'polarities_inGroup',
             'l_mag_inGroup',
             'HalfTurnToInductanceBlock',
-            'M_InductanceBlock_m'
+            'M_InductanceBlock_m'       # set this to M_m to avoid reading it from file by LEDET, (this overwrites zero set in setSelfMutualInductances method)
         ]
         list_of_attr_values = [
             np.array(nT, np.int32),
             np.ones_like(nT, np.int32),
             np.array(list(range(len(nT))))+1,   # set each group to belong to new coil section +1 as it needs to be 1 based
             np.ones_like(nT, np.int32),
             np.ones_like(nT, np.int32) * self.model_data.GeneralParameters.magnetic_length,
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2024.5.4/steam_sdk/builders/BuilderModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,15 +478,15 @@
                     # TODO: geometry when conductor has a combination of ribbon and non-ribbon cables
 
                     # List of flags that are True is the cable type is "Ribbon"
                     list_flag_ribbon = []
                     for i, cond in enumerate(self.model_data.CoilWindings.conductor_to_group):
                         list_flag_ribbon.append(self.model_data.Conductors[cond - 1].cable.type == 'Ribbon')
 
-                    nT_from_original_map2d, nStrands_inGroup_original_map2d, _, _, _, _, _, _ =\
+                    nT_from_original_map2d, nStrands_inGroup_original_map2d, _, _, _, _, _, _, _, _ =\
                         ParserMap2dFile(map2dFile=self.path_map2d).getParametersFromMap2d(headerLines=self.model_data.Options_LEDET.field_map_files.headerLines)
 
                     n_groups_original_file = len(nT_from_original_map2d)
                     geometry_ribbon_cable = []
 
                     for i in range(n_groups_original_file):
                         list = [None, None]
@@ -800,15 +800,15 @@
                 # Add for each magnet the corresponding Lmag and C_ground to the netlist parameters in the format 'Lmag' = 'Lmag_x_Magnet_1'
                 self.circuit_data.Netlist[key].parameters['L_mag']= f'L_mag_{key}'
                 self.circuit_data.Netlist[key].parameters['C_ground'] = f'C_ground_{key}'
                 self.circuit_data.Netlist[key].parameters['Field_interp_value'] = f'Field_interp_value_{key}'
                 for flag in TFM.__dict__.keys():
                     if flag != 'Magnets':
                         # Add for each magnet the corresponding flags to the netlist parameters in the format  'flag_PC' = 'flag_PC'
-                        if flag != 'M_CB_Wedges' or (flag == 'M_CB_Wedges' and TFM.M_CB_Wedges):
+                        if flag != 'M_CB_Wedge' or (flag == 'M_CB_Wedge' and TFM.M_CB_Wedge):
                             self.circuit_data.Netlist[key].parameters[flag] = flag
 
         # Write output .cir file
         parser_xyce = ParserXYCE(circuit_data=self.circuit_data, path_input=self.path_input_file, output_path=output_path)
         path_file_name = os.path.join(output_path, f'{sim_name}{sim_suffix}.cir')  # full path of the XYCE netlist to write
         parser_xyce.write2XYCE(path_file_name, flag_resolve_library_paths=True, flag_copy_additional_files=True, verbose=verbose)
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2024.5.4/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2024.5.4/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/BuilderPySIGMA.py` & `steam-sdk-2024.5.4/steam_sdk/builders/BuilderPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/BuilderTFM.py` & `steam-sdk-2024.5.4/steam_sdk/builders/BuilderTFM.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from steam_sdk.data.DataTFM import General
 from steam_sdk.data.DataTFM import HalfTurns
 from steam_sdk.data.DataTFM import Strands
 from steam_sdk.data.DataTFM import PC
 from steam_sdk.data.DataTFM import Options
 from steam_sdk.data.DataTFM import IFCC
 from steam_sdk.data.DataTFM import ISCC
-from steam_sdk.data.DataTFM import EC_CopperSheath
-from steam_sdk.data.DataTFM import Wedges
-from steam_sdk.data.DataTFM import ColdBore
+from steam_sdk.data.DataTFM import ED
+from steam_sdk.data.DataTFM import Wedge
+from steam_sdk.data.DataTFM import CB
 from steammaterials.STEAM_materials import STEAM_materials
 matpath: str = os.path.dirname(steammaterials.__file__)
 import matplotlib.pyplot as plt
 import time
 
 class BuilderTFM:
     """
@@ -43,32 +43,32 @@
             :param f_mag: field-factor for each strand
             :param f_mag_X: field-factor for each strand along X axis
             :param f_mag_Y: field-factor for each strand along Y axis
             :param output_path: path to save the generated lib file
             :param flag_Roxie: if True it uses the field-factors calculated from Roxie, else it uses the field-factors provided as parameter
             :param flag_IFCC: if True includes the Inter Filament Coupling Current effect
             :param flag_ISCC: if True includes the Inter Strands Coupling Current effect
-            :param flag_Wedges: if True includes the Wedges effect
-            :param flag_ColdBore: if True includes the Cold Bore effect
-            :param flag_EC: if True includes the Eddy Currents effect in the Copper Sheath
+            :param flag_Wedge: if True includes the Wedge effect
+            :param flag_CB: if True includes the Cold Bore effect
+            :param flag_ED: if True includes the Eddy Currents effect in the Copper Sheath
         """
         # TODO I_magnet
         # TODO lib_path
         # TODO hard coded path to steam models
         # Data structures
         self.General = General()
         self.HalfTurns = HalfTurns()
         self.Strands = Strands()
         self.Options = Options()
         self.PC = PC()
         self.IFCC = IFCC()
         self.ISCC = ISCC()
-        self.EC_CopperSheath = EC_CopperSheath()
-        self.Wedges = Wedges()
-        self.ColdBore = ColdBore()
+        self.ED = ED()
+        self.Wedge = Wedge()
+        self.CB = CB()
         self.magnet_name = Magnet_data.name
         self.path_input_file = path_input_file
 
         if flag_build:
             if not builder_LEDET or not self.magnet_name:
                  raise Exception('Cannot build model without providing BuilderLEDET object with Inputs dataclass and magnet_name')
 
@@ -76,24 +76,24 @@
             LedetInputs = asdict(builder_LEDET.Inputs)
             self.LedetInputs = LedetInputs
             self.LedetAuxiliary = builder_LEDET.Auxiliary
             self.LedetOptions = builder_LEDET.Options
             self.TFM_inputs = TFM_inputs
             self.Magnet_data = Magnet_data
 
-            self.M_CB_Wedges = TFM_inputs.M_CB_Wedges
+            self.M_CB_Wedge = TFM_inputs.M_CB_Wedge
             self.T = TFM_inputs.T
             self.Field_interp_value = Magnet_data.Field_interp_value
 
             # TODO: HardCoded values
             self.General.I_magnet = 1
             self.General.lib_path = f"D:\\Code_new\\steam_analyses\\mbrd_tfm\\local_library\\lib\\{magnet_name}_TFM_General.lib"
             # self.General.path_input_file = f"D:\\Code_new\\\steam_analyses\\mbrd_tfm\\local_library\\magnets\\{magnet_name}\\input"
             self.General.path_input_file = f"D:\\Code_new\\\steam_sdk\\tests\\builders\\model_library\\magnets\\{magnet_name}\\input"
-            self.Wedges.RRR_wedges = np.array([50])
+            self.Wedge.RRR_Wedge = np.array([50])
 
             self.conductor_to_group = np.array(builder_LEDET.model_data.CoilWindings.conductor_to_group)
 
             self.translateModelDataToTFMGeneral()
             self.translateModelDataToTFMHalfTurns()
             self.translateModelDataToTFMStrands()
             self.setOptions()
@@ -159,25 +159,24 @@
         self.setAttribute(self.Strands, 'strands_to_conductor', strands_to_conductor)
         for keyLedetData, value in self.LedetInputs.items():
             keyTFM = lookupModelDataToTFMStrands(keyLedetData)
             if keyTFM in self.Strands.__annotations__:
                 repeated_value = np.repeat(value[self.HalfTurns.HalfTurns_to_group - 1], self.HalfTurns.n_strands)
                 self.setAttribute(self.Strands, keyTFM, repeated_value)
 
-    def setOptions(self, flag_PC: bool = False, flag_IFCC: bool = False, flag_ISCC: bool = False,
-                   flag_Wedges: bool = False, flag_ColdBore: bool = False, flag_EC: bool = False, flag_BS: bool = False):
+    def setOptions(self):
         """
             This function sets to the Option DataClass the flags fto know which effects should be included in the magnet model
 
             :param flag_PC: if True includes the Persistent Current effect
             :param flag_IFCC: if True includes the Inter Filament Coupling Current effect
             :param flag_ISCC: if True includes the Inter Strands Coupling Current effect
-            :param flag_Wedges: if True includes the Wedges effect
-            :param flag_ColdBore: if True includes the Cold Bore effect
-            :param flag_EC: if True includes the Eddy Currents effect in the Copper Sheath
+            :param flag_Wedge: if True includes the Wedge effect
+            :param flag_CB: if True includes the Cold Bore effect
+            :param flag_ED: if True includes the Eddy Currents effect in the Copper Sheath
         """
         if self.T < min(self.LedetInputs['Tc0_NbTi_ht_inGroup']):
             flag_SC = True
         else:
             flag_SC = False
         self.setAttribute(self.Options, 'flag_SC', flag_SC)
 
@@ -189,32 +188,46 @@
     def calculate_field_contributions(self):
         '''
         Calculates the field in each filament of the MB magnet - ROXIE Edition
         This function returns the calculated field contributions from ROXIE for the magnet
         '''
         ## Field in all filaments when fully powering the magnet
 
-        if self.Options.flag_Roxie:
-            f_mag, f_mag_X_all, f_mag_Y_all = self.retrieve_field_contributions_Roxie()
-        else:
-            f_mag, f_mag_X_all, f_mag_Y_all = self.retrieve_field_contributions_COMSOL(value=self.Field_interp_value, flag_BS=self.Options.flag_BS)
 
-        self.setAttribute(self.Strands, 'f_mag_X', f_mag_X_all)
-        self.setAttribute(self.Strands, 'f_mag_Y', f_mag_Y_all)
-        self.setAttribute(self.Strands, 'f_mag', f_mag)
+        f_mag_Roxie, f_mag_X_Roxie, f_mag_Y_Roxie = self.retrieve_field_contributions_Roxie()
+
+        local_library_path = os.path.join(Path(self.General.path_input_file).resolve(), 'TFM_input')
+        name = self.General.magnet_name
+        mapping = np.vectorize(lambda t: complex(t.replace('i', 'j')))
+
+        full_file_Comsol = Path(os.path.join(local_library_path, f'Field_Map_{name}.csv')).resolve()
+        df_Comsol = pd.read_csv(full_file_Comsol, header=None, dtype=str, na_filter=False)
+        frequency = np.array(df_Comsol.iloc[1, 2::2]).astype(float)
+        df_Comsol = mapping(df_Comsol.values[2:, 2:]).T
+        f_mag_X_Comsol = np.sqrt(np.real(df_Comsol[::2, :] * np.conjugate(df_Comsol[::2, :]))) * np.sign(f_mag_X_Roxie)
+        f_mag_Y_Comsol = np.sqrt(np.real(df_Comsol[1::2, :] * np.conjugate(df_Comsol[1::2, :]))) * np.sign(f_mag_Y_Roxie)
+        f_mag_Comsol = np.sqrt(f_mag_X_Comsol ** 2 + f_mag_Y_Comsol ** 2)
+
+        self.frequency = frequency
+
+        self.setAttribute(self.Strands, 'f_mag_X_Roxie', f_mag_X_Roxie)
+        self.setAttribute(self.Strands, 'f_mag_Y_Roxie', f_mag_Y_Roxie)
+        self.setAttribute(self.Strands, 'f_mag_Roxie', f_mag_Roxie)
+        self.setAttribute(self.Strands, 'f_mag_X_Comsol', f_mag_X_Comsol)
+        self.setAttribute(self.Strands, 'f_mag_Y_Comsol', f_mag_Y_Comsol)
+        self.setAttribute(self.Strands, 'f_mag_Comsol', f_mag_Comsol)
 
 
-    def calculate_PC(self, frequency: np.ndarray, T: float, fMag: np.ndarray):
+    def calculate_PC(self, frequency: np.ndarray, T: float, fMag: np.ndarray, flag_coupling:bool = True, flag_save:bool=False) -> np.ndarray:
         '''
         Function that calculates the equivalent circuit parameter for the persistent currents and save them to the
         PC dataclass
 
         :param frequency: Frequency vector
         :param T: temperature vector, to be used in the interaction with Eddy-currents
-        :param flag_Roxie: if True it uses f_mag calculated from Roxie, else it uses the f_mag provided as parameter
         :param f_mag: field-factor for each strand
         '''
 
         l_magnet = self.General.magnet_length
         ds_filamentary = self.Strands.d_filamentary
         dws = self.Strands.diameter
         strands_to_conductor = self.Strands.strands_to_conductor
@@ -229,16 +242,19 @@
 
         B = self.General.I_magnet*fMag
         rho_el_0 = self.rhoCu_nist(T=T, RRR=RRR, B=B[0, :])
 
         tb_strand = dws - ds_filamentary
 
         # Calculate the equivalent circuit parameter
-        tau_ed = mu0 / 2 * (ds_filamentary / 2 * tb_strand / 2) / rho_el_0
-        alpha2 = 1 / np.sqrt(np.sqrt((1 + (w * tau_ed) ** 2)))
+        tau_ed = mu0 / 2 * (dws / 2 * tb_strand / 2) / rho_el_0
+        if flag_coupling:
+            alpha2 = 1 / np.sqrt(np.sqrt((1 + (w * tau_ed) ** 2)))
+        else:
+            alpha2 = np.ones(w.shape)
 
         M_temp = (np.pi / 4 * l_magnet * ds_filamentary * fMag * alpha2) ** 2
         Lm = np.array([mu0 * np.pi / 4 * l_magnet] * len(frequency))
         M_if_Pc = mu0 * np.pi / 8 * l_magnet
         I_Pc = np.array([0, 0])
 
         idx_valid = np.where(strands_to_CS - 1 < strands_to_CS / 2)[0]
@@ -248,35 +264,36 @@
         STC_repeated = np.tile(strands_to_conductor, len(frequency))
         STC_pc = np.reshape(STC_repeated, (len(frequency), n_strands), order='F')
 
         L_pc = np.squeeze(L_pc[:, idx_valid])
         STC_pc = np.squeeze(STC_pc[:, idx_valid])
         M_temp = np.squeeze(M_temp[:, idx_valid])
 
-        L_bin, R_bin, M_bin = bin_components(frequency=frequency, L=L_pc, R=STC_pc, M=M_temp, bins=bins, sort_on="R")
+        L_bin, R_bin, M_bin = bin_components(frequency=frequency, L=L_pc, R=STC_pc, M=M_temp, bins=bins, sort_on='R', flag_PC=True)
 
-
-        self.setAttribute(self.PC, 'M', M_bin)
-        self.setAttribute(self.PC, 'I', I_Pc)
-        self.setAttribute(self.PC, 'L', L_bin)
-        self.setAttribute(self.PC, 'M_IF_PC', M_if_Pc)
+        if flag_save:
+            self.setAttribute(self.PC, 'M', M_bin)
+            self.setAttribute(self.PC, 'I', I_Pc)
+            self.setAttribute(self.PC, 'L', L_bin)
+            self.setAttribute(self.PC, 'M_IF_PC', M_if_Pc)
+        else:
+            return L_bin, I_Pc, M_bin
 
 
-    def calculate_IFCC(self, frequency: np.ndarray, T: float, fMag: np.ndarray) -> np.ndarray:
+    def calculate_IFCC(self, frequency: np.ndarray, T: float, fMag: np.ndarray, flag_coupling: bool = True, flag_save: bool = False) -> np.ndarray:
         '''
-        Calculates the equivalent IFCC coupling loops for a given temperature and field
+        Calculates the equivalent IFCL coupling loops for a given temperature and field
 
         :param frequency: Frequency vector
         :param T: temperature vector
-        :param flag_Roxie: if True it uses f_mag calculated from Roxie, else it uses the f_mag provided as parameter
         :param f_mag: field-factor for each strand
         '''
 
         w = 2 * np.pi * frequency.reshape(len(frequency), 1)
-        mu0 = 4 * np.pi / 10 ** 7 # TODO - This factor has to be verified  0.364721485) fsc
+        mu0 = 4 * np.pi / 10 ** 7
         mu0_eff = 4 * np.pi / 10 ** 7
 
         # Setting all required parameters for the MB magnet
         f_ro_eff = self.Strands.f_rho_effective
         l_mag = self.General.magnet_length
         dws = self.Strands.diameter
         ds_filamentary = self.Strands.d_filamentary
@@ -290,53 +307,65 @@
         rho_el_0 = self.rhoCu_nist(T=T, RRR=RRR*f_ro_eff, B=B[0, :]) + 1e-12
         rho_el_Outer = self.rhoCu_nist(T=T, RRR=RRR, B=B[0, :]) + 1e-12
 
         idx_valid = np.where(strands_to_CS - 1 < strands_to_CS / 2)[0]
 
         # Calculating the coupled loop equivalent parameter
         beta_if = (Lp_f / (2 * np.pi)) ** 2 * 1 / (rho_el_0)
-        tau_if = mu0 / 2 * beta_if
+        tau_if = mu0_eff / 2 * beta_if
 
         tb_strand = dws - ds_filamentary
-        tau_ed = mu0 / 2 * (ds_filamentary / 2 * tb_strand / 2) / rho_el_Outer
-        alpha = 1 / np.sqrt((1 + (w * (tau_if+tau_ed)) ** 2))
-        dB = w * fMag * alpha
+        tau_ed = mu0 / 2 * ((dws / 2) * (tb_strand / 2)) / rho_el_Outer
+        if flag_coupling:
+            alpha2 = 1 / np.sqrt((1 + (w * (tau_ed)) ** 2))
+        else:
+            alpha2 = np.ones(w.shape)
+        alpha = 1 / np.sqrt((1 + (w * (tau_if)) ** 2))
+        dB = w * fMag * alpha * alpha2
 
         # Standard method
         I_if = beta_if * ds_filamentary * dB
         P_if = tau_if / (2 * mu0_eff) * ds_filamentary ** 2 * np.pi * l_mag * dB ** 2
         # Power formula proposed in Arjans thesis - not working in XYCE
         # I_if = np.sqrt(np.pi / (2*w)) * beta_if * dS * dB
         # P_if = 2*dS**2*l_mag*np.pi/4*(2*tau_if*np.pi*w)/mu0*(f_mag*alpha)**2
-        R_if = P_if / I_if ** 2
+
+        I_tot_im = I_if * alpha
+        I_tot_re = I_if * alpha * w * tau_if
+        # I_tot_re = np.sqrt(I_if ** 2 - I_tot_im ** 2)
+        I_if = I_tot_re + 1j * I_tot_im
+
+        R_if = P_if / np.real((I_if * np.conjugate(I_if)))
         L_if = np.ones((len(frequency), 1)) * tau_if * R_if[0, :]
         M_if = (1j * w.reshape(len(frequency), 1) * L_if * I_if + I_if * R_if) / (1j * w.reshape(len(frequency), 1) * 1)
-        M_if = np.sqrt(np.real(M_if) ** 2 + np.imag(M_if) ** 2)
-
+        # M_if = np.sqrt(np.real(M_if) ** 2 + np.imag(M_if) ** 2)
 
         R_if = np.squeeze(R_if[:, idx_valid])
         L_if = np.squeeze(L_if[:, idx_valid])
-        M_if = np.squeeze(M_if[:, idx_valid]) ** 2
+        M_if = np.squeeze(M_if[:, idx_valid])
+        I_if = np.squeeze(I_if[:, idx_valid])
 
+        L_if_bin, R_if_bin, M_if_bin, I_if_bin = bin_components(frequency, L_if, R_if, M_if,  sort_on='R', bins=bins, I=I_if)
 
-        L_if_bin, R_if_bin, M_if_bin = bin_components(frequency, L_if, R_if, M_if, bins=bins)
-        self.setAttribute(self.IFCC, 'M', M_if_bin)
-        self.setAttribute(self.IFCC, 'R', R_if_bin)
-        self.setAttribute(self.IFCC, 'L', L_if_bin)
-        self.setAttribute(self.IFCC, 'P', P_if)
-        self.setAttribute(self.IFCC, 'tau', tau_if)
+        if flag_save:
+            self.setAttribute(self.IFCC, 'M', M_if_bin)
+            self.setAttribute(self.IFCC, 'R', R_if_bin)
+            self.setAttribute(self.IFCC, 'L', L_if_bin)
+            self.setAttribute(self.IFCC, 'P', P_if)
+            self.setAttribute(self.IFCC, 'tau', tau_if)
+        else:
+            return L_if_bin, R_if_bin, M_if_bin
 
 
-    def calculate_ISCC(self, frequency: np.ndarray, T: float, fMag_X: np.ndarray, fMag_Y: np.ndarray) -> np.ndarray:
+    def calculate_ISCC(self, frequency: np.ndarray, T: float, fMag_X: np.ndarray, fMag_Y: np.ndarray, flag_save: bool = False) -> np.ndarray:
         '''
-        Function that calculates the power loss and induced currents by ISCC and derives the equivalent circuit parameter
+        Function that calculates the power loss and induced currents by ISCL and derives the equivalent circuit parameter
 
         :param frequency: Frequency vector
         :param T: temperature vector
-        :param flag_Roxie: if True it uses f_mag calculated from Roxie, else it uses the f_mag provided as parameter
         :param f_mag_X_all: field-factor along X axis for each strand
         :param f_mag_Y_all: field-factor along Y axis for each strand
 
         :return f_mag_X_return: return field-factor along X axis for each strand
         :return f_mag_Y_all: return field-factor along Y axis for each strand
         '''
         f = frequency
@@ -358,300 +387,292 @@
         Nc = self.HalfTurns.Nc
         C = self.HalfTurns.C_strand
         R_c = self.HalfTurns.Rc
         HalfTurns_to_CS = self.HalfTurns.HalfTurns_to_coil_sections
         RRR = self.HalfTurns.RRR
         f_ro_eff = self.HalfTurns.f_rho_effective
 
-
-        alphas = np.pi / 2 * mirror_block / 2 - (mirror_block - 1) * alphasRAD - rotation_block / 180 * np.pi
-        alphas = np.repeat(alphas, n_strands)
+        alphas = np.repeat((np.pi/2 * mirror_block/2 - (mirror_block - 1) * alphasRAD - rotation_block/180 * np.pi), n_strands)
         f_magPerp = np.transpose(-fMag_X * np.sin(alphas) + fMag_Y * np.cos(alphas))
         r_magPerp = np.transpose(fMag_X * np.cos(alphas) + fMag_Y * np.sin(alphas))
         B_temp = np.sqrt(fMag_X ** 2 + fMag_Y ** 2).T
 
         ## Reverse action:
         ## fMag_X = r_magPerp.T*np.cos(alphas)-f_magPerp.T*np.sin(alphas)
         ## fMag_Y = r_magPerp.T*np.sin(alphas)+f_magPerp.T*np.cos(alphas)
 
         f_magPerp_ht = np.zeros((self.General.num_HalfTurns, len(frequency)))
         r_magPerp_ht = np.zeros((self.General.num_HalfTurns, len(frequency)))
         alphas_ht = np.zeros((self.General.num_HalfTurns, 1))
         B_ht = np.zeros((self.General.num_HalfTurns, len(frequency)))
         tempS = 0
         for i in range(len(n_strands)):
-            f_magPerp_ht[i] = np.average(f_magPerp[tempS:tempS + n_strands[i]], axis=0)
-            r_magPerp_ht[i] = np.average(r_magPerp[tempS:tempS + n_strands[i]], axis=0)
+            f_magPerp_ht[i] = np.average(f_magPerp[tempS:tempS + n_strands[i], :], axis=0)
+            r_magPerp_ht[i] = np.average(r_magPerp[tempS:tempS + n_strands[i], :], axis=0)
             alphas_ht[i] = np.average(alphas[tempS:tempS + n_strands[i]])
-            B_ht[i] = np.average(B_temp[tempS:tempS + n_strands[i]], axis=0)
+            B_ht[i] = np.average(B_temp[tempS:tempS + n_strands[i], :], axis=0)
             tempS = tempS + n_strands[i]
 
         alpha_c = wBare / hBare
         idx_valid = np.where(HalfTurns_to_CS - 1 < HalfTurns_to_CS / 2)[0]
 
         rho_el_Outer = self.rhoCu_nist(T=T, B=B_ht[:, 0], RRR=RRR*f_ro_eff) + 1e-12
-        rho_C_Strands = R_c / (rho_el_Outer * (n_strands ** 2 - n_strands) / (2 * Lp_s * alpha_c))
+        rho_C_Strands = R_c / (rho_el_Outer * (n_strands ** 2 - n_strands) / (2 * Lp_s * alpha_c)) #Eq. 4.33 in Arjans Thesis p. 78
 
         #  Calculating the equivalent circuit parameter
         beta_is = 1 / 120 * Lp_s / R_c * n_strands * (n_strands - 1) * wBare / hBare
-        tau_is = mu0*beta_is
+        tau_is = mu0 * beta_is
         factor_tau = alpha_c * Nc / (alpha_c + C * (Nc - 1))  # Eq. 4.41 in Arjans Thesis p.89
         # tau_is = 1.65e-08 * (Lp_s * (n_strands ** 2 - 4 * n_strands)) / R_c * factor_tau  # Eq. 4.31 in Arjans Thesis p.78
 
         alpha = 1 / np.sqrt((1 + (w * tau_is) ** 2))
-        dB = w * f_magPerp_ht.T * alpha
+        dB = w * abs(f_magPerp_ht.T) * alpha
 
         P_is = l_mag * beta_is * dB ** 2 * wBare * hBare
         I_is = beta_is * hBare * dB
 
+        I_tot_im = I_is * alpha
+        I_tot_re = I_is * alpha * w * tau_is
+        #I_tot_re = np.sqrt(I_is ** 2 - I_tot_im ** 2)
+        I_is = I_tot_re + 1j * I_tot_im
+
         # Calculate equivalent parameter
-        R_is = P_is / I_is ** 2
+        R_is = P_is / np.real((I_is*np.conjugate(I_is)))
         L_is = np.ones((len(f), 1)) * tau_is * R_is[0, :]
         M_is = (1j * w.reshape(len(f), 1) * L_is * I_is + I_is * R_is) / (1j * w.reshape(len(f), 1) * 1)
-        M_is = np.sqrt(np.real(M_is) ** 2 + np.imag(M_is) ** 2)
+        # M_is = np.sqrt(np.real(M_is) ** 2 + np.imag(M_is) ** 2)
 
         # Calculate warm resistance of a strand-pitch
         if not self.Options.flag_SC:
             ## Add the warm part to account for ISCL in non-superconducting state
             rho_el_Outer = self.rhoCu_nist(T, B_ht[:, 0], RRR*f_ro_eff) + 1e-12
             alpha_st = np.arctan(wBare/(Lp_s/2)) #Half twist-pitch as Lp is the full length until its back at the beginning
             l_strand = 2 * wBare / np.sin(alpha_st) + 2 * hBare  # twice as we go back AND forth
             A_strand = (1 - fsc) * np.pi * (dws / 2) ** 2
             R_strand = rho_el_Outer * l_strand / A_strand
 
-            R_c_warm = 3e-3 * rho_C_Strands * rho_el_Outer * (n_strands** 2 - n_strands) / (2 * Lp_s * alpha_c)
+            R_c_warm = 2e-3 * rho_C_Strands * rho_el_Outer * (n_strands** 2 - n_strands) / (2 * Lp_s * alpha_c)
             R_c_N = R_c_warm + R_strand
-            fT = 1 / (np.log(1.9) ** 0.186) * np.log(T) ** 0.186
-            tau_is_N = 1.65e-8 * C * 1 / (2 * fT) * (Lp_s * (n_strands ** 2 - 4 * n_strands)) / R_c_N * factor_tau
-            beta_is_N = 1 / 120 * fT * Lp_s / R_c_N * n_strands * (n_strands - 1) * wBare / hBare
-
+            # fT = 1/(1.9)**0.08*T**(0.08)
+            # fT = 2*1/(np.log(1.9)**0.186)*np.log(T)**0.186
+            fT = 2.5 * 1 / (np.log(1.9) ** 0.3179) * np.log(T) ** 0.3179
+            tau_is_N = 1.65e-8 * C * 1 / (2 * fT) * (Lp_s * (n_strands ** 2 - 4 * n_strands)) / R_c_N * factor_tau  # Equation 4.31 in Arjans Thesis P.78 and Eq. 4.41
+            # beta_is_N = tau_is_N/ mu0
+            beta_is_N = 1 / 120 * fT * Lp_s / R_c_N * n_strands * (n_strands - 1) * wBare / hBare # 60 works well for 290 K
 
             ## Adjust the components again on the new time constant
             alpha = 1 / np.sqrt((1 + (w * tau_is_N) ** 2))
             dB = w * f_magPerp_ht.T * alpha
 
             P_is = l_mag * beta_is_N * dB ** 2 * wBare * hBare
             I_is = beta_is_N * hBare * dB
+            I_tot_im = I_is * alpha
+            I_tot_re = abs(I_is * alpha * w * tau_is_N)
+            I_is = I_tot_re + 1j * I_tot_im
 
             # Calculate equivalent parameter
-            R_is = P_is / I_is ** 2
+            R_is = P_is/np.real((I_is*np.conjugate(I_is)))
             L_is = np.ones((len(f), 1)) * tau_is_N * R_is[0, :]
             M_is = (1j * w.reshape(len(f), 1) * L_is * I_is + I_is * R_is) / (1j * w.reshape(len(f), 1) * 1)
-            M_is = np.sqrt(np.real(M_is) ** 2 + np.imag(M_is) ** 2)
-
-
-        R_is = np.squeeze(R_is[:, idx_valid])
-        L_is = np.squeeze(L_is[:, idx_valid])
-        M_is = np.squeeze(M_is[:, idx_valid]) ** 2
-
-
-        L, R, M = bin_components(f, L_is, R_is, M_is, bins=bins, sort_on='R')
+            # M_is = np.sqrt(np.real(M_is) ** 2 + np.imag(M_is) ** 2)
 
         # ## Calculate the return field
         # Assuming a current line on each side of the cable
         # Average distance to each strand is hence: (1/2*(dS_outer/2 + (nS/2-1)*dS_outer)), neglecting hBare
         # Twice, as we have one line on each side -> both generating the same field
-        B_return = (2 *(mu0 * I_is)/ np.pi * 1 / (1/2 * (dws/2 + (n_strands/2 - 1) * dws)))
+        B_return = (2 * (mu0 * np.abs(I_is)) / np.pi * 1 / (1 / 2 * (dws / 2 + (n_strands / 2 - 1) * dws)))
+        # dB_return = (B_return/tau_is)
 
-        # f_mag_X_return_ht = r_magPerp_ht * np.cos(alphas_ht) - B_return.T * np.sin(alphas_ht)
-        # f_mag_Y_return_ht = r_magPerp_ht * np.sin(alphas_ht) + B_return.T * np.cos(alphas_ht)
+        # f_mag_X_return_ht = r_magPerp_ht*np.cos(alphas_ht)-B_return.T*np.sin(alphas_ht)
+        # f_mag_Y_return_ht = r_magPerp_ht*np.sin(alphas_ht)+B_return.T*np.cos(alphas_ht)
         ratio_Breturn = B_return / B_ht.T
-        # f_mag_X_return = np.zeros((len(f), len(fMag_X)))
-        # f_mag_Y_return = np.zeros((len(f), len(fMag_Y)))
 
         f_mag_X_return = np.zeros((len(f), fMag_X.shape[1]))
         f_mag_Y_return = np.zeros((len(f), fMag_Y.shape[1]))
 
         tempS = 0
-        # for i in range(len(n_strands)):
-        #     f_mag_X_return[:, tempS:tempS + n_strands[i]] = f_mag_X_return[:, tempS:tempS + n_strands[i]] + f_mag_X_return_ht[
-        #         i, np.newaxis].T
-        #     f_mag_Y_return[:, tempS:tempS + n_strands[i]] = f_mag_Y_return[:, tempS:tempS + n_strands[i]] + f_mag_Y_return_ht[
-        #         i, np.newaxis].T
-        #     tempS = tempS + n_strands[i]
-
         for i in range(len(n_strands)):
             f_mag_X_return[:, tempS:tempS + n_strands[i]] = np.transpose(ratio_Breturn[:, i] * fMag_X[:, tempS:tempS + n_strands[i]].T)
             f_mag_Y_return[:, tempS:tempS + n_strands[i]] = np.transpose(ratio_Breturn[:, i] * fMag_Y[:, tempS:tempS + n_strands[i]].T)
+            # f_mag_X_return[:, tempS:tempS + nS[i]] = np.transpose(f_mag_X_all[:, tempS:tempS + nS[i]].T*0 + dB_return[:,i])
+            # f_mag_Y_return[:, tempS:tempS + nS[i]] = np.transpose(f_mag_Y_all[:, tempS:tempS + nS[i]].T*0 + dB_return[:,i])
             tempS = tempS + n_strands[i]
 
-        self.setAttribute(self.ISCC, 'M', M)
-        self.setAttribute(self.ISCC, 'R', R)
-        self.setAttribute(self.ISCC, 'L', L)
-        self.setAttribute(self.ISCC, 'P', P_is)
-        self.setAttribute(self.ISCC, 'I', I_is)
-        if not self.Options.flag_SC:
-            self.setAttribute(self.ISCC, 'tau', tau_is_N)
+        R_is = np.squeeze(R_is[:, idx_valid])
+        L_is = np.squeeze(L_is[:, idx_valid])
+        M_is = np.squeeze(M_is[:, idx_valid])
+        I_is = np.squeeze(I_is[:, idx_valid])
+        P_is = np.squeeze(P_is[:, idx_valid])
+
+        L, R, M, Iis = bin_components(f, L_is, R_is, M_is, bins=bins, I=I_is)
+        _, _, _, Pis = bin_components(f, L_is, R_is, M_is, bins=bins, I=P_is)
+        I_des = np.sqrt(Pis / R)
+        I = np.real(Iis) * I_des / abs(Iis) + 1j * np.imag(Iis) * I_des / abs(Iis)
+
+        if flag_save:
+            self.setAttribute(self.ISCC, 'M', M)
+            self.setAttribute(self.ISCC, 'R', R)
+            self.setAttribute(self.ISCC, 'L', L)
+            self.setAttribute(self.ISCC, 'P', P_is)
+            self.setAttribute(self.ISCC, 'I', I)
+            if not self.Options.flag_SC:
+                self.setAttribute(self.ISCC, 'tau', tau_is_N)
+            else:
+                self.setAttribute(self.ISCC, 'tau', tau_is)
         else:
-            self.setAttribute(self.ISCC, 'tau', tau_is)
-
-        return f_mag_X_return, f_mag_Y_return
+            return L, R, M, f_mag_X_return, f_mag_Y_return
 
 
-    def calculate_EC_CopperSheath(self, frequency: np.ndarray, T: float, fMag: np.ndarray):
+    def calculate_ED(self, frequency: np.ndarray, T: float, fMag: np.ndarray, flag_coupling: bool = True, flag_save: bool = False) -> np.ndarray:
         '''
         Calculates the equivalent coupling loops in the outer copper sheet for a given temperature and field
 
         :param frequency: Frequency vector
         :param T: temperature vector
-        :param flag_Roxie: if True it uses f_mag calculated from Roxie, else it uses the f_mag provided as parameter
         :param f_mag: field-factor for each strand
         '''
 
         f = frequency
         w = 2 * np.pi * f.reshape(len(f), 1)
 
         bins = self.General.bins
         l_mag = self.General.magnet_length
-        fsc = self.Strands.fsc
         RRR = self.Strands.RRR
-        rws = self.Strands.diameter/2
+        rws = self.Strands.diameter / 2
         strands_to_CS = self.Strands.strands_to_coil_sections
 
         if not self.Options.flag_SC:  # TODO - check if needed or not
-            r_filamentary = self.Strands.d_filamentary/2 * 0.5
+            r_filamentary = self.Strands.d_filamentary / 2 * 0.5
         else:
-            r_filamentary = self.Strands.d_filamentary/2
+            r_filamentary = self.Strands.d_filamentary / 2
 
-        if fMag.ndim == 1:
-            fMag = np.repeat(fMag[:, np.newaxis], len(frequency), axis=1).T
 
         B = self.General.I_magnet * fMag
         rho_el_0 = self.rhoCu_nist(T=T, B=B[0, :], RRR=RRR) + 1e-12
-        mu0 = 4 * np.pi / 10 ** 7 #mu0 = 4 * np.pi / 10 ** 7 / (1 - fsc)  #
+        mu0 = 4 * np.pi / 10 ** 7  # mu0 = 4 * np.pi / 10 ** 7 / (1 - fsc)  #
         tb_strand = rws - r_filamentary
         idx_valid = np.where(strands_to_CS - 1 < strands_to_CS / 2)[0]
         rho_el_0 = rho_el_0 + 1e-12
 
         # Calculating time constant, correction factor and field derivative
-        tau_ed = mu0 / 2 * (r_filamentary * tb_strand) / rho_el_0
+        tau_ed = mu0 / 2 * ((rws) * tb_strand) / rho_el_0
         # tau_ed = mu0 / 8 * dS_outer**2 / rho_el_0 ## Formula from Turck79
         alpha = 1 / np.sqrt((1 + (w * tau_ed) ** 2))
         dB = w * fMag
 
         # Skindepth
         skinDepth = np.sqrt(2 * rho_el_0 / (w * mu0))
         idx_s = np.argmin(abs(skinDepth - (1 - 1 / np.exp(1)) * tb_strand), axis=0)
 
         # Calculating the power loss
         P_DC = ((rws) ** 4 - (r_filamentary) ** 4) * np.pi / (4 * rho_el_0) * (dB * alpha) ** 2  # Derivation, not assuming twist
-        # P_DC = tau_ed/mu0 * (1-(dS_inner/dS_outer)**2) * (dB*alpha)**2 # Formula from Turck
+        # P_DC = tau_ed/mu0/2 * (1-(dS_inner/dS_outer)**2) * (dB*alpha)**2 # Formula from Turck
         # P_DC = v3 * v1v2/(v1v2+1)*beta_if*(dB*alpha)**2 # Formula from Arjan's thesis
 
-        P_AC = skinDepth ** 3 / (rho_el_0) * dB ** 2 * np.pi * (rws)  # Standard derivation
+        P_AC = skinDepth ** 3 / (2 * rho_el_0) * dB ** 2 * np.pi * (rws)  # Standard derivation
         # P_AC = dB ** 2 * skinDepth/(w*4*mu0*dS_outer) #Formula from Turck1979
 
         P_tot = np.zeros((P_DC.shape))
         for j in range(P_DC.shape[1]):
             P_t = [P_DC[:idx_s[j], j], P_AC[idx_s[j]:, j]]
             P_tot[:, j] = np.concatenate(P_t).ravel()
-        P_tot = P_tot * l_mag * 2
-
-
+        P_tot = P_tot * l_mag
         # Calculating the induced current
-        I_eq = 2 * tb_strand / (3 * rho_el_0) * (tb_strand ** 2 - 3 * tb_strand * rws + 3 * rws ** 2) * (
-                    dB * alpha)
-
+        I_tot = 2 * tb_strand / (3 * rho_el_0) * (tb_strand ** 2 - 3 * tb_strand * rws + 3 * rws ** 2) * (dB * alpha)
+        I_tot_im = I_tot * alpha
+        I_tot_re = I_tot * alpha * w * tau_ed
+        #I_tot_re = np.sqrt(I_tot ** 2 - I_tot_im ** 2)
+        I_tot = I_tot_re + 1j * I_tot_im
 
         P_tot = np.squeeze(P_tot[:, idx_valid])
-        I_ed = np.squeeze(I_eq[:, idx_valid])
+        I_ed = np.squeeze(I_tot[:, idx_valid])
         tau_ed = tau_ed[idx_valid]
 
         # Calculating the coupled loop equivalent parameter
-        R_ed = P_tot / I_ed ** 2
+        R_ed = P_tot / np.real(I_ed * np.conjugate(I_ed))
         L_ed = np.ones((len(f), 1)) * tau_ed * R_ed[0, :]
         M_ed = (1j * w * L_ed * I_ed + I_ed * R_ed) / (1j * w * 1)
-        M_ed = np.real(M_ed) ** 2 + np.imag(M_ed) ** 2
+        # M_ed = np.real(M_ed) ** 2 + np.imag(M_ed) ** 2
+
+        if not flag_coupling:
+            L, R, M, Ied = bin_components(f, L_ed, R_ed, M_ed, bins=bins, I=I_ed)
+            _, _, _, Ped = bin_components(f, L_ed, R_ed, M_ed, bins=bins, I=P_tot)
+            I_des = np.sqrt(Ped / R)
+            Ied = np.real(Ied) * I_des / abs(Ied) + 1j * np.imag(Ied) * I_des / abs(Ied)
+        else:
+            L, R, M = bin_components(f, L_ed, R_ed, M_ed, bins=bins)
 
-        L, R, M = bin_components(f, L_ed, R_ed, M_ed, bins=bins)
+        if flag_save:
+            self.setAttribute(self.ED, 'M', M)
+            self.setAttribute(self.ED, 'R', R)
+            self.setAttribute(self.ED, 'L', L)
+            self.setAttribute(self.ED, 'P', P_tot)
+            self.setAttribute(self.ED, 'I', Ied)
+            self.setAttribute(self.ED, 'tau', tau_ed)
+        else:
+            return L, R, M
 
-        self.setAttribute(self.EC_CopperSheath, 'M', M)
-        self.setAttribute(self.EC_CopperSheath, 'R', R)
-        self.setAttribute(self.EC_CopperSheath, 'L', L)
-        self.setAttribute(self.EC_CopperSheath, 'P', P_tot)
-        self.setAttribute(self.EC_CopperSheath, 'I', I_ed)
-        self.setAttribute(self.EC_CopperSheath, 'tau', tau_ed)
 
-    def calculate_Wedges(self, T: float):
+    def calculate_Wedge(self, T: float):
         '''
-        Function that calculates the equivalent parameter for eddy currents in the copper wedges
+        Function that calculates the equivalent parameter for eddy currents in the copper Wedge
         It takes the Temperature. It then calculates the resistivity and
         interpolates the current and power from pre-simulated values.
 
         '''
-        rho_W = self.rhoCu_nist(T=T, RRR=self.Wedges.RRR_wedges, B=np.array([0]))
-        P_tot, I_tot, tau_W, frequency = self.interpolate(rho=rho_W, case='Wedges')
+        rho_W = self.rhoCu_nist(T=T, RRR=self.Wedge.RRR_Wedge, B=np.array([0]))
+        P_tot, I_tot, tau_W, frequency = self.interpolate(rho=rho_W, case='Wedge')
         w = 2 * np.pi * frequency
-        P_tot = P_tot * self.General.magnet_length * 2
+        P_tot = P_tot * self.General.magnet_length
 
         # Calculating the coupled loop equivalent parameter
-        R_W = P_tot / I_tot ** 2
+        # R_W = P_tot / I_tot ** 2
+        R_W = P_tot / np.real((I_tot * np.conjugate(I_tot)))
         L_W = tau_W * R_W[0]
+        L_W = np.repeat(L_W, len(R_W))
         M_W = (1j * w * L_W * I_tot + I_tot * R_W) / (1j * w * 1)
         # M_W = np.sqrt(np.real(M_W*np.conjugate(M_W))) # Checked: is the same as the line below
-        M_W = np.sqrt(np.real(M_W) ** 2 + np.imag(M_W) ** 2)
-        M_W = np.transpose(np.ones(M_W.shape).transpose() * M_W[0])
+        # M_W = np.sqrt(np.real(M_W) ** 2 + np.imag(M_W) ** 2)
+        # M_W = np.transpose(np.ones(M_W.shape).transpose() * M_W
 
-        L_W = np.repeat(L_W, len(R_W))
 
-        self.setAttribute(self.Wedges, 'P', P_tot)
-        self.setAttribute(self.Wedges, 'I', I_tot)
-        self.setAttribute(self.Wedges, 'tau', tau_W)
-        self.setAttribute(self.Wedges, 'L', L_W)
-        self.setAttribute(self.Wedges, 'R', R_W)
-        self.setAttribute(self.Wedges, 'M', M_W)
+        self.setAttribute(self.Wedge, 'P', P_tot)
+        self.setAttribute(self.Wedge, 'I', I_tot)
+        self.setAttribute(self.Wedge, 'tau', tau_W)
+        self.setAttribute(self.Wedge, 'L', L_W)
+        self.setAttribute(self.Wedge, 'R', R_W)
+        self.setAttribute(self.Wedge, 'M', M_W)
 
-    def calculate_ColdBore(self, T: float):
+    def calculate_CB(self, T: float):
         '''
         Function that calculates the equivalent parameter for eddy currents in the cold bore.
         It takes the Temperature. It then calculates the resistivity and
         interpolates the current and power from pre-simulated values.
         '''
 
         rho_CB = self.rhoSS_nist(T=T)
-        P_tot, I_tot, tau_CB, frequency = self.interpolate(rho=rho_CB, case='ColdBore')
+        P_tot, I_tot, tau_CB, frequency = self.interpolate(rho=rho_CB, case='CB')
         w = 2 * np.pi * frequency
-        P_tot = P_tot * self.General.magnet_length #* 2
+        P_tot = P_tot * self.General.magnet_length
 
         # Calculating the coupled loop equivalent parameter
-        R_CB= P_tot / I_tot ** 2
+        # R_W = P_tot / I_tot ** 2
+        R_CB = P_tot / np.real((I_tot * np.conjugate(I_tot)))
         L_CB = tau_CB * R_CB[0]
-        M_CB = (1j * w * L_CB * I_tot + I_tot * R_CB) / (1j * w * 1)
-
-        M_CB = np.sqrt(np.real(M_CB) ** 2 + np.imag(M_CB) ** 2)
-        M_CB = np.transpose(np.ones(M_CB.shape).transpose() * M_CB[0])
-
         L_CB = np.repeat(L_CB, len(R_CB))
-        self.setAttribute(self.ColdBore, 'P', P_tot)
-        self.setAttribute(self.ColdBore, 'I', I_tot)
-        self.setAttribute(self.ColdBore, 'tau', tau_CB)
-        self.setAttribute(self.ColdBore, 'L', L_CB)
-        self.setAttribute(self.ColdBore, 'R', R_CB)
-        self.setAttribute(self.ColdBore, 'M', M_CB)
-
-    def calculate_MutualCoupling_ColdBore_Wedges(self) -> np.ndarray:
-
-        L_wedges = self.Wedges.L
-        R_wedges = self.Wedges.R
-        I_CB = 1
-
-        name = self.General.magnet_name
-        path = Path(self.General.path_input_file).resolve()
-        df_I = pd.read_csv(os.path.join(path, 'TFM_input', f'{name}_InducedCurrent_Mutual_Interpolation.csv')).dropna(axis=1)
-        frequency = df_I['f'].values
-        Re_I = df_I['Re_Jz'].values
-        Im_I = df_I['Im_Jz'].values
-        I_wedges = Re_I + 1j * Im_I
-
-        w = 2 * np.pi * frequency
-
-        M = (1j * w * I_wedges * L_wedges + I_wedges * R_wedges)/(1j * w * I_CB)
-        M_tot = np.real(np.sqrt(M * np.conjugate(M)))
-
-        return M_tot
+        M_CB = (1j * w * L_CB * I_tot + I_tot * R_CB) / (1j * w * 1)
+        # M_W = np.sqrt(np.real(M_W*np.conjugate(M_W))) # Checked: is the same as the line below
+        # M_W = np.sqrt(np.real(M_W) ** 2 + np.imag(M_W) ** 2)
+        # M_W = np.transpose(np.ones(M_W.shape).transpose() * M_W
+        self.setAttribute(self.CB, 'P', P_tot)
+        self.setAttribute(self.CB, 'I', I_tot)
+        self.setAttribute(self.CB, 'tau', tau_CB)
+        self.setAttribute(self.CB, 'L', L_CB)
+        self.setAttribute(self.CB, 'R', R_CB)
+        self.setAttribute(self.CB, 'M', M_CB)
 
 
     def interpolate(self, rho: np.ndarray, case: str) -> np.ndarray:
         '''
         Helper function that takes a CPS group and temperature, fits the respective resistivity to it and interpolates from other resistivity values
         '''
 
@@ -709,146 +730,212 @@
                 self.General.lib_path = Path(self.General.lib_path).resolve()
                 self.General.new_lib_path = Path(output_path).resolve()
 
             frequency = self.frequency
             bins = self.General.bins
             T = self.T
             f_rho_original = self.Strands.f_rho_effective
+            f_mag_Roxie= self.Strands.f_mag_Roxie
+            Mutual_dict = {}
 
             # Inter-Strands Coupling Currents
             if self.Options.flag_ISCC:
-                self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original)
-                f_mag_X_ISCC = self.Strands.f_mag_X
-                f_mag_Y_ISCC = self.Strands.f_mag_Y
-                f_mag_X_ISCC_return, f_mag_Y_ISCC_return = self.calculate_ISCC(frequency=frequency, T=T, fMag_X=f_mag_X_ISCC, fMag_Y=f_mag_Y_ISCC)
+                f_mag_X_ISCC = self.Strands.f_mag_X_Roxie
+                f_mag_Y_ISCC = self.Strands.f_mag_Y_Roxie
+                L_ISCC, R_ISCC, M_ISCC, f_mag_X_ISCC_return, f_mag_Y_ISCC_return = self.calculate_ISCC(frequency=frequency, T=T, fMag_X=f_mag_X_ISCC, fMag_Y=f_mag_Y_ISCC, flag_save=False)
+                self.calculate_ISCC(frequency=frequency, T=T, fMag_X=f_mag_X_ISCC, fMag_Y=f_mag_Y_ISCC, flag_save=True)
                 self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'ISCC', frequency, self.ISCC.L, self.ISCC.R, self.ISCC.M, bins=bins,
                                                  force_new_name=self.General.new_lib_path)
 
             # Persistent currents and magnetization
             if self.Options.flag_PC:
-                if not self.Options.flag_ISCC:
-                    f_mag_PC = self.Strands.f_mag
-                else:
-                    f_mag_PC = np.maximum(self.Strands.f_mag - np.sqrt(f_mag_X_ISCC_return ** 2 + f_mag_Y_ISCC_return ** 2), 1e-12)
                 self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original)
-                self.calculate_PC(frequency=frequency, T=T, fMag=f_mag_PC)
+                if self.Options.flag_ISCC:
+                    f_mag_PC = np.maximum(f_mag_Roxie - np.sqrt(f_mag_X_ISCC_return ** 2 + f_mag_Y_ISCC_return ** 2), 1e-12)
+                    L_PC_ISCC, I_PC_ISCC, M_PC_ISCC = self.calculate_PC(frequency=frequency, T=T, fMag=f_mag_PC, flag_coupling=False, flag_save=False)
+                    Mutual_dict['M_PC_ISCC'] = M_PC_ISCC
+                if self.Options.flag_ED:
+                    L_PC_ED, I_PC_ED, M_PC_ED = self.calculate_PC(frequency=frequency, T=T, fMag=f_mag_Roxie, flag_coupling=True, flag_save=False)
+                    Mutual_dict['M_PC_ED'] = M_PC_ED
+                self.calculate_PC(frequency=frequency, T=T, fMag=f_mag_Roxie, flag_coupling=False, flag_save=True)
                 self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'PC', frequency, self.PC.L, np.array([]), self.PC.M, bins=bins,
                                                  force_new_name=self.General.new_lib_path)
 
             # Inter-Filament Coupling Currents
-            if self.Options.flag_IFCC:  #Change rho_eff to 0.3
-                if not self.Options.flag_ISCC:
-                    f_mag_IFCC = self.Strands.f_mag
-                else:
-                    f_mag_IFCC = np.maximum(self.Strands.f_mag - np.sqrt(f_mag_X_ISCC_return ** 2 + f_mag_Y_ISCC_return ** 2), 1e-12)
-
-                self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original*0.3)
-                self.calculate_IFCC(frequency=frequency, T=T, fMag=f_mag_IFCC)
+            if self.Options.flag_IFCC:
+                self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original*0.3)#Change rho_eff to 0.6
+                if self.Options.flag_ISCC:
+                    f_mag_IFCC = np.maximum(f_mag_Roxie - np.sqrt(f_mag_X_ISCC_return ** 2 + f_mag_Y_ISCC_return ** 2), 1e-12)
+                    L_IFCC_ISCC, R_IFCC_ISCC, M_IFCC_ISCC = self.calculate_IFCC(frequency=frequency, T=T, fMag=f_mag_IFCC, flag_coupling=False, flag_save=False)
+                    Mutual_dict['M_IFCC_ISCC'] = M_IFCC_ISCC
+                if self.Options.flag_ED:
+                    L_IFCC_ED, R_IFCC_ED, M_IFCC_ED = self.calculate_IFCC(frequency=frequency, T=T, fMag=f_mag_Roxie, flag_coupling=True, flag_save=False)
+                    Mutual_dict['M_IFCC_ED'] = M_IFCC_ED
+                self.calculate_IFCC(frequency=frequency, T=T, fMag=f_mag_Roxie, flag_coupling=False, flag_save=True)
                 self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'IFCC', frequency, self.IFCC.L, self.IFCC.R, self.IFCC.M, bins=bins,
                                                  force_new_name=self.General.new_lib_path)
 
             # Eddy currents in the copper sheath
-            if self.Options.flag_EC:
-                f_mag_EC = self.Strands.f_mag
+            if self.Options.flag_ED:
                 self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original)
-                self.calculate_EC_CopperSheath(frequency=frequency, T=T, fMag=f_mag_EC)
-                self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'EC', frequency, self.EC_CopperSheath.L, self.EC_CopperSheath.R, self.EC_CopperSheath.M, bins=bins,
+                if self.Options.flag_ISCC:
+                    f_mag_ED = np.maximum(f_mag_Roxie - np.sqrt(f_mag_X_ISCC_return ** 2 + f_mag_Y_ISCC_return ** 2), 1e-12)
+                    L_ED_ISCC, R_ED_ISCC, M_ED_ISCC = self.calculate_ED(frequency=frequency, T=T, fMag=f_mag_ED, flag_coupling=True, flag_save=False)
+                    Mutual_dict['M_ED_ISCC'] = M_ED_ISCC
+
+                self.calculate_ED(frequency=frequency, T=T, fMag=f_mag_Roxie, flag_coupling=False, flag_save=True)
+                self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'ED', frequency, self.ED.L, self.ED.R, self.ED.M, bins=bins,
                                                  force_new_name=self.General.new_lib_path)
 
-            if self.Options.flag_Wedges:
-                self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original)
-                self.calculate_Wedges(T=T)
-                self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'Wedges', frequency, self.Wedges.L, self.Wedges.R, self.Wedges.M, bins=bins,
+            if self.Options.flag_Wedge:
+                self.calculate_Wedge(T=T)
+                self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'Wedge', frequency, self.Wedge.L, self.Wedge.R, self.Wedge.M, bins=bins,
                                                               force_new_name=self.General.new_lib_path)
+                M_W = self.calculate_Coupling_Components(Effect='Wedge')
+                Mutual_dict.update(M_W)
 
-            if self.Options.flag_ColdBore:
-                self.setAttribute(self.Strands, 'f_rho_effective', f_rho_original)
-                self.calculate_ColdBore(T=T)
-                self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'ColdBore', frequency, self.ColdBore.L, self.ColdBore.R, self.ColdBore.M, bins=bins,
+            if self.Options.flag_CB:
+                self.calculate_CB(T=T)
+                self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'CB', frequency, self.CB.L, self.CB.R, self.CB.M, bins=bins,
                                                               force_new_name=self.General.new_lib_path)
+                M_CB = self.calculate_Coupling_Components(Effect='CB')
+                Mutual_dict.update(M_CB)
 
-            if self.M_CB_Wedges is not None:
-                self.General.lib_path = change_library_MutualCoupling(self.General.lib_path, 'M_Wedges_ColdBore',[1, 1e5], [self.M_CB_Wedges,self.M_CB_Wedges])
-                # self.General.lib_path = change_library_MutualCoupling(self.General.lib_path, 'M_Wedges_ColdBore',
-                #                                                       frequency, M_Wedges_ColdBore)
-
+            if len(Mutual_dict) != 0:
+                self.calculate_Mutual_Coupling(Mutual_dict)
 
-            attributes = [value for attr, value in vars(self.Options).items() if (attr != 'flag_SC' and attr != 'flag_Roxie' and attr != 'flag_BS')]
+            attributes = [value for attr, value in vars(self.Options).items() if (attr != 'flag_SC' and attr != 'flag_BS')]
 
             # Check if all the flags of the effects in the Option class are True, in that case it means that the inductance matrix needs to be checked
             if all(value for value in attributes):
-                self.check_inductance_matrix()
+                self.check_inductance_matrix_losses(Mutual_dict)
 
             # Check if all the flags of the effects in the Option class are False, in that case it means that no lib file has been generated yet,
             # but since the Output path is not None we still need to generate it
             if all(not value for value in attributes):
                 # The value to be sent to change_library_EqLoop needs to have the as .shape[1] the number of bins
                 value = np.zeros((1, self.General.bins))
                 self.General.lib_path = change_library_EqLoop(self.General.lib_path, 'ABC', value, value, value, value, bins=bins, force_new_name=self.General.new_lib_path)
 
 
-    def retrieve_field_contributions_COMSOL(self, value: float = None,  flag_BS: bool = False) -> np.ndarray:
+    def calculate_Mutual_Coupling(self, Mutual_dict: dict):
+        ''' This function calculates the Mutual Coupling between two different efefcts, starting from the M_coupled dictionary'''
+        frequency = self.frequency
+        bins = self.General.bins
+        for key, value in Mutual_dict.items():
+            first_effect = key.split('_')[-2]
+            second_effect = key.split('_')[-1]
+            M_first_effect = self.getAttribute(first_effect, 'M')
+            I_second_effect = self.getAttribute(second_effect, 'I')
+            if second_effect == 'Wedge' or second_effect == 'CB':
+                # If the second effect is Wedge or CB, the I don't have the size [freq,bins], so it must be modified to have it
+                I_second_effect = np.expand_dims(I_second_effect, axis=1)
+                I_second_effect = np.repeat(I_second_effect, bins, axis=1)
+            M_key = f'M_{first_effect}_{second_effect}'
+            M_value = (M_first_effect - value) / I_second_effect
+
+            for i in range(bins):
+                self.General.lib_path = change_library_MutualCoupling(self.General.lib_path, f'{M_key}_{i + 1}', frequency, M_value[:, i])
+
+
+    def calculate_Coupling_Components(self, Effect: str) -> dict:
+        ''' This function calculates the Mutual Coupling between the conductor losses and the Effect
+            Effect: Wedge or CB'''
+
+        M_dict = {}
+        # Retrieve f_mag, f_mag_X and f_mag_Y from the Comsol field files specific for each effect
+        f_mag, f_mag_X, f_mag_Y = self.retrieve_field_contributions_COMSOL(Effect)
+        frequency = self.frequency
+        T = self.T
+
+        # Retrieve the Option class attributes as dictionary
+        options_dict = vars(self.Options)
+        for flag, value in options_dict.items():
+            if flag != 'flag_SC' and flag != 'flag_Wedge' and flag != 'flag_CB' and value == True:
+                # If the flag of an effect is set and the effect is not 'CB' or 'Wedge', takes the name of the effect
+                eff_coupled = flag.split('_')[-1]
+                if eff_coupled == 'ISCC':
+                    # Calls the calculate function of the corresponding effect and calculates the M
+                    _, _, M, _, _ = getattr(self, f'calculate_{eff_coupled}')(frequency=frequency, T=T, fMag_X=f_mag_X, fMag_Y=f_mag_Y, flag_save=False)
+                else:
+                    # Calls the calculate function of the corresponding effect and calculates the M
+                    _, _, M = getattr(self, f'calculate_{eff_coupled}')(frequency=frequency, T=T, fMag=f_mag, flag_coupling=True, flag_save=False)
+                # Save the new M in the dictionary
+                M_dict[f'M_{eff_coupled}_{Effect}'] = M
+
+        return M_dict
+
+    def read_COMSOL_field_file(self, Effect: str = None) -> np.ndarray:
+        '''
+        '''
+
+        f_mag_X_Roxie = self.Strands.f_mag_X_Roxie
+        f_mag_Y_Roxie = self.Strands.f_mag_Y_Roxie
+        f_mag_X_Comsol = self.Strands.f_mag_X_Comsol
+        f_mag_Y_Comsol = self.Strands.f_mag_Y_Comsol
+
+        if Effect is not None:
+            _, f_mag_X_all, f_mag_Y_all = self.retrieve_field_contributions_COMSOL(Effect=Effect)
+
+            f_X_diff = f_mag_X_all * np.sign(f_mag_X_Roxie) - f_mag_X_Comsol
+            f_Y_diff = f_mag_Y_all * np.sign(f_mag_Y_Roxie) - f_mag_Y_Comsol
+
+            f_X = f_mag_X_Roxie + f_X_diff
+            f_Y = f_mag_Y_Roxie + f_Y_diff
+            f_mag = np.sqrt(f_X ** 2 + f_Y ** 2)
+
+            return f_mag, f_X, f_Y
+
+
+    def retrieve_field_contributions_COMSOL(self, Effect: str = None) -> np.ndarray:
         '''
         Retrieve the strand field contributions, simulated by COMSOL and saved in .csv
         :return: f_mag
         '''
 
         local_library_path = os.path.join(Path(self.General.path_input_file).resolve(), 'TFM_input')
+        value = self.Field_interp_value
+        frequency = self.frequency
 
         Param = []
         files_Field = []
         df_array_X = []
         df_array_Y = []
 
         if value is None:
             value = self.T
 
         for dir in os.listdir(local_library_path):
             if dir.startswith('Field_Map'):
-                if not flag_BS:
-                    if 'NoBS' in dir:
-                        parameter = dir.replace('.csv','').split('_')[-2]
-                        Param.append(float(parameter))
-                        files_Field.append(dir)
-                else:
-                    if 'wBS' in dir:
-                        parameter = dir.replace('.csv','').split('_')[-2]
-                        Param.append(float(parameter))
-                        files_Field.append(dir)
+                if Effect in dir:
+                    parameter = dir.replace('.csv','').split('_')[-1]
+                    Param.append(float(parameter))
+                    files_Field.append(dir)
 
         Param = np.array(Param)
         files_Field = np.array(files_Field)
 
         if float(value) in Param:
             closest_Param = np.array([value])
         elif(value < Param.min() or value > Param.max()):
             raise Exception('Error: Parameter out of range')
         else:
             closest_indices = np.argsort(np.abs(Param - value))[:4]
             closest_Param = Param[closest_indices]
 
         for i in range(len(closest_Param)):
-            file =os.path.join(local_library_path, files_Field[i])
+            file = os.path.join(local_library_path, files_Field[i])
             df_COMSOL = pd.read_csv(file, header=None, dtype=str, na_filter=False)
-            if i == 0:
-                frequency = np.array(df_COMSOL.iloc[1, 2::2]).astype(float)
             mapping = np.vectorize(lambda t: complex(t.replace('i', 'j')))
             df_COMSOL = mapping(df_COMSOL.values[2:, 2:]).T
-            # df_COMSOL = df_COMSOL.values[2:, 2:].astype(str)  # Convert to string to perform replacement
-            # df_COMSOl = np.char.replace(df_COMSOL, 'i', 'j').astype(complex).T
             df_X = np.real(df_COMSOL[::2, :] * np.conjugate(df_COMSOL[::2, :]))
             df_Y = np.real(df_COMSOL[1::2, :] * np.conjugate(df_COMSOL[1::2, :]))
             df_array_X.append(df_X)
             df_array_Y.append(df_Y)
 
-
-        _, f_mag_X_Roxie, f_mag_Y_Roxie = self.retrieve_field_contributions_Roxie()
-        sign_x = np.sign(f_mag_X_Roxie)
-        sign_y = np.sign(f_mag_Y_Roxie)
-
         order = np.argsort(closest_Param)
         closest_Param = closest_Param[order]
 
         # Interpolate the X and Y direction for a given rho
         df_array_X = np.array(df_array_X)
         df_array_X = df_array_X[order]
         df_array_Y = np.array(df_array_Y)
@@ -864,21 +951,20 @@
             new_points_Y = (np.array([value]), frequency)
             f_mag_Y = interp_Y(new_points_Y)
         else:
             f_mag_X = df_array_X[0, :, :]
             f_mag_Y = df_array_Y[0, :, :]
 
         f_mag = np.sqrt(f_mag_X + f_mag_Y)
-        f_mag_X = np.sqrt(f_mag_X) * sign_x
-        f_mag_Y = np.sqrt(f_mag_Y) * sign_y
-
-        self.frequency = frequency
+        f_mag_X = np.sqrt(f_mag_X)
+        f_mag_Y = np.sqrt(f_mag_Y)
 
         return f_mag, f_mag_X, f_mag_Y
 
+
     def retrieve_field_contributions_Roxie(self) -> np.ndarray:
 
         Bx = self.LedetAuxiliary.Bx
         By = self.LedetAuxiliary.By
         Iref = self.LedetOptions.Iref
 
         f_mag_X = Bx / Iref
@@ -890,52 +976,72 @@
         peakB_real = np.max(B_E)
         f_peakReal_Superposition = peakB_real / peakB_superPos
 
         f_mag_X_all = f_mag_X * f_peakReal_Superposition
         f_mag_Y_all = f_mag_Y * f_peakReal_Superposition
 
         frequency = np.logspace(0, 6, 120+1)
+        self.frequency=frequency
         f_mag_X_all = np.repeat(f_mag_X_all[:, np.newaxis], len(frequency), axis=1).T
         f_mag_Y_all = np.repeat(f_mag_Y_all[:, np.newaxis], len(frequency), axis=1).T
         f_mag = np.repeat(f_mag[:, np.newaxis], len(frequency), axis=1).T
 
-
-        self.frequency = frequency
-
         return f_mag, f_mag_X_all, f_mag_Y_all
 
-    def check_inductance_matrix(self):
+    def check_inductance_matrix_losses(self, Mutual_dict: dict):
 
         frequency = self.frequency
-        Effects = ['Magnet', 'PC', 'ISCC', 'IFCC', 'EC_CopperSheath', 'ColdBore', 'Wedges']
+        bins = self.General.bins
+        options_dict = vars(self.Options)
+        Effects = []
+        # Looping through all the attributes in the Option class to get the Effects name
+        for flag, value in options_dict.items():
+            if flag != 'flag_SC' and flag != 'flag_BS':
+                Effect = flag.split('_')[-1]
+                Effects.append(Effect)
+        Effects = np.repeat(np.array(Effects), bins)
+        Effects = np.insert(Effects, 0, 'Mag').astype(str)
         L_matrix_list = []
 
-        for i in range(len(frequency)):
+        for freq in range(len(frequency)):
+            # Creating the matrix and filling it with 0
             L_matrix = np.zeros((len(Effects), len(Effects)))
-            for j in range(len(Effects)):
-                if Effects[j] == 'Magnet':
-                    L_matrix[0, 0] = self.General.L_mag
-                else:
-                    if Effects[j] != 'ColdBore' and Effects[j] != 'Wedges':
-                        L_matrix[0, j] = self.__dict__[Effects[j]].M[i, :]
-                        L_matrix[j, 0] = self.__dict__[Effects[j]].M[i, :]
-                        L_matrix[j, j] = self.__dict__[Effects[j]].L[i, :]
+            for eff in range(len(Effects)):
+                    if eff == 0:  # Checking if the Effect[eff] == 'Mag'
+                        L_matrix[0, 0] = self.General.L_mag
                     else:
-                        L_matrix[0, j] = self.__dict__[Effects[j]].M[i]
-                        L_matrix[j, 0] = self.__dict__[Effects[j]].M[i]
-                        L_matrix[j, j] = self.__dict__[Effects[j]].L[i]
+                        if Effects[eff-1] == Effects[eff]: # Checking if it's not the first time that we encounter this effect in the dict
+                            count_bin += 1  # If it's not the first time, the bin counting must be incremented
+                        else:
+                            count_bin = 0  # If it is the first time, the bin counting is set to zero
+
+                        # Filling the matrix with the L values along the diagonal and the M values symmetrically
+                        # on the first row and on the first column, selecting the right values according to count_bin
+                        if Effects[eff] == 'Wedge' or Effects[eff] == 'CB':
+                            L_matrix[0, eff] = self.getAttribute(Effects[eff], 'M')[freq]
+                            L_matrix[eff, 0] = self.getAttribute(Effects[eff], 'M')[freq]
+                            L_matrix[eff, eff] = self.getAttribute(Effects[eff], 'L')[freq]
+                        else:
+                            L_matrix[0, eff] = self.getAttribute(Effects[eff], 'M')[freq, count_bin]
+                            L_matrix[eff, 0] = self.getAttribute(Effects[eff], 'M')[freq, count_bin]
+                            L_matrix[eff, eff] = self.getAttribute(Effects[eff], 'L')[freq, count_bin]
+
+                        for key, value in Mutual_dict.items():
+                            if Effects[eff] in key:  # For each key of the dict, check if the current effect is contained in it
+                                for l in range(len(Effects)):  # If yes, find the other effect contained in the same key
+                                    if l != 0 and eff != l and Effects[l] in key:
+                                        if Effects[l - 1] != Effects[l]:
+                                            # Take the first effect with that name and then select the right column index
+                                            # and the right value by selecting the same count_bin of the Effects[eff] element
+                                            L_matrix[eff, l+count_bin] = value[freq, count_bin]
             L_matrix_list.append(L_matrix)
 
         for i in range(len(L_matrix_list)):
             if not is_positive_definite(L_matrix_list[i]):
                 raise Exception(f'Matrix not positive definite for frequency {frequency[i]}')
-            # else:
-            #     print(f'Matrix positive definite for frequency {frequency[i]}')
-
-
 
 
     def rhoCu_nist(self, T: float, RRR: np.ndarray, B: np.ndarray) -> np.ndarray:
         '''
         Helper function to calculate resistivity of copper. Taken from steam-materials library
 
         :param T: Temperature
@@ -1018,64 +1124,87 @@
         'dcore_inGroup': 'd_core',
     }
 
     returned_key = lookup[key] if key in lookup else None
     return returned_key
 
 
-def bin_components(frequency: np.ndarray, L: np.ndarray, R: np.ndarray, M: np.ndarray, bins: int, sort_on: str = 'L') ->  np.ndarray:
+def bin_components(frequency: np.ndarray, L: np.ndarray, R: np.ndarray, M: np.ndarray, bins: int, sort_on: str = 'L',
+                   I: np.ndarray = np.array([]), flag_PC:bool=False) -> np.ndarray:
     '''
     Helper function that bins components into n bins, based on a sorting on a specific variable out of R,L,M
 
     :param frequency: frequency vector
     :param L: L-vector
     :param R: R-vector
     :param M: M_vector
     :param bins: number of bins to be separated
     :param sort_on: Which variable to sort on
     :return: 3 np.ndarray in the order: L,R,M that are binned into n_bins
     '''
 
-    if sort_on=='L':
-        sort_on = 'L_bin'
-    elif sort_on=='R':
+    if sort_on == 'L':
+        if np.all(np.isclose(L, L[0, 0])):
+            sort_on = 'R_bin'
+        else:
+            sort_on = 'L_bin'
+    elif sort_on == 'R':
         sort_on = 'R_bin'
-    elif sort_on=='M':
+    elif sort_on == 'M':
         sort_on = 'M_bin'
     else:
         raise Exception(f'Do not understand sort_on: {sort_on} - Only R, L, M')
 
     f = frequency
     R_bin = np.zeros((len(f), bins))
-    M_bin = np.zeros((len(f), bins))
+    M_bin = np.zeros((len(f), bins), dtype=np.complex_)
+    s_r = np.zeros((len(f), bins))
+    s_i = np.zeros((len(f), bins))
     L_bin = np.zeros((len(f), bins))
+    I_bin = np.zeros((len(f), bins), dtype=np.complex_)
     for j in range(len(f)):
         # Bin the resistivities and take the mean of their M
         df = pd.DataFrame.from_dict({'R_bin': np.nan_to_num(R[j, :])})
         df['M_bin'] = np.nan_to_num(M[j, :])
         df['L_bin'] = np.nan_to_num(L[j, :])
+        if len(I) != 0:
+            df['I_bin'] = np.nan_to_num(I[j, :])
         x = pd.cut(df[sort_on], np.linspace(min(df[sort_on]) * 0.9, max(df[sort_on]) * 1.1, bins + 1))
         x = x.cat.rename_categories(np.linspace(1, bins, bins).astype(int))
         df['bins'] = x
         df = df.dropna(subset=['bins'])
 
         for i in range(1, bins + 1):
             df.loc[df['bins'] == i, 'R_bin'] = np.average(df.loc[df['bins'] == i, 'R_bin'])
             df.loc[df['bins'] == i, 'L_bin'] = np.average(df.loc[df['bins'] == i, 'L_bin'])
+            if len(I) != 0:
+                df.loc[df['bins'] == i, 'I_bin'] = np.sum(df.loc[df['bins'] == i, 'I_bin'])
             # df.loc[df['bins'] == i, 'R_bin'] = np.nanmedian(df.loc[df['bins'] == i, 'R_bin'])
             # df.loc[df['bins'] == i, 'L_bin'] = np.nanmedian(df.loc[df['bins'] == i, 'L_bin'])
-            df.loc[df['bins'] == i, 'M_bin'] = np.sqrt(np.sum(df.loc[df['bins'] == i, 'M_bin']))
+            M_sel = df.loc[df['bins'] == i, 'M_bin']
+            s_r[j, bins - i] = np.mean(np.round(np.sign(np.real(M_sel))), 0)
+            s_i[j, bins - i] = np.mean(np.round(np.sign(np.imag(M_sel))), 0)
+            if flag_PC:
+                df.loc[df['bins'] == i, 'M_bin'] = np.sqrt(np.sum(M_sel))
+            else:
+                df.loc[df['bins'] == i, 'M_bin'] = np.sqrt(np.sum(M_sel ** 2))
         df = df.drop_duplicates().reset_index(drop=True).drop('bins', axis=1)
         df = df.loc[~(df == 0).all(axis=1)]
 
         R_bin[j, :] = df['R_bin']
         M_bin[j, :] = df['M_bin']
         L_bin[j, :] = df['L_bin']
+        if len(I) != 0:
+            I_bin[j, :] = df['I_bin']
 
-    return L_bin, R_bin, M_bin
+    M_bin = s_r * abs(np.real(M_bin)) + 1j * s_i * abs(np.imag(M_bin))
+    if len(I) != 0:
+        return L_bin, R_bin, M_bin, I_bin
+    else:
+        return L_bin, R_bin, M_bin
 
 
 def change_library_EqLoop(path_file: Path, element: str, frequency: np.ndarray, L_eq: np.ndarray, R_eq: np.ndarray, M_eq: np.ndarray, bins: int = 2, force_new_name: Path = ''):
     '''
     Helper function that changes the TFM magnet .lib file and includes in Table function the given R,L,M parameter
 
     element = Element, for which the RLM to be inserted e.g. BS, CPS, ED ...
@@ -1113,15 +1242,15 @@
     #### Creating string for equivalent mutual inductance
     str_M = []
     if M_eq.size:
         for i in range(bins):
             str_group_M = f'.FUNC M_{element}_{i + 1}(1)					' + '{TABLE{FREQ} =  '
             M = M_eq[:, i]
             for j in range(len(frequency)):
-                str_group_M = str_group_M + f'({frequency[j]},{M[j]})     '
+                str_group_M = str_group_M + f'({frequency[j]},{np.real(M[j])}+{np.imag(M[j])}J)     '
             str_group_M = str_group_M + '}\n'
             str_M.append(str_group_M)
 
     ## Opening library file
     lib_path = path_file
     with open(lib_path) as f:
         lines = f.readlines()
@@ -1152,15 +1281,15 @@
     Helper function that changes the mutual coupling values of element to M_eq. Can be multiple values, e.g. a
     changing coupling over frequency
     '''
 
     #### Creating string for equivalent mutual inductance
     str_group_M = f'.FUNC {element}(1)					' + '{TABLE{FREQ} =  '
     for j in range(len(frequency)):
-        str_group_M = str_group_M + f'({frequency[j]},{M_eq[j]})     '
+        str_group_M = str_group_M + f'({frequency[j]},{np.real(M_eq[j])}+{np.imag(M_eq[j])}J)     '
     str_group_M = str_group_M + '}\n'
 
     ## Opening library file
     lib_path = path_file
     with open(lib_path) as f:
         lines = f.readlines()
 
@@ -1240,15 +1369,10 @@
                 break
         tau_index = int((np.min(list_index) + np.max(list_index)) / 2)
 
     return tau_index
 
 
 def is_positive_definite(matrix):
-    try:
-        # Attempt Cholesky decomposition
-        np.linalg.cholesky(matrix)
-        return True
-    except np.linalg.LinAlgError:
-        return False
+    return np.all(np.linalg.eigvals(matrix) >= 0)
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2024.5.4/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/Solenoids.py` & `steam-sdk-2024.5.4/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2024.5.4/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2024.5.4/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/cosims/CoSimPyCoSim.py` & `steam-sdk-2024.5.4/steam_sdk/cosims/CoSimPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataAPDLCTOptions.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataAPDLCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataConductor.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataFiQuS.py`

 * *Files 7% similar despite different names*

```diff
@@ -164,301 +164,607 @@
     """
     type: Literal['CCT_straight']
     geometry: CCTGeometry = CCTGeometry()
     mesh: CCTMesh = CCTMesh()
     solve: CCTSolve = CCTSolve()
     postproc: CCTPostproc = CCTPostproc()
 
+# CWS
 
 class CWSGeometryConductors(BaseModel):  # Conductor file data for geometry building
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
-    resample: Optional[List[int]] = None
-    skip_middle_from: Optional[List[int]] = None  # decides which bricks are skipped in fuse operation, basically only a few bricks should overlap with the former.
-    skip_middle_to: Optional[List[int]] = None  # decides which bricks are skipped in fuse operation, basically only a few bricks should overlap with the former.
+
+    skip_middle_from: Optional[List[int]] = (
+        None  # decides which bricks are skipped in fuse operation, basically only a few bricks should overlap with the former.
+    )
+    skip_middle_to: Optional[List[int]] = (
+        None  # decides which bricks are skipped in fuse operation, basically only a few bricks should overlap with the former.
+    )
     file_names_large: Optional[List[str]] = None
     file_names: Optional[List[str]] = None  # Inner_17.1mm #[inner_FL, outer_FL] #
-    ends_need_trimming: bool = False    # If there are windings "sticking out" of the air region this needs to set to True. It removes 2 volumes per winding after the fragment operation
+    ends_need_trimming: bool = (
+        False  # If there are windings "sticking out" of the air region this needs to set to True. It removes 2 volumes per winding after the fragment operation
+    )
 
 
 class CWSGeometryFormers(BaseModel):  # STEP file data for geometry building
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
-    file_names: Optional[List[str]] = None    # STEP file names to use
-    air_pockets: Optional[List[int]] = None   # number of air pockets (for e.g. for heater or temperature sensor pads) on the formers
+
+    file_names: Optional[List[str]] = None  # STEP file names to use
+    air_pockets: Optional[List[int]] = (
+        None  # number of air pockets (for e.g. for heater or temperature sensor pads) on the formers
+    )
 
 
 class CWSGeometryShells(BaseModel):  # STEP file data for geometry building
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
-    file_names: Optional[List[str]] = None    # STEP file names to use
+
+    file_names: Optional[List[str]] = None  # STEP file names to use
 
 
 class CWSGeometryAir(BaseModel):  # Geometry related air_region _inputs
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
+
     name: Optional[str] = None  # name to use in gmsh and getdp
-    sh_type: Optional[str] = None  # cylinder, cuboid, cylinder_offset, cylinder_cov or cylinder_link are possible
-    ar: Optional[float] = None  # if box type is cuboid 'a' is taken as a dimension, if cylinder then 'r' is taken
-    z_min: Optional[float] = None  # extend of air region in negative z direction, for cylinder_cov this is ignored
-    z_max: Optional[float] = None  # extend of air region in positive z direction, for cylinder_cov this is ignored
-    rotate: Optional[float] = None    # rotation around z axis in degrees
-    xy_offset: Optional[List[float]] = None  # list with x and y offset of the cylinder, only works if sh_type is set to cylinder_offset, e.g. [0, 0.3]
-    extension_distance: Optional[List[float]] = None # list with distances in meter to take along the line going through bricks of end terminals. For example to extend the air region by 0.5 m each way the entry could be [0.5, -0.5]
+    sh_type: Optional[str] = (
+        None  # cylinder, cuboid, cylinder_offset, cylinder_cov or cylinder_link are possible
+    )
+    ar: Optional[float] = (
+        None  # if box type is cuboid 'a' is taken as a dimension, if cylinder then 'r' is taken
+    )
+    z_min: Optional[float] = (
+        None  # extend of air region in negative z direction, for cylinder_cov this is ignored
+    )
+    z_max: Optional[float] = (
+        None  # extend of air region in positive z direction, for cylinder_cov this is ignored
+    )
+    rotate: Optional[float] = None  # rotation around z axis in degrees
+    xy_offset: Optional[List[float]] = (
+        None  # list with x and y offset of the cylinder, only works if sh_type is set to cylinder_offset, e.g. [0, 0.3]
+    )
+    extension_distance: Optional[List[float]] = (
+        None  # list with distances in meter to take along the line going through bricks of end terminals. For example to extend the air region by 0.5 m each way the entry could be [0.5, -0.5]
+    )
 
 
 class CWSGeometry(BaseModel):
     """
-        Level 2: Class for FiQuS CWS for FiQuS input
+    Level 2: Class for FiQuS CWS for FiQuS input
     """
+
+    iterative_fragment: Optional[bool] = Field(
+        default=None, description="Controls if fragment is handled by gmsh only (false) or python with gmsh (ture)"
+    )
     conductors: CWSGeometryConductors = CWSGeometryConductors()
     formers: CWSGeometryFormers = CWSGeometryFormers()
     shells: CWSGeometryShells = CWSGeometryShells()
     air: CWSGeometryAir = CWSGeometryAir()
 
+
 class CWSSolveMaterialPropertyListConductors(BaseModel):
     constant: Optional[List[float]] = None  # list of values if constant is used
 
 
 class CWSSolveMaterialPropertyList(BaseModel):
     constant: Optional[List[float]] = None  # list of values if constant is used
-    function: Optional[List[str]] = None  # list of material property function names if function is used
+    function: Optional[List[str]] = (
+        None  # list of material property function names if function is used
+    )
 
 
 class CWSSolveMaterialPropertySingle(BaseModel):
     constant: Optional[float] = None  # value if constant is used
-    function: Optional[str] = None  # material property function name if function is used
-
-
-class CWSSolveConductorsExcitationFunction(BaseModel):  # Solution time used Conductor _inputs (materials and BC)
-    """
-        Level 2: Class for FiQuS CWS
-    """
-    initials: Optional[List[float]] = Field(default=None, description="Initial current or voltage in the conductor")
-    names: Optional[List[str]] = Field(default=None, description="Currently, these function names are supported: exp_decrease, exp_increase, linear_decrease, linear_increase ")
-    taus: Optional[List[float]] = Field(default=None, description="Time constant for exponential: Amplitude*Exp(-time/tau), for linear: Amplitude*(time-time_initial)/tau ")
-
-
-class CWSSolveConductorsExcitationFromFile(BaseModel):  # Solution time used Conductor _inputs (materials and BC)
-    """
-        Level 2: Class for FiQuS CWS
-    """
-    file_name: Optional[str] = None  # full file name (i.e. with extension) in the input folder or complete path
-    time_header: Optional[str] = None  # string defining the time signal header in the txt file
-    value_headers: Optional[List[str]] = Field(default=None, description="string defining the value (typically current) signal header in the txt file")
-
-
-class CWSSolveConductorsExcitation(BaseModel):  # Solution time used Conductor _inputs (materials and BC)
+    function: Optional[str] = (
+        None  # material property function name if function is used
+    )
+
+
+class CWSSolveConductorsExcitationFunction(
+    BaseModel
+):  # Solution time used Conductor _inputs (materials and BC)
+    """
+    Level 2: Class for FiQuS CWS
+    """
+
+    initials: Optional[List[float]] = Field(
+        default=None, description="Initial current or voltage in the conductor"
+    )
+    names: Optional[List[Literal["exp_decrease", "exp_increase", "linear_decrease", "linear_increase_from_zero"]]] = Field(
+        default=['exp_decrease'],
+        description="Currently, these function names are supported: exp_decrease, exp_increase, linear_decrease, linear_increase ",
+    )
+    taus: Optional[List[float]] = Field(
+        default=None,
+        description="Time constant for exponential: Amplitude*Exp(-time/tau), for linear: Amplitude*(time-time_initial)/tau ",
+    )
+
+
+class CWSSolveExcitationFromFile(
+    BaseModel
+):  # Solution time used Conductor _inputs (materials and BC)
+    """
+    Level 2: Class for FiQuS CWS
+    """
+
+    file_name: Optional[str] = (
+        None  # full file name (i.e. with extension) in the input folder or complete path
+    )
+    time_header: Optional[str] = (
+        None  # string defining the time signal header in the txt file
+    )
+    value_headers: Optional[List[str]] = Field(
+        default=None,
+        description="string defining the value (typically current [A] or power [W]) signal header in the txt file",
+    )
+
+
+class CWSSolveConductorsExcitation(
+    BaseModel
+):  # Solution time used Conductor _inputs (materials and BC)
+    """
+    Level 2: Class for FiQuS CWS
+    """
+
+    conductors_nw: Optional[List[int]] = Field(
+        default=None,
+        description="Number of conductors in channel in the height direction (pointing out of the channel direction)",
+    )
+    conductors_nh: Optional[List[int]] = Field(
+        default=None,
+        description="Number of conductors in channel in the width direction",
+    )
+    multips: Optional[List[float]] = Field(
+        default=None,
+        description="This is decide on polarity of powering the magnet, most often value of 1 or -1 is used. However, arbitrary multiplication is also supported",
+    )
+    function: CWSSolveConductorsExcitationFunction = (
+        CWSSolveConductorsExcitationFunction()
+    )
+    from_file: CWSSolveExcitationFromFile = (
+        CWSSolveExcitationFromFile()
+    )
+    transient_use: Optional[Literal["function", "from_file"]] = Field(
+        default="function",
+        title="Use Material Property as",
+        description="Either values from a function or from_file can be used",
+    )  # function or from_file allowed
+
+
+class CWSSolveConductors(
+    BaseModel
+):  # Solution time used Conductor _inputs (materials and BC)
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
-    conductors_nw: Optional[List[int]] = Field(default=None, description="Number of conductors in channel in the height direction (pointing out of the channel direction)")
-    conductors_nh: Optional[List[int]] = Field(default=None, description="Number of conductors in channel in the width direction")
-    multips: Optional[List[float]] = Field(default=None, description="This is decide on polarity of powering the magnet, most often value of 1 or -1 is used. However, arbitrary multiplication is also supported")
-    function: CWSSolveConductorsExcitationFunction = CWSSolveConductorsExcitationFunction()
-    from_file: CWSSolveConductorsExcitationFromFile = CWSSolveConductorsExcitationFromFile()
-    transient_use: Optional[str] = None  # function or from_file allowed
 
-
-class CWSSolveConductors(BaseModel):  # Solution time used Conductor _inputs (materials and BC)
-    """
-        Level 2: Class for FiQuS CWS
-    """
     excitation: CWSSolveConductorsExcitation = CWSSolveConductorsExcitation()
-    conductivity_el: CWSSolveMaterialPropertyListConductors = CWSSolveMaterialPropertyListConductors()
+    conductivity_el: CWSSolveMaterialPropertyListConductors = (
+        CWSSolveMaterialPropertyListConductors()
+    )
     permeability: Optional[List[float]] = None  # relative permeability
 
 
 class CWSSolveInduced(BaseModel):  # Solution time used fqpls _inputs (materials and BC)
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
+
+    use: Optional[Literal["function", "constant"]] = Field(
+        default="function",
+        title="Use Material Property as",
+        description="Either values from a function or constant can be used",
+    )
     RRR_functions: Optional[List[float]] = None  # RRR to use in material functions
     conductivity_el: CWSSolveMaterialPropertyList = CWSSolveMaterialPropertyList()
     permeability: List[float] = []  # relative permeability
-    conductivity_th: CWSSolveMaterialPropertyList = Field(default=CWSSolveMaterialPropertyList(), alias="conductivity_th", description="W/mK")
-    heat_capacity: CWSSolveMaterialPropertyList = Field(default=CWSSolveMaterialPropertyList(), alias="heat_capacity", description="J/m^3 K")
+    conductivity_th: CWSSolveMaterialPropertyList = Field(
+        default=CWSSolveMaterialPropertyList(),
+        alias="conductivity_th",
+        description="W/mK",
+    )
+    heat_capacity: CWSSolveMaterialPropertyList = Field(
+        default=CWSSolveMaterialPropertyList(),
+        alias="heat_capacity",
+        description="J/m^3 K",
+    )
+
+
+class CWSSolveHeaterFunction(BaseModel):
+    """
+    Defines entries for function to use in a form of linearly interpolated LOOK-UP-TABLE (LUT) of power vs time
+    """
+    times: Optional[List[List[float]]] = Field(
+        default=None,
+        title="Time look up table",
+        description="Time values for power values. This list must be the same length as power_LUT. It is list of list, with each list per heater.",
+    )
+    powers: Optional[List[List[float]]] = Field(
+        default=None,
+        title="Time look up table",
+        description="Power values [W] for time values specified. This list must be the same length as time_LUT. It is list of list, with each list per heater.",
+    )
+
+
+class CWSSolveHeaters(BaseModel):  # Solver options for applying BC for heaters
+    """
+    Level 2: Class for FiQuS CWS
+    """
+
+    transient_use: Literal["LUT", "from_file", "disabled"] = Field(
+        default="disabled",
+        title="Use Material Property as",
+        description="Either values from a function or from_file can be used",
+    )
+    LUT: CWSSolveHeaterFunction = (
+        CWSSolveConductorsExcitationFunction()
+    )
+    from_file: CWSSolveExcitationFromFile = (
+        CWSSolveExcitationFromFile()
+    )
 
 
 class CWSSolveInsulation(BaseModel):
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
-    thickness: Optional[float] = Field(default=None, description="Thickness of insulation former to former or former to shell")     #
+
+    thickness: Optional[float] = Field(
+        default=None,
+        description="Thickness of insulation former to former or former to shell",
+    )  #
     conductivity_th: CWSSolveMaterialPropertySingle = CWSSolveMaterialPropertySingle()
-    heat_capacity: CWSSolveMaterialPropertySingle = Field(default=CWSSolveMaterialPropertySingle(), alias="heat_capacity", description="J/m^3 K")
+    heat_capacity: CWSSolveMaterialPropertySingle = Field(
+        default=CWSSolveMaterialPropertySingle(),
+        alias="heat_capacity",
+        description="J/m^3 K",
+    )
 
 
 class CWSSolveAir(BaseModel):  # Solution time used air _inputs (materials and BC)
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
-    conductivity_el: Optional[float] = Field(default=None, description="Electrical conductivity")
-    permeability: Optional[float] = Field(default=None, description="Relative permeability")
+
+    conductivity_el: Optional[float] = Field(
+        default=None, description="Electrical conductivity"
+    )
+    permeability: Optional[float] = Field(
+        default=None, description="Relative permeability"
+    )
 
 
 class CWSSolveOutputResample(BaseModel):  # Solution outputs definition
-    enabled: Optional[bool] = Field(default=None, description="Flag to decide if the output is resampled or not")
-    delta_t: Optional[float] = Field(default=None, description="Delta time for resampling")
+    enabled: Optional[bool] = Field(
+        default=None, description="Flag to decide if the output is resampled or not"
+    )
+    delta_t: Optional[float] = Field(
+        default=None, description="Delta time for resampling"
+    )
 
 
 class CWSSolveOutput(BaseModel):  # Solution outputs definition
-    saved: Optional[bool] = Field(default=None, description="Flat to decide if the output is saved")
+    saved: Optional[bool] = Field(
+        default=None, description="Flat to decide if the output is saved"
+    )
     resample: CWSSolveOutputResample = CWSSolveOutputResample()
-    variables: Optional[List[str]] = Field(default=None, description="Name of variable to post-process by GetDP")
-    volumes: Optional[List[str]] = Field(default=None, description="Name of volume to post-process by GetDP")
-    file_exts: Optional[List[str]] = Field(default=None, description="Name of file extensions to output by GetDP")
+    variables: Optional[List[str]] = Field(
+        default=None, description="Name of variable to post-process by GetDP"
+    )
+    volumes: Optional[List[str]] = Field(
+        default=None, description="Name of volume to post-process by GetDP"
+    )
+    file_exts: Optional[List[str]] = Field(
+        default=None, description="Name of file extensions to output by GetDP"
+    )
 
 
 class CWSSolveStaticSettings(BaseModel):
-    solved: Optional[bool] = Field(default=None, description="Chooses if static solution is solved. Note the transient solution starts with a static solution, so if this and the transient are set to true, the static is solved twice")
+    solved: Optional[bool] = Field(
+        default=None,
+        description="Chooses if static solution is solved. Note the transient solution starts with a static solution, so if this and the transient are set to true, the static is solved twice",
+    )
     output: CWSSolveOutput = CWSSolveOutput()
 
 
 class CWSSolveTime(BaseModel):
     initial: Optional[float] = Field(default=None, description="Initial time")
     end: Optional[float] = Field(default=None, description="End time")
 
 
 class CWSSolveTimeFixed(BaseModel):
     step: Optional[float] = Field(default=None, description="Time step")
     theta: Optional[float] = Field(default=None, description="Time stepping scheme")
 
 
 class CWSSolveTimeAdaptiveLTEInputs(BaseModel):
-    names: Optional[List[str]] = Field(default=None, description="string: name of post operation to use")
-    relatives: Optional[List[float]] = Field(default=None, description="relative tolerance")
-    absolutes: Optional[List[float]] = Field(default=None, description="absolute tolerance")
-    normTypes: Optional[List[str]] = Field(default=None, description="string with norm type, allowed: L1Norm, MeanL1Norm, L2Norm, MeanL2Norm, LinfNorm")
+    names: Optional[List[str]] = Field(
+        default=None, description="string: name of post operation to use"
+    )
+    relatives: Optional[List[float]] = Field(
+        default=None, description="relative tolerance"
+    )
+    absolutes: Optional[List[float]] = Field(
+        default=None, description="absolute tolerance"
+    )
+    normTypes: Optional[List[str]] = Field(
+        default=None,
+        description="string with norm type, allowed: L1Norm, MeanL1Norm, L2Norm, MeanL2Norm, LinfNorm",
+    )
 
 
 class CWSSolveTimeAdaptiveLTE(BaseModel):
-    System: CWSSolveTimeAdaptiveLTEInputs = CWSSolveTimeAdaptiveLTEInputs()         # Quantities of interest specified at system level
-    PostOperation: CWSSolveTimeAdaptiveLTEInputs = CWSSolveTimeAdaptiveLTEInputs()  # Quantities of interest specified at PostOperation level
+    System: CWSSolveTimeAdaptiveLTEInputs = (
+        CWSSolveTimeAdaptiveLTEInputs()
+    )  # Quantities of interest specified at system level
+    PostOperation: CWSSolveTimeAdaptiveLTEInputs = (
+        CWSSolveTimeAdaptiveLTEInputs()
+    )  # Quantities of interest specified at PostOperation level
 
 
 class CWSSolveTimeAdaptive(BaseModel):
-    initial_step: Optional[float] = Field(default=None, description="Initial time step. Note this is only used when not starting from previous result")
+    initial_fixed_time_step: Optional[float] = Field(
+        default=-1.0,
+        description="If this value is set to > 0 then an initial fixed time step is performed",
+    )
+    initial_step: Optional[float] = Field(
+        default=None,
+        description="Initial time step. Note this is only used when not starting from previous result",
+    )
     min_step: Optional[float] = Field(default=None, description="Minimum time step")
     max_step: Optional[float] = Field(default=None, description="Maximum time step")
-    integration_method: Optional[str] = Field(default=None, description="string: Euler, Trapezoidal, Gear_2, Gear_3, Gear_4, Gear_5, Gear_6")
-    breakpoints_every: Optional[float] = Field(default=None, description="this creates a list from initial to end time with this step")
-    additional_breakpoints: Optional[List[float]] = Field(default=None, description="Additional break points to request, typically when the solution is expected to change steeply, like t_PC_off of LEDET")
+    integration_method: Optional[str] = Field(
+        default=None,
+        description="string: Euler, Trapezoidal, Gear_2, Gear_3, Gear_4, Gear_5, Gear_6",
+    )
+    breakpoints_every: Optional[float] = Field(
+        default=None,
+        description="this creates a list from initial to end time with this step",
+    )
+    additional_breakpoints: Optional[List[float]] = Field(
+        default=[],
+        description="Additional break points to request, typically when the solution is expected to change steeply, like t_PC_off of LEDET",
+    )
     LTE: CWSSolveTimeAdaptiveLTE = CWSSolveTimeAdaptiveLTE()  # local_truncation_errors
 
 
 class CWSSolveNonLinearThermalSettingsTolerance(BaseModel):
-    name: Optional[str] = Field(default=None, description="string: name of post operation to use")
+    name: Optional[str] = Field(
+        default=None, description="string: name of post operation to use"
+    )
     relative: Optional[float] = Field(default=None, description="relative tolerance")
     absolute: Optional[float] = Field(default=None, description="absolute tolerance")
-    normType: Optional[str] = Field(default=None, description="string with norm type, allowed: L1Norm, MeanL1Norm, L2Norm, MeanL2Norm, LinfNorm")
+    normType: Optional[str] = Field(
+        default=None,
+        description="string with norm type, allowed: L1Norm, MeanL1Norm, L2Norm, MeanL2Norm, LinfNorm",
+    )
 
 
 class CWSSolveNonLinearThermalSettings(BaseModel):
-    enabled: Optional[bool] = Field(default=None, description="Flag to decide if constant material properties or nonlinear material functions should be used")
-    maximumNumberOfIterations: Optional[int] = Field(default=None, description="Number of iterations to use")
-    relaxationFactor: Optional[float] = Field(default=None, description="Relaxation factor to use")
-    tolerance: CWSSolveNonLinearThermalSettingsTolerance = CWSSolveNonLinearThermalSettingsTolerance()
+    enabled: Optional[bool] = Field(
+        default=None,
+        description="Flag to decide if constant material properties or nonlinear material functions should be used",
+    )
+    maximumNumberOfIterations: Optional[int] = Field(
+        default=None, description="Number of iterations to use"
+    )
+    relaxationFactor: Optional[float] = Field(
+        default=None, description="Relaxation factor to use"
+    )
+    tolerance: CWSSolveNonLinearThermalSettingsTolerance = (
+        CWSSolveNonLinearThermalSettingsTolerance()
+    )
 
 
 class CWSSolveTransientSettings(BaseModel):
-    solved: Optional[bool] = Field(default=None, description="Flag to decide if a transient solution is solved (when true), when false the transient is skipped")
-    with_thermal: Optional[bool] = Field(default=None, description="Flag to decide if thermal transient is is solved and weakly coupled to the electromagnetic (when true), when false only electromagnetic is considered (depending on the flag 'solved' above)")
-    thermal_TSA_N_elements: Optional[int] = Field(default=None, description="When set to 0 the thermal TSA is disabled so the is no heat flow between induced parts. Otherwise, this is number of elements across the thin shell")
-    nonlinear_thermal_iterations: CWSSolveNonLinearThermalSettings = CWSSolveNonLinearThermalSettings()
-    time_stepping: Optional[str] = Field(default=None, description="either 'fixed' or 'adaptive'")
-    start_from_previous: Optional[bool] = Field(default=None, description="flag to decide if the previous solution (time window of transient should be used as a starting point for this time window)")
+    solved: Optional[bool] = Field(
+        default=None,
+        description="Flag to decide if a transient solution is solved (when true), when false the transient is skipped",
+    )
+    with_thermal: Optional[bool] = Field(
+        default=None,
+        description="Flag to decide if thermal transient is is solved and weakly coupled to the electromagnetic (when true), when false only electromagnetic is considered (depending on the flag 'solved' above)",
+    )
+    thermal_TSA_N_elements: Optional[int] = Field(
+        default=None,
+        description="When set to 0 the thermal TSA is disabled so the is no heat flow between induced parts. Otherwise, this is number of elements across the thin shell",
+    )
+    nonlinear_thermal_iterations: CWSSolveNonLinearThermalSettings = (
+        CWSSolveNonLinearThermalSettings()
+    )
+    time_stepping: Optional[Literal["fixed", "adaptive"]] = Field(
+        default=None, description="either 'fixed' or 'adaptive'"
+    )
+    start_from_previous: Optional[bool] = Field(
+        default=None,
+        description="flag to decide if the previous solution (time window of transient should be used as a starting point for this time window)",
+    )
     time: CWSSolveTime = CWSSolveTime()
     fixed: CWSSolveTimeFixed = CWSSolveTimeFixed()
     adaptive: CWSSolveTimeAdaptive = CWSSolveTimeAdaptive()
     em_output: CWSSolveOutput = CWSSolveOutput()
     th_output: CWSSolveOutput = CWSSolveOutput()
 
 
 class CWSSolve(BaseModel):
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
+
     verbose_level: Optional[int] = None  # Verbosity level for GetDP
     temperature: Optional[float] = None  # Initial temperature for the thermal solve
-    link: Optional[bool] = Field(default=False, description="Decides if powering volumes in a 'linked' way is used")
-    conductors: CWSSolveConductors = CWSSolveConductors()  # windings solution time _inputs
+    link: Optional[bool] = Field(
+        default=None,
+        description="Decides if powering volumes in a 'linked way' (two windings powered in series with only two terminals) is used. This does not work well, so do not use for now",
+    )
+    save_last: bool = Field(
+        default=False,
+        description="This controls if lastTime step only solution is save to allow starting from previous solution",
+    )
+    conductors: CWSSolveConductors = (
+        CWSSolveConductors()
+    )  # windings solution time _inputs
     formers: CWSSolveInduced = CWSSolveInduced()  # formers solution time _inputs
-    shells: CWSSolveInduced = CWSSolveInduced()   # shells solution time _inputs
-    insulation_th: CWSSolveInsulation = CWSSolveInsulation()  # insulation former to former or former to shell, thermal properties only.
-    insulation_el: Optional[bool] = Field(default=None, description="Flag to decide if windings are insulated from formers and formers from each other")
+    shells: CWSSolveInduced = CWSSolveInduced()  # shells solution time _inputs
+    heaters: CWSSolveHeaters = CWSSolveHeaters()  # shells solution time _inputs
+    insulation_th: CWSSolveInsulation = (
+        CWSSolveInsulation()
+    )  # insulation former to former or former to shell, thermal properties only.
+    insulation_el: Optional[bool] = Field(
+        default=None,
+        description="Flag to decide if windings are insulated from formers and formers from each other",
+    )
     air: CWSSolveAir = CWSSolveAir()  # air solution time _inputs
     pro_template: Optional[str] = None  # file name of .pro template file
-    static: CWSSolveStaticSettings = CWSSolveStaticSettings()  # transient solution settings
-    transient: CWSSolveTransientSettings = CWSSolveTransientSettings() # transient solution settings
+    static: CWSSolveStaticSettings = (
+        CWSSolveStaticSettings()
+    )  # transient solution settings
+    transient: CWSSolveTransientSettings = (
+        CWSSolveTransientSettings()
+    )  # transient solution settings
+
+
+class CWSPMeshFieldCoils(BaseModel):
+    enabled: Optional[bool] = Field(
+        default=False, description="If true the coils lines are added."
+    )
+    coils: Optional[Dict[Union[str, int], List[List[float]]]] = Field(
+        default=None,
+        description="Dictionary with structure: key: [[p1_x,p1_y,p1_z], [p2_x,p2_y,p2_z], [p3_x,p3_y,p3_z], [p4_x,p4_y,p4_z]]. At least 3 points are needed. All the pints will be used to create a closed surface.",
+    )
+
+
+class CWSPMeshThSensorAndHeater(BaseModel):
+    enabled: Optional[bool] = Field(default=False, description="If true the coils lines are added.")
+    surfaces: Optional[List[int]] = Field(default=None, description="Specifies surfaces of the brep file to average temperature over or apply heater power.")
+    names: Optional[List[str]] = Field(default=None, description="Specifies user friendly names for the surfaces")
 
 
 class CWSMesh(BaseModel):
     """
-        Level 2: Class for FiQuS CWS
+    Level 2: Class for FiQuS CWS
     """
-    MaxAspectWindings: Optional[float] = None  # used in transfinite mesh_generators settings to define mesh_generators size along two longer lines of hex elements of windings
-    Min_length_windings: Optional[float] = None  # sets how small the edge length for the winding geometry volumes could be used. Overwrites the calculated value if it is smaller than this number.
-    ThresholdSizeMinWindings: Optional[float] = None  # sets field control of Threshold SizeMin
-    ThresholdSizeMaxWindings: Optional[float] = None  # sets field control of Threshold SizeMax
-    ThresholdDistMinWindings: Optional[float] = None  # sets field control of Threshold DistMin
-    ThresholdDistMaxWindings: Optional[float] = None  # sets field control of Threshold DistMax
-    ThresholdSizeMinFormers: Optional[float] = None  # sets field control of Threshold SizeMin
-    ThresholdSizeMaxFormers: Optional[float] = None  # sets field control of Threshold SizeMax
-    ThresholdDistMinFormers: Optional[float] = None  # sets field control of Threshold DistMin
-    ThresholdDistMaxFormers: Optional[float] = None  # sets field control of Threshold DistMax
-    link_terminal: Optional[List[List[int]]] = Field(default=None, description="Specify which windings are connected by giving indexes of winding to connect in the file_names. This is 0 based indexing. To connect first with second winding this is the entry [[0, 1]]")
+
+    MaxAspectWindings: Optional[float] = (
+        None  # used in transfinite mesh_generators settings to define mesh_generators size along two longer lines of hex elements of windings
+    )
+    Min_length_windings: Optional[float] = (
+        None  # sets how small the edge length for the winding geometry volumes could be used. Overwrites the calculated value if it is smaller than this number.
+    )
+    ThresholdSizeMinWindings: Optional[float] = (
+        None  # sets field control of Threshold SizeMin
+    )
+    ThresholdSizeMaxWindings: Optional[float] = (
+        None  # sets field control of Threshold SizeMax
+    )
+    ThresholdDistMinWindings: Optional[float] = (
+        None  # sets field control of Threshold DistMin
+    )
+    ThresholdDistMaxWindings: Optional[float] = (
+        None  # sets field control of Threshold DistMax
+    )
+    ThresholdSizeMinFormers: Optional[float] = (
+        None  # sets field control of Threshold SizeMin
+    )
+    ThresholdSizeMaxFormers: Optional[float] = (
+        None  # sets field control of Threshold SizeMax
+    )
+    ThresholdDistMinFormers: Optional[float] = (
+        None  # sets field control of Threshold DistMin
+    )
+    ThresholdDistMaxFormers: Optional[float] = (
+        None  # sets field control of Threshold DistMax
+    )
+    link_terminal: Optional[List[List[int]]] = Field(
+        default=None,
+        description="Specify which windings are connected by giving indexes of winding to connect in the file_names. This is 0 based indexing. To connect first with second winding this is the entry [[0, 1]]",
+    )
+    temperature_sensors: CWSPMeshThSensorAndHeater = CWSPMeshThSensorAndHeater()
+    heaters: CWSPMeshThSensorAndHeater = CWSPMeshThSensorAndHeater()
+    field_coils: CWSPMeshFieldCoils = CWSPMeshFieldCoils()
 
 
 class CWSPostproc_FieldMap(BaseModel):
-    process_static: Optional[bool] = None # flag to switch on and off processing of static solution for field map
-    process_transient: Optional[bool] = None # flag to switch on and off processing of transient solution for field map
-    channel_ws: Optional[List[float]] = None # wire width
-    channel_hs: Optional[List[float]] = None # wire height
-    winding_order: Optional[List[int]] = Field(default=None, description="[1, 2, 3, 4, 5, 6, 7, 8]")
+    process_static: Optional[bool] = (
+        None  # flag to switch on and off processing of static solution for field map
+    )
+    process_transient: Optional[bool] = (
+        None  # flag to switch on and off processing of transient solution for field map
+    )
+    channel_ws: Optional[List[float]] = None  # wire width
+    channel_hs: Optional[List[float]] = None  # wire height
+    winding_order: Optional[List[int]] = Field(
+        default=None, description="[1, 2, 3, 4, 5, 6, 7, 8]"
+    )
     trim_from: Optional[List[int]] = None
     trim_to: Optional[List[int]] = None
-    n_points_for_B_avg: Optional[List[int]] = None    # number of points to extract for calculating average for B in the center of each wire turn
-    variable: Optional[str] = Field(default=None, description="Name of variable to post-process by gmsh for LEDET") # Name of variable to post-process by python Gmsh API, like B for magnetic flux density
-    volume: Optional[str] = Field(default=None, description="Name of volume to post-process by gmsh for LEDET") # Name of volume to post-process by python Gmsh API, line Winding_1
-    file_ext: Optional[str] = Field(default=None, description="Name of file extensions to output to by gmsh for LEDET") # Name of file extensions o post-process by python Gmsh API, like .pos
-
-
-class CWSPostproc_Inductance(BaseModel):
-    process_static: Optional[bool] = None # flag to switch on and off processing of static solution for inductance
-    process_transient: Optional[bool] = None # flag to switch on and off processing of transient solution for inductance
-
-
-class CWSPostproc_TemperatureMap(BaseModel):
-    process_transient: Optional[bool] = None # flag to switch on and off processing of transient solution of temperature
-
-
-class CWSPostproc_CircuitValues(BaseModel):
-    process_static_and_transient: Optional[bool] = None # flag to switch on and off processing of static and transient solutions for circuit values
+    n_points_for_B_avg: Optional[List[int]] = (
+        None  # number of points to extract for calculating average for B in the center of each wire turn
+    )
+    variable: Optional[str] = Field(
+        default=None, description="Name of variable to post-process by gmsh for LEDET"
+    )  # Name of variable to post-process by python Gmsh API, like B for magnetic flux density
+    volume: Optional[str] = Field(
+        default=None, description="Name of volume to post-process by gmsh for LEDET"
+    )  # Name of volume to post-process by python Gmsh API, line Winding_1
+    file_ext: Optional[str] = Field(
+        default=None,
+        description="Name of file extensions to output to by gmsh for LEDET",
+    )  # Name of file extensions o post-process by python Gmsh API, like .pos
+
+
+class CWSPostprocStaticOrTransient(BaseModel):
+    process_static: Optional[bool] = Field(
+        default=None,
+        description="If true the postprocessing is performed, if false it is not performed",
+    )
+    process_transient: Optional[bool] = Field(
+        default=None,
+        description="If true the postprocessing is performed, if false it is not performed",
+    )
+
+
+class CWSPostprocTemperature(BaseModel):
+    process_transient: Optional[bool] = (
+        None  # flag to switch on and off processing of transient solution of temperature
+    )
+
+
+class CWSPostprocCircuitValues(BaseModel):
+    process_static_and_transient: Optional[bool] = (
+        None  # flag to switch on and off processing of static and transient solutions for circuit values
+    )
 
 
 class CWSPostproc(BaseModel):
     """
-        Class for FiQuS CWS input file
+    Class for FiQuS CWS input file
     """
+
     field_map: CWSPostproc_FieldMap = CWSPostproc_FieldMap()
-    inductance: CWSPostproc_Inductance = CWSPostproc_Inductance()
-    temperature_map: CWSPostproc_TemperatureMap = CWSPostproc_TemperatureMap()
-    circuit_values: CWSPostproc_CircuitValues = CWSPostproc_CircuitValues()
+    temperature_map: CWSPostprocTemperature = CWSPostprocTemperature()
+    temperature_sensors: CWSPostprocTemperature = CWSPostprocTemperature()
+    inductance: CWSPostprocStaticOrTransient = CWSPostprocStaticOrTransient()
+    circuit_values: CWSPostprocCircuitValues = CWSPostprocCircuitValues()
+    field_coils: CWSPostprocStaticOrTransient = CWSPostprocStaticOrTransient()
 
 
 class CWS(BaseModel):
     """
-        Level 1: Class for FiQuS CWS
+    Level 1: Class for FiQuS CWS
     """
-    type: Literal['CWS']
+
+    type: Literal["CWS"]
     geometry: CWSGeometry = CWSGeometry()
     mesh: CWSMesh = CWSMesh()
     solve: CWSSolve = CWSSolve()
     postproc: CWSPostproc = CWSPostproc()
 
 
 # Multipole
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataFiQuSOptions.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataFiQuSOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataLEDET.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataLEDETOptions.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataLEDETOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataModelCircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,28 +50,27 @@
     """
     component_libraries: List[str] = []
 
 
 class Magnet(BaseModel):
     name: Optional[str] = None
     L_mag: Optional[float] = None
-    C_ground: Optional[float] =None
+    C_ground: Optional[float] = None
     Field_interp_value: Optional[float] = None
 
 class TFMClass(BaseModel):
     flag_PC: Optional[bool] = False
     flag_ISCC: Optional[bool] = False
     flag_IFCC: Optional[bool] = False
-    flag_EC: Optional[bool] = False
-    flag_Wedges: Optional[bool] = False
-    flag_ColdBore: Optional[bool] = False
+    flag_ED: Optional[bool] = False
+    flag_Wedge: Optional[bool] = False
+    flag_CB: Optional[bool] = False
     flag_BS: Optional[bool] = False
-    flag_Roxie: Optional[bool] = False
     M_IF_PC: Optional[float] = None
-    M_CB_Wedges: Optional[float] = None
+    M_CB_Wedge: Optional[float] = None
     T: Optional[float] = None
     Magnets: Dict[str, Magnet] = {}
 
 
 ############################
 # Global parameters
 class Global_Parameters(BaseModel):
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataModelCommon.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataModelCommon.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataModelCosim.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataModelCosim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataModelParsimDakota.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataModelParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataPlot.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataPlot.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataProteCCTOptions.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataProteCCTOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataPyBBQOptions.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataPyBBQOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataPyCoSim.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataPySIGMA.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataPySIGMAOptions.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataPySIGMAOptions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataSettings.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataSignal.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DataTFM.py` & `steam-sdk-2024.5.4/steam_sdk/data/DataTFM.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,32 +47,34 @@
     diameter: np.ndarray = field(default_factory=lambda: np.array([]))
     d_filamentary: np.ndarray = field(default_factory=lambda: np.array([]))
     d_core: np.ndarray = field(default_factory=lambda: np.array([]))
     fsc: np.ndarray = field(default_factory=lambda: np.array([]))
     f_rho_effective: np.ndarray = field(default_factory=lambda: np.array([]))
     fil_twist_pitch: np.ndarray = field(default_factory=lambda: np.array([]))
     RRR: np.ndarray = field(default_factory=lambda: np.array([]))
-    f_mag_X: np.ndarray = field(default_factory=lambda: np.array([]))
-    f_mag_Y: np.ndarray = field(default_factory=lambda: np.array([]))
-    f_mag: np.ndarray = field(default_factory=lambda: np.array([]))
+    f_mag_X_Roxie: np.ndarray = field(default_factory=lambda: np.array([]))
+    f_mag_Y_Roxie: np.ndarray = field(default_factory=lambda: np.array([]))
+    f_mag_Roxie: np.ndarray = field(default_factory=lambda: np.array([]))
+    f_mag_Comsol: np.ndarray = field(default_factory=lambda: np.array([]))
+    f_mag_X_Comsol: np.ndarray = field(default_factory=lambda: np.array([]))
+    f_mag_Y_Comsol: np.ndarray = field(default_factory=lambda: np.array([]))
     strands_to_conductor: np.ndarray = field(default_factory=lambda: np.array([]))
     strands_to_coil_sections: np.ndarray = field(default_factory=lambda: np.array([]))
 
 
 @dataclass
 class Options:
     flag_SC: Optional[bool] = True
     flag_PC: Optional[bool] = False
-    flag_IFCC: Optional[bool] = False
     flag_ISCC: Optional[bool] = False
-    flag_Wedges: Optional[bool] = False
-    flag_ColdBore: Optional[bool] = False
-    flag_EC: Optional[bool] = False
+    flag_IFCC: Optional[bool] = False
+    flag_ED: Optional[bool] = False
+    flag_Wedge: Optional[bool] = False
+    flag_CB: Optional[bool] = False
     flag_BS: Optional[bool] = False
-    flag_Roxie: Optional[bool] = False
 
 @dataclass
 class PC:  # DataClass for persistent current
     L: np.ndarray = field(default_factory=lambda: np.array([]))  # Inductance for PC modelisation
     I: np.ndarray = field(default_factory=lambda: np.array([]))  # Current generator for PC modelisation
     M: np.ndarray = field(default_factory=lambda: np.array([]))  # Coupling factor for PC modelisation
     M_IF_PC: np.ndarray = field(default_factory=lambda: np.array([]))  # Coupling factor between PC currents and interfilament currents
@@ -92,33 +94,33 @@
     R: np.ndarray = field(default_factory=lambda: np.array([]))
     M: np.ndarray = field(default_factory=lambda: np.array([]))
     P: np.ndarray = field(default_factory=lambda: np.array([]))
     I: np.ndarray = field(default_factory=lambda: np.array([]))
     tau: np.ndarray = field(default_factory=lambda: np.array([]))
 
 @dataclass
-class EC_CopperSheath:
+class ED:
     L: np.ndarray = field(default_factory=lambda: np.array([]))
     R: np.ndarray = field(default_factory=lambda: np.array([]))
     M: np.ndarray = field(default_factory=lambda: np.array([]))
     P: np.ndarray = field(default_factory=lambda: np.array([]))
     I: np.ndarray = field(default_factory=lambda: np.array([]))
     tau: np.ndarray = field(default_factory=lambda: np.array([]))
 
 @dataclass
-class Wedges:
+class Wedge:
     RRR_wedges: np.ndarray = field(default_factory=lambda: np.array([]))
     L: np.ndarray = field(default_factory=lambda: np.array([]))
     R: np.ndarray = field(default_factory=lambda: np.array([]))
     M: np.ndarray = field(default_factory=lambda: np.array([]))
     I: np.ndarray = field(default_factory=lambda: np.array([]))
     P: np.ndarray = field(default_factory=lambda: np.array([]))
     tau: np.ndarray = field(default_factory=lambda: np.array([]))
 
 @dataclass
-class ColdBore:
+class CB:
     L: np.ndarray = field(default_factory=lambda: np.array([]))
     R: np.ndarray = field(default_factory=lambda: np.array([]))
     M: np.ndarray = field(default_factory=lambda: np.array([]))
     I: np.ndarray = field(default_factory=lambda: np.array([]))
     P: np.ndarray = field(default_factory=lambda: np.array([]))
     tau: np.ndarray = field(default_factory=lambda: np.array([]))
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2024.5.4/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2024.5.4/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2024.5.4/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2024.5.4/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2024.5.4/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/drivers/DriverANSYS.py` & `steam-sdk-2024.5.4/steam_sdk/drivers/DriverANSYS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2024.5.4/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2024.5.4/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2024.5.4/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2024.5.4/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2024.5.4/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2024.5.4/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/drivers/DriverPySIGMA.py` & `steam-sdk-2024.5.4/steam_sdk/drivers/DriverPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2024.5.4/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserCOSIM.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserCOSIM.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserFile.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserFile.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPSPICE.py`

 * *Files 1% similar despite different names*

```diff
@@ -713,55 +713,55 @@
 def add_initial_condition(name: str, value: str):
     ''' Format initial condition row '''
     formatted_text = '.IC ' + name + ' {' + str(value) + '}'
     return formatted_text
 
 def add_standard_component(name: str, nodes: list, value: str):
     ''' Format standard component netlist row '''
-    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    str_nodes = " ".join(map(str, nodes))   # string with space-separated nodes
     formatted_text = name + ' (' + str_nodes + ') ' + '{' + str(value) + '}'
     return formatted_text
 
 def add_Diode_component(name: str, nodes: list, value: str):
     ''' Format Diode component netlist row '''
-    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    str_nodes = " ".join(map(str, nodes))   # string with space-separated nodes
     formatted_text = name + ' (' + str_nodes + ') ' + str(value)
     return formatted_text
 
 def add_stimulus_controlled_component(name: str, nodes: list, value: str):
     ''' Format stimulus-controlled component netlist row '''
-    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    str_nodes = " ".join(map(str, nodes))   # string with space-separated nodes
     str_stimulus = 'STIMULUS = ' + value
     formatted_text = name + ' (' + str_nodes + ') ' + str_stimulus
     return formatted_text
 
 def add_pulsed_source_component(name: str, nodes: list, value: str):
     ''' Format pulsed-source component netlist row '''
-    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    str_nodes = " ".join(map(str, nodes))   # string with space-separated nodes
     str_pulse = 'PULSE(' + str(value) + ')'
     formatted_text = name + ' (' + str_nodes + ') ' + str_pulse
     return formatted_text
 
 def add_controlled_source_component(name: str, nodes: list, value: str):
     ''' Format controlled-source component netlist row '''
-    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    str_nodes = " ".join(map(str, nodes))   # string with space-separated nodes
     str_stimulus = 'VALUE ' + '{' + value + '}'
     formatted_text = name + ' (' + str_nodes + ') ' + str_stimulus
     return formatted_text
 
 def add_transient_source_component(name: str, nodes: list, value: str):
     ''' Format controlled-source component netlist row '''
-    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    str_nodes = " ".join(map(str, nodes))   # string with space-separated nodes
     str_stimulus = 'AC ' + '{' + value + '}'
     formatted_text = name + ' (' + str_nodes + ') ' + str_stimulus
     return formatted_text
 
 def add_parametrized_component(name: str, nodes: list, value: str, parameters: dict):
     ''' Format parametrized component netlist row '''
-    str_nodes = " ".join(nodes)  # string with space-separated nodes
+    str_nodes = " ".join(map(str, nodes))   # string with space-separated nodes
     formatted_component = name + ' (' + str_nodes + ') ' + value  # First row, which defines the component
     if parameters:
         formatted_component = formatted_component + '\n'
         formatted_parameters = '+ PARAMS:'  # First part of the string in the second row, which defines the component parameters
         # for parameter in parameters:
         #     if len(parameter) != 2:
         #         raise Exception ('All parameters entries in a parametrized element must have 2 elements (name, value), but parameter {} has {} elements.'.format(name, len(parameter)))
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserPyBBQ.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserPyCoSim.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPyCoSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserPySIGMA.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserPySIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/utils_ParserCircuits.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/utils_ParserCircuits.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsers/utils_ParserCosims.py` & `steam-sdk-2024.5.4/steam_sdk/parsers/utils_ParserCosims.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2024.5.4/steam_sdk/parsims/ParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2024.5.4/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2024.5.4/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2024.5.4/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml` & `steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/parsims/translation_dicts/event_column_names.yaml` & `steam-sdk-2024.5.4/steam_sdk/parsims/translation_dicts/event_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/plotters/PlotterGriddedData.py` & `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterGriddedData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2024.5.4/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2024.5.4/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2024.5.4/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 import os
 from pathlib import Path
 import yaml
 from steam_sdk.data.DataModelMagnet import DataModelMagnet
-from steam_sdk.parsers.ParserYAML import model_data_to_yaml
+from steam_sdk.parsers.ParserYAML import model_data_to_yaml, yaml_to_data
 
 if __name__ == "__main__":  # pragma: no cover
     # path_to_models = Path.joinpath(
     #     Path(__file__).parent.parent.parent,
     #     "C:\\Users\emm\cernbox\SWAN_projects\steam_models\magnets",
     # )
     path_to_models = Path.joinpath(
-        Path(__file__).parent.parent.parent, r"D:\Code_new\steam_models\magnets")
+        Path(__file__).parent.parent.parent, r"E:\Python311\steam_models\magnets")
 
     # path_to_models = Path.joinpath(
     #     Path(__file__).parent.parent.parent, "tests/builders/model_library/magnets"
     # )
     model_names = [x.parts[-1] for x in Path(path_to_models).iterdir() if x.is_dir()]
     #model_names = ['MCBRD']
-
+    #model_names = ['CWS_1']
     for model_name in model_names:
+        print(model_name)
         # Read the file:
         yaml_file = Path.joinpath(
             path_to_models, model_name, "input", "modelData_" + model_name + ".yaml"
         )
         if os.path.isfile(yaml_file):
             # Read the yaml file and store the date inside ruamel_yaml_object:
-            with open(yaml_file, "r") as stream:
-                ruamel_yaml_object = yaml.safe_load(stream)
-
-            print(f"The file has been read: {yaml_file}")
-
-            # Create a DataModelMagnet object from the yaml file's data:
-            # Note: Obsolete keys (the keys that are not in DataModelMagnet) will
-            # automatically be deleted. Moreover, if new keys are added to
-            # DataModelMagnet, they will be added to the YAML file. The new key's values
-            # will be DataModelMagnet's default values.
-            # del ruamel_yaml_object["Options_FiQuS"]["Pancake3D"]
-            model_data = DataModelMagnet(**ruamel_yaml_object)
-
+            # with open(yaml_file, "r") as stream:
+            #     ruamel_yaml_object = yaml.safe_load(stream)
+            #
+            # print(f"The file has been read: {yaml_file}")
+            #
+            # # Create a DataModelMagnet object from the yaml file's data:
+            # # Note: Obsolete keys (the keys that are not in DataModelMagnet) will
+            # # automatically be deleted. Moreover, if new keys are added to
+            # # DataModelMagnet, they will be added to the YAML file. The new key's values
+            # # will be DataModelMagnet's default values.
+            # # del ruamel_yaml_object["Options_FiQuS"]["Pancake3D"]
+            # model_data = DataModelMagnet(**ruamel_yaml_object)
+            model_data = yaml_to_data(yaml_file, DataModelMagnet)
+            # model_data.Options_FiQuS.cws.geometry.iterative_fragment = False
+            # model_data.Options_FiQuS.cws.mesh.temperature_sensors.enabled = False
+            # model_data.Options_FiQuS.cws.mesh.heaters.enabled = False
+            # model_data.Options_FiQuS.cws.mesh.field_coils.enabled = False
+            # model_data.Options_FiQuS.cws.solve.formers.use = 'function'
+            # model_data.Options_FiQuS.cws.solve.shells.use = 'function'
             # Some values of the new and old keys can be changed like this:
             # model_data.Options_LEDET.magnet_inductance.flag_calculate_inductance = True
 
             # Old values of obsolete keys can be moved to new keys like this:
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.mirrorY_ht = (
             #     ruamel_yaml_object["CoilWindings"]["multipole"]["mirrorY_ht"]
             # )
```

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2024.5.4/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/ParserRoxieHelpers.py` & `steam-sdk-2024.5.4/steam_sdk/utils/ParserRoxieHelpers.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/attribute_model.py` & `steam-sdk-2024.5.4/steam_sdk/utils/attribute_model.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2024.5.4/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/compare_simulations.py` & `steam-sdk-2024.5.4/steam_sdk/utils/compare_simulations.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2024.5.4/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/correct_RRR_NIST.py` & `steam-sdk-2024.5.4/steam_sdk/utils/correct_RRR_NIST.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2024.5.4/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/make_folder_if_not_existing.py` & `steam-sdk-2024.5.4/steam_sdk/utils/make_folder_if_not_existing.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/misc.py` & `steam-sdk-2024.5.4/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2024.5.4/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/read_settings_file.py` & `steam-sdk-2024.5.4/steam_sdk/utils/read_settings_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/reformat_figure.py` & `steam-sdk-2024.5.4/steam_sdk/utils/reformat_figure.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/tic_toc.py` & `steam-sdk-2024.5.4/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/utils/utils_PC.py` & `steam-sdk-2024.5.4/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/viewers/Viewer.py` & `steam-sdk-2024.5.4/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2024.5.4/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2024.5.3/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2024.5.4/steam_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2024.5.3
+Version: 2024.5.4
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
-Keywords: STEAM,CERN,API,SDK
+Keywords: SDK,STEAM,API,CERN
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh==4.11.1
 Requires-Dist: matplotlib==3.8.3
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: numpy==1.26.4
@@ -30,14 +30,15 @@
 Requires-Dist: seaborn==0.13.2
 Requires-Dist: STEAM-materials==2024.4.2
 Requires-Dist: svglib==1.5.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: steam-pysigma==2024.3.2
 Requires-Dist: pyarrow==15.0.1
 Requires-Dist: tqdm==4.66.2
+Requires-Dist: mplcursors==0.5.3
 Provides-Extra: all
 Requires-Dist: gmsh==4.11.1; extra == "all"
 Requires-Dist: matplotlib==3.8.3; extra == "all"
 Requires-Dist: Jinja2==3.1.3; extra == "all"
 Requires-Dist: numpy==1.26.4; extra == "all"
 Requires-Dist: pandas==2.2.1; extra == "all"
 Requires-Dist: pydantic==2.6.4; extra == "all"
@@ -56,14 +57,15 @@
 Requires-Dist: seaborn==0.13.2; extra == "all"
 Requires-Dist: STEAM-materials==2024.4.2; extra == "all"
 Requires-Dist: svglib==1.5.1; extra == "all"
 Requires-Dist: PyYAML==6.0.1; extra == "all"
 Requires-Dist: steam-pysigma==2024.3.2; extra == "all"
 Requires-Dist: pyarrow==15.0.1; extra == "all"
 Requires-Dist: tqdm==4.66.2; extra == "all"
+Requires-Dist: mplcursors==0.5.3; extra == "all"
 Requires-Dist: Markdown==3.5.2; extra == "all"
 Requires-Dist: markdown-include==0.8.1; extra == "all"
 Requires-Dist: MarkupSafe==2.1.5; extra == "all"
 Requires-Dist: mkdocs==1.5.3; extra == "all"
 Requires-Dist: mkdocs-autorefs==1.0.1; extra == "all"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == "all"
 Requires-Dist: mkdocs-include-markdown-plugin==6.0.4; extra == "all"
```

### Comparing `steam-sdk-2024.5.3/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2024.5.4/steam_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 steam_sdk/drivers/DriverLEDET.py
 steam_sdk/drivers/DriverPSPICE.py
 steam_sdk/drivers/DriverProteCCT.py
 steam_sdk/drivers/DriverPyBBQ.py
 steam_sdk/drivers/DriverPySIGMA.py
 steam_sdk/drivers/DriverXYCE.py
 steam_sdk/drivers/__init__.py
-steam_sdk/drivers/to_DELETE.py
 steam_sdk/parsers/CSD_Reader.py
 steam_sdk/parsers/ParserCOMSOLToTxt.py
 steam_sdk/parsers/ParserCOSIM.py
 steam_sdk/parsers/ParserCond2d.py
 steam_sdk/parsers/ParserCsd.py
 steam_sdk/parsers/ParserCsv.py
 steam_sdk/parsers/ParserDakota.py
@@ -154,22 +153,18 @@
 steam_sdk/utils/__init__.py
 steam_sdk/utils/attribute_model.py
 steam_sdk/utils/clean_NaN_from_signal.py
 steam_sdk/utils/compare_simulations.py
 steam_sdk/utils/compare_two_parameters.py
 steam_sdk/utils/correct_RRR_NIST.py
 steam_sdk/utils/delete_if_existing.py
-steam_sdk/utils/find_delete_files.py
 steam_sdk/utils/get_attribute_type.py
 steam_sdk/utils/isNaN.py
 steam_sdk/utils/make_folder_if_not_existing.py
-steam_sdk/utils/make_json_schema.py
 steam_sdk/utils/misc.py
-steam_sdk/utils/overwrite_files.py
-steam_sdk/utils/overwrite_output_to_reference_files.py
 steam_sdk/utils/parse_str_to_list.py
 steam_sdk/utils/read_settings_file.py
 steam_sdk/utils/reformat_figure.py
 steam_sdk/utils/rgetattr.py
 steam_sdk/utils/rhasattr.py
 steam_sdk/utils/sgetattr.py
 steam_sdk/utils/tic_toc.py
```

### Comparing `steam-sdk-2024.5.3/steam_sdk.egg-info/requires.txt` & `steam-sdk-2024.5.4/steam_sdk.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 seaborn==0.13.2
 STEAM-materials==2024.4.2
 svglib==1.5.1
 PyYAML==6.0.1
 steam-pysigma==2024.3.2
 pyarrow==15.0.1
 tqdm==4.66.2
+mplcursors==0.5.3
 
 [all]
 gmsh==4.11.1
 matplotlib==3.8.3
 Jinja2==3.1.3
 numpy==1.26.4
 pandas==2.2.1
@@ -46,14 +47,15 @@
 seaborn==0.13.2
 STEAM-materials==2024.4.2
 svglib==1.5.1
 PyYAML==6.0.1
 steam-pysigma==2024.3.2
 pyarrow==15.0.1
 tqdm==4.66.2
+mplcursors==0.5.3
 Markdown==3.5.2
 markdown-include==0.8.1
 MarkupSafe==2.1.5
 mkdocs==1.5.3
 mkdocs-autorefs==1.0.1
 mkdocs-git-revision-date-localized-plugin==1.2.4
 mkdocs-include-markdown-plugin==6.0.4
```

