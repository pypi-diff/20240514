# Comparing `tmp/powergenome-0.6.2.tar.gz` & `tmp/powergenome-0.6.3.tar.gz`

## Comparing `powergenome-0.6.2.tar` & `powergenome-0.6.3.tar`

### file list

```diff
@@ -1,83 +1,40 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 powergenome-0.6.2/.codecov.yml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 powergenome-0.6.2/.git-blame-ignore-revs
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 powergenome-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 powergenome-0.6.2/.travis.yml
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 powergenome-0.6.2/.zenodo.json
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 powergenome-0.6.2/environment.yml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 powergenome-0.6.2/requirements.txt
--rw-r--r--   0        0        0  7754322 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/ipm_regions_simple.geojson
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/AZ_additional_tech.csv
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/AZ_additional_tech_2030.csv
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/AZ_additional_tech_2045.csv
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/additional tech documentation.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/sample_additional_tech.csv
--rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/coal_fgd/fgd_output.csv
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/cost_multipliers/EIA regional cost multipliers.csv
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/cpi_data/cpi_data.csv
--rw-r--r--   0        0        0    12734 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/issue_settings.yaml
--rw-r--r--   0        0        0    49625 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/log.txt
--rw-r--r--   0        0        0    77755 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/2030/p1_2030_Full_timeseries/Inputs/Fuels_data.csv
--rw-r--r--   0        0        0   462368 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/2030/p1_2030_Full_timeseries/extra_outputs/existing_gen_units.csv
--rw-r--r--   0        0        0    77755 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/Fuels_data.csv
--rw-r--r--   0        0        0    75207 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_LandbasedWind_Class3_Moderate__site_cluster_assignments.csv
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_OffShoreWind_Class12_Moderate_floating_0_site_cluster_assignments.csv
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_OffShoreWind_Class12_Moderate_floating_1_site_cluster_assignments.csv
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_OffShoreWind_Class3_Moderate_fixed_0_site_cluster_assignments.csv
--rw-r--r--   0        0        0    23159 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_OffShoreWind_Class3_Moderate_fixed_1_site_cluster_assignments.csv
--rw-r--r--   0        0        0   401505 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_UtilityPV_Class1_Moderate__site_cluster_assignments.csv
--rw-r--r--   0        0        0   288788 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_LandbasedWind_Class3_Moderate__site_cluster_assignments.csv
--rw-r--r--   0        0        0    97421 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_OffShoreWind_Class12_Moderate_floating_0_site_cluster_assignments.csv
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_OffShoreWind_Class12_Moderate_floating_1_site_cluster_assignments.csv
--rw-r--r--   0        0        0    86283 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_OffShoreWind_Class3_Moderate_fixed_0_site_cluster_assignments.csv
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_OffShoreWind_Class3_Moderate_fixed_1_site_cluster_assignments.csv
--rw-r--r--   0        0        0  1881138 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_UtilityPV_Class1_Moderate__site_cluster_assignments.csv
--rw-r--r--   0        0        0   140067 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_LandbasedWind_Class3_Moderate__site_cluster_assignments.csv
--rw-r--r--   0        0        0    51701 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_OffShoreWind_Class12_Moderate_floating_0_site_cluster_assignments.csv
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_OffShoreWind_Class12_Moderate_floating_1_site_cluster_assignments.csv
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_OffShoreWind_Class3_Moderate_fixed_0_site_cluster_assignments.csv
--rw-r--r--   0        0        0   861463 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_UtilityPV_Class1_Moderate__site_cluster_assignments.csv
--rw-r--r--   0        0        0   479171 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/existing_gen_units.csv
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/demand.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/distributed_gen.yml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/env.yml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/extra_inputs.yml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/flexible_load.yml
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/fuels.yml
--rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/model_definition.yml
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/resource_tags.yml
--rw-r--r--   0        0        0    15057 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/resources.yml
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/scenario_management.yml
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/startup_costs.yml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/time_clustering.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/transmission.yml
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/.coveragerc
--rw-r--r--   0        0        0    46651 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/GenX.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/__init__.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/cluster_method.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/co2_pipeline_cost.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/debug.py
--rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/distributed_gen.py
--rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/eia_opendata.py
--rw-r--r--   0        0        0    22359 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/external_data.py
--rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/extract_pudl_data.py
--rw-r--r--   0        0        0    13023 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/financials.py
--rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/fuels.py
--rw-r--r--   0        0        0   149932 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/generators.py
--rw-r--r--   0        0        0    11200 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/load_construction.py
--rw-r--r--   0        0        0    33914 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/load_profiles.py
--rw-r--r--   0        0        0    67403 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/nrelatb.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/params.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/price_adjustment.py
--rw-r--r--   0        0        0    46177 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/resource_clusters.py
--rw-r--r--   0        0        0    22404 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/run_powergenome_multiple_outputs_cli.py
--rw-r--r--   0        0        0    18819 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/time_reduction.py
--rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/transmission.py
--rw-r--r--   0        0        0    49513 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/util.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/version.py
--rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/cluster/renewables.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 powergenome-0.6.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 powergenome-0.6.2/LICENSE.md
--rw-r--r--   0        0        0    17355 2020-02-02 00:00:00.000000 powergenome-0.6.2/README.md
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 powergenome-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    18797 2020-02-02 00:00:00.000000 powergenome-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0  7754322 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/ipm_regions_simple.geojson
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/additional_technologies/AZ_additional_tech.csv
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/additional_technologies/AZ_additional_tech_2030.csv
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/additional_technologies/AZ_additional_tech_2045.csv
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/additional_technologies/additional tech documentation.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/additional_technologies/sample_additional_tech.csv
+-rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/coal_fgd/fgd_output.csv
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/cost_multipliers/EIA regional cost multipliers.csv
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 powergenome-0.6.3/data/cpi_data/cpi_data.csv
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/.coveragerc
+-rw-r--r--   0        0        0    46651 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/GenX.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/__init__.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/cluster_method.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/co2_pipeline_cost.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/debug.py
+-rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/distributed_gen.py
+-rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/eia_opendata.py
+-rw-r--r--   0        0        0    22359 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/external_data.py
+-rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/extract_pudl_data.py
+-rw-r--r--   0        0        0    13023 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/financials.py
+-rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/fuels.py
+-rw-r--r--   0        0        0   149932 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/generators.py
+-rw-r--r--   0        0        0    11200 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/load_construction.py
+-rw-r--r--   0        0        0    33914 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/load_profiles.py
+-rw-r--r--   0        0        0    67403 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/nrelatb.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/params.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/price_adjustment.py
+-rw-r--r--   0        0        0    46177 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/resource_clusters.py
+-rw-r--r--   0        0        0    22404 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/run_powergenome_multiple_outputs_cli.py
+-rw-r--r--   0        0        0    18819 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/time_reduction.py
+-rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/transmission.py
+-rw-r--r--   0        0        0    49513 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/util.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/version.py
+-rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 powergenome-0.6.3/powergenome/cluster/renewables.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 powergenome-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 powergenome-0.6.3/LICENSE.md
+-rw-r--r--   0        0        0    17355 2020-02-02 00:00:00.000000 powergenome-0.6.3/README.md
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 powergenome-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    18797 2020-02-02 00:00:00.000000 powergenome-0.6.3/PKG-INFO
```

### Comparing `powergenome-0.6.2/data/ipm_regions_simple.geojson` & `powergenome-0.6.3/data/ipm_regions_simple.geojson`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/data/additional_technologies/AZ_additional_tech.csv` & `powergenome-0.6.3/data/additional_technologies/AZ_additional_tech.csv`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/data/additional_technologies/AZ_additional_tech_2030.csv` & `powergenome-0.6.3/data/additional_technologies/AZ_additional_tech_2030.csv`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/data/additional_technologies/AZ_additional_tech_2045.csv` & `powergenome-0.6.3/data/additional_technologies/AZ_additional_tech_2045.csv`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/data/additional_technologies/additional tech documentation.md` & `powergenome-0.6.3/data/additional_technologies/additional tech documentation.md`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/data/additional_technologies/sample_additional_tech.csv` & `powergenome-0.6.3/data/additional_technologies/sample_additional_tech.csv`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/data/coal_fgd/fgd_output.csv` & `powergenome-0.6.3/data/coal_fgd/fgd_output.csv`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv` & `powergenome-0.6.3/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/data/cost_multipliers/EIA regional cost multipliers.csv` & `powergenome-0.6.3/data/cost_multipliers/EIA regional cost multipliers.csv`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/data/cpi_data/cpi_data.csv` & `powergenome-0.6.3/data/cpi_data/cpi_data.csv`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/GenX.py` & `powergenome-0.6.3/powergenome/GenX.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/cluster_method.py` & `powergenome-0.6.3/powergenome/cluster_method.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/co2_pipeline_cost.py` & `powergenome-0.6.3/powergenome/co2_pipeline_cost.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/debug.py` & `powergenome-0.6.3/powergenome/debug.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/distributed_gen.py` & `powergenome-0.6.3/powergenome/distributed_gen.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/eia_opendata.py` & `powergenome-0.6.3/powergenome/eia_opendata.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/external_data.py` & `powergenome-0.6.3/powergenome/external_data.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/extract_pudl_data.py` & `powergenome-0.6.3/powergenome/extract_pudl_data.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/financials.py` & `powergenome-0.6.3/powergenome/financials.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/fuels.py` & `powergenome-0.6.3/powergenome/fuels.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/generators.py` & `powergenome-0.6.3/powergenome/generators.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/load_construction.py` & `powergenome-0.6.3/powergenome/load_construction.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/load_profiles.py` & `powergenome-0.6.3/powergenome/load_profiles.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/nrelatb.py` & `powergenome-0.6.3/powergenome/nrelatb.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/params.py` & `powergenome-0.6.3/powergenome/params.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 DATA_PATHS["ipm_shapefiles"] = DATA_PATHS["data"] / "IPM Regions v617 04-05-17"
 DATA_PATHS["tests"] = project_path / "tests"
 DATA_PATHS["test_data"] = DATA_PATHS["tests"] / "data"
 DATA_PATHS["settings"] = project_path / "settings"
 DATA_PATHS["eia"] = DATA_PATHS["data"] / "eia"
 DATA_PATHS["eia_860m"] = DATA_PATHS["eia"] / "860m"
 DATA_PATHS["cost_multipliers"] = DATA_PATHS["data"] / "cost_multipliers"
-DATA_PATHS["cache"] = DATA_PATHS["data"] / "cache"
-DATA_PATHS["cache"].mkdir(exist_ok=True)
 DATA_PATHS["additional_techs"] = DATA_PATHS["data"] / "additional_technologies"
 DATA_PATHS["coal_fgd"] = DATA_PATHS["data"] / "coal_fgd" / "fgd_output.csv"
 DATA_PATHS["cpi_data"] = DATA_PATHS["data"] / "cpi_data" / "cpi_data.csv"
 
 IPM_SHAPEFILE_PATH = DATA_PATHS["ipm_shapefiles"] / "IPM_Regions_201770405.shp"
 IPM_GEOJSON_PATH = DATA_PATHS["data"] / "ipm_regions_simple.geojson"
```

### Comparing `powergenome-0.6.2/powergenome/price_adjustment.py` & `powergenome-0.6.3/powergenome/price_adjustment.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/resource_clusters.py` & `powergenome-0.6.3/powergenome/resource_clusters.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/run_powergenome_multiple_outputs_cli.py` & `powergenome-0.6.3/powergenome/run_powergenome_multiple_outputs_cli.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/time_reduction.py` & `powergenome-0.6.3/powergenome/time_reduction.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/transmission.py` & `powergenome-0.6.3/powergenome/transmission.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/util.py` & `powergenome-0.6.3/powergenome/util.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/powergenome/cluster/renewables.py` & `powergenome-0.6.3/powergenome/cluster/renewables.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/.gitignore` & `powergenome-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/LICENSE.md` & `powergenome-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/README.md` & `powergenome-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.2/pyproject.toml` & `powergenome-0.6.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -38,24 +38,22 @@
     "geopandas>=0.11",
 ]
 
 [tool.hatch.version]
 path = "powergenome/version.py"
 
 [tool.hatch.build.targets.sdist]
-exclude = [
-    "/.github",
-    "/docs",
-    "/notebooks",
-    "/data/eia*",
-    "/tests",
-    "/bin",
-    "/example_systems",
-    "/wiki",
-]
+only-include = ["powergenome", "data"]
+exclude = ["/data/eia*"]
+
+
+[tool.hatch.build.targets.wheel]
+only-include = ["powergenome", "data"]
+exclude = ["/data/eia*"]
+
 
 [project.optional-dependencies]
 dev = [
     "black[jupyter] == 24.3.0",
     "pre-commit",
     "pytest",
     "isort",
```

### Comparing `powergenome-0.6.2/PKG-INFO` & `powergenome-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PowerGenome
-Version: 0.6.2
+Version: 0.6.3
 Summary: Create power system inputs for capacity expansion models
 Project-URL: Source, https://github.com/PowerGenome/PowerGenome
 Author-email: Greg Schivley <greg.schivley@princeton.edu>
 Maintainer-email: Greg Schivley <greg.schivley@princeton.edu>
 License: MIT
 License-File: LICENSE.md
 Keywords: capacity expansion,power system data,two
```

