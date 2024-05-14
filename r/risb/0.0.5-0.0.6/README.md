# Comparing `tmp/risb-0.0.5.tar.gz` & `tmp/risb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Oct 31 04:58:26 2023, max compression
+gzip compressed data, last modified: Tue May 14 01:25:26 2024, max compression
```

## Comparing `risb-0.0.5.tar` & `risb-0.0.6.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0      202 2023-10-31 04:58:26.000000 risb-0.0.5/.dockerignore
--rw-r--r--   0        0        0      124 2023-10-31 04:58:26.000000 risb-0.0.5/.git_archival.txt
--rw-r--r--   0        0        0       98 2023-10-31 04:58:26.000000 risb-0.0.5/.gitattributes
--rw-r--r--   0        0        0     3481 2023-10-31 04:58:26.000000 risb-0.0.5/CITATION
--rw-r--r--   0        0        0      822 2023-10-31 04:58:26.000000 risb-0.0.5/COPYRIGHT
--rw-r--r--   0        0        0     1168 2023-10-31 04:58:26.000000 risb-0.0.5/TODO.md
--rw-r--r--   0        0        0       37 2023-10-31 04:58:26.000000 risb-0.0.5/.github/CODEOWNERS
--rw-r--r--   0        0        0     3302 2023-10-31 04:58:26.000000 risb-0.0.5/.github/actions/setup-triqs/action.yml
--rw-r--r--   0        0        0     2752 2023-10-31 04:58:26.000000 risb-0.0.5/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1665 2023-10-31 04:58:26.000000 risb-0.0.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0      382 2023-10-31 04:58:26.000000 risb-0.0.5/docker/Dockerfile
--rw-r--r--   0        0        0     3434 2023-10-31 04:58:26.000000 risb-0.0.5/docker/Dockerfile.dev
--rw-r--r--   0        0        0      608 2023-10-31 04:58:26.000000 risb-0.0.5/docker/Dockerfile.docs
--rw-r--r--   0        0        0      567 2023-10-31 04:58:26.000000 risb-0.0.5/docker/conda.sh
--rw-r--r--   0        0        0      332 2023-10-31 04:58:26.000000 risb-0.0.5/docker/docker-compose-dev.yml
--rw-r--r--   0        0        0      334 2023-10-31 04:58:26.000000 risb-0.0.5/docker/docker-compose-docs.yml
--rw-r--r--   0        0        0      266 2023-10-31 04:58:26.000000 risb-0.0.5/docker/docker-compose.yml
--rw-r--r--   0        0        0       10 2023-10-31 04:58:26.000000 risb-0.0.5/docs/.gitignore
--rw-r--r--   0        0        0     3376 2023-10-31 04:58:26.000000 risb-0.0.5/docs/about.md
--rw-r--r--   0        0        0     2359 2023-10-31 04:58:26.000000 risb-0.0.5/docs/conf.py
--rw-r--r--   0        0        0      422 2023-10-31 04:58:26.000000 risb-0.0.5/docs/index.md
--rw-r--r--   0        0        0      111 2023-10-31 04:58:26.000000 risb-0.0.5/docs/install.md
--rw-r--r--   0        0        0     5636 2023-10-31 04:58:26.000000 risb-0.0.5/docs/explanations/embedding.md
--rw-r--r--   0        0        0      114 2023-10-31 04:58:26.000000 risb-0.0.5/docs/explanations/index.md
--rw-r--r--   0        0        0     2090 2023-10-31 04:58:26.000000 risb-0.0.5/docs/explanations/kweight.md
--rw-r--r--   0        0        0     3176 2023-10-31 04:58:26.000000 risb-0.0.5/docs/explanations/projectors.md
--rw-r--r--   0        0        0     2426 2023-10-31 04:58:26.000000 risb-0.0.5/docs/how-to/diis.md
--rw-r--r--   0        0        0     5629 2023-10-31 04:58:26.000000 risb-0.0.5/docs/how-to/embedding.md
--rw-r--r--   0        0        0      119 2023-10-31 04:58:26.000000 risb-0.0.5/docs/how-to/index.md
--rw-r--r--   0        0        0     2520 2023-10-31 04:58:26.000000 risb-0.0.5/docs/how-to/kweight.md
--rw-r--r--   0        0        0     7176 2023-10-31 04:58:26.000000 risb-0.0.5/docs/how-to/lattice_solver.md
--rw-r--r--   0        0        0     4622 2023-10-31 04:58:26.000000 risb-0.0.5/docs/how-to/projectors.md
--rw-r--r--   0        0        0     9168 2023-10-31 04:58:26.000000 risb-0.0.5/docs/how-to/quadratic_terms.md
--rw-r--r--   0        0        0    13537 2023-10-31 04:58:26.000000 risb-0.0.5/docs/tutorials/hubbard.md
--rw-r--r--   0        0        0       77 2023-10-31 04:58:26.000000 risb-0.0.5/docs/tutorials/index.md
--rw-r--r--   0        0        0     1977 2023-10-31 04:58:26.000000 risb-0.0.5/docs/tutorials/kagome.md
--rw-r--r--   0        0        0    19220 2023-10-31 04:58:26.000000 risb-0.0.5/docs/tutorials/self-consistent.md
--rw-r--r--   0        0        0     3407 2023-10-31 04:58:26.000000 risb-0.0.5/examples/bilayer_hubbard.py
--rw-r--r--   0        0        0     7530 2023-10-31 04:58:26.000000 risb-0.0.5/examples/decorated_honeycomb.py
--rw-r--r--   0        0        0     2785 2023-10-31 04:58:26.000000 risb-0.0.5/examples/hubbard.py
--rw-r--r--   0        0        0     4881 2023-10-31 04:58:26.000000 risb-0.0.5/examples/kagome_hubbard.py
--rw-r--r--   0        0        0      206 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/__init__.py
--rw-r--r--   0        0        0    17227 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/helpers.py
--rw-r--r--   0        0        0     5938 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/helpers_triqs.py
--rw-r--r--   0        0        0    27663 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/solve_lattice.py
--rw-r--r--   0        0        0      411 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/version.py
--rw-r--r--   0        0        0       84 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/embedding/__init__.py
--rw-r--r--   0        0        0     2561 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/embedding/dummy.py
--rw-r--r--   0        0        0    12048 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/embedding/embedding_atom_diag.py
--rw-r--r--   0        0        0       36 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/kweight/__init__.py
--rw-r--r--   0        0        0     1656 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/kweight/from_triqs_hartree.py
--rw-r--r--   0        0        0     4931 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/kweight/kweight.py
--rw-r--r--   0        0        0      234 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/optimize/__init__.py
--rw-r--r--   0        0        0     2969 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/optimize/diis.py
--rw-r--r--   0        0        0      640 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/optimize/linear_mixing.py
--rw-r--r--   0        0        0     6064 2023-10-31 04:58:26.000000 risb-0.0.5/src/risb/optimize/solver_newton.py
--rw-r--r--   0        0        0     1506 2023-10-31 04:58:26.000000 risb-0.0.5/tests/common.py
--rw-r--r--   0        0        0    13056 2023-10-31 04:58:26.000000 risb-0.0.5/tests/data_helpers.h5
--rw-r--r--   0        0        0     7541 2023-10-31 04:58:26.000000 risb-0.0.5/tests/test_atomdiag.py
--rw-r--r--   0        0        0     3450 2023-10-31 04:58:26.000000 risb-0.0.5/tests/test_helpers.py
--rw-r--r--   0        0        0     6360 2023-10-31 04:58:26.000000 risb-0.0.5/tests/test_latticesolver.py
--rw-r--r--   0        0        0      209 2023-10-31 04:58:26.000000 risb-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2023-10-31 04:58:26.000000 risb-0.0.5/LICENSE
--rw-r--r--   0        0        0     3984 2023-10-31 04:58:26.000000 risb-0.0.5/README.md
--rw-r--r--   0        0        0     1827 2023-10-31 04:58:26.000000 risb-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    45795 2023-10-31 04:58:26.000000 risb-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      202 2024-05-14 01:25:26.000000 risb-0.0.6/.dockerignore
+-rw-r--r--   0        0        0      124 2024-05-14 01:25:26.000000 risb-0.0.6/.git_archival.txt
+-rw-r--r--   0        0        0       98 2024-05-14 01:25:26.000000 risb-0.0.6/.gitattributes
+-rw-r--r--   0        0        0     3481 2024-05-14 01:25:26.000000 risb-0.0.6/CITATION
+-rw-r--r--   0        0        0      822 2024-05-14 01:25:26.000000 risb-0.0.6/COPYRIGHT
+-rw-r--r--   0        0        0     1168 2024-05-14 01:25:26.000000 risb-0.0.6/TODO.md
+-rw-r--r--   0        0        0       37 2024-05-14 01:25:26.000000 risb-0.0.6/.github/CODEOWNERS
+-rw-r--r--   0        0        0      223 2024-05-14 01:25:26.000000 risb-0.0.6/.github/dependabot.yml
+-rw-r--r--   0        0        0     3302 2024-05-14 01:25:26.000000 risb-0.0.6/.github/actions/setup-triqs/action.yml
+-rw-r--r--   0        0        0     2752 2024-05-14 01:25:26.000000 risb-0.0.6/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1776 2024-05-14 01:25:26.000000 risb-0.0.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      382 2024-05-14 01:25:26.000000 risb-0.0.6/docker/Dockerfile
+-rw-r--r--   0        0        0     3434 2024-05-14 01:25:26.000000 risb-0.0.6/docker/Dockerfile.dev
+-rw-r--r--   0        0        0      608 2024-05-14 01:25:26.000000 risb-0.0.6/docker/Dockerfile.docs
+-rw-r--r--   0        0        0      567 2024-05-14 01:25:26.000000 risb-0.0.6/docker/conda.sh
+-rw-r--r--   0        0        0      332 2024-05-14 01:25:26.000000 risb-0.0.6/docker/docker-compose-dev.yml
+-rw-r--r--   0        0        0      334 2024-05-14 01:25:26.000000 risb-0.0.6/docker/docker-compose-docs.yml
+-rw-r--r--   0        0        0      266 2024-05-14 01:25:26.000000 risb-0.0.6/docker/docker-compose.yml
+-rw-r--r--   0        0        0       10 2024-05-14 01:25:26.000000 risb-0.0.6/docs/.gitignore
+-rw-r--r--   0        0        0     3376 2024-05-14 01:25:26.000000 risb-0.0.6/docs/about.md
+-rw-r--r--   0        0        0     2359 2024-05-14 01:25:26.000000 risb-0.0.6/docs/conf.py
+-rw-r--r--   0        0        0      422 2024-05-14 01:25:26.000000 risb-0.0.6/docs/index.md
+-rw-r--r--   0        0        0      111 2024-05-14 01:25:26.000000 risb-0.0.6/docs/install.md
+-rw-r--r--   0        0        0     5636 2024-05-14 01:25:26.000000 risb-0.0.6/docs/explanations/embedding.md
+-rw-r--r--   0        0        0      114 2024-05-14 01:25:26.000000 risb-0.0.6/docs/explanations/index.md
+-rw-r--r--   0        0        0     2090 2024-05-14 01:25:26.000000 risb-0.0.6/docs/explanations/kweight.md
+-rw-r--r--   0        0        0     3176 2024-05-14 01:25:26.000000 risb-0.0.6/docs/explanations/projectors.md
+-rw-r--r--   0        0        0     2426 2024-05-14 01:25:26.000000 risb-0.0.6/docs/how-to/diis.md
+-rw-r--r--   0        0        0     5629 2024-05-14 01:25:26.000000 risb-0.0.6/docs/how-to/embedding.md
+-rw-r--r--   0        0        0      119 2024-05-14 01:25:26.000000 risb-0.0.6/docs/how-to/index.md
+-rw-r--r--   0        0        0     2520 2024-05-14 01:25:26.000000 risb-0.0.6/docs/how-to/kweight.md
+-rw-r--r--   0        0        0     7176 2024-05-14 01:25:26.000000 risb-0.0.6/docs/how-to/lattice_solver.md
+-rw-r--r--   0        0        0     4622 2024-05-14 01:25:26.000000 risb-0.0.6/docs/how-to/projectors.md
+-rw-r--r--   0        0        0     9168 2024-05-14 01:25:26.000000 risb-0.0.6/docs/how-to/quadratic_terms.md
+-rw-r--r--   0        0        0    13537 2024-05-14 01:25:26.000000 risb-0.0.6/docs/tutorials/hubbard.md
+-rw-r--r--   0        0        0       77 2024-05-14 01:25:26.000000 risb-0.0.6/docs/tutorials/index.md
+-rw-r--r--   0        0        0     1977 2024-05-14 01:25:26.000000 risb-0.0.6/docs/tutorials/kagome.md
+-rw-r--r--   0        0        0    19265 2024-05-14 01:25:26.000000 risb-0.0.6/docs/tutorials/self-consistent.md
+-rw-r--r--   0        0        0     3407 2024-05-14 01:25:26.000000 risb-0.0.6/examples/bilayer_hubbard.py
+-rw-r--r--   0        0        0     7530 2024-05-14 01:25:26.000000 risb-0.0.6/examples/decorated_honeycomb.py
+-rw-r--r--   0        0        0     4422 2024-05-14 01:25:26.000000 risb-0.0.6/examples/hubbard.py
+-rw-r--r--   0        0        0     4881 2024-05-14 01:25:26.000000 risb-0.0.6/examples/kagome_hubbard.py
+-rw-r--r--   0        0        0      206 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/__init__.py
+-rw-r--r--   0        0        0    17127 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/helpers.py
+-rw-r--r--   0        0        0     8233 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/helpers_triqs.py
+-rw-r--r--   0        0        0    27703 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/solve_lattice.py
+-rw-r--r--   0        0        0      411 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/version.py
+-rw-r--r--   0        0        0       84 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/embedding/__init__.py
+-rw-r--r--   0        0        0     2561 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/embedding/dummy.py
+-rw-r--r--   0        0        0    12048 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/embedding/embedding_atom_diag.py
+-rw-r--r--   0        0        0       36 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/kweight/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/kweight/from_triqs_hartree.py
+-rw-r--r--   0        0        0     4931 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/kweight/kweight.py
+-rw-r--r--   0        0        0      234 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/optimize/__init__.py
+-rw-r--r--   0        0        0     2969 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/optimize/diis.py
+-rw-r--r--   0        0        0      640 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/optimize/linear_mixing.py
+-rw-r--r--   0        0        0     6064 2024-05-14 01:25:26.000000 risb-0.0.6/src/risb/optimize/solver_newton.py
+-rw-r--r--   0        0        0     1506 2024-05-14 01:25:26.000000 risb-0.0.6/tests/common.py
+-rw-r--r--   0        0        0    13056 2024-05-14 01:25:26.000000 risb-0.0.6/tests/data_helpers.h5
+-rw-r--r--   0        0        0     7541 2024-05-14 01:25:26.000000 risb-0.0.6/tests/test_atomdiag.py
+-rw-r--r--   0        0        0     3482 2024-05-14 01:25:26.000000 risb-0.0.6/tests/test_helpers.py
+-rw-r--r--   0        0        0     6360 2024-05-14 01:25:26.000000 risb-0.0.6/tests/test_latticesolver.py
+-rw-r--r--   0        0        0      230 2024-05-14 01:25:26.000000 risb-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2024-05-14 01:25:26.000000 risb-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3984 2024-05-14 01:25:26.000000 risb-0.0.6/README.md
+-rw-r--r--   0        0        0     1775 2024-05-14 01:25:26.000000 risb-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    45795 2024-05-14 01:25:26.000000 risb-0.0.6/PKG-INFO
```

### Comparing `risb-0.0.5/CITATION` & `risb-0.0.6/CITATION`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/COPYRIGHT` & `risb-0.0.6/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/TODO.md` & `risb-0.0.6/TODO.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/.github/actions/setup-triqs/action.yml` & `risb-0.0.6/.github/actions/setup-triqs/action.yml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     required: false
 
 runs:
   using: "composite"
 
   steps:
   - name: Setup Python ${{ inputs.python-version }}
-    uses: actions/setup-python@v4
+    uses: actions/setup-python@v5
     with:
       python-version: ${{ inputs.python-version }}
       allow-prereleases: true
  
   - name: Install updates
     shell: bash
     run: |
@@ -102,15 +102,15 @@
     if: ${{ contains(inputs.cc, 'gcc') }}
     run: |
       echo "CC=${{ inputs.cc }}-${{ inputs.gcc-version }}" >> $GITHUB_ENV
       echo "CXX=${{ inputs.cxx }}-${{ inputs.gcc-version }}" >> $GITHUB_ENV
       
   - name: Cache build TRIQS
     id: build-triqs
-    uses: actions/cache@v3
+    uses: actions/cache@v4
     with:
       path: triqs
       key: triqs-${{ inputs.os }}-${{ inputs.python-version }} ${{ inputs.cc }}-${{ inputs.llvm }}-${{ inputs.gcc-version }}
 
   - name: Build TRIQS
     shell: bash
     if: steps.build-triqs.outputs.cache-hit != 'true'
```

### Comparing `risb-0.0.5/.github/workflows/cd.yml` & `risb-0.0.6/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/.github/workflows/ci.yml` & `risb-0.0.6/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,16 @@
   build:
     
     strategy:
       fail-fast: true
       matrix:
         include:
           - {os: "ubuntu-22.04", python-version: "3.10", cc: "gcc", cxx: "g++", llvm: "15", gcc-version: "12"}
-          #- {os: "ubuntu-22.04", python-version: "3.11", cc: "gcc", cxx: "g++", llvm: "15", gccversion: "12"}
+          - {os: "ubuntu-22.04", python-version: "3.11", cc: "gcc", cxx: "g++", llvm: "15", gcc-version: "12"}
+          - {os: "ubuntu-22.04", python-version: "3.12", cc: "gcc", cxx: "g++", llvm: "15", gcc-version: "12"}
           #- {os: "ubuntu-22.04", python-version: "3.10", cc: "clang", cxx: "clang++", llvm: "15", gcc-version: "12"}
           #- {os: "ubuntu-22.04", python-version: "3.11", cc: "clang", cxx: "clang++", llvm: "15", gcc-version: "12"}
   
     runs-on: ${{ matrix.os }}
     
     name: Test Python ${{ matrix.python-version }}
     steps:
```

### Comparing `risb-0.0.5/docker/Dockerfile.dev` & `risb-0.0.6/docker/Dockerfile.dev`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docker/Dockerfile.docs` & `risb-0.0.6/docker/Dockerfile.docs`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docker/conda.sh` & `risb-0.0.6/docker/conda.sh`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/about.md` & `risb-0.0.6/docs/about.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/conf.py` & `risb-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/explanations/embedding.md` & `risb-0.0.6/docs/explanations/embedding.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/explanations/kweight.md` & `risb-0.0.6/docs/explanations/kweight.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/explanations/projectors.md` & `risb-0.0.6/docs/explanations/projectors.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/how-to/diis.md` & `risb-0.0.6/docs/how-to/diis.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/how-to/embedding.md` & `risb-0.0.6/docs/how-to/embedding.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/how-to/kweight.md` & `risb-0.0.6/docs/how-to/kweight.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/how-to/lattice_solver.md` & `risb-0.0.6/docs/how-to/lattice_solver.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/how-to/projectors.md` & `risb-0.0.6/docs/how-to/projectors.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/how-to/quadratic_terms.md` & `risb-0.0.6/docs/how-to/quadratic_terms.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/tutorials/hubbard.md` & `risb-0.0.6/docs/tutorials/hubbard.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/tutorials/kagome.md` & `risb-0.0.6/docs/tutorials/kagome.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/docs/tutorials/self-consistent.md` & `risb-0.0.6/docs/tutorials/self-consistent.md`

 * *Files 1% similar despite different names*

```diff
@@ -226,25 +226,26 @@
 $\hat{H}^{\mathrm{kin}}_0$ was done.
 
 $\mathcal{R}$ and $\mathcal{\lambda}$ are mean-field matrices and are the 
 input initial guesses to the solution to the self-consistent loop. Often a 
 reasonable initial guess is to choose $\mathcal{R}$ as the identity and 
 $\lambda$ as the zero matrix.
 
-There is a helper function that constructs $\hat{H}^{\mathrm{qp}}$ and 
-returns its eigenvalues and eigenvectors at each $k$-point on the finite 
-grid.
+There is a helper function that constructs $\hat{H}^{\mathrm{qp}}$, and 
+it is simple to get its eigenvalues and eigenvectors at each $k$-point on the 
+finite grid.
 
 ```python
 from risb import helpers
 
 energies_qp = dict()
 bloch_vector_qp = dict()
 for bl, bl_size in gf_struct
-    energies_qp[bl], bloch_vector_qp[bl] = helpers.get_h_qp(R[bl], Lambda[bl], h0_kin_k[bl])
+    h_qp = helpers.get_h_qp(R[bl], Lambda[bl], h0_kin_k[bl])
+    energies_qp[bl], bloch_vector_qp[bl] = np.linalg.eigh(h_qp)
 ```
 
 ## D: Setup k-integrator function
 
 :::{seealso}
 [About k-integration](../explanations/kweight.md) for the theory of how 
 $k$-space integration is numerically done in most condensed matter codes.
```

### Comparing `risb-0.0.5/examples/bilayer_hubbard.py` & `risb-0.0.6/examples/bilayer_hubbard.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/examples/decorated_honeycomb.py` & `risb-0.0.6/examples/decorated_honeycomb.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/examples/kagome_hubbard.py` & `risb-0.0.6/examples/kagome_hubbard.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/src/risb/helpers.py` & `risb-0.0.6/src/risb/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,48 +244,47 @@
     return rho_f - rho_qp.T
 
 def get_h_qp(R : np.ndarray, 
              Lambda : np.ndarray, 
              h0_kin_k : np.ndarray, 
              mu : float = 0) -> tuple[ np.ndarray, np.ndarray ]:
     """
-    Construct eigenvalues and eigenvectors of the quasiparticle Hamiltonian.
+    Construct the quasiparticle Hamiltonian.
     
     Parameters
     ----------
     R : numpy.ndarray
-        Renormalization matrix) from electrons to quasiparticles.
+        Renormalization matrix) from electrons to quasiparticles
     Lambda : numpy.ndarray
         Correlation potential of quasiparticles.
     h0_kin_k : numpy.ndarray
         Single-particle dispersion between local clusters. Indexed as 
-        k, orb_i, orb_j.
+        k, orb_i, orb_j
     mu : float, optional
-        Chemical potential.
+        Chemical potential
 
     Return
     ------
-    eigenvalues : numpy.ndarray
-        Indexed as k, band.
-    eigenvectors : numpy.ndarray
-        Indexed as k, each column an eigenvector.
+    h_qp : numpy.ndarray
+        Indexed as k, orb_i, orb_j
     
     Notes
     -----
     Eq. A34 in `10.1103/PhysRevX.5.011008 <PRX011008_>`__.
 
     .. _PRX011008: https://doi.org/10.1103/PhysRevX.5.011008
     """
     #h_qp = np.einsum('ac,cdk,db->kab', R, h0_kin_k, R.conj().T, optimize='optimal') + (Lambda - mu*np.eye(Lambda.shape[0]))
     h_qp = np.einsum('ac,kcd,db->kab', R, h0_kin_k, R.conj().T) + \
         (Lambda - mu*np.eye(Lambda.shape[0]))
     if not np.allclose(h_qp, np.swapaxes(h_qp, 1, 2).conj()):
         warnings.warn("H_qp is not Hermitian !", RuntimeWarning)
-    eig, vec = np.linalg.eigh(h_qp)
-    return (eig, vec)
+    #eig, vec = np.linalg.eigh(h_qp)
+    #return (eig, vec)
+    return h_qp
 
 def get_h0_kin_k_R(R : np.ndarray, 
                    h0_kin_k : np.ndarray, 
                    vec : np.ndarray) -> np.ndarray:
     """
     Parameters
     ----------
```

### Comparing `risb-0.0.5/src/risb/solve_lattice.py` & `risb-0.0.6/src/risb/solve_lattice.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,16 @@
                 bl_full = self.gf_struct_mapping[0][bl]
                 self.R_full[bl_full] += self.R[0][bl]
                 self.Lambda_full[bl_full] += self.Lambda[0][bl]
         
         h0_k_R = dict()
         #R_h0_k_R = dict()
         for bl in self.h0_kin_k.keys():
-            self.energies_qp[bl], self.bloch_vector_qp[bl] = helpers.get_h_qp(self.R_full[bl], self.Lambda_full[bl], self.h0_kin_k[bl])
+            h_qp = helpers.get_h_qp(self.R_full[bl], self.Lambda_full[bl], self.h0_kin_k[bl])
+            self.energies_qp[bl], self.bloch_vector_qp[bl] = np.linalg.eigh(h_qp)
             h0_k_R[bl] = helpers.get_h0_kin_k_R(self.R_full[bl], self.h0_kin_k[bl], self.bloch_vector_qp[bl])
             #R_h0_k_R[bl] = helpers.get_R_h0_kin_kR(R_full[bl], self.h0_kin_k[bl], self.bloch_vector_qp[bl])
         
         self.kweights = self.update_weights(self.energies_qp, **kweight_param)
 
         for i in range(self.n_clusters):
             for bl, _ in self.gf_struct[i]:
```

### Comparing `risb-0.0.5/src/risb/embedding/dummy.py` & `risb-0.0.6/src/risb/embedding/dummy.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/src/risb/embedding/embedding_atom_diag.py` & `risb-0.0.6/src/risb/embedding/embedding_atom_diag.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/src/risb/kweight/from_triqs_hartree.py` & `risb-0.0.6/src/risb/kweight/from_triqs_hartree.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/src/risb/kweight/kweight.py` & `risb-0.0.6/src/risb/kweight/kweight.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/src/risb/optimize/diis.py` & `risb-0.0.6/src/risb/optimize/diis.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/src/risb/optimize/linear_mixing.py` & `risb-0.0.6/src/risb/optimize/linear_mixing.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/src/risb/optimize/solver_newton.py` & `risb-0.0.6/src/risb/optimize/solver_newton.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/tests/common.py` & `risb-0.0.6/tests/common.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/tests/data_helpers.h5` & `risb-0.0.6/tests/data_helpers.h5`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/tests/test_atomdiag.py` & `risb-0.0.6/tests/test_atomdiag.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/tests/test_helpers.py` & `risb-0.0.6/tests/test_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         h0_k = f['h0_k'][:]
         eig_expected = f['eig'][:]
         vec_expected = f['vec'][:]
     R = np.zeros(shape=(2,2))
     np.fill_diagonal(R, 1)
     Lambda = np.zeros(shape=(2,2))
     np.fill_diagonal(Lambda, 0.5)
-    eig, vec = helpers.get_h_qp(R, Lambda, h0_k)
+    h_qp = helpers.get_h_qp(R, Lambda, h0_k)
+    eig, vec = np.linalg.eigh(h_qp)
     with subtests.test(msg="eigenvalues"):
         assert eig == approx(eig_expected, abs=abs)
     with subtests.test(msg="eigenvectors"):
         assert vec == approx(vec_expected, abs=abs)
 
 def test_get_h0_kin_k_R():
     R = np.zeros(shape=(2,2))
```

### Comparing `risb-0.0.5/tests/test_latticesolver.py` & `risb-0.0.6/tests/test_latticesolver.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/LICENSE` & `risb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/README.md` & `risb-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.5/pyproject.toml` & `risb-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -51,16 +51,15 @@
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = [
-    "ignore:invalid escape sequence:DeprecationWarning",
-    "error",
+  "error:::risb",
 ]
 log_cli_level = "info"
 testpaths = [
   "tests",
 ]
 
 [tool.mypy]
```

### Comparing `risb-0.0.5/PKG-INFO` & `risb-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: risb
-Version: 0.0.5
+Version: 0.0.6
 Summary: Rotationally invariant slave boson mean-field theory.
 Project-URL: Homepage, https://github.com/thenoursehorse/risb
 Project-URL: Documentation, https://thenoursehorse.github.io/risb
 Author: H. L. Nourse
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

