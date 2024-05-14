# Comparing `tmp/altrios-0.2.1.tar.gz` & `tmp/altrios-0.2.2.tar.gz`

## Comparing `altrios-0.2.1.tar` & `altrios-0.2.2.tar`

### file list

```diff
@@ -1,204 +1,204 @@
--rw-r--r--   0     1001      127     1232 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/Cargo.toml
--rw-r--r--   0     1001      127      784 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/README.md
--rw-r--r--   0     1001      127     2475 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/combo_error.rs
--rw-r--r--   0     1001      127    22741 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/consist_model.rs
--rw-r--r--   0     1001      127     4095 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/consist_sim.rs
--rw-r--r--   0     1001      127    12088 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/consist_utils.rs
--rw-r--r--   0     1001      127     3176 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs
--rw-r--r--   0     1001      127     3606 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/conventional_loco.rs
--rw-r--r--   0     1001      127    12008 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs
--rw-r--r--   0     1001      127    13285 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/loco_sim.rs
--rw-r--r--   0     1001      127    39926 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/locomotive_model.rs
--rw-r--r--   0     1001      127      991 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/mod.rs
--rw-r--r--   0     1001      127      430 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.default.yaml
--rw-r--r--   0     1001      127    14859 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs
--rw-r--r--   0     1001      127     1034 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml
--rw-r--r--   0     1001      127    13407 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs
--rw-r--r--   0     1001      127      348 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/generator.default.yaml
--rw-r--r--   0     1001      127    14475 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs
--rw-r--r--   0     1001      127      213 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/mod.rs
--rw-r--r--   0     1001      127      938 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs
--rw-r--r--   0     1001      127     9907 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml
--rw-r--r--   0     1001      127    30918 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs
--rw-r--r--   0     1001      127      200 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/test.rs
--rw-r--r--   0     1001      127     2790 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/locomotive/tests.rs
--rw-r--r--   0     1001      127      752 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/mod.rs
--rw-r--r--   0     1001      127     1039 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/consist/tests.rs
--rw-r--r--   0     1001      127     1254 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/imports.rs
--rw-r--r--   0     1001      127     1142 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/lib.rs
--rw-r--r--   0     1001      127     1602 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/lin_search_hint.rs
--rw-r--r--   0     1001      127     8028 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/macros.rs
--rw-r--r--   0     1001      127      482 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/disp_imports.rs
--rw-r--r--   0     1001      127     5431 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/disp_structs.rs
--rw-r--r--   0     1001      127    11495 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/dispatch.rs
--rw-r--r--   0     1001      127     2661 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs
--rw-r--r--   0     1001      127    29031 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/est_times/mod.rs
--rw-r--r--   0     1001      127     9721 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/est_times/update_times.rs
--rw-r--r--   0     1001      127      281 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/mod.rs
--rw-r--r--   0     1001      127    25666 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs
--rw-r--r--   0     1001      127    36649 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/train_disp/free_path.rs
--rw-r--r--   0     1001      127     9540 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/meet_pass/train_disp/mod.rs
--rw-r--r--   0     1001      127     1969 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/prelude.rs
--rw-r--r--   0     1001      127      255 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/pyo3.rs
--rw-r--r--   0     1001      127     1039 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/si.rs
--rw-r--r--   0     1001      127     2613 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/testing.rs
--rw-r--r--   0     1001      127     2129 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/cat_power.rs
--rw-r--r--   0     1001      127     4039 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/elev.rs
--rw-r--r--   0     1001      127     4947 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/heading.rs
--rw-r--r--   0     1001      127     4752 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/link_idx.rs
--rw-r--r--   0     1001      127    23686 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/link_impl.rs
--rw-r--r--   0     1001      127     1387 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/link_old.rs
--rw-r--r--   0     1001      127     1900 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/location.rs
--rw-r--r--   0     1001      127      246 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/locations.csv
--rw-r--r--   0     1001      127      301 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/mod.rs
--rw-r--r--   0     1001      127     4792 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/speed/speed_limit.rs
--rw-r--r--   0     1001      127     3242 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/speed/speed_param.rs
--rw-r--r--   0     1001      127     5971 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/speed/speed_set.rs
--rw-r--r--   0     1001      127      120 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/link/speed.rs
--rw-r--r--   0     1001      127      120 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/mod.rs
--rw-r--r--   0     1001      127     6079 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/path_track/link_point.rs
--rw-r--r--   0     1001      127      182 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/path_track/mod.rs
--rw-r--r--   0     1001      127     2826 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/path_track/path_res_coeff.rs
--rw-r--r--   0     1001      127    19995 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/path_track/path_tpc.rs
--rw-r--r--   0     1001      127     7804 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/path_track/speed_point.rs
--rw-r--r--   0     1001      127     3842 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/track/path_track/train_params.rs
--rw-r--r--   0     1001      127     6200 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/braking_point.rs
--rw-r--r--   0     1001      127     3503 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/friction_brakes.rs
--rw-r--r--   0     1001      127      344 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/mod.rs
--rw-r--r--   0     1001      127     3605 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/rail_vehicle.rs
--rw-r--r--   0     1001      127     1124 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs
--rw-r--r--   0     1001      127      324 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/kind/bearing.rs
--rw-r--r--   0     1001      127      438 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/kind/davis_b.rs
--rw-r--r--   0     1001      127       90 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/kind/mod.rs
--rw-r--r--   0     1001      127     4158 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/kind/path_res.rs
--rw-r--r--   0     1001      127      397 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/kind/rolling.rs
--rw-r--r--   0     1001      127      133 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/method/mod.rs
--rw-r--r--   0     1001      127     2253 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/method/point.rs
--rw-r--r--   0     1001      127     2684 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/method/strap.rs
--rw-r--r--   0     1001      127     1780 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/resistance/mod.rs
--rw-r--r--   0     1001      127    13755 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/set_speed_train_sim.rs
--rw-r--r--   0     1001      127    24549 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/speed_limit_train_sim.rs
--rw-r--r--   0     1001      127      443 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/test_rail_vehicles.csv
--rw-r--r--   0     1001      127      182 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/timed_path.rs
--rw-r--r--   0     1001      127    40485 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/train_config.rs
--rw-r--r--   0     1001      127      338 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/train_imports.rs
--rw-r--r--   0     1001      127     8167 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/train/train_state.rs
--rw-r--r--   0     1001      127    10138 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/traits.rs
--rw-r--r--   0     1001      127     2849 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/uc.rs
--rw-r--r--   0     1001      127    13949 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/utils/mod.rs
--rw-r--r--   0     1001      127     2455 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/utils/val_range.rs
--rw-r--r--   0     1001      127     7292 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/src/validate.rs
--rw-r--r--   0     1001      127      578 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/Cargo.toml
--rw-r--r--   0     1001      127      707 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/README.md
--rw-r--r--   0     1001      127    10749 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs
--rw-r--r--   0     1001      127    13309 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/altrios_api/mod.rs
--rw-r--r--   0     1001      127     4077 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs
--rw-r--r--   0     1001      127     2741 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs
--rw-r--r--   0     1001      127      367 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/imports.rs
--rw-r--r--   0     1001      127     1192 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/lib.rs
--rw-r--r--   0     1001      127      571 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs
--rw-r--r--   0     1001      127     3154 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/utilities.rs
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 altrios-0.2.1/rust/altrios-py/Cargo.toml
--rw-r--r--   0     1001      127      586 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-py/README.md
--rw-r--r--   0     1001      127     3080 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/altrios-py/src/lib.rs
--rw-r--r--   0     1001      127    63018 2024-04-17 18:08:48.000000 altrios-0.2.1/rust/Cargo.lock
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 altrios-0.2.1/rust/Cargo.toml
--rw-r--r--   0     1001      127     2197 2024-04-17 18:08:48.000000 altrios-0.2.1/pyproject.toml
--rw-r--r--   0     1001      127      766 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/stringline_old.py
--rw-r--r--   0     1001      127      386 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/plot.py
--rw-r--r--   0     1001      127     5988 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/speed_limit_train_sim_demo.py
--rw-r--r--   0     1001      127     4220 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/speed_limit_simple_corr_demo.py
--rw-r--r--   0     1001      127     5592 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/sim_manager_demo.py
--rw-r--r--   0     1001      127     1006 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/version_migration_demo.py
--rw-r--r--   0     1001      127     3410 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/set_speed_simple_corr_demo.py
--rw-r--r--   0     1001      127     3488 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/rollout_demo.py
--rw-r--r--   0     1001      127      111 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/__init__.py
--rw-r--r--   0     1001      127     3903 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/set_speed_train_sim_demo.py
--rw-r--r--   0     1001      127      578 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/test_demos.py
--rw-r--r--   0     1001      127     2357 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/conv_demo.py
--rw-r--r--   0     1001      127     2377 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/bel_demo.py
--rw-r--r--   0     1001      127      278 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/demos/demo_logging.py
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/py.typed
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/fuel_grid.py
--rw-r--r--   0     1001      127    53858 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/train_planner.py
--rw-r--r--   0     1001      127    52841 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/output_12072022.csv
--rw-r--r--   0     1001      127     8741 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/utilities.py
--rw-r--r--   0     1001      127    16755 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/stringline.py
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/objectives.py
--rw-r--r--   0     1001      127     1078 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/__init__.py
--rw-r--r--   0     1001      127    41804 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/metric_calculator.py
--rw-r--r--   0     1001      127  1237826 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv
--rw-r--r--   0     1001      127      994 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv
--rw-r--r--   0     1001      127     2025 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv
--rw-r--r--   0     1001      127     1616 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv
--rw-r--r--   0     1001      127    10562 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv
--rw-r--r--   0     1001      127   128287 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/powertrain_model_input_example.csv
--rw-r--r--   0     1001      127      695 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/Default Demand StoBar.csv
--rw-r--r--   0     1001      127       50 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/tpc_input_example.csv
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/__init__.py
--rw-r--r--   0     1001      127      492 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/rolling_stock/Unit_Empty.yaml
--rw-r--r--   0     1001      127      501 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/rolling_stock/Unit.yaml
--rw-r--r--   0     1001      127      496 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/rolling_stock/Manifest_Empty.yaml
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/rolling_stock/__init__.py
--rw-r--r--   0     1001      127      511 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/rolling_stock/Manifest.yaml
--rw-r--r--   0     1001      127      641 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/rolling_stock/rail_vehicles.csv
--rw-r--r--   0     1001      127      492 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/rolling_stock/Intermodal.yaml
--rw-r--r--   0     1001      127      498 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/rolling_stock/Intermodal_Empty.yaml
--rw-r--r--   0     1001      127      568 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/trains/train_res_temp.yaml
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/trains/__init__.py
--rw-r--r--   0     1001      127    25350 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx
--rw-r--r--   0     1001      127     9907 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/powertrains/reversible_energy_storages/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/powertrains/__init__.py
--rw-r--r--   0     1001      127      999 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/powertrains/fuel_converters/__init__.py
--rw-r--r--   0     1001      127      191 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/demo_data/README.md
--rw-r--r--   0     1001      127       15 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/demo_data/link_points_idx_simple_corridor.csv
--rw-r--r--   0     1001      127     2279 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/demo_data/speed_trace.csv
--rw-r--r--   0     1001      127      274 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/demo_data/speed_trace_simple_corridor.csv
--rw-r--r--   0     1001      127      350 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/demo_data/link_points_idx.csv
--rw-r--r--   0     1001      127      253 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/Default Demand.csv
--rw-r--r--   0     1001      127    67018 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/TimedPaths.csv
--rw-r--r--   0     1001      127  3119913 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/Taconite-NoBalloon.yaml
--rw-r--r--   0     1001      127      390 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/default_locations.csv
--rw-r--r--   0     1001      127     1153 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/links_test.yaml
--rw-r--r--   0     1001      127      136 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/network_charging_guidelines.csv
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/__init__.py
--rw-r--r--   0     1001      127  3128676 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/Taconite_v0.1.6.yaml
--rw-r--r--   0     1001      127      548 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv
--rw-r--r--   0     1001      127     3595 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/simple_corridor_network.yaml
--rw-r--r--   0     1001      127      214 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/simple_corridor_locations.csv
--rw-r--r--   0     1001      127  3192802 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/resources/networks/Taconite.yaml
--rw-r--r--   0     1001      127     2074 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/defaults.py
--rw-r--r--   0     1001      127     6896 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/rollout.py
--rw-r--r--   0     1001      127     3448 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/loaders/powertrain_components.py
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/loaders/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/user_interface.py
--rw-r--r--   0     1001      127     5693 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/sim_manager.py
--rw-r--r--   0     1001      127      603 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_consist.py
--rw-r--r--   0     1001      127      652 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_rail_vehicles.py
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_multi_obj_opt.py
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_fuel_grid.py
--rw-r--r--   0     1001      127     1279 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_powertrain_fuel_conv.py
--rw-r--r--   0     1001      127     1019 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_utilities.py
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_objectives.py
--rw-r--r--   0     1001      127      747 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_powertrain_generator.py
--rw-r--r--   0     1001      127     1533 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_locomotive.py
--rw-r--r--   0     1001      127      229 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_train_planner.py
--rw-r--r--   0     1001      127      874 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_powertrain_edrive.py
--rw-r--r--   0     1001      127        0 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/__init__.py
--rw-r--r--   0     1001      127      675 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_consist_sim.py
--rw-r--r--   0     1001      127     2351 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_multi_obj_cal_and_val.py
--rw-r--r--   0     1001      127     1754 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_powertrain_res.py
--rw-r--r--   0     1001      127      928 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_metric_calculator.py
--rw-r--r--   0     1001      127      386 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_train_simulation.py
--rw-r--r--   0     1001      127     7941 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/mock_resources.py
--rw-r--r--   0     1001      127      689 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/tests/test_locomotive_simulation.py
--rw-r--r--   0     1001      127    29921 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/altrios_pyo3.pyi
--rw-r--r--   0     1001      127       91 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/optimization/multi_obj_opt.py
--rw-r--r--   0     1001      127       25 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/optimization/__init__.py
--rw-r--r--   0     1001      127    24477 2024-04-17 18:08:48.000000 altrios-0.2.1/python/altrios/optimization/cal_and_val.py
--rw-r--r--   0     1001      127     7492 2024-04-17 18:08:48.000000 altrios-0.2.1/README.md
--rw-r--r--   0     1001      127     1660 2024-04-17 18:08:48.000000 altrios-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     9102 1970-01-01 00:00:00.000000 altrios-0.2.1/PKG-INFO
+-rw-r--r--   0     1001      127     1201 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/Cargo.toml
+-rw-r--r--   0     1001      127      784 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/README.md
+-rw-r--r--   0     1001      127     2475 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/combo_error.rs
+-rw-r--r--   0     1001      127    22917 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/consist_model.rs
+-rw-r--r--   0     1001      127     3981 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/consist_sim.rs
+-rw-r--r--   0     1001      127    12088 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/consist_utils.rs
+-rw-r--r--   0     1001      127     3176 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs
+-rw-r--r--   0     1001      127     3606 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/conventional_loco.rs
+-rw-r--r--   0     1001      127    12008 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs
+-rw-r--r--   0     1001      127    13342 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/loco_sim.rs
+-rw-r--r--   0     1001      127    39926 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/locomotive_model.rs
+-rw-r--r--   0     1001      127      991 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/mod.rs
+-rw-r--r--   0     1001      127      430 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.default.yaml
+-rw-r--r--   0     1001      127    14931 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs
+-rw-r--r--   0     1001      127     1034 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml
+-rw-r--r--   0     1001      127    13407 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs
+-rw-r--r--   0     1001      127      348 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/generator.default.yaml
+-rw-r--r--   0     1001      127    14475 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs
+-rw-r--r--   0     1001      127      213 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/mod.rs
+-rw-r--r--   0     1001      127      938 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs
+-rw-r--r--   0     1001      127     9907 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml
+-rw-r--r--   0     1001      127    30918 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs
+-rw-r--r--   0     1001      127      200 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/test.rs
+-rw-r--r--   0     1001      127     2790 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/locomotive/tests.rs
+-rw-r--r--   0     1001      127      752 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/mod.rs
+-rw-r--r--   0     1001      127     1039 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/consist/tests.rs
+-rw-r--r--   0     1001      127     1254 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/imports.rs
+-rw-r--r--   0     1001      127     1141 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/lib.rs
+-rw-r--r--   0     1001      127     1602 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/lin_search_hint.rs
+-rw-r--r--   0     1001      127     8028 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/macros.rs
+-rw-r--r--   0     1001      127      482 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/disp_imports.rs
+-rw-r--r--   0     1001      127     5431 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/disp_structs.rs
+-rw-r--r--   0     1001      127    11495 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/dispatch.rs
+-rw-r--r--   0     1001      127     2661 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs
+-rw-r--r--   0     1001      127    29031 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/mod.rs
+-rw-r--r--   0     1001      127     9721 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/update_times.rs
+-rw-r--r--   0     1001      127      281 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/mod.rs
+-rw-r--r--   0     1001      127    25666 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs
+-rw-r--r--   0     1001      127    36649 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/free_path.rs
+-rw-r--r--   0     1001      127     9540 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/mod.rs
+-rw-r--r--   0     1001      127     1969 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/prelude.rs
+-rw-r--r--   0     1001      127      255 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/pyo3.rs
+-rw-r--r--   0     1001      127     1039 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/si.rs
+-rw-r--r--   0     1001      127     2613 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/testing.rs
+-rw-r--r--   0     1001      127     2129 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/cat_power.rs
+-rw-r--r--   0     1001      127     4039 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/elev.rs
+-rw-r--r--   0     1001      127     4947 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/heading.rs
+-rw-r--r--   0     1001      127     4752 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/link_idx.rs
+-rw-r--r--   0     1001      127    23686 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/link_impl.rs
+-rw-r--r--   0     1001      127     1387 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/link_old.rs
+-rw-r--r--   0     1001      127     1900 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/location.rs
+-rw-r--r--   0     1001      127      246 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/locations.csv
+-rw-r--r--   0     1001      127      301 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/mod.rs
+-rw-r--r--   0     1001      127     4792 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_limit.rs
+-rw-r--r--   0     1001      127     3242 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_param.rs
+-rw-r--r--   0     1001      127     5971 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_set.rs
+-rw-r--r--   0     1001      127      120 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/link/speed.rs
+-rw-r--r--   0     1001      127      120 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/mod.rs
+-rw-r--r--   0     1001      127     6079 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/link_point.rs
+-rw-r--r--   0     1001      127      182 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/mod.rs
+-rw-r--r--   0     1001      127     2826 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/path_res_coeff.rs
+-rw-r--r--   0     1001      127    19995 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/path_tpc.rs
+-rw-r--r--   0     1001      127     7804 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/speed_point.rs
+-rw-r--r--   0     1001      127     3842 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/track/path_track/train_params.rs
+-rw-r--r--   0     1001      127     6200 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/braking_point.rs
+-rw-r--r--   0     1001      127     3503 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/friction_brakes.rs
+-rw-r--r--   0     1001      127      344 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/mod.rs
+-rw-r--r--   0     1001      127     3605 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/rail_vehicle.rs
+-rw-r--r--   0     1001      127     1124 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs
+-rw-r--r--   0     1001      127      324 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/bearing.rs
+-rw-r--r--   0     1001      127      438 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/davis_b.rs
+-rw-r--r--   0     1001      127       90 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/mod.rs
+-rw-r--r--   0     1001      127     4274 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/path_res.rs
+-rw-r--r--   0     1001      127      397 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/rolling.rs
+-rw-r--r--   0     1001      127      133 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/method/mod.rs
+-rw-r--r--   0     1001      127     2253 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/method/point.rs
+-rw-r--r--   0     1001      127     2758 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/method/strap.rs
+-rw-r--r--   0     1001      127     1780 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/resistance/mod.rs
+-rw-r--r--   0     1001      127    13755 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/set_speed_train_sim.rs
+-rw-r--r--   0     1001      127    24549 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/speed_limit_train_sim.rs
+-rw-r--r--   0     1001      127      443 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/test_rail_vehicles.csv
+-rw-r--r--   0     1001      127      182 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/timed_path.rs
+-rw-r--r--   0     1001      127    40485 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/train_config.rs
+-rw-r--r--   0     1001      127      338 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/train_imports.rs
+-rw-r--r--   0     1001      127     8339 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/train/train_state.rs
+-rw-r--r--   0     1001      127    10250 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/traits.rs
+-rw-r--r--   0     1001      127     2849 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/uc.rs
+-rw-r--r--   0     1001      127    13949 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/utils/mod.rs
+-rw-r--r--   0     1001      127     2455 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/utils/val_range.rs
+-rw-r--r--   0     1001      127     7292 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/src/validate.rs
+-rw-r--r--   0     1001      127      578 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/Cargo.toml
+-rw-r--r--   0     1001      127      707 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/README.md
+-rw-r--r--   0     1001      127    10749 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs
+-rw-r--r--   0     1001      127    12388 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/altrios_api/mod.rs
+-rw-r--r--   0     1001      127     4077 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs
+-rw-r--r--   0     1001      127     2741 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs
+-rw-r--r--   0     1001      127      367 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/imports.rs
+-rw-r--r--   0     1001      127     1192 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/lib.rs
+-rw-r--r--   0     1001      127      571 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs
+-rw-r--r--   0     1001      127     3154 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/utilities.rs
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 altrios-0.2.2/rust/altrios-py/Cargo.toml
+-rw-r--r--   0     1001      127      586 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-py/README.md
+-rw-r--r--   0     1001      127     3080 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/altrios-py/src/lib.rs
+-rw-r--r--   0     1001      127    63018 2024-05-14 17:29:53.000000 altrios-0.2.2/rust/Cargo.lock
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 altrios-0.2.2/rust/Cargo.toml
+-rw-r--r--   0     1001      127     2197 2024-05-14 17:29:53.000000 altrios-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      127      766 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/stringline_old.py
+-rw-r--r--   0     1001      127      386 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/plot.py
+-rw-r--r--   0     1001      127     5988 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/speed_limit_train_sim_demo.py
+-rw-r--r--   0     1001      127     4220 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/speed_limit_simple_corr_demo.py
+-rw-r--r--   0     1001      127     5592 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/sim_manager_demo.py
+-rw-r--r--   0     1001      127     1006 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/version_migration_demo.py
+-rw-r--r--   0     1001      127     3410 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/set_speed_simple_corr_demo.py
+-rw-r--r--   0     1001      127     3488 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/rollout_demo.py
+-rw-r--r--   0     1001      127      111 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/__init__.py
+-rw-r--r--   0     1001      127     3903 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/set_speed_train_sim_demo.py
+-rw-r--r--   0     1001      127      578 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/test_demos.py
+-rw-r--r--   0     1001      127     2357 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/conv_demo.py
+-rw-r--r--   0     1001      127     2377 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/bel_demo.py
+-rw-r--r--   0     1001      127      278 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/demos/demo_logging.py
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/py.typed
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/fuel_grid.py
+-rw-r--r--   0     1001      127    53858 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/train_planner.py
+-rw-r--r--   0     1001      127    52841 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/output_12072022.csv
+-rw-r--r--   0     1001      127     8741 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/utilities.py
+-rw-r--r--   0     1001      127    16755 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/stringline.py
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/objectives.py
+-rw-r--r--   0     1001      127     1078 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/__init__.py
+-rw-r--r--   0     1001      127    41804 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/metric_calculator.py
+-rw-r--r--   0     1001      127  1237826 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv
+-rw-r--r--   0     1001      127      994 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv
+-rw-r--r--   0     1001      127     2025 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv
+-rw-r--r--   0     1001      127     1616 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv
+-rw-r--r--   0     1001      127    10562 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv
+-rw-r--r--   0     1001      127   128287 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrain_model_input_example.csv
+-rw-r--r--   0     1001      127      695 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/Default Demand StoBar.csv
+-rw-r--r--   0     1001      127       50 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/tpc_input_example.csv
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/__init__.py
+-rw-r--r--   0     1001      127      492 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Unit_Empty.yaml
+-rw-r--r--   0     1001      127      501 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Unit.yaml
+-rw-r--r--   0     1001      127      496 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Manifest_Empty.yaml
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/__init__.py
+-rw-r--r--   0     1001      127      511 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Manifest.yaml
+-rw-r--r--   0     1001      127      641 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/rail_vehicles.csv
+-rw-r--r--   0     1001      127      492 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Intermodal.yaml
+-rw-r--r--   0     1001      127      498 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/rolling_stock/Intermodal_Empty.yaml
+-rw-r--r--   0     1001      127      568 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/trains/train_res_temp.yaml
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/trains/__init__.py
+-rw-r--r--   0     1001      127    25350 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx
+-rw-r--r--   0     1001      127     9907 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/__init__.py
+-rw-r--r--   0     1001      127      999 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/powertrains/fuel_converters/__init__.py
+-rw-r--r--   0     1001      127      191 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/README.md
+-rw-r--r--   0     1001      127       15 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/link_points_idx_simple_corridor.csv
+-rw-r--r--   0     1001      127     2279 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/speed_trace.csv
+-rw-r--r--   0     1001      127      274 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/speed_trace_simple_corridor.csv
+-rw-r--r--   0     1001      127      350 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/demo_data/link_points_idx.csv
+-rw-r--r--   0     1001      127      253 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/Default Demand.csv
+-rw-r--r--   0     1001      127    67018 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/TimedPaths.csv
+-rw-r--r--   0     1001      127  3119913 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/Taconite-NoBalloon.yaml
+-rw-r--r--   0     1001      127      390 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/default_locations.csv
+-rw-r--r--   0     1001      127     1153 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/links_test.yaml
+-rw-r--r--   0     1001      127      136 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/network_charging_guidelines.csv
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/__init__.py
+-rw-r--r--   0     1001      127  3128676 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/Taconite_v0.1.6.yaml
+-rw-r--r--   0     1001      127      548 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv
+-rw-r--r--   0     1001      127     3595 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/simple_corridor_network.yaml
+-rw-r--r--   0     1001      127      214 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/simple_corridor_locations.csv
+-rw-r--r--   0     1001      127  3192802 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/resources/networks/Taconite.yaml
+-rw-r--r--   0     1001      127     2074 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/defaults.py
+-rw-r--r--   0     1001      127     6896 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/rollout.py
+-rw-r--r--   0     1001      127     3448 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/loaders/powertrain_components.py
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/loaders/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/user_interface.py
+-rw-r--r--   0     1001      127     5693 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/sim_manager.py
+-rw-r--r--   0     1001      127      603 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_consist.py
+-rw-r--r--   0     1001      127      652 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_rail_vehicles.py
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_multi_obj_opt.py
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_fuel_grid.py
+-rw-r--r--   0     1001      127     1279 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_powertrain_fuel_conv.py
+-rw-r--r--   0     1001      127     1019 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_utilities.py
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_objectives.py
+-rw-r--r--   0     1001      127      747 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_powertrain_generator.py
+-rw-r--r--   0     1001      127     1533 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_locomotive.py
+-rw-r--r--   0     1001      127      229 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_train_planner.py
+-rw-r--r--   0     1001      127      874 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_powertrain_edrive.py
+-rw-r--r--   0     1001      127        0 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/__init__.py
+-rw-r--r--   0     1001      127      675 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_consist_sim.py
+-rw-r--r--   0     1001      127     2351 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_multi_obj_cal_and_val.py
+-rw-r--r--   0     1001      127     1754 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_powertrain_res.py
+-rw-r--r--   0     1001      127      928 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_metric_calculator.py
+-rw-r--r--   0     1001      127      386 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_train_simulation.py
+-rw-r--r--   0     1001      127     7941 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/mock_resources.py
+-rw-r--r--   0     1001      127      689 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/tests/test_locomotive_simulation.py
+-rw-r--r--   0     1001      127    29921 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/altrios_pyo3.pyi
+-rw-r--r--   0     1001      127       91 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/optimization/multi_obj_opt.py
+-rw-r--r--   0     1001      127       25 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/optimization/__init__.py
+-rw-r--r--   0     1001      127    24477 2024-05-14 17:29:53.000000 altrios-0.2.2/python/altrios/optimization/cal_and_val.py
+-rw-r--r--   0     1001      127     7492 2024-05-14 17:29:53.000000 altrios-0.2.2/README.md
+-rw-r--r--   0     1001      127     1660 2024-05-14 17:29:53.000000 altrios-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     9102 1970-01-01 00:00:00.000000 altrios-0.2.2/PKG-INFO
```

### Comparing `altrios-0.2.1/rust/altrios-core/Cargo.toml` & `altrios-0.2.2/rust/altrios-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [package]
 name = "altrios-core"
 authors = { workspace = true }
 edition = { workspace = true }
 license = { workspace = true }
 homepage = { workspace = true }
 repository = { workspace = true }
-version = "0.2.1"
+version = "0.2.2"
 description = "ALTRIOS Core model for train simulation"
 readme = "README.md"
 
 [dependencies]
 csv = "1.1.6"
 serde = { version = "1.0.136", features = ["derive"] }
 serde_yaml = "0.8.23"
 serde_json = "1.0"
 uom = { workspace = true }
 paste = "1.0.7"
 easy-ext = "1.0.0"
-altrios-proc-macros = { version = "0.2.0", path = "altrios-proc-macros" }
+altrios-proc-macros = { workspace = true }
 argmin = "0.5.1"
 rayon = "1.5.3"
 bincode = "1.3.3"
 log = "0.4.17"
 anyhow = { workspace = true }
 readonly = "0.2.3"
 duplicate = "0.4.1"
```

### Comparing `altrios-0.2.1/rust/altrios-core/README.md` & `altrios-0.2.2/rust/altrios-core/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/combo_error.rs` & `altrios-0.2.2/rust/altrios-core/src/combo_error.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/consist_model.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/consist_model.rs`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     #[getter("mass_kg")]
     fn get_mass_kg_py(&self) -> anyhow::Result<Option<f64>> {
         Ok(self.mass()?.map(|m| m.get::<si::kilogram>()))
     }
 )]
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
-/// Struct for simulating power distribution controls and energy usage of locomotive consist.  
+/// Struct for simulating power distribution controls and energy usage of locomotive consist.
 pub struct Consist {
     // pretty sure these won't get automatically generated correctly
     #[api(skip_get, skip_set)]
     /// vector of locomotives, must be private to allow for side effects when setting
     pub loco_vec: Vec<Locomotive>,
     #[api(skip_set, skip_get)]
     /// power distribution control type
@@ -119,14 +119,15 @@
     #[api(skip_get, skip_set)]
     n_res_equipped: Option<u8>,
 }
 
 impl SerdeAPI for Consist {
     fn init(&mut self) -> anyhow::Result<()> {
         self.check_mass_consistent()?;
+        self.set_pwr_dyn_brake_max();
         Ok(())
     }
 }
 
 impl Consist {
     pub fn new(
         loco_vec: Vec<Locomotive>,
@@ -282,25 +283,15 @@
         self.state.pwr_out_req = pwr_out_req;
         self.state.pwr_out_deficit =
             (pwr_out_req - self.state.pwr_out_max_reves).max(si::Power::ZERO);
         self.state.pwr_regen_deficit =
             (-pwr_out_req - self.state.pwr_regen_max).max(si::Power::ZERO);
 
         // Sum of dynamic braking capability, including regenerative capability
-        self.state.pwr_dyn_brake_max = self
-            .loco_vec
-            .iter()
-            .map(|loco| match &loco.loco_type {
-                PowertrainType::ConventionalLoco(conv) => conv.edrv.pwr_out_max,
-                PowertrainType::HybridLoco(hel) => hel.edrv.pwr_out_max,
-                PowertrainType::BatteryElectricLoco(bel) => bel.edrv.pwr_out_max,
-                // really big number that is not inf to avoid null in json
-                PowertrainType::DummyLoco(_) => uc::W * 1e15,
-            })
-            .sum();
+        self.set_pwr_dyn_brake_max();
 
         let pwr_out_vec: Vec<si::Power> = if pwr_out_req > si::Power::ZERO {
             // positive tractive power `pwr_out_vec`
             self.pdct
                 .solve_positive_traction(&self.loco_vec, &self.state)?
         } else if pwr_out_req < si::Power::ZERO {
             // negative tractive power `pwr_out_vec`
@@ -316,30 +307,31 @@
             .fold(si::Power::ZERO, |acc, &curr| acc + curr);
 
         if self.assert_limits {
             ensure!(
                 utils::almost_eq_uom(&self.state.pwr_out_req, &self.state.pwr_out, None),
                 format!(
                     "{}
-                    self.state.pwr_out_req: {:.6} MW 
+                    self.state.pwr_out_req: {:.6} MW
                     self.state.pwr_out: {:.6} MW
-                    self.state.pwr_out_deficit: {:.6} MW 
+                    self.state.pwr_out_deficit: {:.6} MW
                     pwr_out_vec: {:?}",
                     format_dbg!(),
                     &self.state.pwr_out_req.get::<si::megawatt>(),
                     &self.state.pwr_out.get::<si::megawatt>(),
                     &self.state.pwr_out_deficit.get::<si::megawatt>(),
                     &pwr_out_vec,
                 )
             );
         }
 
         // maybe put logic for toggling `engine_on` here
 
         for (i, (loco, pwr_out)) in self.loco_vec.iter_mut().zip(pwr_out_vec.iter()).enumerate() {
+            log::info!("Solving locomotive #{}", i);
             loco.solve_energy_consumption(*pwr_out, dt, engine_on)
                 .map_err(|err| {
                     err.context(format!(
                         "loco idx: {}, loco type: {}",
                         i,
                         loco.loco_type.to_string()
                     ))
@@ -374,14 +366,28 @@
         } else {
             self.state.energy_out_neg -= self.state.pwr_out * dt;
         }
         self.state.energy_fuel += self.state.pwr_fuel * dt;
         self.state.energy_res += self.state.pwr_reves * dt;
         Ok(())
     }
+
+    pub fn set_pwr_dyn_brake_max(&mut self) {
+        self.state.pwr_dyn_brake_max = self
+            .loco_vec
+            .iter()
+            .map(|loco| match &loco.loco_type {
+                PowertrainType::ConventionalLoco(conv) => conv.edrv.pwr_out_max,
+                PowertrainType::HybridLoco(hel) => hel.edrv.pwr_out_max,
+                PowertrainType::BatteryElectricLoco(bel) => bel.edrv.pwr_out_max,
+                // really big number that is not inf to avoid null in json
+                PowertrainType::DummyLoco(_) => uc::W * 1e15,
+            })
+            .sum();
+    }
 }
 
 impl Default for Consist {
     fn default() -> Self {
         let bel_type = PowertrainType::BatteryElectricLoco(BatteryElectricLoco::default());
         let mut bel = Locomotive::default();
         bel.loco_type = bel_type;
@@ -563,15 +569,15 @@
     /// [SetSpeedTrainSim](crate::train::SetSpeedTrainSim)
     pub pwr_out_req: si::Power,
     /// Current consist/train-level catenary power limit
     pub pwr_cat_lim: si::Power,
 
     // achieved values
     /// Total tractive power of consist.
-    /// Should always match [pwr_out_req](Self::pwr_out_req)] if `assert_limits == true`.  
+    /// Should always match [pwr_out_req](Self::pwr_out_req)] if `assert_limits == true`.
     pub pwr_out: si::Power,
     /// Total battery power of [RES](locomotive::powertrain::reversible_energy_storage::ReversibleEnergyStorage)-equppped locomotives
     pub pwr_reves: si::Power,
     /// Total fuel power of [FC](locomotive::powertrain::fuel_converter::FuelConverter)-equppped locomotives
     pub pwr_fuel: si::Power,
 
     /// Time-integrated energy form of [pwr_out](Self::pwr_out)
```

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/consist_sim.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/consist_sim.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 use altrios_proc_macros::altrios_api;
-use log::info;
 use serde::{Deserialize, Serialize};
 
 use crate::consist::locomotive::loco_sim::PowerTrace;
 use crate::consist::Consist;
 use crate::consist::LocoTrait;
 use crate::imports::*;
 
@@ -92,17 +91,14 @@
 
     fn save_state(&mut self) {
         self.loco_con.save_state();
     }
 
     /// Iterates step to solve all time steps.
     pub fn walk(&mut self) -> anyhow::Result<()> {
-        // Just here to showcase logging;
-        info!("Performing walk method on consist sim");
-
         self.save_state();
         while self.i < self.power_trace.len() {
             self.step()?;
         }
         Ok(())
     }
```

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/consist_utils.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/consist_utils.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/conventional_loco.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/conventional_loco.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/loco_sim.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/loco_sim.rs`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     #[pyo3(name = "trim_failed_steps")]
     fn trim_failed_steps_py(&mut self) -> anyhow::Result<()> {
         self.trim_failed_steps()?;
         Ok(())
     }
 )]
 #[derive(Clone, Debug, Deserialize, Serialize, PartialEq, SerdeAPI)]
-/// Struct for simulating operation of a standalone locomotive.  
+/// Struct for simulating operation of a standalone locomotive.
 pub struct LocomotiveSimulation {
     pub loco_unit: Locomotive,
     pub power_trace: PowerTrace,
     pub i: usize,
 }
 
 impl LocomotiveSimulation {
@@ -312,14 +312,15 @@
     /// Calls `walk` for each locomotive in vec.
     pub fn walk(&mut self, parallelize: bool) -> anyhow::Result<()> {
         if parallelize {
             self.0
                 .par_iter_mut()
                 .enumerate()
                 .try_for_each(|(i, loco_sim)| {
+                    log::info!("Solving locomotive #{i}");
                     loco_sim
                         .walk()
                         .map_err(|err| err.context(format!("loco_sim idx:{}", i)))
                 })?;
         } else {
             self.0
                 .iter_mut()
```

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/locomotive_model.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/locomotive_model.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/mod.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     /// Efficiency array corresponding to [Self::pwr_out_frac_interp] and [Self::pwr_in_frac_interp]
     pub eta_interp: Vec<f64>,
     /// Electrical input power fraction array at which efficiencies are evaluated.
     /// Calculated during runtime if not provided.
     #[serde(skip)]
     #[api(skip_set)]
     pub pwr_in_frac_interp: Vec<f64>,
-    /// ElectricDrivetrain maximum output power
+    /// ElectricDrivetrain maximum output power assuming that positive and negative tractive powers have same magnitude
     #[serde(rename = "pwr_out_max_watts")]
     pub pwr_out_max: si::Power,
     /// Time step interval between saves. 1 is a good option. If None, no saving occurs.
     pub save_interval: Option<usize>,
     /// Custom vector of [Self::state]
     #[serde(default)]
     pub history: ElectricDrivetrainStateHistoryVec,
```

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/locomotive/tests.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/locomotive/tests.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/mod.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/consist/tests.rs` & `altrios-0.2.2/rust/altrios-core/src/consist/tests.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/imports.rs` & `altrios-0.2.2/rust/altrios-core/src/imports.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/lib.rs` & `altrios-0.2.2/rust/altrios-core/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 //! Crate containing models for second-by-second fuel and energy consumption of simulation
 //! of locomotive consists comprising collections of individual locomotives, which comprise
 //! various powertrain components (engine, generator/alternator, battery, and electric drivetrain)
 //! -- all connected to a detailed train model.  
 //!
 //! # Helpful Tips
-//! Nearly struct in this crate implements methods for serializing/deserializing itself to/from a
+//! Every struct in this crate implements methods for serializing/deserializing itself to/from a
 //! handful of standard data formats as strings or file read/write operations using
 //! [traits::SerdeAPI].   
 //!
 //! # Features:
 //! - pyo3: enable this feature to expose ALTRIOS structs, methods, and functions to Python
 
 #[macro_use]
```

### Comparing `altrios-0.2.1/rust/altrios-core/src/lin_search_hint.rs` & `altrios-0.2.2/rust/altrios-core/src/lin_search_hint.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/macros.rs` & `altrios-0.2.2/rust/altrios-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/meet_pass/disp_structs.rs` & `altrios-0.2.2/rust/altrios-core/src/meet_pass/disp_structs.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/meet_pass/dispatch.rs` & `altrios-0.2.2/rust/altrios-core/src/meet_pass/dispatch.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs` & `altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/meet_pass/est_times/mod.rs` & `altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/meet_pass/est_times/update_times.rs` & `altrios-0.2.2/rust/altrios-core/src/meet_pass/est_times/update_times.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs` & `altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/meet_pass/train_disp/free_path.rs` & `altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/free_path.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/meet_pass/train_disp/mod.rs` & `altrios-0.2.2/rust/altrios-core/src/meet_pass/train_disp/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/prelude.rs` & `altrios-0.2.2/rust/altrios-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/si.rs` & `altrios-0.2.2/rust/altrios-core/src/si.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/testing.rs` & `altrios-0.2.2/rust/altrios-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/cat_power.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/cat_power.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/elev.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/elev.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/heading.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/heading.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/link_idx.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/link_idx.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/link_impl.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/link_impl.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/link_old.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/link_old.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/location.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/location.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/speed/speed_limit.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_limit.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/speed/speed_param.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_param.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/link/speed/speed_set.rs` & `altrios-0.2.2/rust/altrios-core/src/track/link/speed/speed_set.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/path_track/link_point.rs` & `altrios-0.2.2/rust/altrios-core/src/track/path_track/link_point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/path_track/path_res_coeff.rs` & `altrios-0.2.2/rust/altrios-core/src/track/path_track/path_res_coeff.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/path_track/path_tpc.rs` & `altrios-0.2.2/rust/altrios-core/src/track/path_track/path_tpc.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/path_track/speed_point.rs` & `altrios-0.2.2/rust/altrios-core/src/track/path_track/speed_point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/track/path_track/train_params.rs` & `altrios-0.2.2/rust/altrios-core/src/track/path_track/train_params.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/braking_point.rs` & `altrios-0.2.2/rust/altrios-core/src/train/braking_point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/friction_brakes.rs` & `altrios-0.2.2/rust/altrios-core/src/train/friction_brakes.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/rail_vehicle.rs` & `altrios-0.2.2/rust/altrios-core/src/train/rail_vehicle.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs` & `altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/resistance/kind/path_res.rs` & `altrios-0.2.2/rust/altrios-core/src/train/resistance/kind/path_res.rs`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,18 @@
 
         Ok(calc_res_val(res_coeff, state))
     }
     pub fn res_coeff_front(&self, vals: &[PathResCoeff]) -> si::Ratio {
         vals[self.idx_front].res_coeff
     }
 
+    pub fn res_coeff_back(&self, vals: &[PathResCoeff]) -> si::Ratio {
+        vals[self.idx_back].res_coeff
+    }
+
     pub fn res_net_front(&self, vals: &[PathResCoeff], state: &TrainState) -> si::Length {
         vals[self.idx_front].calc_res_val(state.offset)
     }
 
     /// Returns index of current element containing front of train within `PathTPC`
     pub fn path_tpc_idx_front(&self) -> usize {
         self.idx_front
```

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/resistance/method/point.rs` & `altrios-0.2.2/rust/altrios-core/src/train/resistance/method/point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/resistance/method/strap.rs` & `altrios-0.2.2/rust/altrios-core/src/train/resistance/method/strap.rs`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         state.res_bearing = self.bearing.calc_res();
         state.res_rolling = self.rolling.calc_res(state);
         state.res_davis_b = self.davis_b.calc_res(state);
         state.res_aero = self.aerodynamic.calc_res(state);
         state.res_grade = self.grade.calc_res(path_tpc.grades(), state, dir)?;
         state.res_curve = self.curve.calc_res(path_tpc.curves(), state, dir)?;
         state.grade_front = self.grade.res_coeff_front(path_tpc.grades());
+        state.grade_back = self.grade.res_coeff_front(path_tpc.grades());
         state.elev_front = self.grade.res_net_front(path_tpc.grades(), state);
         Ok(())
     }
 
     fn fix_cache(&mut self, link_point_del: &LinkPoint) {
         self.grade.fix_cache(link_point_del.grade_count);
         self.curve.fix_cache(link_point_del.curve_count);
```

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/resistance/mod.rs` & `altrios-0.2.2/rust/altrios-core/src/train/resistance/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/set_speed_train_sim.rs` & `altrios-0.2.2/rust/altrios-core/src/train/set_speed_train_sim.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/speed_limit_train_sim.rs` & `altrios-0.2.2/rust/altrios-core/src/train/speed_limit_train_sim.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/train_config.rs` & `altrios-0.2.2/rust/altrios-core/src/train/train_config.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/train/train_state.rs` & `altrios-0.2.2/rust/altrios-core/src/train/train_state.rs`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,17 @@
     pub res_davis_b: si::Force,
     pub res_aero: si::Force,
     pub res_grade: si::Force,
     pub res_curve: si::Force,
 
     /// Grade at front of train
     pub grade_front: si::Ratio,
+    /// Grade at back of train of train if strap method is used
+    // TODO: make this an option
+    pub grade_back: si::Ratio,
     /// Elevation at front of train
     pub elev_front: si::Length,
 
     /// Power to overcome train resistance forces
     pub pwr_res: si::Power,
     /// Power to overcome inertial forces
     pub pwr_accel: si::Power,
@@ -138,14 +141,15 @@
             length: Default::default(),
             mass_static: Default::default(),
             mass_adj: Default::default(),
             mass_freight: Default::default(),
             elev_front: Default::default(),
             energy_whl_out: Default::default(),
             grade_front: Default::default(),
+            grade_back: Default::default(),
             speed_target: Default::default(),
             weight_static: Default::default(),
             res_rolling: Default::default(),
             res_bearing: Default::default(),
             res_davis_b: Default::default(),
             res_aero: Default::default(),
             res_grade: Default::default(),
```

### Comparing `altrios-0.2.1/rust/altrios-core/src/traits.rs` & `altrios-0.2.2/rust/altrios-core/src/traits.rs`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,16 @@
 impl Linspace for Vec<f64> {}
 
 pub trait SerdeAPI: Serialize + for<'a> Deserialize<'a> {
     const ACCEPTED_BYTE_FORMATS: &'static [&'static str] = &["yaml", "json", "bin"];
     const ACCEPTED_STR_FORMATS: &'static [&'static str] = &["yaml", "json"];
 
     /// Specialized code to execute upon initialization
+    // TODO: make sure that init methods cascades down the hierarchy.
+    // This could be done via proc macro.
     fn init(&mut self) -> anyhow::Result<()> {
         Ok(())
     }
 
     /// Write (serialize) an object to a file.
     /// Supported file extensions are listed in [`ACCEPTED_BYTE_FORMATS`](`SerdeAPI::ACCEPTED_BYTE_FORMATS`).
     /// Creates a new file if it does not already exist, otherwise truncates the existing file.
```

### Comparing `altrios-0.2.1/rust/altrios-core/src/uc.rs` & `altrios-0.2.2/rust/altrios-core/src/uc.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/utils/mod.rs` & `altrios-0.2.2/rust/altrios-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/utils/val_range.rs` & `altrios-0.2.2/rust/altrios-core/src/utils/val_range.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/src/validate.rs` & `altrios-0.2.2/rust/altrios-core/src/validate.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/altrios-proc-macros/Cargo.toml` & `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [package]
 name = "altrios-proc-macros"
 authors = { workspace = true }
 edition = { workspace = true }
 license = { workspace = true }
 homepage = { workspace = true }
 repository = { workspace = true }
-version = "0.2.0"
+version = "0.2.2"
 description = "ALTRIOS procedural macros"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 proc-macro-error = "1.0.4"
```

### Comparing `altrios-0.2.1/rust/altrios-core/altrios-proc-macros/README.md` & `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs` & `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/altrios_api/mod.rs` & `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/altrios_api/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                             fn __setitem__(&mut self, _idx: usize, _new_value: #contained_dtype) -> anyhow::Result<()> {
                                 bail!(PyNotImplementedError::new_err(
                                     "Setting list value at index is not implemented.
                             Run `tolist` method, modify value at index, and
                             then set entire list.",
                                 ))
                             }
-                            /// PyO3-exposed method to convert vec-containing struct to Python list. 
+                            /// PyO3-exposed method to convert vec-containing struct to Python list.
                             fn tolist(&self) -> anyhow::Result<Vec<#contained_dtype>> {
                                 Ok(self.0.clone())
                             }
                             /// Rust-defined `__len__` magic method for Python used exposed via PyO3.
                             /// Returns the length of the Rust vector.
                             fn __len__(&self) -> usize {
                                 self.0.len()
@@ -158,92 +158,71 @@
         #[staticmethod]
         #[pyo3(name = "default")]
         /// Exposes `default` to python.
         fn default_py() -> anyhow::Result<Self> {
             Ok(Self::default())
         }
 
-        /// Write (serialize) an object into a string
-        ///
-        /// # Arguments:
-        ///
-        /// * `format`: `str` - The target format, any of those listed in [`ACCEPTED_STR_FORMATS`](`SerdeAPI::ACCEPTED_STR_FORMATS`)
-        ///
+        /// See [SerdeAPI::to_str]
         #[pyo3(name = "to_str")]
         pub fn to_str_py(&self, format: &str) -> anyhow::Result<String> {
             self.to_str(format)
         }
 
-        /// Read (deserialize) an object from a string
-        ///
-        /// # Arguments:
-        ///
-        /// * `contents`: `str` - The string containing the object data
-        /// * `format`: `str` - The source format, any of those listed in [`ACCEPTED_STR_FORMATS`](`SerdeAPI::ACCEPTED_STR_FORMATS`)
-        ///
+        /// See [SerdeAPI::from_str]
         #[staticmethod]
         #[pyo3(name = "from_str")]
         pub fn from_str_py(contents: &str, format: &str) -> anyhow::Result<Self> {
             Self::from_str(contents, format)
         }
 
-        /// Write (serialize) an object to a JSON string
+        /// See [SerdeAPI::to_json]
         #[pyo3(name = "to_json")]
         fn to_json_py(&self) -> anyhow::Result<String> {
             self.to_json()
         }
 
-        /// Read (deserialize) an object to a JSON string
-        ///
-        /// # Arguments
-        ///
-        /// * `json_str`: `str` - JSON-formatted string to deserialize from
-        ///
+        /// See [SerdeAPI::from_json]
         #[staticmethod]
         #[pyo3(name = "from_json")]
         fn from_json_py(json_str: &str) -> anyhow::Result<Self> {
             Self::from_json(json_str)
         }
 
-        /// Write (serialize) an object to a YAML string
+        /// See [SerdeAPI::to_yaml]
         #[pyo3(name = "to_yaml")]
         fn to_yaml_py(&self) -> anyhow::Result<String> {
             self.to_yaml()
         }
 
-        /// Read (deserialize) an object from a YAML string
-        ///
-        /// # Arguments
-        ///
-        /// * `yaml_str`: `str` - YAML-formatted string to deserialize from
-        ///
+        /// See [SerdeAPI::from_yaml]
         #[staticmethod]
         #[pyo3(name = "from_yaml")]
         fn from_yaml_py(yaml_str: &str) -> anyhow::Result<Self> {
             Self::from_yaml(yaml_str)
         }
 
-        /// Write (serialize) an object to bincode-encoded `bytes`
+        /// See [SerdeAPI::to_bincode]
         #[pyo3(name = "to_bincode")]
         fn to_bincode_py<'py>(&self, py: Python<'py>) -> anyhow::Result<&'py PyBytes> {
             Ok(PyBytes::new(py, &self.to_bincode()?))
         }
 
-        /// Read (deserialize) an object from bincode-encoded `bytes`
-        ///
-        /// # Arguments
-        ///
-        /// * `encoded`: `bytes` - Encoded bytes to deserialize from
-        ///
+        /// See [SerdeAPI::from_bincode]
         #[staticmethod]
         #[pyo3(name = "from_bincode")]
         fn from_bincode_py(encoded: &PyBytes) -> anyhow::Result<Self> {
             Self::from_bincode(encoded.as_bytes())
         }
 
+        #[pyo3(name = "init")]
+        fn init_py(&mut self) -> PyResult<()> {
+            Ok(self.init()?)
+        }
+
         /// `__copy__` magic method that uses `clone`.
         fn __copy__(&self) -> Self {
             self.clone()
         }
 
         /// `__deepcopy__` magic method that uses `clone`.
         fn __deepcopy__(&self) -> Self {
```

### Comparing `altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs` & `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs` & `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/lib.rs` & `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs` & `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-core/altrios-proc-macros/src/utilities.rs` & `altrios-0.2.2/rust/altrios-core/altrios-proc-macros/src/utilities.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-py/Cargo.toml` & `altrios-0.2.2/rust/altrios-py/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 homepage = { workspace = true }
 repository = { workspace = true }
 version = "0.1.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-altrios-core = { path = "../altrios-core", features = ["pyo3"] }
+altrios-core = { workspace = true, features = ["pyo3"] }
 pyo3 = { workspace = true, features = ["extension-module", "anyhow"] }
 pyo3-log = { workspace = true }
 polars = { workspace = true }
 polars-lazy = { workspace = true }
 pyo3-polars = { workspace = true }
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `altrios-0.2.1/rust/altrios-py/README.md` & `altrios-0.2.2/rust/altrios-py/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/altrios-py/src/lib.rs` & `altrios-0.2.2/rust/altrios-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/rust/Cargo.lock` & `altrios-0.2.2/rust/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 name = "allocator-api2"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
 
 [[package]]
 name = "altrios-core"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "altrios-proc-macros",
  "anyhow",
  "argmin",
  "bincode",
  "csv",
  "directories",
@@ -73,15 +73,15 @@
  "serde_yaml",
  "tempfile",
  "uom",
 ]
 
 [[package]]
 name = "altrios-proc-macros"
-version = "0.2.0"
+version = "0.2.2"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "regex",
  "syn 1.0.109",
  "uom",
```

### Comparing `altrios-0.2.1/rust/Cargo.toml` & `altrios-0.2.2/rust/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -34,7 +34,11 @@
 pyo3 = "0.19"
 pyo3-log = "*"
 polars = { version = "0.32" }
 polars-lazy = { version = "0.32" }
 pyo3-polars = { version = "0.6" }
 uom = { version = "0.35.0", features = ["use_serde"] }
 eng_fmt = "0.1.2"
+
+# local crates in this workspace
+altrios-core = { path = "./altrios-core" }
+altrios-proc-macros = { path = "./altrios-core/altrios-proc-macros", version = "0.2.2" }
```

### Comparing `altrios-0.2.1/pyproject.toml` & `altrios-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0"]
 build-backend = "maturin"
 
 [project]
 name = "altrios"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name = "ALTRIOS Team", email = "altrios@nrel.gov" },
     { name = "Chad Baker, Lead Developer" },
     { name = "Nick Reinicke, Developer" },
     { name = "Matt Bruchon, Developer" },
     { name = "Saad Akhtar, Developer" },
     { name = "Steven Shi, Developer" },
```

### Comparing `altrios-0.2.1/python/altrios/stringline_old.py` & `altrios-0.2.2/python/altrios/stringline_old.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/speed_limit_train_sim_demo.py` & `altrios-0.2.2/python/altrios/demos/speed_limit_train_sim_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/speed_limit_simple_corr_demo.py` & `altrios-0.2.2/python/altrios/demos/speed_limit_simple_corr_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/sim_manager_demo.py` & `altrios-0.2.2/python/altrios/demos/sim_manager_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/version_migration_demo.py` & `altrios-0.2.2/python/altrios/demos/version_migration_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/set_speed_simple_corr_demo.py` & `altrios-0.2.2/python/altrios/demos/set_speed_simple_corr_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/rollout_demo.py` & `altrios-0.2.2/python/altrios/demos/rollout_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/set_speed_train_sim_demo.py` & `altrios-0.2.2/python/altrios/demos/set_speed_train_sim_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/test_demos.py` & `altrios-0.2.2/python/altrios/demos/test_demos.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/conv_demo.py` & `altrios-0.2.2/python/altrios/demos/conv_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/demos/bel_demo.py` & `altrios-0.2.2/python/altrios/demos/bel_demo.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/train_planner.py` & `altrios-0.2.2/python/altrios/train_planner.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/output_12072022.csv` & `altrios-0.2.2/python/altrios/output_12072022.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/utilities.py` & `altrios-0.2.2/python/altrios/utilities.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/stringline.py` & `altrios-0.2.2/python/altrios/stringline.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/__init__.py` & `altrios-0.2.2/python/altrios/__init__.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/metric_calculator.py` & `altrios-0.2.2/python/altrios/metric_calculator.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv` & `altrios-0.2.2/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv` & `altrios-0.2.2/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv` & `altrios-0.2.2/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv` & `altrios-0.2.2/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv` & `altrios-0.2.2/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv` & `altrios-0.2.2/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/Default Demand StoBar.csv` & `altrios-0.2.2/python/altrios/resources/Default Demand StoBar.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/rolling_stock/rail_vehicles.csv` & `altrios-0.2.2/python/altrios/resources/rolling_stock/rail_vehicles.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/trains/train_res_temp.yaml` & `altrios-0.2.2/python/altrios/resources/trains/train_res_temp.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx` & `altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml` & `altrios-0.2.2/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml` & `altrios-0.2.2/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/demo_data/speed_trace.csv` & `altrios-0.2.2/python/altrios/resources/demo_data/speed_trace.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/TimedPaths.csv` & `altrios-0.2.2/python/altrios/resources/TimedPaths.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/networks/Taconite-NoBalloon.yaml` & `altrios-0.2.2/python/altrios/resources/networks/Taconite-NoBalloon.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/networks/links_test.yaml` & `altrios-0.2.2/python/altrios/resources/networks/links_test.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/networks/Taconite_v0.1.6.yaml` & `altrios-0.2.2/python/altrios/resources/networks/Taconite_v0.1.6.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv` & `altrios-0.2.2/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/networks/simple_corridor_network.yaml` & `altrios-0.2.2/python/altrios/resources/networks/simple_corridor_network.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/resources/networks/Taconite.yaml` & `altrios-0.2.2/python/altrios/resources/networks/Taconite.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/defaults.py` & `altrios-0.2.2/python/altrios/defaults.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/rollout.py` & `altrios-0.2.2/python/altrios/rollout.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/loaders/powertrain_components.py` & `altrios-0.2.2/python/altrios/loaders/powertrain_components.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/sim_manager.py` & `altrios-0.2.2/python/altrios/sim_manager.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_consist.py` & `altrios-0.2.2/python/altrios/tests/test_consist.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_rail_vehicles.py` & `altrios-0.2.2/python/altrios/tests/test_rail_vehicles.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_powertrain_fuel_conv.py` & `altrios-0.2.2/python/altrios/tests/test_powertrain_fuel_conv.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_utilities.py` & `altrios-0.2.2/python/altrios/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_powertrain_generator.py` & `altrios-0.2.2/python/altrios/tests/test_powertrain_generator.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_locomotive.py` & `altrios-0.2.2/python/altrios/tests/test_locomotive.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_powertrain_edrive.py` & `altrios-0.2.2/python/altrios/tests/test_powertrain_edrive.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_consist_sim.py` & `altrios-0.2.2/python/altrios/tests/test_consist_sim.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_multi_obj_cal_and_val.py` & `altrios-0.2.2/python/altrios/tests/test_multi_obj_cal_and_val.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_powertrain_res.py` & `altrios-0.2.2/python/altrios/tests/test_powertrain_res.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_metric_calculator.py` & `altrios-0.2.2/python/altrios/tests/test_metric_calculator.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/mock_resources.py` & `altrios-0.2.2/python/altrios/tests/mock_resources.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/tests/test_locomotive_simulation.py` & `altrios-0.2.2/python/altrios/tests/test_locomotive_simulation.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/altrios_pyo3.pyi` & `altrios-0.2.2/python/altrios/altrios_pyo3.pyi`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/python/altrios/optimization/cal_and_val.py` & `altrios-0.2.2/python/altrios/optimization/cal_and_val.py`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/README.md` & `altrios-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/LICENSE.md` & `altrios-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `altrios-0.2.1/PKG-INFO` & `altrios-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: altrios
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: pandas >=2
 Requires-Dist: numpy
```

