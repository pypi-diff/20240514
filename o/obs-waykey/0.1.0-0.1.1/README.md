# Comparing `tmp/obs_waykey-0.1.0.tar.gz` & `tmp/obs_waykey-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs_waykey-0.1.0.tar", max compression
+gzip compressed data, was "obs_waykey-0.1.1.tar", max compression
```

## Comparing `obs_waykey-0.1.0.tar` & `obs_waykey-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-11 20:19:27.676324 obs_waykey-0.1.0/LICENSE
--rw-r--r--   0        0        0     1891 2024-05-11 22:55:00.727864 obs_waykey-0.1.0/README.md
--rw-r--r--   0        0        0       90 2024-05-11 21:59:02.087006 obs_waykey-0.1.0/obs_waykey/__init__.py
--rw-r--r--   0        0        0       27 2024-05-11 22:01:29.596525 obs_waykey-0.1.0/obs_waykey/ignition/__init__.py
--rw-r--r--   0        0        0      136 2024-05-11 21:41:27.152336 obs_waykey-0.1.0/obs_waykey/ignition/hotkeys.py
--rw-r--r--   0        0        0      256 2024-05-11 20:19:27.677324 obs_waykey-0.1.0/obs_waykey/toggles.py
--rw-r--r--   0        0        0      398 2024-05-11 22:00:14.393239 obs_waykey-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 obs_waykey-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-11 20:19:27.676324 obs_waykey-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1812 2024-05-12 11:42:25.815367 obs_waykey-0.1.1/README.md
+-rw-r--r--   0        0        0      138 2024-05-14 08:55:24.472435 obs_waykey-0.1.1/obs_waykey/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-11 22:01:29.596525 obs_waykey-0.1.1/obs_waykey/ignition/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-11 21:41:27.152336 obs_waykey-0.1.1/obs_waykey/ignition/hotkeys.py
+-rw-r--r--   0        0        0      256 2024-05-14 08:50:44.135006 obs_waykey-0.1.1/obs_waykey/toggles.py
+-rw-r--r--   0        0        0      452 2024-05-14 08:57:36.995529 obs_waykey-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2347 1970-01-01 00:00:00.000000 obs_waykey-0.1.1/PKG-INFO
```

### Comparing `obs_waykey-0.1.0/LICENSE` & `obs_waykey-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `obs_waykey-0.1.0/README.md` & `obs_waykey-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,38 +10,37 @@
 -   Python 3.9 or greater
 
 # Install and Setup
 
 ## Install
 
 I recommend installing via [pipx](https://github.com/pypa/pipx)
-**ATTENTION:** This package is currently not up on pypi so this command won't work
 
 ```
 pipx install obs-waykey
 ```
 
 If you want a specific version you can grab the `.vhl` from the [releases page](https://github.com/PolyCatDev/obs-waykey/releases) and install it with pipx
 
 ```
 pipx install <file-name>
 ```
 
 ## Setup
 
-ATTENTION: WebScoket authentication must be disabled for this script to work.
+ATTENTION: WebSocket authentication must be disabled for this script to work.
 
-You can find it under `Tools > WebScoket Server Settings > Enable Authentication`.
+You can find it under `Tools > WebSocket Server Settings > Enable Authentication`.
 
 1. Go to your Desktop settings (or WM config file)
 2. Go to where you configure keybinds
 3. Add a new custom keybind
-4. Name it what u want
+4. Name it what you want
 5. Use the command `obs-waykey <toggle>`
-6. Set ur keybind
+6. Set your keybind
 
 ### Here's how mine looks
 
 ![my keybind](https://github.com/PolyCatDev/obs-waykey/blob/main/.github/toggle-rec-config.png)
 
 ## Toggles
```

### Comparing `obs_waykey-0.1.0/PKG-INFO` & `obs_waykey-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: obs-waykey
-Version: 0.1.0
-Summary: OBS global shortcuts workaround for wayland sing websocket
+Version: 0.1.1
+Summary: OBS global shortcuts workaround for wayland using websocket
 Author: PolyCat
 Author-email: polycat@tuta.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,38 +25,37 @@
 -   Python 3.9 or greater
 
 # Install and Setup
 
 ## Install
 
 I recommend installing via [pipx](https://github.com/pypa/pipx)
-**ATTENTION:** This package is currently not up on pypi so this command won't work
 
 ```
 pipx install obs-waykey
 ```
 
 If you want a specific version you can grab the `.vhl` from the [releases page](https://github.com/PolyCatDev/obs-waykey/releases) and install it with pipx
 
 ```
 pipx install <file-name>
 ```
 
 ## Setup
 
-ATTENTION: WebScoket authentication must be disabled for this script to work.
+ATTENTION: WebSocket authentication must be disabled for this script to work.
 
-You can find it under `Tools > WebScoket Server Settings > Enable Authentication`.
+You can find it under `Tools > WebSocket Server Settings > Enable Authentication`.
 
 1. Go to your Desktop settings (or WM config file)
 2. Go to where you configure keybinds
 3. Add a new custom keybind
-4. Name it what u want
+4. Name it what you want
 5. Use the command `obs-waykey <toggle>`
-6. Set ur keybind
+6. Set your keybind
 
 ### Here's how mine looks
 
 ![my keybind](https://github.com/PolyCatDev/obs-waykey/blob/main/.github/toggle-rec-config.png)
 
 ## Toggles
```

