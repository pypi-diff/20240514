# Comparing `tmp/libbs-1.2.7.tar.gz` & `tmp/libbs-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbs-1.2.7.tar", last modified: Tue Apr 16 20:08:02 2024, max compression
+gzip compressed data, was "libbs-1.3.1.tar", last modified: Tue May 14 02:05:15 2024, max compression
```

## Comparing `libbs-1.2.7.tar` & `libbs-1.3.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.582665 libbs-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-16 20:07:58.000000 libbs-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-16 20:08:02.582665 libbs-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-16 20:07:58.000000 libbs-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.566666 libbs-1.2.7/libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.570665 libbs-1.2.7/libbs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/artifact_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/decompiler_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/decompilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/stack_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/artifacts/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/angr_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/angr_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/binja_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/binja_libbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompiler_stubs/ida_libbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompilers/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.574665 libbs-1.2.7/libbs/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/angr/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/angr/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/binja/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/binja/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/artifact_lifter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/decompilers/ghidra/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/compat/ghidra_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/compat/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32838 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ghidra/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/decompilers/ida/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/plugin_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.578665 libbs-1.2.7/libbs/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 20:07:58.000000 libbs-1.2.7/libbs/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.582665 libbs-1.2.7/libbs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 20:08:02.000000 libbs-1.2.7/libbs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 20:08:02.582665 libbs-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 20:07:58.000000 libbs-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:08:02.582665 libbs-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-16 20:07:58.000000 libbs-1.2.7/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-16 20:07:58.000000 libbs-1.2.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-16 20:07:58.000000 libbs-1.2.7/tests/test_decompilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.288371 libbs-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-14 02:05:11.000000 libbs-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-14 02:05:15.288371 libbs-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-14 02:05:11.000000 libbs-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.276371 libbs-1.3.1/libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.280371 libbs-1.3.1/libbs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/api/artifact_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26006 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/api/decompiler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/api/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.280371 libbs-1.3.1/libbs/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/decompilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/stack_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/artifacts/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.280371 libbs-1.3.1/libbs/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.280371 libbs-1.3.1/libbs/decompiler_stubs/angr_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/angr_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.280371 libbs-1.3.1/libbs/decompiler_stubs/binja_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/binja_libbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.280371 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_mainthread_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/ghidra_libbs_shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.284371 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.284371 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89858 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompiler_stubs/ida_libbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.284371 libbs-1.3.1/libbs/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.284371 libbs-1.3.1/libbs/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/angr/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/angr/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.284371 libbs-1.3.1/libbs/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/binja/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20930 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/binja/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.284371 libbs-1.3.1/libbs/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ghidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ghidra/artifact_lifter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.284371 libbs-1.3.1/libbs/decompilers/ghidra/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ghidra/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ghidra/compat/ghidra_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ghidra/compat/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ghidra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32841 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ghidra/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.288371 libbs-1.3.1/libbs/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ida/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ida/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12593 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/decompilers/ida/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/plugin_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.288371 libbs-1.3.1/libbs/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 02:05:11.000000 libbs-1.3.1/libbs/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.288371 libbs-1.3.1/libbs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-14 02:05:15.000000 libbs-1.3.1/libbs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-14 02:05:15.000000 libbs-1.3.1/libbs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:05:15.000000 libbs-1.3.1/libbs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 02:05:15.000000 libbs-1.3.1/libbs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 02:05:15.000000 libbs-1.3.1/libbs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 02:05:15.000000 libbs-1.3.1/libbs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-14 02:05:15.288371 libbs-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 02:05:11.000000 libbs-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:05:15.288371 libbs-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-14 02:05:11.000000 libbs-1.3.1/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-14 02:05:11.000000 libbs-1.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-14 02:05:11.000000 libbs-1.3.1/tests/test_decompilers.py
```

### Comparing `libbs-1.2.7/LICENSE` & `libbs-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/PKG-INFO` & `libbs-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.7
+Version: 1.3.1
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
```

### Comparing `libbs-1.2.7/README.md` & `libbs-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/__main__.py` & `libbs-1.3.1/libbs/__main__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/api/artifact_dict.py` & `libbs-1.3.1/libbs/api/artifact_dict.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/api/artifact_lifter.py` & `libbs-1.3.1/libbs/api/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/api/decompiler_interface.py` & `libbs-1.3.1/libbs/api/decompiler_interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/api/type_parser.py` & `libbs-1.3.1/libbs/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/api/utils.py` & `libbs-1.3.1/libbs/api/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/artifacts/artifact.py` & `libbs-1.3.1/libbs/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/artifacts/comment.py` & `libbs-1.3.1/libbs/artifacts/comment.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/artifacts/decompilation.py` & `libbs-1.3.1/libbs/artifacts/decompilation.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/artifacts/enum.py` & `libbs-1.3.1/libbs/artifacts/enum.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/artifacts/func.py` & `libbs-1.3.1/libbs/artifacts/func.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/artifacts/global_variable.py` & `libbs-1.3.1/libbs/artifacts/global_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/artifacts/patch.py` & `libbs-1.3.1/libbs/artifacts/patch.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/artifacts/stack_variable.py` & `libbs-1.3.1/libbs/artifacts/stack_variable.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/artifacts/struct.py` & `libbs-1.3.1/libbs/artifacts/struct.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py` & `libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/ghidra_bridge_server.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py` & `libbs-1.3.1/libbs/decompiler_stubs/ghidra_libbs/libbs_vendored/jfx_bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/angr/artifact_lifter.py` & `libbs-1.3.1/libbs/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/angr/compat.py` & `libbs-1.3.1/libbs/decompilers/angr/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/angr/interface.py` & `libbs-1.3.1/libbs/decompilers/angr/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/binja/artifact_lifter.py` & `libbs-1.3.1/libbs/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/binja/hooks.py` & `libbs-1.3.1/libbs/decompilers/binja/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/binja/interface.py` & `libbs-1.3.1/libbs/decompilers/binja/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/ghidra/artifact_lifter.py` & `libbs-1.3.1/libbs/decompilers/ghidra/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/ghidra/compat/ghidra_api.py` & `libbs-1.3.1/libbs/decompilers/ghidra/compat/ghidra_api.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/ghidra/hooks.py` & `libbs-1.3.1/libbs/decompilers/ghidra/hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,21 +38,14 @@
                 self.changeManager.DOCR_DATA_TYPE_RENAMED,
                 self.changeManager.DOCR_DATA_TYPE_SETTING_CHANGED,
                 self.changeManager.DOCR_DATA_TYPE_MOVED,
                 self.changeManager.DOCR_DATA_TYPE_ADDED
             ]
         def domainObjectChanged(self, ev):
             for record in ev:
-                # NOTE: This excludes type changes anything as they are DomainObjectChangeRecord
-                # print(f"Event type {record.getEventType()} caught:")
-                # print(f"\tNewValue: {record.getNewValue()}")
-                # print(f"\tOldValue: {record.getOldValue()}")
-                # print(f"\tObjectType: {type(record.getObject())}")
-                if record.getEventType() == 5:
-                    print(record)
                 if not self._interface.ghidra.isinstance(record, self.programChangeRecord):
                     continue
 
                 changeType = record.getEventType()
                 newValue = record.getNewValue()
                 obj = record.getObject()
 
@@ -69,24 +62,40 @@
 
                     try:
                         enum = self._interface.enums[newValue.name]
                         #self._interface.enum_changed(Enum(None, None), deleted=True)
                         self._interface.enum_changed(enum)
                     except KeyError:
                         pass
-
                 elif changeType in self.symDelEvents:
-                    # Currently unused and unsupported
-                    pass
+                    # Globals are deleted first then recreated
+                    if self._interface.ghidra.isinstance(obj, self.db.symbol.CodeSymbol):
+                        removed = GlobalVariable(obj.getAddress().getOffset(), obj.getName())
+                        # deleted kwarg not yet handled by global_variable_changed
+                        self._interface.global_variable_changed(removed, deleted=True)
                 elif changeType in self.symChgEvents:
-                    #if changeType == 52:
-                        #print(f"Record:\n{record}")
+                    # For creation events, obj is stored in newValue
                     if obj is None and newValue is not None:
                         obj = newValue
-                    if self._interface.ghidra.isinstance(obj, self.db.function.VariableDB):
+
+                    if changeType == self.changeManager.DOCR_SYMBOL_ADDED:
+                        if self._interface.ghidra.isinstance(obj, self.db.symbol.CodeSymbol):
+                            gvar = GlobalVariable(obj.getAddress().getOffset(), obj.getName())
+                            self._interface.global_variable_changed(gvar)
+                    elif changeType == self.changeManager.DOCR_SYMBOL_RENAMED:
+                        if self._interface.ghidra.isinstance(obj, self.db.symbol.CodeSymbol):
+                            gvar = GlobalVariable(obj.getAddress().getOffset(), newValue)
+                            self._interface.global_variable_changed(gvar)
+
+                        if self._interface.ghidra.isinstance(obj, self.db.symbol.FunctionSymbol):
+                            header = FunctionHeader(newValue, int(obj.getAddress().offset))
+                            self._interface.function_header_changed(
+                                self._interface.art_lifter.lift(header)
+                            )
+                    elif self._interface.ghidra.isinstance(obj, self.db.function.VariableDB):
                         parent_namespace = obj.getParentNamespace()
                         storage = obj.getVariableStorage()
                         if (
                             (newValue is not None) and (storage is not None) and bool(storage.isStackStorage())
                             and (parent_namespace is not None)
                         ):
                             self._interface.stack_variable_changed(
@@ -106,30 +115,19 @@
                             # print(f"Obj type: {type(obj)}")
                             # print(f"Old value: {oldValue}")
                             # print(f"New value: {newValue}")
                             # typ = obj.getDataType()
                             # stackVar = StackVariable(None, None, typ, None, None)
                             # self._interface.stack_variable_changed(stackVar)
                             pass
-                        continue
-                    elif self._interface.ghidra.isinstance(obj, self.db.symbol.CodeSymbol):
-                        # TODO: Find trigger for global var changes
-                        # gVar = GlobalVariable(None, newValue)
-                        # self._interface.global_variable_changed(gVar)
-                        continue
-                    elif self._interface.ghidra.isinstance(obj, self.db.symbol.FunctionSymbol):
-                        header = FunctionHeader(newValue, int(obj.getAddress().offset))
-                        self._interface.function_header_changed(
-                            self._interface.art_lifter.lift(header)
-                        )
                     elif self._interface.ghidra.isinstance(obj, self.db.function.FunctionDB):
                         # TODO: Fix argument name support
-                        #changed_arg = FunctionArgument(None, newValue, None, None)
-                        #header = FunctionHeader(None, None, args={None: changed_arg})
-                        #self._interface.function_header_changed(header)
+                        # changed_arg = FunctionArgument(None, newValue, None, None)
+                        # header = FunctionHeader(None, None, args={None: changed_arg})
+                        # self._interface.function_header_changed(header)
                         pass
                     else:
                         continue
 
     data_monitor = DataMonitor(interface)
     return data_monitor
```

### Comparing `libbs-1.2.7/libbs/decompilers/ghidra/interface.py` & `libbs-1.3.1/libbs/decompilers/ghidra/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,20 +508,20 @@
 
     def _enums(self) -> Dict[str, Enum]:
         names: Optional[List[str]] = self.ghidra.bridge.remote_eval(
             "[dType.getPathName() "
             "for dType in currentProgram.getDataTypeManager().getAllDataTypes()"
             "if ghidra.isinstance(dType, EnumDBType)]",
         ghidra=self.ghidra,
-        EnumDBType=self.ghidra.import_module_object("ghidra.program.model.data", "EnumDB")
+        EnumDBType=self.ghidra.import_module_object("ghidra.program.database.data", "EnumDB")
         )
         enums = {}
         for name in names:
-            # XXX: we dont really know why this is here, but we assume its because you cant have
-            # an enum nested in a folder in ghidra
+            # Filter out enums nested in categories as currently they are unsupported by the current method of updating
+            # the enum name
             if name.count("/") != 1:
                 continue
 
             enum_name = name[1:]
             is_valid_enum = self._get_ghidra_enum(enum_name)
             if is_valid_enum is None:
                 continue
```

### Comparing `libbs-1.2.7/libbs/decompilers/ida/artifact_lifter.py` & `libbs-1.3.1/libbs/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/ida/compat.py` & `libbs-1.3.1/libbs/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/ida/hooks.py` & `libbs-1.3.1/libbs/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/decompilers/ida/interface.py` & `libbs-1.3.1/libbs/decompilers/ida/interface.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/logger.py` & `libbs-1.3.1/libbs/logger.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/plugin_installer.py` & `libbs-1.3.1/libbs/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/ui/__init__.py` & `libbs-1.3.1/libbs/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/ui/qt_objects.py` & `libbs-1.3.1/libbs/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs/ui/utils.py` & `libbs-1.3.1/libbs/ui/utils.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/libbs.egg-info/PKG-INFO` & `libbs-1.3.1/libbs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbs
-Version: 1.2.7
+Version: 1.3.1
 Summary: Your Only Decompiler API Lib - A generic API to script in and out of decompilers
 Home-page: https://github.com/binsync/libbs
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
```

### Comparing `libbs-1.2.7/libbs.egg-info/SOURCES.txt` & `libbs-1.3.1/libbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/setup.cfg` & `libbs-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/tests/test_artifacts.py` & `libbs-1.3.1/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/tests/test_cli.py` & `libbs-1.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `libbs-1.2.7/tests/test_decompilers.py` & `libbs-1.3.1/tests/test_decompilers.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,14 +107,25 @@
         deci.functions[func_addr] = main
 
         first_changed_func = hits[FunctionHeader][0]
         assert first_changed_func.name == "changed"
         assert first_changed_func.addr == func_addr
         assert len(hits[FunctionHeader]) == 2
 
+        # global var names
+        # TODO: The gvar test cant function until gvar setting is fixed
+        old_global_hits = len(hits[GlobalVariable])
+        g1 = deci.global_vars[0x4008e0]
+        g2 = deci.global_vars[0x601048]
+        g1.name = "gvar1"
+        g2.name = "gvar2"
+        deci.global_vars[0x4008e0] = g1
+        deci.global_vars[0x601048] = g2
+        # assert len(hits[GlobalVariable]) == old_global_hits + 2
+
         # TODO: Fix CI for below
         main.stack_vars[-24].name = "named_char_array"
         main.stack_vars[-12].name = "named_int"
         deci.functions[func_addr] = main
         #first_changed_sv = hits[StackVariable][0]
         #assert first_changed_sv.name == main.stack_vars[-24].name
         #assert len(hits[StackVariable]) == 2
@@ -125,24 +136,15 @@
 
         # TODO: add argument naming
         # func_args = main.header.args
         # func_args[0].name = "changed_name"
         # func_args[1].name = "changed_name2"
         # deci.functions[func_addr] = main
 
-        # TODO: add global var support
-        # g1 = deci.global_vars[0x4008e0]
-        # g2 = deci.global_vars[0x601048]
-        # g1.name = "gvar1"
-        # g2.name = "gvar2"
-        # deci.global_vars[0x4008e0] = g1
-        # deci.global_vars[0x601048] = g2
-
         #assert hits[Struct] == 2 # One change results in 2 hits because the struct is first removed and then added again.
-        #assert hits[GlobalVariable] == 2
 
         deci.shutdown()
 
     def test_angr(self):
         deci = DecompilerInterface.discover(
             force_decompiler=ANGR_DECOMPILER,
             headless=True,
```

