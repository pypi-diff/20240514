# Comparing `tmp/methodicconfigurator-0.4.2.tar.gz` & `tmp/methodicconfigurator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodicconfigurator-0.4.2.tar", last modified: Mon May 13 17:13:34 2024, max compression
+gzip compressed data, was "methodicconfigurator-0.5.1.tar", last modified: Tue May 14 08:38:36 2024, max compression
```

## Comparing `methodicconfigurator-0.4.2.tar` & `methodicconfigurator-0.5.1.tar`

### file list

```diff
@@ -1,255 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.008244 methodicconfigurator-0.4.2/MethodicConfigurator/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/ArduPilot_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/ArduPilot_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27848 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/annotate_params.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5416 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/ardupilot_methodic_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29018 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem_configuration_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem_vehicle_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    30985 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_flightcontroller.py
--rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/backend_mavftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/battery_cell_voltages.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/common_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/extract_param_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18042 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_component_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_component_editor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14623 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_connection_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20073 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_directory_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    37030 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_parameter_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    23945 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/get_release_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/param_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/param_pid_adjustment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/tempcal_imu.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/MethodicConfigurator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20244 2024-05-13 17:13:34.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 17:13:33.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:13:26.000000 methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.004244 methodicconfigurator-0.4.2/vehicle_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.004244 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.004244 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.024244 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    20925 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)    15574 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)    34562 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1476098 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.036244 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    21593 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1599965 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.052245 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    21636 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    14081 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1966610 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:13:34.064245 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1982447 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-13 17:13:04.000000 methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.963529 methodicconfigurator-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.915530 methodicconfigurator-0.5.1/MethodicConfigurator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/ArduPilot_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/ArduPilot_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27851 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/annotate_params.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5426 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/ardupilot_methodic_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29018 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/backend_filesystem_configuration_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/backend_filesystem_vehicle_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31001 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/backend_flightcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/backend_mavftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/battery_cell_voltages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/common_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/extract_param_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18042 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_component_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_component_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_connection_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20073 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_directory_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37123 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_parameter_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26960 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/get_release_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/param_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/param_pid_adjustment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/tempcal_imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/MethodicConfigurator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.963529 methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-14 08:38:36.000000 methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20317 2024-05-14 08:38:36.000000 methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:38:36.000000 methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 08:38:36.000000 methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 08:38:36.000000 methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 08:38:36.000000 methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:38:29.000000 methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-14 08:38:36.963529 methodicconfigurator-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:38:36.963529 methodicconfigurator-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.911530 methodicconfigurator-0.5.1/vehicle_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.911530 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.911530 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.927530 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    20075 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1476098 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.939530 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1599965 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.951530 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    21636 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    14081 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1966610 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:38:36.963529 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1982447 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-14 08:38:08.000000 methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
```

### Comparing `methodicconfigurator-0.4.2/LICENSE.md` & `methodicconfigurator-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/ArduPilot_icon.png` & `methodicconfigurator-0.5.1/MethodicConfigurator/ArduPilot_icon.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/ArduPilot_logo.png` & `methodicconfigurator-0.5.1/MethodicConfigurator/ArduPilot_logo.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/annotate_params.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/annotate_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,16 +235,16 @@
                     output_file.write(line + "\n")
         except IOError as e:
             raise SystemExit(f"ERROR: writing to file {filename_out}: {e}") from e
 
     @staticmethod
     def print_out(formatted_params: List[str], name: str) -> None:
         """
-        Prints out the contents of the provided list.
-        If the list is too large, print only the ones that fit on screen and
+        Print out the contents of the provided list.
+        If the list is too large, print only the ones that fit on the screen and
         wait for user input to continue.
 
         Parameters:
         formatted_params (List[str]): The list of formatted parameters to print.
         name (str): A descriptive string for the list contents
 
         Returns:
```

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/ardupilot_methodic_configurator.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/ardupilot_methodic_configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     Returns:
     argparse.Namespace: An object containing the parsed arguments.
     """
     parser = argparse.ArgumentParser(description='ArduPilot methodic configurator is a simple GUI with a table that lists '
                                      'parameters. The GUI reads intermediate parameter files from a directory and '
                                      'displays their parameters in a table. Each row displays the parameter name, '
                                      'its current value on the flight controller, its new value from the selected '
-                                     'intermediate parameter file, and an "write" checkbox. The GUI includes "Write '
-                                     'Selected to FC" and "Skip" buttons at the bottom. '
-                                     'When "Write Selected to FC" is clicked, it writes the selected parameters to the '
+                                     'intermediate parameter file, and an "Upload" checkbox. The GUI includes "Upload '
+                                     'selected params to FC" and "Skip" buttons at the bottom. '
+                                     'When "Upload Selected to FC" is clicked, it writes the selected parameters to the '
                                      'flight controller. '
                                      'When "Skip" is pressed, it skips to the next intermediate parameter file. '
                                      'The process gets repeated for each intermediate parameter file.')
     parser = FlightController.add_argparse_arguments(parser)
     parser = LocalFilesystem.add_argparse_arguments(parser)
     parser = ComponentEditorWindow.add_argparse_arguments(parser)
     parser.add_argument('--loglevel',
```

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/backend_filesystem.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem_configuration_steps.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/backend_filesystem_configuration_steps.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/backend_filesystem_vehicle_components.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/backend_filesystem_vehicle_components.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/backend_flightcontroller.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/backend_flightcontroller.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
             # logging_info(f"Flight Controller UID if provided by hardware: {m.uid}")
         except (ConnectionError, SerialException, PermissionError, ConnectionRefusedError) as e:
             logging_warning("Connection failed: %s", e)
             logging_error("Failed to connect after %d attempts.", retries)
             return str(e)
         return ""
 
-    def read_params(self, progress_callback=None) -> Dict[str, float]:
+    def download_params(self, progress_callback=None) -> Dict[str, float]:
         """
         Requests all flight controller parameters from a MAVLink connection.
 
         Returns:
             Dict[str, float]: A dictionary of flight controller parameters.
         """
         # FIXME this entire if statement is for testing only, remove it later pylint: disable=fixme
@@ -320,22 +320,22 @@
             return None
 
         # Check if MAVFTP is supported
         # FIXME remove the "not" once it works pylint: disable=fixme
         if self.__capabilities:
             if not (self.__capabilities & mavutil.mavlink.MAV_PROTOCOL_CAPABILITY_FTP):  # pylint: disable=superfluous-parens
                 logging_info("MAVFTP is supported by the %s flight controller", self.comport.device)
-                # parameters, _defaults = self.read_params_via_mavftp(progress_callback)
+                # parameters, _defaults = self.download_params_via_mavftp(progress_callback)
                 return {}  # parameters
 
         logging_info("MAVFTP is not supported by the %s flight controller, fallback to MAVLink", self.comport.device)
         # MAVFTP is not supported, fall back to MAVLink
-        return self.__read_params_via_mavlink(progress_callback)
+        return self.__download_params_via_mavlink(progress_callback)
 
-    def __read_params_via_mavlink(self, progress_callback=None) -> Dict[str, float]:
+    def __download_params_via_mavlink(self, progress_callback=None) -> Dict[str, float]:
         logging_debug("Will fetch all parameters from the %s flight controller", self.comport.device)
         # Request all parameters
         self.master.mav.param_request_list_send(
             self.master.target_system, self.master.target_component
         )
 
         # Dictionary to store parameters
```

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/backend_mavftp.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/backend_mavftp.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/battery_cell_voltages.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/battery_cell_voltages.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/common_arguments.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/common_arguments.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/extract_param_defaults.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/extract_param_defaults.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_base.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_base.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_component_editor.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_component_editor.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_component_editor_base.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_component_editor_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,24 +65,30 @@
         if len(self.data) < 1:
             # Schedule the window to be destroyed after the mainloop has started
             self.root.after(100, self.root.destroy) # Adjust the delay as needed
             return
 
         self.entry_widgets = {} # Dictionary for entry widgets
 
-        self.main_frame = ttk.Frame(self.root)
-        self.main_frame.pack(side=tk.TOP, fill="x", expand=False, pady=(4, 0)) # Pack the frame at the top of the window
+        main_frame = ttk.Frame(self.root)
+        main_frame.pack(side=tk.TOP, fill="x", expand=False, pady=(4, 0)) # Pack the frame at the top of the window
+
+        explanation_text = "Please configure ALL vehicle component properties in this window.\n"
+        explanation_text += "Scroll down and make sure you do not miss a property.\n"
+        explanation_text += "Saving the result will write to the vehicle_components.json file."
+        explanation_label = tk.Label(main_frame, text=explanation_text, wraplength=800, justify=tk.LEFT)
+        explanation_label.pack(side=tk.LEFT, padx=(10, 10), pady=(10, 0), anchor=tk.NW)
 
         # Load the vehicle image and scale it down to image_height pixels in height
         if local_filesystem.vehicle_image_exists():
-            image_label = self.put_image_in_label(self.main_frame, local_filesystem.vehicle_image_filepath(), 100)
+            image_label = self.put_image_in_label(main_frame, local_filesystem.vehicle_image_filepath(), 100)
             image_label.pack(side=tk.RIGHT, anchor=tk.NE, padx=(4, 4), pady=(4, 0))
             show_tooltip(image_label, "Replace the vehicle.jpg file in the vehicle directory to change the vehicle image.")
         else:
-            image_label = tk.Label(self.main_frame, text="No vehicle.jpg image file found on the vehicle directory.")
+            image_label = tk.Label(main_frame, text="No vehicle.jpg image file found on the vehicle directory.")
             image_label.pack(side=tk.RIGHT, anchor=tk.NE, padx=(4, 4), pady=(4, 0))
 
         self.scroll_frame = ScrollFrame(self.root)
         self.scroll_frame.pack(side="top", fill="both", expand=True)
 
         self.__populate_frames()
```

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_connection_selection.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_connection_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from MethodicConfigurator.frontend_tkinter_base import BaseWindow
 
 
 # https://dev.to/geraldew/python-tkinter-an-exercise-in-wrapping-the-combobox-ndb
 class PairTupleCombobox(ttk.Combobox):  # pylint: disable=too-many-ancestors
     """
     A custom Combobox widget that allows for the display of a list of tuples, where each tuple contains a key and a value.
-    This widget processes the list of tuples to separate keys and values for display purposes, and allows for the selection
+    This widget processes the list of tuples to separate keys and values for display purposes and allows for the selection
     of a tuple based on its key.
     """
     def process_list_pair_tuple(self, list_pair_tuple):
         r_list_keys = []
         r_list_shows = []
         for tpl in list_pair_tuple:
             r_list_keys.append(tpl[0])
@@ -85,19 +85,19 @@
     """
     A class for managing the selection of flight controller connections in the GUI.
 
     This class provides functionality for displaying available flight controller connections,
     allowing the user to select a connection, and handling the connection process.
     """
     def __init__(self, parent, parent_frame, flight_controller: FlightController,  # pylint: disable=too-many-arguments
-                 destroy_parent_on_connect: bool, read_params_on_connect: bool):
+                 destroy_parent_on_connect: bool, download_params_on_connect: bool):
         self.parent = parent
         self.flight_controller = flight_controller
         self.destroy_parent_on_connect = destroy_parent_on_connect
-        self.read_params_on_connect = read_params_on_connect
+        self.download_params_on_connect = download_params_on_connect
         self.previous_selection = flight_controller.comport.device if hasattr(self.flight_controller.comport, "device") \
             else None
         self.connection_progress_window = None
 
         # Create a new frame for the flight controller connection selection label and combobox
         self.container_frame = tk.Frame(parent_frame)
 
@@ -154,67 +154,67 @@
             show_no_connection_error(error_message)
             return True
         self.connection_progress_window.destroy()
         # Store the current connection as the previous selection
         self.previous_selection = self.flight_controller.comport.device
         if self.destroy_parent_on_connect:
             self.parent.root.destroy()
-        if self.read_params_on_connect and hasattr(self.parent, "read_flight_controller_parameters"):
-            self.parent.read_flight_controller_parameters(reread=False)
+        if self.download_params_on_connect and hasattr(self.parent, "download_flight_controller_parameters"):
+            self.parent.download_flight_controller_parameters(redownload=False)
         return False
 
 
 class ConnectionSelectionWindow(BaseWindow):
     """
     A window for selecting a flight controller connection.
 
     This class provides a graphical user interface for selecting a connection to a flight controller.
     It inherits from the BaseWindow class and uses the ConnectionSelectionWidgets class to handle
     the UI elements related to connection selection.
     """
     def __init__(self, flight_controller: FlightController, connection_result_string: str):
         super().__init__()
         self.root.title("Flight controller connection")
-        self.root.geometry("400x510") # Set the window size
+        self.root.geometry("420x510") # Set the window size
 
         # Explain why we are here
         if flight_controller.comport is None:
             introduction_text = "No ArduPilot flight controller was auto-detected detected yet."
         else:
             if ":" in connection_result_string:
                 introduction_text = connection_result_string.replace(":", ":\n")
             else:
                 introduction_text = connection_result_string
         self.introduction_label = tk.Label(self.root, text=introduction_text + "\nChoose one of the following three options:")
         self.introduction_label.pack(expand=False, fill=tk.X, padx=6, pady=6)
 
         # Option 1 - Auto-connect
-        option1_label_frame = tk.LabelFrame(self.root, text="Option 1")
+        option1_label_frame = tk.LabelFrame(self.root, text="Auto-connect to flight controller")
         option1_label_frame.pack(expand=False, fill=tk.X, padx=6, pady=6)
         option1_label = tk.Label(option1_label_frame, text="Connect a flight controller to the PC,\n"
                                  "wait 7 seconds for it to fully boot and\n"
                                  "press the Auto-connect button below to connect to it")
         option1_label.pack(expand=False, fill=tk.X, padx=6)
         autoconnect_button = tk.Button(option1_label_frame, text="Auto-connect", command=self.fc_autoconnect)
         autoconnect_button.pack(expand=False, fill=tk.X, padx=100, pady=6)
 
         # Option 2 - Manually select the flight controller connection or add a new one
-        option2_label_frame = tk.LabelFrame(self.root, text="Option 2")
+        option2_label_frame = tk.LabelFrame(self.root, text="Select flight controller connection")
         option2_label_frame.pack(expand=False, fill=tk.X, padx=6, pady=6)
         option2_label = tk.Label(option2_label_frame, text="Connect a flight controller to the PC,\n"
                                  "wait 7 seconds for it to fully boot and\n"
                                  "manually select the fight controller connection or add a new one")
         option2_label.pack(expand=False, fill=tk.X, padx=6)
         self.connection_selection_widgets = ConnectionSelectionWidgets(self, option2_label_frame, flight_controller,
                                                                        destroy_parent_on_connect=True,
-                                                                       read_params_on_connect=False)
+                                                                       download_params_on_connect=False)
         self.connection_selection_widgets.container_frame.pack(expand=True, fill=tk.X, padx=80, pady=6, anchor=tk.CENTER)
 
         # Option 3 - Skip FC connection, just edit the .param files on disk
-        option3_label_frame = tk.LabelFrame(self.root, text="Option 3")
+        option3_label_frame = tk.LabelFrame(self.root, text="No flight controller connection")
         option3_label_frame.pack(expand=False, fill=tk.X, padx=6, pady=6)
         option3_label = tk.Label(option3_label_frame, text="Skip the flight controller connection,\n"
                                  "no default parameter values will be fetched from the FC,\n"
                                  "default parameter values from disk will be used instead\n"
                                  "(if '00_default.param' file is present)\n"
                                  "and just edit the intermediate '.param' files on disk")
         option3_label.pack(expand=False, fill=tk.X, padx=6)
```

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_directory_selection.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_directory_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     configuration directory based on an existing template or using an existing
     vehicle configuration directory.
     """
     def __init__(self, local_filesystem: LocalFilesystem):
         super().__init__()
         self.local_filesystem = local_filesystem
         self.root.title("Select Vehicle directory")
-        self.root.geometry("400x535") # Set the window size
+        self.root.geometry("800x535") # Set the window size
 
         # Explain why we are here
         if local_filesystem.vehicle_dir == LocalFilesystem.getcwd():
             introduction_text = "No intermediate parameter files found\nin current working directory."
         else:
             introduction_text = "No intermediate parameter files found\nin the --vehicle-dir specified directory."
         introduction_label = tk.Label(self.root, text=introduction_text + \
```

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_parameter_editor.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_parameter_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
         self.at_least_one_changed_parameter_written = False
         self.file_selection_combobox = None
         self.show_only_differences = None
         self.annotate_params_into_files = None
         self.parameter_editor_table = None
         self.reset_progress_window = None
-        self.param_read_progress_window = None
+        self.param_download_progress_window = None
         self.tempcal_imu_progress_window = None
 
         self.root.title("Amilcar Lucas's - ArduPilot methodic configurator - " + version + " - Parameter editor")
         self.root.geometry("880x500") # Set the window width
 
         # Bind the close_connection_and_quit function to the window close event
         self.root.protocol("WM_DELETE_WINDOW", self.close_connection_and_quit)
@@ -190,15 +190,15 @@
         self.__create_conf_widgets(version)
 
         # Create a DocumentationFrame object for the Documentation Content
         self.documentation_frame = DocumentationFrame(self.root, self.local_filesystem, self.current_file)
 
         self.__create_parameter_area_widgets()
 
-        self.root.after(50, self.read_flight_controller_parameters(reread=False)) # 50 milliseconds
+        self.root.after(50, self.download_flight_controller_parameters(redownload=False)) # 50 milliseconds
         self.root.after(50, self.__please_read_the_docs())
         self.root.mainloop()
 
     def __create_conf_widgets(self, version: str):
         config_frame = tk.Frame(self.root)
         config_frame.pack(side=tk.TOP, fill="x", expand=False, pady=(4, 0)) # Pack the frame at the top of the window
 
@@ -230,28 +230,28 @@
                                                           "fight controller",
                                                           state='readonly', width=45)
         self.file_selection_combobox.bind("<<ComboboxSelected>>", self.on_param_file_combobox_change)
         self.file_selection_combobox.pack(side=tk.TOP, anchor=tk.NW, pady=(4, 0))
 
         # Create a new frame inside the config_subframe for the flight controller connection selection label and combobox
         csw = ConnectionSelectionWidgets(self, config_subframe, self.flight_controller,
-                                         destroy_parent_on_connect=False, read_params_on_connect=True)
+                                         destroy_parent_on_connect=False, download_params_on_connect=True)
         csw.container_frame.pack(side=tk.RIGHT, fill="x", expand=False, padx=(6, 4))
 
         image_label = BaseWindow.put_image_in_label(config_frame, LocalFilesystem.application_logo_filepath())
         image_label.pack(side=tk.RIGHT, anchor=tk.NE, padx=(4, 4), pady=(4, 0))
         image_label.bind("<Button-1>", lambda event: show_about_window(self.root, version))
         show_tooltip(image_label, "User Manual, Support Forum, Report a Bug, Credits, Source Code")
 
     def __create_parameter_area_widgets(self):
         self.show_only_differences = tk.BooleanVar(value=False)
         self.annotate_params_into_files = tk.BooleanVar(value=False)
 
         # Create a Scrollable parameter editor table
-        self.parameter_editor_table = ParameterEditorTable(self.root, self.local_filesystem)
+        self.parameter_editor_table = ParameterEditorTable(self.root, self.local_filesystem, self)
         self.repopulate_parameter_table(self.current_file)
         self.parameter_editor_table.pack(side="top", fill="both", expand=True)
 
         # Create a frame for the buttons
         buttons_frame = tk.Frame(self.root)
         buttons_frame.pack(side="bottom", fill="x", expand=False, pady=(10, 10))
 
@@ -272,25 +272,25 @@
                                                    variable=self.annotate_params_into_files)
         annotate_params_checkbox.pack(side=tk.TOP, anchor=tk.NW)
         show_tooltip(annotate_params_checkbox, "Annotate ArduPilot parameter documentation metadata into the intermediate "
                      "parameter files\n"
                      "The files will be bigger, but all the existing parameter documentation will be included inside")
 
         # Create write button
-        write_selected_button = tk.Button(buttons_frame, text="Write selected params to FC, and advance to next param file",
-                                          command=self.on_write_selected_click)
+        write_selected_button = tk.Button(buttons_frame, text="Upload selected params to FC, and advance to next param file",
+                                          command=self.on_upload_selected_click)
         write_selected_button.pack(side=tk.LEFT, padx=(8, 8)) # Add padding on both sides of the write selected button
-        show_tooltip(write_selected_button, "Write selected parameters to the flight controller and advance to the next "
+        show_tooltip(write_selected_button, "Upload selected parameters to the flight controller and advance to the next "
                      "intermediate parameter file\nIf changes have been made to the current file it will ask if you want "
-                     "to save them\nIt will reset the FC if necessary, re-read all parameters and validate their value")
+                     "to save them\nIt will reset the FC if necessary, re-download all parameters and validate their value")
 
         # Create skip button
         skip_button = tk.Button(buttons_frame, text="Skip parameter file", command=self.on_skip_click)
         skip_button.pack(side=tk.RIGHT, padx=(8, 8)) # Add right padding to the skip button
-        show_tooltip(skip_button, "Skip to the next intermediate parameter file without writing any changes to the flight "
+        show_tooltip(skip_button, "Skip to the next intermediate parameter file without uploading any changes to the flight "
                      "controller\nIf changes have been made to the current file it will ask if you want to save them")
 
     @staticmethod
     def __please_read_the_docs():
         messagebox.showinfo("Welcome to the ArduPilot Methodic Configurator",
                             "Please read ALL the documentation on top of the parameter table"
                             " before editing the parameters and the reason they changed")
@@ -344,22 +344,22 @@
 
             # Update the current_file attribute to the selected file
             self.current_file = selected_file
             self.at_least_one_changed_parameter_written = False
             self.documentation_frame.update_documentation_labels(selected_file)
             self.repopulate_parameter_table(selected_file)
 
-    def read_flight_controller_parameters(self, reread: bool = False):
-        self.param_read_progress_window = ProgressWindow(self.root, ("Re-r" if reread else "R") + "eading FC parameters",
-                                                         "Read {} of {} parameters")
+    def download_flight_controller_parameters(self, redownload: bool = False):
+        self.param_download_progress_window = ProgressWindow(self.root, ("Re-d" if redownload else "D") + \
+                                                             "ownloading FC parameters", "Downloaded {} of {} parameters")
         # Download all parameters from the flight controller
-        self.flight_controller.fc_parameters = self.flight_controller.read_params(
-            self.param_read_progress_window.update_progress_bar)
-        self.param_read_progress_window.destroy()  # for the case that we are doing a test and there is no real FC connected
-        if not reread:
+        self.flight_controller.fc_parameters = self.flight_controller.download_params(
+            self.param_download_progress_window.update_progress_bar)
+        self.param_download_progress_window.destroy()  # for the case that '--device test' and there is no real FC connected
+        if not redownload:
             self.on_param_file_combobox_change(None, True) # the initial param read will trigger a table update
 
     def repopulate_parameter_table(self, selected_file):
         if not selected_file:
             return  # no file was yet selected, so skip it
         if hasattr(self.flight_controller, 'fc_parameters') and self.flight_controller.fc_parameters:
             fc_parameters = self.flight_controller.fc_parameters
@@ -379,15 +379,15 @@
         # Re-populate the table with the new parameters
         self.parameter_editor_table.repopulate(selected_file, different_params,
                                                fc_parameters, self.show_only_differences.get())
 
     def on_show_only_changed_checkbox_change(self):
         self.repopulate_parameter_table(self.current_file)
 
-    def write_params_that_require_reset(self, selected_params: dict):
+    def upload_params_that_require_reset(self, selected_params: dict):
         """
         Write the selected parameters to the flight controller that require a reset.
 
         After the reset, the other parameters that do not require a reset must still be written to the flight controller.
         """
         fc_reset_required = False
         fc_reset_unsure = []
@@ -431,53 +431,53 @@
         if fc_reset_required:
             self.reset_progress_window = ProgressWindow(self.root, "Resetting Flight Controller",
                                                         "Waiting for {} of {} seconds")
             # Call reset_and_reconnect with a callback to update the reset progress bar and the progress message
             self.flight_controller.reset_and_reconnect(self.reset_progress_window.update_progress_bar)
             self.reset_progress_window.destroy()  # for the case that we are doing a test and there is no real FC connected
 
-    def on_write_selected_click(self):
+    def on_upload_selected_click(self):
         self.parameter_editor_table.generate_edit_widgets_focus_out()
 
         self.write_changes_to_intermediate_parameter_file()
         selected_params = self.parameter_editor_table.get_write_selected_params(self.current_file)
         if selected_params:
             if hasattr(self.flight_controller, 'fc_parameters') and self.flight_controller.fc_parameters:
-                self.write_selected_params(selected_params)
+                self.upload_selected_params(selected_params)
             else:
                 logging_warning("No parameters were yet read from the flight controller, will not write any parameter")
                 messagebox.showwarning("Will not write any parameter", "No flight controller connection")
         else:
             logging_warning("No parameter was selected for write, will not write any parameter")
             messagebox.showwarning("Will not write any parameter", "No parameter was selected for write")
         # Delete the parameter table and create a new one with the next file if available
         self.on_skip_click(force_focus_out_event=False)
 
-    # This function can recurse multiple time if there is a write error
-    def write_selected_params(self, selected_params):
-        logging_info("Writing %d selected %s parameters to flight controller...", len(selected_params), self.current_file)
+    # This function can recurse multiple times if there is a write error
+    def upload_selected_params(self, selected_params):
+        logging_info("Uploading %d selected %s parameters to flight controller...", len(selected_params), self.current_file)
 
-        self.write_params_that_require_reset(selected_params)
+        self.upload_params_that_require_reset(selected_params)
 
         # Write each selected parameter to the flight controller
         for param_name, param in selected_params.items():
             try:
                 self.flight_controller.set_param(param_name, param.value)
                 logging_info("Parameter %s set to %f", param_name, param.value)
                 if param_name not in self.flight_controller.fc_parameters or \
                    not is_within_tolerance(self.flight_controller.fc_parameters[param_name], param.value):
                     self.at_least_one_changed_parameter_written = True
             except ValueError as e:
                 logging_error("Failed to set parameter %s: %s", param_name, e)
                 messagebox.showerror("ArduPilot methodic configurator", f"Failed to set parameter {param_name}: {e}")
 
         if self.at_least_one_changed_parameter_written:
-            # Re-download all parameters, in case one of them changed, and validate that all writes were successful
-            self.read_flight_controller_parameters(True)
-            logging_info("Re-read all parameters from the flight controller")
+            # Re-download all parameters, in case one of them changed, and validate that all uploads were successful
+            self.download_flight_controller_parameters(True)
+            logging_info("Re-download all parameters from the flight controller")
 
             # Validate that the read parameters are the same as the ones in the current_file
             param_write_error = []
             for param_name, param in selected_params.items():
                 if param_name in self.flight_controller.fc_parameters and \
                    param is not None and \
                    not is_within_tolerance(self.flight_controller.fc_parameters[param_name], float(param.value)):
@@ -489,15 +489,15 @@
                                   param_name, param.value)
                     param_write_error.append(param_name)
 
             if param_write_error:
                 if messagebox.askretrycancel("Parameter write error",
                                              "Failed to write the following parameters to the flight controller:\n"
                                              f"{(', ').join(param_write_error)}"):
-                    self.write_selected_params(selected_params)
+                    self.upload_selected_params(selected_params)
             else:
                 logging_info("All parameters written to the flight controller successfully")
         self.local_filesystem.write_last_written_filename(self.current_file)
 
     def on_skip_click(self, _event=None, force_focus_out_event=True):
         if force_focus_out_event:
             self.parameter_editor_table.generate_edit_widgets_focus_out()
```

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 '''
 
 from sys import exit as sys_exit
 
 import tkinter as tk
 from tkinter import messagebox
 from tkinter import ttk
+from tkinter import simpledialog
 
 from logging import debug as logging_debug
 from logging import info as logging_info
 #from logging import warning as logging_warning
 #from logging import error as logging_error
 from logging import critical as logging_critical
 
@@ -25,27 +26,29 @@
 
 #from MethodicConfigurator.backend_flightcontroller import FlightController
 
 from MethodicConfigurator.frontend_tkinter_base import show_tooltip
 #from MethodicConfigurator.frontend_tkinter_base import AutoResizeCombobox
 from MethodicConfigurator.frontend_tkinter_base import ScrollFrame
 
+from MethodicConfigurator.annotate_params import Par
 
 
-class ParameterEditorTable(ScrollFrame):  # pylint: disable=too-many-ancestors
+class ParameterEditorTable(ScrollFrame):  # pylint: disable=too-many-ancestors, too-many-instance-attributes
     """
     A class to manage and display the parameter editor table within the GUI.
 
     This class inherits from ScrollFrame and is responsible for creating,
     managing, and updating the table that displays parameters for editing.
     """
-    def __init__(self, root, local_filesystem):
+    def __init__(self, root, local_filesystem, parameter_editor):
         super().__init__(root)
         self.root = root
         self.local_filesystem = local_filesystem
+        self.parameter_editor = parameter_editor
         self.background_color = root.cget("background")
         self.current_file = None
         self.write_checkbutton_var = {}
         self.at_least_one_param_edited = False
 
         # Prepare a dictionary that maps variable names to their values
         # These variables are used by the forced_parameters and derived_parameters in *_configuration_steps.json files
@@ -70,20 +73,21 @@
 
     def repopulate(self, selected_file: str, different_params: dict, fc_parameters: dict, show_only_differences: bool):
         for widget in self.view_port.winfo_children():
             widget.destroy()
         self.current_file = selected_file
 
         # Create labels for table headers
-        headers = ["Parameter", "Current Value", "New Value", "Unit", "Write", "Change Reason"]
-        tooltips = ["Parameter name must be ^[A-Z][A-Z_0-9]* and most 16 characters long",
+        headers = ["-/+", "Parameter", "Current Value", "New Value", "Unit", "Upload", "Change Reason"]
+        tooltips = ["Delete or add a parameter",
+                    "Parameter name must be ^[A-Z][A-Z_0-9]* and most 16 characters long",
                     "Current value on the flight controller ",
                     "New value from the above selected intermediate parameter file",
                     "Parameter Unit",
-                    "When selected, write the new value to the flight controller",
+                    "When selected, upload the new value to the flight controller",
                     "Reason why respective parameter changed"]
         for i, header in enumerate(headers):
             label = tk.Label(self.view_port, text=header)
             label.grid(row=0, column=i, sticky="ew") # Use sticky="ew" to make the label stretch horizontally
             show_tooltip(label, tooltips[i])
 
         self.write_checkbutton_var = {}
@@ -131,40 +135,52 @@
         try:
             for i, (param_name, param) in enumerate(params.items(), 1):
                 param_metadata = self.local_filesystem.doc_dict.get(param_name, None)
                 param_default = self.local_filesystem.param_default_dict.get(param_name, None)
                 doc_tooltip = param_metadata.get('doc_tooltip') if param_metadata else \
                     "No documentation available in apm.pdef.xml for this parameter"
 
-                column_0 = self.__create_parameter_name(param_name, param_metadata, doc_tooltip)
-                column_1 = self.__create_flightcontroller_value(fc_parameters, param_name, param_default, doc_tooltip)
-                column_2 = self.__create_new_value_entry(param_name, param, param_metadata,
+                column_0 = self.__create_delete_button(param_name)
+                column_1 = self.__create_parameter_name(param_name, param_metadata, doc_tooltip)
+                column_2 = self.__create_flightcontroller_value(fc_parameters, param_name, param_default, doc_tooltip)
+                column_3 = self.__create_new_value_entry(param_name, param, param_metadata,
                                                          param_default, doc_tooltip)
-                column_3 = self.__create_unit_label(param_metadata)
-                column_4 = self.__create_write_write_checkbutton(param_name)
-                column_5 = self.__create_change_reason_entry(param_name, param, column_2)
+                column_4 = self.__create_unit_label(param_metadata)
+                column_5 = self.__create_write_write_checkbutton(param_name)
+                column_6 = self.__create_change_reason_entry(param_name, param, column_3)
 
                 column_0.grid(row=i, column=0, sticky="w", padx=0)
-                column_1.grid(row=i, column=1, sticky="e", padx=0)
+                column_1.grid(row=i, column=1, sticky="w", padx=0)
                 column_2.grid(row=i, column=2, sticky="e", padx=0)
                 column_3.grid(row=i, column=3, sticky="e", padx=0)
                 column_4.grid(row=i, column=4, sticky="e", padx=0)
-                column_5.grid(row=i, column=5, sticky="ew", padx=(0, 5))
+                column_5.grid(row=i, column=5, sticky="e", padx=0)
+                column_6.grid(row=i, column=6, sticky="ew", padx=(0, 5))
+
+            # Add the "Add" button at the bottom of the table
+            add_button = tk.Button(self.view_port, text="Add", command=lambda: self.__on_parameter_add(fc_parameters))
+            add_button.grid(row=len(params)+2, column=0, sticky="w", padx=0)
+
 
         except KeyError as e:
             logging_critical("Parameter %s not found in the %s file: %s", param_name, self.current_file, e, exc_info=True)
             sys_exit(1)
 
         # Configure the table_frame to stretch columns
-        self.view_port.columnconfigure(0, weight=0, minsize=120) # Parameter name
-        self.view_port.columnconfigure(1, weight=0) # Current Value
-        self.view_port.columnconfigure(2, weight=0) # New Value
-        self.view_port.columnconfigure(3, weight=0) # Units
-        self.view_port.columnconfigure(4, weight=0) # write to FC
-        self.view_port.columnconfigure(5, weight=1) # Change Reason
+        self.view_port.columnconfigure(0, weight=0) # Delete and Add buttons
+        self.view_port.columnconfigure(1, weight=0, minsize=120) # Parameter name
+        self.view_port.columnconfigure(2, weight=0) # Current Value
+        self.view_port.columnconfigure(3, weight=0) # New Value
+        self.view_port.columnconfigure(4, weight=0) # Units
+        self.view_port.columnconfigure(5, weight=0) # write to FC
+        self.view_port.columnconfigure(6, weight=1) # Change Reason
+
+    def __create_delete_button(self, param_name):
+        delete_button = tk.Button(self.view_port, text="Del", command=lambda: self.__on_parameter_delete(param_name))
+        return delete_button
 
     def __create_parameter_name(self, param_name, param_metadata, doc_tooltip):
         is_calibration = param_metadata.get('Calibration', False) if param_metadata else False
         is_readonly = param_metadata.get('ReadOnly', False) if param_metadata else False
         parameter_label = tk.Label(self.view_port, text=param_name + (" " * (16 - len(param_name))),
                                            background="red" if is_readonly else "yellow" if is_calibration else
                                            self.background_color)
@@ -304,15 +320,15 @@
             show_tooltip(unit_label, unit_tooltip)
         return unit_label
 
     def __create_write_write_checkbutton(self, param_name):
         self.write_checkbutton_var[param_name] = tk.BooleanVar(value=True) # Default to selected
         write_write_checkbutton = ttk.Checkbutton(self.view_port,
                                                           variable=self.write_checkbutton_var[param_name])
-        show_tooltip(write_write_checkbutton, f'When selected write {param_name} new value to the flight controller')
+        show_tooltip(write_write_checkbutton, f'When selected upload {param_name} new value to the flight controller')
         return write_write_checkbutton
 
     def __create_change_reason_entry(self, param_name, param, new_value_entry):
 
         present_as_forced = False
         if self.current_file in self.local_filesystem.forced_parameters and \
            param_name in self.local_filesystem.forced_parameters[self.current_file]:
@@ -333,14 +349,49 @@
             change_reason_entry.config(state='disabled', background='light grey')
         else:
             change_reason_entry.bind("<FocusOut>", lambda event, current_file=self.current_file, param_name=param_name:
                                      self.__on_parameter_change_reason_change(event, current_file, param_name))
         show_tooltip(change_reason_entry, f'Reason why {param_name} should change to {new_value_entry.get()}')
         return change_reason_entry
 
+    def __on_parameter_delete(self, param_name):
+        if messagebox.askyesno(f"{self.current_file}", f"Are you sure you want to delete the {param_name} parameter?"):
+            del self.local_filesystem.file_parameters[self.current_file][param_name]
+            self.at_least_one_param_edited = True
+            self.parameter_editor.repopulate_parameter_table(self.current_file)
+
+    def __on_parameter_add(self, fc_parameters):
+        # Prompt the user for a parameter name
+        param_name = simpledialog.askstring("New parameter name", "Enter new parameter name:")
+        if not param_name:
+            messagebox.showerror("Parameter name can not be empty.")
+            return
+        if param_name in self.local_filesystem.file_parameters[self.current_file]:
+            messagebox.showerror("Parameter already exists, edit it instead")
+            return
+        if fc_parameters:
+            if param_name in fc_parameters:
+                self.local_filesystem.file_parameters[self.current_file][param_name] = Par(fc_parameters[param_name], "")
+                self.at_least_one_param_edited = True
+                self.parameter_editor.repopulate_parameter_table(self.current_file)
+            else:
+                messagebox.showerror("Invalid parameter name.", "Parameter name not found in the flight controller.")
+        elif self.local_filesystem.doc_dict:
+            if param_name in self.local_filesystem.doc_dict:
+                self.local_filesystem.file_parameters[self.current_file][param_name] = Par( \
+                    self.local_filesystem.param_default_dict.get(param_name, Par(0, "")).value, "")
+                self.at_least_one_param_edited = True
+                self.parameter_editor.repopulate_parameter_table(self.current_file)
+            else:
+                messagebox.showerror("Invalid parameter name.", "Parameter name not found in the apm.pdef.xml file.")
+        else:
+            messagebox.showerror("Operation not possible",
+                                    "Can not add parameter when no FC is connected and no apm.pdef.xml file exists.")
+
+
     def __on_parameter_value_change(self, event, current_file, param_name):
         # Get the new value from the Entry widget
         new_value = event.widget.get()
         try:
             old_value = self.local_filesystem.file_parameters[current_file][param_name].value
         except KeyError as e:
             logging_critical("Parameter %s not found in the %s file: %s", param_name, current_file, e, exc_info=True)
```

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/get_release_stats.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/get_release_stats.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/param_ftp.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/param_ftp.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/param_pid_adjustment_update.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/param_pid_adjustment_update.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator/tempcal_imu.py` & `methodicconfigurator-0.5.1/MethodicConfigurator/tempcal_imu.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/PKG-INFO` & `methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.4.2
+Version: 0.5.1
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
@@ -53,32 +53,32 @@
 
 ## Usage
 
 Usage is detailed in the [USERMANUAL.md](https://github.com/ArduPilot/MethodicConfigurator/blob/master/USERMANUAL.md) file
 
 ## MS Windows Installation
 
-Download the [latest MethodicConfiguratorSetup-x.x.x.exe installer file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest). Just install it and you do not need any other steps.
+Download the [latest MethodicConfiguratorSetup-x.x.x.exe installer file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest).
 
-Otherwise, install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
+## Linux Installation
+
+Install [python pip](https://pypi.org/project/pip/). Then do:
 
 ```bash
-git clone https://github.com/ArduPilot/MethodicConfigurator.git
-cd MethodicConfigurator
-.\install_windows.bat
+pip install -U MethodicConfigurator
 ```
 
-## Linux Installation
+## MacOS Installation
 
 Install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
 
 ```bash
 git clone https://github.com/ArduPilot/MethodicConfigurator.git
 cd MethodicConfigurator
-./install_linux.sh
+./install_macos.sh
 ```
 
 ## Support and Contributing
 
 Please feel free to submit [issues](https://github.com/ArduPilot/MethodicConfigurator/issues) or [pull requests](https://github.com/ArduPilot/MethodicConfigurator/pulls). More information is available on the [contributing and support](https://github.com/ArduPilot/MethodicConfigurator/blob/master/CONTRIBUTING.md) page.
 
 ## Software architecture
```

### Comparing `methodicconfigurator-0.4.2/MethodicConfigurator.egg-info/SOURCES.txt` & `methodicconfigurator-0.5.1/MethodicConfigurator.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
```

### Comparing `methodicconfigurator-0.4.2/PKG-INFO` & `methodicconfigurator-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.4.2
+Version: 0.5.1
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
@@ -53,32 +53,32 @@
 
 ## Usage
 
 Usage is detailed in the [USERMANUAL.md](https://github.com/ArduPilot/MethodicConfigurator/blob/master/USERMANUAL.md) file
 
 ## MS Windows Installation
 
-Download the [latest MethodicConfiguratorSetup-x.x.x.exe installer file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest). Just install it and you do not need any other steps.
+Download the [latest MethodicConfiguratorSetup-x.x.x.exe installer file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest).
 
-Otherwise, install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
+## Linux Installation
+
+Install [python pip](https://pypi.org/project/pip/). Then do:
 
 ```bash
-git clone https://github.com/ArduPilot/MethodicConfigurator.git
-cd MethodicConfigurator
-.\install_windows.bat
+pip install -U MethodicConfigurator
 ```
 
-## Linux Installation
+## MacOS Installation
 
 Install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
 
 ```bash
 git clone https://github.com/ArduPilot/MethodicConfigurator.git
 cd MethodicConfigurator
-./install_linux.sh
+./install_macos.sh
 ```
 
 ## Support and Contributing
 
 Please feel free to submit [issues](https://github.com/ArduPilot/MethodicConfigurator/issues) or [pull requests](https://github.com/ArduPilot/MethodicConfigurator/pulls). More information is available on the [contributing and support](https://github.com/ArduPilot/MethodicConfigurator/blob/master/CONTRIBUTING.md) page.
 
 ## Software architecture
```

### Comparing `methodicconfigurator-0.4.2/README.md` & `methodicconfigurator-0.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 ## Usage
 
 Usage is detailed in the [USERMANUAL.md](USERMANUAL.md) file
 
 ## MS Windows Installation
 
-Download the [latest MethodicConfiguratorSetup-x.x.x.exe installer file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest). Just install it and you do not need any other steps.
+Download the [latest MethodicConfiguratorSetup-x.x.x.exe installer file](https://github.com/ArduPilot/MethodicConfigurator/releases/tag/latest).
 
-Otherwise, install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
+## Linux Installation
+
+Install [python pip](https://pypi.org/project/pip/). Then do:
 
 ```bash
-git clone https://github.com/ArduPilot/MethodicConfigurator.git
-cd MethodicConfigurator
-.\install_windows.bat
+pip install -U MethodicConfigurator
 ```
 
-## Linux Installation
+## MacOS Installation
 
 Install [git](https://git-scm.com/) and [python](https://www.python.org/downloads/). Then do:
 
 ```bash
 git clone https://github.com/ArduPilot/MethodicConfigurator.git
 cd MethodicConfigurator
-./install_linux.sh
+./install_macos.sh
 ```
 
 ## Support and Contributing
 
 Please feel free to submit [issues](https://github.com/ArduPilot/MethodicConfigurator/issues) or [pull requests](https://github.com/ArduPilot/MethodicConfigurator/pulls). More information is available on the [contributing and support](CONTRIBUTING.md) page.
 
 ## Software architecture
```

### Comparing `methodicconfigurator-0.4.2/setup.py` & `methodicconfigurator-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # Sensor Bitmask
 # Bitmap of which IMUs to log batch data for. This option takes effect on the next reboot.
 # Bitmask: 0:IMU1,1:IMU2,2:IMU3
 # RebootRequired: True
 # Default: 0
-INS_LOG_BAT_MASK,3 # the Matek H743 fligth controller only has two IMUs
+INS_LOG_BAT_MASK,3  # the Matek H743 fligth controller only has two IMUs
 
 # Enable temperature calibration
 # Enable the use of temperature calibration parameters for this IMU. For automatic learning set to 2 and
 # also set the INS_TCALn_TMAX to the target temperature, then reboot
 # RebootRequired: True
 # 0: Disabled
 # 1: Enabled
 # 2: LearnCalibration
 # Default: 0
-INS_TCAL1_ENABLE,2 # Activates the temperature calibration for IMU 1 at the next start
+INS_TCAL1_ENABLE,2  # Activates the temperature calibration for IMU 1 at the next start
 
 # Temperature calibration max
 # The maximum temperature that the calibration is valid for. This must be at least 10 degrees above TMIN
 # for calibration
 # Range: -70 80
 # Units: degC (degrees Celsius)
 # Calibration: 1
 # Default: 70
-INS_TCAL1_TMAX,60 # our H7 processor acts as a heater and heats up the board to almost 60 deg
+INS_TCAL1_TMAX,60  # our H7 processor acts as a heater and heats up the board to almost 60 deg
 
 # Enable temperature calibration
 # Enable the use of temperature calibration parameters for this IMU. For automatic learning set to 2 and
 # also set the INS_TCALn_TMAX to the target temperature, then reboot
 # RebootRequired: True
 # 0: Disabled
 # 1: Enabled
 # 2: LearnCalibration
 # Default: 0
-INS_TCAL2_ENABLE,2 # Activates the temperature calibration for IMU 2 at the next start
+INS_TCAL2_ENABLE,2  # Activates the temperature calibration for IMU 2 at the next start
 
 # Temperature calibration max
 # The maximum temperature that the calibration is valid for. This must be at least 10 degrees above TMIN
 # for calibration
 # Range: -70 80
 # Units: degC (degrees Celsius)
 # Calibration: 1
 # Default: 70
-INS_TCAL2_TMAX,60 # our H7 processor acts as a heater and heats up the board to almost 60 deg
+INS_TCAL2_TMAX,60  # our H7 processor acts as a heater and heats up the board to almost 60 deg
 
 # Log bitmask
 # Bitmap of what on-board log types to enable. This value is made up of the sum of each of the log types
 # you want to be saved. It is usually best just to enable all basiclog types by setting this to 65535.
 # Bitmask: 0:Fast Attitude,1:Medium Attitude,2:GPS,3:System Performance,4:Control Tuning,5:Navigation Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,10:RC output,11:Optical Flow,12:PID,13:Compass,15:Camera,17:Motors,18:Fast IMU,19:Raw IMU,20:Video Stabilization,21:Fast harmonic notch logging
 # Default: 176126
-LOG_BITMASK,524416 # Only for IMU and Raw-IMU
+LOG_BITMASK,524416  # Only for IMU and Raw-IMU
 
 # Enable logging while disarmed
 # If LOG_DISARMED is set to 1 then logging will be enabled while disarmed. This can make for very large
 # logfiles but can help a lot when tracking down startup issues
 # 0: Disabled
 # 1: Enabled
 # Default: 0
-LOG_DISARMED,1 # to gather data for the offline IMU temperature compensation while the FC is disarmed
+LOG_DISARMED,1  # Gather data for the offline IMU temperature compensation while the FC is disarmed
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param`

 * *Files 12% similar despite different names*

```diff
@@ -270,29 +270,14 @@
 # 2: RCChannelPwmValue
 # 3: ReceiverProtocol
 # 4: PWMInputPin
 # 5: TelemetryRadioRSSI
 # Default: 0
 RSSI_TYPE,3 # TBS Crossfire protocol provides RSSI
 
-# Telemetry 2 Baud Rate
-# The baud rate of the Telem2 port. Most stm32-based boards can support rates of up to 1500. If you setup a
-# rate you cannot support and then can't connect to your board you should load a firmware from a different
-# vehicle type. That will reset all your parameters to defaults.
-# 1: 1200                                              115: 115200
-# 2: 2400                                              230: 230400
-# 4: 4800                                              256: 256000
-# 9: 9600                                              460: 460800
-# 19: 19200                                            500: 500000
-# 38: 38400                                            921: 921600
-# 57: 57600                                            1500: 1500000
-# 111: 111100
-# Default: 57
-SERIAL2_BAUD,115 # For Mavlink over crossfire
-
 # Serial7 protocol selection
 # Control what protocol Serial7 port should be used for. Note that the Frsky options require external
 # converter hardware. See the wiki for details.
 # RebootRequired: True
 # -1: None                                             24: EFI Serial
 # 1: MAVLink1                                          25: LTM
 # 2: MAVLink2                                          26: RunCam
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param`

 * *Files 9% similar despite different names*

```diff
@@ -43,26 +43,27 @@
 # 2: OneShot125
 # 3: Brushed
 # 4: DShot150
 # 5: DShot300
 # 6: DShot600
 # 7: DShot1200
 # 8: PWMRange
+# 9: PWMAngle
 # Default: 0
 MOT_PWM_TYPE,6  # the most recomended speed for ArduCopter
 
 # Buzzer Driver Types
 # Controls what types of Buzzer will be enabled
 # Bitmask: 0:Built-in buzzer, 1:DShot, 2:DroneCAN
 # Default: 5
 NTF_BUZZ_TYPES,3  # the 4-in-1 ESC uses this
 
 # LED Driver Types
 # Controls what types of LEDs will be enabled
-# Bitmask: 0:Built-in LED, 1:Internal ToshibaLED, 2:External ToshibaLED, 3:External PCA9685, 4:Oreo LED, 5:DroneCAN, 6:NCP5623 External, 7:NCP5623 Internal, 8:NeoPixel, 9:ProfiLED, 10:Scripting, 11:DShot, 12:ProfiLED_SPI
+# Bitmask: 0:Built-in LED, 1:Internal ToshibaLED, 2:External ToshibaLED, 3:External PCA9685, 4:Oreo LED, 5:DroneCAN, 6:NCP5623 External, 7:NCP5623 Internal, 8:NeoPixel, 9:ProfiLED, 10:Scripting, 11:DShot, 12:ProfiLED_SPI, 13:LP5562 External, 14: LP5562 Internal, 15:IS31FL3195 External, 16: IS31FL3195 Internal, 17: DiscreteRGB, 18: NeoPixelRGB
 # Default: 123079
 NTF_LED_TYPES,2369  # Built-in LED, NCP5623 External (Holybro F9P), Neopixel (Matek H743 slim v3), and DShot (4-in-1 ESC)
 
 # Accel (vertical) slew rate limit
 # Sets an upper limit on the slew rate produced by the combined P and D gains. If the amplitude of the
 # control action produced by the rate feedback exceeds this value, then the D+P gain is reduced to respect
 # the limit. This limits the amplitude of high frequency oscillations caused by an excessive gain. The
@@ -81,44 +82,45 @@
 # 1: 1200                                              115: 115200
 # 2: 2400                                              230: 230400
 # 4: 4800                                              256: 256000
 # 9: 9600                                              460: 460800
 # 19: 19200                                            500: 500000
 # 38: 38400                                            921: 921600
 # 57: 57600                                            1500: 1500000
-# 111: 111100
+# 111: 111100                                          2000: 2000000
 # Default: 115
 SERIAL5_BAUD,115  # bi-directional DShot telemetry data rate from T-Motor F45 4in1 ESC V2
 
 # Serial5 protocol selection
 # Control what protocol Serial5 port should be used for. Note that the Frsky options require external
 # converter hardware. See the wiki for details.
 # RebootRequired: True
-# -1: None                                             24: EFI Serial
-# 1: MAVLink1                                          25: LTM
-# 2: MAVLink2                                          26: RunCam
-# 3: Frsky D                                           27: HottTelem
-# 4: Frsky SPort                                       28: Scripting
-# 5: GPS                                               29: Crossfire VTX
-# 7: Alexmos Gimbal Serial                             30: Generator
-# 8: SToRM32 Gimbal Serial                             31: Winch
-# 9: Rangefinder                                       32: MSP
-# 10: FrSky SPort Passthrough (OpenTX)                 33: DJI FPV
-# 11: Lidar360                                         34: AirSpeed
-# 13: Beacon                                           35: ADSB
-# 14: Volz servo out                                   36: AHRS
-# 15: SBus servo out                                   37: SmartAudio
-# 16: ESC Telemetry                                    38: FETtecOneWire
-# 17: Devo Telemetry                                   39: Torqeedo
-# 18: OpticalFlow                                      40: AIS
-# 19: RobotisServo                                     41: CoDevESC
-# 20: NMEA Output                                      42: DisplayPort
-# 21: WindVane                                         43: MAVLink High Latency
-# 22: SLCAN                                            44: IRC Tramp
-# 23: RCIN
+# -1: None                                             25: LTM
+# 1: MAVLink1                                          26: RunCam
+# 2: MAVLink2                                          27: HottTelem
+# 3: Frsky D                                           28: Scripting
+# 4: Frsky SPort                                       29: Crossfire VTX
+# 5: GPS                                               30: Generator
+# 7: Alexmos Gimbal Serial                             31: Winch
+# 8: Gimbal                                            32: MSP
+# 9: Rangefinder                                       33: DJI FPV
+# 10: FrSky SPort Passthrough (OpenTX)                 34: AirSpeed
+# 11: Lidar360                                         35: ADSB
+# 13: Beacon                                           36: AHRS
+# 14: Volz servo out                                   37: SmartAudio
+# 15: SBus servo out                                   38: FETtecOneWire
+# 16: ESC Telemetry                                    39: Torqeedo
+# 17: Devo Telemetry                                   40: AIS
+# 18: OpticalFlow                                      41: CoDevESC
+# 19: RobotisServo                                     42: DisplayPort
+# 20: NMEA Output                                      43: MAVLink High Latency
+# 21: WindVane                                         44: IRC Tramp
+# 22: SLCAN                                            45: DDS XRCE
+# 23: RCIN                                             46: IMUDATA
+# 24: EFI Serial
 # Default: -1
 SERIAL5_PROTOCOL,16  # bi-directional DShot telemetry pin is connected to SERIAL5
 
 # BLHeli pass-thru auto-enable for multicopter motors
 # If set to 1 this auto-enables BLHeli pass-thru support for all multicopter motors
 # RebootRequired: True
 # 0: Disabled
@@ -146,59 +148,63 @@
 # disables telemetry requests
 # Units: Hz (hertz)
 # Range: 0 500
 # Default: 10
 SERVO_BLH_TRATE,5  # Set to a low value because the RPM telemetry uses bi-directional DShot telemetry instead of this UART telemetry
 
 # Servo DShot ESC type
-# This sets the DShot ESC type for all outputs. The ESC type affects the range of DShot commands available.
-# None means that no dshot commands will be executed.
+# DShot ESC type for all outputs. The ESC type affects the range of DShot commands available and the bit
+# widths used. None means that no dshot commands will be executed. Some ESC types support Extended DShot
+# Telemetry (EDT) which allows telemetry other than RPM data to be returned when using bi-directional
+# dshot. If you enable EDT you must install EDT capable firmware for correct operation.
 # 0: None
 # 1: BLHeli32/Kiss
 # 2: BLHeli_S
+# 3: BLHeli32/Kiss+EDT
+# 4: BLHeli_S+EDT
 # Default: 0
-SERVO_DSHOT_ESC,1  # BLHeli32
+SERVO_DSHOT_ESC,1
 
 # Servo DShot output rate
-# This sets the DShot output rate for all outputs as a multiple of the loop rate. 0 sets the output rate to
-# be fixed at 1Khz for low loop rates. This value should never be set below 500Hz.
+# DShot output rate for all outputs as a multiple of the loop rate. 0 sets the output rate to be fixed at
+# 1Khz for low loop rates. This value should never be set below 500Hz.
 # 0: 1Khz
 # 1: loop-rate
 # 2: double loop-rate
 # 3: triple loop-rate
 # 4: quadruple loop rate
 # Default: 0
-SERVO_DSHOT_RATE,2  # Sends DShot control signals to the ESC twice per control loop
+SERVO_DSHOT_RATE,2 # Sends DShot control signals to the ESC twice per control loop
 
 # Maximum PWM
 # maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 2000
-SERVO1_MAX,2000  # Use the full available 1000-2000 DShot range
+SERVO1_MAX,2000
 
 # Minimum PWM
 # minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1000
-SERVO1_MIN,1000  # Use the full available 1000-2000 DShot range
+SERVO1_MIN,1000
 
 # Trim PWM
 # Trim PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1000
-SERVO1_TRIM,1000  # Use the full available 1000-2000 DShot range
+SERVO1_TRIM,1000
 
 # Servo output function
 # Function assigned to this servo. Setting this to Disabled(0) will setup this output for control by auto
 # missions or MAVLink servo set commands. any other value will enable the corresponding function
 # RebootRequired: True
 # -1: GPIO                   40: Motor8                 90: CameraISO              127: RateYaw
 # 0: Disabled                51: RCIN1                  91: CameraAperture         129: ProfiLED1
@@ -233,86 +239,86 @@
 # Maximum PWM
 # maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 2000
-SERVO2_MAX,2000  # Use the full available 1000-2000 DShot range
+SERVO2_MAX,2000
 
 # Minimum PWM
 # minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1000
-SERVO2_MIN,1000  # Use the full available 1000-2000 DShot range
+SERVO2_MIN,1000
 
 # Trim PWM
 # Trim PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1000
-SERVO2_TRIM,1000  # Use the full available 1000-2000 DShot range
+SERVO2_TRIM,1000
 
 # Maximum PWM
 # maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 2000
-SERVO3_MAX,2000  # Use the full available 1000-2000 DShot range
+SERVO3_MAX,2000
 
 # Minimum PWM
 # minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1000
-SERVO3_MIN,1000  # Use the full available 1000-2000 DShot range
+SERVO3_MIN,1000
 
 # Trim PWM
 # Trim PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1000
-SERVO3_TRIM,1000  # Use the full available 1000-2000 DShot range
+SERVO3_TRIM,1000
 
 # Maximum PWM
 # maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 2000
-SERVO4_MAX,2000  # Use the full available 1000-2000 DShot range
+SERVO4_MAX,2000
 
 # Minimum PWM
 # minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1000
-SERVO4_MIN,1000  # Use the full available 1000-2000 DShot range
+SERVO4_MIN,1000
 
 # Trim PWM
 # Trim PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is upper
 # limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1000
-SERVO4_TRIM,1000  # Use the full available 1000-2000 DShot range
+SERVO4_TRIM,1000
 
 # Takeoff Check RPM minimum
 # Takeoff is not permitted until motors report at least this RPM.  Set to zero to disable check
 # Range: 0 10000
 # Default: 0
 TKOFF_RPM_MIN,1400  # Our motors should idle at around 1400 RPM, see https://ardupilot.org/copter/docs/tkoff-rpm-min.html
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param`

 * *Files 24% similar despite different names*

```diff
@@ -86,43 +86,14 @@
 # 21: WindVane                                         44: IRC Tramp
 # 22: SLCAN                                            45: DDS XRCE
 # 23: RCIN                                             46: IMUDATA
 # 24: EFI Serial
 # Default: 5
 SERIAL3_PROTOCOL,5  # GNSS receiver is connected to serial3
 
-# Serial4 protocol selection
-# Control what protocol Serial4 port should be used for. Note that the Frsky options require external
-# converter hardware. See the wiki for details.
-# RebootRequired: True
-# -1: None                                             24: EFI Serial
-# 1: MAVLink1                                          25: LTM
-# 2: MAVLink2                                          26: RunCam
-# 3: Frsky D                                           27: HottTelem
-# 4: Frsky SPort                                       28: Scripting
-# 5: GPS                                               29: Crossfire VTX
-# 7: Alexmos Gimbal Serial                             30: Generator
-# 8: SToRM32 Gimbal Serial                             31: Winch
-# 9: Rangefinder                                       32: MSP
-# 10: FrSky SPort Passthrough (OpenTX)                 33: DJI FPV
-# 11: Lidar360                                         34: AirSpeed
-# 13: Beacon                                           35: ADSB
-# 14: Volz servo out                                   36: AHRS
-# 15: SBus servo out                                   37: SmartAudio
-# 16: ESC Telemetry                                    38: FETtecOneWire
-# 17: Devo Telemetry                                   39: Torqeedo
-# 18: OpticalFlow                                      40: AIS
-# 19: RobotisServo                                     41: CoDevESC
-# 20: NMEA Output                                      42: DisplayPort
-# 21: WindVane                                         43: MAVLink High Latency
-# 22: SLCAN                                            44: IRC Tramp
-# 23: RCIN
-# Default: 5
-SERIAL4_PROTOCOL,-1  # No GNSS connected to serial4, so disable it
-
 # Waypoint Radius
 # Defines the distance from a waypoint, that when crossed indicates the wp has been hit.
 # Units: cm (centimeters)
 # Range: 5 1000
 # Increment: 1
 # Default: 200
 WPNAV_RADIUS,100  # we have a good GNSS receiver so we can afford to fly precisely
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_mp_setup_mandatory_hardware.param`

 * *Files 2% similar despite different names*

```diff
@@ -23,100 +23,100 @@
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_P_MAX,193500.0
+ATC_ACCEL_P_MAX,193500
 
 # Acceleration Max for Roll
 # Maximum acceleration in roll axis
 # Units: cdeg/s/s (centidegrees per square second)
 # Range: 0 180000
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_R_MAX,193500.0
+ATC_ACCEL_R_MAX,193500
 
 # Acceleration Max for Yaw
 # Maximum acceleration in yaw axis
 # Units: cdeg/s/s (centidegrees per square second)
 # Range: 0 72000
 # Increment: 1000
 # 0: Disabled
 # 9000: VerySlow
 # 18000: Slow
 # 36000: Medium
 # 54000: Fast
 # Default: 27000
-ATC_ACCEL_Y_MAX,33300.0
+ATC_ACCEL_Y_MAX,33300
 
 # Pitch axis rate controller derivative frequency in Hz
 # Pitch axis rate controller derivative frequency in Hz
 # Range: 0 50
 # Increment: 1
 # Units: Hz (hertz)
 # Default: 20
-ATC_RAT_PIT_FLTD,57.5  # INS_GYRO_FILTER / 2
+ATC_RAT_PIT_FLTD,57.5 # INS_GYRO_FILTER / 2
 
 # Pitch axis rate controller target frequency in Hz
 # Pitch axis rate controller target frequency in Hz
 # Range: 5 50
 # Increment: 1
 # Units: Hz (hertz)
 # Default: 20
-ATC_RAT_PIT_FLTT,57.5  # INS_GYRO_FILTER / 2
+ATC_RAT_PIT_FLTT,57.5 # INS_GYRO_FILTER / 2
 
 # Roll axis rate controller derivative frequency in Hz
 # Roll axis rate controller derivative frequency in Hz
 # Range: 0 50
 # Increment: 1
 # Units: Hz (hertz)
 # Default: 20
-ATC_RAT_RLL_FLTD,57.5  # INS_GYRO_FILTER / 2
+ATC_RAT_RLL_FLTD,57.5 # INS_GYRO_FILTER / 2
 
 # Roll axis rate controller target frequency in Hz
 # Roll axis rate controller target frequency in Hz
 # Range: 5 50
 # Increment: 1
 # Units: Hz (hertz)
 # Default: 20
-ATC_RAT_RLL_FLTT,57.5  # INS_GYRO_FILTER / 2
+ATC_RAT_RLL_FLTT,57.5 # INS_GYRO_FILTER / 2
 
 # Yaw axis rate controller error frequency in Hz
 # Yaw axis rate controller error frequency in Hz
 # Range: 5 50
 # Increment: 1
 # Units: Hz (hertz)
 # Default: 2.5
-ATC_RAT_YAW_FLTE,2.0
+ATC_RAT_YAW_FLTE,2
 
 # Yaw axis rate controller target frequency in Hz
 # Yaw axis rate controller target frequency in Hz
 # Range: 5 50
 # Increment: 1
 # Units: Hz (hertz)
 # Default: 20
-ATC_RAT_YAW_FLTT,57.5  # INS_GYRO_FILTER / 2
+ATC_RAT_YAW_FLTT,57.5 # INS_GYRO_FILTER / 2
 
 # Compass is attached via an external cable
 # Configure compass so it is attached externally. This is auto-detected on most boards. Set to 1 if the
 # compass is externally connected. When externally connected the COMPASS_ORIENT option operates
 # independently of the AHRS_ORIENTATION board orientation option. If set to 0 or 1 then auto-detection by
 # bus connection can override the value. If set to 2 then auto-detection will be disabled.
 # 0: Internal
 # 1: External
 # 2: ForcedExternal
 # Default: 0
-COMPASS_EXTERNAL,1.0
+COMPASS_EXTERNAL,1
 
 # Compass orientation
 # The orientation of the first external compass relative to the vehicle frame. This value will be ignored
 # unless this compass is set as an external compass. When set correctly in the northern hemisphere,
 # pointing the nose and right side down should increase the MagX and MagY values respectively. Rolling the
 # vehicle upside down should decrease the MagZ value. For southern hemisphere, switch increase and
 # decrease. NOTE: For internal compasses, AHRS_ORIENT is used. The label for each option is specified in
@@ -137,61 +137,61 @@
 # 10: Yaw90Roll180                    26: Yaw90Pitch180                   43: Roll315
 # 11: Yaw135Roll180                   27: Yaw270Pitch180                  100: Custom 4.1 and older
 # 12: Pitch180                        28: Pitch90Roll90                   101: Custom 1
 # 13: Yaw225Roll180                   29: Pitch90Roll180                  102: Custom 2
 # 14: Yaw270Roll180                   30: Pitch90Roll270
 # 15: Yaw315Roll180                   31: Pitch180Roll90
 # Default: 0
-COMPASS_ORIENT,6.0
+COMPASS_ORIENT,6
 
 # Compass device id with 1st order priority
 # Compass device id with 1st order priority, set automatically if 0. Reboot required after change.
 # RebootRequired: True
 # Default: 0
-COMPASS_PRIO1_ID,658953.0
+COMPASS_PRIO1_ID,658953
 
 # Compass2 used for yaw
 # Enable or disable the secondary compass for determining heading.
 # 0: Disabled
 # 1: Enabled
 # Default: 1
-COMPASS_USE2,0.0
+COMPASS_USE2,0
 
 # Compass3 used for yaw
 # Enable or disable the tertiary compass for determining heading.
 # 0: Disabled
 # 1: Enabled
 # Default: 1
-COMPASS_USE3,0.0
+COMPASS_USE3,0
 
 # Fence Action
 # What action should be taken when fence is breached
 # 0: Report Only
 # 1: RTL or Land
 # 2: Always Land
 # 3: SmartRTL or RTL or Land
 # 4: Brake or Land
 # 5: SmartRTL or Land
 # Default: 1
-FENCE_ACTION,3.0
+FENCE_ACTION,3
 
 # Fence Maximum Altitude
 # Maximum altitude allowed before geofence triggers
 # Units: m (meters)
 # Range: 10 1000
 # Increment: 1
 # Default: 100
 FENCE_ALT_MAX,80.0
 
 # Fence enable/disable
 # Allows you to enable (1) or disable (0) the fence functionality
 # 0: Disabled
 # 1: Enabled
 # Default: 0
-FENCE_ENABLE,1.0
+FENCE_ENABLE,1
 
 # Circular Fence Radius
 # Circle fence radius which when breached will cause an RTL
 # Units: m (meters)
 # Range: 30 10000
 # Default: 300
 FENCE_RADIUS,150.0
@@ -202,100 +202,100 @@
 # 1: Acro                    9: Land                    18: Throw                  25: SystemID
 # 2: AltHold                 11: Drift                  19: Avoid_ADSB             26: Heli_Autorotate
 # 3: Auto                    13: Sport                  20: Guided_NoGPS           27: Auto RTL
 # 4: Guided                  14: Flip                   21: Smart_RTL
 # 5: Loiter                  15: AutoTune               22: FlowHold
 # 6: RTL                     16: PosHold                23: Follow
 # Default: 0
-FLTMODE1,0.0
+FLTMODE1,0
 
 # Flight Mode 2
 # Flight mode when pwm of Flightmode channel(FLTMODE_CH) is >1230, <= 1360
 # 0: Stabilize               7: Circle                  17: Brake                  24: ZigZag
 # 1: Acro                    9: Land                    18: Throw                  25: SystemID
 # 2: AltHold                 11: Drift                  19: Avoid_ADSB             26: Heli_Autorotate
 # 3: Auto                    13: Sport                  20: Guided_NoGPS           27: Auto RTL
 # 4: Guided                  14: Flip                   21: Smart_RTL
 # 5: Loiter                  15: AutoTune               22: FlowHold
 # 6: RTL                     16: PosHold                23: Follow
 # Default: 0
-FLTMODE2,2.0
+FLTMODE2,2
 
 # Flight Mode 3
 # Flight mode when pwm of Flightmode channel(FLTMODE_CH) is >1360, <= 1490
 # 0: Stabilize               7: Circle                  17: Brake                  24: ZigZag
 # 1: Acro                    9: Land                    18: Throw                  25: SystemID
 # 2: AltHold                 11: Drift                  19: Avoid_ADSB             26: Heli_Autorotate
 # 3: Auto                    13: Sport                  20: Guided_NoGPS           27: Auto RTL
 # 4: Guided                  14: Flip                   21: Smart_RTL
 # 5: Loiter                  15: AutoTune               22: FlowHold
 # 6: RTL                     16: PosHold                23: Follow
 # Default: 0
-FLTMODE3,5.0
+FLTMODE3,5
 
 # Flight Mode 4
 # Flight mode when pwm of Flightmode channel(FLTMODE_CH) is >1490, <= 1620
 # 0: Stabilize               7: Circle                  17: Brake                  24: ZigZag
 # 1: Acro                    9: Land                    18: Throw                  25: SystemID
 # 2: AltHold                 11: Drift                  19: Avoid_ADSB             26: Heli_Autorotate
 # 3: Auto                    13: Sport                  20: Guided_NoGPS           27: Auto RTL
 # 4: Guided                  14: Flip                   21: Smart_RTL
 # 5: Loiter                  15: AutoTune               22: FlowHold
 # 6: RTL                     16: PosHold                23: Follow
 # Default: 0
-FLTMODE4,3.0
+FLTMODE4,3
 
 # Flight Mode 5
 # Flight mode when pwm of Flightmode channel(FLTMODE_CH) is >1620, <= 1749
 # 0: Stabilize               7: Circle                  17: Brake                  24: ZigZag
 # 1: Acro                    9: Land                    18: Throw                  25: SystemID
 # 2: AltHold                 11: Drift                  19: Avoid_ADSB             26: Heli_Autorotate
 # 3: Auto                    13: Sport                  20: Guided_NoGPS           27: Auto RTL
 # 4: Guided                  14: Flip                   21: Smart_RTL
 # 5: Loiter                  15: AutoTune               22: FlowHold
 # 6: RTL                     16: PosHold                23: Follow
 # Default: 0
-FLTMODE5,6.0
+FLTMODE5,6
 
 # Flight Mode 6
 # Flight mode when pwm of Flightmode channel(FLTMODE_CH) is >=1750
 # 0: Stabilize               7: Circle                  17: Brake                  24: ZigZag
 # 1: Acro                    9: Land                    18: Throw                  25: SystemID
 # 2: AltHold                 11: Drift                  19: Avoid_ADSB             26: Heli_Autorotate
 # 3: Auto                    13: Sport                  20: Guided_NoGPS           27: Auto RTL
 # 4: Guided                  14: Flip                   21: Smart_RTL
 # 5: Loiter                  15: AutoTune               22: FlowHold
 # 6: RTL                     16: PosHold                23: Follow
 # Default: 0
-FLTMODE6,15.0
+FLTMODE6,15
 
 # Frame Class
 # Controls major frame class for multicopter component
 # RebootRequired: True
 # 0: Undefined                        6: Heli                             12: DodecaHexa
 # 1: Quad                             7: Tri                              13: HeliQuad
 # 2: Hexa                             8: SingleCopter                     14: Deca
 # 3: Octa                             9: CoaxCopter                       15: Scripting Matrix
 # 4: OctaQuad                         10: BiCopter                        16: 6DoF Scripting
 # 5: Y6                               11: Heli_Dual                       17: Dynamic Scripting Matrix
 # Default: 0
-FRAME_CLASS,1.0
+FRAME_CLASS,1
 
 # Frame Type (+, X, V, etc)
 # Controls motor mixing for multicopters.  Not used for Tri or Traditional Helicopters.
 # RebootRequired: True
 # 0: Plus                                              11: Y6F
 # 1: X                                                 12: BetaFlightX
 # 2: V                                                 13: DJIX
 # 3: H                                                 14: ClockwiseX
 # 4: V-Tail                                            15: I
 # 5: A-Tail                                            18: BetaFlightXReversed
 # 10: Y6B                                              19: Y4
 # Default: 1
-FRAME_TYPE,1.0
+FRAME_TYPE,1
 
 # Calibration temperature for 1st accelerometer
 # Temperature that the 1st accelerometer was calibrated at
 # Units: degC (degrees Celsius)
 # Calibration: 1
 # Default: -300
 INS_ACC1_CALTEMP,39.97585
@@ -329,29 +329,29 @@
 INS_ACC2SCAL_Z,0.9998143
 
 # Accelerometer3 scaling of X axis
 # Accelerometer3 scaling of X axis.  Calculated during acceleration calibration routine
 # Range: 0.8 1.2
 # Calibration: 1
 # Default: 1
-INS_ACC3SCAL_X,0.0
+INS_ACC3SCAL_X,0
 
 # Accelerometer3 scaling of Y axis
 # Accelerometer3 scaling of Y axis  Calculated during acceleration calibration routine
 # Range: 0.8 1.2
 # Calibration: 1
 # Default: 1
-INS_ACC3SCAL_Y,0.0
+INS_ACC3SCAL_Y,0
 
 # Accelerometer3 scaling of Z axis
 # Accelerometer3 scaling of Z axis  Calculated during acceleration calibration routine
 # Range: 0.8 1.2
 # Calibration: 1
 # Default: 1
-INS_ACC3SCAL_Z,0.0
+INS_ACC3SCAL_Z,0
 
 # Accelerometer scaling of X axis
 # Accelerometer scaling of X axis.  Calculated during acceleration calibration routine
 # Range: 0.8 1.2
 # Calibration: 1
 # Default: 1
 INS_ACCSCAL_X,0.9991518
@@ -372,22 +372,22 @@
 
 # Gyro filter cutoff frequency
 # Filter cutoff frequency for gyroscopes. This can be set to a lower value to try to cope with very high
 # vibration levels in aircraft. A value of zero means no filtering (not recommended!)
 # Units: Hz (hertz)
 # Range: 0 256
 # Default: 20
-INS_GYRO_FILTER,115.0
+INS_GYRO_FILTER,115
 
 # Use third IMU for attitude, velocity and position estimates
 # Use third IMU for attitude, velocity and position estimates
 # 0: Disabled
 # 1: Enabled
 # Default: 1
-INS_USE3,0.0
+INS_USE3,0
 
 # Battery voltage compensation maximum voltage
 # Battery voltage compensation maximum voltage (voltage above this will have no additional scaling effect
 # on thrust).  Recommend 4.2 * cell count, 0 = Disabled
 # Range: 6 53
 # Units: V (volt)
 # Default: 0
@@ -442,249 +442,249 @@
 # RC max PWM
 # RC maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1900
-RC1_MAX,2011.0
+RC1_MAX,2011
 
 # RC min PWM
 # RC minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1100
-RC1_MIN,988.0
+RC1_MIN,988
 
 # RC trim PWM
 # RC trim (neutral) PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and
 # 2000 is upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1500
-RC1_TRIM,1500.0
+RC1_TRIM,1500
 
 # RC max PWM
 # RC maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1900
-RC2_MAX,2011.0
+RC2_MAX,2011
 
 # RC min PWM
 # RC minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1100
-RC2_MIN,988.0
+RC2_MIN,988
 
 # RC trim PWM
 # RC trim (neutral) PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and
 # 2000 is upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1500
-RC2_TRIM,1500.0
+RC2_TRIM,1500
 
 # RC max PWM
 # RC maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1900
-RC3_MAX,2011.0
+RC3_MAX,2011
 
 # RC min PWM
 # RC minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1100
-RC3_MIN,988.0
+RC3_MIN,988
 
 # RC trim PWM
 # RC trim (neutral) PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and
 # 2000 is upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1500
-RC3_TRIM,1466.0
+RC3_TRIM,1466
 
 # RC max PWM
 # RC maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1900
-RC4_MAX,2011.0
+RC4_MAX,2011
 
 # RC min PWM
 # RC minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1100
-RC4_MIN,988.0
+RC4_MIN,988
 
 # RC trim PWM
 # RC trim (neutral) PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and
 # 2000 is upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1500
-RC4_TRIM,1500.0
+RC4_TRIM,1500
 
 # RC max PWM
 # RC maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1900
-RC5_MAX,1856.0
+RC5_MAX,1856
 
 # RC min PWM
 # RC minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1100
-RC5_MIN,1143.0
+RC5_MIN,1143
 
 # RC trim PWM
 # RC trim (neutral) PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and
 # 2000 is upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1500
-RC5_TRIM,1143.0
+RC5_TRIM,1143
 
 # RC max PWM
 # RC maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1900
-RC6_MAX,2011.0
+RC6_MAX,2011
 
 # RC min PWM
 # RC minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1100
-RC6_MIN,988.0
+RC6_MIN,988
 
 # RC trim PWM
 # RC trim (neutral) PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and
 # 2000 is upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1500
-RC6_TRIM,988.0
+RC6_TRIM,988
 
 # RC max PWM
 # RC maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1900
-RC7_MAX,2011.0
+RC7_MAX,2011
 
 # RC min PWM
 # RC minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1100
-RC7_MIN,988.0
+RC7_MIN,988
 
 # RC trim PWM
 # RC trim (neutral) PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and
 # 2000 is upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1500
-RC7_TRIM,988.0
+RC7_TRIM,988
 
 # RC max PWM
 # RC maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1900
-RC8_MAX,2011.0
+RC8_MAX,2011
 
 # RC min PWM
 # RC minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1100
-RC8_MIN,988.0
+RC8_MIN,988
 
 # RC trim PWM
 # RC trim (neutral) PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and
 # 2000 is upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1500
-RC8_TRIM,988.0
+RC8_TRIM,988
 
 # RC max PWM
 # RC maximum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1900
-RC9_MAX,2011.0
+RC9_MAX,2011
 
 # RC min PWM
 # RC minimum PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and 2000 is
 # upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1100
-RC9_MIN,988.0
+RC9_MIN,988
 
 # RC trim PWM
 # RC trim (neutral) PWM pulse width in microseconds. Typically 1000 is lower limit, 1500 is neutral and
 # 2000 is upper limit.
 # Units: PWM (PWM in microseconds)
 # Range: 800 2200
 # Increment: 1
 # Default: 1500
-RC9_TRIM,988.0
+RC9_TRIM,988
 
 # Servo output function
 # Function assigned to this servo. Setting this to Disabled(0) will setup this output for control by auto
 # missions or MAVLink servo set commands. any other value will enable the corresponding function
 # RebootRequired: True
 # -1: GPIO                   40: Motor8                 90: CameraISO              127: RateYaw
 # 0: Disabled                51: RCIN1                  91: CameraAperture         129: ProfiLED1
@@ -710,15 +710,15 @@
 # 34: Motor2                 81: BoostThrottle          121: NeoPixel2             150: RCIN11Scaled
 # 35: Motor3                 82: Motor9                 122: NeoPixel3             151: RCIN12Scaled
 # 36: Motor4                 83: Motor10                123: NeoPixel4             152: RCIN13Scaled
 # 37: Motor5                 84: Motor11                124: RateRoll              153: RCIN14Scaled
 # 38: Motor6                 85: Motor12                125: RatePitch             154: RCIN15Scaled
 # 39: Motor7                 88: Winch                  126: RateThrust            155: RCIN16Scaled
 # Default: 0
-SERVO1_FUNCTION,33.0
+SERVO1_FUNCTION,33
 
 # Servo output function
 # Function assigned to this servo. Setting this to Disabled(0) will setup this output for control by auto
 # missions or MAVLink servo set commands. any other value will enable the corresponding function
 # RebootRequired: True
 # -1: GPIO                   40: Motor8                 90: CameraISO              127: RateYaw
 # 0: Disabled                51: RCIN1                  91: CameraAperture         129: ProfiLED1
@@ -744,15 +744,15 @@
 # 34: Motor2                 81: BoostThrottle          121: NeoPixel2             150: RCIN11Scaled
 # 35: Motor3                 82: Motor9                 122: NeoPixel3             151: RCIN12Scaled
 # 36: Motor4                 83: Motor10                123: NeoPixel4             152: RCIN13Scaled
 # 37: Motor5                 84: Motor11                124: RateRoll              153: RCIN14Scaled
 # 38: Motor6                 85: Motor12                125: RatePitch             154: RCIN15Scaled
 # 39: Motor7                 88: Winch                  126: RateThrust            155: RCIN16Scaled
 # Default: 0
-SERVO2_FUNCTION,34.0
+SERVO2_FUNCTION,34
 
 # Servo output function
 # Function assigned to this servo. Setting this to Disabled(0) will setup this output for control by auto
 # missions or MAVLink servo set commands. any other value will enable the corresponding function
 # RebootRequired: True
 # -1: GPIO                   40: Motor8                 90: CameraISO              127: RateYaw
 # 0: Disabled                51: RCIN1                  91: CameraAperture         129: ProfiLED1
@@ -778,15 +778,15 @@
 # 34: Motor2                 81: BoostThrottle          121: NeoPixel2             150: RCIN11Scaled
 # 35: Motor3                 82: Motor9                 122: NeoPixel3             151: RCIN12Scaled
 # 36: Motor4                 83: Motor10                123: NeoPixel4             152: RCIN13Scaled
 # 37: Motor5                 84: Motor11                124: RateRoll              153: RCIN14Scaled
 # 38: Motor6                 85: Motor12                125: RatePitch             154: RCIN15Scaled
 # 39: Motor7                 88: Winch                  126: RateThrust            155: RCIN16Scaled
 # Default: 0
-SERVO3_FUNCTION,35.0
+SERVO3_FUNCTION,35
 
 # Servo output function
 # Function assigned to this servo. Setting this to Disabled(0) will setup this output for control by auto
 # missions or MAVLink servo set commands. any other value will enable the corresponding function
 # RebootRequired: True
 # -1: GPIO                   40: Motor8                 90: CameraISO              127: RateYaw
 # 0: Disabled                51: RCIN1                  91: CameraAperture         129: ProfiLED1
@@ -812,8 +812,8 @@
 # 34: Motor2                 81: BoostThrottle          121: NeoPixel2             150: RCIN11Scaled
 # 35: Motor3                 82: Motor9                 122: NeoPixel3             151: RCIN12Scaled
 # 36: Motor4                 83: Motor10                123: NeoPixel4             152: RCIN13Scaled
 # 37: Motor5                 84: Motor11                124: RateRoll              153: RCIN14Scaled
 # 38: Motor6                 85: Motor12                125: RatePitch             154: RCIN15Scaled
 # 39: Motor7                 88: Winch                  126: RateThrust            155: RCIN16Scaled
 # Default: 0
-SERVO4_FUNCTION,36.0
+SERVO4_FUNCTION,36
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param`

 * *Files 4% similar despite different names*

```diff
@@ -1,112 +1,112 @@
 # Timezone offset from UTC
 # Adds offset in +- minutes from UTC to calculate local time
 # Range: -720 +840
 # Default: 0
-BRD_RTC_TZ_MIN,60  # Berlin time zone
+BRD_RTC_TZ_MIN,60
 
 # Fence Type
 # Enabled fence types held as bitmask
-# Bitmask: 0:Max altitude,1:Circle,2:Polygon,3:Min altitude
+# Bitmask: 0:Max altitude,1:Circle Centered on Home,2:Inclusion/Exclusion Circles+Polygons,3:Min altitude
 # Default: 7
-FENCE_TYPE,7  # cylinder and max altitude, to obey local regulations and safety measures
+FENCE_TYPE,11
 
 # Accel filter cutoff frequency
 # Filter cutoff frequency for accelerometers. This can be set to a lower value to try to cope with very
 # high vibration levels in aircraft. A value of zero means no filtering (not recommended!)
 # Units: Hz (hertz)
 # Range: 0 256
 # Default: 20
-INS_ACCEL_FILTER,10  # the default is 20 and that lets too much noise in
+INS_ACCEL_FILTER,10 # the default is 20 and that lets too much noise in
 
 # IMU accelerometer X position
 # X position of the first IMU Accelerometer in body frame. Positive X is forward of the origin. Attention:
 # The IMU should be located as close to the vehicle c.g. as practical so that the value of this parameter
 # is minimised. Failure to do so can result in noisy navigation velocity measurements due to vibration and
 # IMU gyro noise. If the IMU cannot be moved and velocity noise is a problem, a location closer to the IMU
 # can be used as the body frame origin.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-INS_POS1_X,0  # was -0.005
+INS_POS1_X,0 # was -0.005
 
 # IMU accelerometer Y position
 # Y position of the first IMU accelerometer in body frame. Positive Y is to the right of the origin.
 # Attention: The IMU should be located as close to the vehicle c.g. as practical so that the value of this
 # parameter is minimised. Failure to do so can result in noisy navigation velocity measurements due to
 # vibration and IMU gyro noise. If the IMU cannot be moved and velocity noise is a problem, a location
 # closer to the IMU can be used as the body frame origin.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-INS_POS1_Y,0  # was -0.011
+INS_POS1_Y,0 # was -0.011
 
 # IMU accelerometer X position
 # X position of the second IMU accelerometer in body frame. Positive X is forward of the origin. Attention:
 # The IMU should be located as close to the vehicle c.g. as practical so that the value of this parameter
 # is minimised. Failure to do so can result in noisy navigation velocity measurements due to vibration and
 # IMU gyro noise. If the IMU cannot be moved and velocity noise is a problem, a location closer to the IMU
 # can be used as the body frame origin.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-INS_POS2_X,0  # was -0.011
+INS_POS2_X,0 # was -0.011
 
 # IMU accelerometer Y position
 # Y position of the second IMU accelerometer in body frame. Positive Y is to the right of the origin.
 # Attention: The IMU should be located as close to the vehicle c.g. as practical so that the value of this
 # parameter is minimised. Failure to do so can result in noisy navigation velocity measurements due to
 # vibration and IMU gyro noise. If the IMU cannot be moved and velocity noise is a problem, a location
 # closer to the IMU can be used as the body frame origin.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-INS_POS2_Y,0  # was -0.01
+INS_POS2_Y,0 # was -0.01
 
 # Land alt low
 # Altitude during Landing at which vehicle slows to LAND_SPEED
 # Units: cm (centimeters)
 # Range: 100 10000
 # Increment: 10
 # Default: 1000
-LAND_ALT_LOW,200  # come down fast and only slow down close to the ground. We have a good GNSS receiver, so thrust it
+LAND_ALT_LOW,200 # come down fast and only slow down close to the ground. We have a good GNSS receiver, so thrust it
 
 # RTL Altitude
 # The minimum alt above home the vehicle will climb to before returning.  If the vehicle is flying higher
 # than this value it will return at its current altitude.
 # Units: cm (centimeters)
-# Range: 200 300000
+# Range: 30 300000
 # Increment: 1
 # Default: 1500
-RTL_ALT,300  # The default is too high for the kind of flights we do. This reduces the altitude for indoors
+RTL_ALT,300 # The default is too high for the kind of flights we do. This reduces the altitude for indoors
 
 # RTL loiter time
 # Time (in milliseconds) to loiter above home before beginning final descent
 # Units: ms (milliseconds)
 # Range: 0 60000
 # Increment: 1000
 # Default: 5000
-RTL_LOIT_TIME,1000  # The default is too long. This reduces the time
+RTL_LOIT_TIME,1000 # The default is too long. This reduces the time
 
 # Scheduling main loop rate
 # This controls the rate of the main control loop in Hz. This should only be changed by developers. This
 # only takes effect on restart. Values over 400 are considered highly experimental.
 # RebootRequired: True
 # 50: 50Hz
 # 100: 100Hz
 # 200: 200Hz
 # 250: 250Hz
 # 300: 300Hz
 # 400: 400Hz
 # Default: 400
-SCHED_LOOP_RATE,800  # On our vehicle the propellers rotate at speeds higher than 400Hz and we have a powerful STM32 H7 family processor. So we increase this for added performance.
+SCHED_LOOP_RATE,800 # On our vehicle the propellers rotate at speeds higher than 400Hz and we have a powerful STM32 H7 family processor. So we increase this for added performance.
 
 # Enable Scripting
 # Controls if scripting is enabled
 # RebootRequired: True
 # 0: None
 # 1: Lua Scripts
 # Default: 0
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_logging.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_pid_adjustment.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_remote_id.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_remote_id.param`

 * *Files 12% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 # 4: Serial4
 # 5: Serial5
 # 6: Serial6
 DID_MAVPORT,2  # The serial port attached to the OpenDroneID module
 
 # OpenDroneID options
 # Options for OpenDroneID subsystem
-# Bitmask: 0:EnforceArming, 1:AllowNonGPSPosition
+# Bitmask: 0:EnforceArming, 1:AllowNonGPSPosition, 2:LockUASIDOnFirstBasicIDRx
 DID_OPTIONS,0
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_notch_filter_setup.param`

 * *Files 9% similar despite different names*

```diff
@@ -37,53 +37,53 @@
 # Harmonic Notch Filter enable
 # 0: Disabled
 # 1: Enabled
 # Default: 0
 INS_HNTCH_ENABLE,1  # the first notch filter will be used to filter the noise created by the motors/propellers
 
 # Harmonic Notch Filter base frequency
-# Harmonic Notch Filter base center frequency in Hz. This should be set at most half the backend gyro rate
-# (which is typically 1Khz). For helicopters using RPM sensor to dynamically set the notch frequency, use
-# this parameter to provide a lower limit to the dynamic notch filter.  Recommend setting it to half the
-# operating rotor speed in Hz.
+# Harmonic Notch Filter base center frequency in Hz. This is the center frequency for static notches, the
+# center frequency for Throttle based notches at the reference thrust value, and the minimum limit of
+# center frequency variation for all other notch types. This should always be set lower than half the
+# backend gyro rate (which is typically 1Khz).
 # Range: 10 495
 # Units: Hz (hertz)
 # Default: 80
 INS_HNTCH_FREQ,160  # Start with 1.4 • INS_GYRO_FILTER
 
 # Harmonic Notch Filter harmonics
 # Bitmask of harmonic frequencies to apply Harmonic Notch Filter to. This option takes effect on the next
 # reboot. A value of 0 disables this filter. The first harmonic refers to the base frequency.
-# Bitmask: 0:1st harmonic,1:2nd harmonic,2:3rd harmonic,3:4th hamronic,4:5th harmonic,5:6th harmonic,6:7th harmonic,7:8th harmonic
+# Bitmask: 0:  1st harmonic, 1:  2nd harmonic, 2:  3rd harmonic, 3:  4th harmonic, 4:  5th harmonic, 5:  6th harmonic, 6:  7th harmonic, 7:  8th harmonic, 8:  9th harmonic, 9:  10th harmonic, 10: 11th harmonic, 11: 12th harmonic, 12: 13th harmonic, 13: 14th harmonic, 14: 15th harmonic, 15: 16th harmonic
 # RebootRequired: True
 # Default: 1
 INS_HNTCH_HMNCS,1  # start with a single frequency
 
 # Harmonic Notch Filter dynamic frequency tracking mode
 # Harmonic Notch Filter dynamic frequency tracking mode. Dynamic updates can be throttle, RPM sensor, ESC
 # telemetry or dynamic FFT based. Throttle-based updates should only be used with multicopters.
-# Range: 0 4
-# 0: Disabled
+# Range: 0 5
+# 0: Fixed
 # 1: Throttle
 # 2: RPM Sensor
 # 3: ESC Telemetry
 # 4: Dynamic FFT
 # 5: Second RPM Sensor
 # Default: 1
 INS_HNTCH_MODE,3  # Use the BDshot600 RPM telemetry to dynamicaly track noise created by the motors/propellers
 
 # Harmonic Notch Filter options
 # Harmonic Notch Filter options. Triple and double-notches can provide deeper attenuation across a wider
-# bandwidth with reduced latency than single notches and are suitable for larger aircraft. Dynamic
-# harmonics attaches a harmonic notch to each detected noise frequency instead of simply being multiples of
-# the base frequency, in the case of FFT it will attach notches to each of three detected noise peaks, in
-# the case of ESC it will attach notches to each of four motor RPM values. Loop rate update changes the
-# notch center frequency at the scheduler loop rate rather than at the default of 200Hz. If both double and
-# triple notches are specified only double notches will take effect.
-# Bitmask: 0:Double notch,1:Dynamic harmonic,2:Update at loop rate,3:EnableOnAllIMUs,4:Triple notch
+# bandwidth with reduced latency than single notches and are suitable for larger aircraft. Multi-Source
+# attaches a harmonic notch to each detected noise frequency instead of simply being multiples of the base
+# frequency, in the case of FFT it will attach notches to each of three detected noise peaks, in the case
+# of ESC it will attach notches to each of four motor RPM values. Loop rate update changes the notch center
+# frequency at the scheduler loop rate rather than at the default of 200Hz. If both double and triple
+# notches are specified only double notches will take effect.
+# Bitmask: 0:Double notch,1:Multi-Source,2:Update at loop rate,3:EnableOnAllIMUs,4:Triple notch, 5:Use min freq on RPM failure
 # RebootRequired: True
 # Default: 0
 INS_HNTCH_OPTS,6  # One Notch per motor, update at loop rate
 
 # Harmonic Notch Filter reference value
 # A reference value of zero disables dynamic updates on the Harmonic Notch Filter and a positive value
 # enables dynamic updates on the Harmonic Notch Filter.  For throttle-based scaling, this parameter is the
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_results.param`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # Harmonic Notch Filter attenuation
 # Harmonic Notch Filter attenuation in dB. Values greater than 40dB will typically produce a hard notch
 # rather than a modest attenuation of motor noise.
 # Range: 5 50
 # Units: dB (decibel)
 # Default: 40
-INS_HNTCH_ATT,30  # just enough to filter the noise created by the motors/propellers
+INS_HNTCH_ATT,30 # just enough to filter the noise created by the motors/propellers
 
 # Harmonic Notch Filter bandwidth
 # Harmonic Notch Filter bandwidth in Hz. This is typically set to half the base frequency. The ratio of
 # base frequency to bandwidth determines the notch quality factor and is fixed across harmonics.
 # Range: 5 250
 # Units: Hz (hertz)
 # Default: 40
-INS_HNTCH_BW,30  # just enough to filter the noise created by the motors/propellers
+INS_HNTCH_BW,30 # just enough to filter the noise created by the motors/propellers
 
 # Throttle notch min freqency ratio
 # The minimum ratio below the configured frequency to take throttle based notch filters when flying at a
 # throttle level below the reference throttle. Note that lower frequency notch filters will have more phase
 # lag. If you want throttle based notch filtering to be effective at a throttle up to 30% below the
 # configured notch frequency then set this parameter to 0.7. The default of 1.0 means the notch will not go
 # below the frequency in the FREQ parameter.
 # Range: 0.1 1.0
 # Default: 1
 INS_HNTCH_FM_RAT,1  # Allowed undercutting of the base frequency of the first notch filter
 
 # Harmonic Notch Filter base frequency
-# Harmonic Notch Filter base center frequency in Hz. This should be set at most half the backend gyro rate
-# (which is typically 1Khz). For helicopters using RPM sensor to dynamically set the notch frequency, use
-# this parameter to provide a lower limit to the dynamic notch filter.  Recommend setting it to half the
-# operating rotor speed in Hz.
+# Harmonic Notch Filter base center frequency in Hz. This is the center frequency for static notches, the
+# center frequency for Throttle based notches at the reference thrust value, and the minimum limit of
+# center frequency variation for all other notch types. This should always be set lower than half the
+# backend gyro rate (which is typically 1Khz).
 # Range: 10 495
 # Units: Hz (hertz)
 # Default: 80
 INS_HNTCH_FREQ,180  # the minimum frequency that the motors are expected to operate at
 
 # Harmonic Notch Filter harmonics
 # Bitmask of harmonic frequencies to apply Harmonic Notch Filter to. This option takes effect on the next
 # reboot. A value of 0 disables this filter. The first harmonic refers to the base frequency.
-# Bitmask: 0:1st harmonic,1:2nd harmonic,2:3rd harmonic,3:4th hamronic,4:5th harmonic,5:6th harmonic,6:7th harmonic,7:8th harmonic
+# Bitmask: 0:  1st harmonic, 1:  2nd harmonic, 2:  3rd harmonic, 3:  4th harmonic, 4:  5th harmonic, 5:  6th harmonic, 6:  7th harmonic, 7:  8th harmonic, 8:  9th harmonic, 9:  10th harmonic, 10: 11th harmonic, 11: 12th harmonic, 12: 13th harmonic, 13: 14th harmonic, 14: 15th harmonic, 15: 16th harmonic
 # RebootRequired: True
 # Default: 1
 INS_HNTCH_HMNCS,3  # the motors produce secondary harmonics on this vehicle
 
 # Harmonic Notch Filter options
 # Harmonic Notch Filter options. Triple and double-notches can provide deeper attenuation across a wider
-# bandwidth with reduced latency than single notches and are suitable for larger aircraft. Dynamic
-# harmonics attaches a harmonic notch to each detected noise frequency instead of simply being multiples of
-# the base frequency, in the case of FFT it will attach notches to each of three detected noise peaks, in
-# the case of ESC it will attach notches to each of four motor RPM values. Loop rate update changes the
-# notch center frequency at the scheduler loop rate rather than at the default of 200Hz. If both double and
-# triple notches are specified only double notches will take effect.
-# Bitmask: 0:Double notch,1:Dynamic harmonic,2:Update at loop rate,3:EnableOnAllIMUs,4:Triple notch
+# bandwidth with reduced latency than single notches and are suitable for larger aircraft. Multi-Source
+# attaches a harmonic notch to each detected noise frequency instead of simply being multiples of the base
+# frequency, in the case of FFT it will attach notches to each of three detected noise peaks, in the case
+# of ESC it will attach notches to each of four motor RPM values. Loop rate update changes the notch center
+# frequency at the scheduler loop rate rather than at the default of 200Hz. If both double and triple
+# notches are specified only double notches will take effect.
+# Bitmask: 0:Double notch,1:Multi-Source,2:Update at loop rate,3:EnableOnAllIMUs,4:Triple notch, 5:Use min freq on RPM failure
 # RebootRequired: True
 # Default: 0
 INS_HNTCH_OPTS,6  # One Notch per motor, update at loop rate
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_throttle_controller.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_throttle_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_inflight_magnetometer_fit_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param`

 * *Files 8% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 # Roll axis rate controller I gain.  Corrects long-term difference in desired roll rate vs actual roll rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
 ATC_RAT_RLL_I,0.2908089
 
 # Roll axis rate controller P gain
-# Roll axis rate controller P gain.  Converts the difference between desired roll rate and actual roll rate
-# into a motor speed output
+# Roll axis rate controller P gain.  Corrects in proportion to the difference between the desired roll rate
+# vs actual roll rate
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
 ATC_RAT_RLL_P,0.2908089
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param`

 * *Files 8% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 # rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
 ATC_RAT_PIT_I,0.5622395
 
 # Pitch axis rate controller P gain
-# Pitch axis rate controller P gain.  Converts the difference between desired pitch rate and actual pitch
-# rate into a motor speed output
+# Pitch axis rate controller P gain.  Corrects in proportion to the difference between the desired pitch
+# rate vs actual pitch rate
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
 ATC_RAT_PIT_P,0.5622395
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_yaw_results.param`

 * *Files 4% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 # Increment: 1000
 # 0: Disabled
 # 9000: VerySlow
 # 18000: Slow
 # 36000: Medium
 # 54000: Fast
 # Default: 27000
-ATC_ACCEL_Y_MAX,57198.53
+ATC_ACCEL_Y_MAX,206781.046875
 
 # Yaw axis angle controller P gain
 # Yaw axis angle controller P gain.  Converts the error between the desired yaw angle and actual angle to a
 # desired yaw rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_YAW_P,8.714352 # higher value mean a tighter tune
+ATC_ANG_YAW_P,25.796528  # higher value mean a tighter tune
 
 # Yaw axis rate controller error frequency in Hz
 # Yaw axis rate controller error frequency in Hz
 # Range: 5 50
 # Increment: 1
 # Units: Hz (hertz)
 # Default: 2.5
-ATC_RAT_YAW_FLTE,2.316456
+ATC_RAT_YAW_FLTE,1.986072
 
 # Yaw axis rate controller I gain
 # Yaw axis rate controller I gain.  Corrects long-term difference in desired yaw rate vs actual yaw rate
 # Range: 0.01 0.2
 # Increment: 0.01
 # Default: 0.018
-ATC_RAT_YAW_I,0.1023194
+ATC_RAT_YAW_I,0.073779
 
 # Yaw axis rate controller P gain
 # Yaw axis rate controller P gain.  Converts the difference between desired yaw rate and actual yaw rate
 # into a motor speed output
 # Range: 0.180 0.60
 # Increment: 0.005
 # Default: 0.18
-ATC_RAT_YAW_P,1.023194
+ATC_RAT_YAW_P,0.737788
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param`

 * *Files 3% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 # Yaw axis rate controller I gain.  Corrects long-term difference in desired yaw rate vs actual yaw rate
 # Range: 0.01 0.2
 # Increment: 0.01
 # Default: 0.018
 ATC_RAT_YAW_I,0.09050494
 
 # Yaw axis rate controller P gain
-# Yaw axis rate controller P gain.  Converts the difference between desired yaw rate and actual yaw rate
-# into a motor speed output
+# Yaw axis rate controller P gain.  Corrects in proportion to the difference between the desired yaw rate
+# vs actual yaw rate
 # Range: 0.180 0.60
 # Increment: 0.005
 # Default: 0.18
 ATC_RAT_YAW_P,0.9050494
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_roll_pitch_retune_results.param`

 * *Files 10% similar despite different names*

```diff
@@ -5,82 +5,82 @@
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_P_MAX,339368.9
+ATC_ACCEL_P_MAX,363812.1875  # Autotuned in a windless hangar
 
 # Acceleration Max for Roll
 # Maximum acceleration in roll axis
 # Units: cdeg/s/s (centidegrees per square second)
 # Range: 0 180000
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_R_MAX,490096.8
+ATC_ACCEL_R_MAX,495292.5625  # Autotuned in a windless hangar
 
 # Pitch axis angle controller P gain
 # Pitch axis angle controller P gain.  Converts the error between the desired pitch angle and actual angle
 # to a desired pitch rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_PIT_P,31.19081 # higher value mean a tighter tune
+ATC_ANG_PIT_P,36  # higher value mean a tighter tune
 
 # Roll axis angle controller P gain
 # Roll axis angle controller P gain.  Converts the error between the desired roll angle and actual angle to
 # a desired roll rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_RLL_P,36 # higher value mean a tighter tune
+ATC_ANG_RLL_P,36  # higher value mean a tighter tune
 
 # Pitch axis rate controller D gain
 # Pitch axis rate controller D gain.  Compensates for short-term change in desired pitch rate vs actual
 # pitch rate
 # Range: 0.0 0.03
 # Increment: 0.001
 # Default: 0.0036
-ATC_RAT_PIT_D,0.006667002
+ATC_RAT_PIT_D,0.003774  # Autotuned in a windless hangar
 
 # Pitch axis rate controller I gain
 # Pitch axis rate controller I gain.  Corrects long-term difference in desired pitch rate vs actual pitch
 # rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_PIT_I,0.3464575
+ATC_RAT_PIT_I,0.193122  # Autotuned in a windless hangar
 
 # Pitch axis rate controller P gain
 # Pitch axis rate controller P gain.  Converts the difference between desired pitch rate and actual pitch
 # rate into a motor speed output
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
-ATC_RAT_PIT_P,0.3464575
+ATC_RAT_PIT_P,0.193122  # Autotuned in a windless hangar
 
 # Roll axis rate controller D gain
 # Roll axis rate controller D gain.  Compensates for short-term change in desired roll rate vs actual roll
 # rate
 # Range: 0.0 0.03
 # Increment: 0.001
 # Default: 0.0036
-ATC_RAT_RLL_D,0.004972266
+ATC_RAT_RLL_D,0.00242  # Autotuned in a windless hangar
 
 # Roll axis rate controller I gain
 # Roll axis rate controller I gain.  Corrects long-term difference in desired roll rate vs actual roll rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_RLL_I,0.286474
+ATC_RAT_RLL_I,0.12357  # Autotuned in a windless hangar
 
 # Roll axis rate controller P gain
 # Roll axis rate controller P gain.  Converts the difference between desired roll rate and actual roll rate
 # into a motor speed output
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
-ATC_RAT_RLL_P,0.286474
+ATC_RAT_RLL_P,0.12357  # Autotuned in a windless hangar
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_windspeed_estimation.param`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # wind drift for vehicles with bluff bodies and without propulsion forces in the X and Y direction (eg
 # multicopters). The drag produced by this effect scales with speed squared.  Set to a postive value > 1.0
 # to enable. A starting value is the mass in Kg divided by the frontal area. The predicted drag from the
 # rotors is specified separately by the EK3_DRAG_MCOEF parameter.
 # Range: 0.0 1000.0
 # Units: kg/m/m (kilograms per square meter)
 # Default: 0
-EK3_DRAG_BCOEF_X,51.0399  # 0.56 kg / 0.01097 m²
+EK3_DRAG_BCOEF_X,54.6857  # 0.600 kg / 0.01097 m²
 
 # Ballistic coefficient for Y axis drag
 # Ratio of mass to drag coefficient measured along the Y body axis. This parameter enables estimation of
 # wind drift for vehicles with bluff bodies and without propulsion forces in the X and Y direction (eg
 # multicopters). The drag produced by this effect scales with speed squared.  Set to a postive value > 1.0
 # to enable. A starting value is the mass in Kg divided by the side area. The predicted drag from the
 # rotors is specified separately by the EK3_DRAG_MCOEF parameter.
 # Range: 50.0 1000.0
 # Units: kg/m/m (kilograms per square meter)
 # Default: 0
-EK3_DRAG_BCOEF_Y,38.4798  # 0.56 kg / 0.01455 m²
+EK3_DRAG_BCOEF_Y,41.2284  # 0.600 kg / 0.01455 m²
 
 # Momentum coefficient for propeller drag
 # This parameter is used to predict the drag produced by the rotors when flying a multi-copter, enabling
 # estimation of wind drift. The drag produced by this effect scales with speed not speed squared and is
 # produced because some of the air velocity normal to the rotors axis of rotation is lost when passing
 # through the rotor disc which changes the momentum of the airflow causing drag. For unducted rotors the
 # effect is roughly proportional to the area of the propeller blades when viewed side on and changes with
@@ -31,25 +31,25 @@
 # 0.1 = (1.5/15.0). Set EK3_MCOEF to a postive value to enable wind estimation using this drag effect. To
 # account for the drag produced by the body which scales with speed squared, see documentation for the
 # EK3_DRAG_BCOEF_X and EK3_DRAG_BCOEF_Y parameters.
 # Range: 0.0 1.0
 # Increment: 0.01
 # Units: 1/s (per second)
 # Default: 0
-EK3_DRAG_MCOEF,0.5127
+EK3_DRAG_MCOEF,0.5195
 
 # Enable logging while disarmed
 # If LOG_DISARMED is set to 1 then logging will be enabled while disarmed. This can make for very large
 # logfiles but can help a lot when tracking down startup issues
 # 0: Disabled
 # 1: Enabled
 # Default: 0
-LOG_DISARMED,1 # allow post flight tuning with Replay
+LOG_DISARMED,1  # allow post flight tuning with Replay
 
 # Enable logging of information needed for Replay
 # If LOG_REPLAY is set to 1 then the EKF2 state estimator will log detailed information needed for
 # diagnosing problems with the Kalman filter. It is suggested that you also raise LOG_FILE_BUFSIZE to give
 # more buffer space for logging and use a high quality microSD card to ensure no sensor data is lost
 # 0: Disabled
 # 1: Enabled
 # Default: 0
-LOG_REPLAY,1 # allow post flight tuning with Replay
+LOG_REPLAY,1  # allow post flight tuning with Replay
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_barometer_compensation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_system_id_roll.param`

 * *Files 10% similar despite different names*

```diff
@@ -16,51 +16,63 @@
 ARMING_CHECK,540126  # disable Parameter check because we need to set ATC_RAT_RLL_I out-of-range (was 30175)
 
 # Roll axis rate controller I gain
 # Roll axis rate controller I gain.  Corrects long-term difference in desired roll rate vs actual roll rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_RLL_I,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
+ATC_RAT_RLL_I,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
 
 # Rate Feedforward Enable
 # Controls whether body-frame rate feedfoward is enabled or disabled
 # 0: Disabled
 # 1: Enabled
 # Default: 1
-ATC_RATE_FF_ENAB,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
+ATC_RATE_FF_ENAB,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
+
+# Flight Mode 5
+# Flight mode when pwm of Flightmode channel(FLTMODE_CH) is >1620, <= 1749
+# 0: Stabilize               7: Circle                  17: Brake                  24: ZigZag
+# 1: Acro                    9: Land                    18: Throw                  25: SystemID
+# 2: AltHold                 11: Drift                  19: Avoid_ADSB             26: Heli_Autorotate
+# 3: Auto                    13: Sport                  20: Guided_NoGPS           27: Auto RTL
+# 4: Guided                  14: Flip                   21: Smart_RTL
+# 5: Loiter                  15: AutoTune               22: FlowHold
+# 6: RTL                     16: PosHold                23: Follow
+# Default: 0
+FLTMODE5,25
 
 # Enable logging while disarmed
 # If LOG_DISARMED is set to 1 then logging will be enabled while disarmed. This can make for very large
 # logfiles but can help a lot when tracking down startup issues
 # 0: Disabled
 # 1: Enabled
 # Default: 0
-LOG_DISARMED,0 # was only needed for wind speed estimation
+LOG_DISARMED,0  # was only needed for wind speed estimation
 
 # Enable logging of information needed for Replay
 # If LOG_REPLAY is set to 1 then the EKF2 state estimator will log detailed information needed for
 # diagnosing problems with the Kalman filter. It is suggested that you also raise LOG_FILE_BUFSIZE to give
 # more buffer space for logging and use a high quality microSD card to ensure no sensor data is lost
 # 0: Disabled
 # 1: Enabled
 # Default: 0
-LOG_REPLAY,0 # was only needed for wind speed estimation
+LOG_REPLAY,0  # was only needed for wind speed estimation
 
 # System identification axis
 # Controls which axis are being excited.  Set to non-zero to see more parameters
 # 0: None                                              7: Rate Roll
 # 1: Input Roll Angle                                  8: Rate Pitch
 # 2: Input Pitch Angle                                 9: Rate Yaw
 # 3: Input Yaw Angle                                   10: Mixer Roll
 # 4: Recovery Roll Angle                               11: Mixer Pitch
 # 5: Recovery Pitch Angle                              12: Mixer Yaw
 # 6: Recovery Yaw Angle                                13: Mixer Thrust
 # Default: 0
-SID_AXIS,10
+SID_AXIS,10  # Inject chip on the mixer roll signal
 
 # System identification Start Frequency
 # Frequency at the start of the sweep
 # Range: 0.01 100
 # Units: Hz (hertz)
 SID_F_START_HZ,0.05
 
@@ -103,20 +115,20 @@
 # 6: Rate Yaw kP                      10: WP Speed                        51: Rate Roll kD
 # 26: Rate Yaw kD                     25: Acro Roll/Pitch deg/s           52: Rate Pitch FF
 # 56: Rate Yaw Filter                 40: Acro Yaw deg/s                  53: Rate Roll FF
 # 55: Motor Yaw Headroom              45: RC Feel                         54: Rate Yaw FF
 # 14: AltHold kP                      13: Heli Ext Gyro                   58: SysID Magnitude
 # 7: Throttle Rate kP                 38: Declination
 # Default: 0
-TUNE,58  # System identification magnitude
+TUNE,0  # System identification magnitude
 
 # Tuning maximum
 # Maximum value that the parameter currently being tuned with the transmitter's channel 6 knob will be set
 # to
 # Default: 0
-TUNE_MAX,0.40  # System identification max magnitude
+TUNE_MAX,0.4  # System identification max magnitude
 
 # Tuning minimum
 # Minimum value that the parameter currently being tuned with the transmitter's channel 6 knob will be set
 # to
 # Default: 0
 TUNE_MIN,0.02  # System identification min magnitude
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_system_id_pitch.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_yaw.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_thrust.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # whatever checks you prefer by adding together the values of each check type to set this parameter. For
 # example, to only allow arming when you have GPS lock and no RC failsafe you would set ARMING_CHECK to 72.
 # Bitmask: 0:All,1:Barometer,2:Compass,3:GPS lock,4:INS,5:Parameters,6:RC Channels,7:Board voltage,8:Battery Level,10:Logging Available,11:Hardware safety switch,12:GPS Configuration,13:System,14:Mission,15:Rangefinder,16:Camera,17:AuxAuth,18:VisualOdometry,19:FFT
 # Default: 1
 ARMING_CHECK,0  # normal state for every day use
 
 # Rate Feedforward Enable
-# Controls whether body-frame rate feedfoward is enabled or disabled
+# Controls whether body-frame rate feedforward is enabled or disabled
 # 0: Disabled
 # 1: Enabled
 # Default: 1
 ATC_RATE_FF_ENAB,1  # restore value now that system identification is done
 
 # Acceleration (vertical) controller I gain
 # Acceleration (vertical) controller I gain.  Corrects long-term difference in desired vertical
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param`

 * *Files 6% similar despite different names*

```diff
@@ -280,29 +280,14 @@
 # 2: RCChannelPwmValue
 # 3: ReceiverProtocol
 # 4: PWMInputPin
 # 5: TelemetryRadioRSSI
 # Default: 0
 RSSI_TYPE,3 # TBS Crossfire protocol provides RSSI
 
-# Telemetry 2 Baud Rate
-# The baud rate of the Telem2 port. Most stm32-based boards can support rates of up to 1500. If you setup a
-# rate you cannot support and then can't connect to your board you should load a firmware from a different
-# vehicle type. That will reset all your parameters to defaults.
-# 1: 1200                                              115: 115200
-# 2: 2400                                              230: 230400
-# 4: 4800                                              256: 256000
-# 9: 9600                                              460: 460800
-# 19: 19200                                            500: 500000
-# 38: 38400                                            921: 921600
-# 57: 57600                                            1500: 1500000
-# 111: 111100                                          2000: 2000000
-# Default: 57
-SERIAL2_BAUD,115 # For Mavlink over crossfire
-
 # Serial7 protocol selection
 # Control what protocol Serial7 port should be used for. Note that the Frsky options require external
 # converter hardware. See the wiki for details.
 # RebootRequired: True
 # -1: None                                             24: EFI Serial
 # 1: MAVLink1                                          25: LTM
 # 2: MAVLink2                                          26: RunCam
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # Increment: 50
 # Default: 3300
 BATT_CAPACITY,1800
 
 # Battery critical capacity
 # Battery capacity at which the critical battery failsafe is triggered. Set to 0 to disable battery
 # remaining failsafe. If the battery capacity drops below this level the vehicle will perform the failsafe
-# specified by the BATT__FS_CRT_ACT parameter.
+# specified by the BATT_FS_CRT_ACT parameter.
 # Units: mAh (milliampere hour)
 # Increment: 50
 # Default: 0
 BATT_CRT_MAH,450
 
 # Critical battery voltage
 # Battery voltage that triggers a critical battery failsafe. Set to 0 to disable. If the battery voltage
@@ -86,27 +86,28 @@
 # Increment: 0.1
 # Default: 10.5
 BATT_LOW_VOLT,14.4
 
 # Battery monitoring
 # Controls enabling monitoring of the battery's voltage and current
 # RebootRequired: True
-# 0: Disabled                                          15: NeoDesign
-# 3: Analog Voltage Only                               16: SMBus-Maxell
-# 4: Analog Voltage and Current                        17: Generator-Elec
-# 5: Solo                                              18: Generator-Fuel
-# 6: Bebop                                             19: Rotoye
-# 7: SMBus-Generic                                     20: MPPT
-# 8: DroneCAN-BatteryInfo                              21: INA2XX
-# 9: ESC                                               22: LTC2946
-# 10: Sum Of Selected Monitors                         23: Torqeedo
-# 11: FuelFlow                                         24: FuelLevelAnalog
-# 12: FuelLevelPWM                                     25: Synthetic Current and Analog Voltage
-# 13: SMBUS-SUI3                                       26: INA239_SPI
-# 14: SMBUS-SUI6                                       27: EFI
+# 0: Disabled                                          16: SMBus-Maxell
+# 3: Analog Voltage Only                               17: Generator-Elec
+# 4: Analog Voltage and Current                        18: Generator-Fuel
+# 5: Solo                                              19: Rotoye
+# 6: Bebop                                             20: MPPT
+# 7: SMBus-Generic                                     21: INA2XX
+# 8: DroneCAN-BatteryInfo                              22: LTC2946
+# 9: ESC                                               23: Torqeedo
+# 10: Sum Of Selected Monitors                         24: FuelLevelAnalog
+# 11: FuelFlow                                         25: Synthetic Current and Analog Voltage
+# 12: FuelLevelPWM                                     26: INA239_SPI
+# 13: SMBUS-SUI3                                       27: EFI
+# 14: SMBUS-SUI6                                       28: AD7091R5
+# 15: NeoDesign                                        29: Scripting
 # Default: 4
 BATT_MONITOR,4
 
 # Voltage Multiplier
 # Used to convert the voltage of the voltage sensing pin (BATT_VOLT_PIN) to the actual battery's voltage
 # (pin_voltage * VOLT_MULT). For the 3DR Power brick with a Pixhawk, this should be set to 10.1. For the
 # Pixhawk with the 3DR 4in1 ESC this should be 12.02. For the PX using the PX4IO power supply this should
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param`

 * *Files 7% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 # Default: 0
 BRD_SAFETY_DEFLT,0  # Matek H743 Slim has no safety switch
 
 # GNSS system configuration
 # Bitmask for what GNSS system to use on the first GPS (all unchecked or zero to leave GPS as configured)
 # Bitmask: 0:GPS,1:SBAS,2:Galileo,3:Beidou,4:IMES,5:QZSS,6:GLONASS
 # Default: 0
-GPS_GNSS_MODE,7 # limit the constalations to ensure an update rate higher than 5Hz
+GPS_GNSS_MODE,7  # limit the constalations to ensure an update rate higher than 5Hz
 
 # Antenna X position offset
 # X position of the first GPS antenna in body frame. Positive X is forward of the origin. Use antenna phase
 # centroid location if provided by the manufacturer.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-GPS_POS1_X,0.056 # HX-CH7604A GNSS antenna pahse center location relative to CG
+GPS_POS1_X,0.056  # HX-CH7604A GNSS antenna pahse center location relative to CG
 
 # Antenna Y position offset
 # Y position of the first GPS antenna in body frame. Positive Y is to the right of the origin. Use antenna
 # phase centroid location if provided by the manufacturer.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-GPS_POS1_Y,0.0 # HX-CH7604A GNSS antenna pahse center location relative to CG
+GPS_POS1_Y,0  # HX-CH7604A GNSS antenna pahse center location relative to CG
 
 # Antenna Z position offset
 # Z position of the first GPS antenna in body frame. Positive Z is down from the origin. Use antenna phase
 # centroid location if provided by the manufacturer.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-GPS_POS1_Z,-0.070 # HX-CH7604A GNSS antenna pahse center location relative to CG
+GPS_POS1_Z,-0.07  # HX-CH7604A GNSS antenna pahse center location relative to CG
 
 # 1st GPS type
 # GPS type of 1st GPS
 # RebootRequired: True
 # 0: None                                              15: NOVA
 # 1: AUTO                                              16: HemisphereNMEA
 # 2: uBlox                                             17: uBlox-MovingBaseline-Base
@@ -53,46 +53,47 @@
 # 6: SiRF                                              19: MSP
 # 7: HIL                                               20: AllyStar
 # 8: SwiftNav                                          21: ExternalAHRS
 # 9: DroneCAN                                          22: DroneCAN-MovingBaseline-Base
 # 10: SBF                                              23: DroneCAN-MovingBaseline-Rover
 # 11: GSOF                                             24: UnicoreNMEA
 # 13: ERB                                              25: UnicoreMovingBaselineNMEA
-# 14: MAV
+# 14: MAV                                              26: SBF-DualAntenna
 # Default: 1
-GPS_TYPE,2
+GPS_TYPE,2  # Defined in component editor
 
-# Serial4 protocol selection
-# Control what protocol Serial4 port should be used for. Note that the Frsky options require external
+# Serial 3 (GPS) protocol selection
+# Control what protocol Serial 3 (GPS) should be used for. Note that the Frsky options require external
 # converter hardware. See the wiki for details.
 # RebootRequired: True
-# -1: None                                             24: EFI Serial
-# 1: MAVLink1                                          25: LTM
-# 2: MAVLink2                                          26: RunCam
-# 3: Frsky D                                           27: HottTelem
-# 4: Frsky SPort                                       28: Scripting
-# 5: GPS                                               29: Crossfire VTX
-# 7: Alexmos Gimbal Serial                             30: Generator
-# 8: Gimbal                                            31: Winch
-# 9: Rangefinder                                       32: MSP
-# 10: FrSky SPort Passthrough (OpenTX)                 33: DJI FPV
-# 11: Lidar360                                         34: AirSpeed
-# 13: Beacon                                           35: ADSB
-# 14: Volz servo out                                   36: AHRS
-# 15: SBus servo out                                   37: SmartAudio
-# 16: ESC Telemetry                                    38: FETtecOneWire
-# 17: Devo Telemetry                                   39: Torqeedo
-# 18: OpticalFlow                                      40: AIS
-# 19: RobotisServo                                     41: CoDevESC
-# 20: NMEA Output                                      42: DisplayPort
-# 21: WindVane                                         43: MAVLink High Latency
-# 22: SLCAN                                            44: IRC Tramp
-# 23: RCIN
+# -1: None                                             25: LTM
+# 1: MAVLink1                                          26: RunCam
+# 2: MAVLink2                                          27: HottTelem
+# 3: Frsky D                                           28: Scripting
+# 4: Frsky SPort                                       29: Crossfire VTX
+# 5: GPS                                               30: Generator
+# 7: Alexmos Gimbal Serial                             31: Winch
+# 8: Gimbal                                            32: MSP
+# 9: Rangefinder                                       33: DJI FPV
+# 10: FrSky SPort Passthrough (OpenTX)                 34: AirSpeed
+# 11: Lidar360                                         35: ADSB
+# 13: Beacon                                           36: AHRS
+# 14: Volz servo out                                   37: SmartAudio
+# 15: SBus servo out                                   38: FETtecOneWire
+# 16: ESC Telemetry                                    39: Torqeedo
+# 17: Devo Telemetry                                   40: AIS
+# 18: OpticalFlow                                      41: CoDevESC
+# 19: RobotisServo                                     42: DisplayPort
+# 20: NMEA Output                                      43: MAVLink High Latency
+# 21: WindVane                                         44: IRC Tramp
+# 22: SLCAN                                            45: DDS XRCE
+# 23: RCIN                                             46: IMUDATA
+# 24: EFI Serial
 # Default: 5
-SERIAL4_PROTOCOL,-1
+SERIAL3_PROTOCOL,5  # GNSS receiver is connected to serial3
 
 # Waypoint Radius
 # Defines the distance from a waypoint, that when crossed indicates the wp has been hit.
 # Units: cm (centimeters)
 # Range: 5 1000
 # Increment: 1
 # Default: 200
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+# Arm Checks to Perform (bitmask)
+# Checks prior to arming motor. This is a bitmask of checks that will be performed before allowing arming.
+# For most users it is recommended to leave this at the default of 1 (all checks enabled). You can select
+# whatever checks you prefer by adding together the values of each check type to set this parameter. For
+# example, to only allow arming when you have GPS lock and no RC failsafe you would set ARMING_CHECK to 72.
+# Bitmask: 0:All,1:Barometer,2:Compass,3:GPS lock,4:INS,5:Parameters,6:RC Channels,7:Board voltage,8:Battery Level,10:Logging Available,11:Hardware safety switch,12:GPS Configuration,13:System,14:Mission,15:Rangefinder,16:Camera,17:AuxAuth,18:VisualOdometry,19:FFT
+# Default: 1
+ARMING_CHECK,1  # perform all arming checks. If you have a problem fix it's source. Do NOT change this
+
 # Timezone offset from UTC
 # Adds offset in +- minutes from UTC to calculate local time
 # Range: -720 +840
 # Default: 0
-BRD_RTC_TZ_MIN,60
+BRD_RTC_TZ_MIN,60  # Berlin time zone
 
 # Fence Type
 # Enabled fence types held as bitmask
-# Bitmask: 0:Max altitude,1:Circle,2:Polygon,3:Min altitude
+# Bitmask: 0:Max altitude,1:Circle Centered on Home,2:Inclusion/Exclusion Circles+Polygons,3:Min altitude
 # Default: 7
-FENCE_TYPE,11
+FENCE_TYPE,7  # cylinder and max altitude, to obey local regulations and safety measures
 
 # Accel filter cutoff frequency
 # Filter cutoff frequency for accelerometers. This can be set to a lower value to try to cope with very
 # high vibration levels in aircraft. A value of zero means no filtering (not recommended!)
 # Units: Hz (hertz)
 # Range: 0 256
 # Default: 20
@@ -106,8 +115,8 @@
 
 # Enable Scripting
 # Controls if scripting is enabled
 # RebootRequired: True
 # 0: None
 # 1: Lua Scripts
 # Default: 0
-SCR_ENABLE,1  # For MagFit automation and Windspeed Estimation automation
+SCR_ENABLE,1  # For VTOL-Quicktune, MagFit automation and Windspeed Estimation automation
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_pid_adjustment.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_autotune_roll_results.param`

 * *Files 6% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_R_MAX,507500
+ATC_ACCEL_R_MAX,523377.3125
 
 # Roll axis angle controller P gain
 # Roll axis angle controller P gain.  Converts the error between the desired roll angle and actual angle to
 # a desired roll rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_RLL_P,36 # higher value mean a tighter tune
+ATC_ANG_RLL_P,36  # higher value mean a tighter tune
 
 # Roll axis rate controller D gain
 # Roll axis rate controller D gain.  Compensates for short-term change in desired roll rate vs actual roll
 # rate
 # Range: 0.0 0.03
 # Increment: 0.001
 # Default: 0.0036
-ATC_RAT_RLL_D,0.005008578
+ATC_RAT_RLL_D,0.002438
 
 # Roll axis rate controller I gain
 # Roll axis rate controller I gain.  Corrects long-term difference in desired roll rate vs actual roll rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_RLL_I,0.2908089
+ATC_RAT_RLL_I,0.125126
 
 # Roll axis rate controller P gain
 # Roll axis rate controller P gain.  Corrects in proportion to the difference between the desired roll rate
 # vs actual roll rate
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
-ATC_RAT_RLL_P,0.2908089
+ATC_RAT_RLL_P,0.125126
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_pitch_results.param`

 * *Files 11% similar despite different names*

```diff
@@ -5,39 +5,39 @@
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_P_MAX,360201.2
+ATC_ACCEL_P_MAX,401666.40625
 
 # Pitch axis angle controller P gain
 # Pitch axis angle controller P gain.  Converts the error between the desired pitch angle and actual angle
 # to a desired pitch rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_PIT_P,28.51195 # higher value mean a tighter tune
+ATC_ANG_PIT_P,34.656452  # higher value mean a tighter tune
 
 # Pitch axis rate controller D gain
 # Pitch axis rate controller D gain.  Compensates for short-term change in desired pitch rate vs actual
 # pitch rate
 # Range: 0.0 0.03
 # Increment: 0.001
 # Default: 0.0036
-ATC_RAT_PIT_D,0.009135851
+ATC_RAT_PIT_D,0.004433
 
 # Pitch axis rate controller I gain
 # Pitch axis rate controller I gain.  Corrects long-term difference in desired pitch rate vs actual pitch
 # rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_PIT_I,0.5622395
+ATC_RAT_PIT_I,0.282138
 
 # Pitch axis rate controller P gain
-# Pitch axis rate controller P gain.  Corrects in proportion to the difference between the desired pitch
-# rate vs actual pitch rate
+# Pitch axis rate controller P gain.  Converts the difference between desired pitch rate and actual pitch
+# rate into a motor speed output
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
-ATC_RAT_PIT_P,0.5622395
+ATC_RAT_PIT_P,0.282138
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_yaw_setup.param`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 # Default: 0
 ATC_RAT_YAW_FLTD,28.75  # INS_GYRO_FILTER / 4
 
 # Autotune aggressiveness
 # Autotune aggressiveness. Defines the bounce back used to detect size of the D term.
 # Range: 0.05 0.10
 # Default: 0.1
-AUTOTUNE_AGGR,0.10 # Use the default for now
+AUTOTUNE_AGGR,0.085  # Use smaller than default value because there is no wind in the Hangar
 
 # Autotune axis bitmask
 # 1-byte bitmap of axes to autotune
 # Bitmask: 0:Roll,1:Pitch,2:Yaw
 # Default: 7
-AUTOTUNE_AXES,4 # Autotune on yaw axis
+AUTOTUNE_AXES,4  # Autotune yaw axis
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_yaw_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_yaw_results.param`

 * *Files 15% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 # Increment: 1000
 # 0: Disabled
 # 9000: VerySlow
 # 18000: Slow
 # 36000: Medium
 # 54000: Fast
 # Default: 27000
-ATC_ACCEL_Y_MAX,91119.27
+ATC_ACCEL_Y_MAX,206781.046875
 
 # Yaw axis angle controller P gain
 # Yaw axis angle controller P gain.  Converts the error between the desired yaw angle and actual angle to a
 # desired yaw rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_YAW_P,14.52818
+ATC_ANG_YAW_P,25.796528  # higher value mean a tighter tune
 
-# Yaw axis rate controller D gain
-# Yaw axis rate controller D gain.  Compensates for short-term change in desired yaw rate vs actual yaw
-# rate
-# Range: 0.000 0.02
-# Increment: 0.001
-# Default: 0
-ATC_RAT_YAW_D,0.003507904 # if == to AUTOTUNE_MIN_D, autotune failed
+# Yaw axis rate controller error frequency in Hz
+# Yaw axis rate controller error frequency in Hz
+# Range: 5 50
+# Increment: 1
+# Units: Hz (hertz)
+# Default: 2.5
+ATC_RAT_YAW_FLTE,1.986072
 
 # Yaw axis rate controller I gain
 # Yaw axis rate controller I gain.  Corrects long-term difference in desired yaw rate vs actual yaw rate
 # Range: 0.01 0.2
 # Increment: 0.01
 # Default: 0.018
-ATC_RAT_YAW_I,0.09050494
+ATC_RAT_YAW_I,0.073779
 
 # Yaw axis rate controller P gain
 # Yaw axis rate controller P gain.  Corrects in proportion to the difference between the desired yaw rate
 # vs actual yaw rate
 # Range: 0.180 0.60
 # Increment: 0.005
 # Default: 0.18
-ATC_RAT_YAW_P,0.9050494
+ATC_RAT_YAW_P,0.737788
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_barometer_compensation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # Roll axis rate controller I gain.  Corrects long-term difference in desired roll rate vs actual roll rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
 ATC_RAT_RLL_I,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
 
 # Rate Feedforward Enable
-# Controls whether body-frame rate feedfoward is enabled or disabled
+# Controls whether body-frame rate feedforward is enabled or disabled
 # 0: Disabled
 # 1: Enabled
 # Default: 1
 ATC_RATE_FF_ENAB,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
 
 # Enable logging while disarmed
 # If LOG_DISARMED is set to 1 then logging will be enabled at all times including when disarmed. Logging
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_system_id_pitch.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_yaw.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_thrust.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_analytical_pid_optimization.param`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Arm Checks to Perform (bitmask)
 # Checks prior to arming motor. This is a bitmask of checks that will be performed before allowing arming.
 # For most users it is recommended to leave this at the default of 1 (all checks enabled). You can select
 # whatever checks you prefer by adding together the values of each check type to set this parameter. For
 # example, to only allow arming when you have GPS lock and no RC failsafe you would set ARMING_CHECK to 72.
 # Bitmask: 0:All,1:Barometer,2:Compass,3:GPS lock,4:INS,5:Parameters,6:RC Channels,7:Board voltage,8:Battery Level,10:Logging Available,11:Hardware safety switch,12:GPS Configuration,13:System,14:Mission,15:Rangefinder,16:Camera,17:AuxAuth,18:VisualOdometry,19:FFT
 # Default: 1
-ARMING_CHECK,0  # normal state for every day use
+ARMING_CHECK,1  # Normal state for everyday use
 
 # Rate Feedforward Enable
 # Controls whether body-frame rate feedfoward is enabled or disabled
 # 0: Disabled
 # 1: Enabled
 # Default: 1
-ATC_RATE_FF_ENAB,1  # restore value now that system identification is done
+ATC_RATE_FF_ENAB,1  # Restore value now that system identification is done
 
 # Acceleration (vertical) controller I gain
 # Acceleration (vertical) controller I gain.  Corrects long-term difference in desired vertical
 # acceleration and actual acceleration
 # Range: 0.000 3.000
 # Default: 1
 PSC_ACCZ_I,0.816  # now that system identification on thrust has been completed, restore it to 2 • MOT_THST_HOVER
@@ -27,8 +27,8 @@
 # 1: Input Roll Angle                                  8: Rate Pitch
 # 2: Input Pitch Angle                                 9: Rate Yaw
 # 3: Input Yaw Angle                                   10: Mixer Roll
 # 4: Recovery Roll Angle                               11: Mixer Pitch
 # 5: Recovery Pitch Angle                              12: Mixer Yaw
 # 6: Recovery Yaw Angle                                13: Mixer Thrust
 # Default: 0
-SID_AXIS,0
+SID_AXIS,0  # No more system identification chip injections
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_everyday_use.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # Default: 176126
 LOG_BITMASK,2241500 # 2:GPS,3:System Performance,4:Control Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,12:PID,13:Compass,17:Motors,21:Fast harmonic notch logging
 
 # RTL Altitude
 # The minimum alt above home the vehicle will climb to before returning.  If the vehicle is flying higher
 # than this value it will return at its current altitude.
 # Units: cm (centimeters)
-# Range: 200 300000
+# Range: 30 300000
 # Increment: 1
 # Default: 1500
 RTL_ALT,500  # The default is too high for the kind of flights we do. This reduces the altitude for outdoors
 
 # RTL minimum climb
 # The vehicle will climb this many cm during the initial climb portion of the RTL
 # Units: cm (centimeters)
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 # 6: SiRF                                              19: MSP
 # 7: HIL                                               20: AllyStar
 # 8: SwiftNav                                          21: ExternalAHRS
 # 9: DroneCAN                                          22: DroneCAN-MovingBaseline-Base
 # 10: SBF                                              23: DroneCAN-MovingBaseline-Rover
 # 11: GSOF                                             24: UnicoreNMEA
 # 13: ERB                                              25: UnicoreMovingBaselineNMEA
-# 14: MAV                                              26: SBF-DualAntenna
+# 14: MAV
 # Default: 1
 GPS_TYPE,2  # Defined in component editor
 
 # Serial 3 (GPS) protocol selection
 # Control what protocol Serial 3 (GPS) should be used for. Note that the Frsky options require external
 # converter hardware. See the wiki for details.
 # RebootRequired: True
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/11_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_general_configuration.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_general_configuration.param`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Adds offset in +- minutes from UTC to calculate local time
 # Range: -720 +840
 # Default: 0
 BRD_RTC_TZ_MIN,60  # Berlin time zone
 
 # Fence Type
 # Enabled fence types held as bitmask
-# Bitmask: 0:Max altitude,1:Circle Centered on Home,2:Inclusion/Exclusion Circles+Polygons,3:Min altitude
+# Bitmask: 0:Max altitude,1:Circle,2:Polygon,3:Min altitude
 # Default: 7
 FENCE_TYPE,7  # cylinder and max altitude, to obey local regulations and safety measures
 
 # Accel filter cutoff frequency
 # Filter cutoff frequency for accelerometers. This can be set to a lower value to try to cope with very
 # high vibration levels in aircraft. A value of zero means no filtering (not recommended!)
 # Units: Hz (hertz)
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_logging.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_pid_adjustment.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_notch_filter_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_quick_tune_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_quick_tune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_inflight_magnetometer_fit_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_inflight_magnetometer_fit_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_quick_tune_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_quick_tune_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_quick_tune_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_quick_tune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_autotune_roll_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_pitch_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_yaw_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_yaw_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yawd_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yawd_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yawd_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yawd_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_windspeed_estimation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_barometer_compensation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_system_id_roll.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_system_id_pitch.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_yaw.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_thrust.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_analytical_pid_optimization.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_guided_operation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # Sensor Bitmask
 # Bitmap of which IMUs to log batch data for. This option takes effect on the next reboot.
 # Bitmask: 0:IMU1,1:IMU2,2:IMU3
 # RebootRequired: True
 # Default: 0
-INS_LOG_BAT_MASK,3 # the Matek H743 fligth controller only has two IMUs
+INS_LOG_BAT_MASK,3  # the Matek H743 fligth controller only has two IMUs
 
 # Enable temperature calibration
 # Enable the use of temperature calibration parameters for this IMU. For automatic learning set to 2 and
 # also set the INS_TCALn_TMAX to the target temperature, then reboot
 # RebootRequired: True
 # 0: Disabled
 # 1: Enabled
 # 2: LearnCalibration
 # Default: 0
-INS_TCAL1_ENABLE,2 # Activates the temperature calibration for IMU 1 at the next start
+INS_TCAL1_ENABLE,2  # Activates the temperature calibration for IMU 1 at the next start
 
 # Temperature calibration max
 # The maximum temperature that the calibration is valid for. This must be at least 10 degrees above TMIN
 # for calibration
 # Range: -70 80
 # Units: degC (degrees Celsius)
 # Calibration: 1
 # Default: 70
-INS_TCAL1_TMAX,60 # our H7 processor acts as a heater and heats up the board to almost 60 deg
+INS_TCAL1_TMAX,60  # our H7 processor acts as a heater and heats up the board to almost 60 deg
 
 # Enable temperature calibration
 # Enable the use of temperature calibration parameters for this IMU. For automatic learning set to 2 and
 # also set the INS_TCALn_TMAX to the target temperature, then reboot
 # RebootRequired: True
 # 0: Disabled
 # 1: Enabled
 # 2: LearnCalibration
 # Default: 0
-INS_TCAL2_ENABLE,2 # Activates the temperature calibration for IMU 2 at the next start
+INS_TCAL2_ENABLE,2  # Activates the temperature calibration for IMU 2 at the next start
 
 # Temperature calibration max
 # The maximum temperature that the calibration is valid for. This must be at least 10 degrees above TMIN
 # for calibration
 # Range: -70 80
 # Units: degC (degrees Celsius)
 # Calibration: 1
 # Default: 70
-INS_TCAL2_TMAX,60 # our H7 processor acts as a heater and heats up the board to almost 60 deg
+INS_TCAL2_TMAX,60  # our H7 processor acts as a heater and heats up the board to almost 60 deg
 
 # Log bitmask
 # Bitmap of what on-board log types to enable. This value is made up of the sum of each of the log types
 # you want to be saved. It is usually best just to enable all basiclog types by setting this to 65535.
 # Bitmask: 0:Fast Attitude,1:Medium Attitude,2:GPS,3:System Performance,4:Control Tuning,5:Navigation Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,10:RC output,11:Optical Flow,12:PID,13:Compass,15:Camera,17:Motors,18:Fast IMU,19:Raw IMU,20:Video Stabilization,21:Fast harmonic notch logging
 # Default: 176126
-LOG_BITMASK,524416 # Only for IMU and Raw-IMU
+LOG_BITMASK,524416  # Only for IMU and Raw-IMU
 
 # Enable logging while disarmed
 # If LOG_DISARMED is set to 1 then logging will be enabled at all times including when disarmed. Logging
 # before arming can make for very large logfiles but can help a lot when tracking down startup issues and
 # is necessary if logging of EKF replay data is selected via the LOG_REPLAY parameter. If LOG_DISARMED is
 # set to 2, then logging will be enabled when disarmed, but not if a USB connection is detected. This can
 # be used to prevent unwanted data logs being generated when the vehicle is connected via USB for log
@@ -60,8 +60,8 @@
 # but if the vehicle never arms then the logs using the filesystem backend will be discarded on the next
 # boot.
 # 0: Disabled
 # 1: Enabled
 # 2: Disabled on USB connection
 # 3: Discard log on reboot if never armed
 # Default: 0
-LOG_DISARMED,1 # to gather data for the offline IMU temperature compensation while the FC is disarmed
+LOG_DISARMED,1  # Gather data for the offline IMU temperature compensation while the FC is disarmed
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # 10: Yaw90Roll180                    26: Yaw90Pitch180                   43: Roll315
 # 11: Yaw135Roll180                   27: Yaw270Pitch180                  100: Custom 4.1 and older
 # 12: Pitch180                        28: Pitch90Roll90                   101: Custom 1
 # 13: Yaw225Roll180                   29: Pitch90Roll180                  102: Custom 2
 # 14: Yaw270Roll180                   30: Pitch90Roll270
 # 15: Yaw315Roll180                   31: Pitch180Roll90
 # Default: 0
-AHRS_ORIENTATION,0
+AHRS_ORIENTATION,0  # Point forward in the direction of travel
 
 # Enable logging while disarmed
 # If LOG_DISARMED is set to 1 then logging will be enabled at all times including when disarmed. Logging
 # before arming can make for very large logfiles but can help a lot when tracking down startup issues and
 # is necessary if logging of EKF replay data is selected via the LOG_REPLAY parameter. If LOG_DISARMED is
 # set to 2, then logging will be enabled when disarmed, but not if a USB connection is detected. This can
 # be used to prevent unwanted data logs being generated when the vehicle is connected via USB for log
@@ -35,8 +35,8 @@
 # but if the vehicle never arms then the logs using the filesystem backend will be discarded on the next
 # boot.
 # 0: Disabled
 # 1: Enabled
 # 2: Disabled on USB connection
 # 3: Discard log on reboot if never armed
 # Default: 0
-LOG_DISARMED,0 # Log disarmed was only required for offline IMU temperature calibration
+LOG_DISARMED,0  # Log disarmed was only required for offline IMU temperature calibration
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Amps per volt
 # Number of amps that a 1V reading on the current sensor corresponds to. With a Pixhawk using the 3DR Power
 # brick this should be set to 17. For the Pixhawk with the 3DR 4in1 ESC this should be 17. For Synthetic
 # Current sensor monitors, this is the maximum, full throttle current draw.
 # Units: A/V (ampere per volt)
 # Default: 40
-BATT_AMP_PERVLT,57
+BATT_AMP_PERVLT,158.4  # new calibrated value for Mamba F45_128k 4in1 ESC
 
 # Required arming voltage
 # Battery voltage level which is required to arm the aircraft. Set to 0 to allow arming at any voltage.
 # Units: V (volt)
 # Increment: 0.1
 # Default: 0
 BATT_ARM_VOLT,15
@@ -19,15 +19,15 @@
 # Increment: 50
 # Default: 3300
 BATT_CAPACITY,1800
 
 # Battery critical capacity
 # Battery capacity at which the critical battery failsafe is triggered. Set to 0 to disable battery
 # remaining failsafe. If the battery capacity drops below this level the vehicle will perform the failsafe
-# specified by the BATT_FS_CRT_ACT parameter.
+# specified by the BATT__FS_CRT_ACT parameter.
 # Units: mAh (milliampere hour)
 # Increment: 50
 # Default: 0
 BATT_CRT_MAH,450
 
 # Critical battery voltage
 # Battery voltage that triggers a critical battery failsafe. Set to 0 to disable. If the battery voltage
@@ -86,28 +86,27 @@
 # Increment: 0.1
 # Default: 10.5
 BATT_LOW_VOLT,14.4
 
 # Battery monitoring
 # Controls enabling monitoring of the battery's voltage and current
 # RebootRequired: True
-# 0: Disabled                                          16: SMBus-Maxell
-# 3: Analog Voltage Only                               17: Generator-Elec
-# 4: Analog Voltage and Current                        18: Generator-Fuel
-# 5: Solo                                              19: Rotoye
-# 6: Bebop                                             20: MPPT
-# 7: SMBus-Generic                                     21: INA2XX
-# 8: DroneCAN-BatteryInfo                              22: LTC2946
-# 9: ESC                                               23: Torqeedo
-# 10: Sum Of Selected Monitors                         24: FuelLevelAnalog
-# 11: FuelFlow                                         25: Synthetic Current and Analog Voltage
-# 12: FuelLevelPWM                                     26: INA239_SPI
-# 13: SMBUS-SUI3                                       27: EFI
-# 14: SMBUS-SUI6                                       28: AD7091R5
-# 15: NeoDesign                                        29: Scripting
+# 0: Disabled                                          15: NeoDesign
+# 3: Analog Voltage Only                               16: SMBus-Maxell
+# 4: Analog Voltage and Current                        17: Generator-Elec
+# 5: Solo                                              18: Generator-Fuel
+# 6: Bebop                                             19: Rotoye
+# 7: SMBus-Generic                                     20: MPPT
+# 8: DroneCAN-BatteryInfo                              21: INA2XX
+# 9: ESC                                               22: LTC2946
+# 10: Sum Of Selected Monitors                         23: Torqeedo
+# 11: FuelFlow                                         24: FuelLevelAnalog
+# 12: FuelLevelPWM                                     25: Synthetic Current and Analog Voltage
+# 13: SMBUS-SUI3                                       26: INA239_SPI
+# 14: SMBUS-SUI6                                       27: EFI
 # Default: 4
 BATT_MONITOR,4
 
 # Voltage Multiplier
 # Used to convert the voltage of the voltage sensing pin (BATT_VOLT_PIN) to the actual battery's voltage
 # (pin_voltage * VOLT_MULT). For the 3DR Power brick with a Pixhawk, this should be set to 10.1. For the
 # Pixhawk with the 3DR 4in1 ESC this should be 12.02. For the PX using the PX4IO power supply this should
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_general_configuration.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_general_configuration.param`

 * *Files 19% similar despite different names*

```diff
@@ -1,113 +1,122 @@
+# Arm Checks to Perform (bitmask)
+# Checks prior to arming motor. This is a bitmask of checks that will be performed before allowing arming.
+# For most users it is recommended to leave this at the default of 1 (all checks enabled). You can select
+# whatever checks you prefer by adding together the values of each check type to set this parameter. For
+# example, to only allow arming when you have GPS lock and no RC failsafe you would set ARMING_CHECK to 72.
+# Bitmask: 0:All,1:Barometer,2:Compass,3:GPS lock,4:INS,5:Parameters,6:RC Channels,7:Board voltage,8:Battery Level,10:Logging Available,11:Hardware safety switch,12:GPS Configuration,13:System,14:Mission,15:Rangefinder,16:Camera,17:AuxAuth,18:VisualOdometry,19:FFT
+# Default: 1
+ARMING_CHECK,1  # perform all arming checks. If you have a problem fix it's source. Do NOT change this
+
 # Timezone offset from UTC
 # Adds offset in +- minutes from UTC to calculate local time
 # Range: -720 +840
 # Default: 0
-BRD_RTC_TZ_MIN,60
+BRD_RTC_TZ_MIN,60  # Berlin time zone
 
 # Fence Type
 # Enabled fence types held as bitmask
-# Bitmask: 0:Max altitude,1:Circle Centered on Home,2:Inclusion/Exclusion Circles+Polygons,3:Min altitude
+# Bitmask: 0:Max altitude,1:Circle,2:Polygon,3:Min altitude
 # Default: 7
-FENCE_TYPE,11
+FENCE_TYPE,7  # cylinder and max altitude, to obey local regulations and safety measures
 
 # Accel filter cutoff frequency
 # Filter cutoff frequency for accelerometers. This can be set to a lower value to try to cope with very
 # high vibration levels in aircraft. A value of zero means no filtering (not recommended!)
 # Units: Hz (hertz)
 # Range: 0 256
 # Default: 20
-INS_ACCEL_FILTER,10 # the default is 20 and that lets too much noise in
+INS_ACCEL_FILTER,10  # the default is 20 and that lets too much noise in
 
 # IMU accelerometer X position
 # X position of the first IMU Accelerometer in body frame. Positive X is forward of the origin. Attention:
 # The IMU should be located as close to the vehicle c.g. as practical so that the value of this parameter
 # is minimised. Failure to do so can result in noisy navigation velocity measurements due to vibration and
 # IMU gyro noise. If the IMU cannot be moved and velocity noise is a problem, a location closer to the IMU
 # can be used as the body frame origin.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-INS_POS1_X,0 # was -0.005
+INS_POS1_X,0  # was -0.005
 
 # IMU accelerometer Y position
 # Y position of the first IMU accelerometer in body frame. Positive Y is to the right of the origin.
 # Attention: The IMU should be located as close to the vehicle c.g. as practical so that the value of this
 # parameter is minimised. Failure to do so can result in noisy navigation velocity measurements due to
 # vibration and IMU gyro noise. If the IMU cannot be moved and velocity noise is a problem, a location
 # closer to the IMU can be used as the body frame origin.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-INS_POS1_Y,0 # was -0.011
+INS_POS1_Y,0  # was -0.011
 
 # IMU accelerometer X position
 # X position of the second IMU accelerometer in body frame. Positive X is forward of the origin. Attention:
 # The IMU should be located as close to the vehicle c.g. as practical so that the value of this parameter
 # is minimised. Failure to do so can result in noisy navigation velocity measurements due to vibration and
 # IMU gyro noise. If the IMU cannot be moved and velocity noise is a problem, a location closer to the IMU
 # can be used as the body frame origin.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-INS_POS2_X,0 # was -0.011
+INS_POS2_X,0  # was -0.011
 
 # IMU accelerometer Y position
 # Y position of the second IMU accelerometer in body frame. Positive Y is to the right of the origin.
 # Attention: The IMU should be located as close to the vehicle c.g. as practical so that the value of this
 # parameter is minimised. Failure to do so can result in noisy navigation velocity measurements due to
 # vibration and IMU gyro noise. If the IMU cannot be moved and velocity noise is a problem, a location
 # closer to the IMU can be used as the body frame origin.
 # Units: m (meters)
 # Range: -5 5
 # Increment: 0.01
 # Default: 0
-INS_POS2_Y,0 # was -0.01
+INS_POS2_Y,0  # was -0.01
 
 # Land alt low
 # Altitude during Landing at which vehicle slows to LAND_SPEED
 # Units: cm (centimeters)
 # Range: 100 10000
 # Increment: 10
 # Default: 1000
-LAND_ALT_LOW,200 # come down fast and only slow down close to the ground. We have a good GNSS receiver, so thrust it
+LAND_ALT_LOW,200  # come down fast and only slow down close to the ground. We have a good GNSS receiver, so thrust it
 
 # RTL Altitude
 # The minimum alt above home the vehicle will climb to before returning.  If the vehicle is flying higher
 # than this value it will return at its current altitude.
 # Units: cm (centimeters)
-# Range: 30 300000
+# Range: 200 300000
 # Increment: 1
 # Default: 1500
-RTL_ALT,300 # The default is too high for the kind of flights we do. This reduces the altitude for indoors
+RTL_ALT,300  # The default is too high for the kind of flights we do. This reduces the altitude for indoors
 
 # RTL loiter time
 # Time (in milliseconds) to loiter above home before beginning final descent
 # Units: ms (milliseconds)
 # Range: 0 60000
 # Increment: 1000
 # Default: 5000
-RTL_LOIT_TIME,1000 # The default is too long. This reduces the time
+RTL_LOIT_TIME,1000  # The default is too long. This reduces the time
 
 # Scheduling main loop rate
 # This controls the rate of the main control loop in Hz. This should only be changed by developers. This
 # only takes effect on restart. Values over 400 are considered highly experimental.
 # RebootRequired: True
 # 50: 50Hz
 # 100: 100Hz
 # 200: 200Hz
 # 250: 250Hz
 # 300: 300Hz
 # 400: 400Hz
 # Default: 400
-SCHED_LOOP_RATE,800 # On our vehicle the propellers rotate at speeds higher than 400Hz and we have a powerful STM32 H7 family processor. So we increase this for added performance.
+SCHED_LOOP_RATE,800  # On our vehicle the propellers rotate at speeds higher than 400Hz and we have a powerful STM32 H7 family processor. So we increase this for added performance.
 
 # Enable Scripting
 # Controls if scripting is enabled
 # RebootRequired: True
 # 0: None
 # 1: Lua Scripts
 # Default: 0
-SCR_ENABLE,1  # For MagFit automation and Windspeed Estimation automation
+SCR_ENABLE,1  # For VTOL-Quicktune, MagFit automation and Windspeed Estimation automation
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_logging.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_logging.param`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 INS_LOG_BAT_OPT,4  # Logs measured data both before and after the filters for Filter Review Webtool usage
 
 # Log bitmask
 # Bitmap of what on-board log types to enable. This value is made up of the sum of each of the log types
 # you want to be saved. It is usually best just to enable all basiclog types by setting this to 65535.
 # Bitmask: 0:Fast Attitude,1:Medium Attitude,2:GPS,3:System Performance,4:Control Tuning,5:Navigation Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,10:RC output,11:Optical Flow,12:PID,13:Compass,15:Camera,17:Motors,18:Fast IMU,19:Raw IMU,20:Video Stabilization,21:Fast harmonic notch logging
 # Default: 176126
-LOG_BITMASK,145372 # Defines the logged signals
+LOG_BITMASK,2242524  # Logs Notch filter data and other control signals
 
 # Stop logging to current file on disarm
 # When set, the current log file is closed when the vehicle is disarmed.  If LOG_DISARMED is set then a
 # fresh log will be opened. Applies to the File and Block logging backends.
 # 0: Disabled
 # 1: Enabled
 # Default: 0
-LOG_FILE_DSRMROT,1 # One .bin log file per flight, not per battery/reboot
+LOG_FILE_DSRMROT,1  # One .bin log file per flight, not per battery/reboot
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_pid_adjustment.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_autotune_roll_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_autotune_roll_results.param`

 * *Files 10% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_R_MAX,507500
+ATC_ACCEL_R_MAX,523377.3125
 
 # Roll axis angle controller P gain
 # Roll axis angle controller P gain.  Converts the error between the desired roll angle and actual angle to
 # a desired roll rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_RLL_P,36 # higher value mean a tighter tune
+ATC_ANG_RLL_P,36  # higher value mean a tighter tune
 
 # Roll axis rate controller D gain
 # Roll axis rate controller D gain.  Compensates for short-term change in desired roll rate vs actual roll
 # rate
 # Range: 0.0 0.03
 # Increment: 0.001
 # Default: 0.0036
-ATC_RAT_RLL_D,0.005008578
+ATC_RAT_RLL_D,0.002438
 
 # Roll axis rate controller I gain
 # Roll axis rate controller I gain.  Corrects long-term difference in desired roll rate vs actual roll rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_RLL_I,0.2908089
+ATC_RAT_RLL_I,0.125126
 
 # Roll axis rate controller P gain
-# Roll axis rate controller P gain.  Corrects in proportion to the difference between the desired roll rate
-# vs actual roll rate
+# Roll axis rate controller P gain.  Converts the difference between desired roll rate and actual roll rate
+# into a motor speed output
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
-ATC_RAT_RLL_P,0.2908089
+ATC_RAT_RLL_P,0.125126
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_pitch_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_pitch_results.param`

 * *Files 15% similar despite different names*

```diff
@@ -5,39 +5,39 @@
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_P_MAX,360201.2
+ATC_ACCEL_P_MAX,401666.40625
 
 # Pitch axis angle controller P gain
 # Pitch axis angle controller P gain.  Converts the error between the desired pitch angle and actual angle
 # to a desired pitch rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_PIT_P,28.51195 # higher value mean a tighter tune
+ATC_ANG_PIT_P,34.656452  # higher value mean a tighter tune
 
 # Pitch axis rate controller D gain
 # Pitch axis rate controller D gain.  Compensates for short-term change in desired pitch rate vs actual
 # pitch rate
 # Range: 0.0 0.03
 # Increment: 0.001
 # Default: 0.0036
-ATC_RAT_PIT_D,0.009135851
+ATC_RAT_PIT_D,0.004433
 
 # Pitch axis rate controller I gain
 # Pitch axis rate controller I gain.  Corrects long-term difference in desired pitch rate vs actual pitch
 # rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_PIT_I,0.5622395
+ATC_RAT_PIT_I,0.282138
 
 # Pitch axis rate controller P gain
 # Pitch axis rate controller P gain.  Corrects in proportion to the difference between the desired pitch
 # rate vs actual pitch rate
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
-ATC_RAT_PIT_P,0.5622395
+ATC_RAT_PIT_P,0.282138
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_yaw_setup.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_yaw_setup.param`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 # Default: 0
 ATC_RAT_YAW_FLTD,28.75  # INS_GYRO_FILTER / 4
 
 # Autotune aggressiveness
 # Autotune aggressiveness. Defines the bounce back used to detect size of the D term.
 # Range: 0.05 0.10
 # Default: 0.1
-AUTOTUNE_AGGR,0.10 # Use the default for now
+AUTOTUNE_AGGR,0.085  # Use smaller than default value because there is no wind in the Hangar
 
 # Autotune axis bitmask
 # 1-byte bitmap of axes to autotune
 # Bitmask: 0:Roll,1:Pitch,2:Yaw
 # Default: 7
-AUTOTUNE_AXES,4 # Autotune on yaw axis
+AUTOTUNE_AXES,4  # Autotune yaw axis
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yawd_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yawd_results.param`

 * *Files 26% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 # Increment: 1000
 # 0: Disabled
 # 9000: VerySlow
 # 18000: Slow
 # 36000: Medium
 # 54000: Fast
 # Default: 27000
-ATC_ACCEL_Y_MAX,91119.27
+ATC_ACCEL_Y_MAX,305912.25  # Autotuned in a windless hangar
 
 # Yaw axis angle controller P gain
 # Yaw axis angle controller P gain.  Converts the error between the desired yaw angle and actual angle to a
 # desired yaw rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_YAW_P,14.52818
+ATC_ANG_YAW_P,29.631269  # Autotuned in a windless hangar
 
 # Yaw axis rate controller D gain
 # Yaw axis rate controller D gain.  Compensates for short-term change in desired yaw rate vs actual yaw
 # rate
 # Range: 0.000 0.02
 # Increment: 0.001
 # Default: 0
-ATC_RAT_YAW_D,0.003507904 # if == to AUTOTUNE_MIN_D, autotune failed
+ATC_RAT_YAW_D,0.017587  # if == to AUTOTUNE_MIN_D, autotune failed
 
 # Yaw axis rate controller I gain
 # Yaw axis rate controller I gain.  Corrects long-term difference in desired yaw rate vs actual yaw rate
 # Range: 0.01 0.2
 # Increment: 0.01
 # Default: 0.018
-ATC_RAT_YAW_I,0.09050494
+ATC_RAT_YAW_I,0.061538  # Autotuned in a windless hangar
 
 # Yaw axis rate controller P gain
-# Yaw axis rate controller P gain.  Corrects in proportion to the difference between the desired yaw rate
-# vs actual yaw rate
+# Yaw axis rate controller P gain.  Converts the difference between desired yaw rate and actual yaw rate
+# into a motor speed output
 # Range: 0.180 0.60
 # Increment: 0.005
 # Default: 0.18
-ATC_RAT_YAW_P,0.9050494
+ATC_RAT_YAW_P,0.615382  # Autotuned in a windless hangar
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_roll_pitch_retune_results.param`

 * *Files 19% similar despite different names*

```diff
@@ -5,82 +5,82 @@
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_P_MAX,339368.9
+ATC_ACCEL_P_MAX,363812.1875  # Autotuned in a windless hangar
 
 # Acceleration Max for Roll
 # Maximum acceleration in roll axis
 # Units: cdeg/s/s (centidegrees per square second)
 # Range: 0 180000
 # Increment: 1000
 # 0: Disabled
 # 30000: VerySlow
 # 72000: Slow
 # 108000: Medium
 # 162000: Fast
 # Default: 110000
-ATC_ACCEL_R_MAX,490096.8
+ATC_ACCEL_R_MAX,495292.5625  # Autotuned in a windless hangar
 
 # Pitch axis angle controller P gain
 # Pitch axis angle controller P gain.  Converts the error between the desired pitch angle and actual angle
 # to a desired pitch rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_PIT_P,31.19081 # higher value mean a tighter tune
+ATC_ANG_PIT_P,36  # higher value mean a tighter tune
 
 # Roll axis angle controller P gain
 # Roll axis angle controller P gain.  Converts the error between the desired roll angle and actual angle to
 # a desired roll rate
 # Range: 3.000 12.000
 # Default: 4.5
-ATC_ANG_RLL_P,36 # higher value mean a tighter tune
+ATC_ANG_RLL_P,36  # higher value mean a tighter tune
 
 # Pitch axis rate controller D gain
 # Pitch axis rate controller D gain.  Compensates for short-term change in desired pitch rate vs actual
 # pitch rate
 # Range: 0.0 0.03
 # Increment: 0.001
 # Default: 0.0036
-ATC_RAT_PIT_D,0.006667002
+ATC_RAT_PIT_D,0.003774  # Autotuned in a windless hangar
 
 # Pitch axis rate controller I gain
 # Pitch axis rate controller I gain.  Corrects long-term difference in desired pitch rate vs actual pitch
 # rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_PIT_I,0.3464575
+ATC_RAT_PIT_I,0.193122  # Autotuned in a windless hangar
 
 # Pitch axis rate controller P gain
 # Pitch axis rate controller P gain.  Corrects in proportion to the difference between the desired pitch
 # rate vs actual pitch rate
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
-ATC_RAT_PIT_P,0.3464575
+ATC_RAT_PIT_P,0.193122  # Autotuned in a windless hangar
 
 # Roll axis rate controller D gain
 # Roll axis rate controller D gain.  Compensates for short-term change in desired roll rate vs actual roll
 # rate
 # Range: 0.0 0.03
 # Increment: 0.001
 # Default: 0.0036
-ATC_RAT_RLL_D,0.004972266
+ATC_RAT_RLL_D,0.00242  # Autotuned in a windless hangar
 
 # Roll axis rate controller I gain
 # Roll axis rate controller I gain.  Corrects long-term difference in desired roll rate vs actual roll rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_RLL_I,0.286474
+ATC_RAT_RLL_I,0.12357  # Autotuned in a windless hangar
 
 # Roll axis rate controller P gain
 # Roll axis rate controller P gain.  Corrects in proportion to the difference between the desired roll rate
 # vs actual roll rate
 # Range: 0.0 0.35
 # Increment: 0.005
 # Default: 0.135
-ATC_RAT_RLL_P,0.286474
+ATC_RAT_RLL_P,0.12357  # Autotuned in a windless hangar
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_windspeed_estimation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_windspeed_estimation.param`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # wind drift for vehicles with bluff bodies and without propulsion forces in the X and Y direction (eg
 # multicopters). The drag produced by this effect scales with speed squared.  Set to a postive value > 1.0
 # to enable. A starting value is the mass in Kg divided by the frontal area. The predicted drag from the
 # rotors is specified separately by the EK3_DRAG_MCOEF parameter.
 # Range: 0.0 1000.0
 # Units: kg/m/m (kilograms per square meter)
 # Default: 0
-EK3_DRAG_BCOEF_X,51.0399  # 0.56 kg / 0.01097 m²
+EK3_DRAG_BCOEF_X,54.6857  # 0.600 kg / 0.01097 m²
 
 # Ballistic coefficient for Y axis drag
 # Ratio of mass to drag coefficient measured along the Y body axis. This parameter enables estimation of
 # wind drift for vehicles with bluff bodies and without propulsion forces in the X and Y direction (eg
 # multicopters). The drag produced by this effect scales with speed squared.  Set to a postive value > 1.0
 # to enable. A starting value is the mass in Kg divided by the side area. The predicted drag from the
 # rotors is specified separately by the EK3_DRAG_MCOEF parameter.
 # Range: 50.0 1000.0
 # Units: kg/m/m (kilograms per square meter)
 # Default: 0
-EK3_DRAG_BCOEF_Y,38.4798  # 0.56 kg / 0.01455 m²
+EK3_DRAG_BCOEF_Y,41.2284  # 0.600 kg / 0.01455 m²
 
 # Momentum coefficient for propeller drag
 # This parameter is used to predict the drag produced by the rotors when flying a multi-copter, enabling
 # estimation of wind drift. The drag produced by this effect scales with speed not speed squared and is
 # produced because some of the air velocity normal to the rotors axis of rotation is lost when passing
 # through the rotor disc which changes the momentum of the airflow causing drag. For unducted rotors the
 # effect is roughly proportional to the area of the propeller blades when viewed side on and changes with
@@ -31,15 +31,15 @@
 # 0.1 = (1.5/15.0). Set EK3_MCOEF to a postive value to enable wind estimation using this drag effect. To
 # account for the drag produced by the body which scales with speed squared, see documentation for the
 # EK3_DRAG_BCOEF_X and EK3_DRAG_BCOEF_Y parameters.
 # Range: 0.0 1.0
 # Increment: 0.01
 # Units: 1/s (per second)
 # Default: 0
-EK3_DRAG_MCOEF,0.5127
+EK3_DRAG_MCOEF,0.5195
 
 # Enable logging while disarmed
 # If LOG_DISARMED is set to 1 then logging will be enabled at all times including when disarmed. Logging
 # before arming can make for very large logfiles but can help a lot when tracking down startup issues and
 # is necessary if logging of EKF replay data is selected via the LOG_REPLAY parameter. If LOG_DISARMED is
 # set to 2, then logging will be enabled when disarmed, but not if a USB connection is detected. This can
 # be used to prevent unwanted data logs being generated when the vehicle is connected via USB for log
@@ -47,19 +47,19 @@
 # but if the vehicle never arms then the logs using the filesystem backend will be discarded on the next
 # boot.
 # 0: Disabled
 # 1: Enabled
 # 2: Disabled on USB connection
 # 3: Discard log on reboot if never armed
 # Default: 0
-LOG_DISARMED,1 # allow post flight tuning with Replay
+LOG_DISARMED,1  # allow post flight tuning with Replay
 
 # Enable logging of information needed for Replay
 # If LOG_REPLAY is set to 1 then the EKF2 and EKF3 state estimators will log detailed information needed
 # for diagnosing problems with the Kalman filter. LOG_DISARMED must be set to 1 or 2 or else the log will
 # not contain the pre-flight data required for replay testing of the EKF's. It is suggested that you also
 # raise LOG_FILE_BUFSIZE to give more buffer space for logging and use a high quality microSD card to
 # ensure no sensor data is lost.
 # 0: Disabled
 # 1: Enabled
 # Default: 0
-LOG_REPLAY,1 # allow post flight tuning with Replay
+LOG_REPLAY,1  # allow post flight tuning with Replay
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_barometer_compensation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_system_id_roll.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_system_id_roll.param`

 * *Files 7% similar despite different names*

```diff
@@ -16,22 +16,34 @@
 ARMING_CHECK,540126  # disable Parameter check because we need to set ATC_RAT_RLL_I out-of-range (was 30175)
 
 # Roll axis rate controller I gain
 # Roll axis rate controller I gain.  Corrects long-term difference in desired roll rate vs actual roll rate
 # Range: 0.0 0.6
 # Increment: 0.01
 # Default: 0.135
-ATC_RAT_RLL_I,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
+ATC_RAT_RLL_I,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
 
 # Rate Feedforward Enable
-# Controls whether body-frame rate feedforward is enabled or disabled
+# Controls whether body-frame rate feedfoward is enabled or disabled
 # 0: Disabled
 # 1: Enabled
 # Default: 1
-ATC_RATE_FF_ENAB,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
+ATC_RATE_FF_ENAB,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
+
+# Flight Mode 5
+# Flight mode when pwm of Flightmode channel(FLTMODE_CH) is >1620, <= 1749
+# 0: Stabilize               7: Circle                  17: Brake                  24: ZigZag
+# 1: Acro                    9: Land                    18: Throw                  25: SystemID
+# 2: AltHold                 11: Drift                  19: Avoid_ADSB             26: Heli_Autorotate
+# 3: Auto                    13: Sport                  20: Guided_NoGPS           27: Auto RTL
+# 4: Guided                  14: Flip                   21: Smart_RTL
+# 5: Loiter                  15: AutoTune               22: FlowHold
+# 6: RTL                     16: PosHold                23: Follow
+# Default: 0
+FLTMODE5,25
 
 # Enable logging while disarmed
 # If LOG_DISARMED is set to 1 then logging will be enabled at all times including when disarmed. Logging
 # before arming can make for very large logfiles but can help a lot when tracking down startup issues and
 # is necessary if logging of EKF replay data is selected via the LOG_REPLAY parameter. If LOG_DISARMED is
 # set to 2, then logging will be enabled when disarmed, but not if a USB connection is detected. This can
 # be used to prevent unwanted data logs being generated when the vehicle is connected via USB for log
@@ -39,38 +51,38 @@
 # but if the vehicle never arms then the logs using the filesystem backend will be discarded on the next
 # boot.
 # 0: Disabled
 # 1: Enabled
 # 2: Disabled on USB connection
 # 3: Discard log on reboot if never armed
 # Default: 0
-LOG_DISARMED,0 # was only needed for wind speed estimation
+LOG_DISARMED,0  # was only needed for wind speed estimation
 
 # Enable logging of information needed for Replay
 # If LOG_REPLAY is set to 1 then the EKF2 and EKF3 state estimators will log detailed information needed
 # for diagnosing problems with the Kalman filter. LOG_DISARMED must be set to 1 or 2 or else the log will
 # not contain the pre-flight data required for replay testing of the EKF's. It is suggested that you also
 # raise LOG_FILE_BUFSIZE to give more buffer space for logging and use a high quality microSD card to
 # ensure no sensor data is lost.
 # 0: Disabled
 # 1: Enabled
 # Default: 0
-LOG_REPLAY,0 # was only needed for wind speed estimation
+LOG_REPLAY,0  # was only needed for wind speed estimation
 
 # System identification axis
 # Controls which axis are being excited.  Set to non-zero to see more parameters
 # 0: None                                              7: Rate Roll
 # 1: Input Roll Angle                                  8: Rate Pitch
 # 2: Input Pitch Angle                                 9: Rate Yaw
 # 3: Input Yaw Angle                                   10: Mixer Roll
 # 4: Recovery Roll Angle                               11: Mixer Pitch
 # 5: Recovery Pitch Angle                              12: Mixer Yaw
 # 6: Recovery Yaw Angle                                13: Mixer Thrust
 # Default: 0
-SID_AXIS,10
+SID_AXIS,10  # Inject chip on the mixer roll signal
 
 # System identification Start Frequency
 # Frequency at the start of the sweep
 # Range: 0.01 100
 # Units: Hz (hertz)
 SID_F_START_HZ,0.05
 
@@ -113,20 +125,20 @@
 # 6: Rate Yaw kP                      10: WP Speed                        51: Rate Roll kD
 # 26: Rate Yaw kD                     25: Acro Roll/Pitch deg/s           52: Rate Pitch FF
 # 56: Rate Yaw Filter                 40: Acro Yaw deg/s                  53: Rate Roll FF
 # 55: Motor Yaw Headroom              45: RC Feel                         54: Rate Yaw FF
 # 14: AltHold kP                      13: Heli Ext Gyro                   58: SysID Magnitude
 # 7: Throttle Rate kP                 38: Declination                     59: PSC Angle Max
 # Default: 0
-TUNE,58  # System identification magnitude
+TUNE,0  # System identification magnitude
 
 # Tuning maximum
 # Maximum value that the parameter currently being tuned with the transmitter's channel 6 knob will be set
 # to
 # Default: 0
-TUNE_MAX,0.40  # System identification max magnitude
+TUNE_MAX,0.4  # System identification max magnitude
 
 # Tuning minimum
 # Minimum value that the parameter currently being tuned with the transmitter's channel 6 knob will be set
 # to
 # Default: 0
 TUNE_MIN,0.02  # System identification min magnitude
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_system_id_pitch.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_yaw.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_thrust.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_analytical_pid_optimization.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_analytical_pid_optimization.param`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Arm Checks to Perform (bitmask)
 # Checks prior to arming motor. This is a bitmask of checks that will be performed before allowing arming.
 # For most users it is recommended to leave this at the default of 1 (all checks enabled). You can select
 # whatever checks you prefer by adding together the values of each check type to set this parameter. For
 # example, to only allow arming when you have GPS lock and no RC failsafe you would set ARMING_CHECK to 72.
 # Bitmask: 0:All,1:Barometer,2:Compass,3:GPS lock,4:INS,5:Parameters,6:RC Channels,7:Board voltage,8:Battery Level,10:Logging Available,11:Hardware safety switch,12:GPS Configuration,13:System,14:Mission,15:Rangefinder,16:Camera,17:AuxAuth,18:VisualOdometry,19:FFT
 # Default: 1
-ARMING_CHECK,0  # normal state for every day use
+ARMING_CHECK,1  # Normal state for everyday use
 
 # Rate Feedforward Enable
-# Controls whether body-frame rate feedforward is enabled or disabled
+# Controls whether body-frame rate feedfoward is enabled or disabled
 # 0: Disabled
 # 1: Enabled
 # Default: 1
-ATC_RATE_FF_ENAB,1  # restore value now that system identification is done
+ATC_RATE_FF_ENAB,1  # Restore value now that system identification is done
 
 # Acceleration (vertical) controller I gain
 # Acceleration (vertical) controller I gain.  Corrects long-term difference in desired vertical
 # acceleration and actual acceleration
 # Range: 0.000 3.000
 # Default: 1
 PSC_ACCZ_I,0.816  # now that system identification on thrust has been completed, restore it to 2 • MOT_THST_HOVER
@@ -27,8 +27,8 @@
 # 1: Input Roll Angle                                  8: Rate Pitch
 # 2: Input Pitch Angle                                 9: Rate Yaw
 # 3: Input Yaw Angle                                   10: Mixer Roll
 # 4: Recovery Roll Angle                               11: Mixer Pitch
 # 5: Recovery Pitch Angle                              12: Mixer Yaw
 # 6: Recovery Yaw Angle                                13: Mixer Thrust
 # Default: 0
-SID_AXIS,0
+SID_AXIS,0  # No more system identification chip injections
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_everyday_use.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_everyday_use.param`

 * *Files 9% similar despite different names*

```diff
@@ -30,21 +30,21 @@
 BATT2_FS_LOW_ACT,2  # outdoors we want the drone to come back
 
 # Log bitmask
 # Bitmap of what on-board log types to enable. This value is made up of the sum of each of the log types
 # you want to be saved. It is usually best just to enable all basiclog types by setting this to 65535.
 # Bitmask: 0:Fast Attitude,1:Medium Attitude,2:GPS,3:System Performance,4:Control Tuning,5:Navigation Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,10:RC output,11:Optical Flow,12:PID,13:Compass,15:Camera,17:Motors,18:Fast IMU,19:Raw IMU,20:Video Stabilization,21:Fast harmonic notch logging
 # Default: 176126
-LOG_BITMASK,2241500 # 2:GPS,3:System Performance,4:Control Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,12:PID,13:Compass,17:Motors,21:Fast harmonic notch logging
+LOG_BITMASK,144348  # 2:GPS,3:System Performance,4:Control Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,12:PID,13:Compass,17:Motors
 
 # RTL Altitude
 # The minimum alt above home the vehicle will climb to before returning.  If the vehicle is flying higher
 # than this value it will return at its current altitude.
 # Units: cm (centimeters)
-# Range: 30 300000
+# Range: 200 300000
 # Increment: 1
 # Default: 1500
 RTL_ALT,500  # The default is too high for the kind of flights we do. This reduces the altitude for outdoors
 
 # RTL minimum climb
 # The vehicle will climb this many cm during the initial climb portion of the RTL
 # Units: cm (centimeters)
```

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.4.2/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json` & `methodicconfigurator-0.5.1/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json`

 * *Files identical despite different names*

