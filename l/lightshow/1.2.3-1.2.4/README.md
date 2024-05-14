# Comparing `tmp/lightshow-1.2.3.tar.gz` & `tmp/lightshow-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightshow-1.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lightshow-1.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lightshow-1.2.3.tar` & `lightshow-1.2.4.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0      135 2024-04-16 14:43:45.136438 lightshow-1.2.3/.coveragerc
--rw-r--r--   0        0        0      248 2024-04-16 14:43:45.136438 lightshow-1.2.3/.flake8
--rw-r--r--   0        0        0       58 2024-04-16 14:43:45.136438 lightshow-1.2.3/.gitattributes
--rw-r--r--   0        0        0      198 2024-04-16 14:43:45.136438 lightshow-1.2.3/.github/dependabot.yml
--rw-r--r--   0        0        0     4662 2024-04-16 14:43:45.136438 lightshow-1.2.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2147 2024-04-16 14:43:45.136438 lightshow-1.2.3/.gitignore
--rw-r--r--   0        0        0      484 2024-04-16 14:43:45.136438 lightshow-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      885 2024-04-16 14:43:45.136438 lightshow-1.2.3/AUTHORS.md
--rw-r--r--   0        0        0     1239 2024-04-16 14:43:45.136438 lightshow-1.2.3/CHANGES.md
--rw-r--r--   0        0        0     1118 2024-04-16 14:43:45.136438 lightshow-1.2.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1574 2024-04-16 14:43:45.136438 lightshow-1.2.3/LICENSE
--rw-r--r--   0        0        0     7436 2024-04-16 14:43:45.136438 lightshow-1.2.3/README.md
--rw-r--r--   0        0        0      673 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/Makefile
--rw-r--r--   0        0        0    60563 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/_static/images/lightshow.jpg
--rw-r--r--   0        0        0   118686 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/_static/images/lightshow_old.jpg
--rw-r--r--   0        0        0      797 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/make.bat
--rw-r--r--   0        0        0        0 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/_static/.placeholder
--rw-r--r--   0        0        0     6725 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/conf.py
--rw-r--r--   0        0        0     2023 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/index.rst
--rw-r--r--   0        0        0     1181 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/installation.rst
--rw-r--r--   0        0        0     1053 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/lightshow.parameters.rst
--rw-r--r--   0        0        0      559 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/lightshow.rst
--rw-r--r--   0        0        0       86 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/modules.rst
--rw-r--r--   0        0        0      337 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/project.rst
--rw-r--r--   0        0        0       35 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/project/authors.rst
--rw-r--r--   0        0        0     1720 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/project/funding.rst
--rw-r--r--   0        0        0       47 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/project/license.rst
--rw-r--r--   0        0        0    20734 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/quickstart.rst
--rw-r--r--   0        0        0    92531 2024-04-16 14:43:45.136438 lightshow-1.2.3/figures/Lightshow_Workflow_Diagram.jpg
--rw-r--r--   0        0        0    25190 2024-04-16 14:43:45.136438 lightshow-1.2.3/figures/Lightshow_Workflow_Diagram.pdf
--rw-r--r--   0        0        0      535 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/__init__.py
--rw-r--r--   0        0        0     2820 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/conftest.py
--rw-r--r--   0        0        0       40 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
--rw-r--r--   0        0        0       42 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
--rw-r--r--   0        0        0       34 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_chpsp_files/O.fch.upf
--rw-r--r--   0        0        0       35 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
--rw-r--r--   0        0        0      476 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
--rw-r--r--   0        0        0      480 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
--rw-r--r--   0        0        0       24 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/dummy_psp_files/O.mock.upf
--rw-r--r--   0        0        0       25 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/dummy_psp_files/Ti.mock.upf
--rw-r--r--   0        0        0      152 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
--rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/helpers/__init__.py
--rw-r--r--   0        0        0    13328 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/helpers/geometry.py
--rw-r--r--   0        0        0       82 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/README.rst
--rw-r--r--   0        0        0    42630 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/ene_dep_broad.txt
--rw-r--r--   0        0        0    43441 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/gauss_broad.txt
--rw-r--r--   0        0        0    43519 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/lorentz_broad.txt
--rw-r--r--   0        0        0    43398 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/voigt_broad.txt
--rw-r--r--   0        0        0      376 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-10734/POSCAR
--rw-r--r--   0        0        0      198 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-1215/POSCAR
--rw-r--r--   0        0        0      814 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-1840/POSCAR
--rw-r--r--   0        0        0      284 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-2657/POSCAR
--rw-r--r--   0        0        0      167 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-2664/POSCAR
--rw-r--r--   0        0        0      287 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-390/POSCAR
--rw-r--r--   0        0        0      460 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-430/POSCAR
--rw-r--r--   0        0        0      403 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-458/POSCAR
--rw-r--r--   0        0        0     1702 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/test_broaden.py
--rw-r--r--   0        0        0     3798 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/test_database.py
--rw-r--r--   0        0        0    12398 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/test_exciting.py
--rw-r--r--   0        0        0     1225 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/test_metadata.py
--rw-r--r--   0        0        0       22 2024-04-16 14:43:50.216423 lightshow-1.2.3/lightshow/_version.py
--rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/common/__init__.py
--rw-r--r--   0        0        0     2580 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/common/kpoints.py
--rw-r--r--   0        0        0     3322 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/common/nbands.py
--rw-r--r--   0        0        0    19997 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/database.py
--rw-r--r--   0        0        0      766 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/defaults.py
--rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/__init__.py
--rw-r--r--   0        0        0      206 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/_base.py
--rw-r--r--   0        0        0     9135 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/exciting.py
--rw-r--r--   0        0        0     8143 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/feff.py
--rw-r--r--   0        0        0    14263 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/ocean.py
--rw-r--r--   0        0        0    29716 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/vasp.py
--rw-r--r--   0        0        0    19869 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/xspectra.py
--rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/postprocess/__init__.py
--rw-r--r--   0        0        0     9023 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/postprocess/broaden.py
--rw-r--r--   0        0        0     7584 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/postprocess/compare_utils.py
--rw-r--r--   0        0        0    12888 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/postprocess/parse.py
--rw-r--r--   0        0        0     4935 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/pymatgen_utils.py
--rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/utils/__init__.py
--rw-r--r--   0        0        0     1227 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/utils/environ_utils.py
--rw-r--r--   0        0        0    32847 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/00_basic_usage.ipynb
--rw-r--r--   0        0        0    10037 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/01_Ti_K_anatase_broaden.ipynb
--rw-r--r--   0        0        0     5829 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/compare_spectra.ipynb
--rw-r--r--   0        0        0     6741 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/parse_spectra.ipynb
--rwxr-xr-x   0        0        0    41029 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/spectra_files/anatase_exciting.txt
--rw-r--r--   0        0        0     3816 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/spectra_files/anatase_exp.txt
--rw-r--r--   0        0        0    54210 2024-04-16 14:43:45.144438 lightshow-1.2.3/notebooks/spectra_files/anatase_ocean.txt
--rw-r--r--   0        0        0     5000 2024-04-16 14:43:45.144438 lightshow-1.2.3/notebooks/spectra_files/anatase_theory_FEFF.txt
--rw-r--r--   0        0        0  2000000 2024-04-16 14:43:45.148438 lightshow-1.2.3/notebooks/spectra_files/anatase_theory_VASP.txt
--rwxr-xr-x   0        0        0    11578 2024-04-16 14:43:45.148438 lightshow-1.2.3/notebooks/spectra_files/anatase_xspectra.txt
--rw-r--r--   0        0        0     1980 2024-04-16 14:43:45.148438 lightshow-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     1204 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/README.rst
--rw-r--r--   0        0        0      575 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/build_docs.sh
--rw-r--r--   0        0        0      184 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/build_project.sh
--rw-r--r--   0        0        0      418 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/install.sh
--rw-r--r--   0        0        0     1076 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/update_version.sh
--rw-r--r--   0        0        0     9166 1970-01-01 00:00:00.000000 lightshow-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      135 2024-05-14 13:51:06.703964 lightshow-1.2.4/.coveragerc
+-rw-r--r--   0        0        0      248 2024-05-14 13:51:06.703964 lightshow-1.2.4/.flake8
+-rw-r--r--   0        0        0       58 2024-05-14 13:51:06.703964 lightshow-1.2.4/.gitattributes
+-rw-r--r--   0        0        0      198 2024-05-14 13:51:06.703964 lightshow-1.2.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     4662 2024-05-14 13:51:06.703964 lightshow-1.2.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2147 2024-05-14 13:51:06.703964 lightshow-1.2.4/.gitignore
+-rw-r--r--   0        0        0      484 2024-05-14 13:51:06.703964 lightshow-1.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      885 2024-05-14 13:51:06.703964 lightshow-1.2.4/AUTHORS.md
+-rw-r--r--   0        0        0     1345 2024-05-14 13:51:06.703964 lightshow-1.2.4/CHANGES.md
+-rw-r--r--   0        0        0     1118 2024-05-14 13:51:06.703964 lightshow-1.2.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1574 2024-05-14 13:51:06.703964 lightshow-1.2.4/LICENSE
+-rw-r--r--   0        0        0     7436 2024-05-14 13:51:06.703964 lightshow-1.2.4/README.md
+-rw-r--r--   0        0        0      673 2024-05-14 13:51:06.703964 lightshow-1.2.4/docs/Makefile
+-rw-r--r--   0        0        0    60563 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/_static/images/lightshow.jpg
+-rw-r--r--   0        0        0   118686 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/_static/images/lightshow_old.jpg
+-rw-r--r--   0        0        0      797 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/make.bat
+-rw-r--r--   0        0        0        0 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/_static/.placeholder
+-rw-r--r--   0        0        0     6725 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/conf.py
+-rw-r--r--   0        0        0     2023 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/index.rst
+-rw-r--r--   0        0        0     1181 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/installation.rst
+-rw-r--r--   0        0        0     1053 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/lightshow.parameters.rst
+-rw-r--r--   0        0        0      559 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/lightshow.rst
+-rw-r--r--   0        0        0       86 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/modules.rst
+-rw-r--r--   0        0        0      337 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/project.rst
+-rw-r--r--   0        0        0       35 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/project/authors.rst
+-rw-r--r--   0        0        0     1720 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/project/funding.rst
+-rw-r--r--   0        0        0       47 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/project/license.rst
+-rw-r--r--   0        0        0    20734 2024-05-14 13:51:06.707964 lightshow-1.2.4/docs/source/quickstart.rst
+-rw-r--r--   0        0        0    92531 2024-05-14 13:51:06.707964 lightshow-1.2.4/figures/Lightshow_Workflow_Diagram.jpg
+-rw-r--r--   0        0        0    25190 2024-05-14 13:51:06.707964 lightshow-1.2.4/figures/Lightshow_Workflow_Diagram.pdf
+-rw-r--r--   0        0        0      535 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/__init__.py
+-rw-r--r--   0        0        0     2820 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/conftest.py
+-rw-r--r--   0        0        0       40 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
+-rw-r--r--   0        0        0       42 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
+-rw-r--r--   0        0        0       34 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/dummy_chpsp_files/O.fch.upf
+-rw-r--r--   0        0        0       35 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
+-rw-r--r--   0        0        0      476 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
+-rw-r--r--   0        0        0      480 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
+-rw-r--r--   0        0        0       24 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/dummy_psp_files/O.mock.upf
+-rw-r--r--   0        0        0       25 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/dummy_psp_files/Ti.mock.upf
+-rw-r--r--   0        0        0      152 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
+-rw-r--r--   0        0        0        0 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/helpers/__init__.py
+-rw-r--r--   0        0        0    13328 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/helpers/geometry.py
+-rw-r--r--   0        0        0       82 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/sample_files/README.rst
+-rw-r--r--   0        0        0    42630 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/sample_files/ene_dep_broad.txt
+-rw-r--r--   0        0        0    43441 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/sample_files/gauss_broad.txt
+-rw-r--r--   0        0        0    43519 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/sample_files/lorentz_broad.txt
+-rw-r--r--   0        0        0    43398 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/sample_files/voigt_broad.txt
+-rw-r--r--   0        0        0      376 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/structure_files/mp-10734/POSCAR
+-rw-r--r--   0        0        0      198 2024-05-14 13:51:06.707964 lightshow-1.2.4/lightshow/_tests/structure_files/mp-1215/POSCAR
+-rw-r--r--   0        0        0      814 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/structure_files/mp-1840/POSCAR
+-rw-r--r--   0        0        0      284 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/structure_files/mp-2657/POSCAR
+-rw-r--r--   0        0        0      167 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/structure_files/mp-2664/POSCAR
+-rw-r--r--   0        0        0      287 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/structure_files/mp-390/POSCAR
+-rw-r--r--   0        0        0      460 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/structure_files/mp-430/POSCAR
+-rw-r--r--   0        0        0      403 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/structure_files/mp-458/POSCAR
+-rw-r--r--   0        0        0     1702 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/test_broaden.py
+-rw-r--r--   0        0        0     3798 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/test_database.py
+-rw-r--r--   0        0        0    12398 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/test_exciting.py
+-rw-r--r--   0        0        0     1225 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/_tests/test_metadata.py
+-rw-r--r--   0        0        0       22 2024-05-14 13:51:10.124003 lightshow-1.2.4/lightshow/_version.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/common/__init__.py
+-rw-r--r--   0        0        0     2580 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/common/kpoints.py
+-rw-r--r--   0        0        0     3322 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/common/nbands.py
+-rw-r--r--   0        0        0    19997 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/database.py
+-rw-r--r--   0        0        0      766 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/defaults.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/parameters/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/parameters/_base.py
+-rw-r--r--   0        0        0     9135 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/parameters/exciting.py
+-rw-r--r--   0        0        0     8143 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/parameters/feff.py
+-rw-r--r--   0        0        0    14263 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/parameters/ocean.py
+-rw-r--r--   0        0        0    29734 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/parameters/vasp.py
+-rw-r--r--   0        0        0    19869 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/parameters/xspectra.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/postprocess/__init__.py
+-rw-r--r--   0        0        0     9023 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/postprocess/broaden.py
+-rw-r--r--   0        0        0     7584 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/postprocess/compare_utils.py
+-rw-r--r--   0        0        0    12888 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/postprocess/parse.py
+-rw-r--r--   0        0        0     4935 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/pymatgen_utils.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/utils/__init__.py
+-rw-r--r--   0        0        0     1227 2024-05-14 13:51:06.711964 lightshow-1.2.4/lightshow/utils/environ_utils.py
+-rw-r--r--   0        0        0    32847 2024-05-14 13:51:06.711964 lightshow-1.2.4/notebooks/00_basic_usage.ipynb
+-rw-r--r--   0        0        0    10037 2024-05-14 13:51:06.711964 lightshow-1.2.4/notebooks/01_Ti_K_anatase_broaden.ipynb
+-rw-r--r--   0        0        0     5829 2024-05-14 13:51:06.711964 lightshow-1.2.4/notebooks/compare_spectra.ipynb
+-rw-r--r--   0        0        0     6741 2024-05-14 13:51:06.711964 lightshow-1.2.4/notebooks/parse_spectra.ipynb
+-rwxr-xr-x   0        0        0    41029 2024-05-14 13:51:06.711964 lightshow-1.2.4/notebooks/spectra_files/anatase_exciting.txt
+-rw-r--r--   0        0        0     3816 2024-05-14 13:51:06.711964 lightshow-1.2.4/notebooks/spectra_files/anatase_exp.txt
+-rw-r--r--   0        0        0    54210 2024-05-14 13:51:06.711964 lightshow-1.2.4/notebooks/spectra_files/anatase_ocean.txt
+-rw-r--r--   0        0        0     5000 2024-05-14 13:51:06.711964 lightshow-1.2.4/notebooks/spectra_files/anatase_theory_FEFF.txt
+-rw-r--r--   0        0        0  2000000 2024-05-14 13:51:06.719964 lightshow-1.2.4/notebooks/spectra_files/anatase_theory_VASP.txt
+-rwxr-xr-x   0        0        0    11578 2024-05-14 13:51:06.719964 lightshow-1.2.4/notebooks/spectra_files/anatase_xspectra.txt
+-rw-r--r--   0        0        0     1980 2024-05-14 13:51:06.719964 lightshow-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1204 2024-05-14 13:51:06.719964 lightshow-1.2.4/scripts/README.rst
+-rw-r--r--   0        0        0      575 2024-05-14 13:51:06.719964 lightshow-1.2.4/scripts/build_docs.sh
+-rw-r--r--   0        0        0      184 2024-05-14 13:51:06.719964 lightshow-1.2.4/scripts/build_project.sh
+-rw-r--r--   0        0        0      418 2024-05-14 13:51:06.719964 lightshow-1.2.4/scripts/install.sh
+-rw-r--r--   0        0        0     1076 2024-05-14 13:51:06.719964 lightshow-1.2.4/scripts/update_version.sh
+-rw-r--r--   0        0        0     9166 1970-01-01 00:00:00.000000 lightshow-1.2.4/PKG-INFO
```

### Comparing `lightshow-1.2.3/.github/workflows/ci.yml` & `lightshow-1.2.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/.gitignore` & `lightshow-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/AUTHORS.md` & `lightshow-1.2.4/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/CHANGES.md` & `lightshow-1.2.4/CHANGES.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Changelog
 
+## v1.2.4
+- Add `Ho_3` potential file. See [#272](https://github.com/AI-multimodal/Lightshow/issues/272).
 ## v1.2.3
 
 - Fix the "ghost atom" problem in VASP. See [#256](https://github.com/AI-multimodal/Lightshow/issues/254).
 - Cleanup the testing suite, replace Black with Ruff.
 
 
 ## v1.2.2
```

### Comparing `lightshow-1.2.3/CONTRIBUTING.md` & `lightshow-1.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/LICENSE` & `lightshow-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/README.md` & `lightshow-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/Makefile` & `lightshow-1.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/_static/images/lightshow.jpg` & `lightshow-1.2.4/docs/_static/images/lightshow.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/_static/images/lightshow_old.jpg` & `lightshow-1.2.4/docs/_static/images/lightshow_old.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/make.bat` & `lightshow-1.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/source/conf.py` & `lightshow-1.2.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/source/index.rst` & `lightshow-1.2.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/source/installation.rst` & `lightshow-1.2.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/source/lightshow.parameters.rst` & `lightshow-1.2.4/docs/source/lightshow.parameters.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/source/lightshow.rst` & `lightshow-1.2.4/docs/source/lightshow.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/source/project/funding.rst` & `lightshow-1.2.4/docs/source/project/funding.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/docs/source/quickstart.rst` & `lightshow-1.2.4/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/figures/Lightshow_Workflow_Diagram.jpg` & `lightshow-1.2.4/figures/Lightshow_Workflow_Diagram.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/figures/Lightshow_Workflow_Diagram.pdf` & `lightshow-1.2.4/figures/Lightshow_Workflow_Diagram.pdf`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/__init__.py` & `lightshow-1.2.4/lightshow/__init__.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/conftest.py` & `lightshow-1.2.4/lightshow/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/helpers/geometry.py` & `lightshow-1.2.4/lightshow/_tests/helpers/geometry.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/sample_files/ene_dep_broad.txt` & `lightshow-1.2.4/lightshow/_tests/sample_files/ene_dep_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/sample_files/gauss_broad.txt` & `lightshow-1.2.4/lightshow/_tests/sample_files/gauss_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/sample_files/lorentz_broad.txt` & `lightshow-1.2.4/lightshow/_tests/sample_files/lorentz_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/sample_files/voigt_broad.txt` & `lightshow-1.2.4/lightshow/_tests/sample_files/voigt_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/structure_files/mp-1840/POSCAR` & `lightshow-1.2.4/lightshow/_tests/structure_files/mp-1840/POSCAR`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/test_broaden.py` & `lightshow-1.2.4/lightshow/_tests/test_broaden.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/test_database.py` & `lightshow-1.2.4/lightshow/_tests/test_database.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/test_exciting.py` & `lightshow-1.2.4/lightshow/_tests/test_exciting.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/_tests/test_metadata.py` & `lightshow-1.2.4/lightshow/_tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/common/kpoints.py` & `lightshow-1.2.4/lightshow/common/kpoints.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/common/nbands.py` & `lightshow-1.2.4/lightshow/common/nbands.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/database.py` & `lightshow-1.2.4/lightshow/database.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/defaults.py` & `lightshow-1.2.4/lightshow/defaults.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/parameters/exciting.py` & `lightshow-1.2.4/lightshow/parameters/exciting.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/parameters/feff.py` & `lightshow-1.2.4/lightshow/parameters/feff.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/parameters/ocean.py` & `lightshow-1.2.4/lightshow/parameters/ocean.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/parameters/vasp.py` & `lightshow-1.2.4/lightshow/parameters/vasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,15 @@
     "Hg": "Hg_sv_GW",
     "Tl": "Tl_d_GW",
     "Pb": "Pb_d_GW",
     "Bi": "Bi_d_GW",
     "Po": "Po_d_GW",
     "At": "At_d_GW",
     "Rn": "Rn_d_GW",
+    "Ho": "Ho_3",
 }
 
 
 class Incar(pmgIncar):
     """Inherits the Pymatgen Incar class. Allows for the standard manipulation
     of the INCAR file as a dictionary but with a few extra methods."""
```

### Comparing `lightshow-1.2.3/lightshow/parameters/xspectra.py` & `lightshow-1.2.4/lightshow/parameters/xspectra.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/postprocess/broaden.py` & `lightshow-1.2.4/lightshow/postprocess/broaden.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/postprocess/compare_utils.py` & `lightshow-1.2.4/lightshow/postprocess/compare_utils.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/postprocess/parse.py` & `lightshow-1.2.4/lightshow/postprocess/parse.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/pymatgen_utils.py` & `lightshow-1.2.4/lightshow/pymatgen_utils.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/lightshow/utils/environ_utils.py` & `lightshow-1.2.4/lightshow/utils/environ_utils.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/00_basic_usage.ipynb` & `lightshow-1.2.4/notebooks/00_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/01_Ti_K_anatase_broaden.ipynb` & `lightshow-1.2.4/notebooks/01_Ti_K_anatase_broaden.ipynb`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/compare_spectra.ipynb` & `lightshow-1.2.4/notebooks/compare_spectra.ipynb`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/parse_spectra.ipynb` & `lightshow-1.2.4/notebooks/parse_spectra.ipynb`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/spectra_files/anatase_exciting.txt` & `lightshow-1.2.4/notebooks/spectra_files/anatase_exciting.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/spectra_files/anatase_exp.txt` & `lightshow-1.2.4/notebooks/spectra_files/anatase_exp.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/spectra_files/anatase_ocean.txt` & `lightshow-1.2.4/notebooks/spectra_files/anatase_ocean.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/spectra_files/anatase_theory_FEFF.txt` & `lightshow-1.2.4/notebooks/spectra_files/anatase_theory_FEFF.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/spectra_files/anatase_theory_VASP.txt` & `lightshow-1.2.4/notebooks/spectra_files/anatase_theory_VASP.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/notebooks/spectra_files/anatase_xspectra.txt` & `lightshow-1.2.4/notebooks/spectra_files/anatase_xspectra.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/pyproject.toml` & `lightshow-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/scripts/README.rst` & `lightshow-1.2.4/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/scripts/build_docs.sh` & `lightshow-1.2.4/scripts/build_docs.sh`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/scripts/update_version.sh` & `lightshow-1.2.4/scripts/update_version.sh`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.3/PKG-INFO` & `lightshow-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightshow
-Version: 1.2.3
+Version: 1.2.4
 Summary: A one-stop-shop for writing computational spectroscopy input files
 Author: Benedikt Maurer, Fabien Peschel, Eli Stavitski, Xiaohui Qu, John T. Vinson, Christian Vorwerk
 Author-email: "Matthew R. Carbone" <mcarbone@bnl.gov>, Fanchen Meng <fmeng1@bnl.gov>, Deyu Lu <dlu@bnl.gov>
 Maintainer-email: "Matthew R. Carbone" <mcarbone@bnl.gov>, Fanchen Meng <fmeng1@bnl.gov>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
```

