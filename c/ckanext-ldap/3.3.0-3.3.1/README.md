# Comparing `tmp/ckanext-ldap-3.3.0.tar.gz` & `tmp/ckanext_ldap-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-ldap-3.3.0.tar", last modified: Mon Jan 22 09:45:36 2024, max compression
+gzip compressed data, was "ckanext_ldap-3.3.1.tar", last modified: Tue May 14 10:45:15 2024, max compression
```

## Comparing `ckanext-ldap-3.3.0.tar` & `ckanext_ldap-3.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.840602 ckanext-ldap-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25348 2024-01-22 09:45:36.840602 ckanext-ldap-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24218 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.832603 ckanext-ldap-3.3.0/ckanext/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.832603 ckanext-ldap-3.3.0/ckanext/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.832603 ckanext-ldap-3.3.0/ckanext/ldap/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/lib/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.832603 ckanext-ldap-3.3.0/ckanext/ldap/logic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/logic/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.836603 ckanext-ldap-3.3.0/ckanext/ldap/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/model/ldap_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.836603 ckanext-ldap-3.3.0/ckanext/ldap/routes/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/routes/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/routes/login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.832603 ckanext-ldap-3.3.0/ckanext/ldap/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.832603 ckanext-ldap-3.3.0/ckanext/ldap/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.836603 ckanext-ldap-3.3.0/ckanext/ldap/theme/templates/user/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/ckanext/ldap/theme/templates/user/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.836603 ckanext-ldap-3.3.0/ckanext_ldap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25348 2024-01-22 09:45:36.000000 ckanext-ldap-3.3.0/ckanext_ldap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-22 09:45:36.000000 ckanext-ldap-3.3.0/ckanext_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 09:45:36.000000 ckanext-ldap-3.3.0/ckanext_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-22 09:45:36.000000 ckanext-ldap-3.3.0/ckanext_ldap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 09:45:36.000000 ckanext-ldap-3.3.0/ckanext_ldap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-22 09:45:36.000000 ckanext-ldap-3.3.0/ckanext_ldap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-22 09:45:36.000000 ckanext-ldap-3.3.0/ckanext_ldap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.832603 ckanext-ldap-3.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.836603 ckanext-ldap-3.3.0/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 09:45:36.840602 ckanext-ldap-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.836603 ckanext-ldap-3.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:36.836603 ckanext-ldap-3.3.0/tests/routes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/tests/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/tests/routes/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-01-22 09:45:28.000000 ckanext-ldap-3.3.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.784153 ckanext_ldap-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25570 2024-05-14 10:45:15.784153 ckanext_ldap-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24440 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.776153 ckanext_ldap-3.3.1/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.780153 ckanext_ldap-3.3.1/ckanext/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.780153 ckanext_ldap-3.3.1/ckanext/ldap/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/lib/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.780153 ckanext_ldap-3.3.1/ckanext/ldap/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/logic/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.780153 ckanext_ldap-3.3.1/ckanext/ldap/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/model/ldap_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.780153 ckanext_ldap-3.3.1/ckanext/ldap/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/routes/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/routes/login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.776153 ckanext_ldap-3.3.1/ckanext/ldap/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.776153 ckanext_ldap-3.3.1/ckanext/ldap/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.780153 ckanext_ldap-3.3.1/ckanext/ldap/theme/templates/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/ckanext/ldap/theme/templates/user/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.784153 ckanext_ldap-3.3.1/ckanext_ldap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25570 2024-05-14 10:45:15.000000 ckanext_ldap-3.3.1/ckanext_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-14 10:45:15.000000 ckanext_ldap-3.3.1/ckanext_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:45:15.000000 ckanext_ldap-3.3.1/ckanext_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 10:45:15.000000 ckanext_ldap-3.3.1/ckanext_ldap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:45:15.000000 ckanext_ldap-3.3.1/ckanext_ldap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 10:45:15.000000 ckanext_ldap-3.3.1/ckanext_ldap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 10:45:15.000000 ckanext_ldap-3.3.1/ckanext_ldap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.776153 ckanext_ldap-3.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.780153 ckanext_ldap-3.3.1/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:45:15.784153 ckanext_ldap-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.784153 ckanext_ldap-3.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:15.784153 ckanext_ldap-3.3.1/tests/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/tests/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/tests/routes/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-14 10:45:11.000000 ckanext_ldap-3.3.1/tests/test_helpers.py
```

### Comparing `ckanext-ldap-3.3.0/LICENSE` & `ckanext_ldap-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/PKG-INFO` & `ckanext_ldap-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-ldap
-Version: 3.3.0
+Version: 3.3.1
 Summary: A CKAN extension that provides LDAP authentication.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-ldap
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-ldap/blob/main/CHANGELOG.md
 Keywords: CKAN,data,ldap
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,26 +42,29 @@
 
 # Overview
 
 <!--overview-start-->
 This plugin provides LDAP authentication for CKAN.
 
 Features include:
+
 - Imports username, full name, email and description;
 - Can match against several LDAP fields (eg. username or full name);
-- Allows to have LDAP only authentication, or combine LDAP and basic CKAN authentication;
+- Allows to have LDAP only authentication, or combine LDAP and basic CKAN
+  authentication;
 - Can add LDAP users to a given organization automatically;
 - Works with Active Directory.
 
 <!--overview-end-->
 
 # Installation
 
 <!--installation-start-->
 Path variables used below:
+
 - `$INSTALL_FOLDER` (i.e. where CKAN is installed), e.g. `/usr/lib/ckan/default`
 - `$CONFIG_FILE`, e.g. `/etc/ckan/default/development.ini`
 
 ## Installing from PyPI
 
 ```shell
 pip install ckanext-ldap
@@ -83,15 +86,18 @@
 3. Install via pip:
    ```shell
    pip install $INSTALL_FOLDER/src/ckanext-ldap
    ```
 
 ### Installing in editable mode
 
-Installing from a `pyproject.toml` in editable mode (i.e. `pip install -e`) requires `setuptools>=64`; however, CKAN 2.9 requires `setuptools==44.1.0`. See [our CKAN fork](https://github.com/NaturalHistoryMuseum/ckan) for a version of v2.9 that uses an updated setuptools if this functionality is something you need.
+Installing from a `pyproject.toml` in editable mode (i.e. `pip install -e`)
+requires `setuptools>=64`; however, CKAN 2.9 requires `setuptools==44.1.0`.
+See [our CKAN fork](https://github.com/NaturalHistoryMuseum/ckan) for a version of v2.9
+that uses an updated setuptools if this functionality is something you need.
 
 ## Post-install setup
 
 1. Add 'ldap' to the list of plugins in your `$CONFIG_FILE`:
    ```ini
    ckan.plugins = ... ldap
    ```
@@ -129,35 +135,40 @@
 | `ckanext.ldap.organization.role`    | The role given to users added in the given organization ('admin', 'editor' or 'member'). **Warning**: Changing this parameter will only affect users that have not yet logged on. It will not modify the role of users who have already logged on. This is only used if `ckanext.ldap.organization.id` is set. There is currently no functionality for mapping LDAP groups to CKAN roles, so this just assigns the same role to _every_ new LDAP user.                                                                                                                                                                                                                                                                                                                                                                                                                  | member, editor, admin           | 'member' |
 | `ckanext.ldap.search.alt`           | An alternative search string for the LDAP filter. If this is present and the search using `ckanext.ldap.search.filter` returns exactly 0 results, then a search using this filter will be performed. If this search returns exactly one result, then it will be accepted. You can use this for example in Active Directory to match against both username and fullname by setting `ckanext.ldap.search.filter` to  'sAMAccountName={login}' and `ckanext.ldap.search.alt` to 'name={login}'. The approach of using two separate filter strings (rather than one with an or statement) ensures that priority will always be given to the unique id match. `ckanext.ldap.search.alt` however can  be used to match against more than one field. For example you could match against either the full name or the email address by setting `ckanext.ldap.search.alt` to '(\ | (name={login})(mail={login}))'. |          |
 | `ckanext.ldap.search.alt_msg`       | A message that is output to the user when the search on `ckanext.ldap.search.filter` returns 0 results, and the search on `ckanext.ldap.search.alt` returns more than one result. Example: 'Please use your short account name instead'.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                                 |          |
 | `ckanext.ldap.migrate`              | If true this will change an existing CKAN user with the same username to an LDAP user. Otherwise, an exception `UserConflictError`is raised if LDAP-login with an already existing local CKAN username is attempted. This option provides a migration path from local CKAN authentication to LDAP authentication: Rename all users to their LDAP usernames and instruct them to login with their LDAP credentials. Migration then happens transparently.                                                                                                                                                                                                                                                                                                                                                                                                                | True/False                      | False    |
 | `ckanext.ldap.debug_level`          | [python-ldap debug level](https://www.python-ldap.org/en/python-ldap-3.0.0b1/reference/ldap.html?highlight=debug_level#ldap.OPT_DEBUG_LEVEL). **Security warning**: it is strongly recommended to keep this parameter set to 0 (zero) on production systems, otherwise [plaintext passwords will be logged by `python-ldap`](https://github.com/python-ldap/python-ldap/issues/384)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | 0-9                             | 0        |
 | `ckanext.ldap.trace_level`          | [python-ldap trace level](https://www.python-ldap.org/en/python-ldap-3.0.0b1/reference/ldap.html?highlight=trace_level#ldap.initialize). **Security warning**: it is strongly recommended to keep this parameter set to 0 (zero) on production systems, otherwise [plaintext passwords will be logged by `python-ldap`](https://github.com/python-ldap/python-ldap/issues/384)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | 0-9                             | 0        |
 | `ckanext.ldap.allow_password_reset` | If true, allows LDAP users to reset their passwords, if false, disallows this functionality. Note that if this is true, the password that is reset is the CKAN user password, not the LDAP one. If set to false, the request to reset will be denied only if the user is an LDAP user, if not they will be allowed to reset regardless of the value of this option.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | True/False                      | true     |
-| `ckanext.ldap.ignore_referrals`     | If true, The plugin will ignore referral query results sent by the LDAP server. This might be necessary if your base_dn is at the domain level, but the LDAP server searches in multiple paths for the user, resulting in queries containing more than one result.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | True/False                      | false     |
+| `ckanext.ldap.ignore_referrals`     | If true, The plugin will ignore referral query results sent by the LDAP server. This might be necessary if your base_dn is at the domain level, but the LDAP server searches in multiple paths for the user, resulting in queries containing more than one result.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | True/False                      | false    |
+
 <!--configuration-end-->
 
 # Usage
 
 <!--usage-start-->
+
 ## Example Test Configuration
-To test that the extension is working correctly without having to set up an LDAP service yourself, you can try this config snippet:
+
+To test that the extension is working correctly without having to set up an LDAP service
+yourself, you can try this config snippet:
 
 ```ini
 ckanext.ldap.uri = ldap://ldap.forumsys.com:389
 ckanext.ldap.base_dn = dc=example,dc=com
 ckanext.ldap.search.filter = cn=*{login}*
 ckanext.ldap.username = cn
 ckanext.ldap.auth.dn = cn=read-only-admin,dc=example,dc=com
 ckanext.ldap.email = mail
 ckanext.ldap.auth.password = password
 ckanext.ldap.auth.method = SIMPLE
 ```
 
-See [here](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/) for more information.
+See [here](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/)
+for more information.
 Then just login with `tesla` or `gauss` for example with `password` as the password.
 
 ## Commands
 
 ### `ldap`
 
 1. `setup-org`: create the organisation specified in `ckanext.ldap.organization.id`.
@@ -168,15 +179,16 @@
 2. `initdb`: ensure the tables needed by this extension exist.
     ```bash
     ckan -c $CONFIG_FILE ldap initdb
     ```
 
 ## Templates
 
-This extension overrides `templates/user/login.html` and sets the form action to the LDAP login handler.
+This extension overrides `templates/user/login.html` and sets the form action to the
+LDAP login handler.
 
 To use it elsewhere:
 
 ```html+jinja
 {% set ldap_action = h.get_login_action() %}
 {% snippet "user/snippets/login_form.html", action=ldap_action, error_summary=error_summary %}
 ```
@@ -184,25 +196,30 @@
 The helper function `h.is_ldap_user()` is also provided for templates.
 
 <!--usage-end-->
 
 # Testing
 
 <!--testing-start-->
-There is a Docker compose configuration available in this repository to make it easier to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
+There is a Docker compose configuration available in this repository to make it easier
+to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
 
-To run the tests against ckan 2.9.x on Python3:
+To run the tests can be run against ckan 2.9.x and 2.10.x on Python3:
 
 1. Build the required images:
    ```shell
    docker-compose build
    ```
 
 2. Then run the tests.
-   The root of the repository is mounted into the ckan container as a volume by the Docker compose
-   configuration, so you should only need to rebuild the ckan image if you change the extension's
-   dependencies.
+   The root of the repository is mounted into the ckan container as a volume by the
+   Docker compose configuration, so you should only need to rebuild the ckan image if
+   you change the extension's dependencies.
    ```shell
+   # run tests against ckan 2.9.x
    docker-compose run latest
+
+   # run tests against ckan 2.10.x
+   docker-compose run next
    ```
 
 <!--testing-end-->
```

### Comparing `ckanext-ldap-3.3.0/README.md` & `ckanext_ldap-3.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,29 @@
 
 # Overview
 
 <!--overview-start-->
 This plugin provides LDAP authentication for CKAN.
 
 Features include:
+
 - Imports username, full name, email and description;
 - Can match against several LDAP fields (eg. username or full name);
-- Allows to have LDAP only authentication, or combine LDAP and basic CKAN authentication;
+- Allows to have LDAP only authentication, or combine LDAP and basic CKAN
+  authentication;
 - Can add LDAP users to a given organization automatically;
 - Works with Active Directory.
 
 <!--overview-end-->
 
 # Installation
 
 <!--installation-start-->
 Path variables used below:
+
 - `$INSTALL_FOLDER` (i.e. where CKAN is installed), e.g. `/usr/lib/ckan/default`
 - `$CONFIG_FILE`, e.g. `/etc/ckan/default/development.ini`
 
 ## Installing from PyPI
 
 ```shell
 pip install ckanext-ldap
@@ -56,15 +59,18 @@
 3. Install via pip:
    ```shell
    pip install $INSTALL_FOLDER/src/ckanext-ldap
    ```
 
 ### Installing in editable mode
 
-Installing from a `pyproject.toml` in editable mode (i.e. `pip install -e`) requires `setuptools>=64`; however, CKAN 2.9 requires `setuptools==44.1.0`. See [our CKAN fork](https://github.com/NaturalHistoryMuseum/ckan) for a version of v2.9 that uses an updated setuptools if this functionality is something you need.
+Installing from a `pyproject.toml` in editable mode (i.e. `pip install -e`)
+requires `setuptools>=64`; however, CKAN 2.9 requires `setuptools==44.1.0`.
+See [our CKAN fork](https://github.com/NaturalHistoryMuseum/ckan) for a version of v2.9
+that uses an updated setuptools if this functionality is something you need.
 
 ## Post-install setup
 
 1. Add 'ldap' to the list of plugins in your `$CONFIG_FILE`:
    ```ini
    ckan.plugins = ... ldap
    ```
@@ -102,35 +108,40 @@
 | `ckanext.ldap.organization.role`    | The role given to users added in the given organization ('admin', 'editor' or 'member'). **Warning**: Changing this parameter will only affect users that have not yet logged on. It will not modify the role of users who have already logged on. This is only used if `ckanext.ldap.organization.id` is set. There is currently no functionality for mapping LDAP groups to CKAN roles, so this just assigns the same role to _every_ new LDAP user.                                                                                                                                                                                                                                                                                                                                                                                                                  | member, editor, admin           | 'member' |
 | `ckanext.ldap.search.alt`           | An alternative search string for the LDAP filter. If this is present and the search using `ckanext.ldap.search.filter` returns exactly 0 results, then a search using this filter will be performed. If this search returns exactly one result, then it will be accepted. You can use this for example in Active Directory to match against both username and fullname by setting `ckanext.ldap.search.filter` to  'sAMAccountName={login}' and `ckanext.ldap.search.alt` to 'name={login}'. The approach of using two separate filter strings (rather than one with an or statement) ensures that priority will always be given to the unique id match. `ckanext.ldap.search.alt` however can  be used to match against more than one field. For example you could match against either the full name or the email address by setting `ckanext.ldap.search.alt` to '(\ | (name={login})(mail={login}))'. |          |
 | `ckanext.ldap.search.alt_msg`       | A message that is output to the user when the search on `ckanext.ldap.search.filter` returns 0 results, and the search on `ckanext.ldap.search.alt` returns more than one result. Example: 'Please use your short account name instead'.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                                 |          |
 | `ckanext.ldap.migrate`              | If true this will change an existing CKAN user with the same username to an LDAP user. Otherwise, an exception `UserConflictError`is raised if LDAP-login with an already existing local CKAN username is attempted. This option provides a migration path from local CKAN authentication to LDAP authentication: Rename all users to their LDAP usernames and instruct them to login with their LDAP credentials. Migration then happens transparently.                                                                                                                                                                                                                                                                                                                                                                                                                | True/False                      | False    |
 | `ckanext.ldap.debug_level`          | [python-ldap debug level](https://www.python-ldap.org/en/python-ldap-3.0.0b1/reference/ldap.html?highlight=debug_level#ldap.OPT_DEBUG_LEVEL). **Security warning**: it is strongly recommended to keep this parameter set to 0 (zero) on production systems, otherwise [plaintext passwords will be logged by `python-ldap`](https://github.com/python-ldap/python-ldap/issues/384)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | 0-9                             | 0        |
 | `ckanext.ldap.trace_level`          | [python-ldap trace level](https://www.python-ldap.org/en/python-ldap-3.0.0b1/reference/ldap.html?highlight=trace_level#ldap.initialize). **Security warning**: it is strongly recommended to keep this parameter set to 0 (zero) on production systems, otherwise [plaintext passwords will be logged by `python-ldap`](https://github.com/python-ldap/python-ldap/issues/384)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | 0-9                             | 0        |
 | `ckanext.ldap.allow_password_reset` | If true, allows LDAP users to reset their passwords, if false, disallows this functionality. Note that if this is true, the password that is reset is the CKAN user password, not the LDAP one. If set to false, the request to reset will be denied only if the user is an LDAP user, if not they will be allowed to reset regardless of the value of this option.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | True/False                      | true     |
-| `ckanext.ldap.ignore_referrals`     | If true, The plugin will ignore referral query results sent by the LDAP server. This might be necessary if your base_dn is at the domain level, but the LDAP server searches in multiple paths for the user, resulting in queries containing more than one result.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | True/False                      | false     |
+| `ckanext.ldap.ignore_referrals`     | If true, The plugin will ignore referral query results sent by the LDAP server. This might be necessary if your base_dn is at the domain level, but the LDAP server searches in multiple paths for the user, resulting in queries containing more than one result.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | True/False                      | false    |
+
 <!--configuration-end-->
 
 # Usage
 
 <!--usage-start-->
+
 ## Example Test Configuration
-To test that the extension is working correctly without having to set up an LDAP service yourself, you can try this config snippet:
+
+To test that the extension is working correctly without having to set up an LDAP service
+yourself, you can try this config snippet:
 
 ```ini
 ckanext.ldap.uri = ldap://ldap.forumsys.com:389
 ckanext.ldap.base_dn = dc=example,dc=com
 ckanext.ldap.search.filter = cn=*{login}*
 ckanext.ldap.username = cn
 ckanext.ldap.auth.dn = cn=read-only-admin,dc=example,dc=com
 ckanext.ldap.email = mail
 ckanext.ldap.auth.password = password
 ckanext.ldap.auth.method = SIMPLE
 ```
 
-See [here](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/) for more information.
+See [here](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/)
+for more information.
 Then just login with `tesla` or `gauss` for example with `password` as the password.
 
 ## Commands
 
 ### `ldap`
 
 1. `setup-org`: create the organisation specified in `ckanext.ldap.organization.id`.
@@ -141,15 +152,16 @@
 2. `initdb`: ensure the tables needed by this extension exist.
     ```bash
     ckan -c $CONFIG_FILE ldap initdb
     ```
 
 ## Templates
 
-This extension overrides `templates/user/login.html` and sets the form action to the LDAP login handler.
+This extension overrides `templates/user/login.html` and sets the form action to the
+LDAP login handler.
 
 To use it elsewhere:
 
 ```html+jinja
 {% set ldap_action = h.get_login_action() %}
 {% snippet "user/snippets/login_form.html", action=ldap_action, error_summary=error_summary %}
 ```
@@ -157,25 +169,30 @@
 The helper function `h.is_ldap_user()` is also provided for templates.
 
 <!--usage-end-->
 
 # Testing
 
 <!--testing-start-->
-There is a Docker compose configuration available in this repository to make it easier to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
+There is a Docker compose configuration available in this repository to make it easier
+to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
 
-To run the tests against ckan 2.9.x on Python3:
+To run the tests can be run against ckan 2.9.x and 2.10.x on Python3:
 
 1. Build the required images:
    ```shell
    docker-compose build
    ```
 
 2. Then run the tests.
-   The root of the repository is mounted into the ckan container as a volume by the Docker compose
-   configuration, so you should only need to rebuild the ckan image if you change the extension's
-   dependencies.
+   The root of the repository is mounted into the ckan container as a volume by the
+   Docker compose configuration, so you should only need to rebuild the ckan image if
+   you change the extension's dependencies.
    ```shell
+   # run tests against ckan 2.9.x
    docker-compose run latest
+
+   # run tests against ckan 2.10.x
+   docker-compose run next
    ```
 
 <!--testing-end-->
```

### Comparing `ckanext-ldap-3.3.0/ckanext/ldap/cli.py` & `ckanext_ldap-3.3.1/ckanext/ldap/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/ckanext/ldap/lib/helpers.py` & `ckanext_ldap-3.3.1/ckanext/ldap/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/ckanext/ldap/lib/search.py` & `ckanext_ldap-3.3.1/ckanext/ldap/lib/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/ckanext/ldap/logic/auth.py` & `ckanext_ldap-3.3.1/ckanext/ldap/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/ckanext/ldap/model/ldap_user.py` & `ckanext_ldap-3.3.1/ckanext/ldap/model/ldap_user.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/ckanext/ldap/plugin.py` & `ckanext_ldap-3.3.1/ckanext/ldap/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
     LdapPlugin.
 
     This plugin provides Ldap authentication by implementing the IAuthenticator
     interface.
     """
 
-    implements(interfaces.IAuthenticator)
+    implements(interfaces.IAuthenticator, inherit=True)
     implements(interfaces.IConfigurable)
     implements(interfaces.IConfigurer)
     implements(interfaces.IBlueprint, inherit=True)
     implements(interfaces.IAuthFunctions)
     implements(interfaces.ITemplateHelpers, inherit=True)
     implements(interfaces.IClick)
```

### Comparing `ckanext-ldap-3.3.0/ckanext/ldap/routes/_helpers.py` & `ckanext_ldap-3.3.1/ckanext/ldap/routes/_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/ckanext/ldap/routes/login.py` & `ckanext_ldap-3.3.1/ckanext/ldap/routes/login.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/ckanext_ldap.egg-info/PKG-INFO` & `ckanext_ldap-3.3.1/ckanext_ldap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-ldap
-Version: 3.3.0
+Version: 3.3.1
 Summary: A CKAN extension that provides LDAP authentication.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-ldap
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-ldap/blob/main/CHANGELOG.md
 Keywords: CKAN,data,ldap
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,26 +42,29 @@
 
 # Overview
 
 <!--overview-start-->
 This plugin provides LDAP authentication for CKAN.
 
 Features include:
+
 - Imports username, full name, email and description;
 - Can match against several LDAP fields (eg. username or full name);
-- Allows to have LDAP only authentication, or combine LDAP and basic CKAN authentication;
+- Allows to have LDAP only authentication, or combine LDAP and basic CKAN
+  authentication;
 - Can add LDAP users to a given organization automatically;
 - Works with Active Directory.
 
 <!--overview-end-->
 
 # Installation
 
 <!--installation-start-->
 Path variables used below:
+
 - `$INSTALL_FOLDER` (i.e. where CKAN is installed), e.g. `/usr/lib/ckan/default`
 - `$CONFIG_FILE`, e.g. `/etc/ckan/default/development.ini`
 
 ## Installing from PyPI
 
 ```shell
 pip install ckanext-ldap
@@ -83,15 +86,18 @@
 3. Install via pip:
    ```shell
    pip install $INSTALL_FOLDER/src/ckanext-ldap
    ```
 
 ### Installing in editable mode
 
-Installing from a `pyproject.toml` in editable mode (i.e. `pip install -e`) requires `setuptools>=64`; however, CKAN 2.9 requires `setuptools==44.1.0`. See [our CKAN fork](https://github.com/NaturalHistoryMuseum/ckan) for a version of v2.9 that uses an updated setuptools if this functionality is something you need.
+Installing from a `pyproject.toml` in editable mode (i.e. `pip install -e`)
+requires `setuptools>=64`; however, CKAN 2.9 requires `setuptools==44.1.0`.
+See [our CKAN fork](https://github.com/NaturalHistoryMuseum/ckan) for a version of v2.9
+that uses an updated setuptools if this functionality is something you need.
 
 ## Post-install setup
 
 1. Add 'ldap' to the list of plugins in your `$CONFIG_FILE`:
    ```ini
    ckan.plugins = ... ldap
    ```
@@ -129,35 +135,40 @@
 | `ckanext.ldap.organization.role`    | The role given to users added in the given organization ('admin', 'editor' or 'member'). **Warning**: Changing this parameter will only affect users that have not yet logged on. It will not modify the role of users who have already logged on. This is only used if `ckanext.ldap.organization.id` is set. There is currently no functionality for mapping LDAP groups to CKAN roles, so this just assigns the same role to _every_ new LDAP user.                                                                                                                                                                                                                                                                                                                                                                                                                  | member, editor, admin           | 'member' |
 | `ckanext.ldap.search.alt`           | An alternative search string for the LDAP filter. If this is present and the search using `ckanext.ldap.search.filter` returns exactly 0 results, then a search using this filter will be performed. If this search returns exactly one result, then it will be accepted. You can use this for example in Active Directory to match against both username and fullname by setting `ckanext.ldap.search.filter` to  'sAMAccountName={login}' and `ckanext.ldap.search.alt` to 'name={login}'. The approach of using two separate filter strings (rather than one with an or statement) ensures that priority will always be given to the unique id match. `ckanext.ldap.search.alt` however can  be used to match against more than one field. For example you could match against either the full name or the email address by setting `ckanext.ldap.search.alt` to '(\ | (name={login})(mail={login}))'. |          |
 | `ckanext.ldap.search.alt_msg`       | A message that is output to the user when the search on `ckanext.ldap.search.filter` returns 0 results, and the search on `ckanext.ldap.search.alt` returns more than one result. Example: 'Please use your short account name instead'.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                                 |          |
 | `ckanext.ldap.migrate`              | If true this will change an existing CKAN user with the same username to an LDAP user. Otherwise, an exception `UserConflictError`is raised if LDAP-login with an already existing local CKAN username is attempted. This option provides a migration path from local CKAN authentication to LDAP authentication: Rename all users to their LDAP usernames and instruct them to login with their LDAP credentials. Migration then happens transparently.                                                                                                                                                                                                                                                                                                                                                                                                                | True/False                      | False    |
 | `ckanext.ldap.debug_level`          | [python-ldap debug level](https://www.python-ldap.org/en/python-ldap-3.0.0b1/reference/ldap.html?highlight=debug_level#ldap.OPT_DEBUG_LEVEL). **Security warning**: it is strongly recommended to keep this parameter set to 0 (zero) on production systems, otherwise [plaintext passwords will be logged by `python-ldap`](https://github.com/python-ldap/python-ldap/issues/384)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | 0-9                             | 0        |
 | `ckanext.ldap.trace_level`          | [python-ldap trace level](https://www.python-ldap.org/en/python-ldap-3.0.0b1/reference/ldap.html?highlight=trace_level#ldap.initialize). **Security warning**: it is strongly recommended to keep this parameter set to 0 (zero) on production systems, otherwise [plaintext passwords will be logged by `python-ldap`](https://github.com/python-ldap/python-ldap/issues/384)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | 0-9                             | 0        |
 | `ckanext.ldap.allow_password_reset` | If true, allows LDAP users to reset their passwords, if false, disallows this functionality. Note that if this is true, the password that is reset is the CKAN user password, not the LDAP one. If set to false, the request to reset will be denied only if the user is an LDAP user, if not they will be allowed to reset regardless of the value of this option.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | True/False                      | true     |
-| `ckanext.ldap.ignore_referrals`     | If true, The plugin will ignore referral query results sent by the LDAP server. This might be necessary if your base_dn is at the domain level, but the LDAP server searches in multiple paths for the user, resulting in queries containing more than one result.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | True/False                      | false     |
+| `ckanext.ldap.ignore_referrals`     | If true, The plugin will ignore referral query results sent by the LDAP server. This might be necessary if your base_dn is at the domain level, but the LDAP server searches in multiple paths for the user, resulting in queries containing more than one result.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | True/False                      | false    |
+
 <!--configuration-end-->
 
 # Usage
 
 <!--usage-start-->
+
 ## Example Test Configuration
-To test that the extension is working correctly without having to set up an LDAP service yourself, you can try this config snippet:
+
+To test that the extension is working correctly without having to set up an LDAP service
+yourself, you can try this config snippet:
 
 ```ini
 ckanext.ldap.uri = ldap://ldap.forumsys.com:389
 ckanext.ldap.base_dn = dc=example,dc=com
 ckanext.ldap.search.filter = cn=*{login}*
 ckanext.ldap.username = cn
 ckanext.ldap.auth.dn = cn=read-only-admin,dc=example,dc=com
 ckanext.ldap.email = mail
 ckanext.ldap.auth.password = password
 ckanext.ldap.auth.method = SIMPLE
 ```
 
-See [here](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/) for more information.
+See [here](https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/)
+for more information.
 Then just login with `tesla` or `gauss` for example with `password` as the password.
 
 ## Commands
 
 ### `ldap`
 
 1. `setup-org`: create the organisation specified in `ckanext.ldap.organization.id`.
@@ -168,15 +179,16 @@
 2. `initdb`: ensure the tables needed by this extension exist.
     ```bash
     ckan -c $CONFIG_FILE ldap initdb
     ```
 
 ## Templates
 
-This extension overrides `templates/user/login.html` and sets the form action to the LDAP login handler.
+This extension overrides `templates/user/login.html` and sets the form action to the
+LDAP login handler.
 
 To use it elsewhere:
 
 ```html+jinja
 {% set ldap_action = h.get_login_action() %}
 {% snippet "user/snippets/login_form.html", action=ldap_action, error_summary=error_summary %}
 ```
@@ -184,25 +196,30 @@
 The helper function `h.is_ldap_user()` is also provided for templates.
 
 <!--usage-end-->
 
 # Testing
 
 <!--testing-start-->
-There is a Docker compose configuration available in this repository to make it easier to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
+There is a Docker compose configuration available in this repository to make it easier
+to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
 
-To run the tests against ckan 2.9.x on Python3:
+To run the tests can be run against ckan 2.9.x and 2.10.x on Python3:
 
 1. Build the required images:
    ```shell
    docker-compose build
    ```
 
 2. Then run the tests.
-   The root of the repository is mounted into the ckan container as a volume by the Docker compose
-   configuration, so you should only need to rebuild the ckan image if you change the extension's
-   dependencies.
+   The root of the repository is mounted into the ckan container as a volume by the
+   Docker compose configuration, so you should only need to rebuild the ckan image if
+   you change the extension's dependencies.
    ```shell
+   # run tests against ckan 2.9.x
    docker-compose run latest
+
+   # run tests against ckan 2.10.x
+   docker-compose run next
    ```
 
 <!--testing-end-->
```

### Comparing `ckanext-ldap-3.3.0/ckanext_ldap.egg-info/SOURCES.txt` & `ckanext_ldap-3.3.1/ckanext_ldap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/docs/_scripts/gen_api_pages.py` & `ckanext_ldap-3.3.1/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/pyproject.toml` & `ckanext_ldap-3.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-ldap"
-version = "3.3.0"
+version = "3.3.1"
 description = "A CKAN extension that provides LDAP authentication."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -52,15 +52,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.ldap.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "3.3.0"
+version = "3.3.1"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version",
     "CITATION.cff:^version"
 ]
```

### Comparing `ckanext-ldap-3.3.0/tests/routes/test_helpers.py` & `ckanext_ldap-3.3.1/tests/routes/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/tests/test_auth.py` & `ckanext_ldap-3.3.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-ldap-3.3.0/tests/test_helpers.py` & `ckanext_ldap-3.3.1/tests/test_helpers.py`

 * *Files identical despite different names*

