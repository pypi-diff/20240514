# Comparing `tmp/yycli-0.0.4.tar.gz` & `tmp/yycli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yycli-0.0.4.tar", last modified: Wed Nov 15 13:45:54 2023, max compression
+gzip compressed data, was "yycli-0.0.5.tar", last modified: Tue May 14 12:27:37 2024, max compression
```

## Comparing `yycli-0.0.4.tar` & `yycli-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:45:54.312324 yycli-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-11-15 13:45:44.000000 yycli-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-11-15 13:45:54.312324 yycli-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-15 13:45:44.000000 yycli-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-11-15 13:45:44.000000 yycli-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-15 13:45:44.000000 yycli-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 13:45:54.312324 yycli-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:45:54.308324 yycli-0.0.4/yycli/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-15 13:45:44.000000 yycli-0.0.4/yycli/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-15 13:45:44.000000 yycli-0.0.4/yycli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-11-15 13:45:44.000000 yycli-0.0.4/yycli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:45:54.312324 yycli-0.0.4/yycli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-15 13:45:44.000000 yycli-0.0.4/yycli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2023-11-15 13:45:44.000000 yycli-0.0.4/yycli/commands/confuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2023-11-15 13:45:44.000000 yycli-0.0.4/yycli/commands/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:45:54.312324 yycli-0.0.4/yycli/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-15 13:45:44.000000 yycli-0.0.4/yycli/conf/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-11-15 13:45:44.000000 yycli-0.0.4/yycli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2023-11-15 13:45:44.000000 yycli-0.0.4/yycli/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 13:45:54.308324 yycli-0.0.4/yycli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-11-15 13:45:54.000000 yycli-0.0.4/yycli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-11-15 13:45:54.000000 yycli-0.0.4/yycli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 13:45:54.000000 yycli-0.0.4/yycli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-15 13:45:54.000000 yycli-0.0.4/yycli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-15 13:45:54.000000 yycli-0.0.4/yycli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-15 13:45:54.000000 yycli-0.0.4/yycli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:27:37.632003 yycli-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 12:27:32.000000 yycli-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-14 12:27:37.632003 yycli-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 12:27:32.000000 yycli-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-14 12:27:32.000000 yycli-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 12:27:32.000000 yycli-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:27:37.632003 yycli-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:27:37.628003 yycli-0.0.5/yycli/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:27:37.632003 yycli-0.0.5/yycli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/commands/confuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/commands/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/commands/ipinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7030 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/commands/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:27:37.632003 yycli-0.0.5/yycli/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/conf/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-14 12:27:32.000000 yycli-0.0.5/yycli/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:27:37.632003 yycli-0.0.5/yycli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-14 12:27:37.000000 yycli-0.0.5/yycli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-14 12:27:37.000000 yycli-0.0.5/yycli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:27:37.000000 yycli-0.0.5/yycli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 12:27:37.000000 yycli-0.0.5/yycli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 12:27:37.000000 yycli-0.0.5/yycli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 12:27:37.000000 yycli-0.0.5/yycli.egg-info/top_level.txt
```

### Comparing `yycli-0.0.4/LICENSE` & `yycli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yycli-0.0.4/pyproject.toml` & `yycli-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yycli-0.0.4/yycli/__main__.py` & `yycli-0.0.5/yycli/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,14 +26,20 @@
                                        dest='command')
     crypt_parser = subparsers.add_parser('crypt', help='crypt help')
     register_command(crypt_parser, 'crypt', commands.crypt.crypt,
                      commands.crypt.args_parser)
     confuse_parser = subparsers.add_parser('confuse', help='confuse help')
     register_command(confuse_parser, 'confuse', commands.confuse.entrypoint,
                      commands.confuse.args_parser)
+    ipinfo_parser = subparsers.add_parser('ipinfo', help='ipinfo help')
+    register_command(ipinfo_parser, 'ipinfo', commands.ipinfo.ipinfo,
+                     commands.ipinfo.args_parser)
+    weather_parser = subparsers.add_parser('weather', help='weather help')
+    register_command(weather_parser, 'weather', commands.weather.weather,
+                     commands.weather.args_parser)
     args = parser.parse_args()
     if args.command is None:
         parser.print_help()
         return
     COMMANDS[args.command]['command'](args)
```

### Comparing `yycli-0.0.4/yycli/commands/confuse.py` & `yycli-0.0.5/yycli/commands/confuse.py`

 * *Files identical despite different names*

### Comparing `yycli-0.0.4/yycli/commands/crypt.py` & `yycli-0.0.5/yycli/commands/crypt.py`

 * *Files identical despite different names*

### Comparing `yycli-0.0.4/yycli/config.py` & `yycli-0.0.5/yycli/config.py`

 * *Files identical despite different names*

### Comparing `yycli-0.0.4/yycli/tests.py` & `yycli-0.0.5/yycli/tests.py`

 * *Files identical despite different names*

