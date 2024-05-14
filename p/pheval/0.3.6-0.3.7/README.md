# Comparing `tmp/pheval-0.3.6.tar.gz` & `tmp/pheval-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheval-0.3.6.tar", max compression
+gzip compressed data, was "pheval-0.3.7.tar", max compression
```

## Comparing `pheval-0.3.6.tar` & `pheval-0.3.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11357 2024-05-10 19:16:19.207976 pheval-0.3.6/LICENSE
--rw-r--r--   0        0        0      751 2024-05-10 19:16:19.207976 pheval-0.3.6/README.md
--rw-r--r--   0        0        0     1529 2024-05-10 19:16:19.267976 pheval-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/__init__.py
--rw-r--r--   0        0        0     7743 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/analysis.py
--rw-r--r--   0        0        0     5943 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/benchmark_generator.py
--rw-r--r--   0        0        0      768 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/benchmarking_data.py
--rw-r--r--   0        0        0    12519 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/binary_classification_stats.py
--rw-r--r--   0        0        0    12649 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/disease_prioritisation_analysis.py
--rw-r--r--   0        0        0    12373 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/gene_prioritisation_analysis.py
--rw-r--r--   0        0        0    21350 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/generate_plots.py
--rw-r--r--   0        0        0     6591 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/generate_summary_outputs.py
--rw-r--r--   0        0        0     2384 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/parse_benchmark_summary.py
--rw-r--r--   0        0        0     1211 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/parse_pheval_result.py
--rw-r--r--   0        0        0     3223 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/prioritisation_rank_recorder.py
--rw-r--r--   0        0        0     1228 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/prioritisation_result_types.py
--rw-r--r--   0        0        0    15785 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/rank_stats.py
--rw-r--r--   0        0        0     1552 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/run_data_parser.py
--rw-r--r--   0        0        0    12384 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/variant_prioritisation_analysis.py
--rw-r--r--   0        0        0     1570 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/cli.py
--rw-r--r--   0        0        0     2424 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/cli_pheval.py
--rw-r--r--   0        0        0    20504 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/cli_pheval_utils.py
--rw-r--r--   0        0        0     1227 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/config_parser.py
--rw-r--r--   0        0        0      349 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/constants.py
--rw-r--r--   0        0        0     1228 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/infra/__init__.py
--rw-r--r--   0        0        0     5080 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/infra/exomiserdb.py
--rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/post_processing/__init__.py
--rw-r--r--   0        0        0    13368 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/post_processing/post_processing.py
--rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/prepare/__init__.py
--rw-r--r--   0        0        0    11236 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/prepare/create_noisy_phenopackets.py
--rw-r--r--   0        0        0    21111 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/prepare/create_spiked_vcf.py
--rw-r--r--   0        0        0     1719 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/prepare/custom_exceptions.py
--rw-r--r--   0        0        0     3692 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/prepare/prepare_corpus.py
--rw-r--r--   0        0        0     4770 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/prepare/update_phenopacket.py
--rw-r--r--   0        0        0      547 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/CADA_results.txt
--rw-r--r--   0        0        0     1508 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt
--rw-r--r--   0        0        0     9845 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/OVA_results.txt
--rw-r--r--   0        0        0    14148 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json
--rw-r--r--   0        0        0      594 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt
--rw-r--r--   0        0        0   431068 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/lirical_results.tsv
--rw-r--r--   0        0        0      714 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/svanna_results.tsv
--rw-r--r--   0        0        0 16462969 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/resources/hgnc_complete_set.txt
--rw-r--r--   0        0        0      919 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/run_metadata.py
--rw-r--r--   0        0        0        0 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/runners/__init__.py
--rw-r--r--   0        0        0     4451 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/runners/runner.py
--rw-r--r--   0        0        0        0 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/__init__.py
--rw-r--r--   0        0        0     3193 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/docs_gen.py
--rwxr-xr-x   0        0        0      477 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/docs_gen.sh
--rw-r--r--   0        0        0      683 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/exomiser.py
--rw-r--r--   0        0        0     4640 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/file_utils.py
--rw-r--r--   0        0        0    26792 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/phenopacket_utils.py
--rw-r--r--   0        0        0     6151 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/semsim_utils.py
--rw-r--r--   0        0        0     2343 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/utils.py
--rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 pheval-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 18:15:45.665955 pheval-0.3.7/LICENSE
+-rw-r--r--   0        0        0      751 2024-05-14 18:15:45.665955 pheval-0.3.7/README.md
+-rw-r--r--   0        0        0     1529 2024-05-14 18:15:45.721956 pheval-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 18:15:45.721956 pheval-0.3.7/src/pheval/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:15:45.721956 pheval-0.3.7/src/pheval/analyse/__init__.py
+-rw-r--r--   0        0        0     7743 2024-05-14 18:15:45.721956 pheval-0.3.7/src/pheval/analyse/analysis.py
+-rw-r--r--   0        0        0     5943 2024-05-14 18:15:45.721956 pheval-0.3.7/src/pheval/analyse/benchmark_generator.py
+-rw-r--r--   0        0        0      768 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/benchmarking_data.py
+-rw-r--r--   0        0        0    12519 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/binary_classification_stats.py
+-rw-r--r--   0        0        0    12451 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/disease_prioritisation_analysis.py
+-rw-r--r--   0        0        0    12190 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/gene_prioritisation_analysis.py
+-rw-r--r--   0        0        0    21350 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/generate_plots.py
+-rw-r--r--   0        0        0     6591 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/generate_summary_outputs.py
+-rw-r--r--   0        0        0     2384 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/parse_benchmark_summary.py
+-rw-r--r--   0        0        0     1438 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/parse_pheval_result.py
+-rw-r--r--   0        0        0     3223 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/prioritisation_rank_recorder.py
+-rw-r--r--   0        0        0     1228 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/prioritisation_result_types.py
+-rw-r--r--   0        0        0    15785 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/rank_stats.py
+-rw-r--r--   0        0        0     1552 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/run_data_parser.py
+-rw-r--r--   0        0        0    12186 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/analyse/variant_prioritisation_analysis.py
+-rw-r--r--   0        0        0     1570 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/cli.py
+-rw-r--r--   0        0        0     2424 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/cli_pheval.py
+-rw-r--r--   0        0        0    20504 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/cli_pheval_utils.py
+-rw-r--r--   0        0        0     1227 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/config_parser.py
+-rw-r--r--   0        0        0      349 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/constants.py
+-rw-r--r--   0        0        0     1228 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/infra/__init__.py
+-rw-r--r--   0        0        0     5080 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/infra/exomiserdb.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/post_processing/__init__.py
+-rw-r--r--   0        0        0    13329 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/post_processing/post_processing.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/prepare/__init__.py
+-rw-r--r--   0        0        0    11236 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/prepare/create_noisy_phenopackets.py
+-rw-r--r--   0        0        0    21111 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/prepare/create_spiked_vcf.py
+-rw-r--r--   0        0        0     1719 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/prepare/custom_exceptions.py
+-rw-r--r--   0        0        0     3692 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/prepare/prepare_corpus.py
+-rw-r--r--   0        0        0     4770 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/prepare/update_phenopacket.py
+-rw-r--r--   0        0        0      547 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/resources/alternate_ouputs/CADA_results.txt
+-rw-r--r--   0        0        0     1508 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt
+-rw-r--r--   0        0        0     9845 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/resources/alternate_ouputs/OVA_results.txt
+-rw-r--r--   0        0        0    14148 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json
+-rw-r--r--   0        0        0      594 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt
+-rw-r--r--   0        0        0   431068 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/resources/alternate_ouputs/lirical_results.tsv
+-rw-r--r--   0        0        0      714 2024-05-14 18:15:45.725956 pheval-0.3.7/src/pheval/resources/alternate_ouputs/svanna_results.tsv
+-rw-r--r--   0        0        0 16462969 2024-05-14 18:15:45.789957 pheval-0.3.7/src/pheval/resources/hgnc_complete_set.txt
+-rw-r--r--   0        0        0      919 2024-05-14 18:15:45.789957 pheval-0.3.7/src/pheval/run_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:15:45.789957 pheval-0.3.7/src/pheval/runners/__init__.py
+-rw-r--r--   0        0        0     4451 2024-05-14 18:15:45.789957 pheval-0.3.7/src/pheval/runners/runner.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:15:45.789957 pheval-0.3.7/src/pheval/utils/__init__.py
+-rw-r--r--   0        0        0     3193 2024-05-14 18:15:45.789957 pheval-0.3.7/src/pheval/utils/docs_gen.py
+-rwxr-xr-x   0        0        0      477 2024-05-14 18:15:45.789957 pheval-0.3.7/src/pheval/utils/docs_gen.sh
+-rw-r--r--   0        0        0      683 2024-05-14 18:15:45.789957 pheval-0.3.7/src/pheval/utils/exomiser.py
+-rw-r--r--   0        0        0     3576 2024-05-14 18:15:45.789957 pheval-0.3.7/src/pheval/utils/file_utils.py
+-rw-r--r--   0        0        0    26792 2024-05-14 18:15:45.793957 pheval-0.3.7/src/pheval/utils/phenopacket_utils.py
+-rw-r--r--   0        0        0     6151 2024-05-14 18:15:45.793957 pheval-0.3.7/src/pheval/utils/semsim_utils.py
+-rw-r--r--   0        0        0     2343 2024-05-14 18:15:45.793957 pheval-0.3.7/src/pheval/utils/utils.py
+-rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 pheval-0.3.7/PKG-INFO
```

### Comparing `pheval-0.3.6/LICENSE` & `pheval-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/README.md` & `pheval-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/pyproject.toml` & `pheval-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pheval"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>",
   "Julius Jacobsen <j.jacobsen@qmul.ac.uk>",
   "Nico Matentzoglu <nicolas.matentzoglu@gmail.com>",
   "Vinícius de Souza <souzadevinicius@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pheval", from = "src"}]
```

### Comparing `pheval-0.3.6/src/pheval/analyse/analysis.py` & `pheval-0.3.7/src/pheval/analyse/analysis.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/benchmark_generator.py` & `pheval-0.3.7/src/pheval/analyse/benchmark_generator.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/benchmarking_data.py` & `pheval-0.3.7/src/pheval/analyse/benchmarking_data.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/binary_classification_stats.py` & `pheval-0.3.7/src/pheval/analyse/binary_classification_stats.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/disease_prioritisation_analysis.py` & `pheval-0.3.7/src/pheval/analyse/disease_prioritisation_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 from pheval.analyse.binary_classification_stats import BinaryClassificationStats
 from pheval.analyse.parse_pheval_result import parse_pheval_result, read_standardised_result
 from pheval.analyse.prioritisation_rank_recorder import PrioritisationRankRecorder
 from pheval.analyse.prioritisation_result_types import DiseasePrioritisationResult
 from pheval.analyse.rank_stats import RankStats
 from pheval.analyse.run_data_parser import TrackInputOutputDirectories
 from pheval.post_processing.post_processing import RankedPhEvalDiseaseResult
-from pheval.utils.file_utils import (
-    all_files,
-    files_with_suffix,
-    obtain_phenopacket_path_from_pheval_result,
-)
+from pheval.utils.file_utils import all_files
 from pheval.utils.phenopacket_utils import PhenopacketUtil, ProbandDisease, phenopacket_reader
 
 
 class AssessDiseasePrioritisation:
     """Class for assessing disease prioritisation based on thresholds and scoring orders."""
 
     def __init__(
@@ -213,37 +209,37 @@
     """
     phenopacket = phenopacket_reader(phenopacket_path)
     phenopacket_util = PhenopacketUtil(phenopacket)
     return phenopacket_util.diagnoses()
 
 
 def assess_phenopacket_disease_prioritisation(
-    standardised_disease_result: Path,
+    phenopacket_path: Path,
     score_order: str,
     results_dir_and_input: TrackInputOutputDirectories,
     threshold: float,
     disease_rank_stats: RankStats,
     disease_rank_comparison: defaultdict,
     disease_binary_classification_stats: BinaryClassificationStats,
 ) -> None:
     """
     Assess disease prioritisation for a Phenopacket by comparing PhEval standardised disease results
     against the recorded causative diseases for a proband in the Phenopacket.
 
     Args:
-        standardised_disease_result (Path): Path to the PhEval standardised disease result file.
+        phenopacket_path (Path): Path to the Phenopacket.
         score_order (str): The order in which scores are arranged, either ascending or descending.
         results_dir_and_input (TrackInputOutputDirectories): Input and output directories.
         threshold (float): Threshold for assessment.
         disease_rank_stats (RankStats): RankStats class instance.
         disease_rank_comparison (defaultdict): Default dictionary for disease rank comparisons.
         disease_binary_classification_stats (BinaryClassificationStats): BinaryClassificationStats class instance.
     """
-    phenopacket_path = obtain_phenopacket_path_from_pheval_result(
-        standardised_disease_result, all_files(results_dir_and_input.phenopacket_dir)
+    standardised_disease_result = results_dir_and_input.results_dir.joinpath(
+        f"pheval_disease_results/{phenopacket_path.stem}-pheval_disease_result.tsv"
     )
     pheval_disease_result = read_standardised_result(standardised_disease_result)
     proband_diseases = _obtain_causative_diseases(phenopacket_path)
     AssessDiseasePrioritisation(
         phenopacket_path,
         results_dir_and_input.results_dir.joinpath("pheval_disease_results/"),
         parse_pheval_result(RankedPhEvalDiseaseResult, pheval_disease_result),
@@ -272,20 +268,17 @@
 
     Returns:
         BenchmarkRunResults: An object containing benchmarking results for disease prioritisation,
         including ranks and rank statistics for the benchmarked directory.
     """
     disease_rank_stats = RankStats()
     disease_binary_classification_stats = BinaryClassificationStats()
-    for standardised_result in files_with_suffix(
-        results_directory_and_input.results_dir.joinpath("pheval_disease_results/"),
-        ".tsv",
-    ):
+    for phenopacket_path in all_files(results_directory_and_input.phenopacket_dir):
         assess_phenopacket_disease_prioritisation(
-            standardised_result,
+            phenopacket_path,
             score_order,
             results_directory_and_input,
             threshold,
             disease_rank_stats,
             disease_rank_comparison,
             disease_binary_classification_stats,
         )
```

### Comparing `pheval-0.3.6/src/pheval/analyse/gene_prioritisation_analysis.py` & `pheval-0.3.7/src/pheval/analyse/gene_prioritisation_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 from pheval.analyse.binary_classification_stats import BinaryClassificationStats
 from pheval.analyse.parse_pheval_result import parse_pheval_result, read_standardised_result
 from pheval.analyse.prioritisation_rank_recorder import PrioritisationRankRecorder
 from pheval.analyse.prioritisation_result_types import GenePrioritisationResult
 from pheval.analyse.rank_stats import RankStats
 from pheval.analyse.run_data_parser import TrackInputOutputDirectories
 from pheval.post_processing.post_processing import RankedPhEvalGeneResult
-from pheval.utils.file_utils import (
-    all_files,
-    files_with_suffix,
-    obtain_phenopacket_path_from_pheval_result,
-)
+from pheval.utils.file_utils import all_files
 from pheval.utils.phenopacket_utils import PhenopacketUtil, ProbandCausativeGene, phenopacket_reader
 
 
 class AssessGenePrioritisation:
     """Class for assessing gene prioritisation based on thresholds and scoring orders."""
 
     def __init__(
@@ -205,37 +201,37 @@
     """
     phenopacket = phenopacket_reader(phenopacket_path)
     phenopacket_util = PhenopacketUtil(phenopacket)
     return phenopacket_util.diagnosed_genes()
 
 
 def assess_phenopacket_gene_prioritisation(
-    standardised_gene_result: Path,
+    phenopacket_path: Path,
     score_order: str,
     results_dir_and_input: TrackInputOutputDirectories,
     threshold: float,
     gene_rank_stats: RankStats,
     gene_rank_comparison: defaultdict,
     gene_binary_classification_stats: BinaryClassificationStats,
 ) -> None:
     """
     Assess gene prioritisation for a Phenopacket by comparing PhEval standardised gene results
     against the recorded causative genes for a proband in the Phenopacket.
 
     Args:
-        standardised_gene_result (Path): Path to the PhEval standardised gene result file.
+        phenopacket_path (Path): Path to the Phenopacket.
         score_order (str): The order in which scores are arranged, either ascending or descending.
         results_dir_and_input (TrackInputOutputDirectories): Input and output directories.
         threshold (float): Threshold for assessment.
         gene_rank_stats (RankStats): RankStats class instance.
         gene_rank_comparison (defaultdict): Default dictionary for gene rank comparisons.
         gene_binary_classification_stats (BinaryClassificationStats): BinaryClassificationStats class instance.
     """
-    phenopacket_path = obtain_phenopacket_path_from_pheval_result(
-        standardised_gene_result, all_files(results_dir_and_input.phenopacket_dir)
+    standardised_gene_result = results_dir_and_input.results_dir.joinpath(
+        f"pheval_gene_results/{phenopacket_path.stem}-pheval_gene_result.tsv"
     )
     pheval_gene_result = read_standardised_result(standardised_gene_result)
     proband_causative_genes = _obtain_causative_genes(phenopacket_path)
     AssessGenePrioritisation(
         phenopacket_path,
         results_dir_and_input.results_dir.joinpath("pheval_gene_results/"),
         parse_pheval_result(RankedPhEvalGeneResult, pheval_gene_result),
@@ -262,19 +258,17 @@
          gene_rank_comparison (defaultdict): Default dictionary for gene rank comparisons.
      Returns:
          BenchmarkRunResults: An object containing benchmarking results for gene prioritisation,
          including ranks and rank statistics for the benchmarked directory.
     """
     gene_rank_stats = RankStats()
     gene_binary_classification_stats = BinaryClassificationStats()
-    for standardised_result in files_with_suffix(
-        results_directory_and_input.results_dir.joinpath("pheval_gene_results/"), ".tsv"
-    ):
+    for phenopacket_path in all_files(results_directory_and_input.phenopacket_dir):
         assess_phenopacket_gene_prioritisation(
-            standardised_result,
+            phenopacket_path,
             score_order,
             results_directory_and_input,
             threshold,
             gene_rank_stats,
             gene_rank_comparison,
             gene_binary_classification_stats,
         )
```

### Comparing `pheval-0.3.6/src/pheval/analyse/generate_plots.py` & `pheval-0.3.7/src/pheval/analyse/generate_plots.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/generate_summary_outputs.py` & `pheval-0.3.7/src/pheval/analyse/generate_summary_outputs.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/parse_benchmark_summary.py` & `pheval-0.3.7/src/pheval/analyse/parse_benchmark_summary.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/parse_pheval_result.py` & `pheval-0.3.7/src/pheval/analyse/parse_pheval_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,33 @@
+import logging
 from pathlib import Path
 from typing import List
 
 import pandas as pd
 
 from pheval.post_processing.post_processing import PhEvalResult
 
+info_log = logging.getLogger("info")
+
 
 def read_standardised_result(standardised_result_path: Path) -> List[dict]:
     """
     Read the standardised result output and return a list of dictionaries.
 
     Args:
         standardised_result_path (Path): The path to the file containing the standardised result output.
 
     Returns:
         List[dict]: A list of dictionaries representing the content of the standardised result file.
     """
-    return pd.read_csv(standardised_result_path, delimiter="\t").to_dict("records")
+    if standardised_result_path.is_file():
+        return pd.read_csv(standardised_result_path, delimiter="\t").to_dict("records")
+    else:
+        info_log.info(f"Could not find {standardised_result_path}")
+        return pd.DataFrame().to_dict("records")
 
 
 def parse_pheval_result(
     data_class_type: PhEvalResult, pheval_result: List[dict]
 ) -> List[PhEvalResult]:
     """
     Parse PhEval result into specified dataclass type.
```

### Comparing `pheval-0.3.6/src/pheval/analyse/prioritisation_rank_recorder.py` & `pheval-0.3.7/src/pheval/analyse/prioritisation_rank_recorder.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/prioritisation_result_types.py` & `pheval-0.3.7/src/pheval/analyse/prioritisation_result_types.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/rank_stats.py` & `pheval-0.3.7/src/pheval/analyse/rank_stats.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/run_data_parser.py` & `pheval-0.3.7/src/pheval/analyse/run_data_parser.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/analyse/variant_prioritisation_analysis.py` & `pheval-0.3.7/src/pheval/analyse/variant_prioritisation_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 from pheval.analyse.binary_classification_stats import BinaryClassificationStats
 from pheval.analyse.parse_pheval_result import parse_pheval_result, read_standardised_result
 from pheval.analyse.prioritisation_rank_recorder import PrioritisationRankRecorder
 from pheval.analyse.prioritisation_result_types import VariantPrioritisationResult
 from pheval.analyse.rank_stats import RankStats
 from pheval.analyse.run_data_parser import TrackInputOutputDirectories
 from pheval.post_processing.post_processing import RankedPhEvalVariantResult
-from pheval.utils.file_utils import (
-    all_files,
-    files_with_suffix,
-    obtain_phenopacket_path_from_pheval_result,
-)
+from pheval.utils.file_utils import all_files
 from pheval.utils.phenopacket_utils import GenomicVariant, PhenopacketUtil, phenopacket_reader
 
 
 class AssessVariantPrioritisation:
     """Class for assessing variant prioritisation based on thresholds and scoring orders."""
 
     def __init__(
@@ -207,39 +203,39 @@
     """
     phenopacket = phenopacket_reader(phenopacket_path)
     phenopacket_util = PhenopacketUtil(phenopacket)
     return phenopacket_util.diagnosed_variants()
 
 
 def assess_phenopacket_variant_prioritisation(
-    standardised_variant_result: Path,
+    phenopacket_path: Path,
     score_order: str,
     results_dir_and_input: TrackInputOutputDirectories,
     threshold: float,
     variant_rank_stats: RankStats,
     variant_rank_comparison: defaultdict,
     variant_binary_classification_stats: BinaryClassificationStats,
 ) -> None:
     """
     Assess variant prioritisation for a Phenopacket by comparing PhEval standardised variant results
     against the recorded causative variants for a proband in the Phenopacket.
 
     Args:
-        standardised_variant_result (Path): Path to the PhEval standardised variant result file.
+        phenopacket_path (Path): Path to the Phenopacket.
         score_order (str): The order in which scores are arranged, either ascending or descending.
         results_dir_and_input (TrackInputOutputDirectories): Input and output directories.
         threshold (float): Threshold for assessment.
         variant_rank_stats (RankStats): RankStats class instance.
         variant_rank_comparison (defaultdict): Default dictionary for variant rank comparisons.
         variant_binary_classification_stats (BinaryClassificationStats): BinaryClassificationStats class instance.
     """
-    phenopacket_path = obtain_phenopacket_path_from_pheval_result(
-        standardised_variant_result, all_files(results_dir_and_input.phenopacket_dir)
-    )
     proband_causative_variants = _obtain_causative_variants(phenopacket_path)
+    standardised_variant_result = results_dir_and_input.results_dir.joinpath(
+        f"pheval_variant_results/{phenopacket_path.stem}-pheval_variant_result.tsv"
+    )
     pheval_variant_result = read_standardised_result(standardised_variant_result)
     AssessVariantPrioritisation(
         phenopacket_path,
         results_dir_and_input.results_dir.joinpath("pheval_variant_results/"),
         parse_pheval_result(RankedPhEvalVariantResult, pheval_variant_result),
         threshold,
         score_order,
@@ -266,20 +262,17 @@
 
     Returns:
         BenchmarkRunResults: An object containing benchmarking results for variant prioritisation,
         including ranks and rank statistics for the benchmarked directory.
     """
     variant_rank_stats = RankStats()
     variant_binary_classification_stats = BinaryClassificationStats()
-    for standardised_result in files_with_suffix(
-        results_directory_and_input.results_dir.joinpath("pheval_variant_results/"),
-        ".tsv",
-    ):
+    for phenopacket_path in all_files(results_directory_and_input.phenopacket_dir):
         assess_phenopacket_variant_prioritisation(
-            standardised_result,
+            phenopacket_path,
             score_order,
             results_directory_and_input,
             threshold,
             variant_rank_stats,
             variant_rank_comparison,
             variant_binary_classification_stats,
         )
```

### Comparing `pheval-0.3.6/src/pheval/cli.py` & `pheval-0.3.7/src/pheval/cli.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/cli_pheval.py` & `pheval-0.3.7/src/pheval/cli_pheval.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/cli_pheval_utils.py` & `pheval-0.3.7/src/pheval/cli_pheval_utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/config_parser.py` & `pheval-0.3.7/src/pheval/config_parser.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/implementations/__init__.py` & `pheval-0.3.7/src/pheval/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/infra/exomiserdb.py` & `pheval-0.3.7/src/pheval/infra/exomiserdb.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/post_processing/post_processing.py` & `pheval-0.3.7/src/pheval/post_processing/post_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,15 +371,15 @@
     Raises:
         ValueError: If the results are not all the same type or an error occurs during file writing.
     """
     if not pheval_result:
         info_log.warning(f"No results found for {tool_result_path.name}")
         return
     ranked_pheval_result = _create_pheval_result(pheval_result, sort_order_str)
-    if all(isinstance(result, RankedPhEvalGeneResult) for result in ranked_pheval_result):
+    if all(isinstance(result, PhEvalGeneResult) for result in pheval_result):
         _write_pheval_gene_result(ranked_pheval_result, output_dir, tool_result_path)
-    elif all(isinstance(result, RankedPhEvalVariantResult) for result in ranked_pheval_result):
+    elif all(isinstance(result, PhEvalVariantResult) for result in pheval_result):
         _write_pheval_variant_result(ranked_pheval_result, output_dir, tool_result_path)
-    elif all(isinstance(result, RankedPhEvalDiseaseResult) for result in ranked_pheval_result):
+    elif all(isinstance(result, PhEvalDiseaseResult) for result in pheval_result):
         _write_pheval_disease_result(ranked_pheval_result, output_dir, tool_result_path)
     else:
         raise ValueError("Results are not all of the same type.")
```

### Comparing `pheval-0.3.6/src/pheval/prepare/create_noisy_phenopackets.py` & `pheval-0.3.7/src/pheval/prepare/create_noisy_phenopackets.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/prepare/create_spiked_vcf.py` & `pheval-0.3.7/src/pheval/prepare/create_spiked_vcf.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/prepare/custom_exceptions.py` & `pheval-0.3.7/src/pheval/prepare/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/prepare/prepare_corpus.py` & `pheval-0.3.7/src/pheval/prepare/prepare_corpus.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/prepare/update_phenopacket.py` & `pheval-0.3.7/src/pheval/prepare/update_phenopacket.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/resources/alternate_ouputs/CADA_results.txt` & `pheval-0.3.7/src/pheval/resources/alternate_ouputs/CADA_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt` & `pheval-0.3.7/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/resources/alternate_ouputs/OVA_results.txt` & `pheval-0.3.7/src/pheval/resources/alternate_ouputs/OVA_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json` & `pheval-0.3.7/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt` & `pheval-0.3.7/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/resources/alternate_ouputs/lirical_results.tsv` & `pheval-0.3.7/src/pheval/resources/alternate_ouputs/lirical_results.tsv`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/resources/alternate_ouputs/svanna_results.tsv` & `pheval-0.3.7/src/pheval/resources/alternate_ouputs/svanna_results.tsv`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/resources/hgnc_complete_set.txt` & `pheval-0.3.7/src/pheval/resources/hgnc_complete_set.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/run_metadata.py` & `pheval-0.3.7/src/pheval/run_metadata.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/runners/runner.py` & `pheval-0.3.7/src/pheval/runners/runner.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/utils/docs_gen.py` & `pheval-0.3.7/src/pheval/utils/docs_gen.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/utils/exomiser.py` & `pheval-0.3.7/src/pheval/utils/exomiser.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/utils/file_utils.py` & `pheval-0.3.7/src/pheval/utils/file_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -66,43 +66,14 @@
     Returns:
         str: The normalised file name without diacritical marks.
     """
     normalised_file_name = unicodedata.normalize("NFD", str(file_path))
     return re.sub("[\u0300-\u036f]", "", normalised_file_name)
 
 
-def obtain_phenopacket_path_from_pheval_result(
-    pheval_result_path: Path, phenopacket_paths: list[Path]
-) -> Path:
-    """
-    Obtains the phenopacket file name when given a pheval result file name
-    and a list of full paths of phenopackets to be queried.
-
-    Args:
-        pheval_result_path (Path): The PhEval result.
-        phenopacket_paths (list[Path]): List of full paths of phenopackets to be queried.
-
-    Returns:
-        Path: The matching phenopacket file path from the provided list.
-    """
-    pheval_result_path_stem_stripped = pheval_result_path.stem.split("-pheval_")[0]
-    matching_phenopacket_paths = [
-        phenopacket_path
-        for phenopacket_path in phenopacket_paths
-        if phenopacket_path.stem == pheval_result_path_stem_stripped
-    ]
-    if matching_phenopacket_paths:
-        return matching_phenopacket_paths[0]
-    else:
-        raise FileNotFoundError(
-            f"Unable to find matching phenopacket file named "
-            f"{pheval_result_path_stem_stripped}.json for {pheval_result_path.name}"
-        )
-
-
 def ensure_file_exists(*files: str):
     """Ensures the existence of files passed as parameter
     Raises:
         FileNotFoundError: If any file passed as a parameter doesn't exist a FileNotFound Exception will be raised
     """
     for file in files:
         if not path.isfile(file):
```

### Comparing `pheval-0.3.6/src/pheval/utils/phenopacket_utils.py` & `pheval-0.3.7/src/pheval/utils/phenopacket_utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/utils/semsim_utils.py` & `pheval-0.3.7/src/pheval/utils/semsim_utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/src/pheval/utils/utils.py` & `pheval-0.3.7/src/pheval/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.6/PKG-INFO` & `pheval-0.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheval
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

