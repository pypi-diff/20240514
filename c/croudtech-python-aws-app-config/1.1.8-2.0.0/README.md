# Comparing `tmp/croudtech-python-aws-app-config-1.1.8.tar.gz` & `tmp/croudtech_python_aws_app_config-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/croudtech-python-aws-app-config-1.1.8.tar", last modified: Tue Oct 12 12:06:06 2021, max compression
+gzip compressed data, was "croudtech_python_aws_app_config-2.0.0.tar", last modified: Tue May 14 16:34:36 2024, max compression
```

## Comparing `croudtech-python-aws-app-config-1.1.8.tar` & `croudtech_python_aws_app_config-2.0.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/
--rw-r--r--   0 jim       (1000) jim       (1000)      614 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/.coveragerc
--rw-r--r--   0 jim       (1000) jim       (1000)      534 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/.gitignore
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.721279 croudtech-python-aws-app-config-1.1.8/.vscode/
--rw-r--r--   0 jim       (1000) jim       (1000)      115 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/.vscode/settings.json
--rw-r--r--   0 jim       (1000) jim       (1000)       79 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/AUTHORS.rst
--rw-r--r--   0 jim       (1000) jim       (1000)      128 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/CHANGELOG.rst
--rw-r--r--   0 jim       (1000) jim       (1000)     1079 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/LICENSE.txt
--rw-r--r--   0 jim       (1000) jim       (1000)     7402 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/PKG-INFO
--rw-r--r--   0 jim       (1000) jim       (1000)      334 2021-07-28 15:20:34.000000 croudtech-python-aws-app-config-1.1.8/Pipfile
--rw-r--r--   0 jim       (1000) jim       (1000)    21362 2021-07-28 15:20:47.000000 croudtech-python-aws-app-config-1.1.8/Pipfile.lock
--rw-r--r--   0 jim       (1000) jim       (1000)     5376 2021-07-28 10:34:33.000000 croudtech-python-aws-app-config-1.1.8/README.md
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.721279 croudtech-python-aws-app-config-1.1.8/docs/
--rw-r--r--   0 jim       (1000) jim       (1000)     7656 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/Makefile
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/docs/_static/
--rw-r--r--   0 jim       (1000) jim       (1000)       18 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/_static/.gitignore
--rw-r--r--   0 jim       (1000) jim       (1000)       41 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/authors.rst
--rw-r--r--   0 jim       (1000) jim       (1000)       43 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/changelog.rst
--rw-r--r--   0 jim       (1000) jim       (1000)     9345 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/conf.py
--rw-r--r--   0 jim       (1000) jim       (1000)     2325 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/index.rst
--rw-r--r--   0 jim       (1000) jim       (1000)       67 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/docs/license.rst
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/nodejs/
--rw-r--r--   0 jim       (1000) jim       (1000)       20 2021-08-16 10:58:50.000000 croudtech-python-aws-app-config-1.1.8/nodejs/.gitignore
--rw-r--r--   0 jim       (1000) jim       (1000)    30752 2021-08-16 11:02:06.000000 croudtech-python-aws-app-config-1.1.8/nodejs/package-lock.json
--rw-r--r--   0 jim       (1000) jim       (1000)      886 2021-08-16 11:02:05.000000 croudtech-python-aws-app-config-1.1.8/nodejs/package.json
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/nodejs/src/
--rw-r--r--   0 jim       (1000) jim       (1000)     1933 2021-08-16 10:13:19.000000 croudtech-python-aws-app-config-1.1.8/nodejs/src/index.ts
--rw-r--r--   0 jim       (1000) jim       (1000)      226 2021-08-13 13:18:11.000000 croudtech-python-aws-app-config-1.1.8/nodejs/tsconfig.json
--rw-r--r--   0 jim       (1000) jim       (1000)       67 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/pytest.ini
--rw-r--r--   0 jim       (1000) jim       (1000)      332 2021-04-26 18:47:32.000000 croudtech-python-aws-app-config-1.1.8/requirements.txt
--rw-r--r--   0 jim       (1000) jim       (1000)     1297 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/setup.cfg
--rw-r--r--   0 jim       (1000) jim       (1000)      933 2021-07-28 15:20:56.000000 croudtech-python-aws-app-config-1.1.8/setup.py
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.721279 croudtech-python-aws-app-config-1.1.8/src/
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/
--rw-r--r--   0 jim       (1000) jim       (1000)      388 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/__init__.py
--rw-r--r--   0 jim       (1000) jim       (1000)     6549 2021-10-12 12:01:52.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/cli.py
--rw-r--r--   0 jim       (1000) jim       (1000)      804 2021-08-11 11:10:04.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/metrics.py
--rw-r--r--   0 jim       (1000) jim       (1000)     2895 2021-08-18 10:20:00.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/redis_config.py
--rw-r--r--   0 jim       (1000) jim       (1000)     2010 2021-07-28 15:20:56.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/response.py
--rw-r--r--   0 jim       (1000) jim       (1000)    13418 2021-10-12 12:04:29.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/ssm_config.py
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/
--rw-r--r--   0 jim       (1000) jim       (1000)        0 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/__init__.py
--rw-r--r--   0 jim       (1000) jim       (1000)      252 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/conftest.py
--rw-r--r--   0 jim       (1000) jim       (1000)      931 2021-07-28 15:20:56.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/redis_config_test.py
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2021-10-12 12:06:06.731279 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/
--rw-r--r--   0 jim       (1000) jim       (1000)     7402 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/PKG-INFO
--rw-r--r--   0 jim       (1000) jim       (1000)     1256 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/SOURCES.txt
--rw-r--r--   0 jim       (1000) jim       (1000)        1 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/dependency_links.txt
--rw-r--r--   0 jim       (1000) jim       (1000)       82 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/entry_points.txt
--rw-r--r--   0 jim       (1000) jim       (1000)        1 2021-04-22 10:05:38.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/not-zip-safe
--rw-r--r--   0 jim       (1000) jim       (1000)      295 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/requires.txt
--rw-r--r--   0 jim       (1000) jim       (1000)       32 2021-10-12 12:06:06.000000 croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/top_level.txt
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/
+-rw-r--r--   0 jim       (1000) jim       (1000)      614 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/.coveragerc
+-rw-r--r--   0 jim       (1000) jim       (1000)      534 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/.gitignore
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/.vscode/
+-rw-r--r--   0 jim       (1000) jim       (1000)      115 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/.vscode/settings.json
+-rw-r--r--   0 jim       (1000) jim       (1000)       79 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/AUTHORS.rst
+-rw-r--r--   0 jim       (1000) jim       (1000)      128 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 jim       (1000) jim       (1000)     1079 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/LICENSE.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)     9319 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/PKG-INFO
+-rw-r--r--   0 jim       (1000) jim       (1000)      350 2024-05-14 15:55:41.000000 croudtech_python_aws_app_config-2.0.0/Pipfile
+-rw-r--r--   0 jim       (1000) jim       (1000)    29811 2024-05-14 15:55:41.000000 croudtech_python_aws_app_config-2.0.0/Pipfile.lock
+-rw-r--r--   0 jim       (1000) jim       (1000)     7362 2021-12-10 12:23:48.000000 croudtech_python_aws_app_config-2.0.0/README.md
+-rw-r--r--   0 jim       (1000) jim       (1000)     1630 2024-05-14 15:55:41.000000 croudtech_python_aws_app_config-2.0.0/azure-pipelines.yml
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/docs/
+-rw-r--r--   0 jim       (1000) jim       (1000)     7656 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/docs/Makefile
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/docs/_static/
+-rw-r--r--   0 jim       (1000) jim       (1000)       18 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/docs/_static/.gitignore
+-rw-r--r--   0 jim       (1000) jim       (1000)       41 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/docs/authors.rst
+-rw-r--r--   0 jim       (1000) jim       (1000)       43 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/docs/changelog.rst
+-rw-r--r--   0 jim       (1000) jim       (1000)     9345 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/docs/conf.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     2325 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/docs/index.rst
+-rw-r--r--   0 jim       (1000) jim       (1000)       67 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/docs/license.rst
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/nodejs/
+-rw-r--r--   0 jim       (1000) jim       (1000)       20 2021-08-16 10:58:50.000000 croudtech_python_aws_app_config-2.0.0/nodejs/.gitignore
+-rw-r--r--   0 jim       (1000) jim       (1000)    30752 2021-08-16 11:02:06.000000 croudtech_python_aws_app_config-2.0.0/nodejs/package-lock.json
+-rw-r--r--   0 jim       (1000) jim       (1000)      886 2021-08-16 11:02:05.000000 croudtech_python_aws_app_config-2.0.0/nodejs/package.json
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/nodejs/src/
+-rw-r--r--   0 jim       (1000) jim       (1000)     1933 2021-08-16 10:13:19.000000 croudtech_python_aws_app_config-2.0.0/nodejs/src/index.ts
+-rw-r--r--   0 jim       (1000) jim       (1000)      226 2021-08-13 13:18:11.000000 croudtech_python_aws_app_config-2.0.0/nodejs/tsconfig.json
+-rw-r--r--   0 jim       (1000) jim       (1000)       67 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/pytest.ini
+-rw-r--r--   0 jim       (1000) jim       (1000)      979 2022-04-27 09:08:36.000000 croudtech_python_aws_app_config-2.0.0/requirements.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)     1297 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/setup.cfg
+-rw-r--r--   0 jim       (1000) jim       (1000)     1076 2024-05-14 16:26:52.000000 croudtech_python_aws_app_config-2.0.0/setup.py
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.114181 croudtech_python_aws_app_config-2.0.0/src/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/
+-rw-r--r--   0 jim       (1000) jim       (1000)      323 2024-05-14 16:15:49.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/__init__.py
+-rw-r--r--   0 jim       (1000) jim       (1000)    11062 2021-12-10 12:18:23.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/cli.py
+-rw-r--r--   0 jim       (1000) jim       (1000)      804 2021-08-11 11:10:04.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/metrics.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     3382 2021-12-10 11:41:22.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/redis_config.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     2010 2021-07-28 15:20:56.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/response.py
+-rw-r--r--   0 jim       (1000) jim       (1000)    14672 2024-04-03 13:42:05.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/ssm_config.py
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/tests/
+-rw-r--r--   0 jim       (1000) jim       (1000)        0 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/tests/__init__.py
+-rw-r--r--   0 jim       (1000) jim       (1000)      252 2021-04-22 10:05:38.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/tests/conftest.py
+-rw-r--r--   0 jim       (1000) jim       (1000)      931 2021-07-28 15:20:56.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/tests/redis_config_test.py
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-05-14 16:34:36.124181 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config.egg-info/
+-rw-r--r--   0 jim       (1000) jim       (1000)     9319 2024-05-14 16:34:36.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config.egg-info/PKG-INFO
+-rw-r--r--   0 jim       (1000) jim       (1000)     1276 2024-05-14 16:34:36.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config.egg-info/SOURCES.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)        1 2024-05-14 16:34:36.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config.egg-info/dependency_links.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)       81 2024-05-14 16:34:36.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config.egg-info/entry_points.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)        1 2024-05-14 16:33:17.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config.egg-info/not-zip-safe
+-rw-r--r--   0 jim       (1000) jim       (1000)      787 2024-05-14 16:34:36.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config.egg-info/requires.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)       32 2024-05-14 16:34:36.000000 croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config.egg-info/top_level.txt
```

### Comparing `croudtech-python-aws-app-config-1.1.8/.coveragerc` & `croudtech_python_aws_app_config-2.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/.gitignore` & `croudtech_python_aws_app_config-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/LICENSE.txt` & `croudtech_python_aws_app_config-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/PKG-INFO` & `croudtech_python_aws_app_config-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,207 +1,260 @@
-Metadata-Version: 2.1
-Name: croudtech-python-aws-app-config
-Version: 1.1.8
-Summary: Applicaton config via AWS SSM
-Home-page: https://github.com/CroudTech/croudtech-python-aws-app-config
-Author: Jim Robinson
-Author-email: jscrobinson@gmail.com
-License: mit
-Description: # croudtech-python-aws-app-config
-        
-        croudtech-python-aws-app-config us a utility to help manage application config using the AWS SSM Parameter Store
-        
-        There is a cli tool to help set the values and a utility to use the SSM parameters within you application.
-        
-        ## Installation
-        
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install croudtech-python-aws-app-config.
-        
-        ```bash
-        pip install croudtech-python-aws-app-config
-        ```
-        
-        ## Command Line Usage
-        
-        ```
-        Usage: cli.py [OPTIONS] COMMAND [ARGS]...
-        
-        Options:
-          --debug / --no-debug
-          --endpoint-url TEXT
-          --help                Show this message and exit.
-        
-        Commands:
-          delete-parameters
-          get-arns
-          get-parameters
-          put-parameters
-          put-parameters-recursive
-        ```
-        
-        --endpoint-url specified the AWS API endpoint URL used. This should be used if using localstack or a similar aws mock service. You can also set the `AWS_ENDPOINT_URL` env var to enable this feature.
-        
-        ### Sub Commands
-        
-        #### delete-parameters
-        
-        Delete parameters from SSM for a specified app and environment
-        
-        ```
-        Usage: cli.py delete-parameters [OPTIONS]
-        
-        Options:
-          --environment-name TEXT  The environment name  [required]
-          --app-name TEXT          The app name  [required]
-          --ssm-prefix TEXT        The ssm path prefix
-          --region TEXT            The AWS region
-          --help                   Show this message and exit.
-        ```
-        
-        #### get-arns
-        
-        Get ARNs for published parameters
-        
-        ```
-        Usage: cli.py get-arns [OPTIONS]
-        
-        Options:
-          --environment-name TEXT         The environment name  [required]
-          --app-name TEXT                 The app name  [required]
-          --ssm-prefix TEXT               The ssm path prefix
-          --region TEXT                   The AWS region
-          --include-common / --ignore-common
-                                          Include shared variables
-          --output-format [ecs]
-          --help                          Show this message and exit.
-        ```
-        
-        #### get-parameters
-        
-        Get parameters for a specific app and environment
-        
-        ```
-        Usage: cli.py get-parameters [OPTIONS]
-        
-        Options:
-          --environment-name TEXT         The environment name  [required]
-          --app-name TEXT                 The app name  [required]
-          --ssm-prefix TEXT               The ssm path prefix
-          --region TEXT                   The AWS region
-          --include-common / --ignore-common
-                                          Include shared variables
-          --output-format [json|yaml|environment|environment-export]
-          --help                          Show this message and exit.
-        ```
-        
-        You can export the variables to your local shell by using
-        
-        ```
-        eval $(croudtech-app-config get-parameters --app-name myapp --environment-name myenv --output-format environment-export)
-        ```
-        #### put-parameters
-        
-        INPUT should be the path to a yaml or json file
-        
-        ```
-        Usage: cli.py put-parameters [OPTIONS] INPUT
-        
-        Options:
-          --environment-name TEXT  The environment name  [required]
-          --app-name TEXT          The app name  [required]
-          --ssm-prefix TEXT        The ssm path prefix
-          --region TEXT            The AWS region
-          --encrypted TEXT         Do you want these parameters to be encrypted?
-          --delete-first           Delete the values in this path before pushing
-                                   (useful for cleanup)
-        
-          --help                   Show this message and exit.
-        ```
-        
-        #### put-parameters-recursive
-        
-        Recursively put parameters from a directory with the following structure
-        
-        ```
-        ├── EnvironmentName1
-        │   ├── AppName1.yaml
-        │   ├── AppName1.secret.yaml
-        │   ├── AppName2.yaml
-        │   └──AppName2.secret.yaml
-        └── EnvironmentName2
-            ├── AppName1.yaml
-            ├── AppName1.secret.yaml
-            ├── AppName2.yaml
-            └──AppName2.secret.yaml
-        ```
-        
-        Files with a *secret.yaml* or *secret.json* suffix will have the parameters encrypted in SSM.
-        
-        ```
-        Usage: cli.py put-parameters-recursive [OPTIONS] VALUES_PATH
-        
-        Options:
-          --ssm-prefix TEXT  The ssm path prefix
-          --region TEXT      The AWS region
-          --delete-first     Delete the values in this path before pushing (useful for
-                             cleanup)
-        
-          --help             Show this message and exit.
-        ```
-        
-        ## Nested file structure and environment variables
-        
-        Nested values will have their keys flattened when being converted to environment variables. This allows for a simpler structure than just adding all your env vars separately.
-        
-        For example:
-        
-        ```
-        SOME_VARIABLE: test
-        ANOTHER_VAR: 123
-        SOME_OTHER_VAR: foo
-        CONNECTIONS:
-          POSTGRESS:
-            HOST: somehost
-            PORT: 1234
-            USERNAME: someuser
-            PASSWORD: somepass
-        ```
-        
-        Would translate into the following environment variables:
-        
-        ```
-        SOME_VARIABLE="test"
-        ANOTHER_VAR="123"
-        SOME_OTHER_VAR="foo"
-        CONNECTIONS_POSTGRESS_HOST="somehost"
-        CONNECTIONS_POSTGRESS_PORT="1234"
-        CONNECTIONS_POSTGRESS_USERNAME="someuser"
-        CONNECTIONS_POSTGRESS_PASSWORD="somepass"
-        ```
-        
-        ## Usage in application code
-        
-        In the top of your application bootstrap file (or settings.py in django) add:
-        
-        ```
-        from croudtech_python_aws_app_config.ssm_config import SsmConfig
-        
-        ssm_config = SsmConfig(
-            environment_name=os.environ.get("ENVIRONMENT_NAME"), app_name=os.environ.get("APP_NAME")
-        )
-        ssm_config.params_to_env()
-        ```
-        
-        Make sure your ENVIRONMENT_NAME and APP_NAME env vars are set.
-        
-        This will pull values from SSM and inject them into your application environment variables.
-        
-        ## Contributing
-        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-        
-        
-        
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown; charset=UTF-8
+# croudtech-python-aws-app-config
+
+croudtech-python-aws-app-config us a utility to help manage application config using the AWS SSM Parameter Store
+
+There is a cli tool to help set the values and a utility to use the SSM parameters within you application.
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install croudtech-python-aws-app-config.
+
+```bash
+pip install croudtech-python-aws-app-config
+```
+
+## Command Line Usage
+
+```
+Usage: cli.py [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --debug / --no-debug
+  --endpoint-url TEXT
+  --help                Show this message and exit.
+
+Commands:
+  delete-parameters
+  get-arns
+  get-parameters
+  put-parameters
+  put-parameters-recursive
+  manage-redis
+```
+
+--endpoint-url specified the AWS API endpoint URL used. This should be used if using localstack or a similar aws mock service. You can also set the `AWS_ENDPOINT_URL` env var to enable this feature.
+
+### Sub Commands
+
+#### delete-parameters
+
+Delete parameters from SSM for a specified app and environment
+
+```
+Usage: cli.py delete-parameters [OPTIONS]
+
+Options:
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The app name  [required]
+  --ssm-prefix TEXT        The ssm path prefix
+  --region TEXT            The AWS region
+  --help                   Show this message and exit.
+```
+
+#### get-arns
+
+Get ARNs for published parameters
+
+```
+Usage: cli.py get-arns [OPTIONS]
+
+Options:
+  --environment-name TEXT         The environment name  [required]
+  --app-name TEXT                 The app name  [required]
+  --ssm-prefix TEXT               The ssm path prefix
+  --region TEXT                   The AWS region
+  --include-common / --ignore-common
+                                  Include shared variables
+  --output-format [ecs]
+  --help                          Show this message and exit.
+```
+
+#### get-parameters
+
+Get parameters for a specific app and environment
+
+```
+Usage: cli.py get-parameters [OPTIONS]
+
+Options:
+  --environment-name TEXT         The environment name  [required]
+  --app-name TEXT                 The app name  [required]
+  --ssm-prefix TEXT               The ssm path prefix
+  --region TEXT                   The AWS region
+  --include-common / --ignore-common
+                                  Include shared variables
+  --output-format [json|yaml|environment|environment-export]
+  --help                          Show this message and exit.
+```
+
+You can export the variables to your local shell by using
+
+```
+eval $(croudtech-app-config get-parameters --app-name myapp --environment-name myenv --output-format environment-export)
+```
+#### put-parameters
+
+INPUT should be the path to a yaml or json file
+
+```
+Usage: cli.py put-parameters [OPTIONS] INPUT
+
+Options:
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The app name  [required]
+  --ssm-prefix TEXT        The ssm path prefix
+  --region TEXT            The AWS region
+  --encrypted TEXT         Do you want these parameters to be encrypted?
+  --delete-first           Delete the values in this path before pushing
+                           (useful for cleanup)
+
+  --help                   Show this message and exit.
+```
+
+#### put-parameters-recursive
+
+Recursively put parameters from a directory with the following structure
+
+```
+├── EnvironmentName1
+│   ├── AppName1.yaml
+│   ├── AppName1.secret.yaml
+│   ├── AppName2.yaml
+│   └──AppName2.secret.yaml
+└── EnvironmentName2
+    ├── AppName1.yaml
+    ├── AppName1.secret.yaml
+    ├── AppName2.yaml
+    └──AppName2.secret.yaml
+```
+
+Files with a *secret.yaml* or *secret.json* suffix will have the parameters encrypted in SSM.
+
+```
+Usage: cli.py put-parameters-recursive [OPTIONS] VALUES_PATH
+
+Options:
+  --ssm-prefix TEXT  The ssm path prefix
+  --region TEXT      The AWS region
+  --delete-first     Delete the values in this path before pushing (useful for
+                     cleanup)
+
+  --help             Show this message and exit.
+```
+
+## Managing Redis DB Allocation
+
+Manage redis DB allocation
+
+### Sub commands
+
+#### allocate-db
+
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis allocate-db
+           [OPTIONS]
+
+  Allocate a Redis database for a specified application and environment
+
+Options:
+  --redis-host TEXT        The redis host  [required]
+  --redis-port INTEGER     The redis port  [required]
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The application name  [required]
+  --help                   Show this message and exit.
+```
+
+#### deallocate-db
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis deallocate-db
+           [OPTIONS]
+
+  Remove Redis database allocation for the specified application and
+  environment
+
+Options:
+  --redis-host TEXT        The redis host  [required]
+  --redis-port INTEGER     The redis port  [required]
+  --environment-name TEXT  The environment name  [required]
+  --app-name TEXT          The application name  [required]
+  --help                   Show this message and exit.
+```
+#### show-db
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis show-db
+           [OPTIONS]
+
+  Show Allocated Redis Database for a specified application
+
+Options:
+  --environment-name TEXT         The environment name  [required]
+  --app-name TEXT                 The app name  [required]
+  --ssm-prefix TEXT               The ssm path prefix
+  --region TEXT                   The AWS region
+  --include-common / --ignore-common
+                                  Include shared variables
+  --help                          Show this message and exit.
+```
+#### show-dbs
+```
+Usage: python -m croudtech_python_aws_app_config.cli manage-redis show-dbs
+           [OPTIONS]
+
+  Show all allocated Redis databases
+
+Options:
+  --redis-host TEXT     The redis host  [required]
+  --redis-port INTEGER  The redis port  [required]
+  --help                Show this message and exit.
+```
+
+## Nested file structure and environment variables
+
+Nested values will have their keys flattened when being converted to environment variables. This allows for a simpler structure than just adding all your env vars separately.
+
+For example:
+
+```
+SOME_VARIABLE: test
+ANOTHER_VAR: 123
+SOME_OTHER_VAR: foo
+CONNECTIONS:
+  POSTGRESS:
+    HOST: somehost
+    PORT: 1234
+    USERNAME: someuser
+    PASSWORD: somepass
+```
+
+Would translate into the following environment variables:
+
+```
+SOME_VARIABLE="test"
+ANOTHER_VAR="123"
+SOME_OTHER_VAR="foo"
+CONNECTIONS_POSTGRESS_HOST="somehost"
+CONNECTIONS_POSTGRESS_PORT="1234"
+CONNECTIONS_POSTGRESS_USERNAME="someuser"
+CONNECTIONS_POSTGRESS_PASSWORD="somepass"
+```
+
+## Usage in application code
+
+In the top of your application bootstrap file (or settings.py in django) add:
+
+```
+from croudtech_python_aws_app_config.ssm_config import SsmConfig
+
+ssm_config = SsmConfig(
+    environment_name=os.environ.get("ENVIRONMENT_NAME"), app_name=os.environ.get("APP_NAME")
+)
+ssm_config.params_to_env()
+```
+
+Make sure your ENVIRONMENT_NAME and APP_NAME env vars are set.
+
+This will pull values from SSM and inject them into your application environment variables.
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+
```

### Comparing `croudtech-python-aws-app-config-1.1.8/Pipfile.lock` & `croudtech_python_aws_app_config-2.0.0/Pipfile.lock`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8107029727095516%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'be115d1fc44352465febc0d3273e7f40a9eade2d230a30f1456abee21c922fa7'}, 'requires': "*

 * *            "{'python_version': '3.12'}}",*

 * * "'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:2824e3dd18743ca50e5b10439d20e74647b1416e8a94509cb30beac92d27a18d', "*

 * *              "'sha256:b2e5cb5b95efcc881e25a3bc872d7a24e75ff4e76f368138e4baf7b9d6ee3422'], "*

 * *              '\'version\': \'==1.34.90\', \'markers\': "python_version >= \'3.8\'"}, '*

 * *              "'botocore': […]*

```diff
@@ -1,380 +1,483 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "cf00fcb5b777681e36c3ca806e013fc65c08776aa159d0eeb6baa2895ba99115"
+            "sha256": "be115d1fc44352465febc0d3273e7f40a9eade2d230a30f1456abee21c922fa7"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.8"
+            "python_version": "3.12"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
+        "async-timeout": {
+            "hashes": [
+                "sha256:4640d96be84d82d02ed59ea2b7105a0f7b33abe8703703cd0ab0bf87c427522f",
+                "sha256:7405140ff1230c310e51dc27b3145b9092d659ce68ff733fb0cefe3ee42be028"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==4.0.3"
+        },
         "boto3": {
             "hashes": [
-                "sha256:19cff13dd9b51ce66fad13c9f04ffcc12d5475dd8cd660e8cd6aac42aa45c24c",
-                "sha256:7ed86cc669bcfa60ef854cc2fbc2d300a8331fb1befdc7eabc51ce013659e86c"
+                "sha256:2824e3dd18743ca50e5b10439d20e74647b1416e8a94509cb30beac92d27a18d",
+                "sha256:b2e5cb5b95efcc881e25a3bc872d7a24e75ff4e76f368138e4baf7b9d6ee3422"
             ],
             "index": "pypi",
-            "version": "==1.18.8"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.34.90"
         },
         "botocore": {
             "hashes": [
-                "sha256:437cdcd518e6f9db72ec87f170cc66d54081c8abc347abb9f9a3cd9c8e993bd1",
-                "sha256:e51ac230169af1325ab64c9935e679fb54f6d3fdf0978fe67a31931febdf94f9"
+                "sha256:113cd4c0cb63e13163ccbc2bb13d551be314ba7f8ba5bfab1c51a19ca01aa133",
+                "sha256:d48f152498e2c60b43ce25b579d26642346a327b6fb2c632d57219e0a4f63392"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.21.8"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.34.90"
         },
         "bson": {
             "hashes": [
                 "sha256:d6511b2ab051139a9123c184de1a04227262173ad593429d21e443d6462d6590"
             ],
             "index": "pypi",
             "version": "==0.5.10"
         },
+        "certifi": {
+            "hashes": [
+                "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
+                "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==2024.2.2"
+        },
+        "charset-normalizer": {
+            "hashes": [
+                "sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027",
+                "sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087",
+                "sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786",
+                "sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8",
+                "sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09",
+                "sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185",
+                "sha256:1ceae2f17a9c33cb48e3263960dc5fc8005351ee19db217e9b1bb15d28c02574",
+                "sha256:1d3193f4a680c64b4b6a9115943538edb896edc190f0b222e73761716519268e",
+                "sha256:1f79682fbe303db92bc2b1136016a38a42e835d932bab5b3b1bfcfbf0640e519",
+                "sha256:2127566c664442652f024c837091890cb1942c30937add288223dc895793f898",
+                "sha256:22afcb9f253dac0696b5a4be4a1c0f8762f8239e21b99680099abd9b2b1b2269",
+                "sha256:25baf083bf6f6b341f4121c2f3c548875ee6f5339300e08be3f2b2ba1721cdd3",
+                "sha256:2e81c7b9c8979ce92ed306c249d46894776a909505d8f5a4ba55b14206e3222f",
+                "sha256:3287761bc4ee9e33561a7e058c72ac0938c4f57fe49a09eae428fd88aafe7bb6",
+                "sha256:34d1c8da1e78d2e001f363791c98a272bb734000fcef47a491c1e3b0505657a8",
+                "sha256:37e55c8e51c236f95b033f6fb391d7d7970ba5fe7ff453dad675e88cf303377a",
+                "sha256:3d47fa203a7bd9c5b6cee4736ee84ca03b8ef23193c0d1ca99b5089f72645c73",
+                "sha256:3e4d1f6587322d2788836a99c69062fbb091331ec940e02d12d179c1d53e25fc",
+                "sha256:42cb296636fcc8b0644486d15c12376cb9fa75443e00fb25de0b8602e64c1714",
+                "sha256:45485e01ff4d3630ec0d9617310448a8702f70e9c01906b0d0118bdf9d124cf2",
+                "sha256:4a78b2b446bd7c934f5dcedc588903fb2f5eec172f3d29e52a9096a43722adfc",
+                "sha256:4ab2fe47fae9e0f9dee8c04187ce5d09f48eabe611be8259444906793ab7cbce",
+                "sha256:4d0d1650369165a14e14e1e47b372cfcb31d6ab44e6e33cb2d4e57265290044d",
+                "sha256:549a3a73da901d5bc3ce8d24e0600d1fa85524c10287f6004fbab87672bf3e1e",
+                "sha256:55086ee1064215781fff39a1af09518bc9255b50d6333f2e4c74ca09fac6a8f6",
+                "sha256:572c3763a264ba47b3cf708a44ce965d98555f618ca42c926a9c1616d8f34269",
+                "sha256:573f6eac48f4769d667c4442081b1794f52919e7edada77495aaed9236d13a96",
+                "sha256:5b4c145409bef602a690e7cfad0a15a55c13320ff7a3ad7ca59c13bb8ba4d45d",
+                "sha256:6463effa3186ea09411d50efc7d85360b38d5f09b870c48e4600f63af490e56a",
+                "sha256:65f6f63034100ead094b8744b3b97965785388f308a64cf8d7c34f2f2e5be0c4",
+                "sha256:663946639d296df6a2bb2aa51b60a2454ca1cb29835324c640dafb5ff2131a77",
+                "sha256:6897af51655e3691ff853668779c7bad41579facacf5fd7253b0133308cf000d",
+                "sha256:68d1f8a9e9e37c1223b656399be5d6b448dea850bed7d0f87a8311f1ff3dabb0",
+                "sha256:6ac7ffc7ad6d040517be39eb591cac5ff87416c2537df6ba3cba3bae290c0fed",
+                "sha256:6b3251890fff30ee142c44144871185dbe13b11bab478a88887a639655be1068",
+                "sha256:6c4caeef8fa63d06bd437cd4bdcf3ffefe6738fb1b25951440d80dc7df8c03ac",
+                "sha256:6ef1d82a3af9d3eecdba2321dc1b3c238245d890843e040e41e470ffa64c3e25",
+                "sha256:753f10e867343b4511128c6ed8c82f7bec3bd026875576dfd88483c5c73b2fd8",
+                "sha256:7cd13a2e3ddeed6913a65e66e94b51d80a041145a026c27e6bb76c31a853c6ab",
+                "sha256:7ed9e526742851e8d5cc9e6cf41427dfc6068d4f5a3bb03659444b4cabf6bc26",
+                "sha256:7f04c839ed0b6b98b1a7501a002144b76c18fb1c1850c8b98d458ac269e26ed2",
+                "sha256:802fe99cca7457642125a8a88a084cef28ff0cf9407060f7b93dca5aa25480db",
+                "sha256:80402cd6ee291dcb72644d6eac93785fe2c8b9cb30893c1af5b8fdd753b9d40f",
+                "sha256:8465322196c8b4d7ab6d1e049e4c5cb460d0394da4a27d23cc242fbf0034b6b5",
+                "sha256:86216b5cee4b06df986d214f664305142d9c76df9b6512be2738aa72a2048f99",
+                "sha256:87d1351268731db79e0f8e745d92493ee2841c974128ef629dc518b937d9194c",
+                "sha256:8bdb58ff7ba23002a4c5808d608e4e6c687175724f54a5dade5fa8c67b604e4d",
+                "sha256:8c622a5fe39a48f78944a87d4fb8a53ee07344641b0562c540d840748571b811",
+                "sha256:8d756e44e94489e49571086ef83b2bb8ce311e730092d2c34ca8f7d925cb20aa",
+                "sha256:8f4a014bc36d3c57402e2977dada34f9c12300af536839dc38c0beab8878f38a",
+                "sha256:9063e24fdb1e498ab71cb7419e24622516c4a04476b17a2dab57e8baa30d6e03",
+                "sha256:90d558489962fd4918143277a773316e56c72da56ec7aa3dc3dbbe20fdfed15b",
+                "sha256:923c0c831b7cfcb071580d3f46c4baf50f174be571576556269530f4bbd79d04",
+                "sha256:95f2a5796329323b8f0512e09dbb7a1860c46a39da62ecb2324f116fa8fdc85c",
+                "sha256:96b02a3dc4381e5494fad39be677abcb5e6634bf7b4fa83a6dd3112607547001",
+                "sha256:9f96df6923e21816da7e0ad3fd47dd8f94b2a5ce594e00677c0013018b813458",
+                "sha256:a10af20b82360ab00827f916a6058451b723b4e65030c5a18577c8b2de5b3389",
+                "sha256:a50aebfa173e157099939b17f18600f72f84eed3049e743b68ad15bd69b6bf99",
+                "sha256:a981a536974bbc7a512cf44ed14938cf01030a99e9b3a06dd59578882f06f985",
+                "sha256:a9a8e9031d613fd2009c182b69c7b2c1ef8239a0efb1df3f7c8da66d5dd3d537",
+                "sha256:ae5f4161f18c61806f411a13b0310bea87f987c7d2ecdbdaad0e94eb2e404238",
+                "sha256:aed38f6e4fb3f5d6bf81bfa990a07806be9d83cf7bacef998ab1a9bd660a581f",
+                "sha256:b01b88d45a6fcb69667cd6d2f7a9aeb4bf53760d7fc536bf679ec94fe9f3ff3d",
+                "sha256:b261ccdec7821281dade748d088bb6e9b69e6d15b30652b74cbbac25e280b796",
+                "sha256:b2b0a0c0517616b6869869f8c581d4eb2dd83a4d79e0ebcb7d373ef9956aeb0a",
+                "sha256:b4a23f61ce87adf89be746c8a8974fe1c823c891d8f86eb218bb957c924bb143",
+                "sha256:bd8f7df7d12c2db9fab40bdd87a7c09b1530128315d047a086fa3ae3435cb3a8",
+                "sha256:beb58fe5cdb101e3a055192ac291b7a21e3b7ef4f67fa1d74e331a7f2124341c",
+                "sha256:c002b4ffc0be611f0d9da932eb0f704fe2602a9a949d1f738e4c34c75b0863d5",
+                "sha256:c083af607d2515612056a31f0a8d9e0fcb5876b7bfc0abad3ecd275bc4ebc2d5",
+                "sha256:c180f51afb394e165eafe4ac2936a14bee3eb10debc9d9e4db8958fe36afe711",
+                "sha256:c235ebd9baae02f1b77bcea61bce332cb4331dc3617d254df3323aa01ab47bd4",
+                "sha256:cd70574b12bb8a4d2aaa0094515df2463cb429d8536cfb6c7ce983246983e5a6",
+                "sha256:d0eccceffcb53201b5bfebb52600a5fb483a20b61da9dbc885f8b103cbe7598c",
+                "sha256:d965bba47ddeec8cd560687584e88cf699fd28f192ceb452d1d7ee807c5597b7",
+                "sha256:db364eca23f876da6f9e16c9da0df51aa4f104a972735574842618b8c6d999d4",
+                "sha256:ddbb2551d7e0102e7252db79ba445cdab71b26640817ab1e3e3648dad515003b",
+                "sha256:deb6be0ac38ece9ba87dea880e438f25ca3eddfac8b002a2ec3d9183a454e8ae",
+                "sha256:e06ed3eb3218bc64786f7db41917d4e686cc4856944f53d5bdf83a6884432e12",
+                "sha256:e27ad930a842b4c5eb8ac0016b0a54f5aebbe679340c26101df33424142c143c",
+                "sha256:e537484df0d8f426ce2afb2d0f8e1c3d0b114b83f8850e5f2fbea0e797bd82ae",
+                "sha256:eb00ed941194665c332bf8e078baf037d6c35d7c4f3102ea2d4f16ca94a26dc8",
+                "sha256:eb6904c354526e758fda7167b33005998fb68c46fbc10e013ca97f21ca5c8887",
+                "sha256:eb8821e09e916165e160797a6c17edda0679379a4be5c716c260e836e122f54b",
+                "sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4",
+                "sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f",
+                "sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5",
+                "sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33",
+                "sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519",
+                "sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561"
+            ],
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.3.2"
+        },
         "click": {
             "hashes": [
-                "sha256:8c04c11192119b1ef78ea049e0a6f0463e4c48ef00a30160c704337586f3ad7a",
-                "sha256:fba402a4a47334742d782209a7c79bc448911afe1149d07bdabdf480b3e2f4b6"
+                "sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28",
+                "sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de"
             ],
             "index": "pypi",
-            "version": "==8.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.1.7"
         },
         "http-status-codes": {
             "hashes": [
                 "sha256:139ccd38af7debc9fc46b876788a08239f3e1be477e5a281555371c6867cf3b2",
                 "sha256:6587d0fc0dc646eeacf14446fe0567981cf6182337708a011c17946f85f632d6"
             ],
             "index": "pypi",
+            "markers": "python_full_version >= '3.6.0'",
             "version": "==1.0.3"
         },
+        "idna": {
+            "hashes": [
+                "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc",
+                "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==3.7"
+        },
         "jmespath": {
             "hashes": [
-                "sha256:b85d0567b8666149a93172712e68920734333c0ce7e89b78b3e987f71e5ed4f9",
-                "sha256:cdf6525904cc597730141d61b36f2e4b8ecc257c420fa2f4549bac2c2d0cb72f"
+                "sha256:02e2e4cc71b5bcab88332eebf907519190dd9e6e82107fa7f83b1003a6252980",
+                "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
-            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.0.1"
         },
         "loguru": {
             "hashes": [
-                "sha256:b28e72ac7a98be3d28ad28570299a393dfcd32e5e3f6a353dec94675767b6319",
-                "sha256:f8087ac396b5ee5f67c963b495d615ebbceac2796379599820e324419d53667c"
+                "sha256:003d71e3d3ed35f0f8984898359d65b79e5b21943f78af86aa5491210429b8eb",
+                "sha256:e671a53522515f34fd406340ee968cb9ecafbc4b36c679da03c18fd8d0bd51ac"
             ],
             "index": "pypi",
-            "version": "==0.5.3"
+            "markers": "python_version >= '3.5'",
+            "version": "==0.7.2"
         },
         "pyaml": {
             "hashes": [
-                "sha256:29a5c2a68660a799103d6949167bd6c7953d031449d08802386372de1db6ad71",
-                "sha256:67081749a82b72c45e5f7f812ee3a14a03b3f5c25ff36ec3b290514f8c4c4b99"
+                "sha256:0e483d9289010e747a325dc43171bcc39d6562dd1dd4719e8cc7e7c96c99fce6",
+                "sha256:acc2b39c55cb0cbe4f694a6d3886f89ad3d2a5b3efcece526202f8de9a6b27de"
             ],
             "index": "pypi",
-            "version": "==20.4.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==24.4.0"
         },
         "python-dateutil": {
             "hashes": [
-                "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
-                "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
+                "sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3",
+                "sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.8.2"
+            "version": "==2.9.0.post0"
         },
         "pyyaml": {
             "hashes": [
-                "sha256:08682f6b72c722394747bddaf0aa62277e02557c0fd1c42cb853016a38f8dedf",
-                "sha256:0f5f5786c0e09baddcd8b4b45f20a7b5d61a7e7e99846e3c799b05c7c53fa696",
-                "sha256:129def1b7c1bf22faffd67b8f3724645203b79d8f4cc81f674654d9902cb4393",
-                "sha256:294db365efa064d00b8d1ef65d8ea2c3426ac366c0c4368d930bf1c5fb497f77",
-                "sha256:3b2b1824fe7112845700f815ff6a489360226a5609b96ec2190a45e62a9fc922",
-                "sha256:3bd0e463264cf257d1ffd2e40223b197271046d09dadf73a0fe82b9c1fc385a5",
-                "sha256:4465124ef1b18d9ace298060f4eccc64b0850899ac4ac53294547536533800c8",
-                "sha256:49d4cdd9065b9b6e206d0595fee27a96b5dd22618e7520c33204a4a3239d5b10",
-                "sha256:4e0583d24c881e14342eaf4ec5fbc97f934b999a6828693a99157fde912540cc",
-                "sha256:5accb17103e43963b80e6f837831f38d314a0495500067cb25afab2e8d7a4018",
-                "sha256:607774cbba28732bfa802b54baa7484215f530991055bb562efbed5b2f20a45e",
-                "sha256:6c78645d400265a062508ae399b60b8c167bf003db364ecb26dcab2bda048253",
-                "sha256:72a01f726a9c7851ca9bfad6fd09ca4e090a023c00945ea05ba1638c09dc3347",
-                "sha256:74c1485f7707cf707a7aef42ef6322b8f97921bd89be2ab6317fd782c2d53183",
-                "sha256:895f61ef02e8fed38159bb70f7e100e00f471eae2bc838cd0f4ebb21e28f8541",
-                "sha256:8c1be557ee92a20f184922c7b6424e8ab6691788e6d86137c5d93c1a6ec1b8fb",
-                "sha256:bb4191dfc9306777bc594117aee052446b3fa88737cd13b7188d0e7aa8162185",
-                "sha256:bfb51918d4ff3d77c1c856a9699f8492c612cde32fd3bcd344af9be34999bfdc",
-                "sha256:c20cfa2d49991c8b4147af39859b167664f2ad4561704ee74c1de03318e898db",
-                "sha256:cb333c16912324fd5f769fff6bc5de372e9e7a202247b48870bc251ed40239aa",
-                "sha256:d2d9808ea7b4af864f35ea216be506ecec180628aced0704e34aca0b040ffe46",
-                "sha256:d483ad4e639292c90170eb6f7783ad19490e7a8defb3e46f97dfe4bacae89122",
-                "sha256:dd5de0646207f053eb0d6c74ae45ba98c3395a571a2891858e87df7c9b9bd51b",
-                "sha256:e1d4970ea66be07ae37a3c2e48b5ec63f7ba6804bdddfdbd3cfd954d25a82e63",
-                "sha256:e4fac90784481d221a8e4b1162afa7c47ed953be40d31ab4629ae917510051df",
-                "sha256:fa5ae20527d8e831e8230cbffd9f8fe952815b2b7dae6ffec25318803a7528fc",
-                "sha256:fd7f6999a8070df521b6384004ef42833b9bd62cfee11a09bda1079b4b704247",
-                "sha256:fdc842473cd33f45ff6bce46aea678a54e3d21f1b61a7750ce3c498eedfe25d6",
-                "sha256:fe69978f3f768926cfa37b867e3843918e012cf83f680806599ddce33c2c68b0"
+                "sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5",
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:326c013efe8048858a6d312ddd31d56e468118ad4cdeda36c719bf5bb6192290",
+                "sha256:40df9b996c2b73138957fe23a16a4f0ba614f4c0efce1e9406a184b6d07fa3a9",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:49a183be227561de579b4a36efbb21b3eab9651dd81b1858589f796549873dd6",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:6c22bec3fbe2524cde73d7ada88f6566758a8f7227bfbf93a408a9d86bcc12a0",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28",
+                "sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d483d2cdf104e7c9fa60c544d92981f12ad66a457afae824d146093b8c294c54",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "index": "pypi",
-            "version": "==5.4.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==6.0.1"
         },
         "redis": {
             "hashes": [
-                "sha256:0e7e0cfca8660dea8b7d5cd8c4f6c5e29e11f31158c0b0ae91a397f00e5a05a2",
-                "sha256:432b788c4530cfe16d8d943a09d40ca6c16149727e4afe8c2c9d5580c59d9f24"
+                "sha256:8a74fae7cbd25493142c8cc2f79c21b2e3c03bf85dd3525a1db9f33ff47a3f2d",
+                "sha256:9cac9a8ce8926a61f2dd81992978ffccd98a2bd065ac97694d49d28e7c928b59"
+            ],
+            "index": "pypi",
+            "markers": "python_version >= '3.8'",
+            "version": "==5.1.0b4"
+        },
+        "requests": {
+            "hashes": [
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==3.5.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "s3transfer": {
             "hashes": [
-                "sha256:50ed823e1dc5868ad40c8dc92072f757aa0e653a192845c94a3b676f4a62da4c",
-                "sha256:9c1dc369814391a6bda20ebbf4b70a0f34630592c9aa520856bf384916af2803"
+                "sha256:5683916b4c724f799e600f41dd9e10a9ff19871bf87623cc8f491cb4f5fa0a19",
+                "sha256:ceb252b11bcf87080fb7850a224fb6e05c8a776bab8f2b64b7f25b969464839d"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.5.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==0.10.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:39fb8672126159acb139a7718dd10806104dec1e2f0f6c88aab05d17df10c8d4",
-                "sha256:f57b4c16c62fa2760b7e3d97c35b255512fb6b59a259730f36ba32ce9f8e342f"
+                "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d",
+                "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.6"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.2.1"
         }
     },
     "develop": {
-        "appdirs": {
-            "hashes": [
-                "sha256:7d5d0167b2b1ba821647616af46a749d1c653740dd0d2415100fe26e27afdf41",
-                "sha256:a841dacd6b99318a741b166adb07e19ee71a274450e68237b4650ca1055ab128"
-            ],
-            "version": "==1.4.4"
-        },
-        "attrs": {
-            "hashes": [
-                "sha256:149e90d6d8ac20db7a955ad60cf0e6881a3f20d37096140088356da6c716b0b1",
-                "sha256:ef6aaac3ca6cd92904cdd0d83f629a15f18053ec84e6432106f7a4d04ae4f5fb"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==21.2.0"
-        },
         "black": {
             "hashes": [
-                "sha256:1c7aa6ada8ee864db745b22790a32f94b2795c253a75d6d9b5e439ff10d23116",
-                "sha256:c8373c6491de9362e39271630b65b964607bc5c79c83783547d76c839b3aa219"
+                "sha256:1bb9ca06e556a09f7f7177bc7cb604e5ed2d2df1e9119e4f7d2f1f7071c32e5d",
+                "sha256:21f9407063ec71c5580b8ad975653c66508d6a9f57bd008bb8691d273705adcd",
+                "sha256:4396ca365a4310beef84d446ca5016f671b10f07abdba3e4e4304218d2c71d33",
+                "sha256:44d99dfdf37a2a00a6f7a8dcbd19edf361d056ee51093b2445de7ca09adac965",
+                "sha256:5cd5b4f76056cecce3e69b0d4c228326d2595f506797f40b9233424e2524c070",
+                "sha256:64578cf99b6b46a6301bc28bdb89f9d6f9b592b1c5837818a177c98525dbe397",
+                "sha256:64e60a7edd71fd542a10a9643bf369bfd2644de95ec71e86790b063aa02ff745",
+                "sha256:652e55bb722ca026299eb74e53880ee2315b181dfdd44dca98e43448620ddec1",
+                "sha256:6644f97a7ef6f401a150cca551a1ff97e03c25d8519ee0bbc9b0058772882665",
+                "sha256:6ad001a9ddd9b8dfd1b434d566be39b1cd502802c8d38bbb1ba612afda2ef436",
+                "sha256:71d998b73c957444fb7c52096c3843875f4b6b47a54972598741fe9a7f737fcb",
+                "sha256:74eb9b5420e26b42c00a3ff470dc0cd144b80a766128b1771d07643165e08d0e",
+                "sha256:75a2d0b4f5eb81f7eebc31f788f9830a6ce10a68c91fbe0fade34fff7a2836e6",
+                "sha256:7852b05d02b5b9a8c893ab95863ef8986e4dda29af80bbbda94d7aee1abf8702",
+                "sha256:7f2966b9b2b3b7104fca9d75b2ee856fe3fdd7ed9e47c753a4bb1a675f2caab8",
+                "sha256:8e5537f456a22cf5cfcb2707803431d2feeb82ab3748ade280d6ccd0b40ed2e8",
+                "sha256:d4e71cdebdc8efeb6deaf5f2deb28325f8614d48426bed118ecc2dcaefb9ebf3",
+                "sha256:dae79397f367ac8d7adb6c779813328f6d690943f64b32983e896bcccd18cbad",
+                "sha256:e3a3a092b8b756c643fe45f4624dbd5a389f770a4ac294cf4d0fce6af86addaf",
+                "sha256:eb949f56a63c5e134dfdca12091e98ffb5fd446293ebae123d10fc1abad00b9e",
+                "sha256:f07b69fda20578367eaebbd670ff8fc653ab181e1ff95d84497f9fa20e7d0641",
+                "sha256:f95cece33329dc4aa3b0e1a771c41075812e46cf3d6e3f1dfe3d91ff09826ed2"
             ],
             "index": "pypi",
-            "version": "==21.7b0"
+            "markers": "python_version >= '3.8'",
+            "version": "==24.4.0"
         },
         "click": {
             "hashes": [
-                "sha256:8c04c11192119b1ef78ea049e0a6f0463e4c48ef00a30160c704337586f3ad7a",
-                "sha256:fba402a4a47334742d782209a7c79bc448911afe1149d07bdabdf480b3e2f4b6"
+                "sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28",
+                "sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de"
             ],
             "index": "pypi",
-            "version": "==8.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.1.7"
         },
         "coverage": {
+            "extras": [
+                "toml"
+            ],
             "hashes": [
-                "sha256:004d1880bed2d97151facef49f08e255a20ceb6f9432df75f4eef018fdd5a78c",
-                "sha256:01d84219b5cdbfc8122223b39a954820929497a1cb1422824bb86b07b74594b6",
-                "sha256:040af6c32813fa3eae5305d53f18875bedd079960822ef8ec067a66dd8afcd45",
-                "sha256:06191eb60f8d8a5bc046f3799f8a07a2d7aefb9504b0209aff0b47298333302a",
-                "sha256:13034c4409db851670bc9acd836243aeee299949bd5673e11844befcb0149f03",
-                "sha256:13c4ee887eca0f4c5a247b75398d4114c37882658300e153113dafb1d76de529",
-                "sha256:184a47bbe0aa6400ed2d41d8e9ed868b8205046518c52464fde713ea06e3a74a",
-                "sha256:18ba8bbede96a2c3dde7b868de9dcbd55670690af0988713f0603f037848418a",
-                "sha256:1aa846f56c3d49205c952d8318e76ccc2ae23303351d9270ab220004c580cfe2",
-                "sha256:217658ec7187497e3f3ebd901afdca1af062b42cfe3e0dafea4cced3983739f6",
-                "sha256:24d4a7de75446be83244eabbff746d66b9240ae020ced65d060815fac3423759",
-                "sha256:2910f4d36a6a9b4214bb7038d537f015346f413a975d57ca6b43bf23d6563b53",
-                "sha256:2949cad1c5208b8298d5686d5a85b66aae46d73eec2c3e08c817dd3513e5848a",
-                "sha256:2a3859cb82dcbda1cfd3e6f71c27081d18aa251d20a17d87d26d4cd216fb0af4",
-                "sha256:2cafbbb3af0733db200c9b5f798d18953b1a304d3f86a938367de1567f4b5bff",
-                "sha256:2e0d881ad471768bf6e6c2bf905d183543f10098e3b3640fc029509530091502",
-                "sha256:30c77c1dc9f253283e34c27935fded5015f7d1abe83bc7821680ac444eaf7793",
-                "sha256:3487286bc29a5aa4b93a072e9592f22254291ce96a9fbc5251f566b6b7343cdb",
-                "sha256:372da284cfd642d8e08ef606917846fa2ee350f64994bebfbd3afb0040436905",
-                "sha256:41179b8a845742d1eb60449bdb2992196e211341818565abded11cfa90efb821",
-                "sha256:44d654437b8ddd9eee7d1eaee28b7219bec228520ff809af170488fd2fed3e2b",
-                "sha256:4a7697d8cb0f27399b0e393c0b90f0f1e40c82023ea4d45d22bce7032a5d7b81",
-                "sha256:51cb9476a3987c8967ebab3f0fe144819781fca264f57f89760037a2ea191cb0",
-                "sha256:52596d3d0e8bdf3af43db3e9ba8dcdaac724ba7b5ca3f6358529d56f7a166f8b",
-                "sha256:53194af30d5bad77fcba80e23a1441c71abfb3e01192034f8246e0d8f99528f3",
-                "sha256:5fec2d43a2cc6965edc0bb9e83e1e4b557f76f843a77a2496cbe719583ce8184",
-                "sha256:6c90e11318f0d3c436a42409f2749ee1a115cd8b067d7f14c148f1ce5574d701",
-                "sha256:74d881fc777ebb11c63736622b60cb9e4aee5cace591ce274fb69e582a12a61a",
-                "sha256:7501140f755b725495941b43347ba8a2777407fc7f250d4f5a7d2a1050ba8e82",
-                "sha256:796c9c3c79747146ebd278dbe1e5c5c05dd6b10cc3bcb8389dfdf844f3ead638",
-                "sha256:869a64f53488f40fa5b5b9dcb9e9b2962a66a87dab37790f3fcfb5144b996ef5",
-                "sha256:8963a499849a1fc54b35b1c9f162f4108017b2e6db2c46c1bed93a72262ed083",
-                "sha256:8d0a0725ad7c1a0bcd8d1b437e191107d457e2ec1084b9f190630a4fb1af78e6",
-                "sha256:900fbf7759501bc7807fd6638c947d7a831fc9fdf742dc10f02956ff7220fa90",
-                "sha256:92b017ce34b68a7d67bd6d117e6d443a9bf63a2ecf8567bb3d8c6c7bc5014465",
-                "sha256:970284a88b99673ccb2e4e334cfb38a10aab7cd44f7457564d11898a74b62d0a",
-                "sha256:972c85d205b51e30e59525694670de6a8a89691186012535f9d7dbaa230e42c3",
-                "sha256:9a1ef3b66e38ef8618ce5fdc7bea3d9f45f3624e2a66295eea5e57966c85909e",
-                "sha256:af0e781009aaf59e25c5a678122391cb0f345ac0ec272c7961dc5455e1c40066",
-                "sha256:b6d534e4b2ab35c9f93f46229363e17f63c53ad01330df9f2d6bd1187e5eaacf",
-                "sha256:b7895207b4c843c76a25ab8c1e866261bcfe27bfaa20c192de5190121770672b",
-                "sha256:c0891a6a97b09c1f3e073a890514d5012eb256845c451bd48f7968ef939bf4ae",
-                "sha256:c2723d347ab06e7ddad1a58b2a821218239249a9e4365eaff6649d31180c1669",
-                "sha256:d1f8bf7b90ba55699b3a5e44930e93ff0189aa27186e96071fac7dd0d06a1873",
-                "sha256:d1f9ce122f83b2305592c11d64f181b87153fc2c2bbd3bb4a3dde8303cfb1a6b",
-                "sha256:d314ed732c25d29775e84a960c3c60808b682c08d86602ec2c3008e1202e3bb6",
-                "sha256:d636598c8305e1f90b439dbf4f66437de4a5e3c31fdf47ad29542478c8508bbb",
-                "sha256:deee1077aae10d8fa88cb02c845cfba9b62c55e1183f52f6ae6a2df6a2187160",
-                "sha256:ebe78fe9a0e874362175b02371bdfbee64d8edc42a044253ddf4ee7d3c15212c",
-                "sha256:f030f8873312a16414c0d8e1a1ddff2d3235655a2174e3648b4fa66b3f2f1079",
-                "sha256:f0b278ce10936db1a37e6954e15a3730bea96a0997c26d7fee88e6c396c2086d",
-                "sha256:f11642dddbb0253cc8853254301b51390ba0081750a8ac03f20ea8103f0c56b6"
+                "sha256:075299460948cd12722a970c7eae43d25d37989da682997687b34ae6b87c0ef0",
+                "sha256:07dfdd492d645eea1bd70fb1d6febdcf47db178b0d99161d8e4eed18e7f62fe7",
+                "sha256:0cbdf2cae14a06827bec50bd58e49249452d211d9caddd8bd80e35b53cb04631",
+                "sha256:2055c4fb9a6ff624253d432aa471a37202cd8f458c033d6d989be4499aed037b",
+                "sha256:262fffc1f6c1a26125d5d573e1ec379285a3723363f3bd9c83923c9593a2ac25",
+                "sha256:280132aada3bc2f0fac939a5771db4fbb84f245cb35b94fae4994d4c1f80dae7",
+                "sha256:2b57780b51084d5223eee7b59f0d4911c31c16ee5aa12737c7a02455829ff067",
+                "sha256:2bd7065249703cbeb6d4ce679c734bef0ee69baa7bff9724361ada04a15b7e3b",
+                "sha256:3235d7c781232e525b0761730e052388a01548bd7f67d0067a253887c6e8df46",
+                "sha256:33c020d3322662e74bc507fb11488773a96894aa82a622c35a5a28673c0c26f5",
+                "sha256:357754dcdfd811462a725e7501a9b4556388e8ecf66e79df6f4b988fa3d0b39a",
+                "sha256:39793731182c4be939b4be0cdecde074b833f6171313cf53481f869937129ed3",
+                "sha256:3c2b77f295edb9fcdb6a250f83e6481c679335ca7e6e4a955e4290350f2d22a4",
+                "sha256:41327143c5b1d715f5f98a397608f90ab9ebba606ae4e6f3389c2145410c52b1",
+                "sha256:427e1e627b0963ac02d7c8730ca6d935df10280d230508c0ba059505e9233475",
+                "sha256:432949a32c3e3f820af808db1833d6d1631664d53dd3ce487aa25d574e18ad1c",
+                "sha256:4ba01d9ba112b55bfa4b24808ec431197bb34f09f66f7cb4fd0258ff9d3711b1",
+                "sha256:4d0e206259b73af35c4ec1319fd04003776e11e859936658cb6ceffdeba0f5be",
+                "sha256:51431d0abbed3a868e967f8257c5faf283d41ec882f58413cf295a389bb22e58",
+                "sha256:565b2e82d0968c977e0b0f7cbf25fd06d78d4856289abc79694c8edcce6eb2de",
+                "sha256:6782cd6216fab5a83216cc39f13ebe30adfac2fa72688c5a4d8d180cd52e8f6a",
+                "sha256:6afd2e84e7da40fe23ca588379f815fb6dbbb1b757c883935ed11647205111cb",
+                "sha256:710c62b6e35a9a766b99b15cdc56d5aeda0914edae8bb467e9c355f75d14ee95",
+                "sha256:84921b10aeb2dd453247fd10de22907984eaf80901b578a5cf0bb1e279a587cb",
+                "sha256:85a5dbe1ba1bf38d6c63b6d2c42132d45cbee6d9f0c51b52c59aa4afba057517",
+                "sha256:9c6384cc90e37cfb60435bbbe0488444e54b98700f727f16f64d8bfda0b84656",
+                "sha256:9dd88fce54abbdbf4c42fb1fea0e498973d07816f24c0e27a1ecaf91883ce69e",
+                "sha256:a81eb64feded34f40c8986869a2f764f0fe2db58c0530d3a4afbcde50f314880",
+                "sha256:a898c11dca8f8c97b467138004a30133974aacd572818c383596f8d5b2eb04a9",
+                "sha256:a9960dd1891b2ddf13a7fe45339cd59ecee3abb6b8326d8b932d0c5da208104f",
+                "sha256:a9a7ef30a1b02547c1b23fa9a5564f03c9982fc71eb2ecb7f98c96d7a0db5cf2",
+                "sha256:ad97ec0da94b378e593ef532b980c15e377df9b9608c7c6da3506953182398af",
+                "sha256:adf032b6c105881f9d77fa17d9eebe0ad1f9bfb2ad25777811f97c5362aa07f2",
+                "sha256:bbfe6389c5522b99768a93d89aca52ef92310a96b99782973b9d11e80511f932",
+                "sha256:bd4bacd62aa2f1a1627352fe68885d6ee694bdaebb16038b6e680f2924a9b2cc",
+                "sha256:bf0b4b8d9caa8d64df838e0f8dcf68fb570c5733b726d1494b87f3da85db3a2d",
+                "sha256:c379cdd3efc0658e652a14112d51a7668f6bfca7445c5a10dee7eabecabba19d",
+                "sha256:c58536f6892559e030e6924896a44098bc1290663ea12532c78cef71d0df8493",
+                "sha256:cbe6581fcff7c8e262eb574244f81f5faaea539e712a058e6707a9d272fe5b64",
+                "sha256:ced268e82af993d7801a9db2dbc1d2322e786c5dc76295d8e89473d46c6b84d4",
+                "sha256:cf3539007202ebfe03923128fedfdd245db5860a36810136ad95a564a2fdffff",
+                "sha256:cf62d17310f34084c59c01e027259076479128d11e4661bb6c9acb38c5e19bb8",
+                "sha256:d0194d654e360b3e6cc9b774e83235bae6b9b2cac3be09040880bb0e8a88f4a1",
+                "sha256:d3d117890b6eee85887b1eed41eefe2e598ad6e40523d9f94c4c4b213258e4a4",
+                "sha256:db2de4e546f0ec4b2787d625e0b16b78e99c3e21bc1722b4977c0dddf11ca84e",
+                "sha256:e768d870801f68c74c2b669fc909839660180c366501d4cc4b87efd6b0eee375",
+                "sha256:e7c211f25777746d468d76f11719e64acb40eed410d81c26cefac641975beb88",
+                "sha256:eed462b4541c540d63ab57b3fc69e7d8c84d5957668854ee4e408b50e92ce26a",
+                "sha256:f0bfe42523893c188e9616d853c47685e1c575fe25f737adf473d0405dcfa7eb",
+                "sha256:f609ebcb0242d84b7adeee2b06c11a2ddaec5464d21888b2c8255f5fd6a98ae4",
+                "sha256:fea9d3ca80bcf17edb2c08a4704259dadac196fe5e9274067e7a20511fad1743",
+                "sha256:fed7a72d54bd52f4aeb6c6e951f363903bd7d70bc1cad64dd1f087980d309ab9"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==5.5"
+            "markers": "python_version >= '3.8'",
+            "version": "==7.5.0"
         },
         "iniconfig": {
             "hashes": [
-                "sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3",
-                "sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32"
+                "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
+                "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
-            "version": "==1.1.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.0"
         },
         "mypy-extensions": {
             "hashes": [
-                "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d",
-                "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"
+                "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
+                "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
-            "version": "==0.4.3"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:7dc96269f53a4ccec5c0670940a4281106dd0bb343f47b7471f779df49c2fbe7",
-                "sha256:c86254f9220d55e31cc94d69bade760f0847da8000def4dfe1c6b872fd14ff14"
+                "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==21.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==24.0"
         },
         "pathspec": {
             "hashes": [
-                "sha256:7d15c4ddb0b5c802d161efc417ec1a2558ea2653c2e8ad9c19098201dc1c993a",
-                "sha256:e564499435a2673d586f6b2130bb5b95f04a3ba06f81b8f895b651a3c76aabb1"
+                "sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08",
+                "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"
             ],
-            "version": "==0.9.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==0.12.1"
         },
-        "pluggy": {
+        "platformdirs": {
             "hashes": [
-                "sha256:15b2acde666561e1298d71b523007ed7364de07029219b604cf808bfa1c765b0",
-                "sha256:966c145cd83c96502c3c3868f50408687b38434af77734af1e9ca461a4081d2d"
+                "sha256:031cd18d4ec63ec53e82dceaac0417d218a6863f7745dfcc9efe7793b7039bdf",
+                "sha256:17d5a1161b3fd67b390023cb2d3b026bbd40abde6fdb052dfbd3a29c3ba22ee1"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.13.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==4.2.1"
         },
-        "py": {
-            "hashes": [
-                "sha256:21b81bda15b66ef5e1a777a21c4dcd9c20ad3efd0b3f817e7a809035269e1bd3",
-                "sha256:3b80836aa6d1feeaa108e046da6423ab8f6ceda6468545ae8d02d9d58d18818a"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.10.0"
-        },
-        "pyparsing": {
+        "pluggy": {
             "hashes": [
-                "sha256:c203ec8783bf771a155b207279b9bccb8dea02d8f0c9e5f8ead507bc3246ecc1",
-                "sha256:ef9d7589ef3c200abe66653d3f1ab1033c3c419ae9b9bdb1240a85b024efc88b"
+                "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1",
+                "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"
             ],
-            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.4.7"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.5.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:50bcad0a0b9c5a72c8e4e7c9855a3ad496ca6a881a3641b4260605450772c54b",
-                "sha256:91ef2131a9bd6be8f76f1f08eac5c5317221d6ad1e143ae03894b862e8976890"
+                "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7",
+                "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"
             ],
             "index": "pypi",
-            "version": "==6.2.4"
+            "markers": "python_version >= '3.8'",
+            "version": "==8.1.1"
         },
         "pytest-cov": {
             "hashes": [
-                "sha256:261bb9e47e65bd099c89c3edf92972865210c36813f80ede5277dceb77a4a62a",
-                "sha256:261ceeb8c227b726249b376b8526b600f38667ee314f910353fa318caa01f4d7"
+                "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652",
+                "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"
             ],
             "index": "pypi",
-            "version": "==2.12.1"
-        },
-        "regex": {
-            "hashes": [
-                "sha256:0eb2c6e0fcec5e0f1d3bcc1133556563222a2ffd2211945d7b1480c1b1a42a6f",
-                "sha256:15dddb19823f5147e7517bb12635b3c82e6f2a3a6b696cc3e321522e8b9308ad",
-                "sha256:173bc44ff95bc1e96398c38f3629d86fa72e539c79900283afa895694229fe6a",
-                "sha256:1c78780bf46d620ff4fff40728f98b8afd8b8e35c3efd638c7df67be2d5cddbf",
-                "sha256:2366fe0479ca0e9afa534174faa2beae87847d208d457d200183f28c74eaea59",
-                "sha256:2bceeb491b38225b1fee4517107b8491ba54fba77cf22a12e996d96a3c55613d",
-                "sha256:2ddeabc7652024803666ea09f32dd1ed40a0579b6fbb2a213eba590683025895",
-                "sha256:2fe5e71e11a54e3355fa272137d521a40aace5d937d08b494bed4529964c19c4",
-                "sha256:319eb2a8d0888fa6f1d9177705f341bc9455a2c8aca130016e52c7fe8d6c37a3",
-                "sha256:3f5716923d3d0bfb27048242a6e0f14eecdb2e2a7fac47eda1d055288595f222",
-                "sha256:422dec1e7cbb2efbbe50e3f1de36b82906def93ed48da12d1714cabcd993d7f0",
-                "sha256:4c9c3155fe74269f61e27617529b7f09552fbb12e44b1189cebbdb24294e6e1c",
-                "sha256:4f64fc59fd5b10557f6cd0937e1597af022ad9b27d454e182485f1db3008f417",
-                "sha256:564a4c8a29435d1f2256ba247a0315325ea63335508ad8ed938a4f14c4116a5d",
-                "sha256:59506c6e8bd9306cd8a41511e32d16d5d1194110b8cfe5a11d102d8b63cf945d",
-                "sha256:598c0a79b4b851b922f504f9f39a863d83ebdfff787261a5ed061c21e67dd761",
-                "sha256:59c00bb8dd8775473cbfb967925ad2c3ecc8886b3b2d0c90a8e2707e06c743f0",
-                "sha256:6110bab7eab6566492618540c70edd4d2a18f40ca1d51d704f1d81c52d245026",
-                "sha256:6afe6a627888c9a6cfbb603d1d017ce204cebd589d66e0703309b8048c3b0854",
-                "sha256:791aa1b300e5b6e5d597c37c346fb4d66422178566bbb426dd87eaae475053fb",
-                "sha256:8394e266005f2d8c6f0bc6780001f7afa3ef81a7a2111fa35058ded6fce79e4d",
-                "sha256:875c355360d0f8d3d827e462b29ea7682bf52327d500a4f837e934e9e4656068",
-                "sha256:89e5528803566af4df368df2d6f503c84fbfb8249e6631c7b025fe23e6bd0cde",
-                "sha256:99d8ab206a5270c1002bfcf25c51bf329ca951e5a169f3b43214fdda1f0b5f0d",
-                "sha256:9a854b916806c7e3b40e6616ac9e85d3cdb7649d9e6590653deb5b341a736cec",
-                "sha256:b85ac458354165405c8a84725de7bbd07b00d9f72c31a60ffbf96bb38d3e25fa",
-                "sha256:bc84fb254a875a9f66616ed4538542fb7965db6356f3df571d783f7c8d256edd",
-                "sha256:c92831dac113a6e0ab28bc98f33781383fe294df1a2c3dfd1e850114da35fd5b",
-                "sha256:cbe23b323988a04c3e5b0c387fe3f8f363bf06c0680daf775875d979e376bd26",
-                "sha256:ccb3d2190476d00414aab36cca453e4596e8f70a206e2aa8db3d495a109153d2",
-                "sha256:d8bbce0c96462dbceaa7ac4a7dfbbee92745b801b24bce10a98d2f2b1ea9432f",
-                "sha256:db2b7df831c3187a37f3bb80ec095f249fa276dbe09abd3d35297fc250385694",
-                "sha256:e586f448df2bbc37dfadccdb7ccd125c62b4348cb90c10840d695592aa1b29e0",
-                "sha256:e5983c19d0beb6af88cb4d47afb92d96751fb3fa1784d8785b1cdf14c6519407",
-                "sha256:e6a1e5ca97d411a461041d057348e578dc344ecd2add3555aedba3b408c9f874",
-                "sha256:eaf58b9e30e0e546cdc3ac06cf9165a1ca5b3de8221e9df679416ca667972035",
-                "sha256:ed693137a9187052fc46eedfafdcb74e09917166362af4cc4fddc3b31560e93d",
-                "sha256:edd1a68f79b89b0c57339bce297ad5d5ffcc6ae7e1afdb10f1947706ed066c9c",
-                "sha256:f080248b3e029d052bf74a897b9d74cfb7643537fbde97fe8225a6467fb559b5",
-                "sha256:f9392a4555f3e4cb45310a65b403d86b589adc773898c25a39184b1ba4db8985",
-                "sha256:f98dc35ab9a749276f1a4a38ab3e0e2ba1662ce710f6530f5b0a6656f1c32b58"
-            ],
-            "version": "==2021.7.6"
-        },
-        "toml": {
-            "hashes": [
-                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
-                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
-            ],
-            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.2"
-        },
-        "tomli": {
-            "hashes": [
-                "sha256:33d7984738f8bb699c9b0a816eb646a8178a69eaa792d258486776a5d21b8ca5",
-                "sha256:f4a182048010e89cbec0ae4686b21f550a7f2903f665e34a6de58ec15424f919"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.1.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.0.0"
         }
     }
 }
```

### Comparing `croudtech-python-aws-app-config-1.1.8/docs/Makefile` & `croudtech_python_aws_app_config-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/docs/conf.py` & `croudtech_python_aws_app_config-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/docs/index.rst` & `croudtech_python_aws_app_config-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/nodejs/package-lock.json` & `croudtech_python_aws_app_config-2.0.0/nodejs/package-lock.json`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/nodejs/package.json` & `croudtech_python_aws_app_config-2.0.0/nodejs/package.json`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/nodejs/src/index.ts` & `croudtech_python_aws_app_config-2.0.0/nodejs/src/index.ts`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/setup.cfg` & `croudtech_python_aws_app_config-2.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = croudtech-python-aws-app-config
 description = Applicaton config via AWS SSM
 author = Jim Robinson
-author-email = jscrobinson@gmail.com
+author_email = jscrobinson@gmail.com
 license = mit
-long-description = file: README.md
-long-description-content-type = text/markdown; charset=UTF-8
+long_description = file: README.md
+long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/CroudTech/croudtech-python-aws-app-config
 platforms = any
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
 	Intended Audience :: Developers
```

### Comparing `croudtech-python-aws-app-config-1.1.8/setup.py` & `croudtech_python_aws_app_config-2.0.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,23 +3,30 @@
     Setup file for croudtech_python_aws_app_config.
     Use setup.cfg to configure your project.
 
     This file was generated with PyScaffold 3.2.3.
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
+import importlib.machinery
+import importlib.metadata
+import importlib.resources
+import importlib.util
 import sys
 
-from pkg_resources import VersionConflict, require
 from setuptools import setup
+import importlib
+
 
 try:
-    require("setuptools>=38.3")
-except VersionConflict:
-    print("Error: version of setuptools is too old (<38.3)!")
+    spec = importlib.metadata.distribution("setuptools")
+
+except importlib.metadata.PackageNotFoundError as err:
+    print(err)
+    print("Error: version of setuptools is too old (<69.5.1)!")
     sys.exit(1)
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
```

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/metrics.py` & `croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/metrics.py`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/redis_config.py` & `croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/redis_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,20 +41,22 @@
     def redis_db_allocations(self):
         return json.loads(self.redis_config.get(self._allocated_dbs_key))
 
     @property
     def db_key(self):
         return "%s_%s" % (self._environment, self._app_name)
 
-    def get_redis_database(self):
+    def get_redis_database(self, allocate=False):
         allocated_dbs = self.redis_db_allocations
-        if self.db_key not in allocated_dbs:
+        if self.db_key not in allocated_dbs and allocate:
             allocated_db = self.allocate_db()
-        else:
+        elif self.db_key in allocated_dbs:
             allocated_db = allocated_dbs[self.db_key]
+        else:
+            allocated_db = None
         if self.put_metrics:
             self.metrics.put_redis_db_metric(
                 app_key=self.db_key,
                 redis_db=allocated_db,
                 redis_host=self._redis_host,
                 environment_name=self._environment,
             )
@@ -65,14 +67,25 @@
         db = unused_dbs[0]
         db_config = self.redis_db_allocations
         db_config[self.db_key] = db
         self._redis_config.set(self._allocated_dbs_key, json.dumps(db_config))
 
         return db
 
+    def deallocate_db(self):
+        unused_dbs = self.get_unused_dbs()        
+        db_config = self.redis_db_allocations
+        if self.db_key in db_config:
+            db = db_config[self.db_key]
+            del(db_config[self.db_key])
+            self._redis_config.set(self._allocated_dbs_key, json.dumps(db_config))
+
+            return True, db
+        return False, None
+
     def get_redis_allocated_db(self, db):
         if db not in self._redis_dbs:
             self._redis_dbs[db] = redis.Redis(
                 host=self._redis_host, port=self._redis_port, db=db
             )
         return self._redis_dbs[db]
```

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/response.py` & `croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/response.py`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/ssm_config.py` & `croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/ssm_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,45 +91,57 @@
     def get_parameters(self):
         if self.include_common:
             parameters = self.fetch_parameters(self.common_ssm_path)
         else:
             parameters = {}
 
         parameters = {**parameters, **self.fetch_parameters(self.ssm_path)}
-        try:
-            parameters = self.parse_parameters(parameters)
-        except:
-            pass
+        parameters = self.parse_parameters(parameters)
         return parameters
 
     def parse_parameters(self, parameters):
-        if self.parse_redis and ("/REDIS_DB" not in parameters or parameters["/REDIS_DB"] == "auto"):
+        if self.parse_redis:
+            redis_db, redis_host, redis_port = self.find_redis_config(parameters, allocate=True)
+            if redis_db:
+                parameters["/REDIS_DB"] = redis_db
+                parameters["/REDIS_URL"] = "redis://%s:%s/%s" % (
+                    redis_host,
+                    redis_port,
+                    redis_db,
+                )
+            else:
+                raise Exception("Couldn't allocate Redis Database")
+        return parameters
+    
+    def get_redis_db(self):
+        parameters = self.get_parameters()
+        redis_db, redis_host, redis_port = self.find_redis_config(parameters)
+        return redis_db, redis_host, redis_port
+
+    def find_redis_config(self, parameters, allocate=False):
+        if "/REDIS_DB" not in parameters or parameters["/REDIS_DB"] == "auto":
             redis_host = (
                 parameters["/REDIS_HOST"] if "/REDIS_HOST" in parameters else False
             )
             redis_port = (
                 parameters["/REDIS_PORT"] if "/REDIS_PORT" in parameters else 6379
             )
+
             if redis_host:
                 redis_config_instance = RedisConfig(
                     redis_host=redis_host,
                     redis_port=redis_port,
                     app_name=self.app_name,
                     environment=self.environment_name,
                     put_metrics=self.put_metrics,
                 )
-                redis_db = redis_config_instance.get_redis_database()
-                parameters["/REDIS_DB"] = redis_db
-                parameters["/REDIS_URL"] = "redis://%s:%s/%s" % (
-                    redis_host,
-                    redis_port,
-                    redis_db,
-                )
-        return parameters
-
+                redis_db = redis_config_instance.get_redis_database(allocate)
+                return redis_db, redis_host, redis_port
+        return None, None, None
+    
     @property
     def current_parameters(self):
         if not hasattr(self, "_current_parameters"):
             self._current_parameters = self.fetch_parameters(
                 path=self.ssm_path, absolute_path=True
             )
         return self._current_parameters
@@ -200,23 +212,39 @@
     def parse_value(self, value):
         try:
             parsed_value = json.dumps(json.loads(value))
         except:
             parsed_value = value
         return str(parsed_value).strip()
 
+    def parse_fetched_parameter(self, parameter):
+        value = parameter['Value']
+        if value.startswith('ssm:'):
+            valueParameterName = value.replace('ssm:', '')
+            encrypted = False
+            if valueParameterName.startswith('encrypted:'):
+                valueParameterName = valueParameterName.replace('encrypted:')
+                encrypted = True
+            parameterresponse = self.ssm_client.get_parameter(
+                Name = valueParameterName,
+                WithDecryption = encrypted
+            )
+            value = parameterresponse['Parameter']['Value']
+        return value
+
     def fetch_parameters(self, path, absolute_path=False):
         try:
             parameters = {}
             for parameter in self.fetch_paginated_parameters(path):
                 if absolute_path:
                     parameter_name = parameter["Name"]
                 else:
                     parameter_name = parameter["Name"].replace(path, "")
-                parameters[parameter_name] = parameter["Value"]            
+                parameter_value = self.parse_fetched_parameter(parameter)
+                parameters[parameter_name] = parameter_value  
         except botocore.exceptions.ClientError as err:
             logger.debug("Failed to fetch parameters. Invalid token")
             return {}
         except botocore.exceptions.NoCredentialsError as err:
             logger.debug("Failed to fetch parameters. Could not find AWS credentials")
             return {}
         return parameters
@@ -317,14 +345,15 @@
         elif file_extension == ".json":
             data = json.loads(contents)
         else:
             raise Exception("File format is not valid")
 
         flattened = convert_flatten(data, sep="/", parent_key=self.ssm_path)
         if delete_first:
+            self.parse_redis = False
             self.delete_existing()
 
         for key, value in flattened.items():
             self.put_parameter(
                 path=key, is_abs_path=True, value=value, encrypted=encrypted
             )
```

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config/tests/redis_config_test.py` & `croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config/tests/redis_config_test.py`

 * *Files identical despite different names*

### Comparing `croudtech-python-aws-app-config-1.1.8/src/croudtech_python_aws_app_config.egg-info/SOURCES.txt` & `croudtech_python_aws_app_config-2.0.0/src/croudtech_python_aws_app_config.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .gitignore
 AUTHORS.rst
 CHANGELOG.rst
 LICENSE.txt
 Pipfile
 Pipfile.lock
 README.md
+azure-pipelines.yml
 pytest.ini
 requirements.txt
 setup.cfg
 setup.py
 .vscode/settings.json
 docs/Makefile
 docs/authors.rst
```

