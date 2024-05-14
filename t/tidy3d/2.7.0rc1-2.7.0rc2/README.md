# Comparing `tmp/tidy3d-2.7.0rc1.tar.gz` & `tmp/tidy3d-2.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.7.0rc1.tar", max compression
+gzip compressed data, was "tidy3d-2.7.0rc2.tar", max compression
```

## Comparing `tidy3d-2.7.0rc1.tar` & `tidy3d-2.7.0rc2.tar`

### file list

```diff
@@ -1,184 +1,195 @@
--rw-r--r--   0        0        0    26526 2024-04-22 21:06:22.038784 tidy3d-2.7.0rc1/LICENSE
--rw-r--r--   0        0        0     4867 2024-04-22 21:06:22.038784 tidy3d-2.7.0rc1/README.md
--rw-r--r--   0        0        0     7174 2024-04-22 21:06:22.090783 tidy3d-2.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2978 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/README.md
--rw-r--r--   0        0        0    12776 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/__init__.py
--rw-r--r--   0        0        0     3085 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/__main__.py
--rw-r--r--   0        0        0    10303 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/components/README.md
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/components/__init__.py
--rw-r--r--   0        0        0     3228 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/components/apodization.py
--rw-r--r--   0        0        0    37727 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/components/base.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/components/base_sim/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/components/base_sim/data/__init__.py
--rw-r--r--   0        0        0      666 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/components/base_sim/data/monitor_data.py
--rw-r--r--   0        0        0     4710 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/components/base_sim/data/sim_data.py
--rw-r--r--   0        0        0     3061 2024-04-22 21:06:22.098783 tidy3d-2.7.0rc1/tidy3d/components/base_sim/monitor.py
--rw-r--r--   0        0        0    23738 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/base_sim/simulation.py
--rw-r--r--   0        0        0      633 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/base_sim/source.py
--rw-r--r--   0        0        0     3211 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/bc_placement.py
--rw-r--r--   0        0        0    33071 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/boundary.py
--rw-r--r--   0        0        0     9733 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/data/README.md
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/data/__init__.py
--rw-r--r--   0        0        0    27766 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/data/data_array.py
--rw-r--r--   0        0        0   102019 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/data/dataset.py
--rw-r--r--   0        0        0   105030 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/data/monitor_data.py
--rw-r--r--   0        0        0    32494 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/data/sim_data.py
--rw-r--r--   0        0        0     2344 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/data/validators.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/eme/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/eme/data/__init__.py
--rw-r--r--   0        0        0     4343 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/eme/data/dataset.py
--rw-r--r--   0        0        0     1404 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/eme/data/monitor_data.py
--rw-r--r--   0        0        0    12601 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/eme/data/sim_data.py
--rw-r--r--   0        0        0    19597 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/eme/grid.py
--rw-r--r--   0        0        0     8711 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/eme/monitor.py
--rw-r--r--   0        0        0    39773 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/eme/simulation.py
--rw-r--r--   0        0        0     1590 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/eme/sweep.py
--rw-r--r--   0        0        0    38186 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/field_projection.py
--rw-r--r--   0        0        0      823 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/file_util.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/geometry/__init__.py
--rw-r--r--   0        0        0   104460 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/geometry/base.py
--rw-r--r--   0        0        0    17260 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/geometry/mesh.py
--rw-r--r--   0        0        0    62537 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/geometry/polyslab.py
--rw-r--r--   0        0        0    23366 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/geometry/primitives.py
--rw-r--r--   0        0        0     4013 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/geometry/triangulation.py
--rw-r--r--   0        0        0     7648 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/geometry/utils.py
--rw-r--r--   0        0        0     9140 2024-04-22 21:06:22.102783 tidy3d-2.7.0rc1/tidy3d/components/geometry/utils_2d.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/grid/__init__.py
--rw-r--r--   0        0        0    21892 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/grid/grid.py
--rw-r--r--   0        0        0    28045 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0        0        0    50912 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/grid/mesher.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/__init__.py
--rw-r--r--   0        0        0     2340 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/boundary.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/data/__init__.py
--rw-r--r--   0        0        0     3807 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/data/monitor_data.py
--rw-r--r--   0        0        0    10737 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/data/sim_data.py
--rw-r--r--   0        0        0     3871 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/grid.py
--rw-r--r--   0        0        0     1629 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/monitor.py
--rw-r--r--   0        0        0    35943 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/simulation.py
--rw-r--r--   0        0        0     1579 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/source.py
--rw-r--r--   0        0        0      347 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat/viz.py
--rw-r--r--   0        0        0     1135 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/heat_spec.py
--rw-r--r--   0        0        0     5451 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/lumped_element.py
--rw-r--r--   0        0        0   216885 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/medium.py
--rw-r--r--   0        0        0     9497 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/mode.py
--rw-r--r--   0        0        0    60115 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/monitor.py
--rw-r--r--   0        0        0    39999 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/parameter_perturbation.py
--rw-r--r--   0        0        0    53836 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/scene.py
--rw-r--r--   0        0        0   180638 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/simulation.py
--rw-r--r--   0        0        0    42829 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/source.py
--rw-r--r--   0        0        0    18102 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/structure.py
--rw-r--r--   0        0        0     7081 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/time.py
--rw-r--r--   0        0        0    10164 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/time_modulation.py
--rw-r--r--   0        0        0     3562 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/transformation.py
--rw-r--r--   0        0        0     7251 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/types.py
--rw-r--r--   0        0        0      362 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/types_extra.py
--rw-r--r--   0        0        0    15509 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/validators.py
--rw-r--r--   0        0        0    12760 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/components/viz.py
--rw-r--r--   0        0        0     1621 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/config.py
--rw-r--r--   0        0        0     3033 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/constants.py
--rw-r--r--   0        0        0     1265 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/exceptions.py
--rw-r--r--   0        0        0    15149 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/log.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.106783 tidy3d-2.7.0rc1/tidy3d/material_library/__init__.py
--rw-r--r--   0        0        0    73628 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/material_library/material_library.py
--rw-r--r--   0        0        0     9842 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/material_library/material_reference.py
--rw-r--r--   0        0        0    15924 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/material_library/parametric_materials.py
--rw-r--r--   0        0        0     5708 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/packaging.py
--rw-r--r--   0        0        0       77 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/__init__.py
--rw-r--r--   0        0        0    33133 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/README.md
--rw-r--r--   0        0        0     1416 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/__init__.py
--rw-r--r--   0        0        0      898 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0        0        0    11473 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/base.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0        0        0    19097 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0        0        0     1049 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0        0        0    18811 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0        0        0    11881 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0        0        0    26241 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0        0        0    16979 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0        0        0    35632 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0        0        0     8930 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0        0        0     2093 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/utils/__init__.py
--rw-r--r--   0        0        0     8126 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/utils/filter.py
--rw-r--r--   0        0        0    10079 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/utils/penalty.py
--rw-r--r--   0        0        0    29879 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/web.py
--rw-r--r--   0        0        0     6401 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/design/README.md
--rw-r--r--   0        0        0      441 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/design/__init__.py
--rw-r--r--   0        0        0     6596 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/design/design.py
--rw-r--r--   0        0        0    14226 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/design/method.py
--rw-r--r--   0        0        0     7087 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/design/parameter.py
--rw-r--r--   0        0        0    11780 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/design/result.py
--rw-r--r--   0        0        0      366 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0        0        0    22651 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0        0        0    33833 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/dispersion/fit_fast.py
--rw-r--r--   0        0        0      213 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/dispersion/fit_web.py
--rw-r--r--   0        0        0    13282 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/dispersion/web.py
--rw-r--r--   0        0        0      395 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/microwave/__init__.py
--rw-r--r--   0        0        0     3287 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/microwave/impedance_calculator.py
--rw-r--r--   0        0        0      159 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/microwave/models/__init__.py
--rw-r--r--   0        0        0     4130 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/microwave/models/coupled_microstrip.py
--rw-r--r--   0        0        0     4795 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/microwave/models/microstrip.py
--rw-r--r--   0        0        0    13499 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/microwave/path_integrals.py
--rw-r--r--   0        0        0     1213 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/mode/LICENSE
--rw-r--r--   0        0        0       42 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/mode/README.md
--rw-r--r--   0        0        0      138 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0        0        0     5733 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0        0        0    42914 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0        0        0    33294 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/mode/solver.py
--rw-r--r--   0        0        0     4370 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/mode/transforms.py
--rw-r--r--   0        0        0       81 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/mode/web.py
--rw-r--r--   0        0        0      116 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0        0        0     2705 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/polyslab/polyslab.py
--rw-r--r--   0        0        0      117 2024-04-22 21:06:22.110783 tidy3d-2.7.0rc1/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0        0        0    17644 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/resonance/resonance.py
--rw-r--r--   0        0        0      526 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0        0        0     8698 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/component_modelers/base.py
--rw-r--r--   0        0        0    15613 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/component_modelers/modal.py
--rw-r--r--   0        0        0    16530 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/component_modelers/terminal.py
--rw-r--r--   0        0        0     6457 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/ports/lumped.py
--rw-r--r--   0        0        0     1605 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/ports/modal.py
--rw-r--r--   0        0        0      212 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/smatrix.py
--rw-r--r--   0        0        0      129 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0        0        0    36178 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0        0        0   549925 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/schema.json
--rw-r--r--   0        0        0    10908 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/updater.py
--rw-r--r--   0        0        0       90 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/version.py
--rw-r--r--   0        0        0     1232 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/web/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/web/api/__init__.py
--rw-r--r--   0        0        0     2773 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/web/api/asynchronous.py
--rw-r--r--   0        0        0   275233 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/web/api/cacert.pem
--rw-r--r--   0        0        0     2284 2024-04-22 21:06:22.114783 tidy3d-2.7.0rc1/tidy3d/web/api/connect_util.py
--rw-r--r--   0        0        0    28521 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/api/container.py
--rw-r--r--   0        0        0     3792 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/api/material_fitter.py
--rw-r--r--   0        0        0     1449 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/api/material_libray.py
--rw-r--r--   0        0        0    18711 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/api/mode.py
--rw-r--r--   0        0        0     8933 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/api/tidy3d_stub.py
--rw-r--r--   0        0        0    33124 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/api/webapi.py
--rw-r--r--   0        0        0       88 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/__init__.py
--rw-r--r--   0        0        0     3491 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/app.py
--rw-r--r--   0        0        0      348 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/constants.py
--rw-r--r--   0        0        0    63715 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/converter.py
--rw-r--r--   0        0        0     1949 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/develop/__init__.py
--rw-r--r--   0        0        0    12380 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/develop/documentation.py
--rw-r--r--   0        0        0      400 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/develop/index.py
--rw-r--r--   0        0        0    15383 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/develop/install.py
--rw-r--r--   0        0        0     4159 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/develop/packaging.py
--rw-r--r--   0        0        0     1961 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/develop/tests.py
--rw-r--r--   0        0        0     1700 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/develop/utils.py
--rw-r--r--   0        0        0     3590 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/migrate.py
--rw-r--r--   0        0        0     3959 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/cli/readme.md
--rw-r--r--   0        0        0       35 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/__init__.py
--rw-r--r--   0        0        0       58 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/cache.py
--rw-r--r--   0        0        0      754 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/constants.py
--rw-r--r--   0        0        0      940 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/core_config.py
--rw-r--r--   0        0        0     4982 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/environment.py
--rw-r--r--   0        0        0      331 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/exceptions.py
--rw-r--r--   0        0        0     2235 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/file_util.py
--rw-r--r--   0        0        0     5917 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/http_util.py
--rw-r--r--   0        0        0    12450 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/s3utils.py
--rw-r--r--   0        0        0     2243 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/stub.py
--rw-r--r--   0        0        0    18838 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/task_core.py
--rw-r--r--   0        0        0     2188 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/task_info.py
--rw-r--r--   0        0        0     1451 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/core/types.py
--rw-r--r--   0        0        0      132 2024-04-22 21:06:22.118783 tidy3d-2.7.0rc1/tidy3d/web/environment.py
--rw-r--r--   0        0        0     9233 1970-01-01 00:00:00.000000 tidy3d-2.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-05-14 14:56:57.602419 tidy3d-2.7.0rc2/LICENSE
+-rw-r--r--   0        0        0     4867 2024-05-14 14:56:57.602419 tidy3d-2.7.0rc2/README.md
+-rw-r--r--   0        0        0     7124 2024-05-14 14:56:57.658419 tidy3d-2.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2978 2024-05-14 14:56:57.666419 tidy3d-2.7.0rc2/tidy3d/README.md
+-rw-r--r--   0        0        0    12861 2024-05-14 14:56:57.666419 tidy3d-2.7.0rc2/tidy3d/__init__.py
+-rw-r--r--   0        0        0     3085 2024-05-14 14:56:57.666419 tidy3d-2.7.0rc2/tidy3d/__main__.py
+-rw-r--r--   0        0        0    10303 2024-05-14 14:56:57.666419 tidy3d-2.7.0rc2/tidy3d/components/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.666419 tidy3d-2.7.0rc2/tidy3d/components/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-14 14:56:57.666419 tidy3d-2.7.0rc2/tidy3d/components/apodization.py
+-rw-r--r--   0        0        0    38447 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/base.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/base_sim/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/base_sim/data/__init__.py
+-rw-r--r--   0        0        0      666 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/base_sim/data/monitor_data.py
+-rw-r--r--   0        0        0     4710 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/base_sim/data/sim_data.py
+-rw-r--r--   0        0        0     3061 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/base_sim/monitor.py
+-rw-r--r--   0        0        0    23738 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/base_sim/simulation.py
+-rw-r--r--   0        0        0      633 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/base_sim/source.py
+-rw-r--r--   0        0        0     3211 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/bc_placement.py
+-rw-r--r--   0        0        0    33071 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/boundary.py
+-rw-r--r--   0        0        0     9733 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/data/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/data/__init__.py
+-rw-r--r--   0        0        0    29623 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/data/data_array.py
+-rw-r--r--   0        0        0   109527 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/data/dataset.py
+-rw-r--r--   0        0        0   105030 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0        0        0    32494 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/data/sim_data.py
+-rw-r--r--   0        0        0     2344 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/data/validators.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/eme/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/eme/data/__init__.py
+-rw-r--r--   0        0        0     4343 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/eme/data/dataset.py
+-rw-r--r--   0        0        0     1404 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/eme/data/monitor_data.py
+-rw-r--r--   0        0        0    12601 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/eme/data/sim_data.py
+-rw-r--r--   0        0        0    19597 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/eme/grid.py
+-rw-r--r--   0        0        0     8711 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/eme/monitor.py
+-rw-r--r--   0        0        0    39778 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/eme/simulation.py
+-rw-r--r--   0        0        0     1590 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/eme/sweep.py
+-rw-r--r--   0        0        0    38186 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/field_projection.py
+-rw-r--r--   0        0        0      823 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/file_util.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.670419 tidy3d-2.7.0rc2/tidy3d/components/geometry/__init__.py
+-rw-r--r--   0        0        0   111774 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/geometry/base.py
+-rw-r--r--   0        0        0    17324 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/geometry/mesh.py
+-rw-r--r--   0        0        0    63025 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/geometry/polyslab.py
+-rw-r--r--   0        0        0    24016 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/geometry/primitives.py
+-rw-r--r--   0        0        0     4013 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/geometry/triangulation.py
+-rw-r--r--   0        0        0     7648 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/geometry/utils.py
+-rw-r--r--   0        0        0     8047 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/geometry/utils_2d.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/grid/__init__.py
+-rw-r--r--   0        0        0    21787 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/grid/grid.py
+-rw-r--r--   0        0        0    28045 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0        0        0    50912 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/grid/mesher.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/__init__.py
+-rw-r--r--   0        0        0     2445 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/boundary.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/data/__init__.py
+-rw-r--r--   0        0        0     6153 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/data/monitor_data.py
+-rw-r--r--   0        0        0    10737 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/data/sim_data.py
+-rw-r--r--   0        0        0     4270 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/grid.py
+-rw-r--r--   0        0        0     1629 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/monitor.py
+-rw-r--r--   0        0        0    38526 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/simulation.py
+-rw-r--r--   0        0        0     1579 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/source.py
+-rw-r--r--   0        0        0      347 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat/viz.py
+-rw-r--r--   0        0        0     1135 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/heat_spec.py
+-rw-r--r--   0        0        0     5451 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/lumped_element.py
+-rw-r--r--   0        0        0   221199 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/medium.py
+-rw-r--r--   0        0        0     9497 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/mode.py
+-rw-r--r--   0        0        0    60115 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/monitor.py
+-rw-r--r--   0        0        0    39999 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/parameter_perturbation.py
+-rw-r--r--   0        0        0     1590 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/run_time_spec.py
+-rw-r--r--   0        0        0    53836 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/scene.py
+-rw-r--r--   0        0        0   187749 2024-05-14 14:56:57.674419 tidy3d-2.7.0rc2/tidy3d/components/simulation.py
+-rw-r--r--   0        0        0    44351 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/components/source.py
+-rw-r--r--   0        0        0    18102 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/components/structure.py
+-rw-r--r--   0        0        0     7081 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/components/time.py
+-rw-r--r--   0        0        0    10164 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/components/time_modulation.py
+-rw-r--r--   0        0        0     3562 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/components/transformation.py
+-rw-r--r--   0        0        0     7251 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/components/types.py
+-rw-r--r--   0        0        0      362 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/components/types_extra.py
+-rw-r--r--   0        0        0    15509 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/components/validators.py
+-rw-r--r--   0        0        0    12768 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/components/viz.py
+-rw-r--r--   0        0        0     1621 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/config.py
+-rw-r--r--   0        0        0     3033 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/constants.py
+-rw-r--r--   0        0        0     1265 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/exceptions.py
+-rw-r--r--   0        0        0    15149 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/log.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/material_library/__init__.py
+-rw-r--r--   0        0        0    73628 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/material_library/material_library.py
+-rw-r--r--   0        0        0     9842 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/material_library/material_reference.py
+-rw-r--r--   0        0        0    15924 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/material_library/parametric_materials.py
+-rw-r--r--   0        0        0     5708 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/packaging.py
+-rw-r--r--   0        0        0       77 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/__init__.py
+-rw-r--r--   0        0        0    33133 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/README.md
+-rw-r--r--   0        0        0     1438 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/__init__.py
+-rw-r--r--   0        0        0      944 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0        0        0    11473 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/base.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0        0        0    20677 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0        0        0     1049 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0        0        0    18811 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0        0        0    11881 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0        0        0    40067 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0        0        0    16979 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0        0        0    40048 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0        0        0     8930 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0        0        0     2093 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/utils/__init__.py
+-rw-r--r--   0        0        0     8126 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/utils/filter.py
+-rw-r--r--   0        0        0    10136 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/utils/penalty.py
+-rw-r--r--   0        0        0    30489 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/web.py
+-rw-r--r--   0        0        0     6401 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/design/README.md
+-rw-r--r--   0        0        0      441 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/design/__init__.py
+-rw-r--r--   0        0        0     6596 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/design/design.py
+-rw-r--r--   0        0        0    14226 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/design/method.py
+-rw-r--r--   0        0        0     7087 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/design/parameter.py
+-rw-r--r--   0        0        0    11780 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/design/result.py
+-rw-r--r--   0        0        0      366 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0        0        0    25156 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0        0        0    36179 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/dispersion/fit_fast.py
+-rw-r--r--   0        0        0      213 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/dispersion/fit_web.py
+-rw-r--r--   0        0        0    13282 2024-05-14 14:56:57.678419 tidy3d-2.7.0rc2/tidy3d/plugins/dispersion/web.py
+-rw-r--r--   0        0        0    22958 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/README.md
+-rw-r--r--   0        0        0      525 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/__init__.py
+-rw-r--r--   0        0        0     3295 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/base.py
+-rw-r--r--   0        0        0    11778 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/design.py
+-rw-r--r--   0        0        0     8329 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/optimizer.py
+-rw-r--r--   0        0        0     2680 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/penalty.py
+-rw-r--r--   0        0        0    11442 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/region.py
+-rw-r--r--   0        0        0     4964 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/result.py
+-rw-r--r--   0        0        0     3048 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/transformation.py
+-rw-r--r--   0        0        0     2286 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/utils.py
+-rw-r--r--   0        0        0     2587 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/invdes/validators.py
+-rw-r--r--   0        0        0      395 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/microwave/__init__.py
+-rw-r--r--   0        0        0     3287 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/microwave/impedance_calculator.py
+-rw-r--r--   0        0        0      159 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/microwave/models/__init__.py
+-rw-r--r--   0        0        0     4130 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/microwave/models/coupled_microstrip.py
+-rw-r--r--   0        0        0     4795 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/microwave/models/microstrip.py
+-rw-r--r--   0        0        0    13499 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/microwave/path_integrals.py
+-rw-r--r--   0        0        0     1213 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/mode/LICENSE
+-rw-r--r--   0        0        0       42 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/mode/README.md
+-rw-r--r--   0        0        0      138 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0        0        0     8452 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0        0        0    42914 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0        0        0    34531 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0        0        0     4370 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/mode/transforms.py
+-rw-r--r--   0        0        0       81 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/mode/web.py
+-rw-r--r--   0        0        0      116 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0        0        0     2705 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/polyslab/polyslab.py
+-rw-r--r--   0        0        0      117 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0        0        0    17644 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/resonance/resonance.py
+-rw-r--r--   0        0        0      526 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0        0        0     9648 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/component_modelers/base.py
+-rw-r--r--   0        0        0    15613 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/component_modelers/modal.py
+-rw-r--r--   0        0        0    16530 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/component_modelers/terminal.py
+-rw-r--r--   0        0        0     6457 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/ports/lumped.py
+-rw-r--r--   0        0        0     1605 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/ports/modal.py
+-rw-r--r--   0        0        0      212 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/smatrix.py
+-rw-r--r--   0        0        0      129 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0        0        0    36178 2024-05-14 14:56:57.682419 tidy3d-2.7.0rc2/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0        0        0   685547 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/schema.json
+-rw-r--r--   0        0        0    10944 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/updater.py
+-rw-r--r--   0        0        0       90 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/version.py
+-rw-r--r--   0        0        0     1232 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/__init__.py
+-rw-r--r--   0        0        0     2773 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/asynchronous.py
+-rw-r--r--   0        0        0   275233 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/cacert.pem
+-rw-r--r--   0        0        0     2284 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/connect_util.py
+-rw-r--r--   0        0        0    33010 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/container.py
+-rw-r--r--   0        0        0     3792 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/material_fitter.py
+-rw-r--r--   0        0        0     1449 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/material_libray.py
+-rw-r--r--   0        0        0    18711 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/mode.py
+-rw-r--r--   0        0        0     8933 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/tidy3d_stub.py
+-rw-r--r--   0        0        0    31912 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/api/webapi.py
+-rw-r--r--   0        0        0       88 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/__init__.py
+-rw-r--r--   0        0        0     3592 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/app.py
+-rw-r--r--   0        0        0      348 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/constants.py
+-rw-r--r--   0        0        0     1949 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/develop/__init__.py
+-rw-r--r--   0        0        0    12380 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/develop/documentation.py
+-rw-r--r--   0        0        0      400 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/develop/index.py
+-rw-r--r--   0        0        0    15383 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/develop/install.py
+-rw-r--r--   0        0        0     4159 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/develop/packaging.py
+-rw-r--r--   0        0        0     1961 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/develop/tests.py
+-rw-r--r--   0        0        0     1700 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/develop/utils.py
+-rw-r--r--   0        0        0     3590 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/migrate.py
+-rw-r--r--   0        0        0     3959 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/cli/readme.md
+-rw-r--r--   0        0        0       35 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/__init__.py
+-rw-r--r--   0        0        0       58 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/cache.py
+-rw-r--r--   0        0        0      754 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/constants.py
+-rw-r--r--   0        0        0      940 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/core_config.py
+-rw-r--r--   0        0        0     4982 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/environment.py
+-rw-r--r--   0        0        0      331 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/exceptions.py
+-rw-r--r--   0        0        0     2235 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/file_util.py
+-rw-r--r--   0        0        0     5917 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/http_util.py
+-rw-r--r--   0        0        0    12450 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/s3utils.py
+-rw-r--r--   0        0        0     2243 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/stub.py
+-rw-r--r--   0        0        0    18838 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/task_core.py
+-rw-r--r--   0        0        0     2188 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/task_info.py
+-rw-r--r--   0        0        0     1451 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/core/types.py
+-rw-r--r--   0        0        0      132 2024-05-14 14:56:57.686419 tidy3d-2.7.0rc2/tidy3d/web/environment.py
+-rw-r--r--   0        0        0     9278 1970-01-01 00:00:00.000000 tidy3d-2.7.0rc2/PKG-INFO
```

### Comparing `tidy3d-2.7.0rc1/LICENSE` & `tidy3d-2.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/README.md` & `tidy3d-2.7.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/pyproject.toml` & `tidy3d-2.7.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tidy3d"
-version = "2.7.0rc1"
+version = "2.7.0rc2"
 description = "A fast FDTD solver"
 authors = ["Tyler Hughes <tyler@flexcompute.com>"]
 license = "LGPLv2+"
 readme = "README.md"
 homepage = "https://github.com/flexcompute/tidy3d"
 repository = "https://github.com/flexcompute/tidy3d"
 classifiers = [
@@ -23,30 +23,31 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
 pyroots = ">=0.5.0"
 xarray = ">=0.16.2"
 importlib-metadata = ">=6.0.0"
 h5netcdf = "1.0.2"
 h5py = "^3.0.0"
-rich = "<12.6.0"
+rich = "^13.0"
 numpy = "<2"
 matplotlib = "*"
 shapely = "^2.0"
 pandas = "<=2.2.1"
 pydantic = "^2.0"
 PyYAML = "*"
 dask = "*"
 toml = "*"
 ### NOT CORE
 scipy = "*"
-boto3 = "1.28.*"
-requests = "2.31.*"
+boto3 = "^1.28.0"
+requests = "^2.31.0"
 pyjwt = "*"
-click = "8.1.*"
+click = "^8.1.0"
 responses = "*"
+joblib = "*"
 ### END NOT CORE
 
 ### Optional dependencies ###
 # development core
 bump-my-version =  {version="*", optional = true}
 black = {version="23.12.1", optional = true}
 coverage = {version="*", optional = true}
@@ -64,16 +65,16 @@
 # gdspy
 gdspy = {version="*", optional = true}
 
 # gdstk
 gdstk = {version=">=0.9.49", optional = true}
 
 # jax
-jaxlib = {version = "^0.4.13,<=0.4.26", source="jaxsource", optional = true}
-jax = {version = "^0.4.13,<=0.4.26", extras = ["cpu"], source="jaxsource", optional = true}
+jaxlib = {version = "0.4.25", source="jaxsource", optional = true}
+jax = {version = "0.4.25", extras = ["cpu"], source="jaxsource", optional = true}
 
 # trimesh
 networkx = {version = "^2.6.3", optional = true}
 rtree = {version = "1.2.0", optional = true}
 trimesh = {version = "^4", optional = true}
 
 # docs
@@ -93,15 +94,15 @@
 sphinx-notfound-page = {version="*", optional = true}
 sphinx-tabs = {version="*", optional = true}
 nbdime = {version="*", optional = true}
 myst-parser = {version="*", optional = true}
 optax = {version=">=0.2.2", optional = true}
 signac = {version="*", optional = true}
 flax = {version=">=0.8.2", optional = true}
-sax = {version="*", optional = true}
+sax = {version="^0.11", optional = true}
 vtk = {version=">=9.2.6", optional = true}
 pyswarms = {version="*", optional = true}
 sphinxemoji = {version="*", optional = true}
 devsim = {version="*", optional = true}
 cma = {version="*", optional = true}
 
 [tool.poetry.extras]
@@ -177,50 +178,49 @@
   "C",  # flake8-comprehensions
   "B",  # flake8-bugbear
   "UP",
   "NPY201", # numpy 2.* compatibility check
 ]
 
 [tool.bumpversion]
-current_version = "2.6.3"
+current_version = "2.7.0rc2"
 parse = """(?x)
     (?P<major>0|[1-9]\\d*)\\.
     (?P<minor>0|[1-9]\\d*)\\.
     (?P<patch>0|[1-9]\\d*)
     (?:
-        -                             # dash seperator for pre-release section
         (?P<pre_l>[a-zA-Z-]+)         # pre-release label
         (?P<pre_n>0|[1-9]\\d*)        # pre-release version number
     )?                                # pre-release section is optional
 """
 serialize = [
     "{major}.{minor}.{patch}{pre_l}{pre_n}",
     "{major}.{minor}.{patch}",
 ]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
-ignore_missing_version = false
+ignore_missing_version = true
 ignore_missing_files = false
 tag = false
 sign_tags = false
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 commit = false
 message = "Bump version: {current_version} → {new_version}"
 commit_args = ""
 
 [tool.bumpversion.parts.pre_l]
-values = ["dev", "rc"]
+values = ["rc", ""]
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
-search = "{current_version}"
-replace = "{new_version}"
+search = "\nversion = \"{current_version}\""
+replace = "\nversion = \"{new_version}\""
 
 [[tool.bumpversion.files]]
 filename = "tidy3d/version.py"
 search = "{current_version}"
 replace = "{new_version}"
 
 target-version = "py310"
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/README.md` & `tidy3d-2.7.0rc2/tidy3d/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/__init__.py` & `tidy3d-2.7.0rc2/tidy3d/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,19 +51,21 @@
 from .components.monitor import FieldProjectionAngleMonitor, FieldProjectionCartesianMonitor
 from .components.monitor import FieldProjectionKSpaceMonitor, FieldProjectionSurface
 from .components.monitor import DiffractionMonitor
 
 # lumped elements
 from .components.lumped_element import LumpedResistor
 
+# run time spec
+from .components.run_time_spec import RunTimeSpec
+
 # simulation
 from .components.simulation import Simulation
 
 # field projection
-
 from .components.field_projection import FieldProjector
 
 # data
 from .components.data.data_array import ScalarFieldDataArray, ScalarModeFieldDataArray
 from .components.data.data_array import ScalarFieldTimeDataArray, SpatialDataArray
 from .components.data.data_array import ModeAmpsDataArray, ModeIndexDataArray
 from .components.data.data_array import FluxDataArray, FluxTimeDataArray
@@ -239,14 +241,15 @@
     "ModeSolverMonitor",
     "PermittivityMonitor",
     "FieldProjectionAngleMonitor",
     "FieldProjectionCartesianMonitor",
     "FieldProjectionKSpaceMonitor",
     "FieldProjectionSurface",
     "DiffractionMonitor",
+    "RunTimeSpec",
     "Simulation",
     "FieldProjector",
     "ScalarFieldDataArray",
     "ScalarModeFieldDataArray",
     "ScalarFieldTimeDataArray",
     "SpatialDataArray",
     "ModeAmpsDataArray",
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/__main__.py` & `tidy3d-2.7.0rc2/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/README.md` & `tidy3d-2.7.0rc2/tidy3d/components/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/apodization.py` & `tidy3d-2.7.0rc2/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/base.py` & `tidy3d-2.7.0rc2/tidy3d/components/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from ..log import log
 
 
 INDENT_JSON_FILE = 4  # default indentation of json string in json files
 INDENT = None  # default indentation of json string used internally
 JSON_TAG = "JSON_STRING"
 # If json string is larger than ``MAX_STRING_LENGTH``, split the string when storing in hdf5
-MAX_STRING_LENGTH = 1e9
+MAX_STRING_LENGTH = 1_000_000_000
 FORBID_SPECIAL_CHARACTERS = ["/"]
 
 
 def cache(prop):
     """Decorates a property to cache the first computed value and return it on subsequent calls."""
 
     # note, we could also just use `prop` as dict key, but hashing property might be slow
@@ -188,14 +188,27 @@
             for character in FORBID_SPECIAL_CHARACTERS:
                 if character in name:
                     raise ValueError(
                         f"Special character '{character}' not allowed in component name {name}."
                     )
         return values
 
+    attrs: dict = pydantic.Field(
+        {},
+        title="Attributes",
+        description="Dictionary storing arbitrary metadata for a Tidy3D object. "
+        "This dictionary can be freely used by the user for storing data without affecting the "
+        "operation of Tidy3D as it is not used internally. "
+        "Note that, unlike regular Tidy3D fields, ``attrs`` are mutable. "
+        "For example, the following is allowed for setting an ``attr`` ``obj.attrs['foo'] = bar``. "
+        "Also note that `Tidy3D`` will raise a ``TypeError`` if ``attrs`` contain objects "
+        "that can not be serialized. One can check if ``attrs`` are serializable "
+        "by calling ``obj.json()``.",
+    )
+
     def copy(self, **kwargs) -> Tidy3dBaseModel:
         """Copy a Tidy3dBaseModel.  With ``deep=True`` as default."""
         if "deep" in kwargs and kwargs["deep"] is False:
             raise ValueError("Can't do shallow copy of component, set `deep=True` in copy().")
         kwargs.update(dict(deep=True))
         new_copy = pydantic.BaseModel.copy(self, **kwargs)
         return self.validate(new_copy.dict())
@@ -823,15 +836,15 @@
         return hash(self) <= hash(other)
 
     def __ge__(self, other):
         """define >= for getting unique indices based on hash."""
         return hash(self) >= hash(other)
 
     def __eq__(self, other):
-        """Define == for two Tidy3DBaseModels."""
+        """Define == for two Tidy3dBaseModels."""
         if other is None:
             return False
 
         def check_equal(dict1: dict, dict2: dict) -> bool:
             """Check if two dictionaries are equal, with special handlings."""
 
             # if different keys, automatically fail
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/base_sim/data/monitor_data.py` & `tidy3d-2.7.0rc2/tidy3d/components/base_sim/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/base_sim/data/sim_data.py` & `tidy3d-2.7.0rc2/tidy3d/components/base_sim/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/base_sim/monitor.py` & `tidy3d-2.7.0rc2/tidy3d/components/base_sim/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/base_sim/simulation.py` & `tidy3d-2.7.0rc2/tidy3d/components/base_sim/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/base_sim/source.py` & `tidy3d-2.7.0rc2/tidy3d/components/base_sim/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/bc_placement.py` & `tidy3d-2.7.0rc2/tidy3d/components/bc_placement.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/boundary.py` & `tidy3d-2.7.0rc2/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/data/README.md` & `tidy3d-2.7.0rc2/tidy3d/components/data/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/data/data_array.py` & `tidy3d-2.7.0rc2/tidy3d/components/data/data_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,20 @@
         return True
 
     @property
     def abs(self):
         """Absolute value of data array."""
         return abs(self)
 
+    @property
+    def is_uniform(self):
+        """Whether each element is of equal value in the data array"""
+        raw_data = self.data.ravel()
+        return np.allclose(raw_data, raw_data[0])
+
     def to_hdf5(self, fname: Union[str, h5py.File], group_path: str) -> None:
         """Save an xr.DataArray to the hdf5 file or file handle with a given path to the group."""
 
         # file name passed
         if isinstance(fname, str):
             with h5py.File(fname, "w") as f_handle:
                 self.to_hdf5_handle(f_handle=f_handle, group_path=group_path)
@@ -261,33 +267,55 @@
 class AbstractSpatialDataArray(DataArray, ABC):
     """Spatial distribution."""
 
     __slots__ = ()
     _dims = ("x", "y", "z")
     _data_attrs = {"long_name": "field value"}
 
+    @property
+    def _spatially_sorted(self) -> SpatialDataArray:
+        """Check whether sorted and sort if not."""
+        needs_sorting = []
+        for axis in "xyz":
+            axis_coords = self.coords[axis].values
+            if len(axis_coords) > 1 and np.any(axis_coords[1:] < axis_coords[:-1]):
+                needs_sorting.append(axis)
+
+        if len(needs_sorting) > 0:
+            return self.sortby(needs_sorting)
+
+        return self
+
     def sel_inside(self, bounds: Bound) -> SpatialDataArray:
         """Return a new SpatialDataArray that contains the minimal amount data necessary to cover
-        a spatial region defined by ``bounds``.
+        a spatial region defined by ``bounds``. Note that the returned data is sorted with respect
+        to spatial coordinates.
 
 
         Parameters
         ----------
         bounds : Tuple[float, float, float], Tuple[float, float float]
             Min and max bounds packaged as ``(minx, miny, minz), (maxx, maxy, maxz)``.
 
         Returns
         -------
         SpatialDataArray
             Extracted spatial data array.
         """
+        if any(bmin > bmax for bmin, bmax in zip(*bounds)):
+            raise DataError(
+                "Min and max bounds must be packaged as '(minx, miny, minz), (maxx, maxy, maxz)'."
+            )
+
+        # make sure data is sorted with respect to coordinates
+        sorted_self = self._spatially_sorted
 
         inds_list = []
 
-        coords = (self.x, self.y, self.z)
+        coords = (sorted_self.x, sorted_self.y, sorted_self.z)
 
         for coord, smin, smax in zip(coords, bounds[0], bounds[1]):
             length = len(coord)
 
             # one point along direction, assume invariance
             if length == 1:
                 comp_inds = [0]
@@ -312,15 +340,15 @@
                     else:
                         ind_max = (coord >= smax).argmax().data
 
                     comp_inds = np.arange(ind_min, ind_max + 1)
 
             inds_list.append(comp_inds)
 
-        return self.isel(x=inds_list[0], y=inds_list[1], z=inds_list[2])
+        return sorted_self.isel(x=inds_list[0], y=inds_list[1], z=inds_list[2])
 
     def does_cover(self, bounds: Bound) -> bool:
         """Check whether data fully covers specified by ``bounds`` spatial region. If data contains
         only one point along a given direction, then it is assumed the data is constant along that
         direction and coverage is not checked.
 
 
@@ -330,18 +358,22 @@
             Min and max bounds packaged as ``(minx, miny, minz), (maxx, maxy, maxz)``.
 
         Returns
         -------
         bool
             Full cover check outcome.
         """
+        if any(bmin > bmax for bmin, bmax in zip(*bounds)):
+            raise DataError(
+                "Min and max bounds must be packaged as '(minx, miny, minz), (maxx, maxy, maxz)'."
+            )
 
         coords = (self.x, self.y, self.z)
         return all(
-            (coord[0] <= smin and coord[-1] >= smax) or len(coord) == 1
+            (np.min(coord) <= smin and np.max(coord) >= smax) or len(coord) == 1
             for coord, smin, smax in zip(coords, bounds[0], bounds[1])
         )
 
 
 class SpatialDataArray(AbstractSpatialDataArray):
     """Spatial distribution.
 
@@ -352,41 +384,55 @@
     >>> z = [3,4,5,6]
     >>> coords = dict(x=x, y=y, z=z)
     >>> fd = SpatialDataArray((1+1j) * np.random.random((2,3,4)), coords=coords)
     """
 
     __slots__ = ()
 
-    def reflect(self, axis: Axis, center: float) -> SpatialDataArray:
+    def reflect(self, axis: Axis, center: float, reflection_only: bool = False) -> SpatialDataArray:
         """Reflect data across the plane define by parameters ``axis`` and ``center`` from right to
-        left.
+        left. Note that the returned data is sorted with respect to spatial coordinates.
 
         Parameters
         ----------
         axis : Literal[0, 1, 2]
             Normal direction of the reflection plane.
         center : float
             Location of the reflection plane along its normal direction.
+        reflection_only : bool = False
+            Return only reflected data.
 
         Returns
         -------
         SpatialDataArray
             Data after reflection is performed.
         """
 
-        coords = list(self.coords.values())
-        data = np.array(self.data)
+        sorted_self = self._spatially_sorted
+
+        coords = [sorted_self.x.values, sorted_self.y.values, sorted_self.z.values]
+        data = np.array(sorted_self.data)
+
+        data_left_bound = coords[axis][0]
 
-        if np.isclose(center, coords[axis].data[0]):
+        if np.isclose(center, data_left_bound):
             num_duplicates = 1
-        elif center > coords[axis].data[0]:
-            raise DataError("Reflection center must be outside and on the left of the data region.")
+        elif center > data_left_bound:
+            raise DataError("Reflection center must be outside and to the left of the data region.")
         else:
             num_duplicates = 0
 
+        if reflection_only:
+            coords[axis] = 2 * center - coords[axis]
+            coords_dict = dict(zip("xyz", coords))
+
+            tmp_arr = SpatialDataArray(sorted_self.data, coords=coords_dict)
+
+            return tmp_arr.sortby("xyz"[axis])
+
         shape = np.array(np.shape(data))
         old_len = shape[axis]
         shape[axis] = 2 * old_len - num_duplicates
 
         ind_left = [slice(shape[0]), slice(shape[1]), slice(shape[2])]
         ind_right = [slice(shape[0]), slice(shape[1]), slice(shape[2])]
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/data/dataset.py` & `tidy3d-2.7.0rc2/tidy3d/components/data/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -546,22 +546,58 @@
         return np.iscomplexobj(self.values)
 
     @property
     def _double_type(self):
         """Corresponding double data type."""
         return np.complex128 if self.is_complex else np.float64
 
-    @pd.validator("cells", always=True)
-    def match_cells_to_vtk_type(cls, val):
-        """Check that cell connections does not have duplicate points."""
-        if vtk is None:
-            return val
+    @pd.validator("points", always=True)
+    def points_right_dims(cls, val):
+        """Check that point coordinates have the right dimensionality."""
+        # currently support only the standard axis ordering, that is 01(2)
+        axis_coords_expected = np.arange(cls._point_dims())
+        axis_coords_given = val.axis.data
+        if np.any(axis_coords_given != axis_coords_expected):
+            raise ValidationError(
+                f"Points array is expected to have {axis_coords_expected} coord values along 'axis'"
+                f" (given: {axis_coords_given})."
+            )
+        return val
 
-        # using val.astype(np.int32/64) directly causes issues when dataarray are later checked ==
-        return CellDataArray(val.data.astype(vtk["id_type"], copy=False), coords=val.coords)
+    @property
+    def is_uniform(self):
+        """Whether each element is of equal value in ``values``."""
+        return self.values.is_uniform
+
+    @pd.validator("points", always=True)
+    def points_right_indexing(cls, val):
+        """Check that points are indexed corrrectly."""
+        indices_expected = np.arange(len(val.data))
+        indices_given = val.index.data
+        if np.any(indices_expected != indices_given):
+            raise ValidationError(
+                "Coordinate 'index' of array 'points' is expected to have values (0, 1, 2, ...). "
+                "This can be easily achieved, for example, by using "
+                "PointDataArray(data, dims=['index', 'axis'])."
+            )
+        return val
+
+    @pd.validator("values", always=True)
+    def values_right_indexing(cls, val):
+        """Check that data values are indexed correctly."""
+        # currently support only simple ordered indexing of points, that is, 0, 1, 2, ...
+        indices_expected = np.arange(len(val.data))
+        indices_given = val.index.data
+        if np.any(indices_expected != indices_given):
+            raise ValidationError(
+                "Coordinate 'index' of array 'values' is expected to have values (0, 1, 2, ...). "
+                "This can be easily achieved, for example, by using "
+                "IndexedDataArray(data, dims=['index'])."
+            )
+        return val
 
     @pd.validator("values", always=True)
     @skip_if_fields_missing(["points"])
     def number_of_values_matches_points(cls, val, values):
         """Check that the number of data values matches the number of grid points."""
         num_values = len(val)
 
@@ -571,29 +607,27 @@
         if num_points != num_values:
             raise ValidationError(
                 f"The number of data values ({num_values}) does not match the number of grid "
                 f"points ({num_points})."
             )
         return val
 
-    @pd.validator("points", always=True)
-    def points_right_dims(cls, val):
-        """Check that point coordinates have the right dimensionality."""
-        axis_coords_expected = np.arange(cls._point_dims())
-        axis_coords_given = val.axis.data
-        if np.any(axis_coords_given != axis_coords_expected):
-            raise ValidationError(
-                f"Points array is expected to have {axis_coords_expected} coord values along 'axis'"
-                f" (given: {axis_coords_given})."
-            )
-        return val
+    @pd.validator("cells", always=True)
+    def match_cells_to_vtk_type(cls, val):
+        """Check that cell connections does not have duplicate points."""
+        if vtk is None:
+            return val
+
+        # using val.astype(np.int32/64) directly causes issues when dataarray are later checked ==
+        return CellDataArray(val.data.astype(vtk["id_type"], copy=False), coords=val.coords)
 
     @pd.validator("cells", always=True)
     def cells_right_type(cls, val):
         """Check that cell are of the right type."""
+        # only supporting the standard ordering of cell vertices 012(3)
         vertex_coords_expected = np.arange(cls._cell_num_vertices())
         vertex_coords_given = val.vertex_index.data
         if np.any(vertex_coords_given != vertex_coords_expected):
             raise ValidationError(
                 f"Cell connections array is expected to have {vertex_coords_expected} coord values"
                 f" along 'vertex_index' (given: {vertex_coords_given})."
             )
@@ -608,32 +642,103 @@
         if len(all_point_indices_used) > 0:
             min_index_used = np.min(all_point_indices_used)
             max_index_used = np.max(all_point_indices_used)
 
             points = values.get("points")
             num_points = len(points)
 
-            if max_index_used != num_points - 1 or min_index_used != 0:
+            if max_index_used > num_points - 1 or min_index_used < 0:
                 raise ValidationError(
                     "Cell connections array uses undefined point indices in the range "
                     f"[{min_index_used}, {max_index_used}]. The valid range of point indices is "
                     f"[0, {num_points-1}]."
                 )
         return val
 
-    @pd.validator("cells", always=True)
-    def check_valid_cells(cls, val):
-        """Check that cell connections does not have duplicate points."""
-        indices = val.data
+    @classmethod
+    def _find_degenerate_cells(cls, cells: CellDataArray):
+        """Find explicitly degenerate cells if any.
+        That is, cells that use the same point indices for their different vertices.
+        """
+        indices = cells.data
         # skip validation if zero size data
+        degenerate_cell_inds = set()
         if len(indices) > 0:
             for i in range(cls._cell_num_vertices() - 1):
                 for j in range(i + 1, cls._cell_num_vertices()):
-                    if np.any(indices[:, i] == indices[:, j]):
-                        log.warning("Unstructured grid contains degenerate cells.")
+                    degenerate_cell_inds = degenerate_cell_inds.union(
+                        np.where(indices[:, i] == indices[:, j])[0]
+                    )
+
+        return degenerate_cell_inds
+
+    @classmethod
+    def _remove_degenerate_cells(cls, cells: CellDataArray):
+        """Remove explicitly degenerate cells if any.
+        That is, cells that use the same point indices for their different vertices.
+        """
+        degenerate_cells = cls._find_degenerate_cells(cells=cells)
+        if len(degenerate_cells) > 0:
+            data = np.delete(cells.values, list(degenerate_cells), axis=0)
+            cell_index = np.delete(cells.cell_index.values, list(degenerate_cells))
+            return CellDataArray(
+                data=data, coords=dict(cell_index=cell_index, vertex_index=cells.vertex_index)
+            )
+        return cells
+
+    @classmethod
+    def _remove_unused_points(
+        cls, points: PointDataArray, values: IndexedDataArray, cells: CellDataArray
+    ):
+        """Remove unused points if any.
+        That is, points that are not used in any grid cell.
+        """
+
+        used_indices = np.unique(cells.values.ravel())
+        num_points = len(points)
+
+        if len(used_indices) != num_points or np.any(np.diff(used_indices) != 1):
+            min_index = np.min(used_indices)
+            map_len = np.max(used_indices) - min_index + 1
+            index_map = np.zeros(map_len)
+            index_map[used_indices - min_index] = np.arange(len(used_indices))
+
+            cells = CellDataArray(data=index_map[cells.data - min_index], coords=cells.coords)
+            points = PointDataArray(points.data[used_indices, :], dims=["index", "axis"])
+            values = IndexedDataArray(values.data[used_indices], dims=["index"])
+
+        return points, values, cells
+
+    def clean(self, remove_degenerate_cells=True, remove_unused_points=True):
+        """Remove degenerate cells and/or unused points."""
+        if remove_degenerate_cells:
+            cells = self._remove_degenerate_cells(cells=self.cells)
+        else:
+            cells = self.cells
+
+        if remove_unused_points:
+            points, values, cells = self._remove_unused_points(self.points, self.values, cells)
+        else:
+            points = self.points
+            values = self.values
+
+        return self.updated_copy(points=points, values=values, cells=cells)
+
+    @pd.validator("cells", always=True)
+    def warn_degenerate_cells(cls, val):
+        """Check that cell connections does not have duplicate points."""
+        degenerate_cells = cls._find_degenerate_cells(val)
+        num_degenerate_cells = len(degenerate_cells)
+        if num_degenerate_cells > 0:
+            log.warning(
+                f"Unstructured grid contains {num_degenerate_cells} degenerate cell(s). "
+                "Such cells can be removed by using function "
+                "'.clean(remove_degenerate_cells: bool = True, remove_unused_points: bool = True)'. "
+                "For example, 'dataset = dataset.clean()'."
+            )
         return val
 
     @pd.root_validator(pre=True, allow_reuse=True)
     def _warn_if_none(cls, values):
         """Warn if any of data arrays are not loaded."""
 
         no_data_fields = []
@@ -651,14 +756,28 @@
             )
             values["cells"] = CellDataArray(
                 np.zeros((0, cls._cell_num_vertices())), dims=["cell_index", "vertex_index"]
             )
             values["values"] = IndexedDataArray(np.zeros(0), dims=["index"])
         return values
 
+    @pd.root_validator(skip_on_failure=True, allow_reuse=True)
+    def _warn_unused_points(cls, values):
+        """Warn if some points are unused."""
+        point_indices = set(np.arange(len(values["values"].data)))
+        used_indices = set(values["cells"].values.ravel())
+
+        if not point_indices.issubset(used_indices):
+            log.warning(
+                "Unstructured grid dataset contains unused points. "
+                "Consider calling 'clean()' to remove them."
+            )
+
+        return values
+
     def rename(self, name: str) -> UnstructuredGridDataset:
         """Return a renamed array."""
         return self.updated_copy(values=self.values.rename(name))
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
         """Override of numpy functions."""
 
@@ -786,15 +905,18 @@
                 f"(extent along axis {axis}: {self.bounds[0][axis]}, {self.bounds[1][axis]})."
             )
 
         origin = [0, 0, 0]
         origin[axis] = pos
 
         normal = [0, 0, 0]
-        normal[axis] = 1
+        # orientation of normal is important for edge (literally) cases
+        normal[axis] = -1
+        if pos > (self.bounds[0][axis] + self.bounds[1][axis]) / 2:
+            normal[axis] = 1
 
         # create cutting plane
         plane = vtk["mod"].vtkPlane()
         plane.SetOrigin(origin[0], origin[1], origin[2])
         plane.SetNormal(normal[0], normal[1], normal[2])
 
         # create cutter
@@ -842,36 +964,57 @@
         grid = reader.GetOutput()
 
         return grid
 
     @classmethod
     @abstractmethod
     @requires_vtk
-    def _from_vtk_obj(cls, vtk_obj, field: str = None) -> UnstructuredGridDataset:
+    def _from_vtk_obj(
+        cls,
+        vtk_obj,
+        field: str = None,
+        remove_degenerate_cells: bool = False,
+        remove_unused_points: bool = False,
+    ) -> UnstructuredGridDataset:
         """Initialize from a vtk object."""
 
     @classmethod
     @requires_vtk
-    def from_vtu(cls, file: str, field: str = None) -> UnstructuredGridDataset:
+    def from_vtu(
+        cls,
+        file: str,
+        field: str = None,
+        remove_degenerate_cells: bool = False,
+        remove_unused_points: bool = False,
+    ) -> UnstructuredGridDataset:
         """Load unstructured data from a vtu file.
 
         Parameters
         ----------
         fname : str
             Full path to the .vtu file to load the unstructured data from.
         field : str = None
             Name of the field to load.
+        remove_degenerate_cells : bool = False
+            Remove explicitly degenerate cells.
+        remove_unused_points : bool = False
+            Remove unused points.
 
         Returns
         -------
         UnstructuredGridDataset
             Unstructured data.
         """
         grid = cls._read_vtkUnstructuredGrid(file)
-        return cls._from_vtk_obj(grid, field=field)
+        return cls._from_vtk_obj(
+            grid,
+            field=field,
+            remove_degenerate_cells=remove_degenerate_cells,
+            remove_unused_points=remove_unused_points,
+        )
 
     @requires_vtk
     def to_vtu(self, fname: str):
         """Exports unstructured grid data into a .vtu file.
 
         Parameters
         ----------
@@ -982,15 +1125,17 @@
         grid_cleaner.Update()
         clean_clip = grid_cleaner.GetOutput()
 
         # no intersection check
         if clean_clip.GetNumberOfPoints() == 0:
             raise DataError("Clipping box does not intersect the unstructured grid.")
 
-        return self._from_vtk_obj(clean_clip)
+        return self._from_vtk_obj(
+            clean_clip, remove_degenerate_cells=True, remove_unused_points=True
+        )
 
     def interp(
         self,
         x: Union[float, ArrayLike],
         y: Union[float, ArrayLike],
         z: Union[float, ArrayLike],
         fill_value: Union[float, Literal["extrapolate"]] = None,
@@ -1718,14 +1863,18 @@
             Min and max bounds packaged as ``(minx, miny, minz), (maxx, maxy, maxz)``.
 
         Returns
         -------
         UnstructuredGridDataset
             Extracted spatial data array.
         """
+        if any(bmin > bmax for bmin, bmax in zip(*bounds)):
+            raise DataError(
+                "Min and max bounds must be packaged as ``(minx, miny, minz), (maxx, maxy, maxz)``."
+            )
 
         data_bounds = self.bounds
         tol = 1e-6
 
         # For extracting cells covering target region we use vtk's filter that extract cells based
         # on provided implicit function. However, when we provide to it the implicit function of
         # the entire box, it has a couple of issues coming from the fact that the algorithm
@@ -1764,15 +1913,15 @@
                     extractor.SetImplicitFunction(plane)
                     extractor.ExtractInsideOn()
                     extractor.ExtractBoundaryCellsOn()
                     extractor.SetInputData(tmp)
                     extractor.Update()
                     tmp = extractor.GetOutput()
 
-        return self._from_vtk_obj(tmp)
+        return self._from_vtk_obj(tmp, remove_degenerate_cells=True, remove_unused_points=True)
 
     def does_cover(self, bounds: Bound) -> bool:
         """Check whether data fully covers specified by ``bounds`` spatial region. If data contains
         only one point along a given direction, then it is assumed the data is constant along that
         direction and coverage is not checked.
 
 
@@ -1902,15 +2051,21 @@
     @requires_vtk
     def _vtk_cell_type(cls):
         """VTK cell type to use in the VTK representation."""
         return vtk["mod"].VTK_TRIANGLE
 
     @classmethod
     @requires_vtk
-    def _from_vtk_obj(cls, vtk_obj, field=None):
+    def _from_vtk_obj(
+        cls,
+        vtk_obj,
+        field=None,
+        remove_degenerate_cells: bool = False,
+        remove_unused_points: bool = False,
+    ):
         """Initialize from a vtkUnstructuredGrid instance."""
 
         # get points cells data from vtk object
         if isinstance(vtk_obj, vtk["mod"].vtkPolyData):
             cells_vtk = vtk_obj.GetPolys()
         elif isinstance(vtk_obj, vtk["mod"].vtkUnstructuredGrid):
             cells_vtk = vtk_obj.GetCells()
@@ -1958,14 +2113,22 @@
         )
 
         points = PointDataArray(
             points_2d_numpy,
             coords=dict(index=np.arange(len(points_numpy)), axis=np.arange(cls._point_dims())),
         )
 
+        if remove_degenerate_cells:
+            cells = cls._remove_degenerate_cells(cells=cells)
+
+        if remove_unused_points:
+            points, values, cells = cls._remove_unused_points(
+                points=points, values=values, cells=cells
+            )
+
         return cls(
             normal_axis=normal_axis,
             normal_pos=normal_pos,
             points=points,
             cells=cells,
             values=values,
         )
@@ -2325,15 +2488,20 @@
         -------
         UnstructuredGridDataset
             Data after reflextion is performed.
         """
 
         # disallow reflecting along normal direction
         if axis == self.normal_axis:
-            raise DataError("Reflection in the normal direction to the grid is prohibited.")
+            if reflection_only:
+                return self.updated_copy(normal_pos=2 * center - self.normal_pos)
+            else:
+                raise DataError(
+                    "Reflection in the normal direction to the grid is prohibited unless 'reflection_only=True'."
+                )
 
         return super().reflect(axis=axis, center=center, reflection_only=reflection_only)
 
     @requires_vtk
     def sel_inside(self, bounds: Bound) -> TriangularGridDataset:
         """Return a new ``TriangularGridDataset`` that contains the minimal amount data necessary to
         cover a spatial region defined by ``bounds``.
@@ -2345,14 +2513,18 @@
             Min and max bounds packaged as ``(minx, miny, minz), (maxx, maxy, maxz)``.
 
         Returns
         -------
         TriangularGridDataset
             Extracted spatial data array.
         """
+        if any(bmin > bmax for bmin, bmax in zip(*bounds)):
+            raise DataError(
+                "Min and max bounds must be packaged as ``(minx, miny, minz), (maxx, maxy, maxz)``."
+            )
 
         # expand along normal direction
         new_bounds = [list(bounds[0]), list(bounds[1])]
 
         new_bounds[0][self.normal_axis] = -inf
         new_bounds[1][self.normal_axis] = inf
 
@@ -2436,15 +2608,21 @@
     @requires_vtk
     def _vtk_cell_type(cls):
         """VTK cell type to use in the VTK representation."""
         return vtk["mod"].VTK_TETRA
 
     @classmethod
     @requires_vtk
-    def _from_vtk_obj(cls, grid, field=None) -> TetrahedralGridDataset:
+    def _from_vtk_obj(
+        cls,
+        grid,
+        field=None,
+        remove_degenerate_cells: bool = False,
+        remove_unused_points: bool = False,
+    ) -> TetrahedralGridDataset:
         """Initialize from a vtkUnstructuredGrid instance."""
 
         # read point, cells, and values info from a vtk instance
         cells_numpy = vtk["vtk_to_numpy"](grid.GetCells().GetConnectivityArray())
         points_numpy = vtk["vtk_to_numpy"](grid.GetPoints().GetData())
         values = cls._get_values_from_vtk(grid, len(points_numpy), field)
 
@@ -2465,14 +2643,22 @@
         )
 
         points = PointDataArray(
             points_numpy,
             coords=dict(index=np.arange(len(points_numpy)), axis=np.arange(cls._point_dims())),
         )
 
+        if remove_degenerate_cells:
+            cells = cls._remove_degenerate_cells(cells=cells)
+
+        if remove_unused_points:
+            points, values, cells = cls._remove_unused_points(
+                points=points, values=values, cells=cells
+            )
+
         return cls(points=points, cells=cells, values=values)
 
     @requires_vtk
     def plane_slice(self, axis: Axis, pos: float) -> TriangularGridDataset:
         """Slice data with a plane and return the resulting :class:.`TriangularGridDataset`.
 
         Parameters
@@ -2486,15 +2672,17 @@
         -------
         TriangularGridDataset
             The resulting slice.
         """
 
         slice_vtk = self._plane_slice_raw(axis=axis, pos=pos)
 
-        return TriangularGridDataset._from_vtk_obj(slice_vtk)
+        return TriangularGridDataset._from_vtk_obj(
+            slice_vtk, remove_degenerate_cells=True, remove_unused_points=True
+        )
 
     @requires_vtk
     def line_slice(self, axis: Axis, pos: Coordinate) -> SpatialDataArray:
         """Slice data with a line and return the resulting :class:.`SpatialDataArray`.
 
         Parameters
         ----------
@@ -2535,15 +2723,17 @@
         prober.Update()
 
         extracted_cells_vtk = prober.GetOutput()
 
         if extracted_cells_vtk.GetNumberOfPoints() == 0:
             raise DataError("Slicing line does not intersect the unstructured grid.")
 
-        extracted_cells = TetrahedralGridDataset._from_vtk_obj(extracted_cells_vtk)
+        extracted_cells = TetrahedralGridDataset._from_vtk_obj(
+            extracted_cells_vtk, remove_degenerate_cells=True, remove_unused_points=True
+        )
 
         tan_dims = [0, 1, 2]
         tan_dims.remove(axis)
 
         # first plane slice
         plane_slice = extracted_cells.plane_slice(axis=tan_dims[0], pos=pos[tan_dims[0]])
         # second plane slice
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/data/monitor_data.py` & `tidy3d-2.7.0rc2/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/data/sim_data.py` & `tidy3d-2.7.0rc2/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/data/validators.py` & `tidy3d-2.7.0rc2/tidy3d/components/data/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/eme/data/dataset.py` & `tidy3d-2.7.0rc2/tidy3d/components/eme/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/eme/data/monitor_data.py` & `tidy3d-2.7.0rc2/tidy3d/components/eme/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/eme/data/sim_data.py` & `tidy3d-2.7.0rc2/tidy3d/components/eme/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/eme/grid.py` & `tidy3d-2.7.0rc2/tidy3d/components/eme/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/eme/monitor.py` & `tidy3d-2.7.0rc2/tidy3d/components/eme/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/eme/simulation.py` & `tidy3d-2.7.0rc2/tidy3d/components/eme/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         title="EME Sweep Specification",
         description="Specification for a parameter sweep to be performed during the EME "
         "propagation step. The results are stored "
         "in 'sim_data.smatrix'. Other simulation monitor data is not included in the sweep.",
     )
 
     constraint: Optional[Literal["passive", "unitary"]] = pd.Field(
-        None,
+        "passive",
         title="EME Constraint",
         description="Constraint for EME propagation, imposed at cell interfaces. "
         "A constraint of 'passive' means that energy can be dissipated but not created at "
         "interfaces. A constraint of 'unitary' means that energy is conserved at interfaces "
         "(but not necessarily within cells). The option 'none' may be faster "
         "for a large number of modes. The option 'passive' can serve as regularization "
         "for the field continuity requirement and give more physical results.",
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/eme/sweep.py` & `tidy3d-2.7.0rc2/tidy3d/components/eme/sweep.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/field_projection.py` & `tidy3d-2.7.0rc2/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/file_util.py` & `tidy3d-2.7.0rc2/tidy3d/components/file_util.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/geometry/base.py` & `tidy3d-2.7.0rc2/tidy3d/components/geometry/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,15 +364,22 @@
                 "Simulation domain (including PML)."
             )
         return (pt_min + pt_max) / 2.0
 
     @cached_property
     def _normal_2dmaterial(self) -> Axis:
         """Get the normal to the given geometry, checking that it is a 2D geometry."""
-        raise ValidationError("'Medium2D' is not conpatible with this geometry class.")
+        raise ValidationError("'Medium2D' is not compatible with this geometry class.")
+
+    def _update_from_bounds(self, bounds: Tuple[float, float], axis: Axis) -> Geometry:
+        """Returns an updated geometry which has been transformed to fit within ``bounds``
+        along the ``axis`` direction."""
+        raise NotImplementedError(
+            "'_update_from_bounds' is not compatible with this geometry class."
+        )
 
     @equal_aspect
     @add_ax_if_none
     def plot(
         self, x: float = None, y: float = None, z: float = None, ax: Ax = None, **patch_kwargs
     ) -> Ax:
         """Plot geometry cross section at single (x,y,z) coordinate.
@@ -1452,15 +1459,84 @@
     def _center_not_inf(cls, val):
         """Make sure center is not infinitiy."""
         if any(np.isinf(v) for v in val):
             raise ValidationError("center can not contain td.inf terms.")
         return val
 
 
-class Planar(Geometry, ABC):
+class SimplePlaneIntersection(Geometry, ABC):
+    """A geometry where intersections with an axis aligned plane may be computed efficiently."""
+
+    def intersections_tilted_plane(
+        self, normal: Coordinate, origin: Coordinate, to_2D: MatrixReal4x4
+    ) -> List[Shapely]:
+        """Return a list of shapely geometries at the plane specified by normal and origin.
+        Checks special cases before relying on the complete computation.
+
+        Parameters
+        ----------
+        normal : Coordinate
+            Vector defining the normal direction to the plane.
+        origin : Coordinate
+            Vector defining the plane origin.
+        to_2D : MatrixReal4x4
+            Transformation matrix to apply to resulting shapes.
+
+        Returns
+        -------
+        List[shapely.geometry.base.BaseGeometry]
+            List of 2D shapes that intersect plane.
+            For more details refer to
+            `Shapely's Documentation <https://shapely.readthedocs.io/en/stable/project.html>`_.
+        """
+
+        # Check if normal is a special case, where the normal is aligned with an axis.
+        if normal.count(0.0) == 2:
+            axis = np.nonzero(normal)[0][0]
+            coord = "xyz"[axis]
+            kwargs = {coord: origin[axis]}
+            section = self.intersections_plane(**kwargs)
+            # Apply transformation in the plane by removing row and column
+            to_2D_in_plane = np.delete(np.delete(to_2D, axis, 0), axis, 1)
+
+            def transform(p_array):
+                return np.dot(
+                    np.hstack((p_array, np.ones((p_array.shape[0], 1)))), to_2D_in_plane.T
+                )[:, :2]
+
+            transformed_section = shapely.transform(section, transformation=transform)
+            return transformed_section
+        else:  # Otherwise compute the arbitrary intersection
+            return self._do_intersections_tilted_plane(normal=normal, origin=origin, to_2D=to_2D)
+
+    @abstractmethod
+    def _do_intersections_tilted_plane(
+        self, normal: Coordinate, origin: Coordinate, to_2D: MatrixReal4x4
+    ) -> List[Shapely]:
+        """Return a list of shapely geometries at the plane specified by normal and origin.
+
+        Parameters
+        ----------
+        normal : Coordinate
+            Vector defining the normal direction to the plane.
+        origin : Coordinate
+            Vector defining the plane origin.
+        to_2D : MatrixReal4x4
+            Transformation matrix to apply to resulting shapes.
+
+        Returns
+        -------
+        List[shapely.geometry.base.BaseGeometry]
+            List of 2D shapes that intersect plane.
+            For more details refer to
+            `Shapely's Documentation <https://shapely.readthedocs.io/en/stable/project.html>`_.
+        """
+
+
+class Planar(SimplePlaneIntersection, Geometry, ABC):
     """Geometry with one ``axis`` that is slab-like with thickness ``height``."""
 
     axis: Axis = pydantic.Field(
         2, title="Axis", description="Specifies dimension of the planar axis (0,1,2) -> (x,y,z)."
     )
 
     sidewall_angle: float = pydantic.Field(
@@ -1652,15 +1728,15 @@
             return None
         return 2 * np.sqrt(self.radius**2 - dz**2)
 
 
 """Primitive classes"""
 
 
-class Box(Centered):
+class Box(SimplePlaneIntersection, Centered):
     """Rectangular prism.
        Also base class for :class:`Simulation`, :class:`Monitor`, and :class:`Source`.
 
     Example
     -------
     >>> b = Box(center=(1,2,3), size=(2,2,2))
     """
@@ -1807,15 +1883,15 @@
         exclude_surfaces = kwargs.pop("exclude_surfaces", None)
         surfaces = cls.surfaces(size=size, center=center, **kwargs)
         if "name" in cls.__dict__["__fields__"] and exclude_surfaces:
             surfaces = [surf for surf in surfaces if surf.name[-2:] not in exclude_surfaces]
         return surfaces
 
     @verify_packages_import(["trimesh"])
-    def intersections_tilted_plane(
+    def _do_intersections_tilted_plane(
         self, normal: Coordinate, origin: Coordinate, to_2D: MatrixReal4x4
     ) -> List[Shapely]:
         """Return a list of shapely geometries at the plane specified by normal and origin.
 
         Parameters
         ----------
         normal : Coordinate
@@ -2000,14 +2076,23 @@
         """Get the normal to the given geometry, checking that it is a 2D geometry."""
         if np.count_nonzero(self.size) != 2:
             raise ValidationError(
                 "'Medium2D' requires exactly one of the 'Box' dimensions to have size zero."
             )
         return self.size.index(0)
 
+    def _update_from_bounds(self, bounds: Tuple[float, float], axis: Axis) -> Box:
+        """Returns an updated geometry which has been transformed to fit within ``bounds``
+        along the ``axis`` direction."""
+        new_center = list(self.center)
+        new_center[axis] = (bounds[0] + bounds[1]) / 2
+        new_size = list(self.size)
+        new_size[axis] = bounds[1] - bounds[0]
+        return self.updated_copy(center=new_center, size=new_size)
+
     def _plot_arrow(
         self,
         direction: Tuple[float, float, float],
         x: float = None,
         y: float = None,
         z: float = None,
         color: str = None,
@@ -2426,14 +2511,41 @@
         bool
             ``True`` if the transformation preserves the axis orientation, ``False`` otherwise.
         """
         i = (axis + 1) % 3
         j = (axis + 2) % 3
         return np.isclose(transform[i, axis], 0) and np.isclose(transform[j, axis], 0)
 
+    @cached_property
+    def _normal_2dmaterial(self) -> Axis:
+        """Get the normal to the given geometry, checking that it is a 2D geometry."""
+        normal = self.geometry._normal_2dmaterial
+        preserves_axis = Transformed.preserves_axis(self.transform, normal)
+
+        if not preserves_axis:
+            raise ValidationError(
+                "'Medium2D' requires geometries of type 'Transformed' to "
+                "perserve the axis normal to the 'Medium2D'."
+            )
+
+        return normal
+
+    def _update_from_bounds(self, bounds: Tuple[float, float], axis: Axis) -> Transformed:
+        """Returns an updated geometry which has been transformed to fit within ``bounds``
+        along the ``axis`` direction."""
+        min_bound = np.array([0, 0, 0, 1.0])
+        min_bound[axis] = bounds[0]
+        max_bound = np.array([0, 0, 0, 1.0])
+        max_bound[axis] = bounds[1]
+        new_bounds = []
+        new_bounds.append(np.dot(self.inverse, min_bound)[axis])
+        new_bounds.append(np.dot(self.inverse, max_bound)[axis])
+        new_geometry = self.geometry._update_from_bounds(bounds=new_bounds, axis=axis)
+        return self.updated_copy(geometry=new_geometry)
+
 
 class ClipOperation(Geometry):
     """Class representing the result of a set operation between geometries."""
 
     operation: ClipOperationType = pydantic.Field(
         ...,
         title="Operation Type",
@@ -2643,14 +2755,42 @@
         return self.geometry_a.volume(bounds) + self.geometry_b.volume(bounds)
 
     def _surface_area(self, bounds: Bound) -> float:
         """Returns object's surface area within given bounds."""
         # Overestimates
         return self.geometry_a.surface_area(bounds) + self.geometry_b.surface_area(bounds)
 
+    @cached_property
+    def _normal_2dmaterial(self) -> Axis:
+        """Get the normal to the given geometry, checking that it is a 2D geometry."""
+        normal_a = self.geometry_a._normal_2dmaterial
+        normal_b = self.geometry_b._normal_2dmaterial
+
+        if normal_a != normal_b:
+            raise ValidationError(
+                "'Medium2D' requires both geometries in the 'ClipOperation' to "
+                "have exactly one dimension with zero size in common."
+            )
+
+        plane_position_a = self.geometry_a.bounds[0][normal_a]
+        plane_position_b = self.geometry_b.bounds[0][normal_b]
+
+        if plane_position_a != plane_position_b:
+            raise ValidationError(
+                "'Medium2D' requires both geometries in the 'ClipOperation' to be co-planar."
+            )
+        return normal_a
+
+    def _update_from_bounds(self, bounds: Tuple[float, float], axis: Axis) -> ClipOperation:
+        """Returns an updated geometry which has been transformed to fit within ``bounds``
+        along the ``axis`` direction."""
+        new_geom_a = self.geometry_a._update_from_bounds(bounds=bounds, axis=axis)
+        new_geom_b = self.geometry_b._update_from_bounds(bounds=bounds, axis=axis)
+        return self.updated_copy(geometry_a=new_geom_a, geometry_b=new_geom_b)
+
 
 class GeometryGroup(Geometry):
     """A collection of Geometry objects that can be called as a single geometry object."""
 
     geometries: Tuple[annotate_type(GeometryType), ...] = pydantic.Field(
         ...,
         title="Geometries",
@@ -2808,9 +2948,36 @@
         return np.sum(individual_volumes)
 
     def _surface_area(self, bounds: Bound) -> float:
         """Returns object's surface area within given bounds."""
         individual_areas = (geometry.surface_area(bounds) for geometry in self.geometries)
         return np.sum(individual_areas)
 
+    @cached_property
+    def _normal_2dmaterial(self) -> Axis:
+        """Get the normal to the given geometry, checking that it is a 2D geometry."""
+
+        normals = {geom._normal_2dmaterial for geom in self.geometries}
+
+        if len(normals) != 1:
+            raise ValidationError(
+                "'Medium2D' requires all geometries in the 'GeometryGroup' to "
+                "share exactly one dimension with zero size."
+            )
+        normal = list(normals)[0]
+        positions = {geom.bounds[0][normal] for geom in self.geometries}
+        if len(positions) != 1:
+            raise ValidationError(
+                "'Medium2D' requires all geometries in the 'GeometryGroup' to be co-planar."
+            )
+        return normal
+
+    def _update_from_bounds(self, bounds: Tuple[float, float], axis: Axis) -> GeometryGroup:
+        """Returns an updated geometry which has been transformed to fit within ``bounds``
+        along the ``axis`` direction."""
+        new_geometries = [
+            geometry._update_from_bounds(bounds=bounds, axis=axis) for geometry in self.geometries
+        ]
+        return self.updated_copy(geometries=new_geometries)
+
 
 from .utils import GeometryType, from_shapely, vertices_from_shapely  # noqa: E402
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/geometry/mesh.py` & `tidy3d-2.7.0rc2/tidy3d/components/geometry/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 import numpy as np
 
 from ..base import cached_property
 from ..types import Ax, Bound, Coordinate, MatrixReal4x4, Shapely
 from ..viz import add_ax_if_none, equal_aspect
 from ...log import log
 from ...exceptions import ValidationError, DataError
-from ...constants import fp_eps, inf
+from ...constants import inf
 from ..data.dataset import TriangleMeshDataset
 from ..data.data_array import TriangleMeshDataArray, DATA_ARRAY_MAP
 from ..data.validators import validate_no_nans
 from ...packaging import verify_packages_import
 
 from . import base
 
+AREA_SIZE_THRESHOLD = 1e-36
+
 
 class TriangleMesh(base.Geometry, ABC):
     """Custom surface geometry given by a triangle mesh, as in the STL file format.
 
     Example
     -------
     >>> vertices = np.array([[0, 0, 0], [1, 0, 0], [0, 1, 0], [0, 0, 1]])
@@ -56,17 +58,17 @@
 
     @pydantic.validator("mesh_dataset", always=True)
     def _check_mesh(cls, val: TriangleMeshDataset) -> TriangleMeshDataset:
         """Check that the mesh is valid."""
         if val is None:
             return None
         mesh = cls._triangles_to_trimesh(val.surface_mesh)
-        if not all(np.array(mesh.area_faces) > fp_eps):
+        if not all(np.array(mesh.area_faces) > AREA_SIZE_THRESHOLD):
             raise ValidationError(
-                "The provided mesh has triangles with zero area. "
+                f"The provided mesh has triangles with near zero area < {AREA_SIZE_THRESHOLD}. "
                 "Consider using numpy-stl's 'from_file' import with 'remove_empty_areas' set "
                 "to True and a suitable 'AREA_SIZE_THRESHOLD' to remove them."
             )
         if not mesh.is_winding_consistent:
             log.warning(
                 "The provided mesh does not have consistent winding (face orientations). "
                 "This can lead to incorrect permittivity distributions. You can use a "
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/geometry/polyslab.py` & `tidy3d-2.7.0rc2/tidy3d/components/geometry/polyslab.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,14 +427,24 @@
     @cached_property
     def _normal_2dmaterial(self) -> Axis:
         """Get the normal to the given geometry, checking that it is a 2D geometry."""
         if self.slab_bounds[0] != self.slab_bounds[1]:
             raise ValidationError("'Medium2D' requires the 'PolySlab' bounds to be equal.")
         return self.axis
 
+    def _update_from_bounds(self, bounds: Tuple[float, float], axis: Axis) -> PolySlab:
+        """Returns an updated geometry which has been transformed to fit within ``bounds``
+        along the ``axis`` direction."""
+        if axis != self.axis:
+            raise ValueError(
+                f"'_update_from_bounds' may only be applied along axis '{self.axis}', "
+                f"but was given axis '{axis}'."
+            )
+        return self.updated_copy(slab_bounds=bounds)
+
     @cached_property
     def is_ccw(self) -> bool:
         """Is this ``PolySlab`` CCW-oriented?"""
         return PolySlab._area(self.vertices) > 0
 
     def inside(
         self, x: np.ndarray[float], y: np.ndarray[float], z: np.ndarray[float]
@@ -530,15 +540,15 @@
             vertices_z = self._shift_vertices(self.middle_polygon, dist)[0]
             face_polygon = shapely.Polygon(vertices_z)
             point = shapely.Point(x, y)
             inside_polygon = face_polygon.covers(point)
         return inside_height * inside_polygon
 
     @verify_packages_import(["trimesh"])
-    def intersections_tilted_plane(
+    def _do_intersections_tilted_plane(
         self, normal: Coordinate, origin: Coordinate, to_2D: MatrixReal4x4
     ) -> List[Shapely]:
         """Return a list of shapely geometries at the plane specified by normal and origin.
 
         Parameters
         ----------
         normal : Coordinate
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/geometry/primitives.py` & `tidy3d-2.7.0rc2/tidy3d/components/geometry/primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from math import isclose
 
 import pydantic.v1 as pydantic
 import numpy as np
 import shapely
 
 from ..base import cached_property, skip_if_fields_missing
-from ..types import Axis, Bound, Coordinate, MatrixReal4x4, Shapely
+from ..types import Axis, Bound, Coordinate, MatrixReal4x4, Shapely, Tuple
 from ...exceptions import SetupError, ValidationError
 from ...constants import MICROMETER, LARGE_NUMBER
 from ...packaging import verify_packages_import
 from . import base
 
 # for sampling conical frustum in visualization
 _N_SAMPLE_CURVE_SHAPELY = 40
@@ -229,16 +229,29 @@
     @cached_property
     def _normal_2dmaterial(self) -> Axis:
         """Get the normal to the given geometry, checking that it is a 2D geometry."""
         if self.length != 0:
             raise ValidationError("'Medium2D' requires the 'Cylinder' length to be zero.")
         return self.axis
 
+    def _update_from_bounds(self, bounds: Tuple[float, float], axis: Axis) -> Cylinder:
+        """Returns an updated geometry which has been transformed to fit within ``bounds``
+        along the ``axis`` direction."""
+        if axis != self.axis:
+            raise ValueError(
+                f"'_update_from_bounds' may only be applied along axis '{self.axis}', "
+                f"but was given axis '{axis}'."
+            )
+        new_center = list(self.center)
+        new_center[axis] = (bounds[0] + bounds[1]) / 2
+        new_length = bounds[1] - bounds[0]
+        return self.updated_copy(center=new_center, length=new_length)
+
     @verify_packages_import(["trimesh"])
-    def intersections_tilted_plane(
+    def _do_intersections_tilted_plane(
         self, normal: Coordinate, origin: Coordinate, to_2D: MatrixReal4x4
     ) -> List[Shapely]:
         """Return a list of shapely geometries at the plane specified by normal and origin.
 
         Parameters
         ----------
         normal : Coordinate
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/geometry/triangulation.py` & `tidy3d-2.7.0rc2/tidy3d/components/geometry/triangulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/geometry/utils.py` & `tidy3d-2.7.0rc2/tidy3d/components/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/geometry/utils_2d.py` & `tidy3d-2.7.0rc2/tidy3d/components/geometry/utils_2d.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 """Utilities for 2D geometry manipulation."""
 import numpy as np
 import shapely
 from typing import Tuple, List
 
 from ..types import Axis
 from ...constants import inf
-from ...exceptions import ValidationError
 from ..geometry.base import Geometry, Box, ClipOperation
-from ..geometry.primitives import Cylinder
 from ..geometry.polyslab import PolySlab
 from ..grid.grid import Grid
 from ..scene import Scene
 from ..structure import Structure
 
-# for 2d materials. to find neighboring media, search a distance on either side
-# equal to this times the grid size
-DIST_NEIGHBOR_REL_2D_MED = 1e-5
-
 
 def increment_float(val: np.float32, sign) -> np.float32:
     """Applies a small positive or negative shift to a 32bit float using numpy.nextafter,"""
     """but additionally handles some corner cases."""
     # Infinity is left unchanged
     if val == inf or val == -inf:
         return val
@@ -44,59 +38,41 @@
 
 
 def get_bounds(geom: Geometry, axis: Axis) -> Tuple[float, float]:
     """Get the bounds of a geometry in the axis direction."""
     return (geom.bounds[0][axis], geom.bounds[1][axis])
 
 
-def set_bounds(geom: Geometry, bounds: Tuple[float, float], axis: Axis) -> Geometry:
-    """Set the bounds of a geometry in the axis direction."""
-    if isinstance(geom, Box):
-        new_center = list(geom.center)
-        new_center[axis] = (bounds[0] + bounds[1]) / 2
-        new_size = list(geom.size)
-        new_size[axis] = bounds[1] - bounds[0]
-        return geom.updated_copy(center=new_center, size=new_size)
-    if isinstance(geom, PolySlab):
-        return geom.updated_copy(slab_bounds=bounds)
-    if isinstance(geom, Cylinder):
-        new_center = list(geom.center)
-        new_center[axis] = (bounds[0] + bounds[1]) / 2
-        new_length = bounds[1] - bounds[0]
-        return geom.updated_copy(center=new_center, length=new_length)
-    raise ValidationError(
-        "'Medium2D' is only compatible with 'Box', 'PolySlab', or 'Cylinder' geometry."
-    )
-
-
 def get_thickened_geom(geom: Geometry, axis: Axis, axis_dl: float):
     """Helper to return a slightly thickened version of a planar geometry."""
     center = get_bounds(geom, axis)[0]
-    neg_thickness = axis_dl * DIST_NEIGHBOR_REL_2D_MED
-    pos_thickness = axis_dl * DIST_NEIGHBOR_REL_2D_MED
-    return set_bounds(geom, bounds=(center - neg_thickness, center + pos_thickness), axis=axis)
+    neg_thickness = increment_float(center, -1.0)
+    pos_thickness = increment_float(center, 1.0)
+    return geom._update_from_bounds(bounds=(neg_thickness, pos_thickness), axis=axis)
 
 
 def get_neighbors(
     geom: Geometry,
     axis: Axis,
     axis_dl: float,
     structures: List[Structure],
 ):
     """Find the neighboring structures and return the tested positions above and below."""
     center = get_bounds(geom, axis)[0]
     check_delta = [
-        -axis_dl * DIST_NEIGHBOR_REL_2D_MED,
-        axis_dl * DIST_NEIGHBOR_REL_2D_MED,
+        increment_float(center, -1.0) - center,
+        increment_float(center, 1.0) - center,
     ]
 
     neighbors_below = []
     neighbors_above = []
     for _, position in enumerate(check_delta):
-        geom_shifted = set_bounds(geom, bounds=(center + position, center + position), axis=axis)
+        geom_shifted = geom._update_from_bounds(
+            bounds=(center + position, center + position), axis=axis
+        )
 
         # to prevent false positives due to 2D materials touching different materials
         # along their sides, shrink the bounds along the tangential directions by
         # a tiny bit before checking for intersections
         bounds = [list(i) for i in geom_shifted.bounds]
         _, tan_dirs = Geometry.pop_axis([0, 1, 2], axis=axis)
         for dim in tan_dirs:
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/grid/grid.py` & `tidy3d-2.7.0rc2/tidy3d/components/grid/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import pydantic.v1 as pd
 
 from ..base import Tidy3dBaseModel
 from ..data.data_array import DataArray, SpatialDataArray, ScalarFieldDataArray
 from ..data.dataset import UnstructuredGridDatasetType, UnstructuredGridDataset
-from ..types import ArrayFloat1D, Axis, TYPE_TAG_STR, InterpMethod, Literal
+from ..types import ArrayFloat1D, Axis, InterpMethod, Literal
 from ..geometry.base import Box
 
 from ...exceptions import SetupError
 
 # data type of one dimensional coordinate array.
 Coords1D = ArrayFloat1D
 
@@ -39,15 +39,15 @@
     z: Coords1D = pd.Field(
         ..., title="Z Coordinates", description="1-dimensional array of z coordinates."
     )
 
     @property
     def to_dict(self):
         """Return a dict of the three Coord1D objects as numpy arrays."""
-        return {key: np.array(value) for key, value in self.dict(exclude={TYPE_TAG_STR}).items()}
+        return {key: self.dict()[key] for key in "xyz"}
 
     @property
     def to_list(self):
         """Return a list of the three Coord1D objects as numpy arrays."""
         return list(self.to_dict.values())
 
     def _interp_from_xarray(
@@ -382,17 +382,15 @@
         >>> x = np.linspace(-1, 1, 10)
         >>> y = np.linspace(-1, 1, 11)
         >>> z = np.linspace(-1, 1, 12)
         >>> coords = Coords(x=x, y=y, z=z)
         >>> grid = Grid(boundaries=coords)
         >>> Nx, Ny, Nz = grid.num_cells
         """
-        return [
-            len(coords1d) - 1 for coords1d in self.boundaries.dict(exclude={TYPE_TAG_STR}).values()
-        ]
+        return [len(self.boundaries.dict()[dim]) - 1 for dim in "xyz"]
 
     @property
     def _primal_steps(self) -> Coords:
         """Return primal steps of the cells in the :class:`Grid`.
 
         Returns
         -------
@@ -408,15 +406,15 @@
         Returns
         -------
         :class:`Coords`
             Distances between each of the cell centers along each dimension, with periodicity
             applied.
         """
 
-        primal_steps = self._primal_steps.dict(exclude={TYPE_TAG_STR})
+        primal_steps = {dim: self._primal_steps.dict()[dim] for dim in "xyz"}
         dsteps = {key: (psteps + np.roll(psteps, 1)) / 2 for (key, psteps) in primal_steps.items()}
 
         return Coords(**dsteps)
 
     @property
     def yee(self) -> YeeGrid:
         """Return the :class:`YeeGrid` defining the yee cell locations for this :class:`Grid`.
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.7.0rc2/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/grid/mesher.py` & `tidy3d-2.7.0rc2/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/heat/boundary.py` & `tidy3d-2.7.0rc2/tidy3d/components/heat/boundary.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from abc import ABC
 from typing import Union
 
 import pydantic.v1 as pd
 
 from ..base import Tidy3dBaseModel
 from ..bc_placement import BCPlacementType
+from ..types import TYPE_TAG_STR
 
 from ...constants import KELVIN, HEAT_FLUX, HEAT_TRANSFER_COEFF
 
 
 class HeatBC(ABC, Tidy3dBaseModel):
     """Abstract thermal boundary conditions."""
 
@@ -81,13 +82,15 @@
     ...     condition=ConvectionBC(ambient_temperature=300, transfer_coeff=1),
     ... )
     """
 
     placement: BCPlacementType = pd.Field(
         title="Boundary Conditions Placement",
         description="Location to apply boundary conditions.",
+        discriminator=TYPE_TAG_STR,
     )
 
     condition: HeatBoundaryConditionType = pd.Field(
         title="Boundary Conditions",
         description="Boundary conditions to apply at the selected location.",
+        discriminator=TYPE_TAG_STR,
     )
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/heat/data/sim_data.py` & `tidy3d-2.7.0rc2/tidy3d/components/heat/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/heat/grid.py` & `tidy3d-2.7.0rc2/tidy3d/components/heat/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 """Defines heat grid specifications"""
 from __future__ import annotations
 
+from abc import ABC
 from typing import Union, Tuple
 import pydantic.v1 as pd
 
 from ..base import Tidy3dBaseModel, skip_if_fields_missing
 from ...constants import MICROMETER
 from ...exceptions import ValidationError
 
 
-class UniformUnstructuredGrid(Tidy3dBaseModel):
+class UnstructuredGrid(Tidy3dBaseModel, ABC):
+    """Abstract unstructured grid."""
 
+    relative_min_dl: pd.NonNegativeFloat = pd.Field(
+        1e-3,
+        title="Relative Mesh Size Limit",
+        description="The minimal allowed mesh size relative to the largest dimension of the simulation domain."
+        "Use ``relative_min_dl=0`` to remove this constraint.",
+    )
+
+
+class UniformUnstructuredGrid(UnstructuredGrid):
     """Uniform grid.
 
     Example
     -------
     >>> heat_grid = UniformUnstructuredGrid(dl=0.1)
     """
 
@@ -43,15 +54,15 @@
         (),
         title="Structures Without Refinement",
         description="List of structures for which ``min_edges_per_circumference`` and "
         "``min_edges_per_side`` will not be enforced. The original ``dl`` is used instead.",
     )
 
 
-class DistanceUnstructuredGrid(Tidy3dBaseModel):
+class DistanceUnstructuredGrid(UnstructuredGrid):
     """Adaptive grid based on distance to material interfaces. Currently not recommended for larger
     simulations.
 
     Example
     -------
     >>> heat_grid = DistanceUnstructuredGrid(
     ...     dl_interface=0.1,
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/heat/monitor.py` & `tidy3d-2.7.0rc2/tidy3d/components/heat/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/heat/simulation.py` & `tidy3d-2.7.0rc2/tidy3d/components/heat/simulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,43 +7,38 @@
 
 import pydantic.v1 as pd
 
 from .boundary import TemperatureBC, HeatFluxBC, ConvectionBC
 from .boundary import HeatBoundarySpec
 from .source import HeatSourceType, UniformHeatSource
 from .monitor import HeatMonitorType
-from .grid import HeatGridType
+from .grid import HeatGridType, UniformUnstructuredGrid, DistanceUnstructuredGrid
 from .viz import HEAT_BC_COLOR_TEMPERATURE, HEAT_BC_COLOR_FLUX, HEAT_BC_COLOR_CONVECTION
 from .viz import plot_params_heat_bc, plot_params_heat_source, HEAT_SOURCE_CMAP
 
 from ..base_sim.simulation import AbstractSimulation
 from ..base import cached_property, skip_if_fields_missing
 from ..types import Ax, Shapely, TYPE_TAG_STR, ScalarSymmetry, Bound
 from ..viz import add_ax_if_none, equal_aspect, PlotParams
 from ..structure import Structure
-from ..geometry.base import Box, GeometryGroup
-from ..geometry.primitives import Sphere, Cylinder
-from ..geometry.polyslab import PolySlab
-from ..geometry.mesh import TriangleMesh
+from ..geometry.base import Box
 from ..scene import Scene
 from ..heat_spec import SolidSpec
 
 from ..bc_placement import StructureBoundary, StructureStructureInterface
 from ..bc_placement import StructureSimulationBoundary, SimulationBoundary
 from ..bc_placement import MediumMediumInterface
 
 from ...exceptions import SetupError
 from ...constants import inf, VOLUMETRIC_HEAT_RATE
 
 from ...log import log
 
 HEAT_BACK_STRUCTURE_STR = "<<<HEAT_BACKGROUND_STRUCTURE>>>"
 
-HeatSingleGeometryType = (Box, Cylinder, Sphere, PolySlab, TriangleMesh)
-
 
 class HeatSimulation(AbstractSimulation):
     """Contains all information about heat simulation.
 
     Example
     -------
     >>> from tidy3d import Medium, SolidSpec, FluidSpec, UniformUnstructuredGrid, TemperatureMonitor
@@ -112,32 +107,86 @@
         """Error if structures contain unsupported yet geometries."""
         for ind, structure in enumerate(val):
             bbox = structure.geometry.bounding_box
             if any(s == 0 for s in bbox.size):
                 raise SetupError(
                     f"'HeatSimulation' does not currently support structures with dimensions of zero size ('structures[{ind}]')."
                 )
+        return val
+
+    @staticmethod
+    def _check_cross_solids(objs: Tuple[Box, ...], values: Dict) -> Tuple[int, ...]:
+        """Given model dictionary ``values``, check whether objects in list ``objs`` cross
+        a ``SolidSpec`` medium.
+        """
+
+        try:
+            size = values["size"]
+            center = values["center"]
+            medium = values["medium"]
+            structures = values["structures"]
+        except KeyError:
+            raise SetupError(
+                "Function '_check_cross_solids' assumes dictionary 'values' contains well-defined "
+                "'size', 'center',  'medium', and 'structures'. Thus, it should only be used in "
+                "validators with @skip_if_fields_missing(['medium', 'center', 'size', 'structures']) "
+                "or root validators with option 'skip_on_failure=True'."
+            )
 
-            if isinstance(structure.geometry, GeometryGroup):
-                geometries = structure.geometry.geometries
+        # list of structures including background as a Box()
+        structure_bg = Structure(
+            geometry=Box(
+                size=size,
+                center=center,
+            ),
+            medium=medium,
+        )
+
+        total_structures = [structure_bg] + list(structures)
+
+        failed_obj_inds = []
+        for ind, obj in enumerate(objs):
+            if obj.size.count(0.0) == 1:
+                # for planar objects we could do a rigorous check
+                medium_set = Scene.intersecting_media(obj, total_structures)
+                crosses_solid = any(
+                    isinstance(medium.heat_spec, SolidSpec) for medium in medium_set
+                )
             else:
-                geometries = [structure.geometry]
-            for geom in geometries:
-                if isinstance(geom, (GeometryGroup)):
-                    raise SetupError(
-                        "'HeatSimulation' does not currently support recursive 'GeometryGroup's ('structures[{ind}]')."
-                    )
-                if not isinstance(geom, HeatSingleGeometryType):
-                    geom_names = [f"'{cl.__name__}'" for cl in HeatSingleGeometryType]
-                    raise SetupError(
-                        "'HeatSimulation' does not currently support geometries of type "
-                        f"'{geom.type}'  ('structures[{ind}]'). Allowed geometries are "
-                        f"{', '.join(geom_names)}, "
-                        "and non-recursive 'GeometryGroup'."
-                    )
+                # approximate check for volumetric objects based on bounding boxes
+                # thus, it could still miss a case when there is no data inside the monitor
+                crosses_solid = any(
+                    obj.intersects(structure.geometry)
+                    for structure in total_structures
+                    if isinstance(structure.medium.heat_spec, SolidSpec)
+                )
+
+            if not crosses_solid:
+                failed_obj_inds.append(ind)
+
+        return failed_obj_inds
+
+    @pd.validator("monitors", always=True)
+    @skip_if_fields_missing(["medium", "center", "size", "structures"])
+    def _monitors_cross_solids(cls, val, values):
+        """Error if monitors does not cross any solid medium."""
+
+        if val is None:
+            return val
+
+        failed_mnt_inds = cls._check_cross_solids(val, values)
+
+        if len(failed_mnt_inds) > 0:
+            monitor_names = [f"'{val[ind].name}'" for ind in failed_mnt_inds]
+            raise SetupError(
+                f"Monitors {monitor_names} do not cross any solid materials "
+                "('heat_spec=SolidSpec(...)'). The heat equation is solved only inside solid "
+                "materials. Thus, no information will be recorded in these monitors."
+            )
+
         return val
 
     @pd.validator("size", always=True)
     def check_zero_dim_domain(cls, val, values):
         """Error if heat domain have zero dimensions."""
 
         dim_names = ["x", "y", "z"]
@@ -169,15 +218,15 @@
 
         for bc_ind, bc_spec in enumerate(val):
             bc_place = bc_spec.placement
             if isinstance(bc_place, (StructureBoundary, StructureSimulationBoundary)):
                 if bc_place.structure not in structures_names:
                     raise SetupError(
                         f"Structure '{bc_place.structure}' provided in "
-                        f"'boundary_spec[{bc_ind}].placement' (type '{bc_place.type}')"
+                        f"'boundary_spec[{bc_ind}].placement' (type '{bc_place.type}') "
                         "is not found among simulation structures."
                     )
             if isinstance(bc_place, (StructureStructureInterface)):
                 for struct_name in bc_place.structures:
                     if struct_name and struct_name not in structures_names:
                         raise SetupError(
                             f"Structure '{struct_name}' provided in "
@@ -218,14 +267,34 @@
                 log.warning(
                     f"Structure '{structure_name}' listed as a non-refined structure in "
                     "'HeatSimulation.grid_spec' is not present in 'HeatSimulation.structures'"
                 )
 
         return val
 
+    @pd.validator("grid_spec", always=True)
+    def warn_if_minimal_mesh_size_override(cls, val, values):
+        """Warn if minimal mesh size limit overrides desired mesh size."""
+
+        max_size = np.max(values.get("size"))
+        min_dl = val.relative_min_dl * max_size
+
+        if isinstance(val, UniformUnstructuredGrid):
+            desired_min_dl = val.dl
+        if isinstance(val, DistanceUnstructuredGrid):
+            desired_min_dl = min(val.dl_interface, val.dl_bulk)
+
+        if desired_min_dl < min_dl:
+            log.warning(
+                f"The resulting limit for minimal mesh size from parameter 'relative_min_dl={val.relative_min_dl}' is {min_dl}, while provided mesh size in 'grid_spec' is {desired_min_dl}. "
+                "Consider lowering parameter 'relative_min_dl' if a finer grid is required."
+            )
+
+        return val
+
     @pd.validator("sources", always=True)
     @skip_if_fields_missing(["structures"])
     def names_exist_sources(cls, val, values):
         """Error if a heat source point to non-existing structures."""
         structures = values.get("structures")
         structures_names = {s.name for s in structures}
 
@@ -237,20 +306,25 @@
                         "is not found among simulation structures."
                     )
         return val
 
     @pd.root_validator(skip_on_failure=True)
     def check_medium_heat_spec(cls, values):
         """Error if no structures with SolidSpec."""
-        medium = values["medium"]
-        structures = values["structures"]
-        if not (
-            isinstance(medium.heat_spec, SolidSpec)
-            or any(isinstance(struct.medium.heat_spec, SolidSpec) for struct in structures)
-        ):
+
+        sim_box = (
+            Box(
+                size=values.get("size"),
+                center=values.get("center"),
+            ),
+        )
+
+        failed = cls._check_cross_solids(sim_box, values)
+
+        if len(failed) > 0:
             raise SetupError(
                 "No solid materials ('SolidSpec') are detected in heat simulation. Solution domain is empty."
             )
 
         return values
 
     @equal_aspect
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/heat/source.py` & `tidy3d-2.7.0rc2/tidy3d/components/heat/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/heat_spec.py` & `tidy3d-2.7.0rc2/tidy3d/components/heat_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/lumped_element.py` & `tidy3d-2.7.0rc2/tidy3d/components/lumped_element.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/medium.py` & `tidy3d-2.7.0rc2/tidy3d/components/medium.py`

 * *Files 2% similar despite different names*

```diff
@@ -677,14 +677,19 @@
                 "not simultaneously supported."
             )
         return val
 
     _name_validator = validate_name_str()
 
     @cached_property
+    def is_spatially_uniform(self) -> bool:
+        """Whether the medium is spatially uniform."""
+        return True
+
+    @cached_property
     def is_time_modulated(self) -> bool:
         """Whether any component of the medium is time modulated."""
         return self.modulation_spec is not None and self.modulation_spec.applied_modulation
 
     @cached_property
     def is_nonlinear(self) -> bool:
         """Whether the medium is nonlinear."""
@@ -754,22 +759,39 @@
     def nk_model(self, frequency: float) -> Tuple[float, float]:
         """Real and imaginary parts of the refactive index as a function of frequency.
 
         Parameters
         ----------
         frequency : float
             Frequency to evaluate permittivity at (Hz).
+
         Returns
         -------
         Tuple[float, float]
             Real part (n) and imaginary part (k) of refractive index of medium.
         """
         eps_complex = self.eps_model(frequency=frequency)
         return self.eps_complex_to_nk(eps_complex)
 
+    def loss_tangent_model(self, frequency: float) -> Tuple[float, float]:
+        """Permittivity and loss tangent as a function of frequency.
+
+        Parameters
+        ----------
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        Tuple[float, float]
+            Real part of permittivity and loss tangent.
+        """
+        eps_complex = self.eps_model(frequency=frequency)
+        return self.eps_complex_to_eps_loss_tangent(eps_complex)
+
     @ensure_freq_in_range
     def eps_diagonal(self, frequency: float) -> Tuple[complex, complex, complex]:
         """Main diagonal of the complex-valued permittivity tensor as a function of frequency.
 
         Parameters
         ----------
         frequency : float
@@ -959,14 +981,49 @@
             Real part of relative permittivity & electric conductivity.
         """
         eps_real, eps_imag = eps_complex.real, eps_complex.imag
         omega = 2 * np.pi * freq
         sigma = omega * eps_imag * EPSILON_0
         return eps_real, sigma
 
+    @staticmethod
+    def eps_complex_to_eps_loss_tangent(eps_complex: complex) -> Tuple[float, float]:
+        """Convert complex permittivity to permittivity and loss tangent.
+
+        Parameters
+        ----------
+        eps_complex : complex
+            Complex-valued relative permittivity.
+
+        Returns
+        -------
+        Tuple[float, float]
+            Real part of relative permittivity & loss tangent
+        """
+        eps_real, eps_imag = eps_complex.real, eps_complex.imag
+        return eps_real, eps_imag / eps_real
+
+    @staticmethod
+    def eps_loss_tangent_to_eps_complex(eps_real: float, loss_tangent: float) -> complex:
+        """Convert permittivity and loss tangent to complex permittivity.
+
+        Parameters
+        ----------
+        eps_real : float
+            Real part of relative permittivity
+        loss_tangent : float
+            Loss tangent
+
+        Returns
+        -------
+        eps_complex : complex
+            Complex-valued relative permittivity.
+        """
+        return eps_real * (1 + 1j * loss_tangent)
+
     @ensure_freq_in_range
     def sigma_model(self, freq: float) -> complex:
         """Complex-valued conductivity as a function of frequency.
 
         Parameters
         ----------
         freq: float
@@ -1481,14 +1538,21 @@
                 "For passive medium, 'conductivity' must be non-negative. "
                 "To simulate a gain medium, please set 'allow_gain=True'. "
                 "Caution: simulations with a gain medium are unstable, and are likely to diverge."
             )
         return val
 
     @cached_property
+    def is_spatially_uniform(self) -> bool:
+        """Whether the medium is spatially uniform."""
+        if self.conductivity is None:
+            return self.permittivity.is_uniform
+        return self.permittivity.is_uniform and self.conductivity.is_uniform
+
+    @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
         material factor into account is multiplied by ``n_cfl``.
 
         For dispersiveless medium, it equals ``sqrt(permittivity)``.
         """
@@ -1838,14 +1902,19 @@
         if self.eps_dataset is None:
             return True
         if self.eps_dataset.eps_xx == self.eps_dataset.eps_yy == self.eps_dataset.eps_zz:
             return True
         return False
 
     @cached_property
+    def is_spatially_uniform(self) -> bool:
+        """Whether the medium is spatially uniform."""
+        return self._medium.is_spatially_uniform
+
+    @cached_property
     def freqs(self) -> np.ndarray:
         """float array of frequencies.
         This field is to be deprecated in v3.0.
         """
         # return dummy values in this case
         if self.eps_dataset is None:
             return np.array([0, 0, 0])
@@ -2916,14 +2985,26 @@
                 if not _check_same_coordinates(coeff, values["eps_inf"]):
                     raise SetupError(
                         "All pole coefficients 'a' and 'c' must have the same coordinates; "
                         "The coordinates must also be consistent with 'eps_inf'."
                     )
         return val
 
+    @cached_property
+    def is_spatially_uniform(self) -> bool:
+        """Whether the medium is spatially uniform."""
+        if not self.eps_inf.is_uniform:
+            return False
+
+        for coeffs in self.poles:
+            for coeff in coeffs:
+                if not coeff.is_uniform:
+                    return False
+        return True
+
     def eps_dataarray_freq(
         self, frequency: float
     ) -> Tuple[CustomSpatialDataType, CustomSpatialDataType, CustomSpatialDataType]:
         """Permittivity array at ``frequency``.
 
         Parameters
         ----------
@@ -3269,14 +3350,23 @@
                     "For passive medium, 'B_i' must be non-negative. "
                     "To simulate a gain medium, please set 'allow_gain=True'. "
                     "Caution: simulations with a gain medium are unstable, "
                     "and are likely to diverge."
                 )
         return val
 
+    @cached_property
+    def is_spatially_uniform(self) -> bool:
+        """Whether the medium is spatially uniform."""
+        for coeffs in self.coeffs:
+            for coeff in coeffs:
+                if not coeff.is_uniform:
+                    return False
+        return True
+
     def _pole_residue_dict(self) -> Dict:
         """Dict representation of Medium as a pole-residue model."""
         poles_dict = Sellmeier._pole_residue_dict(self)
         if len(self.coeffs) > 0:
             poles_dict.update({"eps_inf": _ones_like(self.coeffs[0][0])})
         return poles_dict
 
@@ -3694,14 +3784,25 @@
                     "For passive medium, 'Delta epsilon_i' must be non-negative. "
                     "To simulate a gain medium, please set 'allow_gain=True'. "
                     "Caution: simulations with a gain medium are unstable, "
                     "and are likely to diverge."
                 )
         return val
 
+    @cached_property
+    def is_spatially_uniform(self) -> bool:
+        """Whether the medium is spatially uniform."""
+        if not self.eps_inf.is_uniform:
+            return False
+        for coeffs in self.coeffs:
+            for coeff in coeffs:
+                if not coeff.is_uniform:
+                    return False
+        return True
+
     def eps_dataarray_freq(
         self, frequency: float
     ) -> Tuple[CustomSpatialDataType, CustomSpatialDataType, CustomSpatialDataType]:
         """Permittivity array at ``frequency``.
 
         Parameters
         ----------
@@ -3942,14 +4043,25 @@
                 )
             if not CustomDispersiveMedium._validate_isreal_dataarray_tuple((f, delta)):
                 raise SetupError("All terms in 'coeffs' must be real.")
             if np.any(_get_numpy_array(delta) <= 0):
                 raise SetupError("For stable medium, 'delta' must be positive.")
         return val
 
+    @cached_property
+    def is_spatially_uniform(self) -> bool:
+        """Whether the medium is spatially uniform."""
+        if not self.eps_inf.is_uniform:
+            return False
+        for coeffs in self.coeffs:
+            for coeff in coeffs:
+                if not coeff.is_uniform:
+                    return False
+        return True
+
     def eps_dataarray_freq(
         self, frequency: float
     ) -> Tuple[CustomSpatialDataType, CustomSpatialDataType, CustomSpatialDataType]:
         """Permittivity array at ``frequency``.
 
         Parameters
         ----------
@@ -4203,14 +4315,25 @@
                     "For passive medium, 'Delta epsilon_i' must be non-negative. "
                     "To simulate a gain medium, please set 'allow_gain=True'. "
                     "Caution: simulations with a gain medium are unstable, "
                     "and are likely to diverge."
                 )
         return val
 
+    @cached_property
+    def is_spatially_uniform(self) -> bool:
+        """Whether the medium is spatially uniform."""
+        if not self.eps_inf.is_uniform:
+            return False
+        for coeffs in self.coeffs:
+            for coeff in coeffs:
+                if not coeff.is_uniform:
+                    return False
+        return True
+
     def eps_dataarray_freq(
         self, frequency: float
     ) -> Tuple[CustomSpatialDataType, CustomSpatialDataType, CustomSpatialDataType]:
         """Permittivity array at ``frequency``.
 
         Parameters
         ----------
@@ -4473,14 +4596,20 @@
         """
 
         new_comps = [comp.sel_inside(bounds) for comp in [self.xx, self.yy, self.zz]]
 
         return self.updated_copy(**dict(zip(["xx", "yy", "zz"], new_comps)))
 
 
+class AnisotropicMediumFromMedium2D(AnisotropicMedium):
+    """The same as ``AnisotropicMedium``, but converted from Medium2D.
+    (This class is for internal use only)
+    """
+
+
 class FullyAnisotropicMedium(AbstractMedium):
     """Fully anisotropic medium including all 9 components of the permittivity and conductivity
     tensors.
 
     Notes
     -----
 
@@ -4836,14 +4965,19 @@
             if values.get("subpixel") is not None:
                 log.warning(
                     "The field 'subpixel' is ignored. Please set 'subpixel' in each component."
                 )
         return values
 
     @cached_property
+    def is_spatially_uniform(self) -> bool:
+        """Whether the medium is spatially uniform."""
+        return any(comp.is_spatially_uniform for comp in self.components.values())
+
+    @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
         material factor into account is multiplied by ``n_cfl``.
 
         For this medium, it takes the minimal of ``n_clf`` in all components.
         """
@@ -5354,15 +5488,15 @@
                 pole_res = PoleResidue.from_medium(med)
                 eps_inf += weight * (med.eps_model(np.inf) - 1)
             elif isinstance(med, PECMedium):
                 # special treatment for PEC
                 return med
             else:
                 raise ValidationError("Invalid medium type for the components of 'Medium2D'.")
-            poles += [(a, weight * c) for (a, c) in pole_res.poles]
+            poles += [(a, weight * c) for (a, c) in pole_res.poles if c != 0.0]
         return PoleResidue(eps_inf=np.real(eps_inf), poles=poles)
 
     def volumetric_equivalent(
         self,
         axis: Axis,
         adjacent_media: Tuple[MediumType3D, MediumType3D],
         adjacent_dls: Tuple[float, float],
@@ -5426,15 +5560,17 @@
         ]
 
         # combine the two weighted, planar media with the background medium and put in the xyz basis
         media_3d = Geometry.unpop_axis(
             ax_coord=media_bg[axis], plane_coords=media_fg_weighted, axis=axis
         )
         media_3d_kwargs = {dim + dim: medium for dim, medium in zip("xyz", media_3d)}
-        return AnisotropicMedium(**media_3d_kwargs, frequency_range=self.frequency_range)
+        return AnisotropicMediumFromMedium2D(
+            **media_3d_kwargs, frequency_range=self.frequency_range
+        )
 
     def to_anisotropic_medium(self, axis: Axis, thickness: float) -> AnisotropicMedium:
         """Generate a 3D :class:`.AnisotropicMedium` equivalent of a given thickness.
 
         Parameters
         ----------
         axis: Axis
@@ -5663,15 +5799,15 @@
         return isinstance(elements_3d[comp], PECMedium)
 
 
 PEC2D = Medium2D(ss=PEC, tt=PEC)
 
 # types of mediums that can be used in Simulation and Structures
 
-MediumType = Union[MediumType3D, Medium2D]
+MediumType = Union[MediumType3D, Medium2D, AnisotropicMediumFromMedium2D]
 
 
 # Utility function
 def medium_from_nk(n: float, k: float, freq: float, **kwargs) -> Union[Medium, Lorentz]:
     """Convert ``n`` and ``k`` values at frequency ``freq`` to :class:`Medium` if ``Re[epsilon]>=1``,
     or :class:`Lorentz` if if ``Re[epsilon]<1``.
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/mode.py` & `tidy3d-2.7.0rc2/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/monitor.py` & `tidy3d-2.7.0rc2/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/parameter_perturbation.py` & `tidy3d-2.7.0rc2/tidy3d/components/parameter_perturbation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/scene.py` & `tidy3d-2.7.0rc2/tidy3d/components/scene.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/simulation.py` & `tidy3d-2.7.0rc2/tidy3d/components/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-""" Container holding all information about simulation and its components"""
+"""Container holding all information about simulation and its components"""
+
 from __future__ import annotations
 
 from typing import Dict, Tuple, List, Set, Union
 from abc import ABC, abstractmethod
 
 import pydantic.v1 as pydantic
 import numpy as np
@@ -14,15 +15,15 @@
 from .base import cached_property
 from .base import skip_if_fields_missing
 from .validators import assert_objects_in_sim_bounds
 from .validators import validate_mode_objects_symmetry
 from .geometry.base import Geometry, Box
 from .geometry.mesh import TriangleMesh
 from .geometry.utils import flatten_groups, traverse_geometries
-from .geometry.utils_2d import get_bounds, increment_float, set_bounds, get_thickened_geom
+from .geometry.utils_2d import get_bounds, get_thickened_geom
 from .geometry.utils_2d import subdivide, snap_coordinate_to_grid
 from .types import Ax, FreqBound, Axis, annotate_type, InterpMethod, Symmetry
 from .types import Literal, TYPE_TAG_STR
 from .grid.grid import Coords1D, Grid, Coords
 from .grid.grid_spec import GridSpec, UniformGrid, AutoGrid, CustomGrid
 from .grid.grid_spec import ConformalMeshSpecType, StaircasingConformalMeshSpec
 from .medium import MediumType, AbstractMedium
@@ -30,23 +31,23 @@
 from .medium import AnisotropicMedium, FullyAnisotropicMedium, AbstractPerturbationMedium
 from .boundary import BoundarySpec, BlochBoundary, PECBoundary, PMCBoundary, Periodic, Boundary
 from .boundary import PML, StablePML, Absorber, AbsorberSpec
 from .structure import Structure, MeshOverrideStructure
 from .source import SourceType, PlaneWave, GaussianBeam, AstigmaticGaussianBeam, CustomFieldSource
 from .source import CustomCurrentSource, CustomSourceTime, ContinuousWave
 from .source import TFSF, Source, ModeSource
-from .monitor import MonitorType, Monitor, FreqMonitor, SurfaceIntegrationMonitor
+from .monitor import ModeMonitor, MonitorType, Monitor, FreqMonitor, SurfaceIntegrationMonitor
 from .monitor import AbstractModeMonitor, FieldMonitor, TimeMonitor, FieldTimeMonitor
 from .monitor import PermittivityMonitor, DiffractionMonitor, AbstractFieldProjectionMonitor
 from .monitor import FieldProjectionAngleMonitor, FieldProjectionKSpaceMonitor
 from .lumped_element import LumpedElementType, LumpedResistor
 from .data.dataset import Dataset, CustomSpatialDataType
 from .viz import add_ax_if_none, equal_aspect
 from .scene import Scene, MAX_NUM_MEDIUMS
-
+from .run_time_spec import RunTimeSpec
 from .viz import PlotParams
 from .viz import plot_params_pml, plot_params_override_structures
 from .viz import plot_params_pec, plot_params_pmc, plot_params_bloch, plot_sim_3d
 
 from ..constants import C_0, SECOND, fp_eps, inf
 from ..exceptions import SetupError, ValidationError, Tidy3dError, Tidy3dImportError
 from ..log import log
@@ -1187,15 +1188,15 @@
             return dls
 
         def snap_to_grid(geom: Geometry, axis: Axis) -> Geometry:
             """Snap a 2D material to the Yee grid."""
             center = get_bounds(geom, axis)[0]
             assert get_bounds(geom, axis)[0] == get_bounds(geom, axis)[1]
             snapped_center = snap_coordinate_to_grid(self.grid, center, axis)
-            return set_bounds(geom, (snapped_center, snapped_center), axis)
+            return geom._update_from_bounds(bounds=(snapped_center, snapped_center), axis=axis)
 
         lumped_structures = []
         for lumped_element in self.lumped_elements:
             _, tan_dirs = self.pop_axis([0, 1, 2], axis=lumped_element.normal_axis)
 
             if isinstance(lumped_element, LumpedResistor):
                 conductivity = lumped_element.sheet_conductance
@@ -1241,42 +1242,31 @@
             axis = structure.geometry._normal_2dmaterial
             geometry = structure.geometry
 
             # subdivide
             avg_axis_dl = get_dls(geometry, axis, 1)[0]
             subdivided_geometries = subdivide(geometry, axis, avg_axis_dl, background_structures)
             # Create and add volumetric equivalents
-            background_structures_temp = []
             for subdivided_geometry in subdivided_geometries:
                 # Snap to the grid and create volumetric equivalent
                 snapped_geometry = snap_to_grid(subdivided_geometry[0], axis)
                 snapped_center = get_bounds(snapped_geometry, axis)[0]
                 dls = get_dls(get_thickened_geom(snapped_geometry, axis, avg_axis_dl), axis, 2)
                 adjacent_media = [subdivided_geometry[1].medium, subdivided_geometry[2].medium]
 
                 # Create the new volumetric medium
                 new_medium = structure.medium.volumetric_equivalent(
                     axis=axis, adjacent_media=adjacent_media, adjacent_dls=dls
                 )
 
-                new_bounds = (snapped_center - dls[0] / 2, snapped_center + dls[1] / 2)
-                temp_geometry = set_bounds(snapped_geometry, bounds=new_bounds, axis=axis)
-                temp_structure = structure.updated_copy(geometry=temp_geometry, medium=new_medium)
-
-                if structure.medium.is_pec:
-                    pec_plus = increment_float(snapped_center, 1.0)
-                    pec_minus = increment_float(snapped_center, -1.0)
-                    new_bounds = (pec_minus, pec_plus)
-                new_geometry = set_bounds(snapped_geometry, bounds=new_bounds, axis=axis)
+                new_bounds = (snapped_center, snapped_center)
+                new_geometry = snapped_geometry._update_from_bounds(bounds=new_bounds, axis=axis)
                 new_structure = structure.updated_copy(geometry=new_geometry, medium=new_medium)
 
                 new_structures.append(new_structure)
-                background_structures_temp.append(temp_structure)
-
-            background_structures += background_structures_temp
 
         return tuple(new_structures)
 
     @cached_property
     def volumetric_structures(self) -> Tuple[Structure]:
         """Generate a tuple of structures wherein any 2D materials are converted to 3D
         volumetric equivalents."""
@@ -1964,20 +1954,24 @@
 
     .. image:: ../../notebooks/img/pec_pmc.png
 
 
     .. TODO maybe resize?
     """
 
-    run_time: pydantic.PositiveFloat = pydantic.Field(
+    # TODO: at a later time (once well tested) we could consider making default of RunTimeSpec()
+    run_time: Union[pydantic.PositiveFloat, RunTimeSpec] = pydantic.Field(
         ...,
         title="Run Time",
         description="Total electromagnetic evolution time in seconds. "
         "Note: If simulation 'shutoff' is specified, "
-        "simulation will terminate early when shutoff condition met. ",
+        "simulation will terminate early when shutoff condition met. "
+        "Alternatively, user may supply a :class:`RunTimeSpec` to this field, which will auto-"
+        "compute the ``run_time`` based on the contents of the spec. If this option is used, "
+        "the evaluated ``run_time`` value is available in the ``Simulation._run_time`` property.",
         units=SECOND,
     )
     """
     Total electromagnetic evolution time in seconds. If simulation 'shutoff' is specified, simulation will
     terminate early when shutoff condition met.
 
     **How long to run a simulation?**
@@ -2490,23 +2484,38 @@
             ),
             medium=values.get("medium"),
         )
 
         structures = values.get("structures") or []
         total_structures = [structure_bg] + list(structures)
 
-        for monitor in val:
-            if isinstance(monitor, (AbstractFieldProjectionMonitor, DiffractionMonitor)):
-                mediums = Scene.intersecting_media(monitor, total_structures)
-                # make sure there is no more than one medium in the returned list
-                if len(mediums) > 1:
-                    raise SetupError(
-                        f"{len(mediums)} different mediums detected on plane "
-                        f"intersecting a {monitor.type}. Plane must be homogeneous."
-                    )
+        with log as consolidated_logger:
+            for monitor_ind, monitor in enumerate(val):
+                if isinstance(monitor, (AbstractFieldProjectionMonitor, DiffractionMonitor)):
+                    mediums = Scene.intersecting_media(monitor, total_structures)
+                    # make sure there is no more than one medium in the returned list
+                    if len(mediums) > 1:
+                        raise SetupError(
+                            f"{len(mediums)} different mediums detected on plane "
+                            f"intersecting a {monitor.type}. Plane must be homogeneous."
+                        )
+                    # 0 medium, something is wrong
+                    if len(mediums) < 1:
+                        raise SetupError(
+                            f"No medium detected on plane intersecting a {monitor.type}, "
+                            "indicating an unexpected error. Please create a github issue so "
+                            "that the problem can be investigated."
+                        )
+                    # 1 medium, check if the medium is spatially uniform
+                    if not list(mediums)[0].is_spatially_uniform:
+                        consolidated_logger.warning(
+                            f"Nonuniform custom medium detected on plane intersecting a {monitor.type}. "
+                            "Plane must be homogeneous. Make sure custom medium is uniform on the plane.",
+                            custom_loc=["monitors", monitor_ind],
+                        )
 
         return val
 
     @pydantic.validator("monitors", always=True)
     def _projection_direction(cls, val, values):
         """Warn if field projection observation points are behind surface projection monitors."""
         # This validator is in simulation.py rather than monitor.py because volume monitors are
@@ -2751,31 +2760,45 @@
             medium=values.get("medium"),
         )
 
         structures = values.get("structures") or []
         total_structures = [structure_bg] + list(structures)
 
         # for each plane wave in the sources list
-        for source in val:
-            if isinstance(source, (PlaneWave, GaussianBeam, AstigmaticGaussianBeam)):
-                mediums = Scene.intersecting_media(source, total_structures)
-                # make sure there is no more than one medium in the returned list
-                if len(mediums) > 1:
-                    raise SetupError(
-                        f"{len(mediums)} different mediums detected on plane "
-                        f"intersecting a {source.type} source. Plane must be homogeneous."
-                    )
-                if len(mediums) == 1 and isinstance(
-                    list(mediums)[0], (AnisotropicMedium, FullyAnisotropicMedium)
-                ):
-                    raise SetupError(
-                        f"An anisotropic medium is detected on plane intersecting a {source.type} "
-                        f"source. Injection of {source.type} into anisotropic media currently is "
-                        "not supported."
-                    )
+        with log as consolidated_logger:
+            for source_id, source in enumerate(val):
+                if isinstance(source, (PlaneWave, GaussianBeam, AstigmaticGaussianBeam)):
+                    mediums = Scene.intersecting_media(source, total_structures)
+                    # make sure there is no more than one medium in the returned list
+                    if len(mediums) > 1:
+                        raise SetupError(
+                            f"{len(mediums)} different mediums detected on plane "
+                            f"intersecting a {source.type} source. Plane must be homogeneous."
+                        )
+                    # 0 medium, something is wrong
+                    if len(mediums) < 1:
+                        raise SetupError(
+                            f"No medium detected on plane intersecting a {source.type}, "
+                            "indicating an unexpected error. Please create a github issue so "
+                            "that the problem can be investigated."
+                        )
+                    if isinstance(list(mediums)[0], (AnisotropicMedium, FullyAnisotropicMedium)):
+                        raise SetupError(
+                            f"An anisotropic medium is detected on plane intersecting a {source.type} "
+                            f"source. Injection of {source.type} into anisotropic media currently is "
+                            "not supported."
+                        )
+
+                    # check if the medium is spatially uniform
+                    if not list(mediums)[0].is_spatially_uniform:
+                        consolidated_logger.warning(
+                            f"Nonuniform custom medium detected on plane intersecting a {source.type}. "
+                            "Plane must be homogeneous. Make sure custom medium is uniform on the plane.",
+                            custom_loc=["sources", source_id],
+                        )
 
         return val
 
     @pydantic.validator("normalize_index", always=True)
     @skip_if_fields_missing(["sources"])
     def _check_normalize_index(cls, val, values):
         """Check validity of normalize index in context of simulation.sources."""
@@ -2912,14 +2935,15 @@
         source_required: bool = True
             If ``True``, validation will fail in case no sources are found in the simulation.
         """
         log.begin_capture()
         self._validate_size()
         self._validate_monitor_size()
         self._validate_modes_size()
+        self._validate_num_cells_in_mode_objects()
         self._validate_datasets_not_none()
         self._validate_tfsf_structure_intersections()
         self._warn_time_monitors_outside_run_time()
         self._validate_time_monitors_num_steps()
         _ = self.volumetric_structures
         log.end_capture(self)
         if source_required and len(self.sources) == 0:
@@ -3027,14 +3051,44 @@
         with log as consolidated_logger:
             for mnt_ind, monitor in enumerate(self.monitors):
                 if isinstance(monitor, AbstractModeMonitor):
                     msg_header = f"Mode monitor '{monitor.name}' "
                     custom_loc = ["monitors", mnt_ind]
                     warn_mode_size(monitor=monitor, msg_header=msg_header, custom_loc=custom_loc)
 
+    def _validate_num_cells_in_mode_objects(self) -> None:
+        """Raise an error if mode sources or monitors intersect with a very small number
+        of grid cells in their transverse dimensions."""
+
+        def check_num_cells(
+            mode_object: Tuple[ModeSource, ModeMonitor], normal_axis: Axis, msg_header: str
+        ):
+            disc_grid = self.discretize(mode_object)
+            _, check_axes = Box.pop_axis([0, 1, 2], axis=normal_axis)
+            for axis in check_axes:
+                sim_size = self.size[axis]
+                dim_cells = disc_grid.num_cells[axis]
+                if sim_size > 0 and dim_cells <= 2:
+                    small_dim = "xyz"[axis]
+                    raise SetupError(
+                        msg_header + f"is too small along the "
+                        f"'{small_dim}' axis. Less than '3' grid cells were detected. "
+                        f"Increase the size of the object along '{small_dim}'."
+                    )
+
+        for source in self.sources:
+            if isinstance(source, ModeSource):
+                msg_header = f"Mode source '{source.name}' "
+                check_num_cells(source, source.injection_axis, msg_header)
+
+        for monitor in self.monitors:
+            if isinstance(monitor, ModeMonitor):
+                msg_header = f"Mode monitor '{monitor.name}' "
+                check_num_cells(monitor, monitor.normal_axis, msg_header)
+
     def _validate_time_monitors_num_steps(self) -> None:
         """Raise an error if non-0D time monitors have too many time steps."""
         for monitor in self.monitors:
             if not isinstance(monitor, FieldTimeMonitor) or len(monitor.zero_dims) == 3:
                 continue
             num_time_steps = monitor.num_steps(self.tmesh)
             if num_time_steps > MAX_TIME_MONITOR_STEPS:
@@ -3149,22 +3203,59 @@
         TODO: (remove this comment later) this is done as a pre-upload validator in view of a
         planned change to allow ``run_time`` to accept a ``RunTimeSpec`` which would automatically
         determine a run time based on simulation details. Then, we would have to access the
         dynamically computed run_time e.g. through a ``_run_time`` cached property.
         """
         with log as consolidated_logger:
             for monitor in self.monitors:
-                if isinstance(monitor, TimeMonitor) and monitor.start > self.run_time:
+                if isinstance(monitor, TimeMonitor) and monitor.start > self._run_time:
                     consolidated_logger.warning(
                         f"Monitor {monitor.name} has a start time {monitor.start:1.2e}s exceeding"
-                        f"the simulation run time {self.run_time:1.2e}s. No data will be recorded."
+                        f"the simulation run time {self._run_time:1.2e}s. No data will be recorded."
                     )
 
     """ Accounting """
 
+    @cached_property
+    def _run_time(self) -> float:
+        """Run time evaluated based on self.run_time."""
+
+        if not isinstance(self.run_time, RunTimeSpec):
+            return self.run_time
+
+        run_time_spec = self.run_time
+
+        # contribution from the time of of the source pulses
+        if not self.sources:
+            source_time = 0.0
+        else:
+            source_times = [src.source_time.end_time() for src in self.sources]
+            source_times = [x for x in source_times if x is not None]
+            if not source_times:
+                raise SetupError(
+                    "Could not compute source contributions to run time from 'RunTimeSpec'."
+                    "Please check all of your 'Source.source_time' and ensure that at least one "
+                    "has a decaying (non-DC) pulse profile to be able to compute the 'run_time'."
+                )
+            source_time_max = np.max(source_times)
+            source_time = run_time_spec.source_factor * source_time_max
+
+        # contribution from field decay out of the simulation
+        propagation_lengths = np.array(self.bounds[1]) - np.array(self.bounds[0])
+        max_propagation_length = np.max(propagation_lengths)
+
+        # get the maximum refractive index evaluated over each of all the source central frequencies
+        all_ref_inds = [self.get_refractive_indices(src.source_time.freq0) for src in self.sources]
+        avg_ref_inds = [np.mean(n) for n in all_ref_inds]
+        max_ref_ind = np.max(avg_ref_inds)
+
+        propagation_time = run_time_spec.quality_factor * max_ref_ind * max_propagation_length / C_0
+
+        return source_time + propagation_time
+
     # candidate for removal in 3.0
     @cached_property
     def mediums(self) -> Set[MediumType]:
         """Returns set of distinct :class:`.AbstractMedium` in simulation.
 
         Returns
         -------
@@ -3343,27 +3434,30 @@
         ----------
         x : float = None
             Position of plane in x direction, only one of x,y,z can be specified to define plane.
         y : float = None
             Position of plane in y direction, only one of x,y,z can be specified to define plane.
         z : float = None
             Position of plane in z direction, only one of x,y,z can be specified to define plane.
-        permittivity_threshold : float = 1.001
-            Permitivitty value used to define the shape boundaries for structures with custom
+        permittivity_threshold : float = 1
+            Permittivity value used to define the shape boundaries for structures with custom
             medim
         frequency : float = 0
-            Frequency for permittivity evaluaiton in case of custom medium (Hz).
+            Frequency for permittivity evaluation in case of custom medium (Hz).
         gds_layer_dtype_map : Dict
             Dictionary mapping mediums to GDSII layer and data type tuples.
 
         Return
         ------
         List
             List of `gdstk.Polygon`.
         """
+        if gds_layer_dtype_map is None:
+            gds_layer_dtype_map = {}
+
         axis, _ = self.geometry.parse_xyz_kwargs(x=x, y=y, z=z)
         _, bmin = self.pop_axis(self.bounds[0], axis)
         _, bmax = self.pop_axis(self.bounds[1], axis)
 
         _, symmetry = self.pop_axis(self.symmetry, axis)
         if symmetry[0] != 0:
             bmin = (0, bmin[1])
@@ -3416,14 +3510,17 @@
             Dictionary mapping mediums to GDSII layer and data type tuples.
 
         Return
         ------
         List
             List of `gdspy.Polygon` and `gdspy.PolygonSet`.
         """
+        if gds_layer_dtype_map is None:
+            gds_layer_dtype_map = {}
+
         axis, _ = self.geometry.parse_xyz_kwargs(x=x, y=y, z=z)
         _, bmin = self.pop_axis(self.bounds[0], axis)
         _, bmax = self.pop_axis(self.bounds[1], axis)
 
         _, symmetry = self.pop_axis(self.symmetry, axis)
         if symmetry[0] != 0:
             bmin = (0, bmin[1])
@@ -3469,19 +3566,19 @@
             Cell object to which the generated polygons are added.
         x : float = None
             Position of plane in x direction, only one of x,y,z can be specified to define plane.
         y : float = None
             Position of plane in y direction, only one of x,y,z can be specified to define plane.
         z : float = None
             Position of plane in z direction, only one of x,y,z can be specified to define plane.
-        permittivity_threshold : float = 1.001
-            Permitivitty value used to define the shape boundaries for structures with custom
+        permittivity_threshold : float = 1
+            Permittivity value used to define the shape boundaries for structures with custom
             medim
         frequency : float = 0
-            Frequency for permittivity evaluaiton in case of custom medium (Hz).
+            Frequency for permittivity evaluation in case of custom medium (Hz).
         gds_layer_dtype_map : Dict
             Dictionary mapping mediums to GDSII layer and data type tuples.
         """
         if gds_layer_dtype_map is None:
             gds_layer_dtype_map = {}
 
         if gdstk_available and isinstance(cell, gdstk.Cell):
@@ -3535,19 +3632,19 @@
             Full path to the .gds file to save the :class:`Simulation` slice to.
         x : float = None
             Position of plane in x direction, only one of x,y,z can be specified to define plane.
         y : float = None
             Position of plane in y direction, only one of x,y,z can be specified to define plane.
         z : float = None
             Position of plane in z direction, only one of x,y,z can be specified to define plane.
-        permittivity_threshold : float = 1.001
-            Permitivitty value used to define the shape boundaries for structures with custom
+        permittivity_threshold : float = 1
+            Permittivity value used to define the shape boundaries for structures with custom
             medim
         frequency : float = 0
-            Frequency for permittivity evaluaiton in case of custom medium (Hz).
+            Frequency for permittivity evaluation in case of custom medium (Hz).
         gds_layer_dtype_map : Dict
             Dictionary mapping mediums to GDSII layer and data type tuples.
         gds_cell_name : str = 'MAIN'
             Name of the cell created in the .gds file to store the geometry.
         """
         if gdstk_available:
             library = gdstk.Library()
@@ -3649,15 +3746,15 @@
 
         Returns
         -------
         np.ndarray
             Times (seconds) that the simulation time steps through.
         """
         dt = self.dt
-        return np.arange(0.0, self.run_time + dt, dt)
+        return np.arange(0.0, self._run_time + dt, dt)
 
     @cached_property
     def num_time_steps(self) -> int:
         """Number of time steps in simulation."""
 
         return len(self.tmesh)
 
@@ -3722,28 +3819,80 @@
                 coords_all[axis] = volumetric_grid.boundaries.to_list[axis]
             else:
                 coords_all[axis] = grid.boundaries.to_list[axis]
 
         return Grid(boundaries=Coords(**dict(zip("xyz", coords_all))))
 
     @cached_property
+    def grid(self) -> Grid:
+        """FDTD grid spatial locations and information.
+
+        Returns
+        -------
+        :class:`.Grid`
+            :class:`.Grid` storing the spatial locations relevant to the simulation.
+        """
+
+        # Add a simulation Box as the first structure
+        structures = [Structure(geometry=self.geometry, medium=self.medium)]
+        structures += self.structures
+
+        grid = self.grid_spec.make_grid(
+            structures=structures,
+            symmetry=self.symmetry,
+            periodic=self._periodic,
+            sources=self.sources,
+            num_pml_layers=self.num_pml_layers,
+        )
+
+        # This would AutoGrid the in-plane directions of the 2D materials
+        # return self._grid_corrections_2dmaterials(grid)
+        return grid
+
+    @cached_property
+    def num_cells(self) -> int:
+        """Number of cells in the simulation.
+
+        Returns
+        -------
+        int
+            Number of yee cells in the simulation.
+        """
+
+        return np.prod(self.grid.num_cells, dtype=np.int64)
+
+    def get_refractive_indices(self, freq: float) -> list[float]:
+        """List of refractive indices in the simulation at a given frequency."""
+
+        eps_values = [structure.medium.eps_model(freq) for structure in self.structures]
+        eps_values.append(self.medium.eps_model(freq))
+
+        return [AbstractMedium.eps_complex_to_nk(eps)[0] for eps in eps_values]
+
+    @cached_property
+    def n_max(self) -> float:
+        """Maximum refractive index in the ``Simulation``."""
+        eps_max = max(abs(struct.medium.eps_model(self.freq_max)) for struct in self.all_structures)
+        n_max, _ = AbstractMedium.eps_complex_to_nk(eps_max)
+        return n_max
+
+    @cached_property
     def wvl_mat_min(self) -> float:
-        """Minimum wavelength in the material.
+        """Minimum wavelength in the materials present throughout the simulation.
 
         Returns
         -------
         float
             Minimum wavelength in the material (microns).
         """
         freq_max = max(source.source_time.freq0 for source in self.sources)
         wvl_min = C_0 / freq_max
 
-        all_structures = self.all_structures
-        eps_max = max(abs(structure.medium.eps_model(freq_max)) for structure in all_structures)
-        n_max, _ = AbstractMedium.eps_complex_to_nk(eps_max)
+        n_values = self.get_refractive_indices(freq_max)
+        n_max = max(n_values)
         return wvl_min / n_max
 
     @cached_property
     def complex_fields(self) -> bool:
         """Whether complex fields are used in the simulation. Currently this only happens when there
         are Bloch boundaries.
 
@@ -3896,37 +4045,43 @@
         # spatially dependent mediums by selecting minimal amount of heat and charge data points
         # covering the structure, and create a new structure containing the resulting custom medium
         new_structures = []
         for s_ind, structure in enumerate(structures):
             med = structure.medium
             if isinstance(med, AbstractPerturbationMedium):
                 # get structure's bounding box
-                s_bounds = structure.geometry.bounds
+                s_bounds = np.array(structure.geometry.bounds)
 
                 bounds = [
                     np.max([sim_bounds[0], s_bounds[0]], axis=0),
                     np.min([sim_bounds[1], s_bounds[1]], axis=0),
                 ]
 
-                # for each structure select a minimal subset of data that covers it
-                restricted_arrays = {}
+                # skip structure if it's completely outside of sim box
+                if any(bmin > bmax for bmin, bmax in zip(*bounds)):
+                    new_structures.append(structure)
+                else:
+                    # for each structure select a minimal subset of data that covers it
+                    restricted_arrays = {}
 
-                for name, array in array_dict.items():
-                    if array is not None:
-                        restricted_arrays[name] = array.sel_inside(bounds)
-
-                        # check provided data fully cover structure
-                        if not array.does_cover(bounds):
-                            log.warning(
-                                f"Provided '{name}' does not fully cover structures[{s_ind}]."
-                            )
+                    for name, array in array_dict.items():
+                        if array is not None:
+                            restricted_arrays[name] = array.sel_inside(bounds)
+
+                            # check provided data fully cover structure
+                            if not array.does_cover(bounds):
+                                log.warning(
+                                    f"Provided '{name}' does not fully cover structures[{s_ind}]."
+                                )
 
-                new_medium = med.perturbed_copy(**restricted_arrays, interp_method=interp_method)
-                new_structure = structure.updated_copy(medium=new_medium)
-                new_structures.append(new_structure)
+                    new_medium = med.perturbed_copy(
+                        **restricted_arrays, interp_method=interp_method
+                    )
+                    new_structure = structure.updated_copy(medium=new_medium)
+                    new_structures.append(new_structure)
             else:
                 new_structures.append(structure)
 
         sim_dict["structures"] = new_structures
 
         # do the same for background medium if it a medium with perturbation models.
         med = self.medium
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/source.py` & `tidy3d-2.7.0rc2/tidy3d/components/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 # when checking if custom data spans the source plane, allow for a small tolerance
 # due to numerical precision
 DATA_SPAN_TOL = 1e-8
 # width of Chebyshev grid used for broadband sources (in units of pulse width)
 CHEB_GRID_WIDTH = 1.5
 # Number of frequencies in a broadband source above which to issue a warning
 WARN_NUM_FREQS = 20
+# how many units of ``twidth`` from the ``offset`` until a gaussian pulse is considered "off"
+END_TIME_FACTOR_GAUSSIAN = 10
 
 
 class SourceTime(AbstractTimeDependence):
     """Base class describing the time dependence of a source."""
 
     @add_ax_if_none
     def plot_spectrum(
@@ -74,14 +76,18 @@
             times, fmin, fmax, num_freqs=num_freqs, val=val, ax=ax
         )
 
     @abstractmethod
     def frequency_range(self, num_fwidth: float = 4.0) -> FreqBound:
         """Frequency range within plus/minus ``num_fwidth * fwidth`` of the central frequency."""
 
+    @abstractmethod
+    def end_time(self) -> float | None:
+        """Time after which the source is effectively turned off / close to zero amplitude."""
+
 
 class Pulse(SourceTime, ABC):
     """A source time that ramps up with some ``fwidth`` and oscillates at ``freq0``."""
 
     freq0: pydantic.PositiveFloat = pydantic.Field(
         ..., title="Central Frequency", description="Central frequency of the pulse.", units=HERTZ
     )
@@ -96,14 +102,19 @@
         5.0,
         title="Offset",
         description="Time delay of the maximum value of the "
         "pulse in units of 1 / (``2pi * fwidth``).",
         ge=2.5,
     )
 
+    @property
+    def twidth(self) -> float:
+        """Width of pulse in seconds."""
+        return 1.0 / (2 * np.pi * self.fwidth)
+
     def frequency_range(self, num_fwidth: float = 4.0) -> FreqBound:
         """Frequency range within 5 standard deviations of the central frequency.
 
         Parameters
         ----------
         num_fwidth : float = 4.
             Frequency range defined as plus/minus ``num_fwidth * self.fwdith``.
@@ -139,33 +150,41 @@
         "near zero frequency. Setting this to ``False`` results in an unmodified Gaussian "
         "pulse spectrum which can have a nonzero DC component.",
     )
 
     def amp_time(self, time: float) -> complex:
         """Complex-valued source amplitude as a function of time."""
 
-        twidth = 1.0 / (2 * np.pi * self.fwidth)
         omega0 = 2 * np.pi * self.freq0
-        time_shifted = time - self.offset * twidth
+        time_shifted = time - self.offset * self.twidth
 
         offset = np.exp(1j * self.phase)
         oscillation = np.exp(-1j * omega0 * time)
-        amp = np.exp(-(time_shifted**2) / 2 / twidth**2) * self.amplitude
+        amp = np.exp(-(time_shifted**2) / 2 / self.twidth**2) * self.amplitude
 
         pulse_amp = offset * oscillation * amp
 
         # subtract out DC component
         if self.remove_dc_component:
-            pulse_amp = pulse_amp * (1j + time_shifted / twidth**2 / omega0)
+            pulse_amp = pulse_amp * (1j + time_shifted / self.twidth**2 / omega0)
         else:
             # 1j to make it agree in large omega0 limit
             pulse_amp = pulse_amp * 1j
 
         return pulse_amp
 
+    def end_time(self) -> float | None:
+        """Time after which the source is effectively turned off / close to zero amplitude."""
+
+        # TODO: decide if we should continue to return an end_time if the DC component remains
+        # if not self.remove_dc_component:
+        #     return None
+
+        return self.offset * self.twidth + END_TIME_FACTOR_GAUSSIAN * self.twidth
+
 
 class ContinuousWave(Pulse):
     """Source time dependence that ramps up to continuous oscillation
     and holds until end of simulation.
 
     Note
     ----
@@ -187,14 +206,18 @@
         const = 1.0
         offset = np.exp(1j * self.phase)
         oscillation = np.exp(-1j * omega0 * time)
         amp = 1 / (1 + np.exp(-time_shifted / twidth)) * self.amplitude
 
         return const * offset * oscillation * amp
 
+    def end_time(self) -> float | None:
+        """Time after which the source is effectively turned off / close to zero amplitude."""
+        return None
+
 
 class CustomSourceTime(Pulse):
     """Custom source time dependence consisting of a real or complex envelope
     modulated at a central frequency, as shown below.
 
     Note
     ----
@@ -326,14 +349,28 @@
         omega0 = 2 * np.pi * self.freq0
         offset = np.exp(1j * self.phase)
         oscillation = np.exp(-1j * omega0 * time)
         amp = self.amplitude
 
         return offset * oscillation * amp * envelope
 
+    def end_time(self) -> float | None:
+        """Time after which the source is effectively turned off / close to zero amplitude."""
+
+        if self.source_time_dataset is None:
+            return None
+
+        data_array = self.source_time_dataset.values
+
+        t_coords = data_array.coords["t"]
+        source_is_non_zero = ~np.isclose(abs(data_array), 0)
+        t_non_zero = t_coords[source_is_non_zero]
+
+        return np.max(t_non_zero)
+
 
 SourceTimeType = Union[GaussianPulse, ContinuousWave, CustomSourceTime]
 
 """ Source objects """
 
 
 class Source(Box, AbstractSource, ABC):
@@ -374,15 +411,15 @@
 
     @pydantic.validator("source_time", always=True)
     def _freqs_lower_bound(cls, val):
         """Raise validation error if central frequency is too low."""
         _assert_min_freq(val.freq0, msg_start="'source_time.freq0'")
         return val
 
-    def plot(  #  pylint:disable=too-many-arguments
+    def plot(
         self,
         x: float = None,
         y: float = None,
         z: float = None,
         ax: Ax = None,
         **patch_kwargs,
     ) -> Ax:
@@ -812,34 +849,49 @@
                 custom_loc=["angle_theta"],
             )
         return val
 
     @cached_property
     def _dir_vector(self) -> Tuple[float, float, float]:
         """Source direction normal vector in cartesian coordinates."""
+
+        # Propagation vector assuming propagation along z
         radius = 1.0 if self.direction == "+" else -1.0
         dx = radius * np.cos(self.angle_phi) * np.sin(self.angle_theta)
         dy = radius * np.sin(self.angle_phi) * np.sin(self.angle_theta)
         dz = radius * np.cos(self.angle_theta)
+
+        # Move to original injection axis
         return self.unpop_axis(dz, (dx, dy), axis=self._injection_axis)
 
     @cached_property
     def _pol_vector(self) -> Tuple[float, float, float]:
         """Source polarization normal vector in cartesian coordinates."""
-        normal_dir = [0.0, 0.0, 0.0]
-        normal_dir[int(self._injection_axis)] = 1.0
-        propagation_dir = list(self._dir_vector)
-        if self.angle_theta == 0.0:
-            pol_vector_p = np.array((0, 1, 0)) if self._injection_axis == 0 else np.array((1, 0, 0))
-            pol_vector_p = self.rotate_points(pol_vector_p, normal_dir, angle=self.angle_phi)
-        else:
-            pol_vector_s = np.cross(normal_dir, propagation_dir)
-            pol_vector_p = np.cross(propagation_dir, pol_vector_s)
-            pol_vector_p = np.array(pol_vector_p) / np.linalg.norm(pol_vector_p)
-        return self.rotate_points(pol_vector_p, propagation_dir, angle=self.pol_angle)
+
+        # Polarization vector assuming propagation along z
+        pol_vector_z_normal = np.array([1.0, 0.0, 0.0])
+
+        # Rotate polarization
+        pol_vector_z_normal = self.rotate_points(
+            pol_vector_z_normal, axis=[0, 0, 1], angle=self.pol_angle
+        )
+
+        # Rotate the fields back to the original propagation axes
+        pol_vector_z_normal = self.rotate_points(
+            pol_vector_z_normal, axis=[0, 1, 0], angle=self.angle_theta
+        )
+        pol_vector_z_normal = self.rotate_points(
+            pol_vector_z_normal, axis=[0, 0, 1], angle=self.angle_phi
+        )
+
+        # Move to original injection axis
+        pol_vector = self.unpop_axis(
+            pol_vector_z_normal[2], pol_vector_z_normal[:2], axis=self._injection_axis
+        )
+        return pol_vector
 
 
 class ModeSource(DirectionalSource, PlanarSource, BroadbandSource):
     """Injects current source to excite modal profile on finite extent plane.
 
     Notes
     -----
@@ -1090,15 +1142,15 @@
         """Center of the injection plane."""
         sign = 1 if self.direction == "-" else -1
         center = list(self.center)
         size = [0 if val == inf else val for val in self.size]
         center[self.injection_axis] += sign * size[self.injection_axis] / 2
         return tuple(center)
 
-    def plot(  #  pylint:disable=too-many-arguments
+    def plot(
         self,
         x: float = None,
         y: float = None,
         z: float = None,
         ax: Ax = None,
         **patch_kwargs,
     ) -> Ax:
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/structure.py` & `tidy3d-2.7.0rc2/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/time.py` & `tidy3d-2.7.0rc2/tidy3d/components/time.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/time_modulation.py` & `tidy3d-2.7.0rc2/tidy3d/components/time_modulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/transformation.py` & `tidy3d-2.7.0rc2/tidy3d/components/transformation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/types.py` & `tidy3d-2.7.0rc2/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/validators.py` & `tidy3d-2.7.0rc2/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/components/viz.py` & `tidy3d-2.7.0rc2/tidy3d/components/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             if key not in ("type",) and value is not None and key in self.__fields__
         }
         return self.copy(update=update_dict)
 
     def to_kwargs(self) -> dict:
         """Export the plot parameters as kwargs dict that can be supplied to plot function."""
         kwarg_dict = self.dict()
-        for ignore_key in ("type",):
+        for ignore_key in ("type", "attrs"):
             kwarg_dict.pop(ignore_key)
         return kwarg_dict
 
 
 # defaults for different tidy3d objects
 plot_params_geometry = PlotParams()
 plot_params_structure = PlotParams()
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/config.py` & `tidy3d-2.7.0rc2/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/constants.py` & `tidy3d-2.7.0rc2/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/exceptions.py` & `tidy3d-2.7.0rc2/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/log.py` & `tidy3d-2.7.0rc2/tidy3d/log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/material_library/material_library.py` & `tidy3d-2.7.0rc2/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/material_library/material_reference.py` & `tidy3d-2.7.0rc2/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.7.0rc2/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/packaging.py` & `tidy3d-2.7.0rc2/tidy3d/packaging.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/README.md` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 ### The One Exception: `DataArrays`
 
 Unfortunately, all `Tidy3D` components are not handled so simply. It turns out that `jax` datastructures do not work when added to `xarray.DataArray` containers. Therefore, we needed to find a replacement to the `DataArray` class in regular Tidy3D to use in our `JaxMonitorData` fields. To solve this problem, the adjoint plugin introduces a `JaxDataArray`, which stores `.values` as a `jax` `Array` (basically a `jax` version of `numpy` arrays) and `.coords` as a dictionary of coordinates with a dimensions string mapping to a list of values. 
 
 The `JaxDataArray` may freely store `jax` values and tracers and implements a few basic emulations of `xarray.DataArray` objects, such as `.sel` and `.isel`. Note that at this time `.interp` is not supported, but I think we could consider implementing it later. A user could, in principle, wrap `.sel` to do the interpolation themselves, but it was not considered at this stage because some trials to implement it myself ended badly.
 
-The `JaxDataArray` inherits directly from `Tidy3DBaseModel` alone and therefore implements its own pytree flattening and unflattening operations. Luckily, these operations are quite trivial. There are also a set of custom validations in the `JaxDataArray` to ensure it is set up and used properly as it does not natively provide nearly as strict argument checking as its `xarray.DataArray` counterparts.
+The `JaxDataArray` inherits directly from `Tidy3dBaseModel` alone and therefore implements its own pytree flattening and unflattening operations. Luckily, these operations are quite trivial. There are also a set of custom validations in the `JaxDataArray` to ensure it is set up and used properly as it does not natively provide nearly as strict argument checking as its `xarray.DataArray` counterparts.
 
 ## Adjoint Method
 
 With an understanding on how `jax` is integrated into the plugin through subclasses of `Tidy3D` components, now we can finish the technical discussion with an overview of how the adjoint components are implemented.
 
 ### Gradient Monitors
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 """Imports for adjoint plugin."""
 
 # import the jax version of tidy3d components
 try:
-    from .components.geometry import JaxBox, JaxPolySlab, JaxGeometryGroup
-    from .components.medium import JaxMedium, JaxAnisotropicMedium, JaxCustomMedium
-    from .components.structure import (
-        JaxStructure,
-        JaxStructureStaticGeometry,
-        JaxStructureStaticMedium,
-    )
-    from .components.simulation import JaxSimulation
-    from .components.data.sim_data import JaxSimulationData
-    from .components.data.monitor_data import JaxModeData
-    from .components.data.dataset import JaxPermittivityDataset
-    from .components.data.data_array import JaxDataArray
+    import jax
+
+    jax.config.update("jax_enable_x64", True)
 except ImportError as e:
     raise ImportError(
         "The 'jax' package is required for adjoint plugin. We were not able to import it. "
         "To get the appropriate packages for your system, install tidy3d using '[jax]' option, "
         "for example: $pip install 'tidy3d[jax]'."
     ) from e
 
-try:
-    from .web import run, run_async
-except ImportError:
-    pass
+from .components.geometry import JaxBox, JaxPolySlab, JaxComplexPolySlab, JaxGeometryGroup
+from .components.medium import JaxMedium, JaxAnisotropicMedium, JaxCustomMedium
+from .components.structure import (
+    JaxStructure,
+    JaxStructureStaticGeometry,
+    JaxStructureStaticMedium,
+)
+from .components.simulation import JaxSimulation
+from .components.data.sim_data import JaxSimulationData
+from .components.data.monitor_data import JaxModeData
+from .components.data.dataset import JaxPermittivityDataset
+from .components.data.data_array import JaxDataArray
+from .web import run, run_async
 
 __all__ = [
     "JaxBox",
     "JaxPolySlab",
+    "JaxComplexPolySlab",
     "JaxGeometryGroup",
     "JaxMedium",
     "JaxAnisotropicMedium",
     "JaxCustomMedium",
     "JaxStructure",
     "JaxStructureStaticMedium",
     "JaxStructureStaticGeometry",
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/__init__.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Component imports for adjoint plugin. from tidy3d.plugins.adjoint.components import *"""
 
 # import the jax version of tidy3d components
-from .geometry import JaxBox, JaxPolySlab
+from .geometry import JaxBox, JaxPolySlab, JaxComplexPolySlab
 from .medium import JaxMedium, JaxAnisotropicMedium, JaxCustomMedium
 from .structure import JaxStructure, JaxStructureStaticMedium, JaxStructureStaticGeometry
 from .simulation import JaxSimulation
 from .data.sim_data import JaxSimulationData
 from .data.monitor_data import JaxModeData
 from .data.dataset import JaxPermittivityDataset
 from .data.data_array import JaxDataArray
 
 __all__ = [
     "JaxBox",
     "JaxPolySlab",
+    "JaxComplexPolySlab",
     "JaxGeometryGroup",
     "JaxMedium",
     "JaxAnisotropicMedium",
     "JaxCustomMedium",
     "JaxStructure",
     "JaxStructureStaticMedium",
     "JaxStructureStaticGeometry",
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Defines jax-compatible DataArrays."""
+
 from __future__ import annotations
 
-from typing import Tuple, Any, Dict, List
+from typing import Tuple, Any, Dict, List, Literal, Sequence, Union
 
 import h5py
 import pydantic.v1 as pd
 import numpy as np
 import jax.numpy as jnp
 import jax
 from jax.tree_util import register_pytree_node_class
@@ -308,38 +309,94 @@
                     f"'isel' kwarg '{coord_name}={coord_index}' is out of range "
                     f"for the coordinate '{coord_name}' with {len(coord_list)} values."
                 )
             self_sel = self_sel.isel_single(coord_name=coord_name, coord_index=coord_index)
 
         return self_sel
 
-    def sel(self, indexers: dict = None, method: str = "nearest", **sel_kwargs) -> JaxDataArray:
-        """Select a value from the :class:`.JaxDataArray` by indexing into coordinate values."""
+    def sel(
+        self, indexers: dict = None, method: Literal[None, "nearest"] = None, **sel_kwargs
+    ) -> JaxDataArray:
+        """Select a value from the :class:`.JaxDataArray` by indexing into coordinates by value.
+
+        Parameters
+        ----------
+        sel_kwargs : dict
+            Keyword arguments with names matching the coordinates of :class:`.JaxDataArray` and values
+            given by scalars or lists, e.g. `da.sel(x=0.1, y=[0.2, 0.3])`.
+        method : Literal[None, "nearest"] = None
+            Method to use for matching coordinate values:
+
+            - None (default): only exact matches
+            - nearest: use nearest valid index value
+
+        Returns
+        -------
+        JaxDataArray
+            JaxDataArray with extracted values.
+        """
+        if method not in [None, "nearest"]:
+            raise NotImplementedError(f"Unkown selection method: {method}.")
+
         isel_kwargs = {}
-        for coord_name, sel_kwarg in sel_kwargs.items():
+        for coord_name, vals in sel_kwargs.items():
             coord_list = self.get_coord_list(coord_name)
-            if isinstance(sel_kwarg, (tuple, list, np.ndarray)):
-                sel_kwarg = list(sel_kwarg)
-                isel_kwargs[coord_name] = []
-                for _sel_kwarg in sel_kwarg:
-                    if _sel_kwarg not in coord_list:
-                        raise DataError(
-                            f"Could not select '{coord_name}={_sel_kwarg}', value not found."
-                        )
-                    coord_index = coord_list.index(_sel_kwarg)
-                    isel_kwargs[coord_name].append(coord_index)
-            else:
-                if sel_kwarg not in coord_list:
-                    raise DataError(
-                        f"Could not select '{coord_name}={sel_kwarg}', value not found."
-                    )
-                coord_index = coord_list.index(sel_kwarg)
-                isel_kwargs[coord_name] = coord_index
+
+            try:  # handle non-numeric types (e.g. str)
+                coord_list = jnp.asarray(coord_list)
+            except TypeError:
+                isel_kwargs[coord_name] = self._indices_literal(coord_list, vals)
+                continue
+
+            vals_ary = jnp.atleast_1d(vals)
+            dist = jnp.abs(coord_list[None] - vals_ary[:, None])
+
+            if method is None:
+                indices = jnp.where(jnp.isclose(dist, 0))[1]
+            elif method == "nearest":
+                indices = jnp.argmin(dist, axis=1)
+
+            if indices.size == 0:
+                raise DataError(
+                    f"Could not select '{coord_name}={vals_ary}', some values were not found."
+                )
+
+            if np.isscalar(vals):
+                indices = jnp.squeeze(indices)
+
+            isel_kwargs[coord_name] = indices
+
         return self.isel(**isel_kwargs)
 
+    def _indices_literal(self, coord_list: list, values: Union[Any, Sequence[Any]]) -> np.ndarray:
+        """Find indices of non-numeric `values` in `coord_list`.
+
+        Parameters
+        ----------
+        coord_list : list
+            List of all entries for a specific coordinate.
+        values : Union[Any, Sequence[Any]]
+            Single value or values of which to find the index of.
+
+        Returns
+        -------
+        numpy.ndarray
+            Indices of `values` in `coord_list`.
+        """
+        indices = []
+        for v in np.atleast_1d(values):
+            if v not in coord_list:
+                raise DataError(f"Could not select '{v}' from '{coord_list}', value not found.")
+            indices.append(coord_list.index(v))
+
+        if np.isscalar(values):
+            indices = np.squeeze(indices)
+
+        return indices
+
     def assign_coords(self, coords: dict = None, **coords_kwargs) -> JaxDataArray:
         """Assign new coordinates to this object."""
 
         update_kwargs = self.coords.copy()
 
         for key, val in coords_kwargs.items():
             update_kwargs[key] = val
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 """Defines jax-compatible geometries and their conversion to grad monitors."""
+
 from __future__ import annotations
 
 from abc import ABC
 from typing import Tuple, Union, Dict, List
-from multiprocessing import Pool
+from joblib import Parallel, delayed
 
 import pydantic.v1 as pd
 import numpy as np
 import xarray as xr
 from jax.tree_util import register_pytree_node_class
 import jax
+import jax.numpy as jnp
+import shapely
 
 from ....components.base import cached_property
 from ....components.types import Bound, Coordinate2D  # , annotate_type
 from ....components.geometry.base import Geometry, Box, GeometryGroup
-from ....components.geometry.polyslab import PolySlab
+from ....components.geometry.polyslab import (
+    PolySlab,
+    _IS_CLOSE_RTOL,
+    _COMPLEX_POLYSLAB_DIVISIONS_WARN,
+)
 from ....components.data.monitor_data import FieldData, PermittivityData
 from ....components.data.data_array import ScalarFieldDataArray
 from ....components.monitor import FieldMonitor, PermittivityMonitor
+from ....components.types import ArrayFloat2D
 from ....constants import fp_eps, MICROMETER
 from ....exceptions import AdjointError
 from ....log import log
+from ...polyslab import ComplexPolySlab
 
 from .base import JaxObject, WEB_ADJOINT_MESSAGE
 from .types import JaxFloat
 
 # number of integration points per unit wavelength in material
 PTS_PER_WVL_INTEGRATION = 50
 
@@ -275,26 +284,45 @@
         "polygon face vertices at the ``reference_plane``. "
         "The index of dimension should be in the ascending order: e.g. if "
         "the slab normal axis is ``axis=y``, the coordinate of the vertices will be in (x, z)",
         units=MICROMETER,
         stores_jax_for="vertices",
     )
 
+    slab_bounds_jax: Tuple[JaxFloat, JaxFloat] = pd.Field(
+        ...,
+        title="Slab bounds (Jax)",
+        description="Jax-traced list of (h1, h2) defining the minimum and maximum positions "
+        "of the slab along the ``axis`` dimension. ",
+        units=MICROMETER,
+        stores_jax_for="slab_bounds",
+    )
+
+    sidewall_angle_jax: JaxFloat = pd.Field(
+        default=0.0,
+        title="Sidewall angle (Jax)",
+        description="Jax-traced float defining the sidewall angle of the slab "
+        "along the ``axis`` dimension. ",
+        units=MICROMETER,
+        stores_jax_for="sidewall_angle",
+    )
+
     @pd.validator("sidewall_angle", always=True)
     def no_sidewall(cls, val):
         """Warn if sidewall angle present."""
         if not np.isclose(val, 0.0):
             log.warning(
                 "'JaxPolySlab' does not yet perform the full adjoint gradient treatment "
                 "for slanted sidewalls. "
                 "A straight sidewall angle is assumed when computing the gradient with respect "
                 "to shifting boundaries of the geometry. Therefore, as 'sidewall_angle' becomes "
                 "further from '0.0', the gradient error can be significant. "
                 "If high gradient accuracy is needed, please either reduce your 'sidewall_angle' "
-                "or wait until this feature is supported fully in a later version."
+                "or wait until this feature is supported fully in a later version.",
+                log_once=True,
             )
         return val
 
     @pd.validator("dilation", always=True)
     def no_dilation(cls, val):
         """Don't allow dilation."""
         if not np.isclose(val, 0.0):
@@ -309,14 +337,220 @@
         """Limit the maximum number of vertices."""
         if len(self.vertices_jax) > MAX_NUM_VERTICES:
             raise AdjointError(
                 f"For performance, a maximum of {MAX_NUM_VERTICES} are allowed in 'JaxPolySlab'. "
                 + WEB_ADJOINT_MESSAGE
             )
 
+    def _extrusion_length_to_offset_distance(self, extrusion: float) -> float:
+        """Convert extrusion length to offset distance."""
+        if jnp.isclose(self.sidewall_angle_jax, 0):
+            return 0.0
+        return -extrusion * self._tanq
+
+    @staticmethod
+    def _orient(vertices: jnp.ndarray) -> jnp.ndarray:
+        """Return a CCW-oriented polygon.
+
+        Parameters
+        ----------
+        vertices : np.ndarray
+            Shape (N, 2) defining the polygon vertices in the xy-plane.
+
+        Returns
+        -------
+        np.ndarray
+            Vertices of a CCW-oriented polygon.
+        """
+        return vertices if JaxPolySlab._area(vertices) > 0 else vertices[::-1, :]
+
+    @staticmethod
+    def _area(vertices: jnp.ndarray) -> float:
+        """Compute the signed polygon area (positive for CCW orientation).
+
+        Parameters
+        ----------
+        vertices : np.ndarray
+            Shape (N, 2) defining the polygon vertices in the xy-plane.
+
+        Returns
+        -------
+        float
+            Signed polygon area (positive for CCW orientation).
+        """
+        x = vertices[:, 0]
+        y = vertices[:, 1]
+        return jnp.dot(x, jnp.roll(y, -1)) - jnp.dot(y, jnp.roll(x, -1)) / 2
+
+    @staticmethod
+    def _shift_vertices(
+        vertices: jnp.ndarray, dist
+    ) -> Tuple[jnp.ndarray, jnp.ndarray, Tuple[jnp.ndarray, jnp.ndarray]]:
+        """Shifts the vertices of a polygon outward uniformly by distances
+        `dists`.
+
+        Parameters
+        ----------
+        jnp.ndarray
+            Shape (N, 2) defining the polygon vertices in the xy-plane.
+        dist : float
+            Distance to offset.
+
+        Returns
+        -------
+        Tuple[jnp.ndarray, jnp.narray, Tuple[jnp.ndarray, jnp.ndarray]]
+            New polygon vertices;
+            and the shift of vertices in direction parallel to the edges.
+            Shift along x and y direction.
+        """
+
+        if jnp.isclose(dist, 0):
+            return vertices, jnp.zeros(vertices.shape[0], dtype=float), None
+
+        def rot90(v):
+            return jnp.array([-v[1], v[0]])
+
+        def normalize(v):
+            return v / jnp.linalg.norm(v, axis=0)
+
+        vs = vertices.T
+        vs_next = jnp.roll(vs, axis=-1, shift=-1)
+        vs_previous = jnp.roll(vs, axis=-1, shift=+1)
+
+        asp = normalize(vs_next - vs)
+        asm = normalize(vs - vs_previous)
+
+        # the vertex shift is decomposed into parallel and perpendicular directions
+        perpendicular_shift = -dist
+        det = jnp.cross(asm, asp, axis=0)
+
+        tan_half_angle = jnp.where(
+            jnp.isclose(det, 0, rtol=_IS_CLOSE_RTOL),
+            0.0,
+            jnp.cross(asm, rot90(asm - asp), axis=0)
+            / (det + jnp.isclose(det, 0, rtol=_IS_CLOSE_RTOL)),
+        )
+        parallel_shift = dist * tan_half_angle
+
+        shift_total = perpendicular_shift * rot90(asm) + parallel_shift * asm
+
+        return jnp.swapaxes(vs + shift_total, -2, -1), parallel_shift, shift_total
+
+    @staticmethod
+    def _neighbor_vertices_crossing_detection(
+        vertices: jnp.ndarray, dist: float, ignore_at_dist: bool = True
+    ) -> float:
+        """Detect if neighboring vertices will cross after a dilation distance dist.
+
+        Parameters
+        ----------
+        vertices : jnp.ndarray
+            Shape (N, 2) defining the polygon vertices in the xy-plane.
+        dist : float
+            Distance to offset.
+        ignore_at_dist : bool, optional
+            whether to ignore the event right at ``dist`.
+
+        Returns
+        -------
+        float
+            the absolute value of the maximal allowed dilation
+            if there are any crossing, otherwise return ``None``.
+        """
+        # ignore the event that occurs right at the offset distance
+        if ignore_at_dist:
+            dist -= fp_eps * dist / jnp.abs(dist)
+
+        edge_length, edge_reduction = JaxPolySlab._edge_length_and_reduction_rate(vertices)
+        length_remaining = edge_length - edge_reduction * dist
+
+        mask = length_remaining < 0
+        if jnp.any(mask):
+            return jnp.min(jnp.abs(edge_length[mask] / edge_reduction[mask]))
+        return None
+
+    @staticmethod
+    def _edge_length_and_reduction_rate(vertices: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
+        """Edge length of reduction rate of each edge with unit offset length.
+
+        Parameters
+        ----------
+        vertices : jnp.ndarray
+            Shape (N, 2) defining the polygon vertices in the xy-plane.
+
+        Returns
+        -------
+        Tuple[jnp.ndarray, jnp.narray]
+            edge length, and reduction rate
+        """
+
+        # edge length
+        vs = vertices.T
+        vs_next = jnp.roll(vs, axis=-1, shift=-1)
+        edge_length = jnp.linalg.norm(vs_next - vs, axis=0)
+
+        # edge length remaining
+        parallel_shift = JaxPolySlab._shift_vertices(vertices, 1.0)[1]
+        parallel_shift_p = jnp.roll(parallel_shift, shift=-1)
+        edge_reduction = -(parallel_shift + parallel_shift_p)
+        return edge_length, edge_reduction
+
+    @staticmethod
+    def _remove_duplicate_vertices(vertices: jnp.ndarray) -> jnp.ndarray:
+        """Remove redundant/identical nearest neighbour vertices.
+
+        Parameters
+        ----------
+        vertices : jnp.ndarray
+            Shape (N, 2) defining the polygon vertices in the xy-plane.
+
+        Returns
+        -------
+        np.ndarray
+            Vertices of polygon.
+        """
+
+        vertices_f = jnp.roll(vertices, shift=-1, axis=0)
+        vertices_diff = jnp.linalg.norm(vertices - vertices_f, axis=1)
+        return vertices[~jnp.isclose(vertices_diff, 0, rtol=_IS_CLOSE_RTOL)]
+
+    @staticmethod
+    def _proper_vertices(vertices: ArrayFloat2D) -> jnp.ndarray:
+        """convert vertices to jnp.array format,
+        removing duplicate neighbouring vertices,
+        and oriented in CCW direction.
+
+        Returns
+        -------
+        ArrayLike[float, float]
+           The vertices of the polygon for internal use.
+        """
+
+        vertices_np = JaxPolySlab.vertices_to_array(vertices)
+        return JaxPolySlab._orient(JaxPolySlab._remove_duplicate_vertices(vertices_np))
+
+    @staticmethod
+    def vertices_to_array(vertices_tuple: ArrayFloat2D) -> jnp.ndarray:
+        """Converts a list of tuples (vertices) to a jax array."""
+        return jnp.asarray(vertices_tuple)
+
+    @cached_property
+    def reference_polygon(self) -> jnp.ndarray:
+        """The polygon at the reference plane.
+
+        Returns
+        -------
+        ArrayLike[float, float]
+            The vertices of the polygon at the reference plane.
+        """
+        vertices = JaxPolySlab._proper_vertices(self.vertices_jax)
+        if jnp.isclose(self.dilation, 0):
+            return vertices
+        raise NotImplementedError("JaxPolySlab does not support dilation!")
+
     def edge_contrib(
         self,
         vertex_grad: Coordinate2D,
         vertex_stat: Coordinate2D,
         is_next: bool,
         e_mult_xyz: Tuple[Dict[str, ScalarFieldDataArray]],
         d_mult_xyz: Tuple[Dict[str, ScalarFieldDataArray]],
@@ -355,15 +589,15 @@
             normal_vector *= -1
 
         def edge_position(s: np.array) -> np.array:
             """Parameterization of position along edge from s=0 (static) to s=1 (gradient)."""
             return (1 - s) * vertex_stat[:, None] + s * vertex_grad[:, None]
 
         def edge_basis(
-            xyz_components: Tuple[FieldData, FieldData, FieldData]
+            xyz_components: Tuple[FieldData, FieldData, FieldData],
         ) -> Tuple[FieldData, FieldData, FieldData]:
             """Puts a field component from the (x, y, z) basis to the (t, n, z) basis."""
             cmp_z, (cmp_x_edge, cmp_y_edge) = self.pop_axis(xyz_components, axis=self.axis)
 
             cmp_t = cmp_x_edge * tx + cmp_y_edge * ty
             cmp_n = cmp_x_edge * nx + cmp_y_edge * ny
 
@@ -536,35 +770,39 @@
         wvl_mat: float,
         eps_out: complex,
         eps_in: complex,
     ) -> tuple:
         """Generate arguments for ``vertex_vjp``."""
 
         num_verts = len(self.vertices)
-        args = [range(num_verts)]
 
-        # append all of the arguments that are the same for each call
-        constant_args = [e_mult_xyz, d_mult_xyz, sim_bounds, wvl_mat, eps_out, eps_in]
-        args += [[arg] * num_verts for arg in constant_args]
-        return args
+        arg_list = []
+
+        for i in range(num_verts):
+            args_i = [i] + [e_mult_xyz, d_mult_xyz, sim_bounds, wvl_mat, eps_out, eps_in]
+            arg_list.append(args_i)
+
+        return arg_list
 
     def store_vjp_sequential(
         self,
         e_mult_xyz: FieldData,
         d_mult_xyz: FieldData,
         sim_bounds: Bound,
         wvl_mat: float,
         eps_out: complex,
         eps_in: complex,
     ) -> JaxPolySlab:
         """Stores the gradient of the vertices given forward and adjoint field data."""
         # Construct arguments to pass to the parallel vertices_vjp computation
 
-        args = self._make_vertex_args(e_mult_xyz, d_mult_xyz, sim_bounds, wvl_mat, eps_out, eps_in)
-        vertices_vjp = tuple(map(self.vertex_vjp, *args))
+        arg_list = self._make_vertex_args(
+            e_mult_xyz, d_mult_xyz, sim_bounds, wvl_mat, eps_out, eps_in
+        )
+        vertices_vjp = tuple(self.vertex_vjp(*args) for args in arg_list)
         vertices_vjp = tuple(tuple(x) for x in vertices_vjp)
 
         return self.updated_copy(vertices_jax=vertices_vjp)
 
     def store_vjp_parallel(
         self,
         e_mult_xyz: FieldData,
@@ -574,20 +812,168 @@
         eps_out: complex,
         eps_in: complex,
         num_proc: int = 1,
     ) -> JaxPolySlab:
         """Stores the gradient of the vertices given forward and adjoint field data."""
 
         args = self._make_vertex_args(e_mult_xyz, d_mult_xyz, sim_bounds, wvl_mat, eps_out, eps_in)
-        with Pool(num_proc) as pool:
-            vertices_vjp = pool.starmap(self.vertex_vjp, zip(*args))
+        vertices_vjp = Parallel(n_jobs=num_proc)(delayed(self.vertex_vjp)(*arg) for arg in args)
         vertices_vjp = tuple(tuple(x) for x in vertices_vjp)
         return self.updated_copy(vertices_jax=vertices_vjp)
 
 
+@register_pytree_node_class
+class JaxComplexPolySlab(JaxPolySlab, ComplexPolySlab):
+    """A :class:`.ComplexPolySlab` registered with jax."""
+
+    _tidy3d_class = ComplexPolySlab
+
+    @pd.validator("vertices", always=True)
+    def no_self_intersecting_polygon_during_extrusion(cls, val, values):
+        """Turn off the validation for this class."""
+        return val
+
+    @property
+    def geometry_group(self) -> None:
+        """Divide a complex jax polyslab into a list of simple polyslabs, which
+        are assembled into a :class:`.JaxGeometryGroup`.
+
+        Returns
+        -------
+        :class:`.JaxGeometryGroup`
+            JaxGeometryGroup for a list of simple jax polyslabs divided from the complex
+            polyslab.
+        """
+        return JaxGeometryGroup(geometries=self.sub_polyslabs)
+
+    def _dilation_value_at_reference_to_coord(self, dilation: float) -> float:
+        """Compute the coordinate based on the dilation value to the reference plane."""
+
+        z_coord = -dilation / self._tanq + self.slab_bounds_jax[0]
+        if self.reference_plane == "middle":
+            return z_coord + self.finite_length_axis / 2
+        if self.reference_plane == "top":
+            return z_coord + self.finite_length_axis
+        # bottom case
+        return z_coord
+
+    @property
+    def sub_polyslabs(self) -> List[JaxPolySlab]:
+        """Divide a complex polyslab into a list of simple polyslabs.
+        Only neighboring vertex-vertex crossing events are treated in this
+        version.
+
+        Returns
+        -------
+        List[JaxPolySlab]
+            A list of simple jax polyslabs.
+        """
+        sub_polyslab_list = []
+        num_division_count = 0
+
+        # initialize sub-polyslab parameters
+
+        sub_polyslab_dict = self.dict(
+            exclude={  # all of these NEED to be overwritten, so best to exclude them
+                "type",
+                "vertices",
+                "vertices_jax",
+                "slab_bounds",
+                "slab_bounds_jax",
+                "sidewall_angle",
+                "sidewall_angle_jax",
+                "dilation",
+                "reference_plane",
+            }
+        )
+        if jnp.isclose(self.sidewall_angle_jax, 0):
+            return [
+                JaxPolySlab(
+                    vertices=tuple(map(tuple, self.vertices_jax)),
+                    slab_bounds=tuple(self.slab_bounds_jax),
+                    sidewall_angle=self.sidewall_angle_jax,
+                    dilation=self.dilation,
+                    reference_plane=self.reference_plane,
+                    **sub_polyslab_dict,
+                )
+            ]
+
+        # initialize offset distance
+        offset_distance = 0.0
+
+        for dist_val in self._dilation_length:
+            dist_now = 0.0
+            vertices_now = self.reference_polygon
+
+            # constructing sub-polyslabs until reaching the base/top
+            while not jnp.isclose(dist_now, dist_val):
+                # bounds for sub-polyslabs assuming no self-intersection
+                slab_bounds = [
+                    self._dilation_value_at_reference_to_coord(dist_now),
+                    self._dilation_value_at_reference_to_coord(dist_val),
+                ]
+                # 1) find out any vertices touching events between the current
+                # position to the base/top
+                max_dist = JaxPolySlab._neighbor_vertices_crossing_detection(
+                    vertices_now, dist_val - dist_now
+                )
+
+                # vertices touching events captured, update bounds for sub-polyslab
+                if max_dist is not None:
+                    # max_dist doesn't have sign, so construct signed offset distance
+                    offset_distance = max_dist * dist_val / jnp.abs(dist_val)
+                    slab_bounds = [
+                        self._dilation_value_at_reference_to_coord(dist_now),
+                        self._dilation_value_at_reference_to_coord(dist_now + offset_distance),
+                    ]
+
+                # 2) construct sub-polyslab
+                slab_bounds = jnp.sort(
+                    jnp.asarray(slab_bounds)
+                )  # for reference_plane=top/bottom, bounds need to be ordered
+                # direction of marching
+                reference_plane = "bottom" if dist_val / self._tanq < 0 else "top"
+
+                sub_polyslab_list.append(
+                    JaxPolySlab(
+                        vertices=tuple(map(tuple, vertices_now)),
+                        slab_bounds=tuple(slab_bounds),
+                        sidewall_angle=self.sidewall_angle_jax,
+                        dilation=0.0,  # dilation accounted for in setup
+                        reference_plane=reference_plane,
+                        **sub_polyslab_dict,
+                    )
+                )
+
+                # Now Step 3
+                if max_dist is None:
+                    break
+                dist_now += offset_distance
+                # new polygon vertices where collapsing vertices are removed but keep one
+                vertices_now = JaxPolySlab._shift_vertices(vertices_now, offset_distance)[0]
+                vertices_now = JaxPolySlab._remove_duplicate_vertices(vertices_now)
+                # all vertices collapse
+                if len(vertices_now) < 3:
+                    break
+                # polygon collapse into 1D
+                if shapely.Polygon(jax.lax.stop_gradient(vertices_now)).buffer(0).area < fp_eps:
+                    raise RuntimeError("Unhandled shapely transformation in JaxComplexPolySlab.")
+                vertices_now = JaxPolySlab._orient(vertices_now)
+                num_division_count += 1
+
+        if num_division_count > _COMPLEX_POLYSLAB_DIVISIONS_WARN:
+            log.warning(
+                f"Too many self-intersecting events: the polyslab has been divided into "
+                f"{num_division_count} polyslabs; more than {_COMPLEX_POLYSLAB_DIVISIONS_WARN} may "
+                f"slow down the simulation."
+            )
+
+        return sub_polyslab_list
+
+
 JaxSingleGeometryType = Union[JaxBox, JaxPolySlab]
 
 
 @register_pytree_node_class
 class JaxGeometryGroup(JaxGeometry, GeometryGroup, JaxObject):
     """A collection of Geometry objects that can be called as a single geometry object."""
 
@@ -634,35 +1020,42 @@
         wvl_mat: float,
         eps_out: complex,
         eps_in: complex,
         num_proc: int = 1,
     ) -> JaxGeometryGroup:
         """Returns a ``JaxGeometryGroup`` where the ``.geometries`` store the gradient info."""
 
-        map_args = (
-            self.geometries,
-            [grad_data_fwd] * len(self.geometries),
-            [grad_data_adj] * len(self.geometries),
-            [grad_data_eps] * len(self.geometries),
-            [sim_bounds] * len(self.geometries),
-            [wvl_mat] * len(self.geometries),
-            [eps_out] * len(self.geometries),
-            [eps_in] * len(self.geometries),
-        )
+        args_list = []
+        for geo in self.geometries:
+            args_i = [
+                geo,
+                grad_data_fwd,
+                grad_data_adj,
+                grad_data_eps,
+                sim_bounds,
+                wvl_mat,
+                eps_out,
+                eps_in,
+            ]
+            args_list.append(args_i)
 
         if num_proc == 1:
-            geometries_vjp = tuple(map(self._store_vjp_geometry, *map_args))
+            geometries_vjp = tuple(self._store_vjp_geometry(*args) for args in args_list)
         else:
-            with Pool(num_proc) as pool:
-                geometries_vjp = tuple(pool.starmap(self._store_vjp_geometry, zip(*map_args)))
+            geometries_vjp = tuple(
+                Parallel(n_jobs=num_proc)(
+                    delayed(self._store_vjp_geometry)(*args) for args in args_list
+                )
+            )
 
         return self.updated_copy(geometries=geometries_vjp)
 
 
 JaxGeometryType = Union[JaxSingleGeometryType, JaxGeometryGroup]
 
 
 JAX_GEOMETRY_MAP = {
     Box: JaxBox,
     PolySlab: JaxPolySlab,
+    ComplexPolySlab: JaxComplexPolySlab,
     GeometryGroup: JaxGeometryGroup,
 }
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Defines a jax-compatible simulation."""
+
 from __future__ import annotations
 
 from typing import Tuple, Union, List, Dict, Literal
-from multiprocessing import Pool
+from joblib import Parallel, delayed
+
 
 import pydantic.v1 as pd
 import numpy as np
 import xarray as xr
 
 from jax.tree_util import register_pytree_node_class
 
 from ....log import log
 from ....components.base import cached_property, Tidy3dBaseModel, skip_if_fields_missing
 from ....components.monitor import FieldMonitor, PermittivityMonitor
 from ....components.monitor import ModeMonitor, DiffractionMonitor, Monitor
 from ....components.simulation import Simulation
 from ....components.data.monitor_data import FieldData, PermittivityData
 from ....components.structure import Structure
+from ....components.medium import AbstractMedium
 from ....components.types import Ax, annotate_type
 from ....components.geometry.base import Box
 from ....constants import HERTZ, SECOND
 from ....exceptions import AdjointError
 
 from .base import JaxObject, WEB_ADJOINT_MESSAGE
 from .structure import (
@@ -51,14 +54,17 @@
 NL_WARNING = (
     "The 'adjoint' plugin does not currently support nonlinear materials. "
     "While the gradients might be calculated, they will be inaccurate and the "
     "error will increase as the strength of the nonlinearity is increased. "
     "We strongly recommend using linear simulations only with the adjoint plugin."
 )
 
+OutputMonitorTypes = (DiffractionMonitor, FieldMonitor, ModeMonitor)
+OutputMonitorType = Tuple[annotate_type(Union[OutputMonitorTypes]), ...]
+
 
 class JaxInfo(Tidy3dBaseModel):
     """Class to store information when converting between jax and tidy3d."""
 
     num_input_structures: pd.NonNegativeInt = pd.Field(
         ...,
         title="Number of Input Structures",
@@ -114,17 +120,15 @@
         (),
         title="Input Structures",
         description="Tuple of jax-compatible structures"
         " that may depend on differentiable parameters.",
         jax_field=True,
     )
 
-    output_monitors: Tuple[
-        annotate_type(Union[DiffractionMonitor, FieldMonitor, ModeMonitor]), ...
-    ] = pd.Field(
+    output_monitors: OutputMonitorType = pd.Field(
         (),
         title="Output Monitors",
         description="Tuple of monitors whose data the differentiable output depends on.",
     )
 
     grad_monitors: Tuple[FieldMonitor, ...] = pd.Field(
         (),
@@ -351,26 +355,26 @@
     @cached_property
     def _run_time_adjoint(self: float) -> float:
         """Return the run time of the adjoint simulation as a function of its fwidth."""
 
         if self.run_time_adjoint is not None:
             return self.run_time_adjoint
 
-        run_time_fwd = self.run_time
+        run_time_fwd = self._run_time
         run_time_adjoint = run_time_fwd + RUN_TIME_FACTOR / self._fwidth_adjoint
 
         if self._is_multi_freq:
             log.warning(
                 f"{len(self.freqs_adjoint)} unique frequencies detected in the output monitors "
                 f"with a minimum spacing of {self._min_delta_freq:.3e} (Hz). "
                 f"Setting the 'fwidth' of the adjoint sources to {FWIDTH_FACTOR_MULTIFREQ} times "
                 f"this value = {self._fwidth_adjoint:.3e} (Hz) to avoid spectral overlap. "
                 "To account for this, the corresponding 'run_time' in the adjoint simulation is "
                 f"will be set to {run_time_adjoint:3e} "
-                f"compared to {self.run_time:3e} in the forward simulation. "
+                f"compared to {self._run_time:3e} in the forward simulation. "
                 "If the adjoint 'run_time' is large due to small frequency spacing, "
                 "it could be better to instead run one simulation per frequency, "
                 "which can be done in parallel using 'tidy3d.plugins.adjoint.web.run_async'."
             )
 
         return run_time_adjoint
 
@@ -429,14 +433,126 @@
             fwidth_adjoint=self.fwidth_adjoint,
             run_time_adjoint=self.run_time_adjoint,
             input_structure_types=[s.type for s in self.input_structures],
         )
 
         return sim, jax_info
 
+    def to_gds(
+        self,
+        cell,
+        x: float = None,
+        y: float = None,
+        z: float = None,
+        permittivity_threshold: pd.NonNegativeFloat = 1,
+        frequency: pd.PositiveFloat = 0,
+        gds_layer_dtype_map: Dict[
+            AbstractMedium, Tuple[pd.NonNegativeInt, pd.NonNegativeInt]
+        ] = None,
+    ) -> None:
+        """Append the simulation structures to a .gds cell.
+        Parameters
+        ----------
+        cell : ``gdstk.Cell`` or ``gdspy.Cell``
+            Cell object to which the generated polygons are added.
+        x : float = None
+            Position of plane in x direction, only one of x,y,z can be specified to define plane.
+        y : float = None
+            Position of plane in y direction, only one of x,y,z can be specified to define plane.
+        z : float = None
+            Position of plane in z direction, only one of x,y,z can be specified to define plane.
+        permittivity_threshold : float = 1
+            Permittivity value used to define the shape boundaries for structures with custom
+            medim
+        frequency : float = 0
+            Frequency for permittivity evaluation in case of custom medium (Hz).
+        gds_layer_dtype_map : Dict
+            Dictionary mapping mediums to GDSII layer and data type tuples.
+        """
+        sim, _ = self.to_simulation()
+        return sim.to_gds(
+            cell=cell,
+            x=x,
+            y=y,
+            z=z,
+            permittivity_threshold=permittivity_threshold,
+            frequency=frequency,
+            gds_layer_dtype_map=gds_layer_dtype_map,
+        )
+
+    def to_gdstk(
+        self,
+        x: float = None,
+        y: float = None,
+        z: float = None,
+        permittivity_threshold: pd.NonNegativeFloat = 1,
+        frequency: pd.PositiveFloat = 0,
+        gds_layer_dtype_map: Dict[
+            AbstractMedium, Tuple[pd.NonNegativeInt, pd.NonNegativeInt]
+        ] = None,
+    ) -> List:
+        """Convert a simulation's planar slice to a .gds type polygon list.
+        Parameters
+        ----------
+        x : float = None
+            Position of plane in x direction, only one of x,y,z can be specified to define plane.
+        y : float = None
+            Position of plane in y direction, only one of x,y,z can be specified to define plane.
+        z : float = None
+            Position of plane in z direction, only one of x,y,z can be specified to define plane.
+        permittivity_threshold : float = 1
+            Permittivity value used to define the shape boundaries for structures with custom
+            medim
+        frequency : float = 0
+            Frequency for permittivity evaluation in case of custom medium (Hz).
+        gds_layer_dtype_map : Dict
+            Dictionary mapping mediums to GDSII layer and data type tuples.
+        Return
+        ------
+        List
+            List of `gdstk.Polygon`.
+        """
+        sim, _ = self.to_simulation()
+        return sim.to_gdstk(
+            x=x,
+            y=y,
+            z=z,
+            permittivity_threshold=permittivity_threshold,
+            frequency=frequency,
+            gds_layer_dtype_map=gds_layer_dtype_map,
+        )
+
+    def to_gdspy(
+        self,
+        x: float = None,
+        y: float = None,
+        z: float = None,
+        gds_layer_dtype_map: Dict[
+            AbstractMedium, Tuple[pd.NonNegativeInt, pd.NonNegativeInt]
+        ] = None,
+    ) -> List:
+        """Convert a simulation's planar slice to a .gds type polygon list.
+        Parameters
+        ----------
+        x : float = None
+            Position of plane in x direction, only one of x,y,z can be specified to define plane.
+        y : float = None
+            Position of plane in y direction, only one of x,y,z can be specified to define plane.
+        z : float = None
+            Position of plane in z direction, only one of x,y,z can be specified to define plane.
+        gds_layer_dtype_map : Dict
+            Dictionary mapping mediums to GDSII layer and data type tuples.
+        Return
+        ------
+        List
+            List of `gdspy.Polygon` and `gdspy.PolygonSet`.
+        """
+        sim, _ = self.to_simulation()
+        return sim.to_gdspy(x=x, y=y, z=z, gds_layer_dtype_map=gds_layer_dtype_map)
+
     def plot(
         self,
         x: float = None,
         y: float = None,
         z: float = None,
         ax: Ax = None,
         source_alpha: float = None,
@@ -854,34 +970,41 @@
         inds_par_internal, inds_par_external = [], []
         for index, structure in enumerate(self.input_structures):
             if isinstance(structure.geometry, tuple(internal_par_structs)):
                 inds_par_internal.append(index)
             else:
                 inds_par_external.append(index)
 
-        def make_args(indexes, num_proc_internal):
+        def make_args(indexes, num_proc_internal) -> list:
             """Make the arguments to map over selecting over a set of structure ``indexes``."""
-            structures = [self.input_structures[index] for index in indexes]
-            data_fwd = [grad_data_fwd[index] for index in indexes]
-            data_bwd = [grad_data_adj[index] for index in indexes]
-            eps_data = [grad_eps_data[index] for index in indexes]
-            num_proc = [num_proc_internal] * len(indexes)
+            args_list = []
+            for index in indexes:
+                args_i = [
+                    self.input_structures[index],
+                    grad_data_fwd[index],
+                    grad_data_adj[index],
+                    grad_eps_data[index],
+                    num_proc_internal,
+                ]
+                args_list.append(args_i)
 
-            return (structures, data_fwd, data_bwd, eps_data, num_proc)
+            return args_list
 
         # Get vjps for structures that parallelize internally using simple map
-        args_par_internal = make_args(inds_par_internal, num_proc_internal=num_proc)
-        vjps_par_internal = list(map(self._store_vjp_structure, *args_par_internal))
+        args_list_internal = make_args(inds_par_internal, num_proc_internal=num_proc)
+        vjps_par_internal = [self._store_vjp_structure(*args) for args in args_list_internal]
 
         # Get vjps for structures where we parallelize directly here
-        args_par_external = make_args(inds_par_external, num_proc_internal=NUM_PROC_LOCAL)
-        with Pool(num_proc) as pool:
-            vjps_par_external = list(
-                pool.starmap(self._store_vjp_structure, zip(*args_par_external))
+        args_list_external = make_args(inds_par_external, num_proc_internal=NUM_PROC_LOCAL)
+
+        vjps_par_external = list(
+            Parallel(n_jobs=num_proc)(
+                delayed(self._store_vjp_structure)(*args) for args in args_list_external
             )
+        )
 
         # Reshuffle the two lists back in the correct order
         vjps_all = list(vjps_par_internal) + list(vjps_par_external)
         input_structures_vjp = [None] * len(self.input_structures)
         for index, vjp in zip(inds_par_internal + inds_par_external, vjps_all):
             input_structures_vjp[index] = vjp
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/utils/filter.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/utils/filter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/utils/penalty.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/utils/penalty.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,18 @@
     The amount of change under dilation and erosion is minimized if the structure has large feature
     sizes and large radius of curvature relative to the length scale.
 
     Note
     ----
     For more details, refer to chapter 4 of Hammond, A., "High-Efficiency Topology Optimization
     for Very Large-Scale Integrated-Photonics Inverse Design" (2022).
+
+
+    .. image:: ../../_static/img/erosion_dilation.png
+
     """
 
     length_scale: pd.NonNegativeFloat = pd.Field(
         ...,
         title="Length Scale",
         description="Length scale of erosion and dilation. "
         "Corresponds to ``radius`` in the :class:`ConicFilter` used for filtering. "
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/adjoint/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from tidy3d.web.api.webapi import wait_for_connection
 from tidy3d.web.core.s3utils import download_file, upload_file
 from tidy3d.web.api.asynchronous import run_async as web_run_async
 from ...web.api.container import BatchData, DEFAULT_DATA_DIR, Job, Batch
 from ...components.types import Literal
 
 from .components.base import JaxObject
-from .components.simulation import JaxSimulation, JaxInfo
+from .components.simulation import JaxSimulation, JaxInfo, NUM_PROC_LOCAL
 from .components.data.sim_data import JaxSimulationData
 
 
 # file names and paths for server side adjoint
 SIM_VJP_FILE = "output/jax_sim_vjp.hdf5"
 JAX_INFO_FILE = "jax_info.json"
 
@@ -72,14 +72,39 @@
     """Run a set of regular :class:`.Simulation` objects after conversion from jax type."""
     return web_run_async(simulations=simulations, **kwargs)
 
 
 """ Running a single simulation using web.run. """
 
 
+def _run(
+    simulation: JaxSimulation,
+    task_name: str,
+    folder_name: str = "default",
+    path: str = "simulation_data.hdf5",
+    callback_url: str = None,
+    verbose: bool = True,
+) -> JaxSimulationData:
+    """Split the provided ``JaxSimulation`` into a regular ``Simulation`` and a ``JaxInfo`` part,
+    run using ``tidy3d_run_fn``, which runs on the server by default but can be monkeypatched,
+    and recombine into a ``JaxSimulationData``.
+    """
+    sim, jax_info = simulation.to_simulation()
+
+    sim_data = tidy3d_run_fn(
+        simulation=sim,
+        task_name=str(task_name),
+        folder_name=folder_name,
+        path=path,
+        callback_url=callback_url,
+        verbose=verbose,
+    )
+    return JaxSimulationData.from_sim_data(sim_data, jax_info)
+
+
 @partial(custom_vjp, nondiff_argnums=tuple(range(1, 6)))
 def run(
     simulation: JaxSimulation,
     task_name: str,
     folder_name: str = "default",
     path: str = "simulation_data.hdf5",
     callback_url: str = None,
@@ -109,25 +134,23 @@
     -------
     :class:`.JaxSimulationData`
         Object containing solver results for the supplied :class:`.JaxSimulation`.
     """
 
     simulation._validate_web_adjoint()
 
-    sim, jax_info = simulation.to_simulation()
-
-    sim_data = tidy3d_run_fn(
-        simulation=sim,
-        task_name=str(task_name),
+    # TODO: add task_id
+    return _run(
+        simulation=simulation,
+        task_name=task_name,
         folder_name=folder_name,
         path=path,
         callback_url=callback_url,
         verbose=verbose,
     )
-    return JaxSimulationData.from_sim_data(sim_data, jax_info)
 
 
 def run_fwd(
     simulation: JaxSimulation,
     task_name: str,
     folder_name: str,
     path: str,
@@ -147,15 +170,17 @@
         folder_name=folder_name,
         path=path,
         callback_url=callback_url,
         verbose=verbose,
     )
 
     res = RunResidual(fwd_task_id=task_id)
-    jax_sim_data_orig = JaxSimulationData.from_sim_data(sim_data_orig, jax_info_orig)
+    jax_sim_data_orig = JaxSimulationData.from_sim_data(
+        sim_data_orig, jax_info_orig, task_id=task_id
+    )
 
     return jax_sim_data_orig, (res,)
 
 
 def run_bwd(
     task_name: str,
     folder_name: str,
@@ -237,65 +262,47 @@
     def start(self) -> None:
         """Start running a :class:`AdjointJob`. after uploading jax info.
 
         Note
         ----
         To monitor progress of the :class:`Job`, call :meth:`Job.monitor` after started.
         """
-        upload_jax_info(task_id=self.task_id, jax_info=self.jax_info, verbose=self.verbose)
+        if self.jax_info is not None:
+            upload_jax_info(task_id=self.task_id, jax_info=self.jax_info, verbose=self.verbose)
         super().start()
 
 
 class AdjointBatch(Batch):
     """Batch that uploads a jax_info object and also includes new fields for adjoint tasks."""
 
     simulation_type: AdjointSimulationType = pd.Field(
         "tidy3d",
         title="Simulation Type",
         description="Type of simulation, used internally only.",
     )
 
-    jobs: Dict[str, AdjointJob] = pd.Field(
-        None,
-        title="Simulations",
-        description="Mapping of task names to individual AdjointJob object for each task "
-        "in the batch. Set by ``AdjointBatch.upload``, leave as None.",
-    )
-
     jax_infos: Dict[str, JaxInfo] = pd.Field(
         ...,
         title="Jax Info Dict",
         description="Containers of information needed to reconstruct JaxSimulation for each item.",
     )
 
-    @pd.root_validator()
-    def _add_jax_infos(cls, values) -> None:
-        """Add jax_info fields to the uploaded jobs."""
-        jax_infos = values.get("jax_infos")
-        jobs = values.get("jobs")
-
-        if jobs is None:
-            return values
-
-        for task_name, job in jobs.items():
-            jax_info = jax_infos[task_name]
-            values["jobs"][task_name] = job.updated_copy(jax_info=jax_info)
-
-        return values
+    _job_type = AdjointJob
 
     def start(self) -> None:
-        """Start running all tasks in the :class:`Batch`.
+        """Start running a :class:`AdjointBatch`. after uploading jax info for each job.
 
         Note
         ----
-        To monitor the running simulations, can call :meth:`Batch.monitor`.
+        To monitor progress of the :class:`Batch`, call :meth:`Batch.monitor` after started.
         """
-        for _, job in self.jobs.items():
-            upload_jax_info(task_id=job.task_id, jax_info=job.jax_info, verbose=self.verbose)
-            job.start()
+        for task_name, job in self.jobs.items():
+            jax_info = self.jax_infos.get(task_name)
+            upload_jax_info(task_id=job.task_id, jax_info=jax_info, verbose=job.verbose)
+        super().start()
 
 
 def webapi_run_adjoint_fwd(
     simulation: Simulation,
     jax_info: JaxInfo,
     task_name: str,
     folder_name: str,
@@ -424,14 +431,15 @@
 
     # convert back to jax type and return
     jax_batch_data = []
     for i in range(len(simulations)):
         task_name = str(_task_name_orig(i))
         sim_data_tidy3d = batch_data_tidy3d[task_name]
         jax_info = jax_infos[str(task_name)]
+        # TODO: add task_id
         jax_sim_data = JaxSimulationData.from_sim_data(sim_data_tidy3d, jax_info=jax_info)
         jax_batch_data.append(jax_sim_data)
 
     return jax_batch_data
 
 
 def run_async_fwd(
@@ -464,16 +472,18 @@
         callback_url=callback_url,
         verbose=verbose,
     )
 
     batch_data_orig = [sim_data for _, sim_data in batch_data_orig.items()]
 
     jax_batch_data_orig = []
-    for sim_data_orig, jax_info_orig in zip(batch_data_orig, jax_infos_orig):
-        jax_sim_data = JaxSimulationData.from_sim_data(sim_data_orig, jax_info_orig)
+    for sim_data_orig, jax_info_orig, task_id in zip(batch_data_orig, jax_infos_orig, fwd_task_ids):
+        jax_sim_data = JaxSimulationData.from_sim_data(
+            sim_data_orig, jax_info_orig, task_id=task_id
+        )
         jax_batch_data_orig.append(jax_sim_data)
 
     residual = RunResidualBatch(fwd_task_ids=fwd_task_ids)
     return jax_batch_data_orig, (residual,)
 
 
 def run_async_bwd(
@@ -591,22 +601,23 @@
 # register the custom forward and backward functions
 run_async.defvjp(run_async_fwd, run_async_bwd)
 
 
 """ Options to do the previous but all client side (mainly for testing / debugging)."""
 
 
-@partial(custom_vjp, nondiff_argnums=tuple(range(1, 6)))
+@partial(custom_vjp, nondiff_argnums=tuple(range(1, 7)))
 def run_local(
     simulation: JaxSimulation,
     task_name: str,
     folder_name: str = "default",
     path: str = "simulation_data.hdf5",
     callback_url: str = None,
     verbose: bool = True,
+    num_proc: int = NUM_PROC_LOCAL,
 ) -> JaxSimulationData:
     """Submits a :class:`.JaxSimulation` to server, starts running, monitors progress, downloads,
     and loads results as a :class:`.JaxSimulationData` object.
     Can be included within a function that will have ``jax.grad`` applied.
 
     Parameters
     ----------
@@ -619,14 +630,16 @@
     folder_name : str = "default"
         Name of folder to store task on web UI.
     callback_url : str = None
         Http PUT url to receive simulation finish event. The body content is a json file with
         fields ``{'id', 'status', 'name', 'workUnit', 'solverVersion'}``.
     verbose : bool = True
         If `True`, will print progressbars and status, otherwise, will run silently.
+    num_proc: int = 1
+        Number of processes to use for the gradient computations.
 
     Returns
     -------
     :class:`.JaxSimulationData`
         Object containing solver results for the supplied :class:`.JaxSimulation`.
     """
 
@@ -640,33 +653,35 @@
         folder_name=folder_name,
         path=path,
         callback_url=callback_url,
         verbose=verbose,
     )
 
     # convert back to jax type and return
+    # TODO: add task_id
     return JaxSimulationData.from_sim_data(sim_data_tidy3d, jax_info=jax_info)
 
 
 def run_local_fwd(
     simulation: JaxSimulation,
     task_name: str,
     folder_name: str,
     path: str,
     callback_url: str,
     verbose: bool,
+    num_proc: int,
 ) -> Tuple[JaxSimulationData, tuple]:
     """Run forward pass and stash extra objects for the backwards pass."""
 
     # add the gradient monitors and run the forward simulation
     grad_mnts = simulation.get_grad_monitors(
         input_structures=simulation.input_structures, freqs_adjoint=simulation.freqs_adjoint
     )
     sim_fwd = simulation.updated_copy(**grad_mnts)
-    sim_data_fwd = run(
+    sim_data_fwd = _run(
         simulation=sim_fwd,
         task_name=_task_name_fwd(task_name),
         folder_name=folder_name,
         path=path,
         callback_url=callback_url,
         verbose=verbose,
     )
@@ -678,43 +693,49 @@
 
 def run_local_bwd(
     task_name: str,
     folder_name: str,
     path: str,
     callback_url: str,
     verbose: bool,
+    num_proc: int,
     res: tuple,
     sim_data_vjp: JaxSimulationData,
 ) -> Tuple[JaxSimulation]:
     """Run backward pass and return simulation storing vjp of the objective w.r.t. the sim."""
 
     # grab the forward simulation and its gradient monitor data
     (sim_data_fwd,) = res
     grad_data_fwd = sim_data_fwd.grad_data_symmetry
     grad_eps_data_fwd = sim_data_fwd.grad_eps_data_symmetry
 
     # make and run adjoint simulation
     fwidth_adj = sim_data_fwd.simulation._fwidth_adjoint
     run_time_adj = sim_data_fwd.simulation._run_time_adjoint
     sim_adj = sim_data_vjp.make_adjoint_simulation(fwidth=fwidth_adj, run_time=run_time_adj)
-    sim_data_adj = run(
+    sim_data_adj = _run(
         simulation=sim_adj,
         task_name=_task_name_adj(task_name),
         folder_name=folder_name,
         path=path,
         callback_url=callback_url,
         verbose=verbose,
     )
 
     sim_data_adj = sim_data_adj.normalize_adjoint_fields()
 
     grad_data_adj = sim_data_adj.grad_data_symmetry
 
     # get gradient and insert into the resulting simulation structure medium
-    sim_vjp = sim_data_vjp.simulation.store_vjp(grad_data_fwd, grad_data_adj, grad_eps_data_fwd)
+    sim_vjp = sim_data_vjp.simulation.store_vjp(
+        grad_data_fwd=grad_data_fwd,
+        grad_data_adj=grad_data_adj,
+        grad_eps_data=grad_eps_data_fwd,
+        num_proc=num_proc,
+    )
 
     return (sim_vjp,)
 
 
 # register the custom forward and backward functions
 run_local.defvjp(run_local_fwd, run_local_bwd)
 
@@ -793,14 +814,15 @@
     # convert back to jax type and return
     task_name_suffix = "" if task_name_suffix is None else task_name_suffix
     jax_batch_data = []
     for i in range(len(simulations)):
         task_name = _task_name_orig_local(i, task_name_suffix)
         sim_data_tidy3d = batch_data_tidy3d[task_name]
         jax_info = jax_infos[str(task_name)]
+        # TODO: add task_id
         jax_sim_data = JaxSimulationData.from_sim_data(sim_data_tidy3d, jax_info=jax_info)
         jax_batch_data.append(jax_sim_data)
 
     return jax_batch_data
 
 
 def run_async_local_fwd(
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/design/README.md` & `tidy3d-2.7.0rc2/tidy3d/plugins/design/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/design/design.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/design/design.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/design/method.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/design/method.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/design/parameter.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/design/parameter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/design/result.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/design/result.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/dispersion/fit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Fit PoleResidue Dispersion models to optical NK data
 """
+from __future__ import annotations
 
 from typing import Tuple, List, Optional
 import csv
 import codecs
 import requests
 
 import scipy.optimize as opt
@@ -560,15 +561,17 @@
                 except Exception as e:
                     raise ValidationError("Invalid URL. Float data cannot be recognized.") from e
 
         if has_k > 1:
             raise ValidationError("Invalid URL. Too many k labels.")
 
     @classmethod
-    def from_url(cls, url_file: str, delimiter: str = ",", ignore_k: bool = False, **kwargs):
+    def from_url(
+        cls, url_file: str, delimiter: str = ",", ignore_k: bool = False, **kwargs
+    ) -> DispersionFitter:
         """loads :class:`DispersionFitter` from url linked to a csv/txt file that
         contains wavelength (micron), n, and optionally k data. Preferred from
         refractiveindex.info.
 
         Hint
         ----
         The data file from url should be in this format (delimiter not displayed
@@ -648,15 +651,15 @@
             raise ValidationError(
                 "Invalid URL. Both n and k should be provided at each wavelength."
             )
 
         return cls(wvl_um=n_lam[:, 0], n_data=n_lam[:, 1], **kwargs)
 
     @classmethod
-    def from_file(cls, fname: str, **loadtxt_kwargs):
+    def from_file(cls, fname: str, **loadtxt_kwargs) -> DispersionFitter:
         """Loads :class:`DispersionFitter` from file containing wavelength, n, k data.
 
         Parameters
         ----------
         fname : str
             Path to file containing wavelength (um), n, k (optional) data in columns.
         **loadtxt_kwargs
@@ -693,7 +696,69 @@
         assert data.shape[-1] in (2, 3), "data must have either 2 or 3 rows (if k data)"
         if data.shape[-1] == 2:
             wvl_um, n_data = data.T
             k_data = None
         else:
             wvl_um, n_data, k_data = data.T
         return cls(wvl_um=wvl_um, n_data=n_data, k_data=k_data)
+
+    @classmethod
+    def from_complex_permittivity(
+        cls,
+        wvl_um: ArrayFloat1D,
+        eps_real: ArrayFloat1D,
+        eps_imag: ArrayFloat1D = None,
+        wvl_range: Tuple[Optional[float], Optional[float]] = (None, None),
+    ) -> DispersionFitter:
+        """Loads :class:`DispersionFitter` from wavelength and complex relative permittivity data
+
+        Parameters
+        ----------
+        wvl_um : ArrayFloat1D
+            Wavelength data in micrometers.
+        eps_real : ArrayFloat1D
+            Real parts of relative permittivity data
+        eps_imag : Optional[ArrayFloat1D]
+            Imaginary parts of relative permittivity data; `None` for lossless medium.
+        wvg_range : Tuple[Optional[float], Optional[float]]
+            Wavelength range [wvl_min,wvl_max] for fitting.
+
+        Returns
+        -------
+        :class:`DispersionFitter`
+            A :class:`DispersionFitter` instance.
+        """
+        if eps_imag is None:
+            n, _ = AbstractMedium.eps_complex_to_nk(eps_real + 0j)
+            return cls(wvl_um=wvl_um, n_data=n, wvl_range=wvl_range)
+        n, k = AbstractMedium.eps_complex_to_nk(eps_real + eps_imag * 1j)
+        return cls(wvl_um=wvl_um, n_data=n, k_data=k, wvl_range=wvl_range)
+
+    @classmethod
+    def from_loss_tangent(
+        cls,
+        wvl_um: ArrayFloat1D,
+        eps_real: ArrayFloat1D,
+        loss_tangent: ArrayFloat1D,
+        wvl_range: Tuple[Optional[float], Optional[float]] = (None, None),
+    ) -> DispersionFitter:
+        """Loads :class:`DispersionFitter` from wavelength and loss tangent data.
+
+        Parameters
+        ----------
+        wvl_um : ArrayFloat1D
+            Wavelength data in micrometers.
+        eps_real : ArrayFloat1D
+            Real parts of relative permittivity data
+        loss_tangent : Optional[ArrayFloat1D]
+            Loss tangent data, defined as the ratio of imaginary and real parts of permittivity.
+        wvl_range : Tuple[Optional[float], Optional[float]]
+            Wavelength range [wvl_min,wvl_max] for fitting.
+
+        Returns
+        -------
+        :class:`DispersionFitter`
+            A :class:`DispersionFitter` instance.
+        """
+        eps_complex = AbstractMedium.eps_loss_tangent_to_eps_complex(eps_real, loss_tangent)
+        n, k = AbstractMedium.eps_complex_to_nk(eps_complex)
+        return cls(wvl_um=wvl_um, n_data=n, k_data=k, wvl_range=wvl_range)
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/dispersion/fit_fast.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/dispersion/fit_fast.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from .fit import DispersionFitter
 from ...log import log, get_logging_console
 from ...components.base import Tidy3dBaseModel, cached_property, skip_if_fields_missing
 from ...components.medium import PoleResidue, LOSS_CHECK_MIN, LOSS_CHECK_MAX, LOSS_CHECK_NUM
 from ...components.types import ArrayFloat1D, ArrayComplex1D, ArrayFloat2D, ArrayComplex2D
 from ...exceptions import ValidationError
+from ...constants import C_0
 
 # numerical tolerance for pole relocation for fast fitter
 TOL = 1e-8
 # numerical cutoff for passivity testing
 CUTOFF = np.finfo(np.float32).eps
 # parameters for passivity optimization
 PASSIVITY_NUM_ITERS_DEFAULT = 50
@@ -28,14 +29,17 @@
 DEFAULT_MAX_POLES = 5
 DEFAULT_NUM_ITERS = 20
 DEFAULT_TOLERANCE_RMS = 1e-5
 
 # this avoids divide by zero errors with lossless poles
 SCALE_FACTOR = 1.01
 
+# when poles are close to omega, can cause invalid response function, and we reject model
+OMEGA_POLE_CLOSE_ATOL = 1e-10
+
 
 class AdvancedFastFitterParam(Tidy3dBaseModel):
     """Advanced fast fitter parameters."""
 
     loss_bounds: Tuple[float, float] = Field(
         (0, np.inf),
         title="Loss bounds",
@@ -515,14 +519,24 @@
         Returns
         -------
         :class:`.FastFitterData`
             Result of single fit.
         """
 
         model = self.iterate_poles()
+
+        # if any of the poles align with the test frequencies exactly, we reject the new model
+        if any(
+            np.isclose(omega, 1j * pole, rtol=0, atol=OMEGA_POLE_CLOSE_ATOL)
+            or np.isclose(omega, -1j * pole, rtol=0, atol=OMEGA_POLE_CLOSE_ATOL)
+            for omega in self.omega
+            for pole in self.complex_poles
+        ):
+            return self
+
         model = model.fit_residues()
 
         return model
 
     def iterate_passivity(self, passivity_omega: ArrayFloat1D) -> Tuple[FastFitterData, int]:
         """Iterate passivity enforcement algorithm."""
 
@@ -812,7 +826,52 @@
         if best_model.show_unweighted_rms:
             log.info(
                 "Unweighted RMS error %.3g",
                 best_model.unweighted_rms_error,
             )
 
         return best_model.pole_residue, best_model.rms_error
+
+    @classmethod
+    def constant_loss_tangent_model(
+        cls,
+        eps_real: float,
+        loss_tangent: float,
+        frequency_range: Tuple[float, float],
+        max_num_poles: PositiveInt = DEFAULT_MAX_POLES,
+        number_sampling_frequency: PositiveInt = 10,
+        tolerance_rms: NonNegativeFloat = DEFAULT_TOLERANCE_RMS,
+    ) -> PoleResidue:
+        """Fit a constant loss tangent material model.
+
+        Parameters
+        ----------
+        eps_real : float
+            Real part of permittivity
+        loss_tangent : float
+            Loss tangent.
+        frequency_range : Tuple[float, float]
+            Freqquency range for the material to exhibit constant loss tangent response.
+        max_num_poles : PositiveInt, optional
+            Maximum number of poles in the model.
+        number_sampling_frequency : PositiveInt, optional
+            Number of sampling frequencies to compute RMS error for fitting.
+        tolerance_rms : float, optional
+            Weighted RMS error below which the fit is successful and the result is returned.
+
+        Returns
+        -------
+        :class:`.PoleResidue
+            Best results of multiple fits.
+        """
+        if number_sampling_frequency < 2:
+            frequencies = np.array([np.mean(frequency_range)])
+        else:
+            frequencies = np.linspace(
+                frequency_range[0], frequency_range[1], number_sampling_frequency
+            )
+        wvl_um = C_0 / frequencies
+        eps_real_array = np.ones_like(frequencies) * eps_real
+        loss_tangent_array = np.ones_like(frequencies) * loss_tangent
+        fitter = cls.from_loss_tangent(wvl_um, eps_real_array, loss_tangent_array)
+        material, _ = fitter.fit(max_num_poles=max_num_poles, tolerance_rms=tolerance_rms)
+        return material
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/dispersion/web.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/dispersion/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/microwave/impedance_calculator.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/microwave/impedance_calculator.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/microwave/models/coupled_microstrip.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/microwave/models/coupled_microstrip.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/microwave/models/microstrip.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/microwave/models/microstrip.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/microwave/path_integrals.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/microwave/path_integrals.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/mode/LICENSE` & `tidy3d-2.7.0rc2/tidy3d/plugins/mode/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/mode/mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/mode/solver.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/mode/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,16 @@
         eps_formated = cls.format_medium_data(eps_cross)
         eps_xx, eps_xy, eps_xz, eps_yx, eps_yy, eps_yz, eps_zx, eps_zy, eps_zz = eps_formated
 
         mu_formated = None
         if mu_cross is not None:
             mu_formated = cls.format_medium_data(mu_cross)
 
-        Nx, Ny = eps_xx.shape
+        Nxy = eps_xx.shape
+        Nx, Ny = Nxy
         N = eps_xx.size
 
         if len(coords[0]) != Nx + 1 or len(coords[1]) != Ny + 1:
             raise ValueError("Mismatch between 'coords' and 'esp_cross' shapes.")
         new_coords = [np.copy(c) for c in coords]
 
         """We work with full tensorial epsilon in mu to handle the most general cases that can
@@ -162,32 +163,39 @@
         eps_tensor = np.einsum("ij...,jp...->ip...", jac_e, eps_tensor)  # J.dot(eps)
         eps_tensor = np.einsum("ij...,pj...->ip...", eps_tensor, jac_e)  # (J.dot(eps)).dot(J.T)
         eps_tensor /= jac_e_det
         mu_tensor = np.einsum("ij...,jp...->ip...", jac_h, mu_tensor)
         mu_tensor = np.einsum("ij...,pj...->ip...", mu_tensor, jac_h)
         mu_tensor /= jac_h_det
 
+        # # Uncomment block to force eps and mu to be translationally invariant into the PML.
+        # # This may be important for bends as the jacobian transformation breaks the invariance, but
+        # # tests reveal that it has little effect.
+        # eps_tensor = cls.make_pml_invariant(Nxy, eps_tensor, mode_spec.num_pml)
+        # mu_tensor = cls.make_pml_invariant(Nxy, mu_tensor, mode_spec.num_pml)
+
         """ Boundaries are imposed through the derivative matrices. The forward derivative matrices
         always impose PEC boundary at the xmax and ymax interfaces, and on the xmin and ymin
         interfaces unless PMC symmetry is present. If so, the PMC boundary is imposed through the
         backward derivative matrices."""
         dmin_pmc = [sym == 1 for sym in symmetry]
 
         # Primal grid steps for E-field derivatives
         dl_f = [new_cs[1:] - new_cs[:-1] for new_cs in new_coords]
         # Dual grid steps for H-field derivatives
         dl_tmp = [(dl[:-1] + dl[1:]) / 2 for dl in dl_f]
         dl_b = [np.hstack((d1[0], d2)) for d1, d2 in zip(dl_f, dl_tmp)]
+        dls = (dl_f, dl_b)
 
         # Derivative matrices with PEC boundaries by default and optional PMC at the near end
-        der_mats_tmp = d_mats((Nx, Ny), dl_f, dl_b, dmin_pmc)
+        der_mats_tmp = d_mats(Nxy, dls, dmin_pmc)
 
         # PML matrices; do not impose PML on the bottom when symmetry present
         dmin_pml = np.array(symmetry) == 0
-        pml_mats = s_mats(omega, (Nx, Ny), mode_spec.num_pml, dl_f, dl_b, dmin_pml)
+        pml_mats = s_mats(omega, Nxy, mode_spec.num_pml, dls, eps_tensor, mu_tensor, dmin_pml)
 
         # Add the PML on top of the derivatives; normalize by k0 to match the EM-possible notation
         der_mats = [Smat.dot(Dmat) / k0 for Smat, Dmat in zip(pml_mats, der_mats_tmp)]
 
         # Determine initial guess value for the solver in transformed coordinates
         if mode_spec.target_neff is None:
             eps_physical = np.array(eps_cross)
@@ -810,11 +818,25 @@
 
         E = E.reshape(3, Nx, Ny, field_shape[-1])
         E /= split_curl_scaling[:, :, :, np.newaxis]
         E *= outside_pec[:, :, :, np.newaxis]
         E = E.reshape(field_shape)
         return E
 
+    @staticmethod
+    def make_pml_invariant(Nxy, tensor, num_pml):
+        """For a given epsilon or mu tensor of shape ``(3, 3, Nx, Ny)``, and ``num_pml`` pml layers
+        along ``x`` and ``y``, make all the tensor values in the PML equal by replicating the first
+        pixel into the PML."""
+
+        Nx, Ny = Nxy
+        new_ten = tensor.reshape((3, 3, Nx, Ny))
+        new_ten[:, :, : num_pml[0], :] = new_ten[:, :, num_pml[0], :][:, :, None, :]
+        new_ten[:, :, Nx - num_pml[0] + 1 :, :] = new_ten[:, :, Nx - num_pml[0], :][:, :, None, :]
+        new_ten[:, :, :, : num_pml[1]] = new_ten[:, :, :, num_pml[1]][:, :, :, None]
+        new_ten[:, :, :, Ny - num_pml[1] + 1 :] = new_ten[:, :, :, Ny - num_pml[1]][:, :, :, None]
+        return new_ten.reshape((3, 3, -1))
+
 
 def compute_modes(*args, **kwargs) -> Tuple[Numpy, Numpy, str]:
     """A wrapper around ``EigSolver.compute_modes``, which is used in ``ModeSolver``."""
     return EigSolver.compute_modes(*args, **kwargs)
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/__init__.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/component_modelers/base.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/component_modelers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Base class for generating an S matrix automatically from tidy3d simulations and port definitions."""
 from __future__ import annotations
 from typing import Tuple, Dict, Union
 import os
 from abc import ABC, abstractmethod
+import json
 
 import pydantic.v1 as pd
 import numpy as np
 
 from ....constants import HERTZ
 from ....components.simulation import Simulation
 from ....components.data.data_array import DataArray
@@ -87,14 +88,23 @@
     solver_version: str = pd.Field(
         None,
         title="Solver Version",
         description_str="Custom solver version to use. "
         "If not supplied, uses default for the current front end version.",
     )
 
+    batch_cached: Batch = pd.Field(
+        None,
+        title="Batch (Cached)",
+        description="Optional field to specify ``batch``. Only used as a workaround internally "
+        "so that ``batch`` is written when ``.to_file()`` and then the proper batch is loaded "
+        "from ``.from_file()``. We recommend leaving unset as setting this field along with "
+        "fields that were not used to create the task will cause errors.",
+    )
+
     @pd.validator("simulation", always=True)
     def _sim_has_no_sources(cls, val):
         """Make sure simulation has no sources as they interfere with tool."""
         if len(val.sources) > 0:
             raise SetupError("'AbstractComponentModeler.simulation' must not have any sources.")
         return val
 
@@ -105,20 +115,38 @@
             return f"smatrix_{port.name}_{mode_index}"
         return f"smatrix_{port.name}"
 
     @cached_property
     def sim_dict(self) -> Dict[str, Simulation]:
         """Generate all the :class:`Simulation` objects for the S matrix calculation."""
 
+    def json(self, **kwargs):
+        """Save component to dictionary. Add the ``batch`` if it has been cached."""
+
+        self_json = super().json(**kwargs)
+
+        batch = self._cached_properties.get("batch")
+
+        if not batch:
+            return self_json
+
+        self_dict = json.loads(self_json)
+        self_dict["batch_cached"] = json.loads(batch.json())
+        return json.dumps(self_dict)
+
     @cached_property
     def batch(self) -> Batch:
         """Batch associated with this component modeler."""
 
+        if self.batch_cached is not None:
+            return self.batch_cached
+
         # first try loading the batch from file, if it exists
         batch_path = self._batch_path
+
         if os.path.exists(batch_path):
             return Batch.from_file(fname=batch_path)
 
         return Batch(
             simulations=self.sim_dict,
             folder_name=self.folder_name,
             callback_url=self.callback_url,
@@ -171,15 +199,14 @@
     @abstractmethod
     def _construct_smatrix(self, batch_data: BatchData) -> DataArray:
         """Post process :class:`BatchData` to generate scattering matrix."""
 
     def run(self, path_dir: str = DEFAULT_DATA_DIR) -> DataArray:
         """Solves for the scattering matrix of the system."""
         path_dir = self.get_path_dir(path_dir)
-
         batch_data = self._run_sims(path_dir=path_dir)
         return self._construct_smatrix(batch_data=batch_data)
 
     def load(self, path_dir: str = DEFAULT_DATA_DIR) -> DataArray:
         """Load a scattering matrix from saved :class:`BatchData` object."""
         path_dir = self.get_path_dir(path_dir)
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/component_modelers/modal.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/component_modelers/modal.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/component_modelers/terminal.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/component_modelers/terminal.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/ports/lumped.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/ports/lumped.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/smatrix/ports/modal.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/smatrix/ports/modal.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.7.0rc2/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/updater.py` & `tidy3d-2.7.0rc2/tidy3d/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,26 +89,26 @@
     sim_dict: dict
 
     @classmethod
     def from_file(cls, fname: str) -> Updater:
         """Dictionary representing the simulation loaded from file."""
 
         # TODO: fix this, it broke
-        if ".hdf5" in fname:
+        if any(ext in fname for ext in (".hdf5", ".gz")):
             sim_dict = Tidy3dBaseModel.from_file(fname=fname).dict()
 
         else:
             # try:
             with open(fname, encoding="utf-8") as f:
                 if ".json" in fname:
                     sim_dict = json.load(f)
                 elif ".yaml" in fname:
                     sim_dict = yaml.safe_load(f)
                 else:
-                    raise FileError('file extension must be ".json", ".yaml", or ".hdf5"')
+                    raise FileError('file extension must be ".json", ".yaml", ".hdf5", or ".gz"')
 
             # except Exception as e:
             #     raise FileError(f"Could not load file {fname}") from e
 
         return cls(sim_dict=sim_dict)
 
     @classmethod
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/__init__.py` & `tidy3d-2.7.0rc2/tidy3d/web/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/api/asynchronous.py` & `tidy3d-2.7.0rc2/tidy3d/web/api/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/api/cacert.pem` & `tidy3d-2.7.0rc2/tidy3d/web/api/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/api/connect_util.py` & `tidy3d-2.7.0rc2/tidy3d/web/api/connect_util.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/api/container.py` & `tidy3d-2.7.0rc2/tidy3d/web/api/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 """higher level wrappers for webapi functions for individual (Job) and batch (Batch) tasks."""
 from __future__ import annotations
 
 import os
 from abc import ABC
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Optional
 import time
+import json
+from concurrent.futures import ThreadPoolExecutor
+import concurrent
 
 from rich.progress import Progress
 import pydantic.v1 as pd
 
 from .tidy3d_stub import SimulationType, SimulationDataType
 from ..api import webapi as web
 from ..core.task_info import TaskInfo, RunInfo
 from ..core.constants import TaskId, TaskName
-from ...components.base import Tidy3dBaseModel
+from ...components.base import Tidy3dBaseModel, cached_property
 from ...components.types import annotate_type
 from ...log import log, get_logging_console
 
 from ...exceptions import DataError
 
+# Max # of workers for parallel upload / download: above 10, performance is same but with warnings
+DEFAULT_NUM_WORKERS = 10
 DEFAULT_DATA_PATH = "simulation_data.hdf5"
 DEFAULT_DATA_DIR = "."
+BATCH_MONITOR_PROGRESS_REFRESH_TIME = 0.02
 
 
 class WebContainer(Tidy3dBaseModel, ABC):
     """Base class for :class:`Job` and :class:`Batch`, technically not used"""
 
 
 class Job(WebContainer):
@@ -142,63 +148,78 @@
         description="Type of simulation, used internally only.",
     )
 
     parent_tasks: Tuple[TaskId, ...] = pd.Field(
         None, title="Parent Tasks", description="Tuple of parent task ids, used internally only."
     )
 
-    task_id: TaskId = pd.Field(
+    task_id_cached: TaskId = pd.Field(
         None,
-        title="Task Id",
-        description="Task ID number, set when the task is uploaded, leave as None.",
+        title="Task ID (Cached)",
+        description="Optional field to specify ``task_id``. Only used as a workaround internally "
+        "so that ``task_id`` is written when ``Job.to_file()`` and then the proper task is loaded "
+        "from ``Job.from_file()``. We recommend leaving unset as setting this field along with "
+        "fields that were not used to create the task will cause errors.",
     )
 
     _upload_fields = (
         "simulation",
         "task_name",
         "folder_name",
         "callback_url",
         "verbose",
         "simulation_type",
         "parent_tasks",
     )
 
+    def json(self, **kwargs):
+        """Save ``Job`` to dictionary. Add the `task_id` if it has been cached."""
+
+        self_json = super().json(**kwargs)
+
+        task_id = self._cached_properties.get("task_id")
+
+        if not task_id:
+            return self_json
+
+        self_dict = json.loads(self_json)
+        self_dict["task_id_cached"] = task_id
+        return json.dumps(self_dict)
+
     def run(self, path: str = DEFAULT_DATA_PATH) -> SimulationDataType:
         """Run :class:`Job` all the way through and return data.
 
         Parameters
         ----------
         path_dir : str = "./simulation_data.hdf5"
             Base directory where data will be downloaded, by default current working directory.
 
         Returns
         -------
         Union[:class:`.SimulationData`, :class:`.HeatSimulationData`, :class:`.EMESimulationData`]
             Object containing simulation results.
         """
 
+        self.upload()
         self.start()
         self.monitor()
         return self.load(path=path)
 
-    @pd.root_validator()
-    def _upload(cls, values) -> None:
-        """Upload simulation to server without running."""
-
-        # task_id already present, don't re-upload
-        if values.get("task_id") is not None:
-            return values
+    @cached_property
+    def task_id(self) -> TaskId:
+        """The task ID for this ``Job``. Uploads the ``Job`` if it hasn't already been uploaded."""
+        if self.task_id_cached:
+            return self.task_id_cached
+        return self.upload()
 
+    def upload(self) -> TaskId:
         # upload kwargs with all fields except task_id
-        upload_kwargs = {key: values.get(key) for key in cls._upload_fields}
-        task_id = web.upload(**upload_kwargs)
-
-        # then set the task_id and return
-        values["task_id"] = task_id
-        return values
+        self_dict = self.dict()
+        upload_kwargs = {key: self_dict.get(key) for key in self._upload_fields}
+        return web.upload(**upload_kwargs)
 
     def get_info(self) -> TaskInfo:
         """Return information about a :class:`Job`.
 
         Returns
         -------
         :class:`TaskInfo`
@@ -350,23 +371,25 @@
     )
 
     def load_sim_data(self, task_name: str) -> SimulationDataType:
         """Load a simulation data object from file by task name."""
         task_data_path = self.task_paths[task_name]
         task_id = self.task_ids[task_name]
         web.get_info(task_id)
+
         return web.load(
             task_id=task_id,
             path=task_data_path,
             replace_existing=False,
-            verbose=self.verbose,
+            verbose=False,
         )
 
     def items(self) -> Tuple[TaskName, SimulationDataType]:
         """Iterate through the simulations for each task_name."""
+
         for task_name in self.task_paths.keys():
             yield task_name, self.load_sim_data(task_name)
 
     def __getitem__(self, task_name: TaskName) -> SimulationDataType:
         """Get the simulation data object for a given ``task_name``."""
         return self.load_sim_data(task_name)
 
@@ -458,21 +481,34 @@
 
     parent_tasks: Dict[str, Tuple[TaskId, ...]] = pd.Field(
         None,
         title="Parent Tasks",
         description="Collection of parent task ids for each job in batch, used internally only.",
     )
 
-    jobs: Dict[TaskName, Job] = pd.Field(
+    num_workers: Optional[pd.PositiveInt] = pd.Field(
+        DEFAULT_NUM_WORKERS,
+        title="Number of Workers",
+        description="Number of workers for multi-threading upload and download of batch. "
+        "Corresponds to ``max_workers`` argument passed to "
+        "``concurrent.futures.ThreadPoolExecutor``. When left ``None``, will pass the maximum "
+        "number of threads available on the system.",
+    )
+
+    jobs_cached: Dict[TaskName, Job] = pd.Field(
         None,
-        title="Simulations",
-        description="Mapping of task names to individual Job object for each task in the batch. "
-        "Set by ``Batch.upload``, leave as None.",
+        title="Jobs (Cached)",
+        description="Optional field to specify ``jobs``. Only used as a workaround internally "
+        "so that ``jobs`` is written when ``Batch.to_file()`` and then the proper task is loaded "
+        "from ``Batch.from_file()``. We recommend leaving unset as setting this field along with "
+        "fields that were not used to create the task will cause errors.",
     )
 
+    _job_type = Job
+
     @staticmethod
     def _check_path_dir(path_dir: str) -> None:
         """Make sure ``path_dir`` exists and create one if not."""
 
         if not os.path.exists(path_dir):
             os.makedirs(path_dir, exist_ok=True)
 
@@ -501,48 +537,89 @@
         ...     # do something with data. # doctest: +SKIP
 
         ``bach_data`` does not store all of the data objects in memory,
         rather it iterates over the task names and loads the corresponding
         data from file one by one. If no file exists for that task, it downloads it.
         """
         self._check_path_dir(path_dir)
+        self.upload()
         self.start()
         self.monitor()
+        self.download(path_dir=path_dir)
         return self.load(path_dir=path_dir)
 
-    @pd.validator("jobs", always=True)
-    def _upload(cls, val, values) -> None:
+    @cached_property
+    def jobs(self) -> Dict[TaskName, Job]:
         """Create a series of tasks in the :class:`.Batch` and upload them to server.
 
         Note
         ----
         To start the simulations running, must call :meth:`Batch.start` after uploaded.
         """
-        if val is not None:
-            return val
+
+        if self.jobs_cached is not None:
+            return self.jobs_cached
 
         # the type of job to upload (to generalize to subclasses)
-        JobType = cls.__fields__["jobs"].type_
-        parent_tasks = values.get("parent_tasks")
+        JobType = self._job_type
+        self_dict = self.dict()
 
-        verbose = bool(values.get("verbose"))
-        solver_version = values.get("solver_version")
         jobs = {}
-        for task_name, simulation in values.get("simulations").items():
-            upload_kwargs = {key: values.get(key) for key in JobType._upload_fields}
-            upload_kwargs["task_name"] = task_name
-            upload_kwargs["simulation"] = simulation
-            upload_kwargs["verbose"] = verbose
-            upload_kwargs["solver_version"] = solver_version
-            if parent_tasks and task_name in parent_tasks:
-                upload_kwargs["parent_tasks"] = parent_tasks[task_name]
-            job = JobType(**upload_kwargs)
+        for task_name, simulation in self.simulations.items():
+            job_kwargs = {}
+
+            for key in JobType._upload_fields:
+                if key in self_dict:
+                    job_kwargs[key] = self_dict.get(key)
+
+            job_kwargs["task_name"] = task_name
+            job_kwargs["simulation"] = simulation
+            job_kwargs["verbose"] = False
+            job_kwargs["solver_version"] = self.solver_version
+            if self.parent_tasks and task_name in self.parent_tasks:
+                job_kwargs["parent_tasks"] = self.parent_tasks[task_name]
+            job = JobType(**job_kwargs)
             jobs[task_name] = job
         return jobs
 
+    def json(self, **kwargs):
+        """Save ``Batch`` to dictionary. Add the ``jobs`` if they have been cached."""
+
+        self_json = super().json(**kwargs)
+
+        jobs = self._cached_properties.get("jobs")
+
+        if not jobs:
+            return self_json
+
+        self_dict = json.loads(self_json)
+        self_dict["jobs_cached"] = {k: json.loads(j.json()) for k, j in jobs.items()}
+        return json.dumps(self_dict)
+
+    @property
+    def num_jobs(self) -> int:
+        """Number of jobs in the batch."""
+        return len(self.jobs)
+
+    def upload(self) -> None:
+        """Upload a series of tasks associated with this ``Batch`` using multi-threading."""
+
+        with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
+            futures = [executor.submit(job.upload) for _, job in self.jobs.items()]
+
+            # progressbar (number of tasks uploaded)
+            if self.verbose:
+                console = get_logging_console()
+                with Progress(console=console) as progress:
+                    pbar_message = f"Uploading data for {self.num_jobs} tasks."
+                    pbar = progress.add_task(pbar_message, total=self.num_jobs - 1)
+                    for _ in concurrent.futures.as_completed(futures):
+                        progress.update(pbar, advance=1)
+                    progress.update(pbar, completed=self.num_jobs - 1, refresh=True)
+
     def get_info(self) -> Dict[TaskName, TaskInfo]:
         """Get information about each task in the :class:`Batch`.
 
         Returns
         -------
         Dict[str, :class:`TaskInfo`]
             Mapping of task name to data about task associated with each task.
@@ -556,16 +633,21 @@
     def start(self) -> None:
         """Start running all tasks in the :class:`Batch`.
 
         Note
         ----
         To monitor the running simulations, can call :meth:`Batch.monitor`.
         """
-        for _, job in self.jobs.items():
-            job.start()
+        if self.verbose:
+            console = get_logging_console()
+            console.log(f"Started working on Batch containing {self.num_jobs} tasks.")
+
+        with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
+            for _, job in self.jobs.items():
+                executor.submit(job.start)
 
     def get_run_info(self) -> Dict[TaskName, RunInfo]:
         """get information about a each of the tasks in the :class:`Batch`.
 
         Returns
         -------
         Dict[str: :class:`RunInfo`]
@@ -605,29 +687,32 @@
             "visualize",
             "success",
         ]
         end_statuses = ("success", "error", "errored", "diverged", "diverge", "deleted", "draft")
 
         if self.verbose:
             console = get_logging_console()
-            console.log("Started working on Batch.")
 
             self.estimate_cost()
             console.log(
                 "Use 'Batch.real_cost()' to "
                 "get the billed FlexCredit cost after the Batch has completed."
             )
 
             with Progress(console=console) as progress:
                 # create progressbars
                 pbar_tasks = {}
                 for task_name, job in self.jobs.items():
                     status = job.status
                     description = pbar_description(task_name, status)
-                    pbar = progress.add_task(description, total=len(run_statuses) - 1)
+                    pbar = progress.add_task(
+                        description,
+                        total=len(run_statuses) - 1,
+                        completed=run_statuses.index(status),
+                    )
                     pbar_tasks[task_name] = pbar
 
                 while any(job.status not in end_statuses for job in self.jobs.values()):
                     for task_name, job in self.jobs.items():
                         pbar = pbar_tasks[task_name]
                         status = job.status
                         description = pbar_description(task_name, status)
@@ -635,15 +720,15 @@
                         # if a problem occurred, update progressbar completion to 100%
                         if status not in run_statuses:
                             completed = run_statuses.index("success")
                         else:
                             completed = run_statuses.index(status)
 
                         progress.update(pbar, description=description, completed=completed)
-                    time.sleep(web.REFRESH_TIME)
+                    time.sleep(BATCH_MONITOR_PROGRESS_REFRESH_TIME)
 
                 # set all to 100% completed (if error or diverge, will be red)
                 for task_name, job in self.jobs.items():
                     pbar = pbar_tasks[task_name]
                     status = job.status
                     description = pbar_description(task_name, status)
 
@@ -710,22 +795,40 @@
         The data for each task will be named as ``{path_dir}/{task_id}.hdf5``.
         The :class:`Batch` hdf5 file will be automatically saved as ``{path_dir}/batch.hdf5``,
         allowing one to load this :class:`Batch` later using ``batch = Batch.from_file()``.
         """
 
         self.to_file(self._batch_path(path_dir=path_dir))
 
-        for task_name, job in self.jobs.items():
-            job_path = self._job_data_path(task_id=job.task_id, path_dir=path_dir)
-
-            if "error" in job.status:
-                log.warning(f"Not downloading '{task_name}' as the task errored.")
-                continue
-
-            job.download(path=job_path)
+        with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
+            fns = []
+            for task_name, job in self.jobs.items():
+                job_path = self._job_data_path(task_id=job.task_id, path_dir=path_dir)
+
+                if "error" in job.status:
+                    log.warning(f"Not downloading '{task_name}' as the task errored.")
+                    continue
+
+                def fn(job=job, job_path=job_path) -> None:
+                    """Function to submit by executor, local variables bound by making kwargs."""
+                    return job.download(path=job_path)
+
+                fns.append(fn)
+
+            futures = [executor.submit(fn) for fn in fns]
+
+            # progressbar (number of eligible tasks downloaded)
+            if self.verbose:
+                console = get_logging_console()
+                with Progress(console=console) as progress:
+                    pbar_message = f"Downloading data for {len(fns)} tasks."
+                    pbar = progress.add_task(pbar_message, total=len(fns) - 1)
+                    for _ in concurrent.futures.as_completed(futures):
+                        progress.update(pbar, advance=1)
+                    progress.update(pbar, completed=len(fns) - 1, refresh=True)
 
     def load(self, path_dir: str = DEFAULT_DATA_DIR) -> BatchData:
         """Download results and load them into :class:`.BatchData` object.
 
         Parameters
         ----------
         path_dir : str = './'
@@ -803,15 +906,19 @@
         the full ``run_time``. If early shut-off is triggered, the cost is adjusted proportionately.
 
         Returns
         -------
         float
             Estimated total cost of the tasks in FlexCredits.
         """
-        batch_cost = sum(job.estimate_cost(verbose=False) for _, job in self.jobs.items())
+        job_costs = [job.estimate_cost(verbose=False) for _, job in self.jobs.items()]
+        if any(cost is None for cost in job_costs):
+            batch_cost = None
+        else:
+            batch_cost = sum(job_costs)
 
         if verbose:
             console = get_logging_console()
             if batch_cost is not None and batch_cost > 0:
                 console.log(f"Maximum FlexCredit cost: {batch_cost:1.3f} for the whole batch.")
             else:
                 console.log("Could not get estimated batch cost!")
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/api/material_fitter.py` & `tidy3d-2.7.0rc2/tidy3d/web/api/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/api/material_libray.py` & `tidy3d-2.7.0rc2/tidy3d/web/api/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/api/mode.py` & `tidy3d-2.7.0rc2/tidy3d/web/api/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/api/tidy3d_stub.py` & `tidy3d-2.7.0rc2/tidy3d/web/api/tidy3d_stub.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/api/webapi.py` & `tidy3d-2.7.0rc2/tidy3d/web/api/webapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,23 @@
 
 # time between checking run status
 RUN_REFRESH_TIME = 1.0
 
 # file names when uploading to S3
 SIM_FILE_JSON = "simulation.json"
 
+# not all solvers are supported yet in GUI
+GUI_SUPPORTED_TASK_TYPES = ["FDTD", "MODE_SOLVER", "HEAT"]
+
+# if a solver is in beta stage, cost is subject to change
+BETA_TASK_TYPES = ["HEAT", "EME"]
+
+# map task_type to solver name for display
+SOLVER_NAME = {"FDTD": "FDTD", "HEAT": "Heat", "MODE_SOLVER": "Mode", "EME": "EME"}
+
 
 def _get_url(task_id: str) -> str:
     """Get the URL for a task on our server."""
     return f"{Env.current.website_endpoint}/workbench?taskId={task_id}"
 
 
 @wait_for_connection
@@ -208,26 +217,23 @@
         task_type, task_name, folder_name, callback_url, simulation_type, parent_tasks, "Gz"
     )
     if verbose:
         console = get_logging_console()
         console.log(
             f"Created task '{task_name}' with task_id '{task.task_id}' and task_type '{task_type}'."
         )
-        if task_type == "HEAT":
+        if task_type in BETA_TASK_TYPES:
+            solver_name = SOLVER_NAME[task_type]
             console.log(
-                "Tidy3D's heat solver is currently in the beta stage. Cost of heat simulations "
-                "is subject to change in the future."
+                f"Tidy3D's {solver_name} solver is currently in the beta stage. "
+                f"Cost of {solver_name} simulations is subject to change in the future."
             )
-        elif task_type == "EME":
-            console.log(
-                "Tidy3D's EME solver is currently in the beta stage. Cost of EME simulations "
-                "is subject to change in the future."
-            )
-        url = _get_url(task.task_id)
-        console.log(f"View task using web UI at [link={url}]'{url}'[/link].")
+        if task_type in GUI_SUPPORTED_TASK_TYPES:
+            url = _get_url(task.task_id)
+            console.log(f"View task using web UI at [link={url}]'{url}'[/link].")
 
     task.upload_simulation(stub=stub, verbose=verbose, progress_callback=progress_callback)
 
     # log the url for the task in the web UI
     log.debug(f"{Env.current.website_endpoint}/folders/{task.folder_id}/tasks/{task.task_id}")
     return task.task_id
 
@@ -350,162 +356,136 @@
     To load results when finished, may call :meth:`load`.
     """
 
     console = get_logging_console() if verbose else None
 
     task_info = get_info(task_id)
 
-    if task_info.taskType in ("MODE_SOLVER", "HEAT", "EME"):
-        log_level = "DEBUG" if verbose else "INFO"
-        if task_info.taskType == "MODE_SOLVER":
-            solver_name = "Mode"
-        elif task_info.taskType == "HEAT":
-            solver_name = "Heat"
-        elif task_info.taskType == "EME":
-            solver_name = "EME"
-
-        # Wait for task to finish
-        prev_status = "draft"
-        status = get_status(task_id)
-        while status not in ("success", "error", "diverged", "deleted"):
-            if status != prev_status:
-                log.log(log_level, f"{solver_name} solver status: {status}")
-                if verbose:
-                    console.log(f"{solver_name} solver status: {status}")
-                prev_status = status
-            time.sleep(0.5)
-            status = get_status(task_id)
-
-        log.log(log_level, f"{solver_name} solver status: {status}")
-        if verbose:
-            console.log(f"{solver_name} solver status: {status}")
-
-        if status != "success":
-            # Our cache discards None, so the user is able to re-run
-            return None
-
-    elif task_info.taskType == "FDTD":
-        task_name = task_info.taskName
-
-        break_statuses = ("success", "error", "diverged", "deleted", "draft", "abort")
-
-        def get_estimated_cost() -> float:
-            """Get estimated cost, if None, is not ready."""
-            task_info = get_info(task_id)
-            block_info = task_info.taskBlockInfo
-            if block_info and block_info.chargeType == ChargeType.FREE:
-                est_flex_unit = 0
-                grid_points = block_info.maxGridPoints
-                time_steps = block_info.maxTimeSteps
-                grid_points_str = get_grid_points_str(grid_points)
-                time_steps_str = get_time_steps_str(time_steps)
-                console.log(
-                    f"You are running this simulation for FREE. Your current plan allows"
-                    f" up to {block_info.maxFreeCount} free non-concurrent simulations per"
-                    f" day (under {grid_points_str} grid points and {time_steps_str}"
-                    f" time steps)"
-                )
-            else:
-                est_flex_unit = task_info.estFlexUnit
-                if est_flex_unit is not None and est_flex_unit > 0:
-                    console.log(
-                        f"Maximum FlexCredit cost: {est_flex_unit:1.3f}. Use 'web.real_cost(task_id)'"
-                        f" to get the billed FlexCredit cost after a simulation run."
-                    )
-            return est_flex_unit
-
-        def monitor_preprocess() -> None:
-            """Periodically check the status."""
-            status = get_status(task_id)
-            while status not in break_statuses and status != "running":
-                new_status = get_status(task_id)
-                if new_status != status:
-                    status = new_status
-                    if verbose and status != "running":
-                        console.log(f"status = {status}")
-                time.sleep(REFRESH_TIME)
-
-        status = get_status(task_id)
+    task_name = task_info.taskName
 
-        if verbose:
-            console.log(f"status = {status}")
+    task_type = task_info.taskType
 
-        # already done
-        if status in break_statuses:
-            return
+    break_statuses = ("success", "error", "diverged", "deleted", "draft", "abort")
 
-        # preprocessing
-        if verbose:
+    def get_estimated_cost() -> float:
+        """Get estimated cost, if None, is not ready."""
+        task_info = get_info(task_id)
+        block_info = task_info.taskBlockInfo
+        if block_info and block_info.chargeType == ChargeType.FREE:
+            est_flex_unit = 0
+            grid_points = block_info.maxGridPoints
+            time_steps = block_info.maxTimeSteps
+            grid_points_str = get_grid_points_str(grid_points)
+            time_steps_str = get_time_steps_str(time_steps)
             console.log(
-                "To cancel the simulation, use 'web.abort(task_id)' or 'web.delete(task_id)' "
-                "or abort/delete the task in the web "
-                "UI. Terminating the Python script will not stop the job running on the cloud."
+                f"You are running this simulation for FREE. Your current plan allows"
+                f" up to {block_info.maxFreeCount} free non-concurrent simulations per"
+                f" day (under {grid_points_str} grid points and {time_steps_str}"
+                f" time steps)"
             )
-            with console.status(f"[bold green]Waiting for '{task_name}'...", spinner="runner"):
-                monitor_preprocess()
         else:
-            monitor_preprocess()
-
-        # if the estimated cost is ready, print it
-        if verbose:
-            get_estimated_cost()
-            console.log("starting up solver")
+            est_flex_unit = task_info.estFlexUnit
+            if est_flex_unit is not None and est_flex_unit > 0:
+                console.log(
+                    f"Maximum FlexCredit cost: {est_flex_unit:1.3f}. Use 'web.real_cost(task_id)'"
+                    f" to get the billed FlexCredit cost after a simulation run."
+                )
+        return est_flex_unit
 
-        # while running but before the percentage done is available, keep waiting
-        while get_run_info(task_id)[0] is None and get_status(task_id) == "running":
+    def monitor_preprocess() -> None:
+        """Periodically check the status."""
+        status = get_status(task_id)
+        while status not in break_statuses and status != "running":
+            new_status = get_status(task_id)
+            if new_status != status:
+                status = new_status
+                if verbose and status != "running":
+                    console.log(f"status = {status}")
             time.sleep(REFRESH_TIME)
 
-        # while running but percentage done is available
-        if verbose:
-            # verbose case, update progressbar
-            console.log("running solver")
-            with Progress(console=console) as progress:
-                pbar_pd = progress.add_task("% done", total=100)
-                perc_done, _ = get_run_info(task_id)
-
-                while (
-                    perc_done is not None and perc_done < 100 and get_status(task_id) == "running"
-                ):
-                    perc_done, field_decay = get_run_info(task_id)
-                    new_description = f"solver progress (field decay = {field_decay:.2e})"
-                    progress.update(pbar_pd, completed=perc_done, description=new_description)
-                    time.sleep(RUN_REFRESH_TIME)
+    status = get_status(task_id)
 
-                perc_done, field_decay = get_run_info(task_id)
-                if perc_done is not None and perc_done < 100 and field_decay > 0:
-                    console.log(f"early shutoff detected at {perc_done:1.0f}%, exiting.")
+    if verbose:
+        console.log(f"status = {status}")
 
-                new_description = f"solver progress (field decay = {field_decay:.2e})"
-                progress.update(pbar_pd, completed=100, refresh=True, description=new_description)
+    # already done
+    if status in break_statuses:
+        return
 
-        else:
-            # non-verbose case, just keep checking until status is not running or perc_done >= 100
+    # preprocessing
+    if verbose:
+        console.log(
+            "To cancel the simulation, use 'web.abort(task_id)' or 'web.delete(task_id)' "
+            "or abort/delete the task in the web "
+            "UI. Terminating the Python script will not stop the job running on the cloud."
+        )
+        with console.status(f"[bold green]Waiting for '{task_name}'...", spinner="runner"):
+            monitor_preprocess()
+    else:
+        monitor_preprocess()
+
+    # if the estimated cost is ready, print it
+    if verbose:
+        get_estimated_cost()
+        console.log("starting up solver")
+
+    # while running but before the percentage done is available, keep waiting
+    while get_run_info(task_id)[0] is None and get_status(task_id) == "running":
+        time.sleep(REFRESH_TIME)
+
+    # while running but percentage done is available
+    if verbose and task_type == "FDTD":
+        # verbose case, update progressbar
+        console.log("running solver")
+        with Progress(console=console) as progress:
+            pbar_pd = progress.add_task("% done", total=100)
             perc_done, _ = get_run_info(task_id)
+
             while perc_done is not None and perc_done < 100 and get_status(task_id) == "running":
                 perc_done, field_decay = get_run_info(task_id)
-                time.sleep(1.0)
+                new_description = f"solver progress (field decay = {field_decay:.2e})"
+                progress.update(pbar_pd, completed=perc_done, description=new_description)
+                time.sleep(RUN_REFRESH_TIME)
+
+            perc_done, field_decay = get_run_info(task_id)
+            if perc_done is not None and perc_done < 100 and field_decay > 0:
+                console.log(f"early shutoff detected at {perc_done:1.0f}%, exiting.")
+
+            new_description = f"solver progress (field decay = {field_decay:.2e})"
+            progress.update(pbar_pd, completed=100, refresh=True, description=new_description)
+
+    # TODO: progressbar for EME
+
+    else:
+        # non-verbose case, just keep checking until status is not running or perc_done >= 100
+        perc_done, _ = get_run_info(task_id)
+        while perc_done is not None and perc_done < 100 and get_status(task_id) == "running":
+            perc_done, field_decay = get_run_info(task_id)
+            time.sleep(1.0)
 
-        # post processing
-        if verbose:
-            status = get_status(task_id)
-            if status != "running":
-                console.log(f"status = {status}")
-
-            with console.status(f"[bold green]Finishing '{task_name}'...", spinner="runner"):
-                while status not in break_statuses:
-                    new_status = get_status(task_id)
-                    if new_status != status:
-                        status = new_status
-                        console.log(f"status = {status}")
-                    time.sleep(REFRESH_TIME)
+    # post processing
+    if verbose:
+        status = get_status(task_id)
+        if status != "running":
+            console.log(f"status = {status}")
+
+        with console.status(f"[bold green]Finishing '{task_name}'...", spinner="runner"):
+            while status not in break_statuses:
+                new_status = get_status(task_id)
+                if new_status != status:
+                    status = new_status
+                    console.log(f"status = {status}")
+                time.sleep(REFRESH_TIME)
+
+        if task_type in GUI_SUPPORTED_TASK_TYPES:
             url = _get_url(task_id)
             console.log(f"View simulation result at [blue underline][link={url}]'{url}'[/link].")
-        else:
-            while get_status(task_id) not in break_statuses:
-                time.sleep(REFRESH_TIME)
+    else:
+        while get_status(task_id) not in break_statuses:
+            time.sleep(REFRESH_TIME)
 
 
 @wait_for_connection
 def download(
     task_id: TaskId,
     path: str = "simulation_data.hdf5",
     verbose: bool = True,
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/cli/app.py` & `tidy3d-2.7.0rc2/tidy3d/web/cli/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import requests
 import toml
 
 from ..cli.constants import TIDY3D_DIR, CONFIG_FILE, CREDENTIAL_FILE
 from ..cli.migrate import migrate
 from ..core.constants import KEY_APIKEY, HEADER_APIKEY
 from ..core.environment import Env
-from ..cli.converter import converter_arg
 from .develop.index import develop
 
 if not os.path.exists(TIDY3D_DIR):
     os.mkdir(TIDY3D_DIR)
 
 
 def get_description():
@@ -114,18 +113,22 @@
 @click.command()
 def migration():
     """Click command to migrate the credential to api key."""
     migrate()
 
 
 @click.command()
-@click.argument("lsf_file", type=click.Path(exists=True))
+@click.argument("lsf_file")
 @click.argument("new_file")
 def convert(lsf_file, new_file):
     """Click command to convert .lsf project into Tidy3D .py file"""
-    converter_arg(lsf_file, new_file)
+    raise ValueError(
+        "The converter feature is deprecated. "
+        "To use this feature, please use the external tool at "
+        "'https://github.com/hirako22/Lumerical-to-Tidy3D-Converter'."
+    )
 
 
 tidy3d_cli.add_command(configure)
 tidy3d_cli.add_command(migration)
 tidy3d_cli.add_command(convert)
 tidy3d_cli.add_command(develop)
```

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/cli/develop/__init__.py` & `tidy3d-2.7.0rc2/tidy3d/web/cli/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/cli/develop/documentation.py` & `tidy3d-2.7.0rc2/tidy3d/web/cli/develop/documentation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/cli/develop/install.py` & `tidy3d-2.7.0rc2/tidy3d/web/cli/develop/install.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/cli/develop/packaging.py` & `tidy3d-2.7.0rc2/tidy3d/web/cli/develop/packaging.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/cli/develop/tests.py` & `tidy3d-2.7.0rc2/tidy3d/web/cli/develop/tests.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/cli/develop/utils.py` & `tidy3d-2.7.0rc2/tidy3d/web/cli/develop/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/cli/migrate.py` & `tidy3d-2.7.0rc2/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/cli/readme.md` & `tidy3d-2.7.0rc2/tidy3d/web/cli/readme.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/constants.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/core_config.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/core_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/environment.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/file_util.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/file_util.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/http_util.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/http_util.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/s3utils.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/stub.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/stub.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/task_core.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/task_core.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/task_info.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/task_info.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/tidy3d/web/core/types.py` & `tidy3d-2.7.0rc2/tidy3d/web/core/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.7.0rc1/PKG-INFO` & `tidy3d-2.7.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.7.0rc1
+Version: 2.7.0rc2
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 License: LGPLv2+
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
@@ -20,33 +20,34 @@
 Provides-Extra: gdspy
 Provides-Extra: gdstk
 Provides-Extra: jax
 Provides-Extra: trimesh
 Provides-Extra: vtk
 Requires-Dist: PyYAML
 Requires-Dist: black (==23.12.1) ; extra == "dev"
-Requires-Dist: boto3 (==1.28.*)
+Requires-Dist: boto3 (>=1.28.0,<2.0.0)
 Requires-Dist: bump-my-version ; extra == "dev"
-Requires-Dist: click (==8.1.*)
+Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: cma ; extra == "dev" or extra == "docs"
 Requires-Dist: coverage ; extra == "dev"
 Requires-Dist: dask
 Requires-Dist: devsim ; extra == "dev" or extra == "docs"
 Requires-Dist: dill ; extra == "dev"
 Requires-Dist: flax (>=0.8.2)
 Requires-Dist: gdspy ; extra == "dev" or extra == "gdspy"
 Requires-Dist: gdstk (>=0.9.49) ; extra == "dev" or extra == "dev" or extra == "docs" or extra == "gdstk"
 Requires-Dist: grcwa ; extra == "dev" or extra == "docs"
 Requires-Dist: h5netcdf (==1.0.2)
 Requires-Dist: h5py (>=3.0.0,<4.0.0)
 Requires-Dist: importlib-metadata (>=6.0.0)
 Requires-Dist: ipython ; extra == "dev" or extra == "dev" or extra == "docs"
-Requires-Dist: jax[cpu] (>=0.4.13,<=0.4.26) ; extra == "dev" or extra == "jax"
-Requires-Dist: jaxlib (>=0.4.13,<=0.4.26) ; extra == "dev" or extra == "jax"
+Requires-Dist: jax[cpu] (==0.4.25) ; extra == "dev" or extra == "jax"
+Requires-Dist: jaxlib (==0.4.25) ; extra == "dev" or extra == "jax"
 Requires-Dist: jinja2 (>=3.1.2) ; extra == "dev" or extra == "docs"
+Requires-Dist: joblib
 Requires-Dist: jupyter ; extra == "dev" or extra == "docs"
 Requires-Dist: matplotlib
 Requires-Dist: memory_profiler ; extra == "dev"
 Requires-Dist: myst-parser ; extra == "dev" or extra == "docs"
 Requires-Dist: nbconvert (>=7.11.0) ; extra == "dev" or extra == "docs"
 Requires-Dist: nbdime ; extra == "dev" or extra == "docs"
 Requires-Dist: nbsphinx (>=0.8.7) ; extra == "dev" or extra == "docs"
@@ -59,20 +60,20 @@
 Requires-Dist: pydata-sphinx-theme (>=0.13.3) ; extra == "dev" or extra == "docs"
 Requires-Dist: pyjwt
 Requires-Dist: pylint ; extra == "dev" or extra == "docs"
 Requires-Dist: pyroots (>=0.5.0)
 Requires-Dist: pyswarms ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-timeout ; extra == "dev"
-Requires-Dist: requests (==2.31.*)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: responses
-Requires-Dist: rich (<12.6.0)
+Requires-Dist: rich (>=13.0,<14.0)
 Requires-Dist: rtree (==1.2.0) ; extra == "dev" or extra == "trimesh"
 Requires-Dist: ruff (==0.3.2) ; extra == "dev"
-Requires-Dist: sax ; extra == "dev" or extra == "docs"
+Requires-Dist: sax (>=0.11,<0.12) ; extra == "dev" or extra == "docs"
 Requires-Dist: scipy
 Requires-Dist: shapely (>=2.0,<3.0)
 Requires-Dist: signac ; extra == "dev" or extra == "docs"
 Requires-Dist: sphinx (>=6) ; extra == "dev" or extra == "docs"
 Requires-Dist: sphinx-book-theme (>=1.0.1) ; extra == "dev" or extra == "docs"
 Requires-Dist: sphinx-copybutton (>=0.5.2) ; extra == "dev" or extra == "docs"
 Requires-Dist: sphinx-favicon ; extra == "dev" or extra == "docs"
```

