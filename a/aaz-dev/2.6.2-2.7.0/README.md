# Comparing `tmp/aaz_dev-2.6.2.tar.gz` & `tmp/aaz_dev-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaz_dev-2.6.2.tar", last modified: Fri Apr 26 07:25:41 2024, max compression
+gzip compressed data, was "aaz_dev-2.7.0.tar", last modified: Tue May 14 07:44:45 2024, max compression
```

## Comparing `aaz_dev-2.6.2.tar` & `aaz_dev-2.7.0.tar`

### file list

```diff
@@ -1,248 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-26 07:25:05.000000 aaz_dev-2.6.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-26 07:25:05.000000 aaz_dev-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-26 07:25:05.000000 aaz_dev-2.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-26 07:25:05.000000 aaz_dev-2.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.282156 aaz_dev-2.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.286156 aaz_dev-2.6.2/src/aaz_dev/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/app/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/app/url_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/cli/api/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/api/az.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/api/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/cli/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18546 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_arg_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_client_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_command_ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_command_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27670 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_module_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    39660 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_operation_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_output_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_profile_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_selector_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19027 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/controller/portal_cli_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.290156 aaz_dev-2.6.2/src/aaz_dev/cli/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/common/_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/command/
--rw-r--r--   0 runner    (1001) docker     (127)    31956 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/group/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.294156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/profile/_clients.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/setup.cfg.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/setup.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)    18306 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/macros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/cli/templates/python.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.298156 aaz_dev-2.6.2/src/aaz_dev/command/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/api/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.302156 aaz_dev-2.6.2/src/aaz_dev/command/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42226 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/cfg_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/cfg_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/client_cfg_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    25715 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/specs_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    68895 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_cfg_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_client_cfg_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    48777 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.302156 aaz_dev-2.6.2/src/aaz_dev/command/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26834 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http_response_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    37141 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_selector_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_subresource_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/command/model/editor/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/editor/_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/command/model/specs/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/specs/_command_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/model/specs/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/command/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/command.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/group.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/resource_ref.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/command/templates/tree.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.306156 aaz_dev-2.6.2/src/aaz_dev/swagger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.310156 aaz_dev-2.6.2/src/aaz_dev/swagger/api/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.310156 aaz_dev-2.6.2/src/aaz_dev/swagger/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25776 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/controller/command_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/controller/specs_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.310156 aaz_dev-2.6.2/src/aaz_dev/swagger/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27739 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/cmd_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/external_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    18059 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/items.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/license.py
--rw-r--r--   0 runner    (1001) docker     (127)    12934 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/path_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    29035 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/security_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/swagger.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_odata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_resource_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/swagger/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/swagger/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-26 07:25:24.000000 aaz_dev-2.6.2/src/aaz_dev/ui/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.286156 aaz_dev-2.6.2/src/aaz_dev/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.314156 aaz_dev-2.6.2/src/aaz_dev/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/css/main.e6c13ad2.css
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/css/main.e6c13ad2.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.318156 aaz_dev-2.6.2/src/aaz_dev/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   659880 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2745937 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/src/aaz_dev/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/case.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/error_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/portal_file_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/src/aaz_dev/utils/stage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:25:41.322156 aaz_dev-2.6.2/src/aaz_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 07:25:40.000000 aaz_dev-2.6.2/src/aaz_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-26 07:25:06.000000 aaz_dev-2.6.2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.645983 aaz_dev-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-14 07:44:12.000000 aaz_dev-2.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-14 07:44:12.000000 aaz_dev-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-14 07:44:12.000000 aaz_dev-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-14 07:44:45.645983 aaz_dev-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-05-14 07:44:12.000000 aaz_dev-2.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:44:45.645983 aaz_dev-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.601983 aaz_dev-2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.609983 aaz_dev-2.7.0/src/aaz_dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.609983 aaz_dev-2.7.0/src/aaz_dev/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/app/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/app/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/app/url_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.609983 aaz_dev-2.7.0/src/aaz_dev/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.609983 aaz_dev-2.7.0/src/aaz_dev/cli/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/api/az.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/api/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.613983 aaz_dev-2.7.0/src/aaz_dev/cli/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18546 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_arg_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_client_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_command_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27670 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_module_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39660 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_operation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_profile_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_selector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19027 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/controller/portal_cli_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.613983 aaz_dev-2.7.0/src/aaz_dev/cli/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.613983 aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.613983 aaz_dev-2.7.0/src/aaz_dev/cli/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/common/_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.613983 aaz_dev-2.7.0/src/aaz_dev/cli/model/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/view/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/view/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/view/_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/model/view/_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.617983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.617983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.617983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/command/
+-rw-r--r--   0 runner    (1001) docker     (127)    31956 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.617983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/group/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.617983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/profile/_clients.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.617983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.617983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.617983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.617983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/setup.cfg.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/setup.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    18306 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/macros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.621983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.621983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.621983 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/cli/templates/python.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.621983 aaz_dev-2.7.0/src/aaz_dev/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.621983 aaz_dev-2.7.0/src/aaz_dev/command/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30269 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/api/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.621983 aaz_dev-2.7.0/src/aaz_dev/command/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42226 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/cfg_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/cfg_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/client_cfg_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/shorthand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25715 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/specs_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68895 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/workspace_cfg_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/workspace_client_cfg_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/workspace_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50808 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/controller/workspace_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.621983 aaz_dev-2.7.0/src/aaz_dev/command/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.629983 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26834 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_arg_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_arg_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16144 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16687 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_http_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_http_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_instance_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_instance_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_instance_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37141 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_selector_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_subresource_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.629983 aaz_dev-2.7.0/src/aaz_dev/command/model/editor/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/editor/_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.629983 aaz_dev-2.7.0/src/aaz_dev/command/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/specs/_command_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/model/specs/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.629983 aaz_dev-2.7.0/src/aaz_dev/command/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/templates/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/templates/command.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/templates/group.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/templates/resource_ref.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/command/templates/tree.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.629983 aaz_dev-2.7.0/src/aaz_dev/swagger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.629983 aaz_dev-2.7.0/src/aaz_dev/swagger/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.629983 aaz_dev-2.7.0/src/aaz_dev/swagger/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/controller/_example_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25776 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/controller/command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/controller/example_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/controller/specs_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.633983 aaz_dev-2.7.0/src/aaz_dev/swagger/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.637983 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27739 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/cmd_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/example_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/external_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17502 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/path_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29035 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/security_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_odata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.637983 aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_resource_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_swagger_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_swagger_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_swagger_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.637983 aaz_dev-2.7.0/src/aaz_dev/swagger/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/swagger/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.637983 aaz_dev-2.7.0/src/aaz_dev/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 07:44:44.000000 aaz_dev-2.7.0/src/aaz_dev/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-14 07:44:28.000000 aaz_dev-2.7.0/src/aaz_dev/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 07:44:44.000000 aaz_dev-2.7.0/src/aaz_dev/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-14 07:44:28.000000 aaz_dev-2.7.0/src/aaz_dev/ui/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-14 07:44:28.000000 aaz_dev-2.7.0/src/aaz_dev/ui/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-14 07:44:28.000000 aaz_dev-2.7.0/src/aaz_dev/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 07:44:28.000000 aaz_dev-2.7.0/src/aaz_dev/ui/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.605983 aaz_dev-2.7.0/src/aaz_dev/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.637983 aaz_dev-2.7.0/src/aaz_dev/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 07:44:44.000000 aaz_dev-2.7.0/src/aaz_dev/ui/static/css/main.e6c13ad2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-14 07:44:44.000000 aaz_dev-2.7.0/src/aaz_dev/ui/static/css/main.e6c13ad2.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.641983 aaz_dev-2.7.0/src/aaz_dev/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   663932 2024-05-14 07:44:44.000000 aaz_dev-2.7.0/src/aaz_dev/ui/static/js/main.90022267.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-14 07:44:44.000000 aaz_dev-2.7.0/src/aaz_dev/ui/static/js/main.90022267.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2763409 2024-05-14 07:44:44.000000 aaz_dev-2.7.0/src/aaz_dev/ui/static/js/main.90022267.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.645983 aaz_dev-2.7.0/src/aaz_dev/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/error_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/portal_file_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/src/aaz_dev/utils/stage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:44:45.645983 aaz_dev-2.7.0/src/aaz_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-14 07:44:45.000000 aaz_dev-2.7.0/src/aaz_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-14 07:44:45.000000 aaz_dev-2.7.0/src/aaz_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:44:45.000000 aaz_dev-2.7.0/src/aaz_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 07:44:45.000000 aaz_dev-2.7.0/src/aaz_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 07:44:45.000000 aaz_dev-2.7.0/src/aaz_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 07:44:45.000000 aaz_dev-2.7.0/src/aaz_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-14 07:44:13.000000 aaz_dev-2.7.0/version.py
```

### Comparing `aaz_dev-2.6.2/HISTORY.rst` & `aaz_dev-2.7.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 Release History
 ===============
 
+2.7.0
+++++++
+* Support example generation (#361)
+
 2.6.2
 ++++++
 * Refine documentation (#345, #349, #355, #356)
 * Add response schema for lro delete operation (#350)
 * Support empty free-form object (#348)
 * Display ParseJsonFailed error logs (#347)
 * Fix readOnly parsing problem in Swagger (#346)
```

### Comparing `aaz_dev-2.6.2/LICENSE` & `aaz_dev-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/PKG-INFO` & `aaz_dev-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 2.6.2
+Version: 2.7.0
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aaz_dev-2.6.2/README.md` & `aaz_dev-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/setup.py` & `aaz_dev-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/app/app.py` & `aaz_dev-2.7.0/src/aaz_dev/app/app.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/app/run.py` & `aaz_dev-2.7.0/src/aaz_dev/app/run.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/app/url_converters.py` & `aaz_dev-2.7.0/src/aaz_dev/app/url_converters.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/api/_cmds.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/api/az.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/api/az.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/api/portal.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/api/portal.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_arg_group_generator.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_arg_group_generator.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_atomic_profile_builder.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_atomic_profile_builder.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_client_generator.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_client_generator.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_command_ctx.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_command_ctx.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_command_generator.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_module_manager.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_module_manager.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_operation_generator.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_operation_generator.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_output_generator.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_output_generator.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_profile_generator.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_profile_generator.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/az_selector_generator.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/az_selector_generator.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/controller/portal_cli_generator.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/controller/portal_cli_generator.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_client.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_client.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_command.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_command.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_command_group.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_help.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_help.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/atomic/_profile.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/atomic/_profile.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/common/_fields.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/common/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_command.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/view/_command.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_command_group.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/view/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_module.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/view/_module.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/model/view/_profile.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/model/view/_profile.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/templates/__init__.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/templates/_filters.py` & `aaz_dev-2.7.0/src/aaz_dev/cli/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2` & `aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2` & `aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/templates/aaz/profile/_clients.py.j2` & `aaz_dev-2.7.0/src/aaz_dev/cli/templates/aaz/profile/_clients.py.j2`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2` & `aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/templates/extension/setup.py.j2` & `aaz_dev-2.7.0/src/aaz_dev/cli/templates/extension/setup.py.j2`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/templates/macros.j2` & `aaz_dev-2.7.0/src/aaz_dev/cli/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/cli/templates/main/__init__.py.j2` & `aaz_dev-2.7.0/src/aaz_dev/cli/templates/main/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/api/_cmds.py` & `aaz_dev-2.7.0/src/aaz_dev/command/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/api/editor.py` & `aaz_dev-2.7.0/src/aaz_dev/command/api/editor.py`

 * *Files 5% similar despite different names*

```diff
@@ -252,14 +252,79 @@
     new_node_names = new_name.split(' ')
     node = manager.rename_command_tree_node(*node_names, new_node_names=new_node_names)
     result = node.to_primitive()
     manager.save()
     return jsonify(result)
 
 
+@bp.route("/Workspaces/<name>/CommandTree/Nodes/<names_path:node_names>/Leaves/<name:leaf_name>/GenerateExamples",
+          methods=["POST"])
+def editor_workspace_generate_examples(name, node_names, leaf_name):
+    if node_names[0] != WorkspaceManager.COMMAND_TREE_ROOT_NAME:
+        raise exceptions.ResourceNotFind("Command not exist.")
+
+    manager = WorkspaceManager(name)
+    manager.load()
+
+    node_names = node_names[1:]
+    leaf = manager.find_command_tree_leaf(*node_names, leaf_name)
+    if not leaf:
+        raise exceptions.ResourceNotFind("Command not exist.")
+
+    data = request.get_json()
+    source = data.get("source", None)
+
+    cfg_editor = manager.load_cfg_editor_by_command(leaf)
+    command = cfg_editor.find_command(*leaf.names)
+    if not command:
+        raise exceptions.ResourceNotFind("Command not exist.")
+
+    if source == "swagger":
+        examples = manager.generate_examples_by_swagger(leaf, command)
+        result = [example.to_primitive() for example in examples]
+    else:
+        raise exceptions.InvalidAPIUsage("Invalid request.")
+
+    return jsonify(result)
+
+
+@bp.route("/Workspaces/<name>/CommandTree/Nodes/<names_path:node_names>/Leaves/<name:leaf_name>/Examples",
+          methods=["PATCH"])
+def editor_workspace_examples(name, node_names, leaf_name):
+    if node_names[0] != WorkspaceManager.COMMAND_TREE_ROOT_NAME:
+        raise exceptions.ResourceNotFind("Command not exist")
+    node_names = node_names[1:]
+
+    manager = WorkspaceManager(name)
+    manager.load()
+    leaf = manager.find_command_tree_leaf(*node_names, leaf_name)
+    if not leaf:
+        raise exceptions.ResourceNotFind("Command not exist")
+
+    data = request.get_json()
+    if 'examples' in data:
+        leaf = manager.update_command_tree_leaf_examples(*leaf.names, examples=data['examples'])
+    cfg_editor = manager.load_cfg_editor_by_command(leaf)
+
+    command = cfg_editor.find_command(*leaf.names)
+    result = command.to_primitive()
+    manager.save()
+
+    del result['name']
+    result.update({
+        'names': leaf.names,
+        'help': leaf.help.to_primitive(),
+        'stage': leaf.stage,
+    })
+    if leaf.examples:
+        result['examples'] = [e.to_primitive() for e in leaf.examples]
+
+    return jsonify(result)
+
+
 @bp.route("/Workspaces/<name>/CommandTree/Nodes/<names_path:node_names>/Leaves/<name:leaf_name>",
           methods=("GET", "PATCH"))
 def editor_workspace_command(name, node_names, leaf_name):
     if node_names[0] != WorkspaceManager.COMMAND_TREE_ROOT_NAME:
         raise exceptions.ResourceNotFind("Command not exist")
     node_names = node_names[1:]
```

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/api/specs.py` & `aaz_dev-2.7.0/src/aaz_dev/command/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/controller/cfg_reader.py` & `aaz_dev-2.7.0/src/aaz_dev/command/controller/cfg_reader.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/controller/client_cfg_reader.py` & `aaz_dev-2.7.0/src/aaz_dev/command/controller/client_cfg_reader.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/controller/specs_manager.py` & `aaz_dev-2.7.0/src/aaz_dev/command/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_cfg_editor.py` & `aaz_dev-2.7.0/src/aaz_dev/command/controller/workspace_cfg_editor.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_client_cfg_editor.py` & `aaz_dev-2.7.0/src/aaz_dev/command/controller/workspace_client_cfg_editor.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_helper.py` & `aaz_dev-2.7.0/src/aaz_dev/command/controller/workspace_helper.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/controller/workspace_manager.py` & `aaz_dev-2.7.0/src/aaz_dev/command/controller/workspace_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 import logging
 import os
 import shutil
 from datetime import datetime
 
+from command.model.configuration import CMDHelp, CMDResource, CMDCommandExample, CMDArg, CMDCommand, \
+    CMDBuildInVariants, CMDHttpOperation
 from command.model.editor import CMDEditorWorkspace, CMDCommandTreeNode, CMDCommandTreeLeaf
 from swagger.controller.command_generator import CommandGenerator
+from swagger.controller.example_generator import ExampleGenerator
 from swagger.controller.specs_manager import SwaggerSpecsManager
 from swagger.utils.exceptions import InvalidSwaggerValueError
 from utils import exceptions
 from utils.config import Config
 from utils.plane import PlaneEnum
 from .specs_manager import AAZSpecsManager
 from .workspace_cfg_editor import WorkspaceCfgEditor, build_endpoint_selector_for_client_config
 from .workspace_client_cfg_editor import WorkspaceClientCfgEditor
-from command.model.configuration import CMDHelp, CMDResource, CMDCommandExample, CMDArg, CMDCommand, CMDBuildInVariants
 
 logger = logging.getLogger('backend')
 
 
 class WorkspaceManager:
     COMMAND_TREE_ROOT_NAME = "aaz"
 
@@ -83,14 +85,15 @@
         self._cfg_editors = {}
         self._client_cfg_editor = None
         self._reusable_leaves = {}
 
         self._aaz_specs = aaz_manager
         self._swagger_specs = swagger_manager
         self._swagger_command_generator = None
+        self._swagger_example_generator = None
 
     @property
     def is_in_memory(self):
         return self.folder == self.IN_MEMORY
 
     @property
     def aaz_specs(self):
@@ -106,14 +109,21 @@
 
     @property
     def swagger_command_generator(self):
         if not self._swagger_command_generator:
             self._swagger_command_generator = CommandGenerator()
         return self._swagger_command_generator
 
+    @property
+    def swagger_example_generator(self):
+        if not self._swagger_example_generator:
+            self._swagger_example_generator = ExampleGenerator()
+
+        return self._swagger_example_generator
+
     def load(self):
         assert not self.is_in_memory
         # TODO: handle exception
         if not os.path.exists(self.path) or not os.path.isfile(self.path):
             raise exceptions.ResourceNotFind(
                 f"Workspace json file not exist: {self.path}")
         with open(self.path, 'r', encoding="utf-8") as f:
@@ -466,14 +476,62 @@
                 except Exception as err:
                     # if not example.get('name', None) or not isinstance(example['name'], str):
                     raise exceptions.InvalidAPIUsage(
                         f"Invalid example data: {err}")
                 leaf.examples.append(example)
         return leaf
 
+    def generate_examples_by_swagger(self, leaf, command):
+        def is_ready_to_skip(operations):
+            if not operations:
+                return True
+
+            if len(operations) == 1 and isinstance(operations[0], CMDHttpOperation):
+                return False
+
+            # skip when there is more than one operation and not all operations are get requests
+            for op in operations:
+                if not isinstance(op, CMDHttpOperation) or op.http.request.method != "get":
+                    return True
+
+            return False
+
+        if is_ready_to_skip(command.operations):
+            return []
+
+        return self.generate_operations_examples_by_swagger(
+            command,
+            " ".join(leaf.names)
+        )
+
+    def generate_operations_examples_by_swagger(self, command, cmd_name):
+        root = self.find_command_tree_node()
+        assert root
+
+        # convert cmd resource to swagger resource
+        swagger_resources = []
+        for resource in command.resources:
+            swagger_resources.append(self.swagger_specs.get_module_manager(
+                plane=self.ws.plane,
+                mod_names=self.ws.mod_names
+            ).get_resource_in_version(resource["id"], resource["version"], resource.rp_name))
+
+        # load swagger resource
+        cmd_operation_ids = {op.operation_id: op for op in command.operations}
+        self.swagger_example_generator.load_examples(swagger_resources)
+
+        examples = self.swagger_example_generator.create_draft_examples_by_swagger(
+            swagger_resources,
+            command,
+            cmd_operation_ids,
+            cmd_name
+        )
+
+        return examples
+
     def rename_command_tree_node(self, *node_names, new_node_names):
         new_name = ' '.join(new_node_names)
         if not new_name:
             raise exceptions.InvalidAPIUsage(
                 f"Invalid new command name: {new_name}")
 
         node = self.find_command_tree_node(*node_names)
@@ -1097,15 +1155,15 @@
         try:
             self._client_cfg_editor = WorkspaceClientCfgEditor.load_client_cfg(self.folder)
             return self._client_cfg_editor
         except Exception as e:
             logger.error(
                 f"load workspace client cfg failed: {e}: {self.name}")
             return None
-    
+
     def compare_client_cfg_with_spec(self):
         """ Check whether the client configuration version in workspace is later than the aaz specs one. """
         # compare client configuration from aaz specs
         aaz_client_cfg_reader = self.aaz_specs.load_client_cfg_reader(self.ws.plane)
         client_cfg_reader = self.load_client_cfg_editor()
         if client_cfg_reader and not aaz_client_cfg_reader:
             return True
```

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/__init__.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_arg.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg_builder.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_arg_builder.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_arg_group.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_arg_group.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_client.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_client.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_command.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_command.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_command_group.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_condition.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_condition.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_configuration.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_configuration.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_content.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_content.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_fields.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_format.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_format.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_help.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_help.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_http.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http_request_body.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_http_request_body.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_http_response_body.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_http_response_body.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_create.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_instance_create.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_delete.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_instance_delete.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_instance_update.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_instance_update.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_operation.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_operation.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_output.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_output.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_resource.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_schema.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_schema.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_selector_index.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_selector_index.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_subresource_selector.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_subresource_selector.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_utils.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_utils.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/configuration/_xml.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/configuration/_xml.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/editor/_workspace.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/editor/_workspace.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/model/specs/_command_tree.py` & `aaz_dev-2.7.0/src/aaz_dev/command/model/specs/_command_tree.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/templates/__init__.py` & `aaz_dev-2.7.0/src/aaz_dev/command/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/templates/_filters.py` & `aaz_dev-2.7.0/src/aaz_dev/command/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/templates/command.md.j2` & `aaz_dev-2.7.0/src/aaz_dev/command/templates/command.md.j2`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/command/templates/group.md.j2` & `aaz_dev-2.7.0/src/aaz_dev/command/templates/group.md.j2`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/api/_cmds.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/api/specs.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/controller/command_generator.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/controller/command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/controller/specs_manager.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/cmd_builder.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/cmd_builder.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/contact.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/contact.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/fields.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,30 +203,14 @@
             field=StringType(choices=self.VALID_VALUES),
             serialized_name='x-ms-mutability',
             deserialize_from='x-ms-mutability',
             **kwargs
         )
 
 
-class XmsExamplesField(DictType):
-    """
-    Describes the format for specifying examples for request and response of an operation in an OpenAPI definition. It is a dictionary of different variations of the examples for a given operation.
-
-    https://github.com/Azure/azure-rest-api-specs/blob/master/documentation/x-ms-examples.md
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(
-            field=BaseType(),
-            serialized_name='x-ms-examples',
-            deserialize_from='x-ms-examples',
-            **kwargs
-        )
-
-
 class XmsErrorResponseField(BooleanType):
     """
     Indicates whether the response status code should be treated as an error response or not.
 
     https://github.com/Azure/autorest/blob/main/docs/extensions/readme.md#x-ms-error-response
     """
```

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/info.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/info.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/items.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/items.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/operation.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+import logging
 from urllib.parse import urljoin
 
 from schematics.models import Model
 from schematics.types import StringType, ModelType, ListType, DictType, BooleanType, PolyModelType
 
 from command.model.configuration import CMDHttpOperation, CMDHttpAction, CMDHttpRequest, CMDHttpRequestPath, \
     CMDHttpRequestQuery, CMDHttpRequestHeader, CMDHttpRequestJsonBody, CMDRequestJson, CMDHttpOperationLongRunning
 from swagger.utils import exceptions
 from swagger.utils.tools import swagger_resource_path_to_resource_id_template
+from .example_item import XmsExamplesField
 from .external_documentation import ExternalDocumentation
-from .fields import MimeField, XmsRequestIdField, XmsExamplesField, SecurityRequirementField, XPublishField, \
+from .fields import MimeField, XmsRequestIdField, SecurityRequirementField, XPublishField, \
     XSfCodeGenField, XmsClientNameField
 from .parameter import ParameterField, PathParameter, QueryParameter, HeaderParameter, BodyParameter,\
     FormDataParameter, ParameterBase
 from .reference import Reference, Linkable
 from .response import Response
 from .schema import ReferenceSchema
 from .x_ms_long_running_operation import XmsLongRunningOperationField, XmsLongRunningOperationOptionsField
 from .x_ms_odata import XmsODataField
 from .x_ms_pageable import XmsPageableField
 
+logger = logging.getLogger('backend')
+
 
 class Operation(Model, Linkable):
     """Describes a single API operation on a path."""
 
     tags = ListType(StringType())  # A list of tags for API documentation control. Tags can be used for logical grouping of operations by resources or any other qualifier.
     summary = StringType()  # A short summary of what the operation does. For maximum readability in the swagger-ui, this field SHOULD be less than 120 characters.
     description = StringType()  # A verbose explanation of the operation behavior. GFM syntax can be used for rich text representation.
@@ -49,15 +53,15 @@
 
     x_ms_pageable = XmsPageableField()  # TODO:
     x_ms_long_running_operation = XmsLongRunningOperationField(default=False)
     x_ms_long_running_operation_options = XmsLongRunningOperationOptionsField()
 
     x_ms_odata = XmsODataField()  # TODO: # indicates the operation includes one or more OData query parameters.
     x_ms_request_id = XmsRequestIdField()
-    x_ms_examples = XmsExamplesField()  # TODO:
+    x_ms_examples = XmsExamplesField()
 
     # specific properties
     _x_publish = XPublishField()  # only used in Maps Data Plane
     _x_sf_codegen = XSfCodeGenField()  # only used in ServiceFabricMesh Mgmt Plane
     _x_ms_client_name = XmsClientNameField()  # only used in Maps Data Plane
 
     def __init__(self, *args, **kwargs):
@@ -129,14 +133,21 @@
             self.x_ms_lro_final_state_schema = ReferenceSchema()
             self.x_ms_lro_final_state_schema.ref = self.x_ms_long_running_operation_options.final_state_schema
             self.x_ms_lro_final_state_schema.link(
                 swagger_loader,
                 *self.traces, "x_ms_long_running_operation_options", "final_state_schema"
             )
 
+        if self.x_ms_examples is not None:
+            for key, example in self.x_ms_examples.items():
+                try:
+                    example.link(swagger_loader, *self.traces, "x_ms_examples", key)
+                except Exception as e:
+                    logger.error(f"Link example failed: {e}: {key}.")
+
     def to_cmd(self, builder, parent_parameters, host_path, **kwargs):
         cmd_op = CMDHttpOperation()
         if self.x_ms_long_running_operation:
             cmd_op.long_running = CMDHttpOperationLongRunning()
             if self.x_ms_long_running_operation_options:
                 cmd_op.long_running.final_state_via = self.x_ms_long_running_operation_options.final_state_via
```

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/parameter.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/parameter.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/path_item.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/path_item.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/reference.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/reference.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/response.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from command.model.configuration import CMDHttpResponse, CMDHttpResponseHeader, CMDHttpResponseJsonBody, \
     CMDObjectSchemaBase, CMDArraySchemaBase, CMDHttpResponseHeaderItem, CMDClsSchemaBase, CMDResponseJson, \
     CMDBooleanSchemaBase, CMDStringSchemaBase, CMDFloatSchemaBase, CMDIntegerSchemaBase
 from swagger.model.schema.fields import MutabilityEnum
 from swagger.utils import exceptions
 from utils.error_format import AAZErrorFormatEnum
-from .fields import XmsExamplesField, XmsErrorResponseField, XNullableField
+from .example_item import XmsExamplesField
+from .fields import XmsErrorResponseField, XNullableField
 from .header import Header
 from .reference import Linkable
 from .schema import Schema, ReferenceSchema, schema_and_reference_schema_claim_function
 
 
 class Response(Model, Linkable):
     """Describes a single response from an API Operation."""
```

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/schema.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/schema.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/security_scheme.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/security_scheme.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/swagger.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/swagger.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/tag.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/tag.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_enum.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_enum.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_odata.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_odata.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_pageable.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_pageable.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/schema/xml.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/schema/xml.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_resource.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_resource_provider.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_resource_provider.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_loader.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_swagger_loader.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_module.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_swagger_module.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_swagger_specs.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_swagger_specs.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/model/specs/_utils.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/model/specs/_utils.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/swagger/utils/tools.py` & `aaz_dev-2.7.0/src/aaz_dev/swagger/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/ui/favicon.ico` & `aaz_dev-2.7.0/src/aaz_dev/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/ui/index.html` & `aaz_dev-2.7.0/src/aaz_dev/ui/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site to manage AAZ"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>AAZDev</title><script defer="defer" src="/static/js/main.aa1f209d.js"></script><link href="/static/css/main.e6c13ad2.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site to manage AAZ"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>AAZDev</title><script defer="defer" src="/static/js/main.90022267.js"></script><link href="/static/css/main.e6c13ad2.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `aaz_dev-2.6.2/src/aaz_dev/ui/logo192.png` & `aaz_dev-2.7.0/src/aaz_dev/ui/logo192.png`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/ui/logo512.png` & `aaz_dev-2.7.0/src/aaz_dev/ui/logo512.png`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/ui/static/css/main.e6c13ad2.css.map` & `aaz_dev-2.7.0/src/aaz_dev/ui/static/css/main.e6c13ad2.css.map`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js` & `aaz_dev-2.7.0/src/aaz_dev/ui/static/js/main.90022267.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.aa1f209d.js.LICENSE.txt */
+/*! For license information please see main.90022267.js.LICENSE.txt */
 (() => {
     var e = {
             76: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     Z: () => oe
                 });
@@ -209,34 +209,34 @@
                 }
                 var D = "-ms-",
                     L = "-moz-",
                     F = "-webkit-",
                     W = "comm",
                     B = "rule",
                     _ = "decl",
-                    V = "@keyframes";
+                    U = "@keyframes";
 
-                function U(e, t) {
+                function V(e, t) {
                     for (var n = "", r = f(e), o = 0; o < r; o++) n += t(e[o], o, e, t) || "";
                     return n
                 }
 
                 function G(e, t, n, r) {
                     switch (e.type) {
                         case "@import":
                         case _:
                             return e.return = e.return || e.value;
                         case W:
                             return "";
-                        case V:
-                            return e.return = e.value + "{" + U(e.children, r) + "}";
+                        case U:
+                            return e.return = e.value + "{" + V(e.children, r) + "}";
                         case B:
                             e.value = e.props.join(",")
                     }
-                    return p(n = U(e.children, r)) ? e.return = e.value + "{" + n + "}" : ""
+                    return p(n = V(e.children, r)) ? e.return = e.value + "{" + n + "}" : ""
                 }
 
                 function q(e, t) {
                     switch (function(e, t) {
                             return (((t << 2 ^ d(e, 0)) << 2 ^ d(e, 1)) << 2 ^ d(e, 2)) << 2 ^ d(e, 3)
                         }(e, t)) {
                         case 5103:
@@ -497,32 +497,32 @@
                         }
                     },
                     re = [function(e, t, n, r) {
                         if (e.length > -1 && !e.return) switch (e.type) {
                             case _:
                                 e.return = q(e.value, e.length);
                                 break;
-                            case V:
-                                return U([S(e, {
+                            case U:
+                                return V([S(e, {
                                     value: l(e.value, "@", "@" + F)
                                 })], r);
                             case B:
                                 if (e.length) return function(e, t) {
                                     return e.map(t).join("")
                                 }(e.props, (function(t) {
                                     switch (function(e, t) {
                                             return (e = t.exec(e)) ? e[0] : e
                                         }(t, /(::plac\w+|:read-\w+)/)) {
                                         case ":read-only":
                                         case ":read-write":
-                                            return U([S(e, {
+                                            return V([S(e, {
                                                 props: [l(t, /:(read-\w+)/, ":" + L + "$1")]
                                             })], r);
                                         case "::placeholder":
-                                            return U([S(e, {
+                                            return V([S(e, {
                                                 props: [l(t, /:(plac\w+)/, ":" + F + "input-$1")]
                                             }), S(e, {
                                                 props: [l(t, /:(plac\w+)/, ":" + L + "$1")]
                                             }), S(e, {
                                                 props: [l(t, /:(plac\w+)/, D + "input-$1")]
                                             })], r)
                                     }
@@ -554,15 +554,15 @@
                             var t = f(e);
                             return function(n, r, o, a) {
                                 for (var i = "", s = 0; s < t; s++) i += e[s](n, r, o, a) || "";
                                 return i
                             }
                         }([te, ne].concat(o, u));
                     i = function(e, t, n, r) {
-                        c = n, U(H(e ? e + "{" + t.styles + "}" : t.styles), p), r && (m.inserted[t.name] = !0)
+                        c = n, V(H(e ? e + "{" + t.styles + "}" : t.styles), p), r && (m.inserted[t.name] = !0)
                     };
                     var m = {
                         key: t,
                         sheet: new r({
                             key: t,
                             container: a,
                             nonce: e.nonce,
@@ -2140,14 +2140,15 @@
                     return (0, r.Z)(e, t)
                 }
             },
             1184: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     L7: () => s,
+                    P$: () => l,
                     VO: () => r,
                     W8: () => i,
                     k9: () => a
                 });
                 const r = {
                         xs: 0,
                         sm: 600,
@@ -2189,14 +2190,36 @@
 
                 function s(e, t) {
                     return e.reduce(((e, t) => {
                         const n = e[t];
                         return (!n || 0 === Object.keys(n).length) && delete e[t], e
                     }), t)
                 }
+
+                function l(e) {
+                    let {
+                        values: t,
+                        breakpoints: n,
+                        base: r
+                    } = e;
+                    const o = r || function(e, t) {
+                            if ("object" !== typeof e) return {};
+                            const n = {},
+                                r = Object.keys(t);
+                            return Array.isArray(e) ? r.forEach(((t, r) => {
+                                r < e.length && (n[t] = !0)
+                            })) : r.forEach((t => {
+                                null != e[t] && (n[t] = !0)
+                            })), n
+                        }(t, n),
+                        a = Object.keys(o);
+                    if (0 === a.length) return t;
+                    let i;
+                    return a.reduce(((e, n, r) => (Array.isArray(t) ? (e[n] = null != t[r] ? t[r] : t[i], i = r) : (e[n] = null != t[n] ? t[n] : t[i] || t, i = n), e)), {})
+                }
             },
             2065: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     $n: () => u,
                     Fq: () => c,
                     _j: () => d,
@@ -2792,28 +2815,28 @@
                     B = (0, r.Z)({
                         prop: "fontWeight",
                         themeKey: "typography"
                     }),
                     _ = (0, r.Z)({
                         prop: "letterSpacing"
                     }),
-                    V = (0, r.Z)({
+                    U = (0, r.Z)({
                         prop: "textTransform"
                     }),
-                    U = (0, r.Z)({
+                    V = (0, r.Z)({
                         prop: "lineHeight"
                     }),
                     G = (0, r.Z)({
                         prop: "textAlign"
                     }),
                     q = a((0, r.Z)({
                         prop: "typography",
                         cssProperty: !1,
                         themeKey: "typography"
-                    }), L, F, W, B, _, U, G, V),
+                    }), L, F, W, B, _, V, G, U),
                     H = {
                         borders: y.filterProps,
                         display: w.filterProps,
                         flexbox: S.filterProps,
                         grid: j.filterProps,
                         positions: P.filterProps,
                         palette: E.filterProps,
@@ -4471,28 +4494,28 @@
                 }
                 var W, B = "function" === typeof Symbol && Symbol.iterator;
 
                 function _(e) {
                     return null === e || "object" !== typeof e ? null : "function" === typeof(e = B && e[B] || e["@@iterator"]) ? e : null
                 }
 
-                function V(e) {
+                function U(e) {
                     if (void 0 === W) try {
                         throw Error()
                     } catch (n) {
                         var t = n.stack.trim().match(/\n( *(at )?)/);
                         W = t && t[1] || ""
                     }
                     return "\n" + W + e
                 }
-                var U = !1;
+                var V = !1;
 
                 function G(e, t) {
-                    if (!e || U) return "";
-                    U = !0;
+                    if (!e || V) return "";
+                    V = !0;
                     var n = Error.prepareStackTrace;
                     Error.prepareStackTrace = void 0;
                     try {
                         if (t)
                             if (t = function() {
                                     throw Error()
                                 }, Object.defineProperty(t.prototype, "props", {
@@ -4531,29 +4554,29 @@
                                         do {
                                             if (i--, 0 > --s || o[i] !== a[s]) return "\n" + o[i].replace(" at new ", " at ")
                                         } while (1 <= i && 0 <= s);
                                     break
                                 }
                         }
                     } finally {
-                        U = !1, Error.prepareStackTrace = n
+                        V = !1, Error.prepareStackTrace = n
                     }
-                    return (e = e ? e.displayName || e.name : "") ? V(e) : ""
+                    return (e = e ? e.displayName || e.name : "") ? U(e) : ""
                 }
 
                 function q(e) {
                     switch (e.tag) {
                         case 5:
-                            return V(e.type);
+                            return U(e.type);
                         case 16:
-                            return V("Lazy");
+                            return U("Lazy");
                         case 13:
-                            return V("Suspense");
+                            return U("Suspense");
                         case 19:
-                            return V("SuspenseList");
+                            return U("SuspenseList");
                         case 0:
                         case 2:
                         case 15:
                             return e = G(e.type, !1);
                         case 11:
                             return e = G(e.type.render, !1);
                         case 22:
@@ -5019,26 +5042,26 @@
                     var c = Array.prototype.slice.call(arguments, 3);
                     try {
                         t.apply(n, c)
                     } catch (d) {
                         this.onError(d)
                     }
                 }
-                var Ve = !1,
-                    Ue = null,
+                var Ue = !1,
+                    Ve = null,
                     Ge = !1,
                     qe = null,
                     He = {
                         onError: function(e) {
-                            Ve = !0, Ue = e
+                            Ue = !0, Ve = e
                         }
                     };
 
                 function $e(e, t, n, r, o, a, i, s, l) {
-                    Ve = !1, Ue = null, _e.apply(He, arguments)
+                    Ue = !1, Ve = null, _e.apply(He, arguments)
                 }
 
                 function Ke(e) {
                     var t = e,
                         n = e;
                     if (e.alternate)
                         for (; t.return;) t = t.return;
@@ -5318,20 +5341,20 @@
                         s = e.pingedLanes;
                     if (0 !== a) r = a, o = Nt = 15;
                     else if (0 !== (a = 134217727 & n)) {
                         var l = a & ~i;
                         0 !== l ? (r = zt(l), o = Nt) : 0 !== (s &= a) && (r = zt(s), o = Nt)
                     } else 0 !== (a = n & ~i) ? (r = zt(a), o = Nt) : 0 !== s && (r = zt(s), o = Nt);
                     if (0 === r) return 0;
-                    if (r = n & ((0 > (r = 31 - Vt(r)) ? 0 : 1 << r) << 1) - 1, 0 !== t && t !== r && 0 === (t & i)) {
+                    if (r = n & ((0 > (r = 31 - Ut(r)) ? 0 : 1 << r) << 1) - 1, 0 !== t && t !== r && 0 === (t & i)) {
                         if (zt(t), o <= Nt) return t;
                         Nt = o
                     }
                     if (0 !== (t = e.entangledLanes))
-                        for (e = e.entanglements, t &= r; 0 < t;) o = 1 << (n = 31 - Vt(t)), r |= e[n], t &= ~o;
+                        for (e = e.entanglements, t &= r; 0 < t;) o = 1 << (n = 31 - Ut(t)), r |= e[n], t &= ~o;
                     return r
                 }
 
                 function Lt(e) {
                     return 0 !== (e = -1073741825 & e.pendingLanes) ? e : 1073741824 & e ? 1073741824 : 0
                 }
 
@@ -5361,20 +5384,20 @@
                     for (var t = [], n = 0; 31 > n; n++) t.push(e);
                     return t
                 }
 
                 function _t(e, t, n) {
                     e.pendingLanes |= t;
                     var r = t - 1;
-                    e.suspendedLanes &= r, e.pingedLanes &= r, (e = e.eventTimes)[t = 31 - Vt(t)] = n
+                    e.suspendedLanes &= r, e.pingedLanes &= r, (e = e.eventTimes)[t = 31 - Ut(t)] = n
                 }
-                var Vt = Math.clz32 ? Math.clz32 : function(e) {
-                        return 0 === e ? 32 : 31 - (Ut(e) / Gt | 0) | 0
+                var Ut = Math.clz32 ? Math.clz32 : function(e) {
+                        return 0 === e ? 32 : 31 - (Vt(e) / Gt | 0) | 0
                     },
-                    Ut = Math.log,
+                    Vt = Math.log,
                     Gt = Math.LN2;
                 var qt = a.unstable_UserBlockingPriority,
                     Ht = a.unstable_runWithPriority,
                     $t = !0;
 
                 function Kt(e, t, n, r) {
                     ze || Ae();
@@ -5705,18 +5728,18 @@
                         case "focusout":
                             return !0;
                         default:
                             return !1
                     }
                 }
 
-                function Vn(e) {
+                function Un(e) {
                     return "object" === typeof(e = e.detail) && "data" in e ? e.data : null
                 }
-                var Un = !1;
+                var Vn = !1;
                 var Gn = {
                     color: !0,
                     date: !0,
                     datetime: !0,
                     "datetime-local": !0,
                     email: !0,
                     month: !0,
@@ -5897,18 +5920,18 @@
                 var Zr = "abort canplay canplaythrough durationchange emptied encrypted ended error loadeddata loadedmetadata loadstart pause play playing progress ratechange seeked seeking stalled suspend timeupdate volumechange waiting".split(" "),
                     jr = new Set("cancel close invalid load scroll toggle".split(" ").concat(Zr));
 
                 function Pr(e, t, n) {
                     var r = e.type || "unknown-event";
                     e.currentTarget = n,
                         function(e, t, n, r, o, a, s, l, c) {
-                            if ($e.apply(this, arguments), Ve) {
-                                if (!Ve) throw Error(i(198));
-                                var d = Ue;
-                                Ve = !1, Ue = null, Ge || (Ge = !0, qe = d)
+                            if ($e.apply(this, arguments), Ue) {
+                                if (!Ue) throw Error(i(198));
+                                var d = Ve;
+                                Ue = !1, Ve = null, Ge || (Ge = !0, qe = d)
                             }
                         }(r, t, void 0, e), e.currentTarget = null
                 }
 
                 function Er(e, t) {
                     t = 0 !== (4 & t);
                     for (var n = 0; n < e.length; n++) {
@@ -6167,31 +6190,31 @@
                                         break e;
                                     case "compositionupdate":
                                         b = "onCompositionUpdate";
                                         break e
                                 }
                                 b = void 0
                             }
-                            else Un ? _n(e, n) && (b = "onCompositionEnd") : "keydown" === e && 229 === n.keyCode && (b = "onCompositionStart");
-                            b && (Fn && "ko" !== n.locale && (Un || "onCompositionStart" !== b ? "onCompositionEnd" === b && Un && (x = nn()) : (en = "value" in (Jt = o) ? Jt.value : Jt.textContent, Un = !0)), 0 < (v = zr(r, b)).length && (b = new Sn(b, e, null, n, o), i.push({
+                            else Vn ? _n(e, n) && (b = "onCompositionEnd") : "keydown" === e && 229 === n.keyCode && (b = "onCompositionStart");
+                            b && (Fn && "ko" !== n.locale && (Vn || "onCompositionStart" !== b ? "onCompositionEnd" === b && Vn && (x = nn()) : (en = "value" in (Jt = o) ? Jt.value : Jt.textContent, Vn = !0)), 0 < (v = zr(r, b)).length && (b = new Sn(b, e, null, n, o), i.push({
                                 event: b,
                                 listeners: v
-                            }), x ? b.data = x : null !== (x = Vn(n)) && (b.data = x))), (x = Ln ? function(e, t) {
+                            }), x ? b.data = x : null !== (x = Un(n)) && (b.data = x))), (x = Ln ? function(e, t) {
                                 switch (e) {
                                     case "compositionend":
-                                        return Vn(t);
+                                        return Un(t);
                                     case "keypress":
                                         return 32 !== t.which ? null : (Bn = !0, Wn);
                                     case "textInput":
                                         return (e = t.data) === Wn && Bn ? null : e;
                                     default:
                                         return null
                                 }
                             }(e, n) : function(e, t) {
-                                if (Un) return "compositionend" === e || !zn && _n(e, t) ? (e = nn(), tn = en = Jt = null, Un = !1, e) : null;
+                                if (Vn) return "compositionend" === e || !zn && _n(e, t) ? (e = nn(), tn = en = Jt = null, Vn = !1, e) : null;
                                 switch (e) {
                                     case "paste":
                                     default:
                                         return null;
                                     case "keypress":
                                         if (!(t.ctrlKey || t.altKey || t.metaKey) || t.ctrlKey && t.altKey) {
                                             if (t.char && 1 < t.char.length) return t.char;
@@ -6260,18 +6283,18 @@
                         case "select":
                         case "textarea":
                             return !!t.autoFocus
                     }
                     return !1
                 }
 
-                function Vr(e, t) {
+                function Ur(e, t) {
                     return "textarea" === e || "option" === e || "noscript" === e || "string" === typeof t.children || "number" === typeof t.children || "object" === typeof t.dangerouslySetInnerHTML && null !== t.dangerouslySetInnerHTML && null != t.dangerouslySetInnerHTML.__html
                 }
-                var Ur = "function" === typeof setTimeout ? setTimeout : void 0,
+                var Vr = "function" === typeof setTimeout ? setTimeout : void 0,
                     Gr = "function" === typeof clearTimeout ? clearTimeout : void 0;
 
                 function qr(e) {
                     1 === e.nodeType ? e.textContent = "" : 9 === e.nodeType && (null != (e = e.body) && (e.textContent = ""))
                 }
 
                 function Hr(e) {
@@ -6414,19 +6437,19 @@
                     zo = a.unstable_IdlePriority,
                     Do = {},
                     Lo = void 0 !== Ro ? Ro : function() {},
                     Fo = null,
                     Wo = null,
                     Bo = !1,
                     _o = Mo(),
-                    Vo = 1e4 > _o ? Mo : function() {
+                    Uo = 1e4 > _o ? Mo : function() {
                         return Mo() - _o
                     };
 
-                function Uo() {
+                function Vo() {
                     switch (Io()) {
                         case To:
                             return 99;
                         case Oo:
                             return 98;
                         case Ao:
                             return 97;
@@ -7034,37 +7057,37 @@
                     return null
                 }
                 var Fa = null,
                     Wa = null,
                     Ba = !1;
 
                 function _a(e, t) {
-                    var n = Ul(5, null, null, 0);
+                    var n = Vl(5, null, null, 0);
                     n.elementType = "DELETED", n.type = "DELETED", n.stateNode = t, n.return = e, n.flags = 8, null !== e.lastEffect ? (e.lastEffect.nextEffect = n, e.lastEffect = n) : e.firstEffect = e.lastEffect = n
                 }
 
-                function Va(e, t) {
+                function Ua(e, t) {
                     switch (e.tag) {
                         case 5:
                             var n = e.type;
                             return null !== (t = 1 !== t.nodeType || n.toLowerCase() !== t.nodeName.toLowerCase() ? null : t) && (e.stateNode = t, !0);
                         case 6:
                             return null !== (t = "" === e.pendingProps || 3 !== t.nodeType ? null : t) && (e.stateNode = t, !0);
                         default:
                             return !1
                     }
                 }
 
-                function Ua(e) {
+                function Va(e) {
                     if (Ba) {
                         var t = Wa;
                         if (t) {
                             var n = t;
-                            if (!Va(e, t)) {
-                                if (!(t = Hr(n.nextSibling)) || !Va(e, t)) return e.flags = -1025 & e.flags | 2, Ba = !1, void(Fa = e);
+                            if (!Ua(e, t)) {
+                                if (!(t = Hr(n.nextSibling)) || !Ua(e, t)) return e.flags = -1025 & e.flags | 2, Ba = !1, void(Fa = e);
                                 _a(Fa, n)
                             }
                             Fa = e, Wa = Hr(t.firstChild)
                         } else e.flags = -1025 & e.flags | 2, Ba = !1, Fa = e
                     }
                 }
 
@@ -7073,15 +7096,15 @@
                     Fa = e
                 }
 
                 function qa(e) {
                     if (e !== Fa) return !1;
                     if (!Ba) return Ga(e), Ba = !0, !1;
                     var t = e.type;
-                    if (5 !== e.tag || "head" !== t && "body" !== t && !Vr(t, e.memoizedProps))
+                    if (5 !== e.tag || "head" !== t && "body" !== t && !Ur(t, e.memoizedProps))
                         for (t = Wa; t;) _a(e, t), t = Hr(t.nextSibling);
                     if (Ga(e), 13 === e.tag) {
                         if (!(e = null !== (e = e.memoizedState) ? e.dehydrated : null)) throw Error(i(317));
                         e: {
                             for (e = e.nextSibling, t = 0; e;) {
                                 if (8 === e.nodeType) {
                                     var n = e.data;
@@ -7273,15 +7296,15 @@
                         subscribe: r
                     }, l.useEffect((function() {
                         f.getSnapshot = n, f.setSnapshot = d;
                         var e = a(t._source);
                         if (!cr(s, e)) {
                             e = n(t._source), cr(u, e) || (d(e), e = fl(g), o.mutableReadLanes |= e & o.pendingLanes), e = o.mutableReadLanes, o.entangledLanes |= e;
                             for (var r = o.entanglements, i = e; 0 < i;) {
-                                var l = 31 - Vt(i),
+                                var l = 31 - Ut(i),
                                     c = 1 << l;
                                 r[l] |= e, i &= ~c
                             }
                         }
                     }), [n, t, r]), l.useEffect((function() {
                         return r(t._source, (function() {
                             var e = f.getSnapshot,
@@ -7393,15 +7416,15 @@
                     var n = li();
                     t = void 0 === t ? null : t;
                     var r = n.memoizedState;
                     return null !== r && null !== t && ai(t, r[1]) ? r[0] : (e = e(), n.memoizedState = [e, t], e)
                 }
 
                 function Ri(e, t) {
-                    var n = Uo();
+                    var n = Vo();
                     qo(98 > n ? 98 : n, (function() {
                         e(!0)
                     })), qo(97 < n ? 97 : n, (function() {
                         var n = Ya.transition;
                         Ya.transition = 1;
                         try {
                             e(!1), t()
@@ -7628,15 +7651,15 @@
                 }
 
                 function Wi(e, t, n, r, o, a) {
                     if (null !== e && ur(e.memoizedProps, r) && e.ref === t.ref) {
                         if (zi = !1, 0 === (a & o)) return t.lanes = e.lanes, as(e, t, a);
                         0 !== (16384 & e.flags) && (zi = !0)
                     }
-                    return Vi(e, t, n, r, a)
+                    return Ui(e, t, n, r, a)
                 }
 
                 function Bi(e, t, n) {
                     var r = t.pendingProps,
                         o = r.children,
                         a = null !== e ? e.memoizedState : null;
                     if ("hidden" === r.mode || "unstable-defer-without-hiding" === r.mode)
@@ -7656,20 +7679,20 @@
                 }
 
                 function _i(e, t) {
                     var n = t.ref;
                     (null === e && null !== n || null !== e && e.ref !== n) && (t.flags |= 128)
                 }
 
-                function Vi(e, t, n, r, o) {
+                function Ui(e, t, n, r, o) {
                     var a = vo(n) ? ho : fo.current;
                     return a = go(t, a), aa(t, o), n = ii(e, t, n, r, a, o), null === e || zi ? (t.flags |= 1, Di(e, t, n, o), t.child) : (t.updateQueue = e.updateQueue, t.flags &= -517, e.lanes &= ~o, as(e, t, o))
                 }
 
-                function Ui(e, t, n, r, o) {
+                function Vi(e, t, n, r, o) {
                     if (vo(n)) {
                         var a = !0;
                         wo(t)
                     } else a = !1;
                     if (aa(t, o), null === t.stateNode) null !== e && (e.alternate = null, t.alternate = null, t.flags |= 2), ba(t, n, r), wa(t, n, r, o), r = !0;
                     else if (null === e) {
                         var i = t.stateNode,
@@ -7711,15 +7734,15 @@
                     retryLane: 0
                 };
 
                 function Qi(e, t, n) {
                     var r, o = t.pendingProps,
                         a = Da.current,
                         i = !1;
-                    return (r = 0 !== (64 & t.flags)) || (r = (null === e || null !== e.memoizedState) && 0 !== (2 & a)), r ? (i = !0, t.flags &= -65) : null !== e && null === e.memoizedState || void 0 === o.fallback || !0 === o.unstable_avoidThisFallback || (a |= 1), uo(Da, 1 & a), null === e ? (void 0 !== o.fallback && Ua(t), e = o.children, a = o.fallback, i ? (e = Ji(t, e, a, n), t.child.memoizedState = {
+                    return (r = 0 !== (64 & t.flags)) || (r = (null === e || null !== e.memoizedState) && 0 !== (2 & a)), r ? (i = !0, t.flags &= -65) : null !== e && null === e.memoizedState || void 0 === o.fallback || !0 === o.unstable_avoidThisFallback || (a |= 1), uo(Da, 1 & a), null === e ? (void 0 !== o.fallback && Va(t), e = o.children, a = o.fallback, i ? (e = Ji(t, e, a, n), t.child.memoizedState = {
                         baseLanes: n
                     }, t.memoizedState = Yi, e) : "number" === typeof o.unstable_expectedLoadTime ? (e = Ji(t, e, a, n), t.child.memoizedState = {
                         baseLanes: n
                     }, t.memoizedState = Yi, t.lanes = 33554432, e) : ((n = Kl({
                         mode: "visible",
                         children: e
                     }, t.mode, n, null)).return = t, t.child = n)) : (e.memoizedState, i ? (o = ts(e, t, o.children, o.fallback, n), i = t.child, a = e.child.memoizedState, i.memoizedState = null === a ? {
@@ -8029,24 +8052,24 @@
                                                     lanes: e.lanes,
                                                     firstContext: e.firstContext
                                                 }), n = n.sibling;
                                                 return uo(Da, 1 & Da.current | 2), t.child
                                             }
                                             e = e.sibling
                                         }
-                                    null !== r.tail && Vo() > qs && (t.flags |= 64, s = !0, is(r, !1), t.lanes = 33554432)
+                                    null !== r.tail && Uo() > qs && (t.flags |= 64, s = !0, is(r, !1), t.lanes = 33554432)
                                 }
                             else {
                                 if (!s)
                                     if (null !== (e = La(c))) {
                                         if (t.flags |= 64, s = !0, null !== (n = e.updateQueue) && (t.updateQueue = n, t.flags |= 4), is(r, !0), null === r.tail && "hidden" === r.tailMode && !c.alternate && !Ba) return null !== (t = t.lastEffect = r.lastEffect) && (t.nextEffect = null), null
-                                    } else 2 * Vo() - r.renderingStartTime > qs && 1073741824 !== n && (t.flags |= 64, s = !0, is(r, !1), t.lanes = 33554432);
+                                    } else 2 * Uo() - r.renderingStartTime > qs && 1073741824 !== n && (t.flags |= 64, s = !0, is(r, !1), t.lanes = 33554432);
                                 r.isBackwards ? (c.sibling = t.child, t.child = c) : (null !== (n = r.last) ? n.sibling = c : t.child = c, r.last = c)
                             }
-                            return null !== r.tail ? (n = r.tail, r.rendering = n, r.tail = n.sibling, r.lastEffect = t.lastEffect, r.renderingStartTime = Vo(), n.sibling = null, t = Da.current, uo(Da, s ? 1 & t | 2 : 1 & t), n) : null;
+                            return null !== r.tail ? (n = r.tail, r.rendering = n, r.tail = n.sibling, r.lastEffect = t.lastEffect, r.renderingStartTime = Uo(), n.sibling = null, t = Da.current, uo(Da, s ? 1 & t | 2 : 1 & t), n) : null;
                         case 23:
                         case 24:
                             return Cl(), null !== e && null !== e.memoizedState !== (null !== t.memoizedState) && "unstable-defer-without-hiding" !== r.mode && (t.flags |= 4), null
                     }
                     throw Error(i(156, t.tag))
                 }
 
@@ -8513,15 +8536,15 @@
                             return;
                         case 6:
                             if (null === t.stateNode) throw Error(i(162));
                             return void(t.stateNode.nodeValue = t.memoizedProps);
                         case 3:
                             return void((n = t.stateNode).hydrate && (n.hydrate = !1, wt(n.containerInfo)));
                         case 13:
-                            return null !== t.memoizedState && (Gs = Vo(), xs(t.child, !0)), void Ps(t);
+                            return null !== t.memoizedState && (Gs = Uo(), xs(t.child, !0)), void Ps(t);
                         case 19:
                             return void Ps(t);
                         case 23:
                         case 24:
                             return void xs(t, null !== t.memoizedState)
                     }
                     throw Error(i(163))
@@ -8552,21 +8575,21 @@
                     zs = 0,
                     Ds = lo(0),
                     Ls = 0,
                     Fs = null,
                     Ws = 0,
                     Bs = 0,
                     _s = 0,
-                    Vs = 0,
-                    Us = null,
+                    Us = 0,
+                    Vs = null,
                     Gs = 0,
                     qs = 1 / 0;
 
                 function Hs() {
-                    qs = Vo() + 500
+                    qs = Uo() + 500
                 }
                 var $s, Ks = null,
                     Xs = !1,
                     Ys = null,
                     Qs = null,
                     Js = !1,
                     el = null,
@@ -8579,26 +8602,26 @@
                     sl = -1,
                     ll = 0,
                     cl = 0,
                     dl = null,
                     ul = !1;
 
                 function pl() {
-                    return 0 !== (48 & Ts) ? Vo() : -1 !== sl ? sl : sl = Vo()
+                    return 0 !== (48 & Ts) ? Uo() : -1 !== sl ? sl : sl = Uo()
                 }
 
                 function fl(e) {
                     if (0 === (2 & (e = e.mode))) return 1;
-                    if (0 === (4 & e)) return 99 === Uo() ? 1 : 2;
+                    if (0 === (4 & e)) return 99 === Vo() ? 1 : 2;
                     if (0 === ll && (ll = Ws), 0 !== Xo.transition) {
-                        0 !== cl && (cl = null !== Us ? Us.pendingLanes : 0), e = ll;
+                        0 !== cl && (cl = null !== Vs ? Vs.pendingLanes : 0), e = ll;
                         var t = 4186112 & ~cl;
                         return 0 === (t &= -t) && (0 === (t = (e = 4186112 & ~e) & -e) && (t = 8192)), t
                     }
-                    return e = Uo(), 0 !== (4 & Ts) && 98 === e ? e = Ft(12, ll) : e = Ft(e = function(e) {
+                    return e = Vo(), 0 !== (4 & Ts) && 98 === e ? e = Ft(12, ll) : e = Ft(e = function(e) {
                         switch (e) {
                             case 99:
                                 return 15;
                             case 98:
                                 return 10;
                             case 97:
                             case 96:
@@ -8611,28 +8634,28 @@
                     }(e), ll), e
                 }
 
                 function ml(e, t, n) {
                     if (50 < al) throw al = 0, il = null, Error(i(185));
                     if (null === (e = hl(e, t))) return null;
                     _t(e, t, n), e === Os && (_s |= t, 4 === Ls && xl(e, Ns));
-                    var r = Uo();
-                    1 === t ? 0 !== (8 & Ts) && 0 === (48 & Ts) ? bl(e) : (gl(e, n), 0 === Ts && (Hs(), $o())) : (0 === (4 & Ts) || 98 !== r && 99 !== r || (null === ol ? ol = new Set([e]) : ol.add(e)), gl(e, n)), Us = e
+                    var r = Vo();
+                    1 === t ? 0 !== (8 & Ts) && 0 === (48 & Ts) ? bl(e) : (gl(e, n), 0 === Ts && (Hs(), $o())) : (0 === (4 & Ts) || 98 !== r && 99 !== r || (null === ol ? ol = new Set([e]) : ol.add(e)), gl(e, n)), Vs = e
                 }
 
                 function hl(e, t) {
                     e.lanes |= t;
                     var n = e.alternate;
                     for (null !== n && (n.lanes |= t), n = e, e = e.return; null !== e;) e.childLanes |= t, null !== (n = e.alternate) && (n.childLanes |= t), n = e, e = e.return;
                     return 3 === n.tag ? n.stateNode : null
                 }
 
                 function gl(e, t) {
                     for (var n = e.callbackNode, r = e.suspendedLanes, o = e.pingedLanes, a = e.expirationTimes, s = e.pendingLanes; 0 < s;) {
-                        var l = 31 - Vt(s),
+                        var l = 31 - Ut(s),
                             c = 1 << l,
                             d = a[l];
                         if (-1 === d) {
                             if (0 === (c & r) || 0 !== (c & o)) {
                                 d = t, zt(c);
                                 var u = Nt;
                                 a[l] = 10 <= u ? d + 250 : 6 <= u ? d + 5e3 : -1
@@ -8690,71 +8713,71 @@
                         Rl();
                         break
                     } catch (l) {
                         Zl(e, l)
                     }
                     if (na(), Ms.current = a, Ts = o, null !== As ? r = 0 : (Os = null, Ns = 0, r = Ls), 0 !== (Ws & _s)) kl(e, 0);
                     else if (0 !== r) {
-                        if (2 === r && (Ts |= 64, e.hydrate && (e.hydrate = !1, qr(e.containerInfo)), 0 !== (n = Lt(e)) && (r = Pl(e, n))), 1 === r) throw t = Fs, kl(e, 0), xl(e, n), gl(e, Vo()), t;
+                        if (2 === r && (Ts |= 64, e.hydrate && (e.hydrate = !1, qr(e.containerInfo)), 0 !== (n = Lt(e)) && (r = Pl(e, n))), 1 === r) throw t = Fs, kl(e, 0), xl(e, n), gl(e, Uo()), t;
                         switch (e.finishedWork = e.current.alternate, e.finishedLanes = n, r) {
                             case 0:
                             case 1:
                                 throw Error(i(345));
                             case 2:
                             case 5:
                                 Tl(e);
                                 break;
                             case 3:
-                                if (xl(e, n), (62914560 & n) === n && 10 < (r = Gs + 500 - Vo())) {
+                                if (xl(e, n), (62914560 & n) === n && 10 < (r = Gs + 500 - Uo())) {
                                     if (0 !== Dt(e, 0)) break;
                                     if (((o = e.suspendedLanes) & n) !== n) {
                                         pl(), e.pingedLanes |= e.suspendedLanes & o;
                                         break
                                     }
-                                    e.timeoutHandle = Ur(Tl.bind(null, e), r);
+                                    e.timeoutHandle = Vr(Tl.bind(null, e), r);
                                     break
                                 }
                                 Tl(e);
                                 break;
                             case 4:
                                 if (xl(e, n), (4186112 & n) === n) break;
                                 for (r = e.eventTimes, o = -1; 0 < n;) {
-                                    var s = 31 - Vt(n);
+                                    var s = 31 - Ut(n);
                                     a = 1 << s, (s = r[s]) > o && (o = s), n &= ~a
                                 }
-                                if (n = o, 10 < (n = (120 > (n = Vo() - n) ? 120 : 480 > n ? 480 : 1080 > n ? 1080 : 1920 > n ? 1920 : 3e3 > n ? 3e3 : 4320 > n ? 4320 : 1960 * Rs(n / 1960)) - n)) {
-                                    e.timeoutHandle = Ur(Tl.bind(null, e), n);
+                                if (n = o, 10 < (n = (120 > (n = Uo() - n) ? 120 : 480 > n ? 480 : 1080 > n ? 1080 : 1920 > n ? 1920 : 3e3 > n ? 3e3 : 4320 > n ? 4320 : 1960 * Rs(n / 1960)) - n)) {
+                                    e.timeoutHandle = Vr(Tl.bind(null, e), n);
                                     break
                                 }
                                 Tl(e);
                                 break;
                             default:
                                 throw Error(i(329))
                         }
                     }
-                    return gl(e, Vo()), e.callbackNode === t ? vl.bind(null, e) : null
+                    return gl(e, Uo()), e.callbackNode === t ? vl.bind(null, e) : null
                 }
 
                 function xl(e, t) {
-                    for (t &= ~Vs, t &= ~_s, e.suspendedLanes |= t, e.pingedLanes &= ~t, e = e.expirationTimes; 0 < t;) {
-                        var n = 31 - Vt(t),
+                    for (t &= ~Us, t &= ~_s, e.suspendedLanes |= t, e.pingedLanes &= ~t, e = e.expirationTimes; 0 < t;) {
+                        var n = 31 - Ut(t),
                             r = 1 << n;
                         e[n] = -1, t &= ~r
                     }
                 }
 
                 function bl(e) {
                     if (0 !== (48 & Ts)) throw Error(i(327));
                     if (Nl(), e === Os && 0 !== (e.expiredLanes & Ns)) {
                         var t = Ns,
                             n = Pl(e, t);
                         0 !== (Ws & _s) && (n = Pl(e, t = Dt(e, t)))
                     } else n = Pl(e, t = Dt(e, 0));
-                    if (0 !== e.tag && 2 === n && (Ts |= 64, e.hydrate && (e.hydrate = !1, qr(e.containerInfo)), 0 !== (t = Lt(e)) && (n = Pl(e, t))), 1 === n) throw n = Fs, kl(e, 0), xl(e, t), gl(e, Vo()), n;
-                    return e.finishedWork = e.current.alternate, e.finishedLanes = t, Tl(e), gl(e, Vo()), null
+                    if (0 !== e.tag && 2 === n && (Ts |= 64, e.hydrate && (e.hydrate = !1, qr(e.containerInfo)), 0 !== (t = Lt(e)) && (n = Pl(e, t))), 1 === n) throw n = Fs, kl(e, 0), xl(e, t), gl(e, Uo()), n;
+                    return e.finishedWork = e.current.alternate, e.finishedLanes = t, Tl(e), gl(e, Uo()), null
                 }
 
                 function yl(e, t) {
                     var n = Ts;
                     Ts |= 1;
                     try {
                         return e(t)
@@ -8809,15 +8832,15 @@
                                     break;
                                 case 23:
                                 case 24:
                                     Cl()
                             }
                             n = n.return
                         }
-                    Os = e, As = ql(e.current, null), Ns = zs = Ws = t, Ls = 0, Fs = null, Vs = _s = Bs = 0
+                    Os = e, As = ql(e.current, null), Ns = zs = Ws = t, Ls = 0, Fs = null, Us = _s = Bs = 0
                 }
 
                 function Zl(e, t) {
                     for (;;) {
                         var n = As;
                         try {
                             if (na(), Xa.current = Ii, ni) {
@@ -8961,15 +8984,15 @@
                         if (null !== (t = t.sibling)) return void(As = t);
                         As = t = e
                     } while (null !== t);
                     0 === Ls && (Ls = 5)
                 }
 
                 function Tl(e) {
-                    var t = Uo();
+                    var t = Vo();
                     return qo(99, Ol.bind(null, e, t)), null
                 }
 
                 function Ol(e, t) {
                     do {
                         Nl()
                     } while (null !== el);
@@ -8979,15 +9002,15 @@
                     if (e.finishedWork = null, e.finishedLanes = 0, n === e.current) throw Error(i(177));
                     e.callbackNode = null;
                     var r = n.lanes | n.childLanes,
                         o = r,
                         a = e.pendingLanes & ~o;
                     e.pendingLanes = o, e.suspendedLanes = 0, e.pingedLanes = 0, e.expiredLanes &= o, e.mutableReadLanes &= o, e.entangledLanes &= o, o = e.entanglements;
                     for (var s = e.eventTimes, l = e.expirationTimes; 0 < a;) {
-                        var c = 31 - Vt(a),
+                        var c = 31 - Ut(a),
                             d = 1 << c;
                         o[c] = 0, s[c] = -1, l[c] = -1, a &= ~d
                     }
                     if (null !== ol && 0 === (24 & r) && ol.has(e) && ol.delete(e), e === Os && (As = Os = null, Ns = 0), 1 < n.flags ? null !== n.lastEffect ? (n.lastEffect.nextEffect = n, r = n.firstEffect) : r = n : r = n.firstEffect, null !== r) {
                         if (o = Ts, Ts |= 32, Is.current = null, Wr = $t, gr(s = hr())) {
                             if ("selectionStart" in s) l = {
                                 start: s.selectionStart,
@@ -9112,15 +9135,15 @@
                     } else e.current = n;
                     if (Js) Js = !1, el = e, tl = t;
                     else
                         for (Ks = r; null !== Ks;) t = Ks.nextEffect, Ks.nextEffect = null, 8 & Ks.flags && ((C = Ks).sibling = null, C.stateNode = null), Ks = t;
                     if (0 === (r = e.pendingLanes) && (Qs = null), 1 === r ? e === il ? al++ : (al = 0, il = e) : al = 0, n = n.stateNode, ko && "function" === typeof ko.onCommitFiberRoot) try {
                         ko.onCommitFiberRoot(Co, n, void 0, 64 === (64 & n.current.flags))
                     } catch (j) {}
-                    if (gl(e, Vo()), Xs) throw Xs = !1, e = Ys, Ys = null, e;
+                    if (gl(e, Uo()), Xs) throw Xs = !1, e = Ys, Ys = null, e;
                     return 0 !== (8 & Ts) || $o(), null
                 }
 
                 function Al() {
                     for (; null !== Ks;) {
                         var e = Ks.alternate;
                         ul || null === dl || (0 !== (8 & Ks.flags) ? Je(Ks, dl) && (ul = !0) : 13 === Ks.tag && Es(e, Ks) && Je(Ks, dl) && (ul = !0));
@@ -9209,37 +9232,37 @@
                             }
                             n = n.return
                         }
                 }
 
                 function Bl(e, t, n) {
                     var r = e.pingCache;
-                    null !== r && r.delete(t), t = pl(), e.pingedLanes |= e.suspendedLanes & n, Os === e && (Ns & n) === n && (4 === Ls || 3 === Ls && (62914560 & Ns) === Ns && 500 > Vo() - Gs ? kl(e, 0) : Vs |= n), gl(e, t)
+                    null !== r && r.delete(t), t = pl(), e.pingedLanes |= e.suspendedLanes & n, Os === e && (Ns & n) === n && (4 === Ls || 3 === Ls && (62914560 & Ns) === Ns && 500 > Uo() - Gs ? kl(e, 0) : Us |= n), gl(e, t)
                 }
 
                 function _l(e, t) {
                     var n = e.stateNode;
-                    null !== n && n.delete(t), 0 === (t = 0) && (0 === (2 & (t = e.mode)) ? t = 1 : 0 === (4 & t) ? t = 99 === Uo() ? 1 : 2 : (0 === ll && (ll = Ws), 0 === (t = Wt(62914560 & ~ll)) && (t = 4194304))), n = pl(), null !== (e = hl(e, t)) && (_t(e, t, n), gl(e, n))
+                    null !== n && n.delete(t), 0 === (t = 0) && (0 === (2 & (t = e.mode)) ? t = 1 : 0 === (4 & t) ? t = 99 === Vo() ? 1 : 2 : (0 === ll && (ll = Ws), 0 === (t = Wt(62914560 & ~ll)) && (t = 4194304))), n = pl(), null !== (e = hl(e, t)) && (_t(e, t, n), gl(e, n))
                 }
 
-                function Vl(e, t, n, r) {
+                function Ul(e, t, n, r) {
                     this.tag = e, this.key = n, this.sibling = this.child = this.return = this.stateNode = this.type = this.elementType = null, this.index = 0, this.ref = null, this.pendingProps = t, this.dependencies = this.memoizedState = this.updateQueue = this.memoizedProps = null, this.mode = r, this.flags = 0, this.lastEffect = this.firstEffect = this.nextEffect = null, this.childLanes = this.lanes = 0, this.alternate = null
                 }
 
-                function Ul(e, t, n, r) {
-                    return new Vl(e, t, n, r)
+                function Vl(e, t, n, r) {
+                    return new Ul(e, t, n, r)
                 }
 
                 function Gl(e) {
                     return !(!(e = e.prototype) || !e.isReactComponent)
                 }
 
                 function ql(e, t) {
                     var n = e.alternate;
-                    return null === n ? ((n = Ul(e.tag, t, e.key, e.mode)).elementType = e.elementType, n.type = e.type, n.stateNode = e.stateNode, n.alternate = e, e.alternate = n) : (n.pendingProps = t, n.type = e.type, n.flags = 0, n.nextEffect = null, n.firstEffect = null, n.lastEffect = null), n.childLanes = e.childLanes, n.lanes = e.lanes, n.child = e.child, n.memoizedProps = e.memoizedProps, n.memoizedState = e.memoizedState, n.updateQueue = e.updateQueue, t = e.dependencies, n.dependencies = null === t ? null : {
+                    return null === n ? ((n = Vl(e.tag, t, e.key, e.mode)).elementType = e.elementType, n.type = e.type, n.stateNode = e.stateNode, n.alternate = e, e.alternate = n) : (n.pendingProps = t, n.type = e.type, n.flags = 0, n.nextEffect = null, n.firstEffect = null, n.lastEffect = null), n.childLanes = e.childLanes, n.lanes = e.lanes, n.child = e.child, n.memoizedProps = e.memoizedProps, n.memoizedState = e.memoizedState, n.updateQueue = e.updateQueue, t = e.dependencies, n.dependencies = null === t ? null : {
                         lanes: t.lanes,
                         firstContext: t.firstContext
                     }, n.sibling = e.sibling, n.index = e.index, n.ref = e.ref, n
                 }
 
                 function Hl(e, t, n, r, o, a) {
                     var s = 2;
@@ -9251,23 +9274,23 @@
                         case z:
                             s = 8, o |= 16;
                             break;
                         case Z:
                             s = 8, o |= 1;
                             break;
                         case j:
-                            return (e = Ul(12, n, t, 8 | o)).elementType = j, e.type = j, e.lanes = a, e;
+                            return (e = Vl(12, n, t, 8 | o)).elementType = j, e.type = j, e.lanes = a, e;
                         case M:
-                            return (e = Ul(13, n, t, o)).type = M, e.elementType = M, e.lanes = a, e;
+                            return (e = Vl(13, n, t, o)).type = M, e.elementType = M, e.lanes = a, e;
                         case I:
-                            return (e = Ul(19, n, t, o)).elementType = I, e.lanes = a, e;
+                            return (e = Vl(19, n, t, o)).elementType = I, e.lanes = a, e;
                         case D:
                             return Kl(n, o, a, t);
                         case L:
-                            return (e = Ul(24, n, t, o)).elementType = L, e.lanes = a, e;
+                            return (e = Vl(24, n, t, o)).elementType = L, e.lanes = a, e;
                         default:
                             if ("object" === typeof e && null !== e) switch (e.$$typeof) {
                                 case P:
                                     s = 10;
                                     break e;
                                 case E:
                                     s = 9;
@@ -9283,31 +9306,31 @@
                                     break e;
                                 case A:
                                     s = 22;
                                     break e
                             }
                             throw Error(i(130, null == e ? e : typeof e, ""))
                     }
-                    return (t = Ul(s, n, t, o)).elementType = e, t.type = r, t.lanes = a, t
+                    return (t = Vl(s, n, t, o)).elementType = e, t.type = r, t.lanes = a, t
                 }
 
                 function $l(e, t, n, r) {
-                    return (e = Ul(7, e, r, t)).lanes = n, e
+                    return (e = Vl(7, e, r, t)).lanes = n, e
                 }
 
                 function Kl(e, t, n, r) {
-                    return (e = Ul(23, e, r, t)).elementType = D, e.lanes = n, e
+                    return (e = Vl(23, e, r, t)).elementType = D, e.lanes = n, e
                 }
 
                 function Xl(e, t, n) {
-                    return (e = Ul(6, e, null, t)).lanes = n, e
+                    return (e = Vl(6, e, null, t)).lanes = n, e
                 }
 
                 function Yl(e, t, n) {
-                    return (t = Ul(4, null !== e.children ? e.children : [], e.key, t)).lanes = n, t.stateNode = {
+                    return (t = Vl(4, null !== e.children ? e.children : [], e.key, t)).lanes = n, t.stateNode = {
                         containerInfo: e.containerInfo,
                         pendingChildren: null,
                         implementation: e.implementation
                     }, t
                 }
 
                 function Ql(e, t, n) {
@@ -9364,15 +9387,15 @@
 
                 function nc(e, t) {
                     tc(e, t), (e = e.alternate) && tc(e, t)
                 }
 
                 function rc(e, t, n) {
                     var r = null != n && null != n.hydrationOptions && n.hydrationOptions.mutableSources || null;
-                    if (n = new Ql(e, t, null != n && !0 === n.hydrate), t = Ul(3, null, null, 2 === t ? 7 : 1 === t ? 3 : 0), n.current = t, t.stateNode = n, la(t), e[Jr] = n.current, Ir(8 === e.nodeType ? e.parentNode : e), r)
+                    if (n = new Ql(e, t, null != n && !0 === n.hydrate), t = Vl(3, null, null, 2 === t ? 7 : 1 === t ? 3 : 0), n.current = t, t.stateNode = n, la(t), e[Jr] = n.current, Ir(8 === e.nodeType ? e.parentNode : e), r)
                         for (e = 0; e < r.length; e++) {
                             var o = (t = r[e])._getVersion;
                             o = o(t._source), null == n.mutableSourceEagerHydrationData ? n.mutableSourceEagerHydrationData = [t, o] : n.mutableSourceEagerHydrationData.push(t, o)
                         }
                     this._internalRoot = n
                 }
 
@@ -9491,49 +9514,49 @@
                                         if (void 0 !== e && null !== e) {
                                             if ((e = e.$$typeof) === R) return 11;
                                             if (e === T) return 14
                                         }
                                         return 2
                                     }(o), e = Yo(o, e), a) {
                                     case 0:
-                                        t = Vi(null, t, o, e, n);
+                                        t = Ui(null, t, o, e, n);
                                         break e;
                                     case 1:
-                                        t = Ui(null, t, o, e, n);
+                                        t = Vi(null, t, o, e, n);
                                         break e;
                                     case 11:
                                         t = Li(null, t, o, e, n);
                                         break e;
                                     case 14:
                                         t = Fi(null, t, o, Yo(o.type, e), r, n);
                                         break e
                                 }
                                 throw Error(i(306, o, ""))
                             }
                             return t;
                         case 0:
-                            return r = t.type, o = t.pendingProps, Vi(e, t, r, o = t.elementType === r ? o : Yo(r, o), n);
-                        case 1:
                             return r = t.type, o = t.pendingProps, Ui(e, t, r, o = t.elementType === r ? o : Yo(r, o), n);
+                        case 1:
+                            return r = t.type, o = t.pendingProps, Vi(e, t, r, o = t.elementType === r ? o : Yo(r, o), n);
                         case 3:
                             if (qi(t), r = t.updateQueue, null === e || null === r) throw Error(i(282));
                             if (r = t.pendingProps, o = null !== (o = t.memoizedState) ? o.element : null, ca(e, t), fa(t, r, null, n), (r = t.memoizedState.element) === o) Ha(), t = as(e, t, n);
                             else {
                                 if ((a = (o = t.stateNode).hydrate) && (Wa = Hr(t.stateNode.containerInfo.firstChild), Fa = t, a = Ba = !0), a) {
                                     if (null != (e = o.mutableSourceEagerHydrationData))
                                         for (o = 0; o < e.length; o += 2)(a = e[o])._workInProgressVersionPrimary = e[o + 1], $a.push(a);
                                     for (n = Pa(t, null, r, n), t.child = n; n;) n.flags = -3 & n.flags | 1024, n = n.sibling
                                 } else Di(e, t, r, n), Ha();
                                 t = t.child
                             }
                             return t;
                         case 5:
-                            return Na(t), null === e && Ua(t), r = t.type, o = t.pendingProps, a = null !== e ? e.memoizedProps : null, s = o.children, Vr(r, o) ? s = null : null !== a && Vr(r, a) && (t.flags |= 16), _i(e, t), Di(e, t, s, n), t.child;
+                            return Na(t), null === e && Va(t), r = t.type, o = t.pendingProps, a = null !== e ? e.memoizedProps : null, s = o.children, Ur(r, o) ? s = null : null !== a && Ur(r, a) && (t.flags |= 16), _i(e, t), Di(e, t, s, n), t.child;
                         case 6:
-                            return null === e && Ua(t), null;
+                            return null === e && Va(t), null;
                         case 13:
                             return Qi(e, t, n);
                         case 4:
                             return Oa(t, t.stateNode.containerInfo), r = t.pendingProps, null === e ? t.child = ja(t, null, r, n) : Di(e, t, r, n), t.child;
                         case 11:
                             return r = t.type, o = t.pendingProps, Li(e, t, r, o = t.elementType === r ? o : Yo(r, o), n);
                         case 7:
@@ -9651,15 +9674,15 @@
                         0 === (Ts = a) && (Hs(), $o())
                     }
                 }, Ae = function() {
                     0 === (49 & Ts) && (function() {
                         if (null !== ol) {
                             var e = ol;
                             ol = null, e.forEach((function(e) {
-                                e.expiredLanes |= 24 & e.pendingLanes, gl(e, Vo())
+                                e.expiredLanes |= 24 & e.pendingLanes, gl(e, Uo())
                             }))
                         }
                         $o()
                     }(), Nl())
                 }, Ne = function(e, t) {
                     var n = Ts;
                     Ts |= 2;
@@ -10976,20 +10999,20 @@
                 children: o,
                 location: h.location,
                 navigationType: h.action,
                 navigator: m
             })
         }
         var _ = n(184);
-        class V extends t.Component {
+        class U extends t.Component {
             render() {
                 return (0, _.jsx)(v, {})
             }
         }
-        const U = V;
+        const V = U;
         var G = n(3366),
             q = n(8182),
             H = n(5917),
             $ = n(104),
             K = n(2466),
             X = n(6001);
         const Y = ["sx"],
@@ -11476,19 +11499,19 @@
             })).forEach((function(e) {
                 r[e.key] = function(e) {
                     return n && (0, t.isValidElement)(e) ? n(e) : e
                 }(e)
             })), r
         }
 
-        function Ve(e, t, n) {
+        function Ue(e, t, n) {
             return null != n[t] ? n[t] : e.props[t]
         }
 
-        function Ue(e, n, r) {
+        function Ve(e, n, r) {
             var o = _e(e.children),
                 a = function(e, t) {
                     function n(n) {
                         return n in t ? t[n] : e[n]
                     }
                     e = e || {}, t = t || {};
                     var r, o = Object.create(null),
@@ -11512,23 +11535,23 @@
                     var l = i in n,
                         c = i in o,
                         d = n[i],
                         u = (0, t.isValidElement)(d) && !d.props.in;
                     !c || l && !u ? c || !l || u ? c && l && (0, t.isValidElement)(d) && (a[i] = (0, t.cloneElement)(s, {
                         onExited: r.bind(null, s),
                         in: d.props.in,
-                        exit: Ve(s, "exit", e),
-                        enter: Ve(s, "enter", e)
+                        exit: Ue(s, "exit", e),
+                        enter: Ue(s, "enter", e)
                     })) : a[i] = (0, t.cloneElement)(s, {
                         in: !1
                     }) : a[i] = (0, t.cloneElement)(s, {
                         onExited: r.bind(null, s),
                         in: !0,
-                        exit: Ve(s, "exit", e),
-                        enter: Ve(s, "enter", e)
+                        exit: Ue(s, "exit", e),
+                        enter: Ue(s, "enter", e)
                     })
                 }
             })), a
         }
         var Ge = Object.values || function(e) {
                 return Object.keys(e).map((function(t) {
                     return e[t]
@@ -11562,19 +11585,19 @@
                     var r, o, a = n.children,
                         i = n.handleExited;
                     return {
                         children: n.firstRender ? (r = e, o = i, _e(r.children, (function(e) {
                             return (0, t.cloneElement)(e, {
                                 onExited: o.bind(null, e),
                                 in: !0,
-                                appear: Ve(e, "appear", r),
-                                enter: Ve(e, "enter", r),
-                                exit: Ve(e, "exit", r)
+                                appear: Ue(e, "appear", r),
+                                enter: Ue(e, "enter", r),
+                                exit: Ue(e, "exit", r)
                             })
-                        }))) : Ue(e, a, i),
+                        }))) : Ve(e, a, i),
                         firstRender: !1
                     }
                 }, r.handleExited = function(e, t) {
                     var n = _e(this.props.children);
                     e.key in n || (e.props.onExited && e.props.onExited(t), this.mounted && this.setState((function(t) {
                         var n = (0, a.Z)({}, t.children);
                         return delete n[e.key], {
@@ -11940,45 +11963,45 @@
                     z = (0, Ne.Z)(N, I),
                     {
                         isFocusVisibleRef: D,
                         onFocus: L,
                         onBlur: F,
                         ref: W
                     } = (0, De.Z)(),
-                    [B, V] = t.useState(!1);
+                    [B, U] = t.useState(!1);
 
-                function U(e, t) {
+                function V(e, t) {
                     let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : p;
                     return (0, ze.Z)((r => {
                         t && t(r);
                         return !n && N.current && N.current[e](r), !0
                     }))
                 }
-                d && B && V(!1), t.useImperativeHandle(o, (() => ({
+                d && B && U(!1), t.useImperativeHandle(o, (() => ({
                     focusVisible: () => {
-                        V(!0), A.current.focus()
+                        U(!0), A.current.focus()
                     }
                 })), []), t.useEffect((() => {
                     B && f && !u && N.current.pulsate()
                 }), [u, f, B]);
-                const H = U("start", C),
-                    $ = U("stop", v),
-                    K = U("stop", x),
-                    X = U("stop", Z),
-                    Y = U("stop", (e => {
+                const H = V("start", C),
+                    $ = V("stop", v),
+                    K = V("stop", x),
+                    X = V("stop", Z),
+                    Y = V("stop", (e => {
                         B && e.preventDefault(), k && k(e)
                     })),
-                    Q = U("start", E),
-                    J = U("stop", j),
-                    ee = U("stop", P),
-                    te = U("stop", (e => {
-                        F(e), !1 === D.current && V(!1), h && h(e)
+                    Q = V("start", E),
+                    J = V("stop", j),
+                    ee = V("stop", P),
+                    te = V("stop", (e => {
+                        F(e), !1 === D.current && U(!1), h && h(e)
                     }), !1),
                     ne = (0, ze.Z)((e => {
-                        A.current || (A.current = e.currentTarget), L(e), !0 === D.current && (V(!0), y && y(e)), b && b(e)
+                        A.current || (A.current = e.currentTarget), L(e), !0 === D.current && (U(!0), y && y(e)), b && b(e)
                     })),
                     re = () => {
                         const e = A.current;
                         return c && "button" !== c && !("A" === e.tagName && e.href)
                     },
                     oe = t.useRef(!1),
                     ae = (0, ze.Z)((e => {
@@ -12332,16 +12355,16 @@
                         }, s.label, {
                             children: o
                         })) : null, d]
                     })]
                 }))
             }));
         _t.muiName = "StepLabel";
-        const Vt = _t;
-        var Ut = n(9103);
+        const Ut = _t;
+        var Vt = n(9103);
 
         function Gt(e) {
             return (0, de.Z)("MuiStepButton", e)
         }
         const qt = (0, ue.Z)("MuiStepButton", ["root", "horizontal", "vertical", "touchRipple"]),
             Ht = ["children", "className", "icon", "optional"],
             $t = (0, se.ZP)(Ct, {
@@ -12405,15 +12428,15 @@
                         };
                         return (0, ie.Z)(r, Gt, t)
                     })(p),
                     m = {
                         icon: s,
                         optional: l
                     },
-                    h = (0, Ut.Z)(o, ["StepLabel"]) ? t.cloneElement(o, m) : (0, _.jsx)(Vt, (0, a.Z)({}, m, {
+                    h = (0, Vt.Z)(o, ["StepLabel"]) ? t.cloneElement(o, m) : (0, _.jsx)(Ut, (0, a.Z)({}, m, {
                         children: o
                     }));
                 return (0, _.jsx)($t, (0, a.Z)({
                     focusRipple: !0,
                     disabled: d,
                     TouchRippleProps: {
                         className: f.touchRipple
@@ -13121,16 +13144,16 @@
                         const o = null == (t = e.components) || null == (n = t.MuiCssBaseline) ? void 0 : n.styleOverrides;
                         return o && (r = [r, o]), r
                     }(e, o)
                 }), r]
             })
         };
         var _n = n(2460),
-            Vn = n(7),
-            Un = n(5519);
+            Un = n(7),
+            Vn = n(5519);
         const Gn = (0, oe.Z)({
                 palette: {
                     primary: {
                         light: "#69696a",
                         main: "#28282a",
                         dark: "#1e1e1f"
                     },
@@ -13150,17 +13173,17 @@
                     },
                     error: {
                         light: _n.Z[50],
                         main: _n.Z[500],
                         dark: _n.Z[700]
                     },
                     success: {
-                        light: Vn.Z[50],
-                        main: Vn.Z[500],
-                        dark: Vn.Z[700]
+                        light: Un.Z[50],
+                        main: Un.Z[500],
+                        dark: Un.Z[700]
                     }
                 },
                 typography: {
                     fontFamily: "'Work Sans', sans-serif",
                     fontSize: 14,
                     fontWeightLight: 300,
                     fontWeightRegular: 400,
@@ -13178,15 +13201,15 @@
             Hn = {
                 ...Gn,
                 palette: {
                     ...Gn.palette,
                     background: {
                         ...Gn.palette.background,
                         default: Gn.palette.common.white,
-                        placeholder: Un.Z[200]
+                        placeholder: Vn.Z[200]
                     }
                 },
                 typography: {
                     ...Gn.typography,
                     fontHeader: qn,
                     h1: {
                         ...Gn.typography.h1,
@@ -13984,16 +14007,16 @@
             let W = y;
             W = e => {
                 const t = y(e);
                 return "string" !== typeof t ? String(t) : t
             };
             const B = t.useRef(!1),
                 _ = t.useRef(!0),
-                V = t.useRef(null),
                 U = t.useRef(null),
+                V = t.useRef(null),
                 [G, q] = t.useState(null),
                 [H, $] = t.useState(-1),
                 K = r ? 0 : -1,
                 X = t.useRef(K),
                 [Y, Q] = (0, kr.Z)({
                     controlled: L,
                     default: u,
@@ -14028,32 +14051,32 @@
                 name: d,
                 state: "open"
             }), [se, le] = t.useState(!0), ce = !P && null != Y && J === W(Y), de = ae && !z, ue = de ? g(N.filter((e => !v || !(P ? Y : [Y]).some((t => null !== t && w(e, t))))), {
                 inputValue: ce && se ? "" : J,
                 getOptionLabel: W
             }) : [], pe = ae && ue.length > 0 && !z;
             const fe = (0, Zr.Z)((e => {
-                -1 === e ? V.current.focus() : G.querySelector('[data-tag-index="'.concat(e, '"]')).focus()
+                -1 === e ? U.current.focus() : G.querySelector('[data-tag-index="'.concat(e, '"]')).focus()
             }));
             t.useEffect((() => {
                 P && H > Y.length - 1 && ($(-1), fe(-1))
             }), [Y, P, H, fe]);
             const me = (0, Zr.Z)((e => {
                     let {
                         event: t,
                         index: n,
                         reason: r = "auto"
                     } = e;
-                    if (X.current = n, -1 === n ? V.current.removeAttribute("aria-activedescendant") : V.current.setAttribute("aria-activedescendant", "".concat(F, "-option-").concat(n)), M && M(t, -1 === n ? null : ue[n], r), !U.current) return;
-                    const o = U.current.querySelector('[role="option"].Mui-focused');
+                    if (X.current = n, -1 === n ? U.current.removeAttribute("aria-activedescendant") : U.current.setAttribute("aria-activedescendant", "".concat(F, "-option-").concat(n)), M && M(t, -1 === n ? null : ue[n], r), !V.current) return;
+                    const o = V.current.querySelector('[role="option"].Mui-focused');
                     o && (o.classList.remove("Mui-focused"), o.classList.remove("Mui-focusVisible"));
-                    const a = U.current.parentElement.querySelector('[role="listbox"]');
+                    const a = V.current.parentElement.querySelector('[role="listbox"]');
                     if (!a) return;
                     if (-1 === n) return void(a.scrollTop = 0);
-                    const i = U.current.querySelector('[data-option-index="'.concat(n, '"]'));
+                    const i = V.current.querySelector('[data-option-index="'.concat(n, '"]'));
                     if (i && (i.classList.add("Mui-focused"), "keyboard" === r && i.classList.add("Mui-focusVisible"), a.scrollHeight > a.clientHeight && "mouse" !== r)) {
                         const e = i,
                             t = a.clientHeight + a.scrollTop,
                             n = e.offsetTop + e.offsetHeight;
                         n > t ? a.scrollTop = n - a.clientHeight : e.offsetTop - e.offsetHeight * (S ? 1.3 : 0) < a.scrollTop && (a.scrollTop = e.offsetTop - e.offsetHeight * (S ? 1.3 : 0))
                     }
                 })),
@@ -14062,19 +14085,19 @@
                         event: t,
                         diff: r,
                         direction: o = "next",
                         reason: a = "auto"
                     } = e;
                     if (!de) return;
                     const i = function(e, t) {
-                        if (!U.current || -1 === e) return -1;
+                        if (!V.current || -1 === e) return -1;
                         let n = e;
                         for (;;) {
                             if ("next" === t && n === ue.length || "previous" === t && -1 === n) return -1;
-                            const e = U.current.querySelector('[data-option-index="'.concat(n, '"]')),
+                            const e = V.current.querySelector('[data-option-index="'.concat(n, '"]')),
                                 r = !m && (!e || e.disabled || "true" === e.getAttribute("aria-disabled"));
                             if (!(e && !e.hasAttribute("tabindex") || r)) return n;
                             n += "next" === t ? 1 : -1
                         }
                     }((() => {
                         const e = ue.length - 1;
                         if ("reset" === r) return K;
@@ -14084,26 +14107,26 @@
                         return t < 0 ? -1 === t && Z ? -1 : h && -1 !== X.current || Math.abs(r) > 1 ? 0 : e : t > e ? t === e + 1 && Z ? -1 : h || Math.abs(r) > 1 ? e : 0 : t
                     })(), o);
                     if (me({
                             index: i,
                             reason: a,
                             event: t
                         }), n && "reset" !== r)
-                        if (-1 === i) V.current.value = J;
+                        if (-1 === i) U.current.value = J;
                         else {
                             const e = W(ue[i]);
-                            V.current.value = e;
-                            0 === e.toLowerCase().indexOf(J.toLowerCase()) && J.length > 0 && V.current.setSelectionRange(J.length, e.length)
+                            U.current.value = e;
+                            0 === e.toLowerCase().indexOf(J.toLowerCase()) && J.length > 0 && U.current.setSelectionRange(J.length, e.length)
                         }
                 })),
                 ge = t.useCallback((() => {
                     if (!de) return;
                     const e = P ? Y[0] : Y;
                     if (0 !== ue.length && null != e) {
-                        if (U.current)
+                        if (V.current)
                             if (null == e) X.current >= ue.length - 1 ? me({
                                 index: ue.length - 1
                             }) : me({
                                 index: X.current
                             });
                             else {
                                 const t = ue[X.current];
@@ -14115,15 +14138,15 @@
                                 })
                             }
                     } else he({
                         diff: "reset"
                     })
                 }), [ue.length, !P && Y, v, he, me, de, J, P]),
                 ve = (0, Zr.Z)((e => {
-                    (0, jr.Z)(U, e), e && ge()
+                    (0, jr.Z)(V, e), e && ge()
                 }));
             t.useEffect((() => {
                 ge()
             }), [ge]);
             const xe = e => {
                     ae || (ie(!0), le(!0), T && T(e))
                 },
@@ -14143,15 +14166,15 @@
                         o = t;
                     if (P) {
                         o = Array.isArray(Y) ? Y.slice() : [];
                         const e = Rr(o, (e => w(t, e))); - 1 === e ? o.push(t) : "freeSolo" !== n && (o.splice(e, 1), r = "removeOption")
                     }
                     re(e, o), ye(e, o, r, {
                         option: t
-                    }), f || e.ctrlKey || e.metaKey || be(e, r), (!0 === i || "touch" === i && we.current || "mouse" === i && !we.current) && V.current.blur()
+                    }), f || e.ctrlKey || e.metaKey || be(e, r), (!0 === i || "touch" === i && we.current || "mouse" === i && !we.current) && U.current.blur()
                 };
             const Ce = (e, t) => {
                     if (!P) return;
                     be(e, "toggleInput");
                     let n = H; - 1 === H ? "" === J && "previous" === t && (n = Y.length - 1) : (n += "next" === t ? 1 : -1, n < 0 && (n = 0), n === Y.length && (n = -1)), n = function(e, t) {
                         if (-1 === e) return -1;
                         let n = e;
@@ -14223,15 +14246,15 @@
                             Ce(t, "next");
                             break;
                         case "Enter":
                             if (-1 !== X.current && de) {
                                 const e = ue[X.current],
                                     r = !!b && b(e);
                                 if (t.preventDefault(), r) return;
-                                Se(t, e, "selectOption"), n && V.current.setSelectionRange(V.current.value.length, V.current.value.length)
+                                Se(t, e, "selectOption"), n && U.current.setSelectionRange(U.current.value.length, U.current.value.length)
                             } else x && "" !== J && !1 === ce && (P && t.preventDefault(), Se(t, J, "createOption", "freeSolo"));
                             break;
                         case "Escape":
                             de ? (t.preventDefault(), t.stopPropagation(), be(t, "escape")) : c && ("" !== J || P && Y.length > 0) && (t.preventDefault(), t.stopPropagation(), ke(t));
                             break;
                         case "Backspace":
                             if (P && !z && "" === J && Y.length > 0) {
@@ -14243,15 +14266,15 @@
                             }
                     }
                 },
                 je = e => {
                     ne(!0), A && !B.current && xe(e)
                 },
                 Pe = e => {
-                    null !== U.current && U.current.parentElement.contains(document.activeElement) ? V.current.focus() : (ne(!1), _.current = !0, B.current = !1, o && -1 !== X.current && de ? Se(e, ue[X.current], "blur") : o && x && "" !== J ? Se(e, J, "blur", "freeSolo") : l && re(e, Y), be(e, "blur"))
+                    null !== V.current && V.current.parentElement.contains(document.activeElement) ? U.current.focus() : (ne(!1), _.current = !0, B.current = !1, o && -1 !== X.current && de ? Se(e, ue[X.current], "blur") : o && x && "" !== J ? Se(e, J, "blur", "freeSolo") : l && re(e, Y), be(e, "blur"))
                 },
                 Ee = e => {
                     const t = e.target.value;
                     J !== t && (ee(t), le(!1), I && I(e, t, "input")), "" === t ? p || P || ye(e, null, "clear") : xe(e)
                 },
                 Re = e => {
                     me({
@@ -14276,15 +14299,15 @@
                 Oe = e => {
                     ae ? be(e, "toggleInput") : xe(e)
                 },
                 Ae = e => {
                     e.target.getAttribute("id") !== F && e.preventDefault()
                 },
                 Ne = () => {
-                    V.current.focus(), D && _.current && V.current.selectionEnd - V.current.selectionStart === 0 && V.current.select(), _.current = !1
+                    U.current.focus(), D && _.current && U.current.selectionEnd - U.current.selectionStart === 0 && U.current.select(), _.current = !1
                 },
                 ze = e => {
                     "" !== J && ae || Oe(e)
                 };
             let De = x && J.length > 0;
             De = De || (P ? Y.length > 0 : null !== Y);
             let Le = ue;
@@ -14323,15 +14346,15 @@
                     onChange: Ee,
                     onMouseDown: ze,
                     "aria-activedescendant": de ? "" : null,
                     "aria-autocomplete": n ? "both" : "list",
                     "aria-controls": pe ? "".concat(F, "-listbox") : void 0,
                     "aria-expanded": pe,
                     autoComplete: "off",
-                    ref: V,
+                    ref: U,
                     autoCapitalize: "none",
                     spellCheck: "false",
                     role: "combobox"
                 }),
                 getClearProps: () => ({
                     tabIndex: -1,
                     onClick: ke
@@ -14439,32 +14462,32 @@
                 bottom: n.bottom / o,
                 left: n.left / r,
                 x: n.left / r,
                 y: n.top / o
             }
         }
 
-        function Vr(e) {
+        function Ur(e) {
             var t = Nr(e);
             return {
                 scrollLeft: t.pageXOffset,
                 scrollTop: t.pageYOffset
             }
         }
 
-        function Ur(e) {
+        function Vr(e) {
             return e ? (e.nodeName || "").toLowerCase() : null
         }
 
         function Gr(e) {
             return ((zr(e) ? e.ownerDocument : e.document) || window.document).documentElement
         }
 
         function qr(e) {
-            return _r(Gr(e)).left + Vr(e).scrollLeft
+            return _r(Gr(e)).left + Ur(e).scrollLeft
         }
 
         function Hr(e) {
             return Nr(e).getComputedStyle(e)
         }
 
         function $r(e) {
@@ -14490,19 +14513,19 @@
                     scrollLeft: 0,
                     scrollTop: 0
                 },
                 l = {
                     x: 0,
                     y: 0
                 };
-            return (r || !r && !n) && (("body" !== Ur(t) || $r(a)) && (s = function(e) {
+            return (r || !r && !n) && (("body" !== Vr(t) || $r(a)) && (s = function(e) {
                 return e !== Nr(e) && Dr(e) ? {
                     scrollLeft: (t = e).scrollLeft,
                     scrollTop: t.scrollTop
-                } : Vr(e);
+                } : Ur(e);
                 var t
             }(t)), Dr(t) ? ((l = _r(t, !0)).x += t.clientLeft, l.y += t.clientTop) : a && (l.x = qr(a))), {
                 x: i.left + s.scrollLeft - l.x,
                 y: i.top + s.scrollTop - l.y,
                 width: i.width,
                 height: i.height
             }
@@ -14517,47 +14540,47 @@
                 y: e.offsetTop,
                 width: n,
                 height: r
             }
         }
 
         function Yr(e) {
-            return "html" === Ur(e) ? e : e.assignedSlot || e.parentNode || (Lr(e) ? e.host : null) || Gr(e)
+            return "html" === Vr(e) ? e : e.assignedSlot || e.parentNode || (Lr(e) ? e.host : null) || Gr(e)
         }
 
         function Qr(e) {
-            return ["html", "body", "#document"].indexOf(Ur(e)) >= 0 ? e.ownerDocument.body : Dr(e) && $r(e) ? e : Qr(Yr(e))
+            return ["html", "body", "#document"].indexOf(Vr(e)) >= 0 ? e.ownerDocument.body : Dr(e) && $r(e) ? e : Qr(Yr(e))
         }
 
         function Jr(e, t) {
             var n;
             void 0 === t && (t = []);
             var r = Qr(e),
                 o = r === (null == (n = e.ownerDocument) ? void 0 : n.body),
                 a = Nr(r),
                 i = o ? [a].concat(a.visualViewport || [], $r(r) ? r : []) : r,
                 s = t.concat(i);
             return o ? s : s.concat(Jr(Yr(i)))
         }
 
         function eo(e) {
-            return ["table", "td", "th"].indexOf(Ur(e)) >= 0
+            return ["table", "td", "th"].indexOf(Vr(e)) >= 0
         }
 
         function to(e) {
             return Dr(e) && "fixed" !== Hr(e).position ? e.offsetParent : null
         }
 
         function no(e) {
             for (var t = Nr(e), n = to(e); n && eo(n) && "static" === Hr(n).position;) n = to(n);
-            return n && ("html" === Ur(n) || "body" === Ur(n) && "static" === Hr(n).position) ? t : n || function(e) {
+            return n && ("html" === Vr(n) || "body" === Vr(n) && "static" === Hr(n).position) ? t : n || function(e) {
                 var t = -1 !== navigator.userAgent.toLowerCase().indexOf("firefox");
                 if (-1 !== navigator.userAgent.indexOf("Trident") && Dr(e) && "fixed" === Hr(e).position) return null;
                 var n = Yr(e);
-                for (Lr(n) && (n = n.host); Dr(n) && ["html", "body"].indexOf(Ur(n)) < 0;) {
+                for (Lr(n) && (n = n.host); Dr(n) && ["html", "body"].indexOf(Vr(n)) < 0;) {
                     var r = Hr(n);
                     if ("none" !== r.transform || "none" !== r.perspective || "paint" === r.contain || -1 !== ["transform", "perspective"].indexOf(r.willChange) || t && "filter" === r.willChange || t && r.filter && "none" !== r.filter) return n;
                     n = n.parentNode
                 }
                 return null
             }(e) || t
         }
@@ -14879,15 +14902,15 @@
             phase: "write",
             fn: function(e) {
                 var t = e.state;
                 Object.keys(t.elements).forEach((function(e) {
                     var n = t.styles[e] || {},
                         r = t.attributes[e] || {},
                         o = t.elements[e];
-                    Dr(o) && Ur(o) && (Object.assign(o.style, n), Object.keys(r).forEach((function(e) {
+                    Dr(o) && Vr(o) && (Object.assign(o.style, n), Object.keys(r).forEach((function(e) {
                         var t = r[e];
                         !1 === t ? o.removeAttribute(e) : o.setAttribute(e, !0 === t ? "" : t)
                     })))
                 }))
             },
             effect: function(e) {
                 var t = e.state,
@@ -14907,15 +14930,15 @@
                     function() {
                         Object.keys(t.elements).forEach((function(e) {
                             var r = t.elements[e],
                                 o = t.attributes[e] || {},
                                 a = Object.keys(t.styles.hasOwnProperty(e) ? t.styles[e] : n[e]).reduce((function(e, t) {
                                     return e[t] = "", e
                                 }), {});
-                            Dr(r) && Ur(r) && (Object.assign(r.style, a), Object.keys(o).forEach((function(e) {
+                            Dr(r) && Vr(r) && (Object.assign(r.style, a), Object.keys(o).forEach((function(e) {
                                 r.removeAttribute(e)
                             })))
                         }))
                     }
             },
             requires: ["computeStyles"]
         };
@@ -15015,15 +15038,15 @@
                     y: s
                 }
             }(e)) : zr(t) ? function(e) {
                 var t = _r(e);
                 return t.top = t.top + e.clientTop, t.left = t.left + e.clientLeft, t.bottom = t.top + e.clientHeight, t.right = t.left + e.clientWidth, t.width = e.clientWidth, t.height = e.clientHeight, t.x = t.left, t.y = t.top, t
             }(t) : Lo(function(e) {
                 var t, n = Gr(e),
-                    r = Vr(e),
+                    r = Ur(e),
                     o = null == (t = e.ownerDocument) ? void 0 : t.body,
                     a = Fr(n.scrollWidth, n.clientWidth, o ? o.scrollWidth : 0, o ? o.clientWidth : 0),
                     i = Fr(n.scrollHeight, n.clientHeight, o ? o.scrollHeight : 0, o ? o.clientHeight : 0),
                     s = -r.scrollLeft + qr(e),
                     l = -r.scrollTop;
                 return "rtl" === Hr(o || n).direction && (s += Fr(n.clientWidth, o ? o.clientWidth : 0) - a), {
                     width: a,
@@ -15035,15 +15058,15 @@
         }
 
         function Wo(e, t, n) {
             var r = "clippingParents" === t ? function(e) {
                     var t = Jr(Yr(e)),
                         n = ["absolute", "fixed"].indexOf(Hr(e).position) >= 0 && Dr(e) ? no(e) : e;
                     return zr(n) ? t.filter((function(e) {
-                        return zr(e) && Do(e, n) && "body" !== Ur(e)
+                        return zr(e) && Do(e, n) && "body" !== Vr(e)
                     })) : []
                 }(e) : [].concat(t),
                 o = [].concat(r, [n]),
                 a = o[0],
                 i = o.reduce((function(t, n) {
                     var r = Fo(e, n);
                     return t.top = Fr(r.top, t.top), t.right = Wr(r.right, t.right), t.bottom = Wr(r.bottom, t.bottom), t.left = Fr(r.left, t.left), t
@@ -15062,15 +15085,15 @@
 
         function _o(e, t) {
             return t.reduce((function(t, n) {
                 return t[n] = e, t
             }), {})
         }
 
-        function Vo(e, t) {
+        function Uo(e, t) {
             void 0 === t && (t = {});
             var n = t,
                 r = n.placement,
                 o = void 0 === r ? e.placement : r,
                 a = n.boundary,
                 i = void 0 === a ? po : a,
                 s = n.rootBoundary,
@@ -15109,15 +15132,15 @@
                         n = [ro, oo].indexOf(e) >= 0 ? "y" : "x";
                     k[e] += j[n] * t
                 }))
             }
             return k
         }
 
-        function Uo(e, t, n) {
+        function Vo(e, t, n) {
             return Fr(e, Wr(t, n))
         }
         const Go = {
             name: "preventOverflow",
             enabled: !0,
             phase: "main",
             fn: function(e) {
@@ -15132,15 +15155,15 @@
                     c = n.rootBoundary,
                     d = n.altBoundary,
                     u = n.padding,
                     p = n.tether,
                     f = void 0 === p || p,
                     m = n.tetherOffset,
                     h = void 0 === m ? 0 : m,
-                    g = Vo(t, {
+                    g = Uo(t, {
                         boundary: l,
                         rootBoundary: c,
                         padding: u,
                         altBoundary: d
                     }),
                     v = Zo(t.placement),
                     x = jo(t.placement),
@@ -15184,40 +15207,40 @@
                             B = t.modifiersData["arrow#persistent"] ? t.modifiersData["arrow#persistent"].padding : {
                                 top: 0,
                                 right: 0,
                                 bottom: 0,
                                 left: 0
                             },
                             _ = B[M],
-                            V = B[I],
-                            U = Uo(0, C[T], W[T]),
-                            G = b ? C[T] / 2 - z - U - _ - j.mainAxis : D - U - _ - j.mainAxis,
-                            q = b ? -C[T] / 2 + z + U + V + j.mainAxis : L + U + V + j.mainAxis,
+                            U = B[I],
+                            V = Vo(0, C[T], W[T]),
+                            G = b ? C[T] / 2 - z - V - _ - j.mainAxis : D - V - _ - j.mainAxis,
+                            q = b ? -C[T] / 2 + z + V + U + j.mainAxis : L + V + U + j.mainAxis,
                             H = t.elements.arrow && no(t.elements.arrow),
                             $ = H ? "y" === y ? H.clientTop || 0 : H.clientLeft || 0 : 0,
                             K = null != (R = null == P ? void 0 : P[y]) ? R : 0,
                             X = O + q - K,
-                            Y = Uo(f ? Wr(A, O + G - K - $) : A, O, f ? Fr(N, X) : N);
+                            Y = Vo(f ? Wr(A, O + G - K - $) : A, O, f ? Fr(N, X) : N);
                         S[y] = Y, E[y] = Y - O
                     }
                     if (s) {
                         var Q, J = "x" === y ? ro : io,
                             ee = "x" === y ? oo : ao,
                             te = S[w],
                             ne = "y" === w ? "height" : "width",
                             re = te + g[J],
                             oe = te - g[ee],
                             ae = -1 !== [ro, io].indexOf(v),
                             ie = null != (Q = null == P ? void 0 : P[w]) ? Q : 0,
                             se = ae ? re : te - C[ne] - k[ne] - ie + j.altAxis,
                             le = ae ? te + C[ne] + k[ne] - ie - j.altAxis : oe,
                             ce = f && ae ? function(e, t, n) {
-                                var r = Uo(e, t, n);
+                                var r = Vo(e, t, n);
                                 return r > n ? n : r
-                            }(se, te, le) : Uo(f ? se : re, te, f ? le : oe);
+                            }(se, te, le) : Vo(f ? se : re, te, f ? le : oe);
                         S[w] = ce, E[w] = ce - te
                     }
                     t.modifiersData[r] = E
                 }
             },
             requiresIfExists: ["offset"]
         };
@@ -15247,15 +15270,15 @@
                         h = i[l] - n.rects.reference[l],
                         g = no(a),
                         v = g ? "y" === l ? g.clientHeight || 0 : g.clientWidth || 0 : 0,
                         x = m / 2 - h / 2,
                         b = d[p],
                         y = v - u[c] - d[f],
                         w = v / 2 - u[c] / 2 + x,
-                        S = Uo(b, w, y),
+                        S = Vo(b, w, y),
                         C = l;
                     n.modifiersData[r] = ((t = {})[C] = S, t.centerOffset = S - w, t)
                 }
             },
             effect: function(e) {
                 var t = e.state,
                     n = e.options.element,
@@ -15389,15 +15412,15 @@
                                             return jo(e) === d
                                         })) : lo,
                                         p = u.filter((function(e) {
                                             return c.indexOf(e) >= 0
                                         }));
                                     0 === p.length && (p = u);
                                     var f = p.reduce((function(t, n) {
-                                        return t[n] = Vo(e, {
+                                        return t[n] = Uo(e, {
                                             placement: n,
                                             boundary: o,
                                             rootBoundary: a,
                                             padding: i
                                         })[Zo(n)], t
                                     }), {});
                                     return Object.keys(f).sort((function(e, t) {
@@ -15413,15 +15436,15 @@
                                 }) : n)
                             }), []), y = t.rects.reference, w = t.rects.popper, S = new Map, C = !0, k = b[0], Z = 0; Z < b.length; Z++) {
                             var j = b[Z],
                                 P = Zo(j),
                                 E = jo(j) === co,
                                 R = [ro, oo].indexOf(P) >= 0,
                                 M = R ? "width" : "height",
-                                I = Vo(t, {
+                                I = Uo(t, {
                                     placement: j,
                                     boundary: d,
                                     rootBoundary: u,
                                     altBoundary: p,
                                     padding: c
                                 }),
                                 T = R ? E ? ao : io : E ? oo : ro;
@@ -15462,18 +15485,18 @@
                 requiresIfExists: ["preventOverflow"],
                 fn: function(e) {
                     var t = e.state,
                         n = e.name,
                         r = t.rects.reference,
                         o = t.rects.popper,
                         a = t.modifiersData.preventOverflow,
-                        i = Vo(t, {
+                        i = Uo(t, {
                             elementContext: "reference"
                         }),
-                        s = Vo(t, {
+                        s = Uo(t, {
                             altBoundary: !0
                         }),
                         l = Ho(i, r),
                         c = Ho(s, o, a),
                         d = $o(l),
                         u = $o(c);
                     t.modifiersData[n] = {
@@ -16393,15 +16416,15 @@
                 return (0, a.Z)({
                     padding: 2,
                     marginRight: -2
                 }, t.popupOpen && {
                     transform: "rotate(180deg)"
                 })
             })),
-            Va = (0, se.ZP)(ia, {
+            Ua = (0, se.ZP)(ia, {
                 name: "MuiAutocomplete",
                 slot: "Popper",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
                     return [{
@@ -16415,15 +16438,15 @@
                 } = e;
                 return (0, a.Z)({
                     zIndex: t.zIndex.modal
                 }, n.disablePortal && {
                     position: "absolute"
                 })
             })),
-            Ua = (0, se.ZP)(Jn, {
+            Va = (0, se.ZP)(Jn, {
                 name: "MuiAutocomplete",
                 slot: "Paper",
                 overridesResolver: (e, t) => t.paper
             })((e => {
                 let {
                     theme: t
                 } = e;
@@ -16582,16 +16605,16 @@
                         limitTags: N = -1,
                         ListboxComponent: z = "ul",
                         ListboxProps: D,
                         loading: L = !1,
                         loadingText: F = "Loading\u2026",
                         multiple: W = !1,
                         noOptionsText: B = "No options",
-                        openOnFocus: V = !1,
-                        openText: U = "Open",
+                        openOnFocus: U = !1,
+                        openText: V = "Open",
                         PaperComponent: H = Jn,
                         PopperComponent: $ = ia,
                         popupIcon: K = Da || (Da = (0, _.jsx)(Oa, {})),
                         readOnly: X = !1,
                         renderGroup: Y,
                         renderInput: Q,
                         renderOption: J,
@@ -16735,40 +16758,40 @@
                                         title: g,
                                         ownerState: Pe
                                     }, x.clearIndicator, {
                                         className: (0, q.Z)(Ee.clearIndicator, null == (r = x.clearIndicator) ? void 0 : r.className),
                                         children: f
                                     })) : null, je ? (0, _.jsx)(_a, (0, a.Z)({}, de(), {
                                         disabled: S,
-                                        "aria-label": xe ? v : U,
-                                        title: xe ? v : U,
+                                        "aria-label": xe ? v : V,
+                                        title: xe ? v : V,
                                         className: (0, q.Z)(Ee.popupIndicator),
                                         ownerState: Pe,
                                         children: K
                                     })) : null]
                                 })
                             },
                             inputProps: (0, a.Z)({
                                 className: (0, q.Z)(Ee.input),
                                 disabled: S,
                                 readOnly: X
                             }, ae())
                         })
-                    })), xe && we ? (0, _.jsx)(Va, {
+                    })), xe && we ? (0, _.jsx)(Ua, {
                         as: $,
                         className: (0, q.Z)(Ee.popper),
                         disablePortal: Z,
                         style: {
                             width: we ? we.clientWidth : null
                         },
                         ownerState: Pe,
                         role: "presentation",
                         anchorEl: we,
                         open: !0,
-                        children: (0, _.jsxs)(Ua, (0, a.Z)({
+                        children: (0, _.jsxs)(Va, (0, a.Z)({
                             ownerState: Pe,
                             as: H
                         }, x.paper, {
                             className: (0, q.Z)(Ee.paper, null == (o = x.paper) ? void 0 : o.className),
                             children: [L && 0 === ke.length ? (0, _.jsx)(Ga, {
                                 className: Ee.loading,
                                 ownerState: Pe,
@@ -17090,17 +17113,17 @@
                     {
                         current: F
                     } = t.useRef(null != L),
                     W = t.useRef(),
                     B = t.useCallback((e => {
                         0
                     }), []),
-                    V = (0, Ne.Z)(x.ref, B),
-                    U = (0, Ne.Z)(b, V),
-                    H = (0, Ne.Z)(W, U),
+                    U = (0, Ne.Z)(x.ref, B),
+                    V = (0, Ne.Z)(b, U),
+                    H = (0, Ne.Z)(W, V),
                     [$, K] = t.useState(!1),
                     X = li();
                 const Y = ii({
                     props: r,
                     muiFormControl: X,
                     states: ["color", "disabled", "error", "hiddenLabel", "size", "required", "filled"]
                 });
@@ -17776,15 +17799,15 @@
         const Fi = Li;
 
         function Wi(e) {
             return (0, de.Z)("MuiFormLabel", e)
         }
         const Bi = (0, ue.Z)("MuiFormLabel", ["root", "colorSecondary", "focused", "disabled", "error", "filled", "required", "asterisk"]),
             _i = ["children", "className", "color", "component", "disabled", "error", "filled", "focused", "required"],
-            Vi = (0, se.ZP)("label", {
+            Ui = (0, se.ZP)("label", {
                 name: "MuiFormLabel",
                 slot: "Root",
                 overridesResolver: (e, t) => {
                     let {
                         ownerState: n
                     } = e;
                     return (0, a.Z)({}, t.root, "secondary" === n.color && t.colorSecondary, n.filled && t.filled)
@@ -17807,15 +17830,15 @@
                         color: t.palette.text.disabled
                     },
                     ["&.".concat(Bi.error)]: {
                         color: t.palette.error.main
                     }
                 })
             })),
-            Ui = (0, se.ZP)("span", {
+            Vi = (0, se.ZP)("span", {
                 name: "MuiFormLabel",
                 slot: "Asterisk",
                 overridesResolver: (e, t) => t.asterisk
             })((e => {
                 let {
                     theme: t
                 } = e;
@@ -17861,21 +17884,21 @@
                             required: s
                         } = e, l = {
                             root: ["root", "color".concat((0, ce.Z)(n)), o && "disabled", a && "error", i && "filled", r && "focused", s && "required"],
                             asterisk: ["asterisk", a && "error"]
                         };
                         return (0, ie.Z)(l, Wi, t)
                     })(c);
-                return (0, _.jsxs)(Vi, (0, a.Z)({
+                return (0, _.jsxs)(Ui, (0, a.Z)({
                     as: i,
                     ownerState: c,
                     className: (0, q.Z)(d.root, o),
                     ref: t
                 }, s, {
-                    children: [r, l.required && (0, _.jsxs)(Ui, {
+                    children: [r, l.required && (0, _.jsxs)(Vi, {
                         ownerState: c,
                         "aria-hidden": !0,
                         className: d.asterisk,
                         children: ["\u2009", "*"]
                     })]
                 }))
             }));
@@ -18080,23 +18103,23 @@
                             root: ["root", "none" !== n && "margin".concat((0, ce.Z)(n)), r && "fullWidth"]
                         };
                         return (0, ie.Z)(o, Xi, t)
                     })(b),
                     [w, S] = t.useState((() => {
                         let e = !1;
                         return o && t.Children.forEach(o, (t => {
-                            if (!(0, Ut.Z)(t, ["Input", "Select"])) return;
-                            const n = (0, Ut.Z)(t, ["Select"]) ? t.props.input : t;
+                            if (!(0, Vt.Z)(t, ["Input", "Select"])) return;
+                            const n = (0, Vt.Z)(t, ["Select"]) ? t.props.input : t;
                             n && n.props.startAdornment && (e = !0)
                         })), e
                     })),
                     [C, k] = t.useState((() => {
                         let e = !1;
                         return o && t.Children.forEach(o, (t => {
-                            (0, Ut.Z)(t, ["Input", "Select"]) && ui(t.props, !0) && (e = !0)
+                            (0, Vt.Z)(t, ["Input", "Select"]) && ui(t.props, !0) && (e = !0)
                         })), e
                     })),
                     [Z, j] = t.useState(!1);
                 c && Z && j(!1);
                 const P = void 0 === u || c ? Z : u;
                 const E = t.useCallback((() => {
                         k(!0)
@@ -18792,24 +18815,24 @@
                         disableScrollLock: b
                     }), N.current.scrollTop = 0
                 }, W = (0, Zr.Z)((() => {
                     const e = function(e) {
                         return "function" === typeof e ? e() : e
                     }(f) || (0, Ar.Z)(A.current).body;
                     S.add(L(), e), N.current && F()
-                })), B = t.useCallback((() => S.isTopModal(L())), [S]), V = (0, Zr.Z)((e => {
+                })), B = t.useCallback((() => S.isTopModal(L())), [S]), U = (0, Zr.Z)((e => {
                     A.current = e, e && (j && B() ? F() : Rs(N.current, !0))
-                })), U = t.useCallback((() => {
+                })), V = t.useCallback((() => {
                     S.remove(L())
                 }), [S]);
                 t.useEffect((() => () => {
-                    U()
-                }), [U]), t.useEffect((() => {
-                    j ? W() : D && c || U()
-                }), [j, U, D, c, W]);
+                    V()
+                }), [V]), t.useEffect((() => {
+                    j ? W() : D && c || V()
+                }), [j, V, D, c, W]);
                 const H = (0, a.Z)({}, e, {
                         classes: s,
                         closeAfterTransition: c,
                         disableAutoFocus: m,
                         disableEnforceFocus: h,
                         disableEscapeKeyDown: g,
                         disablePortal: v,
@@ -18830,22 +18853,22 @@
                         return (0, ie.Z)(o, Ls, r)
                     })(H);
                 if (!w && !j && (!D || I)) return null;
                 const K = () => {
                         T(!1), E && E()
                     },
                     X = () => {
-                        T(!0), R && R(), c && U()
+                        T(!0), R && R(), c && V()
                     },
                     Y = {};
                 void 0 === i.props.tabIndex && (Y.tabIndex = "-1"), D && (Y.onEnter = (0, Es.Z)(K, i.props.onEnter), Y.onExited = (0, Es.Z)(X, i.props.onExited));
                 const Q = u.Root || d,
                     J = p.root || {};
                 return (0, _.jsx)(Xo, {
-                    ref: V,
+                    ref: U,
                     container: f,
                     disablePortal: v,
                     children: (0, _.jsxs)(Q, (0, a.Z)({
                         role: "presentation"
                     }, J, !ai(Q) && {
                         as: d,
                         ownerState: (0, a.Z)({}, H, J.ownerState),
@@ -18870,38 +18893,38 @@
                             children: t.cloneElement(i, Y)
                         })]
                     }))
                 })
             })),
             _s = Bs;
 
-        function Vs(e) {
+        function Us(e) {
             return (0, de.Z)("MuiBackdrop", e)
         }(0, ue.Z)("MuiBackdrop", ["root", "invisible"]);
-        const Us = ["classes", "className", "invisible", "component", "components", "componentsProps", "theme"],
+        const Vs = ["classes", "className", "invisible", "component", "components", "componentsProps", "theme"],
             Gs = t.forwardRef((function(e, t) {
                 const {
                     classes: n,
                     className: r,
                     invisible: o = !1,
                     component: i = "div",
                     components: s = {},
                     componentsProps: l = {},
                     theme: c
-                } = e, d = (0, G.Z)(e, Us), u = (0, a.Z)({}, e, {
+                } = e, d = (0, G.Z)(e, Vs), u = (0, a.Z)({}, e, {
                     classes: n,
                     invisible: o
                 }), p = (e => {
                     const {
                         classes: t,
                         invisible: n
                     } = e, r = {
                         root: ["root", n && "invisible"]
                     };
-                    return (0, ie.Z)(r, Vs, t)
+                    return (0, ie.Z)(r, Us, t)
                 })(u), f = s.Root || i, m = l.root || {};
                 return (0, _.jsx)(f, (0, a.Z)({
                     "aria-hidden": !0
                 }, m, !ai(f) && {
                     as: i,
                     ownerState: (0, a.Z)({}, u, m.ownerState),
                     theme: c
@@ -19688,15 +19711,15 @@
         function Bl(e, t) {
             return "object" === typeof t && null !== t ? e === t : String(e) === String(t)
         }
 
         function _l(e) {
             return null == e || "string" === typeof e && !e.trim()
         }
-        const Vl = t.forwardRef((function(e, n) {
+        const Ul = t.forwardRef((function(e, n) {
             const {
                 "aria-describedby": r,
                 "aria-label": o,
                 autoFocus: i,
                 autoWidth: s,
                 children: l,
                 className: c,
@@ -19728,25 +19751,25 @@
                 name: "Select"
             }), [N, z] = (0, Ol.Z)({
                 controlled: Z,
                 default: d,
                 name: "Select"
             }), D = t.useRef(null), L = t.useRef(null), [F, W] = t.useState(null), {
                 current: B
-            } = t.useRef(null != Z), [V, U] = t.useState(), H = (0, Ne.Z)(n, h), $ = t.useCallback((e => {
+            } = t.useRef(null != Z), [U, V] = t.useState(), H = (0, Ne.Z)(n, h), $ = t.useCallback((e => {
                 L.current = e, e && W(e)
             }), []);
             t.useImperativeHandle(H, (() => ({
                 focus: () => {
                     L.current.focus()
                 },
                 node: D.current,
                 value: O
             })), [O]), t.useEffect((() => {
-                d && N && F && !B && (U(s ? null : F.clientWidth), L.current.focus())
+                d && N && F && !B && (V(s ? null : F.clientWidth), L.current.focus())
             }), [F, s]), t.useEffect((() => {
                 i && L.current.focus()
             }), [i]), t.useEffect((() => {
                 if (!g) return;
                 const e = (0, is.Z)(L.current).getElementById(g);
                 if (e) {
                     const t = () => {
@@ -19754,15 +19777,15 @@
                     };
                     return e.addEventListener("click", t), () => {
                         e.removeEventListener("click", t)
                     }
                 }
             }), [g]);
             const K = (e, t) => {
-                    e ? k && k(t) : S && S(t), B || (U(s ? null : F.clientWidth), z(e))
+                    e ? k && k(t) : S && S(t), B || (V(s ? null : F.clientWidth), z(e))
                 },
                 X = t.Children.toArray(l),
                 Y = e => t => {
                     let n;
                     if (t.currentTarget.hasAttribute("tabindex")) {
                         if (x) {
                             n = Array.isArray(O) ? O.slice() : [];
@@ -19807,15 +19830,15 @@
                     role: "option",
                     selected: n,
                     value: void 0,
                     "data-value": e.props.value
                 })
             }));
             ne && (J = x ? 0 === te.length ? null : te.reduce(((e, t, n) => (e.push(t), n < te.length - 1 && e.push(", "), e)), []) : ee);
-            let ae, se = V;
+            let ae, se = U;
             !s && B && F && (se = F.clientWidth), ae = "undefined" !== typeof R ? R : p ? null : 0;
             const le = E.id || (b ? "mui-component-select-".concat(b) : void 0),
                 de = (0, a.Z)({}, e, {
                     variant: I,
                     value: O,
                     open: Q
                 }),
@@ -19916,15 +19939,15 @@
                             minWidth: se
                         }, null != v.PaperProps ? v.PaperProps.style : null)
                     }),
                     children: oe
                 }))]
             })
         }));
-        var Ul, Gl;
+        var Vl, Gl;
         const ql = ["autoWidth", "children", "classes", "className", "defaultOpen", "displayEmpty", "IconComponent", "id", "input", "inputProps", "label", "labelId", "MenuProps", "multiple", "native", "onClose", "onOpen", "open", "renderValue", "SelectDisplayProps", "variant"],
             Hl = {
                 name: "MuiSelect",
                 overridesResolver: (e, t) => t.root,
                 shouldForwardProp: e => (0, se.FO)(e) && "variant" !== e,
                 slot: "Root"
             },
@@ -19956,22 +19979,22 @@
                         onOpen: w,
                         open: S,
                         renderValue: C,
                         SelectDisplayProps: k,
                         variant: Z = "outlined"
                     } = r,
                     j = (0, G.Z)(r, ql),
-                    P = b ? Tl : Vl,
+                    P = b ? Tl : Ul,
                     E = ii({
                         props: r,
                         muiFormControl: li(),
                         states: ["variant"]
                     }).variant || Z,
                     R = f || {
-                        standard: Ul || (Ul = (0, _.jsx)($l, {})),
+                        standard: Vl || (Vl = (0, _.jsx)($l, {})),
                         outlined: (0, _.jsx)(Kl, {
                             label: h
                         }),
                         filled: Gl || (Gl = (0, _.jsx)(Xl, {}))
                     } [E],
                     M = (e => {
                         const {
@@ -20093,17 +20116,17 @@
                             root: ["root"]
                         }, Jl, t)
                     })(D);
                 const F = {};
                 "outlined" === N && (g && "undefined" !== typeof g.shrink && (F.notched = g.shrink), F.label = y), I && (T && T.native || (F.id = void 0), F["aria-describedby"] = void 0);
                 const W = (0, Cr.Z)(h),
                     B = m && W ? "".concat(W, "-helper-text") : void 0,
-                    V = y && W ? "".concat(W, "-label") : void 0,
-                    U = tc[N],
-                    H = (0, _.jsx)(U, (0, a.Z)({
+                    U = y && W ? "".concat(W, "-label") : void 0,
+                    V = tc[N],
+                    H = (0, _.jsx)(V, (0, a.Z)({
                         "aria-describedby": B,
                         autoComplete: r,
                         autoFocus: o,
                         defaultValue: c,
                         fullWidth: f,
                         multiline: C,
                         name: k,
@@ -20129,21 +20152,21 @@
                     required: R,
                     color: l,
                     variant: N,
                     ownerState: D
                 }, z, {
                     children: [null != y && "" !== y && (0, _.jsx)(Ki, (0, a.Z)({
                         htmlFor: W,
-                        id: V
+                        id: U
                     }, g, {
                         children: y
                     })), I ? (0, _.jsx)(Ql, (0, a.Z)({
                         "aria-describedby": B,
                         id: W,
-                        labelId: V,
+                        labelId: U,
                         value: A,
                         input: H
                     }, T, {
                         children: i
                     })) : H, m && (0, _.jsx)(as, (0, a.Z)({
                         id: B
                     }, p, {
@@ -20716,16 +20739,16 @@
                 }, i))
             }));
         var Bc = n(5735);
 
         function _c(e) {
             return (0, de.Z)("MuiButton", e)
         }
-        const Vc = (0, ue.Z)("MuiButton", ["root", "text", "textInherit", "textPrimary", "textSecondary", "outlined", "outlinedInherit", "outlinedPrimary", "outlinedSecondary", "contained", "containedInherit", "containedPrimary", "containedSecondary", "disableElevation", "focusVisible", "disabled", "colorInherit", "textSizeSmall", "textSizeMedium", "textSizeLarge", "outlinedSizeSmall", "outlinedSizeMedium", "outlinedSizeLarge", "containedSizeSmall", "containedSizeMedium", "containedSizeLarge", "sizeMedium", "sizeSmall", "sizeLarge", "fullWidth", "startIcon", "endIcon", "iconSizeSmall", "iconSizeMedium", "iconSizeLarge"]);
-        const Uc = t.createContext({}),
+        const Uc = (0, ue.Z)("MuiButton", ["root", "text", "textInherit", "textPrimary", "textSecondary", "outlined", "outlinedInherit", "outlinedPrimary", "outlinedSecondary", "contained", "containedInherit", "containedPrimary", "containedSecondary", "disableElevation", "focusVisible", "disabled", "colorInherit", "textSizeSmall", "textSizeMedium", "textSizeLarge", "outlinedSizeSmall", "outlinedSizeMedium", "outlinedSizeLarge", "containedSizeSmall", "containedSizeMedium", "containedSizeLarge", "sizeMedium", "sizeSmall", "sizeLarge", "fullWidth", "startIcon", "endIcon", "iconSizeSmall", "iconSizeMedium", "iconSizeLarge"]);
+        const Vc = t.createContext({}),
             Gc = ["children", "color", "component", "className", "disabled", "disableElevation", "disableFocusRipple", "endIcon", "focusVisibleClassName", "fullWidth", "size", "startIcon", "type", "variant"],
             qc = e => (0, a.Z)({}, "small" === e.size && {
                 "& > *:nth-of-type(1)": {
                     fontSize: 18
                 }
             }, "medium" === e.size && {
                 "& > *:nth-of-type(1)": {
@@ -20787,18 +20810,18 @@
                         "@media (hover: none)": {
                             backgroundColor: t.palette[n.color].main
                         }
                     }),
                     "&:active": (0, a.Z)({}, "contained" === n.variant && {
                         boxShadow: t.shadows[8]
                     }),
-                    ["&.".concat(Vc.focusVisible)]: (0, a.Z)({}, "contained" === n.variant && {
+                    ["&.".concat(Uc.focusVisible)]: (0, a.Z)({}, "contained" === n.variant && {
                         boxShadow: t.shadows[6]
                     }),
-                    ["&.".concat(Vc.disabled)]: (0, a.Z)({
+                    ["&.".concat(Uc.disabled)]: (0, a.Z)({
                         color: t.palette.action.disabled
                     }, "outlined" === n.variant && {
                         border: "1px solid ".concat(t.palette.action.disabledBackground)
                     }, "outlined" === n.variant && "secondary" === n.color && {
                         border: "1px solid ".concat(t.palette.action.disabled)
                     }, "contained" === n.variant && {
                         color: t.palette.action.disabled,
@@ -20851,21 +20874,21 @@
                     ownerState: t
                 } = e;
                 return t.disableElevation && {
                     boxShadow: "none",
                     "&:hover": {
                         boxShadow: "none"
                     },
-                    ["&.".concat(Vc.focusVisible)]: {
+                    ["&.".concat(Uc.focusVisible)]: {
                         boxShadow: "none"
                     },
                     "&:active": {
                         boxShadow: "none"
                     },
-                    ["&.".concat(Vc.disabled)]: {
+                    ["&.".concat(Uc.disabled)]: {
                         boxShadow: "none"
                     }
                 }
             })),
             $c = (0, se.ZP)("span", {
                 name: "MuiButton",
                 slot: "StartIcon",
@@ -20905,15 +20928,15 @@
                     marginRight: -4,
                     marginLeft: 8
                 }, "small" === t.size && {
                     marginRight: -2
                 }, qc(t))
             })),
             Xc = t.forwardRef((function(e, n) {
-                const r = t.useContext(Uc),
+                const r = t.useContext(Vc),
                     o = (0, Bc.Z)(r, e),
                     i = (0, le.Z)({
                         props: o,
                         name: "MuiButton"
                     }),
                     {
                         children: s,
@@ -21682,15 +21705,15 @@
                         disableGutters: v
                     },
                     P = t.useRef(null);
                 (0, ci.Z)((() => {
                     i && P.current && P.current.focus()
                 }), [i]);
                 const E = t.Children.toArray(l),
-                    R = E.length && (0, Ut.Z)(E[E.length - 1], ["ListItemSecondaryAction"]),
+                    R = E.length && (0, Vt.Z)(E[E.length - 1], ["ListItemSecondaryAction"]),
                     M = (0, a.Z)({}, r, {
                         alignItems: o,
                         autoFocus: i,
                         button: s,
                         dense: j.dense,
                         disabled: g,
                         disableGutters: v,
@@ -21753,18 +21776,18 @@
                             children: w
                         })]
                     }))
                 })
             }));
         const _d = (0, ue.Z)("MuiDivider", ["root", "absolute", "fullWidth", "inset", "middle", "flexItem", "light", "vertical", "withChildren", "withChildrenVertical", "textAlignRight", "textAlignLeft", "wrapper", "wrapperVertical"]);
 
-        function Vd(e) {
+        function Ud(e) {
             return (0, de.Z)("MuiMenuItem", e)
         }
-        const Ud = (0, ue.Z)("MuiMenuItem", ["root", "focusVisible", "dense", "disabled", "divider", "gutters", "selected"]),
+        const Vd = (0, ue.Z)("MuiMenuItem", ["root", "focusVisible", "dense", "disabled", "divider", "gutters", "selected"]),
             Gd = ["autoFocus", "component", "dense", "divider", "disableGutters", "focusVisibleClassName", "role", "tabIndex"],
             qd = (0, se.ZP)(Ct, {
                 shouldForwardProp: e => (0, se.FO)(e) || "classes" === e,
                 name: "MuiMenuItem",
                 slot: "Root",
                 overridesResolver: (e, t) => {
                     const {
@@ -21798,30 +21821,30 @@
                     "&:hover": {
                         textDecoration: "none",
                         backgroundColor: t.palette.action.hover,
                         "@media (hover: none)": {
                             backgroundColor: "transparent"
                         }
                     },
-                    ["&.".concat(Ud.selected)]: {
+                    ["&.".concat(Vd.selected)]: {
                         backgroundColor: (0, kn.Fq)(t.palette.primary.main, t.palette.action.selectedOpacity),
-                        ["&.".concat(Ud.focusVisible)]: {
+                        ["&.".concat(Vd.focusVisible)]: {
                             backgroundColor: (0, kn.Fq)(t.palette.primary.main, t.palette.action.selectedOpacity + t.palette.action.focusOpacity)
                         }
                     },
-                    ["&.".concat(Ud.selected, ":hover")]: {
+                    ["&.".concat(Vd.selected, ":hover")]: {
                         backgroundColor: (0, kn.Fq)(t.palette.primary.main, t.palette.action.selectedOpacity + t.palette.action.hoverOpacity),
                         "@media (hover: none)": {
                             backgroundColor: (0, kn.Fq)(t.palette.primary.main, t.palette.action.selectedOpacity)
                         }
                     },
-                    ["&.".concat(Ud.focusVisible)]: {
+                    ["&.".concat(Vd.focusVisible)]: {
                         backgroundColor: t.palette.action.focus
                     },
-                    ["&.".concat(Ud.disabled)]: {
+                    ["&.".concat(Vd.disabled)]: {
                         opacity: t.palette.action.disabledOpacity
                     },
                     ["& + .".concat(_d.root)]: {
                         marginTop: t.spacing(1),
                         marginBottom: t.spacing(1)
                     },
                     ["& + .".concat(_d.inset)]: {
@@ -21887,15 +21910,15 @@
                             dense: n,
                             divider: r,
                             disableGutters: o,
                             selected: i,
                             classes: s
                         } = e, l = {
                             root: ["root", n && "dense", t && "disabled", !o && "gutters", r && "divider", i && "selected"]
-                        }, c = (0, ie.Z)(l, Vd, s);
+                        }, c = (0, ie.Z)(l, Ud, s);
                         return (0, a.Z)({}, s, c)
                     })(r),
                     b = (0, Ne.Z)(g, n);
                 let y;
                 return r.disabled || (y = void 0 !== p ? p : -1), (0, _.jsx)(ss.Provider, {
                     value: h,
                     children: (0, _.jsx)(qd, (0, a.Z)({
@@ -23349,15 +23372,15 @@
             })),
             _u = {
                 left: "right",
                 right: "left",
                 top: "down",
                 bottom: "up"
             };
-        const Vu = t.forwardRef((function(e, n) {
+        const Uu = t.forwardRef((function(e, n) {
                 const r = (0, le.Z)({
                         props: e,
                         name: "MuiDrawer"
                     }),
                     o = dn(),
                     i = {
                         enter: o.transitions.duration.enteringScreen,
@@ -23451,15 +23474,15 @@
                     onClose: m,
                     hideBackdrop: p,
                     ref: n
                 }, S, w, {
                     children: R
                 }))
             })),
-            Uu = Vu;
+            Vu = Uu;
 
         function Gu(e) {
             return (0, de.Z)("MuiLinearProgress", e)
         }(0, ue.Z)("MuiLinearProgress", ["root", "colorPrimary", "colorSecondary", "determinate", "indeterminate", "buffer", "query", "dashed", "dashedColorPrimary", "dashedColorSecondary", "bar", "barColorPrimary", "barColorSecondary", "bar1Indeterminate", "bar1Determinate", "bar1Buffer", "bar2Indeterminate", "bar2Buffer"]);
         var qu, Hu, $u, Ku, Xu, Yu;
         const Qu = ["className", "color", "value", "valueBuffer", "variant"];
         let Ju, ep, tp, np, rp, op;
@@ -23895,16 +23918,16 @@
                         TransitionComponent: A = Ps,
                         TransitionProps: N
                     } = d,
                     z = (0, G.Z)(d, bp),
                     D = dn(),
                     L = "rtl" === D.direction,
                     [F, W] = t.useState(),
-                    [B, V] = t.useState(null),
-                    U = t.useRef(!1),
+                    [B, U] = t.useState(null),
+                    V = t.useRef(!1),
                     H = x || C,
                     $ = t.useRef(),
                     K = t.useRef(),
                     X = t.useRef(),
                     Y = t.useRef(),
                     [Q, J] = (0, Ol.Z)({
                         controlled: R,
@@ -23924,19 +23947,19 @@
                 const oe = e => {
                         clearTimeout(kp), Cp = !0, J(!0), E && !ee && E(e)
                     },
                     ae = (0, ze.Z)((e => {
                         clearTimeout(kp), kp = setTimeout((() => {
                             Cp = !1
                         }), 800 + Z), J(!1), P && ee && P(e), clearTimeout($.current), $.current = setTimeout((() => {
-                            U.current = !1
+                            V.current = !1
                         }), D.transitions.duration.shortest)
                     })),
                     se = e => {
-                        U.current && "touchstart" !== e.type || (F && F.removeAttribute("title"), clearTimeout(K.current), clearTimeout(X.current), y || Cp && w ? K.current = setTimeout((() => {
+                        V.current && "touchstart" !== e.type || (F && F.removeAttribute("title"), clearTimeout(K.current), clearTimeout(X.current), y || Cp && w ? K.current = setTimeout((() => {
                             oe(e)
                         }), Cp ? w : y) : oe(e))
                     },
                     de = e => {
                         clearTimeout(K.current), clearTimeout(X.current), X.current = setTimeout((() => {
                             ae(e)
                         }), Z)
@@ -23951,15 +23974,15 @@
                     ge = e => {
                         pe(e), !1 === ue.current && (he(!1), de(e))
                     },
                     ve = e => {
                         F || W(e.currentTarget), fe(e), !0 === ue.current && (he(!0), se(e))
                     },
                     xe = e => {
-                        U.current = !0;
+                        V.current = !0;
                         const t = p.props;
                         t.onTouchStart && t.onTouchStart(e)
                     },
                     be = se,
                     ye = de,
                     we = e => {
                         xe(e), clearTimeout(X.current), clearTimeout($.current), re(), ne.current = document.body.style.WebkitUserSelect, document.body.style.WebkitUserSelect = "none", Y.current = setTimeout((() => {
@@ -24023,15 +24046,15 @@
                     }), [B, T]),
                     Oe = (0, a.Z)({}, d, {
                         isRtl: L,
                         arrow: u,
                         disableInteractive: H,
                         placement: M,
                         PopperComponentProp: I,
-                        touch: U.current
+                        touch: V.current
                     }),
                     Ae = (e => {
                         const {
                             classes: t,
                             disableInteractive: n,
                             arrow: r,
                             touch: o,
@@ -24044,16 +24067,16 @@
                         return (0, ie.Z)(i, vp, t)
                     })(Oe),
                     Le = null != (r = f.Popper) ? r : yp,
                     Fe = null != (o = null != (i = f.Transition) ? i : A) ? o : Ps,
                     We = null != (s = f.Tooltip) ? s : wp,
                     Be = null != (l = f.Arrow) ? l : Sp,
                     _e = hp(Le, (0, a.Z)({}, T, m.popper), Oe),
-                    Ve = hp(Fe, (0, a.Z)({}, N, m.transition), Oe),
-                    Ue = hp(We, (0, a.Z)({}, m.tooltip), Oe),
+                    Ue = hp(Fe, (0, a.Z)({}, N, m.transition), Oe),
+                    Ve = hp(We, (0, a.Z)({}, m.tooltip), Oe),
                     Ge = hp(Be, (0, a.Z)({}, m.arrow), Oe);
                 return (0, _.jsxs)(t.Fragment, {
                     children: [t.cloneElement(p, Me), (0, _.jsx)(Le, (0, a.Z)({
                         as: null != I ? I : ia,
                         placement: M,
                         anchorEl: C ? {
                             getBoundingClientRect: () => ({
@@ -24075,20 +24098,20 @@
                         children: e => {
                             let {
                                 TransitionProps: t
                             } = e;
                             var n, r;
                             return (0, _.jsx)(Fe, (0, a.Z)({
                                 timeout: D.transitions.duration.shorter
-                            }, t, Ve, {
-                                children: (0, _.jsxs)(We, (0, a.Z)({}, Ue, {
+                            }, t, Ue, {
+                                children: (0, _.jsxs)(We, (0, a.Z)({}, Ve, {
                                     className: (0, q.Z)(Ae.tooltip, null == (n = m.tooltip) ? void 0 : n.className),
                                     children: [O, u ? (0, _.jsx)(Be, (0, a.Z)({}, Ge, {
                                         className: (0, q.Z)(Ae.arrow, null == (r = m.arrow) ? void 0 : r.className),
-                                        ref: V
+                                        ref: U
                                     })) : null]
                                 }))
                             }))
                         }
                     }))]
                 })
             })),
@@ -24158,30 +24181,30 @@
                             }), (0, _.jsx)(Xc, {
                                 sx: {
                                     flexShrink: 0,
                                     ml: 3
                                 },
                                 startIcon: (0, _.jsx)(Rp.Z, {
                                     sx: {
-                                        color: Un.Z[100]
+                                        color: Vn.Z[100]
                                     },
                                     fontSize: "small"
                                 }),
                                 onClick: a,
                                 children: (0, _.jsx)(Ip, {
                                     children: "RENAME"
                                 })
                             }), (0, _.jsx)(Xc, {
                                 sx: {
                                     flexShrink: 0,
                                     ml: 1
                                 },
                                 startIcon: (0, _.jsx)(Mp.Z, {
                                     sx: {
-                                        color: Un.Z[100]
+                                        color: Vn.Z[100]
                                     },
                                     fontSize: "small"
                                 }),
                                 onClick: o,
                                 children: (0, _.jsx)(Ip, {
                                     children: "DELETE"
                                 })
@@ -24308,40 +24331,40 @@
                     },
                     generate: t => e(t),
                     reset() {
                         e = Bp
                     }
                 }
             })(),
-            Vp = {
+            Up = {
                 active: "Mui-active",
                 checked: "Mui-checked",
                 completed: "Mui-completed",
                 disabled: "Mui-disabled",
                 error: "Mui-error",
                 expanded: "Mui-expanded",
                 focused: "Mui-focused",
                 focusVisible: "Mui-focusVisible",
                 required: "Mui-required",
                 selected: "Mui-selected"
             };
 
-        function Up(e, t) {
-            return Vp[t] || "".concat(_p.generate(e), "-").concat(t)
+        function Vp(e, t) {
+            return Up[t] || "".concat(_p.generate(e), "-").concat(t)
         }
 
         function Gp(e, t) {
             const n = {};
             return t.forEach((t => {
-                n[t] = Up(e, t)
+                n[t] = Vp(e, t)
             })), n
         }
 
         function qp(e) {
-            return Up("MuiTreeView", e)
+            return Vp("MuiTreeView", e)
         }
         Gp("MuiTreeView", ["root"]);
         const Hp = ["children", "className", "defaultCollapseIcon", "defaultEndIcon", "defaultExpanded", "defaultExpandIcon", "defaultParentIcon", "defaultSelected", "disabledItemsFocusable", "disableSelection", "expanded", "id", "multiSelect", "onBlur", "onFocus", "onKeyDown", "onNodeFocus", "onNodeSelect", "onNodeToggle", "selected"],
             $p = (0, se.ZP)("ul", {
                 name: "MuiTreeView",
                 slot: "Root",
                 overridesResolver: (e, t) => t.root
@@ -24423,27 +24446,27 @@
                         controlled: k,
                         default: p,
                         name: "TreeView",
                         state: "selected"
                     }),
                     W = t.useCallback((e => !!Array.isArray(z) && -1 !== z.indexOf(e)), [z]),
                     B = t.useCallback((e => A.current[e] && A.current[e].expandable), []),
-                    V = t.useCallback((e => Array.isArray(L) ? -1 !== L.indexOf(e) : L === e), [L]),
-                    U = t.useCallback((e => {
+                    U = t.useCallback((e => Array.isArray(L) ? -1 !== L.indexOf(e) : L === e), [L]),
+                    V = t.useCallback((e => {
                         let t = A.current[e];
                         if (!t) return !1;
                         if (t.disabled) return !0;
                         for (; null != t.parentId;)
                             if (t = A.current[t.parentId], t.disabled) return !0;
                         return !1
                     }), []),
                     H = e => Object.keys(A.current).map((e => A.current[e])).filter((t => t.parentId === e)).sort(((e, t) => e.index - t.index)).map((e => e.id)),
                     $ = e => {
                         let t = H(e);
-                        return f || (t = t.filter((e => !U(e)))), t
+                        return f || (t = t.filter((e => !V(e)))), t
                     },
                     K = e => {
                         if (W(e) && $(e).length > 0) return $(e)[0];
                         let t = A.current[e];
                         for (; null != t;) {
                             const e = $(t.parentId),
                                 n = e[e.indexOf(t.id) + 1];
@@ -24535,15 +24558,15 @@
                             let n = L.slice();
                             const {
                                 start: r,
                                 end: o
                             } = t;
                             oe.current && (n = n.filter((e => -1 === ae.current.indexOf(e))));
                             let a = J(r, o);
-                            a = a.filter((e => !U(e))), ae.current = a;
+                            a = a.filter((e => !V(e))), ae.current = a;
                             let i = n.concat(a);
                             i = i.filter(((e, t) => i.indexOf(e) === t)), S && S(e, i), F(i)
                         })(e, {
                             start: r,
                             end: o
                         }), oe.current = !0
                     },
@@ -24572,17 +24595,17 @@
                     ue = t.useCallback(((e, t) => {
                         N.current[e] = t
                     }), []),
                     pe = t.useCallback((e => {
                         const t = (0, a.Z)({}, N.current);
                         delete t[e], N.current = t
                     }), []),
-                    fe = e => (B(T) && (W(T) ? te(e, T) : U(T) || ne(e)), !0),
+                    fe = e => (B(T) && (W(T) ? te(e, T) : V(T) || ne(e)), !0),
                     me = e => {
-                        if (W(T) && !U(T)) return ne(e, T), !0;
+                        if (W(T) && !V(T)) return ne(e, T), !0;
                         const t = (n = T, A.current[n].parentId);
                         var n;
                         return !!t && (ee(e, t), !0)
                     },
                     he = A.current[T] ? A.current[T].idAttribute : null;
                 return (0, _.jsx)(Np.Provider, {
                     value: {
@@ -24593,16 +24616,16 @@
                             defaultEndIcon: l
                         },
                         focus: ee,
                         toggleExpansion: ne,
                         isExpanded: W,
                         isExpandable: B,
                         isFocused: e => T === e,
-                        isSelected: V,
-                        isDisabled: U,
+                        isSelected: U,
+                        isDisabled: V,
                         selectNode: m ? Xp : ie,
                         selectRange: m ? Xp : se,
                         multiSelect: v,
                         disabledItemsFocusable: f,
                         mapFirstChar: ue,
                         unMapFirstChar: pe,
                         registerNode: ce,
@@ -24621,59 +24644,59 @@
                             onKeyDown: e => {
                                 let t = !1;
                                 const n = e.key;
                                 if (e.altKey || e.currentTarget !== e.target || !T) return;
                                 const r = e.ctrlKey || e.metaKey;
                                 switch (n) {
                                     case " ":
-                                        m || U(T) || (v && e.shiftKey ? (se(e, {
+                                        m || V(T) || (v && e.shiftKey ? (se(e, {
                                             end: T
                                         }), t = !0) : t = v ? ie(e, T, !0) : ie(e, T)), e.stopPropagation();
                                         break;
                                     case "Enter":
-                                        U(T) || (B(T) ? (ne(e), t = !0) : t = v ? ie(e, T, !0) : ie(e, T)), e.stopPropagation();
+                                        V(T) || (B(T) ? (ne(e), t = !0) : t = v ? ie(e, T, !0) : ie(e, T)), e.stopPropagation();
                                         break;
                                     case "ArrowDown":
                                         v && e.shiftKey && !m && ((e, t) => {
-                                            U(K(t)) || se(e, {
+                                            V(K(t)) || se(e, {
                                                 end: K(t),
                                                 current: t
                                             }, !0)
                                         })(e, T), te(e, T), t = !0;
                                         break;
                                     case "ArrowUp":
                                         v && e.shiftKey && !m && ((e, t) => {
-                                            U(X(t)) || se(e, {
+                                            V(X(t)) || se(e, {
                                                 end: X(t),
                                                 current: t
                                             }, !0)
                                         })(e, T), ((e, t) => {
                                             ee(e, X(t))
                                         })(e, T), t = !0;
                                         break;
                                     case "ArrowRight":
                                         t = j ? me(e) : fe(e);
                                         break;
                                     case "ArrowLeft":
                                         t = j ? fe(e) : me(e);
                                         break;
                                     case "Home":
-                                        v && r && e.shiftKey && !m && !U(T) && ((e, t) => {
+                                        v && r && e.shiftKey && !m && !V(T) && ((e, t) => {
                                             re.current || (re.current = t);
                                             const n = oe.current ? re.current : t;
                                             se(e, {
                                                 start: n,
                                                 end: Q()
                                             })
                                         })(e, T), (e => {
                                             ee(e, Q())
                                         })(e), t = !0;
                                         break;
                                     case "End":
-                                        v && r && e.shiftKey && !m && !U(T) && ((e, t) => {
+                                        v && r && e.shiftKey && !m && !V(T) && ((e, t) => {
                                             re.current || (re.current = t);
                                             const n = oe.current ? re.current : t;
                                             se(e, {
                                                 start: n,
                                                 end: Y()
                                             })
                                         })(e, T), (e => {
@@ -24696,15 +24719,15 @@
                                             const a = n.toLowerCase(),
                                                 i = [],
                                                 s = [];
                                             Object.keys(N.current).forEach((e => {
                                                 const t = N.current[e],
                                                     n = A.current[e],
                                                     r = !n.parentId || W(n.parentId),
-                                                    o = !f && U(e);
+                                                    o = !f && V(e);
                                                 r && !o && (i.push(e), s.push(t))
                                             })), r = i.indexOf(t) + 1, r >= i.length && (r = 0), o = Kp(s, r, a), -1 === o && (o = Kp(s, 0, a)), o > -1 && ee(e, i[o])
                                         })(e, T, n), t = !0)
                                 }
                                 var o;
                                 t && (e.preventDefault(), e.stopPropagation()), y && y(e)
                             },
@@ -24798,15 +24821,15 @@
                         className: r.label,
                         children: c
                     })]
                 }))
             }));
 
         function rf(e) {
-            return Up("MuiTreeItem", e)
+            return Vp("MuiTreeItem", e)
         }
         const of = Gp("MuiTreeItem", ["root", "group", "content", "expanded", "selected", "focused", "disabled", "iconContainer", "label"]), af = ["children", "className", "collapseIcon", "ContentComponent", "ContentProps", "endIcon", "expandIcon", "disabled", "icon", "id", "label", "nodeId", "onClick", "onMouseDown", "TransitionComponent", "TransitionProps"], sf = (0, se.ZP)("li", {
             name: "MuiTreeItem",
             slot: "Root",
             overridesResolver: (e, t) => t.root
         })({
             listStyle: "none",
@@ -24924,16 +24947,16 @@
             let N = null;
             null != m ? N = m : A && g && (N = "".concat(A, "-").concat(g));
             const [z, D] = t.useState(null), L = t.useRef(null), F = (0, Ne.Z)(D, n), W = t.useMemo((() => ({
                 element: z,
                 id: g
             })), [g, z]), {
                 index: B,
-                parentId: V
-            } = Fp(W), U = Boolean(Array.isArray(o) ? o.length : o), H = !!k && k(g), $ = !!Z && Z(g), K = !!j && j(g), X = !!P && P(g), Y = (0, a.Z)({}, r, {
+                parentId: U
+            } = Fp(W), V = Boolean(Array.isArray(o) ? o.length : o), H = !!k && k(g), $ = !!Z && Z(g), K = !!j && j(g), X = !!P && P(g), Y = (0, a.Z)({}, r, {
                 expanded: H,
                 focused: $,
                 selected: K,
                 disabled: X
             }), Q = (e => {
                 const {
                     classes: t
@@ -24947,33 +24970,33 @@
                     disabled: ["disabled"],
                     iconContainer: ["iconContainer"],
                     label: ["label"],
                     group: ["group"]
                 }, rf, t)
             })(Y);
             let J, ee, te;
-            return U && (ee = H ? s || S.defaultCollapseIcon : u || S.defaultExpandIcon), J = U ? S.defaultParentIcon : d || S.defaultEndIcon, t.useEffect((() => {
+            return V && (ee = H ? s || S.defaultCollapseIcon : u || S.defaultExpandIcon), J = V ? S.defaultParentIcon : d || S.defaultEndIcon, t.useEffect((() => {
                 if (T && O && -1 !== B) return T({
                     id: g,
                     idAttribute: N,
                     index: B,
-                    parentId: V,
-                    expandable: U,
+                    parentId: U,
+                    expandable: V,
                     disabled: p
                 }), () => {
                     O(g)
                 }
-            }), [T, O, V, B, g, U, p, N]), t.useEffect((() => {
+            }), [T, O, U, B, g, V, p, N]), t.useEffect((() => {
                 if (M && I && h) return M(g, L.current.textContent.substring(0, 1).toLowerCase()), () => {
                     I(g)
                 }
             }), [M, I, g, h]), E ? te = K : K && (te = !0), (0, _.jsxs)(sf, (0, a.Z)({
                 className: (0, q.Z)(Q.root, i),
                 role: "treeitem",
-                "aria-expanded": U ? H : null,
+                "aria-expanded": V ? H : null,
                 "aria-selected": te,
                 "aria-disabled": X || null,
                 ref: F,
                 id: N,
                 tabIndex: -1
             }, w, {
                 ownerState: Y,
@@ -25455,15 +25478,15 @@
                     ["& .".concat(Wf.label)]: {
                         ["&.".concat(Wf.disabled)]: {
                             color: t.palette.text.disabled
                         }
                     }
                 })
             })),
-            Vf = t.forwardRef((function(e, n) {
+            Uf = t.forwardRef((function(e, n) {
                 const r = (0, le.Z)({
                         props: e,
                         name: "MuiFormControlLabel"
                     }),
                     {
                         className: o,
                         componentsProps: i = {},
@@ -25515,25 +25538,25 @@
                         component: "span",
                         className: x.label
                     }, i.typography, {
                         children: d
                     }))]
                 }))
             })),
-            Uf = (0, kt.Z)((0, _.jsx)("path", {
+            Vf = (0, kt.Z)((0, _.jsx)("path", {
                 d: "M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.42 0-8-3.58-8-8s3.58-8 8-8 8 3.58 8 8-3.58 8-8 8z"
             }), "RadioButtonUnchecked"),
             Gf = (0, kt.Z)((0, _.jsx)("path", {
                 d: "M8.465 8.465C9.37 7.56 10.62 7 12 7C14.76 7 17 9.24 17 12C17 13.38 16.44 14.63 15.535 15.535C14.63 16.44 13.38 17 12 17C9.24 17 7 14.76 7 12C7 10.62 7.56 9.37 8.465 8.465Z"
             }), "RadioButtonChecked"),
             qf = (0, se.ZP)("span")({
                 position: "relative",
                 display: "flex"
             }),
-            Hf = (0, se.ZP)(Uf)({
+            Hf = (0, se.ZP)(Vf)({
                 transform: "scale(1)"
             }),
             $f = (0, se.ZP)(Gf)((e => {
                 let {
                     theme: t,
                     ownerState: n
                 } = e;
@@ -26111,29 +26134,29 @@
                             value: i,
                             name: "stage",
                             onChange: e => {
                                 this.setState({
                                     stage: e.target.value
                                 })
                             },
-                            children: [(0, _.jsx)(Vf, {
+                            children: [(0, _.jsx)(Uf, {
                                 value: "Stable",
                                 control: (0, _.jsx)(rm, {}),
                                 label: "Stable",
                                 sx: {
                                     ml: 4
                                 }
-                            }), (0, _.jsx)(Vf, {
+                            }), (0, _.jsx)(Uf, {
                                 value: "Preview",
                                 control: (0, _.jsx)(rm, {}),
                                 label: "Preview",
                                 sx: {
                                     ml: 4
                                 }
-                            }), (0, _.jsx)(Vf, {
+                            }), (0, _.jsx)(Uf, {
                                 value: "Experimental",
                                 control: (0, _.jsx)(rm, {}),
                                 label: "Experimental",
                                 sx: {
                                     ml: 4
                                 }
                             })]
@@ -26657,16 +26680,16 @@
                     }), s && (0, _.jsx)(Bm, {
                         className: g.expandIconWrapper,
                         ownerState: h,
                         children: s
                     })]
                 }))
             }));
-        var Vm = n(6950),
-            Um = n(1486),
+        var Um = n(6950),
+            Vm = n(1486),
             Gm = n(4081),
             qm = n(5567);
 
         function Hm(e) {
             return (0, de.Z)("MuiSwitch", e)
         }
         const $m = (0, ue.Z)("MuiSwitch", ["root", "edgeStart", "edgeEnd", "switchBase", "colorPrimary", "colorSecondary", "sizeSmall", "sizeMedium", "checked", "disabled", "input", "thumb", "track"]),
@@ -27026,15 +27049,15 @@
             const t = (t, n) => {
                     let r;
                     r = n ? new Set(e.tree.selectedArgIds).add(t) : new Set(e.tree.selectedArgIds.filter((e => e !== t && !e.startsWith("".concat(t, "/"))))), e.onTreeUpdated(ch(e.tree, r))
                 },
                 n = n => (0, _.jsx)(df, {
                     nodeId: n.id,
                     color: "inherit",
-                    label: (0, _.jsx)(Vf, {
+                    label: (0, _.jsx)(Uf, {
                         control: (0, _.jsx)(kd, {
                             size: "small",
                             checked: n.selectedCount > 0 && n.selectedCount === n.total,
                             indeterminate: n.selectedCount > 0 && n.selectedCount < n.total,
                             onClick: e => {
                                 t(n.id, !(n.selectedCount > 0 && n.selectedCount === n.total)), e.stopPropagation(), e.preventDefault()
                             }
@@ -27045,15 +27068,15 @@
                         }
                     }),
                     children: Array.isArray(n.args) ? n.args.map((n => (n => {
                         const r = -1 !== e.updatedIds.indexOf(n.id);
                         return (0, _.jsx)(df, {
                             nodeId: n.id,
                             color: "inherit",
-                            label: (0, _.jsx)(Vf, {
+                            label: (0, _.jsx)(Uf, {
                                 control: (0, _.jsx)(kd, {
                                     size: "small",
                                     checked: n.isSelected,
                                     onClick: e => {
                                         t(n.id, !n.isSelected), e.stopPropagation(), e.preventDefault()
                                     },
                                     disabled: r
@@ -27065,15 +27088,15 @@
                             })
                         }, n.id)
                     })(n))) : null
                 }, n.id),
                 r = e => (0, _.jsxs)(df, {
                     nodeId: e.id,
                     color: "inherit",
-                    label: (0, _.jsx)(Vf, {
+                    label: (0, _.jsx)(Uf, {
                         control: (0, _.jsx)(kd, {
                             size: "small",
                             checked: e.selectedCount > 0 && e.selectedCount === e.total,
                             indeterminate: e.selectedCount > 0 && e.selectedCount < e.total,
                             onClick: n => {
                                 t(e.id, !(e.selectedCount > 0 && e.selectedCount === e.total)), n.stopPropagation(), n.preventDefault()
                             }
@@ -27548,15 +27571,15 @@
                         }, t)))
                     })]
                 })
             })
         }
 
         function kh(e) {
-            const [n, r] = (0, t.useState)(!1), [o, a] = (0, t.useState)(""), [i, s] = (0, t.useState)(void 0), [l, c] = (0, t.useState)(""), [d, u] = (0, t.useState)(void 0), [p, f] = (0, t.useState)(""), [m, h] = (0, t.useState)(!1), [g, v] = (0, t.useState)(""), [x, b] = (0, t.useState)(""), [y, w] = (0, t.useState)(void 0), [S, C] = (0, t.useState)([]), [k, Z] = (0, t.useState)([]), [j, P] = (0, t.useState)(!1), [E, R] = (0, t.useState)(void 0), [M, I] = (0, t.useState)(!1), [T, O] = (0, t.useState)(!1), [A, N] = (0, t.useState)(void 0), [z, D] = (0, t.useState)(void 0), [L, F] = (0, t.useState)(""), [W, B] = (0, t.useState)(!1), V = () => {
+            const [n, r] = (0, t.useState)(!1), [o, a] = (0, t.useState)(""), [i, s] = (0, t.useState)(void 0), [l, c] = (0, t.useState)(""), [d, u] = (0, t.useState)(void 0), [p, f] = (0, t.useState)(""), [m, h] = (0, t.useState)(!1), [g, v] = (0, t.useState)(""), [x, b] = (0, t.useState)(""), [y, w] = (0, t.useState)(void 0), [S, C] = (0, t.useState)([]), [k, Z] = (0, t.useState)([]), [j, P] = (0, t.useState)(!1), [E, R] = (0, t.useState)(void 0), [M, I] = (0, t.useState)(!1), [T, O] = (0, t.useState)(!1), [A, N] = (0, t.useState)(void 0), [z, D] = (0, t.useState)(void 0), [L, F] = (0, t.useState)(""), [W, B] = (0, t.useState)(!1), U = () => {
                 var t, n;
                 s(void 0);
                 let r = l.trim(),
                     a = null !== (t = null === d || void 0 === d ? void 0 : d.trim()) && void 0 !== t ? t : void 0,
                     i = g.trim(),
                     c = x.trim(),
                     u = p.trim(),
@@ -27695,29 +27718,29 @@
                             }), (0, _.jsxs)(Lf, {
                                 row: !0,
                                 value: o,
                                 name: "stage",
                                 onChange: e => {
                                     a(e.target.value)
                                 },
-                                children: [(0, _.jsx)(Vf, {
+                                children: [(0, _.jsx)(Uf, {
                                     value: "Stable",
                                     control: (0, _.jsx)(rm, {}),
                                     label: "Stable",
                                     sx: {
                                         ml: 4
                                     }
-                                }), (0, _.jsx)(Vf, {
+                                }), (0, _.jsx)(Uf, {
                                     value: "Preview",
                                     control: (0, _.jsx)(rm, {}),
                                     label: "Preview",
                                     sx: {
                                         ml: 4
                                     }
-                                }), (0, _.jsx)(Vf, {
+                                }), (0, _.jsx)(Uf, {
                                     value: "Experimental",
                                     control: (0, _.jsx)(rm, {}),
                                     label: "Experimental",
                                     sx: {
                                         ml: 4
                                     }
                                 })]
@@ -27817,15 +27840,15 @@
                                             N(e.target.value)
                                         },
                                         placeholder: "Please input the prompt hint end with a colon.",
                                         margin: "normal",
                                         "aria-controls": "",
                                         required: !0
                                     }), void 0 !== z && (0, _.jsx)(_.Fragment, {
-                                        children: (0, _.jsx)(Vf, {
+                                        children: (0, _.jsx)(Uf, {
                                             control: (0, _.jsx)(kd, {
                                                 size: "small",
                                                 checked: z,
                                                 onChange: e => {
                                                     D(!z)
                                                 }
                                             }),
@@ -27906,15 +27929,15 @@
                         children: [(0, _.jsx)(Xc, {
                             onClick: () => {
                                 s(void 0), e.onClose(!1)
                             },
                             children: "Cancel"
                         }), !e.arg.var.startsWith("@") && (0, _.jsx)(Xc, {
                             onClick: async t => {
-                                const n = V();
+                                const n = U();
                                 if (void 0 === n) return;
                                 r(!0);
                                 const o = "".concat(e.commandUrl, "/Arguments/").concat(e.arg.var);
                                 try {
                                     Wh((await Qc().patch(o, {
                                         ...n
                                     })).data).arg;
@@ -27927,15 +27950,15 @@
                                     }
                                     r(!1)
                                 }
                             },
                             children: W ? "Update Global" : "Update"
                         }), !W && (0, _.jsx)(Xc, {
                             onClick: () => {
-                                if (void 0 === V()) return;
+                                if (void 0 === U()) return;
                                 r(!0);
                                 const t = "".concat(e.commandUrl, "/Arguments/").concat(e.arg.var, "/FindSimilar");
                                 Qc().post(t).then((e => {
                                     r(!1);
                                     const {
                                         tree: t,
                                         expandedIds: n
@@ -27956,15 +27979,15 @@
                         children: [(0, _.jsx)(Xc, {
                             onClick: () => {
                                 w(void 0), C([])
                             },
                             children: "Back"
                         }), (0, _.jsx)(Xc, {
                             onClick: async () => {
-                                const t = V();
+                                const t = U();
                                 if (void 0 === t) return;
                                 r(!0);
                                 let n = "";
                                 const o = [...k];
                                 for (const e in y.selectedArgIds) {
                                     const r = y.selectedArgIds[e];
                                     if (-1 === o.indexOf(r)) try {
@@ -28804,15 +28827,15 @@
                         }, n.arg
                     })))
                 })), {
                     args: n,
                     clsArgDefineMap: t
                 }
             },
-            Vh = function(e) {
+            Uh = function(e) {
                 const [n, r] = (0, t.useState)(!1), [o, a] = (0, t.useState)(void 0), [i, s] = (0, t.useState)(void 0), [l, c] = (0, t.useState)(!1), [d, u] = (0, t.useState)(!1);
                 return (0, _.jsxs)(t.Fragment, {
                     children: [(0, _.jsxs)(Pf, {
                         sx: {
                             flex: "1 0 auto",
                             display: "flex",
                             flexDirection: "column",
@@ -28892,50 +28915,172 @@
                         arg: o,
                         open: d,
                         onClose: async t => {
                             t && e.onReloadArgs(), u(!1), a(void 0), s(void 0)
                         }
                     })]
                 })
-            },
-            Uh = "az ",
-            Gh = ff(ve)((e => {
+            };
+        var Vh = n(1184),
+            Gh = n(5682);
+        const qh = ["component", "direction", "spacing", "divider", "children"];
+
+        function Hh(e, n) {
+            const r = t.Children.toArray(e).filter(Boolean);
+            return r.reduce(((e, o, a) => (e.push(o), a < r.length - 1 && e.push(t.cloneElement(n, {
+                key: "separator-".concat(a)
+            })), e)), [])
+        }
+        const $h = (0, se.ZP)("div", {
+                name: "MuiStack",
+                slot: "Root",
+                overridesResolver: (e, t) => [t.root]
+            })((e => {
+                let {
+                    ownerState: t,
+                    theme: n
+                } = e, r = (0, a.Z)({
+                    display: "flex"
+                }, (0, Vh.k9)({
+                    theme: n
+                }, (0, Vh.P$)({
+                    values: t.direction,
+                    breakpoints: n.breakpoints.values
+                }), (e => ({
+                    flexDirection: e
+                }))));
+                if (t.spacing) {
+                    const e = (0, Gh.hB)(n),
+                        o = Object.keys(n.breakpoints.values).reduce(((e, n) => (null == t.spacing[n] && null == t.direction[n] || (e[n] = !0), e)), {}),
+                        a = (0, Vh.P$)({
+                            values: t.direction,
+                            base: o
+                        }),
+                        i = (0, Vh.P$)({
+                            values: t.spacing,
+                            base: o
+                        }),
+                        s = (n, r) => {
+                            return {
+                                "& > :not(style) + :not(style)": {
+                                    margin: 0,
+                                    ["margin".concat((o = r ? a[r] : t.direction, {
+                                        row: "Left",
+                                        "row-reverse": "Right",
+                                        column: "Top",
+                                        "column-reverse": "Bottom"
+                                    } [o]))]: (0, Gh.NA)(e, n)
+                                }
+                            };
+                            var o
+                        };
+                    r = (0, K.Z)(r, (0, Vh.k9)({
+                        theme: n
+                    }, i, s))
+                }
+                return r
+            })),
+            Kh = t.forwardRef((function(e, t) {
+                const n = J((0, le.Z)({
+                        props: e,
+                        name: "MuiStack"
+                    })),
+                    {
+                        component: r = "div",
+                        direction: o = "column",
+                        spacing: i = 0,
+                        divider: s,
+                        children: l
+                    } = n,
+                    c = (0, G.Z)(n, qh),
+                    d = {
+                        direction: o,
+                        spacing: i
+                    };
+                return (0, _.jsx)($h, (0, a.Z)({
+                    as: r,
+                    ownerState: d,
+                    ref: t
+                }, c, {
+                    children: s ? Hh(l, s) : l
+                }))
+            })),
+            Xh = Kh;
+        class Yh extends t.Component {
+            constructor(e) {
+                super(e), this.state = {
+                    value: 1 === this.props.options.length ? this.props.options[0] : null
+                }
+            }
+            render() {
+                const {
+                    name: e,
+                    options: t,
+                    commonPrefix: n,
+                    value: r
+                } = this.props;
+                return (0, _.jsx)(Xa, {
+                    id: e,
+                    value: r,
+                    options: t,
+                    onInputChange: (e, t) => {
+                        this.props.onValueUpdate(t)
+                    },
+                    getOptionLabel: e => e.replace(n, ""),
+                    renderOption: (e, t) => (0, _.jsx)(ae, {
+                        component: "li",
+                        ...e,
+                        children: t.replace(n, "")
+                    }),
+                    selectOnFocus: !0,
+                    freeSolo: !0,
+                    renderInput: t => (0, _.jsx)(rc, {
+                        ...t,
+                        size: "small",
+                        label: e,
+                        required: !0
+                    })
+                })
+            }
+        }
+        const Qh = "az ",
+            Jh = ff(ve)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.palette.primary.main,
                     fontFamily: "'Work Sans', sans-serif",
                     fontSize: 14,
                     fontWeight: 400
                 }
             })),
-            qh = ff(ve)((e => {
+            eg = ff(ve)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.palette.primary.main,
                     fontFamily: "'Work Sans', sans-serif",
                     fontSize: 14,
                     fontWeight: 400
                 }
             })),
-            Hh = ff(ve)((e => {
+            tg = ff(ve)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: "#5d64cf",
                     fontFamily: "'Work Sans', sans-serif",
                     fontSize: 14,
                     fontWeight: 400
                 }
             })),
-            $h = ff((e => (0, _.jsx)(_m, {
+            ng = ff((e => (0, _.jsx)(_m, {
                 expandIcon: (0, _.jsx)(qm.Z, {
                     fontSize: "small",
                     color: "primary"
                 }),
                 ...e
             })))((e => {
                 let {
@@ -28944,28 +29089,28 @@
                 return {
                     flexDirection: "row-reverse",
                     "& .MuiAccordionSummary-expandIconWrapper.Mui-expanded": {
                         transform: "rotate(0deg)"
                     }
                 }
             }));
-        class Kh extends t.Component {
+        class rg extends t.Component {
             constructor(e) {
                 super(e), this.loadCommand = async () => {
                     this.setState({
                         loading: !0
                     });
                     let {
                         workspaceUrl: e,
                         previewCommand: t
                     } = this.props, n = t.names;
                     const r = "".concat(e, "/CommandTree/Nodes/aaz/") + n.slice(0, -1).join("/") + "/Leaves/" + n[n.length - 1];
                     try {
                         let e = await Qc().get(r),
-                            t = tg(e.data);
+                            t = cg(e.data);
                         t.id === this.props.previewCommand.id && this.setState({
                             loading: !1,
                             command: t
                         })
                     } catch (o) {
                         return this.setState({
                             loading: !1
@@ -29026,29 +29171,29 @@
                     command: void 0
                 }), this.loadCommand())
             }
             render() {
                 const {
                     workspaceUrl: e,
                     previewCommand: n
-                } = this.props, r = n.names, o = Uh + r.join(" "), a = "".concat(e, "/CommandTree/Nodes/aaz/") + r.slice(0, -1).join("/") + "/Leaves/" + r[r.length - 1], {
+                } = this.props, r = n.names, o = Qh + r.join(" "), a = "".concat(e, "/CommandTree/Nodes/aaz/") + r.slice(0, -1).join("/") + "/Leaves/" + r[r.length - 1], {
                     command: i,
                     displayCommandDialog: s,
                     displayExampleDialog: l,
                     displayCommandDeleteDialog: c,
                     displayAddSubcommandDialog: d,
                     exampleIdx: u,
                     loading: p
                 } = this.state, f = (e, t) => (0, _.jsxs)(Zm, {
                     elevation: 0,
                     expanded: !0,
                     onDoubleClick: () => {
                         this.onExampleDialogDisplay(t)
                     },
-                    children: [(0, _.jsx)($h, {
+                    children: [(0, _.jsx)(ng, {
                         id: "example-".concat(t, "-header"),
                         children: (0, _.jsxs)(ae, {
                             sx: {
                                 ml: 1,
                                 flexGrow: 1,
                                 display: "flex",
                                 flexDirection: "row",
@@ -29067,15 +29212,15 @@
                                 startIcon: (0, _.jsx)(Rp.Z, {
                                     color: "secondary",
                                     fontSize: "small"
                                 }),
                                 onClick: () => {
                                     this.onExampleDialogDisplay(t)
                                 },
-                                children: (0, _.jsx)(Hh, {
+                                children: (0, _.jsx)(tg, {
                                     children: "Edit"
                                 })
                             })]
                         })
                     }), (0, _.jsx)(Rm, {
                         sx: {
                             display: "flex",
@@ -29100,26 +29245,26 @@
                                     display: "flex",
                                     flexDirection: "row",
                                     alignItems: "center",
                                     justifyContent: "flex-start"
                                 },
                                 children: [(0, _.jsx)(Gm.Z, {
                                     fontSize: "small"
-                                }), (0, _.jsx)(Gh, {
+                                }), (0, _.jsx)(Jh, {
                                     sx: {
                                         flexShrink: 0
                                     },
-                                    children: Uh
+                                    children: Qh
                                 })]
                             }), (0, _.jsx)(ae, {
                                 component: "span",
                                 sx: {
                                     ml: .8
                                 },
-                                children: (0, _.jsx)(qh, {
+                                children: (0, _.jsx)(eg, {
                                     children: e
                                 })
                             })]
                         }, "example-".concat(t, "-command-").concat(n))))
                     })]
                 }, "example-".concat(t));
                 return (0, _.jsxs)(t.Fragment, {
@@ -29280,15 +29425,15 @@
                             sx: {
                                 flexGrow: 1,
                                 display: "flex",
                                 flexDirection: "column",
                                 mt: 1,
                                 p: 2
                             },
-                            children: (0, _.jsx)(Vh, {
+                            children: (0, _.jsx)(Uh, {
                                 commandUrl: a,
                                 args: i.args,
                                 clsArgDefineMap: i.clsArgDefineMap,
                                 onReloadArgs: this.loadCommand,
                                 onAddSubCommand: this.onAddSubcommandDialogDisplay
                             })
                         }))(), void 0 !== i && (() => {
@@ -29341,44 +29486,44 @@
                                             variant: "body2",
                                             children: "Add"
                                         })
                                     })
                                 })]
                             })
                         })()]
-                    }), void 0 !== i && s && (0, _.jsx)(Yh, {
+                    }), void 0 !== i && s && (0, _.jsx)(ag, {
                         open: s,
                         workspaceUrl: e,
                         command: i,
                         onClose: this.handleCommandDialogClose
-                    }), void 0 !== i && l && (0, _.jsx)(Jh, {
+                    }), void 0 !== i && l && (0, _.jsx)(sg, {
                         open: l,
                         workspaceUrl: e,
                         command: i,
                         idx: u,
                         onClose: this.handleExampleDialogClose
-                    }), void 0 !== i && c && (0, _.jsx)(Xh, {
+                    }), void 0 !== i && c && (0, _.jsx)(og, {
                         open: c,
                         workspaceUrl: e,
                         command: i,
                         onClose: this.handleCommandDeleteDialogClose
-                    }), void 0 !== i && d && (0, _.jsx)(eg, {
+                    }), void 0 !== i && d && (0, _.jsx)(lg, {
                         open: d,
                         workspaceUrl: e,
                         command: i,
                         onClose: this.handleAddSubcommandDisplayClose,
                         argVar: this.state.subcommandArgVar,
                         subArgOptions: this.state.subcommandSubArgOptions,
                         defaultGroupNames: this.state.subcommandDefaultGroupNames
                     })]
                 })
             }
         }
 
-        function Xh(e) {
+        function og(e) {
             const [n, r] = t.useState(!1), [o, a] = t.useState([]), i = () => {
                 let t = [];
                 return e.command.resources.forEach((n => {
                     const r = btoa(n.id),
                         o = btoa(n.version);
                     if (void 0 !== n.subresource) {
                         let a = btoa(n.subresource);
@@ -29388,15 +29533,15 @@
             };
             t.useEffect((() => {
                 a([]);
                 const e = i().map((e => Qc().get("".concat(e, "/Commands"))));
                 Promise.all(e).then((e => {
                     const t = new Set;
                     e.forEach((e => {
-                        e.data.map((e => tg(e))).forEach((e => {
+                        e.data.map((e => cg(e))).forEach((e => {
                             t.add(e.names.join(" "))
                         }))
                     }));
                     const n = [];
                     t.forEach((e => n.push(e))), n.sort(((e, t) => e.localeCompare(t))), a(n)
                 })).catch((e => {
                     console.error(e.response)
@@ -29407,15 +29552,15 @@
                 open: e.open,
                 children: [(0, _.jsx)(xc, {
                     children: "Delete Commands"
                 }), (0, _.jsx)(Sc, {
                     dividers: !0,
                     children: o.map(((e, t) => (0, _.jsx)(ve, {
                         variant: "body2",
-                        children: "".concat(Uh).concat(e)
+                        children: "".concat(Qh).concat(e)
                     }, "command-".concat(t))))
                 }), (0, _.jsxs)(Wc, {
                     children: [n && (0, _.jsx)(ae, {
                         sx: {
                             width: "100%"
                         },
                         children: (0, _.jsx)(mp, {
@@ -29439,15 +29584,15 @@
                             },
                             children: "Delete"
                         })]
                     })]
                 })]
             })
         }
-        class Yh extends t.Component {
+        class ag extends t.Component {
             constructor(e) {
                 var t, n, r, o, a, i;
                 super(e), this.handleModify = e => {
                     let {
                         name: t,
                         stage: n,
                         shortHelp: r,
@@ -29484,22 +29629,22 @@
                             lines: c
                         },
                         stage: n,
                         confirmation: a
                     }).then((e => {
                         const t = l.join(" ");
                         if (t === s.names.join(" ")) {
-                            const t = tg(e.data);
+                            const t = cg(e.data);
                             this.setState({
                                 updating: !1
                             }), this.props.onClose(t)
                         } else Qc().post("".concat(d, "/Rename"), {
                             name: t
                         }).then((e => {
-                            const t = tg(e.data);
+                            const t = cg(e.data);
                             this.setState({
                                 updating: !1
                             }), this.props.onClose(t)
                         }))
                     })).catch((e => {
                         var t, n;
                         if (console.error(e.response), null !== (t = e.response) && void 0 !== t && null !== (n = t.data) && void 0 !== n && n.message) {
@@ -29563,29 +29708,29 @@
                             value: i,
                             name: "stage",
                             onChange: e => {
                                 this.setState({
                                     stage: e.target.value
                                 })
                             },
-                            children: [(0, _.jsx)(Vf, {
+                            children: [(0, _.jsx)(Uf, {
                                 value: "Stable",
                                 control: (0, _.jsx)(rm, {}),
                                 label: "Stable",
                                 sx: {
                                     ml: 4
                                 }
-                            }), (0, _.jsx)(Vf, {
+                            }), (0, _.jsx)(Uf, {
                                 value: "Preview",
                                 control: (0, _.jsx)(rm, {}),
                                 label: "Preview",
                                 sx: {
                                     ml: 4
                                 }
-                            }), (0, _.jsx)(Vf, {
+                            }), (0, _.jsx)(Uf, {
                                 value: "Experimental",
                                 control: (0, _.jsx)(rm, {}),
                                 label: "Experimental",
                                 sx: {
                                     ml: 4
                                 }
                             })]
@@ -29665,40 +29810,40 @@
                                 children: "Save"
                             })]
                         })]
                     })]
                 })
             }
         }
-        const Qh = ff(ve)((e => {
+        const ig = ff(ve)((e => {
             let {
                 theme: t
             } = e;
             return {
                 color: t.palette.primary.main,
                 fontFamily: "'Roboto Condensed', sans-serif",
                 fontSize: 16,
                 fontWeight: 400
             }
         }));
-        class Jh extends t.Component {
+        class sg extends t.Component {
             constructor(e) {
                 var t;
                 super(e), this.onUpdateExamples = e => {
                     let {
                         workspaceUrl: t,
                         command: n
                     } = this.props;
                     const r = "".concat(t, "/CommandTree/Nodes/aaz/") + n.names.slice(0, -1).join("/") + "/Leaves/" + n.names[n.names.length - 1];
                     this.setState({
                         updating: !0
                     }), Qc().patch(r, {
                         examples: e
                     }).then((e => {
-                        const t = tg(e.data);
+                        const t = cg(e.data);
                         this.setState({
                             updating: !1
                         }), this.props.onClose(t)
                     })).catch((e => {
                         var t, n;
                         if (console.error(e.response), null !== (t = e.response) && void 0 !== t && null !== (n = t.data) && void 0 !== n && n.message) {
                             const t = e.response.data;
@@ -29772,149 +29917,235 @@
                         }
                     }))
                 }, this.onAddExampleCommand = () => {
                     this.setState((e => ({
                         ...e,
                         exampleCommands: [...e.exampleCommands, ""]
                     })))
+                }, this.loadSwaggerExamples = async () => {
+                    try {
+                        let {
+                            workspaceUrl: e,
+                            command: t
+                        } = this.props;
+                        const n = "".concat(e, "/CommandTree/Nodes/aaz/") + t.names.slice(0, -1).join("/") + "/Leaves/" + t.names[t.names.length - 1] + "/GenerateExamples";
+                        this.setState({
+                            source: "swagger",
+                            updating: !0
+                        });
+                        const r = (await Qc().post(n, {
+                            source: "swagger"
+                        })).data.map((e => ({
+                            name: e.name,
+                            commands: e.commands
+                        })));
+                        this.setState({
+                            exampleOptions: r,
+                            updating: !1
+                        }), r.length > 0 && this.onExampleSelectorUpdate(r[0].name)
+                    } catch (n) {
+                        var e, t;
+                        if (console.error(n.response), null !== (e = n.response) && void 0 !== e && null !== (t = e.data) && void 0 !== t && t.message) {
+                            const e = n.response.data;
+                            this.setState({
+                                updating: !1,
+                                invalidText: "ResponseError: ".concat(e.message)
+                            })
+                        }
+                    }
+                }, this.onExampleSelectorUpdate = e => {
+                    var t;
+                    let n = null !== (t = this.state.exampleOptions.find((t => t.name === e))) && void 0 !== t ? t : void 0;
+                    var r, o;
+                    void 0 === n ? this.setState({
+                        name: null !== e && void 0 !== e ? e : ""
+                    }) : this.setState({
+                        name: null !== (r = null === n || void 0 === n ? void 0 : n.name) && void 0 !== r ? r : "",
+                        exampleCommands: null !== (o = null === n || void 0 === n ? void 0 : n.commands) && void 0 !== o ? o : [""]
+                    })
                 };
                 const n = null !== (t = this.props.command.examples) && void 0 !== t ? t : [];
                 if (void 0 === this.props.idx) this.state = {
                     name: "",
                     exampleCommands: [""],
                     isAdd: !0,
                     invalidText: void 0,
-                    updating: !1
+                    updating: !1,
+                    source: void 0,
+                    exampleOptions: []
                 };
                 else {
                     const e = n[this.props.idx];
                     this.state = {
                         name: e.name,
                         exampleCommands: e.commands,
                         isAdd: !1,
                         invalidText: void 0,
-                        updating: !1
+                        updating: !1,
+                        source: void 0,
+                        exampleOptions: []
                     }
                 }
             }
             render() {
                 const {
                     name: e,
                     exampleCommands: n,
                     isAdd: r,
                     invalidText: o,
-                    updating: a
-                } = this.state;
+                    updating: a,
+                    source: i,
+                    exampleOptions: s
+                } = this.state, l = e;
                 return (0, _.jsxs)(fc, {
                     disableEscapeKeyDown: !0,
                     open: this.props.open,
                     sx: {
                         "& .MuiDialog-paper": {
                             width: "80%"
                         }
                     },
-                    children: [(0, _.jsx)(xc, {
-                        children: r ? "Add Example" : "Modify Example"
+                    children: [(0, _.jsxs)(xc, {
+                        children: [r ? "Add Example" : "Modify Example", (0, _.jsx)(ha, {
+                            style: {
+                                position: "absolute",
+                                right: 16,
+                                top: 8
+                            },
+                            edge: "end",
+                            color: "inherit",
+                            onClick: this.handleClose,
+                            "aria-label": "close",
+                            children: (0, _.jsx)(pu.Z, {})
+                        })]
                     }), (0, _.jsxs)(Sc, {
                         dividers: !0,
-                        children: [o && (0, _.jsxs)(zc, {
-                            variant: "filled",
-                            severity: "error",
-                            children: [" ", o, " "]
-                        }), (0, _.jsx)(rc, {
-                            id: "name",
-                            label: "Name",
-                            type: "text",
-                            fullWidth: !0,
-                            variant: "standard",
-                            value: e,
-                            onChange: e => {
-                                this.setState({
-                                    name: e.target.value
+                        children: [r && void 0 === i && (0, _.jsx)(Xh, {
+                            direction: "column",
+                            spacing: 2,
+                            children: (0, _.jsx)(Xc, {
+                                variant: "contained",
+                                size: "large",
+                                color: "secondary",
+                                sx: {
+                                    fontSize: "20px",
+                                    padding: "10px 20px"
+                                },
+                                onClick: () => {
+                                    this.loadSwaggerExamples()
+                                },
+                                children: (0, _.jsx)(ve, {
+                                    variant: "body2",
+                                    children: "By OpenAPI Specification"
                                 })
-                            },
-                            margin: "normal",
-                            required: !0
-                        }), (0, _.jsx)(Ki, {
-                            required: !0,
-                            sx: {
-                                font: "inherit",
-                                mt: 1
-                            },
-                            children: "Commands"
-                        }), n.map(((e, t) => (0, _.jsxs)(ae, {
-                            sx: {
-                                display: "flex",
-                                flexDirection: "row",
-                                alignItems: "center",
-                                justifyContent: "flex-start",
-                                ml: 1
-                            },
-                            children: [(0, _.jsx)(ha, {
-                                edge: "start",
-                                color: "inherit",
-                                onClick: () => this.onRemoveExampleCommand(t),
-                                "aria-label": "remove",
-                                children: (0, _.jsx)(Vm.Z, {
-                                    fontSize: "small"
+                            })
+                        }), (!r || void 0 != i) && (0, _.jsxs)(t.Fragment, {
+                            children: [o && (0, _.jsxs)(zc, {
+                                variant: "filled",
+                                severity: "error",
+                                children: [" ", o, " "]
+                            }), !r && (0, _.jsx)(t.Fragment, {
+                                children: (0, _.jsx)(rc, {
+                                    id: "name",
+                                    label: "Name",
+                                    type: "text",
+                                    fullWidth: !0,
+                                    variant: "standard",
+                                    value: e,
+                                    onChange: e => {
+                                        this.setState({
+                                            name: e.target.value
+                                        })
+                                    },
+                                    margin: "normal",
+                                    required: !0
                                 })
-                            }), (0, _.jsx)(ki, {
-                                id: "command-".concat(t),
-                                multiline: !0,
-                                value: e,
-                                onChange: e => {
-                                    this.onModifyExampleCommand(e.target.value, t)
+                            }), "swagger" === i && (0, _.jsx)(t.Fragment, {
+                                children: (0, _.jsx)(Yh, {
+                                    name: "Name",
+                                    commonPrefix: "",
+                                    options: s.map((e => e.name)),
+                                    value: l,
+                                    onValueUpdate: this.onExampleSelectorUpdate
+                                })
+                            }), (0, _.jsx)(Ki, {
+                                required: !0,
+                                sx: {
+                                    font: "inherit",
+                                    mt: 1
                                 },
+                                children: "Commands"
+                            }), n.map(((e, t) => (0, _.jsxs)(ae, {
                                 sx: {
-                                    flexGrow: 1
+                                    display: "flex",
+                                    flexDirection: "row",
+                                    alignItems: "center",
+                                    justifyContent: "flex-start",
+                                    ml: 1
                                 },
-                                placeholder: "Input a command here.",
-                                startAdornment: (0, _.jsx)(Nm, {
-                                    position: "start",
-                                    children: (0, _.jsx)(Qh, {
-                                        children: Uh
+                                children: [(0, _.jsx)(ha, {
+                                    edge: "start",
+                                    color: "inherit",
+                                    onClick: () => this.onRemoveExampleCommand(t),
+                                    "aria-label": "remove",
+                                    children: (0, _.jsx)(Um.Z, {
+                                        fontSize: "small"
                                     })
-                                })
-                            })]
-                        }, t))), (0, _.jsxs)(ae, {
-                            sx: {
-                                display: "flex",
-                                flexDirection: "row",
-                                alignItems: "center",
-                                justifyContent: "flex-start",
-                                ml: 1
-                            },
-                            children: [(0, _.jsx)(ha, {
-                                edge: "start",
-                                color: "inherit",
-                                onClick: this.onAddExampleCommand,
-                                "aria-label": "add",
-                                children: (0, _.jsx)(Um.Z, {
-                                    fontSize: "small"
-                                })
-                            }), (0, _.jsx)(Qh, {
+                                }), (0, _.jsx)(ki, {
+                                    id: "command-".concat(t),
+                                    multiline: !0,
+                                    value: e,
+                                    onChange: e => {
+                                        this.onModifyExampleCommand(e.target.value, t)
+                                    },
+                                    sx: {
+                                        flexGrow: 1
+                                    },
+                                    placeholder: "Input a command here.",
+                                    startAdornment: (0, _.jsx)(Nm, {
+                                        position: "start",
+                                        children: (0, _.jsx)(ig, {
+                                            children: Qh
+                                        })
+                                    })
+                                })]
+                            }, t))), (0, _.jsxs)(ae, {
                                 sx: {
-                                    flexShrink: 0
+                                    display: "flex",
+                                    flexDirection: "row",
+                                    alignItems: "center",
+                                    justifyContent: "flex-start",
+                                    ml: 1
                                 },
-                                children: " One more command"
+                                children: [(0, _.jsx)(ha, {
+                                    edge: "start",
+                                    color: "inherit",
+                                    onClick: this.onAddExampleCommand,
+                                    "aria-label": "add",
+                                    children: (0, _.jsx)(Vm.Z, {
+                                        fontSize: "small"
+                                    })
+                                }), (0, _.jsx)(ig, {
+                                    sx: {
+                                        flexShrink: 0
+                                    },
+                                    children: " One more command"
+                                })]
                             })]
                         })]
-                    }), (0, _.jsxs)(Wc, {
+                    }), (!r || void 0 != i) && (0, _.jsxs)(Wc, {
                         children: [a && (0, _.jsx)(ae, {
                             sx: {
                                 width: "100%"
                             },
                             children: (0, _.jsx)(mp, {
                                 color: "secondary"
                             })
                         }), !a && (0, _.jsxs)(t.Fragment, {
-                            children: [(0, _.jsx)(Xc, {
-                                onClick: this.handleClose,
-                                children: "Cancel"
-                            }), !r && (0, _.jsxs)(t.Fragment, {
+                            children: [!r && (0, _.jsxs)(t.Fragment, {
                                 children: [(0, _.jsx)(Xc, {
                                     onClick: this.handleDelete,
                                     children: "Delete"
                                 }), (0, _.jsx)(Xc, {
                                     onClick: this.handleModify,
                                     children: "Save"
                                 })]
@@ -29924,15 +30155,15 @@
                             })]
                         })]
                     })]
                 })
             }
         }
 
-        function eg(e) {
+        function lg(e) {
             const [n, r] = (0, t.useState)(!1), [o, a] = (0, t.useState)(void 0), [i, s] = (0, t.useState)(""), [l, c] = (0, t.useState)([]);
             (0, t.useEffect)((() => {
                 s(e.defaultGroupNames.join(" ")), c(e.subArgOptions)
             }), [e.argVar, e.defaultGroupNames]);
             return (0, _.jsxs)(fc, {
                 disableEscapeKeyDown: !0,
                 open: e.open,
@@ -30052,15 +30283,15 @@
                             },
                             children: "Add Subcommands"
                         })]
                     })]
                 })]
             })
         }
-        const tg = e => {
+        const cg = e => {
                 var t;
                 let n = {
                     id: "command:" + e.names.join("/"),
                     names: e.names,
                     help: e.help,
                     stage: null !== (t = e.stage) && void 0 !== t ? t : "Stable",
                     examples: e.examples,
@@ -30068,62 +30299,62 @@
                     version: e.version
                 };
                 return e.confirmation && (n.confirmation = e.confirmation), e.argGroups && (n = {
                     ...n,
                     ..._h(e.argGroups)
                 }), n
             },
-            ng = Kh;
-        let rg;
+            dg = rg;
+        let ug;
 
-        function og() {
-            if (rg) return rg;
+        function pg() {
+            if (ug) return ug;
             const e = document.createElement("div"),
                 t = document.createElement("div");
-            return t.style.width = "10px", t.style.height = "1px", e.appendChild(t), e.dir = "rtl", e.style.fontSize = "14px", e.style.width = "4px", e.style.height = "1px", e.style.position = "absolute", e.style.top = "-1000px", e.style.overflow = "scroll", document.body.appendChild(e), rg = "reverse", e.scrollLeft > 0 ? rg = "default" : (e.scrollLeft = 1, 0 === e.scrollLeft && (rg = "negative")), document.body.removeChild(e), rg
+            return t.style.width = "10px", t.style.height = "1px", e.appendChild(t), e.dir = "rtl", e.style.fontSize = "14px", e.style.width = "4px", e.style.height = "1px", e.style.position = "absolute", e.style.top = "-1000px", e.style.overflow = "scroll", document.body.appendChild(e), ug = "reverse", e.scrollLeft > 0 ? ug = "default" : (e.scrollLeft = 1, 0 === e.scrollLeft && (ug = "negative")), document.body.removeChild(e), ug
         }
 
-        function ag(e, t) {
+        function fg(e, t) {
             const n = e.scrollLeft;
             if ("rtl" !== t) return n;
-            switch (og()) {
+            switch (pg()) {
                 case "negative":
                     return e.scrollWidth - e.clientWidth + n;
                 case "reverse":
                     return e.scrollWidth - e.clientWidth - n;
                 default:
                     return n
             }
         }
 
-        function ig(e) {
+        function mg(e) {
             return (1 + Math.sin(Math.PI * e - Math.PI / 2)) / 2
         }
-        const sg = ["onChange"],
-            lg = {
+        const hg = ["onChange"],
+            gg = {
                 width: 99,
                 height: 99,
                 position: "absolute",
                 top: -9999,
                 overflow: "scroll"
             };
-        const cg = (0, kt.Z)((0, _.jsx)("path", {
+        const vg = (0, kt.Z)((0, _.jsx)("path", {
                 d: "M15.41 16.09l-4.58-4.59 4.58-4.59L14 5.5l-6 6 6 6z"
             }), "KeyboardArrowLeft"),
-            dg = (0, kt.Z)((0, _.jsx)("path", {
+            xg = (0, kt.Z)((0, _.jsx)("path", {
                 d: "M8.59 16.34l4.58-4.59-4.58-4.59L10 5.75l6 6-6 6z"
             }), "KeyboardArrowRight");
 
-        function ug(e) {
+        function bg(e) {
             return (0, de.Z)("MuiTabScrollButton", e)
         }
-        const pg = (0, ue.Z)("MuiTabScrollButton", ["root", "vertical", "horizontal", "disabled"]);
-        var fg, mg;
-        const hg = ["className", "direction", "orientation", "disabled"],
-            gg = (0, se.ZP)(Ct, {
+        const yg = (0, ue.Z)("MuiTabScrollButton", ["root", "vertical", "horizontal", "disabled"]);
+        var wg, Sg;
+        const Cg = ["className", "direction", "orientation", "disabled"],
+            kg = (0, se.ZP)(Ct, {
                 name: "MuiTabScrollButton",
                 slot: "Root",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
                     return [t.root, n.orientation && t[n.orientation]]
@@ -30132,96 +30363,96 @@
                 let {
                     ownerState: t
                 } = e;
                 return (0, a.Z)({
                     width: 40,
                     flexShrink: 0,
                     opacity: .8,
-                    ["&.".concat(pg.disabled)]: {
+                    ["&.".concat(yg.disabled)]: {
                         opacity: 0
                     }
                 }, "vertical" === t.orientation && {
                     width: "100%",
                     height: 40,
                     "& svg": {
                         transform: "rotate(".concat(t.isRtl ? -90 : 90, "deg)")
                     }
                 })
             })),
-            vg = t.forwardRef((function(e, t) {
+            Zg = t.forwardRef((function(e, t) {
                 const n = (0, le.Z)({
                         props: e,
                         name: "MuiTabScrollButton"
                     }),
                     {
                         className: r,
                         direction: o
                     } = n,
-                    i = (0, G.Z)(n, hg),
+                    i = (0, G.Z)(n, Cg),
                     s = "rtl" === dn().direction,
                     l = (0, a.Z)({
                         isRtl: s
                     }, n),
                     c = (e => {
                         const {
                             classes: t,
                             orientation: n,
                             disabled: r
                         } = e, o = {
                             root: ["root", n, r && "disabled"]
                         };
-                        return (0, ie.Z)(o, ug, t)
+                        return (0, ie.Z)(o, bg, t)
                     })(l);
-                return (0, _.jsx)(gg, (0, a.Z)({
+                return (0, _.jsx)(kg, (0, a.Z)({
                     component: "div",
                     className: (0, q.Z)(c.root, r),
                     ref: t,
                     role: null,
                     ownerState: l,
                     tabIndex: null
                 }, i, {
-                    children: "left" === o ? fg || (fg = (0, _.jsx)(cg, {
+                    children: "left" === o ? wg || (wg = (0, _.jsx)(vg, {
                         fontSize: "small"
-                    })) : mg || (mg = (0, _.jsx)(dg, {
+                    })) : Sg || (Sg = (0, _.jsx)(xg, {
                         fontSize: "small"
                     }))
                 }))
             }));
 
-        function xg(e) {
+        function jg(e) {
             return (0, de.Z)("MuiTabs", e)
         }
-        const bg = (0, ue.Z)("MuiTabs", ["root", "vertical", "flexContainer", "flexContainerVertical", "centered", "scroller", "fixed", "scrollableX", "scrollableY", "hideScrollbar", "scrollButtons", "scrollButtonsHideMobile", "indicator"]),
-            yg = ["aria-label", "aria-labelledby", "action", "centered", "children", "className", "component", "allowScrollButtonsMobile", "indicatorColor", "onChange", "orientation", "ScrollButtonComponent", "scrollButtons", "selectionFollowsFocus", "TabIndicatorProps", "TabScrollButtonProps", "textColor", "value", "variant", "visibleScrollbar"],
-            wg = (e, t) => e === t ? e.firstChild : t && t.nextElementSibling ? t.nextElementSibling : e.firstChild,
-            Sg = (e, t) => e === t ? e.lastChild : t && t.previousElementSibling ? t.previousElementSibling : e.lastChild,
-            Cg = (e, t, n) => {
+        const Pg = (0, ue.Z)("MuiTabs", ["root", "vertical", "flexContainer", "flexContainerVertical", "centered", "scroller", "fixed", "scrollableX", "scrollableY", "hideScrollbar", "scrollButtons", "scrollButtonsHideMobile", "indicator"]),
+            Eg = ["aria-label", "aria-labelledby", "action", "centered", "children", "className", "component", "allowScrollButtonsMobile", "indicatorColor", "onChange", "orientation", "ScrollButtonComponent", "scrollButtons", "selectionFollowsFocus", "TabIndicatorProps", "TabScrollButtonProps", "textColor", "value", "variant", "visibleScrollbar"],
+            Rg = (e, t) => e === t ? e.firstChild : t && t.nextElementSibling ? t.nextElementSibling : e.firstChild,
+            Mg = (e, t) => e === t ? e.lastChild : t && t.previousElementSibling ? t.previousElementSibling : e.lastChild,
+            Ig = (e, t, n) => {
                 let r = !1,
                     o = n(e, t);
                 for (; o;) {
                     if (o === e.firstChild) {
                         if (r) return;
                         r = !0
                     }
                     const t = o.disabled || "true" === o.getAttribute("aria-disabled");
                     if (o.hasAttribute("tabindex") && !t) return void o.focus();
                     o = n(e, o)
                 }
             },
-            kg = (0, se.ZP)("div", {
+            Tg = (0, se.ZP)("div", {
                 name: "MuiTabs",
                 slot: "Root",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
                     return [{
-                        ["& .".concat(bg.scrollButtons)]: t.scrollButtons
+                        ["& .".concat(Pg.scrollButtons)]: t.scrollButtons
                     }, {
-                        ["& .".concat(bg.scrollButtons)]: n.scrollButtonsHideMobile && t.scrollButtonsHideMobile
+                        ["& .".concat(Pg.scrollButtons)]: n.scrollButtonsHideMobile && t.scrollButtonsHideMobile
                     }, t.root, n.vertical && t.vertical]
                 }
             })((e => {
                 let {
                     ownerState: t,
                     theme: n
                 } = e;
@@ -30229,22 +30460,22 @@
                     overflow: "hidden",
                     minHeight: 48,
                     WebkitOverflowScrolling: "touch",
                     display: "flex"
                 }, t.vertical && {
                     flexDirection: "column"
                 }, t.scrollButtonsHideMobile && {
-                    ["& .".concat(bg.scrollButtons)]: {
+                    ["& .".concat(Pg.scrollButtons)]: {
                         [n.breakpoints.down("sm")]: {
                             display: "none"
                         }
                     }
                 })
             })),
-            Zg = (0, se.ZP)("div", {
+            Og = (0, se.ZP)("div", {
                 name: "MuiTabs",
                 slot: "Scroller",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
                     return [t.scroller, n.fixed && t.fixed, n.hideScrollbar && t.hideScrollbar, n.scrollableX && t.scrollableX, n.scrollableY && t.scrollableY]
@@ -30270,15 +30501,15 @@
                     overflowX: "auto",
                     overflowY: "hidden"
                 }, t.scrollableY && {
                     overflowY: "auto",
                     overflowX: "hidden"
                 })
             })),
-            jg = (0, se.ZP)("div", {
+            Ag = (0, se.ZP)("div", {
                 name: "MuiTabs",
                 slot: "FlexContainer",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
                     return [t.flexContainer, n.vertical && t.flexContainerVertical, n.centered && t.centered]
@@ -30291,15 +30522,15 @@
                     display: "flex"
                 }, t.vertical && {
                     flexDirection: "column"
                 }, t.centered && {
                     justifyContent: "center"
                 })
             })),
-            Pg = (0, se.ZP)("span", {
+            Ng = (0, se.ZP)("span", {
                 name: "MuiTabs",
                 slot: "Indicator",
                 overridesResolver: (e, t) => t.indicator
             })((e => {
                 let {
                     ownerState: t,
                     theme: n
@@ -30316,48 +30547,48 @@
                     backgroundColor: n.palette.secondary.main
                 }, t.vertical && {
                     height: "100%",
                     width: 2,
                     right: 0
                 })
             })),
-            Eg = (0, se.ZP)((function(e) {
+            zg = (0, se.ZP)((function(e) {
                 const {
                     onChange: n
-                } = e, r = (0, G.Z)(e, sg), o = t.useRef(), i = t.useRef(null), s = () => {
+                } = e, r = (0, G.Z)(e, hg), o = t.useRef(), i = t.useRef(null), s = () => {
                     o.current = i.current.offsetHeight - i.current.clientHeight
                 };
                 return t.useEffect((() => {
                     const e = (0, ws.Z)((() => {
                             const e = o.current;
                             s(), e !== o.current && n(o.current)
                         })),
                         t = (0, Ss.Z)(i.current);
                     return t.addEventListener("resize", e), () => {
                         e.clear(), t.removeEventListener("resize", e)
                     }
                 }), [n]), t.useEffect((() => {
                     s(), n(o.current)
                 }), [n]), (0, _.jsx)("div", (0, a.Z)({
-                    style: lg,
+                    style: gg,
                     ref: i
                 }, r))
             }), {
                 name: "MuiTabs",
                 slot: "ScrollbarSize"
             })({
                 overflowX: "auto",
                 overflowY: "hidden",
                 scrollbarWidth: "none",
                 "&::-webkit-scrollbar": {
                     display: "none"
                 }
             }),
-            Rg = {};
-        const Mg = t.forwardRef((function(e, n) {
+            Dg = {};
+        const Lg = t.forwardRef((function(e, n) {
                 const r = (0, le.Z)({
                         props: e,
                         name: "MuiTabs"
                     }),
                     o = dn(),
                     i = "rtl" === o.direction,
                     {
@@ -30368,25 +30599,25 @@
                         children: u,
                         className: p,
                         component: f = "div",
                         allowScrollButtonsMobile: m = !1,
                         indicatorColor: h = "primary",
                         onChange: g,
                         orientation: v = "horizontal",
-                        ScrollButtonComponent: x = vg,
+                        ScrollButtonComponent: x = Zg,
                         scrollButtons: b = "auto",
                         selectionFollowsFocus: y,
                         TabIndicatorProps: w = {},
                         TabScrollButtonProps: S = {},
                         textColor: C = "primary",
                         value: k,
                         variant: Z = "standard",
                         visibleScrollbar: j = !1
                     } = r,
-                    P = (0, G.Z)(r, yg),
+                    P = (0, G.Z)(r, Eg),
                     E = "scrollable" === Z,
                     R = "vertical" === v,
                     M = R ? "scrollTop" : "scrollLeft",
                     I = R ? "top" : "left",
                     T = R ? "bottom" : "right",
                     O = R ? "clientHeight" : "clientWidth",
                     A = R ? "height" : "width",
@@ -30422,32 +30653,32 @@
                             scroller: ["scroller", n && "fixed", r && "hideScrollbar", o && "scrollableX", a && "scrollableY"],
                             flexContainer: ["flexContainer", t && "flexContainerVertical", i && "centered"],
                             indicator: ["indicator"],
                             scrollButtons: ["scrollButtons", s && "scrollButtonsHideMobile"],
                             scrollableX: [o && "scrollableX"],
                             hideScrollbar: [r && "hideScrollbar"]
                         };
-                        return (0, ie.Z)(c, xg, l)
+                        return (0, ie.Z)(c, jg, l)
                     })(N);
-                const [D, L] = t.useState(!1), [F, W] = t.useState(Rg), [B, V] = t.useState({
+                const [D, L] = t.useState(!1), [F, W] = t.useState(Dg), [B, U] = t.useState({
                     start: !1,
                     end: !1
-                }), [U, H] = t.useState({
+                }), [V, H] = t.useState({
                     overflow: "hidden",
                     scrollbarWidth: 0
                 }), $ = new Map, K = t.useRef(null), X = t.useRef(null), Y = () => {
                     const e = K.current;
                     let t, n;
                     if (e) {
                         const n = e.getBoundingClientRect();
                         t = {
                             clientWidth: e.clientWidth,
                             scrollLeft: e.scrollLeft,
                             scrollTop: e.scrollTop,
-                            scrollLeftNormalized: ag(e, o.direction),
+                            scrollLeftNormalized: fg(e, o.direction),
                             scrollWidth: e.scrollWidth,
                             top: n.top,
                             bottom: n.bottom,
                             left: n.left,
                             right: n.right
                         }
                     }
@@ -30487,15 +30718,15 @@
                     let {
                         animation: t = !0
                     } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     t ? function(e, t, n) {
                         let r = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : {},
                             o = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : () => {};
                         const {
-                            ease: a = ig,
+                            ease: a = mg,
                             duration: i = 300
                         } = r;
                         let s = null;
                         const l = t[e];
                         let c = !1;
                         const d = () => {
                                 c = !0
@@ -30510,15 +30741,15 @@
                             };
                         l === n ? o(new Error("Element already at target position")) : requestAnimationFrame(u)
                     }(M, K.current, e, {
                         duration: o.transitions.duration.standard
                     }) : K.current[M] = e
                 }, ee = e => {
                     let t = K.current[M];
-                    R ? t += e : (t += e * (i ? -1 : 1), t *= i && "reverse" === og() ? -1 : 1), J(t)
+                    R ? t += e : (t += e * (i ? -1 : 1), t *= i && "reverse" === pg() ? -1 : 1), J(t)
                 }, te = () => {
                     const e = K.current[O];
                     let t = 0;
                     const n = Array.from(X.current.children);
                     for (let r = 0; r < n.length; r += 1) {
                         const o = n[r];
                         if (t + o[O] > e) break;
@@ -30559,18 +30790,18 @@
                             clientHeight: n,
                             scrollWidth: r,
                             clientWidth: a
                         } = K.current;
                         let s, l;
                         if (R) s = e > 1, l = e < t - n - 1;
                         else {
-                            const e = ag(K.current, o.direction);
+                            const e = fg(K.current, o.direction);
                             s = i ? e < r - a - 1 : e > 1, l = i ? e > 1 : e < r - a - 1
                         }
-                        s === B.start && l === B.end || V({
+                        s === B.start && l === B.end || U({
                             start: s,
                             end: l
                         })
                     }
                 }));
                 t.useEffect((() => {
                     const e = (0, ws.Z)((() => {
@@ -30590,20 +30821,20 @@
                 t.useEffect((() => () => {
                     ce.clear()
                 }), [ce]), t.useEffect((() => {
                     L(!0)
                 }), []), t.useEffect((() => {
                     Q(), se()
                 })), t.useEffect((() => {
-                    ae(Rg !== F)
+                    ae(Dg !== F)
                 }), [ae, F]), t.useImperativeHandle(c, (() => ({
                     updateIndicator: Q,
                     updateScrollButtons: se
                 })), [Q, se]);
-                const de = (0, _.jsx)(Pg, (0, a.Z)({}, w, {
+                const de = (0, _.jsx)(Ng, (0, a.Z)({}, w, {
                     className: (0, q.Z)(z.indicator, w.className),
                     ownerState: N,
                     style: (0, a.Z)({}, F, w.style)
                 }));
                 let ue = 0;
                 const pe = t.Children.map(u, (e => {
                         if (!t.isValidElement(e)) return null;
@@ -30620,15 +30851,15 @@
                             value: n
                         }, 1 !== ue || !1 !== k || e.props.tabIndex ? {} : {
                             tabIndex: 0
                         }))
                     })),
                     fe = (() => {
                         const e = {};
-                        e.scrollbarSizeListener = E ? (0, _.jsx)(Eg, {
+                        e.scrollbarSizeListener = E ? (0, _.jsx)(zg, {
                             onChange: oe,
                             className: (0, q.Z)(z.scrollableX, z.hideScrollbar)
                         }) : null;
                         const t = B.start || B.end,
                             n = E && ("auto" === b && t || !0 === b);
                         return e.scrollButtonStart = n ? (0, _.jsx)(x, (0, a.Z)({
                             orientation: v,
@@ -30642,70 +30873,70 @@
                             direction: i ? "left" : "right",
                             onClick: re,
                             disabled: !B.end
                         }, S, {
                             className: (0, q.Z)(z.scrollButtons, S.className)
                         })) : null, e
                     })();
-                return (0, _.jsxs)(kg, (0, a.Z)({
+                return (0, _.jsxs)(Tg, (0, a.Z)({
                     className: (0, q.Z)(z.root, p),
                     ownerState: N,
                     ref: n,
                     as: f
                 }, P, {
-                    children: [fe.scrollButtonStart, fe.scrollbarSizeListener, (0, _.jsxs)(Zg, {
+                    children: [fe.scrollButtonStart, fe.scrollbarSizeListener, (0, _.jsxs)(Og, {
                         className: z.scroller,
                         ownerState: N,
                         style: {
-                            overflow: U.overflow,
-                            [R ? "margin".concat(i ? "Left" : "Right") : "marginBottom"]: j ? void 0 : -U.scrollbarWidth
+                            overflow: V.overflow,
+                            [R ? "margin".concat(i ? "Left" : "Right") : "marginBottom"]: j ? void 0 : -V.scrollbarWidth
                         },
                         ref: K,
                         onScroll: ce,
-                        children: [(0, _.jsx)(jg, {
+                        children: [(0, _.jsx)(Ag, {
                             "aria-label": s,
                             "aria-labelledby": l,
                             "aria-orientation": "vertical" === v ? "vertical" : null,
                             className: z.flexContainer,
                             ownerState: N,
                             onKeyDown: e => {
                                 const t = X.current,
                                     n = (0, is.Z)(t).activeElement;
                                 if ("tab" !== n.getAttribute("role")) return;
                                 let r = "horizontal" === v ? "ArrowLeft" : "ArrowUp",
                                     o = "horizontal" === v ? "ArrowRight" : "ArrowDown";
                                 switch ("horizontal" === v && i && (r = "ArrowRight", o = "ArrowLeft"), e.key) {
                                     case r:
-                                        e.preventDefault(), Cg(t, n, Sg);
+                                        e.preventDefault(), Ig(t, n, Mg);
                                         break;
                                     case o:
-                                        e.preventDefault(), Cg(t, n, wg);
+                                        e.preventDefault(), Ig(t, n, Rg);
                                         break;
                                     case "Home":
-                                        e.preventDefault(), Cg(t, null, wg);
+                                        e.preventDefault(), Ig(t, null, Rg);
                                         break;
                                     case "End":
-                                        e.preventDefault(), Cg(t, null, Sg)
+                                        e.preventDefault(), Ig(t, null, Mg)
                                 }
                             },
                             ref: X,
                             role: "tablist",
                             children: pe
                         }), D && de]
                     }), fe.scrollButtonEnd]
                 }))
             })),
-            Ig = Mg;
+            Fg = Lg;
 
-        function Tg(e) {
+        function Wg(e) {
             return (0, de.Z)("MuiTab", e)
         }
-        const Og = (0, ue.Z)("MuiTab", ["root", "labelIcon", "textColorInherit", "textColorPrimary", "textColorSecondary", "selected", "disabled", "fullWidth", "wrapped", "iconWrapper"]),
-            Ag = ["className", "disabled", "disableFocusRipple", "fullWidth", "icon", "iconPosition", "indicator", "label", "onChange", "onClick", "onFocus", "selected", "selectionFollowsFocus", "textColor", "value", "wrapped"],
-            Ng = (0, se.ZP)(Ct, {
+        const Bg = (0, ue.Z)("MuiTab", ["root", "labelIcon", "textColorInherit", "textColorPrimary", "textColorSecondary", "selected", "disabled", "fullWidth", "wrapped", "iconWrapper"]),
+            _g = ["className", "disabled", "disableFocusRipple", "fullWidth", "icon", "iconPosition", "indicator", "label", "onChange", "onClick", "onFocus", "selected", "selectionFollowsFocus", "textColor", "value", "wrapped"],
+            Ug = (0, se.ZP)(Ct, {
                 name: "MuiTab",
                 slot: "Root",
                 overridesResolver: (e, t) => {
                     const {
                         ownerState: n
                     } = e;
                     return [t.root, n.label && n.icon && t.labelIcon, t["textColor".concat((0, ce.Z)(n.textColor))], n.fullWidth && t.fullWidth, n.wrapped && t.wrapped]
@@ -30729,58 +30960,58 @@
                     flexDirection: "top" === n.iconPosition || "bottom" === n.iconPosition ? "column" : "row"
                 }, {
                     lineHeight: 1.25
                 }, n.icon && n.label && {
                     minHeight: 72,
                     paddingTop: 9,
                     paddingBottom: 9,
-                    ["& > .".concat(Og.iconWrapper)]: (0, a.Z)({}, "top" === n.iconPosition && {
+                    ["& > .".concat(Bg.iconWrapper)]: (0, a.Z)({}, "top" === n.iconPosition && {
                         marginBottom: 6
                     }, "bottom" === n.iconPosition && {
                         marginTop: 6
                     }, "start" === n.iconPosition && {
                         marginRight: t.spacing(1)
                     }, "end" === n.iconPosition && {
                         marginLeft: t.spacing(1)
                     })
                 }, "inherit" === n.textColor && {
                     color: "inherit",
                     opacity: .6,
-                    ["&.".concat(Og.selected)]: {
+                    ["&.".concat(Bg.selected)]: {
                         opacity: 1
                     },
-                    ["&.".concat(Og.disabled)]: {
+                    ["&.".concat(Bg.disabled)]: {
                         opacity: t.palette.action.disabledOpacity
                     }
                 }, "primary" === n.textColor && {
                     color: t.palette.text.secondary,
-                    ["&.".concat(Og.selected)]: {
+                    ["&.".concat(Bg.selected)]: {
                         color: t.palette.primary.main
                     },
-                    ["&.".concat(Og.disabled)]: {
+                    ["&.".concat(Bg.disabled)]: {
                         color: t.palette.text.disabled
                     }
                 }, "secondary" === n.textColor && {
                     color: t.palette.text.secondary,
-                    ["&.".concat(Og.selected)]: {
+                    ["&.".concat(Bg.selected)]: {
                         color: t.palette.secondary.main
                     },
-                    ["&.".concat(Og.disabled)]: {
+                    ["&.".concat(Bg.disabled)]: {
                         color: t.palette.text.disabled
                     }
                 }, n.fullWidth && {
                     flexShrink: 1,
                     flexGrow: 1,
                     flexBasis: 0,
                     maxWidth: "none"
                 }, n.wrapped && {
                     fontSize: t.typography.pxToRem(12)
                 })
             })),
-            zg = t.forwardRef((function(e, n) {
+            Vg = t.forwardRef((function(e, n) {
                 const r = (0, le.Z)({
                         props: e,
                         name: "MuiTab"
                     }),
                     {
                         className: o,
                         disabled: i = !1,
@@ -30795,15 +31026,15 @@
                         onFocus: h,
                         selected: g,
                         selectionFollowsFocus: v,
                         textColor: x = "inherit",
                         value: b,
                         wrapped: y = !1
                     } = r,
-                    w = (0, G.Z)(r, Ag),
+                    w = (0, G.Z)(r, _g),
                     S = (0, a.Z)({}, r, {
                         disabled: i,
                         disableFocusRipple: s,
                         selected: g,
                         icon: !!c,
                         iconPosition: d,
                         label: !!p,
@@ -30821,20 +31052,20 @@
                             label: i,
                             selected: s,
                             disabled: l
                         } = e, c = {
                             root: ["root", a && i && "labelIcon", "textColor".concat((0, ce.Z)(n)), r && "fullWidth", o && "wrapped", s && "selected", l && "disabled"],
                             iconWrapper: ["iconWrapper"]
                         };
-                        return (0, ie.Z)(c, Tg, t)
+                        return (0, ie.Z)(c, Wg, t)
                     })(S),
                     k = c && p && t.isValidElement(c) ? t.cloneElement(c, {
                         className: (0, q.Z)(C.iconWrapper, c.props.className)
                     }) : c;
-                return (0, _.jsxs)(Ng, (0, a.Z)({
+                return (0, _.jsxs)(Ug, (0, a.Z)({
                     focusRipple: !s,
                     className: (0, q.Z)(C.root, o),
                     ref: n,
                     role: "tab",
                     "aria-selected": g,
                     disabled: i,
                     onClick: e => {
@@ -30849,46 +31080,46 @@
                     children: ["top" === d || "start" === d ? (0, _.jsxs)(t.Fragment, {
                         children: [k, p]
                     }) : (0, _.jsxs)(t.Fragment, {
                         children: [p, k]
                     }), u]
                 }))
             }));
-        var Dg = n(1758);
-        const Lg = ff(ve)((e => {
+        var Gg = n(1758);
+        const qg = ff(ve)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.palette.primary.main,
                     fontFamily: "'Roboto Condensed', sans-serif",
                     fontSize: 16,
                     fontWeight: 400
                 }
             })),
-            Fg = ff(ve)((e => {
+            Hg = ff(ve)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.palette.primary.main,
                     fontFamily: "'Roboto Condensed', sans-serif",
                     fontSize: 18,
                     fontWeight: 500
                 }
             })),
-            Wg = ff(ae)((e => {
+            $g = ff(ae)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     height: "1.5vh"
                 }
             }));
-        class Bg extends t.Component {
+        class Kg extends t.Component {
             constructor(e) {
                 super(e), this.loadPlanes = async () => {
                     try {
                         this.setState({
                             updating: !0
                         });
                         let e = await Qc().get("/AAZ/Specs/Planes");
@@ -31274,15 +31505,15 @@
                         ml: 1
                     },
                     children: [(0, _.jsx)(ha, {
                         edge: "start",
                         color: "inherit",
                         onClick: () => this.onRemoveAadScope(t),
                         "aria-label": "remove",
-                        children: (0, _.jsx)(Vm.Z, {
+                        children: (0, _.jsx)(Um.Z, {
                             fontSize: "small"
                         })
                     }), (0, _.jsx)(ki, {
                         id: "aadScope-".concat(t),
                         value: e,
                         onChange: e => {
                             this.onModifyAadScope(e.target.value, t)
@@ -31379,27 +31610,27 @@
                                 mt: 1
                             },
                             children: [(0, _.jsx)(ae, {
                                 sx: {
                                     borderBottom: 1,
                                     borderColor: "divider"
                                 },
-                                children: (0, _.jsxs)(Ig, {
+                                children: (0, _.jsxs)(Fg, {
                                     value: a,
                                     textColor: "secondary",
                                     indicatorColor: "secondary",
                                     onChange: (e, t) => {
                                         this.setState({
                                             endpointType: t
                                         })
                                     },
-                                    children: [(0, _.jsx)(zg, {
+                                    children: [(0, _.jsx)(Vg, {
                                         label: "By templates",
                                         value: "template"
-                                    }), (0, _.jsx)(zg, {
+                                    }), (0, _.jsx)(Vg, {
                                         label: "By resource property",
                                         value: "http-operation"
                                     })]
                                 })
                             }), "template" === a && (0, _.jsxs)(ae, {
                                 sx: {
                                     display: "flex",
@@ -31525,15 +31756,15 @@
                                         value: u,
                                         onChange: e => {
                                             this.setState({
                                                 cloudMetadataPrefixTemplate: e.target.value
                                             })
                                         },
                                         margin: "dense"
-                                    }), (0, _.jsx)(Dg.Z, {}), (0, _.jsx)(Fg, {
+                                    }), (0, _.jsx)(Gg.Z, {}), (0, _.jsx)(Hg, {
                                         sx: {
                                             flexShrink: 0,
                                             mr: 1
                                         },
                                         children: ".Suffix"
                                     })]
                                 })]
@@ -31550,37 +31781,37 @@
                                 },
                                 children: [(0, _.jsx)(yu, {
                                     name: "Module",
                                     commonPrefix: this.state.moduleOptionsCommonPrefix,
                                     options: this.state.moduleOptions,
                                     value: p,
                                     onValueUpdate: this.onModuleSelectionUpdate
-                                }), (0, _.jsx)(Wg, {}), (0, _.jsx)(yu, {
+                                }), (0, _.jsx)($g, {}), (0, _.jsx)(yu, {
                                     name: "Resource Provider",
                                     commonPrefix: this.state.resourceProviderOptionsCommonPrefix,
                                     options: this.state.resourceProviderOptions,
                                     value: f,
                                     onValueUpdate: this.onResourceProviderUpdate
-                                }), (0, _.jsx)(Wg, {}), (0, _.jsx)(yu, {
+                                }), (0, _.jsx)($g, {}), (0, _.jsx)(yu, {
                                     name: "API Version",
                                     commonPrefix: "",
                                     options: this.state.versionOptions,
                                     value: m,
                                     onValueUpdate: this.onVersionUpdate
-                                }), (0, _.jsx)(Wg, {}), (0, _.jsx)(yu, {
+                                }), (0, _.jsx)($g, {}), (0, _.jsx)(yu, {
                                     name: "Resource ID",
                                     commonPrefix: "",
                                     options: this.state.resourceIdOptions,
                                     value: h,
                                     onValueUpdate: e => {
                                         this.setState({
                                             selectedResourceId: e
                                         })
                                     }
-                                }), (0, _.jsx)(Wg, {}), (0, _.jsx)(rc, {
+                                }), (0, _.jsx)($g, {}), (0, _.jsx)(rc, {
                                     id: "subresource",
                                     label: "Endpoint Property Index",
                                     type: "text",
                                     InputLabelProps: {
                                         shrink: !0
                                     },
                                     fullWidth: !0,
@@ -31612,18 +31843,18 @@
                                 ml: 1
                             },
                             children: [(0, _.jsx)(ha, {
                                 edge: "start",
                                 color: "inherit",
                                 onClick: this.onAddAadScope,
                                 "aria-label": "add",
-                                children: (0, _.jsx)(Um.Z, {
+                                children: (0, _.jsx)(Vm.Z, {
                                     fontSize: "small"
                                 })
-                            }), (0, _.jsx)(Lg, {
+                            }), (0, _.jsx)(qg, {
                                 sx: {
                                     flexShrink: 0
                                 },
                                 children: " One more scope "
                             })]
                         })]
                     }), (0, _.jsxs)(Wc, {
@@ -31643,23 +31874,23 @@
                                 children: "Update"
                             })]
                         })]
                     })]
                 })
             }
         }
-        const _g = Bg,
-            Vg = t.forwardRef((function(e, t) {
+        const Xg = Kg,
+            Yg = t.forwardRef((function(e, t) {
                 return (0, _.jsx)(Au, {
                     direction: "up",
                     ref: t,
                     ...e
                 })
             }));
-        class Ug extends t.Component {
+        class Qg extends t.Component {
             constructor(e) {
                 super(e), this.loadWorkspace = async e => {
                     const {
                         workspaceUrl: t
                     } = this.state;
                     var n;
                     void 0 === e && (e = null === (n = this.state.selected) || void 0 === n ? void 0 : n.id);
@@ -31667,15 +31898,15 @@
                         let n = await Qc().get("/AAZ/Specs/Planes"),
                             r = n.data.map((e => e.name));
                         n = await Qc().get(t);
                         const o = Date.now(),
                             a = {},
                             i = {},
                             s = e => {
-                                const t = tg(e);
+                                const t = cg(e);
                                 return a[t.id] = t, {
                                     id: t.id,
                                     names: [...t.names]
                                 }
                             },
                             l = e => {
                                 var t, n;
@@ -31911,15 +32142,15 @@
                         onGenerate: this.handleGenerate,
                         onDelete: this.handleDelete,
                         onModify: this.handleModify
                     }), (0, _.jsxs)(ae, {
                         sx: {
                             display: "flex"
                         },
-                        children: [(0, _.jsxs)(Uu, {
+                        children: [(0, _.jsxs)(Vu, {
                             variant: "permanent",
                             sx: {
                                 width: 300,
                                 flexShrink: 0,
                                 "& .MuiDrawer-paper": {
                                     width: 300,
                                     boxSizing: "border-box"
@@ -31946,58 +32177,58 @@
                                     flexShrink: 0
                                 }
                             }), null != c && c.id.startsWith("group:") && (0, _.jsx)(bm, {
                                 workspaceUrl: u,
                                 commandGroup: c,
                                 reloadTimestamp: d,
                                 onUpdateCommandGroup: this.handleCommandGroupUpdate
-                            }), null != c && c.id.startsWith("command:") && (0, _.jsx)(ng, {
+                            }), null != c && c.id.startsWith("command:") && (0, _.jsx)(dg, {
                                 workspaceUrl: u,
                                 previewCommand: c,
                                 reloadTimestamp: d,
                                 onUpdateCommand: this.handleCommandUpdate
                             })]
                         })]
                     }), (0, _.jsx)(fc, {
                         fullScreen: !0,
                         open: e,
                         onClose: this.handleSwaggerResourcePickerClose,
-                        TransitionComponent: Vg,
+                        TransitionComponent: Yg,
                         children: (0, _.jsx)(wu, {
                             plane: i,
                             workspaceName: s,
                             onClose: this.handleSwaggerResourcePickerClose
                         })
-                    }), a && (0, _.jsx)($g, {
+                    }), a && (0, _.jsx)(nv, {
                         workspaceUrl: u,
                         workspaceName: s,
                         open: a,
                         onClose: this.handleModifyClose
-                    }), o && (0, _.jsx)(qg, {
+                    }), o && (0, _.jsx)(ev, {
                         workspaceName: s,
                         open: o,
                         onClose: this.handleDeleteClose
-                    }), r && (0, _.jsx)(Gg, {
+                    }), r && (0, _.jsx)(Jg, {
                         workspaceUrl: u,
                         open: r,
                         clientConfigurable: m,
                         onClose: this.handleGenerationClose
-                    }), n && (0, _.jsx)(Hg, {
+                    }), n && (0, _.jsx)(tv, {
                         workspaceUrl: u,
                         open: n,
                         onClose: this.handleSwaggerReloadDialogClose
-                    }), f && (0, _.jsx)(_g, {
+                    }), f && (0, _.jsx)(Xg, {
                         workspaceUrl: u,
                         open: f,
                         onClose: this.handleClientConfigDialogClose
                     })]
                 })
             }
         }
-        class Gg extends t.Component {
+        class Jg extends t.Component {
             constructor(e) {
                 super(e), this.handleClose = () => {
                     this.props.onClose(!1, !1)
                 }, this.verifyClientConfig = async () => {
                     const e = "".concat(this.props.workspaceUrl, "/ClientConfig/AAZ/Compare");
                     this.setState({
                         updating: !0
@@ -32114,15 +32345,15 @@
                             })]
                         })]
                     })]
                 })
             }
         }
 
-        function qg(e) {
+        function ev(e) {
             const [n, r] = t.useState(!1), [o, a] = t.useState(void 0), [i, s] = t.useState(void 0);
             return (0, _.jsxs)(fc, {
                 disableEscapeKeyDown: !0,
                 open: e.open,
                 children: [(0, _.jsxs)(xc, {
                     children: ["Delete '", e.workspaceName, "' workspace?"]
                 }), (0, _.jsxs)(Sc, {
@@ -32177,15 +32408,15 @@
                             disabled: e.workspaceName !== i,
                             children: "Confirm"
                         })]
                     })]
                 })]
             })
         }
-        class Hg extends t.Component {
+        class tv extends t.Component {
             constructor(e) {
                 super(e), this.loadResourceOptions = async () => {
                     this.setState({
                         invalidText: void 0,
                         updating: !0
                     });
                     try {
@@ -32386,15 +32617,15 @@
                                 children: "Reload"
                             })]
                         })]
                     })]
                 })
             }
         }
-        class $g extends t.Component {
+        class nv extends t.Component {
             constructor(e) {
                 super(e), this.handleModify = e => {
                     let {
                         newWSName: t
                     } = this.state, {
                         workspaceUrl: n,
                         workspaceName: r
@@ -32486,41 +32717,41 @@
                                 children: "Save"
                             })]
                         })]
                     })]
                 })
             }
         }
-        const Kg = e => {
+        const rv = e => {
             const t = k();
-            return (0, _.jsx)(Ug, {
+            return (0, _.jsx)(Qg, {
                 params: t,
                 ...e
             })
         };
-        class Xg extends t.Component {
+        class ov extends t.Component {
             render() {
                 return (0, _.jsx)(t.Fragment, {
                     children: (0, _.jsx)(lr, {
                         pageName: "Commands"
                     })
                 })
             }
         }
-        const Yg = $n(Xg);
-        class Qg extends t.Component {
+        const av = $n(ov);
+        class iv extends t.Component {
             render() {
                 return (0, _.jsx)(t.Fragment, {
                     children: (0, _.jsx)(v, {})
                 })
             }
         }
-        const Jg = $n(Qg),
-            ev = Er();
-        class tv extends t.Component {
+        const sv = $n(iv),
+            lv = Er();
+        class cv extends t.Component {
             constructor(e) {
                 super(e), this.loadModules = () => {
                     Qc().get("/CLI/Az/" + this.props.repo + "/Modules").then((e => {
                         let t = e.data.map((e => ({
                             name: e.name,
                             folder: e.folder,
                             url: e.url
@@ -32610,15 +32841,15 @@
                                     name: t.inputValue,
                                     url: null,
                                     folder: null
                                 }
                             }) : this.onValueUpdated(t)
                         },
                         filterOptions: (e, t) => {
-                            const n = ev(e, t);
+                            const n = lv(e, t);
                             return "" !== t.inputValue && -1 === e.findIndex((e => e.name === t.inputValue)) && n.push({
                                 inputValue: t.inputValue,
                                 title: 'Create "'.concat(t.inputValue, '"')
                             }), n
                         },
                         getOptionLabel: e => "string" === typeof e ? e : e.title ? e.title : e.name,
                         renderOption: (e, t) => {
@@ -32677,32 +32908,32 @@
                                 })]
                             })]
                         })
                     })]
                 })
             }
         }
-        const nv = tv,
-            rv = (0, se.ZP)(ae)((e => {
+        const dv = cv,
+            uv = (0, se.ZP)(ae)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     height: "6vh"
                 }
             })),
-            ov = (0, se.ZP)(ae)((e => {
+            pv = (0, se.ZP)(ae)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     width: "3vh"
                 }
             }));
-        class av extends t.Component {
+        class fv extends t.Component {
             render() {
                 return (0, _.jsxs)(t.Fragment, {
                     children: [(0, _.jsx)(lr, {
                         pageName: "CLI"
                     }), (0, _.jsx)(gr, {
                         children: (0, _.jsxs)(ae, {
                             sx: {
@@ -32724,44 +32955,44 @@
                                     justifyContent: "center",
                                     flexDirection: "column"
                                 },
                                 children: [(0, _.jsx)(ve, {
                                     variant: "h3",
                                     gutterBottom: !0,
                                     children: "Please select a CLI Module"
-                                }), (0, _.jsx)(rv, {}), (0, _.jsxs)(ae, {
+                                }), (0, _.jsx)(uv, {}), (0, _.jsxs)(ae, {
                                     sx: {
                                         display: "flex",
                                         flexDirection: "row",
                                         alignItems: "center"
                                     },
-                                    children: [(0, _.jsx)(nv, {
+                                    children: [(0, _.jsx)(dv, {
                                         repo: "Main",
                                         name: "Azure CLI Module"
-                                    }), (0, _.jsx)(ov, {}), (0, _.jsx)(ve, {
+                                    }), (0, _.jsx)(pv, {}), (0, _.jsx)(ve, {
                                         variant: "h6",
                                         gutterBottom: !0,
                                         children: "Or"
-                                    }), (0, _.jsx)(ov, {}), (0, _.jsx)(nv, {
+                                    }), (0, _.jsx)(pv, {}), (0, _.jsx)(dv, {
                                         repo: "Extension",
                                         name: "Azure CLI Extension Module"
                                     })]
                                 })]
                             }), (0, _.jsx)(ae, {
                                 sx: {
                                     flexGrow: 5
                                 }
                             })]
                         })
                     })]
                 })
             }
         }
-        const iv = av;
-        class sv extends t.Component {
+        const mv = fv;
+        class hv extends t.Component {
             render() {
                 const {
                     moduleName: e,
                     onHomePage: n,
                     onGenerate: r
                 } = this.props;
                 return (0, _.jsx)(t.Fragment, {
@@ -32822,83 +33053,83 @@
                                 })
                             })]
                         })
                     })
                 })
             }
         }
-        const lv = sv;
-        var cv = n(215),
-            dv = n(6759),
-            uv = n(3717);
-        const pv = (0, se.ZP)(ve)((e => {
+        const gv = hv;
+        var vv = n(215),
+            xv = n(6759),
+            bv = n(3717);
+        const yv = (0, se.ZP)(ve)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.palette.primary.main,
                     fontFamily: "'Work Sans', sans-serif",
                     fontSize: 17,
                     fontWeight: 600
                 }
             })),
-            fv = (0, se.ZP)(ve)((e => {
+            wv = (0, se.ZP)(ve)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.palette.primary.main,
                     fontFamily: "'Work Sans', sans-serif",
                     fontSize: 20,
                     fontWeight: 400
                 }
             })),
-            mv = (0, se.ZP)(ve)((e => {
+            Sv = (0, se.ZP)(ve)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: t.palette.grey[700],
                     fontFamily: "'Work Sans', sans-serif",
                     fontSize: 15,
                     fontWeight: 400
                 }
             })),
-            hv = (0, se.ZP)(mv)((e => {
+            Cv = (0, se.ZP)(Sv)((e => {
                 let {
                     theme: t
                 } = e;
                 return {}
             })),
-            gv = (0, se.ZP)(mv)((e => {
+            kv = (0, se.ZP)(Sv)((e => {
                 let {
                     theme: t
                 } = e;
                 return {
                     color: "#d9c136"
                 }
             }));
-        class vv extends t.Component {
+        class Zv extends t.Component {
             constructor(e) {
                 var t;
                 super(e), this.onSelectCommandGroup = (e, t) => {
-                    let n = Cv(this.props.profileCommandTree, e, t);
+                    let n = Iv(this.props.profileCommandTree, e, t);
                     this.props.onChange(n)
                 }, this.onSelectCommand = (e, t) => {
-                    let n = Cv(this.props.profileCommandTree, e, t);
+                    let n = Iv(this.props.profileCommandTree, e, t);
                     this.props.onChange(n)
                 }, this.onSelectCommandVersion = (e, t) => {
-                    let n = Cv(this.props.profileCommandTree, e, !0, t);
+                    let n = Iv(this.props.profileCommandTree, e, !0, t);
                     this.props.onChange(n)
                 }, this.onSelectCommandRegistered = (e, t) => {
-                    let n = Cv(this.props.profileCommandTree, e, !0, void 0, t);
+                    let n = Iv(this.props.profileCommandTree, e, !0, void 0, t);
                     this.props.onChange(n)
                 }, this.state = {
                     defaultExpanded: (t = this.props.profileCommandTree, t.commandGroups.flatMap((e => {
-                        let t = yv(e);
+                        let t = Ev(e);
                         return e.selectedCommands > 0 && t.push(e.id), t
                     })))
                 }
             }
             render() {
                 const {
                     defaultExpanded: e
@@ -32931,15 +33162,15 @@
                                     marginLeft: 1,
                                     minWidth: 100,
                                     display: "flex",
                                     flexDirection: "row",
                                     alignItems: "center",
                                     justifyContent: "flex-start"
                                 },
-                                children: [(0, _.jsx)(fv, {
+                                children: [(0, _.jsx)(wv, {
                                     children: t
                                 }), (0, _.jsxs)(ae, {
                                     sx: {
                                         marginLeft: 1,
                                         width: 20,
                                         display: "flex",
                                         flexDirection: "row",
@@ -32981,15 +33212,15 @@
                                         value: e.selectedVersion,
                                         onChange: t => {
                                             this.onSelectCommandVersion(e.id, t.target.value)
                                         },
                                         size: "small",
                                         children: e.versions.map((t => (0, _.jsx)(Hd, {
                                             value: t.name,
-                                            children: (0, _.jsx)(mv, {
+                                            children: (0, _.jsx)(Sv, {
                                                 children: t.name
                                             })
                                         }, "".concat(e.id, "-version-select-").concat(t.name))))
                                     })]
                                 }), (0, _.jsxs)(Ji, {
                                     sx: {
                                         minWidth: 150,
@@ -33004,20 +33235,20 @@
                                         value: e.registered ? 1 : 0,
                                         onChange: t => {
                                             this.onSelectCommandRegistered(e.id, 1 === t.target.value)
                                         },
                                         size: "small",
                                         children: [(0, _.jsx)(Hd, {
                                             value: 1,
-                                            children: (0, _.jsx)(hv, {
+                                            children: (0, _.jsx)(Cv, {
                                                 children: "Registered"
                                             })
                                         }, "".concat(e.id, "-register-select-registered")), (0, _.jsx)(Hd, {
                                             value: 0,
-                                            children: (0, _.jsx)(gv, {
+                                            children: (0, _.jsx)(kv, {
                                                 children: "Unregistered"
                                             })
                                         }, "".concat(e.id, "-register-select-unregistered"))]
                                     })]
                                 })]
                             })]
                         }),
@@ -33045,15 +33276,15 @@
                             children: [(0, _.jsx)(kd, {
                                 disableRipple: !0,
                                 checked: o,
                                 indeterminate: !o && e.selectedCommands > 0,
                                 onClick: t => {
                                     this.onSelectCommandGroup(e.id, !o), t.stopPropagation(), t.preventDefault()
                                 }
-                            }), (0, _.jsx)(uv.Z, {}), (0, _.jsx)(pv, {
+                            }), (0, _.jsx)(bv.Z, {}), (0, _.jsx)(yv, {
                                 sx: {
                                     marginLeft: 1
                                 },
                                 children: t
                             })]
                         }),
                         onClick: e => {
@@ -33062,23 +33293,23 @@
                         children: [void 0 !== e.commands && e.commands.map((e => n(e))), void 0 !== e.commandGroups && e.commandGroups.map((e => r(e)))]
                     }, e.id)
                 };
                 return (0, _.jsx)(t.Fragment, {
                     children: (0, _.jsx)(ef, {
                         disableSelection: !0,
                         defaultExpanded: e,
-                        defaultCollapseIcon: (0, _.jsx)(dv.Z, {}),
-                        defaultExpandIcon: (0, _.jsx)(cv.Z, {}),
+                        defaultCollapseIcon: (0, _.jsx)(xv.Z, {}),
+                        defaultExpandIcon: (0, _.jsx)(vv.Z, {}),
                         children: this.props.profileCommandTree.commandGroups.map((e => r(e)))
                     })
                 })
             }
         }
 
-        function xv(e) {
+        function jv(e) {
             var t, n;
             let r = void 0 !== e.commands ? Object.keys(e.commands).map((t => function(e) {
                     let t = e.versions.map((e => function(e) {
                         return {
                             name: e.name,
                             stage: e.stage
                         }
@@ -33087,40 +33318,40 @@
                         id: e.names.join("/"),
                         names: [...e.names],
                         help: e.help.short,
                         versions: t,
                         modified: !1
                     }
                 }(e.commands[t]))) : void 0,
-                o = void 0 !== e.commandGroups ? Object.keys(e.commandGroups).map((t => xv(e.commandGroups[t]))) : void 0,
+                o = void 0 !== e.commandGroups ? Object.keys(e.commandGroups).map((t => jv(e.commandGroups[t]))) : void 0,
                 a = null !== (t = null === r || void 0 === r ? void 0 : r.length) && void 0 !== t ? t : 0;
             return a = null !== (n = null === o || void 0 === o ? void 0 : o.reduce(((e, t) => e + t.totalCommands), a)) && void 0 !== n ? n : a, {
                 id: e.names.join("/"),
                 names: [...e.names],
                 help: e.help.short,
                 commandGroups: o,
                 commands: r,
                 totalCommands: a,
                 selectedCommands: 0
             }
         }
 
-        function bv(e, t) {
+        function Pv(e, t) {
             return {
                 name: e,
-                commandGroups: void 0 !== t.commandGroups ? Object.keys(t.commandGroups).map((e => xv(t.commandGroups[e]))) : []
+                commandGroups: void 0 !== t.commandGroups ? Object.keys(t.commandGroups).map((e => jv(t.commandGroups[e]))) : []
             }
         }
 
-        function yv(e) {
+        function Ev(e) {
             var t, n;
-            return null !== (t = null === (n = e.commandGroups) || void 0 === n ? void 0 : n.flatMap((e => [e.id, ...yv(e)]))) && void 0 !== t ? t : []
+            return null !== (t = null === (n = e.commandGroups) || void 0 === n ? void 0 : n.flatMap((e => [e.id, ...Ev(e)]))) && void 0 !== t ? t : []
         }
 
-        function wv(e, t, n, r, o) {
+        function Rv(e, t, n, r, o) {
             if (e.id !== t) return e;
             if (n) {
                 var a, i;
                 let t = null !== (a = null !== r && void 0 !== r ? r : e.selectedVersion) && void 0 !== a ? a : e.versions[0].name,
                     n = null === (i = null !== o && void 0 !== o ? o : e.registered) || void 0 === i || i;
                 return {
                     ...e,
@@ -33133,40 +33364,40 @@
                 ...e,
                 selectedVersion: void 0,
                 registered: void 0,
                 modified: !0
             }
         }
 
-        function Sv(e, t, n, r, o) {
+        function Mv(e, t, n, r, o) {
             var a, i, s, l;
             if (e.id !== t && !t.startsWith("".concat(e.id, "/"))) return e;
             let c, d;
             var u, p, f, m;
-            e.id === t ? (c = null === (u = e.commands) || void 0 === u ? void 0 : u.map((e => wv(e, e.id, n, r, o))), d = null === (p = e.commandGroups) || void 0 === p ? void 0 : p.map((e => Sv(e, e.id, n, r, o)))) : (c = null === (f = e.commands) || void 0 === f ? void 0 : f.map((e => wv(e, t, n, r, o))), d = null === (m = e.commandGroups) || void 0 === m ? void 0 : m.map((e => Sv(e, t, n, r, o))));
+            e.id === t ? (c = null === (u = e.commands) || void 0 === u ? void 0 : u.map((e => Rv(e, e.id, n, r, o))), d = null === (p = e.commandGroups) || void 0 === p ? void 0 : p.map((e => Mv(e, e.id, n, r, o)))) : (c = null === (f = e.commands) || void 0 === f ? void 0 : f.map((e => Rv(e, t, n, r, o))), d = null === (m = e.commandGroups) || void 0 === m ? void 0 : m.map((e => Mv(e, t, n, r, o))));
             let h = null !== (a = null === (i = c) || void 0 === i ? void 0 : i.reduce(((e, t) => void 0 !== t.selectedVersion ? e + 1 : e), 0)) && void 0 !== a ? a : 0;
             return h += null !== (s = null === (l = d) || void 0 === l ? void 0 : l.reduce(((e, t) => e + t.selectedCommands), 0)) && void 0 !== s ? s : 0, {
                 ...e,
                 commands: c,
                 commandGroups: d,
                 selectedCommands: h
             }
         }
 
-        function Cv(e, t, n) {
+        function Iv(e, t, n) {
             let r = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : void 0,
                 o = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : void 0,
-                a = e.commandGroups.map((e => Sv(e, t, n, r, o)));
+                a = e.commandGroups.map((e => Mv(e, t, n, r, o)));
             return {
                 ...e,
                 commandGroups: a
             }
         }
 
-        function kv(e, t) {
+        function Tv(e, t) {
             var n, r, o, a;
             if (e.id !== t.names.join("/")) throw new Error("Invalid command group names: " + t.names.join(" "));
             let i = e.commands;
             if (void 0 !== t.commands) {
                 var s;
                 let n = new Set(Object.keys(t.commands));
                 if (i = null === (s = e.commands) || void 0 === s ? void 0 : s.map((e => n.has(e.names[e.names.length - 1]) ? (n.delete(e.names[e.names.length - 1]), function(e, t) {
@@ -33183,15 +33414,15 @@
                     })), new Error("Miss commands in aaz: " + e.join(", "))
                 }
             }
             let l = e.commandGroups;
             if (void 0 !== t.commandGroups) {
                 var c;
                 let n = new Set(Object.keys(t.commandGroups));
-                if (l = null === (c = e.commandGroups) || void 0 === c ? void 0 : c.map((e => n.has(e.names[e.names.length - 1]) ? (n.delete(e.names[e.names.length - 1]), kv(e, t.commandGroups[e.names[e.names.length - 1]])) : e)), n.size > 0) {
+                if (l = null === (c = e.commandGroups) || void 0 === c ? void 0 : c.map((e => n.has(e.names[e.names.length - 1]) ? (n.delete(e.names[e.names.length - 1]), Tv(e, t.commandGroups[e.names[e.names.length - 1]])) : e)), n.size > 0) {
                     let e = [];
                     throw n.forEach((n => {
                         e.push("`az " + t.commandGroups[n].names.join(" ") + "`")
                     })), new Error("Miss command groups in aaz: " + e.join(", "))
                 }
             }
             let d = null !== (n = null === (r = i) || void 0 === r ? void 0 : r.reduce(((e, t) => void 0 !== t.selectedVersion ? e + 1 : e), 0)) && void 0 !== n ? n : 0;
@@ -33200,98 +33431,98 @@
                 commands: i,
                 commandGroups: l,
                 selectedCommands: d,
                 waitCommand: t.waitCommand
             }
         }
 
-        function Zv(e) {
+        function Ov(e) {
             if (0 === e.selectedCommands) return;
             let t, n;
             return void 0 !== e.commands && (t = {}, e.commands.forEach((e => {
                 let n = function(e) {
                     if (void 0 !== e.selectedVersion) return {
                         names: e.names,
                         registered: e.registered,
                         version: e.selectedVersion,
                         modified: e.modified
                     }
                 }(e);
                 void 0 !== n && (t[e.names[e.names.length - 1]] = n)
             }))), void 0 !== e.commandGroups && (n = {}, e.commandGroups.forEach((e => {
-                let t = Zv(e);
+                let t = Ov(e);
                 void 0 !== t && (n[e.names[e.names.length - 1]] = t)
             }))), {
                 names: e.names,
                 commandGroups: n,
                 commands: t,
                 waitCommand: e.waitCommand
             }
         }
 
-        function jv(e) {
+        function Av(e) {
             let t = {};
             return e.commandGroups.forEach((e => {
-                let n = Zv(e);
+                let n = Ov(e);
                 void 0 !== n && (t[e.names[e.names.length - 1]] = n)
             })), {
                 name: e.name,
                 commandGroups: t
             }
         }
-        const Pv = vv;
-        class Ev extends t.Component {
+        const Nv = Zv;
+        class zv extends t.Component {
             render() {
                 const {
                     value: e,
                     profiles: t,
                     onChange: n
                 } = this.props;
-                return (0, _.jsx)(Ig, {
+                return (0, _.jsx)(Fg, {
                     orientation: "vertical",
                     variant: "scrollable",
                     value: e,
                     onChange: (e, t) => {
                         n(t)
                     },
                     "aria-label": "Vertical tabs example",
                     sx: {
                         borderRight: 1,
                         borderColor: "divider"
                     },
-                    children: t.map(((e, t) => (0, _.jsx)(zg, {
+                    children: t.map(((e, t) => (0, _.jsx)(Vg, {
                         label: e,
                         id: "vertical-tab-".concat(t),
                         "aria-controls": "vertical-tabpanel-".concat(t)
                     }, t)))
                 })
             }
         }
-        const Rv = Ev;
-        class Mv extends t.Component {
+        const Dv = zv;
+        class Lv extends t.Component {
             constructor(e) {
                 super(e), this.loadModule = async () => {
                     try {
                         this.setState({
                             loading: !0
                         });
                         let e = await Qc().get("/CLI/Az/Profiles"),
                             t = e.data;
                         e = await Qc().get("/AAZ/Specs/CommandTree/Nodes/aaz");
-                        let n = t.map((t => bv(t, e.data)));
+                        let n = t.map((t => Pv(t, e.data)));
                         e = await Qc().get("/CLI/Az/".concat(this.props.params.repoName, "/Modules/").concat(this.props.params.moduleName));
                         let r = e.data;
                         Object.keys(r.profiles).forEach((e => {
                             let o = t.findIndex((t => t === e));
                             if (-1 === o) throw new Error("Invalid profile ".concat(e));
                             n[o] = function(e, t) {
                                 let n = e.commandGroups;
                                 if (void 0 !== t.commandGroups) {
                                     let r = new Set(Object.keys(t.commandGroups));
-                                    if (n = e.commandGroups.map((e => r.has(e.names[e.names.length - 1]) ? (r.delete(e.names[e.names.length - 1]), kv(e, t.commandGroups[e.names[e.names.length - 1]])) : e)), r.size > 0) {
+                                    if (n = e.commandGroups.map((e => r.has(e.names[e.names.length - 1]) ? (r.delete(e.names[e.names.length - 1]), Tv(e, t.commandGroups[e.names[e.names.length - 1]])) : e)), r.size > 0) {
                                         let e = [];
                                         throw r.forEach((n => {
                                             e.push("`az " + t.commandGroups[n].names.join(" ") + "`")
                                         })), new Error("Miss command groups in aaz: " + e.join(", "))
                                     }
                                 }
                                 return {
@@ -33360,53 +33591,53 @@
                     showGenerateDialog: e,
                     selectedProfileIdx: n,
                     selectedCommandTree: r,
                     profiles: o,
                     commandTrees: a
                 } = this.state;
                 return (0, _.jsxs)(t.Fragment, {
-                    children: [(0, _.jsx)(lv, {
+                    children: [(0, _.jsx)(gv, {
                         moduleName: this.props.params.moduleName,
                         onHomePage: this.handleBackToHomepage,
                         onGenerate: this.handleGenerate
                     }), (0, _.jsxs)(ae, {
                         sx: {
                             display: "flex"
                         },
-                        children: [(0, _.jsxs)(Uu, {
+                        children: [(0, _.jsxs)(Vu, {
                             variant: "permanent",
                             sx: {
                                 width: 300,
                                 flexShrink: 0,
                                 "& .MuiDrawer-paper": {
                                     width: 300,
                                     boxSizing: "border-box"
                                 }
                             },
-                            children: [(0, _.jsx)(sr, {}), void 0 !== n && (0, _.jsx)(Rv, {
+                            children: [(0, _.jsx)(sr, {}), void 0 !== n && (0, _.jsx)(Dv, {
                                 value: n,
                                 profiles: o,
                                 onChange: this.onProfileChange
                             })]
                         }), (0, _.jsxs)(ae, {
                             component: "main",
                             sx: {
                                 flexGrow: 1,
                                 p: 2
                             },
                             children: [(0, _.jsx)(sr, {
                                 sx: {
                                     flexShrink: 0
                                 }
-                            }), void 0 !== r && (0, _.jsx)(Pv, {
+                            }), void 0 !== r && (0, _.jsx)(Nv, {
                                 profileCommandTree: r,
                                 onChange: this.onSelectedProfileTreeUpdate
                             })]
                         })]
-                    }), e && (0, _.jsx)(Iv, {
+                    }), e && (0, _.jsx)(Fv, {
                         repoName: this.props.params.repoName,
                         moduleName: this.props.params.moduleName,
                         profileCommandTrees: a,
                         open: e,
                         onClose: this.handleGenerationClose
                     }), (0, _.jsxs)(Js, {
                         sx: {
@@ -33435,15 +33666,15 @@
                             color: "inherit"
                         })]
                     })]
                 })
             }
         }
 
-        function Iv(e) {
+        function Fv(e) {
             const [n, r] = t.useState(!1), [o, a] = t.useState(void 0);
             return (0, _.jsxs)(fc, {
                 disableEscapeKeyDown: !0,
                 open: e.open,
                 children: [(0, _.jsxs)(xc, {
                     children: ["Generate CLI commands to ", e.moduleName]
                 }), (0, _.jsx)(Sc, {
@@ -33466,15 +33697,15 @@
                                 e.onClose(!1)
                             },
                             children: "Cancel"
                         }), (0, _.jsx)(Xc, {
                             onClick: () => {
                                 const t = {};
                                 e.profileCommandTrees.forEach((e => {
-                                    t[e.name] = jv(e)
+                                    t[e.name] = Av(e)
                                 }));
                                 const n = {
                                     name: e.moduleName,
                                     profiles: t
                                 };
                                 r(!0), Qc().put("/CLI/Az/".concat(e.repoName, "/Modules/").concat(e.moduleName), n).then((() => {
                                     r(!1), e.onClose(!0)
@@ -33488,15 +33719,15 @@
                                 }))
                             },
                             children: "Generate All"
                         }), (0, _.jsx)(Xc, {
                             onClick: () => {
                                 const t = {};
                                 e.profileCommandTrees.forEach((e => {
-                                    t[e.name] = jv(e)
+                                    t[e.name] = Av(e)
                                 }));
                                 const n = {
                                     name: e.moduleName,
                                     profiles: t
                                 };
                                 r(!0), Qc().patch("/CLI/Az/".concat(e.repoName, "/Modules/").concat(e.moduleName), n).then((() => {
                                     r(!1), e.onClose(!0)
@@ -33511,27 +33742,27 @@
                             },
                             children: "Generate Edited Only"
                         })]
                     })]
                 })]
             })
         }
-        const Tv = e => {
+        const Wv = e => {
             const t = k();
-            return (0, _.jsx)(Mv, {
+            return (0, _.jsx)(Lv, {
                 params: t,
                 ...e
             })
         };
         o.render((0, _.jsx)(t.StrictMode, {
             children: (0, _.jsx)(B, {
                 children: (0, _.jsx)(y, {
                     children: (0, _.jsxs)(x, {
                         path: "/",
-                        element: (0, _.jsx)(U, {}),
+                        element: (0, _.jsx)(V, {}),
                         children: [(0, _.jsx)(x, {
                             index: !0,
                             element: (0, _.jsx)(yr, {})
                         }), (0, _.jsx)(x, {
                             path: "HomePage",
                             element: (0, _.jsx)(yr, {})
                         }), (0, _.jsxs)(x, {
@@ -33541,33 +33772,33 @@
                                 index: !0,
                                 element: (0, _.jsx)(Mu, {})
                             }), (0, _.jsx)(x, {
                                 path: "Instruction",
                                 element: (0, _.jsx)(Mu, {})
                             }), (0, _.jsx)(x, {
                                 path: ":workspaceName",
-                                element: (0, _.jsx)(Kg, {})
+                                element: (0, _.jsx)(rv, {})
                             })]
                         }), (0, _.jsx)(x, {
                             path: "Commands",
-                            element: (0, _.jsx)(Yg, {})
+                            element: (0, _.jsx)(av, {})
                         }), (0, _.jsxs)(x, {
                             path: "CLI",
-                            element: (0, _.jsx)(Jg, {}),
+                            element: (0, _.jsx)(sv, {}),
                             children: [(0, _.jsx)(x, {
                                 index: !0,
-                                element: (0, _.jsx)(iv, {})
+                                element: (0, _.jsx)(mv, {})
                             }), (0, _.jsx)(x, {
                                 path: "Instruction",
-                                element: (0, _.jsx)(iv, {})
+                                element: (0, _.jsx)(mv, {})
                             }), (0, _.jsx)(x, {
                                 path: ":repoName/:moduleName",
-                                element: (0, _.jsx)(Tv, {})
+                                element: (0, _.jsx)(Wv, {})
                             })]
                         })]
                     })
                 })
             })
         }), document.getElementById("root"))
     })()
 })();
-//# sourceMappingURL=main.aa1f209d.js.map
+//# sourceMappingURL=main.90022267.js.map
```

### Comparing `aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js.LICENSE.txt` & `aaz_dev-2.7.0/src/aaz_dev/ui/static/js/main.90022267.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/ui/static/js/main.aa1f209d.js.map` & `aaz_dev-2.7.0/src/aaz_dev/ui/static/js/main.90022267.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8559886277321614%*

 * *Differences: {"'file'": "'static/js/main.90022267.js'",*

 * * "'mappings'": "';yDAqDA,IAAIA,EAA0B,WAC5B,SAASA,EAAWC,GAClB,IAAIC,EAAQC,KAEZA,KAAKC,WAAa,SAAUC,GAC1B,IAAIC,EAIAA,EAFsB,IAAtBJ,EAAMK,KAAKC,OACTN,EAAMO,eACCP,EAAMO,eAAeC,YACrBR,EAAMS,QACNT,EAAMU,UAAUC,WAEhBX,EAAMI,OAGRJ,EAAMK,KAAKL,EAAMK,KAAKC,OAAS,GAAGE,YAG7CR,EAAMU,UAAUE,aAAaT,EAAKC,GAElCJ,EAAMK,KAAKQ,KAAKV,EACjB,EAEDF,KAAKa,cAA8BC,IAAnBhB,EAAQiB,QAA+DjB,EAAQiB,OAC/Ff,KAAKI,KAAO,GACZJ,KAAKgB,IAAM,EACXhB,KAAKiB,MAAQnB,EAAQmB,MAErBjB,KAAKkB,IAAMpB,EAAQoB,IACnBlB,KAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.aa1f209d.js",
+    "file": "static/js/main.90022267.js",
     "names": [
         "StyleSheet",
         "options",
         "_this",
         "this",
         "_insertTag",
         "tag",
@@ -661,14 +661,20 @@
         "createEmptyBreakpointObject",
         "breakpointsInput",
         "_breakpointsInput$key",
         "removeUnusedBreakpoints",
         "breakpointKeys",
         "style",
         "breakpointOutput",
+        "resolveBreakpointValues",
+        "breakpointValues",
+        "base",
+        "customBase",
+        "breakpointsKeys",
+        "computeBreakpointsBase",
         "clamp",
         "min",
         "max",
         "decomposeColor",
         "charAt",
         "re",
         "RegExp",
@@ -843,15 +849,14 @@
         "inputProps",
         "styleFunction",
         "sx",
         "traverse",
         "sxInput",
         "sxObject",
         "emptyBreakpoints",
-        "breakpointsKeys",
         "css",
         "styleKey",
         "maybeFn",
         "objects",
         "allKeys",
         "object",
         "union",
@@ -1353,15 +1358,14 @@
         "rb",
         "sb",
         "tb",
         "setProperty",
         "ub",
         "menuitem",
         "area",
-        "base",
         "br",
         "col",
         "embed",
         "hr",
         "img",
         "keygen",
         "link",
@@ -4577,14 +4581,21 @@
         "displayUnwrapClsDialog",
         "setDisplayUnwrapClsDialog",
         "argStackNames",
         "onAddSubCommand",
         "onReloadArgs",
         "flattened",
         "unwrapped",
+        "joinChildren",
+        "separator",
+        "StackRoot",
+        "directionValues",
+        "spacingValues",
+        "Stack",
+        "ExampleItemSelector",
         "commandPrefix",
         "ExampleCommandHeaderTypography",
         "ExampleCommandBodyTypography",
         "ExampleEditTypography",
         "ExampleAccordionSummary",
         "Label",
         "WSEditorCommandContent",
@@ -4643,15 +4654,20 @@
         "exampleCommands",
         "cmdLine",
         "newExample",
         "handleAdd",
         "onModifyExampleCommand",
         "onRemoveExampleCommand",
         "onAddExampleCommand",
+        "loadSwaggerExamples",
+        "exampleOptions",
+        "onExampleSelectorUpdate",
+        "exampleDisplayName",
         "isAdd",
+        "selectedName",
         "DoDisturbOnRounded",
         "AddCircleRounded",
         "commandGroupName",
         "setCommandGroupName",
         "refArgsOptions",
         "setRefArgsOptions",
         "verifyAddSubresource",
@@ -5415,14 +5431,16 @@
         "../node_modules/@mui/material/InputAdornment/InputAdornment.js",
         "../node_modules/@mui/material/AccordionSummary/accordionSummaryClasses.js",
         "../node_modules/@mui/material/AccordionSummary/AccordionSummary.js",
         "../node_modules/@mui/material/Switch/switchClasses.js",
         "../node_modules/@mui/material/Switch/Switch.js",
         "views/workspace/argument/WSECArgumentSimilarPicker.tsx",
         "views/workspace/WSEditorCommandArgumentsContent.tsx",
+        "../node_modules/@mui/material/Stack/Stack.js",
+        "views/workspace/WSEditorExamplePicker.tsx",
         "views/workspace/WSEditorCommandContent.tsx",
         "../node_modules/@mui/utils/esm/scrollLeft.js",
         "../node_modules/@mui/material/internal/animate.js",
         "../node_modules/@mui/material/Tabs/ScrollbarSize.js",
         "../node_modules/@mui/material/internal/svg-icons/KeyboardArrowLeft.js",
         "../node_modules/@mui/material/internal/svg-icons/KeyboardArrowRight.js",
         "../node_modules/@mui/material/TabScrollButton/tabScrollButtonClasses.js",
@@ -5909,15 +5927,17 @@
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\n\nvar _span;\n\nconst _excluded = [\"children\", \"className\", \"component\", \"disablePointerEvents\", \"disableTypography\", \"position\", \"variant\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport capitalize from '../utils/capitalize';\nimport Typography from '../Typography';\nimport FormControlContext from '../FormControl/FormControlContext';\nimport useFormControl from '../FormControl/useFormControl';\nimport styled from '../styles/styled';\nimport inputAdornmentClasses, { getInputAdornmentUtilityClass } from './inputAdornmentClasses';\nimport useThemeProps from '../styles/useThemeProps';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\n\nconst overridesResolver = (props, styles) => {\n  const {\n    ownerState\n  } = props;\n  return [styles.root, styles[`position${capitalize(ownerState.position)}`], ownerState.disablePointerEvents === true && styles.disablePointerEvents, styles[ownerState.variant]];\n};\n\nconst useUtilityClasses = ownerState => {\n  const {\n    classes,\n    disablePointerEvents,\n    hiddenLabel,\n    position,\n    size,\n    variant\n  } = ownerState;\n  const slots = {\n    root: ['root', disablePointerEvents && 'disablePointerEvents', position && `position${capitalize(position)}`, variant, hiddenLabel && 'hiddenLabel', size && `size${capitalize(size)}`]\n  };\n  return composeClasses(slots, getInputAdornmentUtilityClass, classes);\n};\n\nconst InputAdornmentRoot = styled('div', {\n  name: 'MuiInputAdornment',\n  slot: 'Root',\n  overridesResolver\n})(({\n  theme,\n  ownerState\n}) => _extends({\n  display: 'flex',\n  height: '0.01em',\n  // Fix IE11 flexbox alignment. To remove at some point.\n  maxHeight: '2em',\n  alignItems: 'center',\n  whiteSpace: 'nowrap',\n  color: theme.palette.action.active\n}, ownerState.variant === 'filled' && {\n  // Styles applied to the root element if `variant=\"filled\"`.\n  [`&.${inputAdornmentClasses.positionStart}&:not(.${inputAdornmentClasses.hiddenLabel})`]: {\n    marginTop: 16\n  }\n}, ownerState.position === 'start' && {\n  // Styles applied to the root element if `position=\"start\"`.\n  marginRight: 8\n}, ownerState.position === 'end' && {\n  // Styles applied to the root element if `position=\"end\"`.\n  marginLeft: 8\n}, ownerState.disablePointerEvents === true && {\n  // Styles applied to the root element if `disablePointerEvents={true}`.\n  pointerEvents: 'none'\n}));\nconst InputAdornment = /*#__PURE__*/React.forwardRef(function InputAdornment(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiInputAdornment'\n  });\n\n  const {\n    children,\n    className,\n    component = 'div',\n    disablePointerEvents = false,\n    disableTypography = false,\n    position,\n    variant: variantProp\n  } = props,\n        other = _objectWithoutPropertiesLoose(props, _excluded);\n\n  const muiFormControl = useFormControl() || {};\n  let variant = variantProp;\n\n  if (variantProp && muiFormControl.variant) {\n    if (process.env.NODE_ENV !== 'production') {\n      if (variantProp === muiFormControl.variant) {\n        console.error('MUI: The `InputAdornment` variant infers the variant prop ' + 'you do not have to provide one.');\n      }\n    }\n  }\n\n  if (muiFormControl && !variant) {\n    variant = muiFormControl.variant;\n  }\n\n  const ownerState = _extends({}, props, {\n    hiddenLabel: muiFormControl.hiddenLabel,\n    size: muiFormControl.size,\n    disablePointerEvents,\n    position,\n    variant\n  });\n\n  const classes = useUtilityClasses(ownerState);\n  return /*#__PURE__*/_jsx(FormControlContext.Provider, {\n    value: null,\n    children: /*#__PURE__*/_jsx(InputAdornmentRoot, _extends({\n      as: component,\n      ownerState: ownerState,\n      className: clsx(classes.root, className),\n      ref: ref\n    }, other, {\n      children: typeof children === 'string' && !disableTypography ? /*#__PURE__*/_jsx(Typography, {\n        color: \"text.secondary\",\n        children: children\n      }) : /*#__PURE__*/_jsxs(React.Fragment, {\n        children: [position === 'start' ?\n        /* notranslate needed while Google Translate will not fix zero-width space issue */\n        _span || (_span = /*#__PURE__*/_jsx(\"span\", {\n          className: \"notranslate\",\n          children: \"\\u200B\"\n        })) : null, children]\n      })\n    }))\n  });\n});\nprocess.env.NODE_ENV !== \"production\" ? InputAdornment.propTypes\n/* remove-proptypes */\n= {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n\n  /**\n   * The content of the component, normally an `IconButton` or string.\n   */\n  children: PropTypes.node,\n\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n\n  /**\n   * Disable pointer events on the root.\n   * This allows for the content of the adornment to focus the `input` on click.\n   * @default false\n   */\n  disablePointerEvents: PropTypes.bool,\n\n  /**\n   * If children is a string then disable wrapping in a Typography component.\n   * @default false\n   */\n  disableTypography: PropTypes.bool,\n\n  /**\n   * The position this adornment should appear relative to the `Input`.\n   */\n  position: PropTypes.oneOf(['end', 'start']).isRequired,\n\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object]),\n\n  /**\n   * The variant to use.\n   * Note: If you are using the `TextField` component or the `FormControl` component\n   * you do not have to set this manually.\n   */\n  variant: PropTypes.oneOf(['filled', 'outlined', 'standard'])\n} : void 0;\nexport default InputAdornment;",
         "import { generateUtilityClass, generateUtilityClasses } from '@mui/base';\nexport function getAccordionSummaryUtilityClass(slot) {\n  return generateUtilityClass('MuiAccordionSummary', slot);\n}\nconst accordionSummaryClasses = generateUtilityClasses('MuiAccordionSummary', ['root', 'expanded', 'focusVisible', 'disabled', 'gutters', 'contentGutters', 'content', 'expandIconWrapper']);\nexport default accordionSummaryClasses;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"children\", \"className\", \"expandIcon\", \"focusVisibleClassName\", \"onClick\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\nimport ButtonBase from '../ButtonBase';\nimport AccordionContext from '../Accordion/AccordionContext';\nimport accordionSummaryClasses, { getAccordionSummaryUtilityClass } from './accordionSummaryClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\n\nconst useUtilityClasses = ownerState => {\n  const {\n    classes,\n    expanded,\n    disabled,\n    disableGutters\n  } = ownerState;\n  const slots = {\n    root: ['root', expanded && 'expanded', disabled && 'disabled', !disableGutters && 'gutters'],\n    focusVisible: ['focusVisible'],\n    content: ['content', expanded && 'expanded', !disableGutters && 'contentGutters'],\n    expandIconWrapper: ['expandIconWrapper', expanded && 'expanded']\n  };\n  return composeClasses(slots, getAccordionSummaryUtilityClass, classes);\n};\n\nconst AccordionSummaryRoot = styled(ButtonBase, {\n  name: 'MuiAccordionSummary',\n  slot: 'Root',\n  overridesResolver: (props, styles) => styles.root\n})(({\n  theme,\n  ownerState\n}) => {\n  const transition = {\n    duration: theme.transitions.duration.shortest\n  };\n  return _extends({\n    display: 'flex',\n    minHeight: 48,\n    padding: theme.spacing(0, 2),\n    transition: theme.transitions.create(['min-height', 'background-color'], transition),\n    [`&.${accordionSummaryClasses.focusVisible}`]: {\n      backgroundColor: theme.palette.action.focus\n    },\n    [`&.${accordionSummaryClasses.disabled}`]: {\n      opacity: theme.palette.action.disabledOpacity\n    },\n    [`&:hover:not(.${accordionSummaryClasses.disabled})`]: {\n      cursor: 'pointer'\n    }\n  }, !ownerState.disableGutters && {\n    [`&.${accordionSummaryClasses.expanded}`]: {\n      minHeight: 64\n    }\n  });\n});\nconst AccordionSummaryContent = styled('div', {\n  name: 'MuiAccordionSummary',\n  slot: 'Content',\n  overridesResolver: (props, styles) => styles.content\n})(({\n  theme,\n  ownerState\n}) => _extends({\n  display: 'flex',\n  flexGrow: 1,\n  margin: '12px 0'\n}, !ownerState.disableGutters && {\n  transition: theme.transitions.create(['margin'], {\n    duration: theme.transitions.duration.shortest\n  }),\n  [`&.${accordionSummaryClasses.expanded}`]: {\n    margin: '20px 0'\n  }\n}));\nconst AccordionSummaryExpandIconWrapper = styled('div', {\n  name: 'MuiAccordionSummary',\n  slot: 'ExpandIconWrapper',\n  overridesResolver: (props, styles) => styles.expandIconWrapper\n})(({\n  theme\n}) => ({\n  display: 'flex',\n  color: theme.palette.action.active,\n  transform: 'rotate(0deg)',\n  transition: theme.transitions.create('transform', {\n    duration: theme.transitions.duration.shortest\n  }),\n  [`&.${accordionSummaryClasses.expanded}`]: {\n    transform: 'rotate(180deg)'\n  }\n}));\nconst AccordionSummary = /*#__PURE__*/React.forwardRef(function AccordionSummary(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiAccordionSummary'\n  });\n\n  const {\n    children,\n    className,\n    expandIcon,\n    focusVisibleClassName,\n    onClick\n  } = props,\n        other = _objectWithoutPropertiesLoose(props, _excluded);\n\n  const {\n    disabled = false,\n    disableGutters,\n    expanded,\n    toggle\n  } = React.useContext(AccordionContext);\n\n  const handleChange = event => {\n    if (toggle) {\n      toggle(event);\n    }\n\n    if (onClick) {\n      onClick(event);\n    }\n  };\n\n  const ownerState = _extends({}, props, {\n    expanded,\n    disabled,\n    disableGutters\n  });\n\n  const classes = useUtilityClasses(ownerState);\n  return /*#__PURE__*/_jsxs(AccordionSummaryRoot, _extends({\n    focusRipple: false,\n    disableRipple: true,\n    disabled: disabled,\n    component: \"div\",\n    \"aria-expanded\": expanded,\n    className: clsx(classes.root, className),\n    focusVisibleClassName: clsx(classes.focusVisible, focusVisibleClassName),\n    onClick: handleChange,\n    ref: ref,\n    ownerState: ownerState\n  }, other, {\n    children: [/*#__PURE__*/_jsx(AccordionSummaryContent, {\n      className: classes.content,\n      ownerState: ownerState,\n      children: children\n    }), expandIcon && /*#__PURE__*/_jsx(AccordionSummaryExpandIconWrapper, {\n      className: classes.expandIconWrapper,\n      ownerState: ownerState,\n      children: expandIcon\n    })]\n  }));\n});\nprocess.env.NODE_ENV !== \"production\" ? AccordionSummary.propTypes\n/* remove-proptypes */\n= {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n\n  /**\n   * The icon to display as the expand indicator.\n   */\n  expandIcon: PropTypes.node,\n\n  /**\n   * This prop can help identify which element has keyboard focus.\n   * The class name will be applied when the element gains the focus through keyboard interaction.\n   * It's a polyfill for the [CSS :focus-visible selector](https://drafts.csswg.org/selectors-4/#the-focus-visible-pseudo).\n   * The rationale for using this feature [is explained here](https://github.com/WICG/focus-visible/blob/HEAD/explainer.md).\n   * A [polyfill can be used](https://github.com/WICG/focus-visible) to apply a `focus-visible` class to other components\n   * if needed.\n   */\n  focusVisibleClassName: PropTypes.string,\n\n  /**\n   * @ignore\n   */\n  onClick: PropTypes.func,\n\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default AccordionSummary;",
         "import { generateUtilityClass, generateUtilityClasses } from '@mui/base';\nexport function getSwitchUtilityClass(slot) {\n  return generateUtilityClass('MuiSwitch', slot);\n}\nconst switchClasses = generateUtilityClasses('MuiSwitch', ['root', 'edgeStart', 'edgeEnd', 'switchBase', 'colorPrimary', 'colorSecondary', 'sizeSmall', 'sizeMedium', 'checked', 'disabled', 'input', 'thumb', 'track']);\nexport default switchClasses;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"className\", \"color\", \"edge\", \"size\", \"sx\"];\n// @inheritedComponent IconButton\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { refType } from '@mui/utils';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport { alpha, darken, lighten } from '@mui/system';\nimport capitalize from '../utils/capitalize';\nimport SwitchBase from '../internal/SwitchBase';\nimport useThemeProps from '../styles/useThemeProps';\nimport styled from '../styles/styled';\nimport switchClasses, { getSwitchUtilityClass } from './switchClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nimport { jsxs as _jsxs } from \"react/jsx-runtime\";\n\nconst useUtilityClasses = ownerState => {\n  const {\n    classes,\n    edge,\n    size,\n    color,\n    checked,\n    disabled\n  } = ownerState;\n  const slots = {\n    root: ['root', edge && `edge${capitalize(edge)}`, `size${capitalize(size)}`],\n    switchBase: ['switchBase', `color${capitalize(color)}`, checked && 'checked', disabled && 'disabled'],\n    thumb: ['thumb'],\n    track: ['track'],\n    input: ['input']\n  };\n  const composedClasses = composeClasses(slots, getSwitchUtilityClass, classes);\n  return _extends({}, classes, composedClasses);\n};\n\nconst SwitchRoot = styled('span', {\n  name: 'MuiSwitch',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, ownerState.edge && styles[`edge${capitalize(ownerState.edge)}`], styles[`size${capitalize(ownerState.size)}`]];\n  }\n})(({\n  ownerState\n}) => _extends({\n  display: 'inline-flex',\n  width: 34 + 12 * 2,\n  height: 14 + 12 * 2,\n  overflow: 'hidden',\n  padding: 12,\n  boxSizing: 'border-box',\n  position: 'relative',\n  flexShrink: 0,\n  zIndex: 0,\n  // Reset the stacking context.\n  verticalAlign: 'middle',\n  // For correct alignment with the text.\n  '@media print': {\n    colorAdjust: 'exact'\n  }\n}, ownerState.edge === 'start' && {\n  marginLeft: -8\n}, ownerState.edge === 'end' && {\n  marginRight: -8\n}, ownerState.size === 'small' && {\n  width: 40,\n  height: 24,\n  padding: 7,\n  [`& .${switchClasses.thumb}`]: {\n    width: 16,\n    height: 16\n  },\n  [`& .${switchClasses.switchBase}`]: {\n    padding: 4,\n    [`&.${switchClasses.checked}`]: {\n      transform: 'translateX(16px)'\n    }\n  }\n}));\nconst SwitchSwitchBase = styled(SwitchBase, {\n  name: 'MuiSwitch',\n  slot: 'SwitchBase',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.switchBase, {\n      [`& .${switchClasses.input}`]: styles.input\n    }, ownerState.color !== 'default' && styles[`color${capitalize(ownerState.color)}`]];\n  }\n})(({\n  theme\n}) => ({\n  position: 'absolute',\n  top: 0,\n  left: 0,\n  zIndex: 1,\n  // Render above the focus ripple.\n  color: theme.palette.mode === 'light' ? theme.palette.common.white : theme.palette.grey[300],\n  transition: theme.transitions.create(['left', 'transform'], {\n    duration: theme.transitions.duration.shortest\n  }),\n  [`&.${switchClasses.checked}`]: {\n    transform: 'translateX(20px)'\n  },\n  [`&.${switchClasses.disabled}`]: {\n    color: theme.palette.mode === 'light' ? theme.palette.grey[100] : theme.palette.grey[600]\n  },\n  [`&.${switchClasses.checked} + .${switchClasses.track}`]: {\n    opacity: 0.5\n  },\n  [`&.${switchClasses.disabled} + .${switchClasses.track}`]: {\n    opacity: theme.palette.mode === 'light' ? 0.12 : 0.2\n  },\n  [`& .${switchClasses.input}`]: {\n    left: '-100%',\n    width: '300%'\n  }\n}), ({\n  theme,\n  ownerState\n}) => _extends({\n  '&:hover': {\n    backgroundColor: alpha(theme.palette.action.active, theme.palette.action.hoverOpacity),\n    // Reset on touch devices, it doesn't add specificity\n    '@media (hover: none)': {\n      backgroundColor: 'transparent'\n    }\n  }\n}, ownerState.color !== 'default' && {\n  [`&.${switchClasses.checked}`]: {\n    color: theme.palette[ownerState.color].main,\n    '&:hover': {\n      backgroundColor: alpha(theme.palette[ownerState.color].main, theme.palette.action.hoverOpacity),\n      '@media (hover: none)': {\n        backgroundColor: 'transparent'\n      }\n    },\n    [`&.${switchClasses.disabled}`]: {\n      color: theme.palette.mode === 'light' ? lighten(theme.palette[ownerState.color].main, 0.62) : darken(theme.palette[ownerState.color].main, 0.55)\n    }\n  },\n  [`&.${switchClasses.checked} + .${switchClasses.track}`]: {\n    backgroundColor: theme.palette[ownerState.color].main\n  }\n}));\nconst SwitchTrack = styled('span', {\n  name: 'MuiSwitch',\n  slot: 'Track',\n  overridesResolver: (props, styles) => styles.track\n})(({\n  theme\n}) => ({\n  height: '100%',\n  width: '100%',\n  borderRadius: 14 / 2,\n  zIndex: -1,\n  transition: theme.transitions.create(['opacity', 'background-color'], {\n    duration: theme.transitions.duration.shortest\n  }),\n  backgroundColor: theme.palette.mode === 'light' ? theme.palette.common.black : theme.palette.common.white,\n  opacity: theme.palette.mode === 'light' ? 0.38 : 0.3\n}));\nconst SwitchThumb = styled('span', {\n  name: 'MuiSwitch',\n  slot: 'Thumb',\n  overridesResolver: (props, styles) => styles.thumb\n})(({\n  theme\n}) => ({\n  boxShadow: theme.shadows[1],\n  backgroundColor: 'currentColor',\n  width: 20,\n  height: 20,\n  borderRadius: '50%'\n}));\nconst Switch = /*#__PURE__*/React.forwardRef(function Switch(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiSwitch'\n  });\n\n  const {\n    className,\n    color = 'primary',\n    edge = false,\n    size = 'medium',\n    sx\n  } = props,\n        other = _objectWithoutPropertiesLoose(props, _excluded);\n\n  const ownerState = _extends({}, props, {\n    color,\n    edge,\n    size\n  });\n\n  const classes = useUtilityClasses(ownerState);\n\n  const icon = /*#__PURE__*/_jsx(SwitchThumb, {\n    className: classes.thumb,\n    ownerState: ownerState\n  });\n\n  return /*#__PURE__*/_jsxs(SwitchRoot, {\n    className: clsx(classes.root, className),\n    sx: sx,\n    ownerState: ownerState,\n    children: [/*#__PURE__*/_jsx(SwitchSwitchBase, _extends({\n      type: \"checkbox\",\n      icon: icon,\n      checkedIcon: icon,\n      ref: ref,\n      ownerState: ownerState\n    }, other, {\n      classes: _extends({}, classes, {\n        root: classes.switchBase\n      })\n    })), /*#__PURE__*/_jsx(SwitchTrack, {\n      className: classes.track,\n      ownerState: ownerState\n    })]\n  });\n});\nprocess.env.NODE_ENV !== \"production\" ? Switch.propTypes\n/* remove-proptypes */\n= {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n\n  /**\n   * If `true`, the component is checked.\n   */\n  checked: PropTypes.bool,\n\n  /**\n   * The icon to display when the component is checked.\n   */\n  checkedIcon: PropTypes.node,\n\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n\n  /**\n   * The color of the component. It supports those theme colors that make sense for this component.\n   * @default 'primary'\n   */\n  color: PropTypes\n  /* @typescript-to-proptypes-ignore */\n  .oneOfType([PropTypes.oneOf(['default', 'primary', 'secondary', 'error', 'info', 'success', 'warning']), PropTypes.string]),\n\n  /**\n   * The default checked state. Use when the component is not controlled.\n   */\n  defaultChecked: PropTypes.bool,\n\n  /**\n   * If `true`, the component is disabled.\n   */\n  disabled: PropTypes.bool,\n\n  /**\n   * If `true`, the ripple effect is disabled.\n   */\n  disableRipple: PropTypes.bool,\n\n  /**\n   * If given, uses a negative margin to counteract the padding on one\n   * side (this is often helpful for aligning the left or right\n   * side of the icon with content above or below, without ruining the border\n   * size and shape).\n   * @default false\n   */\n  edge: PropTypes.oneOf(['end', 'start', false]),\n\n  /**\n   * The icon to display when the component is unchecked.\n   */\n  icon: PropTypes.node,\n\n  /**\n   * The id of the `input` element.\n   */\n  id: PropTypes.string,\n\n  /**\n   * [Attributes](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#Attributes) applied to the `input` element.\n   */\n  inputProps: PropTypes.object,\n\n  /**\n   * Pass a ref to the `input` element.\n   */\n  inputRef: refType,\n\n  /**\n   * Callback fired when the state is changed.\n   *\n   * @param {React.ChangeEvent<HTMLInputElement>} event The event source of the callback.\n   * You can pull out the new value by accessing `event.target.value` (string).\n   * You can pull out the new checked state by accessing `event.target.checked` (boolean).\n   */\n  onChange: PropTypes.func,\n\n  /**\n   * If `true`, the `input` element is required.\n   */\n  required: PropTypes.bool,\n\n  /**\n   * The size of the component.\n   * `small` is equivalent to the dense switch styling.\n   * @default 'medium'\n   */\n  size: PropTypes\n  /* @typescript-to-proptypes-ignore */\n  .oneOfType([PropTypes.oneOf(['medium', 'small']), PropTypes.string]),\n\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object]),\n\n  /**\n   * The value of the component. The DOM API casts this to a string.\n   * The browser uses \"on\" as the default value.\n   */\n  value: PropTypes.any\n} : void 0;\nexport default Switch;",
         "import TreeView from '@mui/lab/TreeView';\nimport TreeItem from '@mui/lab/TreeItem';\nimport ExpandMoreIcon from '@mui/icons-material/ExpandMore';\nimport ChevronRightIcon from '@mui/icons-material/ChevronRight';\nimport { Checkbox, FormControlLabel } from '@mui/material';\n\ninterface ArgSimilarArg {\n    id: string,\n    var: string,\n    display: string,\n    indexes: string[],\n    isSelected: boolean,\n}\n\ninterface ArgSimilarCommand {\n    id: string,\n    name: string,\n    args: ArgSimilarArg[],\n    total: number,\n    selectedCount: number,\n}\n\ninterface ArgSimilarGroup {\n    id: string,\n    name: string,\n    groups?: ArgSimilarGroup[],\n    commands?: ArgSimilarCommand[],\n    total: number,\n    selectedCount: number,\n}\n\ninterface ArgSimilarTree {\n    root: ArgSimilarGroup,\n    selectedArgIds: string[],\n}\n\ninterface ResponseArgSimilarCommand {\n    id: string,\n    args: {\n        [argVar: string]: string[],\n    }\n}\n\ninterface ResponseArgSimilarGroup {\n    id: string,\n    commandGroups?: {\n        [name: string]: ResponseArgSimilarGroup\n    },\n    commands?: {\n        [name: string]: ResponseArgSimilarCommand\n    }\n}\n\n\nfunction decodeResponseArgSimilarCommand(responseCommand: ResponseArgSimilarCommand, commandName: string): ArgSimilarCommand {\n    let command: ArgSimilarCommand = {\n        id: responseCommand.id,\n        name: commandName,\n        args: [],\n        total: 0,\n        selectedCount: 0,\n    }\n    for (const argVar in responseCommand.args) {\n        const arg: ArgSimilarArg = {\n            id: `${command.id}/Arguments/${argVar}`,\n            var: argVar,\n            indexes: responseCommand.args[argVar],\n            display: \"\",\n            isSelected: false,\n        }\n        if (arg.indexes.length > 1) {\n            arg.display = `[${arg.var}] ${arg.indexes.map(idx => {\n                if (idx[1] === '.' || idx[1] === '[' || idx[1] === '{') {\n                    return `-${idx}`;\n                } else {\n                    return `--${idx}`;\n                }\n            }).join(' ')}`;\n        } else if (arg.indexes.length === 1) {\n            let idx = arg.indexes[0];\n            if (idx[1] === '.' || idx[1] === '[' || idx[1] === '{') {\n                arg.display = `-${idx}`;\n            } else {\n                arg.display = `--${idx}`;\n            }\n        }\n        command.args.push(arg);\n    }\n    command.total = command.args.length;\n    return command;\n}\n\nfunction decodeResponseArgSimilarGroup(responseGroup: ResponseArgSimilarGroup, groupName: string): ArgSimilarGroup {\n    let group: ArgSimilarGroup = {\n        id: responseGroup.id,\n        name: groupName,\n        total: 0,\n        selectedCount: 0,\n    }\n\n    if (typeof responseGroup.commandGroups === 'object' && responseGroup.commandGroups !== null) {\n        group.groups = [];\n        for (const name in responseGroup.commandGroups) {\n            const subGroup = decodeResponseArgSimilarGroup(responseGroup.commandGroups[name], name);\n            group.groups.push(subGroup);\n            group.total += subGroup.total;\n        }\n    }\n\n    if (typeof responseGroup.commands === 'object' && responseGroup.commands !== null) {\n        group.commands = [];\n        for (const name in responseGroup.commands) {\n            const command = decodeResponseArgSimilarCommand(responseGroup.commands[name], name);\n            group.commands.push(command);\n            group.total += command.total;\n        }\n    }\n    if (group.commands === undefined && group.groups !== undefined && group.groups.length === 1) {\n        group = group.groups[0]\n        group.name = `${groupName} ${group.name}`\n    }\n    return group;\n}\n\nfunction gatherNodeIds(group: ArgSimilarGroup): string[] {\n    let nodeIds: string[] = [group.id];\n    if (group.commands !== undefined) {\n        group.commands.forEach(command => {\n            nodeIds.push(command.id);\n        })\n    }\n    if (group.groups !== undefined) {\n        group.groups.forEach(subGroup => {\n            nodeIds = [...nodeIds, ...gatherNodeIds(subGroup)]\n        })\n    }\n    return nodeIds;\n}\n\n\nfunction BuildArgSimilarTree(response: any): {tree: ArgSimilarTree, expandedIds: string[]} {\n    const tree = {\n        root: decodeResponseArgSimilarGroup(response.data.aaz, 'az'),\n        selectedArgIds: [],\n    };\n    const expandedIds = gatherNodeIds(tree.root);\n    const newTree = updateSelectionStateForArgSimilarTree(tree, new Set<string>([tree.root.id]));\n    return {\n        tree: newTree,\n        expandedIds:  expandedIds,\n    };\n}\n\nfunction updateSelectionStateForArgSimilarCommand(command: ArgSimilarCommand, selectedIds: Set<string>): {command: ArgSimilarCommand, selectedArgIds: string[]} {\n    let newSelectedIds: string[] = [];\n    let newCommand = {\n        ...command,\n        args: command.args.map(arg => {\n            let isSelected = selectedIds.has(arg.id);\n            if (!isSelected) {\n                const idParts = arg.id.split('/');\n                for (let idx = 1; idx < idParts.length; idx += 1) {\n                    let newId = idParts.slice(0, idx+1).join('/');\n                    if (selectedIds.has(newId)) {\n                        isSelected = true;\n                        break;\n                    }\n                }\n            }\n            if (isSelected === true) {\n                newSelectedIds.push(arg.id);\n            }\n\n            let newArg: ArgSimilarArg = {\n                ...arg,\n                indexes: [...arg.indexes],\n                isSelected: isSelected,\n            }\n            return newArg\n        }),\n    }\n\n    newCommand.selectedCount = newSelectedIds.length\n    \n    return {\n        command: newCommand,\n        selectedArgIds: newSelectedIds,\n    };\n}\n\nfunction updateSelectionStateForArgSimilarGroup(group: ArgSimilarGroup, selectedIds: Set<string>): {group: ArgSimilarGroup, selectedArgIds: string[]} {\n    let newSelectedIds: string[] = [];\n    let newGroup = {\n        ...group,\n        groups: group.groups?.map(subGroup => {\n            const {group: newSubGroup, selectedArgIds: subSelectedIds} = updateSelectionStateForArgSimilarGroup(subGroup, selectedIds);\n            newSelectedIds = [...newSelectedIds, ...subSelectedIds];\n            return newSubGroup;\n        }),\n        commands: group.commands?.map(command => {\n            const {command: newCommand, selectedArgIds: subSelectedIds} = updateSelectionStateForArgSimilarCommand(command, selectedIds);\n            newSelectedIds = [...newSelectedIds, ...subSelectedIds];\n            return newCommand;\n        }),\n        \n    }\n\n    newGroup.selectedCount = newSelectedIds.length;\n\n    return {\n        group: newGroup,\n        selectedArgIds: newSelectedIds,\n    };\n}\n\nfunction updateSelectionStateForArgSimilarTree(tree: ArgSimilarTree, selectedIds: Set<string>): ArgSimilarTree {\n    const {group, selectedArgIds} = updateSelectionStateForArgSimilarGroup(tree.root, selectedIds);\n    return {\n        root: group,\n        selectedArgIds: selectedArgIds,\n    }\n}\n\nfunction WSECArgumentSimilarPicker(props: {\n    tree: ArgSimilarTree,\n    expandedIds: string[],\n    updatedIds: string[],\n    onTreeUpdated: (tree: ArgSimilarTree) => void,\n    onToggle: (nodeIds: string[]) => void\n}) {\n\n    const onCheckItem = (itemId: string, select: boolean) => {\n        let selectedIds: Set<string>;\n        if (select) {\n            selectedIds = new Set(props.tree.selectedArgIds).add(itemId);\n        } else {\n            selectedIds = new Set(props.tree.selectedArgIds.filter(id => id !== itemId && !id.startsWith(`${itemId}/`)));\n        }\n        props.onTreeUpdated(updateSelectionStateForArgSimilarTree(props.tree, selectedIds));\n    }\n\n    const onNodeToggle = (event: React.SyntheticEvent, nodeIds: string[]) => {\n        props.onToggle(nodeIds);\n        event.stopPropagation();\n        event.preventDefault();\n    }\n\n    const renderArg = (arg: ArgSimilarArg) => {\n        const isUpdated = props.updatedIds.indexOf(arg.id) !== -1\n        return (\n            <TreeItem key={arg.id} nodeId={arg.id} color='inherit'\n                label={\n                    <FormControlLabel\n                        control={<Checkbox\n                            size=\"small\"\n                            checked={arg.isSelected}\n                            onClick={(event) => {\n                                onCheckItem(arg.id, !arg.isSelected)\n                                event.stopPropagation();\n                                event.preventDefault();\n                            }}\n                            disabled={isUpdated}\n                        />}\n                        label={arg.display}\n                        sx={{\n                            paddingLeft: 1\n                        }}\n                    />\n                }\n            />\n        )\n    }\n\n    const renderCommand = (command: ArgSimilarCommand) => {\n        return (\n            <TreeItem key={command.id} nodeId={command.id} color='inherit'\n                label={\n                    <FormControlLabel\n                        control={<Checkbox size=\"small\"\n                            checked={command.selectedCount > 0 && command.selectedCount === command.total}\n                            indeterminate={command.selectedCount > 0 && command.selectedCount < command.total}\n                            onClick={(event) => {\n                                onCheckItem(command.id, !(command.selectedCount > 0 && command.selectedCount === command.total))\n                                event.stopPropagation();\n                                event.preventDefault();\n                            }}\n                        />}\n                        label={command.name}\n                        sx={{\n                            paddingLeft: 1\n                        }}\n                    />\n                }\n            >\n                {Array.isArray(command.args) ? command.args.map((arg) => renderArg(arg)) : null}\n            </TreeItem>\n        )\n    }\n\n    const renderGroup = (group: ArgSimilarGroup) => {\n        return (\n            <TreeItem key={group.id} nodeId={group.id} color='inherit'\n                label={\n                    <FormControlLabel\n                        control={<Checkbox size=\"small\"\n                            checked={group.selectedCount > 0 && group.selectedCount === group.total}\n                            indeterminate={group.selectedCount > 0 && group.selectedCount < group.total}\n                            onClick={(event) => {\n                                onCheckItem(group.id, !(group.selectedCount > 0 && group.selectedCount === group.total))\n                                event.stopPropagation();\n                                event.preventDefault();\n                            }}\n                        />}\n                        label={group.name}\n                        sx={{\n                            paddingLeft: 1\n                        }}\n                    />\n                }\n            >\n                {Array.isArray(group.commands) ? group.commands.map((command) => renderCommand(command)) : null}\n                {Array.isArray(group.groups) ? group.groups.map((subGroup) => renderGroup(subGroup)) : null}\n            </TreeItem>\n        )\n    }\n\n    return (<>\n        <TreeView\n            sx={{\n                flexGrow: 1,\n                overflowY: 'auto',\n            }}\n            defaultCollapseIcon={<ExpandMoreIcon />}\n            defaultExpandIcon={<ChevronRightIcon />}\n            onNodeToggle={onNodeToggle}\n            selected={[]}\n            expanded={props.expandedIds}\n        >\n            {renderGroup(props.tree.root)}\n        </TreeView>\n    </>)\n}\n\nexport default WSECArgumentSimilarPicker;\nexport { BuildArgSimilarTree };\nexport type { ArgSimilarTree, ArgSimilarGroup, ArgSimilarCommand, ArgSimilarArg }",
         "import { Alert, Box, Button, Checkbox, ButtonBase, CardContent, Dialog, DialogActions, DialogContent, DialogTitle, FormControlLabel, InputLabel, LinearProgress, Radio, RadioGroup, Switch, TextField, Typography, TypographyProps } from '@mui/material';\nimport { styled } from '@mui/system';\nimport axios from 'axios';\nimport React, { useState, useEffect } from 'react';\nimport { CardTitleTypography, ExperimentalTypography, LongHelpTypography, PreviewTypography, ShortHelpPlaceHolderTypography, ShortHelpTypography, SmallExperimentalTypography, SmallPreviewTypography, StableTypography, SubtitleTypography } from './WSEditorTheme';\nimport ArrowBackIosIcon from '@mui/icons-material/ArrowBackIos';\nimport EditIcon from '@mui/icons-material/Edit';\nimport ImportExportIcon from '@mui/icons-material/ImportExport';\nimport CallSplitSharpIcon from '@mui/icons-material/CallSplitSharp';\nimport AddIcon from '@mui/icons-material/Add';\nimport WSECArgumentSimilarPicker, { ArgSimilarTree, BuildArgSimilarTree } from './argument/WSECArgumentSimilarPicker';\nimport pluralize from 'pluralize';\n\n\nfunction WSEditorCommandArgumentsContent(props: {\n    commandUrl: string,\n    args: CMDArg[],\n    clsArgDefineMap: ClsArgDefinitionMap,\n    onReloadArgs: () => Promise<void>,\n    onAddSubCommand: (argVar: string, subArgOptions: { var: string, options: string }[], argStackNames: string[]) => void,\n}) {\n\n    const [displayArgumentDialog, setDisplayArgumentDialog] = useState<boolean>(false);\n    const [editArg, setEditArg] = useState<CMDArg | undefined>(undefined);\n    const [editArgIdxStack, setEditArgIdxStack] = useState<ArgIdx[] | undefined>(undefined);\n    const [displayFlattenDialog, setDisplayFlattenDialog] = useState<boolean>(false);\n    const [displayUnwrapClsDialog, setDisplayUnwrapClsDialog] = useState<boolean>(false);\n\n    const handleArgumentDialogClose = async (updated: boolean) => {\n        if (updated) {\n            props.onReloadArgs();\n        }\n        setDisplayArgumentDialog(false);\n        setEditArg(undefined);\n        setEditArgIdxStack(undefined);\n    }\n\n    const handleEditArgument = (arg: CMDArg, argIdxStack: ArgIdx[]) => {\n        setEditArg(arg)\n        setEditArgIdxStack(argIdxStack)\n        setDisplayArgumentDialog(true)\n    }\n\n    const handleFlattenDialogClose = async (flattened: boolean) => {\n        if (flattened) {\n            props.onReloadArgs()\n        }\n        setDisplayFlattenDialog(false);\n        setEditArg(undefined);\n        setEditArgIdxStack(undefined);\n    }\n\n    const handleArgumentFlatten = (arg: CMDArg, argIdxStack: ArgIdx[]) => {\n        setEditArg(arg)\n        setEditArgIdxStack(argIdxStack)\n        setDisplayFlattenDialog(true)\n    }\n\n    const handleUnwrapClsDialogClose = async (unwrapped: boolean) => {\n        if (unwrapped) {\n            props.onReloadArgs();\n        }\n        setDisplayUnwrapClsDialog(false);\n        setEditArg(undefined);\n        setEditArgIdxStack(undefined);\n    }\n\n    const handleUnwrapClsArgument = (arg: CMDArg, argIdxStack: ArgIdx[]) => {\n        setEditArg(arg)\n        setEditArgIdxStack(argIdxStack)\n        setDisplayUnwrapClsDialog(true)\n    }\n\n    const handleAddSubcommand = (arg: CMDArg, argIdxStack: ArgIdx[]) => {\n        const argVar = arg.var;\n        let argStackNames = argIdxStack.map(argIdx => {\n            let name = argIdx.displayKey;\n            while (name.startsWith('-')) {\n                name = name.slice(1)\n            }\n            if (name.endsWith('[]') || name.endsWith('{}')) {\n                name = name.slice(0, name.length - 2)\n                name = pluralize.singular(name)\n            }\n            return name\n        });\n        let a: CMDArgBase | undefined = arg;\n        if (a.type.startsWith('@')) {\n            let clsName = (a as CMDClsArg).clsName;\n            a = props.clsArgDefineMap[clsName];\n        }\n        if (a.type.startsWith(\"dict<\")) {\n            a = (a as CMDDictArgBase).item;\n        } else if (a.type.startsWith(\"array<\")) {\n            a = (a as CMDArrayArgBase).item;\n        }\n        let subArgOptions: { var: string, options: string }[] = []\n        if (a !== undefined) {\n            let subArgs;\n            if (a.type.startsWith('@')) {\n                let clsName = (a as CMDClsArg).clsName;\n                subArgs = (props.clsArgDefineMap[clsName] as CMDObjectArgBase).args\n            } else {\n                subArgs = (a as CMDObjectArg).args\n            }\n            subArgOptions = subArgs.map(value => {\n                return {\n                    var: value.var,\n                    options: value.options.join(\" \"),\n                };\n            });\n        }\n\n        props.onAddSubCommand(argVar, subArgOptions, argStackNames);\n    }\n\n    return (\n        <React.Fragment>\n            <CardContent sx={{\n                flex: '1 0 auto',\n                display: 'flex',\n                flexDirection: 'column',\n                alignItems: 'stretch',\n            }}>\n                <Box sx={{\n                    mb: 2,\n                    display: 'flex',\n                    flexDirection: 'row',\n                    alignItems: \"center\"\n                }}>\n                    <CardTitleTypography sx={{ flexShrink: 0 }}>\n                        [ ARGUMENT ]\n                    </CardTitleTypography>\n                </Box>\n                <ArgumentNavigation commandUrl={props.commandUrl} args={props.args} clsArgDefineMap={props.clsArgDefineMap} onEdit={handleEditArgument} onFlatten={handleArgumentFlatten} onUnwrap={handleUnwrapClsArgument} onAddSubcommand={handleAddSubcommand} />\n            </CardContent>\n\n            {displayArgumentDialog && <ArgumentDialog commandUrl={props.commandUrl} arg={editArg!} clsArgDefineMap={props.clsArgDefineMap} open={displayArgumentDialog} onClose={handleArgumentDialogClose} />}\n            {displayFlattenDialog && <FlattenDialog commandUrl={props.commandUrl} arg={editArg!} clsArgDefineMap={props.clsArgDefineMap} open={displayFlattenDialog} onClose={handleFlattenDialogClose} />}\n            {displayUnwrapClsDialog && <UnwrapClsDialog commandUrl={props.commandUrl} arg={editArg!} open={displayUnwrapClsDialog} onClose={handleUnwrapClsDialogClose} />}\n        </React.Fragment>\n    )\n}\n\n\ninterface ArgIdx {\n    var: string,\n    displayKey: string,\n}\n\nfunction ArgumentNavigation(props: {\n    commandUrl: string,\n    args: CMDArg[],\n    clsArgDefineMap: ClsArgDefinitionMap,\n    onEdit: (arg: CMDArg, argIdxStack: ArgIdx[]) => void,\n    onFlatten: (arg: CMDArg, argIdxStack: ArgIdx[]) => void,\n    onUnwrap: (arg: CMDArg, argIdxStack: ArgIdx[]) => void,\n    onAddSubcommand: (arg: CMDArg, argIdxStack: ArgIdx[]) => void,\n}) {\n    const [argIdxStack, setArgIdxStack] = useState<ArgIdx[]>([]);\n\n    const getArgProps = (selectedArgBase: CMDArgBase): { title: string, props: CMDArg[], flattenArgVar: string | undefined } | undefined => {\n        if (selectedArgBase.type.startsWith('@')) {\n            let clsArgDefine = props.clsArgDefineMap[(selectedArgBase as CMDClsArgBase).clsName];\n            let clsArgProps = getArgProps(clsArgDefine);\n            if (clsArgProps !== undefined && clsArgDefine.type === \"object\") {\n                clsArgProps!.flattenArgVar = (selectedArgBase as CMDClsArg).var\n            }\n            return clsArgProps;\n        }\n        if (selectedArgBase.type === \"object\") {\n            return {\n                title: \"Props\",\n                props: (selectedArgBase as CMDObjectArgBase).args,\n                flattenArgVar: (selectedArgBase as CMDObjectArg).var,\n            }\n        } else if (selectedArgBase.type.startsWith(\"dict<\")) {\n            let item = (selectedArgBase as CMDDictArgBase).item\n            const itemProps = item ? getArgProps(item) : undefined;\n            if (!itemProps) {\n                return undefined;\n            }\n            return {\n                title: \"Dict Element Props\",\n                props: itemProps.props,\n                flattenArgVar: undefined,\n            }\n        } else if (selectedArgBase.type.startsWith(\"array<\")) {\n            const itemProps = getArgProps((selectedArgBase as CMDArrayArgBase).item);\n            if (!itemProps) {\n                return undefined;\n            }\n            return {\n                title: \"Array Element Props\",\n                props: itemProps.props,\n                flattenArgVar: undefined,\n            }\n        } else {\n            return undefined;\n        }\n    }\n\n    const getSelectedArg = (stack: ArgIdx[]): CMDArg | undefined => {\n        if (stack.length === 0) {\n            return undefined;\n        } else {\n            let args: CMDArg[] = [...props.args]\n            let selectedArg: CMDArg | undefined = undefined;\n            for (const i in stack) {\n                const argVar = stack[i].var;\n                selectedArg = args.find(arg => arg.var === argVar)\n                if (!selectedArg) {\n                    break\n                }\n                args = getArgProps(selectedArg)?.props ?? [];\n            }\n            return selectedArg\n        }\n    }\n\n    useEffect(() => {\n        setArgIdxStack([]);\n    }, [props.commandUrl]);\n\n    useEffect(() => {\n        // update argument idx stack \n        const stack = [...argIdxStack];\n        while (stack.length > 0 && !getSelectedArg(stack)) {\n            stack.pop()\n        }\n        setArgIdxStack(stack);\n    }, [props.args, props.clsArgDefineMap])\n\n    const handleSelectSubArg = (subArgVar: string) => {\n        let subArg\n        if (argIdxStack.length > 0) {\n            const arg = getSelectedArg(argIdxStack);\n            if (!arg) {\n                return\n            }\n            subArg = getArgProps(arg)?.props.find(a => a.var === subArgVar)\n        } else {\n            subArg = props.args.find(a => a.var === subArgVar)\n        }\n\n        if (!subArg) {\n            return\n        }\n        const argIdx: ArgIdx = {\n            var: subArg.var,\n            displayKey: subArg.options[0],\n        }\n        if (argIdxStack.length === 0) {\n            if (argIdx.displayKey.length === 1) {\n                argIdx.displayKey = `-${argIdx.displayKey}`\n            } else {\n                argIdx.displayKey = `--${argIdx.displayKey}`\n            }\n        }\n\n        let argType = subArg.type;\n        if (argType.startsWith(\"@\")) {\n            argType = props.clsArgDefineMap[(subArg as CMDClsArg).clsName].type\n        }\n        if (argType.startsWith(\"dict<\")) {\n            argIdx.displayKey += \"{}\"\n        } else if (argType.startsWith(\"array<\")) {\n            argIdx.displayKey += \"[]\"\n        }\n\n        setArgIdxStack([...argIdxStack, argIdx]);\n    }\n\n    const handleChangeArgIdStack = (end: number) => {\n        setArgIdxStack(argIdxStack.slice(0, end));\n    }\n\n    const buildArgumentReviewer = () => {\n        const selectedArg = getSelectedArg(argIdxStack)\n        if (!selectedArg) {\n            return (<></>)\n        }\n\n        const stage = selectedArg.stage\n\n        return (\n            <React.Fragment>\n                <Box sx={{\n                    display: \"flex\",\n                    flexDirection: \"row\",\n                    alignItems: \"flex-start\",\n                    justifyContent: \"flex-start\"\n                }}>\n                    <ArgNavBar argIdxStack={argIdxStack} onChangeArgIdStack={handleChangeArgIdStack} />\n                    {stage === \"Stable\" && <StableTypography\n                        sx={{ flexShrink: 0 }}\n                    >\n                        {stage}\n                    </StableTypography>}\n                    {stage === \"Preview\" && <PreviewTypography\n                        sx={{ flexShrink: 0 }}\n                    >\n                        {stage}\n                    </PreviewTypography>}\n                    {stage === \"Experimental\" && <ExperimentalTypography\n                        sx={{ flexShrink: 0 }}\n                    >\n                        {stage}\n                    </ExperimentalTypography>}\n                </Box>\n                <ArgumentReviewer\n                    arg={selectedArg}\n                    depth={argIdxStack.length}\n                    onEdit={() => { props.onEdit(selectedArg, argIdxStack) }}\n                    onUnwrap={() => { props.onUnwrap(selectedArg, argIdxStack) }}\n                />\n            </React.Fragment>\n        )\n    }\n\n    const buildArgumentPropsReviewer = () => {\n        if (argIdxStack.length === 0) {\n            if (props.args.length === 0) {\n                return (<></>)\n            }\n            return (<ArgumentPropsReviewer\n                title={\"Argument Groups\"}\n                args={props.args}\n                onFlatten={undefined}\n                onAddSubcommand={undefined}\n                depth={argIdxStack.length}\n                onSelectSubArg={handleSelectSubArg}\n            />)\n        } else {\n            const selectedArg = getSelectedArg(argIdxStack)\n            if (!selectedArg) {\n                return (<></>)\n            }\n            const argProps = getArgProps(selectedArg)\n            if (!argProps) {\n                return (<></>)\n            }\n            const canFlatten = argProps.flattenArgVar !== undefined\n            return (<ArgumentPropsReviewer\n                title={argProps.title}\n                args={argProps.props}\n                depth={argIdxStack.length}\n                selectedArg={selectedArg!}\n                onFlatten={canFlatten ? () => {\n                    props.onFlatten(selectedArg!, argIdxStack)\n                } : undefined}\n                onAddSubcommand={() => { props.onAddSubcommand(selectedArg!, argIdxStack) }}\n                onSelectSubArg={handleSelectSubArg}\n            />)\n        }\n    }\n\n    return (<React.Fragment>\n        {argIdxStack.length > 0 && <React.Fragment>\n            {buildArgumentReviewer()}\n        </React.Fragment>}\n        <React.Fragment>\n            {buildArgumentPropsReviewer()}\n        </React.Fragment>\n    </React.Fragment>)\n}\n\n\nconst NavBarItemTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 14,\n    fontWeight: 400,\n}))\n\nconst NavBarItemHightLightedTypography = styled(NavBarItemTypography)<TypographyProps>(({ theme }) => ({\n    color: '#5d64cf',\n}))\n\nfunction ArgNavBar(props: {\n    argIdxStack: ArgIdx[],\n    onChangeArgIdStack: (end: number) => void,\n}) {\n\n    return (\n        <React.Fragment>\n            <Box\n                sx={{\n                    flexGrow: 1,\n                    display: \"flex\",\n                    flexDirection: \"row\",\n                    alignItems: \"center\",\n                    justifyContent: \"flex-start\",\n                    mt: 1, mb: 0.5, mr: 2,\n                }}>\n                <ButtonBase key=\"Back\" onClick={() => {\n                    props.onChangeArgIdStack(0)\n                }}>\n                    <ArrowBackIosIcon sx={{ fontSize: 14 }} />\n                </ButtonBase>\n                {props.argIdxStack.slice(0, -1).map((argIdx, index) => (\n                    <ButtonBase\n                        key={`${index}`}\n                        onClick={() => {\n                            props.onChangeArgIdStack(index + 1)\n                        }}\n                    >\n                        <NavBarItemTypography sx={{ flexShrink: 0 }} >{index > 0 ? `.${argIdx.displayKey}` : argIdx.displayKey}</NavBarItemTypography>\n                    </ButtonBase>\n                ))}\n                <ButtonBase\n                    key={`${props.argIdxStack.length - 1}`}\n                    onClick={() => {\n                        props.onChangeArgIdStack(props.argIdxStack.length)\n                    }}\n                >\n                    <NavBarItemHightLightedTypography sx={{ flexShrink: 0 }} >{props.argIdxStack.length > 1 ? `.${props.argIdxStack[props.argIdxStack.length - 1].displayKey}` : props.argIdxStack[props.argIdxStack.length - 1].displayKey}</NavBarItemHightLightedTypography>\n                </ButtonBase>\n            </Box>\n        </React.Fragment>\n    )\n}\n\nconst spliceArgOptionsString = (arg: CMDArg, depth: number) => {\n    let optionsString = arg.options.map((option) => {\n        if (depth === 0) {\n            if (option.length === 1) {\n                return '-' + option;\n            } else {\n                return '--' + option;\n            }\n        } else {\n            return '.' + option;\n        }\n    }).join(\" \");\n\n    if ((arg as CMDArrayArg).singularOptions) {\n        let singularOptionString = (arg as CMDArrayArg).singularOptions!.map((option) => {\n            if (depth === 0) {\n                if (option.length === 1) {\n                    return '-' + option;\n                } else {\n                    return '--' + option;\n                }\n            } else {\n                return '.' + option;\n            }\n        }).join(\" \");\n        optionsString += ` (${singularOptionString})`;\n    } else if ((arg as CMDClsArg).singularOptions) {\n        let singularOptionString = (arg as CMDArrayArg).singularOptions!.map((option) => {\n            if (depth === 0) {\n                if (option.length === 1) {\n                    return '-' + option;\n                } else {\n                    return '--' + option;\n                }\n            } else {\n                return '.' + option;\n            }\n        }).join(\" \");\n        optionsString += ` (${singularOptionString})`;\n    }\n\n    return optionsString;\n}\n\n\nconst ArgNameTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 26,\n    fontWeight: 700,\n}))\n\nconst ArgTypeTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 16,\n    fontWeight: 700,\n}))\n\nconst ArgRequiredTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: '#fad105',\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 16,\n    fontWeight: 200,\n}))\n\nconst ArgEditTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: \"#5d64cf\",\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 14,\n    fontWeight: 400,\n}));\n\nconst ArgChoicesTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 14,\n    fontWeight: 700,\n}))\n\nfunction ArgumentReviewer(props: {\n    arg: CMDArg,\n    depth: number,\n    onEdit: () => void,\n    onUnwrap: () => void,\n}) {\n    const [choices, setChoices] = useState<string[]>([]);\n\n    const buildArgOptionsString = () => {\n        const argOptionsString = spliceArgOptionsString(props.arg, props.depth - 1);\n        return (<ArgNameTypography>{argOptionsString}</ArgNameTypography>)\n    }\n\n    useEffect(() => {\n        const newChoices: string[] = [];\n        if ((props.arg as CMDStringArg).enum) {\n            const items = (props.arg as CMDStringArg).enum!.items;\n            for (const idx in items) {\n                const enumItem = items[idx];\n                newChoices.push(enumItem.name);\n            }\n        } else if ((props.arg as CMDNumberArg).enum) {\n            const items = (props.arg as CMDNumberArg).enum!.items;\n            for (const idx in items) {\n                const enumItem = items[idx];\n                newChoices.push(enumItem.name);\n            }\n        }\n        setChoices(newChoices);\n    }, [props.arg]);\n\n    const getUnwrapKeywords = () => {\n        if (props.arg.type.startsWith(\"@\")) {\n            return \"Unwrap\"\n        } else if (props.arg.type.startsWith(\"array\")) {\n            if ((props.arg as CMDArrayArg).item?.type.startsWith(\"@\")) {\n                return \"Unwrap Element\"\n            }\n        } else if (props.arg.type.startsWith(\"dict\")) {\n            if ((props.arg as CMDDictArg).item?.type.startsWith(\"@\")) {\n                return \"Unwrap Element\"\n            }\n        }\n        return null;\n    }\n\n    const getDefaultValueToString = () => {\n        if (props.arg.type === \"object\" || props.arg.type.startsWith(\"dict<\") || props.arg.type.startsWith(\"array<\") || props.arg.type.startsWith(\"@\")) {\n            if (props.arg.default !== undefined && props.arg.default !== null) {\n                return JSON.stringify(props.arg.default.value);\n            }\n        } else {\n            if (props.arg.default !== undefined && props.arg.default !== null) {\n                return props.arg.default.value.toString();\n            }\n        }\n        return \"\"\n    }\n\n    return (<React.Fragment>\n        <Box\n            sx={{\n                display: \"flex\",\n                flexDirection: \"column\",\n                alignItems: \"stretch\",\n                justifyContent: \"flex-start\",\n                mt: 1,\n                mb: 2\n            }}>\n            <Box sx={{\n                flexGrow: 1,\n                display: \"flex\",\n                flexDirection: \"row\",\n                alignItems: \"center\",\n            }}>\n                {buildArgOptionsString()}\n                <Button sx={{ flexShrink: 0, ml: 3 }}\n                    startIcon={<EditIcon color=\"secondary\" fontSize='small' />}\n                    onClick={() => { props.onEdit() }}\n                >\n                    <ArgEditTypography>Edit</ArgEditTypography>\n                </Button>\n            </Box>\n\n            <Box sx={{\n                display: \"flex\",\n                flexDirection: \"row\",\n                justifyContent: \"flex-start\",\n                alignItems: \"stretch\",\n                ml: 6,\n            }}>\n                <Box sx={{\n                    display: \"flex\",\n                    flexDirection: \"row\",\n                    justifyContent: \"flex-start\",\n                    alignItems: \"center\"\n                }}>\n                    <ArgTypeTypography>{`/${props.arg.type}/`}</ArgTypeTypography>\n                </Box>\n                {getUnwrapKeywords() !== null && <Button sx={{ flexShrink: 0, ml: 1 }}\n                    startIcon={<ImportExportIcon color=\"secondary\" fontSize='small' />}\n                    onClick={() => { props.onUnwrap() }}\n                >\n                    <ArgEditTypography>{getUnwrapKeywords()!}</ArgEditTypography>\n                </Button>}\n                <Box sx={{ flexGrow: 1 }} />\n                {props.arg.required && <ArgRequiredTypography>[Required]</ArgRequiredTypography>}\n            </Box>\n            {(props.arg.default !== undefined || choices.length > 0 || props.arg.configurationKey !== undefined) && <Box\n                sx={{\n                    ml: 5,\n                    mt: 0.5,\n                    display: \"flex\",\n                    flexDirection: \"row\",\n                    alignItems: \"center\",\n                }}>\n                {choices.length > 0 && <ArgChoicesTypography sx={{ ml: 1 }}>\n                    {`Choices: ` + choices.join(', ')}\n                </ArgChoicesTypography>}\n                {props.arg.default !== undefined && <ArgChoicesTypography sx={{ ml: 1 }}>\n                    {`Default: ${getDefaultValueToString()}`}\n                </ArgChoicesTypography>\n                }\n                {props.arg.configurationKey !== undefined && <ArgChoicesTypography sx={{ ml: 1 }}>\n                    {`ConfigurationKey: ${props.arg.configurationKey}`}\n                </ArgChoicesTypography>\n                }\n            </Box>}\n            {props.arg.help?.short && <ShortHelpTypography sx={{ ml: 6, mt: 1.5 }}> {props.arg.help?.short} </ShortHelpTypography>}\n            {!(props.arg.help?.short) && <ShortHelpPlaceHolderTypography sx={{ ml: 6, mt: 2 }}>Please add argument short summary!</ShortHelpPlaceHolderTypography>}\n            {props.arg.help?.lines && <Box sx={{ ml: 6, mt: 1, mb: 1 }}>\n                {props.arg.help.lines.map((line, idx) => (<LongHelpTypography key={idx}>{line}</LongHelpTypography>))}\n            </Box>}\n        </Box>\n    </React.Fragment>)\n}\n\nfunction ArgumentDialog(props: {\n    commandUrl: string,\n    arg: CMDArg,\n    clsArgDefineMap: ClsArgDefinitionMap,\n    open: boolean,\n    onClose: (updated: boolean) => Promise<void>,\n}) {\n    const [updating, setUpdating] = useState<boolean>(false);\n    const [stage, setStage] = useState<string>(\"\");\n    const [invalidText, setInvalidText] = useState<string | undefined>(undefined);\n    const [options, setOptions] = useState<string>(\"\");\n    const [singularOptions, setSingularOptions] = useState<string | undefined>(undefined);\n    const [group, setGroup] = useState<string>(\"\")\n    const [hide, setHide] = useState<boolean>(false);\n    const [shortHelp, setShortHelp] = useState<string>(\"\");\n    const [longHelp, setLongHelp] = useState<string>(\"\");\n    const [argSimilarTree, setArgSimilarTree] = useState<ArgSimilarTree | undefined>(undefined);\n    const [argSimilarTreeExpandedIds, setArgSimilarTreeExpandedIds] = useState<string[]>([]);\n    const [argSimilarTreeArgIdsUpdated, setArgSimilarTreeArgIdsUpdated] = useState<string[]>([]);\n    const [hasDefault, setHasDefault] = useState<boolean | undefined>(false);\n    const [defaultValue, setDefaultValue] = useState<any | undefined>(undefined);\n    const [defaultValueInJson, setDefaultValueInJson] = useState<boolean>(false);\n    const [hasPrompt, setHasPrompt] = useState<boolean | undefined>(false);\n    const [promptMsg, setPromptMsg] = useState<string | undefined>(undefined);\n    const [promptConfirm, setPromptConfirm] = useState<boolean | undefined>(undefined);\n    const [configurationKey, setConfigurationKey] = useState<string>(\"\");\n    const [isClientArg, setIsClientArg] = useState<boolean>(false);\n\n    const handleClose = () => {\n        setInvalidText(undefined);\n        props.onClose(false);\n    }\n\n    const verifyModification = () => {\n        setInvalidText(undefined);\n        let name = options.trim();\n        let sName = singularOptions?.trim() ?? undefined;\n        let sHelp = shortHelp.trim();\n        let lHelp = longHelp.trim();\n        let gName = group.trim();\n        let cfgKey = configurationKey.trim();\n\n        const names = name.split(' ').filter(n => n.length > 0);\n        const sNames = sName?.split(' ').filter(n => n.length > 0) ?? undefined;\n\n        if (names.length < 1) {\n            setInvalidText(`Argument 'Option names' is required.`)\n            return undefined\n        }\n\n        for (const idx in names) {\n            const piece = names[idx];\n            if (!/^[a-z0-9]+(-[a-z0-9]+)*$/.test(piece)) {\n                setInvalidText(`Invalid 'Option name': '${piece}'. Supported regular expression is: [a-z0-9]+(-[a-z0-9]+)* `)\n                return undefined\n            }\n        }\n\n        if (sNames) {\n            for (const idx in sNames) {\n                const piece = sNames[idx];\n                if (!/^[a-z0-9]+(-[a-z0-9]+)*$/.test(piece)) {\n                    setInvalidText(`Invalid 'Singular option name': '${piece}'. Supported regular expression is: [a-z0-9]+(-[a-z0-9]+)* `)\n                    return undefined\n                }\n            }\n        }\n\n        if (sHelp.length < 1 && names.find((n) => { return n === \"subscription\" || n === \"resource-group\" }) === undefined) {\n            setInvalidText(`Field 'Short Summary' is required.`)\n            return undefined\n        }\n\n        let lines: string[] | null = null;\n        if (lHelp.length > 1) {\n            lines = lHelp.split('\\n').filter(l => l.length > 0);\n        }\n\n        let argCfgKey: string | null = null;\n        if (cfgKey.length > 0) {\n            argCfgKey = cfgKey;\n        }\n\n        let argDefault = undefined;\n        if (hasDefault === false) {\n            if (props.arg.default !== undefined) {\n                argDefault = null;\n            }\n        } else if (hasDefault === true) {\n            if (defaultValue === undefined) {\n                setInvalidText(`Field 'Default Value' is undefined.`)\n                return undefined;\n            } else {\n                try {\n                    let argType = props.arg.type;\n                    if (argType.startsWith(\"@\")) {\n                        argType = props.clsArgDefineMap[(props.arg as CMDClsArg).clsName].type\n                    }\n                    argDefault = {\n                        value: convertArgDefaultText(defaultValue!, argType),\n                    }\n                } catch (err: any) {\n                    setInvalidText(`Field 'Default Value' is invalid: ${err.message}.`)\n                    return undefined;\n                }\n                if (props.arg.default !== undefined && props.arg.default.value === argDefault.value) {\n                    argDefault = undefined;\n                }\n            }\n        }\n\n        let argPrompt = undefined;\n        if (hasPrompt === false) {\n            if (props.arg.prompt !== undefined) {\n                argPrompt = null;\n            }\n        } else if (hasPrompt === true) {\n            if (promptMsg === undefined) {\n                setInvalidText(`Field 'Prompt Message' is undefined.`)\n                return undefined;\n            } else {\n                let msg = promptMsg.trim();\n                if (msg.length < 1) {\n                    setInvalidText(`Field 'Prompt Message' is empty.`)\n                    return undefined;\n                }\n                if (!msg.endsWith(':')) {\n                    setInvalidText(`Field 'Prompt Message' must end with a colon.`)\n                    return undefined;\n                }\n                argPrompt = {\n                    msg: msg,\n                    confirm: promptConfirm,\n                }\n            }\n        }\n\n        return {\n            options: names,\n            singularOptions: sNames,\n            stage: stage,\n            group: gName,\n            hide: hide,\n            help: {\n                short: sHelp,\n                lines: lines\n            },\n            default: argDefault,\n            prompt: argPrompt,\n            configurationKey: argCfgKey,\n        }\n    }\n\n    const handleModify = async (event: any) => {\n        const data = verifyModification();\n        if (data === undefined) {\n            return;\n        }\n\n        setUpdating(true);\n\n        const argumentUrl = `${props.commandUrl}/Arguments/${props.arg.var}`\n\n        try {\n            let res = await axios.patch(argumentUrl, {\n                ...data,\n            });\n            let newArg = decodeArg(res.data).arg;\n            setUpdating(false);\n            await props.onClose(true);\n        } catch (err: any) {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                setInvalidText(\n                    `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`\n                );\n            }\n            setUpdating(false);\n        }\n    }\n\n    const handleDisplaySimilar = () => {\n        if (verifyModification() === undefined) {\n            return;\n        }\n\n        setUpdating(true);\n\n        const similarUrl = `${props.commandUrl}/Arguments/${props.arg.var}/FindSimilar`\n        axios.post(similarUrl).then(res => {\n            setUpdating(false);\n            const { tree, expandedIds } = BuildArgSimilarTree(res);\n            setArgSimilarTree(tree);\n            setArgSimilarTreeExpandedIds(expandedIds);\n            setArgSimilarTreeArgIdsUpdated([]);\n        }).catch(err => {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                setInvalidText(\n                    `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`\n                );\n            }\n            setUpdating(false);\n        });\n    }\n\n    const handleDisableSimilar = () => {\n        setArgSimilarTree(undefined);\n        setArgSimilarTreeExpandedIds([]);\n    }\n\n    const onSimilarTreeUpdated = (newTree: ArgSimilarTree) => {\n        setArgSimilarTree(newTree);\n    }\n\n    const onSimilarTreeExpandedIdsUpdated = (expandedIds: string[]) => {\n        setArgSimilarTreeExpandedIds(expandedIds);\n    }\n\n    const handleModifySimilar = async () => {\n        const data = verifyModification();\n        if (data === undefined) {\n            return;\n        }\n\n        setUpdating(true);\n        let invalidText = \"\";\n        const updatedIds: string[] = [...argSimilarTreeArgIdsUpdated]\n        for (const idx in argSimilarTree!.selectedArgIds) {\n            const argId = argSimilarTree!.selectedArgIds[idx];\n            if (updatedIds.indexOf(argId) === -1) {\n                try {\n                    await axios.patch(argId, {\n                        ...data\n                    })\n                    updatedIds.push(argId);\n                    setArgSimilarTreeArgIdsUpdated([...updatedIds]);\n                } catch (err: any) {\n                    console.error(err.response);\n                    if (err.response?.data?.message) {\n                        const data = err.response!.data!;\n                        invalidText += `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`\n                    }\n                }\n            }\n        }\n\n        if (invalidText.length > 0) {\n            setInvalidText(invalidText);\n            setUpdating(false);\n        } else {\n            setUpdating(false);\n            await props.onClose(true);\n        }\n    }\n\n    useEffect(() => {\n        let { arg, clsArgDefineMap } = props;\n        setIsClientArg(arg.var.startsWith('$Client.'));\n\n        setOptions(arg.options.join(\" \"));\n        if (arg.type.startsWith(\"array\")) {\n            setSingularOptions((arg as CMDArrayArg).singularOptions?.join(\" \") ?? \"\")\n        } else if (arg.type.startsWith('@') && clsArgDefineMap[(arg as CMDClsArg).clsName].type.startsWith(\"array\")) {\n            setSingularOptions((arg as CMDClsArg).singularOptions?.join(\" \") ?? \"\")\n        } else {\n            setSingularOptions(undefined);\n        }\n\n        if (arg.type === \"object\" || arg.type.startsWith(\"dict<\") || arg.type.startsWith(\"array<\") || arg.type.startsWith(\"@\")) {\n            setHasPrompt(undefined);\n        } else {\n            setHasPrompt(arg.prompt !== undefined);\n            if (arg.prompt !== undefined) {\n                setPromptMsg(arg.prompt.msg);\n                setPromptConfirm(undefined);\n            }\n        }\n        if (arg.type === \"password\") {\n            setPromptConfirm((arg as CMDPasswordArg).prompt?.confirm ?? false);\n        }\n        setStage(props.arg.stage);\n        setGroup(props.arg.group);\n        setHide(props.arg.hide);\n        setShortHelp(props.arg.help?.short ?? \"\");\n        setLongHelp(props.arg.help?.lines?.join(\"\\n\") ?? \"\");\n        setConfigurationKey(props.arg.configurationKey ?? \"\");\n        setUpdating(false);\n        setArgSimilarTree(undefined);\n        setArgSimilarTreeExpandedIds([]);\n\n        if (arg.type === \"object\" || arg.type.startsWith(\"dict<\") || arg.type.startsWith(\"array<\") || arg.type.startsWith(\"@\")) {\n            setDefaultValueInJson(true);\n            if (props.arg.default !== undefined && props.arg.default !== null) {\n                setHasDefault(true);\n                setDefaultValue(JSON.stringify(props.arg.default.value));\n            } else {\n                setHasDefault(false);\n                setDefaultValue(undefined);\n            }\n        } else {\n            setDefaultValueInJson(false);\n            if (props.arg.default !== undefined && props.arg.default !== null) {\n                setHasDefault(true);\n                setDefaultValue(props.arg.default.value.toString());\n            } else {\n                setHasDefault(false);\n                setDefaultValue(undefined);\n            }\n        }\n    }, [props.arg]);\n\n    return (\n        <Dialog\n            disableEscapeKeyDown\n            open={props.open}\n            sx={{ '& .MuiDialog-paper': { width: '80%' } }}\n        >\n            {!argSimilarTree && <>\n                <DialogTitle>{isClientArg ? \"Modify Client Argument\" : \"Modify Argument\"}</DialogTitle>\n                <DialogContent dividers={true}>\n                    {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n                    <TextField\n                        id=\"options\"\n                        label=\"Option names\"\n                        helperText=\"You can input multiple names separated by a space character\"\n                        type=\"text\"\n                        fullWidth\n                        variant='standard'\n                        value={options}\n                        onChange={(event: any) => {\n                            setOptions(event.target.value)\n                        }}\n                        margin=\"normal\"\n                        required\n                    />\n                    {singularOptions !== undefined && <TextField\n                        id=\"singularOptions\"\n                        label=\"Singular option names\"\n                        type=\"text\"\n                        fullWidth\n                        variant='standard'\n                        value={singularOptions}\n                        onChange={(event: any) => {\n                            setSingularOptions(event.target.value)\n                        }}\n                        margin=\"normal\"\n                    />}\n                    {!isClientArg && <><TextField\n                        id=\"group\"\n                        label=\"Argument Group\"\n                        type=\"text\"\n                        fullWidth\n                        variant='standard'\n                        value={group}\n                        onChange={(event: any) => {\n                            setGroup(event.target.value)\n                        }}\n                        margin=\"normal\"\n                    />\n                        <InputLabel required shrink sx={{ font: \"inherit\" }}>Stage</InputLabel>\n                        <RadioGroup\n                            row\n                            value={stage}\n                            name=\"stage\"\n                            onChange={(event: any) => {\n                                setStage(event.target.value);\n                            }}\n                        >\n                            <FormControlLabel value=\"Stable\" control={<Radio />} label=\"Stable\" sx={{ ml: 4 }} />\n                            <FormControlLabel value=\"Preview\" control={<Radio />} label=\"Preview\" sx={{ ml: 4 }} />\n                            <FormControlLabel value=\"Experimental\" control={<Radio />} label=\"Experimental\" sx={{ ml: 4 }} />\n                        </RadioGroup>\n\n                        {!props.arg.required && <>\n                            <InputLabel shrink sx={{ font: \"inherit\" }}>Hide Argument</InputLabel>\n                            <Switch sx={{ ml: 4 }}\n                                checked={hide}\n                                onChange={(event: any) => {\n                                    setHide(!hide);\n                                }}\n                            />\n                        </>}\n                    </>}\n                    {hasDefault !== undefined && <>\n                        <InputLabel shrink sx={{ font: \"inherit\" }}>Default Value</InputLabel>\n                        <Box sx={{\n                            display: \"flex\",\n                            flexDirection: \"row\",\n                            alignItems: \"center\",\n                            justifyContent: \"flex-start\",\n                            ml: 4,\n                        }}>\n                            <Switch\n                                checked={hasDefault}\n                                onChange={(event: any) => {\n                                    setHasDefault(!hasDefault);\n                                    setDefaultValue(undefined);\n                                }}\n                            />\n                            <TextField\n                                id=\"defaultValue\"\n                                label=\"default Value\"\n                                hiddenLabel\n                                type=\"text\"\n                                hidden={!hasDefault}\n                                fullWidth\n                                size=\"small\"\n                                value={defaultValue !== undefined ? defaultValue : \"\"}\n                                onChange={(event: any) => {\n                                    setDefaultValue(event.target.value);\n                                }}\n                                placeholder={defaultValueInJson ? \"Default Value in json format\" : \"Default Value\"}\n                                margin=\"normal\"\n                                aria-controls=''\n                                required\n                            />\n                        </Box>\n                    </>}\n\n                    {hasPrompt !== undefined && <>\n                        <InputLabel shrink sx={{ font: \"inherit\" }}>Prompt Input</InputLabel>\n                        <Box sx={{\n                            display: \"flex\",\n                            flexDirection: \"row\",\n                            alignItems: \"center\",\n                            justifyContent: \"flex-start\",\n                            ml: 4,\n                        }}>\n                            <Switch\n                                checked={hasPrompt}\n                                onChange={(event: any) => {\n                                    setHasPrompt(!hasPrompt);\n                                    setPromptMsg(undefined);\n                                }}\n                            />\n                            <Box sx={{\n                                display: \"flex\",\n                                flexDirection: \"column\",\n                                alignItems: \"stretch\",\n                                justifyContent: \"flex-start\",\n                                flexGrow: 1,\n                            }}>\n                                <TextField\n                                    id=\"SetPromptMsg\"\n                                    label=\"Prompt Message\"\n                                    hiddenLabel\n                                    type=\"text\"\n                                    hidden={!hasPrompt}\n                                    fullWidth\n                                    size=\"small\"\n                                    value={promptMsg !== undefined ? promptMsg : \"\"}\n                                    onChange={(event: any) => {\n                                        setPromptMsg(event.target.value);\n                                    }}\n                                    placeholder=\"Please input the prompt hint end with a colon.\"\n                                    margin=\"normal\"\n                                    aria-controls=''\n                                    required\n                                />\n                                {promptConfirm !== undefined && <>\n                                    <FormControlLabel control={\n                                        <Checkbox\n                                            size='small'\n                                            checked={promptConfirm}\n                                            onChange={(event: any) => {\n                                                setPromptConfirm(!promptConfirm);\n                                            }}\n                                        />\n                                    } label=\"Confirm input\" />\n                                </>}\n                            </Box>\n                        </Box>\n                    </>}\n                    {!isClientArg &&\n                        <TextField\n                            id=\"configurationKey\"\n                            label=\"Configuration Key\"\n                            helperText=\"The key to retrieve the default value from cli Configuration\"\n                            type='text'\n                            fullWidth\n                            variant='standard'\n                            value={configurationKey}\n                            onChange={(event: any) => {\n                                setConfigurationKey(event.target.value);\n                            }}\n                            margin=\"normal\"\n                        />}\n\n                    <TextField\n                        id=\"shortSummary\"\n                        label=\"Short Summary\"\n                        type=\"text\"\n                        fullWidth\n                        variant='standard'\n                        value={shortHelp}\n                        onChange={(event: any) => {\n                            setShortHelp(event.target.value);\n                        }}\n                        margin=\"normal\"\n                        required\n                    />\n                    <TextField\n                        id=\"longSummary\"\n                        label=\"Long Summary\"\n                        helperText=\"Please add long summer in lines.\"\n                        type=\"text\"\n                        fullWidth\n                        multiline\n                        variant='standard'\n                        value={longHelp}\n                        onChange={(event: any) => {\n                            setLongHelp(event.target.value);\n                        }}\n                        margin=\"normal\"\n                    />\n                </DialogContent>\n            </>}\n\n            {argSimilarTree && <>\n                <DialogTitle>Modify Similar Arguments</DialogTitle>\n                <DialogContent dividers={true}>\n                    {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n                    <WSECArgumentSimilarPicker tree={argSimilarTree} expandedIds={argSimilarTreeExpandedIds} updatedIds={argSimilarTreeArgIdsUpdated} onTreeUpdated={onSimilarTreeUpdated} onToggle={onSimilarTreeExpandedIdsUpdated} />\n                </DialogContent>\n            </>}\n            <DialogActions>\n                {updating &&\n                    <Box sx={{ width: '100%' }}>\n                        <LinearProgress color='secondary' />\n                    </Box>\n                }\n                {!updating && !argSimilarTree && <>\n                    <Button onClick={handleClose}>Cancel</Button>\n                    {/* cls argument should flatten similar. Customer should unwrap cls argument before to modify it*/}\n                    {!props.arg.var.startsWith(\"@\") && <Button onClick={handleModify}>{isClientArg ? \"Update Global\" : \"Update\"}</Button>}\n                    {/* TODO: support unwrap and update */}\n                    {!isClientArg && <Button onClick={handleDisplaySimilar}>Update Similar</Button>}\n                </>}\n                {!updating && argSimilarTree && <>\n                    <Button onClick={handleDisableSimilar}>Back</Button>\n                    <Button onClick={handleModifySimilar} disabled={argSimilarTree.selectedArgIds.length === 0}>Update</Button>\n                </>}\n            </DialogActions>\n        </Dialog>\n    )\n}\n\nfunction FlattenDialog(props: {\n    commandUrl: string,\n    arg: CMDArg,\n    clsArgDefineMap: ClsArgDefinitionMap,\n    open: boolean,\n    onClose: (flattened: boolean) => Promise<void>,\n}) {\n    const [updating, setUpdating] = useState<boolean>(false);\n    const [invalidText, setInvalidText] = useState<string | undefined>(undefined);\n    const [subArgOptions, setSubArgOptions] = useState<{ var: string, options: string }[]>([]);\n    const [argSimilarTree, setArgSimilarTree] = useState<ArgSimilarTree | undefined>(undefined);\n    const [argSimilarTreeExpandedIds, setArgSimilarTreeExpandedIds] = useState<string[]>([]);\n    const [argSimilarTreeArgIdsUpdated, setArgSimilarTreeArgIdsUpdated] = useState<string[]>([]);\n\n    useEffect(() => {\n        let { arg, clsArgDefineMap } = props;\n        let subArgs;\n        if (arg.type.startsWith('@')) {\n            let clsName = (arg as CMDClsArg).clsName;\n            subArgs = (clsArgDefineMap[clsName] as CMDObjectArgBase).args\n        } else {\n            subArgs = (arg as CMDObjectArg).args\n        }\n        const subArgOptions = subArgs.map(value => {\n            return {\n                var: value.var,\n                options: value.options.join(\" \"),\n            };\n        });\n\n        setSubArgOptions(subArgOptions);\n        setArgSimilarTree(undefined);\n        setArgSimilarTreeExpandedIds([]);\n    }, [props.arg]);\n\n    const handleClose = () => {\n        setInvalidText(undefined);\n        props.onClose(false);\n    }\n\n    const verifyFlatten = () => {\n        setInvalidText(undefined);\n        const argOptions: { [argVar: string]: string[] } = {};\n        let invalidText: string | undefined = undefined;\n\n        subArgOptions.forEach((arg, idx) => {\n            const names = arg.options.split(' ').filter(n => n.length > 0);\n            if (names.length < 1) {\n                invalidText = `Prop ${idx + 1} option name is required.`\n                return undefined\n            }\n\n            for (const idx in names) {\n                const piece = names[idx];\n                if (!/^[a-z0-9]+(-[a-z0-9]+)*$/.test(piece)) {\n                    invalidText = `Invalid 'Prop ${idx + 1} option name': '${piece}'. Supported regular expression is: [a-z0-9]+(-[a-z0-9]+)* `\n                    return undefined\n                }\n            }\n            argOptions[arg.var] = names;\n        });\n        if (invalidText !== undefined) {\n            setInvalidText(invalidText);\n            return undefined\n        }\n\n        return {\n            subArgsOptions: argOptions,\n        }\n    }\n\n    const handleFlatten = async () => {\n        const data = verifyFlatten();\n        if (data === undefined) {\n            return;\n        }\n\n        setUpdating(true);\n\n        const flattenUrl = `${props.commandUrl}/Arguments/${props.arg.var}/Flatten`\n\n        try {\n            await axios.post(flattenUrl, {\n                ...data\n            });\n            setUpdating(false);\n            await props.onClose(true);\n        } catch (err: any) {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                setInvalidText(\n                    `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`\n                );\n            }\n            setUpdating(false);\n        }\n    }\n\n    const handleDisplaySimilar = () => {\n        if (verifyFlatten() === undefined) {\n            return;\n        }\n\n        setUpdating(true);\n\n        const similarUrl = `${props.commandUrl}/Arguments/${props.arg.var}/FindSimilar`\n        axios.post(similarUrl).then(res => {\n            setUpdating(false);\n            const { tree, expandedIds } = BuildArgSimilarTree(res);\n            setArgSimilarTree(tree);\n            setArgSimilarTreeExpandedIds(expandedIds);\n            setArgSimilarTreeArgIdsUpdated([]);\n        }).catch(err => {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                setInvalidText(\n                    `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`\n                );\n            }\n            setUpdating(false);\n        });\n    }\n\n    const handleDisableSimilar = () => {\n        setArgSimilarTree(undefined);\n        setArgSimilarTreeExpandedIds([]);\n    }\n\n    const onSimilarTreeUpdated = (newTree: ArgSimilarTree) => {\n        setArgSimilarTree(newTree);\n    }\n\n    const onSimilarTreeExpandedIdsUpdated = (expandedIds: string[]) => {\n        setArgSimilarTreeExpandedIds(expandedIds);\n    }\n\n    const handleFlattenSimilar = async () => {\n        const data = verifyFlatten();\n        if (data === undefined) {\n            return;\n        }\n        setUpdating(true);\n        let invalidText = \"\";\n        const updatedIds: string[] = [...argSimilarTreeArgIdsUpdated]\n        for (const idx in argSimilarTree!.selectedArgIds) {\n            const argId = argSimilarTree!.selectedArgIds[idx];\n            if (updatedIds.indexOf(argId) === -1) {\n                const flattenUrl = `${argId}/Flatten`\n                try {\n                    await axios.post(flattenUrl, {\n                        ...data\n                    })\n                    updatedIds.push(argId);\n                    setArgSimilarTreeArgIdsUpdated([...updatedIds]);\n                } catch (err: any) {\n                    console.error(err.response);\n                    if (err.response?.data?.message) {\n                        const data = err.response!.data!;\n                        invalidText += `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`\n                    }\n                }\n            }\n        }\n\n        if (invalidText.length > 0) {\n            setInvalidText(invalidText);\n            setUpdating(false);\n        } else {\n            setUpdating(false);\n            await props.onClose(true);\n        }\n    }\n\n    const buildSubArgText = (arg: { var: string, options: string }, idx: number) => {\n        return (<TextField\n            id={`subArg-${arg.var}`}\n            key={arg.var}\n            label={`Prop ${idx + 1}`}\n            helperText={idx === 0 ? \"You can input multiple names separated by a space character\" : undefined}\n            type=\"text\"\n            fullWidth\n            variant='standard'\n            value={arg.options}\n            onChange={(event: any) => {\n                const options = subArgOptions.map(value => {\n                    if (value.var === arg.var) {\n                        return {\n                            ...value,\n                            options: event.target.value,\n                        }\n                    } else {\n                        return value\n                    }\n                });\n                setSubArgOptions(options)\n            }}\n            margin=\"normal\"\n            required\n        />)\n    }\n\n    return (\n        <Dialog\n            disableEscapeKeyDown\n            open={props.open}\n            sx={{ '& .MuiDialog-paper': { width: '80%' } }}\n        >\n            {!argSimilarTree && <>\n                <DialogTitle>Flatten Props</DialogTitle>\n                <DialogContent dividers={true}>\n                    {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n                    {subArgOptions.map(buildSubArgText)}\n                </DialogContent>\n            </>}\n\n            {argSimilarTree && <>\n                <DialogTitle>Flatten Similar Argument Props</DialogTitle>\n                <DialogContent dividers={true}>\n                    {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n                    <WSECArgumentSimilarPicker tree={argSimilarTree} expandedIds={argSimilarTreeExpandedIds} updatedIds={argSimilarTreeArgIdsUpdated} onTreeUpdated={onSimilarTreeUpdated} onToggle={onSimilarTreeExpandedIdsUpdated} />\n                </DialogContent>\n            </>}\n            <DialogActions>\n                {updating &&\n                    <Box sx={{ width: '100%' }}>\n                        <LinearProgress color='secondary' />\n                    </Box>\n                }\n                {!updating && !argSimilarTree && <>\n                    <Button onClick={handleClose}>Cancel</Button>\n                    {!props.arg.type.startsWith('@') && <Button onClick={handleFlatten}>Flatten</Button>}\n                    {props.arg.type.startsWith('@') && <Button onClick={handleFlatten}>Unwrap & Flatten</Button>}\n                    <Button onClick={handleDisplaySimilar}>Flatten Similar</Button>\n                </>}\n                {!updating && argSimilarTree && <>\n                    <Button onClick={handleDisableSimilar}>Back</Button>\n                    <Button onClick={handleFlattenSimilar} disabled={argSimilarTree.selectedArgIds.length === 0}>Update</Button>\n                </>}\n            </DialogActions>\n        </Dialog>\n    )\n}\n\nfunction UnwrapClsDialog(props: {\n    commandUrl: string,\n    arg: CMDArg,\n    open: boolean,\n    onClose: (unwrapped: boolean) => Promise<void>,\n}) {\n    const [updating, setUpdating] = useState<boolean>(false);\n    const [invalidText, setInvalidText] = useState<string | undefined>(undefined);\n\n    const handleClose = () => {\n        setInvalidText(undefined);\n        props.onClose(false);\n    }\n\n    const handleUnwrap = async () => {\n        setUpdating(true);\n\n        let argVar = props.arg.var;\n        if (props.arg.type.startsWith(\"array\")) {\n            if ((props.arg as CMDArrayArg).item?.type.startsWith(\"@\")) {\n                argVar += \"[]\";\n            }\n        } else if (props.arg.type.startsWith(\"dict\")) {\n            if ((props.arg as CMDDictArg).item?.type.startsWith(\"@\")) {\n                argVar += \"{}\"\n            }\n        }\n\n        const flattenUrl = `${props.commandUrl}/Arguments/${argVar}/UnwrapClass`\n\n        try {\n            await axios.post(flattenUrl);\n            setUpdating(false);\n            await props.onClose(true);\n        } catch (err: any) {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                setInvalidText(\n                    `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`\n                );\n            }\n            setUpdating(false);\n        }\n    }\n\n    return (\n        <Dialog\n            disableEscapeKeyDown\n            open={props.open}\n            sx={{ '& .MuiDialog-paper': { width: '80%' } }}\n        >\n            <DialogTitle>Unwrap Class Type </DialogTitle>\n            <DialogContent dividers={true}>\n                {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n                <ArgTypeTypography>{props.arg.type}</ArgTypeTypography>\n            </DialogContent>\n            <DialogActions>\n                {updating &&\n                    <Box sx={{ width: '100%' }}>\n                        <LinearProgress color='secondary' />\n                    </Box>\n                }\n                {!updating && <>\n                    <Button onClick={handleClose}>Cancel</Button>\n                    <Button onClick={handleUnwrap}>Unwrap Class</Button>\n                </>}\n            </DialogActions>\n        </Dialog>\n    )\n\n}\n\n\nconst PropArgTypeTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 10,\n    fontWeight: 400,\n}))\n\nconst PropRequiredTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: '#dba339',\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 10,\n    fontWeight: 400,\n}))\n\nconst PropHiddenTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: '#8888C3',\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 10,\n    fontWeight: 400,\n}))\n\nconst ArgGroupTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 18,\n    fontWeight: 200,\n}))\n\nconst PropArgOptionTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 16,\n    fontWeight: 700,\n}))\n\nconst PropHiddenArgOptionTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: '#8888C3',\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 16,\n    fontWeight: 700,\n}))\n\nconst PropArgShortSummaryTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 14,\n    fontStyle: \"italic\",\n    fontWeight: 400,\n}))\n\nfunction ArgumentPropsReviewer(props: {\n    title: string,\n    args: CMDArg[],\n    onFlatten?: () => void,\n    onAddSubcommand?: () => void,\n    selectedArg?: CMDArg,\n    depth: number,\n    onSelectSubArg: (subArgVar: string) => void,\n}) {\n    const groupArgs: { [name: string]: CMDArg[] } = {};\n    if (props.args !== undefined) {\n        props.args.forEach((arg) => {\n            const groupName: string = arg.group.length > 0 ? arg.group : \"\";\n            if (!(groupName in groupArgs)) {\n                groupArgs[groupName] = []\n            }\n            groupArgs[groupName].push(arg)\n        })\n    }\n\n    const groups: ArgGroup[] = []\n\n    for (const groupName in groupArgs) {\n        groupArgs[groupName].sort((a, b) => {\n            if (a.required && !b.required) {\n                return -1\n            } else if (!a.required && b.required) {\n                return 1\n            }\n            return a.options[0].localeCompare(b.options[0])\n        });\n        groups.push({\n            name: groupName,\n            args: groupArgs[groupName],\n        })\n    }\n    groups.sort((a, b) => a.name.localeCompare(b.name));\n\n    const checkCanAddSubcommand = () => {\n        if (props.selectedArg && props.args.length > 0) {\n            return true;\n        }\n        return false;\n    }\n\n    const buildArg = (arg: CMDArg, idx: number) => {\n        const argOptionsString = spliceArgOptionsString(arg, props.depth);\n        return (<Box key={`group-arg-${idx}`}\n            sx={{\n                display: \"flex\",\n                flexDirection: \"column\",\n                alignItems: \"stretch\",\n                justifyContent: \"flex-start\",\n                mb: 2\n            }}>\n            <Box sx={{\n                display: \"flex\",\n                flexDirection: \"row\",\n                alignItems: \"flex-end\",\n                justifyContent: \"flex-start\",\n            }}>\n                <ButtonBase onClick={() => {\n                    props.onSelectSubArg(arg.var)\n                }}>\n                    {!arg.hide && <PropArgOptionTypography sx={{ flexShrink: 0 }}>{argOptionsString}</PropArgOptionTypography>}\n                    {arg.hide && <PropHiddenArgOptionTypography sx={{ flexShrink: 0 }}>{argOptionsString}</PropHiddenArgOptionTypography>}\n                </ButtonBase>\n                <Box sx={{ flexGrow: 1 }} />\n                {arg.stage === \"Preview\" && <SmallPreviewTypography\n                    sx={{ flexShrink: 0 }}\n                >\n                    {arg.stage}\n                </SmallPreviewTypography>}\n                {arg.stage === \"Experimental\" && <SmallExperimentalTypography\n                    sx={{ flexShrink: 0 }}\n                >\n                    {arg.stage}\n                </SmallExperimentalTypography>}\n            </Box>\n            <Box sx={{\n                display: \"flex\",\n                flexDirection: \"row\",\n                alignItems: \"flex-start\",\n                justifyContent: \"flex-start\"\n            }}>\n                <Box sx={{\n                    width: 300,\n                    flexShrink: 0,\n                    flexDirection: \"row\",\n                    display: \"flex\",\n                    alignItems: \"center\",\n                }}>\n                    <PropArgTypeTypography sx={{\n                        flexShrink: 0,\n                    }}>{`/${arg.type}/`}</PropArgTypeTypography>\n                    <Box sx={{ flexGrow: 1 }} />\n                    {arg.required && <PropRequiredTypography>[Required]</PropRequiredTypography>}\n                    {arg.hide && <PropHiddenTypography>[Hidden]</PropHiddenTypography>}\n                </Box>\n                {arg.help && <Box sx={{\n                    ml: 4\n                }}>\n                    <PropArgShortSummaryTypography>{arg.help.short}</PropArgShortSummaryTypography>\n                </Box>}\n            </Box>\n\n        </Box>)\n    }\n\n    const buildArgGroup = (group: ArgGroup, idx: number) => {\n        return (\n            <Box\n                key={`group-${idx}`}\n                sx={{\n                    flexGrow: 1,\n                    display: \"flex\",\n                    flexDirection: \"column\",\n                    alignItems: \"stretch\",\n                    justifyContent: \"flex-start\",\n                    ml: 2, mr: 2, mb: 1\n                }}\n            >\n                <Box sx={{ flexShrink: 0, ml: 2, p: 1 }} >\n                    <ArgGroupTypography id={`argGroup-${idx}-header`}>\n                        {group.name.length > 0 ? `${group.name} Group` : \"Default Group\"}\n                    </ArgGroupTypography>\n                </Box>\n                <Box sx={{\n                    display: 'flex',\n                    flexDirection: 'column',\n                    alignItems: 'stretch',\n                    justifyContent: 'flex-start',\n                    ml: 3,\n                    mr: 3,\n                }}>\n                    {group.args.map(buildArg)}\n                </Box>\n            </Box>)\n    }\n\n    if (groups.length === 0) {\n        return (<></>)\n    }\n\n    return (<React.Fragment>\n        <Box sx={{\n            p: 2,\n            display: \"flex\",\n            flexDirection: \"row\",\n            alignItems: \"center\",\n        }}>\n            <SubtitleTypography>{props.title}</SubtitleTypography>\n            {props.onFlatten !== undefined && <Button sx={{ flexShrink: 0, ml: 3 }}\n                startIcon={<CallSplitSharpIcon color=\"secondary\" fontSize='small' />}\n                onClick={props.onFlatten}\n            >\n                <ArgEditTypography>Flatten</ArgEditTypography>\n            </Button>}\n\n            {/* {props.onUnflatten !== undefined && <Button sx={{ flexShrink: 0, ml: 3 }}\n                startIcon={<CallMergeSharpIcon color=\"secondary\" fontSize='small' />}\n                onClick={props.onUnflatten}\n            >\n                <ArgEditTypography>Unflatten</ArgEditTypography>\n            </Button>} */}\n\n            {props.onAddSubcommand !== undefined && checkCanAddSubcommand() && <Button sx={{ flexShrink: 0, ml: 3 }}\n                startIcon={<AddIcon color=\"secondary\" fontSize='small' />}\n                onClick={props.onAddSubcommand}\n            >\n                <ArgEditTypography>Subcommands</ArgEditTypography>\n            </Button>}\n\n        </Box>\n        {groups.map(buildArgGroup)}\n    </React.Fragment>)\n}\n\ninterface ArgGroup {\n    name: string,\n    args: CMDArg[],\n}\n\ntype CMDArgHelp = {\n    short: string\n    lines?: string[]\n    refCommands?: string[]\n}\n\ntype CMDArgDefault<T> = {\n    value: T | null\n}\n\ntype CMDArgBlank<T> = {\n    value: T | null\n}\n\ntype CMDArgEnumItem<T> = {\n    name: string\n    hide: boolean\n    value: T\n}\n\ntype CMDArgEnum<T> = {\n    items: CMDArgEnumItem<T>[]\n}\n\ninterface CMDArgPromptInput {\n    msg: string\n}\n\ninterface CMDPasswordArgPromptInput extends CMDArgPromptInput {\n    confirm: boolean\n}\n\ninterface CMDArgBase {\n    type: string\n    nullable: boolean\n    blank?: CMDArgBlank<any>\n}\n\ninterface CMDArg extends CMDArgBase {\n    var: string\n    options: string[]\n\n    required: boolean\n    stage: \"Stable\" | \"Preview\" | \"Experimental\"\n    hide: boolean\n    group: string\n    help?: CMDArgHelp\n\n    default?: CMDArgDefault<any>\n    idPart?: string\n    prompt?: CMDArgPromptInput\n    configurationKey?: string\n}\n\ninterface CMDArgBaseT<T> extends CMDArgBase {\n    blank?: CMDArgBlank<T>\n}\n\ninterface CMDArgT<T> extends CMDArg {\n    default?: CMDArgDefault<T>\n    blank?: CMDArgBlank<T>\n}\n\n// type: starts with \"@\"\ninterface CMDClsArgBase extends CMDArgBase {\n    clsName: string\n}\n\ninterface CMDClsArg extends CMDClsArgBase, CMDArg {\n    singularOptions?: string[]  // for list use only\n}\n\n// type: string\ninterface CMDStringArgBase extends CMDArgBaseT<string> {\n    enum?: CMDArgEnum<string>\n    // fmt?: CMDStringFormat\n}\n\ninterface CMDStringArg extends CMDStringArgBase, CMDArgT<string> { }\n\n// type: byte\ninterface CMDByteArgBase extends CMDStringArgBase { }\ninterface CMDByteArg extends CMDByteArgBase, CMDStringArg { }\n\n// type: binary\ninterface CMDBinaryArgBase extends CMDStringArgBase { }\ninterface CMDBinaryArg extends CMDBinaryArgBase, CMDStringArg { }\n\n// type: duration\ninterface CMDDurationArgBase extends CMDStringArgBase { }\ninterface CMDDurationArg extends CMDDurationArgBase, CMDStringArg { }\n\n// type: date  As defined by full-date - https://xml2rfc.tools.ietf.org/public/rfc/html/rfc3339.html#anchor14\ninterface CMDDateArgBase extends CMDStringArgBase { }\ninterface CMDDateArg extends CMDDateArgBase, CMDStringArg { }\n\n// type: dateTime  As defined by date-time - https://xml2rfc.tools.ietf.org/public/rfc/html/rfc3339.html#anchor14\ninterface CMDDateTimeArgBase extends CMDStringArgBase { }\ninterface CMDDateTimeArg extends CMDDateTimeArgBase, CMDStringArg { }\n\ninterface CMDTimeArgBase extends CMDStringArgBase { }\ninterface CMDTimeArg extends CMDTimeArgBase, CMDStringArg { }\n\n// type: uuid \ninterface CMDUuidArgBase extends CMDStringArgBase { }\ninterface CMDUuidArg extends CMDUuidArgBase, CMDStringArg { }\n\n// type: password \ninterface CMDPasswordArgBase extends CMDStringArgBase { }\ninterface CMDPasswordArg extends CMDPasswordArgBase, CMDStringArg {\n    prompt?: CMDPasswordArgPromptInput\n}\n\n// type: SubscriptionId\ninterface CMDSubscriptionIdArgBase extends CMDStringArgBase { }\ninterface CMDSubscriptionIdArg extends CMDSubscriptionIdArgBase, CMDStringArg { }\n\n// type: ResourceGroupName \ninterface CMDResourceGroupNameArgBase extends CMDStringArgBase { }\ninterface CMDResourceGroupNameArg extends CMDResourceGroupNameArgBase, CMDStringArg { }\n\n// type: ResourceId \ninterface CMDResourceIdNameArgBase extends CMDStringArgBase { }\ninterface CMDResourceIdNameArg extends CMDResourceIdNameArgBase, CMDStringArg { }\n\n// type: ResourceLocation\ninterface CMDResourceLocationNameArgBase extends CMDStringArgBase { }\ninterface CMDResourceLocationNameArg extends CMDResourceLocationNameArgBase, CMDStringArg { }\n\n\ninterface CMDNumberArgBase extends CMDArgBaseT<number> {\n    enum?: CMDArgEnum<number>\n    // fmt?: CMDIntegerFormat\n}\ninterface CMDNumberArg extends CMDNumberArgBase, CMDArgT<number> { }\n\n// type: integer\ninterface CMDIntegerArgBase extends CMDNumberArgBase { }\ninterface CMDIntegerArg extends CMDIntegerArgBase, CMDNumberArg { }\n\n// type: integer32\ninterface CMDInteger32ArgBase extends CMDNumberArgBase { }\ninterface CMDInteger32Arg extends CMDInteger32ArgBase, CMDNumberArg { }\n\n// type: integer32\ninterface CMDInteger64ArgBase extends CMDNumberArgBase { }\ninterface CMDInteger64Arg extends CMDInteger64ArgBase, CMDNumberArg { }\n\n// type: float\ninterface CMDFloatArgBase extends CMDNumberArgBase { }\ninterface CMDFloatArg extends CMDFloatArgBase, CMDNumberArg { }\n\n// type: float32\ninterface CMDFloat32ArgBase extends CMDNumberArgBase { }\ninterface CMDFloat32Arg extends CMDFloat32ArgBase, CMDNumberArg { }\n\n// type: float64\ninterface CMDFloat64ArgBase extends CMDNumberArgBase { }\ninterface CMDFloat64Arg extends CMDFloat64ArgBase, CMDNumberArg { }\n\n// type: boolean\ninterface CMDBooleanArgBase extends CMDArgBaseT<boolean> { }\ninterface CMDBooleanArg extends CMDBooleanArgBase, CMDArgT<boolean> { }\n\n// type: object\ninterface CMDObjectArgBase extends CMDArgBase {\n    // fmt?: CMDObjectFormat\n    args: CMDArg[]\n}\n\ninterface CMDObjectArg extends CMDObjectArgBase, CMDArg { }\n// type: dict\ninterface CMDDictArgBase extends CMDArgBase {\n    item?: CMDArgBase\n    anyType: boolean\n}\ninterface CMDDictArg extends CMDDictArgBase, CMDArg { }\n\n// type: array\ninterface CMDArrayArgBase extends CMDArgBase {\n    // fmt?: CMDArrayFormat\n    item: CMDArgBase\n}\n\ninterface CMDArrayArg extends CMDArrayArgBase, CMDArg {\n    singularOptions?: string[]\n}\n\ntype ClsArgDefinitionMap = {\n    [clsName: string]: CMDArgBase\n}\n\nfunction decodeArgEnumItem<T>(response: any): CMDArgEnumItem<T> {\n    return {\n        name: response.name,\n        hide: response.hide ?? false,\n        value: response.value as T,\n    }\n}\n\nfunction decodeArgEnum<T>(response: any): CMDArgEnum<T> {\n    let argEnum: CMDArgEnum<T> = {\n        items: response.items.map((item: any) => decodeArgEnumItem<T>(item))\n    }\n    return argEnum;\n}\n\nfunction decodeArgBlank<T>(response: any | undefined): CMDArgBlank<T> | undefined {\n    if (response === undefined || response === null) {\n        return undefined;\n    }\n\n    return {\n        value: response.value as (T | null),\n    }\n}\n\nfunction decodeArgDefault<T>(response: any | undefined): CMDArgDefault<T> | undefined {\n    if (response === undefined || response === null) {\n        return undefined;\n    }\n\n    return {\n        value: response.value as (T | null),\n    }\n}\n\nfunction decodeArgPromptInput(response: any): CMDArgPromptInput | undefined {\n    if (response === undefined || response === null) {\n        return undefined;\n    }\n\n    return {\n        msg: response.msg as string,\n    }\n}\n\nfunction decodePasswordArgPromptInput(response: any): CMDPasswordArgPromptInput | undefined {\n    if (response === undefined || response === null) {\n        return undefined;\n    }\n\n    return {\n        msg: response.msg as string,\n        confirm: (response.confirm ?? false) as boolean,\n    }\n}\n\nfunction decodeArgBase(response: any): { argBase: CMDArgBase, clsDefineMap: ClsArgDefinitionMap } {\n    let argBase: any = {\n        type: response.type,\n        nullable: (response.nullable ?? false) as boolean,\n    }\n\n    let clsDefineMap: ClsArgDefinitionMap = {};\n\n    switch (response.type) {\n        case \"byte\":\n        case \"binary\":\n        case \"duration\":\n        case \"date\":\n        case \"dateTime\":\n        case \"time\":\n        case \"uuid\":\n        case \"password\":\n        case \"SubscriptionId\":\n        case \"ResourceGroupName\":\n        case \"ResourceId\":\n        case \"ResourceLocation\":\n        case \"string\":\n            if (response.enum) {\n                argBase = {\n                    ...argBase,\n                    enum: decodeArgEnum<string>(response.enum),\n                }\n            }\n            if (response.blank) {\n                argBase = {\n                    ...argBase,\n                    blank: decodeArgBlank<string>(response.blank),\n                }\n            }\n            break\n        case \"integer32\":\n        case \"integer64\":\n        case \"integer\":\n            if (response.enum) {\n                argBase = {\n                    ...argBase,\n                    enum: decodeArgEnum<number>(response.enum),\n                }\n            }\n            if (response.blank) {\n                argBase = {\n                    ...argBase,\n                    blank: decodeArgBlank<number>(response.blank),\n                }\n            }\n            break\n        case \"float32\":\n        case \"float64\":\n        case \"float\":\n            if (response.enum) {\n                argBase = {\n                    ...argBase,\n                    enum: decodeArgEnum<number>(response.enum),\n                }\n            }\n            if (response.blank) {\n                argBase = {\n                    ...argBase,\n                    blank: decodeArgBlank<number>(response.blank),\n                }\n            }\n            break\n        case \"boolean\":\n            if (response.blank) {\n                argBase = {\n                    ...argBase,\n                    blank: decodeArgBlank<boolean>(response.blank),\n                }\n            }\n            break\n        case \"object\":\n            if (response.args && Array.isArray(response.args) && response.args.length > 0) {\n                const args: CMDArg[] = response.args.map((resSubArg: any) => {\n                    const subArgParse = decodeArg(resSubArg);\n                    clsDefineMap = {\n                        ...clsDefineMap,\n                        ...subArgParse.clsDefineMap,\n                    }\n                    return subArgParse.arg\n                })\n                argBase = {\n                    ...argBase,\n                    args: args,\n                }\n            } else if (response.additionalProps && response.additionalProps.item) {\n                // Convert additionalProps to dict argBaseType\n                const itemArgBaseParse = decodeArgBase(response.additionalProps.item);\n                clsDefineMap = {\n                    ...clsDefineMap,\n                    ...itemArgBaseParse.clsDefineMap,\n                }\n                const argBaseType = `dict<string, ${itemArgBaseParse.argBase.type}>`\n                argBase = {\n                    ...argBase,\n                    type: argBaseType,\n                    item: itemArgBaseParse.argBase,\n                    anyType: false\n                }\n            } else if (response.additionalProps && response.additionalProps.anyType) {\n                const argBaseType = `dict<string, Any>`\n                argBase = {\n                    ...argBase,\n                    type: argBaseType,\n                    anyType: true\n                }\n            }\n\n            if (response.cls) {\n                const clsName = response.cls;\n                clsDefineMap[clsName] = argBase;\n                argBase = {\n                    type: `@${response.cls}`,\n                    clsName: clsName\n                }\n            }\n            break\n        default:\n            if (response.type.startsWith(\"array<\")) {\n                if (response.item) {\n                    const itemArgBaseParse = decodeArgBase(response.item);\n                    clsDefineMap = {\n                        ...clsDefineMap,\n                        ...itemArgBaseParse.clsDefineMap,\n                    }\n                    const argBaseType = `array<${itemArgBaseParse.argBase.type}>`\n                    argBase = {\n                        ...argBase,\n                        type: argBaseType,\n                        item: itemArgBaseParse.argBase,\n                    }\n                } else {\n                    throw Error(\"Invalid array object. Item is not defined\");\n                }\n\n                if (response.cls) {\n                    const clsName = response.cls;\n                    clsDefineMap[clsName] = argBase;\n                    argBase = {\n                        type: `@${response.cls}`,\n                        clsName: clsName\n                    }\n                }\n            } else if (response.type.startsWith(\"@\")) {\n                argBase[\"clsName\"] = response.type.slice(1);\n            } else {\n                console.error(`Unknown type '${response.type}'`)\n                throw Error(`Unknown type '${response.type}'`)\n            }\n    }\n\n    return {\n        argBase: argBase,\n        clsDefineMap: clsDefineMap,\n    };\n}\n\nfunction decodeArgHelp(response: any): CMDArgHelp {\n    return {\n        short: response.short,\n        lines: response.lines,\n        refCommands: response.refCommands,\n    }\n}\n\nfunction decodeArg(response: any): { arg: CMDArg, clsDefineMap: ClsArgDefinitionMap } {\n    let { argBase, clsDefineMap } = decodeArgBase(response);\n    const options = (response.options as string[]).sort((a, b) => a.length - b.length).reverse();\n    const help = response.help ? decodeArgHelp(response.help) : undefined;\n    const prompt = response.prompt ? decodeArgPromptInput(response.prompt) : undefined;\n\n    let arg: any = {\n        ...argBase,\n        var: response.var as string,\n        options: options,\n        required: (response.required ?? false) as boolean,\n        stage: (response.stage ?? \"Stable\") as (\"Stable\" | \"Preview\" | \"Experimental\"),\n        hide: (response.hide ?? false) as boolean,\n        group: (response.group ?? \"\") as string,\n        help: help,\n        idPart: response.idPart,\n        prompt: prompt,\n        configurationKey: response.configurationKey,\n    }\n\n    switch (argBase.type) {\n        case \"byte\":\n        case \"binary\":\n        case \"duration\":\n        case \"date\":\n        case \"dateTime\":\n        case \"time\":\n        case \"uuid\":\n        case \"SubscriptionId\":\n        case \"ResourceGroupName\":\n        case \"ResourceId\":\n        case \"ResourceLocation\":\n        case \"string\":\n            if (response.default) {\n                arg = {\n                    ...arg,\n                    default: decodeArgDefault<string>(response.default),\n                }\n            }\n            break\n        case \"password\":\n            if (response.prompt) {\n                arg = {\n                    ...arg,\n                    prompt: decodePasswordArgPromptInput(response.prompt),\n                }\n            }\n            if (response.default) {\n                arg = {\n                    ...arg,\n                    default: decodeArgDefault<string>(response.default),\n                }\n            }\n            break\n        case \"integer32\":\n        case \"integer64\":\n        case \"integer\":\n            if (response.default) {\n                arg = {\n                    ...arg,\n                    default: decodeArgDefault<number>(response.default),\n                }\n            }\n            break\n        case \"float32\":\n        case \"float64\":\n        case \"float\":\n            if (response.default) {\n                arg = {\n                    ...arg,\n                    default: decodeArgDefault<number>(response.default),\n                }\n            }\n            break\n        case \"boolean\":\n            if (response.default) {\n                arg = {\n                    ...arg,\n                    default: decodeArgDefault<boolean>(response.default),\n                }\n            }\n            break\n        case \"object\":\n            if (response.default) {\n                arg = {\n                    ...arg,\n                    default: decodeArgDefault<object>(response.default),\n                }\n            }\n            break\n        default:\n            if (argBase.type.startsWith(\"dict<\")) {\n                // dict type\n                if (response.default) {\n                    arg = {\n                        ...arg,\n                        default: decodeArgDefault<object>(response.default),\n                    }\n                }\n            } else if (argBase.type.startsWith(\"array<\")) {\n                // array type\n                if (response.singularOptions) {\n                    arg = {\n                        ...arg,\n                        singularOptions: response.singularOptions as string[],\n                    }\n                }\n                if (response.default) {\n                    arg = {\n                        ...arg,\n                        default: decodeArgDefault<Array<any>>(response.default),\n                    }\n                }\n            } else if (argBase.type.startsWith(\"@\")) {\n                if (response.singularOptions) {\n                    arg = {\n                        ...arg,\n                        singularOptions: response.singularOptions as string[],\n                    }\n                }\n                if (response.default) {\n                    arg = {\n                        ...arg,\n                        default: decodeArgDefault<any>(response.default),\n                    }\n                }\n            } else {\n                console.error(`Unknown type '${argBase.type}'`)\n                throw Error(`Unknown type '${argBase.type}'`)\n            }\n    }\n\n    return {\n        arg: arg,\n        clsDefineMap: clsDefineMap,\n    }\n}\n\nfunction convertArgDefaultText(defaultText: string, argType: string): any {\n    switch (argType) {\n        case \"byte\":\n        case \"binary\":\n        case \"duration\":\n        case \"date\":\n        case \"dateTime\":\n        case \"time\":\n        case \"uuid\":\n        case \"password\":\n        case \"SubscriptionId\":\n        case \"ResourceGroupName\":\n        case \"ResourceId\":\n        case \"ResourceLocation\":\n        case \"string\":\n            if (defaultText.trim().length === 0) {\n                throw Error(`Not supported empty value: '${defaultText}'`);\n            }\n            return defaultText.trim();\n        case \"integer32\":\n        case \"integer64\":\n        case \"integer\":\n            if (Number.isNaN(parseInt(defaultText.trim()))) {\n                throw Error(`Not supported default value for integer type: '${defaultText}'`)\n            }\n            return parseInt(defaultText.trim());\n        case \"float32\":\n        case \"float64\":\n        case \"float\":\n            if (Number.isNaN(parseFloat(defaultText.trim()))) {\n                throw Error(`Not supported default value for float type: '${defaultText}'`)\n            }\n            return parseFloat(defaultText.trim());\n        case \"boolean\":\n            switch (defaultText.trim().toLowerCase()) {\n                case 'true':\n                case 'yes':\n                    return true;\n                case 'false':\n                case 'no':\n                    return false;\n                default:\n                    throw Error(`Not supported default value for boolean type: '${defaultText}'`)\n            }\n        case \"object\":\n            const de = JSON.parse(defaultText.trim());\n            // TODO: verify object\n            return de\n        default:\n            if (argType.startsWith(\"array\")) {\n                const de = JSON.parse(defaultText.trim());\n                // TODO: verify array\n                return de\n            } else if (argType.startsWith(\"dict\")) {\n                const de = JSON.parse(defaultText.trim());\n                // TODO: verify dict\n                return de\n            }\n            throw Error(`Not supported type: ${argType}`)\n    }\n}\n\nconst DecodeArgs = (argGroups: any[]): { args: CMDArg[], clsArgDefineMap: ClsArgDefinitionMap } => {\n    let clsDefineMap: ClsArgDefinitionMap = {};\n    const args: CMDArg[] = [];\n    argGroups.forEach((argGroup: any) => {\n        args.push(...argGroup.args.map((resArg: any) => {\n            const argDecode = decodeArg(resArg);\n            clsDefineMap = {\n                ...clsDefineMap,\n                ...argDecode.clsDefineMap\n            }\n            return argDecode.arg;\n        }))\n    })\n    return {\n        args: args,\n        clsArgDefineMap: clsDefineMap,\n    }\n}\n\nexport default WSEditorCommandArgumentsContent;\nexport { DecodeArgs }\nexport type { CMDArg, ClsArgDefinitionMap };\n",
-        "import { Alert, Box, Button, Card, CardActions, CardContent, Dialog, DialogActions, DialogContent, DialogTitle, FormControlLabel, Accordion, InputLabel, LinearProgress, Radio, RadioGroup, TextField, Typography, TypographyProps, AccordionDetails, IconButton, Input, InputAdornment, AccordionSummaryProps, FormGroup, FormLabel } from '@mui/material';\nimport { styled } from '@mui/system';\nimport axios from 'axios';\nimport React, { useState, useEffect } from 'react';\nimport MuiAccordionSummary from '@mui/material/AccordionSummary';\nimport { NameTypography, ShortHelpTypography, ShortHelpPlaceHolderTypography, LongHelpTypography, StableTypography, PreviewTypography, ExperimentalTypography, SubtitleTypography, CardTitleTypography } from './WSEditorTheme';\nimport DoDisturbOnRoundedIcon from '@mui/icons-material/DoDisturbOnRounded';\nimport AddCircleRoundedIcon from '@mui/icons-material/AddCircleRounded';\nimport KeyboardDoubleArrowRightIcon from '@mui/icons-material/KeyboardDoubleArrowRight';\nimport LabelIcon from '@mui/icons-material/Label';\nimport WSEditorCommandArgumentsContent, { ClsArgDefinitionMap, CMDArg, DecodeArgs } from './WSEditorCommandArgumentsContent';\nimport EditIcon from '@mui/icons-material/Edit';\n\n\ninterface Plane {\n    name: string,\n    displayName: string,\n    moduleOptions?: string[],\n}\n\ninterface Example {\n    name: string,\n    commands: string[],\n}\n\ninterface Resource {\n    id: string,\n    version: string,\n    subresource?: string,\n    swagger: string,\n}\n\ninterface Command {\n    id: string\n    names: string[]\n    help?: {\n        short: string\n        lines?: string[]\n    }\n    stage: \"Stable\" | \"Preview\" | \"Experimental\"\n    version: string\n    examples?: Example[]\n    resources: Resource[]\n\n    // additional property\n    confirmation?: string\n    args?: CMDArg[]\n    clsArgDefineMap?: ClsArgDefinitionMap\n}\n\ninterface ClientConfig {\n    args?: CMDArg[]\n}\n\ninterface ResponseCommand {\n    names: string[],\n    help?: {\n        short: string\n        lines?: string[]\n    }\n    stage?: \"Stable\" | \"Preview\" | \"Experimental\"\n    version: string,\n    examples?: Example[],\n    resources: Resource[],\n    confirmation?: string,\n    argGroups?: any[],\n}\n\ninterface ResponseCommands {\n    [name: string]: ResponseCommand\n}\n\ninterface WSEditorCommandContentProps {\n    workspaceUrl: string\n    previewCommand: Command\n    reloadTimestamp: number\n    onUpdateCommand: (command: Command | null) => void\n}\n\ninterface WSEditorCommandContentState {\n    command?: Command,\n    displayCommandDialog: boolean,\n    displayExampleDialog: boolean,\n    displayCommandDeleteDialog: boolean,\n    displayAddSubcommandDialog: boolean,\n    subcommandDefaultGroupNames?: string[],\n    subcommandArgVar?: string,\n    subcommandSubArgOptions?: { var: string, options: string }[],\n    exampleIdx?: number,\n    loading: boolean,\n}\n\nconst commandPrefix = 'az '\n\nconst ExampleCommandHeaderTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 14,\n    fontWeight: 400,\n}))\n\nconst ExampleCommandBodyTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 14,\n    fontWeight: 400,\n}))\n\nconst ExampleEditTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: \"#5d64cf\",\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 14,\n    fontWeight: 400,\n}));\n\nconst ExampleAccordionSummary = styled((props: AccordionSummaryProps) => (\n    <MuiAccordionSummary\n        expandIcon={<LabelIcon fontSize=\"small\" color=\"primary\" />}\n        {...props}\n    />\n))(({ theme }) => ({\n    flexDirection: 'row-reverse',\n    '& .MuiAccordionSummary-expandIconWrapper.Mui-expanded': {\n        transform: 'rotate(0deg)',\n    },\n}));\n\n\nclass WSEditorCommandContent extends React.Component<WSEditorCommandContentProps, WSEditorCommandContentState> {\n\n    constructor(props: WSEditorCommandContentProps) {\n        super(props);\n        this.state = {\n            command: undefined,\n            displayCommandDialog: false,\n            displayExampleDialog: false,\n            displayCommandDeleteDialog: false,\n            displayAddSubcommandDialog: false,\n            loading: false,\n        }\n    }\n\n    loadCommand = async () => {\n        this.setState({ loading: true })\n        let { workspaceUrl, previewCommand } = this.props\n        let commandNames = previewCommand.names;\n        const leafUrl = `${workspaceUrl}/CommandTree/Nodes/aaz/` + commandNames.slice(0, -1).join('/') + '/Leaves/' + commandNames[commandNames.length - 1];\n        try {\n            let res = await axios.get(leafUrl);\n            let command = DecodeResponseCommand(res.data);\n            if (command.id === this.props.previewCommand.id) {\n                this.setState({\n                    loading: false,\n                    command: command\n                })\n            }\n        } catch (err: any) {\n            this.setState({ loading: false })\n            console.error(err)\n            return\n        }\n    }\n\n    componentDidMount() {\n        this.loadCommand();\n    }\n\n    componentDidUpdate(prevProps: WSEditorCommandContentProps) {\n        if (prevProps.workspaceUrl !== this.props.workspaceUrl || prevProps.previewCommand.id !== this.props.previewCommand.id || prevProps.reloadTimestamp !== this.props.reloadTimestamp) {\n            if (prevProps.previewCommand.id !== this.props.previewCommand.id) {\n                this.setState({ command: undefined })\n            }\n            this.loadCommand();\n        }\n    }\n\n    onCommandDialogDisplay = () => {\n        this.setState({\n            displayCommandDialog: true,\n        })\n    }\n\n    onCommandDeleteDialogDisplay = () => {\n        this.setState({\n            displayCommandDeleteDialog: true,\n        })\n    }\n\n    handleCommandDialogClose = (newCommand?: Command) => {\n        if (newCommand) {\n            this.props.onUpdateCommand(newCommand!);\n        }\n        this.setState({\n            displayCommandDialog: false,\n        })\n    }\n\n    handleCommandDeleteDialogClose = (deleted: boolean) => {\n        if (deleted) {\n            this.props.onUpdateCommand(null);\n        }\n        this.setState({\n            displayCommandDeleteDialog: false,\n        })\n    }\n\n    onExampleDialogDisplay = (idx?: number) => {\n        this.setState({\n            displayExampleDialog: true,\n            exampleIdx: idx,\n        })\n    }\n\n    handleExampleDialogClose = (newCommand?: Command) => {\n        if (newCommand) {\n            this.props.onUpdateCommand(newCommand!);\n        }\n        this.setState({\n            displayExampleDialog: false,\n        })\n    }\n\n    onAddSubcommandDialogDisplay = (argVar: string, subArgOptions: { var: string, options: string }[], argStackNames: string[]) => {\n        this.setState({\n            displayAddSubcommandDialog: true,\n            subcommandArgVar: argVar,\n            subcommandSubArgOptions: subArgOptions,\n            subcommandDefaultGroupNames: [...this.props.previewCommand.names.slice(0, -1), ...argStackNames],\n        })\n    }\n\n    handleAddSubcommandDisplayClose = (add: boolean) => {\n        if (add) {\n            this.props.onUpdateCommand(this.state.command!);\n        }\n        this.setState({\n            displayAddSubcommandDialog: false,\n            subcommandArgVar: undefined,\n            subcommandDefaultGroupNames: undefined\n        })\n    }\n\n    render() {\n        const { workspaceUrl, previewCommand } = this.props;\n        const commandNames = previewCommand.names;\n        const name = commandPrefix + commandNames.join(' ');\n        const commandUrl = `${workspaceUrl}/CommandTree/Nodes/aaz/` + commandNames.slice(0, -1).join('/') + '/Leaves/' + commandNames[commandNames.length - 1];\n\n        const { command, displayCommandDialog, displayExampleDialog, displayCommandDeleteDialog, displayAddSubcommandDialog, exampleIdx, loading } = this.state;\n\n        const buildExampleView = (example: Example, idx: number) => {\n            const buildCommand = (exampleCommand: string, cmdIdx: number) => {\n                return (<Box key={`example-${idx}-command-${cmdIdx}`} sx={{\n                    display: \"flex\",\n                    flexDirection: 'row',\n                    alignItems: 'flex-start',\n                    justifyContent: 'flex-start',\n                }}>\n                    <Box component=\"span\" sx={{\n                        flexShrink: 0,\n                        display: \"flex\",\n                        flexDirection: 'row', alignItems: 'center', justifyContent: 'flex-start',\n                    }}>\n                        <KeyboardDoubleArrowRightIcon fontSize=\"small\" />\n                        <ExampleCommandHeaderTypography sx={{ flexShrink: 0 }}>{commandPrefix}</ExampleCommandHeaderTypography>\n                    </Box>\n                    <Box component=\"span\" sx={{\n                        ml: 0.8,\n                    }}>\n                        <ExampleCommandBodyTypography>{exampleCommand}</ExampleCommandBodyTypography>\n                    </Box>\n                </Box>)\n            }\n            return (\n                <Accordion\n                    elevation={0}\n                    expanded\n                    key={`example-${idx}`}\n                    onDoubleClick={() => { this.onExampleDialogDisplay(idx) }}\n                >\n                    <ExampleAccordionSummary\n                        id={`example-${idx}-header`}\n                    >\n                        <Box sx={{\n                            ml: 1,\n                            flexGrow: 1,\n                            display: \"flex\",\n                            flexDirection: \"row\",\n                            alignItems: \"center\",\n                        }}>\n                            <SubtitleTypography sx={{ flexShrink: 0 }} >{example.name}</SubtitleTypography>\n                            {/* <Box sx={{ flexGrow: 1 }} /> */}\n                            <Button sx={{ flexShrink: 0, ml: 3 }}\n                                startIcon={<EditIcon color=\"secondary\" fontSize='small' />}\n                                onClick={() => { this.onExampleDialogDisplay(idx) }}\n                            >\n                                <ExampleEditTypography>Edit</ExampleEditTypography>\n                            </Button>\n                        </Box>\n                    </ExampleAccordionSummary>\n                    <AccordionDetails sx={{\n                        display: 'flex',\n                        flexDirection: 'column',\n                        alignItems: 'stretch',\n                        justifyContent: 'flex-start',\n                        ml: 3,\n                        mr: 3,\n                        paddingTop: 0,\n                    }}>\n                        {example.commands.map(buildCommand)}\n                    </AccordionDetails>\n                </Accordion>\n            )\n        }\n\n        const buildCommandCard = () => {\n            const shortHelp = (command ?? previewCommand).help?.short;\n            const longHelp = (command ?? previewCommand).help?.lines?.join('\\n');\n            const lines: string[] = (command ?? previewCommand).help?.lines ?? [];\n            const stage = (command ?? previewCommand).stage;\n            const version = (command ?? previewCommand).version;\n\n            return (<Card\n                onDoubleClick={this.onCommandDialogDisplay}\n                elevation={3}\n                sx={{\n                    flexGrow: 1,\n                    display: 'flex',\n                    flexDirection: 'column',\n                    p: 2\n                }}>\n                <CardContent sx={{\n                    flex: '1 0 auto',\n                    display: 'flex',\n                    flexDirection: 'column',\n                    justifyContent: 'stretch',\n                }}>\n                    <Box sx={{\n                        mb: 2,\n                        display: 'flex',\n                        flexDirection: 'row',\n                        alignItems: \"center\"\n                    }}>\n                        <CardTitleTypography sx={{ flexShrink: 0 }}>\n                            [ COMMAND ]\n                        </CardTitleTypography>\n                        <Box sx={{ flexGrow: 1 }} />\n                        {stage === \"Stable\" && <StableTypography\n                            sx={{ flexShrink: 0 }}\n                        >\n                            {`v${version}`}\n                        </StableTypography>}\n                        {stage === \"Preview\" && <PreviewTypography\n                            sx={{ flexShrink: 0 }}\n                        >\n                            {`v${version}`}\n                        </PreviewTypography>}\n                        {stage === \"Experimental\" && <ExperimentalTypography\n                            sx={{ flexShrink: 0 }}\n                        >\n                            {`v${version}`}\n                        </ExperimentalTypography>}\n                    </Box>\n\n                    <NameTypography sx={{ mt: 1 }}>\n                        {name}\n                    </NameTypography>\n                    {shortHelp && <ShortHelpTypography sx={{ ml: 6, mt: 2 }}> {shortHelp} </ShortHelpTypography>}\n                    {!shortHelp && <ShortHelpPlaceHolderTypography sx={{ ml: 6, mt: 2 }}>Please add command short summary!</ShortHelpPlaceHolderTypography>}\n                    {longHelp && <Box sx={{ ml: 6, mt: 1, mb: 1 }}>\n                        {lines.map((line, idx) => (<LongHelpTypography key={idx}>{line}</LongHelpTypography>))}\n                    </Box>}\n                </CardContent>\n                <CardActions sx={{\n                    display: \"flex\",\n                    flexDirection: \"row-reverse\",\n                    alignContent: \"center\",\n                    justifyContent: \"flex-start\"\n                }}>\n                    {loading && <Box sx={{ width: '100%' }}>\n                        <LinearProgress color='secondary' />\n                    </Box>}\n                    {!loading && <Box sx={{\n                        display: \"flex\",\n                        flexDirection: \"row\",\n                        alignContent: \"center\",\n                        justifyContent: \"flex-start\"\n                    }}>\n\n                        <Button\n                            variant='contained' size=\"small\" color='secondary' disableElevation\n                            onClick={this.onCommandDialogDisplay}\n                            disabled={loading}\n                            sx={{ mr: 2 }}\n                        >\n                            <Typography variant='body2'>\n                                Edit\n                            </Typography>\n                        </Button>\n                        <Button\n                            variant='outlined' size=\"small\" color='secondary'\n                            onClick={this.onCommandDeleteDialogDisplay}\n                            disabled={loading}\n                            sx={{ mr: 2 }}\n                        >\n                            <Typography variant='body2'>\n                                Delete\n                            </Typography>\n                        </Button>\n                        <Button\n                            variant='outlined' size=\"small\" color='secondary'\n                            sx={{ mr: 2 }}\n                            disabled\n                        >\n                            <Typography variant='body2'>\n                                Try\n                            </Typography>\n                        </Button>\n                    </Box>}\n                </CardActions>\n            </Card>)\n        }\n\n        const buildArgumentsCard = () => {\n            return (<Card\n                elevation={3}\n                sx={{\n                    flexGrow: 1,\n                    display: 'flex',\n                    flexDirection: 'column',\n                    mt: 1,\n                    p: 2\n                }}>\n                <WSEditorCommandArgumentsContent commandUrl={commandUrl} args={command!.args!} clsArgDefineMap={command!.clsArgDefineMap!} onReloadArgs={this.loadCommand} onAddSubCommand={this.onAddSubcommandDialogDisplay} />\n            </Card>)\n        }\n\n        const buildExampleCard = () => {\n            const examples = command!.examples ?? []\n            return (<Card\n                elevation={3}\n                sx={{\n                    flexGrow: 1,\n                    display: 'flex',\n                    flexDirection: 'column',\n                    mt: 1,\n                    p: 2\n                }}>\n\n                <CardContent sx={{\n                    flex: '1 0 auto',\n                    display: 'flex',\n                    flexDirection: 'column',\n                    alignItems: 'stretch',\n                }}>\n                    <Box sx={{\n                        mb: 2,\n                        display: 'flex',\n                        flexDirection: 'row',\n                        alignItems: \"center\"\n                    }}>\n                        <CardTitleTypography sx={{ flexShrink: 0 }}>\n                            [ EXAMPLE ]\n                        </CardTitleTypography>\n\n                    </Box>\n                    {examples.length > 0 && <Box>\n                        {examples.map(buildExampleView)}\n                    </Box>}\n                </CardContent>\n\n                <CardActions sx={{\n                    display: \"flex\",\n                    flexDirection: \"row-reverse\",\n                }}>\n                    <Button\n                        variant='contained' size=\"small\" color='secondary' disableElevation\n                        onClick={() => this.onExampleDialogDisplay(undefined)}\n                    >\n                        <Typography variant='body2'>\n                            Add\n                        </Typography>\n                    </Button>\n                </CardActions>\n            </Card>)\n        }\n\n        return (\n            <React.Fragment>\n                <Box sx={{\n                    display: 'flex',\n                    flexDirection: 'column',\n                    alignItems: 'stretch',\n                }}>\n                    {buildCommandCard()}\n                    {command !== undefined && command.args !== undefined && buildArgumentsCard()}\n                    {command !== undefined && buildExampleCard()}\n                </Box>\n                {command !== undefined && displayCommandDialog && <CommandDialog open={displayCommandDialog} workspaceUrl={workspaceUrl} command={command!} onClose={this.handleCommandDialogClose} />}\n                {command !== undefined && displayExampleDialog && <ExampleDialog open={displayExampleDialog} workspaceUrl={workspaceUrl} command={command!} idx={exampleIdx} onClose={this.handleExampleDialogClose} />}\n                {command !== undefined && displayCommandDeleteDialog && <CommandDeleteDialog open={displayCommandDeleteDialog} workspaceUrl={workspaceUrl} command={command!} onClose={this.handleCommandDeleteDialogClose} />}\n                {command !== undefined && displayAddSubcommandDialog && <AddSubcommandDialog open={displayAddSubcommandDialog} workspaceUrl={workspaceUrl} command={command!} onClose={this.handleAddSubcommandDisplayClose} argVar={this.state.subcommandArgVar!} subArgOptions={this.state.subcommandSubArgOptions!} defaultGroupNames={this.state.subcommandDefaultGroupNames!} />}\n            </React.Fragment>\n        )\n    }\n}\n\n\nfunction CommandDeleteDialog(props: {\n    workspaceUrl: string,\n    open: boolean,\n    command: Command,\n    onClose: (deleted: boolean) => void\n}) {\n    const [updating, setUpdating] = React.useState<boolean>(false);\n    const [relatedCommands, setRelatedCommands] = React.useState<string[]>([]);\n\n    const getUrls = () => {\n        let urls: string[] = [];\n\n        props.command.resources.forEach(resource => {\n            const resourceId = btoa(resource.id)\n            const version = btoa(resource.version)\n            if (resource.subresource !== undefined) {\n                let subresource = btoa(resource.subresource)\n                // TODO: delete list command together with crud\n                // if (resource.subresource.endsWith('[]') || resource.subresource.endsWith('{}')) {\n                //     let subresource2 = btoa(resource.subresource.slice(0, -2))\n                //     urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources/${subresource2}`)\n                // } else {\n                //     let subresource2 = btoa(resource.subresource + '[]');\n                //     urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources/${subresource2}`)\n                //     subresource2 = btoa(resource.subresource + '{}');\n                //     urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources/${subresource2}`)\n                // }\n                urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources/${subresource}`)\n            } else {\n                urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}`)\n            }\n        })\n        return urls;\n    }\n\n    React.useEffect(() => {\n        setRelatedCommands([]);\n        const urls = getUrls();\n        const promisesAll = urls.map(url => {\n            return axios.get(`${url}/Commands`)\n        })\n        Promise.all(promisesAll)\n            .then(responses => {\n                const commands = new Set<string>();\n                responses.forEach((response: any) => {\n                    const responseCommands: ResponseCommand[] = response.data\n                    responseCommands\n                        .map(responseCommand => DecodeResponseCommand(responseCommand))\n                        .forEach(cmd => { commands.add(cmd.names.join(\" \")) });\n                });\n\n                const cmdNames: string[] = [];\n                commands.forEach(cmdName => cmdNames.push(cmdName));\n                cmdNames.sort((a, b) => a.localeCompare(b));\n                setRelatedCommands(cmdNames);\n            })\n            .catch(err => {\n                console.error(err.response)\n            })\n\n    }, [props.command]);\n\n    const handleClose = () => {\n        props.onClose(false);\n    }\n    const handleDelete = () => {\n        setUpdating(true);\n        const urls = getUrls();\n        const promisesAll = urls.map(url => {\n            return axios.delete(url)\n        })\n        Promise.all(promisesAll)\n            .then(res => {\n                setUpdating(false);\n                props.onClose(true);\n            })\n            .catch(err => {\n                setUpdating(false);\n                console.error(err.response)\n            })\n    }\n    return (\n        <Dialog\n            disableEscapeKeyDown\n            open={props.open}\n        >\n            <DialogTitle>Delete Commands</DialogTitle>\n            <DialogContent dividers={true}>\n                {relatedCommands.map((command, idx) => (\n                    <Typography key={`command-${idx}`} variant=\"body2\">{`${commandPrefix}${command}`}</Typography>\n                ))}\n            </DialogContent>\n            <DialogActions>\n                {updating &&\n                    <Box sx={{ width: '100%' }}>\n                        <LinearProgress color='secondary' />\n                    </Box>\n                }\n                {!updating && <React.Fragment>\n                    <Button onClick={handleClose}>Cancel</Button>\n                    <Button onClick={handleDelete}>Delete</Button>\n                </React.Fragment>}\n            </DialogActions>\n\n        </Dialog>\n    )\n}\n\ninterface CommandDialogProps {\n    workspaceUrl: string,\n    open: boolean\n    command: Command\n    onClose: (newCommand?: Command) => void\n}\n\ninterface CommandDialogState {\n    name: string,\n    stage: string,\n    shortHelp: string,\n    longHelp: string,\n    invalidText?: string,\n    confirmation: string,\n    updating: boolean\n}\n\n\nclass CommandDialog extends React.Component<CommandDialogProps, CommandDialogState> {\n\n    constructor(props: CommandDialogProps) {\n        super(props);\n        this.state = {\n            name: this.props.command.names.join(' '),\n            shortHelp: this.props.command.help?.short ?? \"\",\n            longHelp: this.props.command.help?.lines?.join('\\n') ?? \"\",\n            stage: this.props.command.stage,\n            confirmation: this.props.command.confirmation ?? \"\",\n            updating: false\n        }\n    }\n\n    handleModify = (event: any) => {\n        let { name, stage, shortHelp, longHelp, confirmation } = this.state\n        let { workspaceUrl, command } = this.props\n\n        name = name.trim();\n        shortHelp = shortHelp.trim();\n        longHelp = longHelp.trim();\n        confirmation = confirmation.trim();\n\n        const names = name.split(' ').filter(n => n.length > 0);\n\n        this.setState({\n            invalidText: undefined\n        })\n\n        if (names.length < 1) {\n            this.setState({\n                invalidText: `Field 'Name' is required.`\n            })\n            return\n        }\n\n        for (const idx in names) {\n            const piece = names[idx];\n            if (!/^[a-z0-9]+(-[a-z0-9]+)*$/.test(piece)) {\n                this.setState({\n                    invalidText: `Invalid Name part: '${piece}'. Supported regular expression is: [a-z0-9]+(-[a-z0-9]+)* `\n                })\n                return\n            }\n        }\n\n        if (shortHelp.length < 1) {\n            this.setState({\n                invalidText: `Field 'Short Summary' is required.`\n            })\n            return\n        }\n\n        let lines: string[] | null = null;\n        if (longHelp.length > 1) {\n            lines = longHelp.split('\\n').filter(l => l.length > 0);\n        }\n\n        this.setState({\n            updating: true,\n        })\n\n        const leafUrl = `${workspaceUrl}/CommandTree/Nodes/aaz/` + command.names.slice(0, -1).join('/') + '/Leaves/' + command.names[command.names.length - 1];\n\n        axios.patch(leafUrl, {\n            help: {\n                short: shortHelp,\n                lines: lines,\n            },\n            stage: stage,\n            confirmation: confirmation,\n        }).then(res => {\n            const name = names.join(' ');\n            if (name === command.names.join(' ')) {\n                const cmd = DecodeResponseCommand(res.data);\n                this.setState({\n                    updating: false,\n                })\n                this.props.onClose(cmd);\n            } else {\n                // Rename command\n                axios.post(`${leafUrl}/Rename`, {\n                    name: name\n                }).then(res => {\n                    const cmd = DecodeResponseCommand(res.data);\n                    this.setState({\n                        updating: false,\n                    })\n                    this.props.onClose(cmd);\n                })\n            }\n        }).catch(err => {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                this.setState({\n                    invalidText: `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`,\n                })\n            }\n            this.setState({\n                updating: false,\n            })\n        });\n    }\n\n    handleClose = () => {\n        this.setState({\n            invalidText: undefined\n        });\n        this.props.onClose();\n    }\n\n    render() {\n        const { name, shortHelp, longHelp, invalidText, updating, stage, confirmation } = this.state;\n        return (\n            <Dialog\n                disableEscapeKeyDown\n                open={this.props.open}\n                sx={{ '& .MuiDialog-paper': { width: '80%' } }}\n            >\n                <DialogTitle>Command</DialogTitle>\n                <DialogContent dividers={true}>\n                    {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n                    <InputLabel required shrink sx={{ font: \"inherit\" }}>Stage</InputLabel>\n                    <RadioGroup\n                        row\n                        value={stage}\n                        name=\"stage\"\n                        onChange={(event: any) => {\n                            this.setState({\n                                stage: event.target.value,\n                            })\n                        }}\n                    >\n                        <FormControlLabel value=\"Stable\" control={<Radio />} label=\"Stable\" sx={{ ml: 4 }} />\n                        <FormControlLabel value=\"Preview\" control={<Radio />} label=\"Preview\" sx={{ ml: 4 }} />\n                        <FormControlLabel value=\"Experimental\" control={<Radio />} label=\"Experimental\" sx={{ ml: 4 }} />\n                    </RadioGroup>\n\n                    <TextField\n                        id=\"name\"\n                        label=\"Name\"\n                        type=\"text\"\n                        fullWidth\n                        variant='standard'\n                        value={name}\n                        onChange={(event: any) => {\n                            this.setState({\n                                name: event.target.value,\n                            })\n                        }}\n                        margin=\"normal\"\n                        required\n                    />\n                    <TextField\n                        id=\"shortSummary\"\n                        label=\"Short Summary\"\n                        type=\"text\"\n                        fullWidth\n                        variant='standard'\n                        value={shortHelp}\n                        onChange={(event: any) => {\n                            this.setState({\n                                shortHelp: event.target.value,\n                            })\n                        }}\n                        margin=\"normal\"\n                        required\n                    />\n                    <TextField\n                        id=\"longSummary\"\n                        label=\"Long Summary\"\n                        helperText=\"Please add long summer in lines.\"\n                        type=\"text\"\n                        fullWidth\n                        multiline\n                        variant='standard'\n                        value={longHelp}\n                        onChange={(event: any) => {\n                            this.setState({\n                                longHelp: event.target.value,\n                            })\n                        }}\n                        margin=\"normal\"\n                    />\n                    <TextField\n                        id=\"confirmation\"\n                        label=\"Command confirmation\"\n                        helperText=\"Modify or clear confirmation message as needed.\"\n                        type=\"text\"\n                        fullWidth\n                        multiline\n                        variant='standard'\n                        value={confirmation}\n                        onChange={(event: any) => {\n                            this.setState({\n                                confirmation: event.target.value,\n                            })\n                        }}\n                        margin=\"normal\"\n                    />\n                </DialogContent>\n                <DialogActions>\n                    {updating &&\n                        <Box sx={{ width: '100%' }}>\n                            <LinearProgress color='secondary' />\n                        </Box>\n                    }\n                    {!updating && <React.Fragment>\n                        <Button onClick={this.handleClose}>Cancel</Button>\n                        <Button onClick={this.handleModify}>Save</Button>\n                    </React.Fragment>}\n                </DialogActions>\n            </Dialog>\n        )\n    }\n}\n\n// function CommandDeleteDialog\n\ninterface ExampleDialogProps {\n    workspaceUrl: string\n    open: boolean\n    command: Command\n    idx?: number\n    onClose: (newCommand?: Command) => void\n}\n\ninterface ExampleDialogState {\n    name: string\n    exampleCommands: string[]\n    isAdd: boolean\n    invalidText?: string\n    updating: boolean\n}\n\nconst ExampleCommandTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 16,\n    fontWeight: 400,\n}))\n\nclass ExampleDialog extends React.Component<ExampleDialogProps, ExampleDialogState> {\n\n    constructor(props: ExampleDialogProps) {\n        super(props);\n        const examples: Example[] = this.props.command.examples ?? [];\n        if (this.props.idx === undefined) {\n            this.state = {\n                name: \"\",\n                exampleCommands: [\"\",],\n                isAdd: true,\n                invalidText: undefined,\n                updating: false,\n            }\n        } else {\n            const example = examples[this.props.idx];\n            this.state = {\n                name: example.name,\n                exampleCommands: example.commands,\n                isAdd: false,\n                invalidText: undefined,\n                updating: false,\n            }\n        }\n    }\n\n    onUpdateExamples = (examples: Example[]) => {\n        let { workspaceUrl, command } = this.props;\n\n        const leafUrl = `${workspaceUrl}/CommandTree/Nodes/aaz/` + command.names.slice(0, -1).join('/') + '/Leaves/' + command.names[command.names.length - 1];\n\n        this.setState({\n            updating: true,\n        })\n        axios.patch(leafUrl, {\n            examples: examples\n        }).then(res => {\n            const cmd = DecodeResponseCommand(res.data);\n            this.setState({\n                updating: false,\n            })\n            this.props.onClose(cmd);\n        }).catch(err => {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                this.setState({\n                    invalidText: `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`,\n                })\n            }\n            this.setState({\n                updating: false,\n            })\n        });\n    }\n\n    handleDelete = () => {\n        let { command } = this.props;\n        let examples: Example[] = command.examples ?? [];\n        let idx = this.props.idx!;\n        examples = [...examples.slice(0, idx), ...examples.slice(idx + 1)];\n        this.onUpdateExamples(examples);\n    }\n\n    handleModify = () => {\n        let { command } = this.props;\n        let { name, exampleCommands } = this.state;\n        let examples: Example[] = command.examples ?? [];\n        let idx = this.props.idx!;\n\n        name = name.trim();\n        if (name.length < 1) {\n            this.setState({\n                invalidText: `Field 'Name' is required.`\n            })\n            return\n        }\n        exampleCommands = exampleCommands.map(cmd => {\n            return cmd.split('\\n')\n                .map(cmdLine => cmdLine.trim())\n                .filter(cmdLine => cmdLine.length > 0)\n                .join(' ')\n                .trim();\n        }).filter(cmd => cmd.length > 0);\n\n        if (exampleCommands.length < 1) {\n            this.setState({\n                invalidText: `Field 'Commands' is required.`\n            })\n            return\n        }\n\n        const newExample: Example = {\n            name: name,\n            commands: exampleCommands\n        }\n\n        examples = [...examples.slice(0, idx), newExample, ...examples.slice(idx + 1)];\n\n        this.onUpdateExamples(examples);\n    }\n\n    handleAdd = () => {\n        let { command } = this.props;\n        let { name, exampleCommands } = this.state;\n        let examples: Example[] = command.examples ?? [];\n\n        name = name.trim();\n        if (name.length < 1) {\n            this.setState({\n                invalidText: `Field 'Name' is required.`\n            })\n            return\n        }\n        exampleCommands = exampleCommands.map(cmd => {\n            return cmd.split('\\n')\n                .map(cmdLine => cmdLine.trim())\n                .filter(cmdLine => cmdLine.length > 0)\n                .join(' ')\n                .trim();\n        }).filter(cmd => cmd.length > 0);\n\n        if (exampleCommands.length < 1) {\n            this.setState({\n                invalidText: `Field 'Commands' is required.`\n            })\n            return\n        }\n\n        const newExample: Example = {\n            name: name,\n            commands: exampleCommands\n        }\n        examples.push(newExample);\n\n        this.onUpdateExamples(examples);\n    }\n\n    handleClose = () => {\n        this.setState({\n            invalidText: undefined\n        });\n        this.props.onClose()\n    }\n\n    onModifyExampleCommand = (cmd: string, idx: number) => {\n        this.setState(preState => {\n            return {\n                ...preState,\n                exampleCommands: [...preState.exampleCommands.slice(0, idx), cmd, ...preState.exampleCommands.slice(idx + 1)]\n            }\n        })\n    }\n\n    onRemoveExampleCommand = (idx: number) => {\n        this.setState(preState => {\n            let exampleCommands: string[] = [...preState.exampleCommands.slice(0, idx), ...preState.exampleCommands.slice(idx + 1)];\n            if (exampleCommands.length === 0) {\n                exampleCommands.push(\"\");\n            }\n            return {\n                ...preState,\n                exampleCommands: exampleCommands,\n            }\n        })\n    }\n\n    onAddExampleCommand = () => {\n        this.setState(preState => {\n            return {\n                ...preState,\n                exampleCommands: [...preState.exampleCommands, \"\"]\n            }\n        })\n    }\n\n    render() {\n        const { name, exampleCommands, isAdd, invalidText, updating } = this.state;\n\n        const buildExampleInput = (cmd: string, idx: number) => {\n            return (\n                <Box key={idx} sx={{\n                    display: 'flex',\n                    flexDirection: 'row',\n                    alignItems: 'center',\n                    justifyContent: 'flex-start',\n                    ml: 1,\n                }}>\n                    <IconButton\n                        edge=\"start\"\n                        color=\"inherit\"\n                        onClick={() => this.onRemoveExampleCommand(idx)}\n                        aria-label=\"remove\"\n                    >\n                        <DoDisturbOnRoundedIcon fontSize=\"small\" />\n                    </IconButton>\n                    <Input\n                        id={`command-${idx}`}\n                        multiline\n                        value={cmd}\n                        onChange={(event: any) => {\n                            this.onModifyExampleCommand(event.target.value, idx)\n                        }}\n                        sx={{ flexGrow: 1 }}\n                        placeholder=\"Input a command here.\"\n                        startAdornment={\n                            <InputAdornment position=\"start\">\n                                <ExampleCommandTypography>{commandPrefix}</ExampleCommandTypography>\n                            </InputAdornment>\n                        }\n                    />\n                </Box>\n            );\n        }\n\n        return (\n            <Dialog\n                disableEscapeKeyDown\n                open={this.props.open}\n                sx={{ '& .MuiDialog-paper': { width: '80%' } }}\n            >\n                <DialogTitle>{isAdd ? \"Add Example\" : \"Modify Example\"}</DialogTitle>\n                <DialogContent dividers={true}>\n                    {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n                    <TextField\n                        id=\"name\"\n                        label=\"Name\"\n                        type=\"text\"\n                        fullWidth\n                        variant='standard'\n                        value={name}\n                        onChange={(event: any) => {\n                            this.setState({\n                                name: event.target.value,\n                            })\n                        }}\n                        margin=\"normal\"\n                        required\n                    />\n                    <InputLabel required sx={{ font: \"inherit\", mt: 1 }}>Commands</InputLabel>\n                    {exampleCommands.map(buildExampleInput)}\n                    <Box sx={{\n                        display: 'flex',\n                        flexDirection: 'row',\n                        alignItems: 'center',\n                        justifyContent: 'flex-start',\n                        ml: 1,\n                    }}>\n                        <IconButton\n                            edge=\"start\"\n                            color=\"inherit\"\n                            onClick={this.onAddExampleCommand}\n                            aria-label=\"add\"\n                        >\n                            <AddCircleRoundedIcon fontSize=\"small\" />\n                        </IconButton>\n                        <ExampleCommandTypography sx={{ flexShrink: 0 }}> One more command</ExampleCommandTypography>\n                    </Box>\n                </DialogContent>\n                <DialogActions>\n                    {updating &&\n                        <Box sx={{ width: '100%' }}>\n                            <LinearProgress color='secondary' />\n                        </Box>\n                    }\n                    {!updating && <React.Fragment>\n                        <Button onClick={this.handleClose}>Cancel</Button>\n                        {!isAdd && <React.Fragment>\n                            <Button onClick={this.handleDelete}>Delete</Button>\n                            <Button onClick={this.handleModify}>Save</Button>\n                        </React.Fragment>}\n                        {isAdd && <Button onClick={this.handleAdd}>Add</Button>}\n                    </React.Fragment>}\n                </DialogActions>\n            </Dialog>\n        )\n    }\n}\n\nfunction AddSubcommandDialog(props: {\n    workspaceUrl: string,\n    command: Command,\n    argVar: string,\n    subArgOptions: { var: string, options: string }[],\n    defaultGroupNames: string[],\n    open: boolean,\n    onClose: (added: boolean) => void,\n}) {\n\n    const [updating, setUpdating] = useState<boolean>(false);\n    const [invalidText, setInvalidText] = useState<string | undefined>(undefined);\n    const [commandGroupName, setCommandGroupName] = useState<string>(\"\");\n    const [refArgsOptions, setRefArgsOptions] = useState<{ var: string, options: string }[]>([]);\n\n    useEffect(() => {\n        setCommandGroupName(props.defaultGroupNames.join(' '));\n        setRefArgsOptions(props.subArgOptions);\n    }, [props.argVar, props.defaultGroupNames]);\n\n    const handleClose = () => {\n        setInvalidText(undefined);\n        props.onClose(false);\n    }\n\n    const verifyAddSubresource = () => {\n        setInvalidText(undefined);\n        const argOptions: { [argVar: string]: string[] } = {}\n        let invalidText: string | undefined = undefined;\n        refArgsOptions.forEach((arg, idx) => {\n            const names = arg.options.split(' ').filter(n => n.length > 0);\n            if (names.length < 1) {\n                invalidText = `Prop ${idx + 1} option name is required.`\n                return undefined\n            }\n\n            for (const idx in names) {\n                const piece = names[idx];\n                if (!/^[a-z0-9]+(-[a-z0-9]+)*$/.test(piece)) {\n                    invalidText = `Invalid 'Prop ${idx + 1} option name': '${piece}'. Supported regular expression is: [a-z0-9]+(-[a-z0-9]+)* `\n                    return undefined\n                }\n            }\n            argOptions[arg.var] = names;\n        });\n\n        const names = commandGroupName.split(' ').filter(n => n.length > 0);\n        if (names.length < 1) {\n            invalidText = 'Invalid Command group name';\n            return\n        }\n\n        if (invalidText !== undefined) {\n            setInvalidText(invalidText);\n            return undefined\n        }\n\n        return {\n            commandGroupName: names.join(' '),\n            refArgsOptions: argOptions,\n        }\n    }\n\n    const handleAddSubresource = async () => {\n        const urls = props.command.resources.map(resource => {\n            const resourceId = btoa(resource.id)\n            const version = btoa(resource.version)\n            return `${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources`\n        })\n\n        if (urls.length !== 1) {\n            setInvalidText(`Cannot create subcommands, command contains ${props.command.resources.length} resources`);\n            return;\n        }\n\n        const data = verifyAddSubresource();\n        if (data === undefined) {\n            return;\n        }\n\n        setUpdating(true);\n\n        try {\n            await axios.post(urls[0], {\n                ...data,\n                arg: props.argVar,\n            })\n            props.onClose(true);\n        } catch (err: any) {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                setInvalidText(`ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`);\n            }\n            setUpdating(false);\n        }\n    }\n\n    const buildRefArgText = (arg: { var: string, options: string }, idx: number) => {\n        return (<TextField\n            id={`subArg-${arg.var}`}\n            key={arg.var}\n            label={`${arg.var}`}\n            helperText={idx === 0 ? \"You can input multiple names separated by a space character\" : undefined}\n            type=\"text\"\n            fullWidth\n            variant='standard'\n            value={arg.options}\n            onChange={(event: any) => {\n                const options = refArgsOptions.map(value => {\n                    if (value.var === arg.var) {\n                        return {\n                            ...value,\n                            options: event.target.value,\n                        }\n                    } else {\n                        return value\n                    }\n                });\n                setRefArgsOptions(options)\n            }}\n            margin=\"normal\"\n            required\n        />)\n    }\n\n    return (<Dialog\n        disableEscapeKeyDown\n        open={props.open}\n        sx={{ '& .MuiDialog-paper': { width: '80%' } }}\n    >\n        <DialogTitle>Add Subcommands</DialogTitle>\n        <DialogContent dividers={true}>\n            {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n            <FormLabel>Subcommand Group</FormLabel>\n            <TextField\n                id='subcommand-group-name'\n                label='name'\n                placeholder='Please input command group name for subcommands'\n                type=\"text\"\n                variant='standard'\n                value={commandGroupName}\n                fullWidth\n                margin=\"normal\"\n                required\n                onChange={(event: any) => {\n                    setCommandGroupName(event.target.value)\n                }}\n            />\n            {refArgsOptions.length > 0 && <>\n                <FormLabel>Argument Options</FormLabel>\n                {refArgsOptions.map(buildRefArgText)}\n            </>}\n        </DialogContent>\n        <DialogActions>\n            {updating &&\n                <Box sx={{ width: '100%' }}>\n                    <LinearProgress color='secondary' />\n                </Box>\n            }\n            {!updating && <>\n                <Button onClick={handleClose}>Cancel</Button>\n                <Button onClick={handleAddSubresource}>Add Subcommands</Button>\n            </>}\n        </DialogActions>\n    </Dialog>)\n}\n\nconst DecodeResponseCommand = (command: ResponseCommand): Command => {\n    let cmd: Command = {\n        id: 'command:' + command.names.join('/'),\n        names: command.names,\n        help: command.help,\n        stage: command.stage ?? \"Stable\",\n        examples: command.examples,\n        resources: command.resources,\n        version: command.version,\n    }\n\n    if (command.confirmation) {\n        cmd.confirmation = command.confirmation\n    }\n\n    if (command.argGroups) {\n        cmd = {\n            ...cmd,\n            ...DecodeArgs(command.argGroups!)\n        }\n    }\n\n    return cmd;\n}\n\nconst DecodeResponseClientConfig = (clientConfig: any): ClientConfig => {\n    if (clientConfig.argGroups === undefined) {\n        return {}\n    }\n    return {\n        args: DecodeArgs(clientConfig.argGroups!).args\n    }\n}\n\nexport default WSEditorCommandContent;\n\nexport { DecodeResponseCommand };\nexport type { Plane, Command, Resource, ResponseCommand, ResponseCommands };\n\n",
+        "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\nconst _excluded = [\"component\", \"direction\", \"spacing\", \"divider\", \"children\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport { createUnarySpacing, getValue, handleBreakpoints, unstable_extendSxProp as extendSxProp, unstable_resolveBreakpointValues as resolveBreakpointValues } from '@mui/system';\nimport { deepmerge } from '@mui/utils';\nimport styled from '../styles/styled';\nimport useThemeProps from '../styles/useThemeProps';\n/**\n * Return an array with the separator React element interspersed between\n * each React node of the input children.\n *\n * > joinChildren([1,2,3], 0)\n * [1,0,2,0,3]\n */\n\nimport { jsx as _jsx } from \"react/jsx-runtime\";\n\nfunction joinChildren(children, separator) {\n  const childrenArray = React.Children.toArray(children).filter(Boolean);\n  return childrenArray.reduce((output, child, index) => {\n    output.push(child);\n\n    if (index < childrenArray.length - 1) {\n      output.push( /*#__PURE__*/React.cloneElement(separator, {\n        key: `separator-${index}`\n      }));\n    }\n\n    return output;\n  }, []);\n}\n\nconst getSideFromDirection = direction => {\n  return {\n    row: 'Left',\n    'row-reverse': 'Right',\n    column: 'Top',\n    'column-reverse': 'Bottom'\n  }[direction];\n};\n\nexport const style = ({\n  ownerState,\n  theme\n}) => {\n  let styles = _extends({\n    display: 'flex'\n  }, handleBreakpoints({\n    theme\n  }, resolveBreakpointValues({\n    values: ownerState.direction,\n    breakpoints: theme.breakpoints.values\n  }), propValue => ({\n    flexDirection: propValue\n  })));\n\n  if (ownerState.spacing) {\n    const transformer = createUnarySpacing(theme);\n    const base = Object.keys(theme.breakpoints.values).reduce((acc, breakpoint) => {\n      if (ownerState.spacing[breakpoint] != null || ownerState.direction[breakpoint] != null) {\n        acc[breakpoint] = true;\n      }\n\n      return acc;\n    }, {});\n    const directionValues = resolveBreakpointValues({\n      values: ownerState.direction,\n      base\n    });\n    const spacingValues = resolveBreakpointValues({\n      values: ownerState.spacing,\n      base\n    });\n\n    const styleFromPropValue = (propValue, breakpoint) => {\n      return {\n        '& > :not(style) + :not(style)': {\n          margin: 0,\n          [`margin${getSideFromDirection(breakpoint ? directionValues[breakpoint] : ownerState.direction)}`]: getValue(transformer, propValue)\n        }\n      };\n    };\n\n    styles = deepmerge(styles, handleBreakpoints({\n      theme\n    }, spacingValues, styleFromPropValue));\n  }\n\n  return styles;\n};\nconst StackRoot = styled('div', {\n  name: 'MuiStack',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    return [styles.root];\n  }\n})(style);\nconst Stack = /*#__PURE__*/React.forwardRef(function Stack(inProps, ref) {\n  const themeProps = useThemeProps({\n    props: inProps,\n    name: 'MuiStack'\n  });\n  const props = extendSxProp(themeProps);\n\n  const {\n    component = 'div',\n    direction = 'column',\n    spacing = 0,\n    divider,\n    children\n  } = props,\n        other = _objectWithoutPropertiesLoose(props, _excluded);\n\n  const ownerState = {\n    direction,\n    spacing\n  };\n  return /*#__PURE__*/_jsx(StackRoot, _extends({\n    as: component,\n    ownerState: ownerState,\n    ref: ref\n  }, other, {\n    children: divider ? joinChildren(children, divider) : children\n  }));\n});\nprocess.env.NODE_ENV !== \"production\" ? Stack.propTypes\n/* remove-proptypes */\n= {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n\n  /**\n   * The component used for the root node.\n   * Either a string to use a HTML element or a component.\n   */\n  component: PropTypes.elementType,\n\n  /**\n   * Defines the `flex-direction` style property.\n   * It is applied for all screen sizes.\n   * @default 'column'\n   */\n  direction: PropTypes.oneOfType([PropTypes.oneOf(['column-reverse', 'column', 'row-reverse', 'row']), PropTypes.arrayOf(PropTypes.oneOf(['column-reverse', 'column', 'row-reverse', 'row'])), PropTypes.object]),\n\n  /**\n   * Add an element between each child.\n   */\n  divider: PropTypes.node,\n\n  /**\n   * Defines the space between immediate children.\n   * @default 0\n   */\n  spacing: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.number, PropTypes.string])), PropTypes.number, PropTypes.object, PropTypes.string]),\n\n  /**\n   * The system prop, which allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default Stack;",
+        "import React from 'react';\nimport { Box, Autocomplete, TextField } from '@mui/material';\n\ninterface ExampleItemsSelectorProps {\n    commonPrefix: string,\n    options: string[],\n    name: string,\n    value: string | null,\n    onValueUpdate: (value: string | null) => void\n}\n\n\nclass ExampleItemSelector extends React.Component<ExampleItemsSelectorProps> {\n\n    constructor(props: ExampleItemsSelectorProps) {\n        super(props);\n        this.state = {\n            value: this.props.options.length === 1 ? this.props.options[0] : null,\n        }\n    }\n\n    render() {\n        const { name, options, commonPrefix, value } = this.props;\n        return (\n            <Autocomplete\n                id={name}\n                value={value}\n                options={options}\n                onInputChange={(event, newValue: any) => {\n                    this.props.onValueUpdate(newValue);\n                }}\n                getOptionLabel={(option) => {\n                    return option.replace(commonPrefix, '');\n                }}\n                renderOption={(props, option) => {\n                    return (\n                        <Box component='li'\n                            {...props}\n                        >\n                            {option.replace(commonPrefix, '')}\n                        </Box>\n                    )\n                }}\n                selectOnFocus\n                // clearOnBlur\n                freeSolo\n                renderInput={(params) => (\n                    <TextField\n                        {...params}\n                        size='small'\n                        // variant='filled'\n                        label={name}\n                        required\n                    />\n                )}\n            />\n        )\n    }\n}\n\nexport { ExampleItemSelector };\n",
+        "import { Alert, Box, Button, Card, CardActions, CardContent, Dialog, DialogActions, DialogContent, DialogTitle, FormControlLabel, Accordion, InputLabel, LinearProgress, Radio, RadioGroup, TextField, Typography, TypographyProps, AccordionDetails, IconButton, Input, InputAdornment, AccordionSummaryProps, FormGroup, FormLabel } from '@mui/material';\nimport { styled } from '@mui/system';\nimport axios from 'axios';\nimport React, { useState, useEffect } from 'react';\nimport MuiAccordionSummary from '@mui/material/AccordionSummary';\nimport { NameTypography, ShortHelpTypography, ShortHelpPlaceHolderTypography, LongHelpTypography, StableTypography, PreviewTypography, ExperimentalTypography, SubtitleTypography, CardTitleTypography } from './WSEditorTheme';\nimport DoDisturbOnRoundedIcon from '@mui/icons-material/DoDisturbOnRounded';\nimport AddCircleRoundedIcon from '@mui/icons-material/AddCircleRounded';\nimport KeyboardDoubleArrowRightIcon from '@mui/icons-material/KeyboardDoubleArrowRight';\nimport LabelIcon from '@mui/icons-material/Label';\nimport WSEditorCommandArgumentsContent, { ClsArgDefinitionMap, CMDArg, DecodeArgs } from './WSEditorCommandArgumentsContent';\nimport EditIcon from '@mui/icons-material/Edit';\nimport CloseIcon from '@mui/icons-material/Close';\nimport Stack from '@mui/material/Stack';\nimport { ExampleItemSelector } from './WSEditorExamplePicker';\n\n\ninterface Plane {\n    name: string,\n    displayName: string,\n    moduleOptions?: string[],\n}\n\ninterface Example {\n    name: string,\n    commands: string[],\n}\n\ninterface Resource {\n    id: string,\n    version: string,\n    subresource?: string,\n    swagger: string,\n}\n\ninterface Command {\n    id: string\n    names: string[]\n    help?: {\n        short: string\n        lines?: string[]\n    }\n    stage: \"Stable\" | \"Preview\" | \"Experimental\"\n    version: string\n    examples?: Example[]\n    resources: Resource[]\n\n    // additional property\n    confirmation?: string\n    args?: CMDArg[]\n    clsArgDefineMap?: ClsArgDefinitionMap\n}\n\ninterface ClientConfig {\n    args?: CMDArg[]\n}\n\ninterface ResponseCommand {\n    names: string[],\n    help?: {\n        short: string\n        lines?: string[]\n    }\n    stage?: \"Stable\" | \"Preview\" | \"Experimental\"\n    version: string,\n    examples?: Example[],\n    resources: Resource[],\n    confirmation?: string,\n    argGroups?: any[],\n}\n\ninterface ResponseCommands {\n    [name: string]: ResponseCommand\n}\n\ninterface WSEditorCommandContentProps {\n    workspaceUrl: string\n    previewCommand: Command\n    reloadTimestamp: number\n    onUpdateCommand: (command: Command | null) => void\n}\n\ninterface WSEditorCommandContentState {\n    command?: Command,\n    displayCommandDialog: boolean,\n    displayExampleDialog: boolean,\n    displayCommandDeleteDialog: boolean,\n    displayAddSubcommandDialog: boolean,\n    subcommandDefaultGroupNames?: string[],\n    subcommandArgVar?: string,\n    subcommandSubArgOptions?: { var: string, options: string }[],\n    exampleIdx?: number,\n    loading: boolean,\n}\n\nconst commandPrefix = 'az '\n\nconst ExampleCommandHeaderTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 14,\n    fontWeight: 400,\n}))\n\nconst ExampleCommandBodyTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 14,\n    fontWeight: 400,\n}))\n\nconst ExampleEditTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: \"#5d64cf\",\n    fontFamily: \"'Work Sans', sans-serif\",\n    fontSize: 14,\n    fontWeight: 400,\n}));\n\nconst ExampleAccordionSummary = styled((props: AccordionSummaryProps) => (\n    <MuiAccordionSummary\n        expandIcon={<LabelIcon fontSize=\"small\" color=\"primary\" />}\n        {...props}\n    />\n))(({ theme }) => ({\n    flexDirection: 'row-reverse',\n    '& .MuiAccordionSummary-expandIconWrapper.Mui-expanded': {\n        transform: 'rotate(0deg)',\n    },\n}));\n\n\nclass WSEditorCommandContent extends React.Component<WSEditorCommandContentProps, WSEditorCommandContentState> {\n\n    constructor(props: WSEditorCommandContentProps) {\n        super(props);\n        this.state = {\n            command: undefined,\n            displayCommandDialog: false,\n            displayExampleDialog: false,\n            displayCommandDeleteDialog: false,\n            displayAddSubcommandDialog: false,\n            loading: false,\n        }\n    }\n\n    loadCommand = async () => {\n        this.setState({ loading: true })\n        let { workspaceUrl, previewCommand } = this.props\n        let commandNames = previewCommand.names;\n        const leafUrl = `${workspaceUrl}/CommandTree/Nodes/aaz/` + commandNames.slice(0, -1).join('/') + '/Leaves/' + commandNames[commandNames.length - 1];\n        try {\n            let res = await axios.get(leafUrl);\n            let command = DecodeResponseCommand(res.data);\n            if (command.id === this.props.previewCommand.id) {\n                this.setState({\n                    loading: false,\n                    command: command\n                })\n            }\n        } catch (err: any) {\n            this.setState({ loading: false })\n            console.error(err)\n            return\n        }\n    }\n\n    componentDidMount() {\n        this.loadCommand();\n    }\n\n    componentDidUpdate(prevProps: WSEditorCommandContentProps) {\n        if (prevProps.workspaceUrl !== this.props.workspaceUrl || prevProps.previewCommand.id !== this.props.previewCommand.id || prevProps.reloadTimestamp !== this.props.reloadTimestamp) {\n            if (prevProps.previewCommand.id !== this.props.previewCommand.id) {\n                this.setState({ command: undefined })\n            }\n            this.loadCommand();\n        }\n    }\n\n    onCommandDialogDisplay = () => {\n        this.setState({\n            displayCommandDialog: true,\n        })\n    }\n\n    onCommandDeleteDialogDisplay = () => {\n        this.setState({\n            displayCommandDeleteDialog: true,\n        })\n    }\n\n    handleCommandDialogClose = (newCommand?: Command) => {\n        if (newCommand) {\n            this.props.onUpdateCommand(newCommand!);\n        }\n        this.setState({\n            displayCommandDialog: false,\n        })\n    }\n\n    handleCommandDeleteDialogClose = (deleted: boolean) => {\n        if (deleted) {\n            this.props.onUpdateCommand(null);\n        }\n        this.setState({\n            displayCommandDeleteDialog: false,\n        })\n    }\n\n    onExampleDialogDisplay = (idx?: number) => {\n        this.setState({\n            displayExampleDialog: true,\n            exampleIdx: idx,\n        })\n    }\n\n    handleExampleDialogClose = (newCommand?: Command) => {\n        if (newCommand) {\n            this.props.onUpdateCommand(newCommand!);\n        }\n        this.setState({\n            displayExampleDialog: false,\n        })\n    }\n\n    onAddSubcommandDialogDisplay = (argVar: string, subArgOptions: { var: string, options: string }[], argStackNames: string[]) => {\n        this.setState({\n            displayAddSubcommandDialog: true,\n            subcommandArgVar: argVar,\n            subcommandSubArgOptions: subArgOptions,\n            subcommandDefaultGroupNames: [...this.props.previewCommand.names.slice(0, -1), ...argStackNames],\n        })\n    }\n\n    handleAddSubcommandDisplayClose = (add: boolean) => {\n        if (add) {\n            this.props.onUpdateCommand(this.state.command!);\n        }\n        this.setState({\n            displayAddSubcommandDialog: false,\n            subcommandArgVar: undefined,\n            subcommandDefaultGroupNames: undefined\n        })\n    }\n\n    render() {\n        const { workspaceUrl, previewCommand } = this.props;\n        const commandNames = previewCommand.names;\n        const name = commandPrefix + commandNames.join(' ');\n        const commandUrl = `${workspaceUrl}/CommandTree/Nodes/aaz/` + commandNames.slice(0, -1).join('/') + '/Leaves/' + commandNames[commandNames.length - 1];\n\n        const { command, displayCommandDialog, displayExampleDialog, displayCommandDeleteDialog, displayAddSubcommandDialog, exampleIdx, loading } = this.state;\n\n        const buildExampleView = (example: Example, idx: number) => {\n            const buildCommand = (exampleCommand: string, cmdIdx: number) => {\n                return (<Box key={`example-${idx}-command-${cmdIdx}`} sx={{\n                    display: \"flex\",\n                    flexDirection: 'row',\n                    alignItems: 'flex-start',\n                    justifyContent: 'flex-start',\n                }}>\n                    <Box component=\"span\" sx={{\n                        flexShrink: 0,\n                        display: \"flex\",\n                        flexDirection: 'row', alignItems: 'center', justifyContent: 'flex-start',\n                    }}>\n                        <KeyboardDoubleArrowRightIcon fontSize=\"small\" />\n                        <ExampleCommandHeaderTypography sx={{ flexShrink: 0 }}>{commandPrefix}</ExampleCommandHeaderTypography>\n                    </Box>\n                    <Box component=\"span\" sx={{\n                        ml: 0.8,\n                    }}>\n                        <ExampleCommandBodyTypography>{exampleCommand}</ExampleCommandBodyTypography>\n                    </Box>\n                </Box>)\n            }\n            return (\n                <Accordion\n                    elevation={0}\n                    expanded\n                    key={`example-${idx}`}\n                    onDoubleClick={() => { this.onExampleDialogDisplay(idx) }}\n                >\n                    <ExampleAccordionSummary\n                        id={`example-${idx}-header`}\n                    >\n                        <Box sx={{\n                            ml: 1,\n                            flexGrow: 1,\n                            display: \"flex\",\n                            flexDirection: \"row\",\n                            alignItems: \"center\",\n                        }}>\n                            <SubtitleTypography sx={{ flexShrink: 0 }} >{example.name}</SubtitleTypography>\n                            {/* <Box sx={{ flexGrow: 1 }} /> */}\n                            <Button sx={{ flexShrink: 0, ml: 3 }}\n                                startIcon={<EditIcon color=\"secondary\" fontSize='small' />}\n                                onClick={() => { this.onExampleDialogDisplay(idx) }}\n                            >\n                                <ExampleEditTypography>Edit</ExampleEditTypography>\n                            </Button>\n                        </Box>\n                    </ExampleAccordionSummary>\n                    <AccordionDetails sx={{\n                        display: 'flex',\n                        flexDirection: 'column',\n                        alignItems: 'stretch',\n                        justifyContent: 'flex-start',\n                        ml: 3,\n                        mr: 3,\n                        paddingTop: 0,\n                    }}>\n                        {example.commands.map(buildCommand)}\n                    </AccordionDetails>\n                </Accordion>\n            )\n        }\n\n        const buildCommandCard = () => {\n            const shortHelp = (command ?? previewCommand).help?.short;\n            const longHelp = (command ?? previewCommand).help?.lines?.join('\\n');\n            const lines: string[] = (command ?? previewCommand).help?.lines ?? [];\n            const stage = (command ?? previewCommand).stage;\n            const version = (command ?? previewCommand).version;\n\n            return (<Card\n                onDoubleClick={this.onCommandDialogDisplay}\n                elevation={3}\n                sx={{\n                    flexGrow: 1,\n                    display: 'flex',\n                    flexDirection: 'column',\n                    p: 2\n                }}>\n                <CardContent sx={{\n                    flex: '1 0 auto',\n                    display: 'flex',\n                    flexDirection: 'column',\n                    justifyContent: 'stretch',\n                }}>\n                    <Box sx={{\n                        mb: 2,\n                        display: 'flex',\n                        flexDirection: 'row',\n                        alignItems: \"center\"\n                    }}>\n                        <CardTitleTypography sx={{ flexShrink: 0 }}>\n                            [ COMMAND ]\n                        </CardTitleTypography>\n                        <Box sx={{ flexGrow: 1 }} />\n                        {stage === \"Stable\" && <StableTypography\n                            sx={{ flexShrink: 0 }}\n                        >\n                            {`v${version}`}\n                        </StableTypography>}\n                        {stage === \"Preview\" && <PreviewTypography\n                            sx={{ flexShrink: 0 }}\n                        >\n                            {`v${version}`}\n                        </PreviewTypography>}\n                        {stage === \"Experimental\" && <ExperimentalTypography\n                            sx={{ flexShrink: 0 }}\n                        >\n                            {`v${version}`}\n                        </ExperimentalTypography>}\n                    </Box>\n\n                    <NameTypography sx={{ mt: 1 }}>\n                        {name}\n                    </NameTypography>\n                    {shortHelp && <ShortHelpTypography sx={{ ml: 6, mt: 2 }}> {shortHelp} </ShortHelpTypography>}\n                    {!shortHelp && <ShortHelpPlaceHolderTypography sx={{ ml: 6, mt: 2 }}>Please add command short summary!</ShortHelpPlaceHolderTypography>}\n                    {longHelp && <Box sx={{ ml: 6, mt: 1, mb: 1 }}>\n                        {lines.map((line, idx) => (<LongHelpTypography key={idx}>{line}</LongHelpTypography>))}\n                    </Box>}\n                </CardContent>\n                <CardActions sx={{\n                    display: \"flex\",\n                    flexDirection: \"row-reverse\",\n                    alignContent: \"center\",\n                    justifyContent: \"flex-start\"\n                }}>\n                    {loading && <Box sx={{ width: '100%' }}>\n                        <LinearProgress color='secondary' />\n                    </Box>}\n                    {!loading && <Box sx={{\n                        display: \"flex\",\n                        flexDirection: \"row\",\n                        alignContent: \"center\",\n                        justifyContent: \"flex-start\"\n                    }}>\n\n                        <Button\n                            variant='contained' size=\"small\" color='secondary' disableElevation\n                            onClick={this.onCommandDialogDisplay}\n                            disabled={loading}\n                            sx={{ mr: 2 }}\n                        >\n                            <Typography variant='body2'>\n                                Edit\n                            </Typography>\n                        </Button>\n                        <Button\n                            variant='outlined' size=\"small\" color='secondary'\n                            onClick={this.onCommandDeleteDialogDisplay}\n                            disabled={loading}\n                            sx={{ mr: 2 }}\n                        >\n                            <Typography variant='body2'>\n                                Delete\n                            </Typography>\n                        </Button>\n                        <Button\n                            variant='outlined' size=\"small\" color='secondary'\n                            sx={{ mr: 2 }}\n                            disabled\n                        >\n                            <Typography variant='body2'>\n                                Try\n                            </Typography>\n                        </Button>\n                    </Box>}\n                </CardActions>\n            </Card>)\n        }\n\n        const buildArgumentsCard = () => {\n            return (<Card\n                elevation={3}\n                sx={{\n                    flexGrow: 1,\n                    display: 'flex',\n                    flexDirection: 'column',\n                    mt: 1,\n                    p: 2\n                }}>\n                <WSEditorCommandArgumentsContent commandUrl={commandUrl} args={command!.args!} clsArgDefineMap={command!.clsArgDefineMap!} onReloadArgs={this.loadCommand} onAddSubCommand={this.onAddSubcommandDialogDisplay} />\n            </Card>)\n        }\n\n        const buildExampleCard = () => {\n            const examples = command!.examples ?? []\n            return (<Card\n                elevation={3}\n                sx={{\n                    flexGrow: 1,\n                    display: 'flex',\n                    flexDirection: 'column',\n                    mt: 1,\n                    p: 2\n                }}>\n\n                <CardContent sx={{\n                    flex: '1 0 auto',\n                    display: 'flex',\n                    flexDirection: 'column',\n                    alignItems: 'stretch',\n                }}>\n                    <Box sx={{\n                        mb: 2,\n                        display: 'flex',\n                        flexDirection: 'row',\n                        alignItems: \"center\"\n                    }}>\n                        <CardTitleTypography sx={{ flexShrink: 0 }}>\n                            [ EXAMPLE ]\n                        </CardTitleTypography>\n\n                    </Box>\n                    {examples.length > 0 && <Box>\n                        {examples.map(buildExampleView)}\n                    </Box>}\n                </CardContent>\n\n                <CardActions sx={{\n                    display: \"flex\",\n                    flexDirection: \"row-reverse\",\n                }}>\n                    <Button\n                        variant='contained' size=\"small\" color='secondary' disableElevation\n                        onClick={() => this.onExampleDialogDisplay(undefined)}\n                    >\n                        <Typography variant='body2'>\n                            Add\n                        </Typography>\n                    </Button>\n                </CardActions>\n            </Card>)\n        }\n\n        return (\n            <React.Fragment>\n                <Box sx={{\n                    display: 'flex',\n                    flexDirection: 'column',\n                    alignItems: 'stretch',\n                }}>\n                    {buildCommandCard()}\n                    {command !== undefined && command.args !== undefined && buildArgumentsCard()}\n                    {command !== undefined && buildExampleCard()}\n                </Box>\n                {command !== undefined && displayCommandDialog && <CommandDialog open={displayCommandDialog} workspaceUrl={workspaceUrl} command={command!} onClose={this.handleCommandDialogClose} />}\n                {command !== undefined && displayExampleDialog && <ExampleDialog open={displayExampleDialog} workspaceUrl={workspaceUrl} command={command!} idx={exampleIdx} onClose={this.handleExampleDialogClose} />}\n                {command !== undefined && displayCommandDeleteDialog && <CommandDeleteDialog open={displayCommandDeleteDialog} workspaceUrl={workspaceUrl} command={command!} onClose={this.handleCommandDeleteDialogClose} />}\n                {command !== undefined && displayAddSubcommandDialog && <AddSubcommandDialog open={displayAddSubcommandDialog} workspaceUrl={workspaceUrl} command={command!} onClose={this.handleAddSubcommandDisplayClose} argVar={this.state.subcommandArgVar!} subArgOptions={this.state.subcommandSubArgOptions!} defaultGroupNames={this.state.subcommandDefaultGroupNames!} />}\n            </React.Fragment>\n        )\n    }\n}\n\n\nfunction CommandDeleteDialog(props: {\n    workspaceUrl: string,\n    open: boolean,\n    command: Command,\n    onClose: (deleted: boolean) => void\n}) {\n    const [updating, setUpdating] = React.useState<boolean>(false);\n    const [relatedCommands, setRelatedCommands] = React.useState<string[]>([]);\n\n    const getUrls = () => {\n        let urls: string[] = [];\n\n        props.command.resources.forEach(resource => {\n            const resourceId = btoa(resource.id)\n            const version = btoa(resource.version)\n            if (resource.subresource !== undefined) {\n                let subresource = btoa(resource.subresource)\n                // TODO: delete list command together with crud\n                // if (resource.subresource.endsWith('[]') || resource.subresource.endsWith('{}')) {\n                //     let subresource2 = btoa(resource.subresource.slice(0, -2))\n                //     urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources/${subresource2}`)\n                // } else {\n                //     let subresource2 = btoa(resource.subresource + '[]');\n                //     urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources/${subresource2}`)\n                //     subresource2 = btoa(resource.subresource + '{}');\n                //     urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources/${subresource2}`)\n                // }\n                urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources/${subresource}`)\n            } else {\n                urls.push(`${props.workspaceUrl}/Resources/${resourceId}/V/${version}`)\n            }\n        })\n        return urls;\n    }\n\n    React.useEffect(() => {\n        setRelatedCommands([]);\n        const urls = getUrls();\n        const promisesAll = urls.map(url => {\n            return axios.get(`${url}/Commands`)\n        })\n        Promise.all(promisesAll)\n            .then(responses => {\n                const commands = new Set<string>();\n                responses.forEach((response: any) => {\n                    const responseCommands: ResponseCommand[] = response.data\n                    responseCommands\n                        .map(responseCommand => DecodeResponseCommand(responseCommand))\n                        .forEach(cmd => { commands.add(cmd.names.join(\" \")) });\n                });\n\n                const cmdNames: string[] = [];\n                commands.forEach(cmdName => cmdNames.push(cmdName));\n                cmdNames.sort((a, b) => a.localeCompare(b));\n                setRelatedCommands(cmdNames);\n            })\n            .catch(err => {\n                console.error(err.response)\n            })\n\n    }, [props.command]);\n\n    const handleClose = () => {\n        props.onClose(false);\n    }\n    const handleDelete = () => {\n        setUpdating(true);\n        const urls = getUrls();\n        const promisesAll = urls.map(url => {\n            return axios.delete(url)\n        })\n        Promise.all(promisesAll)\n            .then(res => {\n                setUpdating(false);\n                props.onClose(true);\n            })\n            .catch(err => {\n                setUpdating(false);\n                console.error(err.response)\n            })\n    }\n    return (\n        <Dialog\n            disableEscapeKeyDown\n            open={props.open}\n        >\n            <DialogTitle>Delete Commands</DialogTitle>\n            <DialogContent dividers={true}>\n                {relatedCommands.map((command, idx) => (\n                    <Typography key={`command-${idx}`} variant=\"body2\">{`${commandPrefix}${command}`}</Typography>\n                ))}\n            </DialogContent>\n            <DialogActions>\n                {updating &&\n                    <Box sx={{ width: '100%' }}>\n                        <LinearProgress color='secondary' />\n                    </Box>\n                }\n                {!updating && <React.Fragment>\n                    <Button onClick={handleClose}>Cancel</Button>\n                    <Button onClick={handleDelete}>Delete</Button>\n                </React.Fragment>}\n            </DialogActions>\n\n        </Dialog>\n    )\n}\n\ninterface CommandDialogProps {\n    workspaceUrl: string,\n    open: boolean\n    command: Command\n    onClose: (newCommand?: Command) => void\n}\n\ninterface CommandDialogState {\n    name: string,\n    stage: string,\n    shortHelp: string,\n    longHelp: string,\n    invalidText?: string,\n    confirmation: string,\n    updating: boolean\n}\n\n\nclass CommandDialog extends React.Component<CommandDialogProps, CommandDialogState> {\n\n    constructor(props: CommandDialogProps) {\n        super(props);\n        this.state = {\n            name: this.props.command.names.join(' '),\n            shortHelp: this.props.command.help?.short ?? \"\",\n            longHelp: this.props.command.help?.lines?.join('\\n') ?? \"\",\n            stage: this.props.command.stage,\n            confirmation: this.props.command.confirmation ?? \"\",\n            updating: false\n        }\n    }\n\n    handleModify = (event: any) => {\n        let { name, stage, shortHelp, longHelp, confirmation } = this.state\n        let { workspaceUrl, command } = this.props\n\n        name = name.trim();\n        shortHelp = shortHelp.trim();\n        longHelp = longHelp.trim();\n        confirmation = confirmation.trim();\n\n        const names = name.split(' ').filter(n => n.length > 0);\n\n        this.setState({\n            invalidText: undefined\n        })\n\n        if (names.length < 1) {\n            this.setState({\n                invalidText: `Field 'Name' is required.`\n            })\n            return\n        }\n\n        for (const idx in names) {\n            const piece = names[idx];\n            if (!/^[a-z0-9]+(-[a-z0-9]+)*$/.test(piece)) {\n                this.setState({\n                    invalidText: `Invalid Name part: '${piece}'. Supported regular expression is: [a-z0-9]+(-[a-z0-9]+)* `\n                })\n                return\n            }\n        }\n\n        if (shortHelp.length < 1) {\n            this.setState({\n                invalidText: `Field 'Short Summary' is required.`\n            })\n            return\n        }\n\n        let lines: string[] | null = null;\n        if (longHelp.length > 1) {\n            lines = longHelp.split('\\n').filter(l => l.length > 0);\n        }\n\n        this.setState({\n            updating: true,\n        })\n\n        const leafUrl = `${workspaceUrl}/CommandTree/Nodes/aaz/` + command.names.slice(0, -1).join('/') + '/Leaves/' + command.names[command.names.length - 1];\n\n        axios.patch(leafUrl, {\n            help: {\n                short: shortHelp,\n                lines: lines,\n            },\n            stage: stage,\n            confirmation: confirmation,\n        }).then(res => {\n            const name = names.join(' ');\n            if (name === command.names.join(' ')) {\n                const cmd = DecodeResponseCommand(res.data);\n                this.setState({\n                    updating: false,\n                })\n                this.props.onClose(cmd);\n            } else {\n                // Rename command\n                axios.post(`${leafUrl}/Rename`, {\n                    name: name\n                }).then(res => {\n                    const cmd = DecodeResponseCommand(res.data);\n                    this.setState({\n                        updating: false,\n                    })\n                    this.props.onClose(cmd);\n                })\n            }\n        }).catch(err => {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                this.setState({\n                    invalidText: `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`,\n                })\n            }\n            this.setState({\n                updating: false,\n            })\n        });\n    }\n\n    handleClose = () => {\n        this.setState({\n            invalidText: undefined\n        });\n        this.props.onClose();\n    }\n\n    render() {\n        const { name, shortHelp, longHelp, invalidText, updating, stage, confirmation } = this.state;\n        return (\n            <Dialog\n                disableEscapeKeyDown\n                open={this.props.open}\n                sx={{ '& .MuiDialog-paper': { width: '80%' } }}\n            >\n                <DialogTitle>Command</DialogTitle>\n                <DialogContent dividers={true}>\n                    {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n                    <InputLabel required shrink sx={{ font: \"inherit\" }}>Stage</InputLabel>\n                    <RadioGroup\n                        row\n                        value={stage}\n                        name=\"stage\"\n                        onChange={(event: any) => {\n                            this.setState({\n                                stage: event.target.value,\n                            })\n                        }}\n                    >\n                        <FormControlLabel value=\"Stable\" control={<Radio />} label=\"Stable\" sx={{ ml: 4 }} />\n                        <FormControlLabel value=\"Preview\" control={<Radio />} label=\"Preview\" sx={{ ml: 4 }} />\n                        <FormControlLabel value=\"Experimental\" control={<Radio />} label=\"Experimental\" sx={{ ml: 4 }} />\n                    </RadioGroup>\n\n                    <TextField\n                        id=\"name\"\n                        label=\"Name\"\n                        type=\"text\"\n                        fullWidth\n                        variant='standard'\n                        value={name}\n                        onChange={(event: any) => {\n                            this.setState({\n                                name: event.target.value,\n                            })\n                        }}\n                        margin=\"normal\"\n                        required\n                    />\n                    <TextField\n                        id=\"shortSummary\"\n                        label=\"Short Summary\"\n                        type=\"text\"\n                        fullWidth\n                        variant='standard'\n                        value={shortHelp}\n                        onChange={(event: any) => {\n                            this.setState({\n                                shortHelp: event.target.value,\n                            })\n                        }}\n                        margin=\"normal\"\n                        required\n                    />\n                    <TextField\n                        id=\"longSummary\"\n                        label=\"Long Summary\"\n                        helperText=\"Please add long summer in lines.\"\n                        type=\"text\"\n                        fullWidth\n                        multiline\n                        variant='standard'\n                        value={longHelp}\n                        onChange={(event: any) => {\n                            this.setState({\n                                longHelp: event.target.value,\n                            })\n                        }}\n                        margin=\"normal\"\n                    />\n                    <TextField\n                        id=\"confirmation\"\n                        label=\"Command confirmation\"\n                        helperText=\"Modify or clear confirmation message as needed.\"\n                        type=\"text\"\n                        fullWidth\n                        multiline\n                        variant='standard'\n                        value={confirmation}\n                        onChange={(event: any) => {\n                            this.setState({\n                                confirmation: event.target.value,\n                            })\n                        }}\n                        margin=\"normal\"\n                    />\n                </DialogContent>\n                <DialogActions>\n                    {updating &&\n                        <Box sx={{ width: '100%' }}>\n                            <LinearProgress color='secondary' />\n                        </Box>\n                    }\n                    {!updating && <React.Fragment>\n                        <Button onClick={this.handleClose}>Cancel</Button>\n                        <Button onClick={this.handleModify}>Save</Button>\n                    </React.Fragment>}\n                </DialogActions>\n            </Dialog>\n        )\n    }\n}\n\n// function CommandDeleteDialog\n\ninterface ExampleDialogProps {\n    workspaceUrl: string\n    open: boolean\n    command: Command\n    idx?: number\n    onClose: (newCommand?: Command) => void\n}\n\ninterface ExampleDialogState {\n    name: string\n    exampleCommands: string[]\n    isAdd: boolean\n    invalidText?: string\n    updating: boolean\n    source?: string\n    exampleOptions: Example[]\n}\n\nconst ExampleCommandTypography = styled(Typography)<TypographyProps>(({ theme }) => ({\n    color: theme.palette.primary.main,\n    fontFamily: \"'Roboto Condensed', sans-serif\",\n    fontSize: 16,\n    fontWeight: 400,\n}))\n\nclass ExampleDialog extends React.Component<ExampleDialogProps, ExampleDialogState> {\n\n    constructor(props: ExampleDialogProps) {\n        super(props);\n        const examples: Example[] = this.props.command.examples ?? [];\n        if (this.props.idx === undefined) {\n            this.state = {\n                name: \"\",\n                exampleCommands: [\"\",],\n                isAdd: true,\n                invalidText: undefined,\n                updating: false,\n                source: undefined,\n                exampleOptions: [],\n            }\n        } else {\n            const example = examples[this.props.idx];\n            this.state = {\n                name: example.name,\n                exampleCommands: example.commands,\n                isAdd: false,\n                invalidText: undefined,\n                updating: false,\n                source: undefined,\n                exampleOptions: [],\n            }\n        }\n    }\n\n    onUpdateExamples = (examples: Example[]) => {\n        let { workspaceUrl, command } = this.props;\n\n        const leafUrl = `${workspaceUrl}/CommandTree/Nodes/aaz/` + command.names.slice(0, -1).join('/') + '/Leaves/' + command.names[command.names.length - 1];\n\n        this.setState({\n            updating: true,\n        })\n        axios.patch(leafUrl, {\n            examples: examples\n        }).then(res => {\n            const cmd = DecodeResponseCommand(res.data);\n            this.setState({\n                updating: false,\n            })\n            this.props.onClose(cmd);\n        }).catch(err => {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                this.setState({\n                    invalidText: `ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`,\n                })\n            }\n            this.setState({\n                updating: false,\n            })\n        });\n    }\n\n    handleDelete = () => {\n        let { command } = this.props;\n        let examples: Example[] = command.examples ?? [];\n        let idx = this.props.idx!;\n        examples = [...examples.slice(0, idx), ...examples.slice(idx + 1)];\n        this.onUpdateExamples(examples);\n    }\n\n    handleModify = () => {\n        let { command } = this.props;\n        let { name, exampleCommands } = this.state;\n        let examples: Example[] = command.examples ?? [];\n        let idx = this.props.idx!;\n\n        name = name.trim();\n        if (name.length < 1) {\n            this.setState({\n                invalidText: `Field 'Name' is required.`\n            })\n            return\n        }\n        exampleCommands = exampleCommands.map(cmd => {\n            return cmd.split('\\n')\n                .map(cmdLine => cmdLine.trim())\n                .filter(cmdLine => cmdLine.length > 0)\n                .join(' ')\n                .trim();\n        }).filter(cmd => cmd.length > 0);\n\n        if (exampleCommands.length < 1) {\n            this.setState({\n                invalidText: `Field 'Commands' is required.`\n            })\n            return\n        }\n\n        const newExample: Example = {\n            name: name,\n            commands: exampleCommands\n        }\n\n        examples = [...examples.slice(0, idx), newExample, ...examples.slice(idx + 1)];\n\n        this.onUpdateExamples(examples);\n    }\n\n    handleAdd = () => {\n        let { command } = this.props;\n        let { name, exampleCommands } = this.state;\n        let examples: Example[] = command.examples ?? [];\n\n        name = name.trim();\n        if (name.length < 1) {\n            this.setState({\n                invalidText: `Field 'Name' is required.`\n            })\n            return\n        }\n        exampleCommands = exampleCommands.map(cmd => {\n            return cmd.split('\\n')\n                .map(cmdLine => cmdLine.trim())\n                .filter(cmdLine => cmdLine.length > 0)\n                .join(' ')\n                .trim();\n        }).filter(cmd => cmd.length > 0);\n\n        if (exampleCommands.length < 1) {\n            this.setState({\n                invalidText: `Field 'Commands' is required.`\n            })\n            return\n        }\n\n        const newExample: Example = {\n            name: name,\n            commands: exampleCommands\n        }\n        examples.push(newExample);\n\n        this.onUpdateExamples(examples);\n    }\n\n    handleClose = () => {\n        this.setState({\n            invalidText: undefined\n        });\n        this.props.onClose()\n    }\n\n    onModifyExampleCommand = (cmd: string, idx: number) => {\n        this.setState(preState => {\n            return {\n                ...preState,\n                exampleCommands: [...preState.exampleCommands.slice(0, idx), cmd, ...preState.exampleCommands.slice(idx + 1)]\n            }\n        })\n    }\n\n    onRemoveExampleCommand = (idx: number) => {\n        this.setState(preState => {\n            let exampleCommands: string[] = [...preState.exampleCommands.slice(0, idx), ...preState.exampleCommands.slice(idx + 1)];\n            if (exampleCommands.length === 0) {\n                exampleCommands.push(\"\");\n            }\n            return {\n                ...preState,\n                exampleCommands: exampleCommands,\n            }\n        })\n    }\n\n    onAddExampleCommand = () => {\n        this.setState(preState => {\n            return {\n                ...preState,\n                exampleCommands: [...preState.exampleCommands, \"\"]\n            }\n        })\n    }\n\n    loadSwaggerExamples = async () => {\n        try {\n            let { workspaceUrl, command } = this.props;\n\n            const leafUrl = `${workspaceUrl}/CommandTree/Nodes/aaz/` + command.names.slice(0, -1).join('/') + '/Leaves/' + command.names[command.names.length - 1] + '/GenerateExamples';\n\n            this.setState({\n                source: \"swagger\",\n                updating: true,\n            })\n            let res = await axios.post(leafUrl, {\n                source: \"swagger\"\n            })\n\n            const examples: Example[] = res.data.map((v: any) => {\n                return {\n                    name: v.name,\n                    commands: v.commands\n                }\n            })\n            this.setState({\n                exampleOptions: examples,\n                updating: false\n            })\n            if (examples.length > 0) {\n                this.onExampleSelectorUpdate(examples[0].name);\n            }\n        } catch (err: any) {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                this.setState({\n                    updating: false,\n                    invalidText: `ResponseError: ${data.message!}`,\n                })\n            }\n        }\n    }\n\n    onExampleSelectorUpdate = (exampleDisplayName: string | null) => {\n        let example = this.state.exampleOptions.find((v) => v.name === exampleDisplayName) ?? undefined;\n\n        if (example === undefined) {\n            this.setState({\n                name: exampleDisplayName ?? \"\",\n            })\n        } else {\n            this.setState({\n                name: example?.name ?? \"\",\n                exampleCommands: example?.commands ?? [\"\",],\n            })\n        }\n    }\n\n    render() {\n        const { name, exampleCommands, isAdd, invalidText, updating, source, exampleOptions } = this.state;\n\n        const selectedName = name\n\n        const buildExampleInput = (cmd: string, idx: number) => {\n            return (\n                <Box key={idx} sx={{\n                    display: 'flex',\n                    flexDirection: 'row',\n                    alignItems: 'center',\n                    justifyContent: 'flex-start',\n                    ml: 1,\n                }}>\n                    <IconButton\n                        edge=\"start\"\n                        color=\"inherit\"\n                        onClick={() => this.onRemoveExampleCommand(idx)}\n                        aria-label=\"remove\"\n                    >\n                        <DoDisturbOnRoundedIcon fontSize=\"small\" />\n                    </IconButton>\n                    <Input\n                        id={`command-${idx}`}\n                        multiline\n                        value={cmd}\n                        onChange={(event: any) => {\n                            this.onModifyExampleCommand(event.target.value, idx)\n                        }}\n                        sx={{ flexGrow: 1 }}\n                        placeholder=\"Input a command here.\"\n                        startAdornment={\n                            <InputAdornment position=\"start\">\n                                <ExampleCommandTypography>{commandPrefix}</ExampleCommandTypography>\n                            </InputAdornment>\n                        }\n                    />\n                </Box>\n            );\n        }\n\n        return (\n            <Dialog\n                disableEscapeKeyDown\n                open={this.props.open}\n                sx={{ '& .MuiDialog-paper': { width: '80%' } }}\n            >\n                <DialogTitle>\n                    {isAdd ? \"Add Example\" : \"Modify Example\"}\n                    <IconButton style={{ position: \"absolute\", right: 16, top: 8}} edge=\"end\" color=\"inherit\" onClick={this.handleClose} aria-label=\"close\">\n                        <CloseIcon />\n                    </IconButton>\n                </DialogTitle>\n                <DialogContent dividers={true}>\n                    {isAdd && source === undefined &&\n                        <Stack direction=\"column\" spacing={2}>\n                            <Button variant='contained' size=\"large\" color='secondary' sx={{ fontSize: '20px', padding: '10px 20px' }} onClick={() => {this.loadSwaggerExamples()}}>\n                                <Typography variant='body2'>By OpenAPI Specification</Typography>\n                            </Button>\n                            {/* <Button variant='outlined' size=\"large\" color='secondary' sx={{ fontSize: '20px', padding: '10px 20px' }} disabled>\n                                <Typography variant='body2'>By Testing Record</Typography>\n                            </Button>\n                            <Button variant='outlined' size=\"large\" color='secondary' sx={{ fontSize: '20px', padding: '10px 20px' }} disabled>\n                                <Typography variant='body2'>By Request Payload</Typography>\n                            </Button> */}\n                        </Stack>\n                    }\n                    {(!isAdd || source != undefined) &&\n                        <React.Fragment>\n                            {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n                            {!isAdd &&\n                                <React.Fragment>\n                                    <TextField\n                                        id=\"name\"\n                                        label=\"Name\"\n                                        type=\"text\"\n                                        fullWidth\n                                        variant='standard'\n                                        value={name}\n                                        onChange={(event: any) => {\n                                            this.setState({\n                                                name: event.target.value,\n                                            })\n                                        }}\n                                        margin=\"normal\"\n                                        required\n                                    />\n                                </React.Fragment>\n                            }\n                            {source === \"swagger\" && \n                                <React.Fragment>\n                                    <ExampleItemSelector\n                                        name=\"Name\"\n                                        commonPrefix={\"\"}\n                                        options={exampleOptions.map((v: any) => v.name)}\n                                        value={selectedName}\n                                        onValueUpdate={this.onExampleSelectorUpdate}\n                                    />\n                                </React.Fragment>\n                            }\n                            <InputLabel required sx={{ font: \"inherit\", mt: 1 }}>Commands</InputLabel>\n                            {exampleCommands.map(buildExampleInput)}\n                            <Box sx={{\n                                display: 'flex',\n                                flexDirection: 'row',\n                                alignItems: 'center',\n                                justifyContent: 'flex-start',\n                                ml: 1,\n                            }}>\n                                <IconButton\n                                    edge=\"start\"\n                                    color=\"inherit\"\n                                    onClick={this.onAddExampleCommand}\n                                    aria-label=\"add\"\n                                >\n                                    <AddCircleRoundedIcon fontSize=\"small\" />\n                                </IconButton>\n                                <ExampleCommandTypography sx={{ flexShrink: 0 }}> One more command</ExampleCommandTypography>\n                            </Box>\n                        </React.Fragment>\n                    }\n                </DialogContent>\n                {(!isAdd || source != undefined) &&\n                <DialogActions>\n                    {updating &&\n                        <Box sx={{ width: '100%' }}>\n                            <LinearProgress color='secondary' />\n                        </Box>\n                    }\n                    {!updating && <React.Fragment>\n                        {!isAdd && <React.Fragment>\n                            <Button onClick={this.handleDelete}>Delete</Button>\n                            <Button onClick={this.handleModify}>Save</Button>\n                        </React.Fragment>}\n                        {isAdd && <Button onClick={this.handleAdd}>Add</Button>}\n                    </React.Fragment>}\n                </DialogActions>}\n            </Dialog>\n        )\n    }\n}\n\nfunction AddSubcommandDialog(props: {\n    workspaceUrl: string,\n    command: Command,\n    argVar: string,\n    subArgOptions: { var: string, options: string }[],\n    defaultGroupNames: string[],\n    open: boolean,\n    onClose: (added: boolean) => void,\n}) {\n\n    const [updating, setUpdating] = useState<boolean>(false);\n    const [invalidText, setInvalidText] = useState<string | undefined>(undefined);\n    const [commandGroupName, setCommandGroupName] = useState<string>(\"\");\n    const [refArgsOptions, setRefArgsOptions] = useState<{ var: string, options: string }[]>([]);\n\n    useEffect(() => {\n        setCommandGroupName(props.defaultGroupNames.join(' '));\n        setRefArgsOptions(props.subArgOptions);\n    }, [props.argVar, props.defaultGroupNames]);\n\n    const handleClose = () => {\n        setInvalidText(undefined);\n        props.onClose(false);\n    }\n\n    const verifyAddSubresource = () => {\n        setInvalidText(undefined);\n        const argOptions: { [argVar: string]: string[] } = {}\n        let invalidText: string | undefined = undefined;\n        refArgsOptions.forEach((arg, idx) => {\n            const names = arg.options.split(' ').filter(n => n.length > 0);\n            if (names.length < 1) {\n                invalidText = `Prop ${idx + 1} option name is required.`\n                return undefined\n            }\n\n            for (const idx in names) {\n                const piece = names[idx];\n                if (!/^[a-z0-9]+(-[a-z0-9]+)*$/.test(piece)) {\n                    invalidText = `Invalid 'Prop ${idx + 1} option name': '${piece}'. Supported regular expression is: [a-z0-9]+(-[a-z0-9]+)* `\n                    return undefined\n                }\n            }\n            argOptions[arg.var] = names;\n        });\n\n        const names = commandGroupName.split(' ').filter(n => n.length > 0);\n        if (names.length < 1) {\n            invalidText = 'Invalid Command group name';\n            return\n        }\n\n        if (invalidText !== undefined) {\n            setInvalidText(invalidText);\n            return undefined\n        }\n\n        return {\n            commandGroupName: names.join(' '),\n            refArgsOptions: argOptions,\n        }\n    }\n\n    const handleAddSubresource = async () => {\n        const urls = props.command.resources.map(resource => {\n            const resourceId = btoa(resource.id)\n            const version = btoa(resource.version)\n            return `${props.workspaceUrl}/Resources/${resourceId}/V/${version}/Subresources`\n        })\n\n        if (urls.length !== 1) {\n            setInvalidText(`Cannot create subcommands, command contains ${props.command.resources.length} resources`);\n            return;\n        }\n\n        const data = verifyAddSubresource();\n        if (data === undefined) {\n            return;\n        }\n\n        setUpdating(true);\n\n        try {\n            await axios.post(urls[0], {\n                ...data,\n                arg: props.argVar,\n            })\n            props.onClose(true);\n        } catch (err: any) {\n            console.error(err.response);\n            if (err.response?.data?.message) {\n                const data = err.response!.data!;\n                setInvalidText(`ResponseError: ${data.message!}: ${JSON.stringify(data.details)}`);\n            }\n            setUpdating(false);\n        }\n    }\n\n    const buildRefArgText = (arg: { var: string, options: string }, idx: number) => {\n        return (<TextField\n            id={`subArg-${arg.var}`}\n            key={arg.var}\n            label={`${arg.var}`}\n            helperText={idx === 0 ? \"You can input multiple names separated by a space character\" : undefined}\n            type=\"text\"\n            fullWidth\n            variant='standard'\n            value={arg.options}\n            onChange={(event: any) => {\n                const options = refArgsOptions.map(value => {\n                    if (value.var === arg.var) {\n                        return {\n                            ...value,\n                            options: event.target.value,\n                        }\n                    } else {\n                        return value\n                    }\n                });\n                setRefArgsOptions(options)\n            }}\n            margin=\"normal\"\n            required\n        />)\n    }\n\n    return (<Dialog\n        disableEscapeKeyDown\n        open={props.open}\n        sx={{ '& .MuiDialog-paper': { width: '80%' } }}\n    >\n        <DialogTitle>Add Subcommands</DialogTitle>\n        <DialogContent dividers={true}>\n            {invalidText && <Alert variant=\"filled\" severity='error'> {invalidText} </Alert>}\n            <FormLabel>Subcommand Group</FormLabel>\n            <TextField\n                id='subcommand-group-name'\n                label='name'\n                placeholder='Please input command group name for subcommands'\n                type=\"text\"\n                variant='standard'\n                value={commandGroupName}\n                fullWidth\n                margin=\"normal\"\n                required\n                onChange={(event: any) => {\n                    setCommandGroupName(event.target.value)\n                }}\n            />\n            {refArgsOptions.length > 0 && <>\n                <FormLabel>Argument Options</FormLabel>\n                {refArgsOptions.map(buildRefArgText)}\n            </>}\n        </DialogContent>\n        <DialogActions>\n            {updating &&\n                <Box sx={{ width: '100%' }}>\n                    <LinearProgress color='secondary' />\n                </Box>\n            }\n            {!updating && <>\n                <Button onClick={handleClose}>Cancel</Button>\n                <Button onClick={handleAddSubresource}>Add Subcommands</Button>\n            </>}\n        </DialogActions>\n    </Dialog>)\n}\n\nconst DecodeResponseCommand = (command: ResponseCommand): Command => {\n    let cmd: Command = {\n        id: 'command:' + command.names.join('/'),\n        names: command.names,\n        help: command.help,\n        stage: command.stage ?? \"Stable\",\n        examples: command.examples,\n        resources: command.resources,\n        version: command.version,\n    }\n\n    if (command.confirmation) {\n        cmd.confirmation = command.confirmation\n    }\n\n    if (command.argGroups) {\n        cmd = {\n            ...cmd,\n            ...DecodeArgs(command.argGroups!)\n        }\n    }\n\n    return cmd;\n}\n\nconst DecodeResponseClientConfig = (clientConfig: any): ClientConfig => {\n    if (clientConfig.argGroups === undefined) {\n        return {}\n    }\n    return {\n        args: DecodeArgs(clientConfig.argGroups!).args\n    }\n}\n\nexport default WSEditorCommandContent;\n\nexport { DecodeResponseCommand };\nexport type { Plane, Command, Resource, ResponseCommand, ResponseCommands, Example };\n",
         "// Source from https://github.com/alitaheri/normalize-scroll-left\nlet cachedType;\n/**\n * Based on the jquery plugin https://github.com/othree/jquery.rtl-scroll-type\n *\n * Types of scrollLeft, assuming scrollWidth=100 and direction is rtl.\n *\n * Type             | <- Most Left | Most Right -> | Initial\n * ---------------- | ------------ | ------------- | -------\n * default          | 0            | 100           | 100\n * negative (spec*) | -100         | 0             | 0\n * reverse          | 100          | 0             | 0\n *\n * Edge 85: default\n * Safari 14: negative\n * Chrome 85: negative\n * Firefox 81: negative\n * IE11: reverse\n *\n * spec* https://drafts.csswg.org/cssom-view/#dom-window-scroll\n */\n\nexport function detectScrollType() {\n  if (cachedType) {\n    return cachedType;\n  }\n\n  const dummy = document.createElement('div');\n  const container = document.createElement('div');\n  container.style.width = '10px';\n  container.style.height = '1px';\n  dummy.appendChild(container);\n  dummy.dir = 'rtl';\n  dummy.style.fontSize = '14px';\n  dummy.style.width = '4px';\n  dummy.style.height = '1px';\n  dummy.style.position = 'absolute';\n  dummy.style.top = '-1000px';\n  dummy.style.overflow = 'scroll';\n  document.body.appendChild(dummy);\n  cachedType = 'reverse';\n\n  if (dummy.scrollLeft > 0) {\n    cachedType = 'default';\n  } else {\n    dummy.scrollLeft = 1;\n\n    if (dummy.scrollLeft === 0) {\n      cachedType = 'negative';\n    }\n  }\n\n  document.body.removeChild(dummy);\n  return cachedType;\n} // Based on https://stackoverflow.com/a/24394376\n\nexport function getNormalizedScrollLeft(element, direction) {\n  const scrollLeft = element.scrollLeft; // Perform the calculations only when direction is rtl to avoid messing up the ltr behavior\n\n  if (direction !== 'rtl') {\n    return scrollLeft;\n  }\n\n  const type = detectScrollType();\n\n  switch (type) {\n    case 'negative':\n      return element.scrollWidth - element.clientWidth + scrollLeft;\n\n    case 'reverse':\n      return element.scrollWidth - element.clientWidth - scrollLeft;\n\n    default:\n      return scrollLeft;\n  }\n}",
         "function easeInOutSin(time) {\n  return (1 + Math.sin(Math.PI * time - Math.PI / 2)) / 2;\n}\n\nexport default function animate(property, element, to, options = {}, cb = () => {}) {\n  const {\n    ease = easeInOutSin,\n    duration = 300 // standard\n\n  } = options;\n  let start = null;\n  const from = element[property];\n  let cancelled = false;\n\n  const cancel = () => {\n    cancelled = true;\n  };\n\n  const step = timestamp => {\n    if (cancelled) {\n      cb(new Error('Animation cancelled'));\n      return;\n    }\n\n    if (start === null) {\n      start = timestamp;\n    }\n\n    const time = Math.min(1, (timestamp - start) / duration);\n    element[property] = ease(time) * (to - from) + from;\n\n    if (time >= 1) {\n      requestAnimationFrame(() => {\n        cb(null);\n      });\n      return;\n    }\n\n    requestAnimationFrame(step);\n  };\n\n  if (from === to) {\n    cb(new Error('Element already at target position'));\n    return cancel;\n  }\n\n  requestAnimationFrame(step);\n  return cancel;\n}",
         "import _extends from \"@babel/runtime/helpers/esm/extends\";\nimport _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nconst _excluded = [\"onChange\"];\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport debounce from '../utils/debounce';\nimport { ownerWindow } from '../utils';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nconst styles = {\n  width: 99,\n  height: 99,\n  position: 'absolute',\n  top: -9999,\n  overflow: 'scroll'\n};\n/**\n * @ignore - internal component.\n * The component originates from https://github.com/STORIS/react-scrollbar-size.\n * It has been moved into the core in order to minimize the bundle size.\n */\n\nexport default function ScrollbarSize(props) {\n  const {\n    onChange\n  } = props,\n        other = _objectWithoutPropertiesLoose(props, _excluded);\n\n  const scrollbarHeight = React.useRef();\n  const nodeRef = React.useRef(null);\n\n  const setMeasurements = () => {\n    scrollbarHeight.current = nodeRef.current.offsetHeight - nodeRef.current.clientHeight;\n  };\n\n  React.useEffect(() => {\n    const handleResize = debounce(() => {\n      const prevHeight = scrollbarHeight.current;\n      setMeasurements();\n\n      if (prevHeight !== scrollbarHeight.current) {\n        onChange(scrollbarHeight.current);\n      }\n    });\n    const containerWindow = ownerWindow(nodeRef.current);\n    containerWindow.addEventListener('resize', handleResize);\n    return () => {\n      handleResize.clear();\n      containerWindow.removeEventListener('resize', handleResize);\n    };\n  }, [onChange]);\n  React.useEffect(() => {\n    setMeasurements();\n    onChange(scrollbarHeight.current);\n  }, [onChange]);\n  return /*#__PURE__*/_jsx(\"div\", _extends({\n    style: styles,\n    ref: nodeRef\n  }, other));\n}\nprocess.env.NODE_ENV !== \"production\" ? ScrollbarSize.propTypes = {\n  onChange: PropTypes.func.isRequired\n} : void 0;",
         "import * as React from 'react';\nimport createSvgIcon from '../../utils/createSvgIcon';\n/**\n * @ignore - internal component.\n */\n\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nexport default createSvgIcon( /*#__PURE__*/_jsx(\"path\", {\n  d: \"M15.41 16.09l-4.58-4.59 4.58-4.59L14 5.5l-6 6 6 6z\"\n}), 'KeyboardArrowLeft');",
         "import * as React from 'react';\nimport createSvgIcon from '../../utils/createSvgIcon';\n/**\n * @ignore - internal component.\n */\n\nimport { jsx as _jsx } from \"react/jsx-runtime\";\nexport default createSvgIcon( /*#__PURE__*/_jsx(\"path\", {\n  d: \"M8.59 16.34l4.58-4.59-4.58-4.59L10 5.75l6 6-6 6z\"\n}), 'KeyboardArrowRight');",
         "import { generateUtilityClass, generateUtilityClasses } from '@mui/base';\nexport function getTabScrollButtonUtilityClass(slot) {\n  return generateUtilityClass('MuiTabScrollButton', slot);\n}\nconst tabScrollButtonClasses = generateUtilityClasses('MuiTabScrollButton', ['root', 'vertical', 'horizontal', 'disabled']);\nexport default tabScrollButtonClasses;",
         "import _objectWithoutPropertiesLoose from \"@babel/runtime/helpers/esm/objectWithoutPropertiesLoose\";\nimport _extends from \"@babel/runtime/helpers/esm/extends\";\n\nvar _KeyboardArrowLeft, _KeyboardArrowRight;\n\nconst _excluded = [\"className\", \"direction\", \"orientation\", \"disabled\"];\n\n/* eslint-disable jsx-a11y/aria-role */\nimport * as React from 'react';\nimport PropTypes from 'prop-types';\nimport clsx from 'clsx';\nimport { unstable_composeClasses as composeClasses } from '@mui/base';\nimport KeyboardArrowLeft from '../internal/svg-icons/KeyboardArrowLeft';\nimport KeyboardArrowRight from '../internal/svg-icons/KeyboardArrowRight';\nimport ButtonBase from '../ButtonBase';\nimport useTheme from '../styles/useTheme';\nimport useThemeProps from '../styles/useThemeProps';\nimport styled from '../styles/styled';\nimport tabScrollButtonClasses, { getTabScrollButtonUtilityClass } from './tabScrollButtonClasses';\nimport { jsx as _jsx } from \"react/jsx-runtime\";\n\nconst useUtilityClasses = ownerState => {\n  const {\n    classes,\n    orientation,\n    disabled\n  } = ownerState;\n  const slots = {\n    root: ['root', orientation, disabled && 'disabled']\n  };\n  return composeClasses(slots, getTabScrollButtonUtilityClass, classes);\n};\n\nconst TabScrollButtonRoot = styled(ButtonBase, {\n  name: 'MuiTabScrollButton',\n  slot: 'Root',\n  overridesResolver: (props, styles) => {\n    const {\n      ownerState\n    } = props;\n    return [styles.root, ownerState.orientation && styles[ownerState.orientation]];\n  }\n})(({\n  ownerState\n}) => _extends({\n  width: 40,\n  flexShrink: 0,\n  opacity: 0.8,\n  [`&.${tabScrollButtonClasses.disabled}`]: {\n    opacity: 0\n  }\n}, ownerState.orientation === 'vertical' && {\n  width: '100%',\n  height: 40,\n  '& svg': {\n    transform: `rotate(${ownerState.isRtl ? -90 : 90}deg)`\n  }\n}));\nconst TabScrollButton = /*#__PURE__*/React.forwardRef(function TabScrollButton(inProps, ref) {\n  const props = useThemeProps({\n    props: inProps,\n    name: 'MuiTabScrollButton'\n  });\n\n  const {\n    className,\n    direction\n  } = props,\n        other = _objectWithoutPropertiesLoose(props, _excluded);\n\n  const theme = useTheme();\n  const isRtl = theme.direction === 'rtl';\n\n  const ownerState = _extends({\n    isRtl\n  }, props);\n\n  const classes = useUtilityClasses(ownerState);\n  return /*#__PURE__*/_jsx(TabScrollButtonRoot, _extends({\n    component: \"div\",\n    className: clsx(classes.root, className),\n    ref: ref,\n    role: null,\n    ownerState: ownerState,\n    tabIndex: null\n  }, other, {\n    children: direction === 'left' ? _KeyboardArrowLeft || (_KeyboardArrowLeft = /*#__PURE__*/_jsx(KeyboardArrowLeft, {\n      fontSize: \"small\"\n    })) : _KeyboardArrowRight || (_KeyboardArrowRight = /*#__PURE__*/_jsx(KeyboardArrowRight, {\n      fontSize: \"small\"\n    }))\n  }));\n});\nprocess.env.NODE_ENV !== \"production\" ? TabScrollButton.propTypes\n/* remove-proptypes */\n= {\n  // ----------------------------- Warning --------------------------------\n  // | These PropTypes are generated from the TypeScript type definitions |\n  // |     To update them edit the d.ts file and run \"yarn proptypes\"     |\n  // ----------------------------------------------------------------------\n\n  /**\n   * The content of the component.\n   */\n  children: PropTypes.node,\n\n  /**\n   * Override or extend the styles applied to the component.\n   */\n  classes: PropTypes.object,\n\n  /**\n   * @ignore\n   */\n  className: PropTypes.string,\n\n  /**\n   * The direction the button should indicate.\n   */\n  direction: PropTypes.oneOf(['left', 'right']).isRequired,\n\n  /**\n   * If `true`, the component is disabled.\n   */\n  disabled: PropTypes.bool,\n\n  /**\n   * The component orientation (layout flow direction).\n   */\n  orientation: PropTypes.oneOf(['horizontal', 'vertical']).isRequired,\n\n  /**\n   * The system prop that allows defining system overrides as well as additional CSS styles.\n   */\n  sx: PropTypes.oneOfType([PropTypes.arrayOf(PropTypes.oneOfType([PropTypes.func, PropTypes.object, PropTypes.bool])), PropTypes.func, PropTypes.object])\n} : void 0;\nexport default TabScrollButton;",
```

### Comparing `aaz_dev-2.6.2/src/aaz_dev/utils/config.py` & `aaz_dev-2.7.0/src/aaz_dev/utils/config.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/utils/error_format.py` & `aaz_dev-2.7.0/src/aaz_dev/utils/error_format.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/utils/exceptions.py` & `aaz_dev-2.7.0/src/aaz_dev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/utils/fields.py` & `aaz_dev-2.7.0/src/aaz_dev/utils/fields.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/utils/plane.py` & `aaz_dev-2.7.0/src/aaz_dev/utils/plane.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/utils/portal_file_schema.py` & `aaz_dev-2.7.0/src/aaz_dev/utils/portal_file_schema.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev/utils/stage.py` & `aaz_dev-2.7.0/src/aaz_dev/utils/stage.py`

 * *Files identical despite different names*

### Comparing `aaz_dev-2.6.2/src/aaz_dev.egg-info/PKG-INFO` & `aaz_dev-2.7.0/src/aaz_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 2.6.2
+Version: 2.7.0
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aaz_dev-2.6.2/src/aaz_dev.egg-info/SOURCES.txt` & `aaz_dev-2.7.0/src/aaz_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 src/aaz_dev/command/api/_cmds.py
 src/aaz_dev/command/api/editor.py
 src/aaz_dev/command/api/specs.py
 src/aaz_dev/command/controller/__init__.py
 src/aaz_dev/command/controller/cfg_reader.py
 src/aaz_dev/command/controller/cfg_validator.py
 src/aaz_dev/command/controller/client_cfg_reader.py
+src/aaz_dev/command/controller/shorthand.py
 src/aaz_dev/command/controller/specs_manager.py
 src/aaz_dev/command/controller/workspace_cfg_editor.py
 src/aaz_dev/command/controller/workspace_client_cfg_editor.py
 src/aaz_dev/command/controller/workspace_helper.py
 src/aaz_dev/command/controller/workspace_manager.py
 src/aaz_dev/command/model/__init__.py
 src/aaz_dev/command/model/configuration/__init__.py
@@ -135,20 +136,23 @@
 src/aaz_dev/command/templates/resource_ref.md.j2
 src/aaz_dev/command/templates/tree.md.j2
 src/aaz_dev/swagger/__init__.py
 src/aaz_dev/swagger/api/__init__.py
 src/aaz_dev/swagger/api/_cmds.py
 src/aaz_dev/swagger/api/specs.py
 src/aaz_dev/swagger/controller/__init__.py
+src/aaz_dev/swagger/controller/_example_builder.py
 src/aaz_dev/swagger/controller/command_generator.py
+src/aaz_dev/swagger/controller/example_generator.py
 src/aaz_dev/swagger/controller/specs_manager.py
 src/aaz_dev/swagger/model/__init__.py
 src/aaz_dev/swagger/model/schema/__init__.py
 src/aaz_dev/swagger/model/schema/cmd_builder.py
 src/aaz_dev/swagger/model/schema/contact.py
+src/aaz_dev/swagger/model/schema/example_item.py
 src/aaz_dev/swagger/model/schema/external_documentation.py
 src/aaz_dev/swagger/model/schema/fields.py
 src/aaz_dev/swagger/model/schema/header.py
 src/aaz_dev/swagger/model/schema/info.py
 src/aaz_dev/swagger/model/schema/items.py
 src/aaz_dev/swagger/model/schema/license.py
 src/aaz_dev/swagger/model/schema/operation.py
@@ -182,17 +186,17 @@
 src/aaz_dev/ui/index.html
 src/aaz_dev/ui/logo192.png
 src/aaz_dev/ui/logo512.png
 src/aaz_dev/ui/manifest.json
 src/aaz_dev/ui/robots.txt
 src/aaz_dev/ui/static/css/main.e6c13ad2.css
 src/aaz_dev/ui/static/css/main.e6c13ad2.css.map
-src/aaz_dev/ui/static/js/main.aa1f209d.js
-src/aaz_dev/ui/static/js/main.aa1f209d.js.LICENSE.txt
-src/aaz_dev/ui/static/js/main.aa1f209d.js.map
+src/aaz_dev/ui/static/js/main.90022267.js
+src/aaz_dev/ui/static/js/main.90022267.js.LICENSE.txt
+src/aaz_dev/ui/static/js/main.90022267.js.map
 src/aaz_dev/utils/__init__.py
 src/aaz_dev/utils/base64.py
 src/aaz_dev/utils/case.py
 src/aaz_dev/utils/client.py
 src/aaz_dev/utils/config.py
 src/aaz_dev/utils/error_format.py
 src/aaz_dev/utils/exceptions.py
```
