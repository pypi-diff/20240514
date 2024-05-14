# Comparing `tmp/numqi-0.1.1b0.tar.gz` & `tmp/numqi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numqi-0.1.1b0.tar", last modified: Mon Mar 25 02:54:07 2024, max compression
+gzip compressed data, was "numqi-0.2.0.tar", last modified: Tue May 14 16:04:18 2024, max compression
```

## Comparing `numqi-0.1.1b0.tar` & `numqi-0.2.0.tar`

### file list

```diff
@@ -1,401 +1,406 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.142752 numqi-0.1.1b0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.070752 numqi-0.1.1b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.082752 numqi-0.1.1b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-25 02:54:02.000000 numqi-0.1.1b0/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-25 02:54:02.000000 numqi-0.1.1b0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-25 02:54:02.000000 numqi-0.1.1b0/.github/workflows/unittest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-25 02:54:02.000000 numqi-0.1.1b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-25 02:54:02.000000 numqi-0.1.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-03-25 02:54:07.142752 numqi-0.1.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-03-25 02:54:02.000000 numqi-0.1.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.082752 numqi-0.1.1b0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.086752 numqi-0.1.1b0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/dicke.md
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/entangle.md
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/entangle_cha.md
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/entangle_eof.md
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/entangle_measure.md
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/entangle_ppt.md
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/entangle_pureb.md
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/entangle_symext.md
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/entangle_upb.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/gate.md
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/gellmann.md
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/group.md
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/group_lie.md
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/group_spf2.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/group_sym.md
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/group_symext.md
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/manifold.md
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/matrix_space.md
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/random.md
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/sim.md
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/sim_dm.md
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/sim_state.md
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/state.md
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/unique_determine.md
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/api/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.074752 numqi-0.1.1b0/docs/application/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.086752 numqi-0.1.1b0/docs/application/circuit/
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/circuit/basic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/circuit/customized_gate.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/circuit/gate_decomposition.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.086752 numqi-0.1.1b0/docs/application/communication/
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/communication/channel_capacity_1_inf.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.086752 numqi-0.1.1b0/docs/application/control/
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/control/simulate_dynamics.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.086752 numqi-0.1.1b0/docs/application/entangle/
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/entangle/bipartite.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/entangle/boundary_method.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/entangle/cha.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/entangle/gme_subspace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/entangle/measure.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/entangle/multipartite.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/entangle/overview_method.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/entangle/pureb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/entangle/sym_bos_ext.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.086752 numqi-0.1.1b0/docs/application/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/geometry/bloch_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/geometry/numerical_range_dm.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.086752 numqi-0.1.1b0/docs/application/get_started/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/get_started/overview.md
--rw-r--r--   0 runner    (1001) docker     (127)    12686 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/get_started/quantum_state.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.090752 numqi-0.1.1b0/docs/application/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/misc/advanced01.md
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/misc/maxent.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/misc/query_grover.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/misc/special_state.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/misc/three_is_different.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.090752 numqi-0.1.1b0/docs/application/qecc/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/qecc/basic.md
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/qecc/qecc733.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/qecc/varqecc.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.090752 numqi-0.1.1b0/docs/application/tomography/
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/tomography/advanced00.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/tomography/advanced01.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/tomography/basic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/tomography/channel_tomography.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/tomography/optimal_povm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/application/tomography/state_tomography.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.094752 numqi-0.1.1b0/docs/data/
--rw-r--r--   0 runner    (1001) docker     (127)    32356 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/data/circuit_basic_pgate.png
--rw-r--r--   0 runner    (1001) docker     (127)   131375 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/data/detect_entanglement.png
--rw-r--r--   0 runner    (1001) docker     (127)   252677 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/data/maxent_2qubit_pauli.png
--rw-r--r--   0 runner    (1001) docker     (127)   175520 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/data/maxent_3qubit_2local_random.png
--rw-r--r--   0 runner    (1001) docker     (127)   209136 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/data/maxent_4qubit_2local_random.png
--rw-r--r--   0 runner    (1001) docker     (127)    75201 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/data/project-structure.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.074752 numqi-0.1.1b0/docs/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.094752 numqi-0.1.1b0/docs/foundation/group/
--rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/group/basic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/group/clifford.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/group/pauli.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/group/spf2.md
--rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/group/symext.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/group/young-tableaux.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.094752 numqi-0.1.1b0/docs/foundation/manifold/
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/manifold/basic_sphere.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/manifold/basic_stiefel.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/manifold/trivialization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.094752 numqi-0.1.1b0/docs/foundation/matrix_space/
--rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/matrix_space/numerical_range.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/matrix_space/numerical_range1.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11168 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/matrix_space/space_schmidt_rank.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/matrix_space/space_schmidt_rank_real.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.094752 numqi-0.1.1b0/docs/foundation/misc/
--rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/misc/dicke.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/misc/gellmann.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/misc/random.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.094752 numqi-0.1.1b0/docs/foundation/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/optimize/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/optimize/adam-vs-lbfgs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/optimize/basic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/optimize/wiki-test-function-ALM.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22551 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/foundation/optimize/wiki-test-function.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-25 02:54:02.000000 numqi-0.1.1b0/docs/misc.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.098752 numqi-0.1.1b0/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.098752 numqi-0.1.1b0/example/data/
--rw-r--r--   0 runner    (1001) docker     (127)   131326 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/data/20220905_realign_upb_bes.png
--rw-r--r--   0 runner    (1001) docker     (127)    64162 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/data/demo_get_ABk_symmetric_extension_ree_werner.png
--rw-r--r--   0 runner    (1001) docker     (127)    70594 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/data/demo_pureb_quantum_werner.png
--rw-r--r--   0 runner    (1001) docker     (127)    87853 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/data/demo_tiles_upb_pureb_ree.png
--rw-r--r--   0 runner    (1001) docker     (127)    93840 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/data/superactivation-loss.png
--rw-r--r--   0 runner    (1001) docker     (127)    62778 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/data/superactivation_landscope_random.png
--rw-r--r--   0 runner    (1001) docker     (127)    90289 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/data/superactivation_landscope_xystar.png
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/demo_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/demo_sqrtm_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/demo_superactivation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/demo_unique_determine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.098752 numqi-0.1.1b0/example/ws_entangle/
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/ws_entangle/demo_symext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/ws_entangle/draft_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/ws_entangle/draft_find_BES.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/ws_entangle/draft_ppt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/ws_entangle/draft_pureb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-03-25 02:54:02.000000 numqi-0.1.1b0/example/ws_entangle/draft_ree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-03-25 02:54:02.000000 numqi-0.1.1b0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.098752 numqi-0.1.1b0/project/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.102752 numqi-0.1.1b0/project/entangled_subspace/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.102752 numqi-0.1.1b0/project/entangled_subspace/data/
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/Maciej2019_bipartite_gm.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/analytic_gm.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/analytic_gm.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   148850 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/analytic_gm.png
--rw-r--r--   0 runner    (1001) docker     (127)    15768 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/qubit_dicke_state_border_rank.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/qubit_dicke_state_border_rank.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   148698 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/qubit_dicke_state_border_rank.png
--rw-r--r--   0 runner    (1001) docker     (127)    15885 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/robustness.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   480381 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/robustness.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    71423 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/data/robustness.png
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/demo_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/demo_schmidt_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/draft_ces.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/draft_graph_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/draft_paper_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangled_subspace/draft_pymanopt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.102752 numqi-0.1.1b0/project/entangler/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/entangler/draft00.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.106752 numqi-0.1.1b0/project/gme_dm/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/gme_dm/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/gme_dm/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/gme_dm/draft01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.106752 numqi-0.1.1b0/project/ws00/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws00/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws00/draft02.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws00/draft04.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws00/draft_rayleigh_quotient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.106752 numqi-0.1.1b0/project/ws_ame/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_ame/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_ame/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_ame/draft01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.106752 numqi-0.1.1b0/project/ws_ce/
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_ce/draft00.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.106752 numqi-0.1.1b0/project/ws_clifford/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_clifford/draft00.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.106752 numqi-0.1.1b0/project/ws_dmrg/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_dmrg/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_dmrg/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_dmrg/draft01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.106752 numqi-0.1.1b0/project/ws_gme/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_gme/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_gme/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)    47416 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_gme/ghz3_basic.png
--rw-r--r--   0 runner    (1001) docker     (127)    46992 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_gme/ghz4_basic.png
--rw-r--r--   0 runner    (1001) docker     (127)    49424 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_gme/ghz5_basic.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.110752 numqi-0.1.1b0/project/ws_iUD/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_iUD/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_iUD/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_iUD/draft01.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_iUD/draft02.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_iUD/draft03.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_iUD/draft04.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_iUD/draft05.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.110752 numqi-0.1.1b0/project/ws_irrep/
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_irrep/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_irrep/SymmetricExtensionBoundary.m
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_irrep/demo_hermitian_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_irrep/demo_qetlab_time.m
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_irrep/draft00.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.110752 numqi-0.1.1b0/project/ws_numerical_range/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.114752 numqi-0.1.1b0/project/ws_numerical_range/data/
--rw-r--r--   0 runner    (1001) docker     (127)   182565 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k3_ppt_pyramid_tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)   122790 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k3_werner_isotropic.png
--rw-r--r--   0 runner    (1001) docker     (127)   148919 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k3_werner_tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)   199060 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k4_werner_isotropic.png
--rw-r--r--   0 runner    (1001) docker     (127)   181870 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k5_ppt_pyramid_tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)    63622 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/eigen_degen_2x2_4ext.png
--rw-r--r--   0 runner    (1001) docker     (127)    95117 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/example-1b.png
--rw-r--r--   0 runner    (1001) docker     (127)    90869 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/example-1c.png
--rw-r--r--   0 runner    (1001) docker     (127)   145927 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/example-abc.png
--rw-r--r--   0 runner    (1001) docker     (127)    52467 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/data/rand_2x2_4ext.png
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/draft01.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/draft03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_numerical_range/draft04.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.114752 numqi-0.1.1b0/project/ws_optimal_control/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_optimal_control/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_optimal_control/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_optimal_control/draft01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.114752 numqi-0.1.1b0/project/ws_pureb/
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_pureb/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_pureb/draft01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.114752 numqi-0.1.1b0/project/ws_qec733/
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_qec733/draft00.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.114752 numqi-0.1.1b0/project/ws_qnn_material/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_qnn_material/draft00.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.118752 numqi-0.1.1b0/project/ws_sep_classifier/
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/draft01.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/draft02.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/draft_bes_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/draft_haar_k.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.118752 numqi-0.1.1b0/project/ws_sep_classifier/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    39152 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/fig/clf_logits_dist.png
--rw-r--r--   0 runner    (1001) docker     (127)    83008 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/fig/clf_random_random.png
--rw-r--r--   0 runner    (1001) docker     (127)    71284 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/fig/clf_werner_isotropic.png
--rw-r--r--   0 runner    (1001) docker     (127)    91449 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/fig/clf_werner_tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)    56547 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/fig/ginibre_sep.png
--rw-r--r--   0 runner    (1001) docker     (127)    76103 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/fig/regr_werner_isotropic.png
--rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/ppt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/ppt_rank_sampling.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/qudit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/qudit_rank_sampling.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/sep.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_sep_classifier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.118752 numqi-0.1.1b0/project/ws_trotter/
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_trotter/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_trotter/draft01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.122752 numqi-0.1.1b0/project/ws_upb/
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_upb/draft00.py
--rw-r--r--   0 runner    (1001) docker     (127)   216704 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_upb/upb-genshifts-graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   639023 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_upb/upb-gentiles1-graph.png
--rw-r--r--   0 runner    (1001) docker     (127)   522015 2024-03-25 02:54:02.000000 numqi-0.1.1b0/project/ws_upb/upb-gentiles2-graph.png
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-25 02:54:02.000000 numqi-0.1.1b0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.078752 numqi-0.1.1b0/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.122752 numqi-0.1.1b0/python/numqi/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.122752 numqi-0.1.1b0/python/numqi/_data/
--rw-r--r--   0 runner    (1001) docker     (127)   612708 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/_data/pauli_ud_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/_torch_op.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-25 02:54:06.000000 numqi-0.1.1b0/python/numqi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.126752 numqi-0.1.1b0/python/numqi/channel/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/channel/_gradient_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/channel/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/dicke.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.126752 numqi-0.1.1b0/python/numqi/entangle/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/cha.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/eof.py
--rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    18230 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/ppt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/pureb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/pureb_quantum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18141 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/symext.py
--rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/entangle/upb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.126752 numqi-0.1.1b0/python/numqi/gate/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/gate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/gate/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    17987 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/gate/_pauli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/gellmann.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.126752 numqi-0.1.1b0/python/numqi/group/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/group/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/group/_lie.py
--rw-r--r--   0 runner    (1001) docker     (127)    16166 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/group/_symmetric.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/group/spf2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/group/symext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.130752 numqi-0.1.1b0/python/numqi/manifold/
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/manifold/_ABk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/manifold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/manifold/_compose.py
--rw-r--r--   0 runner    (1001) docker     (127)    34318 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/manifold/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/manifold/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18139 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/manifold/_stiefel.py
--rw-r--r--   0 runner    (1001) docker     (127)    19326 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/manifold/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.130752 numqi-0.1.1b0/python/numqi/matrix_space/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/matrix_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/matrix_space/_clebsch_gordan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/matrix_space/_geometric_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    18076 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/matrix_space/_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/matrix_space/_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)    21252 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/matrix_space/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/matrix_space/_numerical_range.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.130752 numqi-0.1.1b0/python/numqi/maximum_entropy/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/maximum_entropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/maximum_entropy/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/maximum_entropy/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/optimal_control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.130752 numqi-0.1.1b0/python/numqi/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/optimize/_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.130752 numqi-0.1.1b0/python/numqi/qec/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/qec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/qec/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/qec/_qecc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/qec/_varqec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.134752 numqi-0.1.1b0/python/numqi/query/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/query/_gradient_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/query/_sdp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/query/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.134752 numqi-0.1.1b0/python/numqi/random/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20231 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/random/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/random/_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/random/_spf2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.134752 numqi-0.1.1b0/python/numqi/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/sim/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/sim/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/sim/_torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/sim/circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/sim/clifford.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/sim/dm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/sim/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.134752 numqi-0.1.1b0/python/numqi/state/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/state/_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.134752 numqi-0.1.1b0/python/numqi/unique_determine/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/unique_determine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/unique_determine/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/unique_determine/_recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/unique_determine/_uda_udp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14529 2024-03-25 02:54:02.000000 numqi-0.1.1b0/python/numqi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.142752 numqi-0.1.1b0/python/numqi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-03-25 02:54:06.000000 numqi-0.1.1b0/python/numqi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-03-25 02:54:07.000000 numqi-0.1.1b0/python/numqi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 02:54:06.000000 numqi-0.1.1b0/python/numqi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-25 02:54:06.000000 numqi-0.1.1b0/python/numqi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 02:54:06.000000 numqi-0.1.1b0/python/numqi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 02:54:07.142752 numqi-0.1.1b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.138752 numqi-0.1.1b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_dicke.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.138752 numqi-0.1.1b0/tests/test_entangle/
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_entangle/test_entangle_bes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_entangle/test_entangle_cha.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_entangle/test_entangle_eof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_entangle/test_entangle_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_entangle/test_entangle_ppt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_entangle/test_entangle_pureb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_entangle/test_entangle_symext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_entangle/test_entangle_upb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_entangle/test_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_gellmann.py
--rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_manifold.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_manifold_ABk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_maximum_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_optimal_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_qec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_torch_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_unique_determine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.138752 numqi-0.1.1b0/tests/tests_group/
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_group/test_group_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_group/test_group_lie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_group/test_group_spf2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_group/test_group_symext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_group/test_group_symmetric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.142752 numqi-0.1.1b0/tests/tests_matrix_space/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_matrix_space/test_geometric_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    15919 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_clebsch_gordan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_numerical_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_superactivation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:54:07.142752 numqi-0.1.1b0/tests/tests_sim/
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_sim/test_sim_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_sim/test_sim_clifford.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_sim/test_sim_dm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-25 02:54:02.000000 numqi-0.1.1b0/tests/tests_sim/test_sim_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.974701 numqi-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.906701 numqi-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.914701 numqi-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-14 16:04:13.000000 numqi-0.2.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-14 16:04:13.000000 numqi-0.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-14 16:04:13.000000 numqi-0.2.0/.github/workflows/unittest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 16:04:13.000000 numqi-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-14 16:04:13.000000 numqi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-05-14 16:04:18.974701 numqi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-14 16:04:13.000000 numqi-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.914701 numqi-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.918701 numqi-0.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/dicke.md
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/entangle.md
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/entangle_cha.md
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/entangle_eof.md
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/entangle_measure.md
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/entangle_ppt.md
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/entangle_pureb.md
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/entangle_symext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/entangle_upb.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/gate.md
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/gellmann.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/group.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/group_lie.md
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/group_spf2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/group_sym.md
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/group_symext.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/manifold.md
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/matrix_space.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/random.md
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/sim.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/sim_dm.md
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/sim_state.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/state.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/unique_determine.md
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/api/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.906701 numqi-0.2.0/docs/application/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.918701 numqi-0.2.0/docs/application/circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/circuit/basic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/circuit/customized_gate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/circuit/gate_decomposition.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.918701 numqi-0.2.0/docs/application/communication/
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/communication/channel_capacity_1_inf.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.918701 numqi-0.2.0/docs/application/control/
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/control/simulate_dynamics.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.922701 numqi-0.2.0/docs/application/entangle/
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/entangle/bipartite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/entangle/boundary_method.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/entangle/cha.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/entangle/gme_subspace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18109 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/entangle/measure.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/entangle/multipartite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/entangle/overview_method.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/entangle/pureb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/entangle/sym_bos_ext.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.922701 numqi-0.2.0/docs/application/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)    16641 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/geometry/bloch_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/geometry/numerical_range_dm.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.922701 numqi-0.2.0/docs/application/get_started/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/get_started/overview.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13041 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/get_started/quantum_state.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.922701 numqi-0.2.0/docs/application/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/misc/advanced01.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/misc/maxent.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/misc/query_grover.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/misc/special_state.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/misc/three_is_different.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.922701 numqi-0.2.0/docs/application/qecc/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/qecc/basic.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/qecc/qecc733.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/qecc/varqecc.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.922701 numqi-0.2.0/docs/application/tomography/
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/tomography/advanced00.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/tomography/advanced01.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/tomography/basic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/tomography/channel_tomography.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/tomography/optimal_povm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/application/tomography/state_tomography.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.926701 numqi-0.2.0/docs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    32356 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/data/circuit_basic_pgate.png
+-rw-r--r--   0 runner    (1001) docker     (127)   131375 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/data/detect_entanglement.png
+-rw-r--r--   0 runner    (1001) docker     (127)   252677 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/data/maxent_2qubit_pauli.png
+-rw-r--r--   0 runner    (1001) docker     (127)   175520 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/data/maxent_3qubit_2local_random.png
+-rw-r--r--   0 runner    (1001) docker     (127)   209136 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/data/maxent_4qubit_2local_random.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75201 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/data/project-structure.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.906701 numqi-0.2.0/docs/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.926701 numqi-0.2.0/docs/foundation/get_started/
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/get_started/get_started.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.926701 numqi-0.2.0/docs/foundation/group/
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/group/basic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/group/clifford.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/group/pauli.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/group/spf2.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/group/symext.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/group/young-tableaux.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.926701 numqi-0.2.0/docs/foundation/manifold/
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/manifold/basic_sphere.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/manifold/basic_stiefel.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/manifold/trivialization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.926701 numqi-0.2.0/docs/foundation/matrix_space/
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/matrix_space/numerical_range.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/matrix_space/numerical_range1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11569 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/matrix_space/space_schmidt_rank.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/matrix_space/space_schmidt_rank_real.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.930701 numqi-0.2.0/docs/foundation/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/misc/dicke.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/misc/gellmann.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/misc/random.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.930701 numqi-0.2.0/docs/foundation/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/optimize/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/optimize/adam-vs-lbfgs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/optimize/basic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/optimize/wiki-test-function-ALM.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22938 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/foundation/optimize/wiki-test-function.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-14 16:04:13.000000 numqi-0.2.0/docs/misc.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.930701 numqi-0.2.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.930701 numqi-0.2.0/example/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   131326 2024-05-14 16:04:13.000000 numqi-0.2.0/example/data/20220905_realign_upb_bes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64162 2024-05-14 16:04:13.000000 numqi-0.2.0/example/data/demo_get_ABk_symmetric_extension_ree_werner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70594 2024-05-14 16:04:13.000000 numqi-0.2.0/example/data/demo_pureb_quantum_werner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    87853 2024-05-14 16:04:13.000000 numqi-0.2.0/example/data/demo_tiles_upb_pureb_ree.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93840 2024-05-14 16:04:13.000000 numqi-0.2.0/example/data/superactivation-loss.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62778 2024-05-14 16:04:13.000000 numqi-0.2.0/example/data/superactivation_landscope_random.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90289 2024-05-14 16:04:13.000000 numqi-0.2.0/example/data/superactivation_landscope_xystar.png
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 16:04:13.000000 numqi-0.2.0/example/demo_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-14 16:04:13.000000 numqi-0.2.0/example/demo_sqrtm_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-05-14 16:04:13.000000 numqi-0.2.0/example/demo_superactivation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-14 16:04:13.000000 numqi-0.2.0/example/demo_unique_determine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.934701 numqi-0.2.0/example/ws_entangle/
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-14 16:04:13.000000 numqi-0.2.0/example/ws_entangle/demo_symext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-14 16:04:13.000000 numqi-0.2.0/example/ws_entangle/draft_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-14 16:04:13.000000 numqi-0.2.0/example/ws_entangle/draft_find_BES.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-14 16:04:13.000000 numqi-0.2.0/example/ws_entangle/draft_ppt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-14 16:04:13.000000 numqi-0.2.0/example/ws_entangle/draft_pureb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-05-14 16:04:13.000000 numqi-0.2.0/example/ws_entangle/draft_ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-14 16:04:13.000000 numqi-0.2.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.934701 numqi-0.2.0/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-14 16:04:13.000000 numqi-0.2.0/project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.934701 numqi-0.2.0/project/entangled_subspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.938701 numqi-0.2.0/project/entangled_subspace/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/Maciej2019_bipartite_gm.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/analytic_gm.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/analytic_gm.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   148850 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/analytic_gm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15768 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/qubit_dicke_state_border_rank.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/qubit_dicke_state_border_rank.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   148698 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/qubit_dicke_state_border_rank.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15885 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/robustness.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   480381 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/robustness.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    71423 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/data/robustness.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/demo_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/demo_schmidt_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/draft_ces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/draft_graph_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/draft_paper_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangled_subspace/draft_pymanopt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.938701 numqi-0.2.0/project/entangler/
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangler/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-14 16:04:13.000000 numqi-0.2.0/project/entangler/draft01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.938701 numqi-0.2.0/project/gme_dm/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 16:04:13.000000 numqi-0.2.0/project/gme_dm/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-14 16:04:13.000000 numqi-0.2.0/project/gme_dm/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-14 16:04:13.000000 numqi-0.2.0/project/gme_dm/draft01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.938701 numqi-0.2.0/project/ws00/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws00/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws00/draft02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws00/draft04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws00/draft_rayleigh_quotient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.938701 numqi-0.2.0/project/ws_ame/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_ame/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_ame/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_ame/draft01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.938701 numqi-0.2.0/project/ws_ce/
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_ce/draft00.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.938701 numqi-0.2.0/project/ws_clifford/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_clifford/draft00.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.938701 numqi-0.2.0/project/ws_dmrg/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_dmrg/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_dmrg/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_dmrg/draft01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.938701 numqi-0.2.0/project/ws_gme/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_gme/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_gme/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47416 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_gme/ghz3_basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46992 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_gme/ghz4_basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49424 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_gme/ghz5_basic.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.942701 numqi-0.2.0/project/ws_iUD/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_iUD/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_iUD/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_iUD/draft01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_iUD/draft02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_iUD/draft03.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_iUD/draft04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_iUD/draft05.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.942701 numqi-0.2.0/project/ws_irrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_irrep/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_irrep/SymmetricExtensionBoundary.m
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_irrep/demo_hermitian_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_irrep/demo_qetlab_time.m
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_irrep/draft00.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.942701 numqi-0.2.0/project/ws_numerical_range/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.946701 numqi-0.2.0/project/ws_numerical_range/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   182565 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/3x3_k3_ppt_pyramid_tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122790 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/3x3_k3_werner_isotropic.png
+-rw-r--r--   0 runner    (1001) docker     (127)   148919 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/3x3_k3_werner_tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)   199060 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/3x3_k4_werner_isotropic.png
+-rw-r--r--   0 runner    (1001) docker     (127)   181870 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/3x3_k5_ppt_pyramid_tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63622 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/eigen_degen_2x2_4ext.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95117 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/example-1b.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90869 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/example-1c.png
+-rw-r--r--   0 runner    (1001) docker     (127)   145927 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/example-abc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    52467 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/data/rand_2x2_4ext.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/draft01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/draft03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_numerical_range/draft04.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.946701 numqi-0.2.0/project/ws_optimal_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_optimal_control/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_optimal_control/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_optimal_control/draft01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.946701 numqi-0.2.0/project/ws_pureb/
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_pureb/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_pureb/draft01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.946701 numqi-0.2.0/project/ws_qec733/
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_qec733/draft00.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.946701 numqi-0.2.0/project/ws_qnn_material/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_qnn_material/draft00.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.950701 numqi-0.2.0/project/ws_sep_classifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/draft01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/draft02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/draft_bes_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/draft_haar_k.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.950701 numqi-0.2.0/project/ws_sep_classifier/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    39152 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/fig/clf_logits_dist.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83008 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/fig/clf_random_random.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71284 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/fig/clf_werner_isotropic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91449 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/fig/clf_werner_tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56547 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/fig/ginibre_sep.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76103 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/fig/regr_werner_isotropic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/ppt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/ppt_rank_sampling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/qudit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/qudit_rank_sampling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/sep.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_sep_classifier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.950701 numqi-0.2.0/project/ws_trotter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_trotter/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_trotter/draft01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.950701 numqi-0.2.0/project/ws_upb/
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_upb/draft00.py
+-rw-r--r--   0 runner    (1001) docker     (127)   216704 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_upb/upb-genshifts-graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   639023 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_upb/upb-gentiles1-graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   522015 2024-05-14 16:04:13.000000 numqi-0.2.0/project/ws_upb/upb-gentiles2-graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 16:04:13.000000 numqi-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.910701 numqi-0.2.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.954701 numqi-0.2.0/python/numqi/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.954701 numqi-0.2.0/python/numqi/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   612708 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/_data/pauli_ud_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/_torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 16:04:18.000000 numqi-0.2.0/python/numqi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.954701 numqi-0.2.0/python/numqi/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/channel/_gradient_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/channel/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/dicke.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.958701 numqi-0.2.0/python/numqi/entangle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/cha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/eof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18230 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/pureb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/pureb_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18141 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/symext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15875 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/entangle/upb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.958701 numqi-0.2.0/python/numqi/gate/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/gate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/gate/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17987 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/gate/_pauli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/gellmann.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.958701 numqi-0.2.0/python/numqi/group/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/group/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/group/_lie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16166 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/group/_symmetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/group/spf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/group/symext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.958701 numqi-0.2.0/python/numqi/manifold/
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/manifold/_ABk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/manifold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/manifold/_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34347 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/manifold/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/manifold/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/manifold/_stiefel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19326 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/manifold/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.962701 numqi-0.2.0/python/numqi/matrix_space/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/matrix_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/matrix_space/_clebsch_gordan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/matrix_space/_geometric_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18076 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/matrix_space/_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/matrix_space/_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21252 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/matrix_space/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/matrix_space/_numerical_range.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.962701 numqi-0.2.0/python/numqi/maximum_entropy/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/maximum_entropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/maximum_entropy/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/maximum_entropy/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/optimal_control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.962701 numqi-0.2.0/python/numqi/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/optimize/_internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.962701 numqi-0.2.0/python/numqi/qec/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/qec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/qec/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/qec/_qecc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/qec/_varqec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.962701 numqi-0.2.0/python/numqi/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/query/_gradient_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/query/_sdp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/query/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.962701 numqi-0.2.0/python/numqi/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20231 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/random/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/random/_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/random/_spf2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.966701 numqi-0.2.0/python/numqi/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/sim/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/sim/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/sim/_torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19960 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/sim/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/sim/clifford.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/sim/dm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/sim/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.966701 numqi-0.2.0/python/numqi/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13227 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/state/_internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.966701 numqi-0.2.0/python/numqi/unique_determine/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/unique_determine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/unique_determine/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/unique_determine/_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/unique_determine/_uda_udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14515 2024-05-14 16:04:13.000000 numqi-0.2.0/python/numqi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.970701 numqi-0.2.0/python/numqi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-05-14 16:04:18.000000 numqi-0.2.0/python/numqi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-05-14 16:04:18.000000 numqi-0.2.0/python/numqi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:04:18.000000 numqi-0.2.0/python/numqi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-14 16:04:18.000000 numqi-0.2.0/python/numqi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 16:04:18.000000 numqi-0.2.0/python/numqi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.966701 numqi-0.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-14 16:04:13.000000 numqi-0.2.0/scripts/draft_action_mkdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:04:18.974701 numqi-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.966701 numqi-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_dicke.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.970701 numqi-0.2.0/tests/test_entangle/
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_entangle/test_entangle_bes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_entangle/test_entangle_cha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_entangle/test_entangle_eof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_entangle/test_entangle_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_entangle/test_entangle_ppt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_entangle/test_entangle_pureb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_entangle/test_entangle_symext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_entangle/test_entangle_upb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_entangle/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_gellmann.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13429 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_manifold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_manifold_ABk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_maximum_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_optimal_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_qec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_unique_determine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.970701 numqi-0.2.0/tests/tests_group/
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_group/test_group_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_group/test_group_lie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_group/test_group_spf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_group/test_group_symext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_group/test_group_symmetric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.970701 numqi-0.2.0/tests/tests_matrix_space/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_matrix_space/test_geometric_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15919 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_matrix_space/test_matrix_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_clebsch_gordan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_numerical_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_superactivation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:04:18.970701 numqi-0.2.0/tests/tests_sim/
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_sim/test_sim_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_sim/test_sim_clifford.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_sim/test_sim_dm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-14 16:04:13.000000 numqi-0.2.0/tests/tests_sim/test_sim_state.py
```

### Comparing `numqi-0.1.1b0/.github/workflows/doc.yml` & `numqi-0.2.0/.github/workflows/doc.yml`

 * *Files 7% similar despite different names*

```diff
@@ -32,35 +32,39 @@
     runs-on: ubuntu-latest
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     steps:
       - uses: actions/checkout@v3
 
+        with:
+          fetch-depth: 0
+          # see https://github.com/actions/checkout and https://github.com/timvink/mkdocs-git-revision-date-localized-plugin for this parameter
+
       - name: Setup Python
         uses: actions/setup-python@v4
 
       - name: Upgrade pip
         run: python3 -m pip install --upgrade pip
 
       - name: install jupyter
         run: python3 -m pip install --upgrade pip jupyter ipywidgets
 
-      - name: install cvxpy-1.3
-        # cvxpy-1.4.0 has bad performance issue on SDP see https://github.com/cvxpy/cvxpy/issues/2257
-        run: python3 -m pip install "cvxpy<1.4"
-
       # pypi defaults to cuda-torch which is not necessary
       - name: install torch-cpu
         run: python3 -m pip install torch --index-url https://download.pytorch.org/whl/cpu
 
       - name: install numqi
         run: python3 -m pip install -e .[dev]
 
-      - run: OMP_NUM_THREADS=1 mkdocs build
+      - name: set parameters in mkdocs.yml
+        run: python3 scripts/draft_action_mkdocs.py
+
+      - name: run mkdocs
+        run: OMP_NUM_THREADS=1 mkdocs build
 
       - name: Upload artifact
         uses: actions/upload-pages-artifact@v1
         with:
           # Upload entire repository
           path: 'site'
       - name: Deploy to GitHub Pages
```

### Comparing `numqi-0.1.1b0/.github/workflows/pypi-publish.yml` & `numqi-0.2.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/.github/workflows/unittest.yml` & `numqi-0.2.0/.github/workflows/unittest.yml`

 * *Files 10% similar despite different names*

```diff
@@ -32,17 +32,17 @@
       - name: install numqi
         run: python3 -m pip install -e .[dev]
 
       - name: run pytest
         run: OMP_NUM_THREADS=1 python3 -m pytest -n auto --cov=python/numqi --durations=10 tests/
 
       - name: Upload coverage reports to Codecov
-        uses: codecov/codecov-action@v3
-        env:
-          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+        uses: codecov/codecov-action@v4.0.1
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
 
       # TODO
       # - name: Upload coverage report
       #   uses: codecov/codecov-action@v3
       #   with:
       #     token: ${{ secrets.CODECOV_TOKEN }}
       #     fail_ci_if_error: false
```

### Comparing `numqi-0.1.1b0/LICENSE` & `numqi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/PKG-INFO` & `numqi-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 Metadata-Version: 2.1
 Name: numqi
-Version: 0.1.1b0
+Version: 0.2.0
 Summary: a numpy-based quantum information toolbox
 Author-email: husisy <donot@mail.me>
 License: GNU Affero General Public License v3.0
-Project-URL: Homepage, https://github.com/husisy/numqi/
-Project-URL: Documentation, https://husisy.github.io/numqi/
-Project-URL: Issues, https://github.com/husisy/numqi/issues
+Project-URL: Homepage, https://github.com/numqi/numqi/
+Project-URL: Documentation, https://numqi.github.io/numqi/
+Project-URL: Issues, https://github.com/numqi/numqi/issues
 Keywords: quantum information
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: opt_einsum
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: sympy
 Requires-Dist: torch
 Requires-Dist: cvxpy
 Requires-Dist: matplotlib
 Provides-Extra: dev
-Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: ipywidgets; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mkdocs-git-revision-date-localized-plugin; extra == "dev"
+Requires-Dist: mkdocs-git-authors-plugin; extra == "dev"
+Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # numqi: a numpy-based quantum information package
 
-[![codecov](https://codecov.io/gh/husisy/numqi/graph/badge.svg?token=50YC4KD4M1)](https://codecov.io/gh/husisy/numqi)
+[![DOI](https://zenodo.org/badge/568701845.svg)](https://zenodo.org/doi/10.5281/zenodo.10867067)
+[![codecov](https://codecov.io/github/numqi/numqi/graph/badge.svg?token=sKLURoXVji)](https://codecov.io/github/numqi/numqi)
 
 WARNING: no backward compatibility guarantee until version `1.0.0`
 
 keyword: quantum information, numpy, pytorch, manifold optimization, trivialization
 
 ## Quickstart
 
@@ -147,15 +151,15 @@
 1. `python/numqi/`: source code
 2. `docs/`: kinds of markdown files for generating website
 3. `tests/`: unit tests
 4. `examples/`: single file scripts to demonstrate how to use `numqi`
 5. `project/`: some projects based on `numqi`, whether finished or not
 6. misc
    * `README.md`: this file
-   * `pyproject.toml`: to make a pip-instalable package
+   * `pyproject.toml`: to make a pip-installable package
    * `mkdocs.yml`: to generate website
    * `LICENSE`
    * `.gitignore`
 
 ## How to contribute
 
 see [docs/installation](./docs/installation.md) "Guide-for-contributors" section
@@ -187,7 +191,19 @@
    id5 -->|large loss| id6
    id6 -->|no| id3
    id6 -->|yes| id7
    id7 -.->|zero loss| id2
    id7 -.->|large loss| id3
    id5 -->|zero loss| id2
 ```
+
+## Recommended courses
+
+1. point-set topology
+    * [youtube-link](https://youtube.com/playlist?list=PLd8NbPjkXPliJunBhtDNMuFsnZPeHpm-0&si=Y5-wnge2rWO1HNVb) Marius Furter
+2. smooth manifold
+    * [youtube-link](https://www.youtube.com/playlist?list=PLBh2i93oe2qvRGAtgkTszX7szZDVd6jh1) The Bright Side of Mathematics
+    * [youtube-link](https://www.youtube.com/playlist?list=PLD2r7XEOtm-AGjr3ynbljbx3oWHdus9Xb) qncubed3
+3. Riemannian manifold
+4. Differential geometry
+5. algebraic topology
+    * [youtube-link](https://www.youtube.com/playlist?list=PLOROtRhtegr7DmeMyFxfKxsljAVsAn_X4) Presented by Dr. Anthony Bosman.
```

### Comparing `numqi-0.1.1b0/README.md` & `numqi-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # numqi: a numpy-based quantum information package
 
-[![codecov](https://codecov.io/gh/husisy/numqi/graph/badge.svg?token=50YC4KD4M1)](https://codecov.io/gh/husisy/numqi)
+[![DOI](https://zenodo.org/badge/568701845.svg)](https://zenodo.org/doi/10.5281/zenodo.10867067)
+[![codecov](https://codecov.io/github/numqi/numqi/graph/badge.svg?token=sKLURoXVji)](https://codecov.io/github/numqi/numqi)
 
 WARNING: no backward compatibility guarantee until version `1.0.0`
 
 keyword: quantum information, numpy, pytorch, manifold optimization, trivialization
 
 ## Quickstart
 
@@ -111,15 +112,15 @@
 1. `python/numqi/`: source code
 2. `docs/`: kinds of markdown files for generating website
 3. `tests/`: unit tests
 4. `examples/`: single file scripts to demonstrate how to use `numqi`
 5. `project/`: some projects based on `numqi`, whether finished or not
 6. misc
    * `README.md`: this file
-   * `pyproject.toml`: to make a pip-instalable package
+   * `pyproject.toml`: to make a pip-installable package
    * `mkdocs.yml`: to generate website
    * `LICENSE`
    * `.gitignore`
 
 ## How to contribute
 
 see [docs/installation](./docs/installation.md) "Guide-for-contributors" section
@@ -151,7 +152,19 @@
    id5 -->|large loss| id6
    id6 -->|no| id3
    id6 -->|yes| id7
    id7 -.->|zero loss| id2
    id7 -.->|large loss| id3
    id5 -->|zero loss| id2
 ```
+
+## Recommended courses
+
+1. point-set topology
+    * [youtube-link](https://youtube.com/playlist?list=PLd8NbPjkXPliJunBhtDNMuFsnZPeHpm-0&si=Y5-wnge2rWO1HNVb) Marius Furter
+2. smooth manifold
+    * [youtube-link](https://www.youtube.com/playlist?list=PLBh2i93oe2qvRGAtgkTszX7szZDVd6jh1) The Bright Side of Mathematics
+    * [youtube-link](https://www.youtube.com/playlist?list=PLD2r7XEOtm-AGjr3ynbljbx3oWHdus9Xb) qncubed3
+3. Riemannian manifold
+4. Differential geometry
+5. algebraic topology
+    * [youtube-link](https://www.youtube.com/playlist?list=PLOROtRhtegr7DmeMyFxfKxsljAVsAn_X4) Presented by Dr. Anthony Bosman.
```

### Comparing `numqi-0.1.1b0/docs/api/entangle.md` & `numqi-0.2.0/docs/api/entangle.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/entangle_eof.md` & `numqi-0.2.0/docs/api/entangle_eof.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/entangle_ppt.md` & `numqi-0.2.0/docs/api/entangle_ppt.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/gate.md` & `numqi-0.2.0/docs/api/gate.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/gellmann.md` & `numqi-0.2.0/docs/api/gellmann.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/group.md` & `numqi-0.2.0/docs/api/group.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/group_lie.md` & `numqi-0.2.0/docs/api/group_lie.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/group_spf2.md` & `numqi-0.2.0/docs/api/group_spf2.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/group_sym.md` & `numqi-0.2.0/docs/api/group_sym.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/group_symext.md` & `numqi-0.2.0/docs/api/group_symext.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/manifold.md` & `numqi-0.2.0/docs/api/manifold.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/random.md` & `numqi-0.2.0/docs/api/random.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/sim_state.md` & `numqi-0.2.0/docs/api/sim_state.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/state.md` & `numqi-0.2.0/docs/api/state.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,18 @@
     options:
       heading_level: 2
 
 ::: numqi.state.maximally_entangled_state
     options:
       heading_level: 2
 
+::: numqi.state.maximally_coherent_state
+    options:
+      heading_level: 2
+
 ::: numqi.state.get_2qutrit_Antoine2022
     options:
       heading_level: 2
 
 ::: numqi.state.get_bes2x4_Horodecki1997
     options:
       heading_level: 2
```

### Comparing `numqi-0.1.1b0/docs/api/unique_determine.md` & `numqi-0.2.0/docs/api/unique_determine.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/api/utils.md` & `numqi-0.2.0/docs/api/utils.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/application/circuit/basic.ipynb` & `numqi-0.2.0/docs/application/circuit/basic.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666667%*

 * *Differences: {"'cells'": '{0: {\'source\': [\'# Quantum circuit simulator\\n\', \'\\n\', \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/circuit/basic.ipynb">\\n\', '*

 * *            '\'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In '*

 * *            'Colab"/>\\n\', \'</a>\']}, 1: {\'source\': {insert: [(3, \'try:\\n\'), (4, \'    '*

 * *            "import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip install num […]*

```diff
@@ -1,26 +1,34 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Quantum circuit simulator"
+                "# Quantum circuit simulator\n",
+                "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/circuit/basic.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## First quantum circuit\n",
```

### Comparing `numqi-0.1.1b0/docs/application/circuit/customized_gate.ipynb` & `numqi-0.2.0/docs/application/circuit/customized_gate.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982266865079366%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/circuit/customized_gate.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(2, \'try:\\n\'), '*

 * *            "(3, '    import numqi\\n'), (4, 'except ImportError:\\n'), (5, '    %pip insta […]*

```diff
@@ -2,26 +2,34 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Customized quantum gate\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/circuit/customized_gate.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "The `numqi.sim` submodule supports customized quantum gate, even the not-unitary \"gate\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's define a measurement \"gate\""
```

### Comparing `numqi-0.1.1b0/docs/application/circuit/gate_decomposition.ipynb` & `numqi-0.2.0/docs/application/circuit/gate_decomposition.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984623015873015%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/circuit/gate_decomposition.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(3, \'try:\\n\'), '*

 * *            "(4, '    import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip in […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Gate Decomposition\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/circuit/gate_decomposition.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "Adapted from [qgopt/docs/gate-decomposition](https://qgopt.readthedocs.io/en/latest/quick_start.html)\n",
                 "\n",
                 "It's known that any two-qubits gate can be decomposed as follows:\n",
                 "\n",
                 "```text\n",
                 "u1 u2\n",
                 "cnot\n",
@@ -28,15 +32,19 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import torch\n",
                 "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `numqi-0.1.1b0/docs/application/communication/channel_capacity_1_inf.ipynb` & `numqi-0.2.0/docs/application/communication/channel_capacity_1_inf.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951488095238095%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/communication/channel_capacity_1_inf.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(4, \'try:\\n\'), '*

 * *            "(5, '    import numqi\\n'), (6, 'except ImportError:\\n'), (7, '  […]*

```diff
@@ -2,28 +2,36 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Channel Capacity\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/communication/channel_capacity_1_inf.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "[arxiv-link](http://arxiv.org/abs/quant-ph/0304102v1) Capacities of Quantum Channels and How to Find Them"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import torch\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `numqi-0.1.1b0/docs/application/control/simulate_dynamics.ipynb` & `numqi-0.2.0/docs/application/control/simulate_dynamics.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992559523809523%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/control/simulate_dynamics.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}}'}*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Hamiltonian dynamic simulation\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/control/simulate_dynamics.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "In this notebook, we will simulate the dynamics of the Hamiltonian system using the basic module, only `numpy/scipy/matplotlib`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `numqi-0.1.1b0/docs/application/entangle/bipartite.ipynb` & `numqi-0.2.0/docs/application/entangle/bipartite.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988756613756613%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/bipartite.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(3, \'try:\\n\'), '*

 * *            "(4, '    import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip install "*

 * * […]*

```diff
@@ -2,27 +2,35 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Bipartite entanglement\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/bipartite.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "One of the basic concepts in quantum information is entanglement. It is a property of quantum states that is not shared by classical states. One key problem is to determine whether a given quantum state is entangled or not. This is a NP problem in general, but there are some useful criteria to detect entanglement. In this tutorial, we will introduce some basic concepts about bipartite entanglement, which means we only care about the entanglement between two different parties.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Pure state\n",
```

### Comparing `numqi-0.1.1b0/docs/application/entangle/boundary_method.ipynb` & `numqi-0.2.0/docs/application/entangle/boundary_method.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966269841269841%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/boundary_method.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(3, \'try:\\n\'), '*

 * *            "(4, '    import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip inst […]*

```diff
@@ -2,27 +2,35 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Boundary of detection method\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/boundary_method.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "We are showing various Joint Algebraic Numerical Range (JANR) related to different boundaries obtained by different methods (PPT, CHA, and PureB)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Fixed operators\n",
```

### Comparing `numqi-0.1.1b0/docs/application/entangle/cha.ipynb` & `numqi-0.2.0/docs/application/entangle/cha.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986766975308642%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/cha.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(4, \'try:\\n\'), '*

 * *            "(5, '    import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip install "*

 * *       […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Convex hull approximation\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/cha.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "Convex hull [wiki-link](https://en.wikipedia.org/wiki/Convex_hull) is a general math concept: given a set of points (could be infinite, but let's assume finite for simplicity) in Euclidean plane $\\{a_1,a_2,\\cdots,a_m\\}\\subset \\mathbb{R}^n$, the convex hull is defined as\n",
                 "\n",
                 "$$ \\mathrm{conv}(\\{a\\}) = \\{ x: x=\\sum_i p_ia_i, p_i\\geq 0,\\sum_ip_i=1 \\}. $$\n",
                 "\n",
                 "For infinite set of points $A$, the definition should be the intersection of all convex sets containing $A$.\n",
                 "\n",
                 "In quantum information field, the density matrix set is the convex hull of all pure states\n",
@@ -35,15 +39,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from tqdm.notebook import tqdm\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Parametrization\n",
```

### Comparing `numqi-0.1.1b0/docs/application/entangle/gme_subspace.ipynb` & `numqi-0.2.0/docs/application/entangle/gme_subspace.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990482390873017%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/gme_subspace.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(1, \'\\n\'), (2, '*

 * *            "'try:\\n'), (3, '    import numqi\\n'), (4, 'except ImportError:\\n'), (5, '     […]*

```diff
@@ -2,25 +2,34 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Geometric measure of subspace entanglement\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/gme_subspace.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "In the previous tutorial ([doc-link](../measure)), we introduce the concept of *geometric measure of entanglement* $E_G$. In this tutorial, we will introduce how to use `numqi` to calculate the geometric measure of *subspace entanglement*. For more details, please check [arxiv-link](https://arxiv.org/abs/2311.10353)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
-                "import numqi"
+                "\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Recall that the geometric measure of $r$-bounded rank is defined as\n",
```

### Comparing `numqi-0.1.1b0/docs/application/entangle/measure.ipynb` & `numqi-0.2.0/docs/application/entangle/measure.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989506172839506%*

 * *Differences: {"'cells'": '{0: {\'source\': [\'# Entanglement measure\\n\', \'\\n\', \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/measure.ipynb">\\n\', '*

 * *            '\'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In '*

 * *            'Colab"/>\\n\', \'</a>\']}, 2: {\'source\': {insert: [(4, \'try:\\n\'), (5, \'    '*

 * *            "import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip install numqi […]*

```diff
@@ -1,14 +1,18 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Entanglement measure"
+                "# Entanglement measure\n",
+                "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/measure.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "There are various entanglement measures [wiki-link](https://en.wikipedia.org/wiki/Quantum_entanglement#As_a_measure_of_entanglement) with different meanings:\n",
@@ -34,15 +38,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from tqdm.notebook import tqdm\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Abstractly defined based on convex roof"
```

### Comparing `numqi-0.1.1b0/docs/application/entangle/multipartite.ipynb` & `numqi-0.2.0/docs/application/entangle/multipartite.ipynb`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/application/entangle/overview_method.ipynb` & `numqi-0.2.0/docs/application/entangle/overview_method.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9566697191697191%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/overview_method.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 2: {\'source\': {delete: [3, 2, 1, 0]}}, '*

 * *            "insert: [(1, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *   […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Overview\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/overview_method.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "Many entanglement detection methods have been proposed. Here, we summarize the pros and cons of each method.\n",
                 "\n",
                 "1. Positive Partial Transpose (PPT) criterion\n",
                 "    * pros: computationally efficient\n",
                 "    * cons: false positive (bound entangled states)\n",
                 "2. Convex Hull Approximation (CHA) method\n",
                 "    * pros: computationally efficient\n",
@@ -32,16 +36,27 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "import numqi\n",
-                "\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "dimA = 3\n",
                 "dimB = 3\n",
                 "\n",
                 "dm0 = numqi.random.rand_density_matrix(dimA*dimB, k=2*dimA*dimB)\n",
                 "\n",
                 "tag_ppt = numqi.entangle.is_ppt(dm0, (dimA,dimB))\n",
                 "if not tag_ppt:\n",
```

### Comparing `numqi-0.1.1b0/docs/application/entangle/pureb.ipynb` & `numqi-0.2.0/docs/application/entangle/pureb.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9754227053140097%*

 * *Differences: {"'cells'": '{0: {\'source\': [\'# Pure bosonic extension\\n\', \'\\n\', \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/pureb.ipynb">\\n\', '*

 * *            '\'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In '*

 * *            'Colab"/>\\n\', \'</a>\\n\']}, 3: {\'source\': {delete: [2, 1, 0]}}, insert: [(2, '*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', " […]*

```diff
@@ -1,14 +1,18 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Pure bosonic extension"
+                "# Pure bosonic extension\n",
+                "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/pureb.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Given a quantum state $\\rho_{AB}$, we know that bosonic extension can be used to compute the lower bounds of REE, as the following:\n",
@@ -83,16 +87,28 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
-                "import numqi\n",
                 "\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "dim = 2\n",
                 "alpha_list = np.linspace(0, 1, 100, endpoint=False) # alpha=1 is unstable for matrix logarithm\n",
                 "dm_target_list = [numqi.state.Werner(dim, x) for x in alpha_list]\n",
                 "# Analytical REE of Werner states\n",
                 "ree_analytical = np.array([numqi.state.get_Werner_ree(dim, x) for x in alpha_list])\n",
                 "# REE of Werner states obtained by PPT\n",
                 "ree_ppt = numqi.entangle.get_ppt_ree(dm_target_list, dim, dim)\n",
```

### Comparing `numqi-0.1.1b0/docs/application/entangle/sym_bos_ext.ipynb` & `numqi-0.2.0/docs/application/entangle/sym_bos_ext.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970833333333333%*

 * *Differences: {"'cells'": '{0: {\'source\': [\'# Symmetric/bosonic extension\\n\', \'\\n\', \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/sym_bos_ext.ipynb">\\n\', '*

 * *            '\'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In '*

 * *            'Colab"/>\\n\', \'</a>\\n\']}, 1: {\'source\': {insert: [(3, \'try:\\n\'), (4, \'    '*

 * *            "import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip […]*

```diff
@@ -1,26 +1,34 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Symmetric/bosonic extension"
+                "# Symmetric/bosonic extension\n",
+                "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/entangle/sym_bos_ext.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Symmetric extension is a hierarchical method to approximate the set of separable states. A bipartite state $\\rho_{AB}$ is said to be $k$-symmetric extendible if there exists a global state $\\rho_{AB^k}:=\\rho_{AB_1B_2...B_k}$ such that for any $i,j$\n",
```

### Comparing `numqi-0.1.1b0/docs/application/geometry/bloch_vector.ipynb` & `numqi-0.2.0/docs/application/geometry/bloch_vector.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988715277777778%*

 * *Differences: {"'cells'": '{0: {\'source\': [\'# Generalized Bloch vector\\n\', \'\\n\', \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/geometry/bloch_vector.ipynb">\\n\', '*

 * *            '\'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In '*

 * *            'Colab"/>\\n\', \'</a>\\n\']}, 1: {\'source\': {insert: [(4, \'try:\\n\'), (5, \'    '*

 * *            "import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip i […]*

```diff
@@ -1,27 +1,35 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Generalized Bloch vector"
+                "# Generalized Bloch vector\n",
+                "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/geometry/bloch_vector.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import itertools\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `numqi-0.1.1b0/docs/application/geometry/numerical_range_dm.ipynb` & `numqi-0.2.0/docs/application/geometry/numerical_range_dm.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982638888888888%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/geometry/numerical_range_dm.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(3, \'try:\\n\'), '*

 * *            "(4, '    import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip i […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Numerical range of density matrix\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/geometry/numerical_range_dm.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "*Comment*: the numerical range in this page is actually \"joint algebraic numerical range\" to be precise, but we will just call it numerical range for simplicity. \n",
                 "\n",
                 "For more mathematical details of numerical range, please check [doc-link](../../../foundation/matrix_space/numerical_range).\n",
                 "\n",
                 "Density matrix is postive semi-definite, Hermitian, trace one matrix.\n",
                 "\n",
                 "$$ \\{ \\rho\\in\\mathbb{C}^{d\\times d}: \\rho\\succeq 0,\\mathrm{Tr}[\\rho]=1 \\} $$\n",
@@ -22,15 +26,19 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## One qubit case\n",
```

### Comparing `numqi-0.1.1b0/docs/application/get_started/quantum_state.ipynb` & `numqi-0.2.0/docs/application/get_started/quantum_state.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990319865319865%*

 * *Differences: {"'cells'": '{0: {\'source\': [\'# Quantum state\\n\', \'\\n\', \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/get_started/quantum_state.ipynb">\\n\', '*

 * *            '\'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In '*

 * *            'Colab"/>\\n\', \'</a>\']}, 1: {\'source\': {insert: [(1, \'\\n\'), (2, \'try:\\n\'), '*

 * *            "(3, '    import numqi\\n'), (4, 'except ImportError:\\n'), (5, '    %pi […]*

```diff
@@ -1,25 +1,33 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Quantum state"
+                "# Quantum state\n",
+                "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/get_started/quantum_state.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
-                "import matplotlib.pyplot as plt\n",
-                "import numqi"
+                "\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Pure state\n",
```

### Comparing `numqi-0.1.1b0/docs/application/misc/advanced01.md` & `numqi-0.2.0/docs/application/misc/advanced01.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/application/misc/maxent.ipynb` & `numqi-0.2.0/docs/application/misc/maxent.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998561507936508%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/misc/maxent.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(4, \'try:\\n\'), '*

 * *            "(5, '    import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip install "*

 * *        […]*

```diff
@@ -2,28 +2,36 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# maximum entropy method\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/misc/maxent.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "see paper \"Maximum entropy methods for quantum state compatibility problems\" [arxiv-link](https://arxiv.org/abs/2207.11645) for more details."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import functools\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "hf_kron = lambda *x: functools.reduce(np.kron, x)\n",
                 "hf_trace0 = lambda x: x-(np.trace(x)/x.shape[0])*np.eye(x.shape[0])\n",
                 "np_rng = np.random.default_rng()\n"
             ]
         },
         {
```

### Comparing `numqi-0.1.1b0/docs/application/misc/query_grover.ipynb` & `numqi-0.2.0/docs/application/misc/query_grover.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949404761904762%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/misc/query_grover.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(3, \'try:\\n\'), '*

 * *            "(4, '    import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip install "*

 * *  […]*

```diff
@@ -2,27 +2,35 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Query Grover algorithm\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/misc/query_grover.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "see paper \"Variational learning algorithms for quantum query complexity\" [arxiv-link](https://arxiv.org/abs/2205.07449) for details"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import torch\n",
                 "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `numqi-0.1.1b0/docs/application/misc/special_state.ipynb` & `numqi-0.2.0/docs/application/misc/special_state.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991563146997929%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/misc/special_state.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(4, \'try:\\n\'), '*

 * *            "(5, '    import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip install "*

 * * […]*

```diff
@@ -2,28 +2,36 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Special states\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/misc/special_state.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "`numqi.state` implements those speical / interesting states in quantum information."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "from tqdm.auto import tqdm\n",
                 "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Werner state\n",
```

### Comparing `numqi-0.1.1b0/docs/application/qecc/qecc733.ipynb` & `numqi-0.2.0/docs/application/qecc/qecc733.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957440476190476%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/qecc/qecc733.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(4, \'try:\\n\'), '*

 * *            "(5, '    import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip install "*

 * *       […]*

```diff
@@ -2,34 +2,36 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# QECC-733\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/qecc/qecc733.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "Whether quantum error-correction code (QECC) `((7,3,3))` exists or not is an open question. This notebook is to explore the possibility of QECC-733."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
-                "os.environ['MKL_NUM_THREADS'] = '1'\n",
-                "os.environ['OMP_NUM_THREADS'] = '1'\n",
                 "import numpy as np\n",
                 "import torch\n",
                 "\n",
-                "# more threads seem to slow things down\n",
-                "if torch.get_num_threads() != 1:\n",
-                "    torch.set_num_threads(1)\n",
-                "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `numqi-0.1.1b0/docs/application/qecc/varqecc.ipynb` & `numqi-0.2.0/docs/application/qecc/varqecc.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985073260073261%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/qecc/varqecc.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(2, \'try:\\n\'), '*

 * *            "(3, '    import numqi\\n'), (4, 'except ImportError:\\n'), (5, '    %pip install "*

 * *       […]*

```diff
@@ -2,26 +2,34 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# VarQECC\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/qecc/varqecc.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "see paper \"Quantum variational learning for quantum error-correcting codes\" [doi-link](https://doi.org/10.22331%2Fq-2022-10-06-828)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `numqi-0.1.1b0/docs/application/tomography/advanced00.ipynb` & `numqi-0.2.0/docs/application/tomography/advanced00.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981770833333333%*

 * *Differences: {"'cells'": '{0: {\'source\': [\'# advanced 00\\n\', \'\\n\', \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/advanced00.ipynb">\\n\', '*

 * *            '\'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In '*

 * *            'Colab"/>\\n\', \'</a>\']}, 1: {\'source\': {insert: [(3, \'try:\\n\'), (4, \'    '*

 * *            "import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip install numqi\\n' […]*

```diff
@@ -1,26 +1,34 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# advanced 00"
+                "# advanced 00\n",
+                "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/advanced00.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import collections\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Optimal Pauli UD\n",
```

### Comparing `numqi-0.1.1b0/docs/application/tomography/advanced01.ipynb` & `numqi-0.2.0/docs/application/tomography/advanced01.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983932733932734%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/advanced01.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(4, \'try:\\n\'), '*

 * *            "(5, '    import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip install […]*

```diff
@@ -2,28 +2,36 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# advanced 01\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/advanced01.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "Stability coefficient"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "from tqdm.auto import tqdm\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n",
                 "cp_tableau = ['#006BA4', '#FF800E', '#ABABAB', '#595959', '#5F9ED1', '#C85200', '#898989', '#A2C8EC', '#FFBC79', '#CFCFCF']"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `numqi-0.1.1b0/docs/application/tomography/basic.ipynb` & `numqi-0.2.0/docs/application/tomography/basic.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992013888888889%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/basic.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(2, \'try:\\n\'), '*

 * *            "(3, '    import numqi\\n'), (4, 'except ImportError:\\n'), (5, '    %pip install "*

 * *   […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# basic\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/basic.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "references:\n",
                 "\n",
                 "1. [doi-link](https://doi.org/10.1103/PhysRevA.93.032140) Pure-state tomography with the expectation value of Pauli operators\n",
                 "2. [arxiv-link](https://arxiv.org/abs/2305.10811) A Variational Approach to Unique Determinedness in Pure-state Tomography\n",
                 "\n",
                 "Measurement scheme $A$ for quantum state tomography is a collection of Hermitian operators\n",
                 "\n",
@@ -38,15 +42,19 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 2-qubits UD with Pauli measurements\n",
```

### Comparing `numqi-0.1.1b0/docs/application/tomography/channel_tomography.ipynb` & `numqi-0.2.0/docs/application/tomography/channel_tomography.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982142857142857%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/channel_tomography.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(7, \'try:\\n\'), '*

 * *            "(8, '    import numqi\\n'), (9, 'except ImportError:\\n'), (10, '    %pi […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Quantum Channel Tomography\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/channel_tomography.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "Adapted from [QGopt/docs/channel-tomography](https://qgopt.readthedocs.io/en/latest/channel_tomography.html)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -18,15 +22,19 @@
                 "# https://qgopt.readthedocs.io/en/latest/channel_tomography.html\n",
                 "import numpy as np\n",
                 "import torch\n",
                 "import scipy.optimize\n",
                 "import matplotlib.pyplot as plt\n",
                 "import opt_einsum\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n",
                 "\n",
                 "hf_trace_distance = lambda x,y: np.abs(np.linalg.eigvalsh(x-y)).sum()\n",
                 "# https://en.wikipedia.org/wiki/Trace_distance\n"
             ]
         },
```

### Comparing `numqi-0.1.1b0/docs/application/tomography/optimal_povm.ipynb` & `numqi-0.2.0/docs/application/tomography/optimal_povm.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977513227513228%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/optimal_povm.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(3, \'try:\\n\'), '*

 * *            "(4, '    import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip insta […]*

```diff
@@ -2,27 +2,35 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Optimal POVM\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/optimal_povm.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "Adapted from [QGopt/docs/optimal-povm](https://qgopt.readthedocs.io/en/latest/optimal_povm.html)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import torch\n",
                 "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `numqi-0.1.1b0/docs/application/tomography/state_tomography.ipynb` & `numqi-0.2.0/docs/application/tomography/state_tomography.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983683473389355%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/state_tomography.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(6, \'try:\\n\'), '*

 * *            "(7, '    import numqi\\n'), (8, 'except ImportError:\\n'), (9, '    %pip i […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Quantum State Tomography\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/tomography/state_tomography.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "Adapted from [QGopt/docs/state-tomography](https://qgopt.readthedocs.io/en/latest/state_tomography.html)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -17,15 +21,19 @@
             "source": [
                 "import numpy as np\n",
                 "import collections\n",
                 "import torch\n",
                 "import scipy.optimize\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n",
                 "\n",
                 "hf_trace_distance = lambda x,y: np.abs(np.linalg.eigvalsh(x-y)).sum()\n",
                 "# https://en.wikipedia.org/wiki/Trace_distance\n"
             ]
         },
```

### Comparing `numqi-0.1.1b0/docs/data/circuit_basic_pgate.png` & `numqi-0.2.0/docs/data/circuit_basic_pgate.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/data/detect_entanglement.png` & `numqi-0.2.0/docs/data/detect_entanglement.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/data/maxent_2qubit_pauli.png` & `numqi-0.2.0/docs/data/maxent_2qubit_pauli.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/data/maxent_3qubit_2local_random.png` & `numqi-0.2.0/docs/data/maxent_3qubit_2local_random.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/data/maxent_4qubit_2local_random.png` & `numqi-0.2.0/docs/data/maxent_4qubit_2local_random.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/data/project-structure.png` & `numqi-0.2.0/docs/data/project-structure.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/foundation/group/basic.ipynb` & `numqi-0.2.0/docs/foundation/group/basic.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990826023391812%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/basic.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(2, \'try:\\n\'), '*

 * *            "(3, '    import numqi\\n'), (4, 'except ImportError:\\n'), (5, '    %pip install "*

 * *         […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Basic\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/basic.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "`numqi` implements a minimum set of group theory operations required in other numqi modules. It is based on the `sympy` library.\n",
                 "\n",
                 "Cayley table (multiplication table): a table of all possible products of group elements.\n",
                 "\n",
                 "Left regular form: a permutation representation of a group.\n",
                 "\n",
                 "One featured function is to give all inequivalent, irreducible representations of a finite group.\n",
@@ -25,15 +29,19 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Irreducible representations of $S_3$"
```

### Comparing `numqi-0.1.1b0/docs/foundation/group/clifford.ipynb` & `numqi-0.2.0/docs/foundation/group/clifford.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988771645021645%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/clifford.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(2, \'try:\\n\'), '*

 * *            "(3, '    import numqi\\n'), (4, 'except ImportError:\\n'), (5, '    %pip install "*

 * *      […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Clifford group\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/clifford.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "This note explain how Clifford circuit can be simulated efficiently on classical computers.\n",
                 "\n",
                 "1. link\n",
                 "    * [wiki/symplectic-group](https://en.wikipedia.org/wiki/Symplectic_group)\n",
                 "    * How to efficiently select an arbitrary clifford group element [doi-link](https://doi.org/10.1063%2F1.4903507)\n",
                 "    * 2004 Improved simulation of stabilizer circuits [doi-link](https://doi.org/10.1103/PhysRevA.70.052328)\n",
                 "    * Stabilizer Codes and Quantum Error Correction [arxiv-link](https://arxiv.org/abs/quant-ph/9705052)\n",
@@ -34,15 +38,19 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Clifford group\n",
```

### Comparing `numqi-0.1.1b0/docs/foundation/group/pauli.ipynb` & `numqi-0.2.0/docs/foundation/group/pauli.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982407407407408%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/pauli.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(1, \'try:\\n\'), '*

 * *            "(2, '    import numqi\\n'), (3, 'except ImportError:\\n'), (4, '    %pip install "*

 * *         […]*

```diff
@@ -2,27 +2,35 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Pauli group\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/pauli.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "The famous 1-qubit Pauli matrices are defined as\n",
                 "\n",
                 "$$ \\sigma_0=I=\\begin{bmatrix}1&0\\\\0&1\\end{bmatrix},\\quad\\sigma_1=\\sigma_x=X=\\begin{bmatrix}0&1\\\\1&0\\end{bmatrix},\\quad \\sigma_2=\\sigma_y=Y=\\begin{bmatrix}0&-i\\\\i&0\\end{bmatrix},\\quad \\sigma_3=\\sigma_z=Z=\\begin{bmatrix}1&0\\\\0&-1\\end{bmatrix} $$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `numqi-0.1.1b0/docs/foundation/group/spf2.md` & `numqi-0.2.0/docs/foundation/group/spf2.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/foundation/group/symext.ipynb` & `numqi-0.2.0/docs/foundation/group/symext.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995134032634032%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/symext.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(4, \'try:\\n\'), '*

 * *            "(5, '    import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip install "*

 * *        […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# k-Symmetric density matrix\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/symext.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "This notebooks demonstrate algorithm in the paper\n",
                 "\n",
                 "Tapping into Permutation Symmetry for Improved Detection of k-Symmetric Extensions [doi-link](https://doi.org/10.3390/e25101425)\n",
                 "\n",
                 "For systems $B_1,B_2,\\cdots,B_k$ each of dimension $d$, if the density matirx $\\rho\\in(\\mathcal{H}^d)^{\\otimes k}$ is symmetric with respect to the permutation group $S_k$, which means $\\rho$ is invariant under any permutation of the subsystems:\n",
                 "\n",
                 "$$ P_{B_iB_j} \\rho P_{B_iB_j}=\\rho $$\n",
@@ -34,15 +38,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import time\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Example: 2 qutrits\n",
```

### Comparing `numqi-0.1.1b0/docs/foundation/group/young-tableaux.ipynb` & `numqi-0.2.0/docs/foundation/group/young-tableaux.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949810606060606%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/young-tableaux.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': [\'try:\\n\', \'    import '*

 * *            "numqi\\n', 'except ImportError:\\n', '    %pip install numqi\\n', '    import "*

 * *    […]*

```diff
@@ -2,28 +2,36 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Young tableaux\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/group/young-tableaux.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "[wiki-link](https://en.wikipedia.org/wiki/Young_tableau)\n",
                 "\n",
                 "numqi implements functions to list all Young diagram and Young tableaux.\n",
                 "\n",
                 "Young diagram / tableaux is used in symmetric extension to detect quantum entanglement."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `numqi-0.1.1b0/docs/foundation/manifold/basic_sphere.ipynb` & `numqi-0.2.0/docs/foundation/manifold/basic_sphere.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945833333333334%*

 * *Differences: {"'cells'": '{0: {\'source\': [\'# n-Sphere manifold\\n\', \'\\n\', \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/manifold/basic_sphere.ipynb">\\n\', '*

 * *            '\'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In '*

 * *            'Colab"/>\\n\', \'</a>\']}, 1: {\'source\': {insert: [(4, \'try:\\n\'), (5, \'    '*

 * *            "import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip install numq […]*

```diff
@@ -1,27 +1,35 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# n-Sphere manifold"
+                "# n-Sphere manifold\n",
+                "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/manifold/basic_sphere.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "import torch\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `numqi-0.1.1b0/docs/foundation/manifold/basic_stiefel.ipynb` & `numqi-0.2.0/docs/foundation/manifold/basic_stiefel.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996994301994302%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/manifold/basic_stiefel.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(5, \'try:\\n\'), '*

 * *            "(6, '    import numqi\\n'), (7, 'except ImportError:\\n'), (8, '    %pip install […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Stiefel manifold\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/manifold/basic_stiefel.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "This notebook is to reproduce the results of the paper: Riemannian geometry and automatic differentiation for optimization problems of quantum physics and quantum technologies [doi-link](https://doi.org/10.1088/1367-2630/ac0b02)\n",
                 "\n",
                 "also see paper \"A Global Cayley Parametrization of Stiefel Manifold for Direct Utilization of Optimization Mechanisms Over Vector Spaces\" [doi-link](https://doi.org/10.1109/ICASSP39728.2021.9414157)"
             ]
         },
         {
             "cell_type": "code",
@@ -18,15 +22,19 @@
             "outputs": [],
             "source": [
                 "import time\n",
                 "import torch\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng(234) #fix seed for documentation\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `numqi-0.1.1b0/docs/foundation/manifold/trivialization.ipynb` & `numqi-0.2.0/docs/foundation/manifold/trivialization.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999516369047619%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Trivialization\\n'), (1, '\\n'), (2, '<a "*

 * *            'target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/manifold/trivialization.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')], delete: [0]}}, 2: {\'source\': {insert: [(3, '*

 * *            "'try:\\n'), (4, '    import numqi\\n'), (5 […]*

```diff
@@ -1,14 +1,18 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Trivialization on manifold\n",
+                "# Trivialization\n",
+                "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/manifold/trivialization.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
                 "\n",
                 "[arxiv-link](https://arxiv.org/abs/1909.09501) Trivializations for Gradient-Based Optimization on Manifolds\n",
                 "\n",
                 "[arxiv-link](https://arxiv.org/abs/2203.04794) Geometric Optimisation on Manifolds with Applications to Deep Learning\n",
                 "\n",
                 "**Trivialization**: given a manifold $\\mathcal{M}$, trivialization is defined as a surjective map from the Euclidean space onto the manifold:\n",
                 "\n",
@@ -46,15 +50,19 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import torch\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Positive real number\n",
```

### Comparing `numqi-0.1.1b0/docs/foundation/matrix_space/numerical_range.ipynb` & `numqi-0.2.0/docs/foundation/matrix_space/numerical_range.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991957199546485%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/matrix_space/numerical_range.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(2, \'\\n\'), (3, '*

 * *            "'try:\\n'), (4, '    import numqi\\n'), (5, 'except ImportError:\\n'), (6, […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Numerical range\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/matrix_space/numerical_range.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "[wiki/Numerical-range](https://en.wikipedia.org/wiki/Numerical_range)\n",
                 "\n",
                 "Given a complex matrix $A\\in\\mathbb{C}^{d\\times d}$, its numerical range $W(A)\\subset \\mathbb{C}$ is defined as the set\n",
                 "\n",
                 "$$ W(A)=\\left\\{ x^{\\dagger}Ax:x\\in\\mathbb{C}^{d},\\lVert x\\rVert_{2}=1\\right\\} $$\n",
                 "\n",
                 "and Hausdorff\u2013Toeplitz theorem proved that the numerical range is convex and compact.\n",
@@ -27,15 +31,20 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
-                "import numqi\n",
+                "\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n",
                 "hf_randc = lambda *x: np_rng.normal(size=x) + 1j*np_rng.normal(size=x)\n"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `numqi-0.1.1b0/docs/foundation/matrix_space/numerical_range1.ipynb` & `numqi-0.2.0/docs/foundation/matrix_space/numerical_range1.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962554112554113%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/matrix_space/numerical_range1.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(3, \'try:\\n\'), '*

 * *            "(4, '    import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip  […]*

```diff
@@ -2,27 +2,35 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# How to solve numerical range\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/matrix_space/numerical_range1.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "In previous tutorial, we have defined the numerical range of a matrix $A$ as the set of all possible values of $x^*Ax$ for all unit vectors $x$. In this tutorial, we will focus on different methods to solve the numerical range of a matrix."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `numqi-0.1.1b0/docs/foundation/matrix_space/space_schmidt_rank.ipynb` & `numqi-0.2.0/docs/foundation/matrix_space/space_schmidt_rank.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984464031339031%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/matrix_space/space_schmidt_rank.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(1, \'\\n\'), (2, '*

 * *            "'try:\\n'), (3, '    import numqi\\n'), (4, 'except ImportError:\\n'),  […]*

```diff
@@ -2,27 +2,36 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Schmidt Rank in matrix subspace\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/matrix_space/space_schmidt_rank.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "see paper \"Complete hierarchy of linear systems for certifying quantum entanglement of subspaces\" [doi-link](https://doi.org/10.1103/PhysRevA.106.062443) for more details\n",
                 "\n",
                 "An important and difficult problem in quantum information field is to ask whether there is a product state in matrix subspace. For this problem, Nathaniel et al. proposed a method to solve it by constructing a set of vectors in higher dimensional space and then inspecting the linear dependency of these vectors. `numqi.matrix_space` implements this methods and does some optimization to make it more efficient (see last section for a benchmarking)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
-                "import numqi\n"
+                "\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Matrix subspace\n",
```

### Comparing `numqi-0.1.1b0/docs/foundation/misc/dicke.ipynb` & `numqi-0.2.0/docs/foundation/misc/dicke.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986960955710955%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/misc/dicke.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(2, \'try:\\n\'), '*

 * *            "(3, '    import numqi\\n'), (4, 'except ImportError:\\n'), (5, '    %pip install "*

 * *          […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Dicke basis\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/misc/dicke.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "See paper \"Deterministic Preparation of Dicke States\" [arxiv-link](http://arxiv.org/abs/1904.07358) for details.\n",
                 "\n",
                 "Dicke basis is a basis for symmetric subspace. A more well-known name is the basis for Bosons. They are useful in quantum entanglement detection and quantum many-body physics.\n",
                 "\n",
                 "TODO, the strucutre of this tutorial"
             ]
         },
@@ -17,15 +21,19 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "import numqi\n"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Qubit case\n",
```

### Comparing `numqi-0.1.1b0/docs/foundation/misc/gellmann.ipynb` & `numqi-0.2.0/docs/foundation/misc/gellmann.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985246598639456%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/misc/gellmann.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(1, \'\\n\'), (2, '*

 * *            "'try:\\n'), (3, '    import numqi\\n'), (4, 'except ImportError:\\n'), (5, '    %pip "*

 * *   […]*

```diff
@@ -2,25 +2,34 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Gell-Mann matrix\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/misc/gellmann.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "Gell-Mann matrices are a set of Hermitian matrices."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
-                "import numqi\n",
+                "\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `numqi-0.1.1b0/docs/foundation/misc/random.ipynb` & `numqi-0.2.0/docs/foundation/misc/random.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993313234384663%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/misc/random.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(3, \'try:\\n\'), '*

 * *            "(4, '    import numqi\\n'), (5, 'except ImportError:\\n'), (6, '    %pip install "*

 * *         […]*

```diff
@@ -2,27 +2,35 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Random\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/misc/random.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "The submodule `numqi.random` is designed to generate various random distribution, like random Hermitian matrix, random state, random unitary matrix etc."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `numqi-0.1.1b0/docs/foundation/optimize/adam-vs-lbfgs.ipynb` & `numqi-0.2.0/docs/foundation/optimize/adam-vs-lbfgs.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989583333333334%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(2, 'given a series of real matrix $B^{\\\\alpha}\\\\in "*

 * *            '\\\\mathbb{R}^{16\\\\times 16},\\\\alpha=1,2,\\\\cdots,64$ (see '*

 * *            "[github-link](https://github.com/numqi/biquadratic-optimization) for detailed)\\n')], "*

 * *            'delete: [2]}}}'}*

```diff
@@ -50,15 +50,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Example: Super-activation\n",
                 "\n",
-                "given a series of real matrix $B^{\\alpha}\\in \\mathbb{R}^{16\\times 16},\\alpha=1,2,\\cdots,64$ (see [github-link](https://github.com/husisy/biquadratic-optimization) for detailed)\n",
+                "given a series of real matrix $B^{\\alpha}\\in \\mathbb{R}^{16\\times 16},\\alpha=1,2,\\cdots,64$ (see [github-link](https://github.com/numqi/biquadratic-optimization) for detailed)\n",
                 "\n",
                 "$$\\min_{a,b} \\sum_{\\alpha}\\left|\\left\\langle a\\right|B^{\\alpha}\\left|b\\right\\rangle \\right|^{2}$$\n",
                 "\n",
                 "comment: the solution is almost unique, non convex, the success probability for random initialization is almost 1 over thousand."
             ]
         },
         {
```

### Comparing `numqi-0.1.1b0/docs/foundation/optimize/basic.ipynb` & `numqi-0.2.0/docs/foundation/optimize/basic.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999092261904762%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/optimize/basic.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(6, \'try:\\n\'), '*

 * *            "(7, '    import numqi\\n'), (8, 'except ImportError:\\n'), (9, '    %pip install "*

 * *      […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# basic\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/optimize/basic.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "`numqi.optimize` module provides a wrapper for `L-BFGS-B` optimization algorithm from `scipy.optimize.minimize` function and `Adam` optimizer from `torch.optim` module. It is designed to directly apply the optimization algorithm on the `torch.nn.Module` with few lines of code."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -17,15 +21,19 @@
             "source": [
                 "import time\n",
                 "import numpy as np\n",
                 "import scipy.optimize\n",
                 "import matplotlib.pyplot as plt\n",
                 "import torch\n",
                 "\n",
-                "import numqi"
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## mathematical statement\n",
```

### Comparing `numqi-0.1.1b0/docs/foundation/optimize/wiki-test-function.ipynb` & `numqi-0.2.0/docs/foundation/optimize/wiki-test-function.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996745124793905%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(1, \'\\n\'), (2, \'<a target="_blank" '*

 * *            'href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/optimize/wiki-test-function.ipynb">\\n\'), '*

 * *            '(3, \'  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open '*

 * *            'In Colab"/>\\n\'), (4, \'</a>\\n\')]}}, 1: {\'source\': {insert: [(4, \'try:\\n\'), '*

 * *            "(5, '    import numqi\\n'), (6, 'except ImportError:\\n'), (7, '    %pip in […]*

```diff
@@ -2,14 +2,18 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# test function list\n",
                 "\n",
+                "<a target=\"_blank\" href=\"https://colab.research.google.com/github/numqi/numqi/blob/main/docs/foundation/optimize/wiki-test-function.ipynb\">\n",
+                "  <img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/>\n",
+                "</a>\n",
+                "\n",
                 "In this part, we will show gradient descent optimization on various 2-dimensioanl test function from this wiki page [wiki/test-function-for-optimization](https://en.wikipedia.org/wiki/Test_functions_for_optimization).\n",
                 "\n",
                 "We will plot the function landscape around the optimal point and also the optimization path.\n",
                 "\n",
                 "We choose the initial point for optimization uniformly from the range $[-1, 1]$, so it could be biased to the local optimal point around the origin."
             ]
         },
@@ -19,15 +23,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "import torch\n",
                 "\n",
-                "import numqi\n",
+                "try:\n",
+                "    import numqi\n",
+                "except ImportError:\n",
+                "    %pip install numqi\n",
+                "    import numqi\n",
                 "\n",
                 "np_rng = np.random.default_rng()\n",
                 "hf_uniform_para = lambda *x: torch.nn.Parameter(torch.tensor(np_rng.uniform(-1, 1, size=x), dtype=torch.float64))\n"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `numqi-0.1.1b0/docs/index.md` & `numqi-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/docs/installation.md` & `numqi-0.2.0/docs/installation.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Installation
 
+Try without installing anything: `application/get-started` in colab
+
+<a target="_blank" href="https://colab.research.google.com/github/numqi/numqi/blob/main/docs/application/get_started/quantum_state.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
+## pip installation
+
 The following command should be okay for `win/mac/linux`
 
 ```bash
 pip install numqi
 ```
 
 test whether succuessfully installed (run it in `python/ipython` REPL)
@@ -21,104 +29,101 @@
 # apply mosek academic license https://www.mosek.com/products/academic-licenses/
 conda install -n <xxx> -c MOSEK MOSEK
 ```
 
 For macOS user, you might need to install `openblas` first and then install `scs` as below.
 
 ```bash
-# macOS m1/m2 user (Apple silicon M series)
-# also see https://www.cvxgrp.org/scs/install/python.html
+# macOS m1/m2 user (Apple silicon M series), see https://www.cvxgrp.org/scs/install/python.html
 brew install openblas
 OPENBLAS="$(brew --prefix openblas)" pip install scs
 ```
 
 ## Conda environment
 
 conda can create isolated Python environment to install package. If you have any problems install `numqi` using the above `pip install` command, please try following conda commands [miniconda-documentation](https://docs.conda.io/en/latest/miniconda.html)
 
 ```bash
-# for linux users without naivdia-GPU (this should also works for windows user)
-# nocuda is the environment name (you can change it what you like)
+# for win/linux users without naivdia-GPU, nocuda is the environment name (you can change it what you like)
 conda create -y -n nocuda
 conda install -y -n nocuda -c conda-forge pytorch ipython pytest matplotlib scipy tqdm cvxpy
 conda activate nocuda
 pip install numqi
 
-# for linux users with nvidia-GPU (this should also works for windows user)
-# cuda118 is the environment name (you can change it what you like)
+# for win/linux users with nvidia-GPU, cuda118 is the environment name
 conda create -y -n cuda118
-conda install -y -n cuda118 -c conda-forge pytorch ipython pytest matplotlib scipy tqdm cvxpy
+conda install -y -n cuda118 -c conda-forge ipython pytest matplotlib scipy tqdm cvxpy
+conda install -y -n cuda118 -c pytorch pytorch
 conda activate cuda118
 pip install numqi
 
-# for mac user
-# metal is the environment name (you can change it what you like)
+# for macOS user, metal is the environment name
 conda create -y -n metal
 conda install -y -n metal -c conda-forge ipython pytest matplotlib scipy requests tqdm cvxpy
+conda install -y -n metal -c pytorch pytorch torchvision torchaudio
+# conda-forge/macos/pytorch is broken https://github.com/conda-forge/pytorch-cpu-feedstock/issues/180
 conda activate metal
-pip install torch #conda-forge/macos/pytorch is broken https://github.com/conda-forge/pytorch-cpu-feedstock/issues/180
-brew install openblas
-OPENBLAS="$(brew --prefix openblas)" pip install scs
+## scs-macos issue, see https://www.cvxgrp.org/scs/install/python.html
+# brew install openblas
+# OPENBLAS="$(brew --prefix openblas)" pip install scs
 pip install numqi
 ```
 
 (PS) notice some weird problems if installed `conda-forge/numpy` on ubuntu, then use `pip install --force-reinstall numpy` instead.
 
 ## Guide for contributors
 
-Personally i use `conda/miniconda/mamba/micromamba` to create a virtual environment.
+
+Quick start for contributors: open this project in GitHub Codespaces and then `pip install -e ".[dev]"`
+
+[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/numqi/numqi)
+
+### local development environment
+
+It is recommended to install `numqi` in a virtual environment.  You may use `conda/miniconda/mamba/micromamba` to create a virtual environment.
 
 ```bash
 conda create -n env-numqi python
 conda activate env-numqi
 ```
 
-install `numqi`
+Then you should install `numqi` as developer
 
 ```bash
-git clone git@github.com:husisy/numqi.git
+git clone git@github.com:numqi/numqi.git
 cd numqi
 pip install -e ".[dev]"
 ```
 
-run the unittest
+### Unittest
+
+You can now run the unittest
 
 ```bash
 # "OMP_NUM_THREADS=1" usually runs faster (some unnecessay threads are disabled)
 OMP_NUM_THREADS=1 pytest --durations=10 --cov=python/numqi
 
 # if you have a multi-core CPU, you can run the unittest in parallel (take about 120 seconds on my laptop)
 OMP_NUM_THREADS=1 pytest -n 8 --durations=10 --cov=python/numqi
 ```
 
-build and Serve the documentation locally, then brower the website `127.0.0.1:8000`
+### Documentation
+
+You can now build the documentation locally.
 
 ```bash
 mkdocs serve
 ```
+then browse the website `127.0.0.1:8000`
 
 1. **WARNING**: second indentaion must be 4 spaces, not 3 spaces (necessary for `mkdoc`)
 2. api style: [griffe/usage](https://mkdocstrings.github.io/griffe/docstrings/)
 3. toolchain
     * [github/mkdocstrings](https://github.com/mkdocstrings/mkdocstrings)
     * [github/mkdocstrings/python](https://github.com/mkdocstrings/python)
     * [github/mkdocstrings/griffe](https://github.com/mkdocstrings/griffe)
     * [github/best-of-mkdocs](https://github.com/mkdocs/best-of-mkdocs)
 4. special module name, not for users
    * `._xxx.py`: internal functions, not for users
    * `._internal.py`: private to submodules. E.g., `numqi.A._internal` should only be imported in `numqi.A.xxx`
    * `._public.py`: library public functions. E.g., `numqi.A._public` can be imported by `numqi.B`
 5. strip the jupyter notebook output before commit
-
-Recommended courses
-
-TODO add quantum stuff
-
-1. point-set topology
-    * [youtube-link](https://youtube.com/playlist?list=PLd8NbPjkXPliJunBhtDNMuFsnZPeHpm-0&si=Y5-wnge2rWO1HNVb) Marius Furter
-2. smooth manifold
-    * [youtube-link](https://www.youtube.com/playlist?list=PLBh2i93oe2qvRGAtgkTszX7szZDVd6jh1) The Bright Side of Mathematics
-    * [youtube-link](https://www.youtube.com/playlist?list=PLD2r7XEOtm-AGjr3ynbljbx3oWHdus9Xb) qncubed3
-3. Riemannian manifold
-4. Differential geometry
-5. algebraic topology
-    * [youtube-link](https://www.youtube.com/playlist?list=PLOROtRhtegr7DmeMyFxfKxsljAVsAn_X4) Presented by Dr. Anthony Bosman.
```

### Comparing `numqi-0.1.1b0/docs/misc.md` & `numqi-0.2.0/docs/misc.md`

 * *Files 22% similar despite different names*

```diff
@@ -18,22 +18,21 @@
 
 `233` is a prime number! Internet slang that essentially means “LOL.”
 
 ## Publications
 
 This package is to support following papers
 
-1. detecting entanglement by pure bosonic extension [arxiv-link](https://arxiv.org/abs/2209.10934) `numqi.entangle`
-2. Quantum variational learning for quantum error-correcting codes [doi-link](https://doi.org/10.22331/q-2022-10-06-828) `numqi.qec`
-3. Tapping into Permutation Symmetry for Improved Detection of k-Symmetric Extensions [doi-link](https://doi.org/10.3390/e25101425) `numqi.entangle` `numqi.group.symext`
-4. Variational learning algorithms for quantum query complexity [arxiv-link](https://arxiv.org/abs/2205.07449) `numqi.query`
-5. Variational approach to unique determinedness in pure-state tomography [arxiv-link](https://arxiv.org/abs/2305.10811) [doi-link](https://doi.org/10.1103/PhysRevA.109.022425) `numqi.unique_determine`
-6. Maximum entropy methods for quantum state compatibility problems [arxiv-link](https://arxiv.org/abs/2207.11645) `numqi.maximum_entropy`
-7. Simulating Noisy Quantum Circuits with Matrix Product Density Operators [arxiv-link](https://arxiv.org/abs/2004.02388) `numqi.sim`
-8. Quantifying Subspace Entanglement with Geometric Measures [arxiv-link](https://arxiv.org/abs/2311.10353) `numqi.matrix_space`
+1. [doi-link](https://doi.org/10.1103/PhysRevResearch.6.013249) [arxiv-link](https://arxiv.org/abs/2209.10934) `numqi.entangle` Detecting entanglement by pure bosonic extension
+2. [doi-link](https://doi.org/10.22331/q-2022-10-06-828) [arxiv-link](https://arxiv.org/abs/2204.03560) `numqi.qec` Quantum variational learning for quantum error-correcting codes
+3. [doi-link](https://doi.org/10.3390/e25101425) [arxiv-link](https://arxiv.org/abs/2309.04144) `numqi.entangle` `numqi.group.symext` Tapping into Permutation Symmetry for Improved Detection of k-Symmetric Extensions
+4. [doi-link](https://doi.org/10.1088/1367-2630/ad309c) [arxiv-link](https://arxiv.org/abs/2205.07449) `numqi.query` Variational learning algorithms for quantum query complexity
+5. [doi-link](https://doi.org/10.1103/PhysRevA.109.022425) [arxiv-link](https://arxiv.org/abs/2305.10811) `numqi.unique_determine` Variational approach to unique determinedness in pure-state tomography
+6. [arxiv-link](https://arxiv.org/abs/2207.11645) `numqi.maximum_entropy` Maximum entropy methods for quantum state compatibility problems
+7. [arxiv-link](https://arxiv.org/abs/2311.10353) `numqi.matrix_space` Quantifying Subspace Entanglement with Geometric Measures
 
 ## Acknowledgement
 
 Thanks to (alphabetical order)
 
 1. Bei ZENG
 2. Chenfeng CAO [github](https://github.com/caochenfeng)
@@ -58,41 +57,12 @@
 3. QEC: quantum error correction
 4. QECC: quantum error correction code
 
 model name
 
 1. `pureb`: pure bosonic extension
 2. `symext`: symmetric extension
-3. `varqecc`: variational quantum
-
-## TODO
-
-1. [ ] check `functools.lru_cache`, all type of input should be simple-typed, e.g. `int(1)` not `np.array([1])[0]`
-2. [ ] make it a conda-forge package [link](https://conda-forge.org/docs/maintainer/adding_pkgs.html#the-staging-process)
-3. [ ] github CI
-4. [x] coverage
-5. [ ] documentation
-    * [ ] numerical range
-    * [ ] jupyter notebook: numqi.optimize.minimize_adam
-    * [ ] [arxiv-link](https://arxiv.org/abs/quant-ph/0301152) The Bloch Vector for N-Level Systems fig2
-    * [ ] manifold, add trivialization map for each model
-    * [ ] check is there any notes in overleaf which should be added to the documentation
-6. [ ] learn from QETLAB
-7. [ ] make a conda-forge package [link](https://conda-forge.org/docs/maintainer/adding_pkgs.html#the-staging-process)
-8. [x] go through cvxquad [github-link](https://github.com/hfawzi/cvxquad) and replace `numqi.entangle.qetlab` module [arxiv-link](https://arxiv.org/abs/1705.00812)
-9. [ ] roadmap for packaging development
-10. [x] quantum optimal control
-11. [ ] learn from qutip
-12. [ ] add a zenodo record
-13. [ ] move `example/` to `docs`
-14. [ ] cupy/torch LBFGS
-15. [x] GPU support in `numqi.manifold`
-16. [ ] multi-processing support [link0](https://github.com/pytorch/pytorch/wiki/Autograd-and-Fork) [link1](https://github.com/numpy/numpy/issues/11826) [link2](https://github.com/joblib/threadpoolctl)
-17. [ ] gradient back-propagation for density matrix circuit `numqi.circuit.dm`
-18. [ ] Clifford circuit simulator is not in good states
-19. [ ] host gitee pages
-20. [ ] REE / EoF for pure states [arxiv-link0](https://arxiv.org/abs/2009.04982) [arxiv-link1](https://arxiv.org/abs/quant-ph/0409009)
-21. [ ] github codespace `devcontainer.json`
+3. `varqecc`: variational quantum error correction code
 
 ## license
 
-GNU Affero General Public License v3.0, see [github-repo/LICENSE](https://github.com/husisy/numqi/blob/main/LICENSE)
+GNU Affero General Public License v3.0, see [github-repo/LICENSE](https://github.com/numqi/numqi/blob/main/LICENSE)
```

### Comparing `numqi-0.1.1b0/example/data/20220905_realign_upb_bes.png` & `numqi-0.2.0/example/data/20220905_realign_upb_bes.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/data/demo_get_ABk_symmetric_extension_ree_werner.png` & `numqi-0.2.0/example/data/demo_get_ABk_symmetric_extension_ree_werner.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/data/demo_pureb_quantum_werner.png` & `numqi-0.2.0/example/data/demo_pureb_quantum_werner.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/data/demo_tiles_upb_pureb_ree.png` & `numqi-0.2.0/example/data/demo_tiles_upb_pureb_ree.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/data/superactivation-loss.png` & `numqi-0.2.0/example/data/superactivation-loss.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/data/superactivation_landscope_random.png` & `numqi-0.2.0/example/data/superactivation_landscope_random.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/data/superactivation_landscope_xystar.png` & `numqi-0.2.0/example/data/superactivation_landscope_xystar.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/demo_misc.py` & `numqi-0.2.0/example/demo_misc.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/demo_sqrtm_time.py` & `numqi-0.2.0/example/demo_sqrtm_time.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/demo_superactivation.py` & `numqi-0.2.0/example/demo_superactivation.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/demo_unique_determine.py` & `numqi-0.2.0/example/demo_unique_determine.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/ws_entangle/demo_symext.py` & `numqi-0.2.0/example/ws_entangle/demo_symext.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/ws_entangle/draft_boundary.py` & `numqi-0.2.0/example/ws_entangle/draft_boundary.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/ws_entangle/draft_find_BES.py` & `numqi-0.2.0/example/ws_entangle/draft_find_BES.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/ws_entangle/draft_ppt.py` & `numqi-0.2.0/example/ws_entangle/draft_ppt.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/ws_entangle/draft_pureb.py` & `numqi-0.2.0/example/ws_entangle/draft_pureb.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/example/ws_entangle/draft_ree.py` & `numqi-0.2.0/example/ws_entangle/draft_ree.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/mkdocs.yml` & `numqi-0.2.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,39 @@
-site_name: numqi
-site_url: https://husisy.github.io/numqi/
+site_name: NumQI
+site_url: https://numqi.github.io/numqi/
+repo_url: https://github.com/numqi/numqi
+edit_uri: edit/main/docs/
 theme:
   name: material
   features:
     - toc.integrate
     - navigation.tabs
     - search.highlight
     - search.share
     - search.suggest
     - content.code.copy
+    - content.action.edit
   palette:
     - scheme: default
       toggle:
         icon: material/toggle-switch-off-outline
         name: Switch to dark mode
     - scheme: slate
       toggle:
         icon: material/toggle-switch
         name: Switch to light mode
 plugins:
   search:
+  git-authors:
+    show_email_address: false
+  git-revision-date-localized:
+    enable_creation_date: true
   mkdocs-jupyter:
     include: ["foundation/**/*.ipynb", "application/**/*.ipynb"] # Default: ["*.py", "*.ipynb"]
-    execute: true
+    execute: false
   mkdocstrings:
     default_handler: python
     handlers:
       python:
         paths: [python]
         options:
           docstring_style: google
@@ -49,14 +56,15 @@
   - https://polyfill.io/v3/polyfill.min.js?features=es6
   - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
 # TODO add colab link
 nav:
   - Home: index.md
   - Installation: installation.md
   - Foundation:
+    - foundation/get_started/get_started.ipynb
     - Group:
       - foundation/group/basic.ipynb
       - foundation/group/young-tableaux.ipynb
       - foundation/group/symext.ipynb
       - Symplectic-Group-F2: foundation/group/spf2.md
       - foundation/group/pauli.ipynb
       - foundation/group/clifford.ipynb
```

### Comparing `numqi-0.1.1b0/project/entangled_subspace/README.md` & `numqi-0.2.0/project/entangled_subspace/README.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/Maciej2019_bipartite_gm.pdf` & `numqi-0.2.0/project/entangled_subspace/data/Maciej2019_bipartite_gm.pdf`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/analytic_gm.pdf` & `numqi-0.2.0/project/entangled_subspace/data/analytic_gm.pdf`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/analytic_gm.pkl` & `numqi-0.2.0/project/entangled_subspace/data/analytic_gm.pkl`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/analytic_gm.png` & `numqi-0.2.0/project/entangled_subspace/data/analytic_gm.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/qubit_dicke_state_border_rank.pdf` & `numqi-0.2.0/project/entangled_subspace/data/qubit_dicke_state_border_rank.pdf`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/qubit_dicke_state_border_rank.pkl` & `numqi-0.2.0/project/entangled_subspace/data/qubit_dicke_state_border_rank.pkl`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/qubit_dicke_state_border_rank.png` & `numqi-0.2.0/project/entangled_subspace/data/qubit_dicke_state_border_rank.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/robustness.pdf` & `numqi-0.2.0/project/entangled_subspace/data/robustness.pdf`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/robustness.pkl` & `numqi-0.2.0/project/entangled_subspace/data/robustness.pkl`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/data/robustness.png` & `numqi-0.2.0/project/entangled_subspace/data/robustness.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/demo_basic.py` & `numqi-0.2.0/project/entangled_subspace/demo_basic.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/demo_schmidt_rank.py` & `numqi-0.2.0/project/entangled_subspace/demo_schmidt_rank.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/draft_ces.py` & `numqi-0.2.0/project/entangled_subspace/draft_ces.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/draft_graph_state.py` & `numqi-0.2.0/project/entangled_subspace/draft_graph_state.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/draft_paper_example.py` & `numqi-0.2.0/project/entangled_subspace/draft_paper_example.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangled_subspace/draft_pymanopt.py` & `numqi-0.2.0/project/entangled_subspace/draft_pymanopt.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/entangler/draft00.py` & `numqi-0.2.0/project/entangler/draft00.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,17 +53,32 @@
         z0.append((matU,theta_optim.fun))
     z1 = max(z0, key=lambda x: x[1])
     print(z1[1])
 
 
 def hf_dummy_232(theta_u, kwargs_model, kwargs_optim):
     dimA,dimB = kwargs_model['dim']
+    if 'last_psiAB' in kwargs_model:
+        last_psiAB = kwargs_model['last_psiAB']
+        del kwargs_model['last_psiAB']
+    else:
+        last_psiAB = None
     matU = numqi.manifold.to_special_orthogonal_exp(theta_u, dimA*dimB)
     model = DummyModel(matU, **kwargs_model)
-    fval = -numqi.optimize.minimize(model, **kwargs_optim).fun
+    theta_optim = numqi.optimize.minimize(model, **kwargs_optim)
+    fval = -theta_optim.fun
+    if last_psiAB is not None:
+        tmp0 = dict(**kwargs_optim)
+        tmp0['theta0'] = last_psiAB
+        tmp0['num_repeat'] = 1
+        tmp1 = numqi.optimize.minimize(model, **tmp0)
+        if tmp1.fun < theta_optim.fun:
+            theta_optim = tmp1
+    fval = -theta_optim.fun
+    kwargs_model['last_psiAB'] = theta_optim.x
     return fval
 
 def hf_dummy_233(theta_u, tag_grad, kwargs_model, kwargs_optim, zero_eps=1e-9, num_worker=18):
     ret = hf_dummy_232(theta_u, kwargs_model, kwargs_optim)
     if tag_grad:
         arg_list = []
         for ind0 in range(len(theta_u)):
@@ -106,21 +121,42 @@
         hf0 = lambda x, tag_grad=False: hf_dummy_233(x, tag_grad, kwargs_model, kwargs_optim, zero_eps=1e-7, num_worker=16)
         hf_callback = numqi.optimize.MinimizeCallback(print_freq=50).to_callable(hf0) #extra_key='path'
         theta_optim = scipy.optimize.minimize(hf0, theta_u, method='Nelder-Mead', callback=hf_callback)
         total_time = time.time() - t0
         average_time = total_time / (ind_round+1)
         eta_time = total_time*num_round / (ind_round+1) - total_time
         to_pickle(theta_optim_u=theta_optim.x)
-        print(f'[{ind_round+1}/{num_round}][{average_time:.0f}s / {eta_time:.0f}s / {total_time:.0f}s] loss={theta_optim.fun:.6f}')
+        print(f'[{ind_round+1}/{num_round}][{average_time:.0f}s / {eta_time:.0f}s / {total_time:.0f}s] loss={-theta_optim.fun:.6f}')
         loss_list.append(theta_optim.fun)
     for x in loss_list:
         print(x)
     to_pickle(loss_list=loss_list)
 
     # theta_optim_u = from_pickle('theta_optim_u')
     # matU = numqi.manifold.to_special_orthogonal_exp(theta_optim_u, dimA*dimB)
     # model = DummyModel(matU, **kwargs_model)
     # fval = -numqi.optimize.minimize(model, **kwargs_optim).fun
     # model.loss = 'eigen'
     # hf_dummy_233(theta_optim_u, True, dict(dim=(dimA,dimB), loss='eigen'), kwargs_optim, zero_eps=1e-9, num_worker=16)
 
 # https://www.sciencedirect.com/science/article/pii/S037596011401216X
+
+# import os
+# import numqi
+# import pickle
+# from zzz233 import to_pickle,from_pickle
+# from utils import matU_to_reduce_su, get_unitary_fidelity
+
+# def hf0(z0, dimA, dimB):
+#     matU = numqi.manifold.to_special_orthogonal_exp(z0, dimA*dimB)
+#     z1 = matU_to_reduce_su(matU, return_coeff=True)
+#     matU1 = numqi.manifold.to_special_orthogonal_exp(z1, dimA*dimB)
+#     fidelity = get_unitary_fidelity(matU, matU1)
+#     print(f'norm0={np.linalg.norm(z0)}, norm1={np.linalg.norm(z1)}, fidelity={fidelity}')
+#     return z1
+
+# with open(os.path.expanduser('~/project/numqi/project/entangler/tbd00.pkl'), 'rb') as fid:
+#     z0 = pickle.load(fid)['theta_optim_u']
+# dimA = 3
+# dimB = 4
+# z1 = hf0(z0, dimA=3, dimB=4)
+# to_pickle(theta_optim_u=z1)
```

### Comparing `numqi-0.1.1b0/project/gme_dm/draft00.py` & `numqi-0.2.0/project/gme_dm/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/gme_dm/draft01.py` & `numqi-0.2.0/project/gme_dm/draft01.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws00/draft00.py` & `numqi-0.2.0/project/ws00/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws00/draft02.py` & `numqi-0.2.0/project/ws00/draft02.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws00/draft04.py` & `numqi-0.2.0/project/ws00/draft04.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws00/draft_rayleigh_quotient.py` & `numqi-0.2.0/project/ws00/draft_rayleigh_quotient.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_ame/draft00.py` & `numqi-0.2.0/project/ws_ame/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_ame/draft01.py` & `numqi-0.2.0/project/ws_ame/draft01.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_ce/draft00.py` & `numqi-0.2.0/project/ws_ce/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_clifford/draft00.py` & `numqi-0.2.0/project/ws_clifford/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_dmrg/draft00.py` & `numqi-0.2.0/project/ws_dmrg/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_dmrg/draft01.py` & `numqi-0.2.0/project/ws_dmrg/draft01.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_gme/draft00.py` & `numqi-0.2.0/project/ws_gme/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_gme/ghz3_basic.png` & `numqi-0.2.0/project/ws_gme/ghz3_basic.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_gme/ghz4_basic.png` & `numqi-0.2.0/project/ws_gme/ghz4_basic.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_gme/ghz5_basic.png` & `numqi-0.2.0/project/ws_gme/ghz5_basic.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_iUD/README.md` & `numqi-0.2.0/project/ws_iUD/README.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_iUD/draft00.py` & `numqi-0.2.0/project/ws_iUD/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_iUD/draft01.py` & `numqi-0.2.0/project/ws_iUD/draft01.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_iUD/draft02.py` & `numqi-0.2.0/project/ws_iUD/draft02.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_iUD/draft03.py` & `numqi-0.2.0/project/ws_iUD/draft03.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_iUD/draft04.py` & `numqi-0.2.0/project/ws_iUD/draft04.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_iUD/draft05.py` & `numqi-0.2.0/project/ws_iUD/draft05.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_irrep/README.md` & `numqi-0.2.0/project/ws_irrep/README.md`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_irrep/SymmetricExtensionBoundary.m` & `numqi-0.2.0/project/ws_irrep/SymmetricExtensionBoundary.m`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_irrep/demo_hermitian_basis.py` & `numqi-0.2.0/project/ws_irrep/demo_hermitian_basis.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_irrep/demo_qetlab_time.m` & `numqi-0.2.0/project/ws_irrep/demo_qetlab_time.m`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_irrep/draft00.py` & `numqi-0.2.0/project/ws_irrep/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k3_ppt_pyramid_tiles.png` & `numqi-0.2.0/project/ws_numerical_range/data/3x3_k3_ppt_pyramid_tiles.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k3_werner_isotropic.png` & `numqi-0.2.0/project/ws_numerical_range/data/3x3_k3_werner_isotropic.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k3_werner_tiles.png` & `numqi-0.2.0/project/ws_numerical_range/data/3x3_k3_werner_tiles.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k4_werner_isotropic.png` & `numqi-0.2.0/project/ws_numerical_range/data/3x3_k4_werner_isotropic.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/3x3_k5_ppt_pyramid_tiles.png` & `numqi-0.2.0/project/ws_numerical_range/data/3x3_k5_ppt_pyramid_tiles.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/eigen_degen_2x2_4ext.png` & `numqi-0.2.0/project/ws_numerical_range/data/eigen_degen_2x2_4ext.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/example-1b.png` & `numqi-0.2.0/project/ws_numerical_range/data/example-1b.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/example-1c.png` & `numqi-0.2.0/project/ws_numerical_range/data/example-1c.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/example-abc.png` & `numqi-0.2.0/project/ws_numerical_range/data/example-abc.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/data/rand_2x2_4ext.png` & `numqi-0.2.0/project/ws_numerical_range/data/rand_2x2_4ext.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/draft00.py` & `numqi-0.2.0/project/ws_numerical_range/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/draft01.py` & `numqi-0.2.0/project/ws_numerical_range/draft01.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/draft03.py` & `numqi-0.2.0/project/ws_numerical_range/draft03.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_numerical_range/draft04.py` & `numqi-0.2.0/project/ws_numerical_range/draft04.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_optimal_control/draft00.py` & `numqi-0.2.0/project/ws_optimal_control/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_optimal_control/draft01.py` & `numqi-0.2.0/project/ws_optimal_control/draft01.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_pureb/draft00.py` & `numqi-0.2.0/project/ws_pureb/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_pureb/draft01.py` & `numqi-0.2.0/project/ws_pureb/draft01.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_qec733/draft00.py` & `numqi-0.2.0/project/ws_qec733/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_qnn_material/draft00.py` & `numqi-0.2.0/project/ws_qnn_material/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/draft00.py` & `numqi-0.2.0/project/ws_sep_classifier/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/draft01.py` & `numqi-0.2.0/project/ws_sep_classifier/draft01.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/draft02.py` & `numqi-0.2.0/project/ws_sep_classifier/draft02.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/draft_bes_volume.py` & `numqi-0.2.0/project/ws_sep_classifier/draft_bes_volume.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/draft_haar_k.py` & `numqi-0.2.0/project/ws_sep_classifier/draft_haar_k.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/fig/clf_logits_dist.png` & `numqi-0.2.0/project/ws_sep_classifier/fig/clf_logits_dist.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/fig/clf_random_random.png` & `numqi-0.2.0/project/ws_sep_classifier/fig/clf_random_random.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/fig/clf_werner_isotropic.png` & `numqi-0.2.0/project/ws_sep_classifier/fig/clf_werner_isotropic.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/fig/clf_werner_tiles.png` & `numqi-0.2.0/project/ws_sep_classifier/fig/clf_werner_tiles.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/fig/ginibre_sep.png` & `numqi-0.2.0/project/ws_sep_classifier/fig/ginibre_sep.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/fig/regr_werner_isotropic.png` & `numqi-0.2.0/project/ws_sep_classifier/fig/regr_werner_isotropic.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/ppt.ipynb` & `numqi-0.2.0/project/ws_sep_classifier/ppt.ipynb`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/ppt_rank_sampling.ipynb` & `numqi-0.2.0/project/ws_sep_classifier/ppt_rank_sampling.ipynb`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/qudit.ipynb` & `numqi-0.2.0/project/ws_sep_classifier/qudit.ipynb`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/qudit_rank_sampling.ipynb` & `numqi-0.2.0/project/ws_sep_classifier/qudit_rank_sampling.ipynb`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/sep.ipynb` & `numqi-0.2.0/project/ws_sep_classifier/sep.ipynb`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_sep_classifier/utils.py` & `numqi-0.2.0/project/ws_sep_classifier/utils.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_trotter/draft00.py` & `numqi-0.2.0/project/ws_trotter/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_upb/draft00.py` & `numqi-0.2.0/project/ws_upb/draft00.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_upb/upb-genshifts-graph.png` & `numqi-0.2.0/project/ws_upb/upb-genshifts-graph.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_upb/upb-gentiles1-graph.png` & `numqi-0.2.0/project/ws_upb/upb-gentiles1-graph.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/project/ws_upb/upb-gentiles2-graph.png` & `numqi-0.2.0/project/ws_upb/upb-gentiles2-graph.png`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/pyproject.toml` & `numqi-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -10,49 +10,53 @@
 description = "a numpy-based quantum information toolbox"
 readme = "README.md"
 keywords = ["quantum information"]
 license = { text = "GNU Affero General Public License v3.0" }
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
+requires-python = ">= 3.10"
 dependencies = [
     'numpy',
     'opt_einsum',
     'scipy',
     'tqdm',
     'sympy',
     'torch',
     'cvxpy',
     'matplotlib',
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
-    "twine",
+    # below for testing
     "pytest",
     "pytest-cov",
     "pytest-xdist",
     # below for building documentation
     "mkdocs",
     "jupyter",
     "ipywidgets",
     "mkdocs-material",
     "mkdocs-jupyter",
     "pymdown-extensions",
     "mkdocstrings[python]",
+    "mkdocs-git-revision-date-localized-plugin",
+    "mkdocs-git-authors-plugin",
+    "pyyaml",
     # below for building pypi package
     "build",
     "twine",
 ]
 
 [project.urls]
-Homepage = "https://github.com/husisy/numqi/"
-Documentation = "https://husisy.github.io/numqi/"
-Issues = "https://github.com/husisy/numqi/issues"
+Homepage = "https://github.com/numqi/numqi/"
+Documentation = "https://numqi.github.io/numqi/"
+Issues = "https://github.com/numqi/numqi/issues"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 
 [tool.setuptools_scm]
 write_to = "python/numqi/_version.py"
```

### Comparing `numqi-0.1.1b0/python/numqi/_data/pauli_ud_core.json` & `numqi-0.2.0/python/numqi/_data/pauli_ud_core.json`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/_torch_op.py` & `numqi-0.2.0/python/numqi/_torch_op.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/channel/_gradient_model.py` & `numqi-0.2.0/python/numqi/channel/_gradient_model.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/channel/_internal.py` & `numqi-0.2.0/python/numqi/channel/_internal.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/dicke.py` & `numqi-0.2.0/python/numqi/dicke.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/entangle/__init__.py` & `numqi-0.2.0/python/numqi/entangle/__init__.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/entangle/_misc.py` & `numqi-0.2.0/python/numqi/entangle/_misc.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/entangle/cha.py` & `numqi-0.2.0/python/numqi/entangle/cha.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/entangle/eof.py` & `numqi-0.2.0/python/numqi/entangle/eof.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,14 @@
         r'''Initialize the model
 
         Parameters:
             dimA (int): the dimension of the first subsystem
             dimB (int): the dimension of the second subsystem
             num_term (int): the number of terms in the variational ansatz, `num_term` is bounded by (dimA*dimB)**2
             rank (int): the rank of the density matrix
-            zero_eps (float): a small number to avoid sqrt(0)
         '''
         super().__init__()
         self.dtype = torch.float64
         self.cdtype = torch.complex128
         self.dimA = dimA
         self.dimB = dimB
         if rank is None:
```

### Comparing `numqi-0.1.1b0/python/numqi/entangle/measure.py` & `numqi-0.2.0/python/numqi/entangle/measure.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/entangle/ppt.py` & `numqi-0.2.0/python/numqi/entangle/ppt.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/entangle/pureb.py` & `numqi-0.2.0/python/numqi/entangle/pureb.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/entangle/pureb_quantum.py` & `numqi-0.2.0/python/numqi/entangle/pureb_quantum.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/entangle/symext.py` & `numqi-0.2.0/python/numqi/entangle/symext.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/entangle/upb.py` & `numqi-0.2.0/python/numqi/entangle/upb.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/gate/_internal.py` & `numqi-0.2.0/python/numqi/gate/_internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
         tmp1 = np.exp(1j*phi)
         ret = np.stack([ct,-st*tmp0,st*tmp1,ct*tmp0*tmp1], axis=-1).reshape(*ct.shape, 2, 2)
     return ret
 
 
 def get_quditX(d):
     # Weyl–Heisenberg matrices https://en.wikipedia.org/wiki/Generalizations_of_Pauli_matrices
-    ret = np.diag(np.ones(d-1), 1)
-    ret[-1,0] = 1
+    ret = np.diag(np.ones(d-1), -1)
+    ret[0,-1] = 1
     return ret
 
 
 def get_quditH(d):
     # Weyl–Heisenberg matrices https://en.wikipedia.org/wiki/Generalizations_of_Pauli_matrices
     tmp0 = np.exp(2j*np.pi*np.arange(d)/d)
     ret = np.vander(tmp0, d, increasing=True) / np.sqrt(d)
@@ -120,15 +120,15 @@
     return ret
 
 
 @functools.lru_cache
 def _get_quditX_eigen(d:int, is_torch:bool):
     tmp0 = np.arange(d) - (np.arange(d)>(d/2))*d
     EVL_log = tmp0 * (2*np.pi / d)
-    EVC = get_quditH(d)
+    EVC = get_quditH(d).T.conj().copy()
     if is_torch:
         EVL_log_torch = torch.tensor(EVL_log, dtype=torch.complex128)
         EVC_torch = torch.tensor(EVC, dtype=torch.complex128)
         ret = EVL_log_torch, EVC_torch
     else:
         ret = EVL_log, EVC
     return ret
```

### Comparing `numqi-0.1.1b0/python/numqi/gate/_pauli.py` & `numqi-0.2.0/python/numqi/gate/_pauli.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/gellmann.py` & `numqi-0.2.0/python/numqi/gellmann.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/group/__init__.py` & `numqi-0.2.0/python/numqi/group/__init__.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/group/_internal.py` & `numqi-0.2.0/python/numqi/group/_internal.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/group/_lie.py` & `numqi-0.2.0/python/numqi/group/_lie.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/group/_symmetric.py` & `numqi-0.2.0/python/numqi/group/_symmetric.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/group/spf2.py` & `numqi-0.2.0/python/numqi/group/spf2.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/group/symext.py` & `numqi-0.2.0/python/numqi/group/symext.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/manifold/_ABk.py` & `numqi-0.2.0/python/numqi/manifold/_ABk.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/manifold/__init__.py` & `numqi-0.2.0/python/numqi/manifold/__init__.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/manifold/_compose.py` & `numqi-0.2.0/python/numqi/manifold/_compose.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,35 +112,37 @@
     assert dtype in {torch.complex64,torch.complex128}
     ret = SpecialOrthogonal(dim, batch_size, method, cayley_order, requires_grad, dtype, device)
     return ret
 
 
 class QuantumChannel(torch.nn.Module):
     def __init__(self, dim_in:int, dim_out:int, choi_rank:(int|None)=None, batch_size:(int|None)=None, method:str='qr',
-                return_kind:str='kraus', requires_grad:bool=True, dtype:torch.dtype=torch.complex128, device:torch.device=_CPU):
+                euler_with_phase:bool=False, return_kind:str='kraus', requires_grad:bool=True, dtype:torch.dtype=torch.complex128, device:torch.device=_CPU):
         r'''manifold of quantum channel, wrapper of numqi.manifold.Stiefel
 
         Parameters:
             dim_in (int): dimension of the input quantum state
             dim_out (int): dimension of the output quantum state
             choi_rank (int|None): rank of the Choi matrix
             batch_size (int|None): batch size of quantum channel
             method (str): method to represent quantum channel, choleskyL / qr / polar / so-exp / so-cayley
+            euler_with_phase (bool): whether to use Euler angles with phase
             return_kind (str): return kind of quantum channel, 'kraus' or 'choi'
             requires_grad (bool): whether to require gradient
             dtype (torch.dtype): data type of quantum channel
             device (torch.device): device of quantum channel
         '''
         super().__init__()
         # TODO set polar as default, see chatgpt discussion
         if choi_rank is None:
             choi_rank = dim_in*dim_out
         assert dtype in {torch.complex64,torch.complex128}
         assert return_kind in {'kraus','choi'}
-        self.manifold = Stiefel(choi_rank*dim_out, dim_in, batch_size, method, requires_grad, dtype, device)
+        self.manifold = Stiefel(choi_rank*dim_out, dim_in, batch_size, method=method, euler_with_phase=euler_with_phase,
+                                requires_grad=requires_grad, dtype=dtype, device=device)
         self.dim_in = dim_in
         self.dim_out = dim_out
         self.choi_rank = choi_rank
         self.batch_size = batch_size
         self.return_kind = return_kind
 
     def forward(self):
```

### Comparing `numqi-0.1.1b0/python/numqi/manifold/_internal.py` & `numqi-0.2.0/python/numqi/manifold/_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,15 @@
 
 class Sphere(torch.nn.Module):
     def __init__(self, dim:int, batch_size:(int|None)=None, method:str='quotient',
                 requires_grad:bool=True, dtype:torch.dtype=torch.float64, device:torch.device=_CPU):
         r'''sphere manifold
 
         Parameters:
-            dim (int): dimension of the sphere.
+            dim (int): size of point in Euclidean space, must be at least 2.
             batch_size (int,None): batch size.
             method (str): method to map real vector to a point on the sphere.
                 'quotient': quotient map.
                 'coordinate': cosine and sine functions.
             requires_grad (bool): whether to track the gradients of the parameters.
             dtype (torch.dtype): data type of the parameters, either torch.float32 or torch.float64
             device (torch.device): device of the parameters.
```

### Comparing `numqi-0.1.1b0/python/numqi/manifold/_misc.py` & `numqi-0.2.0/python/numqi/manifold/_misc.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/manifold/_stiefel.py` & `numqi-0.2.0/python/numqi/manifold/_stiefel.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,55 +3,59 @@
 
 from ._internal import _CPU, _hf_para
 from ._internal import to_special_orthogonal_exp, to_special_orthogonal_cayley
 import numqi._torch_op
 
 
 class Stiefel(torch.nn.Module):
-    def __init__(self, dim:int, rank:int, batch_size:(int|None)=None, method:str='polar',
+    def __init__(self, dim:int, rank:int, batch_size:(int|None)=None, method:str='polar', euler_with_phase:bool=False,
                 requires_grad:bool=True, dtype:torch.dtype=torch.float64, device:torch.device=_CPU):
         r'''Stiefel manifold
 
         Parameters:
             dim (int): dimension of the matrix.
             rank (int): rank of the matrix.
             batch_size (int,None): batch size.
             method (str): method to map real vector to a Stiefel matrix.
                 'choleskyL': Cholesky decomposition.
                 'euler': Euler-Hurwitz angles.
                 'qr': QR decomposition.
                 'polar': square root of a matrix.
                 'so-exp': exponential map of special orthogonal group.
                 'so-cayley': Cayley transform of special orthogonal group.
+            euler_with_phase(bool): whether to append phase for `method='euler'`.
             requires_grad (bool): whether to track the gradients of the parameters.
             dtype (torch.dtype): data type of the parameters
                 torch.float32 / torch.float64: real Stiefel matrix
                 torch.complex64 / torch.complex128: complex Stiefel matrix
             device (torch.device): device of the parameters.
         '''
         # TODO polar decomposition https://openreview.net/forum?id=5mtwoRNzjm
         super().__init__()
         assert (dim>=2) and (rank>=1) and (rank<=dim)
         assert dtype in {torch.float32,torch.float64,torch.complex64,torch.complex128}
         assert (batch_size is None) or (batch_size>0)
         assert isinstance(device, torch.device)
         # choleskyL is really bad
-        assert method!='euler', '[TODO] euler is not correctly implemented' #TODO
         assert method in {'choleskyL','qr','so-exp','so-cayley','polar','euler'}
         if method in {'qr','polar'}:
             tmp0 = dim*rank if (dtype in {torch.float32,torch.float64}) else 2*dim*rank
         elif method=='choleskyL':
             tmp0 = (dim*rank-((rank*(rank+1))//2)) * (1 if (dtype in {torch.float32,torch.float64}) else 2)
         elif method in {'so-exp','so-cayley'}: #special orthogonal (SO)
             tmp0 = ((dim*(dim-1))//2) if (dtype in {torch.float32,torch.float64}) else (dim*dim-1)
         else: #euler
-            tmp0 = (dim*rank-rank*(rank+1)//2) if (dtype in {torch.float32,torch.float64}) else (2*dim*rank-rank*(rank+1))
+            if dtype in {torch.float32,torch.float64}:
+                tmp0 = dim*rank-rank*(rank+1)//2
+            else:
+                tmp0 = 2*dim*rank-rank*rank if euler_with_phase else 2*dim*rank-rank*(rank+1)
         tmp1 = (tmp0,) if (batch_size is None) else (batch_size, tmp0)
         tmp2 = torch.float32 if (dtype in {torch.float32,torch.complex64}) else torch.float64
         self.theta = _hf_para(tmp2, requires_grad, *tmp1).to(device)
+        self.euler_with_phase = bool(euler_with_phase)
         self.dim = int(dim)
         self.rank = int(rank)
         self.dtype = dtype
         self.method = method
         self.batch_size = batch_size
 
     def forward(self):
@@ -62,15 +66,15 @@
         elif self.method=='polar':
             ret = to_stiefel_polar(self.theta, self.dim, self.rank)
         elif self.method=='so-exp': #so
             ret = to_special_orthogonal_exp(self.theta, self.dim)[...,:self.rank]
         elif self.method=='so-cayley':
             ret = to_special_orthogonal_cayley(self.theta, self.dim)[...,:self.rank]
         else: #euler
-            ret = to_stiefel_euler(self.theta, self.dim, self.rank)
+            ret = to_stiefel_euler(self.theta, self.dim, self.rank, self.euler_with_phase)
         return ret
 
 def to_stiefel_polar(theta, dim:int, rank:int):
     r'''map real vector to a Stiefel manifold via polar decomposition
 
     [wiki-link](https://en.wikipedia.org/wiki/Stiefel_manifold)
 
@@ -268,19 +272,22 @@
                     if indI+1 < N0:
                         tmp0 = tmp1, ret[:,indI+1]
                     else:
                         zi.append(tmp1)
                 ret = np.concatenate([rowJ, np.stack(zi, axis=1)], axis=2)
     return ret
 
-def _to_stiefel_euler_complex(theta, dim, rank):
-    # TODO add phase
+def _to_stiefel_euler_complex(theta, dim, rank, with_phase):
     # TODO manually backward
     batch = theta.shape[0]
-    theta = theta.reshape(batch, -1, 2)
+    if with_phase:
+        theta_phase = theta[:,(-rank):]
+        theta = theta[:,:(-rank)].reshape(batch, -1, 2)
+    else:
+        theta = theta.reshape(batch, -1, 2)
     tmp0 = np.cumsum(np.arange(dim-rank, dim)).tolist()
     theta_list = [(theta[:,x:y,0],theta[:,x:y,1]) for x,y in zip([0]+tmp0,tmp0)]
     ret = None
     if isinstance(theta, torch.Tensor):
         for theta_i,phi_i in theta_list:
             N0 = theta_i.shape[1]
             tmp0 = phi_i[:,:1]*0
@@ -299,14 +306,16 @@
                     zi.append((ct[:,indI]/expp[:,indI])*tmp0[0] - (st[:,indI]/expp[:,indI])*tmp0[1])
                     tmp1 = (ct[:,indI]*expp[:,indI])*tmp0[1] + (st[:,indI]*expp[:,indI])*tmp0[0]
                     if indI+1 < N0:
                         tmp0 = tmp1, ret[:,indI+1]
                     else:
                         zi.append(tmp1)
                 ret = torch.concat([rowJ, torch.stack(zi, dim=1)], dim=2)
+        if with_phase:
+            ret = ret * torch.exp(1j*theta_phase).reshape(batch,1,rank)
     else:
         for theta_i,phi_i in theta_list:
             N0 = theta_i.shape[1]
             tmp0 = np.zeros((batch,1))
             cum_expp = np.exp(1j*(np.cumsum(np.concatenate([tmp0, phi_i], axis=1), axis=1) - np.concatenate([phi_i, tmp0], axis=1)))
             expp = np.exp(1j*phi_i)
             ct = np.cos(theta_i)
@@ -322,66 +331,72 @@
                     zi.append((ct[:,indI]/expp[:,indI])*tmp0[0] - (st[:,indI]/expp[:,indI])*tmp0[1])
                     tmp1 = (ct[:,indI]*expp[:,indI])*tmp0[1] + (st[:,indI]*expp[:,indI])*tmp0[0]
                     if indI+1 < N0:
                         tmp0 = tmp1, ret[:,indI+1]
                     else:
                         zi.append(tmp1)
                 ret = np.concatenate([rowJ, np.stack(zi, axis=1)], axis=2)
+        if with_phase:
+            ret = ret * np.exp(1j*theta_phase).reshape(batch,1,rank)
     return ret
 
-def to_stiefel_euler(theta:np.ndarray|torch.Tensor, dim:int, rank:int):
+
+def to_stiefel_euler(theta:np.ndarray|torch.Tensor, dim:int, rank:int, with_phase:bool=False):
     r'''map real vector to a Stiefel manifold via Euler-Hurwitz angles
 
     Numerical evaluation of convex-roof entanglement measures with applications to spin rings
     [doi-link](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.80.042301)
 
     real Stiefel: theta [0,pi/2]
 
     complex Stiefel: theta [0,pi/2], phi (-pi,pi)
 
     Parameters:
         theta (np.ndarray,torch.Tensor): if `ndim>1`, then the last dimension will be expanded to the matrix
                 and the rest dimensions will be batch dimensions.
         dim (int): dimension of the matrix.
         rank (int): rank of the matrix.
+        with_phase (bool): whether phase is appended in theta
 
     Returns:
         ret (np.ndarray,torch.Tensor): array of shape `theta.shape[:-1]+(dim,rank)`
     '''
     assert (theta.ndim==1) or (theta.ndim==2)
     shape = theta.shape
     if theta.ndim==1:
         theta = theta.reshape(1, -1)
     else:
         theta = theta.reshape(-1, theta.shape[-1])
     N0 = dim*rank - rank*(rank+1)//2
-    assert (theta.shape[1]==N0) or (theta.shape[1]==2*N0)
+    assert (theta.shape[1]==N0) or (theta.shape[1]==((2*N0+rank) if with_phase else 2*N0))
     if theta.shape[1]==N0:
         ret = _to_stiefel_euler_real(theta, dim, rank)
     else:
-        ret = _to_stiefel_euler_complex(theta, dim, rank)
+        ret = _to_stiefel_euler_complex(theta, dim, rank, with_phase)
     ret = ret.reshape(shape[:-1] + (dim,rank))
     return ret
 
 
-def from_stiefel_euler(np0:np.ndarray, zero_eps:float=1e-10):
+def from_stiefel_euler(np0:np.ndarray, append_phase:bool=False, zero_eps:float=1e-10):
     r'''map a Stiefel manifold to real vector via Euler-Hurwitz angles
 
     Numerical evaluation of convex-roof entanglement measures with applications to spin rings
     [doi-link](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.80.042301)
 
     complex Stiefel ordering: [theta,phi,theta,phi,...]
 
     Parameters:
         np0 (np.ndarray): array of shape (dim,rank)
+        append_phase (bool): whether to append phase to the output.
         zero_eps (float): small number to avoid division by zero.
 
     Returns:
         ret (np.ndarray): array of shape (N0,) where N0=dim*rank-rank*(rank+1)//2 for real Stiefel,
-            and N0=2*dim*rank-rank*(rank+1) for complex Stiefel.
+            and N0=2*dim*rank-rank*(rank+1) for complex Stiefel (if `append_phase=True`, N0+rank).
+        phase (np.ndarray): real array of shape (rank,)
     '''
     assert isinstance(np0, np.ndarray) and (np0.ndim==2)
     dim,rank = np0.shape
     isreal = not np.iscomplexobj(np0)
     ret = []
     np1 = np0.copy()
     for indJ in range(rank):
@@ -413,8 +428,10 @@
     if isreal:
         ret = np.array(ret[::-1])
     else:
         ret = np.array(ret).reshape(-1,2)[::-1].reshape(-1)
     # sign = np.sign(np.diag(np1))
     # for real Stiefel, seems sign are always 1, we don't see negative sign
     phase = np.angle(np.diag(np1))
+    if (not isreal) and append_phase:
+        ret = np.concatenate([ret,phase])
     return ret,phase
```

### Comparing `numqi-0.1.1b0/python/numqi/manifold/plot.py` & `numqi-0.2.0/python/numqi/manifold/plot.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/matrix_space/__init__.py` & `numqi-0.2.0/python/numqi/matrix_space/__init__.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/matrix_space/_clebsch_gordan.py` & `numqi-0.2.0/python/numqi/matrix_space/_clebsch_gordan.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/matrix_space/_geometric_measure.py` & `numqi-0.2.0/python/numqi/matrix_space/_geometric_measure.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/matrix_space/_gradient.py` & `numqi-0.2.0/python/numqi/matrix_space/_gradient.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/matrix_space/_hierarchy.py` & `numqi-0.2.0/python/numqi/matrix_space/_hierarchy.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/matrix_space/_misc.py` & `numqi-0.2.0/python/numqi/matrix_space/_misc.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/matrix_space/_numerical_range.py` & `numqi-0.2.0/python/numqi/matrix_space/_numerical_range.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/maximum_entropy/_internal.py` & `numqi-0.2.0/python/numqi/maximum_entropy/_internal.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/maximum_entropy/_model.py` & `numqi-0.2.0/python/numqi/maximum_entropy/_model.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/optimal_control.py` & `numqi-0.2.0/python/numqi/optimal_control.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/optimize/_internal.py` & `numqi-0.2.0/python/numqi/optimize/_internal.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/qec/__init__.py` & `numqi-0.2.0/python/numqi/qec/__init__.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/qec/_internal.py` & `numqi-0.2.0/python/numqi/qec/_internal.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/qec/_qecc.py` & `numqi-0.2.0/python/numqi/qec/_qecc.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/qec/_varqec.py` & `numqi-0.2.0/python/numqi/qec/_varqec.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/query/_gradient_model.py` & `numqi-0.2.0/python/numqi/query/_gradient_model.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/query/_sdp_model.py` & `numqi-0.2.0/python/numqi/query/_sdp_model.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/query/utils.py` & `numqi-0.2.0/python/numqi/query/utils.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/random/__init__.py` & `numqi-0.2.0/python/numqi/random/__init__.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/random/_internal.py` & `numqi-0.2.0/python/numqi/random/_internal.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/random/_public.py` & `numqi-0.2.0/python/numqi/random/_public.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/random/_spf2.py` & `numqi-0.2.0/python/numqi/random/_spf2.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/sim/_misc.py` & `numqi-0.2.0/python/numqi/sim/_misc.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/sim/_torch_utils.py` & `numqi-0.2.0/python/numqi/sim/_torch_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import numpy as np
 import torch
 import itertools
 
 import numqi.sim.state
 
+from ._internal import _ParameterHolder
+
 class _CircuitFunction(torch.autograd.Function):
     @staticmethod
     def forward(ctx, *args):
         gate_torch = args[:-2]
         q0 = args[-2]
         if isinstance(q0, torch.Tensor):
             q0 = q0.detach().numpy()
         ind_gate_to_info = args[-1]
         name_list = ind_gate_to_info[-1]
         gate_np_dict = {x:y.detach().numpy() for x,y in zip(name_list, gate_torch)}
         for ind0 in range(max(ind_gate_to_info.keys())+1):
             info = ind_gate_to_info[ind0]
             kind = info['kind']
-            if 'ind_theta' in info:
-                array = gate_np_dict[info['name']][info['ind_theta']]
+            if 'ind_torch' in info:
+                array = gate_np_dict[info['name']][info['ind_torch']]
             else:
                 array = info.get('array', None)
             index = info['index']
             gate = info.get('gate', None)
             if kind=='unitary':
                 q0 = numqi.sim.state.apply_gate(q0, array, index)
             elif kind=='control':
@@ -48,17 +50,17 @@
         q0_conj = ctx.saved_tensors[0].detach().numpy().conj()
         q0_grad = grad_output.detach().numpy()
         for ind0 in reversed(range(max(ind_gate_to_info.keys())+1)):
             info = ind_gate_to_info[ind0]
             kind = info['kind']
             name = info['name']
             assert kind!='measure', 'not support measure in gradient backward yet'
-            require_grad = 'ind_theta' in info
+            require_grad = 'ind_torch' in info
             if require_grad:
-                array = gate_np_dict[info['name']][info['ind_theta']]
+                array = gate_np_dict[info['name']][info['ind_torch']]
             else:
                 array = info.get('array', None)
             index = info['index']
             gate = info.get('gate', None)
             if kind=='control':
                 q0_conj, q0_grad, op_grad = numqi.sim.state.apply_control_n_gate_grad(
                         q0_conj, q0_grad, array, index[0], index[1], tag_op_grad=require_grad)
@@ -66,15 +68,15 @@
                 q0_conj, q0_grad, op_grad = numqi.sim.state.apply_gate_grad(q0_conj,
                         q0_grad, array, index, tag_op_grad=require_grad)
             elif kind=='custom':
                 q0_conj, q0_grad, op_grad = gate.grad_backward(q0_conj, q0_grad)#TODO
             else:
                 raise KeyError(f'not recognized gate "{gate}"')
             if require_grad:
-                gate_grad_np_dict[name][info['ind_theta']] += op_grad
+                gate_grad_np_dict[name][info['ind_torch']] += op_grad
         name_list = ind_gate_to_info[-1]
         ret = tuple(torch.from_numpy(gate_grad_np_dict[x]) for x in name_list) + (torch.from_numpy(q0_grad),None)
         return ret
 
 
 def _get_first_come_id(object_list, index_list):
     id_to_index = dict()
@@ -96,90 +98,125 @@
         self.num_qubit = circuit.num_qubit
         self._setup(circuit.gate_index_list)
 
     def _setup(self, gate_index_list):
         hf0 = lambda x: x.name
         tmp0 = (x for x,_ in gate_index_list)
         tmp0 = {x:list(y) for x,y in itertools.groupby(sorted(tmp0, key=hf0), key=hf0)}
-        # name must be unique
+        # for each name, all hf0 must be the same
+        hf0_dict = dict()
         for key,value in tmp0.items():
             assert len({x.kind for x in value})==1
             tmp1 = [x.hf0 for x in value if hasattr(x, 'hf0')]
             if len(tmp1)>1:
                 assert all(x==tmp1[0] for x in tmp1[1:])
+            if any((x.requires_grad or (hasattr(x,'args') and isinstance(x.args, _ParameterHolder))) for x in value):
+                hf0_dict[key] = value[0].hf0
+
+        # pgate
         theta = dict()
         ind_theta_to_ind_gate = dict()
-        tmp0 = [(ind0,x) for ind0,(x,_) in enumerate(gate_index_list) if x.requires_grad]
+        tmp0 = [(ind0,x) for ind0,(x,_) in enumerate(gate_index_list) if (x.requires_grad) and (not isinstance(x.args, _ParameterHolder))]
         hf0 = lambda x: x[1].name
         tmp0 = {x:list(y) for x,y in itertools.groupby(sorted(tmp0, key=hf0), key=hf0)}
         for key,value in tmp0.items():
             tmp1 = _get_first_come_id([x[1] for x in value], [x[0] for x in value])
             tmp2 = torch.from_numpy(np.array([gate_index_list[x[0]][0].args for x in tmp1], dtype=np.float64))
             theta[key] = torch.nn.Parameter(tmp2)
             ind_theta_to_ind_gate[key] = tmp1
         ind_gate_to_ind_theta = {y:(k,x0) for k,v in ind_theta_to_ind_gate.items() for x0,x1 in enumerate(v) for y in x1}
-        pgate_name_list = sorted(theta.keys())
-        pgate_custom_name_list = [x for x in pgate_name_list if (gate_index_list[ind_theta_to_ind_gate[x][0][0]][0].kind=='custom')]
-        theta = torch.nn.ParameterDict(theta)
-        hf0_dict = {x:gate_index_list[ind_theta_to_ind_gate[x][0][0]][0].hf0 for x in pgate_name_list}
 
-        ind_gate_to_info = {-1: pgate_name_list}
+        # hgate_name_list
+        hgate_list = [x for x,_ in gate_index_list if (hasattr(x,'args') and isinstance(x.args, _ParameterHolder))]
+        assert len(hgate_list)==len(set(id(x) for x in hgate_list)), 'PlaceHolder gate cannot be re-used'
+        tmp0 = [(ind0,x) for ind0,(x,_) in enumerate(gate_index_list) if (hasattr(x,'args') and isinstance(x.args, _ParameterHolder))]
+        hf0 = lambda x: x[1].name
+        ind_torch_to_ind_hgate = {x:[z[0] for z in y] for x,y in itertools.groupby(sorted(tmp0, key=hf0), key=hf0)}
+        tmp0 = {x1:(k,(x0+len(ind_theta_to_ind_gate.get(k,[])))) for k,v in ind_torch_to_ind_hgate.items() for x0,x1 in enumerate(v)}
+        assert len(set(tmp0.keys()).intersection(set(ind_gate_to_ind_theta.keys())))==0
+        ind_gate_to_ind_torch = ind_gate_to_ind_theta | tmp0
+
+        hpgate_name_list = sorted({x[0] for x in ind_gate_to_ind_torch.values()})
+        ind_gate_to_info = {-1: hpgate_name_list}
         for ind0,(gate,index) in enumerate(gate_index_list):
             kind = gate.kind
             name = gate.name
-            if ind0 in ind_gate_to_ind_theta:
-                ind_theta = ind_gate_to_ind_theta[ind0][1]
+            if ind0 in ind_gate_to_ind_torch:
+                ind_torch = ind_gate_to_ind_torch[ind0][1]
                 if kind=='custom':
                     info = dict(kind=kind, name=name, index=index, gate=gate)
                 else:
                     assert kind in {'unitary','control'}
-                    info = dict(kind=kind, name=name, index=index, ind_theta=ind_theta)
+                    info = dict(kind=kind, name=name, index=index, ind_torch=ind_torch)
             else:
                 if kind in {'unitary','control'}:
                     info = dict(kind=kind, name=name, index=index, array=gate.array)
                 else: #custom measure
                     info = dict(kind=kind, name=name, index=index, gate=gate)
             ind_gate_to_info[ind0] = info
 
         self.ind_theta_to_ind_gate = ind_theta_to_ind_gate
         # ind_theta_to_ind_gate: (dict, str, (list, (list,int)))
         self.ind_gate_to_ind_theta = ind_gate_to_ind_theta
         # ind_gate_to_ind_theta: (dict, int, (str, int))
-        self.pgate_name_list = pgate_name_list
-        # pgate_name_list(list,str)
-        self.pgate_custom_name_list = pgate_custom_name_list
-        # pgate_custom_name_list(list,str)
-        self.theta = theta
+        self.theta = torch.nn.ParameterDict(theta)
         # theta(torch.nn.ParameterDict)
         self.hf0_dict = hf0_dict
         # hf0_dict(dict, str, function)
         self.ind_gate_to_info = ind_gate_to_info
         # key=-1: (list,str) list of pgate name
         # key=0...: dict
         #   kind: str, control, unitary, measure, custom
         #   name: str
         #   index: (tuple,int)
-        #   ind_theta: int, required for pgate
+        #   ind_torch: int, required for pgate
         #   array: np.ndarray, required for kind=unitary or kind=control
         #   gate: Gate, required for kind=custom
 
+        self.ind_gate_to_ind_torch = ind_gate_to_ind_torch
+        self.ind_torch_to_ind_hgate = ind_torch_to_ind_hgate
+        self.hgate_torch_dict = {}
+
+    def setP(self, *args, **kwargs):
+        if len(args)>0:
+            assert len(args)==1
+            self.circuit._P[''] = args[0]
+        for k,v in kwargs.items():
+            self.circuit._P[k] = v
+        self.hgate_torch_dict.clear()
+        for key,value in self.ind_torch_to_ind_hgate.items():
+            tmp0 = [self.circuit.gate_index_list[x][0].args.resolve() for x in value]
+            tmp1 = torch.stack(tmp0).reshape(len(tmp0), -1)
+            self.hgate_torch_dict[key] = self.hf0_dict[key](*tmp1.T)
+
     def forward(self, q0):
-        gate_torch_dict = {k: self.hf0_dict[k](*v.T) for k,v in self.theta.items()}
+        pgate_torch_dict = {k: self.hf0_dict[k](*v.T) for k,v in self.theta.items()}
         # custom pgate must be set_args before calling
-        for name in self.pgate_custom_name_list:
-            tmp0 = gate_torch_dict[name].detach().numpy()
+        tmp0 = [x for x in self.theta.keys() if (self.circuit.gate_index_list[self.ind_theta_to_ind_gate[x][0][0]][0].kind=='custom')]
+        for name in tmp0:
+            tmp0 = pgate_torch_dict[name].detach().numpy()
             tmp1 = self.theta[name].detach().numpy()
             for x0,x1 in enumerate(self.ind_theta_to_ind_gate[name]):
                 self.circuit.gate_index_list[x1[0]][0].set_args(tmp1[x0], tmp0[x0])
-        tmp0 = sorted(gate_torch_dict.items(), key=lambda x: x[0])
-        gate_torch_list = [x[1] for x in tmp0]
+        tmp0 = sorted({x[0] for x in self.ind_gate_to_ind_torch.values()})
+        gate_torch_list = []
+        for key in tmp0:
+            x = pgate_torch_dict.get(key, None)
+            y = self.hgate_torch_dict.get(key, None)
+            assert not ((x is None) and (y is None))
+            if x is None:
+                gate_torch_list.append(y)
+            elif y is None:
+                gate_torch_list.append(x)
+            else:
+                gate_torch_list.append(torch.concat([x,y], axis=0))
         q0 = _CircuitFunction.apply(*gate_torch_list, q0, self.ind_gate_to_info)
         return q0
 
     def fresh_gate_parameter(self):
         with torch.no_grad():
             gate_torch_dict = {k: self.hf0_dict[k](*v.T) for k,v in self.theta.items()}
-        for name in self.pgate_name_list:
+        for name in gate_torch_dict.keys():
             tmp0 = gate_torch_dict[name].detach().numpy()
             tmp1 = self.theta[name].detach().numpy()
             for x0,x1 in enumerate(self.ind_theta_to_ind_gate[name]):
                 self.circuit.gate_index_list[x1[0]][0].set_args(tmp1[x0], tmp0[x0])
```

### Comparing `numqi-0.1.1b0/python/numqi/sim/circuit.py` & `numqi-0.2.0/python/numqi/sim/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch
 
 import numqi.gate
 import numqi.channel
 import numqi.sim.state
 from numqi.utils import hf_tuple_of_int, hf_tuple_of_any
 
-from ._internal import Gate, ParameterGate
+from ._internal import Gate, ParameterGate, _ParameterHolder
 from ._torch_utils import CircuitTorchWrapper
 
 CANONICAL_GATE_KIND = {'unitary','control','measure'}
 # TODO kraus
 
 
 class MeasureGate:
@@ -63,18 +63,19 @@
     return hf0
 
 
 def _unitary_parameter_gate(name_, hf0, num_index, num_parameter):
     def hf1(self, index, args=None, name=name_, requires_grad=None):
         if requires_grad is None:
             requires_grad = self.default_requires_grad
-        if args is None:
-            args = (0.,)*num_parameter #initialize to zero
-        else:
-            args = hf_tuple_of_any(args, type_=float) #convert float/int into tuple
+        if not isinstance(args, _ParameterHolder): #_ParameterHolder is handled in ParameterGate
+            if args is None:
+                args = (0.,)*num_parameter #initialize to zero
+            else:
+                args = hf_tuple_of_any(args, type_=float) #convert float/int into tuple
         gate = ParameterGate('unitary', hf0, args, name=name, requires_grad=requires_grad)
         index = hf_tuple_of_int(index)
         assert len(index)==num_index
         self.gate_index_list.append((gate, index))
         return gate
     return hf1
 
@@ -110,14 +111,31 @@
         r'''initialize the circuit
 
         Parameters:
             default_requires_grad (bool): default value of requires_grad for the parameterized gate
         '''
         self.gate_index_list = []
         self.default_requires_grad = default_requires_grad
+        self._P:dict = dict()
+        self.P:_ParameterHolder = _ParameterHolder(self._P) #parameter placeholder
+
+    def setP(self, *args, **kwargs):
+        if len(args)>0:
+            assert len(args)==1
+            self._P[''] = args[0]
+        for k,v in kwargs.items():
+            self._P[k] = v
+        for gate,_ in self.gate_index_list:
+            if hasattr(gate, 'args') and isinstance(gate.args, _ParameterHolder):
+                tmp0 = gate.args.resolve()
+                if hasattr(tmp0, '__len__'):
+                    array = gate.hf0(*tmp0)
+                else:
+                    array = gate.hf0(tmp0)
+                gate.set_args(tmp0, array)
 
     def append_gate(self, gate:Gate, index:int|tuple[int]):
         r'''append a gate to the circuit. Trainable parameters are re-used.
 
 
         Parameters:
             gate (numqi.sim.Gate): the gate to be appended
@@ -472,14 +490,16 @@
 
         Parameters:
             q0 (np.ndarray): the quantum state, `shape=(2**num_qubit,)`
 
         Returns:
             ret (np.ndarray): the quantum state after the circuit, `shape=(2**num_qubit,)`
         '''
+        if any(hasattr(x,'args') and isinstance(x.args, _ParameterHolder) and (x.array is None) for x,_ in self.gate_index_list):
+            raise ValueError('Parameterized gate with placeholder is used, call "circ.setP" to initialize those gates first')
         for gate,index in self.gate_index_list:
             if gate.kind=='unitary':
                 q0 = numqi.sim.state.apply_gate(q0, gate.array, index)
             elif gate.kind=='control':
                 q0 = numqi.sim.state.apply_control_n_gate(q0, gate.array, index[0], index[1])
             elif gate.kind=='measure':
                 q0 = gate.forward(q0)
```

### Comparing `numqi-0.1.1b0/python/numqi/sim/clifford.py` & `numqi-0.2.0/python/numqi/sim/clifford.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/sim/dm.py` & `numqi-0.2.0/python/numqi/sim/dm.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/sim/state.py` & `numqi-0.2.0/python/numqi/sim/state.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/state/_internal.py` & `numqi-0.2.0/python/numqi/state/_internal.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,7 +416,25 @@
     ret = np.eye(9, dtype=np.float64)*(a/(8*a+1))
     ret[[0,0,4,4,8,8],[4,8,0,8,0,4]] = a/(8*a+1)
     ret[[6,8],[6,8]] = (1+a)/(16*a+2)
     ret[[6,8], [8,6]] = np.sqrt(1-a*a)/(16*a+2)
     return ret
 
 
+def maximally_coherent_state(d:int, return_dm:bool=False):
+    r'''get the maximally coherent state
+
+    reference: [arxiv-link](https://arxiv.org/abs/1503.07103)
+
+    Parameters:
+        d (int): the dimension of the Hilbert space
+        return_dm (bool): whether to return the density matrix
+
+    Returns:
+        ret (np.ndarray): the maximally coherent state, `ret.ndim=1` or `ret.ndim=2`
+    '''
+    assert d>=1
+    if return_dm:
+        ret = np.eye(d, dtype=np.float64) / d
+    else:
+        ret = np.ones(d, dtype=np.float64) / np.sqrt(d)
+    return ret
```

### Comparing `numqi-0.1.1b0/python/numqi/unique_determine/_internal.py` & `numqi-0.2.0/python/numqi/unique_determine/_internal.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/unique_determine/_recovery.py` & `numqi-0.2.0/python/numqi/unique_determine/_recovery.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/unique_determine/_uda_udp.py` & `numqi-0.2.0/python/numqi/unique_determine/_uda_udp.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/python/numqi/utils.py` & `numqi-0.2.0/python/numqi/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,18 +52,18 @@
     r'''convert a complex matrix to a real matrix
 
     `complex -> [[real,-imag], [imag,real]]`
 
     $$ A\in\mathbb{C}^{m\times n}\mapsto\begin{bmatrix} \Re[A] & -\Im[A]\\ \Im[A] & \Re[A] \end{bmatrix}\in\mathbb{R}^{2m\times2n} $$
 
     Parameters:
-        x (np.ndarray,torch.Tensor): a complex matrix, shape=(...,dim0,dim1), support batch
+        x (np.ndarray,torch.Tensor): a complex matrix, shape=(...,m,n), support batch
 
     Returns:
-        ret (np.ndarray,torch.Tensor): a real matrix, shape=(...,2*dim0,2*dim1)
+        ret (np.ndarray,torch.Tensor): a real matrix, shape=(...,2m,2n)
     '''
     dim0,dim1 = x.shape[-2:]
     shape = x.shape[:-2]
     x = x.reshape(-1, dim0, dim1)
     # ret = np.block([[x.real,-x.imag],[x.imag,x.real]])
     if isinstance(x, torch.Tensor):
         tmp0 = torch.concat([x.real, -x.imag], dim=2)
```

### Comparing `numqi-0.1.1b0/python/numqi.egg-info/PKG-INFO` & `numqi-0.2.0/python/numqi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 Metadata-Version: 2.1
 Name: numqi
-Version: 0.1.1b0
+Version: 0.2.0
 Summary: a numpy-based quantum information toolbox
 Author-email: husisy <donot@mail.me>
 License: GNU Affero General Public License v3.0
-Project-URL: Homepage, https://github.com/husisy/numqi/
-Project-URL: Documentation, https://husisy.github.io/numqi/
-Project-URL: Issues, https://github.com/husisy/numqi/issues
+Project-URL: Homepage, https://github.com/numqi/numqi/
+Project-URL: Documentation, https://numqi.github.io/numqi/
+Project-URL: Issues, https://github.com/numqi/numqi/issues
 Keywords: quantum information
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: opt_einsum
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: sympy
 Requires-Dist: torch
 Requires-Dist: cvxpy
 Requires-Dist: matplotlib
 Provides-Extra: dev
-Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: ipywidgets; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mkdocs-git-revision-date-localized-plugin; extra == "dev"
+Requires-Dist: mkdocs-git-authors-plugin; extra == "dev"
+Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # numqi: a numpy-based quantum information package
 
-[![codecov](https://codecov.io/gh/husisy/numqi/graph/badge.svg?token=50YC4KD4M1)](https://codecov.io/gh/husisy/numqi)
+[![DOI](https://zenodo.org/badge/568701845.svg)](https://zenodo.org/doi/10.5281/zenodo.10867067)
+[![codecov](https://codecov.io/github/numqi/numqi/graph/badge.svg?token=sKLURoXVji)](https://codecov.io/github/numqi/numqi)
 
 WARNING: no backward compatibility guarantee until version `1.0.0`
 
 keyword: quantum information, numpy, pytorch, manifold optimization, trivialization
 
 ## Quickstart
 
@@ -147,15 +151,15 @@
 1. `python/numqi/`: source code
 2. `docs/`: kinds of markdown files for generating website
 3. `tests/`: unit tests
 4. `examples/`: single file scripts to demonstrate how to use `numqi`
 5. `project/`: some projects based on `numqi`, whether finished or not
 6. misc
    * `README.md`: this file
-   * `pyproject.toml`: to make a pip-instalable package
+   * `pyproject.toml`: to make a pip-installable package
    * `mkdocs.yml`: to generate website
    * `LICENSE`
    * `.gitignore`
 
 ## How to contribute
 
 see [docs/installation](./docs/installation.md) "Guide-for-contributors" section
@@ -187,7 +191,19 @@
    id5 -->|large loss| id6
    id6 -->|no| id3
    id6 -->|yes| id7
    id7 -.->|zero loss| id2
    id7 -.->|large loss| id3
    id5 -->|zero loss| id2
 ```
+
+## Recommended courses
+
+1. point-set topology
+    * [youtube-link](https://youtube.com/playlist?list=PLd8NbPjkXPliJunBhtDNMuFsnZPeHpm-0&si=Y5-wnge2rWO1HNVb) Marius Furter
+2. smooth manifold
+    * [youtube-link](https://www.youtube.com/playlist?list=PLBh2i93oe2qvRGAtgkTszX7szZDVd6jh1) The Bright Side of Mathematics
+    * [youtube-link](https://www.youtube.com/playlist?list=PLD2r7XEOtm-AGjr3ynbljbx3oWHdus9Xb) qncubed3
+3. Riemannian manifold
+4. Differential geometry
+5. algebraic topology
+    * [youtube-link](https://www.youtube.com/playlist?list=PLOROtRhtegr7DmeMyFxfKxsljAVsAn_X4) Presented by Dr. Anthony Bosman.
```

### Comparing `numqi-0.1.1b0/python/numqi.egg-info/SOURCES.txt` & `numqi-0.2.0/python/numqi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 docs/application/tomography/state_tomography.ipynb
 docs/data/circuit_basic_pgate.png
 docs/data/detect_entanglement.png
 docs/data/maxent_2qubit_pauli.png
 docs/data/maxent_3qubit_2local_random.png
 docs/data/maxent_4qubit_2local_random.png
 docs/data/project-structure.png
+docs/foundation/get_started/get_started.ipynb
 docs/foundation/group/basic.ipynb
 docs/foundation/group/clifford.ipynb
 docs/foundation/group/pauli.ipynb
 docs/foundation/group/spf2.md
 docs/foundation/group/symext.ipynb
 docs/foundation/group/young-tableaux.ipynb
 docs/foundation/manifold/basic_sphere.ipynb
@@ -125,14 +126,15 @@
 project/entangled_subspace/data/qubit_dicke_state_border_rank.pdf
 project/entangled_subspace/data/qubit_dicke_state_border_rank.pkl
 project/entangled_subspace/data/qubit_dicke_state_border_rank.png
 project/entangled_subspace/data/robustness.pdf
 project/entangled_subspace/data/robustness.pkl
 project/entangled_subspace/data/robustness.png
 project/entangler/draft00.py
+project/entangler/draft01.py
 project/gme_dm/README.md
 project/gme_dm/draft00.py
 project/gme_dm/draft01.py
 project/ws00/draft00.py
 project/ws00/draft02.py
 project/ws00/draft04.py
 project/ws00/draft_rayleigh_quotient.py
@@ -281,14 +283,15 @@
 python/numqi/sim/state.py
 python/numqi/state/__init__.py
 python/numqi/state/_internal.py
 python/numqi/unique_determine/__init__.py
 python/numqi/unique_determine/_internal.py
 python/numqi/unique_determine/_recovery.py
 python/numqi/unique_determine/_uda_udp.py
+scripts/draft_action_mkdocs.py
 tests/test_channel.py
 tests/test_dicke.py
 tests/test_gate.py
 tests/test_gellmann.py
 tests/test_manifold.py
 tests/test_manifold_ABk.py
 tests/test_maximum_entropy.py
```

### Comparing `numqi-0.1.1b0/tests/test_channel.py` & `numqi-0.2.0/tests/test_channel.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_dicke.py` & `numqi-0.2.0/tests/test_dicke.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_entangle/test_entangle_bes.py` & `numqi-0.2.0/tests/test_entangle/test_entangle_bes.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_entangle/test_entangle_cha.py` & `numqi-0.2.0/tests/test_entangle/test_entangle_cha.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_entangle/test_entangle_eof.py` & `numqi-0.2.0/tests/test_entangle/test_entangle_eof.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_entangle/test_entangle_misc.py` & `numqi-0.2.0/tests/test_entangle/test_entangle_misc.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_entangle/test_entangle_ppt.py` & `numqi-0.2.0/tests/test_entangle/test_entangle_ppt.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_entangle/test_entangle_pureb.py` & `numqi-0.2.0/tests/test_entangle/test_entangle_pureb.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_entangle/test_entangle_symext.py` & `numqi-0.2.0/tests/test_entangle/test_entangle_symext.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_entangle/test_entangle_upb.py` & `numqi-0.2.0/tests/test_entangle/test_entangle_upb.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_entangle/test_measure.py` & `numqi-0.2.0/tests/test_entangle/test_measure.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_gate.py` & `numqi-0.2.0/tests/test_gate.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 
 def test_quditXZH():
     for d in range(2,7):
         X = numqi.gate.get_quditX(d)
         Z = numqi.gate.get_quditZ(d)
         H = numqi.gate.get_quditH(d)
-        assert np.abs(X - H @ Z @ H.T.conj()).max() < 1e-10
+        assert np.abs(X - H.T.conj() @ Z @ H).max() < 1e-10
 
 def test_rx_qudit():
     theta = np_rng.uniform(0, 1, size=23)
     z0 = numqi.gate.rx(theta)
     z1 = numqi.gate._internal._rx_qudit(theta, 2)
     assert np.abs(z0-z1).max() < 1e-10
 
@@ -94,15 +94,15 @@
     assert np.abs(z0-z1).max() < 1e-10
 
     for d in range(2, 7):
         theta = np_rng.uniform(0, 1, size=23)
         z0 = numqi.gate.rx(theta, d)
         H = numqi.gate.get_quditH(d)
         z1 = numqi.gate.rz(theta, d, diag_only=False)
-        assert np.abs(z0 - H @ z1 @ H.T.conj()).max() < 1e-10
+        assert np.abs(z0 - H.T.conj() @ z1 @ H).max() < 1e-10
 
         z2 = numqi.gate.rz(torch.tensor(theta, dtype=torch.float64), d, diag_only=False).numpy()
         assert np.abs(z1-z2).max() < 1e-10
 
 
 def test_PauliOperator_convert():
     example_list = [
```

### Comparing `numqi-0.1.1b0/tests/test_gellmann.py` & `numqi-0.2.0/tests/test_gellmann.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_manifold.py` & `numqi-0.2.0/tests/test_manifold.py`

 * *Files 8% similar despite different names*

```diff
@@ -315,7 +315,15 @@
         np1 = numqi.manifold.to_stiefel_euler(theta1, dim, rank)
         assert np.abs(np0-np1*np.exp(1j*phase)).max() < 1e-10
         torch1 = numqi.manifold.to_stiefel_euler(torch.tensor(theta1,dtype=torch.float32), dim, rank)
         torch2 = numqi.manifold.to_stiefel_euler(torch.tensor(theta1,dtype=torch.float64), dim, rank)
         assert (torch1.dtype==torch.float32) or (torch1.dtype==torch.complex64)
         assert np.abs(np1-torch1.numpy()).max() < 1e-5
         assert np.abs(np1-torch2.numpy()).max() < 1e-10
+
+        theta1, phase = numqi.manifold.from_stiefel_euler(np0, append_phase=True)
+        np1 = numqi.manifold.to_stiefel_euler(theta1, dim, rank, with_phase=True)
+        torch1 = numqi.manifold.to_stiefel_euler(torch.tensor(theta1,dtype=torch.float32), dim, rank, with_phase=True)
+        torch2 = numqi.manifold.to_stiefel_euler(torch.tensor(theta1,dtype=torch.float64), dim, rank, with_phase=True)
+        assert (torch1.dtype==torch.float32) or (torch1.dtype==torch.complex64)
+        assert np.abs(np1-torch1.numpy()).max() < 1e-5
+        assert np.abs(np1-torch2.numpy()).max() < 1e-10
```

### Comparing `numqi-0.1.1b0/tests/test_manifold_ABk.py` & `numqi-0.2.0/tests/test_manifold_ABk.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_maximum_entropy.py` & `numqi-0.2.0/tests/test_maximum_entropy.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_optimal_control.py` & `numqi-0.2.0/tests/test_optimal_control.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_optimize.py` & `numqi-0.2.0/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_qec.py` & `numqi-0.2.0/tests/test_qec.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_query.py` & `numqi-0.2.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_random.py` & `numqi-0.2.0/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_state.py` & `numqi-0.2.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_torch_op.py` & `numqi-0.2.0/tests/test_torch_op.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_unique_determine.py` & `numqi-0.2.0/tests/test_unique_determine.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/test_utils.py` & `numqi-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_group/test_group_basic.py` & `numqi-0.2.0/tests/tests_group/test_group_basic.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_group/test_group_lie.py` & `numqi-0.2.0/tests/tests_group/test_group_lie.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_group/test_group_spf2.py` & `numqi-0.2.0/tests/tests_group/test_group_spf2.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_group/test_group_symext.py` & `numqi-0.2.0/tests/tests_group/test_group_symext.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_group/test_group_symmetric.py` & `numqi-0.2.0/tests/tests_group/test_group_symmetric.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_matrix_space/test_geometric_measure.py` & `numqi-0.2.0/tests/tests_matrix_space/test_geometric_measure.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space.py` & `numqi-0.2.0/tests/tests_matrix_space/test_matrix_space.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_clebsch_gordan.py` & `numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_clebsch_gordan.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_gradient.py` & `numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_gradient.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_hierarchy.py` & `numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_hierarchy.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_numerical_range.py` & `numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_numerical_range.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_matrix_space/test_matrix_space_superactivation.py` & `numqi-0.2.0/tests/tests_matrix_space/test_matrix_space_superactivation.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_sim/test_sim_circuit.py` & `numqi-0.2.0/tests/tests_sim/test_sim_circuit.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,14 +48,67 @@
     num_qubit = 5
     num_depth = 2
     circuit = build_dummy_circuit(num_depth, num_qubit)
     model = DummyQNNModel(circuit)
     numqi.optimize.check_model_gradient(model)
 
 
+def build_dummy_circuit_holder(num_depth, num_qubit, seed=None):
+    np_rng = numqi.random.get_numpy_rng(seed)
+    circ = numqi.sim.Circuit(default_requires_grad=True)
+    for ind0 in range(num_depth):
+        tmp0 = list(range(0, num_qubit-1, 2)) + list(range(1, num_qubit-1, 2))
+        for ind1 in tmp0:
+            circ.ry(ind1, circ.P['ry'][ind0,ind1])
+            circ.ry(ind1+1, circ.P['ry'][ind0,ind1+1])
+            circ.rz(ind1, circ.P['rz'][ind0,ind1])
+            circ.rz(ind1+1, circ.P['rz'][ind0,ind1+1])
+            circ.rzz((ind1, ind1+1), circ.P['rzz'][ind0,ind1//2])
+            circ.cnot(ind1, ind1+1)
+            tmp0 = numqi.random.rand_special_orthogonal_matrix(2, tag_complex=True, seed=np_rng)
+            circ.controlled_single_qubit_gate(tmp0, (ind1+1,(ind1-1)%num_qubit), ind1)
+            circ.double_qubit_gate(numqi.random.rand_special_orthogonal_matrix(4, tag_complex=True, seed=np_rng), ind1, ind1+1)
+    return circ
+
+
+class DummyHolderQNNModel(torch.nn.Module):
+    def __init__(self, circuit, num_depth):
+        super().__init__()
+        self.circuit_torch = numqi.sim.CircuitTorchWrapper(circuit)
+        self.num_qubit = circuit.num_qubit
+        np_rng = np.random.default_rng()
+        tmp0 = np_rng.normal(size=2**self.num_qubit) + 1j*np_rng.normal(size=2**self.num_qubit)
+        self.target_state = torch.tensor(tmp0 / np.linalg.norm(tmp0), dtype=torch.complex128)
+        hf0 = lambda *x: torch.nn.Parameter(torch.tensor(np_rng.uniform(0, 2*np.pi, size=x), dtype=torch.float64))
+        tmp0 = { #not all parameters are used
+            'ry': hf0(num_depth, self.num_qubit),
+            'rz': hf0(num_depth, self.num_qubit),
+            'rzz': hf0(num_depth, self.num_qubit//2+1),
+        }
+        self.theta = torch.nn.ParameterDict(tmp0)
+        self.q0 = torch.empty(2**self.num_qubit, dtype=torch.complex128, requires_grad=False)
+
+    def forward(self):
+        self.q0[:] = 0
+        self.q0[0] = 1
+        self.circuit_torch.setP(ry=self.theta['ry'], rz=self.theta['rz'], rzz=self.theta['rzz'])
+        q0 = self.circuit_torch(self.q0)
+        tmp0 = torch.vdot(self.target_state, q0)
+        loss = (tmp0*tmp0.conj()).real
+        return loss
+
+
+def test_DummyHolderQNNModel():
+    num_qubit = 5
+    num_depth = 2
+    circuit = build_dummy_circuit_holder(num_depth, num_qubit)
+    model = DummyHolderQNNModel(circuit, num_depth)
+    numqi.optimize.check_model_gradient(model)
+
+
 def test_circuit_to_unitary():
     num_qubit = 5
     num_depth = 3
     circ = build_dummy_circuit(num_depth, num_qubit)
     np0 = numqi.random.rand_haar_state(2**num_qubit)
 
     ret_ = circ.apply_state(np0)
@@ -245,7 +298,27 @@
         # all fundamentally different graph
         # Number of graphs on n unlabeled nodes
         # https://oeis.org/A000088
         # https://qr.ae/pymd0r
         # https://math.stackexchange.com/q/353053
         # https://www.graphclasses.org/smallgraphs.html
         # 1 1 2 4 11 34 156 1044 12346 274668
+
+
+def test_circuit_ParameterHolder():
+    parameter = np_rng.uniform(0, 2*np.pi, size=3)
+    tmp0 = np_rng.normal(size=8) + 1j*np_rng.normal(size=8)
+    q0 = tmp0 / np.linalg.norm(tmp0)
+
+    circ0 = numqi.sim.Circuit()
+    circ0.rx(0, parameter[0])
+    circ0.ry(1, parameter[1])
+    circ0.rz(2, parameter[2])
+    ret_ = circ0.apply_state(q0)
+
+    circ = numqi.sim.Circuit()
+    circ.rx(0, circ.P[0])
+    circ.ry(1, circ.P['ry'])
+    circ.rz(2, circ.P['rz'][0])
+    circ.setP([parameter[0]], ry=parameter[1], rz=[parameter[2]])
+    ret0 = circ.apply_state(q0)
+    assert np.abs(ret_-ret0).max() < 1e-10
```

### Comparing `numqi-0.1.1b0/tests/tests_sim/test_sim_clifford.py` & `numqi-0.2.0/tests/tests_sim/test_sim_clifford.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_sim/test_sim_dm.py` & `numqi-0.2.0/tests/tests_sim/test_sim_dm.py`

 * *Files identical despite different names*

### Comparing `numqi-0.1.1b0/tests/tests_sim/test_sim_state.py` & `numqi-0.2.0/tests/tests_sim/test_sim_state.py`

 * *Files identical despite different names*

