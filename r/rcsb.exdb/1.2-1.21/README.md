# Comparing `tmp/rcsb_exdb-1.2.tar.gz` & `tmp/rcsb_exdb-1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb_exdb-1.2.tar", last modified: Thu May  9 19:30:32 2024, max compression
+gzip compressed data, was "rcsb_exdb-1.21.tar", last modified: Tue May 14 14:13:42 2024, max compression
```

## Comparing `rcsb_exdb-1.2.tar` & `rcsb_exdb-1.21.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.841911 rcsb_exdb-1.2/
--rw-r--r--   0 vsts      (1001) docker     (127)     8127 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     6115 2024-05-09 19:30:32.841911 rcsb_exdb-1.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4716 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.821910 rcsb_exdb-1.2/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.821910 rcsb_exdb-1.2/rcsb/exdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.821910 rcsb_exdb-1.2/rcsb/exdb/branch/
--rw-r--r--   0 vsts      (1001) docker     (127)     2645 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/branch/BranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/branch/GlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4507 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/branch/GlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/branch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.825911 rcsb_exdb-1.2/rcsb/exdb/chemref/
--rw-r--r--   0 vsts      (1001) docker     (127)     4719 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/chemref/ChemRefEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2538 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/chemref/ChemRefExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5290 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/chemref/ChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15479 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/chemref/PubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11699 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/chemref/PubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29394 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/chemref/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.825911 rcsb_exdb-1.2/rcsb/exdb/citation/
--rw-r--r--   0 vsts      (1001) docker     (127)     3501 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/citation/CitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7574 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/citation/CitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1487 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/citation/CitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/citation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.825911 rcsb_exdb-1.2/rcsb/exdb/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)     9835 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/cli/ExDbExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.825911 rcsb_exdb-1.2/rcsb/exdb/entry/
--rw-r--r--   0 vsts      (1001) docker     (127)     5095 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/entry/EntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/entry/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.829911 rcsb_exdb-1.2/rcsb/exdb/seq/
--rw-r--r--   0 vsts      (1001) docker     (127)     2741 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/AnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3423 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3744 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/LigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14538 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/PolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31160 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9560 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25935 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18181 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19497 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2315 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/TaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7594 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/UniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2695 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/UniProtExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/seq/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.837911 rcsb_exdb-1.2/rcsb/exdb/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3999 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9766 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/fixturePdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2657 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testAnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2936 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testBranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3696 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testChemRefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3353 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3625 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testCitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3141 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testCitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3064 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testCitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2340 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3360 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testEntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5358 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2295 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testGlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3201 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testGlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testGlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3040 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14144 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2944 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3536 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testPolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4679 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testPubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5187 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testPubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6511 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testPubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4326 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4897 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5005 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4631 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3469 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2536 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testTaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3654 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testTreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3403 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2604 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tests/testUniProtExtractor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.837911 rcsb_exdb-1.2/rcsb/exdb/tree/
--rw-r--r--   0 vsts      (1001) docker     (127)    12617 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tree/TreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/tree/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.837911 rcsb_exdb-1.2/rcsb/exdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/utils/ObjectAdapterBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11057 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/utils/ObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5210 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/utils/ObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5089 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/utils/ObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6954 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/utils/ObjectValidator.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.837911 rcsb_exdb-1.2/rcsb/exdb/wf/
--rw-r--r--   0 vsts      (1001) docker     (127)     2570 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19813 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/wf/ExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/wf/GlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11235 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/wf/PubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/rcsb/exdb/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 19:30:32.837911 rcsb_exdb-1.2/rcsb.exdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     6115 2024-05-09 19:30:32.000000 rcsb_exdb-1.2/rcsb.exdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3525 2024-05-09 19:30:32.000000 rcsb_exdb-1.2/rcsb.exdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 19:30:32.000000 rcsb_exdb-1.2/rcsb.exdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-05-09 19:30:32.000000 rcsb_exdb-1.2/rcsb.exdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 19:05:42.000000 rcsb_exdb-1.2/rcsb.exdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      419 2024-05-09 19:30:32.000000 rcsb_exdb-1.2/rcsb.exdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-09 19:30:32.000000 rcsb_exdb-1.2/rcsb.exdb.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      465 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-09 19:30:32.841911 rcsb_exdb-1.2/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2184 2024-05-09 18:59:14.000000 rcsb_exdb-1.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.549466 rcsb_exdb-1.21/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8178 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     6116 2024-05-14 14:13:42.549466 rcsb_exdb-1.21/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4716 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.537466 rcsb_exdb-1.21/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.537466 rcsb_exdb-1.21/rcsb/exdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.537466 rcsb_exdb-1.21/rcsb/exdb/branch/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2645 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/branch/BranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/branch/GlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4507 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/branch/GlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/branch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.541466 rcsb_exdb-1.21/rcsb/exdb/chemref/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5027 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/chemref/ChemRefEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2538 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/chemref/ChemRefExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5290 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/chemref/ChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15479 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/chemref/PubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11699 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/chemref/PubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29437 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/chemref/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.541466 rcsb_exdb-1.21/rcsb/exdb/citation/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3501 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/citation/CitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7574 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/citation/CitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1487 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/citation/CitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/citation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.541466 rcsb_exdb-1.21/rcsb/exdb/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9835 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/cli/ExDbExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.541466 rcsb_exdb-1.21/rcsb/exdb/entry/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5095 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/entry/EntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/entry/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.541466 rcsb_exdb-1.21/rcsb/exdb/seq/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2741 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/AnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3423 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3744 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/LigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14538 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/PolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31160 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9560 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25935 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18181 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19497 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2315 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/TaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7590 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/UniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2695 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/UniProtExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/seq/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.545466 rcsb_exdb-1.21/rcsb/exdb/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3999 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9766 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/fixturePdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2657 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testAnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2936 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testBranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3696 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testChemRefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3353 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3625 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testCitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3141 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testCitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3064 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testCitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2340 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3360 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testEntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5358 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2295 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testGlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3201 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testGlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testGlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3040 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14144 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2944 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3536 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testPolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4679 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testPubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5187 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testPubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6511 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testPubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4354 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4897 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5005 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4631 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3469 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2536 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testTaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3654 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testTreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3403 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2604 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tests/testUniProtExtractor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.545466 rcsb_exdb-1.21/rcsb/exdb/tree/
+-rw-r--r--   0 vsts      (1001) docker     (127)    12617 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tree/TreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/tree/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.549466 rcsb_exdb-1.21/rcsb/exdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/utils/ObjectAdapterBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11057 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/utils/ObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5229 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/utils/ObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5089 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/utils/ObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6973 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/utils/ObjectValidator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.549466 rcsb_exdb-1.21/rcsb/exdb/wf/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2570 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19813 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/wf/ExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/wf/GlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11235 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/wf/PubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/rcsb/exdb/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 14:13:42.549466 rcsb_exdb-1.21/rcsb.exdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6116 2024-05-14 14:13:42.000000 rcsb_exdb-1.21/rcsb.exdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3525 2024-05-14 14:13:42.000000 rcsb_exdb-1.21/rcsb.exdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-14 14:13:42.000000 rcsb_exdb-1.21/rcsb.exdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-05-14 14:13:42.000000 rcsb_exdb-1.21/rcsb.exdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-14 13:53:42.000000 rcsb_exdb-1.21/rcsb.exdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      419 2024-05-14 14:13:42.000000 rcsb_exdb-1.21/rcsb.exdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-14 14:13:42.000000 rcsb_exdb-1.21/rcsb.exdb.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      465 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-14 14:13:42.549466 rcsb_exdb-1.21/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2184 2024-05-14 13:47:16.000000 rcsb_exdb-1.21/setup.py
```

### Comparing `rcsb_exdb-1.2/HISTORY.txt` & `rcsb_exdb-1.21/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -96,7 +96,8 @@
 19-Sep-2023 V0.99 Add reload method to ChemRefMappingProvider and LigandNeighborMappingProvider;
                   Add documentation to reference sequence providers
  9-Jan-2024 V1.00 Update PolymerEntityExtractor to turn off usage of uniprot_exdb as source data;
                   This package update also coincides with the turning off of uniprot_exdb data loading during the weekly workflow
  6-May-2024 V1.1  Update ExDbExec CLI and ExDbWorkflow to support CLI usage from weekly-update workflow;
                   Update unit tests and setuptools config
  9-May-2024 V1.2  Adjust provider type exclusion input to accept a list of types
+13-May-2024 V1.21 Update requirements; fix linting
```

### Comparing `rcsb_exdb-1.2/LICENSE` & `rcsb_exdb-1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/PKG-INFO` & `rcsb_exdb-1.21/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 1.2
+Version: 1.21
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,26 +14,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: OpenEye-toolkits>=2020.2.2
 Requires-Dist: numpy
 Requires-Dist: jsonschema>=2.6.0
-Requires-Dist: rcsb.utils.io>=1.28
-Requires-Dist: rcsb.db>=1.720
-Requires-Dist: rcsb.utils.chemref>=0.79
-Requires-Dist: rcsb.utils.chem>=0.75
-Requires-Dist: rcsb.utils.citation>=0.16
-Requires-Dist: rcsb.utils.config>=0.35
-Requires-Dist: rcsb.utils.ec>=0.22
-Requires-Dist: rcsb.utils.go>=0.17
-Requires-Dist: rcsb.utils.seq>=0.63
-Requires-Dist: rcsb.utils.struct>=0.37
-Requires-Dist: rcsb.utils.taxonomy>=0.39
-Requires-Dist: rcsb.utils.dictionary>=1.23
+Requires-Dist: rcsb.utils.io>=1.46
+Requires-Dist: rcsb.db>=1.721
+Requires-Dist: rcsb.utils.chem>=0.79
+Requires-Dist: rcsb.utils.chemref>=0.91
+Requires-Dist: rcsb.utils.citation>=0.22
+Requires-Dist: rcsb.utils.config>=0.40
+Requires-Dist: rcsb.utils.ec>=0.25
+Requires-Dist: rcsb.utils.go>=0.18
+Requires-Dist: rcsb.utils.seq>=0.79
+Requires-Dist: rcsb.utils.struct>=0.47
+Requires-Dist: rcsb.utils.taxonomy>=0.43
+Requires-Dist: rcsb.utils.dictionary>=1.24
 Requires-Dist: rcsb.workflow>=0.42
 Requires-Dist: statistics; python_version < "3.0"
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
```

### Comparing `rcsb_exdb-1.2/README.md` & `rcsb_exdb-1.21/README.md`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/branch/BranchedEntityExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/branch/BranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/branch/GlycanProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/branch/GlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/branch/GlycanUtils.py` & `rcsb_exdb-1.21/rcsb/exdb/branch/GlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/chemref/ChemRefEtlWorker.py` & `rcsb_exdb-1.21/rcsb/exdb/chemref/ChemRefEtlWorker.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
     def load(self, updateId, extResource, loadType="full"):
         """Load chemical reference integrated data for the input external resource-"""
         try:
             self.__statusList = []
             desp = DataExchangeStatus()
             statusStartTimestamp = desp.setStartTime()
+            addValues = {}
             #
             if extResource == "DrugBank":
                 databaseName = "drugbank_core"
                 configName = self.__cfgOb.getDefaultSectionName()
                 user = self.__cfgOb.get("_DRUGBANK_AUTH_USERNAME", sectionName=configName)
                 pw = self.__cfgOb.get("_DRUGBANK_AUTH_PASSWORD", sectionName=configName)
                 #
@@ -81,18 +82,18 @@
                 logger.info("Resource %r extracted mapped document length %d", extResource, len(dList))
                 logger.debug("Objects %r", dList[:2])
                 sD, _, collectionList, _ = self.__schP.getSchemaInfo(databaseName)
                 collectionName = collectionList[0] if collectionList else "unassigned"
                 indexL = sD.getDocumentIndex(collectionName, "primary")
                 logger.info("Database %r collection %r index attributes %r", databaseName, collectionName, indexL)
                 #
-                collectionVersion = sD.getCollectionVersion(collectionName)
-                addValues = {"_schema_version": collectionVersion}
-                #
-                addValues = {}
+                # For some reason, 'addValues' was being overwritten with an empty dict (https://github.com/rcsb/py-rcsb_exdb/commit/26bd79e9a2fffc97c034b4116dece9248d1c1f39)
+                # Will need to review this -- do we want to add the schema version values or not? (Also, see similar logic in UniProtCoreEtlWorker.py)
+                # collectionVersion = sD.getCollectionVersion(collectionName)
+                # addValues = {"_schema_version": collectionVersion}
             #
             dl = DocumentLoader(
                 self.__cfgOb,
                 self.__cachePath,
                 self.__resourceName,
                 numProc=self.__numProc,
                 chunkSize=self.__chunkSize,
```

### Comparing `rcsb_exdb-1.2/rcsb/exdb/chemref/ChemRefExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/chemref/ChemRefExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/chemref/ChemRefMappingProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/chemref/ChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/chemref/PubChemDataCacheProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/chemref/PubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/chemref/PubChemEtlWrapper.py` & `rcsb_exdb-1.21/rcsb/exdb/chemref/PubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/chemref/PubChemIndexCacheProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/chemref/PubChemIndexCacheProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         Args:
             ccId (str): chemical component identifiers
 
         Returns:
             (list): list of ChemicalIdentifier() objects corresponding to the input chemical component.
         """
         chemIdList = []
+        idType = None
+        descr = None
         if ccId in self.__lookupD:
             for sD in self.__lookupD[ccId]:
                 if "inchi-key" in sD:
                     idType = "inchikey"
                     descr = sD["inchi-key"]
                 elif "smiles" in sD:
                     idType = "smiles"
```

### Comparing `rcsb_exdb-1.2/rcsb/exdb/citation/CitationAdapter.py` & `rcsb_exdb-1.21/rcsb/exdb/citation/CitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/citation/CitationExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/citation/CitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/citation/CitationUtils.py` & `rcsb_exdb-1.21/rcsb/exdb/citation/CitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/cli/ExDbExec.py` & `rcsb_exdb-1.21/rcsb/exdb/cli/ExDbExec.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/entry/EntryInfoProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/entry/EntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/AnnotationExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/AnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/LigandNeighborMappingExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/LigandNeighborMappingExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/LigandNeighborMappingProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/LigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/PolymerEntityExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/PolymerEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/TaxonomyExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/TaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/UniProtCoreEtlWorker.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/UniProtCoreEtlWorker.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         try:
             self.__statusList = []
             desp = DataExchangeStatus()
             statusStartTimestamp = desp.setStartTime()
             #
             dList = indexL = []
             databaseName = collectionName = collectionVersion = None
+            addValues = {}
             #
             if extResource == "UniProt":
                 databaseName = "uniprot_core"
                 # configName = self.__cfgOb.getDefaultSectionName()
                 # dirPath = os.path.join(self.__cachePath, self.__cfgOb.get("EXDB_CACHE_DIR", self.__cfgOb.getDefaultSectionName()))
                 #
                 ok, rsP = self.__getReferenceSequenceProvider()
@@ -110,15 +111,14 @@
                 logger.debug("Objects %r", dList[:2])
                 #
                 cDL = self.__docHelper.getCollectionInfo(databaseName)
                 collectionName = cDL[0]["NAME"]
                 collectionVersion = cDL[0]["VERSION"]
                 indexL = self.__docHelper.getDocumentIndexAttributes(collectionName, "primary")
                 logger.info("Database %r collection %r version %r index attributes %r", databaseName, collectionName, collectionVersion, indexL)
-                addValues = {}
             else:
                 logger.error("Unsupported external resource %r", extResource)
             #
             if self.__doValidate:
                 self.__valInst = self.__getValidator(databaseName, collectionName, schemaLevel="full")
                 for dObj in dList:
                     self.__validateObj(databaseName, collectionName, dObj, label="Original")
```

### Comparing `rcsb_exdb-1.2/rcsb/exdb/seq/UniProtExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/seq/UniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/fixturePdbxLoader.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/fixturePdbxLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testAnnotationExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testAnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testBranchedEntityExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testBranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testChemRefLoader.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testChemRefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testChemRefMappingProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testCitationAdapter.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testCitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testCitationExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testCitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testCitationUtils.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testCitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testEntryInfoProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testEntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testExDbWorkflow.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testExDbWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testGlycanEtlWorkflow.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testGlycanEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testGlycanProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testGlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testGlycanUtils.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testGlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testLigandNeighborMappingProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testLigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testObjectExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testObjectExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testObjectTransformer.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testObjectTransformer.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testObjectUpdater.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testPolymerEntityExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testPolymerEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testPubChemDataCacheProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testPubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testPubChemEtlWorkflow.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testPubChemEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testPubChemEtlWrapper.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testPubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testPubChemIndexCacheProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testPubChemIndexCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,32 +56,32 @@
     def tearDown(self):
         unitS = "MB" if platform.system() == "Darwin" else "GB"
         rusageMax = resource.getrusage(resource.RUSAGE_SELF).ru_maxrss
         logger.info("Maximum resident memory size %.4f %s", rusageMax / 10 ** 6, unitS)
         endTime = time.time()
         logger.info("Completed %s at %s (%.4f seconds)", self.id(), time.strftime("%Y %m %d %H:%M:%S", time.localtime()), endTime - self.__startTime)
 
-    @unittest.skip("Disable test - no longer using in production, and fails too frequently with 'Bad xml text' when fetching from UniProt")
+    # @unittest.skip("Disable test - no longer using in production, and fails too frequently with 'Bad xml text' when fetching from UniProt")
     def testAnnotationAdapter(self):
         """Test case - create and read cache reference sequences assignments and related data."""
         try:
             databaseName = "pdbx_core"
             collectionName = "pdbx_core_polymer_entity"
             polymerType = "Protein"
             #  -- create cache ---
             rsaP = ReferenceSequenceAnnotationProvider(
                 self.__cfgOb, databaseName, collectionName, polymerType, fetchLimit=self.__fetchLimit, siftsAbbreviated="TEST", cachePath=self.__cachePath, useCache=True
             )
-            ok = rsaP.testCache()
+            ok = rsaP.testCache(minMissing=10)
             self.assertTrue(ok)
             numRef1 = rsaP.getRefDataCount()
             #
             # ---  Reload from cache ---
             rsaP = ReferenceSequenceAnnotationProvider(self.__cfgOb, databaseName, collectionName, polymerType, cachePath=self.__cachePath, useCache=True)
-            ok = rsaP.testCache()
+            ok = rsaP.testCache(minMissing=10)
             self.assertTrue(ok)
             numRef2 = rsaP.getRefDataCount()
             self.assertEqual(numRef1, numRef2)
             #
             rsa = ReferenceSequenceAnnotationAdapter(rsaP)
             obTr = ObjectTransformer(self.__cfgOb, objectAdapter=rsa)
             ok = obTr.doTransform(
```

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testTaxonomyExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testTaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testTreeNodeListWorker.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testTreeNodeListWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testUniProtCoreEtlWorker.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testUniProtCoreEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tests/testUniProtExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/tests/testUniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/tree/TreeNodeListWorker.py` & `rcsb_exdb-1.21/rcsb/exdb/tree/TreeNodeListWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/utils/ObjectExtractor.py` & `rcsb_exdb-1.21/rcsb/exdb/utils/ObjectExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/utils/ObjectTransformer.py` & `rcsb_exdb-1.21/rcsb/exdb/utils/ObjectTransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         tU = TimeUtil()
         updateId = kwargs.get("updateId", tU.getCurrentWeekSignature())
         #
         docSelectList = self.__selectObjectIds(databaseName, collectionName, selectionQueryD)
         docSelectList = docSelectList[:fetchLimit] if fetchLimit else docSelectList
         ok = self.__transform(databaseName, collectionName, docSelectList)
         #
+        okS = True
         if updateId:
             okS = self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
         return ok and okS
 
     def __selectObjectIds(self, databaseName, collectionName, selectionQueryD):
         """Return a list of object identifiers for the input selection query."""
         try:
```

### Comparing `rcsb_exdb-1.2/rcsb/exdb/utils/ObjectUpdater.py` & `rcsb_exdb-1.21/rcsb/exdb/utils/ObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/utils/ObjectValidator.py` & `rcsb_exdb-1.21/rcsb/exdb/utils/ObjectValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         updateId = kwargs.get("updateId", tU.getCurrentWeekSignature())
         #
         docSelectList = self.__selectObjectIds(databaseName, collectionName, selectionQueryD)
         docSelectList = docSelectList[:fetchLimit] if fetchLimit else docSelectList
 
         ok = self.__transform(databaseName, collectionName, docSelectList)
         #
+        okS = True
         if updateId:
             okS = self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
         return ok and okS
 
     def __selectObjectIds(self, databaseName, collectionName, selectionQueryD):
         """Return a list of object identifiers for the input selection query."""
         try:
```

### Comparing `rcsb_exdb-1.2/rcsb/exdb/wf/EntryInfoEtlWorkflow.py` & `rcsb_exdb-1.21/rcsb/exdb/wf/EntryInfoEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/wf/ExDbWorkflow.py` & `rcsb_exdb-1.21/rcsb/exdb/wf/ExDbWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/wf/GlycanEtlWorkflow.py` & `rcsb_exdb-1.21/rcsb/exdb/wf/GlycanEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb/exdb/wf/PubChemEtlWorkflow.py` & `rcsb_exdb-1.21/rcsb/exdb/wf/PubChemEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/rcsb.exdb.egg-info/PKG-INFO` & `rcsb_exdb-1.21/rcsb.exdb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 1.2
+Version: 1.21
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,26 +14,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: OpenEye-toolkits>=2020.2.2
 Requires-Dist: numpy
 Requires-Dist: jsonschema>=2.6.0
-Requires-Dist: rcsb.utils.io>=1.28
-Requires-Dist: rcsb.db>=1.720
-Requires-Dist: rcsb.utils.chemref>=0.79
-Requires-Dist: rcsb.utils.chem>=0.75
-Requires-Dist: rcsb.utils.citation>=0.16
-Requires-Dist: rcsb.utils.config>=0.35
-Requires-Dist: rcsb.utils.ec>=0.22
-Requires-Dist: rcsb.utils.go>=0.17
-Requires-Dist: rcsb.utils.seq>=0.63
-Requires-Dist: rcsb.utils.struct>=0.37
-Requires-Dist: rcsb.utils.taxonomy>=0.39
-Requires-Dist: rcsb.utils.dictionary>=1.23
+Requires-Dist: rcsb.utils.io>=1.46
+Requires-Dist: rcsb.db>=1.721
+Requires-Dist: rcsb.utils.chem>=0.79
+Requires-Dist: rcsb.utils.chemref>=0.91
+Requires-Dist: rcsb.utils.citation>=0.22
+Requires-Dist: rcsb.utils.config>=0.40
+Requires-Dist: rcsb.utils.ec>=0.25
+Requires-Dist: rcsb.utils.go>=0.18
+Requires-Dist: rcsb.utils.seq>=0.79
+Requires-Dist: rcsb.utils.struct>=0.47
+Requires-Dist: rcsb.utils.taxonomy>=0.43
+Requires-Dist: rcsb.utils.dictionary>=1.24
 Requires-Dist: rcsb.workflow>=0.42
 Requires-Dist: statistics; python_version < "3.0"
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
```

### Comparing `rcsb_exdb-1.2/rcsb.exdb.egg-info/SOURCES.txt` & `rcsb_exdb-1.21/rcsb.exdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb_exdb-1.2/setup.py` & `rcsb_exdb-1.21/setup.py`

 * *Files identical despite different names*

